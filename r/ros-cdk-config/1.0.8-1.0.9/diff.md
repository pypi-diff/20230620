# Comparing `tmp/ros-cdk-config-1.0.8.tar.gz` & `tmp/ros-cdk-config-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-config-1.0.8.tar", last modified: Thu Jul 14 02:28:14 2022, max compression
+gzip compressed data, was "dist/ros-cdk-config-1.0.9.tar", last modified: Fri Sep 23 11:18:28 2022, max compression
```

## Comparing `ros-cdk-config-1.0.8.tar` & `ros-cdk-config-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:28:14.000000 ros-cdk-config-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:28:13.000000 ros-cdk-config-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:28:13.000000 ros-cdk-config-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:28:13.000000 ros-cdk-config-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1252 2022-07-14 02:28:14.000000 ros-cdk-config-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      188 2022-07-14 02:28:13.000000 ros-cdk-config-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:28:13.000000 ros-cdk-config-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:28:14.000000 ros-cdk-config-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1812 2022-07-14 02:28:13.000000 ros-cdk-config-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:28:14.000000 ros-cdk-config-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:28:14.000000 ros-cdk-config-1.0.8/src/ros_cdk_config/
--rw-r--r--   0 root         (0) root         (0)   107301 2022-07-14 02:28:13.000000 ros-cdk-config-1.0.8/src/ros_cdk_config/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:28:14.000000 ros-cdk-config-1.0.8/src/ros_cdk_config/_jsii/
--rw-r--r--   0 root         (0) root         (0)      389 2022-07-14 02:28:13.000000 ros-cdk-config-1.0.8/src/ros_cdk_config/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    55808 2022-07-14 02:28:13.000000 ros-cdk-config-1.0.8/src/ros_cdk_config/_jsii/ros-cdk-config@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:28:13.000000 ros-cdk-config-1.0.8/src/ros_cdk_config/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:28:14.000000 ros-cdk-config-1.0.8/src/ros_cdk_config.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1252 2022-07-14 02:28:13.000000 ros-cdk-config-1.0.8/src/ros_cdk_config.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      430 2022-07-14 02:28:14.000000 ros-cdk-config-1.0.8/src/ros_cdk_config.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:28:13.000000 ros-cdk-config-1.0.8/src/ros_cdk_config.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:28:13.000000 ros-cdk-config-1.0.8/src/ros_cdk_config.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2022-07-14 02:28:13.000000 ros-cdk-config-1.0.8/src/ros_cdk_config.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:18:28.000000 ros-cdk-config-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 11:18:28.000000 ros-cdk-config-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 11:18:28.000000 ros-cdk-config-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 11:18:28.000000 ros-cdk-config-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1252 2022-09-23 11:18:28.000000 ros-cdk-config-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      188 2022-09-23 11:18:28.000000 ros-cdk-config-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 11:18:28.000000 ros-cdk-config-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 11:18:28.000000 ros-cdk-config-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1841 2022-09-23 11:18:28.000000 ros-cdk-config-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:18:28.000000 ros-cdk-config-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:18:28.000000 ros-cdk-config-1.0.9/src/ros_cdk_config/
+-rw-r--r--   0 root         (0) root         (0)   125191 2022-09-23 11:18:28.000000 ros-cdk-config-1.0.9/src/ros_cdk_config/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:18:28.000000 ros-cdk-config-1.0.9/src/ros_cdk_config/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      423 2022-09-23 11:18:28.000000 ros-cdk-config-1.0.9/src/ros_cdk_config/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    55876 2022-09-23 11:18:28.000000 ros-cdk-config-1.0.9/src/ros_cdk_config/_jsii/ros-cdk-config@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:18:28.000000 ros-cdk-config-1.0.9/src/ros_cdk_config/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:18:28.000000 ros-cdk-config-1.0.9/src/ros_cdk_config.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1252 2022-09-23 11:18:28.000000 ros-cdk-config-1.0.9/src/ros_cdk_config.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      430 2022-09-23 11:18:28.000000 ros-cdk-config-1.0.9/src/ros_cdk_config.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:18:28.000000 ros-cdk-config-1.0.9/src/ros_cdk_config.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 11:18:28.000000 ros-cdk-config-1.0.9/src/ros_cdk_config.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2022-09-23 11:18:28.000000 ros-cdk-config-1.0.9/src/ros_cdk_config.egg-info/top_level.txt
```

### Comparing `ros-cdk-config-1.0.8/LICENSE` & `ros-cdk-config-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-config-1.0.8/PKG-INFO` & `ros-cdk-config-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-config
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS CONFIG Construct Library
```

### Comparing `ros-cdk-config-1.0.8/setup.py` & `ros-cdk-config-1.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-config",
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
         "ros_cdk_config",
         "ros_cdk_config._jsii"
     ],
     "package_data": {
         "ros_cdk_config._jsii": [
-            "ros-cdk-config@1.0.8.jsii.tgz"
+            "ros-cdk-config@1.0.9.jsii.tgz"
         ],
         "ros_cdk_config": [
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

### Comparing `ros-cdk-config-1.0.8/src/ros_cdk_config/__init__.py` & `ros-cdk-config-1.0.9/src/ros_cdk_config/__init__.py`

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
 
 
 class CompliancePack(
     ros_cdk_core.Resource,
@@ -29,61 +31,67 @@
 ):
     '''A ROS resource type:  ``ALIYUN::Config::CompliancePack``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "CompliancePackProps",
+        props: typing.Union["CompliancePackProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::Config::CompliancePack``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(CompliancePack.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAccountId")
     def attr_account_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute AccountId: Aliyun User Id.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAccountId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCompliancePackId")
     def attr_compliance_pack_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute CompliancePackId: Compliance Package ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCompliancePackId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCompliancePackName")
     def attr_compliance_pack_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute CompliancePackName: Compliance Package Name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCompliancePackName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCompliancePackTemplateId")
     def attr_compliance_pack_template_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute CompliancePackTemplateId: Compliance Package Template Id.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCompliancePackTemplateId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDescription")
     def attr_description(self) -> ros_cdk_core.IResolvable:
         '''Attribute Description: Description.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDescription"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrRiskLevel")
     def attr_risk_level(self) -> ros_cdk_core.IResolvable:
         '''Attribute RiskLevel: Ris Level.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRiskLevel"))
 
 
 @jsii.data_type(
@@ -101,24 +109,31 @@
     def __init__(
         self,
         *,
         compliance_pack_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         description: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         risk_level: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
         compliance_pack_template_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        config_rules: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosCompliancePack.ConfigRulesProperty"]]]] = None,
+        config_rules: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosCompliancePack.ConfigRulesProperty", typing.Dict[str, typing.Any]]]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::Config::CompliancePack``.
 
         :param compliance_pack_name: Property compliancePackName: Compliance Package Name.
         :param description: Property description: Description.
         :param risk_level: Property riskLevel: Ris Level.
         :param compliance_pack_template_id: Property compliancePackTemplateId: Compliance Package Template Id.
         :param config_rules: Property configRules: Config Rule List.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(CompliancePackProps.__init__)
+            check_type(argname="argument compliance_pack_name", value=compliance_pack_name, expected_type=type_hints["compliance_pack_name"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument risk_level", value=risk_level, expected_type=type_hints["risk_level"])
+            check_type(argname="argument compliance_pack_template_id", value=compliance_pack_template_id, expected_type=type_hints["compliance_pack_template_id"])
+            check_type(argname="argument config_rules", value=config_rules, expected_type=type_hints["config_rules"])
         self._values: typing.Dict[str, typing.Any] = {
             "compliance_pack_name": compliance_pack_name,
             "description": description,
             "risk_level": risk_level,
         }
         if compliance_pack_template_id is not None:
             self._values["compliance_pack_template_id"] = compliance_pack_template_id
@@ -183,31 +198,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::Config::DeliveryChannel``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "DeliveryChannelProps",
+        props: typing.Union["DeliveryChannelProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::Config::DeliveryChannel``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(DeliveryChannel.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDeliveryChannelId")
     def attr_delivery_channel_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute DeliveryChannelId: The ID of the delivery method.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDeliveryChannelId"))
 
 
 @jsii.data_type(
@@ -238,14 +259,22 @@
         :param delivery_channel_assume_role_arn: Property deliveryChannelAssumeRoleArn: The Alibaba Cloud Resource Name (ARN) of the role to be assumed by the delivery method. This parameter is required when you create a delivery method. Note If the delivery method assumes the service linked role for Cloud Config, you can specify the ARN in the format of the provided example and replace the account ID with the ID of your Alibaba Cloud account.
         :param delivery_channel_target_arn: Property deliveryChannelTargetArn: The ARN of the delivery destination. This parameter is required when you create a delivery method. The value must be in one of the following formats: acs:oss:{RegionId}:{Aliuid}:{bucketName} if your delivery destination is an Object Storage Service (OSS) bucket. acs:mns:{RegionId}:{Aliuid}:/topics/{topicName} if your delivery destination is a Message Service (MNS) topic. acs:log:{RegionId}:{Aliuid}:project/{projectName}/logstore/{logstoreName} if your delivery destination is a Log Service Logstore.
         :param delivery_channel_type: Property deliveryChannelType: The type of the delivery method. This parameter is required when you create a delivery method. Valid values: OSS MNS SLS
         :param delivery_channel_condition: Property deliveryChannelCondition: The rule attached to the delivery method. This parameter is applicable only to delivery methods of the MNS type. This parameter allows you to specify the lowest risk level for the events to subscribe to and the resource types for which you want to subscribe to events. To specify the lowest risk level for the events to subscribe to, use the following format:{"filterType":"RuleRiskLevel","value":"1","multiple":false}. The value field indicates the lowest risk level and can be set to 1, 2, or 3, which indicates the high risk level, the medium risk level, and the low risk level, respectively. To specify the resource types for which you want to subscribe to events, use the following format:{"filterType":"ResourceType","values":["ACS::ACK::Cluster","ACS::ActionTrail::Trail","ACS::CBWP::CommonBandwidthPackage"],"multiple":true}. The values field indicates the resource types. Its value is a JSON array. Example: [{"filterType":"ResourceType","values":["ACS::ActionTrail::Trail","ACS::CBWP::CommonBandwidthPackage","ACS::CDN::Domain","ACS::CEN::CenBandwidthPackage","ACS::CEN::CenInstance","ACS::CEN::Flowlog","ACS::DdosCoo::Instance"],"multiple":true}]
         :param delivery_channel_name: Property deliveryChannelName: The name of the delivery method.
         :param description: Property description: The description of the delivery method.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(DeliveryChannelProps.__init__)
+            check_type(argname="argument delivery_channel_assume_role_arn", value=delivery_channel_assume_role_arn, expected_type=type_hints["delivery_channel_assume_role_arn"])
+            check_type(argname="argument delivery_channel_target_arn", value=delivery_channel_target_arn, expected_type=type_hints["delivery_channel_target_arn"])
+            check_type(argname="argument delivery_channel_type", value=delivery_channel_type, expected_type=type_hints["delivery_channel_type"])
+            check_type(argname="argument delivery_channel_condition", value=delivery_channel_condition, expected_type=type_hints["delivery_channel_condition"])
+            check_type(argname="argument delivery_channel_name", value=delivery_channel_name, expected_type=type_hints["delivery_channel_name"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
         self._values: typing.Dict[str, typing.Any] = {
             "delivery_channel_assume_role_arn": delivery_channel_assume_role_arn,
             "delivery_channel_target_arn": delivery_channel_target_arn,
             "delivery_channel_type": delivery_channel_type,
         }
         if delivery_channel_condition is not None:
             self._values["delivery_channel_condition"] = delivery_channel_condition
@@ -358,183 +387,210 @@
 ):
     '''A ROS template type:  ``ALIYUN::Config::CompliancePack``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosCompliancePackProps",
+        props: typing.Union["RosCompliancePackProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::Config::CompliancePack``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosCompliancePack.__init__)
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
+            type_hints = typing.get_type_hints(RosCompliancePack._render_properties)
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
     @jsii.member(jsii_name="attrAccountId")
     def attr_account_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: AccountId: Aliyun User Id
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAccountId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCompliancePackId")
     def attr_compliance_pack_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: CompliancePackId: Compliance Package ID
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCompliancePackId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCompliancePackName")
     def attr_compliance_pack_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: CompliancePackName: Compliance Package Name
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCompliancePackName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCompliancePackTemplateId")
     def attr_compliance_pack_template_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: CompliancePackTemplateId: Compliance Package Template Id
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCompliancePackTemplateId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDescription")
     def attr_description(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Description: Description
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDescription"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrRiskLevel")
     def attr_risk_level(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: RiskLevel: Ris Level
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRiskLevel"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="compliancePackName")
     def compliance_pack_name(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: compliancePackName: Compliance Package Name
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "compliancePackName"))
 
     @compliance_pack_name.setter
     def compliance_pack_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCompliancePack, "compliance_pack_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "compliancePackName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: description: Description
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCompliancePack, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCompliancePack, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="riskLevel")
     def risk_level(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property: riskLevel: Ris Level
         '''
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "riskLevel"))
 
     @risk_level.setter
     def risk_level(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCompliancePack, "risk_level").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "riskLevel", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="compliancePackTemplateId")
     def compliance_pack_template_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: compliancePackTemplateId: Compliance Package Template Id
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "compliancePackTemplateId"))
 
     @compliance_pack_template_id.setter
     def compliance_pack_template_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCompliancePack, "compliance_pack_template_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "compliancePackTemplateId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="configRules")
     def config_rules(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosCompliancePack.ConfigRulesProperty"]]]]:
         '''
         :Property: configRules: Config Rule List
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosCompliancePack.ConfigRulesProperty"]]]], jsii.get(self, "configRules"))
 
     @config_rules.setter
     def config_rules(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosCompliancePack.ConfigRulesProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCompliancePack, "config_rules").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "configRules", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-config.RosCompliancePack.ConfigRuleParametersProperty",
         jsii_struct_bases=[],
         name_mapping={
             "parameter_name": "parameterName",
@@ -551,14 +607,19 @@
             required: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param parameter_name: 
             :param parameter_value: 
             :param required: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosCompliancePack.ConfigRuleParametersProperty.__init__)
+                check_type(argname="argument parameter_name", value=parameter_name, expected_type=type_hints["parameter_name"])
+                check_type(argname="argument parameter_value", value=parameter_value, expected_type=type_hints["parameter_value"])
+                check_type(argname="argument required", value=required, expected_type=type_hints["required"])
             self._values: typing.Dict[str, typing.Any] = {}
             if parameter_name is not None:
                 self._values["parameter_name"] = parameter_name
             if parameter_value is not None:
                 self._values["parameter_value"] = parameter_value
             if required is not None:
                 self._values["required"] = required
@@ -616,23 +677,29 @@
     )
     class ConfigRulesProperty:
         def __init__(
             self,
             *,
             config_rule_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             config_rule_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-            config_rule_parameters: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosCompliancePack.ConfigRuleParametersProperty"]]]] = None,
+            config_rule_parameters: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosCompliancePack.ConfigRuleParametersProperty", typing.Dict[str, typing.Any]]]]]] = None,
             managed_rule_identifier: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param config_rule_id: 
             :param config_rule_name: 
             :param config_rule_parameters: 
             :param managed_rule_identifier: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosCompliancePack.ConfigRulesProperty.__init__)
+                check_type(argname="argument config_rule_id", value=config_rule_id, expected_type=type_hints["config_rule_id"])
+                check_type(argname="argument config_rule_name", value=config_rule_name, expected_type=type_hints["config_rule_name"])
+                check_type(argname="argument config_rule_parameters", value=config_rule_parameters, expected_type=type_hints["config_rule_parameters"])
+                check_type(argname="argument managed_rule_identifier", value=managed_rule_identifier, expected_type=type_hints["managed_rule_identifier"])
             self._values: typing.Dict[str, typing.Any] = {}
             if config_rule_id is not None:
                 self._values["config_rule_id"] = config_rule_id
             if config_rule_name is not None:
                 self._values["config_rule_name"] = config_rule_name
             if config_rule_parameters is not None:
                 self._values["config_rule_parameters"] = config_rule_parameters
@@ -706,24 +773,31 @@
     def __init__(
         self,
         *,
         compliance_pack_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         description: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         risk_level: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
         compliance_pack_template_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        config_rules: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosCompliancePack.ConfigRulesProperty]]]] = None,
