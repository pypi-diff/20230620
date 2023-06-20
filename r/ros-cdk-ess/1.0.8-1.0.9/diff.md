# Comparing `tmp/ros-cdk-ess-1.0.8.tar.gz` & `tmp/ros-cdk-ess-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-ess-1.0.8.tar", last modified: Thu Jul 14 02:27:13 2022, max compression
+gzip compressed data, was "dist/ros-cdk-ess-1.0.9.tar", last modified: Fri Sep 23 11:13:59 2022, max compression
```

## Comparing `ros-cdk-ess-1.0.8.tar` & `ros-cdk-ess-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:27:13.000000 ros-cdk-ess-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:27:13.000000 ros-cdk-ess-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:27:13.000000 ros-cdk-ess-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:27:13.000000 ros-cdk-ess-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:27:13.000000 ros-cdk-ess-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      179 2022-07-14 02:27:13.000000 ros-cdk-ess-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:27:13.000000 ros-cdk-ess-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:27:13.000000 ros-cdk-ess-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1794 2022-07-14 02:27:13.000000 ros-cdk-ess-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:27:13.000000 ros-cdk-ess-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:27:13.000000 ros-cdk-ess-1.0.8/src/ros_cdk_ess/
--rw-r--r--   0 root         (0) root         (0)   389461 2022-07-14 02:27:13.000000 ros-cdk-ess-1.0.8/src/ros_cdk_ess/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:27:13.000000 ros-cdk-ess-1.0.8/src/ros_cdk_ess/_jsii/
--rw-r--r--   0 root         (0) root         (0)      370 2022-07-14 02:27:13.000000 ros-cdk-ess-1.0.8/src/ros_cdk_ess/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)   163995 2022-07-14 02:27:13.000000 ros-cdk-ess-1.0.8/src/ros_cdk_ess/_jsii/ros-cdk-ess@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:27:13.000000 ros-cdk-ess-1.0.8/src/ros_cdk_ess/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:27:13.000000 ros-cdk-ess-1.0.8/src/ros_cdk_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:27:13.000000 ros-cdk-ess-1.0.8/src/ros_cdk_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      400 2022-07-14 02:27:13.000000 ros-cdk-ess-1.0.8/src/ros_cdk_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:27:13.000000 ros-cdk-ess-1.0.8/src/ros_cdk_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:27:13.000000 ros-cdk-ess-1.0.8/src/ros_cdk_ess.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-07-14 02:27:13.000000 ros-cdk-ess-1.0.8/src/ros_cdk_ess.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:13:59.000000 ros-cdk-ess-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 11:13:58.000000 ros-cdk-ess-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 11:13:58.000000 ros-cdk-ess-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 11:13:58.000000 ros-cdk-ess-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 11:13:59.000000 ros-cdk-ess-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      179 2022-09-23 11:13:58.000000 ros-cdk-ess-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 11:13:58.000000 ros-cdk-ess-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 11:13:59.000000 ros-cdk-ess-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1823 2022-09-23 11:13:58.000000 ros-cdk-ess-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:13:59.000000 ros-cdk-ess-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:13:59.000000 ros-cdk-ess-1.0.9/src/ros_cdk_ess/
+-rw-r--r--   0 root         (0) root         (0)   459748 2022-09-23 11:13:58.000000 ros-cdk-ess-1.0.9/src/ros_cdk_ess/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:13:59.000000 ros-cdk-ess-1.0.9/src/ros_cdk_ess/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      404 2022-09-23 11:13:58.000000 ros-cdk-ess-1.0.9/src/ros_cdk_ess/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   163999 2022-09-23 11:13:58.000000 ros-cdk-ess-1.0.9/src/ros_cdk_ess/_jsii/ros-cdk-ess@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:13:58.000000 ros-cdk-ess-1.0.9/src/ros_cdk_ess/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:13:59.000000 ros-cdk-ess-1.0.9/src/ros_cdk_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 11:13:59.000000 ros-cdk-ess-1.0.9/src/ros_cdk_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      400 2022-09-23 11:13:59.000000 ros-cdk-ess-1.0.9/src/ros_cdk_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:13:59.000000 ros-cdk-ess-1.0.9/src/ros_cdk_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 11:13:59.000000 ros-cdk-ess-1.0.9/src/ros_cdk_ess.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-09-23 11:13:59.000000 ros-cdk-ess-1.0.9/src/ros_cdk_ess.egg-info/top_level.txt
```

### Comparing `ros-cdk-ess-1.0.8/LICENSE` & `ros-cdk-ess-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-ess-1.0.8/PKG-INFO` & `ros-cdk-ess-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-ess
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS ESS Construct Library
```

### Comparing `ros-cdk-ess-1.0.8/setup.py` & `ros-cdk-ess-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-ess",
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
         "ros_cdk_ess",
         "ros_cdk_ess._jsii"
     ],
     "package_data": {
         "ros_cdk_ess._jsii": [
-            "ros-cdk-ess@1.0.8.jsii.tgz"
+            "ros-cdk-ess@1.0.9.jsii.tgz"
         ],
         "ros_cdk_ess": [
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

### Comparing `ros-cdk-ess-1.0.8/src/ros_cdk_ess/__init__.py` & `ros-cdk-ess-1.0.9/src/ros_cdk_ess/__init__.py`

 * *Files 27% similar despite different names*

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
 
 
 class AlarmTask(
     ros_cdk_core.Resource,
@@ -29,31 +31,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::ESS::AlarmTask``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "AlarmTaskProps",
+        props: typing.Union["AlarmTaskProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::ESS::AlarmTask``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(AlarmTask.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAlarmTaskId")
     def attr_alarm_task_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute AlarmTaskId: The alarm task ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAlarmTaskId"))
 
 
 class AlarmTaskEnable(
@@ -63,28 +71,34 @@
 ):
     '''A ROS resource type:  ``ALIYUN::ESS::AlarmTaskEnable``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "AlarmTaskEnableProps",
+        props: typing.Union["AlarmTaskEnableProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::ESS::AlarmTaskEnable``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(AlarmTaskEnable.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-ess.AlarmTaskEnableProps",
     jsii_struct_bases=[],
     name_mapping={"alarm_task_id": "alarmTaskId", "enable": "enable"},
@@ -97,14 +111,18 @@
         enable: typing.Union[builtins.bool, ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::ESS::AlarmTaskEnable``.
 
         :param alarm_task_id: Property alarmTaskId: The id of alarm task.
         :param enable: Property enable: Enable alarm task or not.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(AlarmTaskEnableProps.__init__)
+            check_type(argname="argument alarm_task_id", value=alarm_task_id, expected_type=type_hints["alarm_task_id"])
+            check_type(argname="argument enable", value=enable, expected_type=type_hints["enable"])
         self._values: typing.Dict[str, typing.Any] = {
             "alarm_task_id": alarm_task_id,
             "enable": enable,
         }
 
     @builtins.property
     def alarm_task_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -157,15 +175,15 @@
         *,
         alarm_action: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]],
         metric_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         scaling_group_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         threshold: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
         comparison_operator: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        dimensions: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosAlarmTask.DimensionsProperty"]]]] = None,
+        dimensions: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosAlarmTask.DimensionsProperty", typing.Dict[str, typing.Any]]]]]] = None,
         evaluation_count: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         group_id: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         metric_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         period: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         statistics: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
@@ -181,14 +199,29 @@
         :param evaluation_count: Property evaluationCount: Evaluation Count.
         :param group_id: Property groupId: Group Id.
         :param metric_type: Property metricType: Metric Type.
         :param name: Property name: Name.
         :param period: Property period: Period.
         :param statistics: Property statistics: Statistics.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(AlarmTaskProps.__init__)
+            check_type(argname="argument alarm_action", value=alarm_action, expected_type=type_hints["alarm_action"])
+            check_type(argname="argument metric_name", value=metric_name, expected_type=type_hints["metric_name"])
+            check_type(argname="argument scaling_group_id", value=scaling_group_id, expected_type=type_hints["scaling_group_id"])
+            check_type(argname="argument threshold", value=threshold, expected_type=type_hints["threshold"])
+            check_type(argname="argument comparison_operator", value=comparison_operator, expected_type=type_hints["comparison_operator"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument dimensions", value=dimensions, expected_type=type_hints["dimensions"])
+            check_type(argname="argument evaluation_count", value=evaluation_count, expected_type=type_hints["evaluation_count"])
+            check_type(argname="argument group_id", value=group_id, expected_type=type_hints["group_id"])
+            check_type(argname="argument metric_type", value=metric_type, expected_type=type_hints["metric_type"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+            check_type(argname="argument statistics", value=statistics, expected_type=type_hints["statistics"])
         self._values: typing.Dict[str, typing.Any] = {
             "alarm_action": alarm_action,
             "metric_name": metric_name,
             "scaling_group_id": scaling_group_id,
             "threshold": threshold,
         }
         if comparison_operator is not None:
@@ -331,31 +364,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::ESS::LifecycleHook``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "LifecycleHookProps",
+        props: typing.Union["LifecycleHookProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::ESS::LifecycleHook``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(LifecycleHook.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrLifecycleHookId")
     def attr_lifecycle_hook_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute LifecycleHookId: The lifecycle hook ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLifecycleHookId"))
 
 
 @jsii.data_type(
@@ -389,14 +428,23 @@
         :param scaling_group_id: Property scalingGroupId: The ID of the scaling group.
         :param default_result: Property defaultResult: The action that the scaling group takes when the lifecycle hook times out. Value range: CONTINUE: the scaling group continues with the scale-in or scale-out process. ABANDON: the scaling group stops any remaining action of the scale-in or scale-out event. Default value: CONTINUE If the scaling group has multiple lifecycle hooks and one of them is terminated by the DefaultResult=ABANDON parameter during a scale-in event (SCALE_IN), the remaining lifecycle hooks under the same scaling group will also be terminated. Otherwise, the action following the wait state is the next action, as specified in the parameter DefaultResult, after the last lifecycle event under the same scaling group.
         :param heartbeat_timeout: Property heartbeatTimeout: The time, in seconds, that can elapse before the lifecycle hook times out. If the lifecycle hook times out, the scaling group performs the default action (DefaultResult). The range is from 30 to 86400 seconds. The default value is 600 seconds. You can prevent the lifecycle hook from timing out by calling the RecordLifecycleActionHeartbeat operation. You can also terminate the lifecycle action by calling the CompleteLifecycleAction operation.
         :param lifecycle_hook_name: Property lifecycleHookName: The name of the lifecycle hook. Each name must be unique within a scaling group. The name must be 2 to 64 characters in length and can contain letters, numbers, Chinese characters, and special characters including underscores (_), hyphens (-) and periods (.). Default value: Lifecycle Hook ID
         :param notification_arn: Property notificationArn: The Alibaba Cloud Resource Name (ARN) of the notification target that Auto Scaling will use to notify you when an instance is in the transition state for the lifecycle hook. This target can be either an MNS queue or an MNS topic. The format of the parameter value is acs:ess:{region}:{account-id}:{resource-relative-id}. region: the region to which the scaling group locates account-id: Alibaba Cloud ID For example: MNS queue: acs:ess:{region}:{account-id}:queue/{queuename} MNS topic: acs:ess:{region}:{account-id}:topic/{topicname} OOS template: acs:ess:{region}:{account-id}:oos/{templatename}
         :param notification_metadata: Property notificationMetadata: The fixed string that you want to include when Auto Scaling sends a message about the wait state of the scaling activity to the notification target. The length of the parameter can be up to 4096 characters. Auto Scaling will send the specified NotificationMetadata parameter along with the notification message so that you can easily categorize your notifications. The NotificationMetadata parameter will only take effect after you specify the NotificationArn parameter.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(LifecycleHookProps.__init__)
+            check_type(argname="argument lifecycle_transition", value=lifecycle_transition, expected_type=type_hints["lifecycle_transition"])
+            check_type(argname="argument scaling_group_id", value=scaling_group_id, expected_type=type_hints["scaling_group_id"])
+            check_type(argname="argument default_result", value=default_result, expected_type=type_hints["default_result"])
+            check_type(argname="argument heartbeat_timeout", value=heartbeat_timeout, expected_type=type_hints["heartbeat_timeout"])
+            check_type(argname="argument lifecycle_hook_name", value=lifecycle_hook_name, expected_type=type_hints["lifecycle_hook_name"])
+            check_type(argname="argument notification_arn", value=notification_arn, expected_type=type_hints["notification_arn"])
+            check_type(argname="argument notification_metadata", value=notification_metadata, expected_type=type_hints["notification_metadata"])
         self._values: typing.Dict[str, typing.Any] = {
             "lifecycle_transition": lifecycle_transition,
             "scaling_group_id": scaling_group_id,
         }
         if default_result is not None:
             self._values["default_result"] = default_result
         if heartbeat_timeout is not None:
@@ -510,277 +558,328 @@
 ):
     '''A ROS template type:  ``ALIYUN::ESS::AlarmTask``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosAlarmTaskProps",
+        props: typing.Union["RosAlarmTaskProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::ESS::AlarmTask``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosAlarmTask.__init__)
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
+            type_hints = typing.get_type_hints(RosAlarmTask._render_properties)
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
     @jsii.member(jsii_name="attrAlarmTaskId")
     def attr_alarm_task_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: AlarmTaskId: The alarm task ID
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAlarmTaskId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="alarmAction")
     def alarm_action(
         self,
     ) -> typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]:
         '''
         :Property: alarmAction: Alarm Actions
         '''
         return typing.cast(typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]], jsii.get(self, "alarmAction"))
 
     @alarm_action.setter
     def alarm_action(
         self,
         value: typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAlarmTask, "alarm_action").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "alarmAction", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAlarmTask, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="metricName")
     def metric_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: metricName: Metric Name
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "metricName"))
 
     @metric_name.setter
     def metric_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAlarmTask, "metric_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "metricName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="scalingGroupId")
     def scaling_group_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: scalingGroupId: The ID of the scaling group.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "scalingGroupId"))
 
     @scaling_group_id.setter
     def scaling_group_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAlarmTask, "scaling_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "scalingGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="threshold")
     def threshold(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property: threshold: Threshold
         '''
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "threshold"))
 
     @threshold.setter
     def threshold(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAlarmTask, "threshold").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "threshold", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="comparisonOperator")
     def comparison_operator(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: comparisonOperator: Comparison Operator
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "comparisonOperator"))
 
     @comparison_operator.setter
     def comparison_operator(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAlarmTask, "comparison_operator").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "comparisonOperator", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: description: Description
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAlarmTask, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dimensions")
     def dimensions(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosAlarmTask.DimensionsProperty"]]]]:
         '''
         :Property: dimensions: Dimensions
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosAlarmTask.DimensionsProperty"]]]], jsii.get(self, "dimensions"))
 
     @dimensions.setter
     def dimensions(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosAlarmTask.DimensionsProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAlarmTask, "dimensions").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dimensions", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="evaluationCount")
     def evaluation_count(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: evaluationCount: Evaluation Count
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "evaluationCount"))
 
     @evaluation_count.setter
     def evaluation_count(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAlarmTask, "evaluation_count").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "evaluationCount", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="groupId")
     def group_id(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: groupId: Group Id
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "groupId"))
 
     @group_id.setter
     def group_id(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAlarmTask, "group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "groupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="metricType")
     def metric_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: metricType: Metric Type
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "metricType"))
 
     @metric_type.setter
     def metric_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAlarmTask, "metric_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "metricType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="name")
     def name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: name: Name
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "name"))
 
     @name.setter
     def name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAlarmTask, "name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "name", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="period")
     def period(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: period: Period
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "period"))
 
     @period.setter
     def period(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAlarmTask, "period").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "period", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="statistics")
     def statistics(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: statistics: Statistics
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "statistics"))
 
     @statistics.setter
     def statistics(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAlarmTask, "statistics").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "statistics", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-ess.RosAlarmTask.DimensionsProperty",
         jsii_struct_bases=[],
         name_mapping={
             "dimension_key": "dimensionKey",
@@ -794,14 +893,18 @@
             dimension_key: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             dimension_value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param dimension_key: 
             :param dimension_value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosAlarmTask.DimensionsProperty.__init__)
