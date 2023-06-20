# Comparing `tmp/ros-cdk-ros-1.0.8.tar.gz` & `tmp/ros-cdk-ros-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-ros-1.0.8.tar", last modified: Thu Jul 14 02:22:16 2022, max compression
+gzip compressed data, was "dist/ros-cdk-ros-1.0.9.tar", last modified: Fri Sep 23 12:03:01 2022, max compression
```

## Comparing `ros-cdk-ros-1.0.8.tar` & `ros-cdk-ros-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:22:16.000000 ros-cdk-ros-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:22:15.000000 ros-cdk-ros-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:22:15.000000 ros-cdk-ros-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:22:15.000000 ros-cdk-ros-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:22:16.000000 ros-cdk-ros-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      179 2022-07-14 02:22:15.000000 ros-cdk-ros-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:22:15.000000 ros-cdk-ros-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:22:16.000000 ros-cdk-ros-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1794 2022-07-14 02:22:15.000000 ros-cdk-ros-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:22:16.000000 ros-cdk-ros-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:22:16.000000 ros-cdk-ros-1.0.8/src/ros_cdk_ros/
--rw-r--r--   0 root         (0) root         (0)   241738 2022-07-14 02:22:15.000000 ros-cdk-ros-1.0.8/src/ros_cdk_ros/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:22:16.000000 ros-cdk-ros-1.0.8/src/ros_cdk_ros/_jsii/
--rw-r--r--   0 root         (0) root         (0)      370 2022-07-14 02:22:15.000000 ros-cdk-ros-1.0.8/src/ros_cdk_ros/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)   114078 2022-07-14 02:22:15.000000 ros-cdk-ros-1.0.8/src/ros_cdk_ros/_jsii/ros-cdk-ros@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:22:15.000000 ros-cdk-ros-1.0.8/src/ros_cdk_ros/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:22:16.000000 ros-cdk-ros-1.0.8/src/ros_cdk_ros.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:22:16.000000 ros-cdk-ros-1.0.8/src/ros_cdk_ros.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      400 2022-07-14 02:22:16.000000 ros-cdk-ros-1.0.8/src/ros_cdk_ros.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:22:16.000000 ros-cdk-ros-1.0.8/src/ros_cdk_ros.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:22:16.000000 ros-cdk-ros-1.0.8/src/ros_cdk_ros.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-07-14 02:22:16.000000 ros-cdk-ros-1.0.8/src/ros_cdk_ros.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:03:01.000000 ros-cdk-ros-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 12:03:01.000000 ros-cdk-ros-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 12:03:01.000000 ros-cdk-ros-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 12:03:01.000000 ros-cdk-ros-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 12:03:01.000000 ros-cdk-ros-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      179 2022-09-23 12:03:01.000000 ros-cdk-ros-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 12:03:01.000000 ros-cdk-ros-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 12:03:01.000000 ros-cdk-ros-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1823 2022-09-23 12:03:01.000000 ros-cdk-ros-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:03:01.000000 ros-cdk-ros-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:03:01.000000 ros-cdk-ros-1.0.9/src/ros_cdk_ros/
+-rw-r--r--   0 root         (0) root         (0)   287213 2022-09-23 12:03:01.000000 ros-cdk-ros-1.0.9/src/ros_cdk_ros/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:03:01.000000 ros-cdk-ros-1.0.9/src/ros_cdk_ros/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      404 2022-09-23 12:03:01.000000 ros-cdk-ros-1.0.9/src/ros_cdk_ros/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   113826 2022-09-23 12:03:01.000000 ros-cdk-ros-1.0.9/src/ros_cdk_ros/_jsii/ros-cdk-ros@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 12:03:01.000000 ros-cdk-ros-1.0.9/src/ros_cdk_ros/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:03:01.000000 ros-cdk-ros-1.0.9/src/ros_cdk_ros.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 12:03:01.000000 ros-cdk-ros-1.0.9/src/ros_cdk_ros.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      400 2022-09-23 12:03:01.000000 ros-cdk-ros-1.0.9/src/ros_cdk_ros.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 12:03:01.000000 ros-cdk-ros-1.0.9/src/ros_cdk_ros.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 12:03:01.000000 ros-cdk-ros-1.0.9/src/ros_cdk_ros.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-09-23 12:03:01.000000 ros-cdk-ros-1.0.9/src/ros_cdk_ros.egg-info/top_level.txt
```

### Comparing `ros-cdk-ros-1.0.8/LICENSE` & `ros-cdk-ros-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-ros-1.0.8/PKG-INFO` & `ros-cdk-ros-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-ros
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS ROS Construct Library
```

### Comparing `ros-cdk-ros-1.0.8/setup.py` & `ros-cdk-ros-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-ros",
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
         "ros_cdk_ros",
         "ros_cdk_ros._jsii"
     ],
     "package_data": {
         "ros_cdk_ros._jsii": [
-            "ros-cdk-ros@1.0.8.jsii.tgz"
+            "ros-cdk-ros@1.0.9.jsii.tgz"
         ],
         "ros_cdk_ros": [
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

### Comparing `ros-cdk-ros-1.0.8/src/ros_cdk_ros/__init__.py` & `ros-cdk-ros-1.0.9/src/ros_cdk_ros/__init__.py`

 * *Files 19% similar despite different names*

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
 
 
 class AutoEnableService(
     ros_cdk_core.Resource,
@@ -29,28 +31,34 @@
 ):
     '''A ROS resource type:  ``ALIYUN::ROS::AutoEnableService``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "AutoEnableServiceProps",
+        props: typing.Union["AutoEnableServiceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::ROS::AutoEnableService``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(AutoEnableService.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-ros.AutoEnableServiceProps",
     jsii_struct_bases=[],
     name_mapping={"service_name": "serviceName"},
@@ -61,14 +69,17 @@
         *,
         service_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::ROS::AutoEnableService``.
 
         :param service_name: Property serviceName: Which service to enable. Valid values: AHAS: Application High Availability Service ARMS: Realtime Monitoring Service ApiGateway: API Gateway BatchCompute: Batch Compute BrainIndustrial: Brain Industrial CloudStorageGateway: Cloud Storage Gateway CMS: Cloud Monitor Service CR: Container Registry CS: Container Service DataHub: Data Hub DataWorks: DataWorks DCDN: Dynamic Route for CDN EDAS: Enterprise Distributed Application Service EMAS: Enterprise Mobile Application Studio FC: Function Compute FNF: Serverless Workflow MaxCompute: MaxCompute NAS: Network Attached Storage MNS: Message Service (MNS) HBR: Hybrid Backup Recovery IMM: Intelligent Media Management IOT: IoT Platform KMS: Key Management Service NLP: Natural Language Processing OSS: Object Storage Service OTS: Table Store PrivateLink: Private Link PrivateZone: Private Zone RocketMQ: RocketMQ SAE: Serverless App Engine SLS: Log Service TrafficMirror: VPC Traffic Mirroring VS: Video Surveillance Xtrace: Tracing Anlaysis
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(AutoEnableServiceProps.__init__)
+            check_type(argname="argument service_name", value=service_name, expected_type=type_hints["service_name"])
         self._values: typing.Dict[str, typing.Any] = {
             "service_name": service_name,
         }
 
     @builtins.property
     def service_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''Property serviceName: Which service to enable.
@@ -132,31 +143,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::ROS::CustomResource``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "CustomResourceProps",
+        props: typing.Union["CustomResourceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::ROS::CustomResource``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(CustomResource.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrOutputs")
     def attr_outputs(self) -> ros_cdk_core.IResolvable:
         '''Attribute Outputs: Output data received from service provider.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrOutputs"))
 
 
 @jsii.data_type(
@@ -171,24 +188,30 @@
 )
 class CustomResourceProps:
     def __init__(
         self,
         *,
         service_token: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         timeout: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
-        http_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosCustomResource.HttpConfigProperty"]] = None,
+        http_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosCustomResource.HttpConfigProperty", typing.Dict[str, typing.Any]]]] = None,
         parameters: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::ROS::CustomResource``.
 
         :param service_token: Property serviceToken: The service token that was given to the template developer by the service provider to access the service. Allowed values: - Function Compute: acs:fc:<region_id>:<account_id>:services/<service_name>/functions/<function_name> - MNS Queue: acs:mns:<region_id>:<account_id>:queues/<queue_name> or acs:mns:<region_id>:<account_id>:/queues/<queue_name> - MNS Topic: acs:mns:<region_id>:<account_id>:topics/<topic_name> or acs:mns:<region_id>:<account_id>:/topics/<topic_name> - HTTP&HTTPS: web[options]: Two options are supported: - sync: sync HTTP&HTTPS request. - idempotent: indicates that the Create request is idempotent. Update and Delete requests should be always idempotent. Examples: - acs:fc:cn-hangzhou:123456789:services/test-service/functions/test-function - acs:mns:cn-hangzhou:123456789:queues/test-queue - acs:mns:cn-hangzhou:123456789:/queues/test-queue - acs:mns:cn-hangzhou:123456789:topics/test-topic - acs:mns:cn-hangzhou:123456789:/topics/test-topic - web:https://abc.com - web[sync]:http://abc.com - web[sync,idempotent]:https://abc.com
         :param timeout: Property timeout: Timeout seconds before service provider responses. It takes effects only if the type of ServiceToken is Function Compute, MNS Queue, MNS Topic or async HTTP&HTTPS request. Timeout seconds are always 10 for sync HTTP&HTTPS request.
         :param http_config: Property httpConfig: Config for HTTP&HTTPS service provider.
         :param parameters: Property parameters: Parameters to be passed to service provider.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(CustomResourceProps.__init__)
+            check_type(argname="argument service_token", value=service_token, expected_type=type_hints["service_token"])
+            check_type(argname="argument timeout", value=timeout, expected_type=type_hints["timeout"])
+            check_type(argname="argument http_config", value=http_config, expected_type=type_hints["http_config"])
+            check_type(argname="argument parameters", value=parameters, expected_type=type_hints["parameters"])
         self._values: typing.Dict[str, typing.Any] = {
             "service_token": service_token,
             "timeout": timeout,
         }
         if http_config is not None:
             self._values["http_config"] = http_config
         if parameters is not None:
@@ -268,31 +291,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::ROS::ResourceCleaner``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "ResourceCleanerProps",
+        props: typing.Union["ResourceCleanerProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::ROS::ResourceCleaner``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ResourceCleaner.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCleanResult")
     def attr_clean_result(self) -> ros_cdk_core.IResolvable:
         '''Attribute CleanResult: The cleanup result.
 
         Valid values:
 
         - Success: All resources are cleaned up successfully.
@@ -301,35 +330,35 @@
         - CheckFailure: Pre check of cleanup fails.
         - UnknownFailure: Unexpected failure.
         - UserCancelled: Cleanup is cancelled by user.
         - None: Cleanup is not triggered.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCleanResult"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrNoCleanupResourceDetails")
     def attr_no_cleanup_resource_details(self) -> ros_cdk_core.IResolvable:
         '''Attribute NoCleanupResourceDetails: The details of the resources that are scanned but filtered.
 
         Only resources with the resource types ResourceCleaner supports and the regions not filtered are scanned.
         The format is the same as ResourceDetails.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrNoCleanupResourceDetails"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrNoCleanupResourcePartialDetails")
     def attr_no_cleanup_resource_partial_details(self) -> ros_cdk_core.IResolvable:
         '''Attribute NoCleanupResourcePartialDetails: The partial details of the resources that are scanned but filtered.
 
         Only resources with the resource types ResourceCleaner supports and the regions not filtered are scanned.
         The format is the same as ResourcePartialDetails.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrNoCleanupResourcePartialDetails"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrResourceDetails")
     def attr_resource_details(self) -> ros_cdk_core.IResolvable:
         '''Attribute ResourceDetails: The details of resources to be cleaned up.
 
         The value is a list of dict. The dict contains the fields below:
 
         - ResourceType: Resource type of the resource.
@@ -351,15 +380,15 @@
         - Dependencies: The resources that need to be deleted before the deletion of the resource. The value is a list of dict. The dict contains the fields below:
         - ResourceType: Resource type of the dependency resource.
         - RegionId: Region ID of the dependency resource.
         - ResourceId: ID of the dependency resource.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrResourceDetails"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrResourcePartialDetails")
     def attr_resource_partial_details(self) -> ros_cdk_core.IResolvable:
         '''Attribute ResourcePartialDetails: The partial details of resources to be cleaned up.
 
         The value is a list of dict. The dict contains the fields below:
 
         - ResourceType: Resource type of the resource.
@@ -372,15 +401,15 @@
         - Success: The resource is deleted.
         - Skipped: The deletion of the resource is skipped.
         - Pending: The deletion of the resource is not started.
         - ResourceStatusReason: The information of the related ResourceStatus.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrResourcePartialDetails"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrResourceSummary")
     def attr_resource_summary(self) -> ros_cdk_core.IResolvable:
         '''Attribute ResourceSummary: The details of resources to be cleaned up.
 
         The value is a list of dict. The dict contains the fields below:
 
         - ResourceType: Resource type of the resources.
@@ -390,15 +419,15 @@
         - SkippedCount: Number of skipped resources of the resource type.
         - PendingCount: Number of resources that have not been deleted of the resource type.
         - OtherCount: Number of other resources of the resource type.
         - TotalCount: Number of total resources of the resource type.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrResourceSummary"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScanErrors")
     def attr_scan_errors(self) -> ros_cdk_core.IResolvable:
         '''Attribute ScanErrors: The scan errors.
 
         It takes effect only when property Mode is Loose.
         The value is a list of dict. The dict contains the fields below:
 
@@ -431,19 +460,19 @@
         self,
         *,
         action: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         clean_up_algorithm: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         clean_up_retry_count: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         clean_up_timeout: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         disabled_side_effects: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
-        excluded_resources: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosResourceCleaner.ExcludedResourcesProperty"]]]] = None,
+        excluded_resources: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosResourceCleaner.ExcludedResourcesProperty", typing.Dict[str, typing.Any]]]]]] = None,
         failure_option: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         mode: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        resource_filters: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosResourceCleaner.ResourceFiltersProperty"]]]] = None,
-        resources: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosResourceCleaner.ResourcesProperty"]]]] = None,
+        resource_filters: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosResourceCleaner.ResourceFiltersProperty", typing.Dict[str, typing.Any]]]]]] = None,
+        resources: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosResourceCleaner.ResourcesProperty", typing.Dict[str, typing.Any]]]]]] = None,
         resource_type_order: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::ROS::ResourceCleaner``.
 
         :param action: Property action: Resource cleaner actions: - Scan: Scanning phase. Scan out the resources to be cleaned up. - CleanUp: Cleanup phase. Clean up the scanned resources. It it not allowed for resource creation. - Scan+CleanUp: Scan first, then CleanUp. - ScanWhenCreatingAndUpdating+CleanUpWhenDeleting: Scan when creating or updating resource, and CleanUp when deleting stack.
         :param clean_up_algorithm: Property cleanUpAlgorithm: The cleanup algorithm of cleanup phase: - ResourceDependency: Clean up by resource dependency tree. - ResourceTypeOrder: Clean up by resource type order. Property ResourceTypeOrder can be used to specify resource type order. If it is not specified, a default order will be used. Default to ResourceDependency.
         :param clean_up_retry_count: Property cleanUpRetryCount: The maximum number of executions of cleanup phase. Default to 1, which means no retry. Conditions that trigger a retry: (the relationship is or) 1.There are resources which fail to be cleaned up. 2.The cleanup is timeout.
@@ -452,14 +481,27 @@
         :param excluded_resources: Property excludedResources: Exclude parts from resources to be cleaned up.
         :param failure_option: Property failureOption: The failure option of cleanup phase: - Normal: Resource failure does not affect the resources that depend on it. - Fast: Resource failure causes all resources that depend on it to fail. Default to Normal.
         :param mode: Property mode: The result mode of resource cleaner: - Strict: Any scanning or cleanup failure leads to the failure of the cleaner. - Loose: Only a little scanning and cleanup failures lead to the failure of the cleaner. Most scanning failures will be ignored, failure messages can be found in ScanErrors or ResourceDetails. Most cleanup failures will be ignored, failure messages can be found in ResourceDetails. Default to Loose.
         :param resource_filters: Property resourceFilters: Resource filters that ResourceCleaner uses to filter out the resources to be cleaned up during scanning. Only one of ResourceFilters and Resources can be specified. There are two filtering behaviors(Effect): Allow and Deny. The filters work as below: 1.Any resource denied by any Deny filter will not be cleaned up. 2.Only resources allowed by some Allow filter and not denied by any Deny filter will be cleaned up. If filters are changed during resource update, ResourceCleaner requires to rescan. And if Action equals CleanUp, an error occurs.
         :param resources: Property resources: Resources to be cleaned up. Only one of Resources and ResourceFilters can be specified.
         :param resource_type_order: Property resourceTypeOrder: This property takes effect only when property CleanUpAlgorithm is ResourceTypeOrder. If it takes effect: - Resources will be cleaned up in order from front to back. - Resource with resource type not specified in this property will not be cleaned up.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ResourceCleanerProps.__init__)
+            check_type(argname="argument action", value=action, expected_type=type_hints["action"])
+            check_type(argname="argument clean_up_algorithm", value=clean_up_algorithm, expected_type=type_hints["clean_up_algorithm"])
+            check_type(argname="argument clean_up_retry_count", value=clean_up_retry_count, expected_type=type_hints["clean_up_retry_count"])
+            check_type(argname="argument clean_up_timeout", value=clean_up_timeout, expected_type=type_hints["clean_up_timeout"])
+            check_type(argname="argument disabled_side_effects", value=disabled_side_effects, expected_type=type_hints["disabled_side_effects"])
+            check_type(argname="argument excluded_resources", value=excluded_resources, expected_type=type_hints["excluded_resources"])
+            check_type(argname="argument failure_option", value=failure_option, expected_type=type_hints["failure_option"])
+            check_type(argname="argument mode", value=mode, expected_type=type_hints["mode"])
+            check_type(argname="argument resource_filters", value=resource_filters, expected_type=type_hints["resource_filters"])
+            check_type(argname="argument resources", value=resources, expected_type=type_hints["resources"])
+            check_type(argname="argument resource_type_order", value=resource_type_order, expected_type=type_hints["resource_type_order"])
         self._values: typing.Dict[str, typing.Any] = {
             "action": action,
         }
         if clean_up_algorithm is not None:
             self._values["clean_up_algorithm"] = clean_up_algorithm
         if clean_up_retry_count is not None:
             self._values["clean_up_retry_count"] = clean_up_retry_count
@@ -634,58 +676,70 @@
 ):
     '''A ROS template type:  ``ALIYUN::ROS::AutoEnableService``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosAutoEnableServiceProps",
