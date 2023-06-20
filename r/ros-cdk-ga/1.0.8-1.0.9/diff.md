# Comparing `tmp/ros-cdk-ga-1.0.8.tar.gz` & `tmp/ros-cdk-ga-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-ga-1.0.8.tar", last modified: Thu Jul 14 02:35:18 2022, max compression
+gzip compressed data, was "dist/ros-cdk-ga-1.0.9.tar", last modified: Fri Sep 23 10:46:45 2022, max compression
```

## Comparing `ros-cdk-ga-1.0.8.tar` & `ros-cdk-ga-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:35:18.000000 ros-cdk-ga-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:35:18.000000 ros-cdk-ga-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:35:18.000000 ros-cdk-ga-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:35:18.000000 ros-cdk-ga-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1236 2022-07-14 02:35:18.000000 ros-cdk-ga-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      176 2022-07-14 02:35:18.000000 ros-cdk-ga-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:35:18.000000 ros-cdk-ga-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:35:18.000000 ros-cdk-ga-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1788 2022-07-14 02:35:18.000000 ros-cdk-ga-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:35:18.000000 ros-cdk-ga-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:35:18.000000 ros-cdk-ga-1.0.8/src/ros_cdk_ga/
--rw-r--r--   0 root         (0) root         (0)   171200 2022-07-14 02:35:18.000000 ros-cdk-ga-1.0.8/src/ros_cdk_ga/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:35:18.000000 ros-cdk-ga-1.0.8/src/ros_cdk_ga/_jsii/
--rw-r--r--   0 root         (0) root         (0)      368 2022-07-14 02:35:18.000000 ros-cdk-ga-1.0.8/src/ros_cdk_ga/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    72864 2022-07-14 02:35:18.000000 ros-cdk-ga-1.0.8/src/ros_cdk_ga/_jsii/ros-cdk-ga@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:35:18.000000 ros-cdk-ga-1.0.8/src/ros_cdk_ga/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:35:18.000000 ros-cdk-ga-1.0.8/src/ros_cdk_ga.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1236 2022-07-14 02:35:18.000000 ros-cdk-ga-1.0.8/src/ros_cdk_ga.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      390 2022-07-14 02:35:18.000000 ros-cdk-ga-1.0.8/src/ros_cdk_ga.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:35:18.000000 ros-cdk-ga-1.0.8/src/ros_cdk_ga.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:35:18.000000 ros-cdk-ga-1.0.8/src/ros_cdk_ga.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2022-07-14 02:35:18.000000 ros-cdk-ga-1.0.8/src/ros_cdk_ga.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:46:45.000000 ros-cdk-ga-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 10:46:45.000000 ros-cdk-ga-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 10:46:45.000000 ros-cdk-ga-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 10:46:45.000000 ros-cdk-ga-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1236 2022-09-23 10:46:45.000000 ros-cdk-ga-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      176 2022-09-23 10:46:45.000000 ros-cdk-ga-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 10:46:45.000000 ros-cdk-ga-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 10:46:45.000000 ros-cdk-ga-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1817 2022-09-23 10:46:45.000000 ros-cdk-ga-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:46:45.000000 ros-cdk-ga-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:46:45.000000 ros-cdk-ga-1.0.9/src/ros_cdk_ga/
+-rw-r--r--   0 root         (0) root         (0)   204974 2022-09-23 10:46:45.000000 ros-cdk-ga-1.0.9/src/ros_cdk_ga/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:46:45.000000 ros-cdk-ga-1.0.9/src/ros_cdk_ga/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      402 2022-09-23 10:46:45.000000 ros-cdk-ga-1.0.9/src/ros_cdk_ga/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    72931 2022-09-23 10:46:45.000000 ros-cdk-ga-1.0.9/src/ros_cdk_ga/_jsii/ros-cdk-ga@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 10:46:45.000000 ros-cdk-ga-1.0.9/src/ros_cdk_ga/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:46:45.000000 ros-cdk-ga-1.0.9/src/ros_cdk_ga.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1236 2022-09-23 10:46:45.000000 ros-cdk-ga-1.0.9/src/ros_cdk_ga.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      390 2022-09-23 10:46:45.000000 ros-cdk-ga-1.0.9/src/ros_cdk_ga.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 10:46:45.000000 ros-cdk-ga-1.0.9/src/ros_cdk_ga.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 10:46:45.000000 ros-cdk-ga-1.0.9/src/ros_cdk_ga.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2022-09-23 10:46:45.000000 ros-cdk-ga-1.0.9/src/ros_cdk_ga.egg-info/top_level.txt
```

### Comparing `ros-cdk-ga-1.0.8/LICENSE` & `ros-cdk-ga-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-ga-1.0.8/PKG-INFO` & `ros-cdk-ga-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-ga
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS GA Construct Library
```

### Comparing `ros-cdk-ga-1.0.8/setup.py` & `ros-cdk-ga-1.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-ga",
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
         "ros_cdk_ga",
         "ros_cdk_ga._jsii"
     ],
     "package_data": {
         "ros_cdk_ga._jsii": [
-            "ros-cdk-ga@1.0.8.jsii.tgz"
+            "ros-cdk-ga@1.0.9.jsii.tgz"
         ],
         "ros_cdk_ga": [
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

### Comparing `ros-cdk-ga-1.0.8/src/ros_cdk_ga/__init__.py` & `ros-cdk-ga-1.0.9/src/ros_cdk_ga/__init__.py`

 * *Files 22% similar despite different names*

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
 
 
 class Accelerator(
     ros_cdk_core.Resource,
@@ -29,79 +31,85 @@
 ):
     '''A ROS resource type:  ``ALIYUN::GA::Accelerator``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "AcceleratorProps",
+        props: typing.Union["AcceleratorProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::GA::Accelerator``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Accelerator.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAcceleratorId")
     def attr_accelerator_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute AcceleratorId: The ID of the GA instance to query.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAcceleratorId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAcceleratorName")
     def attr_accelerator_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute AcceleratorName: The Name of the GA instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAcceleratorName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAutoPay")
     def attr_auto_pay(self) -> ros_cdk_core.IResolvable:
         '''Attribute AutoPay: The AutoPay of the GA instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAutoPay"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAutoUseCoupon")
     def attr_auto_use_coupon(self) -> ros_cdk_core.IResolvable:
         '''Attribute AutoUseCoupon: The AutoUseCoupon of the GA instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAutoUseCoupon"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDuration")
     def attr_duration(self) -> ros_cdk_core.IResolvable:
         '''Attribute Duration: The Duration of the GA instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDuration"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrOrderId")
     def attr_order_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute OrderId: The OrderId of the GA instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrOrderId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPaymentType")
     def attr_payment_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute PaymentType: The Payment Typethe GA instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPaymentType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPricingCycle")
     def attr_pricing_cycle(self) -> ros_cdk_core.IResolvable:
         '''Attribute PricingCycle: The PricingCycle of the GA instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPricingCycle"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSpec")
     def attr_spec(self) -> ros_cdk_core.IResolvable:
         '''Attribute Spec: The instance type of the GA instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSpec"))
 
 
 @jsii.data_type(
@@ -132,14 +140,22 @@
         :param duration: Property duration: The Duration of the GA instance.
         :param pricing_cycle: Property pricingCycle: The PricingCycle of the GA instance.
         :param spec: Property spec: The instance type of the GA instance.
         :param accelerator_name: Property acceleratorName: The Name of the GA instance.
         :param auto_pay: Property autoPay: The AutoPay of the GA instance.
         :param auto_use_coupon: Property autoUseCoupon: The AutoUseCoupon of the GA instance.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(AcceleratorProps.__init__)
+            check_type(argname="argument duration", value=duration, expected_type=type_hints["duration"])
+            check_type(argname="argument pricing_cycle", value=pricing_cycle, expected_type=type_hints["pricing_cycle"])
+            check_type(argname="argument spec", value=spec, expected_type=type_hints["spec"])
+            check_type(argname="argument accelerator_name", value=accelerator_name, expected_type=type_hints["accelerator_name"])
+            check_type(argname="argument auto_pay", value=auto_pay, expected_type=type_hints["auto_pay"])
+            check_type(argname="argument auto_use_coupon", value=auto_use_coupon, expected_type=type_hints["auto_use_coupon"])
         self._values: typing.Dict[str, typing.Any] = {
             "duration": duration,
             "pricing_cycle": pricing_cycle,
             "spec": spec,
         }
         if accelerator_name is not None:
             self._values["accelerator_name"] = accelerator_name
@@ -212,103 +228,109 @@
 ):
     '''A ROS resource type:  ``ALIYUN::GA::BandwidthPackage``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "BandwidthPackageProps",
+        props: typing.Union["BandwidthPackageProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::GA::BandwidthPackage``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(BandwidthPackage.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAutoPay")
     def attr_auto_pay(self) -> ros_cdk_core.IResolvable:
         '''Attribute AutoPay: The AutoPay of the bandwidth.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAutoPay"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAutoUseCoupon")
     def attr_auto_use_coupon(self) -> ros_cdk_core.IResolvable:
         '''Attribute AutoUseCoupon: The AutoUseCoupon  of the bandwidth.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAutoUseCoupon"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrBandwidth")
     def attr_bandwidth(self) -> ros_cdk_core.IResolvable:
         '''Attribute Bandwidth: The bandwidth provided by the bandwidth plan.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrBandwidth"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrBandwidthPackageId")
     def attr_bandwidth_package_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute BandwidthPackageId: The Resource ID of the bandwidth.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrBandwidthPackageId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrBandwidthPackageName")
     def attr_bandwidth_package_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute BandwidthPackageName: The Resource name of the bandwidth.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrBandwidthPackageName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrBandwidthType")
     def attr_bandwidth_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute BandwidthType: the bandwidth BandwidthType of the bandwidth.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrBandwidthType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrBillingType")
     def attr_billing_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute BillingType: The BillingType of the bandwidth.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrBillingType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCbnGeographicRegionIdA")
     def attr_cbn_geographic_region_id_a(self) -> ros_cdk_core.IResolvable:
         '''Attribute CbnGeographicRegionIdA: The CbnGeographicRegionIdA  of the bandwidth.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCbnGeographicRegionIdA"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCbnGeographicRegionIdB")
     def attr_cbn_geographic_region_id_b(self) -> ros_cdk_core.IResolvable:
         '''Attribute CbnGeographicRegionIdB: The CbnGeographicRegionIdB of the bandwidth.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCbnGeographicRegionIdB"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrChargeType")
     def attr_charge_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute ChargeType: The ChargeType of the bandwidth.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrChargeType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPaymentType")
     def attr_payment_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute PaymentType: The Payment Type of the bandwidth.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPaymentType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrRatio")
     def attr_ratio(self) -> ros_cdk_core.IResolvable:
         '''Attribute Ratio: The Ratio of the bandwidth.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRatio"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrType")
     def attr_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute Type: The type of the bandwidth plan.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrType"))
 
 
 class BandwidthPackageAcceleratorAddition(
@@ -318,37 +340,43 @@
 ):
     '''A ROS resource type:  ``ALIYUN::GA::BandwidthPackageAcceleratorAddition``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "BandwidthPackageAcceleratorAdditionProps",
