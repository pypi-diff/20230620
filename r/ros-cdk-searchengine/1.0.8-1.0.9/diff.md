# Comparing `tmp/ros-cdk-searchengine-1.0.8.tar.gz` & `tmp/ros-cdk-searchengine-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-searchengine-1.0.8.tar", last modified: Thu Jul 14 02:13:18 2022, max compression
+gzip compressed data, was "dist/ros-cdk-searchengine-1.0.9.tar", last modified: Fri Sep 23 10:48:35 2022, max compression
```

## Comparing `ros-cdk-searchengine-1.0.8.tar` & `ros-cdk-searchengine-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:13:18.000000 ros-cdk-searchengine-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:13:18.000000 ros-cdk-searchengine-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:13:18.000000 ros-cdk-searchengine-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:13:18.000000 ros-cdk-searchengine-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1276 2022-07-14 02:13:18.000000 ros-cdk-searchengine-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      206 2022-07-14 02:13:18.000000 ros-cdk-searchengine-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:13:18.000000 ros-cdk-searchengine-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:13:18.000000 ros-cdk-searchengine-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1848 2022-07-14 02:13:18.000000 ros-cdk-searchengine-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:13:18.000000 ros-cdk-searchengine-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:13:18.000000 ros-cdk-searchengine-1.0.8/src/ros_cdk_searchengine/
--rw-r--r--   0 root         (0) root         (0)    24560 2022-07-14 02:13:18.000000 ros-cdk-searchengine-1.0.8/src/ros_cdk_searchengine/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:13:18.000000 ros-cdk-searchengine-1.0.8/src/ros_cdk_searchengine/_jsii/
--rw-r--r--   0 root         (0) root         (0)      401 2022-07-14 02:13:18.000000 ros-cdk-searchengine-1.0.8/src/ros_cdk_searchengine/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33364 2022-07-14 02:13:18.000000 ros-cdk-searchengine-1.0.8/src/ros_cdk_searchengine/_jsii/ros-cdk-searchengine@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:13:18.000000 ros-cdk-searchengine-1.0.8/src/ros_cdk_searchengine/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:13:18.000000 ros-cdk-searchengine-1.0.8/src/ros_cdk_searchengine.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1276 2022-07-14 02:13:18.000000 ros-cdk-searchengine-1.0.8/src/ros_cdk_searchengine.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      490 2022-07-14 02:13:18.000000 ros-cdk-searchengine-1.0.8/src/ros_cdk_searchengine.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:13:18.000000 ros-cdk-searchengine-1.0.8/src/ros_cdk_searchengine.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:13:18.000000 ros-cdk-searchengine-1.0.8/src/ros_cdk_searchengine.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2022-07-14 02:13:18.000000 ros-cdk-searchengine-1.0.8/src/ros_cdk_searchengine.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:48:35.000000 ros-cdk-searchengine-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 10:48:35.000000 ros-cdk-searchengine-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 10:48:35.000000 ros-cdk-searchengine-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 10:48:35.000000 ros-cdk-searchengine-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1276 2022-09-23 10:48:35.000000 ros-cdk-searchengine-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      206 2022-09-23 10:48:35.000000 ros-cdk-searchengine-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 10:48:35.000000 ros-cdk-searchengine-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 10:48:35.000000 ros-cdk-searchengine-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1877 2022-09-23 10:48:35.000000 ros-cdk-searchengine-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:48:35.000000 ros-cdk-searchengine-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:48:35.000000 ros-cdk-searchengine-1.0.9/src/ros_cdk_searchengine/
+-rw-r--r--   0 root         (0) root         (0)    30385 2022-09-23 10:48:35.000000 ros-cdk-searchengine-1.0.9/src/ros_cdk_searchengine/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:48:35.000000 ros-cdk-searchengine-1.0.9/src/ros_cdk_searchengine/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      435 2022-09-23 10:48:35.000000 ros-cdk-searchengine-1.0.9/src/ros_cdk_searchengine/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33429 2022-09-23 10:48:35.000000 ros-cdk-searchengine-1.0.9/src/ros_cdk_searchengine/_jsii/ros-cdk-searchengine@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 10:48:35.000000 ros-cdk-searchengine-1.0.9/src/ros_cdk_searchengine/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:48:35.000000 ros-cdk-searchengine-1.0.9/src/ros_cdk_searchengine.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1276 2022-09-23 10:48:35.000000 ros-cdk-searchengine-1.0.9/src/ros_cdk_searchengine.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      490 2022-09-23 10:48:35.000000 ros-cdk-searchengine-1.0.9/src/ros_cdk_searchengine.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 10:48:35.000000 ros-cdk-searchengine-1.0.9/src/ros_cdk_searchengine.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 10:48:35.000000 ros-cdk-searchengine-1.0.9/src/ros_cdk_searchengine.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2022-09-23 10:48:35.000000 ros-cdk-searchengine-1.0.9/src/ros_cdk_searchengine.egg-info/top_level.txt
```

### Comparing `ros-cdk-searchengine-1.0.8/LICENSE` & `ros-cdk-searchengine-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-searchengine-1.0.8/PKG-INFO` & `ros-cdk-searchengine-1.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-searchengine
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS SEARCHENGINE Construct Library
```

### Comparing `ros-cdk-searchengine-1.0.8/setup.py` & `ros-cdk-searchengine-1.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-searchengine",
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
         "ros_cdk_searchengine",
         "ros_cdk_searchengine._jsii"
     ],
     "package_data": {
         "ros_cdk_searchengine._jsii": [
-            "ros-cdk-searchengine@1.0.8.jsii.tgz"
+            "ros-cdk-searchengine@1.0.9.jsii.tgz"
         ],
         "ros_cdk_searchengine": [
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

### Comparing `ros-cdk-searchengine-1.0.8/src/ros_cdk_searchengine/__init__.py` & `ros-cdk-searchengine-1.0.9/src/ros_cdk_searchengine/__init__.py`

 * *Files 20% similar despite different names*

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
 
 
 class Instance(
     ros_cdk_core.Resource,
@@ -29,37 +31,43 @@
 ):
     '''A ROS resource type:  ``ALIYUN::SearchEngine::Instance``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "InstanceProps",
+        props: typing.Union["InstanceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::SearchEngine::Instance``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Instance.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrEndpoint")
     def attr_endpoint(self) -> ros_cdk_core.IResolvable:
         '''Attribute Endpoint: The endpoint of instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrEndpoint"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceId")
     def attr_instance_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute InstanceId: The ID of instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceId"))
 
 
 @jsii.data_type(
@@ -102,14 +110,26 @@
         :param searcher_doc_size: Property searcherDocSize: The storage size of single data node.
         :param searcher_num: Property searcherNum: The number of data nodes.
         :param searcher_spec: Property searcherSpec: The specification of data nodes.
         :param user_name: Property userName: The user name of instance. Begin with a letter, support upper and lower case letters, numbers, underscores, length 1-30 characters.
         :param vpc_id: Property vpcId: The ID of VPC.
         :param v_switch_id: Property vSwitchId: The ID of vSwitch.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(InstanceProps.__init__)
+            check_type(argname="argument charge_type", value=charge_type, expected_type=type_hints["charge_type"])
+            check_type(argname="argument password", value=password, expected_type=type_hints["password"])
+            check_type(argname="argument qrs_num", value=qrs_num, expected_type=type_hints["qrs_num"])
+            check_type(argname="argument qrs_spec", value=qrs_spec, expected_type=type_hints["qrs_spec"])
+            check_type(argname="argument searcher_doc_size", value=searcher_doc_size, expected_type=type_hints["searcher_doc_size"])
+            check_type(argname="argument searcher_num", value=searcher_num, expected_type=type_hints["searcher_num"])
+            check_type(argname="argument searcher_spec", value=searcher_spec, expected_type=type_hints["searcher_spec"])
+            check_type(argname="argument user_name", value=user_name, expected_type=type_hints["user_name"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "charge_type": charge_type,
             "password": password,
             "qrs_num": qrs_num,
             "qrs_spec": qrs_spec,
             "searcher_doc_size": searcher_doc_size,
             "searcher_num": searcher_num,
@@ -218,64 +238,73 @@
 ):
     '''A ROS template type:  ``ALIYUN::SearchEngine::Instance``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosInstanceProps",
+        props: typing.Union["RosInstanceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::SearchEngine::Instance``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosInstance.__init__)
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
+            type_hints = typing.get_type_hints(RosInstance._render_properties)
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
     @jsii.member(jsii_name="attrEndpoint")
     def attr_endpoint(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Endpoint: The endpoint of instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrEndpoint"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceId")
     def attr_instance_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: InstanceId: The ID of instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="chargeType")
     def charge_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         chargeType: The billing method. Valid values: POSTPAY.
         POSTPAY: pay-as-you-go.
@@ -283,158 +312,191 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "chargeType"))
 
     @charge_type.setter
     def charge_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "charge_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "chargeType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="password")
     def password(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: password: The password of instance. It consists of lowercase letters and numbers, and the length is 6-8 characters.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "password"))
 
     @password.setter
     def password(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "password").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "password", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="qrsNum")
     def qrs_num(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property: qrsNum: The number of query nodes.
         '''
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "qrsNum"))
 
     @qrs_num.setter
     def qrs_num(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "qrs_num").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "qrsNum", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="qrsSpec")
     def qrs_spec(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: qrsSpec: The specification of query nodes.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "qrsSpec"))
 
     @qrs_spec.setter
     def qrs_spec(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "qrs_spec").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "qrsSpec", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="searcherDocSize")
     def searcher_doc_size(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property: searcherDocSize: The storage size of single data node.
         '''
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "searcherDocSize"))
 
     @searcher_doc_size.setter
     def searcher_doc_size(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "searcher_doc_size").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "searcherDocSize", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="searcherNum")
     def searcher_num(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property: searcherNum: The number of data nodes.
         '''
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "searcherNum"))
 
     @searcher_num.setter
     def searcher_num(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "searcher_num").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "searcherNum", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="searcherSpec")
     def searcher_spec(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: searcherSpec: The specification of data nodes.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "searcherSpec"))
 
     @searcher_spec.setter
     def searcher_spec(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "searcher_spec").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "searcherSpec", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="userName")
     def user_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: userName: The user name of instance. Begin with a letter, support upper and lower case letters, numbers, underscores, length 1-30 characters.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "userName"))
 
     @user_name.setter
     def user_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "user_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "userName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vpcId")
     def vpc_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: vpcId: The ID of VPC.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "vpcId"))
 
     @vpc_id.setter
     def vpc_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "vpc_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vpcId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vSwitchId")
     def v_switch_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: vSwitchId: The ID of vSwitch.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "vSwitchId"))
 
     @v_switch_id.setter
     def v_switch_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "v_switch_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vSwitchId", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-searchengine.RosInstanceProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -474,14 +536,26 @@
         :param searcher_doc_size: 
         :param searcher_num: 
         :param searcher_spec: 
         :param user_name: 
         :param vpc_id: 
         :param v_switch_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosInstanceProps.__init__)