+        props: typing.Union["RosAutoEnableServiceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::ROS::AutoEnableService``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosAutoEnableService.__init__)
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
+            type_hints = typing.get_type_hints(RosAutoEnableService._render_properties)
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
+            type_hints = typing.get_type_hints(getattr(RosAutoEnableService, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="serviceName")
     def service_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         serviceName: Which service to enable. Valid values:
         AHAS: Application High Availability Service
@@ -726,14 +780,17 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "serviceName"))
 
     @service_name.setter
     def service_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAutoEnableService, "service_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "serviceName", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-ros.RosAutoEnableServiceProps",
     jsii_struct_bases=[],
     name_mapping={"service_name": "serviceName"},
@@ -744,14 +801,17 @@
         *,
         service_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::ROS::AutoEnableService``.
 
         :param service_name: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosAutoEnableServiceProps.__init__)
+            check_type(argname="argument service_name", value=service_name, expected_type=type_hints["service_name"])
         self._values: typing.Dict[str, typing.Any] = {
             "service_name": service_name,
         }
 
     @builtins.property
     def service_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
@@ -816,65 +876,77 @@
 ):
     '''A ROS template type:  ``ALIYUN::ROS::CustomResource``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosCustomResourceProps",
+        props: typing.Union["RosCustomResourceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::ROS::CustomResource``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosCustomResource.__init__)
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
+            type_hints = typing.get_type_hints(RosCustomResource._render_properties)
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
     @jsii.member(jsii_name="attrOutputs")
     def attr_outputs(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Outputs: Output data received from service provider.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrOutputs"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosCustomResource, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="serviceToken")
     def service_token(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         serviceToken: The service token that was given to the template developer by the service provider to access the service.
         Allowed values:
@@ -899,17 +971,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "serviceToken"))
 
     @service_token.setter
     def service_token(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCustomResource, "service_token").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "serviceToken", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="timeout")
     def timeout(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         timeout: Timeout seconds before service provider responses.
         It takes effects only if the type of ServiceToken is Function Compute, MNS Queue, MNS Topic or async HTTP&HTTPS request.
@@ -918,48 +993,57 @@
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "timeout"))
 
     @timeout.setter
     def timeout(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCustomResource, "timeout").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "timeout", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="httpConfig")
     def http_config(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosCustomResource.HttpConfigProperty"]]:
         '''
         :Property: httpConfig: Config for HTTP&HTTPS service provider.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosCustomResource.HttpConfigProperty"]], jsii.get(self, "httpConfig"))
 
     @http_config.setter
     def http_config(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosCustomResource.HttpConfigProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCustomResource, "http_config").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "httpConfig", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="parameters")
     def parameters(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]]:
         '''
         :Property: parameters: Parameters to be passed to service provider.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]], jsii.get(self, "parameters"))
 
     @parameters.setter
     def parameters(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCustomResource, "parameters").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "parameters", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-ros.RosCustomResource.HttpConfigProperty",
         jsii_struct_bases=[],
         name_mapping={
             "content_type": "contentType",
@@ -976,14 +1060,19 @@
             sign_key: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param content_type: 
             :param headers: 
             :param sign_key: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosCustomResource.HttpConfigProperty.__init__)
+                check_type(argname="argument content_type", value=content_type, expected_type=type_hints["content_type"])
+                check_type(argname="argument headers", value=headers, expected_type=type_hints["headers"])
+                check_type(argname="argument sign_key", value=sign_key, expected_type=type_hints["sign_key"])
             self._values: typing.Dict[str, typing.Any] = {}
             if content_type is not None:
                 self._values["content_type"] = content_type
             if headers is not None:
                 self._values["headers"] = headers
             if sign_key is not None:
                 self._values["sign_key"] = sign_key
@@ -1060,24 +1149,30 @@
 )
 class RosCustomResourceProps:
     def __init__(
         self,
         *,
         service_token: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         timeout: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
-        http_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosCustomResource.HttpConfigProperty]] = None,
+        http_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosCustomResource.HttpConfigProperty, typing.Dict[str, typing.Any]]]] = None,
         parameters: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::ROS::CustomResource``.
 
         :param service_token: 
         :param timeout: 
         :param http_config: 
         :param parameters: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosCustomResourceProps.__init__)
+            check_type(argname="argument service_token", value=service_token, expected_type=type_hints["service_token"])
+            check_type(argname="argument timeout", value=timeout, expected_type=type_hints["timeout"])
+            check_type(argname="argument http_config", value=http_config, expected_type=type_hints["http_config"])
+            check_type(argname="argument parameters", value=parameters, expected_type=type_hints["parameters"])
         self._values: typing.Dict[str, typing.Any] = {
             "service_token": service_token,
             "timeout": timeout,
         }
         if http_config is not None:
             self._values["http_config"] = http_config
         if parameters is not None:
@@ -1164,43 +1259,52 @@
 ):
     '''A ROS template type:  ``ALIYUN::ROS::ResourceCleaner``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosResourceCleanerProps",