+        props: typing.Union["BandwidthPackageAcceleratorAdditionProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::GA::BandwidthPackageAcceleratorAddition``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(BandwidthPackageAcceleratorAddition.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAcceleratorId")
     def attr_accelerator_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute AcceleratorId: The ID of the Global Accelerator instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAcceleratorId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrBandwidthPackageId")
     def attr_bandwidth_package_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute BandwidthPackageId: The ID of the bandwidth package which is associated.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrBandwidthPackageId"))
 
 
 @jsii.data_type(
@@ -367,14 +395,18 @@
         bandwidth_package_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::GA::BandwidthPackageAcceleratorAddition``.
 
         :param accelerator_id: Property acceleratorId: The ID of the Global Accelerator instance with which you want to associate the bandwidth plan.
         :param bandwidth_package_id: Property bandwidthPackageId: The ID of the bandwidth package to associate.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(BandwidthPackageAcceleratorAdditionProps.__init__)
+            check_type(argname="argument accelerator_id", value=accelerator_id, expected_type=type_hints["accelerator_id"])
+            check_type(argname="argument bandwidth_package_id", value=bandwidth_package_id, expected_type=type_hints["bandwidth_package_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "accelerator_id": accelerator_id,
             "bandwidth_package_id": bandwidth_package_id,
         }
 
     @builtins.property
     def accelerator_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -450,14 +482,28 @@
         :param cbn_geographic_region_id_a: Property cbnGeographicRegionIdA: The CbnGeographicRegionIdA of the bandwidth.
         :param cbn_geographic_region_id_b: Property cbnGeographicRegionIdB: The CbnGeographicRegionIdB of the bandwidth.
         :param charge_type: Property chargeType: The ChargeType of the bandwidth.
         :param duration: Property duration:.
         :param pricing_cycle: Property pricingCycle:.
         :param ratio: Property ratio: The Ratio of the bandwidth.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(BandwidthPackageProps.__init__)
+            check_type(argname="argument bandwidth", value=bandwidth, expected_type=type_hints["bandwidth"])
+            check_type(argname="argument type", value=type, expected_type=type_hints["type"])
+            check_type(argname="argument auto_pay", value=auto_pay, expected_type=type_hints["auto_pay"])
+            check_type(argname="argument auto_use_coupon", value=auto_use_coupon, expected_type=type_hints["auto_use_coupon"])
+            check_type(argname="argument bandwidth_type", value=bandwidth_type, expected_type=type_hints["bandwidth_type"])
+            check_type(argname="argument billing_type", value=billing_type, expected_type=type_hints["billing_type"])
+            check_type(argname="argument cbn_geographic_region_id_a", value=cbn_geographic_region_id_a, expected_type=type_hints["cbn_geographic_region_id_a"])
+            check_type(argname="argument cbn_geographic_region_id_b", value=cbn_geographic_region_id_b, expected_type=type_hints["cbn_geographic_region_id_b"])
+            check_type(argname="argument charge_type", value=charge_type, expected_type=type_hints["charge_type"])
+            check_type(argname="argument duration", value=duration, expected_type=type_hints["duration"])
+            check_type(argname="argument pricing_cycle", value=pricing_cycle, expected_type=type_hints["pricing_cycle"])
+            check_type(argname="argument ratio", value=ratio, expected_type=type_hints["ratio"])
         self._values: typing.Dict[str, typing.Any] = {
             "bandwidth": bandwidth,
             "type": type,
         }
         if auto_pay is not None:
             self._values["auto_pay"] = auto_pay
         if auto_use_coupon is not None:
@@ -592,31 +638,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::GA::EndpointGroup``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "EndpointGroupProps",
+        props: typing.Union["EndpointGroupProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::GA::EndpointGroup``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(EndpointGroup.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrEndpointGroupId")
     def attr_endpoint_group_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute EndpointGroupId: The ID of the endpoint group.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrEndpointGroupId"))
 
 
 @jsii.data_type(
@@ -641,15 +693,15 @@
     },
 )
 class EndpointGroupProps:
     def __init__(
         self,
         *,
         accelerator_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        endpoint_configurations: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosEndpointGroup.EndpointConfigurationsProperty"]]],
+        endpoint_configurations: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosEndpointGroup.EndpointConfigurationsProperty", typing.Dict[str, typing.Any]]]]],
         endpoint_group_region: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         listener_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         endpoint_group_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         endpoint_request_protocol: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         health_check_enabled: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         health_check_interval_seconds: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
@@ -674,14 +726,31 @@
         :param health_check_path: Property healthCheckPath: The path set as the destination on the targets for health checks.
         :param health_check_port: Property healthCheckPort: The port that is used to connect with the targets for health checks.
         :param health_check_protocol: Property healthCheckProtocol: The protocol that is used to connect with the targets for health checks. tcp: TCP protocol http: HTTP protocol https: HTTPS protocol
         :param name: Property name: The name of the endpoint group.
         :param threshold_count: Property thresholdCount: The number of consecutive health check failures that must occur before a healthy endpoint is considered unhealthy, or the number of consecutive health check successes that must occur before an unhealthy endpoint is considered healthy. Valid values: 2 to 10. Default value: 3.
         :param traffic_percentage: Property trafficPercentage: The weight of the endpoint group when the corresponding listener is associated with multiple endpoint groups.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(EndpointGroupProps.__init__)
+            check_type(argname="argument accelerator_id", value=accelerator_id, expected_type=type_hints["accelerator_id"])
+            check_type(argname="argument endpoint_configurations", value=endpoint_configurations, expected_type=type_hints["endpoint_configurations"])
+            check_type(argname="argument endpoint_group_region", value=endpoint_group_region, expected_type=type_hints["endpoint_group_region"])
+            check_type(argname="argument listener_id", value=listener_id, expected_type=type_hints["listener_id"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument endpoint_group_type", value=endpoint_group_type, expected_type=type_hints["endpoint_group_type"])
+            check_type(argname="argument endpoint_request_protocol", value=endpoint_request_protocol, expected_type=type_hints["endpoint_request_protocol"])
+            check_type(argname="argument health_check_enabled", value=health_check_enabled, expected_type=type_hints["health_check_enabled"])
+            check_type(argname="argument health_check_interval_seconds", value=health_check_interval_seconds, expected_type=type_hints["health_check_interval_seconds"])
+            check_type(argname="argument health_check_path", value=health_check_path, expected_type=type_hints["health_check_path"])
+            check_type(argname="argument health_check_port", value=health_check_port, expected_type=type_hints["health_check_port"])
+            check_type(argname="argument health_check_protocol", value=health_check_protocol, expected_type=type_hints["health_check_protocol"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument threshold_count", value=threshold_count, expected_type=type_hints["threshold_count"])
+            check_type(argname="argument traffic_percentage", value=traffic_percentage, expected_type=type_hints["traffic_percentage"])
         self._values: typing.Dict[str, typing.Any] = {
             "accelerator_id": accelerator_id,
             "endpoint_configurations": endpoint_configurations,
             "endpoint_group_region": endpoint_group_region,
             "listener_id": listener_id,
         }
         if description is not None:
@@ -870,43 +939,49 @@
 ):
     '''A ROS resource type:  ``ALIYUN::GA::IpSets``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "IpSetsProps",
+        props: typing.Union["IpSetsProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::GA::IpSets``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(IpSets.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAccelerateRegionIds")
     def attr_accelerate_region_ids(self) -> ros_cdk_core.IResolvable:
         '''Attribute AccelerateRegionIds: The ID list of the accelerate region.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAccelerateRegionIds"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrIpSetIds")
     def attr_ip_set_ids(self) -> ros_cdk_core.IResolvable:
         '''Attribute IpSetIds: The ID list of the ip set.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrIpSetIds"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrIpVersions")
     def attr_ip_versions(self) -> ros_cdk_core.IResolvable:
         '''Attribute IpVersions: The IP version list of the accelerate region.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrIpVersions"))
 
 
 @jsii.data_type(
@@ -917,22 +992,26 @@
         "accelerator_id": "acceleratorId",
     },
 )
 class IpSetsProps:
     def __init__(
         self,
         *,
-        accelerate_region: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosIpSets.AccelerateRegionProperty"]]],
+        accelerate_region: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosIpSets.AccelerateRegionProperty", typing.Dict[str, typing.Any]]]]],
         accelerator_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::GA::IpSets``.
 
         :param accelerate_region: Property accelerateRegion:.
         :param accelerator_id: Property acceleratorId: The ID of the GA instance.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(IpSetsProps.__init__)
+            check_type(argname="argument accelerate_region", value=accelerate_region, expected_type=type_hints["accelerate_region"])
+            check_type(argname="argument accelerator_id", value=accelerator_id, expected_type=type_hints["accelerator_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "accelerate_region": accelerate_region,
             "accelerator_id": accelerator_id,
         }
 
     @builtins.property
     def accelerate_region(
@@ -969,31 +1048,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::GA::Listener``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "ListenerProps",
+        props: typing.Union["ListenerProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::GA::Listener``.
 
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
     @jsii.member(jsii_name="attrListenerId")
     def attr_listener_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ListenerId: The ID of the listener.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrListenerId"))
 
 
 @jsii.data_type(
@@ -1013,37 +1098,49 @@
     },
 )
 class ListenerProps:
     def __init__(
         self,
         *,
         accelerator_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        port_ranges: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosListener.PortRangesProperty"]]],
+        port_ranges: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosListener.PortRangesProperty", typing.Dict[str, typing.Any]]]]],
         protocol: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        certificates: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosListener.CertificatesProperty"]]]] = None,
+        certificates: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosListener.CertificatesProperty", typing.Dict[str, typing.Any]]]]]] = None,
         client_affinity: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         proxy_protocol: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         security_policy_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        x_forwarded_for_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosListener.XForwardedForConfigProperty"]] = None,
+        x_forwarded_for_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosListener.XForwardedForConfigProperty", typing.Dict[str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::GA::Listener``.
 
         :param accelerator_id: Property acceleratorId: The ID of the Global Accelerator instance to which the listener will be added.
         :param port_ranges: Property portRanges:.
         :param protocol: Property protocol: The network transmission protocol of the listener. Valid values: tcp: TCP protocol udp: UDP protocol http: HTTP protocolhttps: HTTPS protocol.
         :param certificates: Property certificates:.
         :param client_affinity: Property clientAffinity: Specifies whether to enable client affinity for the listener. If you do not specify the default value in the parameter, client affinity is disabled. When client affinity is disabled, the connections from a specific source (client) IP address are not always routed to the same endpoint. If you set the value to SOURCE_IP, client affinity is enabled. When client affinity is enabled, the connections from a specific source (client) IP address are always routed to the same endpoint.
         :param description: Property description: The description of the listener.
         :param name: Property name: The name of the listener. The name must be 2 to 128 characters in length and can contain letters, digits, underscores (_), and hyphens (-). It must start with a letter or Chinese character.
         :param proxy_protocol: Property proxyProtocol: Specifies whether to preserve client IP addresses. Valid values: true: preserves client IP addresses. After this feature is enabled, backend servers can retrieve client IP addresses. false (default): does not preserve client IP addresses.
         :param security_policy_id: Property securityPolicyId: The ID of the security policy. Valid values: tls_cipher_policy_1_0 tls_cipher_policy_1_1 tls_cipher_policy_1_2 tls_cipher_policy_1_2_strict tls_cipher_policy_1_2_strict_with_1_3 Note Only HTTPS listeners support this parameter.
         :param x_forwarded_for_config: Property xForwardedForConfig: The configuration of the XForward field.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ListenerProps.__init__)
+            check_type(argname="argument accelerator_id", value=accelerator_id, expected_type=type_hints["accelerator_id"])
+            check_type(argname="argument port_ranges", value=port_ranges, expected_type=type_hints["port_ranges"])
+            check_type(argname="argument protocol", value=protocol, expected_type=type_hints["protocol"])
+            check_type(argname="argument certificates", value=certificates, expected_type=type_hints["certificates"])
+            check_type(argname="argument client_affinity", value=client_affinity, expected_type=type_hints["client_affinity"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument proxy_protocol", value=proxy_protocol, expected_type=type_hints["proxy_protocol"])
+            check_type(argname="argument security_policy_id", value=security_policy_id, expected_type=type_hints["security_policy_id"])
+            check_type(argname="argument x_forwarded_for_config", value=x_forwarded_for_config, expected_type=type_hints["x_forwarded_for_config"])
         self._values: typing.Dict[str, typing.Any] = {
             "accelerator_id": accelerator_id,
             "port_ranges": port_ranges,
             "protocol": protocol,
         }
         if certificates is not None:
             self._values["certificates"] = certificates
@@ -1189,219 +1286,249 @@
 ):
     '''A ROS template type:  ``ALIYUN::GA::Accelerator``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosAcceleratorProps",
+        props: typing.Union["RosAcceleratorProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::GA::Accelerator``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosAccelerator.__init__)
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
+            type_hints = typing.get_type_hints(RosAccelerator._render_properties)
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
     @jsii.member(jsii_name="attrAcceleratorId")
     def attr_accelerator_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: AcceleratorId: The ID of the GA instance to query.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAcceleratorId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAcceleratorName")
     def attr_accelerator_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: AcceleratorName: The Name of the GA instance
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAcceleratorName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAutoPay")
     def attr_auto_pay(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: AutoPay: The AutoPay of the GA instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAutoPay"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAutoUseCoupon")
     def attr_auto_use_coupon(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: AutoUseCoupon: The AutoUseCoupon of the GA instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAutoUseCoupon"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDuration")
     def attr_duration(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Duration: The Duration of the GA instance
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDuration"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrOrderId")
     def attr_order_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: OrderId: The OrderId of the GA instance
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrOrderId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPaymentType")
     def attr_payment_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: PaymentType: The Payment Typethe GA instance
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPaymentType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPricingCycle")
     def attr_pricing_cycle(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: PricingCycle: The PricingCycle of the GA instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPricingCycle"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSpec")
     def attr_spec(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Spec: The instance type of the GA instance
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSpec"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="duration")
     def duration(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: duration: The Duration of the GA instance
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "duration"))
 
     @duration.setter
     def duration(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAccelerator, "duration").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "duration", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAccelerator, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="pricingCycle")
     def pricing_cycle(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: pricingCycle: The PricingCycle of the GA instance.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "pricingCycle"))
 
     @pricing_cycle.setter
     def pricing_cycle(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAccelerator, "pricing_cycle").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "pricingCycle", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="spec")
     def spec(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: spec: The instance type of the GA instance
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "spec"))
 
     @spec.setter
     def spec(self, value: typing.Union[builtins.str, ros_cdk_core.IResolvable]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAccelerator, "spec").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "spec", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="acceleratorName")
     def accelerator_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: acceleratorName: The Name of the GA instance
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "acceleratorName"))
 
     @accelerator_name.setter
     def accelerator_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAccelerator, "accelerator_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "acceleratorName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="autoPay")
     def auto_pay(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: autoPay: The AutoPay of the GA instance.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "autoPay"))
 
     @auto_pay.setter
     def auto_pay(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAccelerator, "auto_pay").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "autoPay", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="autoUseCoupon")
     def auto_use_coupon(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: autoUseCoupon: The AutoUseCoupon of the GA instance.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "autoUseCoupon"))
 
     @auto_use_coupon.setter
     def auto_use_coupon(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAccelerator, "auto_use_coupon").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "autoUseCoupon", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-ga.RosAcceleratorProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -1429,14 +1556,22 @@
         :param duration: 
         :param pricing_cycle: 
         :param spec: 
         :param accelerator_name: 
         :param auto_pay: 
         :param auto_use_coupon: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosAcceleratorProps.__init__)
+            check_type(argname="argument duration", value=duration, expected_type=type_hints["duration"])
+            check_type(argname="argument pricing_cycle", value=pricing_cycle, expected_type=type_hints["pricing_cycle"])
+            check_type(argname="argument spec", value=spec, expected_type=type_hints["spec"])
+            check_type(argname="argument accelerator_name", value=accelerator_name, expected_type=type_hints["accelerator_name"])
+            check_type(argname="argument auto_pay", value=auto_pay, expected_type=type_hints["auto_pay"])
+            check_type(argname="argument auto_use_coupon", value=auto_use_coupon, expected_type=type_hints["auto_use_coupon"])
         self._values: typing.Dict[str, typing.Any] = {
             "duration": duration,
             "pricing_cycle": pricing_cycle,
             "spec": spec,
         }
         if accelerator_name is not None:
             self._values["accelerator_name"] = accelerator_name
@@ -1521,419 +1656,476 @@
 ):
     '''A ROS template type:  ``ALIYUN::GA::BandwidthPackage``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosBandwidthPackageProps",
+        props: typing.Union["RosBandwidthPackageProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::GA::BandwidthPackage``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosBandwidthPackage.__init__)
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
+            type_hints = typing.get_type_hints(RosBandwidthPackage._render_properties)
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
     @jsii.member(jsii_name="attrAutoPay")
     def attr_auto_pay(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: AutoPay: The AutoPay of the bandwidth
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAutoPay"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAutoUseCoupon")
     def attr_auto_use_coupon(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: AutoUseCoupon: The AutoUseCoupon  of the bandwidth
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAutoUseCoupon"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrBandwidth")
     def attr_bandwidth(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Bandwidth: The bandwidth provided by the bandwidth plan.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrBandwidth"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrBandwidthPackageId")
     def attr_bandwidth_package_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: BandwidthPackageId: The Resource ID of the bandwidth
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrBandwidthPackageId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrBandwidthPackageName")
     def attr_bandwidth_package_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: BandwidthPackageName: The Resource name of the bandwidth
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrBandwidthPackageName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrBandwidthType")
     def attr_bandwidth_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: BandwidthType: the bandwidth BandwidthType of the bandwidth
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrBandwidthType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrBillingType")
     def attr_billing_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: BillingType: The BillingType of the bandwidth
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrBillingType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCbnGeographicRegionIdA")
     def attr_cbn_geographic_region_id_a(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: CbnGeographicRegionIdA: The CbnGeographicRegionIdA  of the bandwidth
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCbnGeographicRegionIdA"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCbnGeographicRegionIdB")
     def attr_cbn_geographic_region_id_b(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: CbnGeographicRegionIdB: The CbnGeographicRegionIdB of the bandwidth
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCbnGeographicRegionIdB"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrChargeType")
     def attr_charge_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ChargeType: The ChargeType of the bandwidth
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrChargeType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPaymentType")
     def attr_payment_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: PaymentType: The Payment Type of the bandwidth
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPaymentType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrRatio")
     def attr_ratio(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Ratio: The Ratio of the bandwidth
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRatio"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrType")
     def attr_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Type: The type of the bandwidth plan
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrType"))
 
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
         :Property: bandwidth: The bandwidth provided by the bandwidth plan.
         '''
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "bandwidth"))
 
     @bandwidth.setter
     def bandwidth(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosBandwidthPackage, "bandwidth").fset)
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
+            type_hints = typing.get_type_hints(getattr(RosBandwidthPackage, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="type")
     def type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: type: The type of the bandwidth plan
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "type"))
 
     @type.setter
     def type(self, value: typing.Union[builtins.str, ros_cdk_core.IResolvable]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosBandwidthPackage, "type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "type", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="autoPay")
     def auto_pay(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: autoPay: The AutoPay of the bandwidth
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "autoPay"))
 
     @auto_pay.setter
     def auto_pay(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosBandwidthPackage, "auto_pay").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "autoPay", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="autoUseCoupon")
     def auto_use_coupon(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: autoUseCoupon: The AutoUseCoupon  of the bandwidth
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "autoUseCoupon"))
 
     @auto_use_coupon.setter
     def auto_use_coupon(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosBandwidthPackage, "auto_use_coupon").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "autoUseCoupon", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="bandwidthType")
     def bandwidth_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: bandwidthType: the bandwidth BandwidthType of the bandwidth
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "bandwidthType"))
 
     @bandwidth_type.setter
     def bandwidth_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosBandwidthPackage, "bandwidth_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "bandwidthType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="billingType")
     def billing_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: billingType: The BillingType of the bandwidth
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "billingType"))
 
     @billing_type.setter
     def billing_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosBandwidthPackage, "billing_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "billingType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="cbnGeographicRegionIdA")
     def cbn_geographic_region_id_a(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: cbnGeographicRegionIdA: The CbnGeographicRegionIdA  of the bandwidth
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "cbnGeographicRegionIdA"))
 
     @cbn_geographic_region_id_a.setter
     def cbn_geographic_region_id_a(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosBandwidthPackage, "cbn_geographic_region_id_a").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "cbnGeographicRegionIdA", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="cbnGeographicRegionIdB")
     def cbn_geographic_region_id_b(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: cbnGeographicRegionIdB: The CbnGeographicRegionIdB of the bandwidth
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "cbnGeographicRegionIdB"))
 
     @cbn_geographic_region_id_b.setter
     def cbn_geographic_region_id_b(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosBandwidthPackage, "cbn_geographic_region_id_b").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "cbnGeographicRegionIdB", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="chargeType")
     def charge_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: chargeType: The ChargeType of the bandwidth
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "chargeType"))
 
     @charge_type.setter
     def charge_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosBandwidthPackage, "charge_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "chargeType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="duration")
     def duration(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: duration:
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "duration"))
 
     @duration.setter
     def duration(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosBandwidthPackage, "duration").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "duration", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="pricingCycle")
     def pricing_cycle(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: pricingCycle:
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "pricingCycle"))
 
     @pricing_cycle.setter
     def pricing_cycle(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosBandwidthPackage, "pricing_cycle").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "pricingCycle", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="ratio")
     def ratio(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: ratio: The Ratio of the bandwidth
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "ratio"))
 
     @ratio.setter
     def ratio(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosBandwidthPackage, "ratio").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ratio", value)
 
 
 class RosBandwidthPackageAcceleratorAddition(
     ros_cdk_core.RosResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-ga.RosBandwidthPackageAcceleratorAddition",
 ):
     '''A ROS template type:  ``ALIYUN::GA::BandwidthPackageAcceleratorAddition``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosBandwidthPackageAcceleratorAdditionProps",
+        props: typing.Union["RosBandwidthPackageAcceleratorAdditionProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::GA::BandwidthPackageAcceleratorAddition``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosBandwidthPackageAcceleratorAddition.__init__)
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
+            type_hints = typing.get_type_hints(RosBandwidthPackageAcceleratorAddition._render_properties)
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
     @jsii.member(jsii_name="attrAcceleratorId")
     def attr_accelerator_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: AcceleratorId: The ID of the Global Accelerator instance
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAcceleratorId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrBandwidthPackageId")
     def attr_bandwidth_package_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: BandwidthPackageId: The ID of the bandwidth package which is associated
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrBandwidthPackageId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="acceleratorId")
     def accelerator_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         acceleratorId: The ID of the Global Accelerator instance with which you want to associate the bandwidth
         plan.
@@ -1941,40 +2133,49 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "acceleratorId"))
 
     @accelerator_id.setter
     def accelerator_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosBandwidthPackageAcceleratorAddition, "accelerator_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "acceleratorId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="bandwidthPackageId")
     def bandwidth_package_id(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: bandwidthPackageId: The ID of the bandwidth package to associate.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "bandwidthPackageId"))
 
     @bandwidth_package_id.setter
     def bandwidth_package_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosBandwidthPackageAcceleratorAddition, "bandwidth_package_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "bandwidthPackageId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosBandwidthPackageAcceleratorAddition, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-ga.RosBandwidthPackageAcceleratorAdditionProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -1990,14 +2191,18 @@
         bandwidth_package_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::GA::BandwidthPackageAcceleratorAddition``.
 
         :param accelerator_id: 
         :param bandwidth_package_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosBandwidthPackageAcceleratorAdditionProps.__init__)
+            check_type(argname="argument accelerator_id", value=accelerator_id, expected_type=type_hints["accelerator_id"])
+            check_type(argname="argument bandwidth_package_id", value=bandwidth_package_id, expected_type=type_hints["bandwidth_package_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "accelerator_id": accelerator_id,
             "bandwidth_package_id": bandwidth_package_id,
         }
 
     @builtins.property
     def accelerator_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -2080,14 +2285,28 @@
         :param cbn_geographic_region_id_a: 
         :param cbn_geographic_region_id_b: 
         :param charge_type: 
         :param duration: 
         :param pricing_cycle: 
         :param ratio: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosBandwidthPackageProps.__init__)
+            check_type(argname="argument bandwidth", value=bandwidth, expected_type=type_hints["bandwidth"])
+            check_type(argname="argument type", value=type, expected_type=type_hints["type"])
+            check_type(argname="argument auto_pay", value=auto_pay, expected_type=type_hints["auto_pay"])
+            check_type(argname="argument auto_use_coupon", value=auto_use_coupon, expected_type=type_hints["auto_use_coupon"])
+            check_type(argname="argument bandwidth_type", value=bandwidth_type, expected_type=type_hints["bandwidth_type"])
+            check_type(argname="argument billing_type", value=billing_type, expected_type=type_hints["billing_type"])
+            check_type(argname="argument cbn_geographic_region_id_a", value=cbn_geographic_region_id_a, expected_type=type_hints["cbn_geographic_region_id_a"])
+            check_type(argname="argument cbn_geographic_region_id_b", value=cbn_geographic_region_id_b, expected_type=type_hints["cbn_geographic_region_id_b"])
+            check_type(argname="argument charge_type", value=charge_type, expected_type=type_hints["charge_type"])
+            check_type(argname="argument duration", value=duration, expected_type=type_hints["duration"])
+            check_type(argname="argument pricing_cycle", value=pricing_cycle, expected_type=type_hints["pricing_cycle"])
+            check_type(argname="argument ratio", value=ratio, expected_type=type_hints["ratio"])
         self._values: typing.Dict[str, typing.Any] = {
             "bandwidth": bandwidth,
             "type": type,
         }
         if auto_pay is not None:
             self._values["auto_pay"] = auto_pay
         if auto_use_coupon is not None:
@@ -2246,146 +2465,173 @@
 ):
     '''A ROS template type:  ``ALIYUN::GA::EndpointGroup``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosEndpointGroupProps",
+        props: typing.Union["RosEndpointGroupProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::GA::EndpointGroup``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosEndpointGroup.__init__)
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
+            type_hints = typing.get_type_hints(RosEndpointGroup._render_properties)
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
     @jsii.member(jsii_name="attrEndpointGroupId")
     def attr_endpoint_group_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: EndpointGroupId: The ID of the endpoint group.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrEndpointGroupId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="acceleratorId")
     def accelerator_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: acceleratorId: The ID of the Global Accelerator instance with which the endpoint group will be associated.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "acceleratorId"))
 
     @accelerator_id.setter
     def accelerator_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosEndpointGroup, "accelerator_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "acceleratorId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosEndpointGroup, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="endpointConfigurations")
     def endpoint_configurations(
         self,
     ) -> typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosEndpointGroup.EndpointConfigurationsProperty"]]]:
         '''
         :Property: endpointConfigurations:
         '''
         return typing.cast(typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosEndpointGroup.EndpointConfigurationsProperty"]]], jsii.get(self, "endpointConfigurations"))
 
     @endpoint_configurations.setter
     def endpoint_configurations(
         self,
         value: typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosEndpointGroup.EndpointConfigurationsProperty"]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosEndpointGroup, "endpoint_configurations").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "endpointConfigurations", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="endpointGroupRegion")
     def endpoint_group_region(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: endpointGroupRegion: The region ID of the endpoint group.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "endpointGroupRegion"))
 
     @endpoint_group_region.setter
     def endpoint_group_region(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosEndpointGroup, "endpoint_group_region").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "endpointGroupRegion", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="listenerId")
     def listener_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: listenerId: The ID of the listener to be associated with the endpoint group.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "listenerId"))
 
     @listener_id.setter
     def listener_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosEndpointGroup, "listener_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "listenerId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: description: The description of the endpoint group.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosEndpointGroup, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="endpointGroupType")
     def endpoint_group_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2397,17 +2643,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "endpointGroupType"))
 
     @endpoint_group_type.setter
     def endpoint_group_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosEndpointGroup, "endpoint_group_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "endpointGroupType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="endpointRequestProtocol")
     def endpoint_request_protocol(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2420,85 +2669,100 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "endpointRequestProtocol"))
 
     @endpoint_request_protocol.setter
     def endpoint_request_protocol(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosEndpointGroup, "endpoint_request_protocol").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "endpointRequestProtocol", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="healthCheckEnabled")
     def health_check_enabled(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: healthCheckEnabled: Specifies whether to enable the health check feature.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "healthCheckEnabled"))
 
     @health_check_enabled.setter
     def health_check_enabled(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosEndpointGroup, "health_check_enabled").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "healthCheckEnabled", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="healthCheckIntervalSeconds")
     def health_check_interval_seconds(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: healthCheckIntervalSeconds: The interval between two consecutive health checks. Unit: seconds.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "healthCheckIntervalSeconds"))
 
     @health_check_interval_seconds.setter
     def health_check_interval_seconds(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosEndpointGroup, "health_check_interval_seconds").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "healthCheckIntervalSeconds", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="healthCheckPath")
     def health_check_path(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: healthCheckPath: The path set as the destination on the targets for health checks.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "healthCheckPath"))
 
     @health_check_path.setter
     def health_check_path(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosEndpointGroup, "health_check_path").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "healthCheckPath", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="healthCheckPort")
     def health_check_port(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: healthCheckPort: The port that is used to connect with the targets for health checks.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "healthCheckPort"))
 
     @health_check_port.setter
     def health_check_port(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosEndpointGroup, "health_check_port").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "healthCheckPort", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="healthCheckProtocol")
     def health_check_protocol(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2510,34 +2774,40 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "healthCheckProtocol"))
 
     @health_check_protocol.setter
     def health_check_protocol(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosEndpointGroup, "health_check_protocol").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "healthCheckProtocol", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="name")
     def name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: name: The name of the endpoint group.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "name"))
 
     @name.setter
     def name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosEndpointGroup, "name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "name", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="thresholdCount")
     def threshold_count(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2547,17 +2817,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "thresholdCount"))
 
     @threshold_count.setter
     def threshold_count(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosEndpointGroup, "threshold_count").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "thresholdCount", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="trafficPercentage")
     def traffic_percentage(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2567,14 +2840,17 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "trafficPercentage"))
 
     @traffic_percentage.setter
     def traffic_percentage(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosEndpointGroup, "traffic_percentage").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "trafficPercentage", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-ga.RosEndpointGroup.EndpointConfigurationsProperty",
         jsii_struct_bases=[],
         name_mapping={
             "endpoint": "endpoint",
@@ -2597,14 +2873,21 @@
             '''
             :param endpoint: 
             :param type: 
             :param weight: 
             :param enable_client_ip_preservation: 
             :param enable_proxy_protocol: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosEndpointGroup.EndpointConfigurationsProperty.__init__)
+                check_type(argname="argument endpoint", value=endpoint, expected_type=type_hints["endpoint"])
+                check_type(argname="argument type", value=type, expected_type=type_hints["type"])
+                check_type(argname="argument weight", value=weight, expected_type=type_hints["weight"])
+                check_type(argname="argument enable_client_ip_preservation", value=enable_client_ip_preservation, expected_type=type_hints["enable_client_ip_preservation"])
+                check_type(argname="argument enable_proxy_protocol", value=enable_proxy_protocol, expected_type=type_hints["enable_proxy_protocol"])
             self._values: typing.Dict[str, typing.Any] = {
                 "endpoint": endpoint,
                 "type": type,
                 "weight": weight,
             }
             if enable_client_ip_preservation is not None:
                 self._values["enable_client_ip_preservation"] = enable_client_ip_preservation
@@ -2710,15 +2993,15 @@
     },
 )
 class RosEndpointGroupProps:
     def __init__(
         self,
         *,
         accelerator_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        endpoint_configurations: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosEndpointGroup.EndpointConfigurationsProperty]]],
