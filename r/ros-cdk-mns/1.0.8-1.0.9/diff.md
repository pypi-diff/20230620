# Comparing `tmp/ros-cdk-mns-1.0.8.tar.gz` & `tmp/ros-cdk-mns-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-mns-1.0.8.tar", last modified: Thu Jul 14 02:13:19 2022, max compression
+gzip compressed data, was "dist/ros-cdk-mns-1.0.9.tar", last modified: Fri Sep 23 11:43:00 2022, max compression
```

## Comparing `ros-cdk-mns-1.0.8.tar` & `ros-cdk-mns-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:13:19.000000 ros-cdk-mns-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:13:19.000000 ros-cdk-mns-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:13:19.000000 ros-cdk-mns-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:13:19.000000 ros-cdk-mns-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:13:19.000000 ros-cdk-mns-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      179 2022-07-14 02:13:19.000000 ros-cdk-mns-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:13:19.000000 ros-cdk-mns-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:13:19.000000 ros-cdk-mns-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1794 2022-07-14 02:13:19.000000 ros-cdk-mns-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:13:19.000000 ros-cdk-mns-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:13:19.000000 ros-cdk-mns-1.0.8/src/ros_cdk_mns/
--rw-r--r--   0 root         (0) root         (0)    60721 2022-07-14 02:13:19.000000 ros-cdk-mns-1.0.8/src/ros_cdk_mns/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:13:19.000000 ros-cdk-mns-1.0.8/src/ros_cdk_mns/_jsii/
--rw-r--r--   0 root         (0) root         (0)      370 2022-07-14 02:13:19.000000 ros-cdk-mns-1.0.8/src/ros_cdk_mns/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    46816 2022-07-14 02:13:19.000000 ros-cdk-mns-1.0.8/src/ros_cdk_mns/_jsii/ros-cdk-mns@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:13:19.000000 ros-cdk-mns-1.0.8/src/ros_cdk_mns/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:13:19.000000 ros-cdk-mns-1.0.8/src/ros_cdk_mns.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:13:19.000000 ros-cdk-mns-1.0.8/src/ros_cdk_mns.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      400 2022-07-14 02:13:19.000000 ros-cdk-mns-1.0.8/src/ros_cdk_mns.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:13:19.000000 ros-cdk-mns-1.0.8/src/ros_cdk_mns.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:13:19.000000 ros-cdk-mns-1.0.8/src/ros_cdk_mns.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-07-14 02:13:19.000000 ros-cdk-mns-1.0.8/src/ros_cdk_mns.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:43:00.000000 ros-cdk-mns-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 11:42:59.000000 ros-cdk-mns-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 11:42:59.000000 ros-cdk-mns-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 11:42:59.000000 ros-cdk-mns-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 11:43:00.000000 ros-cdk-mns-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      179 2022-09-23 11:42:59.000000 ros-cdk-mns-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 11:42:59.000000 ros-cdk-mns-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 11:43:00.000000 ros-cdk-mns-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1823 2022-09-23 11:42:59.000000 ros-cdk-mns-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:43:00.000000 ros-cdk-mns-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:43:00.000000 ros-cdk-mns-1.0.9/src/ros_cdk_mns/
+-rw-r--r--   0 root         (0) root         (0)    72804 2022-09-23 11:42:59.000000 ros-cdk-mns-1.0.9/src/ros_cdk_mns/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:43:00.000000 ros-cdk-mns-1.0.9/src/ros_cdk_mns/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      404 2022-09-23 11:42:59.000000 ros-cdk-mns-1.0.9/src/ros_cdk_mns/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    46879 2022-09-23 11:42:59.000000 ros-cdk-mns-1.0.9/src/ros_cdk_mns/_jsii/ros-cdk-mns@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:42:59.000000 ros-cdk-mns-1.0.9/src/ros_cdk_mns/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:43:00.000000 ros-cdk-mns-1.0.9/src/ros_cdk_mns.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 11:42:59.000000 ros-cdk-mns-1.0.9/src/ros_cdk_mns.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      400 2022-09-23 11:42:59.000000 ros-cdk-mns-1.0.9/src/ros_cdk_mns.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:42:59.000000 ros-cdk-mns-1.0.9/src/ros_cdk_mns.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 11:42:59.000000 ros-cdk-mns-1.0.9/src/ros_cdk_mns.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-09-23 11:42:59.000000 ros-cdk-mns-1.0.9/src/ros_cdk_mns.egg-info/top_level.txt
```

### Comparing `ros-cdk-mns-1.0.8/LICENSE` & `ros-cdk-mns-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-mns-1.0.8/PKG-INFO` & `ros-cdk-mns-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-mns
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS MNS Construct Library
```

### Comparing `ros-cdk-mns-1.0.8/setup.py` & `ros-cdk-mns-1.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-mns",
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
         "ros_cdk_mns",
         "ros_cdk_mns._jsii"
     ],
     "package_data": {
         "ros_cdk_mns._jsii": [
-            "ros-cdk-mns@1.0.8.jsii.tgz"
+            "ros-cdk-mns@1.0.9.jsii.tgz"
         ],
         "ros_cdk_mns": [
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

### Comparing `ros-cdk-mns-1.0.8/src/ros_cdk_mns/__init__.py` & `ros-cdk-mns-1.0.9/src/ros_cdk_mns/__init__.py`

 * *Files 10% similar despite different names*

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
 
 
 class Queue(
     ros_cdk_core.Resource,
@@ -29,43 +31,49 @@
 ):
     '''A ROS resource type:  ``ALIYUN::MNS::Queue``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "QueueProps",
+        props: typing.Union["QueueProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::MNS::Queue``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Queue.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrArnWithSlash")
     def attr_arn_with_slash(self) -> ros_cdk_core.IResolvable:
         '''Attribute ARN.WithSlash: The ARN: acs:mns:$region:$accountid:/queues/$queueName.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrArnWithSlash"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrQueueName")
     def attr_queue_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute QueueName: Queue name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrQueueName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrQueueUrl")
     def attr_queue_url(self) -> ros_cdk_core.IResolvable:
         '''Attribute QueueUrl: URL of created queue.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrQueueUrl"))
 
 
 @jsii.data_type(
@@ -99,14 +107,23 @@
         :param delay_seconds: Property delaySeconds: It is measured in seconds. All messages sent to the queue can be consumed until the DelaySeconds expires. An integer between 0 and 604800 (7 days). The default value is 0
         :param logging_enabled: Property loggingEnabled: Whether to enable log management. "true" indicates that log management is enabled, whereas "false" indicates that log management is disabled. The default value is false
         :param maximum_message_size: Property maximumMessageSize: Maximum body length of a message sent to the queue, measured in bytes. An integer between 1024 (1K) and 65536 (64K). The default value is 65536 (64K).
         :param message_retention_period: Property messageRetentionPeriod: Maximum lifetime of the message in the queue, measured in seconds. After the time specified by this parameter expires, the message will be deleted no matter whether it has been consumed or not. An integer between 60 (1 minute) and 1296000 (15 days). The default value is 345600 (4 days)
         :param polling_wait_seconds: Property pollingWaitSeconds: It is the maximum time that a ReceiveMessage request could be waiting for any incoming messages, while there are no message in the queue. Measured in seconds. An integer between 0 and 30 seconds. The default value is 0 (seconds)
         :param visibility_timeout: Property visibilityTimeout: Duration in which a message stays in Inactive status after it is consumed from the queue. Measured in seconds. An integer between 1 and 43200 (12 hours). The default value is 30 (seconds)
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(QueueProps.__init__)
+            check_type(argname="argument queue_name", value=queue_name, expected_type=type_hints["queue_name"])
+            check_type(argname="argument delay_seconds", value=delay_seconds, expected_type=type_hints["delay_seconds"])
+            check_type(argname="argument logging_enabled", value=logging_enabled, expected_type=type_hints["logging_enabled"])
+            check_type(argname="argument maximum_message_size", value=maximum_message_size, expected_type=type_hints["maximum_message_size"])
+            check_type(argname="argument message_retention_period", value=message_retention_period, expected_type=type_hints["message_retention_period"])
+            check_type(argname="argument polling_wait_seconds", value=polling_wait_seconds, expected_type=type_hints["polling_wait_seconds"])
+            check_type(argname="argument visibility_timeout", value=visibility_timeout, expected_type=type_hints["visibility_timeout"])
         self._values: typing.Dict[str, typing.Any] = {
             "queue_name": queue_name,
         }
         if delay_seconds is not None:
             self._values["delay_seconds"] = delay_seconds
         if logging_enabled is not None:
             self._values["logging_enabled"] = logging_enabled
@@ -216,96 +233,111 @@
 ):
     '''A ROS template type:  ``ALIYUN::MNS::Queue``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosQueueProps",
+        props: typing.Union["RosQueueProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::MNS::Queue``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosQueue.__init__)
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
+            type_hints = typing.get_type_hints(RosQueue._render_properties)
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
     @jsii.member(jsii_name="attrArnWithSlash")
     def attr_arn_with_slash(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ARN.WithSlash: The ARN: acs:mns:$region:$accountid:/queues/$queueName
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrArnWithSlash"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrQueueName")
     def attr_queue_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: QueueName: Queue name
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrQueueName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrQueueUrl")
     def attr_queue_url(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: QueueUrl: URL of created queue
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrQueueUrl"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosQueue, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="queueName")
     def queue_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: queueName: Queue name
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "queueName"))
 
     @queue_name.setter
     def queue_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosQueue, "queue_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "queueName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="delaySeconds")
     def delay_seconds(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -315,17 +347,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "delaySeconds"))
 
     @delay_seconds.setter
     def delay_seconds(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosQueue, "delay_seconds").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "delaySeconds", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="loggingEnabled")
     def logging_enabled(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -335,17 +370,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "loggingEnabled"))
 
     @logging_enabled.setter
     def logging_enabled(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosQueue, "logging_enabled").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "loggingEnabled", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="maximumMessageSize")
     def maximum_message_size(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -355,17 +393,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "maximumMessageSize"))
 
     @maximum_message_size.setter
     def maximum_message_size(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosQueue, "maximum_message_size").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "maximumMessageSize", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="messageRetentionPeriod")
     def message_retention_period(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -375,17 +416,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "messageRetentionPeriod"))
 
     @message_retention_period.setter
     def message_retention_period(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosQueue, "message_retention_period").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "messageRetentionPeriod", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="pollingWaitSeconds")
     def polling_wait_seconds(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -395,17 +439,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "pollingWaitSeconds"))
 
     @polling_wait_seconds.setter
     def polling_wait_seconds(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosQueue, "polling_wait_seconds").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "pollingWaitSeconds", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="visibilityTimeout")
     def visibility_timeout(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -415,14 +462,17 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "visibilityTimeout"))
 
     @visibility_timeout.setter
     def visibility_timeout(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosQueue, "visibility_timeout").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "visibilityTimeout", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-mns.RosQueueProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -453,14 +503,23 @@
         :param delay_seconds: 
         :param logging_enabled: 
         :param maximum_message_size: 
         :param message_retention_period: 
         :param polling_wait_seconds: 
         :param visibility_timeout: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosQueueProps.__init__)