+                check_type(argname="argument dimension_key", value=dimension_key, expected_type=type_hints["dimension_key"])
+                check_type(argname="argument dimension_value", value=dimension_value, expected_type=type_hints["dimension_value"])
             self._values: typing.Dict[str, typing.Any] = {
                 "dimension_key": dimension_key,
                 "dimension_value": dimension_value,
             }
 
         @builtins.property
         def dimension_key(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -842,85 +945,103 @@
 ):
     '''A ROS template type:  ``ALIYUN::ESS::AlarmTaskEnable``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosAlarmTaskEnableProps",
+        props: typing.Union["RosAlarmTaskEnableProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::ESS::AlarmTaskEnable``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosAlarmTaskEnable.__init__)
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
+            type_hints = typing.get_type_hints(RosAlarmTaskEnable._render_properties)
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
     @jsii.member(jsii_name="alarmTaskId")
     def alarm_task_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: alarmTaskId: The id of alarm task.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "alarmTaskId"))
 
     @alarm_task_id.setter
     def alarm_task_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAlarmTaskEnable, "alarm_task_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "alarmTaskId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enable")
     def enable(self) -> typing.Union[builtins.bool, ros_cdk_core.IResolvable]:
         '''
         :Property: enable: Enable alarm task or not
         '''
         return typing.cast(typing.Union[builtins.bool, ros_cdk_core.IResolvable], jsii.get(self, "enable"))
 
     @enable.setter
     def enable(
         self,
         value: typing.Union[builtins.bool, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAlarmTaskEnable, "enable").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enable", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         '''A factory method that creates a new instance of this class from an object containing the properties of this ROS resource.'''
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAlarmTaskEnable, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-ess.RosAlarmTaskEnableProps",
     jsii_struct_bases=[],
     name_mapping={"alarm_task_id": "alarmTaskId", "enable": "enable"},
@@ -933,14 +1054,18 @@
         enable: typing.Union[builtins.bool, ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::ESS::AlarmTaskEnable``.
 
         :param alarm_task_id: 
         :param enable: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosAlarmTaskEnableProps.__init__)
+            check_type(argname="argument alarm_task_id", value=alarm_task_id, expected_type=type_hints["alarm_task_id"])
+            check_type(argname="argument enable", value=enable, expected_type=type_hints["enable"])
         self._values: typing.Dict[str, typing.Any] = {
             "alarm_task_id": alarm_task_id,
             "enable": enable,
         }
 
     @builtins.property
     def alarm_task_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -997,15 +1122,15 @@
         *,
         alarm_action: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]],
         metric_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         scaling_group_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         threshold: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
         comparison_operator: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        dimensions: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosAlarmTask.DimensionsProperty]]]] = None,
+        dimensions: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosAlarmTask.DimensionsProperty, typing.Dict[str, typing.Any]]]]]] = None,
         evaluation_count: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         group_id: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         metric_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         period: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         statistics: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
@@ -1021,14 +1146,29 @@
         :param evaluation_count: 
         :param group_id: 
         :param metric_type: 
         :param name: 
         :param period: 
         :param statistics: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosAlarmTaskProps.__init__)
+            check_type(argname="argument alarm_action", value=alarm_action, expected_type=type_hints["alarm_action"])
+            check_type(argname="argument metric_name", value=metric_name, expected_type=type_hints["metric_name"])
+            check_type(argname="argument scaling_group_id", value=scaling_group_id, expected_type=type_hints["scaling_group_id"])
+            check_type(argname="argument threshold", value=threshold, expected_type=type_hints["threshold"])
+            check_type(argname="argument comparison_operator", value=comparison_operator, expected_type=type_hints["comparison_operator"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument dimensions", value=dimensions, expected_type=type_hints["dimensions"])
+            check_type(argname="argument evaluation_count", value=evaluation_count, expected_type=type_hints["evaluation_count"])
+            check_type(argname="argument group_id", value=group_id, expected_type=type_hints["group_id"])
+            check_type(argname="argument metric_type", value=metric_type, expected_type=type_hints["metric_type"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+            check_type(argname="argument statistics", value=statistics, expected_type=type_hints["statistics"])
         self._values: typing.Dict[str, typing.Any] = {
             "alarm_action": alarm_action,
             "metric_name": metric_name,
             "scaling_group_id": scaling_group_id,
             "threshold": threshold,
         }
         if comparison_operator is not None:
@@ -1197,65 +1337,77 @@
 ):
     '''A ROS template type:  ``ALIYUN::ESS::LifecycleHook``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosLifecycleHookProps",
+        props: typing.Union["RosLifecycleHookProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::ESS::LifecycleHook``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosLifecycleHook.__init__)
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
+            type_hints = typing.get_type_hints(RosLifecycleHook._render_properties)
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
     @jsii.member(jsii_name="attrLifecycleHookId")
     def attr_lifecycle_hook_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: LifecycleHookId: The lifecycle hook ID
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLifecycleHookId"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosLifecycleHook, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="lifecycleTransition")
     def lifecycle_transition(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
@@ -1266,32 +1418,38 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "lifecycleTransition"))
 
     @lifecycle_transition.setter
     def lifecycle_transition(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLifecycleHook, "lifecycle_transition").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "lifecycleTransition", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="scalingGroupId")
     def scaling_group_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: scalingGroupId: The ID of the scaling group.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "scalingGroupId"))
 
     @scaling_group_id.setter
     def scaling_group_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLifecycleHook, "scaling_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "scalingGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="defaultResult")
     def default_result(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1304,17 +1462,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "defaultResult"))
 
     @default_result.setter
     def default_result(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLifecycleHook, "default_result").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "defaultResult", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="heartbeatTimeout")
     def heartbeat_timeout(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1324,17 +1485,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "heartbeatTimeout"))
 
     @heartbeat_timeout.setter
     def heartbeat_timeout(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLifecycleHook, "heartbeat_timeout").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "heartbeatTimeout", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="lifecycleHookName")
     def lifecycle_hook_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1344,17 +1508,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "lifecycleHookName"))
 
     @lifecycle_hook_name.setter
     def lifecycle_hook_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLifecycleHook, "lifecycle_hook_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "lifecycleHookName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="notificationArn")
     def notification_arn(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1369,31 +1536,37 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "notificationArn"))
 
     @notification_arn.setter
     def notification_arn(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLifecycleHook, "notification_arn").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "notificationArn", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="notificationMetadata")
     def notification_metadata(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: notificationMetadata: The fixed string that you want to include when Auto Scaling sends a message about the wait state of the scaling activity to the notification target. The length of the parameter can be up to 4096 characters. Auto Scaling will send the specified NotificationMetadata parameter along with the notification message so that you can easily categorize your notifications. The NotificationMetadata parameter will only take effect after you specify the NotificationArn parameter.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "notificationMetadata"))
 
     @notification_metadata.setter
     def notification_metadata(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLifecycleHook, "notification_metadata").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "notificationMetadata", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-ess.RosLifecycleHookProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -1424,14 +1597,23 @@
         :param scaling_group_id: 
         :param default_result: 
         :param heartbeat_timeout: 
         :param lifecycle_hook_name: 
         :param notification_arn: 
         :param notification_metadata: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosLifecycleHookProps.__init__)
+            check_type(argname="argument lifecycle_transition", value=lifecycle_transition, expected_type=type_hints["lifecycle_transition"])
+            check_type(argname="argument scaling_group_id", value=scaling_group_id, expected_type=type_hints["scaling_group_id"])
+            check_type(argname="argument default_result", value=default_result, expected_type=type_hints["default_result"])
+            check_type(argname="argument heartbeat_timeout", value=heartbeat_timeout, expected_type=type_hints["heartbeat_timeout"])
+            check_type(argname="argument lifecycle_hook_name", value=lifecycle_hook_name, expected_type=type_hints["lifecycle_hook_name"])
+            check_type(argname="argument notification_arn", value=notification_arn, expected_type=type_hints["notification_arn"])
+            check_type(argname="argument notification_metadata", value=notification_metadata, expected_type=type_hints["notification_metadata"])
         self._values: typing.Dict[str, typing.Any] = {
             "lifecycle_transition": lifecycle_transition,
             "scaling_group_id": scaling_group_id,
         }
         if default_result is not None:
             self._values["default_result"] = default_result
         if heartbeat_timeout is not None:
