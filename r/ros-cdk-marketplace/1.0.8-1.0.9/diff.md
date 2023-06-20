# Comparing `tmp/ros-cdk-marketplace-1.0.8.tar.gz` & `tmp/ros-cdk-marketplace-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-marketplace-1.0.8.tar", last modified: Thu Jul 14 02:38:25 2022, max compression
+gzip compressed data, was "dist/ros-cdk-marketplace-1.0.9.tar", last modified: Fri Sep 23 11:27:53 2022, max compression
```

## Comparing `ros-cdk-marketplace-1.0.8.tar` & `ros-cdk-marketplace-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:38:25.000000 ros-cdk-marketplace-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:38:25.000000 ros-cdk-marketplace-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:38:25.000000 ros-cdk-marketplace-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:38:25.000000 ros-cdk-marketplace-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1272 2022-07-14 02:38:25.000000 ros-cdk-marketplace-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      203 2022-07-14 02:38:25.000000 ros-cdk-marketplace-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:38:25.000000 ros-cdk-marketplace-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:38:25.000000 ros-cdk-marketplace-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1842 2022-07-14 02:38:25.000000 ros-cdk-marketplace-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:38:25.000000 ros-cdk-marketplace-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:38:25.000000 ros-cdk-marketplace-1.0.8/src/ros_cdk_marketplace/
--rw-r--r--   0 root         (0) root         (0)    19587 2022-07-14 02:38:25.000000 ros-cdk-marketplace-1.0.8/src/ros_cdk_marketplace/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:38:25.000000 ros-cdk-marketplace-1.0.8/src/ros_cdk_marketplace/_jsii/
--rw-r--r--   0 root         (0) root         (0)      399 2022-07-14 02:38:25.000000 ros-cdk-marketplace-1.0.8/src/ros_cdk_marketplace/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31306 2022-07-14 02:38:25.000000 ros-cdk-marketplace-1.0.8/src/ros_cdk_marketplace/_jsii/ros-cdk-marketplace@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:38:25.000000 ros-cdk-marketplace-1.0.8/src/ros_cdk_marketplace/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:38:25.000000 ros-cdk-marketplace-1.0.8/src/ros_cdk_marketplace.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1272 2022-07-14 02:38:25.000000 ros-cdk-marketplace-1.0.8/src/ros_cdk_marketplace.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      480 2022-07-14 02:38:25.000000 ros-cdk-marketplace-1.0.8/src/ros_cdk_marketplace.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:38:25.000000 ros-cdk-marketplace-1.0.8/src/ros_cdk_marketplace.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:38:25.000000 ros-cdk-marketplace-1.0.8/src/ros_cdk_marketplace.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2022-07-14 02:38:25.000000 ros-cdk-marketplace-1.0.8/src/ros_cdk_marketplace.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:27:53.000000 ros-cdk-marketplace-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 11:27:52.000000 ros-cdk-marketplace-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 11:27:52.000000 ros-cdk-marketplace-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 11:27:52.000000 ros-cdk-marketplace-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1272 2022-09-23 11:27:53.000000 ros-cdk-marketplace-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      203 2022-09-23 11:27:52.000000 ros-cdk-marketplace-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 11:27:52.000000 ros-cdk-marketplace-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 11:27:53.000000 ros-cdk-marketplace-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1871 2022-09-23 11:27:52.000000 ros-cdk-marketplace-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:27:53.000000 ros-cdk-marketplace-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:27:53.000000 ros-cdk-marketplace-1.0.9/src/ros_cdk_marketplace/
+-rw-r--r--   0 root         (0) root         (0)    24171 2022-09-23 11:27:52.000000 ros-cdk-marketplace-1.0.9/src/ros_cdk_marketplace/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:27:53.000000 ros-cdk-marketplace-1.0.9/src/ros_cdk_marketplace/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      433 2022-09-23 11:27:52.000000 ros-cdk-marketplace-1.0.9/src/ros_cdk_marketplace/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31366 2022-09-23 11:27:52.000000 ros-cdk-marketplace-1.0.9/src/ros_cdk_marketplace/_jsii/ros-cdk-marketplace@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:27:52.000000 ros-cdk-marketplace-1.0.9/src/ros_cdk_marketplace/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:27:53.000000 ros-cdk-marketplace-1.0.9/src/ros_cdk_marketplace.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1272 2022-09-23 11:27:53.000000 ros-cdk-marketplace-1.0.9/src/ros_cdk_marketplace.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      480 2022-09-23 11:27:53.000000 ros-cdk-marketplace-1.0.9/src/ros_cdk_marketplace.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:27:53.000000 ros-cdk-marketplace-1.0.9/src/ros_cdk_marketplace.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 11:27:53.000000 ros-cdk-marketplace-1.0.9/src/ros_cdk_marketplace.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2022-09-23 11:27:53.000000 ros-cdk-marketplace-1.0.9/src/ros_cdk_marketplace.egg-info/top_level.txt
```

### Comparing `ros-cdk-marketplace-1.0.8/LICENSE` & `ros-cdk-marketplace-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-marketplace-1.0.8/PKG-INFO` & `ros-cdk-marketplace-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-marketplace
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS MARKETPLACE Construct Library
```

### Comparing `ros-cdk-marketplace-1.0.8/setup.py` & `ros-cdk-marketplace-1.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-marketplace",
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
         "ros_cdk_marketplace",
         "ros_cdk_marketplace._jsii"
     ],
     "package_data": {
         "ros_cdk_marketplace._jsii": [
-            "ros-cdk-marketplace@1.0.8.jsii.tgz"
+            "ros-cdk-marketplace@1.0.9.jsii.tgz"
         ],
         "ros_cdk_marketplace": [
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

### Comparing `ros-cdk-marketplace-1.0.8/src/ros_cdk_marketplace/__init__.py` & `ros-cdk-marketplace-1.0.9/src/ros_cdk_marketplace/__init__.py`

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
 
 
 class Order(
     ros_cdk_core.Resource,
@@ -29,31 +31,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::MarketPlace::Order``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "OrderProps",
+        props: typing.Union["OrderProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::MarketPlace::Order``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Order.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrOrderId")
     def attr_order_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute OrderId: Order ID of created instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrOrderId"))
 
 
 @jsii.data_type(
@@ -87,14 +95,23 @@
         :param sku_code: Property skuCode: Sku code for the resource.
         :param charge_type: Property chargeType: The resource charge type. Default value is Prepaid
         :param duration: Property duration: Duration of the resource. If ChargeType is specified as Postpaid, this value will be ignore.
         :param preference: Property preference: Customized parameters.
         :param pricing_cycle: Property pricingCycle: Price cycle of the resource. This property has no default value. If ChargeType is specified as Postpaid, this value will be ignore.
         :param quantity: Property quantity: Resource number. Default value is 1
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(OrderProps.__init__)
+            check_type(argname="argument product_code", value=product_code, expected_type=type_hints["product_code"])
+            check_type(argname="argument sku_code", value=sku_code, expected_type=type_hints["sku_code"])
+            check_type(argname="argument charge_type", value=charge_type, expected_type=type_hints["charge_type"])
+            check_type(argname="argument duration", value=duration, expected_type=type_hints["duration"])
+            check_type(argname="argument preference", value=preference, expected_type=type_hints["preference"])
+            check_type(argname="argument pricing_cycle", value=pricing_cycle, expected_type=type_hints["pricing_cycle"])
+            check_type(argname="argument quantity", value=quantity, expected_type=type_hints["quantity"])
         self._values: typing.Dict[str, typing.Any] = {
             "product_code": product_code,
             "sku_code": sku_code,
         }
         if charge_type is not None:
             self._values["charge_type"] = charge_type
         if duration is not None:
@@ -191,177 +208,210 @@
 ):
     '''A ROS template type:  ``ALIYUN::MarketPlace::Order``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosOrderProps",
+        props: typing.Union["RosOrderProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::MarketPlace::Order``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosOrder.__init__)
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
+            type_hints = typing.get_type_hints(RosOrder._render_properties)
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
     @jsii.member(jsii_name="attrOrderId")
     def attr_order_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: OrderId: Order ID of created instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrOrderId"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosOrder, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="productCode")
     def product_code(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: productCode: Product code for the resource.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "productCode"))
 
     @product_code.setter
     def product_code(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosOrder, "product_code").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "productCode", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="skuCode")
     def sku_code(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: skuCode: Sku code for the resource.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "skuCode"))
 
     @sku_code.setter
     def sku_code(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosOrder, "sku_code").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "skuCode", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="chargeType")
     def charge_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: chargeType: The resource charge type. Default value is Prepaid
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "chargeType"))
 
     @charge_type.setter
     def charge_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosOrder, "charge_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "chargeType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="duration")
     def duration(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: duration: Duration of the resource. If ChargeType is specified as Postpaid, this value will be ignore.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "duration"))
 
     @duration.setter
     def duration(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosOrder, "duration").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "duration", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="preference")
     def preference(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]]:
         '''
         :Property: preference: Customized parameters.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]], jsii.get(self, "preference"))
 
     @preference.setter
     def preference(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosOrder, "preference").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "preference", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="pricingCycle")
     def pricing_cycle(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: pricingCycle: Price cycle of the resource. This property has no default value. If ChargeType is specified as Postpaid, this value will be ignore.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "pricingCycle"))
 
     @pricing_cycle.setter
     def pricing_cycle(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosOrder, "pricing_cycle").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "pricingCycle", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="quantity")
     def quantity(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: quantity: Resource number. Default value is 1
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "quantity"))
 
     @quantity.setter
     def quantity(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosOrder, "quantity").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "quantity", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-marketplace.RosOrderProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -392,14 +442,23 @@
         :param sku_code: 
         :param charge_type: 
         :param duration: 
         :param preference: 
         :param pricing_cycle: 
         :param quantity: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosOrderProps.__init__)
+            check_type(argname="argument product_code", value=product_code, expected_type=type_hints["product_code"])
+            check_type(argname="argument sku_code", value=sku_code, expected_type=type_hints["sku_code"])
+            check_type(argname="argument charge_type", value=charge_type, expected_type=type_hints["charge_type"])
+            check_type(argname="argument duration", value=duration, expected_type=type_hints["duration"])
+            check_type(argname="argument preference", value=preference, expected_type=type_hints["preference"])
+            check_type(argname="argument pricing_cycle", value=pricing_cycle, expected_type=type_hints["pricing_cycle"])
+            check_type(argname="argument quantity", value=quantity, expected_type=type_hints["quantity"])
         self._values: typing.Dict[str, typing.Any] = {
             "product_code": product_code,
             "sku_code": sku_code,
         }
         if charge_type is not None:
             self._values["charge_type"] = charge_type
         if duration is not None:
```

### Comparing `ros-cdk-marketplace-1.0.8/src/ros_cdk_marketplace.egg-info/PKG-INFO` & `ros-cdk-marketplace-1.0.9/src/ros_cdk_marketplace.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-marketplace
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS MARKETPLACE Construct Library
```