+        props: typing.Union["RosResourceCleanerProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::ROS::ResourceCleaner``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosResourceCleaner.__init__)
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
+            type_hints = typing.get_type_hints(RosResourceCleaner._render_properties)
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
     @jsii.member(jsii_name="attrCleanResult")
     def attr_clean_result(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute:
 
         CleanResult: The cleanup result. Valid values:
 
@@ -1210,39 +1314,39 @@
         - CheckFailure: Pre check of cleanup fails.
         - UnknownFailure: Unexpected failure.
         - UserCancelled: Cleanup is cancelled by user.
         - None: Cleanup is not triggered.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCleanResult"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrNoCleanupResourceDetails")
     def attr_no_cleanup_resource_details(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute:
 
         NoCleanupResourceDetails: The details of the resources that are scanned but filtered.
         Only resources with the resource types ResourceCleaner supports and the regions not filtered are scanned.
         The format is the same as ResourceDetails.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrNoCleanupResourceDetails"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrNoCleanupResourcePartialDetails")
     def attr_no_cleanup_resource_partial_details(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute:
 
         NoCleanupResourcePartialDetails: The partial details of the resources that are scanned but filtered.
         Only resources with the resource types ResourceCleaner supports and the regions not filtered are scanned.
         The format is the same as ResourcePartialDetails.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrNoCleanupResourcePartialDetails"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrResourceDetails")
     def attr_resource_details(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute:
 
         ResourceDetails: The details of resources to be cleaned up.
         The value is a list of dict. The dict contains the fields below:
@@ -1266,15 +1370,15 @@
         - Dependencies: The resources that need to be deleted before the deletion of the resource. The value is a list of dict. The dict contains the fields below:
         - ResourceType: Resource type of the dependency resource.
         - RegionId: Region ID of the dependency resource.
         - ResourceId: ID of the dependency resource.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrResourceDetails"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrResourcePartialDetails")
     def attr_resource_partial_details(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute:
 
         ResourcePartialDetails: The partial details of resources to be cleaned up.
         The value is a list of dict. The dict contains the fields below:
@@ -1289,15 +1393,15 @@
         - Success: The resource is deleted.
         - Skipped: The deletion of the resource is skipped.
         - Pending: The deletion of the resource is not started.
         - ResourceStatusReason: The information of the related ResourceStatus.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrResourcePartialDetails"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrResourceSummary")
     def attr_resource_summary(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute:
 
         ResourceSummary: The details of resources to be cleaned up.
         The value is a list of dict. The dict contains the fields below:
@@ -1309,35 +1413,35 @@
         - SkippedCount: Number of skipped resources of the resource type.
         - PendingCount: Number of resources that have not been deleted of the resource type.
         - OtherCount: Number of other resources of the resource type.
         - TotalCount: Number of total resources of the resource type.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrResourceSummary"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScanErrors")
     def attr_scan_errors(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute:
 
         ScanErrors: The scan errors. It takes effect only when property Mode is Loose.
         The value is a list of dict. The dict contains the fields below:
 
         - ResourceType: Resource type for scanning.
         - RegionId: Region ID for scanning.
         - ErrorMessage: Error message of scanning with specified resource type and region ID.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScanErrors"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="action")
     def action(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         action: Resource cleaner actions:
 
@@ -1349,26 +1453,32 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "action"))
 
     @action.setter
     def action(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosResourceCleaner, "action").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "action", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosResourceCleaner, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="cleanUpAlgorithm")
     def clean_up_algorithm(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1381,17 +1491,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "cleanUpAlgorithm"))
 
     @clean_up_algorithm.setter
     def clean_up_algorithm(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosResourceCleaner, "clean_up_algorithm").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "cleanUpAlgorithm", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="cleanUpRetryCount")
     def clean_up_retry_count(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1404,17 +1517,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "cleanUpRetryCount"))
 
     @clean_up_retry_count.setter
     def clean_up_retry_count(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosResourceCleaner, "clean_up_retry_count").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "cleanUpRetryCount", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="cleanUpTimeout")
     def clean_up_timeout(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1424,17 +1540,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "cleanUpTimeout"))
 
     @clean_up_timeout.setter
     def clean_up_timeout(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosResourceCleaner, "clean_up_timeout").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "cleanUpTimeout", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="disabledSideEffects")
     def disabled_side_effects(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
         '''
         :Property:
 
@@ -1445,34 +1564,40 @@
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]], jsii.get(self, "disabledSideEffects"))
 
     @disabled_side_effects.setter
     def disabled_side_effects(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosResourceCleaner, "disabled_side_effects").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "disabledSideEffects", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="excludedResources")
     def excluded_resources(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosResourceCleaner.ExcludedResourcesProperty"]]]]:
         '''
         :Property: excludedResources: Exclude parts from resources to be cleaned up.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosResourceCleaner.ExcludedResourcesProperty"]]]], jsii.get(self, "excludedResources"))
 
     @excluded_resources.setter
     def excluded_resources(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosResourceCleaner.ExcludedResourcesProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosResourceCleaner, "excluded_resources").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "excludedResources", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="failureOption")
     def failure_option(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1485,17 +1610,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "failureOption"))
 
     @failure_option.setter
     def failure_option(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosResourceCleaner, "failure_option").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "failureOption", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="mode")
     def mode(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1508,17 +1636,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "mode"))
 
     @mode.setter
     def mode(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosResourceCleaner, "mode").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "mode", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="resourceFilters")
     def resource_filters(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosResourceCleaner.ResourceFiltersProperty"]]]]:
         '''
         :Property:
 
@@ -1532,17 +1663,20 @@
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosResourceCleaner.ResourceFiltersProperty"]]]], jsii.get(self, "resourceFilters"))
 
     @resource_filters.setter
     def resource_filters(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosResourceCleaner.ResourceFiltersProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosResourceCleaner, "resource_filters").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "resourceFilters", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="resources")
     def resources(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosResourceCleaner.ResourcesProperty"]]]]:
         '''
         :Property:
 
@@ -1552,17 +1686,20 @@
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosResourceCleaner.ResourcesProperty"]]]], jsii.get(self, "resources"))
 
     @resources.setter
     def resources(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosResourceCleaner.ResourcesProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosResourceCleaner, "resources").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "resources", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="resourceTypeOrder")
     def resource_type_order(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
         '''
         :Property:
 
@@ -1575,14 +1712,17 @@
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]], jsii.get(self, "resourceTypeOrder"))
 
     @resource_type_order.setter
     def resource_type_order(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosResourceCleaner, "resource_type_order").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "resourceTypeOrder", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-ros.RosResourceCleaner.ExcludedResourcesProperty",
         jsii_struct_bases=[],
         name_mapping={
             "resource_id": "resourceId",
@@ -1599,14 +1739,19 @@
             resource_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param resource_id: 
             :param region_id: 
             :param resource_type: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosResourceCleaner.ExcludedResourcesProperty.__init__)
+                check_type(argname="argument resource_id", value=resource_id, expected_type=type_hints["resource_id"])
+                check_type(argname="argument region_id", value=region_id, expected_type=type_hints["region_id"])
+                check_type(argname="argument resource_type", value=resource_type, expected_type=type_hints["resource_type"])
             self._values: typing.Dict[str, typing.Any] = {
                 "resource_id": resource_id,
             }
             if region_id is not None:
                 self._values["region_id"] = region_id
             if resource_type is not None:
                 self._values["resource_type"] = resource_type
@@ -1675,26 +1820,36 @@
             effect: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             include_deletion_protection: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
             region_ids: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
             resource_group_ids: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
             resource_ids: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
             resource_name_patterns: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
             resource_type_patterns: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
-            tags: typing.Optional[typing.Sequence["RosResourceCleaner.TagsProperty"]] = None,
+            tags: typing.Optional[typing.Sequence[typing.Union["RosResourceCleaner.TagsProperty", typing.Dict[str, typing.Any]]]] = None,
         ) -> None:
             '''
             :param effect: 
             :param include_deletion_protection: 
             :param region_ids: 
             :param resource_group_ids: 
             :param resource_ids: 
             :param resource_name_patterns: 
             :param resource_type_patterns: 
             :param tags: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosResourceCleaner.ResourceFiltersProperty.__init__)