@@ -1556,80 +1738,95 @@
 ):
     '''A ROS template type:  ``ALIYUN::ESS::ScalingConfiguration``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosScalingConfigurationProps",
+        props: typing.Union["RosScalingConfigurationProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::ESS::ScalingConfiguration``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosScalingConfiguration.__init__)
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
+            type_hints = typing.get_type_hints(RosScalingConfiguration._render_properties)
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
     @jsii.member(jsii_name="attrScalingConfigurationId")
     def attr_scaling_configuration_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ScalingConfigurationId: The scaling configuration id
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScalingConfigurationId"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosScalingConfiguration, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="scalingGroupId")
     def scaling_group_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: scalingGroupId: Scaling group id to create the scaling configuration.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "scalingGroupId"))
 
     @scaling_group_id.setter
     def scaling_group_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingConfiguration, "scaling_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "scalingGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="creditSpecification")
     def credit_specification(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1640,204 +1837,240 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "creditSpecification"))
 
     @credit_specification.setter
     def credit_specification(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingConfiguration, "credit_specification").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "creditSpecification", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="deploymentSetId")
     def deployment_set_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: deploymentSetId: Deployment set ID.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "deploymentSetId"))
 
     @deployment_set_id.setter
     def deployment_set_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingConfiguration, "deployment_set_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "deploymentSetId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="diskMappings")
     def disk_mappings(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosScalingConfiguration.DiskMappingsProperty"]]]]:
         '''
         :Property: diskMappings: Disk mappings to attach to instance.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosScalingConfiguration.DiskMappingsProperty"]]]], jsii.get(self, "diskMappings"))
 
     @disk_mappings.setter
     def disk_mappings(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosScalingConfiguration.DiskMappingsProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingConfiguration, "disk_mappings").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "diskMappings", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="hpcClusterId")
     def hpc_cluster_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: hpcClusterId: The HPC cluster ID to which the instance belongs.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "hpcClusterId"))
 
     @hpc_cluster_id.setter
     def hpc_cluster_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingConfiguration, "hpc_cluster_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "hpcClusterId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="imageFamily")
     def image_family(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: imageFamily: The name of the image family. You can configure this parameter to obtain the latest available custom images within the specified image family. The images are used to create ECS instances. If you have set the ImageId parameter, you cannot set the ImageFamily parameter.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "imageFamily"))
 
     @image_family.setter
     def image_family(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingConfiguration, "image_family").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "imageFamily", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="imageId")
     def image_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: imageId: Image ID to create ecs instance .
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "imageId"))
 
     @image_id.setter
     def image_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingConfiguration, "image_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "imageId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceId")
     def instance_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: instanceId: Source ECS instance to copy configuration, if the properties is setting, Which will copy the InstanceType, ImageId, InternetChargeType, IoOptimized,UserData, KeyPairName, RamRoleName, InternetMaxBandwidthIn,InternetMaxBandwidthOut, and first security group id from source instance, you can also specify the relative properties to overwrite the properties copy from source instance id.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "instanceId"))
 
     @instance_id.setter
     def instance_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingConfiguration, "instance_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceName")
     def instance_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: instanceName: The name of the instance launched from the current scaling configuration.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "instanceName"))
 
     @instance_name.setter
     def instance_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingConfiguration, "instance_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceType")
     def instance_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: instanceType: ecs supported instance type.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "instanceType"))
 
     @instance_type.setter
     def instance_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingConfiguration, "instance_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceTypes")
     def instance_types(
         self,
     ) -> typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]]:
         '''
         :Property: instanceTypes: ecs supported instance types. Length [1,10]. If InstanceTypes is specified,the InstanceType will be ignored.
         '''
         return typing.cast(typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]], jsii.get(self, "instanceTypes"))
 
     @instance_types.setter
     def instance_types(
         self,
         value: typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingConfiguration, "instance_types").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceTypes", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="internetChargeType")
     def internet_charge_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: internetChargeType: Instance internet access charge type.Support 'PayByBandwidth' and 'PayByTraffic' only.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "internetChargeType"))
 
     @internet_charge_type.setter
     def internet_charge_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingConfiguration, "internet_charge_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internetChargeType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="internetMaxBandwidthIn")
     def internet_max_bandwidth_in(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: internetMaxBandwidthIn: Maximum incoming bandwidth from the public network, measured in Mbps (Mega bit per second). The value range is [1,200]. If this parameter value is not specified, AliyunAPI automatically sets the value to 200 Mbps.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "internetMaxBandwidthIn"))
 
     @internet_max_bandwidth_in.setter
     def internet_max_bandwidth_in(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingConfiguration, "internet_max_bandwidth_in").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internetMaxBandwidthIn", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="internetMaxBandwidthOut")
     def internet_max_bandwidth_out(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1848,68 +2081,80 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "internetMaxBandwidthOut"))
 
     @internet_max_bandwidth_out.setter
     def internet_max_bandwidth_out(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingConfiguration, "internet_max_bandwidth_out").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internetMaxBandwidthOut", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="ioOptimized")
     def io_optimized(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: ioOptimized: The 'optimized' instance can provide better IO performance. Support 'none' and 'optimized' only, default is 'none'.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "ioOptimized"))
 
     @io_optimized.setter
     def io_optimized(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingConfiguration, "io_optimized").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ioOptimized", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="ipv6AddressCount")
     def ipv6_address_count(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: ipv6AddressCount: The number of randomly generated IPv6 addresses to be assigned to the elastic network interface (ENI).
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "ipv6AddressCount"))
 
     @ipv6_address_count.setter
     def ipv6_address_count(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingConfiguration, "ipv6_address_count").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ipv6AddressCount", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="keyPairName")
     def key_pair_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: keyPairName: SSH key pair name.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "keyPairName"))
 
     @key_pair_name.setter
     def key_pair_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingConfiguration, "key_pair_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "keyPairName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="loadBalancerWeight")
     def load_balancer_weight(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1919,119 +2164,140 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "loadBalancerWeight"))
 
     @load_balancer_weight.setter
     def load_balancer_weight(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingConfiguration, "load_balancer_weight").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "loadBalancerWeight", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="passwordInherit")
     def password_inherit(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: passwordInherit: Whether to use the password pre-configured in the image you select or not. When PasswordInherit is specified, the Password must be null. For a secure access, make sure that the selected image has password configured.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "passwordInherit"))
 
     @password_inherit.setter
     def password_inherit(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingConfiguration, "password_inherit").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "passwordInherit", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="ramRoleName")
     def ram_role_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: ramRoleName: Instance RAM role name. The name is provided and maintained by Resource Access Management (RAM) and can be queried using ListRoles. For more information, see RAM API CreateRole and ListRoles.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "ramRoleName"))
 
     @ram_role_name.setter
     def ram_role_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingConfiguration, "ram_role_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ramRoleName", value)
 
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
+            type_hints = typing.get_type_hints(getattr(RosScalingConfiguration, "resource_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "resourceGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="scalingConfigurationName")
     def scaling_configuration_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: scalingConfigurationName: Name of created scaling configuration.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "scalingConfigurationName"))
 
     @scaling_configuration_name.setter
     def scaling_configuration_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingConfiguration, "scaling_configuration_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "scalingConfigurationName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="securityGroupId")
     def security_group_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: securityGroupId: Security Group to create ecs instance.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "securityGroupId"))
 
     @security_group_id.setter
     def security_group_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingConfiguration, "security_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "securityGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="spotPriceLimit")
     def spot_price_limit(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: spotPriceLimit: Set the hourly maximum price for the instance. Supports a maximum of 3 decimal places, and the parameter takes effect only when the value of SpotStrategy is SpotWithPriceLimit.It is a default value for all instance types, and can be overwrite by SpotPriceLimitForInstanceType
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "spotPriceLimit"))
 
     @spot_price_limit.setter
     def spot_price_limit(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingConfiguration, "spot_price_limit").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "spotPriceLimit", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="spotPriceLimitForInstanceType")
     def spot_price_limit_for_instance_type(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]]:
         '''
         :Property:
 
@@ -2047,17 +2313,20 @@
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]], jsii.get(self, "spotPriceLimitForInstanceType"))
 
     @spot_price_limit_for_instance_type.setter
     def spot_price_limit_for_instance_type(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingConfiguration, "spot_price_limit_for_instance_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "spotPriceLimitForInstanceType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="spotStrategy")
     def spot_strategy(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2070,85 +2339,100 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "spotStrategy"))
 
     @spot_strategy.setter
     def spot_strategy(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingConfiguration, "spot_strategy").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "spotStrategy", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="systemDiskAutoSnapshotPolicyId")
     def system_disk_auto_snapshot_policy_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: systemDiskAutoSnapshotPolicyId: Auto snapshot policy ID.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "systemDiskAutoSnapshotPolicyId"))
 
     @system_disk_auto_snapshot_policy_id.setter
     def system_disk_auto_snapshot_policy_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingConfiguration, "system_disk_auto_snapshot_policy_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "systemDiskAutoSnapshotPolicyId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="systemDiskCategory")
     def system_disk_category(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: systemDiskCategory: Category of system disk. Default is cloud.support cloud|cloud_efficiency|cloud_ssd|cloud_essd|ephemeral_ssd
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "systemDiskCategory"))
 
     @system_disk_category.setter
     def system_disk_category(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingConfiguration, "system_disk_category").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "systemDiskCategory", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="systemDiskPerformanceLevel")
     def system_disk_performance_level(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: systemDiskPerformanceLevel: The performance level of an ESSD.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "systemDiskPerformanceLevel"))
 
     @system_disk_performance_level.setter
     def system_disk_performance_level(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingConfiguration, "system_disk_performance_level").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "systemDiskPerformanceLevel", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="systemDiskSize")
     def system_disk_size(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: systemDiskSize: Size of system disk. Unit is GB.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "systemDiskSize"))
 
     @system_disk_size.setter
     def system_disk_size(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingConfiguration, "system_disk_size").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "systemDiskSize", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tagList")
     def tag_list(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosScalingConfiguration.TagListProperty"]]]]:
         '''
         :Property:
 
@@ -2170,31 +2454,37 @@
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosScalingConfiguration.TagListProperty"]]]], jsii.get(self, "tagList"))
 
     @tag_list.setter
     def tag_list(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosScalingConfiguration.TagListProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingConfiguration, "tag_list").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tagList", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="userData")
     def user_data(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: userData: User data to pass to instance. [1, 16KB] characters.User data should not be base64 encoded. If you want to pass base64 encoded string to the property, use function Fn::Base64Decode to decode the base64 string first.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "userData"))
 
     @user_data.setter
     def user_data(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingConfiguration, "user_data").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "userData", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-ess.RosScalingConfiguration.DiskMappingsProperty",
         jsii_struct_bases=[],
         name_mapping={
             "auto_snapshot_policy_id": "autoSnapshotPolicyId",
@@ -2232,14 +2522,26 @@
             :param disk_name: 
             :param encrypted: 
             :param kms_key_id: 
             :param performance_level: 
             :param size: 
             :param snapshot_id: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosScalingConfiguration.DiskMappingsProperty.__init__)
+                check_type(argname="argument auto_snapshot_policy_id", value=auto_snapshot_policy_id, expected_type=type_hints["auto_snapshot_policy_id"])
+                check_type(argname="argument category", value=category, expected_type=type_hints["category"])
+                check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+                check_type(argname="argument device", value=device, expected_type=type_hints["device"])
+                check_type(argname="argument disk_name", value=disk_name, expected_type=type_hints["disk_name"])
+                check_type(argname="argument encrypted", value=encrypted, expected_type=type_hints["encrypted"])
+                check_type(argname="argument kms_key_id", value=kms_key_id, expected_type=type_hints["kms_key_id"])
+                check_type(argname="argument performance_level", value=performance_level, expected_type=type_hints["performance_level"])
+                check_type(argname="argument size", value=size, expected_type=type_hints["size"])
+                check_type(argname="argument snapshot_id", value=snapshot_id, expected_type=type_hints["snapshot_id"])
             self._values: typing.Dict[str, typing.Any] = {}
             if auto_snapshot_policy_id is not None:
                 self._values["auto_snapshot_policy_id"] = auto_snapshot_policy_id
             if category is not None:
                 self._values["category"] = category
             if description is not None:
                 self._values["description"] = description
@@ -2386,14 +2688,18 @@
             key: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param key: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosScalingConfiguration.TagListProperty.__init__)
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {
                 "key": key,
             }
             if value is not None:
                 self._values["value"] = value
 
         @builtins.property
@@ -2468,15 +2774,15 @@
 class RosScalingConfigurationProps:
     def __init__(
         self,
         *,
         scaling_group_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         credit_specification: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         deployment_set_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        disk_mappings: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosScalingConfiguration.DiskMappingsProperty]]]] = None,
+        disk_mappings: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosScalingConfiguration.DiskMappingsProperty, typing.Dict[str, typing.Any]]]]]] = None,
         hpc_cluster_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         image_family: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         image_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         instance_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         instance_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         instance_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         instance_types: typing.Optional[typing.Union[typing.Sequence[typing.Any], ros_cdk_core.IResolvable]] = None,
@@ -2495,15 +2801,15 @@
         spot_price_limit: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         spot_price_limit_for_instance_type: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]] = None,
         spot_strategy: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         system_disk_auto_snapshot_policy_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         system_disk_category: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         system_disk_performance_level: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         system_disk_size: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
-        tag_list: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosScalingConfiguration.TagListProperty]]]] = None,
+        tag_list: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosScalingConfiguration.TagListProperty, typing.Dict[str, typing.Any]]]]]] = None,
         user_data: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::ESS::ScalingConfiguration``.
 
         :param scaling_group_id: 
         :param credit_specification: 
         :param deployment_set_id: 
@@ -2533,14 +2839,48 @@
         :param system_disk_auto_snapshot_policy_id: 
         :param system_disk_category: 
         :param system_disk_performance_level: 
         :param system_disk_size: 
         :param tag_list: 
         :param user_data: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosScalingConfigurationProps.__init__)
