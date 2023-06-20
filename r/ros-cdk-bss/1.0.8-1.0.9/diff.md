# Comparing `tmp/ros-cdk-bss-1.0.8.tar.gz` & `tmp/ros-cdk-bss-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-bss-1.0.8.tar", last modified: Thu Jul 14 02:34:36 2022, max compression
+gzip compressed data, was "dist/ros-cdk-bss-1.0.9.tar", last modified: Fri Sep 23 11:51:34 2022, max compression
```

## Comparing `ros-cdk-bss-1.0.8.tar` & `ros-cdk-bss-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:34:36.000000 ros-cdk-bss-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:34:36.000000 ros-cdk-bss-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:34:36.000000 ros-cdk-bss-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:34:36.000000 ros-cdk-bss-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:34:36.000000 ros-cdk-bss-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      179 2022-07-14 02:34:36.000000 ros-cdk-bss-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:34:36.000000 ros-cdk-bss-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:34:36.000000 ros-cdk-bss-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1794 2022-07-14 02:34:36.000000 ros-cdk-bss-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:34:36.000000 ros-cdk-bss-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:34:36.000000 ros-cdk-bss-1.0.8/src/ros_cdk_bss/
--rw-r--r--   0 root         (0) root         (0)    32324 2022-07-14 02:34:36.000000 ros-cdk-bss-1.0.8/src/ros_cdk_bss/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:34:36.000000 ros-cdk-bss-1.0.8/src/ros_cdk_bss/_jsii/
--rw-r--r--   0 root         (0) root         (0)      370 2022-07-14 02:34:36.000000 ros-cdk-bss-1.0.8/src/ros_cdk_bss/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35863 2022-07-14 02:34:36.000000 ros-cdk-bss-1.0.8/src/ros_cdk_bss/_jsii/ros-cdk-bss@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:34:36.000000 ros-cdk-bss-1.0.8/src/ros_cdk_bss/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:34:36.000000 ros-cdk-bss-1.0.8/src/ros_cdk_bss.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:34:36.000000 ros-cdk-bss-1.0.8/src/ros_cdk_bss.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      400 2022-07-14 02:34:36.000000 ros-cdk-bss-1.0.8/src/ros_cdk_bss.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:34:36.000000 ros-cdk-bss-1.0.8/src/ros_cdk_bss.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:34:36.000000 ros-cdk-bss-1.0.8/src/ros_cdk_bss.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-07-14 02:34:36.000000 ros-cdk-bss-1.0.8/src/ros_cdk_bss.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:51:34.000000 ros-cdk-bss-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 11:51:34.000000 ros-cdk-bss-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 11:51:34.000000 ros-cdk-bss-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 11:51:34.000000 ros-cdk-bss-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 11:51:34.000000 ros-cdk-bss-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      179 2022-09-23 11:51:34.000000 ros-cdk-bss-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 11:51:34.000000 ros-cdk-bss-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 11:51:34.000000 ros-cdk-bss-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1823 2022-09-23 11:51:34.000000 ros-cdk-bss-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:51:34.000000 ros-cdk-bss-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:51:34.000000 ros-cdk-bss-1.0.9/src/ros_cdk_bss/
+-rw-r--r--   0 root         (0) root         (0)    39789 2022-09-23 11:51:34.000000 ros-cdk-bss-1.0.9/src/ros_cdk_bss/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:51:34.000000 ros-cdk-bss-1.0.9/src/ros_cdk_bss/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      404 2022-09-23 11:51:34.000000 ros-cdk-bss-1.0.9/src/ros_cdk_bss/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35936 2022-09-23 11:51:34.000000 ros-cdk-bss-1.0.9/src/ros_cdk_bss/_jsii/ros-cdk-bss@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:51:34.000000 ros-cdk-bss-1.0.9/src/ros_cdk_bss/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:51:34.000000 ros-cdk-bss-1.0.9/src/ros_cdk_bss.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 11:51:34.000000 ros-cdk-bss-1.0.9/src/ros_cdk_bss.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      400 2022-09-23 11:51:34.000000 ros-cdk-bss-1.0.9/src/ros_cdk_bss.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:51:34.000000 ros-cdk-bss-1.0.9/src/ros_cdk_bss.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 11:51:34.000000 ros-cdk-bss-1.0.9/src/ros_cdk_bss.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-09-23 11:51:34.000000 ros-cdk-bss-1.0.9/src/ros_cdk_bss.egg-info/top_level.txt
```

### Comparing `ros-cdk-bss-1.0.8/LICENSE` & `ros-cdk-bss-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-bss-1.0.8/PKG-INFO` & `ros-cdk-bss-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-bss
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS BSS Construct Library
```

### Comparing `ros-cdk-bss-1.0.8/setup.py` & `ros-cdk-bss-1.0.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-bss",
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
         "ros_cdk_bss",
         "ros_cdk_bss._jsii"
     ],
     "package_data": {
         "ros_cdk_bss._jsii": [
-            "ros-cdk-bss@1.0.8.jsii.tgz"
+            "ros-cdk-bss@1.0.9.jsii.tgz"
         ],
         "ros_cdk_bss": [
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

### Comparing `ros-cdk-bss-1.0.8/src/ros_cdk_bss/__init__.py` & `ros-cdk-bss-1.0.9/src/ros_cdk_bss/__init__.py`

 * *Files 15% similar despite different names*

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
 
 
 class ResourcePackage(
     ros_cdk_core.Resource,
@@ -29,37 +31,43 @@
 ):
     '''A ROS resource type:  ``ALIYUN::BSS::ResourcePackage``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "ResourcePackageProps",
+        props: typing.Union["ResourcePackageProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::BSS::ResourcePackage``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ResourcePackage.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceId")
     def attr_instance_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute InstanceId: The ID of the specified instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrOrderId")
     def attr_order_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute OrderId: The ID of the specified order.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrOrderId"))
 
 
 @jsii.data_type(
@@ -90,14 +98,22 @@
         :param duration: Property duration: The validity of the specified resource package. The value is the same as the Value of AvailableDuration returned by DescribeResourcePackageProduct.
         :param package_type: Property packageType: The type of the specified resource package. The value is the same as the value of the Code value of the ResourcePackage object returned by DescribeResourcePackageProduct.
         :param product_code: Property productCode: The code of the specified product. The value is the same as the value of ProductType returned by QueryProductList.
         :param specification: Property specification: The size of the specified resource package. The value is the same as the Value of Specification returned by DescribeResourcePackageProduct.
         :param effective_date: Property effectiveDate: The effective date of the specified resource package. The resource package will take effect immediately if the effective date is unspecified. The date format follows the ISO8601 standard and uses UTC time. Format: yyyy-MM-ddTHH:mm:ssZ
         :param pricing_cycle: Property pricingCycle: The validity of the specified resource package. Default value: Month. Valid values: Month, Year
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ResourcePackageProps.__init__)
+            check_type(argname="argument duration", value=duration, expected_type=type_hints["duration"])
+            check_type(argname="argument package_type", value=package_type, expected_type=type_hints["package_type"])
+            check_type(argname="argument product_code", value=product_code, expected_type=type_hints["product_code"])
+            check_type(argname="argument specification", value=specification, expected_type=type_hints["specification"])
+            check_type(argname="argument effective_date", value=effective_date, expected_type=type_hints["effective_date"])
+            check_type(argname="argument pricing_cycle", value=pricing_cycle, expected_type=type_hints["pricing_cycle"])
         self._values: typing.Dict[str, typing.Any] = {
             "duration": duration,
             "package_type": package_type,
             "product_code": product_code,
             "specification": specification,
         }
         if effective_date is not None:
@@ -186,164 +202,194 @@
 ):
     '''A ROS template type:  ``ALIYUN::BSS::ResourcePackage``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosResourcePackageProps",
+        props: typing.Union["RosResourcePackageProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::BSS::ResourcePackage``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosResourcePackage.__init__)
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
+            type_hints = typing.get_type_hints(RosResourcePackage._render_properties)
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
         :Attribute: InstanceId: The ID of the specified instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrOrderId")
     def attr_order_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: OrderId: The ID of the specified order.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrOrderId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="duration")
     def duration(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property: duration: The validity of the specified resource package. The value is the same as the Value of AvailableDuration returned by DescribeResourcePackageProduct.
         '''
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "duration"))
 
     @duration.setter
     def duration(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosResourcePackage, "duration").fset)
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
+            type_hints = typing.get_type_hints(getattr(RosResourcePackage, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="packageType")
     def package_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: packageType: The type of the specified resource package. The value is the same as the value of the Code value of the ResourcePackage object returned by DescribeResourcePackageProduct.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "packageType"))
 
     @package_type.setter
     def package_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosResourcePackage, "package_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "packageType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="productCode")
     def product_code(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: productCode: The code of the specified product. The value is the same as the value of ProductType returned by QueryProductList.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "productCode"))
 
     @product_code.setter
     def product_code(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosResourcePackage, "product_code").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "productCode", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="specification")
     def specification(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: specification: The size of the specified resource package. The value is the same as the Value of Specification returned by DescribeResourcePackageProduct.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "specification"))
 
     @specification.setter
     def specification(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosResourcePackage, "specification").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "specification", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="effectiveDate")
     def effective_date(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: effectiveDate: The effective date of the specified resource package. The resource package will take effect immediately if the effective date is unspecified. The date format follows the ISO8601 standard and uses UTC time. Format: yyyy-MM-ddTHH:mm:ssZ
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "effectiveDate"))
 
     @effective_date.setter
     def effective_date(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosResourcePackage, "effective_date").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "effectiveDate", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="pricingCycle")
     def pricing_cycle(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: pricingCycle: The validity of the specified resource package. Default value: Month. Valid values: Month, Year
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "pricingCycle"))
 
     @pricing_cycle.setter
     def pricing_cycle(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosResourcePackage, "pricing_cycle").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "pricingCycle", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-bss.RosResourcePackageProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -371,14 +417,22 @@
         :param duration: 
         :param package_type: 
         :param product_code: 
         :param specification: 
         :param effective_date: 
         :param pricing_cycle: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosResourcePackageProps.__init__)
+            check_type(argname="argument duration", value=duration, expected_type=type_hints["duration"])
+            check_type(argname="argument package_type", value=package_type, expected_type=type_hints["package_type"])
+            check_type(argname="argument product_code", value=product_code, expected_type=type_hints["product_code"])
+            check_type(argname="argument specification", value=specification, expected_type=type_hints["specification"])
+            check_type(argname="argument effective_date", value=effective_date, expected_type=type_hints["effective_date"])
+            check_type(argname="argument pricing_cycle", value=pricing_cycle, expected_type=type_hints["pricing_cycle"])
         self._values: typing.Dict[str, typing.Any] = {
             "duration": duration,
             "package_type": package_type,
             "product_code": product_code,
             "specification": specification,
         }
         if effective_date is not None:
@@ -461,92 +515,110 @@
 ):
     '''A ROS template type:  ``ALIYUN::BSS::WaitOrder``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosWaitOrderProps",
+        props: typing.Union["RosWaitOrderProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::BSS::WaitOrder``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosWaitOrder.__init__)
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
+            type_hints = typing.get_type_hints(RosWaitOrder._render_properties)
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
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         '''A factory method that creates a new instance of this class from an object containing the properties of this ROS resource.'''
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosWaitOrder, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="orderIds")
     def order_ids(
         self,
     ) -> typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]:
         '''
         :Property: orderIds: A list of order ids.
         '''
         return typing.cast(typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable], jsii.get(self, "orderIds"))
 
     @order_ids.setter
     def order_ids(
         self,
         value: typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosWaitOrder, "order_ids").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "orderIds", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="cancelOnDelete")
     def cancel_on_delete(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: cancelOnDelete: Cancel order where delete the resource. Ignore the paid order. Default true
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "cancelOnDelete"))
 
     @cancel_on_delete.setter
     def cancel_on_delete(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosWaitOrder, "cancel_on_delete").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "cancelOnDelete", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="waitForOrderProduced")
     def wait_for_order_produced(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -556,14 +628,17 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "waitForOrderProduced"))
 
     @wait_for_order_produced.setter
     def wait_for_order_produced(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosWaitOrder, "wait_for_order_produced").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "waitForOrderProduced", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-bss.RosWaitOrderProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -582,14 +657,19 @@
     ) -> None:
         '''Properties for defining a ``ALIYUN::BSS::WaitOrder``.
 
         :param order_ids: 
         :param cancel_on_delete: 
         :param wait_for_order_produced: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosWaitOrderProps.__init__)
+            check_type(argname="argument order_ids", value=order_ids, expected_type=type_hints["order_ids"])
+            check_type(argname="argument cancel_on_delete", value=cancel_on_delete, expected_type=type_hints["cancel_on_delete"])
+            check_type(argname="argument wait_for_order_produced", value=wait_for_order_produced, expected_type=type_hints["wait_for_order_produced"])
         self._values: typing.Dict[str, typing.Any] = {
             "order_ids": order_ids,
         }
         if cancel_on_delete is not None:
             self._values["cancel_on_delete"] = cancel_on_delete
         if wait_for_order_produced is not None:
             self._values["wait_for_order_produced"] = wait_for_order_produced
@@ -647,28 +727,34 @@
 ):
     '''A ROS resource type:  ``ALIYUN::BSS::WaitOrder``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "WaitOrderProps",