+                check_type(argname="argument effect", value=effect, expected_type=type_hints["effect"])
+                check_type(argname="argument include_deletion_protection", value=include_deletion_protection, expected_type=type_hints["include_deletion_protection"])
+                check_type(argname="argument region_ids", value=region_ids, expected_type=type_hints["region_ids"])
+                check_type(argname="argument resource_group_ids", value=resource_group_ids, expected_type=type_hints["resource_group_ids"])
+                check_type(argname="argument resource_ids", value=resource_ids, expected_type=type_hints["resource_ids"])
+                check_type(argname="argument resource_name_patterns", value=resource_name_patterns, expected_type=type_hints["resource_name_patterns"])
+                check_type(argname="argument resource_type_patterns", value=resource_type_patterns, expected_type=type_hints["resource_type_patterns"])
+                check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
             self._values: typing.Dict[str, typing.Any] = {}
             if effect is not None:
                 self._values["effect"] = effect
             if include_deletion_protection is not None:
                 self._values["include_deletion_protection"] = include_deletion_protection
             if region_ids is not None:
                 self._values["region_ids"] = region_ids
@@ -1844,14 +1999,19 @@
             resource_type: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param region_id: 
             :param resource_id: 
             :param resource_type: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosResourceCleaner.ResourcesProperty.__init__)
+                check_type(argname="argument region_id", value=region_id, expected_type=type_hints["region_id"])
+                check_type(argname="argument resource_id", value=resource_id, expected_type=type_hints["resource_id"])
+                check_type(argname="argument resource_type", value=resource_type, expected_type=type_hints["resource_type"])
             self._values: typing.Dict[str, typing.Any] = {
                 "region_id": region_id,
                 "resource_id": resource_id,
                 "resource_type": resource_type,
             }
 
         @builtins.property
@@ -1907,14 +2067,18 @@
             key: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param key: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosResourceCleaner.TagsProperty.__init__)
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {
                 "key": key,
             }
             if value is not None:
                 self._values["value"] = value
 
         @builtins.property
@@ -1974,19 +2138,19 @@
         self,
         *,
         action: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         clean_up_algorithm: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         clean_up_retry_count: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         clean_up_timeout: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         disabled_side_effects: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
-        excluded_resources: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosResourceCleaner.ExcludedResourcesProperty]]]] = None,
+        excluded_resources: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosResourceCleaner.ExcludedResourcesProperty, typing.Dict[str, typing.Any]]]]]] = None,
         failure_option: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         mode: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        resource_filters: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosResourceCleaner.ResourceFiltersProperty]]]] = None,
-        resources: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosResourceCleaner.ResourcesProperty]]]] = None,
+        resource_filters: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosResourceCleaner.ResourceFiltersProperty, typing.Dict[str, typing.Any]]]]]] = None,
+        resources: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosResourceCleaner.ResourcesProperty, typing.Dict[str, typing.Any]]]]]] = None,
         resource_type_order: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::ROS::ResourceCleaner``.
 
         :param action: 
         :param clean_up_algorithm: 
         :param clean_up_retry_count: 
@@ -1995,14 +2159,27 @@
         :param excluded_resources: 
         :param failure_option: 
         :param mode: 
         :param resource_filters: 
         :param resources: 
         :param resource_type_order: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosResourceCleanerProps.__init__)
+            check_type(argname="argument action", value=action, expected_type=type_hints["action"])
+            check_type(argname="argument clean_up_algorithm", value=clean_up_algorithm, expected_type=type_hints["clean_up_algorithm"])
+            check_type(argname="argument clean_up_retry_count", value=clean_up_retry_count, expected_type=type_hints["clean_up_retry_count"])
+            check_type(argname="argument clean_up_timeout", value=clean_up_timeout, expected_type=type_hints["clean_up_timeout"])
+            check_type(argname="argument disabled_side_effects", value=disabled_side_effects, expected_type=type_hints["disabled_side_effects"])
+            check_type(argname="argument excluded_resources", value=excluded_resources, expected_type=type_hints["excluded_resources"])
+            check_type(argname="argument failure_option", value=failure_option, expected_type=type_hints["failure_option"])
+            check_type(argname="argument mode", value=mode, expected_type=type_hints["mode"])
+            check_type(argname="argument resource_filters", value=resource_filters, expected_type=type_hints["resource_filters"])
+            check_type(argname="argument resources", value=resources, expected_type=type_hints["resources"])
+            check_type(argname="argument resource_type_order", value=resource_type_order, expected_type=type_hints["resource_type_order"])
         self._values: typing.Dict[str, typing.Any] = {
             "action": action,
         }
         if clean_up_algorithm is not None:
             self._values["clean_up_algorithm"] = clean_up_algorithm
         if clean_up_retry_count is not None:
             self._values["clean_up_retry_count"] = clean_up_retry_count
@@ -2205,140 +2382,167 @@
 ):
     '''A ROS template type:  ``ALIYUN::ROS::Sleep``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosSleepProps",
+        props: typing.Union["RosSleepProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::ROS::Sleep``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosSleep.__init__)
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
+            type_hints = typing.get_type_hints(RosSleep._render_properties)
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
+            type_hints = typing.get_type_hints(getattr(RosSleep, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="createDuration")
     def create_duration(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: createDuration: The number of seconds to wait before resource creation.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "createDuration"))
 
     @create_duration.setter
     def create_duration(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSleep, "create_duration").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "createDuration", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="deleteDuration")
     def delete_duration(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: deleteDuration: The number of seconds to wait before resource deletion.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "deleteDuration"))
 
     @delete_duration.setter
     def delete_duration(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSleep, "delete_duration").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "deleteDuration", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="triggers")
     def triggers(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]]:
         '''
         :Property: triggers: Arbitrary map of values that, when changed, will run update or update rollback delays again.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]], jsii.get(self, "triggers"))
 
     @triggers.setter
     def triggers(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSleep, "triggers").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "triggers", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="updateDuration")
     def update_duration(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: updateDuration: The number of seconds to wait before resource update. It only triggers when the property Triggers change and the status of stack is UPDATE_IN_PROGRESS.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "updateDuration"))
 
     @update_duration.setter
     def update_duration(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSleep, "update_duration").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "updateDuration", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="updateRollbackDuration")
     def update_rollback_duration(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: updateRollbackDuration: The number of seconds to wait before resource update rollback. It only triggers when stack update failed and resource was updated.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "updateRollbackDuration"))
 
     @update_rollback_duration.setter
     def update_rollback_duration(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSleep, "update_rollback_duration").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "updateRollbackDuration", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-ros.RosSleepProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -2363,14 +2567,21 @@
 
         :param create_duration: 
         :param delete_duration: 
         :param triggers: 
         :param update_duration: 
         :param update_rollback_duration: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosSleepProps.__init__)
