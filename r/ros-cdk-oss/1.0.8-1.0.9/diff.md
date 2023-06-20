# Comparing `tmp/ros-cdk-oss-1.0.8.tar.gz` & `tmp/ros-cdk-oss-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-oss-1.0.8.tar", last modified: Thu Jul 14 02:39:58 2022, max compression
+gzip compressed data, was "dist/ros-cdk-oss-1.0.9.tar", last modified: Fri Sep 23 11:48:51 2022, max compression
```

## Comparing `ros-cdk-oss-1.0.8.tar` & `ros-cdk-oss-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:39:58.000000 ros-cdk-oss-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:39:58.000000 ros-cdk-oss-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:39:58.000000 ros-cdk-oss-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:39:58.000000 ros-cdk-oss-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:39:58.000000 ros-cdk-oss-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      179 2022-07-14 02:39:58.000000 ros-cdk-oss-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:39:58.000000 ros-cdk-oss-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:39:58.000000 ros-cdk-oss-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1794 2022-07-14 02:39:58.000000 ros-cdk-oss-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:39:58.000000 ros-cdk-oss-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:39:58.000000 ros-cdk-oss-1.0.8/src/ros_cdk_oss/
--rw-r--r--   0 root         (0) root         (0)    59923 2022-07-14 02:39:58.000000 ros-cdk-oss-1.0.8/src/ros_cdk_oss/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:39:58.000000 ros-cdk-oss-1.0.8/src/ros_cdk_oss/_jsii/
--rw-r--r--   0 root         (0) root         (0)      370 2022-07-14 02:39:58.000000 ros-cdk-oss-1.0.8/src/ros_cdk_oss/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44115 2022-07-14 02:39:58.000000 ros-cdk-oss-1.0.8/src/ros_cdk_oss/_jsii/ros-cdk-oss@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:39:58.000000 ros-cdk-oss-1.0.8/src/ros_cdk_oss/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:39:58.000000 ros-cdk-oss-1.0.8/src/ros_cdk_oss.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:39:58.000000 ros-cdk-oss-1.0.8/src/ros_cdk_oss.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      400 2022-07-14 02:39:58.000000 ros-cdk-oss-1.0.8/src/ros_cdk_oss.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:39:58.000000 ros-cdk-oss-1.0.8/src/ros_cdk_oss.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:39:58.000000 ros-cdk-oss-1.0.8/src/ros_cdk_oss.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-07-14 02:39:58.000000 ros-cdk-oss-1.0.8/src/ros_cdk_oss.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:48:51.000000 ros-cdk-oss-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 11:48:51.000000 ros-cdk-oss-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 11:48:51.000000 ros-cdk-oss-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 11:48:51.000000 ros-cdk-oss-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 11:48:51.000000 ros-cdk-oss-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      179 2022-09-23 11:48:51.000000 ros-cdk-oss-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 11:48:51.000000 ros-cdk-oss-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 11:48:51.000000 ros-cdk-oss-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1823 2022-09-23 11:48:51.000000 ros-cdk-oss-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:48:51.000000 ros-cdk-oss-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:48:51.000000 ros-cdk-oss-1.0.9/src/ros_cdk_oss/
+-rw-r--r--   0 root         (0) root         (0)    71922 2022-09-23 11:48:51.000000 ros-cdk-oss-1.0.9/src/ros_cdk_oss/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:48:51.000000 ros-cdk-oss-1.0.9/src/ros_cdk_oss/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      404 2022-09-23 11:48:51.000000 ros-cdk-oss-1.0.9/src/ros_cdk_oss/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44185 2022-09-23 11:48:51.000000 ros-cdk-oss-1.0.9/src/ros_cdk_oss/_jsii/ros-cdk-oss@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:48:51.000000 ros-cdk-oss-1.0.9/src/ros_cdk_oss/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:48:51.000000 ros-cdk-oss-1.0.9/src/ros_cdk_oss.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 11:48:51.000000 ros-cdk-oss-1.0.9/src/ros_cdk_oss.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      400 2022-09-23 11:48:51.000000 ros-cdk-oss-1.0.9/src/ros_cdk_oss.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:48:51.000000 ros-cdk-oss-1.0.9/src/ros_cdk_oss.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 11:48:51.000000 ros-cdk-oss-1.0.9/src/ros_cdk_oss.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-09-23 11:48:51.000000 ros-cdk-oss-1.0.9/src/ros_cdk_oss.egg-info/top_level.txt
```

### Comparing `ros-cdk-oss-1.0.8/LICENSE` & `ros-cdk-oss-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-oss-1.0.8/PKG-INFO` & `ros-cdk-oss-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-oss
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS OSS Construct Library
```

### Comparing `ros-cdk-oss-1.0.8/setup.py` & `ros-cdk-oss-1.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-oss",
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
         "ros_cdk_oss",
         "ros_cdk_oss._jsii"
     ],
     "package_data": {
         "ros_cdk_oss._jsii": [
-            "ros-cdk-oss@1.0.8.jsii.tgz"
+            "ros-cdk-oss@1.0.9.jsii.tgz"
         ],
         "ros_cdk_oss": [
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

### Comparing `ros-cdk-oss-1.0.8/src/ros_cdk_oss/__init__.py` & `ros-cdk-oss-1.0.9/src/ros_cdk_oss/__init__.py`

 * *Files 22% similar despite different names*

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
 
 
 class Bucket(
     ros_cdk_core.Resource,
@@ -29,43 +31,49 @@
 ):
     '''A ROS resource type:  ``ALIYUN::OSS::Bucket``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "BucketProps",
+        props: typing.Union["BucketProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::OSS::Bucket``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Bucket.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDomainName")
     def attr_domain_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute DomainName: The public DNS name of the specified bucket.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDomainName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInternalDomainName")
     def attr_internal_domain_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute InternalDomainName: The internal DNS name of the specified bucket.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInternalDomainName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrName")
     def attr_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute Name: The name of Bucket.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrName"))
 
 
 @jsii.data_type(
@@ -88,24 +96,24 @@
 )
 class BucketProps:
     def __init__(
         self,
         *,
         bucket_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         access_control: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        cors_configuration: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosBucket.CORSConfigurationProperty"]] = None,
+        cors_configuration: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosBucket.CORSConfigurationProperty", typing.Dict[str, typing.Any]]]] = None,
         deletion_force: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
-        lifecycle_configuration: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosBucket.LifecycleConfigurationProperty"]] = None,
-        logging_configuration: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosBucket.LoggingConfigurationProperty"]] = None,
+        lifecycle_configuration: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosBucket.LifecycleConfigurationProperty", typing.Dict[str, typing.Any]]]] = None,
+        logging_configuration: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosBucket.LoggingConfigurationProperty", typing.Dict[str, typing.Any]]]] = None,
         policy: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]] = None,
-        referer_configuration: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosBucket.RefererConfigurationProperty"]] = None,
-        server_side_encryption_configuration: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosBucket.ServerSideEncryptionConfigurationProperty"]] = None,
+        referer_configuration: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosBucket.RefererConfigurationProperty", typing.Dict[str, typing.Any]]]] = None,
+        server_side_encryption_configuration: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosBucket.ServerSideEncryptionConfigurationProperty", typing.Dict[str, typing.Any]]]] = None,
         storage_class: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         tags: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
-        website_configuration: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosBucket.WebsiteConfigurationProperty"]] = None,
+        website_configuration: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosBucket.WebsiteConfigurationProperty", typing.Dict[str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::OSS::Bucket``.
 
         :param bucket_name: Property bucketName: bucket name.
         :param access_control: Property accessControl: The access control list.
         :param cors_configuration: Property corsConfiguration: Rules that define cross-origin resource sharing of objects in this bucket.
         :param deletion_force: Property deletionForce: Whether force delete the relative objects in the bucket. Default value is false.
@@ -114,14 +122,28 @@
         :param policy: Property policy: Bucket policy.
         :param referer_configuration: Property refererConfiguration: undefined.
         :param server_side_encryption_configuration: Property serverSideEncryptionConfiguration: Specifies the bucket used to store the server-side encryption rule.
         :param storage_class: Property storageClass: Specifies the storage class of the bucket. Default is "Standard".
         :param tags: Property tags: Bucket tags in k-v pairs format.
         :param website_configuration: Property websiteConfiguration: The properties of website config.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(BucketProps.__init__)
+            check_type(argname="argument bucket_name", value=bucket_name, expected_type=type_hints["bucket_name"])
+            check_type(argname="argument access_control", value=access_control, expected_type=type_hints["access_control"])
+            check_type(argname="argument cors_configuration", value=cors_configuration, expected_type=type_hints["cors_configuration"])
+            check_type(argname="argument deletion_force", value=deletion_force, expected_type=type_hints["deletion_force"])
+            check_type(argname="argument lifecycle_configuration", value=lifecycle_configuration, expected_type=type_hints["lifecycle_configuration"])
+            check_type(argname="argument logging_configuration", value=logging_configuration, expected_type=type_hints["logging_configuration"])
+            check_type(argname="argument policy", value=policy, expected_type=type_hints["policy"])
+            check_type(argname="argument referer_configuration", value=referer_configuration, expected_type=type_hints["referer_configuration"])
+            check_type(argname="argument server_side_encryption_configuration", value=server_side_encryption_configuration, expected_type=type_hints["server_side_encryption_configuration"])
+            check_type(argname="argument storage_class", value=storage_class, expected_type=type_hints["storage_class"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument website_configuration", value=website_configuration, expected_type=type_hints["website_configuration"])
         self._values: typing.Dict[str, typing.Any] = {
             "bucket_name": bucket_name,
         }
         if access_control is not None:
             self._values["access_control"] = access_control
         if cors_configuration is not None:
             self._values["cors_configuration"] = cors_configuration
@@ -262,278 +284,326 @@
 ):
     '''A ROS template type:  ``ALIYUN::OSS::Bucket``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosBucketProps",
+        props: typing.Union["RosBucketProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::OSS::Bucket``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosBucket.__init__)
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
+            type_hints = typing.get_type_hints(RosBucket._render_properties)
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
     @jsii.member(jsii_name="attrDomainName")
     def attr_domain_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DomainName: The public DNS name of the specified bucket.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDomainName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInternalDomainName")
     def attr_internal_domain_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: InternalDomainName: The internal DNS name of the specified bucket.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInternalDomainName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrName")
     def attr_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Name: The name of Bucket
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="bucketName")
     def bucket_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: bucketName: bucket name.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "bucketName"))
 
     @bucket_name.setter
     def bucket_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosBucket, "bucket_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "bucketName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosBucket, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="accessControl")
     def access_control(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: accessControl: The access control list.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "accessControl"))
 
     @access_control.setter
     def access_control(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosBucket, "access_control").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "accessControl", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="corsConfiguration")
     def cors_configuration(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosBucket.CORSConfigurationProperty"]]:
         '''
         :Property: corsConfiguration: Rules that define cross-origin resource sharing of objects in this bucket.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosBucket.CORSConfigurationProperty"]], jsii.get(self, "corsConfiguration"))
 
     @cors_configuration.setter
     def cors_configuration(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosBucket.CORSConfigurationProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosBucket, "cors_configuration").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "corsConfiguration", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="deletionForce")
     def deletion_force(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: deletionForce: Whether force delete the relative objects in the bucket. Default value is false.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "deletionForce"))
 
     @deletion_force.setter
     def deletion_force(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosBucket, "deletion_force").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "deletionForce", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="lifecycleConfiguration")
     def lifecycle_configuration(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosBucket.LifecycleConfigurationProperty"]]:
         '''
         :Property: lifecycleConfiguration: Rules that define how oss bucket manages objects during their lifetime.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosBucket.LifecycleConfigurationProperty"]], jsii.get(self, "lifecycleConfiguration"))
 
     @lifecycle_configuration.setter
     def lifecycle_configuration(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosBucket.LifecycleConfigurationProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosBucket, "lifecycle_configuration").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "lifecycleConfiguration", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="loggingConfiguration")
     def logging_configuration(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosBucket.LoggingConfigurationProperty"]]:
         '''
         :Property: loggingConfiguration: Settings that defines where logs are stored.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosBucket.LoggingConfigurationProperty"]], jsii.get(self, "loggingConfiguration"))
 
     @logging_configuration.setter
     def logging_configuration(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosBucket.LoggingConfigurationProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosBucket, "logging_configuration").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "loggingConfiguration", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="policy")
     def policy(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]]:
         '''
         :Property: policy: Bucket policy
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]], jsii.get(self, "policy"))
 
     @policy.setter
     def policy(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosBucket, "policy").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "policy", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="refererConfiguration")
     def referer_configuration(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosBucket.RefererConfigurationProperty"]]:
         '''
         :Property: refererConfiguration: undefined
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosBucket.RefererConfigurationProperty"]], jsii.get(self, "refererConfiguration"))
 
     @referer_configuration.setter
     def referer_configuration(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosBucket.RefererConfigurationProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosBucket, "referer_configuration").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "refererConfiguration", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="serverSideEncryptionConfiguration")
     def server_side_encryption_configuration(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosBucket.ServerSideEncryptionConfigurationProperty"]]:
         '''
         :Property: serverSideEncryptionConfiguration: Specifies the bucket used to store the server-side encryption rule.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosBucket.ServerSideEncryptionConfigurationProperty"]], jsii.get(self, "serverSideEncryptionConfiguration"))
 
     @server_side_encryption_configuration.setter
     def server_side_encryption_configuration(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosBucket.ServerSideEncryptionConfigurationProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosBucket, "server_side_encryption_configuration").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "serverSideEncryptionConfiguration", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="storageClass")
     def storage_class(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: storageClass: Specifies the storage class of the bucket. Default is "Standard".
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "storageClass"))
 
     @storage_class.setter
     def storage_class(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosBucket, "storage_class").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "storageClass", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tags")
     def tags(self) -> typing.Optional[typing.Mapping[builtins.str, typing.Any]]:
         '''
         :Property: tags: Bucket tags in k-v pairs format.
         '''
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, typing.Any]], jsii.get(self, "tags"))
 
     @tags.setter
     def tags(
         self,
         value: typing.Optional[typing.Mapping[builtins.str, typing.Any]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosBucket, "tags").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tags", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="websiteConfiguration")
     def website_configuration(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosBucket.WebsiteConfigurationProperty"]]:
         '''
         :Property: websiteConfiguration: The properties of website config.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosBucket.WebsiteConfigurationProperty"]], jsii.get(self, "websiteConfiguration"))
 
     @website_configuration.setter
     def website_configuration(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosBucket.WebsiteConfigurationProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosBucket, "website_configuration").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "websiteConfiguration", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-oss.RosBucket.AbortMultipartUploadProperty",
         jsii_struct_bases=[],
         name_mapping={"created_before_date": "createdBeforeDate", "days": "days"},
     )
@@ -544,14 +614,18 @@
             created_before_date: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             days: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param created_before_date: 
             :param days: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosBucket.AbortMultipartUploadProperty.__init__)
+                check_type(argname="argument created_before_date", value=created_before_date, expected_type=type_hints["created_before_date"])
+                check_type(argname="argument days", value=days, expected_type=type_hints["days"])
             self._values: typing.Dict[str, typing.Any] = {}
             if created_before_date is not None:
                 self._values["created_before_date"] = created_before_date
             if days is not None:
                 self._values["days"] = days
 
         @builtins.property
@@ -590,19 +664,22 @@
         jsii_struct_bases=[],
         name_mapping={"cors_rule": "corsRule"},
     )
     class CORSConfigurationProperty:
         def __init__(
             self,
             *,
-            cors_rule: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosBucket.CORSRuleProperty"]]]] = None,
+            cors_rule: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosBucket.CORSRuleProperty", typing.Dict[str, typing.Any]]]]]] = None,
         ) -> None:
             '''
             :param cors_rule: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosBucket.CORSConfigurationProperty.__init__)
+                check_type(argname="argument cors_rule", value=cors_rule, expected_type=type_hints["cors_rule"])
             self._values: typing.Dict[str, typing.Any] = {}
             if cors_rule is not None:
                 self._values["cors_rule"] = cors_rule
 
         @builtins.property
         def cors_rule(
             self,
@@ -648,14 +725,21 @@
             '''
             :param allowed_header: 
             :param allowed_method: 
             :param allowed_origin: 
             :param expose_header: 
             :param max_age_seconds: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosBucket.CORSRuleProperty.__init__)
+                check_type(argname="argument allowed_header", value=allowed_header, expected_type=type_hints["allowed_header"])
+                check_type(argname="argument allowed_method", value=allowed_method, expected_type=type_hints["allowed_method"])
+                check_type(argname="argument allowed_origin", value=allowed_origin, expected_type=type_hints["allowed_origin"])
+                check_type(argname="argument expose_header", value=expose_header, expected_type=type_hints["expose_header"])
+                check_type(argname="argument max_age_seconds", value=max_age_seconds, expected_type=type_hints["max_age_seconds"])
             self._values: typing.Dict[str, typing.Any] = {}
             if allowed_header is not None:
                 self._values["allowed_header"] = allowed_header
             if allowed_method is not None:
                 self._values["allowed_method"] = allowed_method
             if allowed_origin is not None:
                 self._values["allowed_origin"] = allowed_origin
@@ -737,14 +821,18 @@
             created_before_date: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             days: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param created_before_date: 
             :param days: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosBucket.ExpirationProperty.__init__)
+                check_type(argname="argument created_before_date", value=created_before_date, expected_type=type_hints["created_before_date"])
+                check_type(argname="argument days", value=days, expected_type=type_hints["days"])
             self._values: typing.Dict[str, typing.Any] = {}
             if created_before_date is not None:
                 self._values["created_before_date"] = created_before_date
             if days is not None:
                 self._values["days"] = days
 
         @builtins.property
@@ -783,19 +871,22 @@
         jsii_struct_bases=[],
         name_mapping={"rule": "rule"},
     )
     class LifecycleConfigurationProperty:
         def __init__(
             self,
             *,
-            rule: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosBucket.RuleProperty"]]],
+            rule: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosBucket.RuleProperty", typing.Dict[str, typing.Any]]]]],
         ) -> None:
             '''
             :param rule: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosBucket.LifecycleConfigurationProperty.__init__)
+                check_type(argname="argument rule", value=rule, expected_type=type_hints["rule"])
             self._values: typing.Dict[str, typing.Any] = {
                 "rule": rule,
             }
 
         @builtins.property
         def rule(
             self,
@@ -833,14 +924,18 @@
             target_bucket: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             target_prefix: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param target_bucket: 
             :param target_prefix: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosBucket.LoggingConfigurationProperty.__init__)
+                check_type(argname="argument target_bucket", value=target_bucket, expected_type=type_hints["target_bucket"])
+                check_type(argname="argument target_prefix", value=target_prefix, expected_type=type_hints["target_prefix"])
             self._values: typing.Dict[str, typing.Any] = {}
             if target_bucket is not None:
                 self._values["target_bucket"] = target_bucket
             if target_prefix is not None:
                 self._values["target_prefix"] = target_prefix
 
         @builtins.property
@@ -889,14 +984,18 @@
             allow_empty_referer: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
             referer_list: typing.Optional[typing.Union[typing.Sequence[typing.Any], ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param allow_empty_referer: 
             :param referer_list: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosBucket.RefererConfigurationProperty.__init__)
+                check_type(argname="argument allow_empty_referer", value=allow_empty_referer, expected_type=type_hints["allow_empty_referer"])
+                check_type(argname="argument referer_list", value=referer_list, expected_type=type_hints["referer_list"])
             self._values: typing.Dict[str, typing.Any] = {}
             if allow_empty_referer is not None:
                 self._values["allow_empty_referer"] = allow_empty_referer
             if referer_list is not None:
                 self._values["referer_list"] = referer_list
 
         @builtins.property
@@ -942,26 +1041,33 @@
         },
     )
     class RuleProperty:
         def __init__(
             self,
             *,
             prefix: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-            abort_multipart_upload: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosBucket.AbortMultipartUploadProperty"]] = None,
-            expiration: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosBucket.ExpirationProperty"]] = None,
+            abort_multipart_upload: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosBucket.AbortMultipartUploadProperty", typing.Dict[str, typing.Any]]]] = None,
+            expiration: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosBucket.ExpirationProperty", typing.Dict[str, typing.Any]]]] = None,
             id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             status: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param prefix: 
             :param abort_multipart_upload: 
             :param expiration: 
             :param id: 
             :param status: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosBucket.RuleProperty.__init__)