+        endpoint_configurations: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosEndpointGroup.EndpointConfigurationsProperty, typing.Dict[str, typing.Any]]]]],
         endpoint_group_region: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         listener_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         endpoint_group_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         endpoint_request_protocol: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         health_check_enabled: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         health_check_interval_seconds: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
@@ -2743,14 +3026,31 @@
         :param health_check_path: 
         :param health_check_port: 
         :param health_check_protocol: 
         :param name: 
         :param threshold_count: 
         :param traffic_percentage: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosEndpointGroupProps.__init__)
+            check_type(argname="argument accelerator_id", value=accelerator_id, expected_type=type_hints["accelerator_id"])
+            check_type(argname="argument endpoint_configurations", value=endpoint_configurations, expected_type=type_hints["endpoint_configurations"])
+            check_type(argname="argument endpoint_group_region", value=endpoint_group_region, expected_type=type_hints["endpoint_group_region"])
+            check_type(argname="argument listener_id", value=listener_id, expected_type=type_hints["listener_id"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument endpoint_group_type", value=endpoint_group_type, expected_type=type_hints["endpoint_group_type"])
+            check_type(argname="argument endpoint_request_protocol", value=endpoint_request_protocol, expected_type=type_hints["endpoint_request_protocol"])
+            check_type(argname="argument health_check_enabled", value=health_check_enabled, expected_type=type_hints["health_check_enabled"])
+            check_type(argname="argument health_check_interval_seconds", value=health_check_interval_seconds, expected_type=type_hints["health_check_interval_seconds"])
+            check_type(argname="argument health_check_path", value=health_check_path, expected_type=type_hints["health_check_path"])
+            check_type(argname="argument health_check_port", value=health_check_port, expected_type=type_hints["health_check_port"])
+            check_type(argname="argument health_check_protocol", value=health_check_protocol, expected_type=type_hints["health_check_protocol"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument threshold_count", value=threshold_count, expected_type=type_hints["threshold_count"])
+            check_type(argname="argument traffic_percentage", value=traffic_percentage, expected_type=type_hints["traffic_percentage"])
         self._values: typing.Dict[str, typing.Any] = {
             "accelerator_id": accelerator_id,
             "endpoint_configurations": endpoint_configurations,
             "endpoint_group_region": endpoint_group_region,
             "listener_id": listener_id,
         }
         if description is not None:
@@ -2967,110 +3267,128 @@
 ):
     '''A ROS template type:  ``ALIYUN::GA::IpSets``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosIpSetsProps",
+        props: typing.Union["RosIpSetsProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::GA::IpSets``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosIpSets.__init__)
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
+            type_hints = typing.get_type_hints(RosIpSets._render_properties)
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
     @jsii.member(jsii_name="attrAccelerateRegionIds")
     def attr_accelerate_region_ids(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: AccelerateRegionIds: The ID list of the accelerate region.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAccelerateRegionIds"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrIpSetIds")
     def attr_ip_set_ids(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: IpSetIds: The ID list of the ip set.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrIpSetIds"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrIpVersions")
     def attr_ip_versions(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: IpVersions: The IP version list of the accelerate region.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrIpVersions"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="accelerateRegion")
     def accelerate_region(
         self,
     ) -> typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosIpSets.AccelerateRegionProperty"]]]:
         '''
         :Property: accelerateRegion:
         '''
         return typing.cast(typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosIpSets.AccelerateRegionProperty"]]], jsii.get(self, "accelerateRegion"))
 
     @accelerate_region.setter
     def accelerate_region(
         self,
         value: typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosIpSets.AccelerateRegionProperty"]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosIpSets, "accelerate_region").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "accelerateRegion", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="acceleratorId")
     def accelerator_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: acceleratorId: The ID of the GA instance.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "acceleratorId"))
 
     @accelerator_id.setter
     def accelerator_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosIpSets, "accelerator_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "acceleratorId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosIpSets, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-ga.RosIpSets.AccelerateRegionProperty",
         jsii_struct_bases=[],
         name_mapping={
             "accelerate_region_id": "accelerateRegionId",
@@ -3087,14 +3405,19 @@
             ip_version: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param accelerate_region_id: 
             :param bandwidth: 
             :param ip_version: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosIpSets.AccelerateRegionProperty.__init__)
+                check_type(argname="argument accelerate_region_id", value=accelerate_region_id, expected_type=type_hints["accelerate_region_id"])
+                check_type(argname="argument bandwidth", value=bandwidth, expected_type=type_hints["bandwidth"])
+                check_type(argname="argument ip_version", value=ip_version, expected_type=type_hints["ip_version"])
             self._values: typing.Dict[str, typing.Any] = {
                 "accelerate_region_id": accelerate_region_id,
                 "bandwidth": bandwidth,
             }
             if ip_version is not None:
                 self._values["ip_version"] = ip_version
 
@@ -3154,22 +3477,26 @@
         "accelerator_id": "acceleratorId",
     },
 )
 class RosIpSetsProps:
     def __init__(
         self,
         *,
-        accelerate_region: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosIpSets.AccelerateRegionProperty]]],
+        accelerate_region: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosIpSets.AccelerateRegionProperty, typing.Dict[str, typing.Any]]]]],
         accelerator_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::GA::IpSets``.
 
         :param accelerate_region: 
         :param accelerator_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosIpSetsProps.__init__)
+            check_type(argname="argument accelerate_region", value=accelerate_region, expected_type=type_hints["accelerate_region"])
+            check_type(argname="argument accelerator_id", value=accelerator_id, expected_type=type_hints["accelerator_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "accelerate_region": accelerate_region,
             "accelerator_id": accelerator_id,
         }
 
     @builtins.property
     def accelerate_region(
@@ -3210,97 +3537,115 @@
 ):
     '''A ROS template type:  ``ALIYUN::GA::Listener``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosListenerProps",
+        props: typing.Union["RosListenerProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::GA::Listener``.
 
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
     @jsii.member(jsii_name="attrListenerId")
     def attr_listener_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ListenerId: The ID of the listener.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrListenerId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="acceleratorId")
     def accelerator_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: acceleratorId: The ID of the Global Accelerator instance to which the listener will be added.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "acceleratorId"))
 
     @accelerator_id.setter
     def accelerator_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosListener, "accelerator_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "acceleratorId", value)
 
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
     @jsii.member(jsii_name="portRanges")
     def port_ranges(
         self,
     ) -> typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosListener.PortRangesProperty"]]]:
         '''
         :Property: portRanges:
         '''
         return typing.cast(typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosListener.PortRangesProperty"]]], jsii.get(self, "portRanges"))
 
     @port_ranges.setter
     def port_ranges(
         self,
         value: typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosListener.PortRangesProperty"]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosListener, "port_ranges").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "portRanges", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="protocol")
     def protocol(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         protocol: The network transmission protocol of the listener. Valid values:
         tcp: TCP protocol
@@ -3310,34 +3655,40 @@
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
     @jsii.member(jsii_name="certificates")
     def certificates(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosListener.CertificatesProperty"]]]]:
         '''
         :Property: certificates:
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosListener.CertificatesProperty"]]]], jsii.get(self, "certificates"))
 
     @certificates.setter
     def certificates(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosListener.CertificatesProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosListener, "certificates").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "certificates", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="clientAffinity")
     def client_affinity(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3351,34 +3702,40 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "clientAffinity"))
 
     @client_affinity.setter
     def client_affinity(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosListener, "client_affinity").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "clientAffinity", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: description: The description of the listener.
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
     @jsii.member(jsii_name="name")
     def name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3389,17 +3746,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "name"))
 
     @name.setter
     def name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosListener, "name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "name", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="proxyProtocol")
     def proxy_protocol(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3410,17 +3770,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "proxyProtocol"))
 
     @proxy_protocol.setter
     def proxy_protocol(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosListener, "proxy_protocol").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "proxyProtocol", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="securityPolicyId")
     def security_policy_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3435,31 +3798,37 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "securityPolicyId"))
 
     @security_policy_id.setter
     def security_policy_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosListener, "security_policy_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "securityPolicyId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="xForwardedForConfig")
     def x_forwarded_for_config(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosListener.XForwardedForConfigProperty"]]:
         '''
         :Property: xForwardedForConfig: The configuration of the XForward field.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosListener.XForwardedForConfigProperty"]], jsii.get(self, "xForwardedForConfig"))
 
     @x_forwarded_for_config.setter
     def x_forwarded_for_config(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosListener.XForwardedForConfigProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosListener, "x_forwarded_for_config").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "xForwardedForConfig", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-ga.RosListener.CertificatesProperty",
         jsii_struct_bases=[],
         name_mapping={"id": "id"},
     )
@@ -3468,14 +3837,17 @@
             self,
             *,
             id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param id: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosListener.CertificatesProperty.__init__)
+                check_type(argname="argument id", value=id, expected_type=type_hints["id"])
             self._values: typing.Dict[str, typing.Any] = {
                 "id": id,
             }
 
         @builtins.property
         def id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
             '''
@@ -3508,14 +3880,18 @@
             from_port: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
             to_port: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param from_port: 
             :param to_port: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosListener.PortRangesProperty.__init__)
+                check_type(argname="argument from_port", value=from_port, expected_type=type_hints["from_port"])
+                check_type(argname="argument to_port", value=to_port, expected_type=type_hints["to_port"])
             self._values: typing.Dict[str, typing.Any] = {
                 "from_port": from_port,
                 "to_port": to_port,
             }
 
         @builtins.property
         def from_port(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
@@ -3576,14 +3952,21 @@
             '''
             :param x_forwarded_for_ga_ap_enabled: 
             :param x_forwarded_for_ga_id_enabled: 
             :param x_forwarded_for_port_enabled: 
             :param x_forwarded_for_proto_enabled: 
             :param x_real_ip_enabled: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosListener.XForwardedForConfigProperty.__init__)
+                check_type(argname="argument x_forwarded_for_ga_ap_enabled", value=x_forwarded_for_ga_ap_enabled, expected_type=type_hints["x_forwarded_for_ga_ap_enabled"])
+                check_type(argname="argument x_forwarded_for_ga_id_enabled", value=x_forwarded_for_ga_id_enabled, expected_type=type_hints["x_forwarded_for_ga_id_enabled"])
+                check_type(argname="argument x_forwarded_for_port_enabled", value=x_forwarded_for_port_enabled, expected_type=type_hints["x_forwarded_for_port_enabled"])
+                check_type(argname="argument x_forwarded_for_proto_enabled", value=x_forwarded_for_proto_enabled, expected_type=type_hints["x_forwarded_for_proto_enabled"])
+                check_type(argname="argument x_real_ip_enabled", value=x_real_ip_enabled, expected_type=type_hints["x_real_ip_enabled"])
             self._values: typing.Dict[str, typing.Any] = {}
             if x_forwarded_for_ga_ap_enabled is not None:
                 self._values["x_forwarded_for_ga_ap_enabled"] = x_forwarded_for_ga_ap_enabled
             if x_forwarded_for_ga_id_enabled is not None:
                 self._values["x_forwarded_for_ga_id_enabled"] = x_forwarded_for_ga_id_enabled
             if x_forwarded_for_port_enabled is not None:
                 self._values["x_forwarded_for_port_enabled"] = x_forwarded_for_port_enabled
@@ -3696,37 +4079,49 @@
     },
 )
 class RosListenerProps:
     def __init__(
         self,
         *,
         accelerator_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        port_ranges: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosListener.PortRangesProperty]]],