+            check_type(argname="argument create_duration", value=create_duration, expected_type=type_hints["create_duration"])
+            check_type(argname="argument delete_duration", value=delete_duration, expected_type=type_hints["delete_duration"])
+            check_type(argname="argument triggers", value=triggers, expected_type=type_hints["triggers"])
+            check_type(argname="argument update_duration", value=update_duration, expected_type=type_hints["update_duration"])
+            check_type(argname="argument update_rollback_duration", value=update_rollback_duration, expected_type=type_hints["update_rollback_duration"])
         self._values: typing.Dict[str, typing.Any] = {}
         if create_duration is not None:
             self._values["create_duration"] = create_duration
         if delete_duration is not None:
             self._values["delete_duration"] = delete_duration
         if triggers is not None:
             self._values["triggers"] = triggers
@@ -2448,92 +2659,110 @@
 ):
     '''A ROS template type:  ``ALIYUN::ROS::Stack``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosStackProps",
+        props: typing.Union["RosStackProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::ROS::Stack``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosStack.__init__)
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
+            type_hints = typing.get_type_hints(RosStack._render_properties)
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
+            type_hints = typing.get_type_hints(getattr(RosStack, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="parameters")
     def parameters(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]]:
         '''
         :Property: parameters: The set of parameters passed to this nested stack.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]], jsii.get(self, "parameters"))
 
     @parameters.setter
     def parameters(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosStack, "parameters").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "parameters", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="resourceGroupId")
     def resource_group_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: resourceGroupId: Resource group.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "resourceGroupId"))
 
     @resource_group_id.setter
     def resource_group_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosStack, "resource_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "resourceGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="templateBody")
     def template_body(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]]:
         '''
         :Property:
 
@@ -2544,34 +2773,40 @@
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]], jsii.get(self, "templateBody"))
 
     @template_body.setter
     def template_body(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosStack, "template_body").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "templateBody", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="templateId")
     def template_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: templateId: Template ID of template containing the template body.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "templateId"))
 
     @template_id.setter
     def template_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosStack, "template_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "templateId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="templateUrl")
     def template_url(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2581,329 +2816,389 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "templateUrl"))
 
     @template_url.setter
     def template_url(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosStack, "template_url").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "templateUrl", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="templateVersion")
     def template_version(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: templateVersion: Template version of template containing the template body.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "templateVersion"))
 
     @template_version.setter
     def template_version(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosStack, "template_version").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "templateVersion", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="timeoutMins")
     def timeout_mins(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: timeoutMins: The length of time, in minutes, to wait for the nested stack creation or update. Default to 60 minutes.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "timeoutMins"))
 
     @timeout_mins.setter
     def timeout_mins(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosStack, "timeout_mins").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "timeoutMins", value)
 
 
 class RosStackGroup(
     ros_cdk_core.RosResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-ros.RosStackGroup",
 ):
     '''A ROS template type:  ``ALIYUN::ROS::StackGroup``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosStackGroupProps",
+        props: typing.Union["RosStackGroupProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::ROS::StackGroup``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosStackGroup.__init__)
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
+            type_hints = typing.get_type_hints(RosStackGroup._render_properties)
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
     @jsii.member(jsii_name="attrStackGroupId")
     def attr_stack_group_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: StackGroupId: undefined
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrStackGroupId"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosStackGroup, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="stackGroupName")
     def stack_group_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: stackGroupName: undefined
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "stackGroupName"))
 
     @stack_group_name.setter
     def stack_group_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosStackGroup, "stack_group_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "stackGroupName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="administrationRoleName")
     def administration_role_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: administrationRoleName: undefined
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "administrationRoleName"))
 
     @administration_role_name.setter
     def administration_role_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosStackGroup, "administration_role_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "administrationRoleName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="autoDeployment")
     def auto_deployment(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosStackGroup.AutoDeploymentProperty"]]:
         '''
         :Property: autoDeployment: undefined
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosStackGroup.AutoDeploymentProperty"]], jsii.get(self, "autoDeployment"))
 
     @auto_deployment.setter
     def auto_deployment(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosStackGroup.AutoDeploymentProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosStackGroup, "auto_deployment").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "autoDeployment", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: description: undefined
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosStackGroup, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dynamicTemplateBody")
     def dynamic_template_body(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]]:
         '''
         :Property: dynamicTemplateBody: undefined
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]], jsii.get(self, "dynamicTemplateBody"))
 
     @dynamic_template_body.setter
     def dynamic_template_body(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosStackGroup, "dynamic_template_body").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dynamicTemplateBody", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="executionRoleName")
     def execution_role_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: executionRoleName: undefined
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "executionRoleName"))
 
     @execution_role_name.setter
     def execution_role_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosStackGroup, "execution_role_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "executionRoleName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="parameters")
     def parameters(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]]:
         '''
         :Property: parameters: undefined
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]], jsii.get(self, "parameters"))
 
     @parameters.setter
     def parameters(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosStackGroup, "parameters").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "parameters", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="permissionModel")
     def permission_model(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: permissionModel: undefined
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "permissionModel"))
 
     @permission_model.setter
     def permission_model(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosStackGroup, "permission_model").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "permissionModel", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="resourceGroupId")
     def resource_group_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: resourceGroupId: undefined
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "resourceGroupId"))
 
     @resource_group_id.setter
     def resource_group_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosStackGroup, "resource_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "resourceGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="templateBody")
     def template_body(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]]:
         '''
         :Property: templateBody: undefined
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]], jsii.get(self, "templateBody"))
 
     @template_body.setter
     def template_body(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosStackGroup, "template_body").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "templateBody", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="templateId")
     def template_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: templateId: undefined
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "templateId"))
 
     @template_id.setter
     def template_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosStackGroup, "template_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "templateId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="templateUrl")
     def template_url(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: templateUrl: undefined
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "templateUrl"))
 
     @template_url.setter
     def template_url(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosStackGroup, "template_url").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "templateUrl", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="templateVersion")
     def template_version(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: templateVersion: undefined
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "templateVersion"))
 
     @template_version.setter
     def template_version(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosStackGroup, "template_version").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "templateVersion", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-ros.RosStackGroup.AutoDeploymentProperty",
         jsii_struct_bases=[],
         name_mapping={
             "enabled": "enabled",
@@ -2917,14 +3212,18 @@
             enabled: typing.Union[builtins.bool, ros_cdk_core.IResolvable],
             retain_stacks_on_account_removal: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param enabled: 
             :param retain_stacks_on_account_removal: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosStackGroup.AutoDeploymentProperty.__init__)
+                check_type(argname="argument enabled", value=enabled, expected_type=type_hints["enabled"])
+                check_type(argname="argument retain_stacks_on_account_removal", value=retain_stacks_on_account_removal, expected_type=type_hints["retain_stacks_on_account_removal"])
             self._values: typing.Dict[str, typing.Any] = {
                 "enabled": enabled,
             }
             if retain_stacks_on_account_removal is not None:
                 self._values["retain_stacks_on_account_removal"] = retain_stacks_on_account_removal
 
         @builtins.property
@@ -2979,15 +3278,15 @@
 )
 class RosStackGroupProps:
     def __init__(
         self,
         *,
         stack_group_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         administration_role_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        auto_deployment: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosStackGroup.AutoDeploymentProperty]] = None,
+        auto_deployment: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosStackGroup.AutoDeploymentProperty, typing.Dict[str, typing.Any]]]] = None,
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         dynamic_template_body: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]] = None,
         execution_role_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         parameters: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]] = None,
         permission_model: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         resource_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         template_body: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]] = None,
@@ -3007,14 +3306,29 @@
         :param permission_model: 
         :param resource_group_id: 
         :param template_body: 
         :param template_id: 
         :param template_url: 
         :param template_version: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosStackGroupProps.__init__)
