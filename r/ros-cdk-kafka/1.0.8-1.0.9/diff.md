# Comparing `tmp/ros-cdk-kafka-1.0.8.tar.gz` & `tmp/ros-cdk-kafka-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-kafka-1.0.8.tar", last modified: Thu Jul 14 02:20:14 2022, max compression
+gzip compressed data, was "dist/ros-cdk-kafka-1.0.9.tar", last modified: Fri Sep 23 11:29:58 2022, max compression
```

## Comparing `ros-cdk-kafka-1.0.8.tar` & `ros-cdk-kafka-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:20:14.000000 ros-cdk-kafka-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:20:14.000000 ros-cdk-kafka-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:20:14.000000 ros-cdk-kafka-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:20:14.000000 ros-cdk-kafka-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1248 2022-07-14 02:20:14.000000 ros-cdk-kafka-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      185 2022-07-14 02:20:14.000000 ros-cdk-kafka-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:20:14.000000 ros-cdk-kafka-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:20:14.000000 ros-cdk-kafka-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1806 2022-07-14 02:20:14.000000 ros-cdk-kafka-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:20:14.000000 ros-cdk-kafka-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:20:14.000000 ros-cdk-kafka-1.0.8/src/ros_cdk_kafka/
--rw-r--r--   0 root         (0) root         (0)    89600 2022-07-14 02:20:14.000000 ros-cdk-kafka-1.0.8/src/ros_cdk_kafka/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:20:14.000000 ros-cdk-kafka-1.0.8/src/ros_cdk_kafka/_jsii/
--rw-r--r--   0 root         (0) root         (0)      374 2022-07-14 02:20:14.000000 ros-cdk-kafka-1.0.8/src/ros_cdk_kafka/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    57700 2022-07-14 02:20:14.000000 ros-cdk-kafka-1.0.8/src/ros_cdk_kafka/_jsii/ros-cdk-kafka@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:20:14.000000 ros-cdk-kafka-1.0.8/src/ros_cdk_kafka/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:20:14.000000 ros-cdk-kafka-1.0.8/src/ros_cdk_kafka.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1248 2022-07-14 02:20:14.000000 ros-cdk-kafka-1.0.8/src/ros_cdk_kafka.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2022-07-14 02:20:14.000000 ros-cdk-kafka-1.0.8/src/ros_cdk_kafka.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:20:14.000000 ros-cdk-kafka-1.0.8/src/ros_cdk_kafka.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:20:14.000000 ros-cdk-kafka-1.0.8/src/ros_cdk_kafka.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2022-07-14 02:20:14.000000 ros-cdk-kafka-1.0.8/src/ros_cdk_kafka.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:29:58.000000 ros-cdk-kafka-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 11:29:58.000000 ros-cdk-kafka-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 11:29:58.000000 ros-cdk-kafka-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 11:29:58.000000 ros-cdk-kafka-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1248 2022-09-23 11:29:58.000000 ros-cdk-kafka-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      185 2022-09-23 11:29:58.000000 ros-cdk-kafka-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 11:29:58.000000 ros-cdk-kafka-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 11:29:58.000000 ros-cdk-kafka-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1835 2022-09-23 11:29:58.000000 ros-cdk-kafka-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:29:58.000000 ros-cdk-kafka-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:29:58.000000 ros-cdk-kafka-1.0.9/src/ros_cdk_kafka/
+-rw-r--r--   0 root         (0) root         (0)   104545 2022-09-23 11:29:58.000000 ros-cdk-kafka-1.0.9/src/ros_cdk_kafka/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:29:58.000000 ros-cdk-kafka-1.0.9/src/ros_cdk_kafka/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      408 2022-09-23 11:29:58.000000 ros-cdk-kafka-1.0.9/src/ros_cdk_kafka/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    57772 2022-09-23 11:29:58.000000 ros-cdk-kafka-1.0.9/src/ros_cdk_kafka/_jsii/ros-cdk-kafka@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:29:58.000000 ros-cdk-kafka-1.0.9/src/ros_cdk_kafka/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:29:58.000000 ros-cdk-kafka-1.0.9/src/ros_cdk_kafka.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1248 2022-09-23 11:29:58.000000 ros-cdk-kafka-1.0.9/src/ros_cdk_kafka.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2022-09-23 11:29:58.000000 ros-cdk-kafka-1.0.9/src/ros_cdk_kafka.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:29:58.000000 ros-cdk-kafka-1.0.9/src/ros_cdk_kafka.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 11:29:58.000000 ros-cdk-kafka-1.0.9/src/ros_cdk_kafka.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2022-09-23 11:29:58.000000 ros-cdk-kafka-1.0.9/src/ros_cdk_kafka.egg-info/top_level.txt
```

### Comparing `ros-cdk-kafka-1.0.8/LICENSE` & `ros-cdk-kafka-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-kafka-1.0.8/PKG-INFO` & `ros-cdk-kafka-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-kafka
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS KAFKA Construct Library
```

### Comparing `ros-cdk-kafka-1.0.8/setup.py` & `ros-cdk-kafka-1.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-kafka",
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
         "ros_cdk_kafka",
         "ros_cdk_kafka._jsii"
     ],
     "package_data": {
         "ros_cdk_kafka._jsii": [
-            "ros-cdk-kafka@1.0.8.jsii.tgz"
+            "ros-cdk-kafka@1.0.9.jsii.tgz"
         ],
         "ros_cdk_kafka": [
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

### Comparing `ros-cdk-kafka-1.0.8/src/ros_cdk_kafka/__init__.py` & `ros-cdk-kafka-1.0.9/src/ros_cdk_kafka/__init__.py`

 * *Files 13% similar despite different names*

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
@@ -29,73 +31,79 @@
 ):
     '''A ROS resource type:  ``ALIYUN::KAFKA::Instance``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "InstanceProps",
+        props: typing.Union["InstanceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::KAFKA::Instance``.
 
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
     @jsii.member(jsii_name="attrDomainEndpoint")
     def attr_domain_endpoint(self) -> ros_cdk_core.IResolvable:
         '''Attribute DomainEndpoint: The default endpoints of the instance in domain name mode.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDomainEndpoint"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrEndpoint")
     def attr_endpoint(self) -> ros_cdk_core.IResolvable:
         '''Attribute Endpoint: The SSL endpoints of the instance in IP address mode.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrEndpoint"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceId")
     def attr_instance_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute InstanceId: Id of the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrName")
     def attr_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute Name: Name of the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrOrderId")
     def attr_order_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute OrderId: Id of the order.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrOrderId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSaslDomainEndpoint")
     def attr_sasl_domain_endpoint(self) -> ros_cdk_core.IResolvable:
         '''Attribute SaslDomainEndpoint: The Simple Authentication and Security Layer (SASL) endpoints of the instance in domain name mode.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSaslDomainEndpoint"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSslDomainEndpoint")
     def attr_ssl_domain_endpoint(self) -> ros_cdk_core.IResolvable:
         '''Attribute SslDomainEndpoint: The SSL endpoints of the instance in domain name mode.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSslDomainEndpoint"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSslEndpoint")
     def attr_ssl_endpoint(self) -> ros_cdk_core.IResolvable:
         '''Attribute SslEndpoint: The SSL endpoints of the instance in IP address mode.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSslEndpoint"))
 
 
 @jsii.data_type(
@@ -122,22 +130,22 @@
         self,
         *,
         deploy_type: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
         disk_size: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
         disk_type: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         topic_quota: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
         deletion_force: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
-        deploy_option: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosInstance.DeployOptionProperty"]] = None,
+        deploy_option: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosInstance.DeployOptionProperty", typing.Dict[str, typing.Any]]]] = None,
         eip_max: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         io_max: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         io_max_spec: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         open_connector: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         pay_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         spec_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence["RosInstance.TagsProperty"]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union["RosInstance.TagsProperty", typing.Dict[str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::KAFKA::Instance``.
 
         :param deploy_type: Property deployType: The deployment mode of the Message Queue for Apache Kafka instance. Valid values: 4: Instance of the public type 5: Instance of the VPC type
         :param disk_size: Property diskSize: The size of the disk to be configured for the Message Queue for Apache Kafka instance.
         :param disk_type: Property diskType: The type of the disk to be configured for the Message Queue for Apache Kafka instance. Valid values: 0: Ultra disk 1: SSD
         :param topic_quota: Property topicQuota: The number of topics to be configured for the Message Queue for Apache Kafka instance. The default value of this parameter varies with different peak traffic values. Additional fees are charged if the default values are exceeded. Different specifications have different default values, and extra fees are charged. For more information, see Billing.
@@ -147,14 +155,29 @@
         :param io_max: Property ioMax: The peak traffic to be configured for the Message Queue for Apache Kafka instance. For more information about the value range, see Billing.
         :param io_max_spec: Property ioMaxSpec: Flow specification (recommended) The IoMax and IoMaxSpec must be optional. When filling in at the same time, subject to IoMaxSpec. It is recommended that you only fill in the flow specification
         :param open_connector: Property openConnector: Whether open kafka connector or not.
         :param pay_type: Property payType: Pay by hour or month.
         :param spec_type: Property specType: The edition of the Message Queue for Apache Kafka instance. Valid values: professional: Professional Edition normal: Normal version
         :param tags: Property tags: Tags to attach to instance. Max support 20 tags to add during create instance. Each tag with two properties Key and Value, and Key is required.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(InstanceProps.__init__)
+            check_type(argname="argument deploy_type", value=deploy_type, expected_type=type_hints["deploy_type"])
+            check_type(argname="argument disk_size", value=disk_size, expected_type=type_hints["disk_size"])
+            check_type(argname="argument disk_type", value=disk_type, expected_type=type_hints["disk_type"])
+            check_type(argname="argument topic_quota", value=topic_quota, expected_type=type_hints["topic_quota"])
+            check_type(argname="argument deletion_force", value=deletion_force, expected_type=type_hints["deletion_force"])
+            check_type(argname="argument deploy_option", value=deploy_option, expected_type=type_hints["deploy_option"])
+            check_type(argname="argument eip_max", value=eip_max, expected_type=type_hints["eip_max"])
+            check_type(argname="argument io_max", value=io_max, expected_type=type_hints["io_max"])
+            check_type(argname="argument io_max_spec", value=io_max_spec, expected_type=type_hints["io_max_spec"])
+            check_type(argname="argument open_connector", value=open_connector, expected_type=type_hints["open_connector"])
+            check_type(argname="argument pay_type", value=pay_type, expected_type=type_hints["pay_type"])
+            check_type(argname="argument spec_type", value=spec_type, expected_type=type_hints["spec_type"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
         self._values: typing.Dict[str, typing.Any] = {
             "deploy_type": deploy_type,
             "disk_size": disk_size,
             "disk_type": disk_type,
             "topic_quota": topic_quota,
         }
         if deletion_force is not None:
@@ -330,112 +353,121 @@
 ):
     '''A ROS template type:  ``ALIYUN::KAFKA::Instance``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosInstanceProps",
+        props: typing.Union["RosInstanceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::KAFKA::Instance``.
 
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
     @jsii.member(jsii_name="attrDomainEndpoint")
     def attr_domain_endpoint(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DomainEndpoint: The default endpoints of the instance in domain name mode.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDomainEndpoint"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrEndpoint")
     def attr_endpoint(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Endpoint: The SSL endpoints of the instance in IP address mode.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrEndpoint"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceId")
     def attr_instance_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: InstanceId: Id of the instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrName")
     def attr_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Name: Name of the instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrOrderId")
     def attr_order_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: OrderId: Id of the order.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrOrderId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSaslDomainEndpoint")
     def attr_sasl_domain_endpoint(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: SaslDomainEndpoint: The Simple Authentication and Security Layer (SASL) endpoints of the instance in domain name mode.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSaslDomainEndpoint"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSslDomainEndpoint")
     def attr_ssl_domain_endpoint(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: SslDomainEndpoint: The SSL endpoints of the instance in domain name mode.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSslDomainEndpoint"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSslEndpoint")
     def attr_ssl_endpoint(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: SslEndpoint: The SSL endpoints of the instance in IP address mode.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSslEndpoint"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="deployType")
     def deploy_type(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         deployType: The deployment mode of the Message Queue for Apache Kafka instance. Valid values:
         4: Instance of the public type
@@ -444,32 +476,38 @@
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "deployType"))
 
     @deploy_type.setter
     def deploy_type(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "deploy_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "deployType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="diskSize")
     def disk_size(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property: diskSize: The size of the disk to be configured for the Message Queue for Apache Kafka instance.
         '''
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "diskSize"))
 
     @disk_size.setter
     def disk_size(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "disk_size").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "diskSize", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="diskType")
     def disk_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         diskType: The type of the disk to be configured for the Message Queue for Apache Kafka instance. Valid values:
         0: Ultra disk
@@ -478,26 +516,32 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "diskType"))
 
     @disk_type.setter
     def disk_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "disk_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "diskType", value)
 
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
     @jsii.member(jsii_name="topicQuota")
     def topic_quota(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         topicQuota: The number of topics to be configured for the Message Queue for Apache Kafka instance.
         The default value of this parameter varies with different peak traffic values.
@@ -508,51 +552,60 @@
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "topicQuota"))
 
     @topic_quota.setter
     def topic_quota(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "topic_quota").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "topicQuota", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="deletionForce")
     def deletion_force(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: deletionForce: Whether delete all topics, consumer groups of the kafka instance and then delete instance. Default is false
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "deletionForce"))
 
     @deletion_force.setter
     def deletion_force(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "deletion_force").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "deletionForce", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="deployOption")
     def deploy_option(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosInstance.DeployOptionProperty"]]:
         '''
         :Property: deployOption: If you want to deploy instance after create at once, the VSwitchId and DeployModule parameters is required
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosInstance.DeployOptionProperty"]], jsii.get(self, "deployOption"))
 
     @deploy_option.setter
     def deploy_option(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosInstance.DeployOptionProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "deploy_option").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "deployOption", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="eipMax")
     def eip_max(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -562,17 +615,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "eipMax"))
 
     @eip_max.setter
     def eip_max(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "eip_max").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "eipMax", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="ioMax")
     def io_max(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -582,17 +638,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "ioMax"))
 
     @io_max.setter
     def io_max(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "io_max").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ioMax", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="ioMaxSpec")
     def io_max_spec(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -604,51 +663,60 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "ioMaxSpec"))
 
     @io_max_spec.setter
     def io_max_spec(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "io_max_spec").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ioMaxSpec", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="openConnector")
     def open_connector(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: openConnector: Whether open kafka connector or not
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "openConnector"))
 
     @open_connector.setter
     def open_connector(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "open_connector").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "openConnector", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="payType")
     def pay_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: payType: Pay by hour or month.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "payType"))
 
     @pay_type.setter
     def pay_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "pay_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "payType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="specType")
     def spec_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -659,29 +727,35 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "specType"))
 
     @spec_type.setter
     def spec_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "spec_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "specType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tags")
     def tags(self) -> typing.Optional[typing.List["RosInstance.TagsProperty"]]:
         '''
         :Property: tags: Tags to attach to instance. Max support 20 tags to add during create instance. Each tag with two properties Key and Value, and Key is required.
         '''
         return typing.cast(typing.Optional[typing.List["RosInstance.TagsProperty"]], jsii.get(self, "tags"))
 
     @tags.setter
     def tags(
         self,
         value: typing.Optional[typing.List["RosInstance.TagsProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "tags").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tags", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-kafka.RosInstance.DeployOptionProperty",
         jsii_struct_bases=[],
         name_mapping={
             "deploy_module": "deployModule",
@@ -725,14 +799,28 @@
             :param password: 
             :param security_group: 
             :param service_version: 
             :param username: 
             :param vpc_id: 
             :param zone_id: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosInstance.DeployOptionProperty.__init__)
+                check_type(argname="argument deploy_module", value=deploy_module, expected_type=type_hints["deploy_module"])
+                check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
+                check_type(argname="argument config", value=config, expected_type=type_hints["config"])
+                check_type(argname="argument is_eip_inner", value=is_eip_inner, expected_type=type_hints["is_eip_inner"])
+                check_type(argname="argument is_set_user_and_password", value=is_set_user_and_password, expected_type=type_hints["is_set_user_and_password"])
+                check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+                check_type(argname="argument password", value=password, expected_type=type_hints["password"])
+                check_type(argname="argument security_group", value=security_group, expected_type=type_hints["security_group"])
+                check_type(argname="argument service_version", value=service_version, expected_type=type_hints["service_version"])
+                check_type(argname="argument username", value=username, expected_type=type_hints["username"])
+                check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+                check_type(argname="argument zone_id", value=zone_id, expected_type=type_hints["zone_id"])
             self._values: typing.Dict[str, typing.Any] = {
                 "deploy_module": deploy_module,
                 "v_switch_id": v_switch_id,
             }
             if config is not None:
                 self._values["config"] = config
             if is_eip_inner is not None:
@@ -944,14 +1032,18 @@
             key: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param key: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosInstance.TagsProperty.__init__)
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {
                 "key": key,
             }
             if value is not None:
                 self._values["value"] = value
 
         @builtins.property
@@ -1009,22 +1101,22 @@
         self,
         *,
         deploy_type: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
         disk_size: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
         disk_type: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         topic_quota: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
         deletion_force: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
-        deploy_option: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosInstance.DeployOptionProperty]] = None,
+        deploy_option: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosInstance.DeployOptionProperty, typing.Dict[str, typing.Any]]]] = None,
         eip_max: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         io_max: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         io_max_spec: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         open_connector: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         pay_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         spec_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence[RosInstance.TagsProperty]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union[RosInstance.TagsProperty, typing.Dict[str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::KAFKA::Instance``.
 
         :param deploy_type: 
         :param disk_size: 
         :param disk_type: 
         :param topic_quota: 
@@ -1034,14 +1126,29 @@
         :param io_max: 
         :param io_max_spec: 
         :param open_connector: 
         :param pay_type: 
         :param spec_type: 
         :param tags: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosInstanceProps.__init__)
+            check_type(argname="argument deploy_type", value=deploy_type, expected_type=type_hints["deploy_type"])
+            check_type(argname="argument disk_size", value=disk_size, expected_type=type_hints["disk_size"])
+            check_type(argname="argument disk_type", value=disk_type, expected_type=type_hints["disk_type"])
+            check_type(argname="argument topic_quota", value=topic_quota, expected_type=type_hints["topic_quota"])
+            check_type(argname="argument deletion_force", value=deletion_force, expected_type=type_hints["deletion_force"])
+            check_type(argname="argument deploy_option", value=deploy_option, expected_type=type_hints["deploy_option"])
+            check_type(argname="argument eip_max", value=eip_max, expected_type=type_hints["eip_max"])
+            check_type(argname="argument io_max", value=io_max, expected_type=type_hints["io_max"])
+            check_type(argname="argument io_max_spec", value=io_max_spec, expected_type=type_hints["io_max_spec"])
+            check_type(argname="argument open_connector", value=open_connector, expected_type=type_hints["open_connector"])
+            check_type(argname="argument pay_type", value=pay_type, expected_type=type_hints["pay_type"])
+            check_type(argname="argument spec_type", value=spec_type, expected_type=type_hints["spec_type"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
         self._values: typing.Dict[str, typing.Any] = {
             "deploy_type": deploy_type,
             "disk_size": disk_size,
             "disk_type": disk_type,
             "topic_quota": topic_quota,
         }
         if deletion_force is not None:
@@ -1235,76 +1342,88 @@
 ):
     '''A ROS template type:  ``ALIYUN::KAFKA::Topic``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosTopicProps",
+        props: typing.Union["RosTopicProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::KAFKA::Topic``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosTopic.__init__)
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
+            type_hints = typing.get_type_hints(RosTopic._render_properties)
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
         :Attribute:
 
         InstanceId: The ID of the Message Queue for Apache Kafka instance where the topic is located.
         You can call the GetInstanceList operation to query instances.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTopic")
     def attr_topic(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Topic: Topic name.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTopic"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosTopic, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceId")
     def instance_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         instanceId: The ID of the Message Queue for Apache Kafka instance where the topic is located.
         You can call the GetInstanceList operation to query instances.
@@ -1312,17 +1431,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "instanceId"))
 
     @instance_id.setter
     def instance_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTopic, "instance_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="remark")
     def remark(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         remark: The description of the topic. The value of this parameter must meet the following
         requirements:
@@ -1332,17 +1454,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "remark"))
 
     @remark.setter
     def remark(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTopic, "remark").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "remark", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="topic")
     def topic(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         topic: The name of the topic. The value of this parameter must meet the following requirements:
         The name can only contain letters, digits, hyphens (-), and underscores (_).
@@ -1353,17 +1478,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "topic"))
 
     @topic.setter
     def topic(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTopic, "topic").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "topic", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="compactTopic")
     def compact_topic(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1374,17 +1502,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "compactTopic"))
 
     @compact_topic.setter
     def compact_topic(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTopic, "compact_topic").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "compactTopic", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="config")
     def config(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]]:
         '''
         :Property:
 
@@ -1396,17 +1527,20 @@
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]], jsii.get(self, "config"))
 
     @config.setter
     def config(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTopic, "config").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "config", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="localTopic")
     def local_topic(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1417,17 +1551,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "localTopic"))
 
     @local_topic.setter
     def local_topic(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTopic, "local_topic").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "localTopic", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="minInsyncReplicas")
     def min_insync_replicas(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1439,17 +1576,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "minInsyncReplicas"))
 
     @min_insync_replicas.setter
     def min_insync_replicas(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTopic, "min_insync_replicas").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "minInsyncReplicas", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="partitionNum")
     def partition_num(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1461,17 +1601,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "partitionNum"))
 
     @partition_num.setter
     def partition_num(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTopic, "partition_num").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "partitionNum", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="replicationFactor")
     def replication_factor(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1483,29 +1626,35 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "replicationFactor"))
 
     @replication_factor.setter
     def replication_factor(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTopic, "replication_factor").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "replicationFactor", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tags")
     def tags(self) -> typing.Optional[typing.List["RosTopic.TagsProperty"]]:
         '''
         :Property: tags: Tags to attach to instance. Max support 20 tags to add during create instance. Each tag with two properties Key and Value, and Key is required.
         '''
         return typing.cast(typing.Optional[typing.List["RosTopic.TagsProperty"]], jsii.get(self, "tags"))
 
     @tags.setter
     def tags(
         self,
         value: typing.Optional[typing.List["RosTopic.TagsProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTopic, "tags").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tags", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-kafka.RosTopic.TagsProperty",
         jsii_struct_bases=[],
         name_mapping={"key": "key", "value": "value"},
     )
@@ -1516,14 +1665,18 @@
             key: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param key: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosTopic.TagsProperty.__init__)
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {
                 "key": key,
             }
             if value is not None:
                 self._values["value"] = value
 
         @builtins.property
@@ -1582,29 +1735,41 @@
         topic: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         compact_topic: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]] = None,
         local_topic: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         min_insync_replicas: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         partition_num: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         replication_factor: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence[RosTopic.TagsProperty]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union[RosTopic.TagsProperty, typing.Dict[str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::KAFKA::Topic``.
 
         :param instance_id: 
         :param remark: 
         :param topic: 
         :param compact_topic: 
         :param config: 
         :param local_topic: 
         :param min_insync_replicas: 
         :param partition_num: 
         :param replication_factor: 
         :param tags: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosTopicProps.__init__)
+            check_type(argname="argument instance_id", value=instance_id, expected_type=type_hints["instance_id"])
+            check_type(argname="argument remark", value=remark, expected_type=type_hints["remark"])
+            check_type(argname="argument topic", value=topic, expected_type=type_hints["topic"])
+            check_type(argname="argument compact_topic", value=compact_topic, expected_type=type_hints["compact_topic"])
+            check_type(argname="argument config", value=config, expected_type=type_hints["config"])
+            check_type(argname="argument local_topic", value=local_topic, expected_type=type_hints["local_topic"])
+            check_type(argname="argument min_insync_replicas", value=min_insync_replicas, expected_type=type_hints["min_insync_replicas"])
+            check_type(argname="argument partition_num", value=partition_num, expected_type=type_hints["partition_num"])
+            check_type(argname="argument replication_factor", value=replication_factor, expected_type=type_hints["replication_factor"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
         self._values: typing.Dict[str, typing.Any] = {
             "instance_id": instance_id,
             "remark": remark,
             "topic": topic,
         }
         if compact_topic is not None:
             self._values["compact_topic"] = compact_topic
@@ -1777,40 +1942,46 @@
 ):
     '''A ROS resource type:  ``ALIYUN::KAFKA::Topic``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "TopicProps",