+        config_rules: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosCompliancePack.ConfigRulesProperty, typing.Dict[str, typing.Any]]]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::Config::CompliancePack``.
 
         :param compliance_pack_name: 
         :param description: 
         :param risk_level: 
         :param compliance_pack_template_id: 
         :param config_rules: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosCompliancePackProps.__init__)
+            check_type(argname="argument compliance_pack_name", value=compliance_pack_name, expected_type=type_hints["compliance_pack_name"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument risk_level", value=risk_level, expected_type=type_hints["risk_level"])
+            check_type(argname="argument compliance_pack_template_id", value=compliance_pack_template_id, expected_type=type_hints["compliance_pack_template_id"])
+            check_type(argname="argument config_rules", value=config_rules, expected_type=type_hints["config_rules"])
         self._values: typing.Dict[str, typing.Any] = {
             "compliance_pack_name": compliance_pack_name,
             "description": description,
             "risk_level": risk_level,
         }
         if compliance_pack_template_id is not None:
             self._values["compliance_pack_template_id"] = compliance_pack_template_id
@@ -798,56 +872,65 @@
 ):
     '''A ROS template type:  ``ALIYUN::Config::DeliveryChannel``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosDeliveryChannelProps",
+        props: typing.Union["RosDeliveryChannelProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::Config::DeliveryChannel``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDeliveryChannel.__init__)
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
+            type_hints = typing.get_type_hints(RosDeliveryChannel._render_properties)
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
     @jsii.member(jsii_name="attrDeliveryChannelId")
     def attr_delivery_channel_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DeliveryChannelId: The ID of the delivery method.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDeliveryChannelId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="deliveryChannelAssumeRoleArn")
     def delivery_channel_assume_role_arn(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
@@ -860,17 +943,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "deliveryChannelAssumeRoleArn"))
 
     @delivery_channel_assume_role_arn.setter
     def delivery_channel_assume_role_arn(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDeliveryChannel, "delivery_channel_assume_role_arn").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "deliveryChannelAssumeRoleArn", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="deliveryChannelTargetArn")
     def delivery_channel_target_arn(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
@@ -883,17 +969,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "deliveryChannelTargetArn"))
 
     @delivery_channel_target_arn.setter
     def delivery_channel_target_arn(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDeliveryChannel, "delivery_channel_target_arn").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "deliveryChannelTargetArn", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="deliveryChannelType")
     def delivery_channel_type(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
@@ -906,26 +995,32 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "deliveryChannelType"))
 
     @delivery_channel_type.setter
     def delivery_channel_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDeliveryChannel, "delivery_channel_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "deliveryChannelType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDeliveryChannel, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="deliveryChannelCondition")
     def delivery_channel_condition(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -945,48 +1040,57 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "deliveryChannelCondition"))
 
     @delivery_channel_condition.setter
     def delivery_channel_condition(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDeliveryChannel, "delivery_channel_condition").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "deliveryChannelCondition", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="deliveryChannelName")
     def delivery_channel_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: deliveryChannelName: The name of the delivery method.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "deliveryChannelName"))
 
     @delivery_channel_name.setter
     def delivery_channel_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDeliveryChannel, "delivery_channel_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "deliveryChannelName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: description: The description of the delivery method.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDeliveryChannel, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-config.RosDeliveryChannelProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -1014,14 +1118,22 @@
         :param delivery_channel_assume_role_arn: 
         :param delivery_channel_target_arn: 
         :param delivery_channel_type: 
         :param delivery_channel_condition: 
         :param delivery_channel_name: 
         :param description: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDeliveryChannelProps.__init__)
+            check_type(argname="argument delivery_channel_assume_role_arn", value=delivery_channel_assume_role_arn, expected_type=type_hints["delivery_channel_assume_role_arn"])
+            check_type(argname="argument delivery_channel_target_arn", value=delivery_channel_target_arn, expected_type=type_hints["delivery_channel_target_arn"])
+            check_type(argname="argument delivery_channel_type", value=delivery_channel_type, expected_type=type_hints["delivery_channel_type"])
+            check_type(argname="argument delivery_channel_condition", value=delivery_channel_condition, expected_type=type_hints["delivery_channel_condition"])
+            check_type(argname="argument delivery_channel_name", value=delivery_channel_name, expected_type=type_hints["delivery_channel_name"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
         self._values: typing.Dict[str, typing.Any] = {
             "delivery_channel_assume_role_arn": delivery_channel_assume_role_arn,
             "delivery_channel_target_arn": delivery_channel_target_arn,
             "delivery_channel_type": delivery_channel_type,
         }
         if delivery_channel_condition is not None:
             self._values["delivery_channel_condition"] = delivery_channel_condition
@@ -1143,437 +1255,494 @@
 ):
     '''A ROS template type:  ``ALIYUN::Config::Rule``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosRuleProps",
+        props: typing.Union["RosRuleProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::Config::Rule``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosRule.__init__)
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
+            type_hints = typing.get_type_hints(RosRule._render_properties)
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
     @jsii.member(jsii_name="attrConfigRuleArn")
     def attr_config_rule_arn(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ConfigRuleArn: config rule arn
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrConfigRuleArn"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrConfigRuleId")
     def attr_config_rule_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ConfigRuleId: The ID of the rule
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrConfigRuleId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrConfigRuleTriggerTypes")
     def attr_config_rule_trigger_types(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ConfigRuleTriggerTypes: The trigger type of the rule. Valid values:  ConfigurationItemChangeNotification: The rule is triggered upon configuration changes. ScheduledNotification: The rule is triggered as scheduled.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrConfigRuleTriggerTypes"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDescription")
     def attr_description(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Description: The description of the rule
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDescription"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrEventSource")
     def attr_event_source(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: EventSource: The event source of the rule.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrEventSource"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrExcludeResourceIdsScope")
     def attr_exclude_resource_ids_scope(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ExcludeResourceIdsScope: The rule monitors excluded resource IDs, multiple of which are separated by commas, only applies to rules created based on managed rules, , custom rule this field is empty
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrExcludeResourceIdsScope"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInputParameters")
     def attr_input_parameters(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: InputParameters: The settings of the input parameters for the rule
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInputParameters"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrMaximumExecutionFrequency")
     def attr_maximum_execution_frequency(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: MaximumExecutionFrequency: The frequency of the compliance evaluations. Valid values:  One_Hour Three_Hours Six_Hours Twelve_Hours TwentyFour_Hours
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrMaximumExecutionFrequency"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrRegionIdsScope")
     def attr_region_ids_scope(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: RegionIdsScope: The rule monitors region IDs, separated by commas, only applies to rules created based on managed rules
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRegionIdsScope"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrResourceGroupIdsScope")
     def attr_resource_group_ids_scope(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ResourceGroupIdsScope: The rule monitors resource group IDs, separated by commas, only applies to rules created based on managed rules
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrResourceGroupIdsScope"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrResourceTypesScope")
     def attr_resource_types_scope(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ResourceTypesScope: The types of the resources to be evaluated against the rule
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrResourceTypesScope"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrRiskLevel")
     def attr_risk_level(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: RiskLevel: The risk level of the resources that are not compliant with the rule. Valid values:  1: critical 2: warning 3: info
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRiskLevel"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrRuleName")
     def attr_rule_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: RuleName: The name of the rule.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRuleName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSourceIdentifier")
     def attr_source_identifier(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: SourceIdentifier: The identifier of the rule.  For a managed rule, the value is the name of the managed rule. For a custom rule, the value is the ARN of the custom rule
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSourceIdentifier"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSourceOwner")
     def attr_source_owner(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: SourceOwner: Specifies whether you or Alibaba Cloud owns and manages the rule. Valid values:  CUSTOM_FC: The rule is a custom rule and you own the rule. ALIYUN: The rule is a managed rule and Alibaba Cloud owns the rule
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSourceOwner"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTagKeyScope")
     def attr_tag_key_scope(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TagKeyScope: The rule monitors the tag key, only applies to rules created based on managed rules
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTagKeyScope"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTagValueScope")
     def attr_tag_value_scope(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TagValueScope: The rule monitors the tag value, only applies to rules created based on managed rules
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTagValueScope"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="configRuleTriggerTypes")
     def config_rule_trigger_types(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: configRuleTriggerTypes: The trigger type of the rule. Valid values:  ConfigurationItemChangeNotification: The rule is triggered upon configuration changes. ScheduledNotification: The rule is triggered as scheduled.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "configRuleTriggerTypes"))
 
     @config_rule_trigger_types.setter
     def config_rule_trigger_types(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRule, "config_rule_trigger_types").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "configRuleTriggerTypes", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRule, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="resourceTypesScope")
     def resource_types_scope(
         self,
     ) -> typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]:
         '''
         :Property: resourceTypesScope: The types of the resources to be evaluated against the rule
         '''
         return typing.cast(typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]], jsii.get(self, "resourceTypesScope"))
 
     @resource_types_scope.setter
     def resource_types_scope(
         self,
         value: typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRule, "resource_types_scope").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "resourceTypesScope", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="riskLevel")
     def risk_level(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property: riskLevel: The risk level of the resources that are not compliant with the rule. Valid values:  1: critical 2: warning 3: info
         '''
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "riskLevel"))
 
     @risk_level.setter
     def risk_level(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRule, "risk_level").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "riskLevel", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="ruleName")
     def rule_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: ruleName: The name of the rule.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "ruleName"))
 
     @rule_name.setter
     def rule_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRule, "rule_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ruleName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="sourceIdentifier")
     def source_identifier(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: sourceIdentifier: The identifier of the rule.  For a managed rule, the value is the name of the managed rule. For a custom rule, the value is the ARN of the custom rule
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "sourceIdentifier"))
 
     @source_identifier.setter
     def source_identifier(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRule, "source_identifier").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "sourceIdentifier", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="sourceOwner")
     def source_owner(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: sourceOwner: Specifies whether you or Alibaba Cloud owns and manages the rule. Valid values:  CUSTOM_FC: The rule is a custom rule and you own the rule. ALIYUN: The rule is a managed rule and Alibaba Cloud owns the rule
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "sourceOwner"))
 
     @source_owner.setter
     def source_owner(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRule, "source_owner").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "sourceOwner", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: description: The description of the rule
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRule, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="excludeResourceIdsScope")
     def exclude_resource_ids_scope(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: excludeResourceIdsScope: The rule monitors excluded resource IDs, multiple of which are separated by commas, only applies to rules created based on managed rules, , custom rule this field is empty
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "excludeResourceIdsScope"))
 
     @exclude_resource_ids_scope.setter
     def exclude_resource_ids_scope(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRule, "exclude_resource_ids_scope").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "excludeResourceIdsScope", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="inputParameters")
     def input_parameters(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]]:
         '''
         :Property: inputParameters: The settings of the input parameters for the rule
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]], jsii.get(self, "inputParameters"))
 
     @input_parameters.setter
     def input_parameters(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRule, "input_parameters").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "inputParameters", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="maximumExecutionFrequency")
     def maximum_execution_frequency(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: maximumExecutionFrequency: The frequency of the compliance evaluations. Valid values:  One_Hour Three_Hours Six_Hours Twelve_Hours TwentyFour_Hours
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "maximumExecutionFrequency"))
 
     @maximum_execution_frequency.setter
     def maximum_execution_frequency(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRule, "maximum_execution_frequency").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "maximumExecutionFrequency", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="regionIdsScope")
     def region_ids_scope(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: regionIdsScope: The rule monitors region IDs, separated by commas, only applies to rules created based on managed rules
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "regionIdsScope"))
 
     @region_ids_scope.setter
     def region_ids_scope(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRule, "region_ids_scope").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "regionIdsScope", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="resourceGroupIdsScope")
     def resource_group_ids_scope(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: resourceGroupIdsScope: The rule monitors resource group IDs, separated by commas, only applies to rules created based on managed rules
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "resourceGroupIdsScope"))
 
     @resource_group_ids_scope.setter
     def resource_group_ids_scope(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRule, "resource_group_ids_scope").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "resourceGroupIdsScope", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tagKeyLogicScope")
     def tag_key_logic_scope(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: tagKeyLogicScope:
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "tagKeyLogicScope"))
 
     @tag_key_logic_scope.setter
     def tag_key_logic_scope(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRule, "tag_key_logic_scope").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tagKeyLogicScope", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tagKeyScope")
     def tag_key_scope(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: tagKeyScope: The rule monitors the tag key, only applies to rules created based on managed rules
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "tagKeyScope"))
 
     @tag_key_scope.setter
     def tag_key_scope(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRule, "tag_key_scope").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tagKeyScope", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tagValueScope")
     def tag_value_scope(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: tagValueScope: The rule monitors the tag value, only applies to rules created based on managed rules
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "tagValueScope"))
 
     @tag_value_scope.setter
     def tag_value_scope(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRule, "tag_value_scope").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tagValueScope", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-config.RosRuleProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -1628,14 +1797,31 @@
         :param maximum_execution_frequency: 
         :param region_ids_scope: 
         :param resource_group_ids_scope: 
         :param tag_key_logic_scope: 
         :param tag_key_scope: 
         :param tag_value_scope: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosRuleProps.__init__)