+        port_ranges: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosListener.PortRangesProperty, typing.Dict[str, typing.Any]]]]],
         protocol: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        certificates: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosListener.CertificatesProperty]]]] = None,
+        certificates: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosListener.CertificatesProperty, typing.Dict[str, typing.Any]]]]]] = None,
         client_affinity: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         proxy_protocol: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         security_policy_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        x_forwarded_for_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosListener.XForwardedForConfigProperty]] = None,
+        x_forwarded_for_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosListener.XForwardedForConfigProperty, typing.Dict[str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::GA::Listener``.
 
         :param accelerator_id: 
         :param port_ranges: 
         :param protocol: 
         :param certificates: 
         :param client_affinity: 
         :param description: 
         :param name: 
         :param proxy_protocol: 
         :param security_policy_id: 
         :param x_forwarded_for_config: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosListenerProps.__init__)
+            check_type(argname="argument accelerator_id", value=accelerator_id, expected_type=type_hints["accelerator_id"])
+            check_type(argname="argument port_ranges", value=port_ranges, expected_type=type_hints["port_ranges"])
+            check_type(argname="argument protocol", value=protocol, expected_type=type_hints["protocol"])
+            check_type(argname="argument certificates", value=certificates, expected_type=type_hints["certificates"])
+            check_type(argname="argument client_affinity", value=client_affinity, expected_type=type_hints["client_affinity"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument proxy_protocol", value=proxy_protocol, expected_type=type_hints["proxy_protocol"])
+            check_type(argname="argument security_policy_id", value=security_policy_id, expected_type=type_hints["security_policy_id"])
+            check_type(argname="argument x_forwarded_for_config", value=x_forwarded_for_config, expected_type=type_hints["x_forwarded_for_config"])
         self._values: typing.Dict[str, typing.Any] = {
             "accelerator_id": accelerator_id,
             "port_ranges": port_ranges,
             "protocol": protocol,
         }
         if certificates is not None:
             self._values["certificates"] = certificates
```

### Comparing `ros-cdk-ga-1.0.8/src/ros_cdk_ga.egg-info/PKG-INFO` & `ros-cdk-ga-1.0.9/src/ros_cdk_ga.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-ga
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS GA Construct Library
```

