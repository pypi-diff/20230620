# Comparing `tmp/ros-cdk-cas-1.0.8.tar.gz` & `tmp/ros-cdk-cas-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-cas-1.0.8.tar", last modified: Thu Jul 14 02:19:47 2022, max compression
+gzip compressed data, was "dist/ros-cdk-cas-1.0.9.tar", last modified: Fri Sep 23 12:22:31 2022, max compression
```

## Comparing `ros-cdk-cas-1.0.8.tar` & `ros-cdk-cas-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:19:47.000000 ros-cdk-cas-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:19:47.000000 ros-cdk-cas-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:19:47.000000 ros-cdk-cas-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:19:47.000000 ros-cdk-cas-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:19:47.000000 ros-cdk-cas-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      179 2022-07-14 02:19:47.000000 ros-cdk-cas-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:19:47.000000 ros-cdk-cas-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:19:47.000000 ros-cdk-cas-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1794 2022-07-14 02:19:47.000000 ros-cdk-cas-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:19:47.000000 ros-cdk-cas-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:19:47.000000 ros-cdk-cas-1.0.8/src/ros_cdk_cas/
--rw-r--r--   0 root         (0) root         (0)    14657 2022-07-14 02:19:47.000000 ros-cdk-cas-1.0.8/src/ros_cdk_cas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:19:47.000000 ros-cdk-cas-1.0.8/src/ros_cdk_cas/_jsii/
--rw-r--r--   0 root         (0) root         (0)      370 2022-07-14 02:19:47.000000 ros-cdk-cas-1.0.8/src/ros_cdk_cas/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29544 2022-07-14 02:19:47.000000 ros-cdk-cas-1.0.8/src/ros_cdk_cas/_jsii/ros-cdk-cas@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:19:47.000000 ros-cdk-cas-1.0.8/src/ros_cdk_cas/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:19:47.000000 ros-cdk-cas-1.0.8/src/ros_cdk_cas.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:19:47.000000 ros-cdk-cas-1.0.8/src/ros_cdk_cas.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      400 2022-07-14 02:19:47.000000 ros-cdk-cas-1.0.8/src/ros_cdk_cas.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:19:47.000000 ros-cdk-cas-1.0.8/src/ros_cdk_cas.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:19:47.000000 ros-cdk-cas-1.0.8/src/ros_cdk_cas.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-07-14 02:19:47.000000 ros-cdk-cas-1.0.8/src/ros_cdk_cas.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:22:31.000000 ros-cdk-cas-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 12:22:30.000000 ros-cdk-cas-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 12:22:30.000000 ros-cdk-cas-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 12:22:30.000000 ros-cdk-cas-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 12:22:31.000000 ros-cdk-cas-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      179 2022-09-23 12:22:30.000000 ros-cdk-cas-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 12:22:30.000000 ros-cdk-cas-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 12:22:31.000000 ros-cdk-cas-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1823 2022-09-23 12:22:30.000000 ros-cdk-cas-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:22:31.000000 ros-cdk-cas-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:22:31.000000 ros-cdk-cas-1.0.9/src/ros_cdk_cas/
+-rw-r--r--   0 root         (0) root         (0)    18311 2022-09-23 12:22:30.000000 ros-cdk-cas-1.0.9/src/ros_cdk_cas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:22:31.000000 ros-cdk-cas-1.0.9/src/ros_cdk_cas/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      404 2022-09-23 12:22:30.000000 ros-cdk-cas-1.0.9/src/ros_cdk_cas/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29608 2022-09-23 12:22:30.000000 ros-cdk-cas-1.0.9/src/ros_cdk_cas/_jsii/ros-cdk-cas@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 12:22:30.000000 ros-cdk-cas-1.0.9/src/ros_cdk_cas/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:22:31.000000 ros-cdk-cas-1.0.9/src/ros_cdk_cas.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 12:22:30.000000 ros-cdk-cas-1.0.9/src/ros_cdk_cas.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      400 2022-09-23 12:22:30.000000 ros-cdk-cas-1.0.9/src/ros_cdk_cas.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 12:22:30.000000 ros-cdk-cas-1.0.9/src/ros_cdk_cas.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 12:22:30.000000 ros-cdk-cas-1.0.9/src/ros_cdk_cas.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-09-23 12:22:30.000000 ros-cdk-cas-1.0.9/src/ros_cdk_cas.egg-info/top_level.txt
```

### Comparing `ros-cdk-cas-1.0.8/LICENSE` & `ros-cdk-cas-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-cas-1.0.8/PKG-INFO` & `ros-cdk-cas-1.0.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-cas
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS CAS Construct Library
```

### Comparing `ros-cdk-cas-1.0.8/setup.py` & `ros-cdk-cas-1.0.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-cas",
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
         "ros_cdk_cas",
         "ros_cdk_cas._jsii"
     ],
     "package_data": {
         "ros_cdk_cas._jsii": [
-            "ros-cdk-cas@1.0.8.jsii.tgz"
+            "ros-cdk-cas@1.0.9.jsii.tgz"
         ],
         "ros_cdk_cas": [
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

### Comparing `ros-cdk-cas-1.0.8/src/ros_cdk_cas/__init__.py` & `ros-cdk-cas-1.0.9/src/ros_cdk_cas/__init__.py`

 * *Files 18% similar despite different names*

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
 
 
 class Certificate(
     ros_cdk_core.Resource,
@@ -29,31 +31,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::CAS::Certificate``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "CertificateProps",
+        props: typing.Union["CertificateProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::CAS::Certificate``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Certificate.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCertId")
     def attr_cert_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute CertId: Certificate ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCertId"))
 
 
 @jsii.data_type(
@@ -81,14 +89,21 @@
 
         :param cert: Property cert: Specify the content of the certificate. To use the PEM encoding format.
         :param key: Property key: Specify the certificate private key content. To use the PEM encoding format.
         :param name: Property name: Custom certificate name. The certificate name under a user cannot be duplicated.
         :param lang: Property lang: Specifies the language type for requesting and receiving messages.
         :param source_ip: Property sourceIp: Specifies the source IP address of the request.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(CertificateProps.__init__)
+            check_type(argname="argument cert", value=cert, expected_type=type_hints["cert"])
+            check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument lang", value=lang, expected_type=type_hints["lang"])
+            check_type(argname="argument source_ip", value=source_ip, expected_type=type_hints["source_ip"])
         self._values: typing.Dict[str, typing.Any] = {
             "cert": cert,
             "key": key,
             "name": name,
         }
         if lang is not None:
             self._values["lang"] = lang
@@ -160,132 +175,159 @@
 ):
     '''A ROS template type:  ``ALIYUN::CAS::Certificate``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosCertificateProps",
+        props: typing.Union["RosCertificateProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::CAS::Certificate``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosCertificate.__init__)
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
+            type_hints = typing.get_type_hints(RosCertificate._render_properties)
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
     @jsii.member(jsii_name="attrCertId")
     def attr_cert_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: CertId: Certificate ID.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCertId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="cert")
     def cert(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: cert: Specify the content of the certificate. To use the PEM encoding format.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "cert"))
 
     @cert.setter
     def cert(self, value: typing.Union[builtins.str, ros_cdk_core.IResolvable]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCertificate, "cert").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "cert", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCertificate, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="key")
     def key(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: key: Specify the certificate private key content. To use the PEM encoding format.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "key"))
 
     @key.setter
     def key(self, value: typing.Union[builtins.str, ros_cdk_core.IResolvable]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCertificate, "key").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "key", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="name")
     def name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: name: Custom certificate name. The certificate name under a user cannot be duplicated.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "name"))
 
     @name.setter
     def name(self, value: typing.Union[builtins.str, ros_cdk_core.IResolvable]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCertificate, "name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "name", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="lang")
     def lang(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: lang: Specifies the language type for requesting and receiving messages.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "lang"))
 
     @lang.setter
     def lang(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCertificate, "lang").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "lang", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="sourceIp")
     def source_ip(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: sourceIp: Specifies the source IP address of the request.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "sourceIp"))
 
     @source_ip.setter
     def source_ip(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCertificate, "source_ip").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "sourceIp", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-cas.RosCertificateProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -310,14 +352,21 @@
 
         :param cert: 
         :param key: 
         :param name: 
         :param lang: 
         :param source_ip: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosCertificateProps.__init__)
+            check_type(argname="argument cert", value=cert, expected_type=type_hints["cert"])
+            check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument lang", value=lang, expected_type=type_hints["lang"])
+            check_type(argname="argument source_ip", value=source_ip, expected_type=type_hints["source_ip"])
         self._values: typing.Dict[str, typing.Any] = {
             "cert": cert,
             "key": key,
             "name": name,
         }
         if lang is not None:
             self._values["lang"] = lang
```

### Comparing `ros-cdk-cas-1.0.8/src/ros_cdk_cas.egg-info/PKG-INFO` & `ros-cdk-cas-1.0.9/src/ros_cdk_cas.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-cas
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS CAS Construct Library
```