+        props: typing.Union["WaitOrderProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::BSS::WaitOrder``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(WaitOrder.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-bss.WaitOrderProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -687,14 +773,19 @@
     ) -> None:
         '''Properties for defining a ``ALIYUN::BSS::WaitOrder``.
 
         :param order_ids: Property orderIds: A list of order ids.
         :param cancel_on_delete: Property cancelOnDelete: Cancel order where delete the resource. Ignore the paid order. Default true
         :param wait_for_order_produced: Property waitForOrderProduced: Wait util all orders related ROS resources are produced. Support ALIYUN::ECS::PrepayInstance, ALIYUN::RDS::PrepayDBInstance, ALIYUN::REDIS::PrepayInstance, ALIYUN::SLB::LoadBalancer, ALIYUN::VPC::EIP, ALIYUN::VPC::VpnGateway.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(WaitOrderProps.__init__)
+            check_type(argname="argument order_ids", value=order_ids, expected_type=type_hints["order_ids"])
+            check_type(argname="argument cancel_on_delete", value=cancel_on_delete, expected_type=type_hints["cancel_on_delete"])
+            check_type(argname="argument wait_for_order_produced", value=wait_for_order_produced, expected_type=type_hints["wait_for_order_produced"])
         self._values: typing.Dict[str, typing.Any] = {
             "order_ids": order_ids,
         }
         if cancel_on_delete is not None:
             self._values["cancel_on_delete"] = cancel_on_delete
         if wait_for_order_produced is not None:
             self._values["wait_for_order_produced"] = wait_for_order_produced
```

### Comparing `ros-cdk-bss-1.0.8/src/ros_cdk_bss.egg-info/PKG-INFO` & `ros-cdk-bss-1.0.9/src/ros_cdk_bss.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-bss
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS BSS Construct Library
```