+            check_type(argname="argument scaling_group_id", value=scaling_group_id, expected_type=type_hints["scaling_group_id"])
+            check_type(argname="argument credit_specification", value=credit_specification, expected_type=type_hints["credit_specification"])
+            check_type(argname="argument deployment_set_id", value=deployment_set_id, expected_type=type_hints["deployment_set_id"])
+            check_type(argname="argument disk_mappings", value=disk_mappings, expected_type=type_hints["disk_mappings"])
+            check_type(argname="argument hpc_cluster_id", value=hpc_cluster_id, expected_type=type_hints["hpc_cluster_id"])
+            check_type(argname="argument image_family", value=image_family, expected_type=type_hints["image_family"])
+            check_type(argname="argument image_id", value=image_id, expected_type=type_hints["image_id"])
+            check_type(argname="argument instance_id", value=instance_id, expected_type=type_hints["instance_id"])
+            check_type(argname="argument instance_name", value=instance_name, expected_type=type_hints["instance_name"])
+            check_type(argname="argument instance_type", value=instance_type, expected_type=type_hints["instance_type"])
+            check_type(argname="argument instance_types", value=instance_types, expected_type=type_hints["instance_types"])
+            check_type(argname="argument internet_charge_type", value=internet_charge_type, expected_type=type_hints["internet_charge_type"])
+            check_type(argname="argument internet_max_bandwidth_in", value=internet_max_bandwidth_in, expected_type=type_hints["internet_max_bandwidth_in"])
+            check_type(argname="argument internet_max_bandwidth_out", value=internet_max_bandwidth_out, expected_type=type_hints["internet_max_bandwidth_out"])
+            check_type(argname="argument io_optimized", value=io_optimized, expected_type=type_hints["io_optimized"])
+            check_type(argname="argument ipv6_address_count", value=ipv6_address_count, expected_type=type_hints["ipv6_address_count"])
+            check_type(argname="argument key_pair_name", value=key_pair_name, expected_type=type_hints["key_pair_name"])
+            check_type(argname="argument load_balancer_weight", value=load_balancer_weight, expected_type=type_hints["load_balancer_weight"])
+            check_type(argname="argument password_inherit", value=password_inherit, expected_type=type_hints["password_inherit"])
+            check_type(argname="argument ram_role_name", value=ram_role_name, expected_type=type_hints["ram_role_name"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument scaling_configuration_name", value=scaling_configuration_name, expected_type=type_hints["scaling_configuration_name"])
+            check_type(argname="argument security_group_id", value=security_group_id, expected_type=type_hints["security_group_id"])
+            check_type(argname="argument spot_price_limit", value=spot_price_limit, expected_type=type_hints["spot_price_limit"])
+            check_type(argname="argument spot_price_limit_for_instance_type", value=spot_price_limit_for_instance_type, expected_type=type_hints["spot_price_limit_for_instance_type"])
+            check_type(argname="argument spot_strategy", value=spot_strategy, expected_type=type_hints["spot_strategy"])
+            check_type(argname="argument system_disk_auto_snapshot_policy_id", value=system_disk_auto_snapshot_policy_id, expected_type=type_hints["system_disk_auto_snapshot_policy_id"])
+            check_type(argname="argument system_disk_category", value=system_disk_category, expected_type=type_hints["system_disk_category"])
+            check_type(argname="argument system_disk_performance_level", value=system_disk_performance_level, expected_type=type_hints["system_disk_performance_level"])
+            check_type(argname="argument system_disk_size", value=system_disk_size, expected_type=type_hints["system_disk_size"])
+            check_type(argname="argument tag_list", value=tag_list, expected_type=type_hints["tag_list"])
+            check_type(argname="argument user_data", value=user_data, expected_type=type_hints["user_data"])
         self._values: typing.Dict[str, typing.Any] = {
             "scaling_group_id": scaling_group_id,
         }
         if credit_specification is not None:
             self._values["credit_specification"] = credit_specification
         if deployment_set_id is not None:
             self._values["deployment_set_id"] = deployment_set_id
@@ -2982,103 +3322,121 @@
 ):
     '''A ROS template type:  ``ALIYUN::ESS::ScalingGroup``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosScalingGroupProps",
+        props: typing.Union["RosScalingGroupProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::ESS::ScalingGroup``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosScalingGroup.__init__)
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
+            type_hints = typing.get_type_hints(RosScalingGroup._render_properties)
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
     @jsii.member(jsii_name="attrScalingGroupId")
     def attr_scaling_group_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ScalingGroupId: Scaling group Id
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScalingGroupId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScalingGroupName")
     def attr_scaling_group_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ScalingGroupName: Scaling group name
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScalingGroupName"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosScalingGroup, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="maxSize")
     def max_size(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property: maxSize: Maximum number of ECS instances in the scaling group. Value range: [0, 1000].
         '''
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "maxSize"))
 
     @max_size.setter
     def max_size(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingGroup, "max_size").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "maxSize", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="minSize")
     def min_size(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property: minSize: Minimum number of ECS instances in the scaling group. Value range: [0, 1000].
         '''
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "minSize"))
 
     @min_size.setter
     def min_size(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingGroup, "min_size").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "minSize", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="compensateWithOnDemand")
     def compensate_with_on_demand(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3088,51 +3446,60 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "compensateWithOnDemand"))
 
     @compensate_with_on_demand.setter
     def compensate_with_on_demand(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingGroup, "compensate_with_on_demand").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "compensateWithOnDemand", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="containerGroupId")
     def container_group_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: containerGroupId: The ID of the elastic container instance.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "containerGroupId"))
 
     @container_group_id.setter
     def container_group_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingGroup, "container_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "containerGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbInstanceIds")
     def db_instance_ids(
         self,
     ) -> typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]]:
         '''
         :Property: dbInstanceIds: ID list of an RDS instance. A Json Array with format: [ "rm-id0", "rm-id1", ... "rm-idz" ], support up to 100 RDS instance.
         '''
         return typing.cast(typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]], jsii.get(self, "dbInstanceIds"))
 
     @db_instance_ids.setter
     def db_instance_ids(
         self,
         value: typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingGroup, "db_instance_ids").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbInstanceIds", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="defaultCooldown")
     def default_cooldown(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3142,34 +3509,40 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "defaultCooldown"))
 
     @default_cooldown.setter
     def default_cooldown(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingGroup, "default_cooldown").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "defaultCooldown", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="desiredCapacity")
     def desired_capacity(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: desiredCapacity: The expected number of ECS instances in a scaling group. The scaling group automatically keeps the number of ECS instances as expected. The number of ECS instances cannot be greater than the value of MaxSize and cannot be less than the value of MinSize.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "desiredCapacity"))
 
     @desired_capacity.setter
     def desired_capacity(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingGroup, "desired_capacity").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "desiredCapacity", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="groupDeletionProtection")
     def group_deletion_protection(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3179,17 +3552,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "groupDeletionProtection"))
 
     @group_deletion_protection.setter
     def group_deletion_protection(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingGroup, "group_deletion_protection").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "groupDeletionProtection", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="groupType")
     def group_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3201,68 +3577,80 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "groupType"))
 
     @group_type.setter
     def group_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingGroup, "group_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "groupType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="healthCheckType")
     def health_check_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: healthCheckType: The health check type. Allow values is "ECS" and "NONE", default to "ECS".
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "healthCheckType"))
 
     @health_check_type.setter
     def health_check_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingGroup, "health_check_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "healthCheckType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceId")
     def instance_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: instanceId: The ID of the ECS instance from which the scaling group obtains configuration information of the specified instance.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "instanceId"))
 
     @instance_id.setter
     def instance_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingGroup, "instance_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="launchTemplateId")
     def launch_template_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: launchTemplateId: The ID of the instance launch template from which the scaling group obtains launch configurations.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "launchTemplateId"))
 
     @launch_template_id.setter
     def launch_template_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingGroup, "launch_template_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "launchTemplateId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="launchTemplateVersion")
     def launch_template_version(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3274,34 +3662,40 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "launchTemplateVersion"))
 
     @launch_template_version.setter
     def launch_template_version(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingGroup, "launch_template_version").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "launchTemplateVersion", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="loadBalancerIds")
     def load_balancer_ids(
         self,
     ) -> typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]]:
         '''
         :Property: loadBalancerIds: ID list of a Server Load Balancer instance. A Json Array with format: [ "lb-id0", "lb-id1", ... "lb-idz" ], support up to 100 Load Balancer instance.
         '''
         return typing.cast(typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]], jsii.get(self, "loadBalancerIds"))
 
     @load_balancer_ids.setter
     def load_balancer_ids(
         self,
         value: typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingGroup, "load_balancer_ids").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "loadBalancerIds", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="multiAzPolicy")
     def multi_az_policy(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3314,85 +3708,100 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "multiAzPolicy"))
 
     @multi_az_policy.setter
     def multi_az_policy(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingGroup, "multi_az_policy").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "multiAzPolicy", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="notificationConfigurations")
     def notification_configurations(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosScalingGroup.NotificationConfigurationsProperty"]]]]:
         '''
         :Property: notificationConfigurations: When a scaling event occurs in a scaling group, ESS will send a notification to Cloud Monitor or MNS.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosScalingGroup.NotificationConfigurationsProperty"]]]], jsii.get(self, "notificationConfigurations"))
 
     @notification_configurations.setter
     def notification_configurations(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosScalingGroup.NotificationConfigurationsProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingGroup, "notification_configurations").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "notificationConfigurations", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="onDemandBaseCapacity")
     def on_demand_base_capacity(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: onDemandBaseCapacity: The minimum number of pay-as-you-go instances required in the scaling group. Valid values: 0 to 1000. If the number of pay-as-you-go instances is less than the value of this parameter, Auto Scaling preferentially creates pay-as-you-go instances.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "onDemandBaseCapacity"))
 
     @on_demand_base_capacity.setter
     def on_demand_base_capacity(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingGroup, "on_demand_base_capacity").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "onDemandBaseCapacity", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="onDemandPercentageAboveBaseCapacity")
     def on_demand_percentage_above_base_capacity(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: onDemandPercentageAboveBaseCapacity: The percentage of pay-as-you-go instances that can be created when instances are added to the scaling group. This parameter takes effect when the number of pay-as-you-go instances reaches the value for the OnDemandBaseCapacity parameter. Valid values: 0 to 100.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "onDemandPercentageAboveBaseCapacity"))
 
     @on_demand_percentage_above_base_capacity.setter
     def on_demand_percentage_above_base_capacity(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingGroup, "on_demand_percentage_above_base_capacity").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "onDemandPercentageAboveBaseCapacity", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="protectedInstances")
     def protected_instances(
         self,
     ) -> typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]]:
         '''
         :Property: protectedInstances: ECS instances of protected mode in the scaling group.
         '''
         return typing.cast(typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]], jsii.get(self, "protectedInstances"))
 
     @protected_instances.setter
     def protected_instances(
         self,
         value: typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingGroup, "protected_instances").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "protectedInstances", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="removalPolicys")
     def removal_policys(
         self,
     ) -> typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3406,17 +3815,20 @@
         return typing.cast(typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]], jsii.get(self, "removalPolicys"))
 
     @removal_policys.setter
     def removal_policys(
         self,
         value: typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingGroup, "removal_policys").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "removalPolicys", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="scalingGroupName")
     def scaling_group_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3426,17 +3838,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "scalingGroupName"))
 
     @scaling_group_name.setter
     def scaling_group_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingGroup, "scaling_group_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "scalingGroupName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="scalingPolicy")
     def scaling_policy(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3448,100 +3863,118 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "scalingPolicy"))
 
     @scaling_policy.setter
     def scaling_policy(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingGroup, "scaling_policy").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "scalingPolicy", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="spotInstancePools")
     def spot_instance_pools(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: spotInstancePools: The number of instance types that are available. The system creates preemptible instances of multiple instance types that are available at the lowest cost in the scaling group. Valid values: 1 to 10.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "spotInstancePools"))
 
     @spot_instance_pools.setter
     def spot_instance_pools(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingGroup, "spot_instance_pools").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "spotInstancePools", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="spotInstanceRemedy")
     def spot_instance_remedy(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: spotInstanceRemedy: Specifies whether to supplement preemptible instances. If this parameter is set to true, Auto Scaling attempts to create an instance to replace a preemptible instance when Auto Scaling receives a system message which indicates that the preemptible instance is to be reclaimed.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "spotInstanceRemedy"))
 
     @spot_instance_remedy.setter
     def spot_instance_remedy(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingGroup, "spot_instance_remedy").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "spotInstanceRemedy", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="standbyInstances")
     def standby_instances(
         self,
     ) -> typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]]:
         '''
         :Property: standbyInstances: ECS instances of standby mode in the scaling group.
         '''
         return typing.cast(typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]], jsii.get(self, "standbyInstances"))
 
     @standby_instances.setter
     def standby_instances(
         self,
         value: typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingGroup, "standby_instances").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "standbyInstances", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tags")
     def tags(self) -> typing.Optional[typing.List["RosScalingGroup.TagsProperty"]]:
         '''
         :Property: tags: Tags to attach to instance. Max support 20 tags to add during create instance. Each tag with two properties Key and Value, and Key is required.
         '''
         return typing.cast(typing.Optional[typing.List["RosScalingGroup.TagsProperty"]], jsii.get(self, "tags"))
 
     @tags.setter
     def tags(
         self,
         value: typing.Optional[typing.List["RosScalingGroup.TagsProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingGroup, "tags").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tags", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vSwitchId")
     def v_switch_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: vSwitchId: If you create a VPC scaling group, you must specify the ID of a VSwitch.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "vSwitchId"))
 
     @v_switch_id.setter
     def v_switch_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingGroup, "v_switch_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vSwitchId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vSwitchIds")
     def v_switch_ids(
         self,
     ) -> typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3553,14 +3986,17 @@
         return typing.cast(typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]], jsii.get(self, "vSwitchIds"))
 
     @v_switch_ids.setter
     def v_switch_ids(
         self,
         value: typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingGroup, "v_switch_ids").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vSwitchIds", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-ess.RosScalingGroup.NotificationConfigurationsProperty",
         jsii_struct_bases=[],
         name_mapping={
             "notification_arn": "notificationArn",
@@ -3574,14 +4010,18 @@
             notification_arn: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             notification_types: typing.Union[typing.Sequence[typing.Any], ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param notification_arn: 
             :param notification_types: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosScalingGroup.NotificationConfigurationsProperty.__init__)
+                check_type(argname="argument notification_arn", value=notification_arn, expected_type=type_hints["notification_arn"])
+                check_type(argname="argument notification_types", value=notification_types, expected_type=type_hints["notification_types"])
             self._values: typing.Dict[str, typing.Any] = {
                 "notification_arn": notification_arn,
                 "notification_types": notification_types,
             }
 
         @builtins.property
         def notification_arn(
@@ -3646,14 +4086,18 @@
             key: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param key: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosScalingGroup.TagsProperty.__init__)
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {
                 "key": key,
             }
             if value is not None:
                 self._values["value"] = value
 
         @builtins.property
@@ -3694,193 +4138,217 @@
 ):
     '''A ROS template type:  ``ALIYUN::ESS::ScalingGroupEnable``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosScalingGroupEnableProps",
+        props: typing.Union["RosScalingGroupEnableProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::ESS::ScalingGroupEnable``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosScalingGroupEnable.__init__)
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
+            type_hints = typing.get_type_hints(RosScalingGroupEnable._render_properties)
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
     @jsii.member(jsii_name="attrLifecycleState")
     def attr_lifecycle_state(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: LifecycleState: The scaling group status
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLifecycleState"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScalingGroupId")
     def attr_scaling_group_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ScalingGroupId: The scaling group id
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScalingGroupId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScalingInstanceDetails")
     def attr_scaling_instance_details(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ScalingInstanceDetails: Detail information of auto created scaling instances
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScalingInstanceDetails"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScalingInstances")
     def attr_scaling_instances(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ScalingInstances: The auto created scaling instances
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScalingInstances"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScalingRuleArisExecuteErrorInfo")
     def attr_scaling_rule_aris_execute_error_info(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ScalingRuleArisExecuteErrorInfo: The error info of the execution of scaling rule aris
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScalingRuleArisExecuteErrorInfo"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScalingRuleArisExecuteResultInstancesAdded")
     def attr_scaling_rule_aris_execute_result_instances_added(
         self,
     ) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ScalingRuleArisExecuteResultInstancesAdded: Instances added via the execution of scaling rule aris
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScalingRuleArisExecuteResultInstancesAdded"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScalingRuleArisExecuteResultInstancesRemoved")
     def attr_scaling_rule_aris_execute_result_instances_removed(
         self,
     ) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ScalingRuleArisExecuteResultInstancesRemoved: Instances removed via the execution of scaling rule aris
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScalingRuleArisExecuteResultInstancesRemoved"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScalingRuleArisExecuteResultNumberOfAddedInstances")
     def attr_scaling_rule_aris_execute_result_number_of_added_instances(
         self,
     ) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ScalingRuleArisExecuteResultNumberOfAddedInstances: The number of added vm via the execution of scaling rule aris
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScalingRuleArisExecuteResultNumberOfAddedInstances"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosScalingGroupEnable, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="scalingGroupId")
     def scaling_group_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: scalingGroupId: The id of operated scaling group.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "scalingGroupId"))
 
     @scaling_group_id.setter
     def scaling_group_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingGroupEnable, "scaling_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "scalingGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceIds")
     def instance_ids(
         self,
     ) -> typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]]:
         '''
         :Property: instanceIds: The id list of ECS instance which will be attached. Max support 1000 instances.
         '''
         return typing.cast(typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]], jsii.get(self, "instanceIds"))
 
     @instance_ids.setter
     def instance_ids(
         self,
         value: typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingGroupEnable, "instance_ids").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceIds", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="removeInstanceIds")
     def remove_instance_ids(
         self,
     ) -> typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]]:
         '''
         :Property: removeInstanceIds: The id list of ECS instance which will be removed. Max support 1000 instances.
         '''
         return typing.cast(typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]], jsii.get(self, "removeInstanceIds"))
 
     @remove_instance_ids.setter
     def remove_instance_ids(
         self,
         value: typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingGroupEnable, "remove_instance_ids").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "removeInstanceIds", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="scalingConfigurationId")
     def scaling_configuration_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: scalingConfigurationId: The id of scaling configuration which will be activate.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "scalingConfigurationId"))
 
     @scaling_configuration_id.setter
     def scaling_configuration_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingGroupEnable, "scaling_configuration_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "scalingConfigurationId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="scalingRuleAris")
     def scaling_rule_aris(
         self,
     ) -> typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3891,31 +4359,37 @@
         return typing.cast(typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]], jsii.get(self, "scalingRuleAris"))
 
     @scaling_rule_aris.setter
     def scaling_rule_aris(
         self,
         value: typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingGroupEnable, "scaling_rule_aris").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "scalingRuleAris", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="scalingRuleArisExecuteVersion")
     def scaling_rule_aris_execute_version(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: scalingRuleArisExecuteVersion: The change of the property leads to the execution of all the scaling rule aris in ScalingRuleAris.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "scalingRuleArisExecuteVersion"))
 
     @scaling_rule_aris_execute_version.setter
     def scaling_rule_aris_execute_version(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingGroupEnable, "scaling_rule_aris_execute_version").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "scalingRuleArisExecuteVersion", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-ess.RosScalingGroupEnableProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -3943,14 +4417,22 @@
         :param scaling_group_id: 
         :param instance_ids: 
         :param remove_instance_ids: 
         :param scaling_configuration_id: 
         :param scaling_rule_aris: 
         :param scaling_rule_aris_execute_version: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosScalingGroupEnableProps.__init__)
+            check_type(argname="argument scaling_group_id", value=scaling_group_id, expected_type=type_hints["scaling_group_id"])
+            check_type(argname="argument instance_ids", value=instance_ids, expected_type=type_hints["instance_ids"])
+            check_type(argname="argument remove_instance_ids", value=remove_instance_ids, expected_type=type_hints["remove_instance_ids"])
+            check_type(argname="argument scaling_configuration_id", value=scaling_configuration_id, expected_type=type_hints["scaling_configuration_id"])
+            check_type(argname="argument scaling_rule_aris", value=scaling_rule_aris, expected_type=type_hints["scaling_rule_aris"])
+            check_type(argname="argument scaling_rule_aris_execute_version", value=scaling_rule_aris_execute_version, expected_type=type_hints["scaling_rule_aris_execute_version"])
         self._values: typing.Dict[str, typing.Any] = {
             "scaling_group_id": scaling_group_id,
         }
         if instance_ids is not None:
             self._values["instance_ids"] = instance_ids
         if remove_instance_ids is not None:
             self._values["remove_instance_ids"] = remove_instance_ids
@@ -4085,25 +4567,25 @@
         group_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         health_check_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         instance_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         launch_template_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         launch_template_version: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         load_balancer_ids: typing.Optional[typing.Union[typing.Sequence[typing.Any], ros_cdk_core.IResolvable]] = None,
         multi_az_policy: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        notification_configurations: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosScalingGroup.NotificationConfigurationsProperty]]]] = None,
+        notification_configurations: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosScalingGroup.NotificationConfigurationsProperty, typing.Dict[str, typing.Any]]]]]] = None,
         on_demand_base_capacity: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         on_demand_percentage_above_base_capacity: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         protected_instances: typing.Optional[typing.Union[typing.Sequence[typing.Any], ros_cdk_core.IResolvable]] = None,
         removal_policys: typing.Optional[typing.Union[typing.Sequence[typing.Any], ros_cdk_core.IResolvable]] = None,
         scaling_group_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         scaling_policy: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         spot_instance_pools: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         spot_instance_remedy: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         standby_instances: typing.Optional[typing.Union[typing.Sequence[typing.Any], ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence[RosScalingGroup.TagsProperty]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union[RosScalingGroup.TagsProperty, typing.Dict[str, typing.Any]]]] = None,
         v_switch_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         v_switch_ids: typing.Optional[typing.Union[typing.Sequence[typing.Any], ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::ESS::ScalingGroup``.
 
         :param max_size: 
         :param min_size: 
@@ -4130,14 +4612,44 @@
         :param spot_instance_pools: 
         :param spot_instance_remedy: 
         :param standby_instances: 
         :param tags: 
         :param v_switch_id: 
         :param v_switch_ids: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosScalingGroupProps.__init__)
+            check_type(argname="argument max_size", value=max_size, expected_type=type_hints["max_size"])
+            check_type(argname="argument min_size", value=min_size, expected_type=type_hints["min_size"])
+            check_type(argname="argument compensate_with_on_demand", value=compensate_with_on_demand, expected_type=type_hints["compensate_with_on_demand"])
+            check_type(argname="argument container_group_id", value=container_group_id, expected_type=type_hints["container_group_id"])
+            check_type(argname="argument db_instance_ids", value=db_instance_ids, expected_type=type_hints["db_instance_ids"])
+            check_type(argname="argument default_cooldown", value=default_cooldown, expected_type=type_hints["default_cooldown"])
+            check_type(argname="argument desired_capacity", value=desired_capacity, expected_type=type_hints["desired_capacity"])
+            check_type(argname="argument group_deletion_protection", value=group_deletion_protection, expected_type=type_hints["group_deletion_protection"])
+            check_type(argname="argument group_type", value=group_type, expected_type=type_hints["group_type"])
+            check_type(argname="argument health_check_type", value=health_check_type, expected_type=type_hints["health_check_type"])
+            check_type(argname="argument instance_id", value=instance_id, expected_type=type_hints["instance_id"])
+            check_type(argname="argument launch_template_id", value=launch_template_id, expected_type=type_hints["launch_template_id"])
+            check_type(argname="argument launch_template_version", value=launch_template_version, expected_type=type_hints["launch_template_version"])
+            check_type(argname="argument load_balancer_ids", value=load_balancer_ids, expected_type=type_hints["load_balancer_ids"])
+            check_type(argname="argument multi_az_policy", value=multi_az_policy, expected_type=type_hints["multi_az_policy"])
+            check_type(argname="argument notification_configurations", value=notification_configurations, expected_type=type_hints["notification_configurations"])
+            check_type(argname="argument on_demand_base_capacity", value=on_demand_base_capacity, expected_type=type_hints["on_demand_base_capacity"])
+            check_type(argname="argument on_demand_percentage_above_base_capacity", value=on_demand_percentage_above_base_capacity, expected_type=type_hints["on_demand_percentage_above_base_capacity"])
+            check_type(argname="argument protected_instances", value=protected_instances, expected_type=type_hints["protected_instances"])
+            check_type(argname="argument removal_policys", value=removal_policys, expected_type=type_hints["removal_policys"])
+            check_type(argname="argument scaling_group_name", value=scaling_group_name, expected_type=type_hints["scaling_group_name"])
+            check_type(argname="argument scaling_policy", value=scaling_policy, expected_type=type_hints["scaling_policy"])
+            check_type(argname="argument spot_instance_pools", value=spot_instance_pools, expected_type=type_hints["spot_instance_pools"])
+            check_type(argname="argument spot_instance_remedy", value=spot_instance_remedy, expected_type=type_hints["spot_instance_remedy"])
+            check_type(argname="argument standby_instances", value=standby_instances, expected_type=type_hints["standby_instances"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
+            check_type(argname="argument v_switch_ids", value=v_switch_ids, expected_type=type_hints["v_switch_ids"])
         self._values: typing.Dict[str, typing.Any] = {
             "max_size": max_size,
             "min_size": min_size,
         }
         if compensate_with_on_demand is not None:
             self._values["compensate_with_on_demand"] = compensate_with_on_demand
         if container_group_id is not None:
@@ -4531,88 +5043,103 @@
 ):
     '''A ROS template type:  ``ALIYUN::ESS::ScalingRule``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosScalingRuleProps",