+            check_type(argname="argument config_rule_trigger_types", value=config_rule_trigger_types, expected_type=type_hints["config_rule_trigger_types"])
+            check_type(argname="argument resource_types_scope", value=resource_types_scope, expected_type=type_hints["resource_types_scope"])
+            check_type(argname="argument risk_level", value=risk_level, expected_type=type_hints["risk_level"])
+            check_type(argname="argument rule_name", value=rule_name, expected_type=type_hints["rule_name"])
+            check_type(argname="argument source_identifier", value=source_identifier, expected_type=type_hints["source_identifier"])
+            check_type(argname="argument source_owner", value=source_owner, expected_type=type_hints["source_owner"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument exclude_resource_ids_scope", value=exclude_resource_ids_scope, expected_type=type_hints["exclude_resource_ids_scope"])
+            check_type(argname="argument input_parameters", value=input_parameters, expected_type=type_hints["input_parameters"])
+            check_type(argname="argument maximum_execution_frequency", value=maximum_execution_frequency, expected_type=type_hints["maximum_execution_frequency"])
+            check_type(argname="argument region_ids_scope", value=region_ids_scope, expected_type=type_hints["region_ids_scope"])
+            check_type(argname="argument resource_group_ids_scope", value=resource_group_ids_scope, expected_type=type_hints["resource_group_ids_scope"])
+            check_type(argname="argument tag_key_logic_scope", value=tag_key_logic_scope, expected_type=type_hints["tag_key_logic_scope"])
+            check_type(argname="argument tag_key_scope", value=tag_key_scope, expected_type=type_hints["tag_key_scope"])
+            check_type(argname="argument tag_value_scope", value=tag_value_scope, expected_type=type_hints["tag_value_scope"])
         self._values: typing.Dict[str, typing.Any] = {
             "config_rule_trigger_types": config_rule_trigger_types,
             "resource_types_scope": resource_types_scope,
             "risk_level": risk_level,
             "rule_name": rule_name,
             "source_identifier": source_identifier,
             "source_owner": source_owner,
@@ -1826,142 +2012,148 @@
 ):
     '''A ROS resource type:  ``ALIYUN::Config::Rule``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RuleProps",
+        props: typing.Union["RuleProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::Config::Rule``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Rule.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrConfigRuleArn")
     def attr_config_rule_arn(self) -> ros_cdk_core.IResolvable:
         '''Attribute ConfigRuleArn: config rule arn.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrConfigRuleArn"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrConfigRuleId")
     def attr_config_rule_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ConfigRuleId: The ID of the rule.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrConfigRuleId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrConfigRuleTriggerTypes")
     def attr_config_rule_trigger_types(self) -> ros_cdk_core.IResolvable:
         '''Attribute ConfigRuleTriggerTypes: The trigger type of the rule.
 
         Valid values:  ConfigurationItemChangeNotification: The rule is triggered upon configuration changes. ScheduledNotification: The rule is triggered as scheduled.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrConfigRuleTriggerTypes"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDescription")
     def attr_description(self) -> ros_cdk_core.IResolvable:
         '''Attribute Description: The description of the rule.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDescription"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrEventSource")
     def attr_event_source(self) -> ros_cdk_core.IResolvable:
         '''Attribute EventSource: The event source of the rule.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrEventSource"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrExcludeResourceIdsScope")
     def attr_exclude_resource_ids_scope(self) -> ros_cdk_core.IResolvable:
         '''Attribute ExcludeResourceIdsScope: The rule monitors excluded resource IDs, multiple of which are separated by commas, only applies to rules created based on managed rules, , custom rule this field is empty.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrExcludeResourceIdsScope"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInputParameters")
     def attr_input_parameters(self) -> ros_cdk_core.IResolvable:
         '''Attribute InputParameters: The settings of the input parameters for the rule.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInputParameters"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrMaximumExecutionFrequency")
     def attr_maximum_execution_frequency(self) -> ros_cdk_core.IResolvable:
         '''Attribute MaximumExecutionFrequency: The frequency of the compliance evaluations.
 
         Valid values:  One_Hour Three_Hours Six_Hours Twelve_Hours TwentyFour_Hours
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrMaximumExecutionFrequency"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrRegionIdsScope")
     def attr_region_ids_scope(self) -> ros_cdk_core.IResolvable:
         '''Attribute RegionIdsScope: The rule monitors region IDs, separated by commas, only applies to rules created based on managed rules.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRegionIdsScope"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrResourceGroupIdsScope")
     def attr_resource_group_ids_scope(self) -> ros_cdk_core.IResolvable:
         '''Attribute ResourceGroupIdsScope: The rule monitors resource group IDs, separated by commas, only applies to rules created based on managed rules.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrResourceGroupIdsScope"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrResourceTypesScope")
     def attr_resource_types_scope(self) -> ros_cdk_core.IResolvable:
         '''Attribute ResourceTypesScope: The types of the resources to be evaluated against the rule.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrResourceTypesScope"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrRiskLevel")
     def attr_risk_level(self) -> ros_cdk_core.IResolvable:
         '''Attribute RiskLevel: The risk level of the resources that are not compliant with the rule.
 
         Valid values:  1: critical 2: warning 3: info
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRiskLevel"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrRuleName")
     def attr_rule_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute RuleName: The name of the rule.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRuleName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSourceIdentifier")
     def attr_source_identifier(self) -> ros_cdk_core.IResolvable:
         '''Attribute SourceIdentifier: The identifier of the rule.
 
         For a managed rule, the value is the name of the managed rule. For a custom rule, the value is the ARN of the custom rule
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSourceIdentifier"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSourceOwner")
     def attr_source_owner(self) -> ros_cdk_core.IResolvable:
         '''Attribute SourceOwner: Specifies whether you or Alibaba Cloud owns and manages the rule.
 
         Valid values:  CUSTOM_FC: The rule is a custom rule and you own the rule. ALIYUN: The rule is a managed rule and Alibaba Cloud owns the rule
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSourceOwner"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTagKeyScope")
     def attr_tag_key_scope(self) -> ros_cdk_core.IResolvable:
         '''Attribute TagKeyScope: The rule monitors the tag key, only applies to rules created based on managed rules.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTagKeyScope"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTagValueScope")
     def attr_tag_value_scope(self) -> ros_cdk_core.IResolvable:
         '''Attribute TagValueScope: The rule monitors the tag value, only applies to rules created based on managed rules.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTagValueScope"))
 
 
 @jsii.data_type(
@@ -2019,14 +2211,31 @@
         :param maximum_execution_frequency: Property maximumExecutionFrequency: The frequency of the compliance evaluations. Valid values: One_Hour Three_Hours Six_Hours Twelve_Hours TwentyFour_Hours
         :param region_ids_scope: Property regionIdsScope: The rule monitors region IDs, separated by commas, only applies to rules created based on managed rules.
         :param resource_group_ids_scope: Property resourceGroupIdsScope: The rule monitors resource group IDs, separated by commas, only applies to rules created based on managed rules.
         :param tag_key_logic_scope: Property tagKeyLogicScope:.
         :param tag_key_scope: Property tagKeyScope: The rule monitors the tag key, only applies to rules created based on managed rules.
         :param tag_value_scope: Property tagValueScope: The rule monitors the tag value, only applies to rules created based on managed rules.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RuleProps.__init__)
