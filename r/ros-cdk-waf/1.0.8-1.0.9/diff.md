# Comparing `tmp/ros-cdk-waf-1.0.8.tar.gz` & `tmp/ros-cdk-waf-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-waf-1.0.8.tar", last modified: Thu Jul 14 02:32:58 2022, max compression
+gzip compressed data, was "dist/ros-cdk-waf-1.0.9.tar", last modified: Fri Sep 23 11:02:15 2022, max compression
```

## Comparing `ros-cdk-waf-1.0.8.tar` & `ros-cdk-waf-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:32:58.000000 ros-cdk-waf-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:32:58.000000 ros-cdk-waf-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:32:58.000000 ros-cdk-waf-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:32:58.000000 ros-cdk-waf-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:32:58.000000 ros-cdk-waf-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      179 2022-07-14 02:32:58.000000 ros-cdk-waf-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:32:58.000000 ros-cdk-waf-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:32:58.000000 ros-cdk-waf-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1794 2022-07-14 02:32:58.000000 ros-cdk-waf-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:32:58.000000 ros-cdk-waf-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:32:58.000000 ros-cdk-waf-1.0.8/src/ros_cdk_waf/
--rw-r--r--   0 root         (0) root         (0)   152359 2022-07-14 02:32:58.000000 ros-cdk-waf-1.0.8/src/ros_cdk_waf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:32:58.000000 ros-cdk-waf-1.0.8/src/ros_cdk_waf/_jsii/
--rw-r--r--   0 root         (0) root         (0)      370 2022-07-14 02:32:58.000000 ros-cdk-waf-1.0.8/src/ros_cdk_waf/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    68139 2022-07-14 02:32:58.000000 ros-cdk-waf-1.0.8/src/ros_cdk_waf/_jsii/ros-cdk-waf@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:32:58.000000 ros-cdk-waf-1.0.8/src/ros_cdk_waf/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:32:58.000000 ros-cdk-waf-1.0.8/src/ros_cdk_waf.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:32:58.000000 ros-cdk-waf-1.0.8/src/ros_cdk_waf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      400 2022-07-14 02:32:58.000000 ros-cdk-waf-1.0.8/src/ros_cdk_waf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:32:58.000000 ros-cdk-waf-1.0.8/src/ros_cdk_waf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:32:58.000000 ros-cdk-waf-1.0.8/src/ros_cdk_waf.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-07-14 02:32:58.000000 ros-cdk-waf-1.0.8/src/ros_cdk_waf.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:02:15.000000 ros-cdk-waf-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 11:02:15.000000 ros-cdk-waf-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 11:02:15.000000 ros-cdk-waf-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 11:02:15.000000 ros-cdk-waf-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 11:02:15.000000 ros-cdk-waf-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      179 2022-09-23 11:02:15.000000 ros-cdk-waf-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 11:02:15.000000 ros-cdk-waf-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 11:02:15.000000 ros-cdk-waf-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1823 2022-09-23 11:02:15.000000 ros-cdk-waf-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:02:15.000000 ros-cdk-waf-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:02:15.000000 ros-cdk-waf-1.0.9/src/ros_cdk_waf/
+-rw-r--r--   0 root         (0) root         (0)   184094 2022-09-23 11:02:15.000000 ros-cdk-waf-1.0.9/src/ros_cdk_waf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:02:15.000000 ros-cdk-waf-1.0.9/src/ros_cdk_waf/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      404 2022-09-23 11:02:15.000000 ros-cdk-waf-1.0.9/src/ros_cdk_waf/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    68205 2022-09-23 11:02:15.000000 ros-cdk-waf-1.0.9/src/ros_cdk_waf/_jsii/ros-cdk-waf@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:02:15.000000 ros-cdk-waf-1.0.9/src/ros_cdk_waf/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:02:15.000000 ros-cdk-waf-1.0.9/src/ros_cdk_waf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 11:02:15.000000 ros-cdk-waf-1.0.9/src/ros_cdk_waf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      400 2022-09-23 11:02:15.000000 ros-cdk-waf-1.0.9/src/ros_cdk_waf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:02:15.000000 ros-cdk-waf-1.0.9/src/ros_cdk_waf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 11:02:15.000000 ros-cdk-waf-1.0.9/src/ros_cdk_waf.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-09-23 11:02:15.000000 ros-cdk-waf-1.0.9/src/ros_cdk_waf.egg-info/top_level.txt
```

### Comparing `ros-cdk-waf-1.0.8/LICENSE` & `ros-cdk-waf-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-waf-1.0.8/PKG-INFO` & `ros-cdk-waf-1.0.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-waf
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS WAF Construct Library
```

### Comparing `ros-cdk-waf-1.0.8/setup.py` & `ros-cdk-waf-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-waf",
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
         "ros_cdk_waf",
         "ros_cdk_waf._jsii"
     ],
     "package_data": {
         "ros_cdk_waf._jsii": [
-            "ros-cdk-waf@1.0.8.jsii.tgz"
+            "ros-cdk-waf@1.0.9.jsii.tgz"
         ],
         "ros_cdk_waf": [
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

### Comparing `ros-cdk-waf-1.0.8/src/ros_cdk_waf/__init__.py` & `ros-cdk-waf-1.0.9/src/ros_cdk_waf/__init__.py`

 * *Files 25% similar despite different names*

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
 
 
 class AclRule(
     ros_cdk_core.Resource,
@@ -29,28 +31,34 @@
 ):
     '''A ROS resource type:  ``ALIYUN::WAF::AclRule``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "AclRuleProps",
+        props: typing.Union["AclRuleProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::WAF::AclRule``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(AclRule.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-waf.AclRuleProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -75,14 +83,21 @@
 
         :param domain: Property domain: Domain name.
         :param instance_id: Property instanceId: WAF instance ID. Description Interface You can view your current WAF instance ID by calling DescribePayInfo.
         :param rules: Property rules: Detailed information of precise access control rules, expressed in JSON format strings.
         :param region: Property region: Examples of areas where the WAF. Value: cn: China mainland (default) cn-hongkong: China HongKong and other overseas
         :param rule_id: Property ruleId: Precise access control rule ID.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(AclRuleProps.__init__)
+            check_type(argname="argument domain", value=domain, expected_type=type_hints["domain"])
+            check_type(argname="argument instance_id", value=instance_id, expected_type=type_hints["instance_id"])
+            check_type(argname="argument rules", value=rules, expected_type=type_hints["rules"])
+            check_type(argname="argument region", value=region, expected_type=type_hints["region"])
+            check_type(argname="argument rule_id", value=rule_id, expected_type=type_hints["rule_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "domain": domain,
             "instance_id": instance_id,
             "rules": rules,
         }
         if region is not None:
             self._values["region"] = region
@@ -153,115 +168,121 @@
 ):
     '''A ROS resource type:  ``ALIYUN::WAF::Domain``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "DomainProps",
+        props: typing.Union["DomainProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::WAF::Domain``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Domain.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrClusterType")
     def attr_cluster_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute ClusterType: Cluster type.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClusterType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCname")
     def attr_cname(self) -> ros_cdk_core.IResolvable:
         '''Attribute Cname: CNAME assigned by WAF instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCname"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDomainName")
     def attr_domain_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute DomainName: Domain name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDomainName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrHttp2Port")
     def attr_http2_port(self) -> ros_cdk_core.IResolvable:
         '''Attribute Http2Port: Http2 port configuration.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrHttp2Port"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrHttpPort")
     def attr_http_port(self) -> ros_cdk_core.IResolvable:
         '''Attribute HttpPort: Http port configuration.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrHttpPort"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrHttpsPort")
     def attr_https_port(self) -> ros_cdk_core.IResolvable:
         '''Attribute HttpsPort: Https port configuration.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrHttpsPort"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrHttpsRedirect")
     def attr_https_redirect(self) -> ros_cdk_core.IResolvable:
         '''Attribute HttpsRedirect: Https forced redirect configuration.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrHttpsRedirect"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrHttpToUserIp")
     def attr_http_to_user_ip(self) -> ros_cdk_core.IResolvable:
         '''Attribute HttpToUserIp: Http back to source.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrHttpToUserIp"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceId")
     def attr_instance_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute InstanceId: Instance id.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrIsAccessProduct")
     def attr_is_access_product(self) -> ros_cdk_core.IResolvable:
         '''Attribute IsAccessProduct: Is there a seven-layer agency before WAF.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrIsAccessProduct"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrLoadBalancing")
     def attr_load_balancing(self) -> ros_cdk_core.IResolvable:
         '''Attribute LoadBalancing: Load balancing configuration.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLoadBalancing"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrLogHeaders")
     def attr_log_headers(self) -> ros_cdk_core.IResolvable:
         '''Attribute LogHeaders: Domain traffic tagging.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLogHeaders"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrResourceGroupId")
     def attr_resource_group_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ResourceGroupId: Resource group Id.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrResourceGroupId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSourceIps")
     def attr_source_ips(self) -> ros_cdk_core.IResolvable:
         '''Attribute SourceIps: Back to source IP configuration.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSourceIps"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVersion")
     def attr_version(self) -> ros_cdk_core.IResolvable:
         '''Attribute Version: Optimistic lock version.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVersion"))
 
 
 class DomainConfig(
@@ -271,37 +292,43 @@
 ):
     '''A ROS resource type:  ``ALIYUN::WAF::DomainConfig``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "DomainConfigProps",
