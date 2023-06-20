# Comparing `tmp/ros-cdk-sae-1.0.8.tar.gz` & `tmp/ros-cdk-sae-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-sae-1.0.8.tar", last modified: Thu Jul 14 02:29:18 2022, max compression
+gzip compressed data, was "dist/ros-cdk-sae-1.0.9.tar", last modified: Fri Sep 23 11:11:35 2022, max compression
```

## Comparing `ros-cdk-sae-1.0.8.tar` & `ros-cdk-sae-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:29:18.000000 ros-cdk-sae-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:29:18.000000 ros-cdk-sae-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:29:18.000000 ros-cdk-sae-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:29:18.000000 ros-cdk-sae-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:29:18.000000 ros-cdk-sae-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      179 2022-07-14 02:29:18.000000 ros-cdk-sae-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:29:18.000000 ros-cdk-sae-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:29:18.000000 ros-cdk-sae-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1794 2022-07-14 02:29:18.000000 ros-cdk-sae-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:29:18.000000 ros-cdk-sae-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:29:18.000000 ros-cdk-sae-1.0.8/src/ros_cdk_sae/
--rw-r--r--   0 root         (0) root         (0)   113051 2022-07-14 02:29:18.000000 ros-cdk-sae-1.0.8/src/ros_cdk_sae/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:29:18.000000 ros-cdk-sae-1.0.8/src/ros_cdk_sae/_jsii/
--rw-r--r--   0 root         (0) root         (0)      370 2022-07-14 02:29:18.000000 ros-cdk-sae-1.0.8/src/ros_cdk_sae/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    59828 2022-07-14 02:29:18.000000 ros-cdk-sae-1.0.8/src/ros_cdk_sae/_jsii/ros-cdk-sae@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:29:18.000000 ros-cdk-sae-1.0.8/src/ros_cdk_sae/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:29:18.000000 ros-cdk-sae-1.0.8/src/ros_cdk_sae.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:29:18.000000 ros-cdk-sae-1.0.8/src/ros_cdk_sae.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      400 2022-07-14 02:29:18.000000 ros-cdk-sae-1.0.8/src/ros_cdk_sae.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:29:18.000000 ros-cdk-sae-1.0.8/src/ros_cdk_sae.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:29:18.000000 ros-cdk-sae-1.0.8/src/ros_cdk_sae.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-07-14 02:29:18.000000 ros-cdk-sae-1.0.8/src/ros_cdk_sae.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:11:35.000000 ros-cdk-sae-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 11:11:34.000000 ros-cdk-sae-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 11:11:34.000000 ros-cdk-sae-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 11:11:34.000000 ros-cdk-sae-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 11:11:35.000000 ros-cdk-sae-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      179 2022-09-23 11:11:34.000000 ros-cdk-sae-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 11:11:34.000000 ros-cdk-sae-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 11:11:35.000000 ros-cdk-sae-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1823 2022-09-23 11:11:34.000000 ros-cdk-sae-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:11:35.000000 ros-cdk-sae-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:11:35.000000 ros-cdk-sae-1.0.9/src/ros_cdk_sae/
+-rw-r--r--   0 root         (0) root         (0)   136124 2022-09-23 11:11:34.000000 ros-cdk-sae-1.0.9/src/ros_cdk_sae/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:11:35.000000 ros-cdk-sae-1.0.9/src/ros_cdk_sae/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      404 2022-09-23 11:11:34.000000 ros-cdk-sae-1.0.9/src/ros_cdk_sae/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    59887 2022-09-23 11:11:34.000000 ros-cdk-sae-1.0.9/src/ros_cdk_sae/_jsii/ros-cdk-sae@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:11:34.000000 ros-cdk-sae-1.0.9/src/ros_cdk_sae/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:11:35.000000 ros-cdk-sae-1.0.9/src/ros_cdk_sae.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 11:11:35.000000 ros-cdk-sae-1.0.9/src/ros_cdk_sae.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      400 2022-09-23 11:11:35.000000 ros-cdk-sae-1.0.9/src/ros_cdk_sae.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:11:35.000000 ros-cdk-sae-1.0.9/src/ros_cdk_sae.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 11:11:35.000000 ros-cdk-sae-1.0.9/src/ros_cdk_sae.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-09-23 11:11:35.000000 ros-cdk-sae-1.0.9/src/ros_cdk_sae.egg-info/top_level.txt
```

### Comparing `ros-cdk-sae-1.0.8/LICENSE` & `ros-cdk-sae-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-sae-1.0.8/PKG-INFO` & `ros-cdk-sae-1.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-sae
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS SAE Construct Library
```

### Comparing `ros-cdk-sae-1.0.8/setup.py` & `ros-cdk-sae-1.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-sae",
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
         "ros_cdk_sae",
         "ros_cdk_sae._jsii"
     ],
     "package_data": {
         "ros_cdk_sae._jsii": [
-            "ros-cdk-sae@1.0.8.jsii.tgz"
+            "ros-cdk-sae@1.0.9.jsii.tgz"
         ],
         "ros_cdk_sae": [
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

### Comparing `ros-cdk-sae-1.0.8/src/ros_cdk_sae/__init__.py` & `ros-cdk-sae-1.0.9/src/ros_cdk_sae/__init__.py`

 * *Files 24% similar despite different names*

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
 
 
 class Application(
     ros_cdk_core.Resource,
@@ -29,37 +31,43 @@
 ):
     '''A ROS resource type:  ``ALIYUN::SAE::Application``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "ApplicationProps",
+        props: typing.Union["ApplicationProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::SAE::Application``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Application.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAppId")
     def attr_app_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute AppId: Creating successful application ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAppId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrChangeOrderId")
     def attr_change_order_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ChangeOrderId: Return to release a single ID, used to query task execution status.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrChangeOrderId"))
 
 
 @jsii.data_type(
@@ -130,15 +138,15 @@
         package_url: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         package_version: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         post_start: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         pre_stop: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         readiness: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         security_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         sls_configs: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence["RosApplication.TagsProperty"]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union["RosApplication.TagsProperty", typing.Dict[str, typing.Any]]]] = None,
         timezone: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         vpc_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         v_switch_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         war_start_options: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         web_container: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::SAE::Application``.
@@ -174,14 +182,50 @@
         :param tags: Property tags: Tags to attach to application. Max support 20 tags to add during create application. Each tag with two properties Key and Value, and Key is required.
         :param timezone: Property timezone: Application time zone. Default Asia/Shanghai.
         :param vpc_id: Property vpcId: EDAS namespace corresponding VPC. In Serverless in a corresponding one of the VPC namespace only, and can not be modified. Serverless first created in the application name space will form a binding relationship. You may correspond to a plurality of namespaces VPC. Do not fill was VpcId namespace binding.
         :param v_switch_id: Property vSwitchId: Application examples where the elastic card virtual switch. The switch must be located above the VPC. The same switch with EDAS namespace binding relationship. Do not fill was VSwitchId namespace binding.
         :param war_start_options: Property warStartOptions: War Start the application package option. Apply the default startup command: java $ JAVA_OPTS $ CATALINA_OPTS -Options org.apache.catalina.startup.Bootstrap "$ @" start
         :param web_container: Property webContainer: Tomcat deployment of the package depends on the version. Mirroring not supported.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ApplicationProps.__init__)
+            check_type(argname="argument app_name", value=app_name, expected_type=type_hints["app_name"])
+            check_type(argname="argument cpu", value=cpu, expected_type=type_hints["cpu"])
+            check_type(argname="argument memory", value=memory, expected_type=type_hints["memory"])
+            check_type(argname="argument namespace_id", value=namespace_id, expected_type=type_hints["namespace_id"])
+            check_type(argname="argument package_type", value=package_type, expected_type=type_hints["package_type"])
+            check_type(argname="argument replicas", value=replicas, expected_type=type_hints["replicas"])
+            check_type(argname="argument app_description", value=app_description, expected_type=type_hints["app_description"])
+            check_type(argname="argument command", value=command, expected_type=type_hints["command"])
+            check_type(argname="argument command_args", value=command_args, expected_type=type_hints["command_args"])
+            check_type(argname="argument custom_host_alias", value=custom_host_alias, expected_type=type_hints["custom_host_alias"])
+            check_type(argname="argument deploy", value=deploy, expected_type=type_hints["deploy"])
+            check_type(argname="argument edas_container_version", value=edas_container_version, expected_type=type_hints["edas_container_version"])
+            check_type(argname="argument envs", value=envs, expected_type=type_hints["envs"])
+            check_type(argname="argument image_url", value=image_url, expected_type=type_hints["image_url"])
+            check_type(argname="argument jar_start_args", value=jar_start_args, expected_type=type_hints["jar_start_args"])
+            check_type(argname="argument jar_start_options", value=jar_start_options, expected_type=type_hints["jar_start_options"])
+            check_type(argname="argument jdk", value=jdk, expected_type=type_hints["jdk"])
+            check_type(argname="argument liveness", value=liveness, expected_type=type_hints["liveness"])
+            check_type(argname="argument mount_desc", value=mount_desc, expected_type=type_hints["mount_desc"])
+            check_type(argname="argument mount_host", value=mount_host, expected_type=type_hints["mount_host"])
+            check_type(argname="argument nas_id", value=nas_id, expected_type=type_hints["nas_id"])
+            check_type(argname="argument package_url", value=package_url, expected_type=type_hints["package_url"])
+            check_type(argname="argument package_version", value=package_version, expected_type=type_hints["package_version"])
+            check_type(argname="argument post_start", value=post_start, expected_type=type_hints["post_start"])
+            check_type(argname="argument pre_stop", value=pre_stop, expected_type=type_hints["pre_stop"])
+            check_type(argname="argument readiness", value=readiness, expected_type=type_hints["readiness"])
+            check_type(argname="argument security_group_id", value=security_group_id, expected_type=type_hints["security_group_id"])
+            check_type(argname="argument sls_configs", value=sls_configs, expected_type=type_hints["sls_configs"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument timezone", value=timezone, expected_type=type_hints["timezone"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
+            check_type(argname="argument war_start_options", value=war_start_options, expected_type=type_hints["war_start_options"])
+            check_type(argname="argument web_container", value=web_container, expected_type=type_hints["web_container"])
         self._values: typing.Dict[str, typing.Any] = {
             "app_name": app_name,
             "cpu": cpu,
             "memory": memory,
             "namespace_id": namespace_id,
             "package_type": package_type,
             "replicas": replicas,
@@ -604,31 +648,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::SAE::Namespace``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "NamespaceProps",
+        props: typing.Union["NamespaceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::SAE::Namespace``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Namespace.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrNamespaceId")
     def attr_namespace_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute NamespaceId: Namespace ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrNamespaceId"))
 
 
 @jsii.data_type(
@@ -650,14 +700,19 @@
     ) -> None:
         '''Properties for defining a ``ALIYUN::SAE::Namespace``.
 
         :param namespace_id: Property namespaceId: Namespace ID. Format: "regionId:logicalId" or "logicalId"
         :param namespace_name: Property namespaceName: Namespace name.
         :param namespace_description: Property namespaceDescription: Namespace description.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(NamespaceProps.__init__)
+            check_type(argname="argument namespace_id", value=namespace_id, expected_type=type_hints["namespace_id"])
+            check_type(argname="argument namespace_name", value=namespace_name, expected_type=type_hints["namespace_name"])
+            check_type(argname="argument namespace_description", value=namespace_description, expected_type=type_hints["namespace_description"])
         self._values: typing.Dict[str, typing.Any] = {
             "namespace_id": namespace_id,
             "namespace_name": namespace_name,
         }
         if namespace_description is not None:
             self._values["namespace_description"] = namespace_description
 
@@ -705,115 +760,136 @@
 ):
     '''A ROS template type:  ``ALIYUN::SAE::Application``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosApplicationProps",
+        props: typing.Union["RosApplicationProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::SAE::Application``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosApplication.__init__)
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
+            type_hints = typing.get_type_hints(RosApplication._render_properties)
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
     @jsii.member(jsii_name="attrAppId")
     def attr_app_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: AppId: Creating successful application ID.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAppId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrChangeOrderId")
     def attr_change_order_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ChangeOrderId: Return to release a single ID, used to query task execution status.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrChangeOrderId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="appName")
     def app_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: appName: Application Name. Allowed numbers, letters and underlined combinations thereof. We must begin with the letters, the maximum length of 36 characters.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "appName"))
 
     @app_name.setter
     def app_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApplication, "app_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "appName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="cpu")
     def cpu(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property: cpu: Each instance of the CPU required, in units of milli core, can not be zero. Currently only supports fixed specifications instance type.
         '''
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "cpu"))
 
     @cpu.setter
     def cpu(self, value: typing.Union[jsii.Number, ros_cdk_core.IResolvable]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApplication, "cpu").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "cpu", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApplication, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="memory")
     def memory(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property: memory: Each instance of the required memory, in units of MB, can not be zero. Currently only supports fixed specifications instance type.
         '''
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "memory"))
 
     @memory.setter
     def memory(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApplication, "memory").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "memory", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="namespaceId")
     def namespace_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         namespaceId: EDAS namespace corresponding to ID. Canada supports only the name of the scribe lowercase namespace must begin with a letter.
         Namespace can interface to obtain from DescribeNamespaceList.
@@ -821,183 +897,216 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "namespaceId"))
 
     @namespace_id.setter
     def namespace_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApplication, "namespace_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "namespaceId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="packageType")
     def package_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: packageType: Application package type. Support FatJar, War, Image.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "packageType"))
 
     @package_type.setter
     def package_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApplication, "package_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "packageType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="replicas")
     def replicas(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property: replicas: The initial number of instances.
         '''
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "replicas"))
 
     @replicas.setter
     def replicas(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApplication, "replicas").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "replicas", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="appDescription")
     def app_description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: appDescription: Application description. No more than 1024 characters.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "appDescription"))
 
     @app_description.setter
     def app_description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApplication, "app_description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "appDescription", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="command")
     def command(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: command: Mirroring the start command. The command object in memory executable container must be. For example: sleep. This command will cause the image to set the original startup command failure.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "command"))
 
     @command.setter
     def command(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApplication, "command").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "command", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="commandArgs")
     def command_args(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: commandArgs: Mirroring the start command parameters. Parameters required for the start-command. For example: [ "1d"]
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "commandArgs"))
 
     @command_args.setter
     def command_args(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApplication, "command_args").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "commandArgs", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="customHostAlias")
     def custom_host_alias(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: customHostAlias: Custom mapping host vessel. For example: [{ "hostName": "samplehost", "ip": "127.0.0.1"}]
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "customHostAlias"))
 
     @custom_host_alias.setter
     def custom_host_alias(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApplication, "custom_host_alias").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "customHostAlias", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="deploy")
     def deploy(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: deploy: Whether deployed immediately take effect, the default is false.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "deploy"))
 
     @deploy.setter
     def deploy(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApplication, "deploy").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "deploy", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="edasContainerVersion")
     def edas_container_version(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: edasContainerVersion: EDAS pandora runtime environment used by the application.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "edasContainerVersion"))
 
     @edas_container_version.setter
     def edas_container_version(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApplication, "edas_container_version").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "edasContainerVersion", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="envs")
     def envs(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: envs: Container environment variable parameters. For example: [{ "name": "envtmp", "value": "0"}]
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "envs"))
 
     @envs.setter
     def envs(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApplication, "envs").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "envs", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="imageUrl")
     def image_url(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: imageUrl: Mirroring address. Image only type of application can be configured to mirror address.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "imageUrl"))
 
     @image_url.setter
     def image_url(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApplication, "image_url").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "imageUrl", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="jarStartArgs")
     def jar_start_args(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1007,17 +1116,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "jarStartArgs"))
 
     @jar_start_args.setter
     def jar_start_args(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApplication, "jar_start_args").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "jarStartArgs", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="jarStartOptions")
     def jar_start_options(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1027,287 +1139,338 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "jarStartOptions"))
 
     @jar_start_options.setter
     def jar_start_options(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApplication, "jar_start_options").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "jarStartOptions", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="jdk")
     def jdk(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: jdk: Deployment of JDK version of the package depends on. Mirroring not supported.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "jdk"))
 
     @jdk.setter
     def jdk(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApplication, "jdk").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "jdk", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="liveness")
     def liveness(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: liveness: Container health check, health check fails container will be killed and recovery. Currently only supports mode command issued in the container. The columns: { "exec": { "command": [ "sleep", "5s"]}, "initialDelaySeconds": 10, "timeoutSeconds": 11}
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "liveness"))
 
     @liveness.setter
     def liveness(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApplication, "liveness").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "liveness", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="mountDesc")
     def mount_desc(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: mountDesc: Mount Description
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "mountDesc"))
 
     @mount_desc.setter
     def mount_desc(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApplication, "mount_desc").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "mountDesc", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="mountHost")
     def mount_host(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: mountHost: nas mount point in the application of vpc.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "mountHost"))
 
     @mount_host.setter
     def mount_host(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApplication, "mount_host").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "mountHost", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="nasId")
     def nas_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: nasId: Mount the NAS ID, you must be in the same region and cluster. It must be available to create a mount point limit, or switch on its mount point already in the VPC. If you do not fill, and there mountDescs field, the default will automatically purchase a NAS and mount it onto the switch within the VPC.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "nasId"))
 
     @nas_id.setter
     def nas_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApplication, "nas_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "nasId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="packageUrl")
     def package_url(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: packageUrl: Deployment packages address. Only FatJar War or the type of application can be configured to deploy packet address.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "packageUrl"))
 
     @package_url.setter
     def package_url(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApplication, "package_url").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "packageUrl", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="packageVersion")
     def package_version(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: packageVersion: The version number of the deployed package, War FatJar type required. Please customize it meaning.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "packageVersion"))
 
     @package_version.setter
     def package_version(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApplication, "package_version").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "packageVersion", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="postStart")
     def post_start(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: postStart: Executing the script, such as after starting the format: { "exec": { "command": "cat", "/ etc / group"}}
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "postStart"))
 
     @post_start.setter
     def post_start(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApplication, "post_start").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "postStart", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="preStop")
     def pre_stop(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: preStop: Script is executed before stopping the format as: { "exec": { "command": "cat", "/ etc / group"}}
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "preStop"))
 
     @pre_stop.setter
     def pre_stop(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApplication, "pre_stop").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "preStop", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="readiness")
     def readiness(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: readiness: Application launch status check, health check fails repeatedly container will be killed and restarted. Do not pass health check of the vessel will not have to enter SLB traffic. For example: { "exec": { "command": [ "sleep", "6s"]}, "initialDelaySeconds": 15, "timeoutSeconds": 12}
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "readiness"))
 
     @readiness.setter
     def readiness(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApplication, "readiness").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "readiness", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="securityGroupId")
     def security_group_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: securityGroupId: Security group ID.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "securityGroupId"))
 
     @security_group_id.setter
     def security_group_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApplication, "security_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "securityGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="slsConfigs")
     def sls_configs(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: slsConfigs: Log collection configuration file
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "slsConfigs"))
 
     @sls_configs.setter
     def sls_configs(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApplication, "sls_configs").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "slsConfigs", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tags")
     def tags(self) -> typing.Optional[typing.List["RosApplication.TagsProperty"]]:
         '''
         :Property: tags: Tags to attach to application. Max support 20 tags to add during create application. Each tag with two properties Key and Value, and Key is required.
         '''
         return typing.cast(typing.Optional[typing.List["RosApplication.TagsProperty"]], jsii.get(self, "tags"))
 
     @tags.setter
     def tags(
         self,
         value: typing.Optional[typing.List["RosApplication.TagsProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApplication, "tags").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tags", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="timezone")
     def timezone(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: timezone: Application time zone. Default Asia/Shanghai.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "timezone"))
 
     @timezone.setter
     def timezone(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApplication, "timezone").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "timezone", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vpcId")
     def vpc_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: vpcId: EDAS namespace corresponding VPC. In Serverless in a corresponding one of the VPC namespace only, and can not be modified. Serverless first created in the application name space will form a binding relationship. You may correspond to a plurality of namespaces VPC. Do not fill was VpcId namespace binding.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "vpcId"))
 
     @vpc_id.setter
     def vpc_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApplication, "vpc_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vpcId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vSwitchId")
     def v_switch_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: vSwitchId: Application examples where the elastic card virtual switch. The switch must be located above the VPC. The same switch with EDAS namespace binding relationship. Do not fill was VSwitchId namespace binding.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "vSwitchId"))
 
     @v_switch_id.setter
     def v_switch_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApplication, "v_switch_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vSwitchId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="warStartOptions")
     def war_start_options(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :: " start
         :Property: warStartOptions: War Start the application package option. Apply the default startup command: java $ JAVA_OPTS $ CATALINA_OPTS -Options org.apache.catalina.startup.Bootstrap "$
@@ -1315,31 +1478,37 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "warStartOptions"))
 
     @war_start_options.setter
     def war_start_options(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApplication, "war_start_options").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "warStartOptions", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="webContainer")
     def web_container(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: webContainer: Tomcat deployment of the package depends on the version. Mirroring not supported.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "webContainer"))
 
     @web_container.setter
     def web_container(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApplication, "web_container").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "webContainer", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-sae.RosApplication.TagsProperty",
         jsii_struct_bases=[],
         name_mapping={"key": "key", "value": "value"},
     )