+            check_type(argname="argument charge_type", value=charge_type, expected_type=type_hints["charge_type"])
+            check_type(argname="argument password", value=password, expected_type=type_hints["password"])
+            check_type(argname="argument qrs_num", value=qrs_num, expected_type=type_hints["qrs_num"])
+            check_type(argname="argument qrs_spec", value=qrs_spec, expected_type=type_hints["qrs_spec"])
+            check_type(argname="argument searcher_doc_size", value=searcher_doc_size, expected_type=type_hints["searcher_doc_size"])
+            check_type(argname="argument searcher_num", value=searcher_num, expected_type=type_hints["searcher_num"])
+            check_type(argname="argument searcher_spec", value=searcher_spec, expected_type=type_hints["searcher_spec"])
+            check_type(argname="argument user_name", value=user_name, expected_type=type_hints["user_name"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "charge_type": charge_type,
             "password": password,
             "qrs_num": qrs_num,
             "qrs_spec": qrs_spec,
             "searcher_doc_size": searcher_doc_size,
             "searcher_num": searcher_num,
```

### Comparing `ros-cdk-searchengine-1.0.8/src/ros_cdk_searchengine.egg-info/PKG-INFO` & `ros-cdk-searchengine-1.0.9/src/ros_cdk_searchengine.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-searchengine
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS SEARCHENGINE Construct Library
```

