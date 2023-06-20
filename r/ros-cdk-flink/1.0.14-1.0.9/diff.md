# Comparing `tmp/ros-cdk-flink-1.0.14.tar.gz` & `tmp/ros-cdk-flink-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-flink-1.0.14.tar", last modified: Tue Jun 20 02:54:16 2023, max compression
+gzip compressed data, was "dist/ros-cdk-flink-1.0.9.tar", last modified: Fri Sep 23 12:30:37 2022, max compression
```

## Comparing `ros-cdk-flink-1.0.14.tar` & `ros-cdk-flink-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:54:16.000000 ros-cdk-flink-1.0.14/
--rw-r--r--   0 root         (0) root         (0)    10279 2023-06-20 02:54:16.000000 ros-cdk-flink-1.0.14/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-20 02:54:16.000000 ros-cdk-flink-1.0.14/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2023-06-20 02:54:16.000000 ros-cdk-flink-1.0.14/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1300 2023-06-20 02:54:16.000000 ros-cdk-flink-1.0.14/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      185 2023-06-20 02:54:16.000000 ros-cdk-flink-1.0.14/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-06-20 02:54:16.000000 ros-cdk-flink-1.0.14/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-20 02:54:16.000000 ros-cdk-flink-1.0.14/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1887 2023-06-20 02:54:16.000000 ros-cdk-flink-1.0.14/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:54:16.000000 ros-cdk-flink-1.0.14/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:54:16.000000 ros-cdk-flink-1.0.14/src/ros_cdk_flink/
--rw-r--r--   0 root         (0) root         (0)    71072 2023-06-20 02:54:16.000000 ros-cdk-flink-1.0.14/src/ros_cdk_flink/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:54:16.000000 ros-cdk-flink-1.0.14/src/ros_cdk_flink/_jsii/
--rw-r--r--   0 root         (0) root         (0)      423 2023-06-20 02:54:16.000000 ros-cdk-flink-1.0.14/src/ros_cdk_flink/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    40367 2023-06-20 02:54:16.000000 ros-cdk-flink-1.0.14/src/ros_cdk_flink/_jsii/ros-cdk-flink@1.0.14.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 02:54:16.000000 ros-cdk-flink-1.0.14/src/ros_cdk_flink/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:54:16.000000 ros-cdk-flink-1.0.14/src/ros_cdk_flink.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1300 2023-06-20 02:54:16.000000 ros-cdk-flink-1.0.14/src/ros_cdk_flink.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      421 2023-06-20 02:54:16.000000 ros-cdk-flink-1.0.14/src/ros_cdk_flink.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 02:54:16.000000 ros-cdk-flink-1.0.14/src/ros_cdk_flink.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      109 2023-06-20 02:54:16.000000 ros-cdk-flink-1.0.14/src/ros_cdk_flink.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-20 02:54:16.000000 ros-cdk-flink-1.0.14/src/ros_cdk_flink.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:30:37.000000 ros-cdk-flink-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 12:30:36.000000 ros-cdk-flink-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 12:30:36.000000 ros-cdk-flink-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 12:30:36.000000 ros-cdk-flink-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1248 2022-09-23 12:30:37.000000 ros-cdk-flink-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      185 2022-09-23 12:30:36.000000 ros-cdk-flink-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 12:30:36.000000 ros-cdk-flink-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 12:30:37.000000 ros-cdk-flink-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1835 2022-09-23 12:30:36.000000 ros-cdk-flink-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:30:37.000000 ros-cdk-flink-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:30:37.000000 ros-cdk-flink-1.0.9/src/ros_cdk_flink/
+-rw-r--r--   0 root         (0) root         (0)    57763 2022-09-23 12:30:36.000000 ros-cdk-flink-1.0.9/src/ros_cdk_flink/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:30:37.000000 ros-cdk-flink-1.0.9/src/ros_cdk_flink/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      408 2022-09-23 12:30:36.000000 ros-cdk-flink-1.0.9/src/ros_cdk_flink/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    40616 2022-09-23 12:30:36.000000 ros-cdk-flink-1.0.9/src/ros_cdk_flink/_jsii/ros-cdk-flink@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 12:30:36.000000 ros-cdk-flink-1.0.9/src/ros_cdk_flink/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:30:37.000000 ros-cdk-flink-1.0.9/src/ros_cdk_flink.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1248 2022-09-23 12:30:37.000000 ros-cdk-flink-1.0.9/src/ros_cdk_flink.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2022-09-23 12:30:37.000000 ros-cdk-flink-1.0.9/src/ros_cdk_flink.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 12:30:37.000000 ros-cdk-flink-1.0.9/src/ros_cdk_flink.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 12:30:37.000000 ros-cdk-flink-1.0.9/src/ros_cdk_flink.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2022-09-23 12:30:37.000000 ros-cdk-flink-1.0.9/src/ros_cdk_flink.egg-info/top_level.txt
```

### Comparing `ros-cdk-flink-1.0.14/LICENSE` & `ros-cdk-flink-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-flink-1.0.14/PKG-INFO` & `ros-cdk-flink-1.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-flink
-Version: 1.0.14
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS FLINK Construct Library
         