+        props: typing.Union["RosScalingRuleProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::ESS::ScalingRule``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosScalingRule.__init__)
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
+            type_hints = typing.get_type_hints(RosScalingRule._render_properties)
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
     @jsii.member(jsii_name="attrScalingRuleAri")
     def attr_scaling_rule_ari(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ScalingRuleAri: Unique identifier of a scaling rule.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScalingRuleAri"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScalingRuleId")
     def attr_scaling_rule_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ScalingRuleId: ID of a scaling rule, generated by the system and globally unique.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScalingRuleId"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosScalingRule, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="scalingGroupId")
     def scaling_group_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: scalingGroupId: ID of the scaling group of a scaling rule.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "scalingGroupId"))
 
     @scaling_group_id.setter
     def scaling_group_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingRule, "scaling_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "scalingGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="adjustmentType")
     def adjustment_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -4625,17 +5152,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "adjustmentType"))
 
     @adjustment_type.setter
     def adjustment_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingRule, "adjustment_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "adjustmentType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="adjustmentValue")
     def adjustment_value(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -4648,34 +5178,40 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "adjustmentValue"))
 
     @adjustment_value.setter
     def adjustment_value(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingRule, "adjustment_value").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "adjustmentValue", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="cooldown")
     def cooldown(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: cooldown: Cool-down time of a scaling rule. Value range: [0, 86,400], in seconds. The default value is empty.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "cooldown"))
 
     @cooldown.setter
     def cooldown(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingRule, "cooldown").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "cooldown", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="disableScaleIn")
     def disable_scale_in(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -4685,17 +5221,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "disableScaleIn"))
 
     @disable_scale_in.setter
     def disable_scale_in(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingRule, "disable_scale_in").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "disableScaleIn", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="estimatedInstanceWarmup")
     def estimated_instance_warmup(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -4706,17 +5245,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "estimatedInstanceWarmup"))
 
     @estimated_instance_warmup.setter
     def estimated_instance_warmup(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingRule, "estimated_instance_warmup").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "estimatedInstanceWarmup", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="initialMaxSize")
     def initial_max_size(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -4726,17 +5268,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "initialMaxSize"))
 
     @initial_max_size.setter
     def initial_max_size(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingRule, "initial_max_size").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "initialMaxSize", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="metricName")
     def metric_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -4757,34 +5302,40 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "metricName"))
 
     @metric_name.setter
     def metric_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingRule, "metric_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "metricName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="minAdjustmentMagnitude")
     def min_adjustment_magnitude(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: minAdjustmentMagnitude: The minimum number of ECS instances to be adjusted in a scaling rule. This parameter takes effect only when the scaling rule type is SimpleScalingRule or StepScalingRule and AdjustmentType is PercentChangeInCapacity.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "minAdjustmentMagnitude"))
 
     @min_adjustment_magnitude.setter
     def min_adjustment_magnitude(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingRule, "min_adjustment_magnitude").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "minAdjustmentMagnitude", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="predictiveScalingMode")
     def predictive_scaling_mode(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -4797,17 +5348,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "predictiveScalingMode"))
 
     @predictive_scaling_mode.setter
     def predictive_scaling_mode(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingRule, "predictive_scaling_mode").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "predictiveScalingMode", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="predictiveTaskBufferTime")
     def predictive_task_buffer_time(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -4817,17 +5371,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "predictiveTaskBufferTime"))
 
     @predictive_task_buffer_time.setter
     def predictive_task_buffer_time(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingRule, "predictive_task_buffer_time").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "predictiveTaskBufferTime", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="predictiveValueBehavior")
     def predictive_value_behavior(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -4841,17 +5398,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "predictiveValueBehavior"))
 
     @predictive_value_behavior.setter
     def predictive_value_behavior(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingRule, "predictive_value_behavior").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "predictiveValueBehavior", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="predictiveValueBuffer")
     def predictive_value_buffer(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -4861,34 +5421,40 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "predictiveValueBuffer"))
 
     @predictive_value_buffer.setter
     def predictive_value_buffer(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingRule, "predictive_value_buffer").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "predictiveValueBuffer", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="scalingRuleName")
     def scaling_rule_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: scalingRuleName: Name shown for the scaling group, which is a string containing 2 to 40 English or Chinese characters. It must begin with a number, a letter (case-insensitive) or a Chinese character and can contain numbers, "_", "-" or ".". The account name in the same scaling group is unique in the same region. If this parameter value is not specified, the default value is ScalingRuleId.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "scalingRuleName"))
 
     @scaling_rule_name.setter
     def scaling_rule_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingRule, "scaling_rule_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "scalingRuleName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="scalingRuleType")
     def scaling_rule_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -4903,48 +5469,57 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "scalingRuleType"))
 
     @scaling_rule_type.setter
     def scaling_rule_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingRule, "scaling_rule_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "scalingRuleType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="stepAdjustment")
     def step_adjustment(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosScalingRule.StepAdjustmentProperty"]]]]:
         '''
         :Property: stepAdjustment:
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosScalingRule.StepAdjustmentProperty"]]]], jsii.get(self, "stepAdjustment"))
 
     @step_adjustment.setter
     def step_adjustment(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosScalingRule.StepAdjustmentProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingRule, "step_adjustment").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "stepAdjustment", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="targetValue")
     def target_value(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: targetValue: The target value of a metric. This parameter is required and applicable only to target tracking scaling rules and predictive scaling rules. The value of TargetValue must be greater than 0 and can have a maximum of three decimal places.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "targetValue"))
 
     @target_value.setter
     def target_value(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScalingRule, "target_value").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "targetValue", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-ess.RosScalingRule.StepAdjustmentProperty",
         jsii_struct_bases=[],
         name_mapping={
             "metric_interval_lower_bound": "metricIntervalLowerBound",
@@ -4961,14 +5536,19 @@
             scaling_adjustment: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param metric_interval_lower_bound: 
             :param metric_interval_upper_bound: 
             :param scaling_adjustment: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosScalingRule.StepAdjustmentProperty.__init__)
+                check_type(argname="argument metric_interval_lower_bound", value=metric_interval_lower_bound, expected_type=type_hints["metric_interval_lower_bound"])
+                check_type(argname="argument metric_interval_upper_bound", value=metric_interval_upper_bound, expected_type=type_hints["metric_interval_upper_bound"])
+                check_type(argname="argument scaling_adjustment", value=scaling_adjustment, expected_type=type_hints["scaling_adjustment"])
             self._values: typing.Dict[str, typing.Any] = {}
             if metric_interval_lower_bound is not None:
                 self._values["metric_interval_lower_bound"] = metric_interval_lower_bound
             if metric_interval_upper_bound is not None:
                 self._values["metric_interval_upper_bound"] = metric_interval_upper_bound
             if scaling_adjustment is not None:
                 self._values["scaling_adjustment"] = scaling_adjustment
@@ -5059,15 +5639,15 @@
         min_adjustment_magnitude: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         predictive_scaling_mode: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         predictive_task_buffer_time: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         predictive_value_behavior: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         predictive_value_buffer: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         scaling_rule_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         scaling_rule_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        step_adjustment: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosScalingRule.StepAdjustmentProperty]]]] = None,
+        step_adjustment: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosScalingRule.StepAdjustmentProperty, typing.Dict[str, typing.Any]]]]]] = None,
         target_value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::ESS::ScalingRule``.
 
         :param scaling_group_id: 
         :param adjustment_type: 
         :param adjustment_value: 
@@ -5082,14 +5662,33 @@
         :param predictive_value_behavior: 
         :param predictive_value_buffer: 
         :param scaling_rule_name: 
         :param scaling_rule_type: 
         :param step_adjustment: 
         :param target_value: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosScalingRuleProps.__init__)
+            check_type(argname="argument scaling_group_id", value=scaling_group_id, expected_type=type_hints["scaling_group_id"])
+            check_type(argname="argument adjustment_type", value=adjustment_type, expected_type=type_hints["adjustment_type"])
+            check_type(argname="argument adjustment_value", value=adjustment_value, expected_type=type_hints["adjustment_value"])
+            check_type(argname="argument cooldown", value=cooldown, expected_type=type_hints["cooldown"])
+            check_type(argname="argument disable_scale_in", value=disable_scale_in, expected_type=type_hints["disable_scale_in"])
+            check_type(argname="argument estimated_instance_warmup", value=estimated_instance_warmup, expected_type=type_hints["estimated_instance_warmup"])
+            check_type(argname="argument initial_max_size", value=initial_max_size, expected_type=type_hints["initial_max_size"])
+            check_type(argname="argument metric_name", value=metric_name, expected_type=type_hints["metric_name"])
+            check_type(argname="argument min_adjustment_magnitude", value=min_adjustment_magnitude, expected_type=type_hints["min_adjustment_magnitude"])
+            check_type(argname="argument predictive_scaling_mode", value=predictive_scaling_mode, expected_type=type_hints["predictive_scaling_mode"])
+            check_type(argname="argument predictive_task_buffer_time", value=predictive_task_buffer_time, expected_type=type_hints["predictive_task_buffer_time"])
+            check_type(argname="argument predictive_value_behavior", value=predictive_value_behavior, expected_type=type_hints["predictive_value_behavior"])
+            check_type(argname="argument predictive_value_buffer", value=predictive_value_buffer, expected_type=type_hints["predictive_value_buffer"])
+            check_type(argname="argument scaling_rule_name", value=scaling_rule_name, expected_type=type_hints["scaling_rule_name"])
+            check_type(argname="argument scaling_rule_type", value=scaling_rule_type, expected_type=type_hints["scaling_rule_type"])
+            check_type(argname="argument step_adjustment", value=step_adjustment, expected_type=type_hints["step_adjustment"])
+            check_type(argname="argument target_value", value=target_value, expected_type=type_hints["target_value"])
         self._values: typing.Dict[str, typing.Any] = {
             "scaling_group_id": scaling_group_id,
         }
         if adjustment_type is not None:
             self._values["adjustment_type"] = adjustment_type
         if adjustment_value is not None:
             self._values["adjustment_value"] = adjustment_value
@@ -5373,65 +5972,77 @@
 ):
     '''A ROS template type:  ``ALIYUN::ESS::ScheduledTask``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosScheduledTaskProps",
+        props: typing.Union["RosScheduledTaskProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::ESS::ScheduledTask``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosScheduledTask.__init__)
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
+            type_hints = typing.get_type_hints(RosScheduledTask._render_properties)
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
     @jsii.member(jsii_name="attrScheduledTaskId")
     def attr_scheduled_task_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ScheduledTaskId: ID of the scheduled task, which is generated by the system and globally unique.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScheduledTaskId"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosScheduledTask, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="launchTime")
     def launch_time(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         launchTime: Time point at which the scheduled task is triggered.
         The date format follows the ISO8601 standard and uses UTC time. It is in the format of YYYY-MM-DDThh:mmZ.
@@ -5441,49 +6052,58 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "launchTime"))
 
     @launch_time.setter
     def launch_time(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScheduledTask, "launch_time").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "launchTime", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="scheduledAction")
     def scheduled_action(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: scheduledAction: Operations performed when the scheduled task is triggered. Fill in the unique identifier of the scaling rule.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "scheduledAction"))
 
     @scheduled_action.setter
     def scheduled_action(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScheduledTask, "scheduled_action").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "scheduledAction", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: description: Description of the scheduled task, which is 2-200 characters (English or Chinese) long.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScheduledTask, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="launchExpirationTime")
     def launch_expiration_time(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5494,17 +6114,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "launchExpirationTime"))
 
     @launch_expiration_time.setter
     def launch_expiration_time(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScheduledTask, "launch_expiration_time").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "launchExpirationTime", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="recurrenceEndTime")
     def recurrence_end_time(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5516,17 +6139,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "recurrenceEndTime"))
 
     @recurrence_end_time.setter
     def recurrence_end_time(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScheduledTask, "recurrence_end_time").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "recurrenceEndTime", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="recurrenceType")
     def recurrence_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5540,17 +6166,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "recurrenceType"))
 
     @recurrence_type.setter
     def recurrence_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScheduledTask, "recurrence_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "recurrenceType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="recurrenceValue")
     def recurrence_value(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5564,17 +6193,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "recurrenceValue"))
 
     @recurrence_value.setter
     def recurrence_value(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScheduledTask, "recurrence_value").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "recurrenceValue", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="scheduledTaskName")
     def scheduled_task_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5585,17 +6217,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "scheduledTaskName"))
 
     @scheduled_task_name.setter
     def scheduled_task_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScheduledTask, "scheduled_task_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "scheduledTaskName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="taskEnabled")
     def task_enabled(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5608,14 +6243,17 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "taskEnabled"))
 
     @task_enabled.setter
     def task_enabled(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosScheduledTask, "task_enabled").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "taskEnabled", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-ess.RosScheduledTaskProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -5652,14 +6290,25 @@
         :param launch_expiration_time: 
         :param recurrence_end_time: 
         :param recurrence_type: 
         :param recurrence_value: 
         :param scheduled_task_name: 
         :param task_enabled: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosScheduledTaskProps.__init__)