+            check_type(argname="argument queue_name", value=queue_name, expected_type=type_hints["queue_name"])
+            check_type(argname="argument delay_seconds", value=delay_seconds, expected_type=type_hints["delay_seconds"])
+            check_type(argname="argument logging_enabled", value=logging_enabled, expected_type=type_hints["logging_enabled"])
+            check_type(argname="argument maximum_message_size", value=maximum_message_size, expected_type=type_hints["maximum_message_size"])
+            check_type(argname="argument message_retention_period", value=message_retention_period, expected_type=type_hints["message_retention_period"])
+            check_type(argname="argument polling_wait_seconds", value=polling_wait_seconds, expected_type=type_hints["polling_wait_seconds"])
+            check_type(argname="argument visibility_timeout", value=visibility_timeout, expected_type=type_hints["visibility_timeout"])
         self._values: typing.Dict[str, typing.Any] = {
             "queue_name": queue_name,
         }
         if delay_seconds is not None:
             self._values["delay_seconds"] = delay_seconds
         if logging_enabled is not None:
             self._values["logging_enabled"] = logging_enabled
@@ -579,81 +638,93 @@
 ):
     '''A ROS template type:  ``ALIYUN::MNS::Subscription``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosSubscriptionProps",
+        props: typing.Union["RosSubscriptionProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::MNS::Subscription``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosSubscription.__init__)
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
+            type_hints = typing.get_type_hints(RosSubscription._render_properties)
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
     @jsii.member(jsii_name="attrSubscriptionName")
     def attr_subscription_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: SubscriptionName: Subscription name
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSubscriptionName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSubscriptionUrl")
     def attr_subscription_url(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: SubscriptionUrl: URL of created subscription
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSubscriptionUrl"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTopicName")
     def attr_topic_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TopicName: Topic name
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTopicName"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosSubscription, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="endpoint")
     def endpoint(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         endpoint: Terminal address of the message recipient for the created subscription.
         Currently, four types of endpoints are supported:
@@ -666,47 +737,56 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "endpoint"))
 
     @endpoint.setter
     def endpoint(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSubscription, "endpoint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "endpoint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="subscriptionName")
     def subscription_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: subscriptionName: Subscription name
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "subscriptionName"))
 
     @subscription_name.setter
     def subscription_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSubscription, "subscription_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "subscriptionName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="topicName")
     def topic_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: topicName: Topic name
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "topicName"))
 
     @topic_name.setter
     def topic_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSubscription, "topic_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "topicName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="filterTag")
     def filter_tag(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -716,17 +796,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "filterTag"))
 
     @filter_tag.setter
     def filter_tag(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSubscription, "filter_tag").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "filterTag", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="notifyContentFormat")
     def notify_content_format(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -736,17 +819,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "notifyContentFormat"))
 
     @notify_content_format.setter
     def notify_content_format(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSubscription, "notify_content_format").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "notifyContentFormat", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="notifyStrategy")
     def notify_strategy(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -756,14 +842,17 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "notifyStrategy"))
 
     @notify_strategy.setter
     def notify_strategy(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSubscription, "notify_strategy").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "notifyStrategy", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-mns.RosSubscriptionProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -791,14 +880,22 @@
         :param endpoint: 
         :param subscription_name: 
         :param topic_name: 
         :param filter_tag: 
         :param notify_content_format: 
         :param notify_strategy: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosSubscriptionProps.__init__)
+            check_type(argname="argument endpoint", value=endpoint, expected_type=type_hints["endpoint"])
+            check_type(argname="argument subscription_name", value=subscription_name, expected_type=type_hints["subscription_name"])
+            check_type(argname="argument topic_name", value=topic_name, expected_type=type_hints["topic_name"])
+            check_type(argname="argument filter_tag", value=filter_tag, expected_type=type_hints["filter_tag"])
+            check_type(argname="argument notify_content_format", value=notify_content_format, expected_type=type_hints["notify_content_format"])
+            check_type(argname="argument notify_strategy", value=notify_strategy, expected_type=type_hints["notify_strategy"])
         self._values: typing.Dict[str, typing.Any] = {
             "endpoint": endpoint,
             "subscription_name": subscription_name,
             "topic_name": topic_name,
         }
         if filter_tag is not None:
             self._values["filter_tag"] = filter_tag
@@ -900,96 +997,111 @@
 ):
     '''A ROS template type:  ``ALIYUN::MNS::Topic``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosTopicProps",