+        props: typing.Union["DomainConfigProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::WAF::DomainConfig``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(DomainConfig.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCname")
     def attr_cname(self) -> ros_cdk_core.IResolvable:
         '''Attribute Cname: CNAME assigned by WAF instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCname"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrProtocolType")
     def attr_protocol_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute ProtocolType: agreement type:0: indicates that the HTTP protocol is supported.1: indicates that the HTTPS protocol is supported.2: indicates that both HTTP and HTTPS protocols are supported.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrProtocolType"))
 
 
 @jsii.data_type(
@@ -350,14 +377,28 @@
         :param https_redirect: Property httpsRedirect: HTTPS is turned forcefully jump the argument: 0: off (default) 1: Turn Description required to complete the request parameters using only HTTPS access protocol. After opening force will show a jump HTTP request is HTTPS, a default jump to 443.
         :param http_to_user_ip: Property httpToUserIp: Whether to open HTTPS access request is forwarded back to the source station via the HTTP protocol, the value of: 0: off (default) 1: Turn Note If your site does not support HTTPS back to the source, open source HTTP return (default back to the source port is port 80) function key, can be realized by WAF HTTPS access.
         :param load_balancing: Property loadBalancing: Back to the source load balancing policy values: 0: IP Hash way. 1: represents a polling mode.
         :param region: Property region: Examples of areas where the WAF. Value: cn: China mainland (default) cn-hongkong: China HongKong and other overseas
         :param rs_type: Property rsType: Back to the source address type the domain name values: 0: back to the source to IP. 1: Indicates the domain name back to the source.
         :param source_ips: Property sourceIps: Source station IP, supports a plurality of specified IP. Example values: [ "1.1.1.1"].
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(DomainConfigProps.__init__)
+            check_type(argname="argument domain", value=domain, expected_type=type_hints["domain"])
+            check_type(argname="argument instance_id", value=instance_id, expected_type=type_hints["instance_id"])
+            check_type(argname="argument is_access_product", value=is_access_product, expected_type=type_hints["is_access_product"])
+            check_type(argname="argument protocols", value=protocols, expected_type=type_hints["protocols"])
+            check_type(argname="argument http_port", value=http_port, expected_type=type_hints["http_port"])
+            check_type(argname="argument https_port", value=https_port, expected_type=type_hints["https_port"])
+            check_type(argname="argument https_redirect", value=https_redirect, expected_type=type_hints["https_redirect"])
+            check_type(argname="argument http_to_user_ip", value=http_to_user_ip, expected_type=type_hints["http_to_user_ip"])
+            check_type(argname="argument load_balancing", value=load_balancing, expected_type=type_hints["load_balancing"])
+            check_type(argname="argument region", value=region, expected_type=type_hints["region"])
+            check_type(argname="argument rs_type", value=rs_type, expected_type=type_hints["rs_type"])
+            check_type(argname="argument source_ips", value=source_ips, expected_type=type_hints["source_ips"])
         self._values: typing.Dict[str, typing.Any] = {
             "domain": domain,
             "instance_id": instance_id,
             "is_access_product": is_access_product,
             "protocols": protocols,
         }
         if http_port is not None:
@@ -547,15 +588,15 @@
         connection_time: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         http2_port: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
         http_port: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
         https_port: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
         https_redirect: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         http_to_user_ip: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         load_balancing: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        log_headers: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosDomain.LogHeadersProperty"]]]] = None,
+        log_headers: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosDomain.LogHeadersProperty", typing.Dict[str, typing.Any]]]]]] = None,
         read_time: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         resource_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         write_time: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::WAF::Domain``.
 
         :param domain_name: Property domainName: Domain name.
@@ -571,14 +612,32 @@
         :param http_to_user_ip: Property httpToUserIp: Http back to source.
         :param load_balancing: Property loadBalancing: Load balancing configuration.
         :param log_headers: Property logHeaders: Domain traffic tagging.
         :param read_time: Property readTime: Read connection timeout period.
         :param resource_group_id: Property resourceGroupId: Resource group Id.
         :param write_time: Property writeTime: Write connection timeout period.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(DomainProps.__init__)
+            check_type(argname="argument domain_name", value=domain_name, expected_type=type_hints["domain_name"])
+            check_type(argname="argument instance_id", value=instance_id, expected_type=type_hints["instance_id"])
+            check_type(argname="argument is_access_product", value=is_access_product, expected_type=type_hints["is_access_product"])
+            check_type(argname="argument source_ips", value=source_ips, expected_type=type_hints["source_ips"])
+            check_type(argname="argument cluster_type", value=cluster_type, expected_type=type_hints["cluster_type"])
+            check_type(argname="argument connection_time", value=connection_time, expected_type=type_hints["connection_time"])
+            check_type(argname="argument http2_port", value=http2_port, expected_type=type_hints["http2_port"])
+            check_type(argname="argument http_port", value=http_port, expected_type=type_hints["http_port"])
+            check_type(argname="argument https_port", value=https_port, expected_type=type_hints["https_port"])
+            check_type(argname="argument https_redirect", value=https_redirect, expected_type=type_hints["https_redirect"])
+            check_type(argname="argument http_to_user_ip", value=http_to_user_ip, expected_type=type_hints["http_to_user_ip"])
+            check_type(argname="argument load_balancing", value=load_balancing, expected_type=type_hints["load_balancing"])
+            check_type(argname="argument log_headers", value=log_headers, expected_type=type_hints["log_headers"])
+            check_type(argname="argument read_time", value=read_time, expected_type=type_hints["read_time"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument write_time", value=write_time, expected_type=type_hints["write_time"])
         self._values: typing.Dict[str, typing.Any] = {
             "domain_name": domain_name,
             "instance_id": instance_id,
             "is_access_product": is_access_product,
             "source_ips": source_ips,
         }
         if cluster_type is not None:
@@ -751,61 +810,67 @@
 ):
     '''A ROS resource type:  ``ALIYUN::WAF::Instance``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "InstanceProps",