@@ -19,13 +19,12 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
```

### Comparing `ros-cdk-flink-1.0.14/setup.py` & `ros-cdk-flink-1.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-flink",
-    "version": "1.0.14",
+    "version": "1.0.9",
     "description": "Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com",
     "license": "Apache-2.0",
     "url": "https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git",
     "long_description_content_type": "text/markdown",
     "author": "ROS Development Team",
     "bdist_wheel": {
         "universal": true
@@ -22,38 +22,37 @@
     },
     "packages": [
         "ros_cdk_flink",
         "ros_cdk_flink._jsii"
     ],
     "package_data": {
         "ros_cdk_flink._jsii": [
-            "ros-cdk-flink@1.0.14.jsii.tgz"
+            "ros-cdk-flink@1.0.9.jsii.tgz"
         ],
         "ros_cdk_flink": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "constructs>=3.0.4, <4.0.0",
-        "jsii>=1.84.0, <2.0.0",
+        "jsii>=1.68.0, <2.0.0",
         "publication>=0.0.3",
         "ros-cdk-core>=1.0.6, <2.0.0",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "License :: OSI Approved",
         "Programming Language :: Python :: 3"
     ],
     "scripts": []
 }
 """
```

### Comparing `ros-cdk-flink-1.0.14/src/ros_cdk_flink/__init__.py` & `ros-cdk-flink-1.0.9/src/ros_cdk_flink/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,61 +17,61 @@
 import publication
 import typing_extensions
 
 from typeguard import check_type
 
 from ._jsii import *
 
-import ros_cdk_core as _ros_cdk_core_7adfd82f
+import ros_cdk_core
 
 
 class Instance(
-    _ros_cdk_core_7adfd82f.Resource,
+    ros_cdk_core.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-flink.Instance",
 ):
     '''A ROS resource type:  ``ALIYUN::Flink::Instance``.'''
 
     def __init__(
         self,
-        scope: _ros_cdk_core_7adfd82f.Construct,
+        scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: typing.Union["InstanceProps", typing.Dict[builtins.str, typing.Any]],
+        props: typing.Union["InstanceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::Flink::Instance``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__7ac06ec3a5b462ac2e1cc27879335e2b5a2554adaed27232209ad964bf56332b)
+            type_hints = typing.get_type_hints(Instance.__init__)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
             check_type(argname="argument props", value=props, expected_type=type_hints["props"])
             check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
     @builtins.property
     @jsii.member(jsii_name="attrInstanceId")
-    def attr_instance_id(self) -> _ros_cdk_core_7adfd82f.IResolvable:
+    def attr_instance_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute InstanceId: Instance ID.'''
-        return typing.cast(_ros_cdk_core_7adfd82f.IResolvable, jsii.get(self, "attrInstanceId"))
+        return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceId"))
 
     @builtins.property
     @jsii.member(jsii_name="attrOrderId")
-    def attr_order_id(self) -> _ros_cdk_core_7adfd82f.IResolvable:
+    def attr_order_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute OrderId: Order information.'''
-        return typing.cast(_ros_cdk_core_7adfd82f.IResolvable, jsii.get(self, "attrOrderId"))
+        return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrOrderId"))
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-flink.InstanceProps",
     jsii_struct_bases=[],
     name_mapping={
         "bucket": "bucket",
@@ -88,26 +88,26 @@
         "use_promotion_code": "usePromotionCode",
     },
 )
 class InstanceProps:
     def __init__(
         self,
         *,
-        bucket: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
-        charge_type: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
-        instance_name: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
-        vpc_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
-        v_switch_ids: typing.Union[typing.Sequence[typing.Any], _ros_cdk_core_7adfd82f.IResolvable],
-        zone_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
-        auto_renew: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-        duration: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-        pricing_cycle: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-        promotion_code: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-        resource_spec: typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Union["RosInstance.ResourceSpecProperty", typing.Dict[builtins.str, typing.Any]]]] = None,
-        use_promotion_code: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+        bucket: typing.Union[builtins.str, ros_cdk_core.IResolvable],
+        charge_type: typing.Union[builtins.str, ros_cdk_core.IResolvable],
+        instance_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
+        vpc_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
+        v_switch_ids: typing.Union[typing.Sequence[typing.Any], ros_cdk_core.IResolvable],
+        zone_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
+        auto_renew: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
+        duration: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
+        pricing_cycle: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
+        promotion_code: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
+        resource_spec: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosInstance.ResourceSpecProperty", typing.Dict[str, typing.Any]]]] = None,
+        use_promotion_code: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::Flink::Instance``.
 
         :param bucket: Property bucket: OSS bucket name.
         :param charge_type: Property chargeType: The payment type, the value of the value is as follows: POST: pay as you go. PRE: subscription.
         :param instance_name: Property instanceName: The name of instance.
         :param vpc_id: Property vpcId: VPC ID.
@@ -117,28 +117,28 @@
         :param duration: Property duration: Number of order cycle. When ChargeType is configured as PRE, the duration parameter must be filled. If PricingCycle is Month, the valid range is 1, 2, 3, 6, 7, 8, 9, 12, 24, 36 If PricingCycle is year, the valid range is 1 to 3
         :param pricing_cycle: Property pricingCycle: The ordering cycle only supports ordering in the year and month.
         :param promotion_code: Property promotionCode: Promo Code.
         :param resource_spec: Property resourceSpec: Resource specifications. When ChargeType is configured as PRE, the resource specification parameters must be filled.
         :param use_promotion_code: Property usePromotionCode: Whether to use coupons.The value is as follows: true: Use. false: Not in use.
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__92f8fcd41ef922ea4bbdd21e7b570a2ba79e56738c3c1a4f4e819b0369bd1198)
+            type_hints = typing.get_type_hints(InstanceProps.__init__)
             check_type(argname="argument bucket", value=bucket, expected_type=type_hints["bucket"])
             check_type(argname="argument charge_type", value=charge_type, expected_type=type_hints["charge_type"])
             check_type(argname="argument instance_name", value=instance_name, expected_type=type_hints["instance_name"])
             check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
             check_type(argname="argument v_switch_ids", value=v_switch_ids, expected_type=type_hints["v_switch_ids"])
             check_type(argname="argument zone_id", value=zone_id, expected_type=type_hints["zone_id"])
             check_type(argname="argument auto_renew", value=auto_renew, expected_type=type_hints["auto_renew"])
             check_type(argname="argument duration", value=duration, expected_type=type_hints["duration"])
             check_type(argname="argument pricing_cycle", value=pricing_cycle, expected_type=type_hints["pricing_cycle"])
             check_type(argname="argument promotion_code", value=promotion_code, expected_type=type_hints["promotion_code"])
             check_type(argname="argument resource_spec", value=resource_spec, expected_type=type_hints["resource_spec"])
             check_type(argname="argument use_promotion_code", value=use_promotion_code, expected_type=type_hints["use_promotion_code"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "bucket": bucket,
             "charge_type": charge_type,
             "instance_name": instance_name,
             "vpc_id": vpc_id,
             "v_switch_ids": v_switch_ids,
             "zone_id": zone_id,
         }
@@ -152,179 +152,175 @@
             self._values["promotion_code"] = promotion_code
         if resource_spec is not None:
             self._values["resource_spec"] = resource_spec
         if use_promotion_code is not None:
             self._values["use_promotion_code"] = use_promotion_code
 
     @builtins.property
-    def bucket(self) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+    def bucket(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''Property bucket: OSS bucket name.'''
         result = self._values.get("bucket")
         assert result is not None, "Required property 'bucket' is missing"
-        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+        return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
 
     @builtins.property
-    def charge_type(
-        self,
-    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+    def charge_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''Property chargeType: The payment type, the value of the value is as follows: POST: pay as you go.
 
         PRE: subscription.
         '''
         result = self._values.get("charge_type")
         assert result is not None, "Required property 'charge_type' is missing"
-        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+        return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
 
     @builtins.property
-    def instance_name(
-        self,
-    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+    def instance_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''Property instanceName: The name of instance.'''
         result = self._values.get("instance_name")
         assert result is not None, "Required property 'instance_name' is missing"
-        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+        return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
 
     @builtins.property
-    def vpc_id(self) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+    def vpc_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''Property vpcId: VPC ID.'''
         result = self._values.get("vpc_id")
         assert result is not None, "Required property 'vpc_id' is missing"
-        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+        return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
 
     @builtins.property
     def v_switch_ids(
         self,
-    ) -> typing.Union[typing.List[typing.Any], _ros_cdk_core_7adfd82f.IResolvable]:
+    ) -> typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]:
         '''Property vSwitchIds: Virtual switch ID.'''
         result = self._values.get("v_switch_ids")
         assert result is not None, "Required property 'v_switch_ids' is missing"
-        return typing.cast(typing.Union[typing.List[typing.Any], _ros_cdk_core_7adfd82f.IResolvable], result)
+        return typing.cast(typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable], result)
 
     @builtins.property
-    def zone_id(self) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+    def zone_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''Property zoneId: The available area ID of the instance.'''
         result = self._values.get("zone_id")
         assert result is not None, "Required property 'zone_id' is missing"
-        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+        return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
 
     @builtins.property
     def auto_renew(
         self,
-    ) -> typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''Property autoRenew: When the payment type is the monthly package, the value of the value is as follows: true: Automatic renewal.
 
         false: Manual renewal.
         '''
         result = self._values.get("auto_renew")
-        return typing.cast(typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]], result)
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def duration(
         self,
-    ) -> typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''Property duration: Number of order cycle.
 
         When ChargeType is configured as PRE, the duration parameter must be filled.
         If PricingCycle is Month, the valid range is 1, 2, 3, 6, 7, 8, 9, 12, 24, 36
         If PricingCycle is year, the valid range is 1 to 3
         '''
         result = self._values.get("duration")
-        return typing.cast(typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]], result)
+        return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def pricing_cycle(
         self,
-    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''Property pricingCycle: The ordering cycle only supports ordering in the year and month.'''
         result = self._values.get("pricing_cycle")
-        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def promotion_code(
         self,
-    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''Property promotionCode: Promo Code.'''
         result = self._values.get("promotion_code")
-        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def resource_spec(
         self,
-    ) -> typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, "RosInstance.ResourceSpecProperty"]]:
+    ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosInstance.ResourceSpecProperty"]]:
         '''Property resourceSpec: Resource specifications.
 
         When ChargeType is configured as PRE, the resource specification parameters must be filled.
         '''
         result = self._values.get("resource_spec")
-        return typing.cast(typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, "RosInstance.ResourceSpecProperty"]], result)
+        return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosInstance.ResourceSpecProperty"]], result)
 
     @builtins.property
     def use_promotion_code(
         self,
-    ) -> typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''Property usePromotionCode: Whether to use coupons.The value is as follows: true: Use. false: Not in use.'''
         result = self._values.get("use_promotion_code")
-        return typing.cast(typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]], result)
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
         return "InstanceProps(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 class Namespace(
-    _ros_cdk_core_7adfd82f.Resource,
+    ros_cdk_core.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-flink.Namespace",
 ):
     '''A ROS resource type:  ``ALIYUN::Flink::Namespace``.'''
 
     def __init__(
         self,
-        scope: _ros_cdk_core_7adfd82f.Construct,
+        scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: typing.Union["NamespaceProps", typing.Dict[builtins.str, typing.Any]],
+        props: typing.Union["NamespaceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::Flink::Namespace``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__f429333a5e22f08d25a6d8cee2f94a9afac4e7c85bdeec6706e8ae09fe8d4062)
+            type_hints = typing.get_type_hints(Namespace.__init__)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
             check_type(argname="argument props", value=props, expected_type=type_hints["props"])
             check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
     @builtins.property
     @jsii.member(jsii_name="attrInstanceId")
-    def attr_instance_id(self) -> _ros_cdk_core_7adfd82f.IResolvable:
+    def attr_instance_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute InstanceId: Instance ID.'''
-        return typing.cast(_ros_cdk_core_7adfd82f.IResolvable, jsii.get(self, "attrInstanceId"))
+        return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceId"))
 
     @builtins.property
     @jsii.member(jsii_name="attrNamespace")
-    def attr_namespace(self) -> _ros_cdk_core_7adfd82f.IResolvable:
+    def attr_namespace(self) -> ros_cdk_core.IResolvable:
         '''Attribute Namespace: Project space name.'''
-        return typing.cast(_ros_cdk_core_7adfd82f.IResolvable, jsii.get(self, "attrNamespace"))
+        return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrNamespace"))
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-flink.NamespaceProps",
     jsii_struct_bases=[],
     name_mapping={
         "instance_id": "instanceId",
@@ -332,97 +328,93 @@
         "resource_spec": "resourceSpec",
     },
 )
 class NamespaceProps:
     def __init__(
         self,
         *,
-        instance_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
-        namespace: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
-        resource_spec: typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Union["RosNamespace.ResourceSpecProperty", typing.Dict[builtins.str, typing.Any]]]] = None,
+        instance_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
+        namespace: typing.Union[builtins.str, ros_cdk_core.IResolvable],
+        resource_spec: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosNamespace.ResourceSpecProperty", typing.Dict[str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::Flink::Namespace``.
 
         :param instance_id: Property instanceId: Instance ID.
         :param namespace: Property namespace: Project space name.
         :param resource_spec: Property resourceSpec: Resource specifications.
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__073613f9bc7eed8c84f6e94da628751f3a2a6ed3818d6c5d7492ea9a6d4a1e65)
+            type_hints = typing.get_type_hints(NamespaceProps.__init__)
             check_type(argname="argument instance_id", value=instance_id, expected_type=type_hints["instance_id"])
             check_type(argname="argument namespace", value=namespace, expected_type=type_hints["namespace"])
             check_type(argname="argument resource_spec", value=resource_spec, expected_type=type_hints["resource_spec"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "instance_id": instance_id,
             "namespace": namespace,
         }
         if resource_spec is not None:
             self._values["resource_spec"] = resource_spec
 
     @builtins.property
-    def instance_id(
-        self,
-    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+    def instance_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''Property instanceId: Instance ID.'''
         result = self._values.get("instance_id")
         assert result is not None, "Required property 'instance_id' is missing"
-        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+        return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
 
     @builtins.property
-    def namespace(
-        self,
-    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+    def namespace(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''Property namespace: Project space name.'''
         result = self._values.get("namespace")
         assert result is not None, "Required property 'namespace' is missing"
-        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+        return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
 
     @builtins.property
     def resource_spec(
         self,
-    ) -> typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, "RosNamespace.ResourceSpecProperty"]]:
+    ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosNamespace.ResourceSpecProperty"]]:
         '''Property resourceSpec: Resource specifications.'''
         result = self._values.get("resource_spec")
-        return typing.cast(typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, "RosNamespace.ResourceSpecProperty"]], result)
+        return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosNamespace.ResourceSpecProperty"]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
         return "NamespaceProps(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 class RosInstance(
-    _ros_cdk_core_7adfd82f.RosResource,
+    ros_cdk_core.RosResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-flink.RosInstance",
 ):
     '''A ROS template type:  ``ALIYUN::Flink::Instance``.'''
 
     def __init__(
         self,
-        scope: _ros_cdk_core_7adfd82f.Construct,
+        scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: typing.Union["RosInstanceProps", typing.Dict[builtins.str, typing.Any]],
+        props: typing.Union["RosInstanceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::Flink::Instance``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__c771f15512f6ebcc1d3d22d2ddbfaa72e36a3dde32318fbc15694d8a68a9ae68)
+            type_hints = typing.get_type_hints(RosInstance.__init__)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
             check_type(argname="argument props", value=props, expected_type=type_hints["props"])
             check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
     @jsii.member(jsii_name="renderProperties")
@@ -430,359 +422,355 @@
         self,
         props: typing.Mapping[builtins.str, typing.Any],
     ) -> typing.Mapping[builtins.str, typing.Any]:
         '''
         :param props: -
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__4a7131e510066a730f31640c47be62722e13a49723e93297118d30aa0f9dba27)
+            type_hints = typing.get_type_hints(RosInstance._render_properties)
             check_type(argname="argument props", value=props, expected_type=type_hints["props"])
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.invoke(self, "renderProperties", [props]))
 
     @jsii.python.classproperty
     @jsii.member(jsii_name="ROS_RESOURCE_TYPE_NAME")
     def ROS_RESOURCE_TYPE_NAME(cls) -> builtins.str:
         '''The resource type name for this resource class.'''
         return typing.cast(builtins.str, jsii.sget(cls, "ROS_RESOURCE_TYPE_NAME"))
 
     @builtins.property
     @jsii.member(jsii_name="attrInstanceId")
-    def attr_instance_id(self) -> _ros_cdk_core_7adfd82f.IResolvable:
+    def attr_instance_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: InstanceId: Instance ID.
         '''
-        return typing.cast(_ros_cdk_core_7adfd82f.IResolvable, jsii.get(self, "attrInstanceId"))
+        return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceId"))
 
     @builtins.property
     @jsii.member(jsii_name="attrOrderId")
-    def attr_order_id(self) -> _ros_cdk_core_7adfd82f.IResolvable:
+    def attr_order_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: OrderId: Order information.
         '''
-        return typing.cast(_ros_cdk_core_7adfd82f.IResolvable, jsii.get(self, "attrOrderId"))
+        return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrOrderId"))
 
     @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
     @builtins.property
     @jsii.member(jsii_name="bucket")
-    def bucket(self) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+    def bucket(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: bucket: OSS bucket name.
         '''
-        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], jsii.get(self, "bucket"))
+        return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "bucket"))
 
     @bucket.setter
     def bucket(
         self,
-        value: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+        value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__8c9eb76c9064707f4e73c88556f5e3ebb942d9401ae211a216348c83da9280d8)
+            type_hints = typing.get_type_hints(getattr(RosInstance, "bucket").fset)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "bucket", value)
 
     @builtins.property
     @jsii.member(jsii_name="chargeType")
-    def charge_type(
-        self,
-    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+    def charge_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         chargeType: The payment type, the value of the value is as follows:
         POST: pay as you go.
         PRE: subscription.
         '''
-        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], jsii.get(self, "chargeType"))
+        return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "chargeType"))
 
     @charge_type.setter
     def charge_type(
         self,
-        value: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+        value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__122e9ab8466f2765dc113ee600c3771ad3d7d32ce33886963fa7aad43343350c)
+            type_hints = typing.get_type_hints(getattr(RosInstance, "charge_type").fset)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "chargeType", value)
 
     @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__caa25191be3a2a6309406987cb293a0a420a57a49a7f0b0c714b5a680d10cfdf)
+            type_hints = typing.get_type_hints(getattr(RosInstance, "enable_resource_property_constraint").fset)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
     @builtins.property
     @jsii.member(jsii_name="instanceName")
-    def instance_name(
-        self,
-    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+    def instance_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: instanceName: The name of instance.
         '''
-        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], jsii.get(self, "instanceName"))
+        return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "instanceName"))
 
     @instance_name.setter
     def instance_name(
         self,
-        value: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+        value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__44d1d25e77e8a85aabd7c20e0b5c99c2e77748ea759e1e1ace25251df6f02026)
+            type_hints = typing.get_type_hints(getattr(RosInstance, "instance_name").fset)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceName", value)
 
     @builtins.property
     @jsii.member(jsii_name="vpcId")
-    def vpc_id(self) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+    def vpc_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: vpcId: VPC ID.
         '''
-        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], jsii.get(self, "vpcId"))
+        return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "vpcId"))
 
     @vpc_id.setter
     def vpc_id(
         self,
-        value: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+        value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__8703527cd5c85622777d8cde9a7dc2d2b03c9fd365cc6c9223834cb17f81ddd7)
+            type_hints = typing.get_type_hints(getattr(RosInstance, "vpc_id").fset)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vpcId", value)
 
     @builtins.property
     @jsii.member(jsii_name="vSwitchIds")
     def v_switch_ids(
         self,
-    ) -> typing.Union[typing.List[typing.Any], _ros_cdk_core_7adfd82f.IResolvable]:
+    ) -> typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]:
         '''
         :Property: vSwitchIds: Virtual switch ID.
         '''
-        return typing.cast(typing.Union[typing.List[typing.Any], _ros_cdk_core_7adfd82f.IResolvable], jsii.get(self, "vSwitchIds"))
+        return typing.cast(typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable], jsii.get(self, "vSwitchIds"))
 
     @v_switch_ids.setter
     def v_switch_ids(
         self,
-        value: typing.Union[typing.List[typing.Any], _ros_cdk_core_7adfd82f.IResolvable],
+        value: typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__054167fc63bad102dad10aa15cfb7a2a440daa7cb3fee16113ca76ccade55def)
+            type_hints = typing.get_type_hints(getattr(RosInstance, "v_switch_ids").fset)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vSwitchIds", value)
 
     @builtins.property
     @jsii.member(jsii_name="zoneId")
-    def zone_id(self) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+    def zone_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: zoneId: The available area ID of the instance.
         '''
-        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], jsii.get(self, "zoneId"))
+        return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "zoneId"))
 
     @zone_id.setter
     def zone_id(
         self,
-        value: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+        value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__844677c246f1cf4c31df3316c74c77f0d90d82d3244f52e63c4ad070c119394d)
+            type_hints = typing.get_type_hints(getattr(RosInstance, "zone_id").fset)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "zoneId", value)
 
     @builtins.property
     @jsii.member(jsii_name="autoRenew")
     def auto_renew(
         self,
-    ) -> typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
         autoRenew: When the payment type is the monthly package, the value of the value is as follows:
         true: Automatic renewal.
         false: Manual renewal.
         '''
-        return typing.cast(typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]], jsii.get(self, "autoRenew"))
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "autoRenew"))
 
     @auto_renew.setter
     def auto_renew(
         self,
-        value: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]],
+        value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__364c0a63c673104d9cd4040effa29129ad4ef48a8dc4a0622ce353a8ca85ec96)
+            type_hints = typing.get_type_hints(getattr(RosInstance, "auto_renew").fset)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "autoRenew", value)
 
     @builtins.property
     @jsii.member(jsii_name="duration")
     def duration(
         self,
-    ) -> typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
         duration: Number of order cycle.
         When ChargeType is configured as PRE, the duration parameter must be filled.
         If PricingCycle is Month, the valid range is 1, 2, 3, 6, 7, 8, 9, 12, 24, 36
         If PricingCycle is year, the valid range is 1 to 3
         '''
-        return typing.cast(typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]], jsii.get(self, "duration"))
+        return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "duration"))
 
     @duration.setter
     def duration(
         self,
-        value: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]],
+        value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__db96ecfd89754323be433c6a3b130bdada9b41393630ce6ba5fcc3aa9cde9454)
+            type_hints = typing.get_type_hints(getattr(RosInstance, "duration").fset)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "duration", value)
 
     @builtins.property
     @jsii.member(jsii_name="pricingCycle")
     def pricing_cycle(
         self,
-    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: pricingCycle: The ordering cycle only supports ordering in the year and month.
         '''
-        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], jsii.get(self, "pricingCycle"))
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "pricingCycle"))
 
     @pricing_cycle.setter
     def pricing_cycle(
         self,
-        value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
+        value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__6fd26b3eeb0b49ff4648b8baafb600a5adbf61d2be7b4e3538a1a5f9af889083)
+            type_hints = typing.get_type_hints(getattr(RosInstance, "pricing_cycle").fset)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "pricingCycle", value)
 
     @builtins.property
     @jsii.member(jsii_name="promotionCode")
     def promotion_code(
         self,
-    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: promotionCode: Promo Code.
         '''
-        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], jsii.get(self, "promotionCode"))
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "promotionCode"))
 
     @promotion_code.setter
     def promotion_code(
         self,
-        value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
+        value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__952672c7328fe8fd753b7b7c059a1bddf29bf4b89a4fd7b80aac2050b4e482ba)
+            type_hints = typing.get_type_hints(getattr(RosInstance, "promotion_code").fset)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "promotionCode", value)
 
     @builtins.property
     @jsii.member(jsii_name="resourceSpec")
     def resource_spec(
         self,
-    ) -> typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, "RosInstance.ResourceSpecProperty"]]:
+    ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosInstance.ResourceSpecProperty"]]:
         '''
         :Property:
 
         resourceSpec: Resource specifications.
         When ChargeType is configured as PRE, the resource specification parameters must be filled.
         '''
-        return typing.cast(typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, "RosInstance.ResourceSpecProperty"]], jsii.get(self, "resourceSpec"))
+        return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosInstance.ResourceSpecProperty"]], jsii.get(self, "resourceSpec"))
 
     @resource_spec.setter
     def resource_spec(
         self,
-        value: typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, "RosInstance.ResourceSpecProperty"]],
+        value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosInstance.ResourceSpecProperty"]],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__8d0bb2b35196173ef949e0ff9c055d8c6c2718f4574dd691a70bf314b97eaae9)
+            type_hints = typing.get_type_hints(getattr(RosInstance, "resource_spec").fset)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "resourceSpec", value)
 
     @builtins.property
     @jsii.member(jsii_name="usePromotionCode")
     def use_promotion_code(
         self,
-    ) -> typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
         usePromotionCode: Whether to use coupons.The value is as follows:
         true: Use.
         false: Not in use.
         '''
-        return typing.cast(typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]], jsii.get(self, "usePromotionCode"))
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "usePromotionCode"))
 
     @use_promotion_code.setter
     def use_promotion_code(
         self,
-        value: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]],
+        value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__4e1a9e56b27e9178ac083bfe083c479d3eaf230a6f66b6a02f28723efbed7175)
+            type_hints = typing.get_type_hints(getattr(RosInstance, "use_promotion_code").fset)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "usePromotionCode", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-flink.RosInstance.ResourceSpecProperty",
         jsii_struct_bases=[],
         name_mapping={"cpu": "cpu", "memory_gb": "memoryGb"},
     )
     class ResourceSpecProperty:
         def __init__(
             self,
             *,
-            cpu: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-            memory_gb: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+            cpu: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
+            memory_gb: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param cpu: 
             :param memory_gb: 
             '''
             if __debug__:
-                type_hints = typing.get_type_hints(_typecheckingstub__69292397a3fb0e28780277edcde87adcb9a4a94ba84158a0dea3fe49fab6ae7f)
+                type_hints = typing.get_type_hints(RosInstance.ResourceSpecProperty.__init__)
                 check_type(argname="argument cpu", value=cpu, expected_type=type_hints["cpu"])
                 check_type(argname="argument memory_gb", value=memory_gb, expected_type=type_hints["memory_gb"])
-            self._values: typing.Dict[builtins.str, typing.Any] = {}
+            self._values: typing.Dict[str, typing.Any] = {}
             if cpu is not None:
                 self._values["cpu"] = cpu
             if memory_gb is not None:
                 self._values["memory_gb"] = memory_gb
 
         @builtins.property
         def cpu(
             self,
-        ) -> typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]]:
+        ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
             '''
             :Property: cpu: CPU number.
             '''
             result = self._values.get("cpu")
-            return typing.cast(typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]], result)
+            return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], result)
 
         @builtins.property
         def memory_gb(
             self,
-        ) -> typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]]:
+        ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
             '''
             :Property:
 
             memoryGb: memory size.The unit is GB.
             It shows that the amount of memory must be 4 times the number of CPUs.
             '''
             result = self._values.get("memory_gb")
-            return typing.cast(typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]], result)
+            return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], result)
 
         def __eq__(self, rhs: typing.Any) -> builtins.bool:
             return isinstance(rhs, self.__class__) and rhs._values == self._values
 
         def __ne__(self, rhs: typing.Any) -> builtins.bool:
             return not (rhs == self)
 
@@ -810,26 +798,26 @@
         "use_promotion_code": "usePromotionCode",
     },
 )
 class RosInstanceProps:
     def __init__(
         self,
         *,
-        bucket: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
-        charge_type: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
-        instance_name: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
-        vpc_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
-        v_switch_ids: typing.Union[typing.Sequence[typing.Any], _ros_cdk_core_7adfd82f.IResolvable],
-        zone_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
-        auto_renew: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-        duration: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-        pricing_cycle: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-        promotion_code: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-        resource_spec: typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Union[RosInstance.ResourceSpecProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
-        use_promotion_code: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+        bucket: typing.Union[builtins.str, ros_cdk_core.IResolvable],
+        charge_type: typing.Union[builtins.str, ros_cdk_core.IResolvable],
+        instance_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
+        vpc_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
+        v_switch_ids: typing.Union[typing.Sequence[typing.Any], ros_cdk_core.IResolvable],
+        zone_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
+        auto_renew: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
+        duration: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
+        pricing_cycle: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
+        promotion_code: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
+        resource_spec: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosInstance.ResourceSpecProperty, typing.Dict[str, typing.Any]]]] = None,
+        use_promotion_code: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::Flink::Instance``.
 
         :param bucket: 
         :param charge_type: 
         :param instance_name: 
         :param vpc_id: 
@@ -839,28 +827,28 @@
         :param duration: 
         :param pricing_cycle: 
         :param promotion_code: 
         :param resource_spec: 
         :param use_promotion_code: 
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__b3e0cb8a67e4fc721681b849306490fc8c0a5a469d2f01a5f043d1130ff6140b)
+            type_hints = typing.get_type_hints(RosInstanceProps.__init__)
             check_type(argname="argument bucket", value=bucket, expected_type=type_hints["bucket"])
             check_type(argname="argument charge_type", value=charge_type, expected_type=type_hints["charge_type"])
             check_type(argname="argument instance_name", value=instance_name, expected_type=type_hints["instance_name"])
             check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
             check_type(argname="argument v_switch_ids", value=v_switch_ids, expected_type=type_hints["v_switch_ids"])
             check_type(argname="argument zone_id", value=zone_id, expected_type=type_hints["zone_id"])
             check_type(argname="argument auto_renew", value=auto_renew, expected_type=type_hints["auto_renew"])
             check_type(argname="argument duration", value=duration, expected_type=type_hints["duration"])
             check_type(argname="argument pricing_cycle", value=pricing_cycle, expected_type=type_hints["pricing_cycle"])
             check_type(argname="argument promotion_code", value=promotion_code, expected_type=type_hints["promotion_code"])
             check_type(argname="argument resource_spec", value=resource_spec, expected_type=type_hints["resource_spec"])
             check_type(argname="argument use_promotion_code", value=use_promotion_code, expected_type=type_hints["use_promotion_code"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "bucket": bucket,
             "charge_type": charge_type,
             "instance_name": instance_name,
             "vpc_id": vpc_id,
             "v_switch_ids": v_switch_ids,
             "zone_id": zone_id,
         }
@@ -874,188 +862,184 @@
             self._values["promotion_code"] = promotion_code
         if resource_spec is not None:
             self._values["resource_spec"] = resource_spec
         if use_promotion_code is not None:
             self._values["use_promotion_code"] = use_promotion_code
 
     @builtins.property
-    def bucket(self) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+    def bucket(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: bucket: OSS bucket name.
         '''
         result = self._values.get("bucket")
         assert result is not None, "Required property 'bucket' is missing"
-        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+        return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
 
     @builtins.property
-    def charge_type(
-        self,
-    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+    def charge_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         chargeType: The payment type, the value of the value is as follows:
         POST: pay as you go.
         PRE: subscription.
         '''
         result = self._values.get("charge_type")
         assert result is not None, "Required property 'charge_type' is missing"
-        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+        return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
 
     @builtins.property
-    def instance_name(
-        self,
-    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+    def instance_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: instanceName: The name of instance.
         '''
         result = self._values.get("instance_name")
         assert result is not None, "Required property 'instance_name' is missing"
-        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+        return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
 
     @builtins.property
-    def vpc_id(self) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+    def vpc_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: vpcId: VPC ID.
         '''
         result = self._values.get("vpc_id")
         assert result is not None, "Required property 'vpc_id' is missing"
-        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+        return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
 
     @builtins.property
     def v_switch_ids(
         self,
-    ) -> typing.Union[typing.List[typing.Any], _ros_cdk_core_7adfd82f.IResolvable]:
+    ) -> typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]:
         '''
         :Property: vSwitchIds: Virtual switch ID.
         '''
         result = self._values.get("v_switch_ids")
         assert result is not None, "Required property 'v_switch_ids' is missing"
-        return typing.cast(typing.Union[typing.List[typing.Any], _ros_cdk_core_7adfd82f.IResolvable], result)
+        return typing.cast(typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable], result)
 
     @builtins.property
-    def zone_id(self) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+    def zone_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: zoneId: The available area ID of the instance.
         '''
         result = self._values.get("zone_id")
         assert result is not None, "Required property 'zone_id' is missing"
-        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+        return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
 
     @builtins.property
     def auto_renew(
         self,
-    ) -> typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
         autoRenew: When the payment type is the monthly package, the value of the value is as follows:
         true: Automatic renewal.
         false: Manual renewal.
         '''
         result = self._values.get("auto_renew")
-        return typing.cast(typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]], result)
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def duration(
         self,
-    ) -> typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
         duration: Number of order cycle.
         When ChargeType is configured as PRE, the duration parameter must be filled.
         If PricingCycle is Month, the valid range is 1, 2, 3, 6, 7, 8, 9, 12, 24, 36
         If PricingCycle is year, the valid range is 1 to 3
         '''
         result = self._values.get("duration")
-        return typing.cast(typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]], result)
+        return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def pricing_cycle(
         self,
-    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: pricingCycle: The ordering cycle only supports ordering in the year and month.
         '''
         result = self._values.get("pricing_cycle")
-        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def promotion_code(
         self,
-    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: promotionCode: Promo Code.
         '''
         result = self._values.get("promotion_code")
-        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def resource_spec(
         self,
-    ) -> typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, RosInstance.ResourceSpecProperty]]:
+    ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosInstance.ResourceSpecProperty]]:
         '''
         :Property:
 
         resourceSpec: Resource specifications.
         When ChargeType is configured as PRE, the resource specification parameters must be filled.
         '''
         result = self._values.get("resource_spec")
-        return typing.cast(typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, RosInstance.ResourceSpecProperty]], result)
+        return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosInstance.ResourceSpecProperty]], result)
 
     @builtins.property
     def use_promotion_code(
         self,
-    ) -> typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]]:
+    ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
         usePromotionCode: Whether to use coupons.The value is as follows:
         true: Use.
         false: Not in use.
         '''
         result = self._values.get("use_promotion_code")
-        return typing.cast(typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]], result)
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
         return "RosInstanceProps(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 class RosNamespace(
-    _ros_cdk_core_7adfd82f.RosResource,
+    ros_cdk_core.RosResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-flink.RosNamespace",
 ):
     '''A ROS template type:  ``ALIYUN::Flink::Namespace``.'''
 
     def __init__(
         self,
-        scope: _ros_cdk_core_7adfd82f.Construct,
+        scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: typing.Union["RosNamespaceProps", typing.Dict[builtins.str, typing.Any]],
+        props: typing.Union["RosNamespaceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::Flink::Namespace``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__58f2a56d24b075b4780a1f6935688c6394f152ce2111381ec954b71d6924671e)
+            type_hints = typing.get_type_hints(RosNamespace.__init__)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
             check_type(argname="argument props", value=props, expected_type=type_hints["props"])
             check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
     @jsii.member(jsii_name="renderProperties")
@@ -1063,170 +1047,166 @@
         self,
         props: typing.Mapping[builtins.str, typing.Any],
     ) -> typing.Mapping[builtins.str, typing.Any]:
         '''
         :param props: -
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__e3768dd8ad1ea82c08981a493ea3a195dfbf42cb24446c8e0fbedcbdafa93aad)
+            type_hints = typing.get_type_hints(RosNamespace._render_properties)
             check_type(argname="argument props", value=props, expected_type=type_hints["props"])
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.invoke(self, "renderProperties", [props]))
 
     @jsii.python.classproperty
     @jsii.member(jsii_name="ROS_RESOURCE_TYPE_NAME")
     def ROS_RESOURCE_TYPE_NAME(cls) -> builtins.str:
         '''The resource type name for this resource class.'''
         return typing.cast(builtins.str, jsii.sget(cls, "ROS_RESOURCE_TYPE_NAME"))
 
     @builtins.property
     @jsii.member(jsii_name="attrInstanceId")
-    def attr_instance_id(self) -> _ros_cdk_core_7adfd82f.IResolvable:
+    def attr_instance_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: InstanceId: Instance ID.
         '''
-        return typing.cast(_ros_cdk_core_7adfd82f.IResolvable, jsii.get(self, "attrInstanceId"))
+        return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceId"))
 
     @builtins.property
     @jsii.member(jsii_name="attrNamespace")
-    def attr_namespace(self) -> _ros_cdk_core_7adfd82f.IResolvable:
+    def attr_namespace(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Namespace: Project space name.
         '''
-        return typing.cast(_ros_cdk_core_7adfd82f.IResolvable, jsii.get(self, "attrNamespace"))
+        return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrNamespace"))
 
     @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
     @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__1ad1487516706ced1dae9bb97f7f08d398357867f01c501f22b6847ceaf3dbf2)
+            type_hints = typing.get_type_hints(getattr(RosNamespace, "enable_resource_property_constraint").fset)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
     @builtins.property
     @jsii.member(jsii_name="instanceId")
-    def instance_id(
-        self,
-    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+    def instance_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: instanceId: Instance ID.
         '''
-        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], jsii.get(self, "instanceId"))
+        return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "instanceId"))
 
     @instance_id.setter
     def instance_id(
         self,
-        value: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+        value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__db6dc84bc58dc44c8075b6e9b04104b33c57947e7d954359f8cf467af12b02c7)
+            type_hints = typing.get_type_hints(getattr(RosNamespace, "instance_id").fset)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceId", value)
 
     @builtins.property
     @jsii.member(jsii_name="namespace")
-    def namespace(
-        self,
-    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+    def namespace(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: namespace: Project space name.
         '''
-        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], jsii.get(self, "namespace"))
+        return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "namespace"))
 
     @namespace.setter
     def namespace(
         self,
-        value: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+        value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__f5e153cdca5534618107c75058e89e198269a4055ee9c23c4ef853d45358338f)
+            type_hints = typing.get_type_hints(getattr(RosNamespace, "namespace").fset)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "namespace", value)
 
     @builtins.property
     @jsii.member(jsii_name="resourceSpec")
     def resource_spec(
         self,
-    ) -> typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, "RosNamespace.ResourceSpecProperty"]]:
+    ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosNamespace.ResourceSpecProperty"]]:
         '''
         :Property: resourceSpec: Resource specifications.
         '''
-        return typing.cast(typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, "RosNamespace.ResourceSpecProperty"]], jsii.get(self, "resourceSpec"))
+        return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosNamespace.ResourceSpecProperty"]], jsii.get(self, "resourceSpec"))
 
     @resource_spec.setter
     def resource_spec(
         self,
-        value: typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, "RosNamespace.ResourceSpecProperty"]],
+        value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosNamespace.ResourceSpecProperty"]],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__804b4695e2e9feb0977904d60c730ddee40645d96a6de41c1cc67d157d4341a1)
+            type_hints = typing.get_type_hints(getattr(RosNamespace, "resource_spec").fset)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "resourceSpec", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-flink.RosNamespace.ResourceSpecProperty",
         jsii_struct_bases=[],
         name_mapping={"cpu": "cpu", "memory_gb": "memoryGb"},
     )
     class ResourceSpecProperty:
         def __init__(
             self,
             *,
-            cpu: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-            memory_gb: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+            cpu: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
+            memory_gb: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param cpu: 
             :param memory_gb: 
             '''
             if __debug__:
-                type_hints = typing.get_type_hints(_typecheckingstub__fe251838f933d1628f78e6e07d513864d458262095430252cf49017026f4e7c2)
+                type_hints = typing.get_type_hints(RosNamespace.ResourceSpecProperty.__init__)
                 check_type(argname="argument cpu", value=cpu, expected_type=type_hints["cpu"])
                 check_type(argname="argument memory_gb", value=memory_gb, expected_type=type_hints["memory_gb"])
-            self._values: typing.Dict[builtins.str, typing.Any] = {}
+            self._values: typing.Dict[str, typing.Any] = {}
             if cpu is not None:
                 self._values["cpu"] = cpu
             if memory_gb is not None:
                 self._values["memory_gb"] = memory_gb
 
         @builtins.property
         def cpu(
             self,
-        ) -> typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]]:
+        ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
             '''
             :Property:
 
             cpu: CPU number.
             In the working space of the annual package, the number of CPUs must be filled.Under the working space of paying in volume, you can not fill in the number of CPUs.
             The number of CPUs created by the target project space is less than the number of CPU remaining in the working space (the total number of CPU purchased by the work space minus the number of other project spaces that has been assigned the number of CPUs), otherwise an error will be reported.
             '''
             result = self._values.get("cpu")
-            return typing.cast(typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]], result)
+            return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], result)
 
         @builtins.property
         def memory_gb(
             self,
-        ) -> typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]]:
+        ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
             '''
             :Property:
 
             memoryGb: Memory.
             In the working space of the annual package, the amount of memory must be filled, and the amount of memory must be 4 times.Under the working space of paying in volume, you can fill in the amount of memory without filling in the amount of memory.
             The amount of memory in the target project space is less than the remaining memory of the working space (the total amount of memory purchased by the work space minus the number of other project spaces that have been assigned the amount of memory), otherwise an error will be reported.
             '''
             result = self._values.get("memory_gb")
-            return typing.cast(typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]], result)
+            return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], result)
 
         def __eq__(self, rhs: typing.Any) -> builtins.bool:
             return isinstance(rhs, self.__class__) and rhs._values == self._values
 
         def __ne__(self, rhs: typing.Any) -> builtins.bool:
             return not (rhs == self)
 
@@ -1245,67 +1225,63 @@
         "resource_spec": "resourceSpec",
     },
 )
 class RosNamespaceProps:
     def __init__(
         self,
         *,
-        instance_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
-        namespace: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
-        resource_spec: typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Union[RosNamespace.ResourceSpecProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
+        instance_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
+        namespace: typing.Union[builtins.str, ros_cdk_core.IResolvable],
+        resource_spec: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosNamespace.ResourceSpecProperty, typing.Dict[str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::Flink::Namespace``.
 
         :param instance_id: 
         :param namespace: 
         :param resource_spec: 
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__a2fac56047c070a8586e9a30e78f42ab6f0eba905792fd3c51d4a274b0510fec)
+            type_hints = typing.get_type_hints(RosNamespaceProps.__init__)
             check_type(argname="argument instance_id", value=instance_id, expected_type=type_hints["instance_id"])
             check_type(argname="argument namespace", value=namespace, expected_type=type_hints["namespace"])
             check_type(argname="argument resource_spec", value=resource_spec, expected_type=type_hints["resource_spec"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "instance_id": instance_id,
             "namespace": namespace,
         }
         if resource_spec is not None:
             self._values["resource_spec"] = resource_spec
 
     @builtins.property
-    def instance_id(
-        self,
-    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+    def instance_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: instanceId: Instance ID.
         '''
         result = self._values.get("instance_id")
         assert result is not None, "Required property 'instance_id' is missing"
-        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+        return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
 
     @builtins.property
-    def namespace(
-        self,
-    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+    def namespace(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: namespace: Project space name.
         '''
         result = self._values.get("namespace")
         assert result is not None, "Required property 'namespace' is missing"
-        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+        return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
 
     @builtins.property
     def resource_spec(
         self,
-    ) -> typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, RosNamespace.ResourceSpecProperty]]:
+    ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosNamespace.ResourceSpecProperty]]:
         '''
         :Property: resourceSpec: Resource specifications.
         '''
         result = self._values.get("resource_spec")
-        return typing.cast(typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, RosNamespace.ResourceSpecProperty]], result)
+        return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosNamespace.ResourceSpecProperty]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
@@ -1323,227 +1299,7 @@
     "RosInstance",
     "RosInstanceProps",
     "RosNamespace",
     "RosNamespaceProps",
 ]
 
 publication.publish()
-
-def _typecheckingstub__7ac06ec3a5b462ac2e1cc27879335e2b5a2554adaed27232209ad964bf56332b(
-    scope: _ros_cdk_core_7adfd82f.Construct,
-    id: builtins.str,
-    props: typing.Union[InstanceProps, typing.Dict[builtins.str, typing.Any]],
-    enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__92f8fcd41ef922ea4bbdd21e7b570a2ba79e56738c3c1a4f4e819b0369bd1198(
-    *,
-    bucket: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
-    charge_type: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
-    instance_name: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
-    vpc_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
-    v_switch_ids: typing.Union[typing.Sequence[typing.Any], _ros_cdk_core_7adfd82f.IResolvable],
-    zone_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
-    auto_renew: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-    duration: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-    pricing_cycle: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-    promotion_code: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-    resource_spec: typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Union[RosInstance.ResourceSpecProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
-    use_promotion_code: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__f429333a5e22f08d25a6d8cee2f94a9afac4e7c85bdeec6706e8ae09fe8d4062(
-    scope: _ros_cdk_core_7adfd82f.Construct,
-    id: builtins.str,
-    props: typing.Union[NamespaceProps, typing.Dict[builtins.str, typing.Any]],
-    enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__073613f9bc7eed8c84f6e94da628751f3a2a6ed3818d6c5d7492ea9a6d4a1e65(
-    *,
-    instance_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
-    namespace: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
-    resource_spec: typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Union[RosNamespace.ResourceSpecProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__c771f15512f6ebcc1d3d22d2ddbfaa72e36a3dde32318fbc15694d8a68a9ae68(
-    scope: _ros_cdk_core_7adfd82f.Construct,
-    id: builtins.str,
-    props: typing.Union[RosInstanceProps, typing.Dict[builtins.str, typing.Any]],
-    enable_resource_property_constraint: builtins.bool,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__4a7131e510066a730f31640c47be62722e13a49723e93297118d30aa0f9dba27(
-    props: typing.Mapping[builtins.str, typing.Any],
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__8c9eb76c9064707f4e73c88556f5e3ebb942d9401ae211a216348c83da9280d8(
-    value: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__122e9ab8466f2765dc113ee600c3771ad3d7d32ce33886963fa7aad43343350c(
-    value: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__caa25191be3a2a6309406987cb293a0a420a57a49a7f0b0c714b5a680d10cfdf(
-    value: builtins.bool,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__44d1d25e77e8a85aabd7c20e0b5c99c2e77748ea759e1e1ace25251df6f02026(
-    value: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__8703527cd5c85622777d8cde9a7dc2d2b03c9fd365cc6c9223834cb17f81ddd7(
-    value: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__054167fc63bad102dad10aa15cfb7a2a440daa7cb3fee16113ca76ccade55def(
-    value: typing.Union[typing.List[typing.Any], _ros_cdk_core_7adfd82f.IResolvable],
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__844677c246f1cf4c31df3316c74c77f0d90d82d3244f52e63c4ad070c119394d(
-    value: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__364c0a63c673104d9cd4040effa29129ad4ef48a8dc4a0622ce353a8ca85ec96(
-    value: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]],
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__db96ecfd89754323be433c6a3b130bdada9b41393630ce6ba5fcc3aa9cde9454(
-    value: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]],
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__6fd26b3eeb0b49ff4648b8baafb600a5adbf61d2be7b4e3538a1a5f9af889083(
-    value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__952672c7328fe8fd753b7b7c059a1bddf29bf4b89a4fd7b80aac2050b4e482ba(
-    value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__8d0bb2b35196173ef949e0ff9c055d8c6c2718f4574dd691a70bf314b97eaae9(
-    value: typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, RosInstance.ResourceSpecProperty]],
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__4e1a9e56b27e9178ac083bfe083c479d3eaf230a6f66b6a02f28723efbed7175(
-    value: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]],
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__69292397a3fb0e28780277edcde87adcb9a4a94ba84158a0dea3fe49fab6ae7f(
-    *,
-    cpu: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-    memory_gb: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__b3e0cb8a67e4fc721681b849306490fc8c0a5a469d2f01a5f043d1130ff6140b(
-    *,
-    bucket: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
-    charge_type: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
-    instance_name: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
-    vpc_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
-    v_switch_ids: typing.Union[typing.Sequence[typing.Any], _ros_cdk_core_7adfd82f.IResolvable],
-    zone_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
-    auto_renew: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-    duration: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-    pricing_cycle: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-    promotion_code: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-    resource_spec: typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Union[RosInstance.ResourceSpecProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
-    use_promotion_code: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__58f2a56d24b075b4780a1f6935688c6394f152ce2111381ec954b71d6924671e(
-    scope: _ros_cdk_core_7adfd82f.Construct,
-    id: builtins.str,
-    props: typing.Union[RosNamespaceProps, typing.Dict[builtins.str, typing.Any]],
-    enable_resource_property_constraint: builtins.bool,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__e3768dd8ad1ea82c08981a493ea3a195dfbf42cb24446c8e0fbedcbdafa93aad(
-    props: typing.Mapping[builtins.str, typing.Any],
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__1ad1487516706ced1dae9bb97f7f08d398357867f01c501f22b6847ceaf3dbf2(
-    value: builtins.bool,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__db6dc84bc58dc44c8075b6e9b04104b33c57947e7d954359f8cf467af12b02c7(
-    value: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__f5e153cdca5534618107c75058e89e198269a4055ee9c23c4ef853d45358338f(
-    value: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__804b4695e2e9feb0977904d60c730ddee40645d96a6de41c1cc67d157d4341a1(
-    value: typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, RosNamespace.ResourceSpecProperty]],
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__fe251838f933d1628f78e6e07d513864d458262095430252cf49017026f4e7c2(
-    *,
-    cpu: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-    memory_gb: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__a2fac56047c070a8586e9a30e78f42ab6f0eba905792fd3c51d4a274b0510fec(
-    *,
-    instance_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
-    namespace: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
-    resource_spec: typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Union[RosNamespace.ResourceSpecProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
```

### Comparing `ros-cdk-flink-1.0.14/src/ros_cdk_flink.egg-info/PKG-INFO` & `ros-cdk-flink-1.0.9/src/ros_cdk_flink.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-flink
-Version: 1.0.14
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS FLINK Construct Library
         
@@ -19,13 +19,12 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
```