+        props: typing.Union["RosTopicProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::MNS::Topic``.
 
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
     @jsii.member(jsii_name="attrArnWithSlash")
     def attr_arn_with_slash(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ARN.WithSlash: The ARN: acs:mns:$region:$accountid:/topics/$topicName
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrArnWithSlash"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTopicName")
     def attr_topic_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TopicName: Topic name
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTopicName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTopicUrl")
     def attr_topic_url(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TopicUrl: URL of created topic
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTopicUrl"))
 
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
     @jsii.member(jsii_name="topicName")
     def topic_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: topicName: Topic name
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "topicName"))
 
     @topic_name.setter
     def topic_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTopic, "topic_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "topicName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="loggingEnabled")
     def logging_enabled(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -999,17 +1111,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "loggingEnabled"))
 
     @logging_enabled.setter
     def logging_enabled(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTopic, "logging_enabled").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "loggingEnabled", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="maximumMessageSize")
     def maximum_message_size(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1019,14 +1134,17 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "maximumMessageSize"))
 
     @maximum_message_size.setter
     def maximum_message_size(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTopic, "maximum_message_size").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "maximumMessageSize", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-mns.RosTopicProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -1045,14 +1163,19 @@
     ) -> None:
         '''Properties for defining a ``ALIYUN::MNS::Topic``.
 
         :param topic_name: 
         :param logging_enabled: 
         :param maximum_message_size: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosTopicProps.__init__)
+            check_type(argname="argument topic_name", value=topic_name, expected_type=type_hints["topic_name"])
+            check_type(argname="argument logging_enabled", value=logging_enabled, expected_type=type_hints["logging_enabled"])
+            check_type(argname="argument maximum_message_size", value=maximum_message_size, expected_type=type_hints["maximum_message_size"])
         self._values: typing.Dict[str, typing.Any] = {
             "topic_name": topic_name,
         }
         if logging_enabled is not None:
             self._values["logging_enabled"] = logging_enabled
         if maximum_message_size is not None:
             self._values["maximum_message_size"] = maximum_message_size
@@ -1111,43 +1234,49 @@
 ):
     '''A ROS resource type:  ``ALIYUN::MNS::Subscription``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "SubscriptionProps",