+        props: typing.Union["InstanceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::WAF::Instance``.
 
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
     @jsii.member(jsii_name="attrEndDate")
     def attr_end_date(self) -> ros_cdk_core.IResolvable:
         '''Attribute EndDate: Due date of the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrEndDate"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInDebt")
     def attr_in_debt(self) -> ros_cdk_core.IResolvable:
         '''Attribute InDebt: Instance is overdue.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInDebt"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceId")
     def attr_instance_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute InstanceId: Instance ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrRemainDay")
     def attr_remain_day(self) -> ros_cdk_core.IResolvable:
         '''Attribute RemainDay: Number of available days for WAF Trial version.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRemainDay"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSubscriptionType")
     def attr_subscription_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute SubscriptionType: Subscription type of the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSubscriptionType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTrial")
     def attr_trial(self) -> ros_cdk_core.IResolvable:
         '''Attribute Trial: Trial version.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTrial"))
 
 
 @jsii.data_type(
@@ -857,14 +922,29 @@
         :param prefessional_service: Property prefessionalService:.
         :param subscription_type: Property subscriptionType: Subscription type of the instance.
         :param waf_log: Property wafLog:.
         :param period: Property period:.
         :param renewal_status: Property renewalStatus:.
         :param renew_period: Property renewPeriod:.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(InstanceProps.__init__)
+            check_type(argname="argument big_screen", value=big_screen, expected_type=type_hints["big_screen"])
+            check_type(argname="argument exclusive_ip_package", value=exclusive_ip_package, expected_type=type_hints["exclusive_ip_package"])
+            check_type(argname="argument ext_bandwidth", value=ext_bandwidth, expected_type=type_hints["ext_bandwidth"])
+            check_type(argname="argument ext_domain_package", value=ext_domain_package, expected_type=type_hints["ext_domain_package"])
+            check_type(argname="argument log_storage", value=log_storage, expected_type=type_hints["log_storage"])
+            check_type(argname="argument log_time", value=log_time, expected_type=type_hints["log_time"])
+            check_type(argname="argument package_code", value=package_code, expected_type=type_hints["package_code"])
+            check_type(argname="argument prefessional_service", value=prefessional_service, expected_type=type_hints["prefessional_service"])
+            check_type(argname="argument subscription_type", value=subscription_type, expected_type=type_hints["subscription_type"])
+            check_type(argname="argument waf_log", value=waf_log, expected_type=type_hints["waf_log"])
+            check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+            check_type(argname="argument renewal_status", value=renewal_status, expected_type=type_hints["renewal_status"])
+            check_type(argname="argument renew_period", value=renew_period, expected_type=type_hints["renew_period"])
         self._values: typing.Dict[str, typing.Any] = {
             "big_screen": big_screen,
             "exclusive_ip_package": exclusive_ip_package,
             "ext_bandwidth": ext_bandwidth,
             "ext_domain_package": ext_domain_package,
             "log_storage": log_storage,
             "log_time": log_time,
@@ -999,37 +1079,43 @@
 ):
     '''A ROS resource type:  ``ALIYUN::WAF::LogServiceEnable``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "LogServiceEnableProps",
+        props: typing.Union["LogServiceEnableProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::WAF::LogServiceEnable``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(LogServiceEnable.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDomain")
     def attr_domain(self) -> ros_cdk_core.IResolvable:
         '''Attribute Domain: The domain name that is added to WAF.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDomain"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceId")
     def attr_instance_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute InstanceId: The ID of the WAF instance.
 
         You can call the DescribeInstanceInfo operation to query the ID of the WAF instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceId"))