+            check_type(argname="argument stack_group_name", value=stack_group_name, expected_type=type_hints["stack_group_name"])
+            check_type(argname="argument administration_role_name", value=administration_role_name, expected_type=type_hints["administration_role_name"])
+            check_type(argname="argument auto_deployment", value=auto_deployment, expected_type=type_hints["auto_deployment"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument dynamic_template_body", value=dynamic_template_body, expected_type=type_hints["dynamic_template_body"])
+            check_type(argname="argument execution_role_name", value=execution_role_name, expected_type=type_hints["execution_role_name"])
+            check_type(argname="argument parameters", value=parameters, expected_type=type_hints["parameters"])
+            check_type(argname="argument permission_model", value=permission_model, expected_type=type_hints["permission_model"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument template_body", value=template_body, expected_type=type_hints["template_body"])
+            check_type(argname="argument template_id", value=template_id, expected_type=type_hints["template_id"])
+            check_type(argname="argument template_url", value=template_url, expected_type=type_hints["template_url"])
+            check_type(argname="argument template_version", value=template_version, expected_type=type_hints["template_version"])
         self._values: typing.Dict[str, typing.Any] = {
             "stack_group_name": stack_group_name,
         }
         if administration_role_name is not None:
             self._values["administration_role_name"] = administration_role_name
         if auto_deployment is not None:
             self._values["auto_deployment"] = auto_deployment
@@ -3187,238 +3501,280 @@
 ):
     '''A ROS template type:  ``ALIYUN::ROS::StackInstances``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosStackInstancesProps",
+        props: typing.Union["RosStackInstancesProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::ROS::StackInstances``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosStackInstances.__init__)
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
+            type_hints = typing.get_type_hints(RosStackInstances._render_properties)
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
     @jsii.member(jsii_name="attrLastOperationId")
     def attr_last_operation_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: LastOperationId: undefined
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLastOperationId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrStacks")
     def attr_stacks(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Stacks: undefined
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrStacks"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosStackInstances, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="regionIds")
     def region_ids(
         self,
     ) -> typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]:
         '''
         :Property: regionIds: undefined
         '''
         return typing.cast(typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]], jsii.get(self, "regionIds"))
 
     @region_ids.setter
     def region_ids(
         self,
         value: typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosStackInstances, "region_ids").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "regionIds", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="stackGroupName")
     def stack_group_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: stackGroupName: undefined
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "stackGroupName"))
 
     @stack_group_name.setter
     def stack_group_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosStackInstances, "stack_group_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "stackGroupName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="accountIds")
     def account_ids(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
         '''
         :Property: accountIds: undefined
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]], jsii.get(self, "accountIds"))
 
     @account_ids.setter
     def account_ids(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosStackInstances, "account_ids").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "accountIds", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="deploymentTargets")
     def deployment_targets(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosStackInstances.DeploymentTargetsProperty"]]:
         '''
         :Property: deploymentTargets: undefined
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosStackInstances.DeploymentTargetsProperty"]], jsii.get(self, "deploymentTargets"))
 
     @deployment_targets.setter
     def deployment_targets(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosStackInstances.DeploymentTargetsProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosStackInstances, "deployment_targets").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "deploymentTargets", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="disableRollback")
     def disable_rollback(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: disableRollback: undefined
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "disableRollback"))
 
     @disable_rollback.setter
     def disable_rollback(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosStackInstances, "disable_rollback").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "disableRollback", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="operationDescription")
     def operation_description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: operationDescription: undefined
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "operationDescription"))
 
     @operation_description.setter
     def operation_description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosStackInstances, "operation_description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "operationDescription", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="operationPreferences")
     def operation_preferences(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosStackInstances.OperationPreferencesProperty"]]:
         '''
         :Property: operationPreferences: undefined
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosStackInstances.OperationPreferencesProperty"]], jsii.get(self, "operationPreferences"))
 
     @operation_preferences.setter
     def operation_preferences(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosStackInstances.OperationPreferencesProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosStackInstances, "operation_preferences").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "operationPreferences", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="parameterOverrides")
     def parameter_overrides(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]]:
         '''
         :Property: parameterOverrides: undefined
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]], jsii.get(self, "parameterOverrides"))
 
     @parameter_overrides.setter
     def parameter_overrides(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosStackInstances, "parameter_overrides").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "parameterOverrides", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="retainStacks")
     def retain_stacks(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: retainStacks: undefined
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "retainStacks"))
 
     @retain_stacks.setter
     def retain_stacks(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosStackInstances, "retain_stacks").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "retainStacks", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="timeoutInMinutes")
     def timeout_in_minutes(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: timeoutInMinutes: undefined
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "timeoutInMinutes"))
 
     @timeout_in_minutes.setter
     def timeout_in_minutes(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosStackInstances, "timeout_in_minutes").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "timeoutInMinutes", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-ros.RosStackInstances.DeploymentTargetsProperty",
         jsii_struct_bases=[],
         name_mapping={"rd_folder_ids": "rdFolderIds"},
     )
@@ -3427,14 +3783,17 @@
             self,
             *,
             rd_folder_ids: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
         ) -> None:
             '''
             :param rd_folder_ids: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosStackInstances.DeploymentTargetsProperty.__init__)
+                check_type(argname="argument rd_folder_ids", value=rd_folder_ids, expected_type=type_hints["rd_folder_ids"])
             self._values: typing.Dict[str, typing.Any] = {}
             if rd_folder_ids is not None:
                 self._values["rd_folder_ids"] = rd_folder_ids
 
         @builtins.property
         def rd_folder_ids(
             self,
@@ -3477,14 +3836,20 @@
         ) -> None:
             '''
             :param failure_tolerance_count: 
             :param failure_tolerance_percentage: 
             :param max_concurrent_count: 
             :param max_concurrent_percentage: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosStackInstances.OperationPreferencesProperty.__init__)
+                check_type(argname="argument failure_tolerance_count", value=failure_tolerance_count, expected_type=type_hints["failure_tolerance_count"])
+                check_type(argname="argument failure_tolerance_percentage", value=failure_tolerance_percentage, expected_type=type_hints["failure_tolerance_percentage"])
+                check_type(argname="argument max_concurrent_count", value=max_concurrent_count, expected_type=type_hints["max_concurrent_count"])
+                check_type(argname="argument max_concurrent_percentage", value=max_concurrent_percentage, expected_type=type_hints["max_concurrent_percentage"])
             self._values: typing.Dict[str, typing.Any] = {}
             if failure_tolerance_count is not None:
                 self._values["failure_tolerance_count"] = failure_tolerance_count
             if failure_tolerance_percentage is not None:
                 self._values["failure_tolerance_percentage"] = failure_tolerance_percentage
             if max_concurrent_count is not None:
                 self._values["max_concurrent_count"] = max_concurrent_count
@@ -3562,18 +3927,18 @@
 class RosStackInstancesProps:
     def __init__(
         self,
         *,
         region_ids: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]],
         stack_group_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         account_ids: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
-        deployment_targets: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosStackInstances.DeploymentTargetsProperty]] = None,
+        deployment_targets: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosStackInstances.DeploymentTargetsProperty, typing.Dict[str, typing.Any]]]] = None,
         disable_rollback: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         operation_description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        operation_preferences: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosStackInstances.OperationPreferencesProperty]] = None,
+        operation_preferences: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosStackInstances.OperationPreferencesProperty, typing.Dict[str, typing.Any]]]] = None,
         parameter_overrides: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]] = None,
         retain_stacks: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         timeout_in_minutes: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::ROS::StackInstances``.
 
         :param region_ids: 
@@ -3583,14 +3948,26 @@
         :param disable_rollback: 
         :param operation_description: 
         :param operation_preferences: 
         :param parameter_overrides: 
         :param retain_stacks: 
         :param timeout_in_minutes: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosStackInstancesProps.__init__)
+            check_type(argname="argument region_ids", value=region_ids, expected_type=type_hints["region_ids"])
+            check_type(argname="argument stack_group_name", value=stack_group_name, expected_type=type_hints["stack_group_name"])
+            check_type(argname="argument account_ids", value=account_ids, expected_type=type_hints["account_ids"])
+            check_type(argname="argument deployment_targets", value=deployment_targets, expected_type=type_hints["deployment_targets"])
+            check_type(argname="argument disable_rollback", value=disable_rollback, expected_type=type_hints["disable_rollback"])
+            check_type(argname="argument operation_description", value=operation_description, expected_type=type_hints["operation_description"])
+            check_type(argname="argument operation_preferences", value=operation_preferences, expected_type=type_hints["operation_preferences"])
+            check_type(argname="argument parameter_overrides", value=parameter_overrides, expected_type=type_hints["parameter_overrides"])
+            check_type(argname="argument retain_stacks", value=retain_stacks, expected_type=type_hints["retain_stacks"])
+            check_type(argname="argument timeout_in_minutes", value=timeout_in_minutes, expected_type=type_hints["timeout_in_minutes"])
         self._values: typing.Dict[str, typing.Any] = {
             "region_ids": region_ids,
             "stack_group_name": stack_group_name,
         }
         if account_ids is not None:
             self._values["account_ids"] = account_ids
         if deployment_targets is not None:
@@ -3751,14 +4128,23 @@
         :param resource_group_id: 
         :param template_body: 
         :param template_id: 
         :param template_url: 
         :param template_version: 
         :param timeout_mins: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosStackProps.__init__)
+            check_type(argname="argument parameters", value=parameters, expected_type=type_hints["parameters"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument template_body", value=template_body, expected_type=type_hints["template_body"])
+            check_type(argname="argument template_id", value=template_id, expected_type=type_hints["template_id"])
+            check_type(argname="argument template_url", value=template_url, expected_type=type_hints["template_url"])
+            check_type(argname="argument template_version", value=template_version, expected_type=type_hints["template_version"])
+            check_type(argname="argument timeout_mins", value=timeout_mins, expected_type=type_hints["timeout_mins"])
         self._values: typing.Dict[str, typing.Any] = {}
         if parameters is not None:
             self._values["parameters"] = parameters
         if resource_group_id is not None:
             self._values["resource_group_id"] = resource_group_id
         if template_body is not None:
             self._values["template_body"] = template_body
@@ -3867,239 +4253,275 @@
 ):
     '''A ROS template type:  ``ALIYUN::ROS::WaitCondition``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosWaitConditionProps",