+                check_type(argname="argument prefix", value=prefix, expected_type=type_hints["prefix"])
+                check_type(argname="argument abort_multipart_upload", value=abort_multipart_upload, expected_type=type_hints["abort_multipart_upload"])
+                check_type(argname="argument expiration", value=expiration, expected_type=type_hints["expiration"])
+                check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+                check_type(argname="argument status", value=status, expected_type=type_hints["status"])
             self._values: typing.Dict[str, typing.Any] = {
                 "prefix": prefix,
             }
             if abort_multipart_upload is not None:
                 self._values["abort_multipart_upload"] = abort_multipart_upload
             if expiration is not None:
                 self._values["expiration"] = expiration
@@ -1045,14 +1151,18 @@
             sse_algorithm: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             kms_master_key_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param sse_algorithm: 
             :param kms_master_key_id: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosBucket.ServerSideEncryptionConfigurationProperty.__init__)
+                check_type(argname="argument sse_algorithm", value=sse_algorithm, expected_type=type_hints["sse_algorithm"])
+                check_type(argname="argument kms_master_key_id", value=kms_master_key_id, expected_type=type_hints["kms_master_key_id"])
             self._values: typing.Dict[str, typing.Any] = {
                 "sse_algorithm": sse_algorithm,
             }
             if kms_master_key_id is not None:
                 self._values["kms_master_key_id"] = kms_master_key_id
 
         @builtins.property