@@ -1048,14 +1134,18 @@
         instance_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::WAF::LogServiceEnable``.
 
         :param domain: Property domain: The domain name that is added to WAF.
         :param instance_id: Property instanceId: The ID of the WAF instance. You can call the DescribeInstanceInfo operation to query the ID of the WAF instance.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(LogServiceEnableProps.__init__)
+            check_type(argname="argument domain", value=domain, expected_type=type_hints["domain"])
+            check_type(argname="argument instance_id", value=instance_id, expected_type=type_hints["instance_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "domain": domain,
             "instance_id": instance_id,
         }
 
     @builtins.property
     def domain(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -1093,73 +1183,88 @@
 ):
     '''A ROS template type:  ``ALIYUN::WAF::AclRule``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosAclRuleProps",
+        props: typing.Union["RosAclRuleProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::WAF::AclRule``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosAclRule.__init__)
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
+            type_hints = typing.get_type_hints(RosAclRule._render_properties)
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
     @jsii.member(jsii_name="domain")
     def domain(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: domain: Domain name.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "domain"))
 
     @domain.setter
     def domain(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAclRule, "domain").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "domain", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         '''A factory method that creates a new instance of this class from an object containing the properties of this ROS resource.'''
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAclRule, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceId")
     def instance_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         instanceId: WAF instance ID.
         Description Interface You can view your current WAF instance ID by calling DescribePayInfo.
@@ -1167,32 +1272,38 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "instanceId"))
 
     @instance_id.setter
     def instance_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAclRule, "instance_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rules")
     def rules(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: rules: Detailed information of precise access control rules, expressed in JSON format strings.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "rules"))
 
     @rules.setter
     def rules(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAclRule, "rules").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "rules", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="region")
     def region(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1203,31 +1314,37 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "region"))
 
     @region.setter
     def region(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAclRule, "region").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "region", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="ruleId")
     def rule_id(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: ruleId: Precise access control rule ID
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "ruleId"))
 
     @rule_id.setter
     def rule_id(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAclRule, "rule_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ruleId", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-waf.RosAclRuleProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -1252,14 +1369,21 @@
 
         :param domain: 
         :param instance_id: 
         :param rules: 
         :param region: 
         :param rule_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosAclRuleProps.__init__)
+            check_type(argname="argument domain", value=domain, expected_type=type_hints["domain"])
+            check_type(argname="argument instance_id", value=instance_id, expected_type=type_hints["instance_id"])
+            check_type(argname="argument rules", value=rules, expected_type=type_hints["rules"])
+            check_type(argname="argument region", value=region, expected_type=type_hints["region"])
+            check_type(argname="argument rule_id", value=rule_id, expected_type=type_hints["rule_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "domain": domain,
             "instance_id": instance_id,
             "rules": rules,
         }
         if region is not None:
             self._values["region"] = region
@@ -1339,440 +1463,500 @@
 ):
     '''A ROS template type:  ``ALIYUN::WAF::Domain``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosDomainProps",
+        props: typing.Union["RosDomainProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::WAF::Domain``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDomain.__init__)
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
+            type_hints = typing.get_type_hints(RosDomain._render_properties)
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
     @jsii.member(jsii_name="attrClusterType")
     def attr_cluster_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ClusterType: Cluster type
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClusterType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCname")
     def attr_cname(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Cname: CNAME assigned by WAF instance
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCname"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDomainName")
     def attr_domain_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DomainName: Domain name
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDomainName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrHttp2Port")
     def attr_http2_port(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Http2Port: Http2 port configuration
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrHttp2Port"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrHttpPort")
     def attr_http_port(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: HttpPort: Http port configuration
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrHttpPort"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrHttpsPort")
     def attr_https_port(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: HttpsPort: Https port configuration
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrHttpsPort"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrHttpsRedirect")
     def attr_https_redirect(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: HttpsRedirect: Https forced redirect configuration
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrHttpsRedirect"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrHttpToUserIp")
     def attr_http_to_user_ip(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: HttpToUserIp: Http back to source
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrHttpToUserIp"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceId")
     def attr_instance_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: InstanceId: Instance id
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrIsAccessProduct")
     def attr_is_access_product(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: IsAccessProduct: Is there a seven-layer agency before WAF
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrIsAccessProduct"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrLoadBalancing")
     def attr_load_balancing(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: LoadBalancing: Load balancing configuration
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLoadBalancing"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrLogHeaders")
     def attr_log_headers(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: LogHeaders: Domain traffic tagging
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLogHeaders"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrResourceGroupId")
     def attr_resource_group_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ResourceGroupId: Resource group Id
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrResourceGroupId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSourceIps")
     def attr_source_ips(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: SourceIps: Back to source IP configuration
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSourceIps"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVersion")
     def attr_version(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Version: Optimistic lock version
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVersion"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="domainName")
     def domain_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: domainName: Domain name
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "domainName"))
 
     @domain_name.setter
     def domain_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDomain, "domain_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "domainName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDomain, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceId")
     def instance_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: instanceId: Instance id
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "instanceId"))
 
     @instance_id.setter
     def instance_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDomain, "instance_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="isAccessProduct")
     def is_access_product(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: isAccessProduct: Is there a seven-layer agency before WAF
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "isAccessProduct"))
 
     @is_access_product.setter
     def is_access_product(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDomain, "is_access_product").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "isAccessProduct", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="sourceIps")
     def source_ips(
         self,
     ) -> typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]:
         '''
         :Property: sourceIps: Back to source IP configuration
         '''
         return typing.cast(typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]], jsii.get(self, "sourceIps"))
 
     @source_ips.setter
     def source_ips(
         self,
         value: typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDomain, "source_ips").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "sourceIps", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="clusterType")
     def cluster_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: clusterType: Cluster type
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "clusterType"))
 
     @cluster_type.setter
     def cluster_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDomain, "cluster_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "clusterType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="connectionTime")
     def connection_time(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: connectionTime: Connection timeout
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "connectionTime"))
 
     @connection_time.setter
     def connection_time(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDomain, "connection_time").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "connectionTime", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="http2Port")
     def http2_port(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
         '''
         :Property: http2Port: Http2 port configuration
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]], jsii.get(self, "http2Port"))
 
     @http2_port.setter
     def http2_port(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDomain, "http2_port").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "http2Port", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="httpPort")
     def http_port(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
         '''
         :Property: httpPort: Http port configuration
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]], jsii.get(self, "httpPort"))
 
     @http_port.setter
     def http_port(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDomain, "http_port").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "httpPort", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="httpsPort")
     def https_port(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
         '''
         :Property: httpsPort: Https port configuration
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]], jsii.get(self, "httpsPort"))
 
     @https_port.setter
     def https_port(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDomain, "https_port").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "httpsPort", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="httpsRedirect")
     def https_redirect(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: httpsRedirect: Https forced redirect configuration
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "httpsRedirect"))
 
     @https_redirect.setter
     def https_redirect(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDomain, "https_redirect").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "httpsRedirect", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="httpToUserIp")
     def http_to_user_ip(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: httpToUserIp: Http back to source
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "httpToUserIp"))
 
     @http_to_user_ip.setter
     def http_to_user_ip(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDomain, "http_to_user_ip").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "httpToUserIp", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="loadBalancing")
     def load_balancing(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: loadBalancing: Load balancing configuration
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "loadBalancing"))
 
     @load_balancing.setter
     def load_balancing(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDomain, "load_balancing").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "loadBalancing", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="logHeaders")
     def log_headers(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosDomain.LogHeadersProperty"]]]]:
         '''
         :Property: logHeaders: Domain traffic tagging
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosDomain.LogHeadersProperty"]]]], jsii.get(self, "logHeaders"))
 
     @log_headers.setter
     def log_headers(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosDomain.LogHeadersProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDomain, "log_headers").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "logHeaders", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="readTime")
     def read_time(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: readTime: Read connection timeout period
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "readTime"))
 
     @read_time.setter
     def read_time(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDomain, "read_time").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "readTime", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="resourceGroupId")
     def resource_group_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: resourceGroupId: Resource group Id
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "resourceGroupId"))
 
     @resource_group_id.setter
     def resource_group_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDomain, "resource_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "resourceGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="writeTime")
     def write_time(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: writeTime: Write connection timeout period
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "writeTime"))
 
     @write_time.setter
     def write_time(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDomain, "write_time").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "writeTime", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-waf.RosDomain.LogHeadersProperty",
         jsii_struct_bases=[],
         name_mapping={"k": "k", "v": "v"},
     )