+        props: typing.Union["RosWaitConditionProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::ROS::WaitCondition``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosWaitCondition.__init__)
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
+            type_hints = typing.get_type_hints(RosWaitCondition._render_properties)
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
     @jsii.member(jsii_name="attrData")
     def attr_data(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Data: JSON serialized dict containing data associated with wait condition signals sent to the handle.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrData"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrErrorData")
     def attr_error_data(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ErrorData: JSON serialized dict containing data associated with wait condition error signals sent to the handle.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrErrorData"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrJoinedErrorData")
     def attr_joined_error_data(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: JoinedErrorData: String containing data associated with wait condition error signals sent to the handle.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrJoinedErrorData"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosWaitCondition, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="handle")
     def handle(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: handle: A reference to the wait condition handle used to signal this wait condition.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "handle"))
 
     @handle.setter
     def handle(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosWaitCondition, "handle").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "handle", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="timeout")
     def timeout(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property: timeout: The number of seconds to wait for the correct number of signals to arrive.
         '''
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "timeout"))
 
     @timeout.setter
     def timeout(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosWaitCondition, "timeout").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "timeout", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="count")
     def count(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: count: The number of success signals that must be received before the stack creation process continues.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "count"))
 
     @count.setter
     def count(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosWaitCondition, "count").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "count", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="showProgressEvent")
     def show_progress_event(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: showProgressEvent: Whether to generate progress changed event. Default to Disabled.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "showProgressEvent"))
 
     @show_progress_event.setter
     def show_progress_event(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosWaitCondition, "show_progress_event").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "showProgressEvent", value)
 
 
 class RosWaitConditionHandle(
     ros_cdk_core.RosResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-ros.RosWaitConditionHandle",
 ):
     '''A ROS template type:  ``ALIYUN::ROS::WaitConditionHandle``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosWaitConditionHandleProps",
+        props: typing.Union["RosWaitConditionHandleProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::ROS::WaitConditionHandle``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosWaitConditionHandle.__init__)
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
+            type_hints = typing.get_type_hints(RosWaitConditionHandle._render_properties)
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
     @jsii.member(jsii_name="attrCurlCli")
     def attr_curl_cli(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: CurlCli: Convenience attribute, provides curl CLI command prefix, which can be used for signalling handle completion or failure.  You can signal success by adding --data-binary '{"status": "SUCCESS"}' , or signal failure by adding --data-binary '{"status": "FAILURE"}'
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCurlCli"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrHeaders")
     def attr_headers(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Headers: HTTP POST Headers used for signalling handle completion or failure.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrHeaders"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPowerShellCurlCli")
     def attr_power_shell_curl_cli(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: PowerShellCurlCli: Convenience attribute, provides curl CLI command prefix for PowerShell, which can be used for signalling handle completion or failure. As this cmdlet was introduced in PowerShell 3.0, ensure the version of PowerShell satisfies the constraint. (Show the version via $PSVersionTable.PSVersion.) You can signal success by adding -Body '{"status": "SUCCESS"}' , or signal failure by adding -Body '{"status": "FAILURE"}'
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPowerShellCurlCli"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrUrl")
     def attr_url(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: URL: HTTP POST URL used for signalling handle completion or failure.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrUrl"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrWindowsCurlCli")
     def attr_windows_curl_cli(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: WindowsCurlCli: Convenience attribute, provides curl CLI command prefix for Windows, which can be used for signalling handle completion or failure. As Windows does not support curl command, you need to install curl.exe and add it to PATH first. You can signal success by adding --data-binary "{"status": "SUCCESS"}" , or signal failure by adding --data-binary "{"status": "FAILURE"}"
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrWindowsCurlCli"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosWaitConditionHandle, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="count")
     def count(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -4115,17 +4537,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "count"))
 
     @count.setter
     def count(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosWaitConditionHandle, "count").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "count", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="mode")
     def mode(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -4138,14 +4563,17 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "mode"))
 
     @mode.setter
     def mode(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosWaitConditionHandle, "mode").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "mode", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-ros.RosWaitConditionHandleProps",
     jsii_struct_bases=[],
     name_mapping={"count": "count", "mode": "mode"},
@@ -4158,14 +4586,18 @@
         mode: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::ROS::WaitConditionHandle``.
 
         :param count: 
         :param mode: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosWaitConditionHandleProps.__init__)
+            check_type(argname="argument count", value=count, expected_type=type_hints["count"])
+            check_type(argname="argument mode", value=mode, expected_type=type_hints["mode"])
         self._values: typing.Dict[str, typing.Any] = {}
         if count is not None:
             self._values["count"] = count
         if mode is not None:
             self._values["mode"] = mode
 
     @builtins.property
@@ -4237,14 +4669,20 @@
         '''Properties for defining a ``ALIYUN::ROS::WaitCondition``.
 
         :param handle: 
         :param timeout: 
         :param count: 
         :param show_progress_event: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosWaitConditionProps.__init__)
+            check_type(argname="argument handle", value=handle, expected_type=type_hints["handle"])
+            check_type(argname="argument timeout", value=timeout, expected_type=type_hints["timeout"])
+            check_type(argname="argument count", value=count, expected_type=type_hints["count"])
+            check_type(argname="argument show_progress_event", value=show_progress_event, expected_type=type_hints["show_progress_event"])
         self._values: typing.Dict[str, typing.Any] = {
             "handle": handle,
             "timeout": timeout,
         }
         if count is not None:
             self._values["count"] = count
         if show_progress_event is not None:
@@ -4307,28 +4745,34 @@
 ):
     '''A ROS resource type:  ``ALIYUN::ROS::Sleep``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: typing.Optional["SleepProps"] = None,
+        props: typing.Optional[typing.Union["SleepProps", typing.Dict[str, typing.Any]]] = None,
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::ROS::Sleep``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Sleep.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-ros.SleepProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -4353,14 +4797,21 @@
 
         :param create_duration: Property createDuration: The number of seconds to wait before resource creation.
         :param delete_duration: Property deleteDuration: The number of seconds to wait before resource deletion.
         :param triggers: Property triggers: Arbitrary map of values that, when changed, will run update or update rollback delays again.
         :param update_duration: Property updateDuration: The number of seconds to wait before resource update. It only triggers when the property Triggers change and the status of stack is UPDATE_IN_PROGRESS.
         :param update_rollback_duration: Property updateRollbackDuration: The number of seconds to wait before resource update rollback. It only triggers when stack update failed and resource was updated.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(SleepProps.__init__)
+            check_type(argname="argument create_duration", value=create_duration, expected_type=type_hints["create_duration"])
+            check_type(argname="argument delete_duration", value=delete_duration, expected_type=type_hints["delete_duration"])
+            check_type(argname="argument triggers", value=triggers, expected_type=type_hints["triggers"])
+            check_type(argname="argument update_duration", value=update_duration, expected_type=type_hints["update_duration"])
+            check_type(argname="argument update_rollback_duration", value=update_rollback_duration, expected_type=type_hints["update_rollback_duration"])
         self._values: typing.Dict[str, typing.Any] = {}
         if create_duration is not None:
             self._values["create_duration"] = create_duration
         if delete_duration is not None:
             self._values["delete_duration"] = delete_duration
         if triggers is not None:
             self._values["triggers"] = triggers
@@ -4434,59 +4885,71 @@
 ):
     '''A ROS resource type:  ``ALIYUN::ROS::Stack``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: typing.Optional["StackProps"] = None,
+        props: typing.Optional[typing.Union["StackProps", typing.Dict[str, typing.Any]]] = None,
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::ROS::Stack``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Stack.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
 
 class StackGroup(
     ros_cdk_core.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-ros.StackGroup",
 ):
     '''A ROS resource type:  ``ALIYUN::ROS::StackGroup``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "StackGroupProps",
+        props: typing.Union["StackGroupProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::ROS::StackGroup``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(StackGroup.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrStackGroupId")
     def attr_stack_group_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute StackGroupId: undefined.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrStackGroupId"))
 
 
 @jsii.data_type(
@@ -4510,15 +4973,15 @@
 )
 class StackGroupProps:
     def __init__(
         self,
         *,
         stack_group_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         administration_role_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        auto_deployment: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosStackGroup.AutoDeploymentProperty]] = None,
+        auto_deployment: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosStackGroup.AutoDeploymentProperty, typing.Dict[str, typing.Any]]]] = None,
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         dynamic_template_body: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]] = None,
         execution_role_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         parameters: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]] = None,
         permission_model: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         resource_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         template_body: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]] = None,
@@ -4538,14 +5001,29 @@
         :param permission_model: Property permissionModel: undefined.
         :param resource_group_id: Property resourceGroupId: undefined.
         :param template_body: Property templateBody: undefined.
         :param template_id: Property templateId: undefined.
         :param template_url: Property templateUrl: undefined.
         :param template_version: Property templateVersion: undefined.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(StackGroupProps.__init__)
+            check_type(argname="argument stack_group_name", value=stack_group_name, expected_type=type_hints["stack_group_name"])
+            check_type(argname="argument administration_role_name", value=administration_role_name, expected_type=type_hints["administration_role_name"])
+            check_type(argname="argument auto_deployment", value=auto_deployment, expected_type=type_hints["auto_deployment"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument dynamic_template_body", value=dynamic_template_body, expected_type=type_hints["dynamic_template_body"])
+            check_type(argname="argument execution_role_name", value=execution_role_name, expected_type=type_hints["execution_role_name"])
+            check_type(argname="argument parameters", value=parameters, expected_type=type_hints["parameters"])
+            check_type(argname="argument permission_model", value=permission_model, expected_type=type_hints["permission_model"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument template_body", value=template_body, expected_type=type_hints["template_body"])
+            check_type(argname="argument template_id", value=template_id, expected_type=type_hints["template_id"])
+            check_type(argname="argument template_url", value=template_url, expected_type=type_hints["template_url"])
+            check_type(argname="argument template_version", value=template_version, expected_type=type_hints["template_version"])
         self._values: typing.Dict[str, typing.Any] = {
             "stack_group_name": stack_group_name,
         }
         if administration_role_name is not None:
             self._values["administration_role_name"] = administration_role_name
         if auto_deployment is not None:
             self._values["auto_deployment"] = auto_deployment
@@ -4692,37 +5170,43 @@
 ):
     '''A ROS resource type:  ``ALIYUN::ROS::StackInstances``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "StackInstancesProps",
+        props: typing.Union["StackInstancesProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::ROS::StackInstances``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(StackInstances.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrLastOperationId")
     def attr_last_operation_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute LastOperationId: undefined.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLastOperationId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrStacks")
     def attr_stacks(self) -> ros_cdk_core.IResolvable:
         '''Attribute Stacks: undefined.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrStacks"))
 
 
 @jsii.data_type(
@@ -4744,18 +5228,18 @@
 class StackInstancesProps:
     def __init__(
         self,
         *,
         region_ids: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]],
         stack_group_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         account_ids: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
-        deployment_targets: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosStackInstances.DeploymentTargetsProperty]] = None,
+        deployment_targets: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosStackInstances.DeploymentTargetsProperty, typing.Dict[str, typing.Any]]]] = None,
         disable_rollback: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         operation_description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        operation_preferences: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosStackInstances.OperationPreferencesProperty]] = None,