@@ -1100,14 +1210,18 @@
             error_document: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             index_document: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param error_document: 
             :param index_document: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosBucket.WebsiteConfigurationProperty.__init__)
+                check_type(argname="argument error_document", value=error_document, expected_type=type_hints["error_document"])
+                check_type(argname="argument index_document", value=index_document, expected_type=type_hints["index_document"])
             self._values: typing.Dict[str, typing.Any] = {}
             if error_document is not None:
                 self._values["error_document"] = error_document
             if index_document is not None:
                 self._values["index_document"] = index_document
 
         @builtins.property
@@ -1162,24 +1276,24 @@
 )
 class RosBucketProps:
     def __init__(
         self,
         *,
         bucket_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         access_control: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        cors_configuration: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosBucket.CORSConfigurationProperty]] = None,
+        cors_configuration: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosBucket.CORSConfigurationProperty, typing.Dict[str, typing.Any]]]] = None,
         deletion_force: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
-        lifecycle_configuration: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosBucket.LifecycleConfigurationProperty]] = None,
-        logging_configuration: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosBucket.LoggingConfigurationProperty]] = None,
+        lifecycle_configuration: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosBucket.LifecycleConfigurationProperty, typing.Dict[str, typing.Any]]]] = None,
+        logging_configuration: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosBucket.LoggingConfigurationProperty, typing.Dict[str, typing.Any]]]] = None,
         policy: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]] = None,