@@ -1783,14 +1967,18 @@
             k: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             v: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param k: 
             :param v: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosDomain.LogHeadersProperty.__init__)
+                check_type(argname="argument k", value=k, expected_type=type_hints["k"])
+                check_type(argname="argument v", value=v, expected_type=type_hints["v"])
             self._values: typing.Dict[str, typing.Any] = {}
             if k is not None:
                 self._values["k"] = k
             if v is not None:
                 self._values["v"] = v
 
         @builtins.property
@@ -1832,88 +2020,103 @@
 ):
     '''A ROS template type:  ``ALIYUN::WAF::DomainConfig``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosDomainConfigProps",
+        props: typing.Union["RosDomainConfigProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::WAF::DomainConfig``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDomainConfig.__init__)
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
+            type_hints = typing.get_type_hints(RosDomainConfig._render_properties)
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
     @jsii.member(jsii_name="attrCname")
     def attr_cname(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Cname: CNAME assigned by WAF instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCname"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrProtocolType")
     def attr_protocol_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ProtocolType: agreement type:0: indicates that the HTTP protocol is supported.1: indicates that the HTTPS protocol is supported.2: indicates that both HTTP and HTTPS protocols are supported.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrProtocolType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="domain")
     def domain(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: domain: Domain name.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "domain"))
 
     @domain.setter
     def domain(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDomainConfig, "domain").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "domain", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDomainConfig, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceId")
     def instance_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         instanceId: WAF instance ID.
         Description Interface You can view your current WAF instance ID by calling DescribePayInfo.
@@ -1921,17 +2124,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "instanceId"))
 
     @instance_id.setter
     def instance_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDomainConfig, "instance_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="isAccessProduct")
     def is_access_product(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         isAccessProduct: The domain before WAF is configured with seven agents (eg, high defense, CDN, etc.), the value of:
         0: none.
@@ -1940,17 +2146,20 @@
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "isAccessProduct"))
 
     @is_access_product.setter
     def is_access_product(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDomainConfig, "is_access_product").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "isAccessProduct", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="protocols")
     def protocols(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         protocols: The domain supports access protocols, values:
         http: expressed support for the HTTP protocol.
@@ -1960,17 +2169,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "protocols"))
 
     @protocols.setter
     def protocols(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDomainConfig, "protocols").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "protocols", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="httpPort")
     def http_port(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1980,17 +2192,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "httpPort"))
 
     @http_port.setter
     def http_port(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDomainConfig, "http_port").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "httpPort", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="httpsPort")
     def https_port(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2000,17 +2215,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "httpsPort"))
 
     @https_port.setter
     def https_port(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDomainConfig, "https_port").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "httpsPort", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="httpsRedirect")
     def https_redirect(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2022,17 +2240,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "httpsRedirect"))
 
     @https_redirect.setter
     def https_redirect(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDomainConfig, "https_redirect").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "httpsRedirect", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="httpToUserIp")
     def http_to_user_ip(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2044,17 +2265,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "httpToUserIp"))
 
     @http_to_user_ip.setter
     def http_to_user_ip(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDomainConfig, "http_to_user_ip").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "httpToUserIp", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="loadBalancing")
     def load_balancing(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2065,17 +2289,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "loadBalancing"))
 
     @load_balancing.setter
     def load_balancing(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDomainConfig, "load_balancing").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "loadBalancing", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="region")
     def region(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2086,17 +2313,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "region"))
 
     @region.setter
     def region(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDomainConfig, "region").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "region", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rsType")
     def rs_type(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2107,31 +2337,37 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "rsType"))
 
     @rs_type.setter
     def rs_type(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDomainConfig, "rs_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "rsType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="sourceIps")
     def source_ips(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: sourceIps: Source station IP, supports a plurality of specified IP. Example values: [ "1.1.1.1"].
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "sourceIps"))
 
     @source_ips.setter
     def source_ips(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDomainConfig, "source_ips").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "sourceIps", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-waf.RosDomainConfigProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -2177,14 +2413,28 @@
         :param https_redirect: 
         :param http_to_user_ip: 
         :param load_balancing: 
         :param region: 
         :param rs_type: 
         :param source_ips: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDomainConfigProps.__init__)
+            check_type(argname="argument domain", value=domain, expected_type=type_hints["domain"])
+            check_type(argname="argument instance_id", value=instance_id, expected_type=type_hints["instance_id"])
+            check_type(argname="argument is_access_product", value=is_access_product, expected_type=type_hints["is_access_product"])
+            check_type(argname="argument protocols", value=protocols, expected_type=type_hints["protocols"])
+            check_type(argname="argument http_port", value=http_port, expected_type=type_hints["http_port"])
+            check_type(argname="argument https_port", value=https_port, expected_type=type_hints["https_port"])
+            check_type(argname="argument https_redirect", value=https_redirect, expected_type=type_hints["https_redirect"])
+            check_type(argname="argument http_to_user_ip", value=http_to_user_ip, expected_type=type_hints["http_to_user_ip"])
+            check_type(argname="argument load_balancing", value=load_balancing, expected_type=type_hints["load_balancing"])
+            check_type(argname="argument region", value=region, expected_type=type_hints["region"])
+            check_type(argname="argument rs_type", value=rs_type, expected_type=type_hints["rs_type"])
+            check_type(argname="argument source_ips", value=source_ips, expected_type=type_hints["source_ips"])
         self._values: typing.Dict[str, typing.Any] = {
             "domain": domain,
             "instance_id": instance_id,
             "is_access_product": is_access_product,
             "protocols": protocols,
         }
         if http_port is not None:
@@ -2406,15 +2656,15 @@
         connection_time: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         http2_port: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
         http_port: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
         https_port: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
         https_redirect: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         http_to_user_ip: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         load_balancing: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        log_headers: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosDomain.LogHeadersProperty]]]] = None,
+        log_headers: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosDomain.LogHeadersProperty, typing.Dict[str, typing.Any]]]]]] = None,
         read_time: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         resource_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         write_time: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::WAF::Domain``.
 
         :param domain_name: 
@@ -2430,14 +2680,32 @@
         :param http_to_user_ip: 
         :param load_balancing: 
         :param log_headers: 
         :param read_time: 
         :param resource_group_id: 
         :param write_time: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDomainProps.__init__)
+            check_type(argname="argument domain_name", value=domain_name, expected_type=type_hints["domain_name"])
+            check_type(argname="argument instance_id", value=instance_id, expected_type=type_hints["instance_id"])
+            check_type(argname="argument is_access_product", value=is_access_product, expected_type=type_hints["is_access_product"])
+            check_type(argname="argument source_ips", value=source_ips, expected_type=type_hints["source_ips"])
+            check_type(argname="argument cluster_type", value=cluster_type, expected_type=type_hints["cluster_type"])
+            check_type(argname="argument connection_time", value=connection_time, expected_type=type_hints["connection_time"])
+            check_type(argname="argument http2_port", value=http2_port, expected_type=type_hints["http2_port"])
+            check_type(argname="argument http_port", value=http_port, expected_type=type_hints["http_port"])
+            check_type(argname="argument https_port", value=https_port, expected_type=type_hints["https_port"])
+            check_type(argname="argument https_redirect", value=https_redirect, expected_type=type_hints["https_redirect"])
+            check_type(argname="argument http_to_user_ip", value=http_to_user_ip, expected_type=type_hints["http_to_user_ip"])
+            check_type(argname="argument load_balancing", value=load_balancing, expected_type=type_hints["load_balancing"])
+            check_type(argname="argument log_headers", value=log_headers, expected_type=type_hints["log_headers"])
+            check_type(argname="argument read_time", value=read_time, expected_type=type_hints["read_time"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument write_time", value=write_time, expected_type=type_hints["write_time"])
         self._values: typing.Dict[str, typing.Any] = {
             "domain_name": domain_name,
             "instance_id": instance_id,
             "is_access_product": is_access_product,
             "source_ips": source_ips,
         }
         if cluster_type is not None:
@@ -2642,309 +2910,360 @@
 ):
     '''A ROS template type:  ``ALIYUN::WAF::Instance``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosInstanceProps",