+        props: typing.Union["SubscriptionProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::MNS::Subscription``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Subscription.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSubscriptionName")
     def attr_subscription_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute SubscriptionName: Subscription name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSubscriptionName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSubscriptionUrl")
     def attr_subscription_url(self) -> ros_cdk_core.IResolvable:
         '''Attribute SubscriptionUrl: URL of created subscription.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSubscriptionUrl"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTopicName")
     def attr_topic_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute TopicName: Topic name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTopicName"))
 
 
 @jsii.data_type(
@@ -1178,14 +1307,22 @@
         :param endpoint: Property endpoint: Terminal address of the message recipient for the created subscription. Currently, four types of endpoints are supported: 1. HttpEndpoint, which must be prefixed with "http://"; 2. QueueEndpoint, in the format of acs:mns:{REGION}:{AccountID}:queues/{QueueName}; 3. MailEndpoint, in the format of mail:directmail:{MailAddress}; 4. SmsEndpoint, in the format of sms:directsms:anonymous or sms:directsms:{Phone}.
         :param subscription_name: Property subscriptionName: Subscription name.
         :param topic_name: Property topicName: Topic name.
         :param filter_tag: Property filterTag: Message filter tag in the created subscription (Only messages with consistent tags are pushed.) The value is a string of no more than 16 characters. The default value is no message filter.
         :param notify_content_format: Property notifyContentFormat: Format of the message content pushed to the endpoint. XML, JSON, or SIMPLIFIED; default value: XML. For details about message formats, refer to Basic Concepts/NotifyContentFormat.
         :param notify_strategy: Property notifyStrategy: Retry policy that will be applied when an error occurs during message push to the endpoint. BACKOFF_RETRY or EXPONENTIAL_DECAY_RETRY; default value: BACKOFF_RETRY. For details about retry policies, refer to Basic Concepts/NotifyStrategy.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(SubscriptionProps.__init__)
+            check_type(argname="argument endpoint", value=endpoint, expected_type=type_hints["endpoint"])
+            check_type(argname="argument subscription_name", value=subscription_name, expected_type=type_hints["subscription_name"])
+            check_type(argname="argument topic_name", value=topic_name, expected_type=type_hints["topic_name"])
+            check_type(argname="argument filter_tag", value=filter_tag, expected_type=type_hints["filter_tag"])
+            check_type(argname="argument notify_content_format", value=notify_content_format, expected_type=type_hints["notify_content_format"])
+            check_type(argname="argument notify_strategy", value=notify_strategy, expected_type=type_hints["notify_strategy"])
         self._values: typing.Dict[str, typing.Any] = {
             "endpoint": endpoint,
             "subscription_name": subscription_name,
             "topic_name": topic_name,
         }
         if filter_tag is not None:
             self._values["filter_tag"] = filter_tag
@@ -1272,43 +1409,49 @@
 ):
     '''A ROS resource type:  ``ALIYUN::MNS::Topic``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "TopicProps",