@@ -1350,14 +1519,18 @@
             key: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param key: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosApplication.TagsProperty.__init__)
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {
                 "key": key,
             }
             if value is not None:
                 self._values["value"] = value
 
         @builtins.property
@@ -1459,15 +1632,15 @@
         package_url: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         package_version: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         post_start: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         pre_stop: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         readiness: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         security_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         sls_configs: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence[RosApplication.TagsProperty]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union[RosApplication.TagsProperty, typing.Dict[str, typing.Any]]]] = None,
         timezone: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         vpc_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         v_switch_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         war_start_options: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         web_container: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::SAE::Application``.
@@ -1503,14 +1676,50 @@
         :param tags: 
         :param timezone: 
         :param vpc_id: 
         :param v_switch_id: 
         :param war_start_options: 
         :param web_container: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosApplicationProps.__init__)
+            check_type(argname="argument app_name", value=app_name, expected_type=type_hints["app_name"])
+            check_type(argname="argument cpu", value=cpu, expected_type=type_hints["cpu"])
+            check_type(argname="argument memory", value=memory, expected_type=type_hints["memory"])
+            check_type(argname="argument namespace_id", value=namespace_id, expected_type=type_hints["namespace_id"])
+            check_type(argname="argument package_type", value=package_type, expected_type=type_hints["package_type"])
+            check_type(argname="argument replicas", value=replicas, expected_type=type_hints["replicas"])
+            check_type(argname="argument app_description", value=app_description, expected_type=type_hints["app_description"])
+            check_type(argname="argument command", value=command, expected_type=type_hints["command"])
+            check_type(argname="argument command_args", value=command_args, expected_type=type_hints["command_args"])
+            check_type(argname="argument custom_host_alias", value=custom_host_alias, expected_type=type_hints["custom_host_alias"])
+            check_type(argname="argument deploy", value=deploy, expected_type=type_hints["deploy"])
+            check_type(argname="argument edas_container_version", value=edas_container_version, expected_type=type_hints["edas_container_version"])
+            check_type(argname="argument envs", value=envs, expected_type=type_hints["envs"])
+            check_type(argname="argument image_url", value=image_url, expected_type=type_hints["image_url"])
+            check_type(argname="argument jar_start_args", value=jar_start_args, expected_type=type_hints["jar_start_args"])
+            check_type(argname="argument jar_start_options", value=jar_start_options, expected_type=type_hints["jar_start_options"])
+            check_type(argname="argument jdk", value=jdk, expected_type=type_hints["jdk"])
+            check_type(argname="argument liveness", value=liveness, expected_type=type_hints["liveness"])
+            check_type(argname="argument mount_desc", value=mount_desc, expected_type=type_hints["mount_desc"])
+            check_type(argname="argument mount_host", value=mount_host, expected_type=type_hints["mount_host"])
+            check_type(argname="argument nas_id", value=nas_id, expected_type=type_hints["nas_id"])
+            check_type(argname="argument package_url", value=package_url, expected_type=type_hints["package_url"])
+            check_type(argname="argument package_version", value=package_version, expected_type=type_hints["package_version"])
+            check_type(argname="argument post_start", value=post_start, expected_type=type_hints["post_start"])
+            check_type(argname="argument pre_stop", value=pre_stop, expected_type=type_hints["pre_stop"])
+            check_type(argname="argument readiness", value=readiness, expected_type=type_hints["readiness"])
+            check_type(argname="argument security_group_id", value=security_group_id, expected_type=type_hints["security_group_id"])
+            check_type(argname="argument sls_configs", value=sls_configs, expected_type=type_hints["sls_configs"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument timezone", value=timezone, expected_type=type_hints["timezone"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
+            check_type(argname="argument war_start_options", value=war_start_options, expected_type=type_hints["war_start_options"])
+            check_type(argname="argument web_container", value=web_container, expected_type=type_hints["web_container"])
         self._values: typing.Dict[str, typing.Any] = {
             "app_name": app_name,
             "cpu": cpu,
             "memory": memory,
             "namespace_id": namespace_id,
             "package_type": package_type,
             "replicas": replicas,
@@ -1933,109 +2142,130 @@
 ):
     '''A ROS template type:  ``ALIYUN::SAE::Namespace``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosNamespaceProps",
+        props: typing.Union["RosNamespaceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::SAE::Namespace``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosNamespace.__init__)
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
+            type_hints = typing.get_type_hints(RosNamespace._render_properties)
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
     @jsii.member(jsii_name="attrNamespaceId")
     def attr_namespace_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: NamespaceId: Namespace ID
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrNamespaceId"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosNamespace, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="namespaceId")
     def namespace_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: namespaceId: Namespace ID. Format: "regionId:logicalId" or "logicalId"
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "namespaceId"))
 
     @namespace_id.setter
     def namespace_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosNamespace, "namespace_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "namespaceId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="namespaceName")
     def namespace_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: namespaceName: Namespace name
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "namespaceName"))
 
     @namespace_name.setter
     def namespace_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosNamespace, "namespace_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "namespaceName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="namespaceDescription")
     def namespace_description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: namespaceDescription: Namespace description
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "namespaceDescription"))
 
     @namespace_description.setter
     def namespace_description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosNamespace, "namespace_description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "namespaceDescription", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-sae.RosNamespaceProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -2054,14 +2284,19 @@
     ) -> None:
         '''Properties for defining a ``ALIYUN::SAE::Namespace``.
 
         :param namespace_id: 
         :param namespace_name: 
         :param namespace_description: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosNamespaceProps.__init__)
+            check_type(argname="argument namespace_id", value=namespace_id, expected_type=type_hints["namespace_id"])
+            check_type(argname="argument namespace_name", value=namespace_name, expected_type=type_hints["namespace_name"])
+            check_type(argname="argument namespace_description", value=namespace_description, expected_type=type_hints["namespace_description"])
         self._values: typing.Dict[str, typing.Any] = {
             "namespace_id": namespace_id,
             "namespace_name": namespace_name,
         }
         if namespace_description is not None:
             self._values["namespace_description"] = namespace_description
 
@@ -2112,153 +2347,180 @@
 ):
     '''A ROS template type:  ``ALIYUN::SAE::SlbBinding``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosSlbBindingProps",
+        props: typing.Union["RosSlbBindingProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::SAE::SlbBinding``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosSlbBinding.__init__)
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
+            type_hints = typing.get_type_hints(RosSlbBinding._render_properties)
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
     @jsii.member(jsii_name="attrAppId")
     def attr_app_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: AppId: Successful application deployment target ID
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAppId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrChangeOrderId")
     def attr_change_order_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ChangeOrderId: Return to release a single ID, used to query task execution status.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrChangeOrderId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="appId")
     def app_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: appId: Successful application deployment target ID
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "appId"))
 
     @app_id.setter
     def app_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSlbBinding, "app_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "appId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSlbBinding, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="internet")
     def internet(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: internet: Binding public SLB. For example: [{ "port": 80, "targetPort": 8080, "protocol": "TCP"}], shows a container port 8080 through port 80 slb exposed service, the protocol is TCP, the blank is ignored.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "internet"))
 
     @internet.setter
     def internet(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSlbBinding, "internet").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internet", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="internetSlbId")
     def internet_slb_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: internetSlbId: Use SLB purchased specified, currently only supports non-shared examples
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "internetSlbId"))
 
     @internet_slb_id.setter
     def internet_slb_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSlbBinding, "internet_slb_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internetSlbId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="intranet")
     def intranet(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: intranet: Bind private SLB. For example: [{ "port": 80, "targetPort": 8080, "protocol": "TCP"}], shows a container port 8080 through port 80 slb exposed service, the protocol is TCP, the blank is ignored.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "intranet"))
 
     @intranet.setter
     def intranet(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSlbBinding, "intranet").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "intranet", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="intranetSlbId")
     def intranet_slb_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: intranetSlbId: Use SLB purchased specified, currently only supports non-shared examples
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "intranetSlbId"))
 
     @intranet_slb_id.setter
     def intranet_slb_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSlbBinding, "intranet_slb_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "intranetSlbId", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-sae.RosSlbBindingProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -2283,14 +2545,21 @@
 
         :param app_id: 
         :param internet: 
         :param internet_slb_id: 
         :param intranet: 
         :param intranet_slb_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosSlbBindingProps.__init__)
+            check_type(argname="argument app_id", value=app_id, expected_type=type_hints["app_id"])
+            check_type(argname="argument internet", value=internet, expected_type=type_hints["internet"])
+            check_type(argname="argument internet_slb_id", value=internet_slb_id, expected_type=type_hints["internet_slb_id"])
+            check_type(argname="argument intranet", value=intranet, expected_type=type_hints["intranet"])
+            check_type(argname="argument intranet_slb_id", value=intranet_slb_id, expected_type=type_hints["intranet_slb_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "app_id": app_id,
         }
         if internet is not None:
             self._values["internet"] = internet
         if internet_slb_id is not None:
             self._values["internet_slb_id"] = internet_slb_id
@@ -2367,37 +2636,43 @@
 ):
     '''A ROS resource type:  ``ALIYUN::SAE::SlbBinding``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "SlbBindingProps",