+        operation_preferences: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosStackInstances.OperationPreferencesProperty, typing.Dict[str, typing.Any]]]] = None,
         parameter_overrides: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]] = None,
         retain_stacks: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         timeout_in_minutes: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::ROS::StackInstances``.
 
         :param region_ids: Property regionIds: undefined.
@@ -4765,14 +5249,26 @@
         :param disable_rollback: Property disableRollback: undefined.
         :param operation_description: Property operationDescription: undefined.
         :param operation_preferences: Property operationPreferences: undefined.
         :param parameter_overrides: Property parameterOverrides: undefined.
         :param retain_stacks: Property retainStacks: undefined.
         :param timeout_in_minutes: Property timeoutInMinutes: undefined.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(StackInstancesProps.__init__)
+            check_type(argname="argument region_ids", value=region_ids, expected_type=type_hints["region_ids"])
+            check_type(argname="argument stack_group_name", value=stack_group_name, expected_type=type_hints["stack_group_name"])
+            check_type(argname="argument account_ids", value=account_ids, expected_type=type_hints["account_ids"])
+            check_type(argname="argument deployment_targets", value=deployment_targets, expected_type=type_hints["deployment_targets"])
+            check_type(argname="argument disable_rollback", value=disable_rollback, expected_type=type_hints["disable_rollback"])
+            check_type(argname="argument operation_description", value=operation_description, expected_type=type_hints["operation_description"])
+            check_type(argname="argument operation_preferences", value=operation_preferences, expected_type=type_hints["operation_preferences"])
+            check_type(argname="argument parameter_overrides", value=parameter_overrides, expected_type=type_hints["parameter_overrides"])
+            check_type(argname="argument retain_stacks", value=retain_stacks, expected_type=type_hints["retain_stacks"])
+            check_type(argname="argument timeout_in_minutes", value=timeout_in_minutes, expected_type=type_hints["timeout_in_minutes"])
         self._values: typing.Dict[str, typing.Any] = {
             "region_ids": region_ids,
             "stack_group_name": stack_group_name,
         }
         if account_ids is not None:
             self._values["account_ids"] = account_ids
         if deployment_targets is not None:
@@ -4913,14 +5409,23 @@
         :param resource_group_id: Property resourceGroupId: Resource group.
         :param template_body: Property templateBody: Structure containing the template body. It is just to facilitate the passing of template. It is raw content.Functions in TemplateBody will not be resolved in parent stack. You must specify either the TemplateBody or the TemplateURL property. If both are specified, TemplateBody will be used.
         :param template_id: Property templateId: Template ID of template containing the template body.
         :param template_url: Property templateUrl: Location of file containing the template body. The URL must point to a template (max size: 524288 bytes) that is located in a http web server(http, https), or an Aliyun OSS bucket(Such as oss://ros-template/demo?RegionId=cn-hangzhou, oss://ros-template/demo. RegionId is default to the value of RegionId Parameter of the request.). You must specify either the TemplateBody or the TemplateURL property. If both are specified, TemplateBody will be used.
         :param template_version: Property templateVersion: Template version of template containing the template body.
         :param timeout_mins: Property timeoutMins: The length of time, in minutes, to wait for the nested stack creation or update. Default to 60 minutes.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(StackProps.__init__)
+            check_type(argname="argument parameters", value=parameters, expected_type=type_hints["parameters"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument template_body", value=template_body, expected_type=type_hints["template_body"])
+            check_type(argname="argument template_id", value=template_id, expected_type=type_hints["template_id"])
+            check_type(argname="argument template_url", value=template_url, expected_type=type_hints["template_url"])
+            check_type(argname="argument template_version", value=template_version, expected_type=type_hints["template_version"])
+            check_type(argname="argument timeout_mins", value=timeout_mins, expected_type=type_hints["timeout_mins"])
         self._values: typing.Dict[str, typing.Any] = {}
         if parameters is not None:
             self._values["parameters"] = parameters
         if resource_group_id is not None:
             self._values["resource_group_id"] = resource_group_id
         if template_body is not None:
             self._values["template_body"] = template_body
@@ -5019,43 +5524,49 @@
 ):
     '''A ROS resource type:  ``ALIYUN::ROS::WaitCondition``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "WaitConditionProps",
+        props: typing.Union["WaitConditionProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::ROS::WaitCondition``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(WaitCondition.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrData")
     def attr_data(self) -> ros_cdk_core.IResolvable:
         '''Attribute Data: JSON serialized dict containing data associated with wait condition signals sent to the handle.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrData"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrErrorData")
     def attr_error_data(self) -> ros_cdk_core.IResolvable:
         '''Attribute ErrorData: JSON serialized dict containing data associated with wait condition error signals sent to the handle.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrErrorData"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrJoinedErrorData")
     def attr_joined_error_data(self) -> ros_cdk_core.IResolvable:
         '''Attribute JoinedErrorData: String containing data associated with wait condition error signals sent to the handle.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrJoinedErrorData"))
 
 
 class WaitConditionHandle(
@@ -5065,61 +5576,67 @@
 ):
     '''A ROS resource type:  ``ALIYUN::ROS::WaitConditionHandle``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: typing.Optional["WaitConditionHandleProps"] = None,
+        props: typing.Optional[typing.Union["WaitConditionHandleProps", typing.Dict[str, typing.Any]]] = None,
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::ROS::WaitConditionHandle``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(WaitConditionHandle.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCurlCli")
     def attr_curl_cli(self) -> ros_cdk_core.IResolvable:
         '''Attribute CurlCli: Convenience attribute, provides curl CLI command prefix, which can be used for signalling handle completion or failure.
 
         You can signal success by adding --data-binary '{"status": "SUCCESS"}' , or signal failure by adding --data-binary '{"status": "FAILURE"}'
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCurlCli"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrHeaders")
     def attr_headers(self) -> ros_cdk_core.IResolvable:
         '''Attribute Headers: HTTP POST Headers used for signalling handle completion or failure.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrHeaders"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPowerShellCurlCli")
     def attr_power_shell_curl_cli(self) -> ros_cdk_core.IResolvable:
         '''Attribute PowerShellCurlCli: Convenience attribute, provides curl CLI command prefix for PowerShell, which can be used for signalling handle completion or failure.
 
         As this cmdlet was introduced in PowerShell 3.0, ensure the version of PowerShell satisfies the constraint. (Show the version via $PSVersionTable.PSVersion.) You can signal success by adding -Body '{"status": "SUCCESS"}' , or signal failure by adding -Body '{"status": "FAILURE"}'
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPowerShellCurlCli"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrUrl")
     def attr_url(self) -> ros_cdk_core.IResolvable:
         '''Attribute URL: HTTP POST URL used for signalling handle completion or failure.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrUrl"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrWindowsCurlCli")
     def attr_windows_curl_cli(self) -> ros_cdk_core.IResolvable:
         '''Attribute WindowsCurlCli: Convenience attribute, provides curl CLI command prefix for Windows, which can be used for signalling handle completion or failure.
 
         As Windows does not support curl command, you need to install curl.exe and add it to PATH first. You can signal success by adding --data-binary "{"status": "SUCCESS"}" , or signal failure by adding --data-binary "{"status": "FAILURE"}"
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrWindowsCurlCli"))
@@ -5138,14 +5655,18 @@
         mode: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::ROS::WaitConditionHandle``.
 
         :param count: Property count: There are 3 preconditions that make Count taking effect: 1.Mode is set to Full. 2.Count >= 0. 3.The id of signal is not specified. If so, it will be a self-increasing integer started from 1. For example, the id of the first signal is 1, the id of the second signal is 2, and so on. If Count takes effect, signals with id > Count will be deleted before update. The default value is -1, which means no effect. It is recommended to quote the same value with WaitCondition.Count.
         :param mode: Property mode: If set to Increment, all old signals will be deleted before update. In this mode, WaitCondition.Count should reference an incremental value instead of a full value, such as ScalingGroupEnable.ScalingRuleArisExecuteResultNumberOfAddedInstances. If set to Full, no old signal will be deleted unless Count is set. In this mode, WaitCondition.Count should reference a full value, such as the same value with InstanceGroup.MaxAmount. It is recommended to use this mode with Count. Default to Full.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(WaitConditionHandleProps.__init__)
+            check_type(argname="argument count", value=count, expected_type=type_hints["count"])
+            check_type(argname="argument mode", value=mode, expected_type=type_hints["mode"])
         self._values: typing.Dict[str, typing.Any] = {}
         if count is not None:
             self._values["count"] = count
         if mode is not None:
             self._values["mode"] = mode
 
     @builtins.property
@@ -5210,14 +5731,20 @@
         '''Properties for defining a ``ALIYUN::ROS::WaitCondition``.
 
         :param handle: Property handle: A reference to the wait condition handle used to signal this wait condition.
         :param timeout: Property timeout: The number of seconds to wait for the correct number of signals to arrive.
         :param count: Property count: The number of success signals that must be received before the stack creation process continues.
         :param show_progress_event: Property showProgressEvent: Whether to generate progress changed event. Default to Disabled.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(WaitConditionProps.__init__)
+            check_type(argname="argument handle", value=handle, expected_type=type_hints["handle"])
+            check_type(argname="argument timeout", value=timeout, expected_type=type_hints["timeout"])
+            check_type(argname="argument count", value=count, expected_type=type_hints["count"])
+            check_type(argname="argument show_progress_event", value=show_progress_event, expected_type=type_hints["show_progress_event"])
         self._values: typing.Dict[str, typing.Any] = {
             "handle": handle,
             "timeout": timeout,
         }
         if count is not None:
             self._values["count"] = count
         if show_progress_event is not None:
```

### Comparing `ros-cdk-ros-1.0.8/src/ros_cdk_ros.egg-info/PKG-INFO` & `ros-cdk-ros-1.0.9/src/ros_cdk_ros.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-ros
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS ROS Construct Library
```