+        props: typing.Union["RosInstanceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::WAF::Instance``.
 
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
     @jsii.member(jsii_name="attrEndDate")
     def attr_end_date(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: EndDate: Due date of the instance
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrEndDate"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInDebt")
     def attr_in_debt(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: InDebt: Instance is overdue
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInDebt"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceId")
     def attr_instance_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: InstanceId: Instance ID
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrRemainDay")
     def attr_remain_day(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: RemainDay: Number of available days for WAF Trial version
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRemainDay"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSubscriptionType")
     def attr_subscription_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: SubscriptionType: Subscription type of the instance
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSubscriptionType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTrial")
     def attr_trial(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Trial: Trial version
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTrial"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="bigScreen")
     def big_screen(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: bigScreen:
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "bigScreen"))
 
     @big_screen.setter
     def big_screen(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "big_screen").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "bigScreen", value)
 
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
     @jsii.member(jsii_name="exclusiveIpPackage")
     def exclusive_ip_package(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: exclusiveIpPackage:
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "exclusiveIpPackage"))
 
     @exclusive_ip_package.setter
     def exclusive_ip_package(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "exclusive_ip_package").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "exclusiveIpPackage", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="extBandwidth")
     def ext_bandwidth(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: extBandwidth:
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "extBandwidth"))
 
     @ext_bandwidth.setter
     def ext_bandwidth(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "ext_bandwidth").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "extBandwidth", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="extDomainPackage")
     def ext_domain_package(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: extDomainPackage:
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "extDomainPackage"))
 
     @ext_domain_package.setter
     def ext_domain_package(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "ext_domain_package").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "extDomainPackage", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="logStorage")
     def log_storage(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: logStorage:
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "logStorage"))
 
     @log_storage.setter
     def log_storage(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "log_storage").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "logStorage", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="logTime")
     def log_time(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: logTime:
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "logTime"))
 
     @log_time.setter
     def log_time(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "log_time").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "logTime", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="packageCode")
     def package_code(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: packageCode:
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "packageCode"))
 
     @package_code.setter
     def package_code(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "package_code").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "packageCode", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="prefessionalService")
     def prefessional_service(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: prefessionalService:
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "prefessionalService"))
 
     @prefessional_service.setter
     def prefessional_service(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "prefessional_service").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "prefessionalService", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="subscriptionType")
     def subscription_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: subscriptionType: Subscription type of the instance
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "subscriptionType"))
 
     @subscription_type.setter
     def subscription_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "subscription_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "subscriptionType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="wafLog")
     def waf_log(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: wafLog:
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "wafLog"))
 
     @waf_log.setter
     def waf_log(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "waf_log").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "wafLog", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="period")
     def period(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: period:
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "period"))
 
     @period.setter
     def period(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "period").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "period", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="renewalStatus")
     def renewal_status(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: renewalStatus:
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "renewalStatus"))
 
     @renewal_status.setter
     def renewal_status(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "renewal_status").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "renewalStatus", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="renewPeriod")
     def renew_period(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: renewPeriod:
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "renewPeriod"))
 
     @renew_period.setter
     def renew_period(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "renew_period").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "renewPeriod", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-waf.RosInstanceProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -2993,14 +3312,29 @@
         :param prefessional_service: 
         :param subscription_type: 
         :param waf_log: 
         :param period: 
         :param renewal_status: 
         :param renew_period: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosInstanceProps.__init__)