+            check_type(argname="argument launch_time", value=launch_time, expected_type=type_hints["launch_time"])
+            check_type(argname="argument scheduled_action", value=scheduled_action, expected_type=type_hints["scheduled_action"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument launch_expiration_time", value=launch_expiration_time, expected_type=type_hints["launch_expiration_time"])
+            check_type(argname="argument recurrence_end_time", value=recurrence_end_time, expected_type=type_hints["recurrence_end_time"])
+            check_type(argname="argument recurrence_type", value=recurrence_type, expected_type=type_hints["recurrence_type"])
+            check_type(argname="argument recurrence_value", value=recurrence_value, expected_type=type_hints["recurrence_value"])
+            check_type(argname="argument scheduled_task_name", value=scheduled_task_name, expected_type=type_hints["scheduled_task_name"])
+            check_type(argname="argument task_enabled", value=task_enabled, expected_type=type_hints["task_enabled"])
         self._values: typing.Dict[str, typing.Any] = {
             "launch_time": launch_time,
             "scheduled_action": scheduled_action,
         }
         if description is not None:
             self._values["description"] = description
         if launch_expiration_time is not None:
@@ -5820,31 +6469,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::ESS::ScalingConfiguration``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "ScalingConfigurationProps",
+        props: typing.Union["ScalingConfigurationProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::ESS::ScalingConfiguration``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ScalingConfiguration.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScalingConfigurationId")
     def attr_scaling_configuration_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ScalingConfigurationId: The scaling configuration id.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScalingConfigurationId"))
 
 
 @jsii.data_type(
@@ -5888,15 +6543,15 @@
 class ScalingConfigurationProps:
     def __init__(
         self,
         *,
         scaling_group_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         credit_specification: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         deployment_set_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        disk_mappings: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosScalingConfiguration.DiskMappingsProperty]]]] = None,
+        disk_mappings: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosScalingConfiguration.DiskMappingsProperty, typing.Dict[str, typing.Any]]]]]] = None,
         hpc_cluster_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         image_family: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         image_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         instance_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         instance_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         instance_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         instance_types: typing.Optional[typing.Union[typing.Sequence[typing.Any], ros_cdk_core.IResolvable]] = None,
@@ -5915,15 +6570,15 @@
         spot_price_limit: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         spot_price_limit_for_instance_type: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]] = None,
         spot_strategy: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         system_disk_auto_snapshot_policy_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         system_disk_category: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         system_disk_performance_level: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         system_disk_size: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
-        tag_list: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosScalingConfiguration.TagListProperty]]]] = None,
+        tag_list: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosScalingConfiguration.TagListProperty, typing.Dict[str, typing.Any]]]]]] = None,
         user_data: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::ESS::ScalingConfiguration``.
 
         :param scaling_group_id: Property scalingGroupId: Scaling group id to create the scaling configuration.
         :param credit_specification: Property creditSpecification: The performance mode of the burstable instance. Valid values: Standard: the standard mode. Unlimited: the unlimited mode.
         :param deployment_set_id: Property deploymentSetId: Deployment set ID.