+        props: typing.Union["TopicProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::KAFKA::Topic``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Topic.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceId")
     def attr_instance_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute InstanceId: The ID of the Message Queue for Apache Kafka instance where the topic is located.
 
         You can call the GetInstanceList operation to query instances.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTopic")
     def attr_topic(self) -> ros_cdk_core.IResolvable:
         '''Attribute Topic: Topic name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTopic"))
 
 
 @jsii.data_type(
@@ -1838,29 +2009,41 @@
         topic: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         compact_topic: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]] = None,
         local_topic: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         min_insync_replicas: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         partition_num: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         replication_factor: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence[RosTopic.TagsProperty]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union[RosTopic.TagsProperty, typing.Dict[str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::KAFKA::Topic``.
 
         :param instance_id: Property instanceId: The ID of the Message Queue for Apache Kafka instance where the topic is located. You can call the GetInstanceList operation to query instances.
         :param remark: Property remark: The description of the topic. The value of this parameter must meet the following requirements: The value can only contain letters, digits, hyphens (-), and underscores (_). The value must be 3 to 64 characters in length.
         :param topic: Property topic: The name of the topic. The value of this parameter must meet the following requirements: The name can only contain letters, digits, hyphens (-), and underscores (_). The name must be 3 to 64 characters in length, and will be automatically truncated if it contains more characters. The name cannot be modified after being created.
         :param compact_topic: Property compactTopic: The log cleanup policy for the topic. This parameter is available when the Local Storage mode is specified for the topic. Valid values: false: uses the default log cleanup policy. true: uses the Apache Kafka log compaction policy.
         :param config: Property config: Supplementary configuration. Currently supports Key as replications. Indicates the number of Topic copies, the value type is Integer, and the value limit is 1~3. This parameter can only be specified if the LocalTopic value is true. NOTE If replications is specified in this parameter, the specified ReplicationFactor parameter no longer takes effect.
         :param local_topic: Property localTopic: The storage engine of the topic. Valid values: false: the Cloud Storage mode. true: the Local Storage mode.
         :param min_insync_replicas: Property minInsyncReplicas: The minimum number of ISR sync replicas. This parameter can only be specified if the LocalTopic value is true. The value must be less than the number of Topic copies. The number of synchronous replicas is limited to 1~3.
         :param partition_num: Property partitionNum: The number of partitions in the topic. Valid values: 1 to 48 We recommend that you set the number of partitions to a multiple of 6 to reduce the risk of data skew.Note:For special requirements,submit a ticket.
         :param replication_factor: Property replicationFactor: The number of copies of the topic. This parameter can only be specified if the LocalTopic value is true. The number of copies is limited to 1~3. Note When the number of replicas is 1, there is a risk of data loss. Please set it carefully.
         :param tags: Property tags: Tags to attach to instance. Max support 20 tags to add during create instance. Each tag with two properties Key and Value, and Key is required.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(TopicProps.__init__)
+            check_type(argname="argument instance_id", value=instance_id, expected_type=type_hints["instance_id"])
+            check_type(argname="argument remark", value=remark, expected_type=type_hints["remark"])
+            check_type(argname="argument topic", value=topic, expected_type=type_hints["topic"])
+            check_type(argname="argument compact_topic", value=compact_topic, expected_type=type_hints["compact_topic"])
+            check_type(argname="argument config", value=config, expected_type=type_hints["config"])
+            check_type(argname="argument local_topic", value=local_topic, expected_type=type_hints["local_topic"])
+            check_type(argname="argument min_insync_replicas", value=min_insync_replicas, expected_type=type_hints["min_insync_replicas"])
+            check_type(argname="argument partition_num", value=partition_num, expected_type=type_hints["partition_num"])
+            check_type(argname="argument replication_factor", value=replication_factor, expected_type=type_hints["replication_factor"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
         self._values: typing.Dict[str, typing.Any] = {
             "instance_id": instance_id,
             "remark": remark,
             "topic": topic,
         }
         if compact_topic is not None:
             self._values["compact_topic"] = compact_topic
```

### Comparing `ros-cdk-kafka-1.0.8/src/ros_cdk_kafka.egg-info/PKG-INFO` & `ros-cdk-kafka-1.0.9/src/ros_cdk_kafka.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-kafka
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS KAFKA Construct Library
```