+            check_type(argname="argument big_screen", value=big_screen, expected_type=type_hints["big_screen"])
+            check_type(argname="argument exclusive_ip_package", value=exclusive_ip_package, expected_type=type_hints["exclusive_ip_package"])
+            check_type(argname="argument ext_bandwidth", value=ext_bandwidth, expected_type=type_hints["ext_bandwidth"])
+            check_type(argname="argument ext_domain_package", value=ext_domain_package, expected_type=type_hints["ext_domain_package"])
+            check_type(argname="argument log_storage", value=log_storage, expected_type=type_hints["log_storage"])
+            check_type(argname="argument log_time", value=log_time, expected_type=type_hints["log_time"])
+            check_type(argname="argument package_code", value=package_code, expected_type=type_hints["package_code"])
+            check_type(argname="argument prefessional_service", value=prefessional_service, expected_type=type_hints["prefessional_service"])
+            check_type(argname="argument subscription_type", value=subscription_type, expected_type=type_hints["subscription_type"])
+            check_type(argname="argument waf_log", value=waf_log, expected_type=type_hints["waf_log"])
+            check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+            check_type(argname="argument renewal_status", value=renewal_status, expected_type=type_hints["renewal_status"])
+            check_type(argname="argument renew_period", value=renew_period, expected_type=type_hints["renew_period"])
         self._values: typing.Dict[str, typing.Any] = {
             "big_screen": big_screen,
             "exclusive_ip_package": exclusive_ip_package,
             "ext_bandwidth": ext_bandwidth,
             "ext_domain_package": ext_domain_package,
             "log_storage": log_storage,
             "log_time": log_time,
@@ -3161,91 +3495,106 @@
 ):
     '''A ROS template type:  ``ALIYUN::WAF::LogServiceEnable``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosLogServiceEnableProps",
+        props: typing.Union["RosLogServiceEnableProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::WAF::LogServiceEnable``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosLogServiceEnable.__init__)
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
+            type_hints = typing.get_type_hints(RosLogServiceEnable._render_properties)
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
     @jsii.member(jsii_name="attrDomain")
     def attr_domain(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Domain: The domain name that is added to WAF.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDomain"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceId")
     def attr_instance_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute:
 
         InstanceId: The ID of the WAF instance.
         You can call the DescribeInstanceInfo operation to query the ID of the WAF instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="domain")
     def domain(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: domain: The domain name that is added to WAF.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "domain"))
 
     @domain.setter
     def domain(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLogServiceEnable, "domain").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "domain", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLogServiceEnable, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceId")
     def instance_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         instanceId: The ID of the WAF instance.
         You can call the DescribeInstanceInfo operation to query the ID of the WAF instance.
@@ -3253,14 +3602,17 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "instanceId"))
 
     @instance_id.setter
     def instance_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLogServiceEnable, "instance_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceId", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-waf.RosLogServiceEnableProps",
     jsii_struct_bases=[],
     name_mapping={"domain": "domain", "instance_id": "instanceId"},
@@ -3273,14 +3625,18 @@
         instance_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::WAF::LogServiceEnable``.
 
         :param domain: 
         :param instance_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosLogServiceEnableProps.__init__)
+            check_type(argname="argument domain", value=domain, expected_type=type_hints["domain"])
+            check_type(argname="argument instance_id", value=instance_id, expected_type=type_hints["instance_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "domain": domain,
             "instance_id": instance_id,
         }
 
     @builtins.property
     def domain(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -3322,73 +3678,88 @@
 ):
     '''A ROS template type:  ``ALIYUN::WAF::WafSwitch``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosWafSwitchProps",