+        props: typing.Union["SlbBindingProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::SAE::SlbBinding``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(SlbBinding.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAppId")
     def attr_app_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute AppId: Successful application deployment target ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAppId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrChangeOrderId")
     def attr_change_order_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ChangeOrderId: Return to release a single ID, used to query task execution status.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrChangeOrderId"))
 
 
 @jsii.data_type(
@@ -2425,14 +2700,21 @@
 
         :param app_id: Property appId: Successful application deployment target ID.
         :param internet: Property internet: Binding public SLB. For example: [{ "port": 80, "targetPort": 8080, "protocol": "TCP"}], shows a container port 8080 through port 80 slb exposed service, the protocol is TCP, the blank is ignored.
         :param internet_slb_id: Property internetSlbId: Use SLB purchased specified, currently only supports non-shared examples.
         :param intranet: Property intranet: Bind private SLB. For example: [{ "port": 80, "targetPort": 8080, "protocol": "TCP"}], shows a container port 8080 through port 80 slb exposed service, the protocol is TCP, the blank is ignored.
         :param intranet_slb_id: Property intranetSlbId: Use SLB purchased specified, currently only supports non-shared examples.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(SlbBindingProps.__init__)
+            check_type(argname="argument app_id", value=app_id, expected_type=type_hints["app_id"])
+            check_type(argname="argument internet", value=internet, expected_type=type_hints["internet"])
+            check_type(argname="argument internet_slb_id", value=internet_slb_id, expected_type=type_hints["internet_slb_id"])
+            check_type(argname="argument intranet", value=intranet, expected_type=type_hints["intranet"])
+            check_type(argname="argument intranet_slb_id", value=intranet_slb_id, expected_type=type_hints["intranet_slb_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "app_id": app_id,
         }
         if internet is not None:
             self._values["internet"] = internet
         if internet_slb_id is not None:
             self._values["internet_slb_id"] = internet_slb_id
```

### Comparing `ros-cdk-sae-1.0.8/src/ros_cdk_sae.egg-info/PKG-INFO` & `ros-cdk-sae-1.0.9/src/ros_cdk_sae.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-sae
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS SAE Construct Library
```