+        props: typing.Union["TopicProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::MNS::Topic``.
 
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
     @jsii.member(jsii_name="attrArnWithSlash")
     def attr_arn_with_slash(self) -> ros_cdk_core.IResolvable:
         '''Attribute ARN.WithSlash: The ARN: acs:mns:$region:$accountid:/topics/$topicName.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrArnWithSlash"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTopicName")
     def attr_topic_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute TopicName: Topic name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTopicName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTopicUrl")
     def attr_topic_url(self) -> ros_cdk_core.IResolvable:
         '''Attribute TopicUrl: URL of created topic.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTopicUrl"))
 
 
 @jsii.data_type(
@@ -1330,14 +1473,19 @@
     ) -> None:
         '''Properties for defining a ``ALIYUN::MNS::Topic``.
 
         :param topic_name: Property topicName: Topic name.
         :param logging_enabled: Property loggingEnabled: Whether to enable log management. "true" indicates that log management is enabled, whereas "false" indicates that log management is disabled. The default value is false
         :param maximum_message_size: Property maximumMessageSize: Maximum body length of a message sent to the topic, in the unit of bytes. An integer in the range of 1,024 (1 KB) to 65, 536 (64 KB); default value: 65,536 (64 KB).
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(TopicProps.__init__)
+            check_type(argname="argument topic_name", value=topic_name, expected_type=type_hints["topic_name"])
+            check_type(argname="argument logging_enabled", value=logging_enabled, expected_type=type_hints["logging_enabled"])
+            check_type(argname="argument maximum_message_size", value=maximum_message_size, expected_type=type_hints["maximum_message_size"])
         self._values: typing.Dict[str, typing.Any] = {
             "topic_name": topic_name,
         }
         if logging_enabled is not None:
             self._values["logging_enabled"] = logging_enabled
         if maximum_message_size is not None:
             self._values["maximum_message_size"] = maximum_message_size
```

### Comparing `ros-cdk-mns-1.0.8/src/ros_cdk_mns.egg-info/PKG-INFO` & `ros-cdk-mns-1.0.9/src/ros_cdk_mns.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-mns
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS MNS Construct Library
```