+            check_type(argname="argument config_rule_trigger_types", value=config_rule_trigger_types, expected_type=type_hints["config_rule_trigger_types"])
+            check_type(argname="argument resource_types_scope", value=resource_types_scope, expected_type=type_hints["resource_types_scope"])
+            check_type(argname="argument risk_level", value=risk_level, expected_type=type_hints["risk_level"])
+            check_type(argname="argument rule_name", value=rule_name, expected_type=type_hints["rule_name"])
+            check_type(argname="argument source_identifier", value=source_identifier, expected_type=type_hints["source_identifier"])
+            check_type(argname="argument source_owner", value=source_owner, expected_type=type_hints["source_owner"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument exclude_resource_ids_scope", value=exclude_resource_ids_scope, expected_type=type_hints["exclude_resource_ids_scope"])
+            check_type(argname="argument input_parameters", value=input_parameters, expected_type=type_hints["input_parameters"])
+            check_type(argname="argument maximum_execution_frequency", value=maximum_execution_frequency, expected_type=type_hints["maximum_execution_frequency"])
+            check_type(argname="argument region_ids_scope", value=region_ids_scope, expected_type=type_hints["region_ids_scope"])
+            check_type(argname="argument resource_group_ids_scope", value=resource_group_ids_scope, expected_type=type_hints["resource_group_ids_scope"])
+            check_type(argname="argument tag_key_logic_scope", value=tag_key_logic_scope, expected_type=type_hints["tag_key_logic_scope"])
+            check_type(argname="argument tag_key_scope", value=tag_key_scope, expected_type=type_hints["tag_key_scope"])
+            check_type(argname="argument tag_value_scope", value=tag_value_scope, expected_type=type_hints["tag_value_scope"])
         self._values: typing.Dict[str, typing.Any] = {
             "config_rule_trigger_types": config_rule_trigger_types,
             "resource_types_scope": resource_types_scope,
             "risk_level": risk_level,
             "rule_name": rule_name,
             "source_identifier": source_identifier,
             "source_owner": source_owner,
```

### Comparing `ros-cdk-config-1.0.8/src/ros_cdk_config.egg-info/PKG-INFO` & `ros-cdk-config-1.0.9/src/ros_cdk_config.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-config
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS CONFIG Construct Library
```