+        props: typing.Union["RosWafSwitchProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::WAF::WafSwitch``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosWafSwitch.__init__)
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
+            type_hints = typing.get_type_hints(RosWafSwitch._render_properties)
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
     @jsii.member(jsii_name="domain")
     def domain(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: domain: Domain name.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "domain"))
 
     @domain.setter
     def domain(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosWafSwitch, "domain").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "domain", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         '''A factory method that creates a new instance of this class from an object containing the properties of this ROS resource.'''
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosWafSwitch, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceId")
     def instance_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         instanceId: WAF instance ID.
         Description Interface You can view your current WAF instance ID by calling DescribePayInfo.
@@ -3396,17 +3767,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "instanceId"))
 
     @instance_id.setter
     def instance_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosWafSwitch, "instance_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="serviceOn")
     def service_on(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         serviceOn: Web attack protection switch, the value of:
         0: closed.
@@ -3415,17 +3789,20 @@
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "serviceOn"))
 
     @service_on.setter
     def service_on(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosWafSwitch, "service_on").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "serviceOn", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="region")
     def region(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3436,14 +3813,17 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "region"))
 
     @region.setter
     def region(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosWafSwitch, "region").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "region", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-waf.RosWafSwitchProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -3465,14 +3845,20 @@
         '''Properties for defining a ``ALIYUN::WAF::WafSwitch``.
 
         :param domain: 
         :param instance_id: 
         :param service_on: 
         :param region: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosWafSwitchProps.__init__)
+            check_type(argname="argument domain", value=domain, expected_type=type_hints["domain"])
+            check_type(argname="argument instance_id", value=instance_id, expected_type=type_hints["instance_id"])
+            check_type(argname="argument service_on", value=service_on, expected_type=type_hints["service_on"])
+            check_type(argname="argument region", value=region, expected_type=type_hints["region"])
         self._values: typing.Dict[str, typing.Any] = {
             "domain": domain,
             "instance_id": instance_id,
             "service_on": service_on,
         }
         if region is not None:
             self._values["region"] = region
@@ -3544,28 +3930,34 @@
 ):
     '''A ROS resource type:  ``ALIYUN::WAF::WafSwitch``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "WafSwitchProps",
+        props: typing.Union["WafSwitchProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::WAF::WafSwitch``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(WafSwitch.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-waf.WafSwitchProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -3587,14 +3979,20 @@
         '''Properties for defining a ``ALIYUN::WAF::WafSwitch``.
 
         :param domain: Property domain: Domain name.
         :param instance_id: Property instanceId: WAF instance ID. Description Interface You can view your current WAF instance ID by calling DescribePayInfo.
         :param service_on: Property serviceOn: Web attack protection switch, the value of: 0: closed. 1: indicate on.
         :param region: Property region: Examples of areas where the WAF. Value: cn: China mainland (default) cn-hongkong: China HongKong and other overseas
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(WafSwitchProps.__init__)
+            check_type(argname="argument domain", value=domain, expected_type=type_hints["domain"])
+            check_type(argname="argument instance_id", value=instance_id, expected_type=type_hints["instance_id"])
+            check_type(argname="argument service_on", value=service_on, expected_type=type_hints["service_on"])
+            check_type(argname="argument region", value=region, expected_type=type_hints["region"])
         self._values: typing.Dict[str, typing.Any] = {
             "domain": domain,
             "instance_id": instance_id,
             "service_on": service_on,
         }
         if region is not None:
             self._values["region"] = region
```

### Comparing `ros-cdk-waf-1.0.8/src/ros_cdk_waf.egg-info/PKG-INFO` & `ros-cdk-waf-1.0.9/src/ros_cdk_waf.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-waf
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS WAF Construct Library
```