@@ -5953,14 +6608,48 @@
         :param system_disk_auto_snapshot_policy_id: Property systemDiskAutoSnapshotPolicyId: Auto snapshot policy ID.
         :param system_disk_category: Property systemDiskCategory: Category of system disk. Default is cloud.support cloud|cloud_efficiency|cloud_ssd|cloud_essd|ephemeral_ssd
         :param system_disk_performance_level: Property systemDiskPerformanceLevel: The performance level of an ESSD.
         :param system_disk_size: Property systemDiskSize: Size of system disk. Unit is GB.
         :param tag_list: Property tagList: The tags of an instance in list format. Do not use with Tags at the same time. You should input the information of the tag with the format of Key-Value list, such as [{"Key":"key1","Value":"value1"}, ...]. At most 20 tags can be specified. Key It can be up to 64 characters in length. Cannot begin with aliyun. Cannot begin with http:// or https://. Cannot be a null string. Value It can be up to 128 characters in length. Cannot begin with aliyun. Cannot begin with http:// or https://. Can be a null string.If less then 20 tags are specified, ros will add a tag(Key: "ros-aliyun-created", Value:"<resource_name>*stack*<stack_id>") if possible.
         :param user_data: Property userData: User data to pass to instance. [1, 16KB] characters.User data should not be base64 encoded. If you want to pass base64 encoded string to the property, use function Fn::Base64Decode to decode the base64 string first.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ScalingConfigurationProps.__init__)
+            check_type(argname="argument scaling_group_id", value=scaling_group_id, expected_type=type_hints["scaling_group_id"])
+            check_type(argname="argument credit_specification", value=credit_specification, expected_type=type_hints["credit_specification"])
+            check_type(argname="argument deployment_set_id", value=deployment_set_id, expected_type=type_hints["deployment_set_id"])
+            check_type(argname="argument disk_mappings", value=disk_mappings, expected_type=type_hints["disk_mappings"])
+            check_type(argname="argument hpc_cluster_id", value=hpc_cluster_id, expected_type=type_hints["hpc_cluster_id"])
+            check_type(argname="argument image_family", value=image_family, expected_type=type_hints["image_family"])
+            check_type(argname="argument image_id", value=image_id, expected_type=type_hints["image_id"])
+            check_type(argname="argument instance_id", value=instance_id, expected_type=type_hints["instance_id"])
+            check_type(argname="argument instance_name", value=instance_name, expected_type=type_hints["instance_name"])
+            check_type(argname="argument instance_type", value=instance_type, expected_type=type_hints["instance_type"])
+            check_type(argname="argument instance_types", value=instance_types, expected_type=type_hints["instance_types"])
+            check_type(argname="argument internet_charge_type", value=internet_charge_type, expected_type=type_hints["internet_charge_type"])
+            check_type(argname="argument internet_max_bandwidth_in", value=internet_max_bandwidth_in, expected_type=type_hints["internet_max_bandwidth_in"])
+            check_type(argname="argument internet_max_bandwidth_out", value=internet_max_bandwidth_out, expected_type=type_hints["internet_max_bandwidth_out"])
+            check_type(argname="argument io_optimized", value=io_optimized, expected_type=type_hints["io_optimized"])
+            check_type(argname="argument ipv6_address_count", value=ipv6_address_count, expected_type=type_hints["ipv6_address_count"])
+            check_type(argname="argument key_pair_name", value=key_pair_name, expected_type=type_hints["key_pair_name"])
+            check_type(argname="argument load_balancer_weight", value=load_balancer_weight, expected_type=type_hints["load_balancer_weight"])
+            check_type(argname="argument password_inherit", value=password_inherit, expected_type=type_hints["password_inherit"])
+            check_type(argname="argument ram_role_name", value=ram_role_name, expected_type=type_hints["ram_role_name"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument scaling_configuration_name", value=scaling_configuration_name, expected_type=type_hints["scaling_configuration_name"])
+            check_type(argname="argument security_group_id", value=security_group_id, expected_type=type_hints["security_group_id"])
+            check_type(argname="argument spot_price_limit", value=spot_price_limit, expected_type=type_hints["spot_price_limit"])
+            check_type(argname="argument spot_price_limit_for_instance_type", value=spot_price_limit_for_instance_type, expected_type=type_hints["spot_price_limit_for_instance_type"])
+            check_type(argname="argument spot_strategy", value=spot_strategy, expected_type=type_hints["spot_strategy"])
+            check_type(argname="argument system_disk_auto_snapshot_policy_id", value=system_disk_auto_snapshot_policy_id, expected_type=type_hints["system_disk_auto_snapshot_policy_id"])
+            check_type(argname="argument system_disk_category", value=system_disk_category, expected_type=type_hints["system_disk_category"])
+            check_type(argname="argument system_disk_performance_level", value=system_disk_performance_level, expected_type=type_hints["system_disk_performance_level"])
+            check_type(argname="argument system_disk_size", value=system_disk_size, expected_type=type_hints["system_disk_size"])
+            check_type(argname="argument tag_list", value=tag_list, expected_type=type_hints["tag_list"])
+            check_type(argname="argument user_data", value=user_data, expected_type=type_hints["user_data"])
         self._values: typing.Dict[str, typing.Any] = {
             "scaling_group_id": scaling_group_id,
         }
         if credit_specification is not None:
             self._values["credit_specification"] = credit_specification
         if deployment_set_id is not None:
             self._values["deployment_set_id"] = deployment_set_id
@@ -6371,37 +7060,43 @@
 ):
     '''A ROS resource type:  ``ALIYUN::ESS::ScalingGroup``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "ScalingGroupProps",
+        props: typing.Union["ScalingGroupProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::ESS::ScalingGroup``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ScalingGroup.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScalingGroupId")
     def attr_scaling_group_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ScalingGroupId: Scaling group Id.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScalingGroupId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScalingGroupName")
     def attr_scaling_group_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute ScalingGroupName: Scaling group name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScalingGroupName"))
 
 
 class ScalingGroupEnable(
@@ -6411,77 +7106,83 @@
 ):
     '''A ROS resource type:  ``ALIYUN::ESS::ScalingGroupEnable``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "ScalingGroupEnableProps",
+        props: typing.Union["ScalingGroupEnableProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::ESS::ScalingGroupEnable``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ScalingGroupEnable.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrLifecycleState")
     def attr_lifecycle_state(self) -> ros_cdk_core.IResolvable:
         '''Attribute LifecycleState: The scaling group status.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLifecycleState"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScalingGroupId")
     def attr_scaling_group_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ScalingGroupId: The scaling group id.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScalingGroupId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScalingInstanceDetails")
     def attr_scaling_instance_details(self) -> ros_cdk_core.IResolvable:
         '''Attribute ScalingInstanceDetails: Detail information of auto created scaling instances.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScalingInstanceDetails"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScalingInstances")
     def attr_scaling_instances(self) -> ros_cdk_core.IResolvable:
         '''Attribute ScalingInstances: The auto created scaling instances.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScalingInstances"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScalingRuleArisExecuteErrorInfo")
     def attr_scaling_rule_aris_execute_error_info(self) -> ros_cdk_core.IResolvable:
         '''Attribute ScalingRuleArisExecuteErrorInfo: The error info of the execution of scaling rule aris.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScalingRuleArisExecuteErrorInfo"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScalingRuleArisExecuteResultInstancesAdded")
     def attr_scaling_rule_aris_execute_result_instances_added(
         self,
     ) -> ros_cdk_core.IResolvable:
         '''Attribute ScalingRuleArisExecuteResultInstancesAdded: Instances added via the execution of scaling rule aris.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScalingRuleArisExecuteResultInstancesAdded"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScalingRuleArisExecuteResultInstancesRemoved")
     def attr_scaling_rule_aris_execute_result_instances_removed(
         self,
     ) -> ros_cdk_core.IResolvable:
         '''Attribute ScalingRuleArisExecuteResultInstancesRemoved: Instances removed via the execution of scaling rule aris.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScalingRuleArisExecuteResultInstancesRemoved"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScalingRuleArisExecuteResultNumberOfAddedInstances")
     def attr_scaling_rule_aris_execute_result_number_of_added_instances(
         self,
     ) -> ros_cdk_core.IResolvable:
         '''Attribute ScalingRuleArisExecuteResultNumberOfAddedInstances: The number of added vm via the execution of scaling rule aris.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScalingRuleArisExecuteResultNumberOfAddedInstances"))
 
@@ -6514,14 +7215,22 @@
         :param scaling_group_id: Property scalingGroupId: The id of operated scaling group.
         :param instance_ids: Property instanceIds: The id list of ECS instance which will be attached. Max support 1000 instances.
         :param remove_instance_ids: Property removeInstanceIds: The id list of ECS instance which will be removed. Max support 1000 instances.
         :param scaling_configuration_id: Property scalingConfigurationId: The id of scaling configuration which will be activate.
         :param scaling_rule_aris: Property scalingRuleAris: A list of scaling rule aris which will be executed. Max support 10 scaling rule aris. When creating the resource, all the scaling rule aris in the list will be executed. When updating the resource, none of scaling rule aris in the list will be executed, unless ScalingRuleArisExecuteVersion is changed.
         :param scaling_rule_aris_execute_version: Property scalingRuleArisExecuteVersion: The change of the property leads to the execution of all the scaling rule aris in ScalingRuleAris.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ScalingGroupEnableProps.__init__)
+            check_type(argname="argument scaling_group_id", value=scaling_group_id, expected_type=type_hints["scaling_group_id"])
+            check_type(argname="argument instance_ids", value=instance_ids, expected_type=type_hints["instance_ids"])
+            check_type(argname="argument remove_instance_ids", value=remove_instance_ids, expected_type=type_hints["remove_instance_ids"])
+            check_type(argname="argument scaling_configuration_id", value=scaling_configuration_id, expected_type=type_hints["scaling_configuration_id"])
+            check_type(argname="argument scaling_rule_aris", value=scaling_rule_aris, expected_type=type_hints["scaling_rule_aris"])
+            check_type(argname="argument scaling_rule_aris_execute_version", value=scaling_rule_aris_execute_version, expected_type=type_hints["scaling_rule_aris_execute_version"])
         self._values: typing.Dict[str, typing.Any] = {
             "scaling_group_id": scaling_group_id,
         }
         if instance_ids is not None:
             self._values["instance_ids"] = instance_ids
         if remove_instance_ids is not None:
             self._values["remove_instance_ids"] = remove_instance_ids
@@ -6651,25 +7360,25 @@
         group_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         health_check_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         instance_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         launch_template_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         launch_template_version: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         load_balancer_ids: typing.Optional[typing.Union[typing.Sequence[typing.Any], ros_cdk_core.IResolvable]] = None,
         multi_az_policy: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        notification_configurations: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosScalingGroup.NotificationConfigurationsProperty]]]] = None,
+        notification_configurations: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosScalingGroup.NotificationConfigurationsProperty, typing.Dict[str, typing.Any]]]]]] = None,
         on_demand_base_capacity: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         on_demand_percentage_above_base_capacity: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         protected_instances: typing.Optional[typing.Union[typing.Sequence[typing.Any], ros_cdk_core.IResolvable]] = None,
         removal_policys: typing.Optional[typing.Union[typing.Sequence[typing.Any], ros_cdk_core.IResolvable]] = None,
         scaling_group_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         scaling_policy: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         spot_instance_pools: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         spot_instance_remedy: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         standby_instances: typing.Optional[typing.Union[typing.Sequence[typing.Any], ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence[RosScalingGroup.TagsProperty]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union[RosScalingGroup.TagsProperty, typing.Dict[str, typing.Any]]]] = None,
         v_switch_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         v_switch_ids: typing.Optional[typing.Union[typing.Sequence[typing.Any], ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::ESS::ScalingGroup``.
 
         :param max_size: Property maxSize: Maximum number of ECS instances in the scaling group. Value range: [0, 1000].
         :param min_size: Property minSize: Minimum number of ECS instances in the scaling group. Value range: [0, 1000].
@@ -6696,14 +7405,44 @@
         :param spot_instance_pools: Property spotInstancePools: The number of instance types that are available. The system creates preemptible instances of multiple instance types that are available at the lowest cost in the scaling group. Valid values: 1 to 10.
         :param spot_instance_remedy: Property spotInstanceRemedy: Specifies whether to supplement preemptible instances. If this parameter is set to true, Auto Scaling attempts to create an instance to replace a preemptible instance when Auto Scaling receives a system message which indicates that the preemptible instance is to be reclaimed.
         :param standby_instances: Property standbyInstances: ECS instances of standby mode in the scaling group.
         :param tags: Property tags: Tags to attach to instance. Max support 20 tags to add during create instance. Each tag with two properties Key and Value, and Key is required.
         :param v_switch_id: Property vSwitchId: If you create a VPC scaling group, you must specify the ID of a VSwitch.
         :param v_switch_ids: Property vSwitchIds: Parameter VSwitchIds.N is used to create instance in multiple zones. Parameter VSwitchIds.N has a priority over parameter VSwitchId. The valid range of N is [1, 8], and you can specify at most 5 VSwitches in a VPC. The priority of VSwitches descends from 1 to 8, and 1 indicates the highest priority. When you fail to create an instance in the zone to which a specified VSwitch belongs, another VSwitch with less priority replaces the specified one automatically.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ScalingGroupProps.__init__)
+            check_type(argname="argument max_size", value=max_size, expected_type=type_hints["max_size"])
+            check_type(argname="argument min_size", value=min_size, expected_type=type_hints["min_size"])
+            check_type(argname="argument compensate_with_on_demand", value=compensate_with_on_demand, expected_type=type_hints["compensate_with_on_demand"])
+            check_type(argname="argument container_group_id", value=container_group_id, expected_type=type_hints["container_group_id"])
+            check_type(argname="argument db_instance_ids", value=db_instance_ids, expected_type=type_hints["db_instance_ids"])
+            check_type(argname="argument default_cooldown", value=default_cooldown, expected_type=type_hints["default_cooldown"])
+            check_type(argname="argument desired_capacity", value=desired_capacity, expected_type=type_hints["desired_capacity"])
+            check_type(argname="argument group_deletion_protection", value=group_deletion_protection, expected_type=type_hints["group_deletion_protection"])
+            check_type(argname="argument group_type", value=group_type, expected_type=type_hints["group_type"])
+            check_type(argname="argument health_check_type", value=health_check_type, expected_type=type_hints["health_check_type"])
+            check_type(argname="argument instance_id", value=instance_id, expected_type=type_hints["instance_id"])
+            check_type(argname="argument launch_template_id", value=launch_template_id, expected_type=type_hints["launch_template_id"])
+            check_type(argname="argument launch_template_version", value=launch_template_version, expected_type=type_hints["launch_template_version"])
+            check_type(argname="argument load_balancer_ids", value=load_balancer_ids, expected_type=type_hints["load_balancer_ids"])
+            check_type(argname="argument multi_az_policy", value=multi_az_policy, expected_type=type_hints["multi_az_policy"])
+            check_type(argname="argument notification_configurations", value=notification_configurations, expected_type=type_hints["notification_configurations"])
+            check_type(argname="argument on_demand_base_capacity", value=on_demand_base_capacity, expected_type=type_hints["on_demand_base_capacity"])
+            check_type(argname="argument on_demand_percentage_above_base_capacity", value=on_demand_percentage_above_base_capacity, expected_type=type_hints["on_demand_percentage_above_base_capacity"])
+            check_type(argname="argument protected_instances", value=protected_instances, expected_type=type_hints["protected_instances"])
+            check_type(argname="argument removal_policys", value=removal_policys, expected_type=type_hints["removal_policys"])
+            check_type(argname="argument scaling_group_name", value=scaling_group_name, expected_type=type_hints["scaling_group_name"])
+            check_type(argname="argument scaling_policy", value=scaling_policy, expected_type=type_hints["scaling_policy"])
+            check_type(argname="argument spot_instance_pools", value=spot_instance_pools, expected_type=type_hints["spot_instance_pools"])
+            check_type(argname="argument spot_instance_remedy", value=spot_instance_remedy, expected_type=type_hints["spot_instance_remedy"])
+            check_type(argname="argument standby_instances", value=standby_instances, expected_type=type_hints["standby_instances"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
+            check_type(argname="argument v_switch_ids", value=v_switch_ids, expected_type=type_hints["v_switch_ids"])
         self._values: typing.Dict[str, typing.Any] = {
             "max_size": max_size,
             "min_size": min_size,
         }
         if compensate_with_on_demand is not None:
             self._values["compensate_with_on_demand"] = compensate_with_on_demand
         if container_group_id is not None:
@@ -7076,37 +7815,43 @@
 ):
     '''A ROS resource type:  ``ALIYUN::ESS::ScalingRule``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "ScalingRuleProps",