-        referer_configuration: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosBucket.RefererConfigurationProperty]] = None,
-        server_side_encryption_configuration: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosBucket.ServerSideEncryptionConfigurationProperty]] = None,
+        referer_configuration: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosBucket.RefererConfigurationProperty, typing.Dict[str, typing.Any]]]] = None,
+        server_side_encryption_configuration: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosBucket.ServerSideEncryptionConfigurationProperty, typing.Dict[str, typing.Any]]]] = None,
         storage_class: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         tags: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
-        website_configuration: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosBucket.WebsiteConfigurationProperty]] = None,
+        website_configuration: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosBucket.WebsiteConfigurationProperty, typing.Dict[str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::OSS::Bucket``.
 
         :param bucket_name: 
         :param access_control: 
         :param cors_configuration: 
         :param deletion_force: 
@@ -1188,14 +1302,28 @@
         :param policy: 
         :param referer_configuration: 
         :param server_side_encryption_configuration: 
         :param storage_class: 
         :param tags: 
         :param website_configuration: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosBucketProps.__init__)
+            check_type(argname="argument bucket_name", value=bucket_name, expected_type=type_hints["bucket_name"])
+            check_type(argname="argument access_control", value=access_control, expected_type=type_hints["access_control"])
+            check_type(argname="argument cors_configuration", value=cors_configuration, expected_type=type_hints["cors_configuration"])
+            check_type(argname="argument deletion_force", value=deletion_force, expected_type=type_hints["deletion_force"])
+            check_type(argname="argument lifecycle_configuration", value=lifecycle_configuration, expected_type=type_hints["lifecycle_configuration"])
+            check_type(argname="argument logging_configuration", value=logging_configuration, expected_type=type_hints["logging_configuration"])
+            check_type(argname="argument policy", value=policy, expected_type=type_hints["policy"])
+            check_type(argname="argument referer_configuration", value=referer_configuration, expected_type=type_hints["referer_configuration"])
+            check_type(argname="argument server_side_encryption_configuration", value=server_side_encryption_configuration, expected_type=type_hints["server_side_encryption_configuration"])
+            check_type(argname="argument storage_class", value=storage_class, expected_type=type_hints["storage_class"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument website_configuration", value=website_configuration, expected_type=type_hints["website_configuration"])
         self._values: typing.Dict[str, typing.Any] = {
             "bucket_name": bucket_name,
         }
         if access_control is not None:
             self._values["access_control"] = access_control
         if cors_configuration is not None:
             self._values["cors_configuration"] = cors_configuration
```

### Comparing `ros-cdk-oss-1.0.8/src/ros_cdk_oss.egg-info/PKG-INFO` & `ros-cdk-oss-1.0.9/src/ros_cdk_oss.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-oss
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS OSS Construct Library
```