+        props: typing.Union["ScalingRuleProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::ESS::ScalingRule``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ScalingRule.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScalingRuleAri")
     def attr_scaling_rule_ari(self) -> ros_cdk_core.IResolvable:
         '''Attribute ScalingRuleAri: Unique identifier of a scaling rule.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScalingRuleAri"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScalingRuleId")
     def attr_scaling_rule_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ScalingRuleId: ID of a scaling rule, generated by the system and globally unique.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScalingRuleId"))
 
 
 @jsii.data_type(
@@ -7147,15 +7892,15 @@
         min_adjustment_magnitude: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         predictive_scaling_mode: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         predictive_task_buffer_time: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         predictive_value_behavior: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         predictive_value_buffer: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         scaling_rule_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         scaling_rule_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        step_adjustment: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosScalingRule.StepAdjustmentProperty]]]] = None,
+        step_adjustment: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosScalingRule.StepAdjustmentProperty, typing.Dict[str, typing.Any]]]]]] = None,
         target_value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::ESS::ScalingRule``.
 
         :param scaling_group_id: Property scalingGroupId: ID of the scaling group of a scaling rule.
         :param adjustment_type: Property adjustmentType: Adjustment mode of a scaling rule. Optional values: - QuantityChangeInCapacity: It is used to increase or decrease a specified number of ECS instances. - PercentChangeInCapacity: It is used to increase or decrease a specified proportion of ECS instances. - TotalCapacity: It is used to adjust the quantity of ECS instances in the current scaling group to a specified value.
         :param adjustment_value: Property adjustmentValue: Adjusted value of a scaling rule. Value range: - QuantityChangeInCapacity: [-500, 500] - PercentChangeInCapacity: [-100, 10000] - TotalCapacity: [0, 1000]
@@ -7170,14 +7915,33 @@
         :param predictive_value_behavior: Property predictiveValueBehavior: The action taken on the predicted maximum value. Valid values: - MaxOverridePredictiveValue: uses the initial maximum capacity as the maximum value for forecast tasks when the predicted value is greater than the initial maximum capacity. - PredictiveValueOverrideMax: uses the predicted value as the maximum value for forecast tasks when the predicted value is greater than the initial maximum capacity. - PredictiveValueOverrideMaxWithBuffer: increases the predicted value with a ratio, which is specified by PredictiveValueBuffer. If the value after the increase is greater than the initial maximum capacity, the value after the increase is used as the maximum value for forecast tasks. Default value: MaxOverridePredictiveValue
         :param predictive_value_buffer: Property predictiveValueBuffer: The ratio of the increment to the predicted value when PredictiveValueBehavior is set to PredictiveValueOverrideMaxWithBuffer. When the value after the increase is greater than the initial maximum capacity, the value after the increase is used for forecast tasks. Valid values: 0 to 100 Default value: 0
         :param scaling_rule_name: Property scalingRuleName: Name shown for the scaling group, which is a string containing 2 to 40 English or Chinese characters. It must begin with a number, a letter (case-insensitive) or a Chinese character and can contain numbers, "_", "-" or ".". The account name in the same scaling group is unique in the same region. If this parameter value is not specified, the default value is ScalingRuleId.
         :param scaling_rule_type: Property scalingRuleType: The type of the scaling rule. Valid values: - SimpleScalingRule: scales ECS instances based on the values of AdjustmentType and AdjustmentValue. - TargetTrackingScalingRule: dynamically calculates the number of ECS instances to be adjusted and tries to keep the value of a predefined monitoring metric close to TargetValue. - StepScalingRule: scales ECS instances in steps based on specified thresholds and metric values. - PredictiveScalingRule: uses machine learning to analyze historical monitoring data of the scaling group and then predicts the future values of monitored metrics, the rule then automatically creates scheduled tasks to set the boundary values for the scaling group. If this parameter value is not specified, the default value is SimpleScalingRule.
         :param step_adjustment: Property stepAdjustment:.
         :param target_value: Property targetValue: The target value of a metric. This parameter is required and applicable only to target tracking scaling rules and predictive scaling rules. The value of TargetValue must be greater than 0 and can have a maximum of three decimal places.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ScalingRuleProps.__init__)
+            check_type(argname="argument scaling_group_id", value=scaling_group_id, expected_type=type_hints["scaling_group_id"])
+            check_type(argname="argument adjustment_type", value=adjustment_type, expected_type=type_hints["adjustment_type"])
+            check_type(argname="argument adjustment_value", value=adjustment_value, expected_type=type_hints["adjustment_value"])
+            check_type(argname="argument cooldown", value=cooldown, expected_type=type_hints["cooldown"])
+            check_type(argname="argument disable_scale_in", value=disable_scale_in, expected_type=type_hints["disable_scale_in"])
+            check_type(argname="argument estimated_instance_warmup", value=estimated_instance_warmup, expected_type=type_hints["estimated_instance_warmup"])
+            check_type(argname="argument initial_max_size", value=initial_max_size, expected_type=type_hints["initial_max_size"])
+            check_type(argname="argument metric_name", value=metric_name, expected_type=type_hints["metric_name"])
+            check_type(argname="argument min_adjustment_magnitude", value=min_adjustment_magnitude, expected_type=type_hints["min_adjustment_magnitude"])
+            check_type(argname="argument predictive_scaling_mode", value=predictive_scaling_mode, expected_type=type_hints["predictive_scaling_mode"])
+            check_type(argname="argument predictive_task_buffer_time", value=predictive_task_buffer_time, expected_type=type_hints["predictive_task_buffer_time"])
+            check_type(argname="argument predictive_value_behavior", value=predictive_value_behavior, expected_type=type_hints["predictive_value_behavior"])
+            check_type(argname="argument predictive_value_buffer", value=predictive_value_buffer, expected_type=type_hints["predictive_value_buffer"])
+            check_type(argname="argument scaling_rule_name", value=scaling_rule_name, expected_type=type_hints["scaling_rule_name"])
+            check_type(argname="argument scaling_rule_type", value=scaling_rule_type, expected_type=type_hints["scaling_rule_type"])
+            check_type(argname="argument step_adjustment", value=step_adjustment, expected_type=type_hints["step_adjustment"])
+            check_type(argname="argument target_value", value=target_value, expected_type=type_hints["target_value"])
         self._values: typing.Dict[str, typing.Any] = {
             "scaling_group_id": scaling_group_id,
         }
         if adjustment_type is not None:
             self._values["adjustment_type"] = adjustment_type
         if adjustment_value is not None:
             self._values["adjustment_value"] = adjustment_value
@@ -7450,31 +8214,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::ESS::ScheduledTask``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "ScheduledTaskProps",
+        props: typing.Union["ScheduledTaskProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::ESS::ScheduledTask``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ScheduledTask.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScheduledTaskId")
     def attr_scheduled_task_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ScheduledTaskId: ID of the scheduled task, which is generated by the system and globally unique.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScheduledTaskId"))
 
 
 @jsii.data_type(
@@ -7514,14 +8284,25 @@
         :param launch_expiration_time: Property launchExpirationTime: Time period within which the failed scheduled task is retried. The default value is 600s. Value range: [0, 21600]
         :param recurrence_end_time: Property recurrenceEndTime: End time of the scheduled task to be repeated. The date format follows the ISO8601 standard and uses UTC time. It is in the format of YYYY-MM-DDThh:mmZ. A time point 90 days after creation or modification cannot be entered. RecurrenceType, RecurrenceValue and RecurrenceEndTime must be specified.
         :param recurrence_type: Property recurrenceType: Type of the scheduled task to be repeated. Optional values: - Daily: Recurrence interval by day for a scheduled task. - Weekly: Recurrence interval by week for a scheduled task. - Monthly: Recurrence interval by month for a scheduled task. RecurrenceType, RecurrenceValue and RecurrenceEndTime must be specified.
         :param recurrence_value: Property recurrenceValue: Value of the scheduled task to be repeated. - Daily: Only one value in the range [1,31] can be filled. - Weekly: Multiple values can be filled. The values of Sunday to Saturday are 0 to 6 in sequence. Multiple values shall be separated by a comma ",". - Monthly: In the format of A-B. The value range of A and B is 1 to 31, and the B value must be greater than the A value. RecurrenceType, RecurrenceValue and RecurrenceEndTime must be specified.
         :param scheduled_task_name: Property scheduledTaskName: Display name of the scheduled task, which must be 2-40 characters (English or Chinese) long. It must begin with a number, an upper/lower-case letter or a Chinese character and may contain numbers, "_", "-" or ".". The account name is unique in the same region. If this parameter is not specified, the default value ScheduledScalingTaskId is used.
         :param task_enabled: Property taskEnabled: Whether to enable the scheduled task. - When the parameter is set to true, the task is enabled. - When the parameter is set to false, the task is disabled. The default value is true.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ScheduledTaskProps.__init__)
+            check_type(argname="argument launch_time", value=launch_time, expected_type=type_hints["launch_time"])
+            check_type(argname="argument scheduled_action", value=scheduled_action, expected_type=type_hints["scheduled_action"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument launch_expiration_time", value=launch_expiration_time, expected_type=type_hints["launch_expiration_time"])
+            check_type(argname="argument recurrence_end_time", value=recurrence_end_time, expected_type=type_hints["recurrence_end_time"])
+            check_type(argname="argument recurrence_type", value=recurrence_type, expected_type=type_hints["recurrence_type"])
+            check_type(argname="argument recurrence_value", value=recurrence_value, expected_type=type_hints["recurrence_value"])
+            check_type(argname="argument scheduled_task_name", value=scheduled_task_name, expected_type=type_hints["scheduled_task_name"])
+            check_type(argname="argument task_enabled", value=task_enabled, expected_type=type_hints["task_enabled"])
         self._values: typing.Dict[str, typing.Any] = {
             "launch_time": launch_time,
             "scheduled_action": scheduled_action,
         }
         if description is not None:
             self._values["description"] = description
         if launch_expiration_time is not None:
```

### Comparing `ros-cdk-ess-1.0.8/src/ros_cdk_ess.egg-info/PKG-INFO` & `ros-cdk-ess-1.0.9/src/ros_cdk_ess.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-ess
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS ESS Construct Library
```

