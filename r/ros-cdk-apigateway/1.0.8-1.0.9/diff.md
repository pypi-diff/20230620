# Comparing `tmp/ros-cdk-apigateway-1.0.8.tar.gz` & `tmp/ros-cdk-apigateway-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-apigateway-1.0.8.tar", last modified: Thu Jul 14 02:16:46 2022, max compression
+gzip compressed data, was "dist/ros-cdk-apigateway-1.0.9.tar", last modified: Fri Sep 23 12:00:40 2022, max compression
```

## Comparing `ros-cdk-apigateway-1.0.8.tar` & `ros-cdk-apigateway-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:16:46.000000 ros-cdk-apigateway-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:16:45.000000 ros-cdk-apigateway-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:16:45.000000 ros-cdk-apigateway-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:16:45.000000 ros-cdk-apigateway-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1268 2022-07-14 02:16:46.000000 ros-cdk-apigateway-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      200 2022-07-14 02:16:45.000000 ros-cdk-apigateway-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:16:45.000000 ros-cdk-apigateway-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:16:46.000000 ros-cdk-apigateway-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1836 2022-07-14 02:16:45.000000 ros-cdk-apigateway-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:16:46.000000 ros-cdk-apigateway-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:16:46.000000 ros-cdk-apigateway-1.0.8/src/ros_cdk_apigateway/
--rw-r--r--   0 root         (0) root         (0)   359513 2022-07-14 02:16:45.000000 ros-cdk-apigateway-1.0.8/src/ros_cdk_apigateway/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:16:46.000000 ros-cdk-apigateway-1.0.8/src/ros_cdk_apigateway/_jsii/
--rw-r--r--   0 root         (0) root         (0)      397 2022-07-14 02:16:45.000000 ros-cdk-apigateway-1.0.8/src/ros_cdk_apigateway/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)   130546 2022-07-14 02:16:45.000000 ros-cdk-apigateway-1.0.8/src/ros_cdk_apigateway/_jsii/ros-cdk-apigateway@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:16:45.000000 ros-cdk-apigateway-1.0.8/src/ros_cdk_apigateway/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:16:46.000000 ros-cdk-apigateway-1.0.8/src/ros_cdk_apigateway.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1268 2022-07-14 02:16:46.000000 ros-cdk-apigateway-1.0.8/src/ros_cdk_apigateway.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      470 2022-07-14 02:16:46.000000 ros-cdk-apigateway-1.0.8/src/ros_cdk_apigateway.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:16:46.000000 ros-cdk-apigateway-1.0.8/src/ros_cdk_apigateway.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:16:46.000000 ros-cdk-apigateway-1.0.8/src/ros_cdk_apigateway.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2022-07-14 02:16:46.000000 ros-cdk-apigateway-1.0.8/src/ros_cdk_apigateway.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:00:40.000000 ros-cdk-apigateway-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 12:00:40.000000 ros-cdk-apigateway-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 12:00:40.000000 ros-cdk-apigateway-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 12:00:40.000000 ros-cdk-apigateway-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1268 2022-09-23 12:00:40.000000 ros-cdk-apigateway-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      200 2022-09-23 12:00:40.000000 ros-cdk-apigateway-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 12:00:40.000000 ros-cdk-apigateway-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 12:00:40.000000 ros-cdk-apigateway-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1865 2022-09-23 12:00:40.000000 ros-cdk-apigateway-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:00:40.000000 ros-cdk-apigateway-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:00:40.000000 ros-cdk-apigateway-1.0.9/src/ros_cdk_apigateway/
+-rw-r--r--   0 root         (0) root         (0)   439266 2022-09-23 12:00:40.000000 ros-cdk-apigateway-1.0.9/src/ros_cdk_apigateway/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:00:40.000000 ros-cdk-apigateway-1.0.9/src/ros_cdk_apigateway/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      431 2022-09-23 12:00:40.000000 ros-cdk-apigateway-1.0.9/src/ros_cdk_apigateway/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   130615 2022-09-23 12:00:40.000000 ros-cdk-apigateway-1.0.9/src/ros_cdk_apigateway/_jsii/ros-cdk-apigateway@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 12:00:40.000000 ros-cdk-apigateway-1.0.9/src/ros_cdk_apigateway/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:00:40.000000 ros-cdk-apigateway-1.0.9/src/ros_cdk_apigateway.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1268 2022-09-23 12:00:40.000000 ros-cdk-apigateway-1.0.9/src/ros_cdk_apigateway.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      470 2022-09-23 12:00:40.000000 ros-cdk-apigateway-1.0.9/src/ros_cdk_apigateway.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 12:00:40.000000 ros-cdk-apigateway-1.0.9/src/ros_cdk_apigateway.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 12:00:40.000000 ros-cdk-apigateway-1.0.9/src/ros_cdk_apigateway.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2022-09-23 12:00:40.000000 ros-cdk-apigateway-1.0.9/src/ros_cdk_apigateway.egg-info/top_level.txt
```

### Comparing `ros-cdk-apigateway-1.0.8/LICENSE` & `ros-cdk-apigateway-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-apigateway-1.0.8/PKG-INFO` & `ros-cdk-apigateway-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-apigateway
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS APIGATEWAY Construct Library
```

### Comparing `ros-cdk-apigateway-1.0.8/setup.py` & `ros-cdk-apigateway-1.0.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-apigateway",
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
         "ros_cdk_apigateway",
         "ros_cdk_apigateway._jsii"
     ],
     "package_data": {
         "ros_cdk_apigateway._jsii": [
-            "ros-cdk-apigateway@1.0.8.jsii.tgz"
+            "ros-cdk-apigateway@1.0.9.jsii.tgz"
         ],
         "ros_cdk_apigateway": [
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

### Comparing `ros-cdk-apigateway-1.0.8/src/ros_cdk_apigateway/__init__.py` & `ros-cdk-apigateway-1.0.9/src/ros_cdk_apigateway/__init__.py`

 * *Files 17% similar despite different names*

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
 
 
 class Api(
     ros_cdk_core.Resource,
@@ -29,31 +31,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::ApiGateway::Api``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "ApiProps",
+        props: typing.Union["ApiProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::ApiGateway::Api``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Api.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrApiId")
     def attr_api_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ApiId: The id of the API.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrApiId"))
 
 
 @jsii.data_type(
@@ -85,33 +93,33 @@
 )
 class ApiProps:
     def __init__(
         self,
         *,
         api_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         group_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        request_config: typing.Union[ros_cdk_core.IResolvable, "RosApi.RequestConfigProperty"],
+        request_config: typing.Union[ros_cdk_core.IResolvable, typing.Union["RosApi.RequestConfigProperty", typing.Dict[str, typing.Any]]],
         result_sample: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         result_type: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        service_config: typing.Union[ros_cdk_core.IResolvable, "RosApi.ServiceConfigProperty"],
+        service_config: typing.Union[ros_cdk_core.IResolvable, typing.Union["RosApi.ServiceConfigProperty", typing.Dict[str, typing.Any]]],
         visibility: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         app_code_auth_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         auth_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        const_parameters: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosApi.ConstParametersProperty"]]]] = None,
+        const_parameters: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosApi.ConstParametersProperty", typing.Dict[str, typing.Any]]]]]] = None,
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         disable_internet: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
-        error_code_samples: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosApi.ErrorCodeSamplesProperty"]]]] = None,
+        error_code_samples: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosApi.ErrorCodeSamplesProperty", typing.Dict[str, typing.Any]]]]]] = None,
         fail_result_sample: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         force_nonce_check: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
-        open_id_connect_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosApi.OpenIdConnectConfigProperty"]] = None,
-        request_parameters: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosApi.RequestParametersProperty"]]]] = None,
-        service_parameters: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosApi.ServiceParametersProperty"]]]] = None,
-        service_parameters_map: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosApi.ServiceParametersMapProperty"]]]] = None,
-        system_parameters: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosApi.SystemParametersProperty"]]]] = None,
-        tags: typing.Optional[typing.Sequence["RosApi.TagsProperty"]] = None,
+        open_id_connect_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosApi.OpenIdConnectConfigProperty", typing.Dict[str, typing.Any]]]] = None,
+        request_parameters: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosApi.RequestParametersProperty", typing.Dict[str, typing.Any]]]]]] = None,
+        service_parameters: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosApi.ServiceParametersProperty", typing.Dict[str, typing.Any]]]]]] = None,
+        service_parameters_map: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosApi.ServiceParametersMapProperty", typing.Dict[str, typing.Any]]]]]] = None,
+        system_parameters: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosApi.SystemParametersProperty", typing.Dict[str, typing.Any]]]]]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union["RosApi.TagsProperty", typing.Dict[str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::ApiGateway::Api``.
 
         :param api_name: Property apiName: The name of the API.Need [4, 50] Chinese\\English\\Number characters or "_",and should start with Chinese/English character.
         :param group_id: Property groupId: The id of the Group.
         :param request_config: Property requestConfig: The configuration of the request.
         :param result_sample: Property resultSample: The sample of the result.
@@ -129,14 +137,37 @@
         :param open_id_connect_config: Property openIdConnectConfig: The configuration of the open id.
         :param request_parameters: Property requestParameters: The request parameters.
         :param service_parameters: Property serviceParameters: The service parameters.
         :param service_parameters_map: Property serviceParametersMap: The mapping relation between (request parameters\\const parameters\\system parameters) and service parameters.
         :param system_parameters: Property systemParameters: The system parameters.
         :param tags: Property tags: Tags to attach to instance. Max support 20 tags to add during create instance. Each tag with two properties Key and Value, and Key is required.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ApiProps.__init__)
+            check_type(argname="argument api_name", value=api_name, expected_type=type_hints["api_name"])
+            check_type(argname="argument group_id", value=group_id, expected_type=type_hints["group_id"])
+            check_type(argname="argument request_config", value=request_config, expected_type=type_hints["request_config"])
+            check_type(argname="argument result_sample", value=result_sample, expected_type=type_hints["result_sample"])
+            check_type(argname="argument result_type", value=result_type, expected_type=type_hints["result_type"])
+            check_type(argname="argument service_config", value=service_config, expected_type=type_hints["service_config"])
+            check_type(argname="argument visibility", value=visibility, expected_type=type_hints["visibility"])
+            check_type(argname="argument app_code_auth_type", value=app_code_auth_type, expected_type=type_hints["app_code_auth_type"])
+            check_type(argname="argument auth_type", value=auth_type, expected_type=type_hints["auth_type"])
+            check_type(argname="argument const_parameters", value=const_parameters, expected_type=type_hints["const_parameters"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument disable_internet", value=disable_internet, expected_type=type_hints["disable_internet"])
+            check_type(argname="argument error_code_samples", value=error_code_samples, expected_type=type_hints["error_code_samples"])
+            check_type(argname="argument fail_result_sample", value=fail_result_sample, expected_type=type_hints["fail_result_sample"])
+            check_type(argname="argument force_nonce_check", value=force_nonce_check, expected_type=type_hints["force_nonce_check"])
+            check_type(argname="argument open_id_connect_config", value=open_id_connect_config, expected_type=type_hints["open_id_connect_config"])
+            check_type(argname="argument request_parameters", value=request_parameters, expected_type=type_hints["request_parameters"])
+            check_type(argname="argument service_parameters", value=service_parameters, expected_type=type_hints["service_parameters"])
+            check_type(argname="argument service_parameters_map", value=service_parameters_map, expected_type=type_hints["service_parameters_map"])
+            check_type(argname="argument system_parameters", value=system_parameters, expected_type=type_hints["system_parameters"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
         self._values: typing.Dict[str, typing.Any] = {
             "api_name": api_name,
             "group_id": group_id,
             "request_config": request_config,
             "result_sample": result_sample,
             "result_type": result_type,
             "service_config": service_config,
@@ -378,49 +409,55 @@
 ):
     '''A ROS resource type:  ``ALIYUN::ApiGateway::App``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "AppProps",
+        props: typing.Union["AppProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::ApiGateway::App``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(App.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAppId")
     def attr_app_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute AppId: The id of the created APP.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAppId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAppKey")
     def attr_app_key(self) -> ros_cdk_core.IResolvable:
         '''Attribute AppKey: The key of the APP.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAppKey"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAppSecret")
     def attr_app_secret(self) -> ros_cdk_core.IResolvable:
         '''Attribute AppSecret: The secret of the APP.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAppSecret"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTags")
     def attr_tags(self) -> ros_cdk_core.IResolvable:
         '''Attribute Tags: Tags of app.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTags"))
 
 
 @jsii.data_type(
@@ -430,22 +467,27 @@
 )
 class AppProps:
     def __init__(
         self,
         *,
         app_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence["RosApp.TagsProperty"]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union["RosApp.TagsProperty", typing.Dict[str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::ApiGateway::App``.
 
         :param app_name: Property appName: The name of the App.Need [4, 26] Chinese\\English\\Number characters or "_",and should start with Chinese/English character.
         :param description: Property description: Description of the App, less than 180 characters.
         :param tags: Property tags: Tags to attach to app. Max support 20 tags to add during create app. Each tag with two properties Key and Value, and Key is required.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(AppProps.__init__)
+            check_type(argname="argument app_name", value=app_name, expected_type=type_hints["app_name"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
         self._values: typing.Dict[str, typing.Any] = {
             "app_name": app_name,
         }
         if description is not None:
             self._values["description"] = description
         if tags is not None:
             self._values["tags"] = tags
@@ -493,28 +535,34 @@
 ):
     '''A ROS resource type:  ``ALIYUN::ApiGateway::Authorization``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "AuthorizationProps",
+        props: typing.Union["AuthorizationProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::ApiGateway::Authorization``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Authorization.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-apigateway.AuthorizationProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -539,14 +587,21 @@
 
         :param api_ids: Property apiIds: APIs to authorize.
         :param app_ids: Property appIds: APPs are authorized to APIs.
         :param group_id: Property groupId: The id of the group.
         :param stage_name: Property stageName: Authorize in this stage.
         :param description: Property description: Description of the authorization, less than 180 characters.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(AuthorizationProps.__init__)
+            check_type(argname="argument api_ids", value=api_ids, expected_type=type_hints["api_ids"])
+            check_type(argname="argument app_ids", value=app_ids, expected_type=type_hints["app_ids"])
+            check_type(argname="argument group_id", value=group_id, expected_type=type_hints["group_id"])
+            check_type(argname="argument stage_name", value=stage_name, expected_type=type_hints["stage_name"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
         self._values: typing.Dict[str, typing.Any] = {
             "api_ids": api_ids,
             "app_ids": app_ids,
             "group_id": group_id,
             "stage_name": stage_name,
         }
         if description is not None:
@@ -611,31 +666,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::ApiGateway::CustomDomain``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "CustomDomainProps",
+        props: typing.Union["CustomDomainProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::ApiGateway::CustomDomain``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(CustomDomain.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCertificateId")
     def attr_certificate_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute CertificateId: The id of the certificate.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCertificateId"))
 
 
 @jsii.data_type(
@@ -663,14 +724,21 @@
 
         :param domain_name: Property domainName: Custom domain name.
         :param group_id: Property groupId: The id of the Group.
         :param certificate_body: Property certificateBody: SSL certificate body.
         :param certificate_name: Property certificateName: SSL certificate name.
         :param certificate_private_key: Property certificatePrivateKey: SSL certificate key.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(CustomDomainProps.__init__)
+            check_type(argname="argument domain_name", value=domain_name, expected_type=type_hints["domain_name"])
+            check_type(argname="argument group_id", value=group_id, expected_type=type_hints["group_id"])
+            check_type(argname="argument certificate_body", value=certificate_body, expected_type=type_hints["certificate_body"])
+            check_type(argname="argument certificate_name", value=certificate_name, expected_type=type_hints["certificate_name"])
+            check_type(argname="argument certificate_private_key", value=certificate_private_key, expected_type=type_hints["certificate_private_key"])
         self._values: typing.Dict[str, typing.Any] = {
             "domain_name": domain_name,
             "group_id": group_id,
         }
         if certificate_body is not None:
             self._values["certificate_body"] = certificate_body
         if certificate_name is not None:
@@ -735,28 +803,34 @@
 ):
     '''A ROS resource type:  ``ALIYUN::ApiGateway::Deployment``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "DeploymentProps",
+        props: typing.Union["DeploymentProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::ApiGateway::Deployment``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Deployment.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-apigateway.DeploymentProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -781,14 +855,21 @@
 
         :param api_id: Property apiId: The id of the API.
         :param group_id: Property groupId: The id of the Group.
         :param stage_name: Property stageName: Bind traffic in this stage.
         :param description: Property description: Description of the deployment, less than 180 characters.
         :param history_version: Property historyVersion: The history version.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(DeploymentProps.__init__)
+            check_type(argname="argument api_id", value=api_id, expected_type=type_hints["api_id"])
+            check_type(argname="argument group_id", value=group_id, expected_type=type_hints["group_id"])
+            check_type(argname="argument stage_name", value=stage_name, expected_type=type_hints["stage_name"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument history_version", value=history_version, expected_type=type_hints["history_version"])
         self._values: typing.Dict[str, typing.Any] = {
             "api_id": api_id,
             "group_id": group_id,
             "stage_name": stage_name,
         }
         if description is not None:
             self._values["description"] = description
@@ -851,43 +932,49 @@
 ):
     '''A ROS resource type:  ``ALIYUN::ApiGateway::Group``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "GroupProps",
+        props: typing.Union["GroupProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::ApiGateway::Group``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Group.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrGroupId")
     def attr_group_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute GroupId: The id of the created Group resource.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrGroupId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSubDomain")
     def attr_sub_domain(self) -> ros_cdk_core.IResolvable:
         '''Attribute SubDomain: The sub domain assigned to the Group by the system.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSubDomain"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTags")
     def attr_tags(self) -> ros_cdk_core.IResolvable:
         '''Attribute Tags: Tags of app.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTags"))
 
 
 @jsii.data_type(
@@ -908,27 +995,36 @@
         self,
         *,
         group_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         instance_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         internet_enable: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         passthrough_headers: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence["RosGroup.TagsProperty"]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union["RosGroup.TagsProperty", typing.Dict[str, typing.Any]]]] = None,
         vpc_intranet_enable: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::ApiGateway::Group``.
 
         :param group_name: Property groupName: The name of the Group.Need [4, 50] Chinese\\English\\Number characters or "_",and should start with Chinese/English character.
         :param description: Property description: Description of the Group, less than 180 characters.
         :param instance_id: Property instanceId: API gateway instance ID. For example, "api-shared-vpc-001" means vpc instance, while "api-shared-classic-001" means classic instance.
         :param internet_enable: Property internetEnable: Enable or disable internet subdomain. True for enable.
         :param passthrough_headers: Property passthroughHeaders: Pass through headers setting. values: host: pass through host headers
         :param tags: Property tags: Tags to attach to group. Max support 20 tags to add during create group. Each tag with two properties Key and Value, and Key is required.
         :param vpc_intranet_enable: Property vpcIntranetEnable: Enable or disable VPC intranet subdomain. True for enable.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(GroupProps.__init__)
+            check_type(argname="argument group_name", value=group_name, expected_type=type_hints["group_name"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument instance_id", value=instance_id, expected_type=type_hints["instance_id"])
+            check_type(argname="argument internet_enable", value=internet_enable, expected_type=type_hints["internet_enable"])
+            check_type(argname="argument passthrough_headers", value=passthrough_headers, expected_type=type_hints["passthrough_headers"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument vpc_intranet_enable", value=vpc_intranet_enable, expected_type=type_hints["vpc_intranet_enable"])
         self._values: typing.Dict[str, typing.Any] = {
             "group_name": group_name,
         }
         if description is not None:
             self._values["description"] = description
         if instance_id is not None:
             self._values["instance_id"] = instance_id
@@ -1029,73 +1125,79 @@
 ):
     '''A ROS resource type:  ``ALIYUN::ApiGateway::Instance``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "InstanceProps",
+        props: typing.Union["InstanceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::ApiGateway::Instance``.
 
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
     @jsii.member(jsii_name="attrEgressIpv6Enable")
     def attr_egress_ipv6_enable(self) -> ros_cdk_core.IResolvable:
         '''Attribute EgressIpv6Enable: Whether enable egress IPV6.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrEgressIpv6Enable"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceId")
     def attr_instance_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute InstanceId: Instance ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceType")
     def attr_instance_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute InstanceType: Instance type.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInternetEgressAddress")
     def attr_internet_egress_address(self) -> ros_cdk_core.IResolvable:
         '''Attribute InternetEgressAddress: Internet egress dddress.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInternetEgressAddress"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSupportIpv6")
     def attr_support_ipv6(self) -> ros_cdk_core.IResolvable:
         '''Attribute SupportIpv6: Whether support IPV6.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSupportIpv6"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVpcEgressAddress")
     def attr_vpc_egress_address(self) -> ros_cdk_core.IResolvable:
         '''Attribute VpcEgressAddress: VPC network egress address.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVpcEgressAddress"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVpcIntranetEnable")
     def attr_vpc_intranet_enable(self) -> ros_cdk_core.IResolvable:
         '''Attribute VpcIntranetEnable: Whether enable VPC intranet.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVpcIntranetEnable"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVpcSlbIntranetEnable")
     def attr_vpc_slb_intranet_enable(self) -> ros_cdk_core.IResolvable:
         '''Attribute VpcSlbIntranetEnable: Whether enable VPC SLB intranet.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVpcSlbIntranetEnable"))
 
 
 @jsii.data_type(
@@ -1123,29 +1225,41 @@
         instance_spec: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         zone_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         auto_pay: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         charge_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         deletion_force: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         duration: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         pricing_cycle: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence["RosInstance.TagsProperty"]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union["RosInstance.TagsProperty", typing.Dict[str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::ApiGateway::Instance``.
 
         :param https_policy: Property httpsPolicy: HTTPS security policy. Valid values: HTTPS2_TLS1_0, HTTPS2_TLS1_2, HTTPS1_1_TLS1_0
         :param instance_name: Property instanceName: Instance name.
         :param instance_spec: Property instanceSpec: Instance specification. For example: api.s1.small
         :param zone_id: Property zoneId: Zone to which the instance belongs. For example: cn-beijing-MAZ2(f,g). Pleas call DescribeZones to get supported zone list.
         :param auto_pay: Property autoPay: Indicates whether automatic payment is enabled. Valid values: false: Automatic payment is disabled. You need to go to Orders to make the payment once an order is generated. true: Automatic payment is enabled. The payment is automatically made.
         :param charge_type: Property chargeType: The billing method of the router interface. Valid values: PrePaid (Subscription), PostPaid (default, Pay-As-You-Go). Default value: PostPaid.
         :param deletion_force: Property deletionForce: Whether force delete the instance even if its status is START_FAILED. Default value is false.
         :param duration: Property duration: Prepaid time period. It could be from 1 to 9 when PricingCycle is Month, or 1 to 3 when PricingCycle is Year. Default value is 3.
         :param pricing_cycle: Property pricingCycle: Unit of the payment cycle. It could be Month (default) or Year.
         :param tags: Property tags: Tags to attach to instance. Max support 20 tags to add during create instance. Each tag with two properties Key and Value, and Key is required.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(InstanceProps.__init__)
+            check_type(argname="argument https_policy", value=https_policy, expected_type=type_hints["https_policy"])
+            check_type(argname="argument instance_name", value=instance_name, expected_type=type_hints["instance_name"])
+            check_type(argname="argument instance_spec", value=instance_spec, expected_type=type_hints["instance_spec"])
+            check_type(argname="argument zone_id", value=zone_id, expected_type=type_hints["zone_id"])
+            check_type(argname="argument auto_pay", value=auto_pay, expected_type=type_hints["auto_pay"])
+            check_type(argname="argument charge_type", value=charge_type, expected_type=type_hints["charge_type"])
+            check_type(argname="argument deletion_force", value=deletion_force, expected_type=type_hints["deletion_force"])
+            check_type(argname="argument duration", value=duration, expected_type=type_hints["duration"])
+            check_type(argname="argument pricing_cycle", value=pricing_cycle, expected_type=type_hints["pricing_cycle"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
         self._values: typing.Dict[str, typing.Any] = {
             "https_policy": https_policy,
             "instance_name": instance_name,
             "instance_spec": instance_spec,
             "zone_id": zone_id,
         }
         if auto_pay is not None:
@@ -1284,37 +1398,43 @@
 ):
     '''A ROS resource type:  ``ALIYUN::ApiGateway::LogConfig``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "LogConfigProps",
+        props: typing.Union["LogConfigProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::ApiGateway::LogConfig``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(LogConfig.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSlsLogStore")
     def attr_sls_log_store(self) -> ros_cdk_core.IResolvable:
         '''Attribute SlsLogStore: Logstore name of SLS.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSlsLogStore"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSlsProject")
     def attr_sls_project(self) -> ros_cdk_core.IResolvable:
         '''Attribute SlsProject: Project name of SLS.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSlsProject"))
 
 
 @jsii.data_type(
@@ -1330,14 +1450,18 @@
         sls_project: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::ApiGateway::LogConfig``.
 
         :param sls_log_store: Property slsLogStore: Logstore name of SLS.
         :param sls_project: Property slsProject: Project name of SLS.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(LogConfigProps.__init__)
+            check_type(argname="argument sls_log_store", value=sls_log_store, expected_type=type_hints["sls_log_store"])
+            check_type(argname="argument sls_project", value=sls_project, expected_type=type_hints["sls_project"])
         self._values: typing.Dict[str, typing.Any] = {
             "sls_log_store": sls_log_store,
             "sls_project": sls_project,
         }
 
     @builtins.property
     def sls_log_store(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -1372,61 +1496,67 @@
 ):
     '''A ROS resource type:  ``ALIYUN::ApiGateway::Plugin``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "PluginProps",
+        props: typing.Union["PluginProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::ApiGateway::Plugin``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Plugin.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDescription")
     def attr_description(self) -> ros_cdk_core.IResolvable:
         '''Attribute Description: The description of the plug-in, which cannot exceed 200 characters.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDescription"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPluginData")
     def attr_plugin_data(self) -> ros_cdk_core.IResolvable:
         '''Attribute PluginData: The definition statement of the plug-in.
 
         Plug-in definition statements in the JSON and YAML formats are supported.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPluginData"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPluginId")
     def attr_plugin_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute PluginId: The generated plugin ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPluginId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPluginName")
     def attr_plugin_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute PluginName: The name of the plug-in that you want to create.
 
         It can contain uppercase English letters, lowercase English letters, Chinese characters, numbers, and underscores (). It must be 4 to 50 characters in length and cannot start with an underscore ().
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPluginName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPluginType")
     def attr_plugin_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute PluginType: The type of the plug-in.
 
         Valid values: ipControl: indicates IP address-based access control. trafficControl: indicates throttling. backendSignature: indicates backend signature. jwtAuth: indicates JWT (OpenId Connect). cors: indicates cross-origin resource access (CORS). caching: indicates caching.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPluginType"))
@@ -1439,37 +1569,43 @@
 ):
     '''A ROS resource type:  ``ALIYUN::ApiGateway::PluginAttachment``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "PluginAttachmentProps",
+        props: typing.Union["PluginAttachmentProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::ApiGateway::PluginAttachment``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(PluginAttachment.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrApiId")
     def attr_api_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ApiId: The api id.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrApiId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPluginId")
     def attr_plugin_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute PluginId: The plugin id.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPluginId"))
 
 
 @jsii.data_type(
@@ -1491,14 +1627,19 @@
     ) -> None:
         '''Properties for defining a ``ALIYUN::ApiGateway::PluginAttachment``.
 
         :param api_id: Property apiId: The ID of the API to which you want to bind the plug-in.
         :param plugin_id: Property pluginId: The ID of the plugin that you want to bind.
         :param stage_name: Property stageName: The name of the runtime environment. Valid values: RELEASE: indicates the release environment. PRE: indicates the pre-release environment. TEST: indicates the test environment.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(PluginAttachmentProps.__init__)
+            check_type(argname="argument api_id", value=api_id, expected_type=type_hints["api_id"])
+            check_type(argname="argument plugin_id", value=plugin_id, expected_type=type_hints["plugin_id"])
+            check_type(argname="argument stage_name", value=stage_name, expected_type=type_hints["stage_name"])
         self._values: typing.Dict[str, typing.Any] = {
             "api_id": api_id,
             "plugin_id": plugin_id,
             "stage_name": stage_name,
         }
 
     @builtins.property
@@ -1555,24 +1696,31 @@
     def __init__(
         self,
         *,
         plugin_data: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         plugin_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         plugin_type: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence["RosPlugin.TagsProperty"]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union["RosPlugin.TagsProperty", typing.Dict[str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::ApiGateway::Plugin``.
 
         :param plugin_data: Property pluginData: The definition statement of the plug-in. Plug-in definition statements in the JSON and YAML formats are supported.
         :param plugin_name: Property pluginName: The name of the plug-in that you want to create. It can contain uppercase English letters, lowercase English letters, Chinese characters, numbers, and underscores (). It must be 4 to 50 characters in length and cannot start with an underscore ().
         :param plugin_type: Property pluginType: The type of the plug-in. Valid values: ipControl: indicates IP address-based access control. trafficControl: indicates throttling. backendSignature: indicates backend signature. jwtAuth: indicates JWT (OpenId Connect). cors: indicates cross-origin resource access (CORS). caching: indicates caching.
         :param description: Property description: The description of the plug-in, which cannot exceed 200 characters.
         :param tags: Property tags: Tags to attach to instance. Max support 20 tags to add during create instance. Each tag with two properties Key and Value, and Key is required.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(PluginProps.__init__)
+            check_type(argname="argument plugin_data", value=plugin_data, expected_type=type_hints["plugin_data"])
+            check_type(argname="argument plugin_name", value=plugin_name, expected_type=type_hints["plugin_name"])
+            check_type(argname="argument plugin_type", value=plugin_type, expected_type=type_hints["plugin_type"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
         self._values: typing.Dict[str, typing.Any] = {
             "plugin_data": plugin_data,
             "plugin_name": plugin_name,
             "plugin_type": plugin_type,
         }
         if description is not None:
             self._values["description"] = description
@@ -1645,174 +1793,207 @@
 ):
     '''A ROS template type:  ``ALIYUN::ApiGateway::Api``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosApiProps",
+        props: typing.Union["RosApiProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::ApiGateway::Api``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosApi.__init__)
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
+            type_hints = typing.get_type_hints(RosApi._render_properties)
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
     @jsii.member(jsii_name="attrApiId")
     def attr_api_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ApiId: The id of the API.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrApiId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="apiName")
     def api_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: apiName: The name of the API.Need [4, 50] Chinese\\English\\Number characters or "_",and should start with Chinese/English character.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "apiName"))
 
     @api_name.setter
     def api_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApi, "api_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "apiName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApi, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="groupId")
     def group_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: groupId: The id of the Group.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "groupId"))
 
     @group_id.setter
     def group_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApi, "group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "groupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="requestConfig")
     def request_config(
         self,
     ) -> typing.Union[ros_cdk_core.IResolvable, "RosApi.RequestConfigProperty"]:
         '''
         :Property: requestConfig: The configuration of the request
         '''
         return typing.cast(typing.Union[ros_cdk_core.IResolvable, "RosApi.RequestConfigProperty"], jsii.get(self, "requestConfig"))
 
     @request_config.setter
     def request_config(
         self,
         value: typing.Union[ros_cdk_core.IResolvable, "RosApi.RequestConfigProperty"],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApi, "request_config").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "requestConfig", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="resultSample")
     def result_sample(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: resultSample: The sample of the result.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "resultSample"))
 
     @result_sample.setter
     def result_sample(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApi, "result_sample").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "resultSample", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="resultType")
     def result_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: resultType: The format of service's response, "JSON", "TEXT", "BINARY", "XML", "HTML" or "PASSTHROUGH". Default is "JSON".
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "resultType"))
 
     @result_type.setter
     def result_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApi, "result_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "resultType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="serviceConfig")
     def service_config(
         self,
     ) -> typing.Union[ros_cdk_core.IResolvable, "RosApi.ServiceConfigProperty"]:
         '''
         :Property: serviceConfig: The configuration of the service.
         '''
         return typing.cast(typing.Union[ros_cdk_core.IResolvable, "RosApi.ServiceConfigProperty"], jsii.get(self, "serviceConfig"))
 
     @service_config.setter
     def service_config(
         self,
         value: typing.Union[ros_cdk_core.IResolvable, "RosApi.ServiceConfigProperty"],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApi, "service_config").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "serviceConfig", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="visibility")
     def visibility(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: visibility: Whether to make the API public. "PUBLIC" or "PRIVATE".
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "visibility"))
 
     @visibility.setter
     def visibility(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApi, "visibility").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "visibility", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="appCodeAuthType")
     def app_code_auth_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1825,68 +2006,80 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "appCodeAuthType"))
 
     @app_code_auth_type.setter
     def app_code_auth_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApi, "app_code_auth_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "appCodeAuthType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="authType")
     def auth_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: authType: Type of authorization of the API . "APP","ANONYMOUS", or "APPOPENID"
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "authType"))
 
     @auth_type.setter
     def auth_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApi, "auth_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "authType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="constParameters")
     def const_parameters(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosApi.ConstParametersProperty"]]]]:
         '''
         :Property: constParameters: The const parameters.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosApi.ConstParametersProperty"]]]], jsii.get(self, "constParameters"))
 
     @const_parameters.setter
     def const_parameters(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosApi.ConstParametersProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApi, "const_parameters").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "constParameters", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: description: Description of the API, less than 180 characters.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApi, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="disableInternet")
     def disable_internet(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1896,51 +2089,60 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "disableInternet"))
 
     @disable_internet.setter
     def disable_internet(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApi, "disable_internet").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "disableInternet", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="errorCodeSamples")
     def error_code_samples(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosApi.ErrorCodeSamplesProperty"]]]]:
         '''
         :Property: errorCodeSamples: The Error Code samples.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosApi.ErrorCodeSamplesProperty"]]]], jsii.get(self, "errorCodeSamples"))
 
     @error_code_samples.setter
     def error_code_samples(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosApi.ErrorCodeSamplesProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApi, "error_code_samples").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "errorCodeSamples", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="failResultSample")
     def fail_result_sample(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: failResultSample: The sample of the fail result.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "failResultSample"))
 
     @fail_result_sample.setter
     def fail_result_sample(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApi, "fail_result_sample").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "failResultSample", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="forceNonceCheck")
     def force_nonce_check(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1953,111 +2155,132 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "forceNonceCheck"))
 
     @force_nonce_check.setter
     def force_nonce_check(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApi, "force_nonce_check").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "forceNonceCheck", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="openIdConnectConfig")
     def open_id_connect_config(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosApi.OpenIdConnectConfigProperty"]]:
         '''
         :Property: openIdConnectConfig: The configuration of the open id.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosApi.OpenIdConnectConfigProperty"]], jsii.get(self, "openIdConnectConfig"))
 
     @open_id_connect_config.setter
     def open_id_connect_config(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosApi.OpenIdConnectConfigProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApi, "open_id_connect_config").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "openIdConnectConfig", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="requestParameters")
     def request_parameters(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosApi.RequestParametersProperty"]]]]:
         '''
         :Property: requestParameters: The request parameters.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosApi.RequestParametersProperty"]]]], jsii.get(self, "requestParameters"))
 
     @request_parameters.setter
     def request_parameters(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosApi.RequestParametersProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApi, "request_parameters").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "requestParameters", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="serviceParameters")
     def service_parameters(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosApi.ServiceParametersProperty"]]]]:
         '''
         :Property: serviceParameters: The service parameters.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosApi.ServiceParametersProperty"]]]], jsii.get(self, "serviceParameters"))
 
     @service_parameters.setter
     def service_parameters(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosApi.ServiceParametersProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApi, "service_parameters").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "serviceParameters", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="serviceParametersMap")
     def service_parameters_map(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosApi.ServiceParametersMapProperty"]]]]:
         '''
         :Property: serviceParametersMap: The mapping relation between (request parameters\\const parameters\\system parameters) and service parameters.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosApi.ServiceParametersMapProperty"]]]], jsii.get(self, "serviceParametersMap"))
 
     @service_parameters_map.setter
     def service_parameters_map(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosApi.ServiceParametersMapProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApi, "service_parameters_map").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "serviceParametersMap", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="systemParameters")
     def system_parameters(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosApi.SystemParametersProperty"]]]]:
         '''
         :Property: systemParameters: The system parameters.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosApi.SystemParametersProperty"]]]], jsii.get(self, "systemParameters"))
 
     @system_parameters.setter
     def system_parameters(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosApi.SystemParametersProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApi, "system_parameters").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "systemParameters", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tags")
     def tags(self) -> typing.Optional[typing.List["RosApi.TagsProperty"]]:
         '''
         :Property: tags: Tags to attach to instance. Max support 20 tags to add during create instance. Each tag with two properties Key and Value, and Key is required.
         '''
         return typing.cast(typing.Optional[typing.List["RosApi.TagsProperty"]], jsii.get(self, "tags"))
 
     @tags.setter
     def tags(self, value: typing.Optional[typing.List["RosApi.TagsProperty"]]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApi, "tags").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tags", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-apigateway.RosApi.ConstParametersProperty",
         jsii_struct_bases=[],
         name_mapping={
             "const_value": "constValue",
@@ -2077,14 +2300,20 @@
         ) -> None:
             '''
             :param const_value: 
             :param location: 
             :param service_parameter_name: 
             :param description: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosApi.ConstParametersProperty.__init__)
+                check_type(argname="argument const_value", value=const_value, expected_type=type_hints["const_value"])
+                check_type(argname="argument location", value=location, expected_type=type_hints["location"])
+                check_type(argname="argument service_parameter_name", value=service_parameter_name, expected_type=type_hints["service_parameter_name"])
+                check_type(argname="argument description", value=description, expected_type=type_hints["description"])
             self._values: typing.Dict[str, typing.Any] = {
                 "const_value": const_value,
                 "location": location,
                 "service_parameter_name": service_parameter_name,
             }
             if description is not None:
                 self._values["description"] = description
@@ -2157,14 +2386,19 @@
             description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param code: 
             :param message: 
             :param description: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosApi.ErrorCodeSamplesProperty.__init__)
+                check_type(argname="argument code", value=code, expected_type=type_hints["code"])
+                check_type(argname="argument message", value=message, expected_type=type_hints["message"])
+                check_type(argname="argument description", value=description, expected_type=type_hints["description"])
             self._values: typing.Dict[str, typing.Any] = {
                 "code": code,
                 "message": message,
             }
             if description is not None:
                 self._values["description"] = description
 
@@ -2252,14 +2486,28 @@
             :param method: 
             :param only_business_path: 
             :param path: 
             :param qualifier: 
             :param role_arn: 
             :param service_name: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosApi.FunctionComputeConfigProperty.__init__)
+                check_type(argname="argument content_type_catagory", value=content_type_catagory, expected_type=type_hints["content_type_catagory"])
+                check_type(argname="argument content_type_value", value=content_type_value, expected_type=type_hints["content_type_value"])
+                check_type(argname="argument fc_base_url", value=fc_base_url, expected_type=type_hints["fc_base_url"])
+                check_type(argname="argument fc_region_id", value=fc_region_id, expected_type=type_hints["fc_region_id"])
+                check_type(argname="argument fc_type", value=fc_type, expected_type=type_hints["fc_type"])
+                check_type(argname="argument function_name", value=function_name, expected_type=type_hints["function_name"])
+                check_type(argname="argument method", value=method, expected_type=type_hints["method"])
+                check_type(argname="argument only_business_path", value=only_business_path, expected_type=type_hints["only_business_path"])
+                check_type(argname="argument path", value=path, expected_type=type_hints["path"])
+                check_type(argname="argument qualifier", value=qualifier, expected_type=type_hints["qualifier"])
+                check_type(argname="argument role_arn", value=role_arn, expected_type=type_hints["role_arn"])
+                check_type(argname="argument service_name", value=service_name, expected_type=type_hints["service_name"])
             self._values: typing.Dict[str, typing.Any] = {}
             if content_type_catagory is not None:
                 self._values["content_type_catagory"] = content_type_catagory
             if content_type_value is not None:
                 self._values["content_type_value"] = content_type_value
             if fc_base_url is not None:
                 self._values["fc_base_url"] = fc_base_url
@@ -2428,14 +2676,18 @@
             header_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             header_value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param header_name: 
             :param header_value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosApi.MockHeadersProperty.__init__)
+                check_type(argname="argument header_name", value=header_name, expected_type=type_hints["header_name"])
+                check_type(argname="argument header_value", value=header_value, expected_type=type_hints["header_value"])
             self._values: typing.Dict[str, typing.Any] = {
                 "header_name": header_name,
                 "header_value": header_value,
             }
 
         @builtins.property
         def header_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -2487,14 +2739,20 @@
         ) -> None:
             '''
             :param open_id_api_type: 
             :param id_token_param_name: 
             :param public_key: 
             :param public_key_id: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosApi.OpenIdConnectConfigProperty.__init__)
+                check_type(argname="argument open_id_api_type", value=open_id_api_type, expected_type=type_hints["open_id_api_type"])
+                check_type(argname="argument id_token_param_name", value=id_token_param_name, expected_type=type_hints["id_token_param_name"])
+                check_type(argname="argument public_key", value=public_key, expected_type=type_hints["public_key"])
+                check_type(argname="argument public_key_id", value=public_key_id, expected_type=type_hints["public_key_id"])
             self._values: typing.Dict[str, typing.Any] = {
                 "open_id_api_type": open_id_api_type,
             }
             if id_token_param_name is not None:
                 self._values["id_token_param_name"] = id_token_param_name
             if public_key is not None:
                 self._values["public_key"] = public_key
@@ -2580,14 +2838,22 @@
             :param request_http_method: 
             :param request_mode: 
             :param request_path: 
             :param request_protocol: 
             :param body_format: 
             :param post_body_description: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosApi.RequestConfigProperty.__init__)
+                check_type(argname="argument request_http_method", value=request_http_method, expected_type=type_hints["request_http_method"])
+                check_type(argname="argument request_mode", value=request_mode, expected_type=type_hints["request_mode"])
+                check_type(argname="argument request_path", value=request_path, expected_type=type_hints["request_path"])
+                check_type(argname="argument request_protocol", value=request_protocol, expected_type=type_hints["request_protocol"])
+                check_type(argname="argument body_format", value=body_format, expected_type=type_hints["body_format"])
+                check_type(argname="argument post_body_description", value=post_body_description, expected_type=type_hints["post_body_description"])
             self._values: typing.Dict[str, typing.Any] = {
                 "request_http_method": request_http_method,
                 "request_mode": request_mode,
                 "request_path": request_path,
                 "request_protocol": request_protocol,
             }
             if body_format is not None:
@@ -2723,14 +2989,32 @@
             :param json_scheme: 
             :param max_length: 
             :param max_value: 
             :param min_length: 
             :param min_value: 
             :param regular_expression: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosApi.RequestParametersProperty.__init__)
+                check_type(argname="argument api_parameter_name", value=api_parameter_name, expected_type=type_hints["api_parameter_name"])
+                check_type(argname="argument location", value=location, expected_type=type_hints["location"])
+                check_type(argname="argument parameter_type", value=parameter_type, expected_type=type_hints["parameter_type"])
+                check_type(argname="argument required", value=required, expected_type=type_hints["required"])
+                check_type(argname="argument default_value", value=default_value, expected_type=type_hints["default_value"])
+                check_type(argname="argument demo_value", value=demo_value, expected_type=type_hints["demo_value"])
+                check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+                check_type(argname="argument doc_order", value=doc_order, expected_type=type_hints["doc_order"])
+                check_type(argname="argument doc_show", value=doc_show, expected_type=type_hints["doc_show"])
+                check_type(argname="argument enum_value", value=enum_value, expected_type=type_hints["enum_value"])
+                check_type(argname="argument json_scheme", value=json_scheme, expected_type=type_hints["json_scheme"])
+                check_type(argname="argument max_length", value=max_length, expected_type=type_hints["max_length"])
+                check_type(argname="argument max_value", value=max_value, expected_type=type_hints["max_value"])
+                check_type(argname="argument min_length", value=min_length, expected_type=type_hints["min_length"])
+                check_type(argname="argument min_value", value=min_value, expected_type=type_hints["min_value"])
+                check_type(argname="argument regular_expression", value=regular_expression, expected_type=type_hints["regular_expression"])
             self._values: typing.Dict[str, typing.Any] = {
                 "api_parameter_name": api_parameter_name,
                 "location": location,
                 "parameter_type": parameter_type,
                 "required": required,
             }
             if default_value is not None:
@@ -2951,26 +3235,26 @@
     )
     class ServiceConfigProperty:
         def __init__(
             self,
             *,
             content_type_catagory: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             content_type_value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-            function_compute_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosApi.FunctionComputeConfigProperty"]] = None,
+            function_compute_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosApi.FunctionComputeConfigProperty", typing.Dict[str, typing.Any]]]] = None,
             mock: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-            mock_headers: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosApi.MockHeadersProperty"]]]] = None,
+            mock_headers: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosApi.MockHeadersProperty", typing.Dict[str, typing.Any]]]]]] = None,
             mock_result: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             mock_status_code: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
             service_address: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             service_http_method: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             service_path: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             service_protocol: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             service_time_out: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
             service_vpc_enable: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-            vpc_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosApi.VpcConfigProperty"]] = None,
+            vpc_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosApi.VpcConfigProperty", typing.Dict[str, typing.Any]]]] = None,
         ) -> None:
             '''
             :param content_type_catagory: 
             :param content_type_value: 
             :param function_compute_config: 
             :param mock: 
             :param mock_headers: 
@@ -2980,14 +3264,30 @@
             :param service_http_method: 
             :param service_path: 
             :param service_protocol: 
             :param service_time_out: 
             :param service_vpc_enable: 
             :param vpc_config: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosApi.ServiceConfigProperty.__init__)
+                check_type(argname="argument content_type_catagory", value=content_type_catagory, expected_type=type_hints["content_type_catagory"])
+                check_type(argname="argument content_type_value", value=content_type_value, expected_type=type_hints["content_type_value"])
+                check_type(argname="argument function_compute_config", value=function_compute_config, expected_type=type_hints["function_compute_config"])
+                check_type(argname="argument mock", value=mock, expected_type=type_hints["mock"])
+                check_type(argname="argument mock_headers", value=mock_headers, expected_type=type_hints["mock_headers"])
+                check_type(argname="argument mock_result", value=mock_result, expected_type=type_hints["mock_result"])
+                check_type(argname="argument mock_status_code", value=mock_status_code, expected_type=type_hints["mock_status_code"])
+                check_type(argname="argument service_address", value=service_address, expected_type=type_hints["service_address"])
+                check_type(argname="argument service_http_method", value=service_http_method, expected_type=type_hints["service_http_method"])
+                check_type(argname="argument service_path", value=service_path, expected_type=type_hints["service_path"])
+                check_type(argname="argument service_protocol", value=service_protocol, expected_type=type_hints["service_protocol"])
+                check_type(argname="argument service_time_out", value=service_time_out, expected_type=type_hints["service_time_out"])
+                check_type(argname="argument service_vpc_enable", value=service_vpc_enable, expected_type=type_hints["service_vpc_enable"])
+                check_type(argname="argument vpc_config", value=vpc_config, expected_type=type_hints["vpc_config"])
             self._values: typing.Dict[str, typing.Any] = {}
             if content_type_catagory is not None:
                 self._values["content_type_catagory"] = content_type_catagory
             if content_type_value is not None:
                 self._values["content_type_value"] = content_type_value
             if function_compute_config is not None:
                 self._values["function_compute_config"] = function_compute_config
@@ -3180,14 +3480,18 @@
             request_parameter_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             service_parameter_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param request_parameter_name: 
             :param service_parameter_name: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosApi.ServiceParametersMapProperty.__init__)
+                check_type(argname="argument request_parameter_name", value=request_parameter_name, expected_type=type_hints["request_parameter_name"])
+                check_type(argname="argument service_parameter_name", value=service_parameter_name, expected_type=type_hints["service_parameter_name"])
             self._values: typing.Dict[str, typing.Any] = {
                 "request_parameter_name": request_parameter_name,
                 "service_parameter_name": service_parameter_name,
             }
 
         @builtins.property
         def request_parameter_name(
@@ -3240,14 +3544,19 @@
             service_parameter_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param location: 
             :param parameter_type: 
             :param service_parameter_name: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosApi.ServiceParametersProperty.__init__)
+                check_type(argname="argument location", value=location, expected_type=type_hints["location"])
+                check_type(argname="argument parameter_type", value=parameter_type, expected_type=type_hints["parameter_type"])
+                check_type(argname="argument service_parameter_name", value=service_parameter_name, expected_type=type_hints["service_parameter_name"])
             self._values: typing.Dict[str, typing.Any] = {
                 "location": location,
                 "parameter_type": parameter_type,
                 "service_parameter_name": service_parameter_name,
             }
 
         @builtins.property
@@ -3316,14 +3625,21 @@
             '''
             :param location: 
             :param parameter_name: 
             :param service_parameter_name: 
             :param demo_value: 
             :param description: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosApi.SystemParametersProperty.__init__)
+                check_type(argname="argument location", value=location, expected_type=type_hints["location"])
+                check_type(argname="argument parameter_name", value=parameter_name, expected_type=type_hints["parameter_name"])
+                check_type(argname="argument service_parameter_name", value=service_parameter_name, expected_type=type_hints["service_parameter_name"])
+                check_type(argname="argument demo_value", value=demo_value, expected_type=type_hints["demo_value"])
+                check_type(argname="argument description", value=description, expected_type=type_hints["description"])
             self._values: typing.Dict[str, typing.Any] = {
                 "location": location,
                 "parameter_name": parameter_name,
                 "service_parameter_name": service_parameter_name,
             }
             if demo_value is not None:
                 self._values["demo_value"] = demo_value
@@ -3404,14 +3720,18 @@
             key: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param key: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosApi.TagsProperty.__init__)
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {
                 "key": key,
             }
             if value is not None:
                 self._values["value"] = value
 
         @builtins.property
@@ -3458,14 +3778,19 @@
             vpc_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param instance_id: 
             :param port: 
             :param vpc_id: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosApi.VpcConfigProperty.__init__)
+                check_type(argname="argument instance_id", value=instance_id, expected_type=type_hints["instance_id"])
+                check_type(argname="argument port", value=port, expected_type=type_hints["port"])
+                check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
             self._values: typing.Dict[str, typing.Any] = {
                 "instance_id": instance_id,
                 "port": port,
                 "vpc_id": vpc_id,
             }
 
         @builtins.property
@@ -3536,33 +3861,33 @@
 )
 class RosApiProps:
     def __init__(
         self,
         *,
         api_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         group_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        request_config: typing.Union[ros_cdk_core.IResolvable, RosApi.RequestConfigProperty],
+        request_config: typing.Union[ros_cdk_core.IResolvable, typing.Union[RosApi.RequestConfigProperty, typing.Dict[str, typing.Any]]],
         result_sample: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         result_type: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        service_config: typing.Union[ros_cdk_core.IResolvable, RosApi.ServiceConfigProperty],
+        service_config: typing.Union[ros_cdk_core.IResolvable, typing.Union[RosApi.ServiceConfigProperty, typing.Dict[str, typing.Any]]],
         visibility: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         app_code_auth_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         auth_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        const_parameters: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosApi.ConstParametersProperty]]]] = None,
+        const_parameters: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosApi.ConstParametersProperty, typing.Dict[str, typing.Any]]]]]] = None,
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         disable_internet: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
-        error_code_samples: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosApi.ErrorCodeSamplesProperty]]]] = None,
+        error_code_samples: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosApi.ErrorCodeSamplesProperty, typing.Dict[str, typing.Any]]]]]] = None,
         fail_result_sample: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         force_nonce_check: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
-        open_id_connect_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosApi.OpenIdConnectConfigProperty]] = None,
-        request_parameters: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosApi.RequestParametersProperty]]]] = None,
-        service_parameters: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosApi.ServiceParametersProperty]]]] = None,
-        service_parameters_map: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosApi.ServiceParametersMapProperty]]]] = None,
-        system_parameters: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosApi.SystemParametersProperty]]]] = None,
-        tags: typing.Optional[typing.Sequence[RosApi.TagsProperty]] = None,
+        open_id_connect_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosApi.OpenIdConnectConfigProperty, typing.Dict[str, typing.Any]]]] = None,
+        request_parameters: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosApi.RequestParametersProperty, typing.Dict[str, typing.Any]]]]]] = None,
+        service_parameters: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosApi.ServiceParametersProperty, typing.Dict[str, typing.Any]]]]]] = None,
+        service_parameters_map: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosApi.ServiceParametersMapProperty, typing.Dict[str, typing.Any]]]]]] = None,
+        system_parameters: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosApi.SystemParametersProperty, typing.Dict[str, typing.Any]]]]]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union[RosApi.TagsProperty, typing.Dict[str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::ApiGateway::Api``.
 
         :param api_name: 
         :param group_id: 
         :param request_config: 
         :param result_sample: 
@@ -3580,14 +3905,37 @@
         :param open_id_connect_config: 
         :param request_parameters: 
         :param service_parameters: 
         :param service_parameters_map: 
         :param system_parameters: 
         :param tags: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosApiProps.__init__)
+            check_type(argname="argument api_name", value=api_name, expected_type=type_hints["api_name"])
+            check_type(argname="argument group_id", value=group_id, expected_type=type_hints["group_id"])
+            check_type(argname="argument request_config", value=request_config, expected_type=type_hints["request_config"])
+            check_type(argname="argument result_sample", value=result_sample, expected_type=type_hints["result_sample"])
+            check_type(argname="argument result_type", value=result_type, expected_type=type_hints["result_type"])
+            check_type(argname="argument service_config", value=service_config, expected_type=type_hints["service_config"])
+            check_type(argname="argument visibility", value=visibility, expected_type=type_hints["visibility"])
+            check_type(argname="argument app_code_auth_type", value=app_code_auth_type, expected_type=type_hints["app_code_auth_type"])
+            check_type(argname="argument auth_type", value=auth_type, expected_type=type_hints["auth_type"])
+            check_type(argname="argument const_parameters", value=const_parameters, expected_type=type_hints["const_parameters"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument disable_internet", value=disable_internet, expected_type=type_hints["disable_internet"])
+            check_type(argname="argument error_code_samples", value=error_code_samples, expected_type=type_hints["error_code_samples"])
+            check_type(argname="argument fail_result_sample", value=fail_result_sample, expected_type=type_hints["fail_result_sample"])
+            check_type(argname="argument force_nonce_check", value=force_nonce_check, expected_type=type_hints["force_nonce_check"])
+            check_type(argname="argument open_id_connect_config", value=open_id_connect_config, expected_type=type_hints["open_id_connect_config"])
+            check_type(argname="argument request_parameters", value=request_parameters, expected_type=type_hints["request_parameters"])
+            check_type(argname="argument service_parameters", value=service_parameters, expected_type=type_hints["service_parameters"])
+            check_type(argname="argument service_parameters_map", value=service_parameters_map, expected_type=type_hints["service_parameters_map"])
+            check_type(argname="argument system_parameters", value=system_parameters, expected_type=type_hints["system_parameters"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
         self._values: typing.Dict[str, typing.Any] = {
             "api_name": api_name,
             "group_id": group_id,
             "request_config": request_config,
             "result_sample": result_sample,
             "result_type": result_type,
             "service_config": service_config,
@@ -3861,130 +4209,151 @@
 ):
     '''A ROS template type:  ``ALIYUN::ApiGateway::App``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosAppProps",
+        props: typing.Union["RosAppProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::ApiGateway::App``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosApp.__init__)
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
+            type_hints = typing.get_type_hints(RosApp._render_properties)
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
         :Attribute: AppId: The id of the created APP
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAppId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAppKey")
     def attr_app_key(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: AppKey: The key of the APP
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAppKey"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAppSecret")
     def attr_app_secret(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: AppSecret: The secret of the APP
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAppSecret"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTags")
     def attr_tags(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Tags: Tags of app
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTags"))
 
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
         :Property: appName: The name of the App.Need [4, 26] Chinese\\English\\Number characters or "_",and should start with Chinese/English character.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "appName"))
 
     @app_name.setter
     def app_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApp, "app_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "appName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApp, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: description: Description of the App, less than 180 characters.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApp, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tags")
     def tags(self) -> typing.Optional[typing.List["RosApp.TagsProperty"]]:
         '''
         :Property: tags: Tags to attach to app. Max support 20 tags to add during create app. Each tag with two properties Key and Value, and Key is required.
         '''
         return typing.cast(typing.Optional[typing.List["RosApp.TagsProperty"]], jsii.get(self, "tags"))
 
     @tags.setter
     def tags(self, value: typing.Optional[typing.List["RosApp.TagsProperty"]]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApp, "tags").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tags", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-apigateway.RosApp.TagsProperty",
         jsii_struct_bases=[],
         name_mapping={"key": "key", "value": "value"},
     )
@@ -3995,14 +4364,18 @@
             key: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param key: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosApp.TagsProperty.__init__)
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {
                 "key": key,
             }
             if value is not None:
                 self._values["value"] = value
 
         @builtins.property
@@ -4043,22 +4416,27 @@
 )
 class RosAppProps:
     def __init__(
         self,
         *,
         app_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence[RosApp.TagsProperty]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union[RosApp.TagsProperty, typing.Dict[str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::ApiGateway::App``.
 
         :param app_name: 
         :param description: 
         :param tags: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosAppProps.__init__)
+            check_type(argname="argument app_name", value=app_name, expected_type=type_hints["app_name"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
         self._values: typing.Dict[str, typing.Any] = {
             "app_name": app_name,
         }
         if description is not None:
             self._values["description"] = description
         if tags is not None:
             self._values["tags"] = tags
@@ -4109,136 +4487,163 @@
 ):
     '''A ROS template type:  ``ALIYUN::ApiGateway::Authorization``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosAuthorizationProps",
+        props: typing.Union["RosAuthorizationProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::ApiGateway::Authorization``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosAuthorization.__init__)
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
+            type_hints = typing.get_type_hints(RosAuthorization._render_properties)
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
     @jsii.member(jsii_name="apiIds")
     def api_ids(
         self,
     ) -> typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]:
         '''
         :Property: apiIds: APIs to authorize.
         '''
         return typing.cast(typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable], jsii.get(self, "apiIds"))
 
     @api_ids.setter
     def api_ids(
         self,
         value: typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAuthorization, "api_ids").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "apiIds", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="appIds")
     def app_ids(
         self,
     ) -> typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]:
         '''
         :Property: appIds: APPs are authorized to APIs.
         '''
         return typing.cast(typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable], jsii.get(self, "appIds"))
 
     @app_ids.setter
     def app_ids(
         self,
         value: typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAuthorization, "app_ids").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "appIds", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         '''A factory method that creates a new instance of this class from an object containing the properties of this ROS resource.'''
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAuthorization, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="groupId")
     def group_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: groupId: The id of the group.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "groupId"))
 
     @group_id.setter
     def group_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAuthorization, "group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "groupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="stageName")
     def stage_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: stageName: Authorize in this stage.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "stageName"))
 
     @stage_name.setter
     def stage_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAuthorization, "stage_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "stageName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: description: Description of the authorization, less than 180 characters.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAuthorization, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-apigateway.RosAuthorizationProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -4263,14 +4668,21 @@
 
         :param api_ids: 
         :param app_ids: 
         :param group_id: 
         :param stage_name: 
         :param description: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosAuthorizationProps.__init__)
+            check_type(argname="argument api_ids", value=api_ids, expected_type=type_hints["api_ids"])
+            check_type(argname="argument app_ids", value=app_ids, expected_type=type_hints["app_ids"])
+            check_type(argname="argument group_id", value=group_id, expected_type=type_hints["group_id"])
+            check_type(argname="argument stage_name", value=stage_name, expected_type=type_hints["stage_name"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
         self._values: typing.Dict[str, typing.Any] = {
             "api_ids": api_ids,
             "app_ids": app_ids,
             "group_id": group_id,
             "stage_name": stage_name,
         }
         if description is not None:
@@ -4345,143 +4757,170 @@
 ):
     '''A ROS template type:  ``ALIYUN::ApiGateway::CustomDomain``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosCustomDomainProps",
+        props: typing.Union["RosCustomDomainProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::ApiGateway::CustomDomain``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosCustomDomain.__init__)
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
+            type_hints = typing.get_type_hints(RosCustomDomain._render_properties)
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
     @jsii.member(jsii_name="attrCertificateId")
     def attr_certificate_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: CertificateId: The id of the certificate.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCertificateId"))
 
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
         :Property: domainName: Custom domain name.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "domainName"))
 
     @domain_name.setter
     def domain_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCustomDomain, "domain_name").fset)
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
+            type_hints = typing.get_type_hints(getattr(RosCustomDomain, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="groupId")
     def group_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: groupId: The id of the Group.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "groupId"))
 
     @group_id.setter
     def group_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCustomDomain, "group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "groupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="certificateBody")
     def certificate_body(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: certificateBody: SSL certificate body.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "certificateBody"))
 
     @certificate_body.setter
     def certificate_body(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCustomDomain, "certificate_body").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "certificateBody", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="certificateName")
     def certificate_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: certificateName: SSL certificate name.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "certificateName"))
 
     @certificate_name.setter
     def certificate_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCustomDomain, "certificate_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "certificateName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="certificatePrivateKey")
     def certificate_private_key(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: certificatePrivateKey: SSL certificate key.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "certificatePrivateKey"))
 
     @certificate_private_key.setter
     def certificate_private_key(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCustomDomain, "certificate_private_key").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "certificatePrivateKey", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-apigateway.RosCustomDomainProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -4506,14 +4945,21 @@
 
         :param domain_name: 
         :param group_id: 
         :param certificate_body: 
         :param certificate_name: 
         :param certificate_private_key: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosCustomDomainProps.__init__)
+            check_type(argname="argument domain_name", value=domain_name, expected_type=type_hints["domain_name"])
+            check_type(argname="argument group_id", value=group_id, expected_type=type_hints["group_id"])
+            check_type(argname="argument certificate_body", value=certificate_body, expected_type=type_hints["certificate_body"])
+            check_type(argname="argument certificate_name", value=certificate_name, expected_type=type_hints["certificate_name"])
+            check_type(argname="argument certificate_private_key", value=certificate_private_key, expected_type=type_hints["certificate_private_key"])
         self._values: typing.Dict[str, typing.Any] = {
             "domain_name": domain_name,
             "group_id": group_id,
         }
         if certificate_body is not None:
             self._values["certificate_body"] = certificate_body
         if certificate_name is not None:
@@ -4588,134 +5034,161 @@
 ):
     '''A ROS template type:  ``ALIYUN::ApiGateway::Deployment``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosDeploymentProps",
+        props: typing.Union["RosDeploymentProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::ApiGateway::Deployment``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDeployment.__init__)
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
+            type_hints = typing.get_type_hints(RosDeployment._render_properties)
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
     @jsii.member(jsii_name="apiId")
     def api_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: apiId: The id of the API.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "apiId"))
 
     @api_id.setter
     def api_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDeployment, "api_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "apiId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         '''A factory method that creates a new instance of this class from an object containing the properties of this ROS resource.'''
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDeployment, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="groupId")
     def group_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: groupId: The id of the Group.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "groupId"))
 
     @group_id.setter
     def group_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDeployment, "group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "groupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="stageName")
     def stage_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: stageName: Bind traffic in this stage.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "stageName"))
 
     @stage_name.setter
     def stage_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDeployment, "stage_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "stageName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: description: Description of the deployment, less than 180 characters.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDeployment, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="historyVersion")
     def history_version(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: historyVersion: The history version.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "historyVersion"))
 
     @history_version.setter
     def history_version(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDeployment, "history_version").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "historyVersion", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-apigateway.RosDeploymentProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -4740,14 +5213,21 @@
 
         :param api_id: 
         :param group_id: 
         :param stage_name: 
         :param description: 
         :param history_version: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDeploymentProps.__init__)
+            check_type(argname="argument api_id", value=api_id, expected_type=type_hints["api_id"])
+            check_type(argname="argument group_id", value=group_id, expected_type=type_hints["group_id"])
+            check_type(argname="argument stage_name", value=stage_name, expected_type=type_hints["stage_name"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument history_version", value=history_version, expected_type=type_hints["history_version"])
         self._values: typing.Dict[str, typing.Any] = {
             "api_id": api_id,
             "group_id": group_id,
             "stage_name": stage_name,
         }
         if description is not None:
             self._values["description"] = description
@@ -4820,147 +5300,171 @@
 ):
     '''A ROS template type:  ``ALIYUN::ApiGateway::Group``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosGroupProps",
+        props: typing.Union["RosGroupProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::ApiGateway::Group``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosGroup.__init__)
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
+            type_hints = typing.get_type_hints(RosGroup._render_properties)
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
     @jsii.member(jsii_name="attrGroupId")
     def attr_group_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: GroupId: The id of the created Group resource
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrGroupId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSubDomain")
     def attr_sub_domain(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: SubDomain: The sub domain assigned to the Group by the system
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSubDomain"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTags")
     def attr_tags(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Tags: Tags of app
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTags"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosGroup, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="groupName")
     def group_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: groupName: The name of the Group.Need [4, 50] Chinese\\English\\Number characters or "_",and should start with Chinese/English character.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "groupName"))
 
     @group_name.setter
     def group_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGroup, "group_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "groupName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: description: Description of the Group, less than 180 characters.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGroup, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceId")
     def instance_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: instanceId: API gateway instance ID. For example, "api-shared-vpc-001" means vpc instance, while "api-shared-classic-001" means classic instance.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "instanceId"))
 
     @instance_id.setter
     def instance_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGroup, "instance_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="internetEnable")
     def internet_enable(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: internetEnable: Enable or disable internet subdomain. True for enable.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "internetEnable"))
 
     @internet_enable.setter
     def internet_enable(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGroup, "internet_enable").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internetEnable", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="passthroughHeaders")
     def passthrough_headers(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -4970,46 +5474,55 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "passthroughHeaders"))
 
     @passthrough_headers.setter
     def passthrough_headers(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGroup, "passthrough_headers").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "passthroughHeaders", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tags")
     def tags(self) -> typing.Optional[typing.List["RosGroup.TagsProperty"]]:
         '''
         :Property: tags: Tags to attach to group. Max support 20 tags to add during create group. Each tag with two properties Key and Value, and Key is required.
         '''
         return typing.cast(typing.Optional[typing.List["RosGroup.TagsProperty"]], jsii.get(self, "tags"))
 
     @tags.setter
     def tags(
         self,
         value: typing.Optional[typing.List["RosGroup.TagsProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGroup, "tags").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tags", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vpcIntranetEnable")
     def vpc_intranet_enable(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: vpcIntranetEnable: Enable or disable VPC intranet subdomain. True for enable.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "vpcIntranetEnable"))
 
     @vpc_intranet_enable.setter
     def vpc_intranet_enable(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGroup, "vpc_intranet_enable").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vpcIntranetEnable", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-apigateway.RosGroup.TagsProperty",
         jsii_struct_bases=[],
         name_mapping={"key": "key", "value": "value"},
     )
@@ -5020,14 +5533,18 @@
             key: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param key: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosGroup.TagsProperty.__init__)
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {
                 "key": key,
             }
             if value is not None:
                 self._values["value"] = value
 
         @builtins.property
@@ -5079,27 +5596,36 @@
         self,
         *,
         group_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         instance_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         internet_enable: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         passthrough_headers: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence[RosGroup.TagsProperty]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union[RosGroup.TagsProperty, typing.Dict[str, typing.Any]]]] = None,
         vpc_intranet_enable: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::ApiGateway::Group``.
 
         :param group_name: 
         :param description: 
         :param instance_id: 
         :param internet_enable: 
         :param passthrough_headers: 
         :param tags: 
         :param vpc_intranet_enable: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosGroupProps.__init__)
+            check_type(argname="argument group_name", value=group_name, expected_type=type_hints["group_name"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument instance_id", value=instance_id, expected_type=type_hints["instance_id"])
+            check_type(argname="argument internet_enable", value=internet_enable, expected_type=type_hints["internet_enable"])
+            check_type(argname="argument passthrough_headers", value=passthrough_headers, expected_type=type_hints["passthrough_headers"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument vpc_intranet_enable", value=vpc_intranet_enable, expected_type=type_hints["vpc_intranet_enable"])
         self._values: typing.Dict[str, typing.Any] = {
             "group_name": group_name,
         }
         if description is not None:
             self._values["description"] = description
         if instance_id is not None:
             self._values["instance_id"] = instance_id
@@ -5201,166 +5727,187 @@
 ):
     '''A ROS template type:  ``ALIYUN::ApiGateway::Instance``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosInstanceProps",
+        props: typing.Union["RosInstanceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::ApiGateway::Instance``.
 
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
     @jsii.member(jsii_name="attrEgressIpv6Enable")
     def attr_egress_ipv6_enable(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: EgressIpv6Enable: Whether enable egress IPV6.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrEgressIpv6Enable"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceId")
     def attr_instance_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: InstanceId: Instance ID.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceType")
     def attr_instance_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: InstanceType: Instance type.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInternetEgressAddress")
     def attr_internet_egress_address(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: InternetEgressAddress: Internet egress dddress.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInternetEgressAddress"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSupportIpv6")
     def attr_support_ipv6(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: SupportIpv6: Whether support IPV6.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSupportIpv6"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVpcEgressAddress")
     def attr_vpc_egress_address(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: VpcEgressAddress: VPC network egress address.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVpcEgressAddress"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVpcIntranetEnable")
     def attr_vpc_intranet_enable(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: VpcIntranetEnable: Whether enable VPC intranet.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVpcIntranetEnable"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVpcSlbIntranetEnable")
     def attr_vpc_slb_intranet_enable(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: VpcSlbIntranetEnable: Whether enable VPC SLB intranet.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVpcSlbIntranetEnable"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosInstance, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="httpsPolicy")
     def https_policy(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: httpsPolicy: HTTPS security policy. Valid values: HTTPS2_TLS1_0, HTTPS2_TLS1_2, HTTPS1_1_TLS1_0
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "httpsPolicy"))
 
     @https_policy.setter
     def https_policy(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "https_policy").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "httpsPolicy", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceName")
     def instance_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: instanceName: Instance name
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "instanceName"))
 
     @instance_name.setter
     def instance_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "instance_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceSpec")
     def instance_spec(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: instanceSpec: Instance specification. For example: api.s1.small
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "instanceSpec"))
 
     @instance_spec.setter
     def instance_spec(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "instance_spec").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceSpec", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="zoneId")
     def zone_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         zoneId: Zone to which the instance belongs. For example: cn-beijing-MAZ2(f,g).
         Pleas call DescribeZones to get supported zone list.
@@ -5368,17 +5915,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "zoneId"))
 
     @zone_id.setter
     def zone_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "zone_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "zoneId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="autoPay")
     def auto_pay(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5389,97 +5939,115 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "autoPay"))
 
     @auto_pay.setter
     def auto_pay(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "auto_pay").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "autoPay", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="chargeType")
     def charge_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: chargeType: The billing method of the router interface. Valid values: PrePaid (Subscription), PostPaid (default, Pay-As-You-Go). Default value: PostPaid.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "chargeType"))
 
     @charge_type.setter
     def charge_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "charge_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "chargeType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="deletionForce")
     def deletion_force(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: deletionForce: Whether force delete the instance even if its status is START_FAILED. Default value is false.
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
     @jsii.member(jsii_name="duration")
     def duration(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: duration: Prepaid time period. It could be from 1 to 9 when PricingCycle is Month, or 1 to 3 when PricingCycle is Year. Default value is 3.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "duration"))
 
     @duration.setter
     def duration(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "duration").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "duration", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="pricingCycle")
     def pricing_cycle(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: pricingCycle: Unit of the payment cycle. It could be Month (default) or Year.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "pricingCycle"))
 
     @pricing_cycle.setter
     def pricing_cycle(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "pricing_cycle").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "pricingCycle", value)
 
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
         jsii_type="@alicloud/ros-cdk-apigateway.RosInstance.TagsProperty",
         jsii_struct_bases=[],
         name_mapping={"key": "key", "value": "value"},
     )
@@ -5490,14 +6058,18 @@
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
@@ -5556,29 +6128,41 @@
         instance_spec: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         zone_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         auto_pay: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         charge_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         deletion_force: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         duration: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         pricing_cycle: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence[RosInstance.TagsProperty]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union[RosInstance.TagsProperty, typing.Dict[str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::ApiGateway::Instance``.
 
         :param https_policy: 
         :param instance_name: 
         :param instance_spec: 
         :param zone_id: 
         :param auto_pay: 
         :param charge_type: 
         :param deletion_force: 
         :param duration: 
         :param pricing_cycle: 
         :param tags: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosInstanceProps.__init__)
+            check_type(argname="argument https_policy", value=https_policy, expected_type=type_hints["https_policy"])
+            check_type(argname="argument instance_name", value=instance_name, expected_type=type_hints["instance_name"])
+            check_type(argname="argument instance_spec", value=instance_spec, expected_type=type_hints["instance_spec"])
+            check_type(argname="argument zone_id", value=zone_id, expected_type=type_hints["zone_id"])
+            check_type(argname="argument auto_pay", value=auto_pay, expected_type=type_hints["auto_pay"])
+            check_type(argname="argument charge_type", value=charge_type, expected_type=type_hints["charge_type"])
+            check_type(argname="argument deletion_force", value=deletion_force, expected_type=type_hints["deletion_force"])
+            check_type(argname="argument duration", value=duration, expected_type=type_hints["duration"])
+            check_type(argname="argument pricing_cycle", value=pricing_cycle, expected_type=type_hints["pricing_cycle"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
         self._values: typing.Dict[str, typing.Any] = {
             "https_policy": https_policy,
             "instance_name": instance_name,
             "instance_spec": instance_spec,
             "zone_id": zone_id,
         }
         if auto_pay is not None:
@@ -5714,100 +6298,118 @@
 ):
     '''A ROS template type:  ``ALIYUN::ApiGateway::LogConfig``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosLogConfigProps",
+        props: typing.Union["RosLogConfigProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::ApiGateway::LogConfig``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosLogConfig.__init__)
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
+            type_hints = typing.get_type_hints(RosLogConfig._render_properties)
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
     @jsii.member(jsii_name="attrSlsLogStore")
     def attr_sls_log_store(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: SlsLogStore: Logstore name of SLS
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSlsLogStore"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSlsProject")
     def attr_sls_project(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: SlsProject: Project name of SLS
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSlsProject"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosLogConfig, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="slsLogStore")
     def sls_log_store(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: slsLogStore: Logstore name of SLS
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "slsLogStore"))
 
     @sls_log_store.setter
     def sls_log_store(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLogConfig, "sls_log_store").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "slsLogStore", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="slsProject")
     def sls_project(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: slsProject: Project name of SLS
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "slsProject"))
 
     @sls_project.setter
     def sls_project(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLogConfig, "sls_project").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "slsProject", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-apigateway.RosLogConfigProps",
     jsii_struct_bases=[],
     name_mapping={"sls_log_store": "slsLogStore", "sls_project": "slsProject"},
@@ -5820,14 +6422,18 @@
         sls_project: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::ApiGateway::LogConfig``.
 
         :param sls_log_store: 
         :param sls_project: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosLogConfigProps.__init__)
+            check_type(argname="argument sls_log_store", value=sls_log_store, expected_type=type_hints["sls_log_store"])
+            check_type(argname="argument sls_project", value=sls_project, expected_type=type_hints["sls_project"])
         self._values: typing.Dict[str, typing.Any] = {
             "sls_log_store": sls_log_store,
             "sls_project": sls_project,
         }
 
     @builtins.property
     def sls_log_store(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -5866,171 +6472,198 @@
 ):
     '''A ROS template type:  ``ALIYUN::ApiGateway::Plugin``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosPluginProps",
+        props: typing.Union["RosPluginProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::ApiGateway::Plugin``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosPlugin.__init__)
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
+            type_hints = typing.get_type_hints(RosPlugin._render_properties)
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
     @jsii.member(jsii_name="attrDescription")
     def attr_description(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Description: The description of the plug-in, which cannot exceed 200 characters.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDescription"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPluginData")
     def attr_plugin_data(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: PluginData: The definition statement of the plug-in. Plug-in definition statements in the JSON and YAML formats are supported.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPluginData"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPluginId")
     def attr_plugin_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: PluginId: The generated plugin ID.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPluginId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPluginName")
     def attr_plugin_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: PluginName: The name of the plug-in that you want to create. It can contain uppercase English letters, lowercase English letters, Chinese characters, numbers, and underscores (). It must be 4 to 50 characters in length and cannot start with an underscore ().
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPluginName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPluginType")
     def attr_plugin_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: PluginType: The type of the plug-in. Valid values: ipControl: indicates IP address-based access control. trafficControl: indicates throttling. backendSignature: indicates backend signature. jwtAuth: indicates JWT (OpenId Connect). cors: indicates cross-origin resource access (CORS). caching: indicates caching.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPluginType"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosPlugin, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="pluginData")
     def plugin_data(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: pluginData: The definition statement of the plug-in. Plug-in definition statements in the JSON and YAML formats are supported.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "pluginData"))
 
     @plugin_data.setter
     def plugin_data(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPlugin, "plugin_data").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "pluginData", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="pluginName")
     def plugin_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: pluginName: The name of the plug-in that you want to create. It can contain uppercase English letters, lowercase English letters, Chinese characters, numbers, and underscores (). It must be 4 to 50 characters in length and cannot start with an underscore ().
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "pluginName"))
 
     @plugin_name.setter
     def plugin_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPlugin, "plugin_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "pluginName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="pluginType")
     def plugin_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: pluginType: The type of the plug-in. Valid values: ipControl: indicates IP address-based access control. trafficControl: indicates throttling. backendSignature: indicates backend signature. jwtAuth: indicates JWT (OpenId Connect). cors: indicates cross-origin resource access (CORS). caching: indicates caching.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "pluginType"))
 
     @plugin_type.setter
     def plugin_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPlugin, "plugin_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "pluginType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: description: The description of the plug-in, which cannot exceed 200 characters.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPlugin, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tags")
     def tags(self) -> typing.Optional[typing.List["RosPlugin.TagsProperty"]]:
         '''
         :Property: tags: Tags to attach to instance. Max support 20 tags to add during create instance. Each tag with two properties Key and Value, and Key is required.
         '''
         return typing.cast(typing.Optional[typing.List["RosPlugin.TagsProperty"]], jsii.get(self, "tags"))
 
     @tags.setter
     def tags(
         self,
         value: typing.Optional[typing.List["RosPlugin.TagsProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPlugin, "tags").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tags", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-apigateway.RosPlugin.TagsProperty",
         jsii_struct_bases=[],
         name_mapping={"key": "key", "value": "value"},
     )
@@ -6041,14 +6674,18 @@
             key: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param key: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosPlugin.TagsProperty.__init__)
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {
                 "key": key,
             }
             if value is not None:
                 self._values["value"] = value
 
         @builtins.property
@@ -6089,103 +6726,121 @@
 ):
     '''A ROS template type:  ``ALIYUN::ApiGateway::PluginAttachment``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosPluginAttachmentProps",
+        props: typing.Union["RosPluginAttachmentProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::ApiGateway::PluginAttachment``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosPluginAttachment.__init__)
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
+            type_hints = typing.get_type_hints(RosPluginAttachment._render_properties)
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
     @jsii.member(jsii_name="attrApiId")
     def attr_api_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ApiId: The api id.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrApiId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPluginId")
     def attr_plugin_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: PluginId: The plugin id.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPluginId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="apiId")
     def api_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: apiId: The ID of the API to which you want to bind the plug-in.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "apiId"))
 
     @api_id.setter
     def api_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPluginAttachment, "api_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "apiId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPluginAttachment, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="pluginId")
     def plugin_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: pluginId: The ID of the plugin that you want to bind.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "pluginId"))
 
     @plugin_id.setter
     def plugin_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPluginAttachment, "plugin_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "pluginId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="stageName")
     def stage_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         stageName: The name of the runtime environment. Valid values:
         RELEASE: indicates the release environment.
@@ -6195,14 +6850,17 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "stageName"))
 
     @stage_name.setter
     def stage_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPluginAttachment, "stage_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "stageName", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-apigateway.RosPluginAttachmentProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -6221,14 +6879,19 @@
     ) -> None:
         '''Properties for defining a ``ALIYUN::ApiGateway::PluginAttachment``.
 
         :param api_id: 
         :param plugin_id: 
         :param stage_name: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosPluginAttachmentProps.__init__)
+            check_type(argname="argument api_id", value=api_id, expected_type=type_hints["api_id"])
+            check_type(argname="argument plugin_id", value=plugin_id, expected_type=type_hints["plugin_id"])
+            check_type(argname="argument stage_name", value=stage_name, expected_type=type_hints["stage_name"])
         self._values: typing.Dict[str, typing.Any] = {
             "api_id": api_id,
             "plugin_id": plugin_id,
             "stage_name": stage_name,
         }
 
     @builtins.property
@@ -6290,24 +6953,31 @@
     def __init__(
         self,
         *,
         plugin_data: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         plugin_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         plugin_type: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence[RosPlugin.TagsProperty]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union[RosPlugin.TagsProperty, typing.Dict[str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::ApiGateway::Plugin``.
 
         :param plugin_data: 
         :param plugin_name: 
         :param plugin_type: 
         :param description: 
         :param tags: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosPluginProps.__init__)
+            check_type(argname="argument plugin_data", value=plugin_data, expected_type=type_hints["plugin_data"])
+            check_type(argname="argument plugin_name", value=plugin_name, expected_type=type_hints["plugin_name"])
+            check_type(argname="argument plugin_type", value=plugin_type, expected_type=type_hints["plugin_type"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
         self._values: typing.Dict[str, typing.Any] = {
             "plugin_data": plugin_data,
             "plugin_name": plugin_name,
             "plugin_type": plugin_type,
         }
         if description is not None:
             self._values["description"] = description
@@ -6378,224 +7048,269 @@
 ):
     '''A ROS template type:  ``ALIYUN::ApiGateway::Signature``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosSignatureProps",
+        props: typing.Union["RosSignatureProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::ApiGateway::Signature``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosSignature.__init__)
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
+            type_hints = typing.get_type_hints(RosSignature._render_properties)
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
     @jsii.member(jsii_name="attrSignatureId")
     def attr_signature_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: SignatureId: The id of the created signature
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSignatureId"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosSignature, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="signatureKey")
     def signature_key(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: signatureKey: The key of the signature.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "signatureKey"))
 
     @signature_key.setter
     def signature_key(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSignature, "signature_key").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "signatureKey", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="signatureName")
     def signature_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: signatureName: The name of the Signature.Need [4, 50] Chinese\\English\\Number characters or "_",and should start with Chinese/English character.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "signatureName"))
 
     @signature_name.setter
     def signature_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSignature, "signature_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "signatureName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="signatureSecret")
     def signature_secret(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: signatureSecret: The secret of the signature.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "signatureSecret"))
 
     @signature_secret.setter
     def signature_secret(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSignature, "signature_secret").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "signatureSecret", value)
 
 
 class RosSignatureBinding(
     ros_cdk_core.RosResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-apigateway.RosSignatureBinding",
 ):
     '''A ROS template type:  ``ALIYUN::ApiGateway::SignatureBinding``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosSignatureBindingProps",
+        props: typing.Union["RosSignatureBindingProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::ApiGateway::SignatureBinding``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosSignatureBinding.__init__)
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
+            type_hints = typing.get_type_hints(RosSignatureBinding._render_properties)
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
     @jsii.member(jsii_name="apiIds")
     def api_ids(
         self,
     ) -> typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]:
         '''
         :Property: apiIds: APIs to bind with the signature.
         '''
         return typing.cast(typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable], jsii.get(self, "apiIds"))
 
     @api_ids.setter
     def api_ids(
         self,
         value: typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSignatureBinding, "api_ids").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "apiIds", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         '''A factory method that creates a new instance of this class from an object containing the properties of this ROS resource.'''
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSignatureBinding, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="groupId")
     def group_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: groupId: The id of group.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "groupId"))
 
     @group_id.setter
     def group_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSignatureBinding, "group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "groupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="signatureId")
     def signature_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: signatureId: The id of the Signature.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "signatureId"))
 
     @signature_id.setter
     def signature_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSignatureBinding, "signature_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "signatureId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="stageName")
     def stage_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: stageName: Bind signature in this stage.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "stageName"))
 
     @stage_name.setter
     def stage_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSignatureBinding, "stage_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "stageName", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-apigateway.RosSignatureBindingProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -6617,14 +7332,20 @@
         '''Properties for defining a ``ALIYUN::ApiGateway::SignatureBinding``.
 
         :param api_ids: 
         :param group_id: 
         :param signature_id: 
         :param stage_name: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosSignatureBindingProps.__init__)
+            check_type(argname="argument api_ids", value=api_ids, expected_type=type_hints["api_ids"])
+            check_type(argname="argument group_id", value=group_id, expected_type=type_hints["group_id"])
+            check_type(argname="argument signature_id", value=signature_id, expected_type=type_hints["signature_id"])
+            check_type(argname="argument stage_name", value=stage_name, expected_type=type_hints["stage_name"])
         self._values: typing.Dict[str, typing.Any] = {
             "api_ids": api_ids,
             "group_id": group_id,
             "signature_id": signature_id,
             "stage_name": stage_name,
         }
 
@@ -6697,14 +7418,19 @@
     ) -> None:
         '''Properties for defining a ``ALIYUN::ApiGateway::Signature``.
 
         :param signature_key: 
         :param signature_name: 
         :param signature_secret: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosSignatureProps.__init__)
+            check_type(argname="argument signature_key", value=signature_key, expected_type=type_hints["signature_key"])
+            check_type(argname="argument signature_name", value=signature_name, expected_type=type_hints["signature_name"])
+            check_type(argname="argument signature_secret", value=signature_secret, expected_type=type_hints["signature_secret"])
         self._values: typing.Dict[str, typing.Any] = {
             "signature_key": signature_key,
             "signature_name": signature_name,
             "signature_secret": signature_secret,
         }
 
     @builtins.property
@@ -6753,102 +7479,123 @@
 ):
     '''A ROS template type:  ``ALIYUN::ApiGateway::StageConfig``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosStageConfigProps",
+        props: typing.Union["RosStageConfigProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::ApiGateway::StageConfig``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosStageConfig.__init__)
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
+            type_hints = typing.get_type_hints(RosStageConfig._render_properties)
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
+            type_hints = typing.get_type_hints(getattr(RosStageConfig, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="groupId")
     def group_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: groupId: The id of the Group.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "groupId"))
 
     @group_id.setter
     def group_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosStageConfig, "group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "groupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="stageName")
     def stage_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: stageName: The name of the Stage.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "stageName"))
 
     @stage_name.setter
     def stage_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosStageConfig, "stage_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "stageName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="variables")
     def variables(
         self,
     ) -> typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]:
         '''
         :Property: variables: Variables in the stage, key-value pairs.
         '''
         return typing.cast(typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]], jsii.get(self, "variables"))
 
     @variables.setter
     def variables(
         self,
         value: typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosStageConfig, "variables").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "variables", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-apigateway.RosStageConfigProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -6867,14 +7614,19 @@
     ) -> None:
         '''Properties for defining a ``ALIYUN::ApiGateway::StageConfig``.
 
         :param group_id: 
         :param stage_name: 
         :param variables: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosStageConfigProps.__init__)
+            check_type(argname="argument group_id", value=group_id, expected_type=type_hints["group_id"])
+            check_type(argname="argument stage_name", value=stage_name, expected_type=type_hints["stage_name"])
+            check_type(argname="argument variables", value=variables, expected_type=type_hints["variables"])
         self._values: typing.Dict[str, typing.Any] = {
             "group_id": group_id,
             "stage_name": stage_name,
             "variables": variables,
         }
 
     @builtins.property
@@ -6925,179 +7677,212 @@
 ):
     '''A ROS template type:  ``ALIYUN::ApiGateway::TrafficControl``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosTrafficControlProps",
+        props: typing.Union["RosTrafficControlProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::ApiGateway::TrafficControl``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosTrafficControl.__init__)
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
+            type_hints = typing.get_type_hints(RosTrafficControl._render_properties)
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
     @jsii.member(jsii_name="attrTrafficControlId")
     def attr_traffic_control_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TrafficControlId: The id of the traffic control
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTrafficControlId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="apiDefault")
     def api_default(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property: apiDefault: Default API traffic value.
         '''
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "apiDefault"))
 
     @api_default.setter
     def api_default(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTrafficControl, "api_default").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "apiDefault", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTrafficControl, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="trafficControlName")
     def traffic_control_name(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: trafficControlName: The name of the traffic control.Need [4, 50] Chinese\\English\\Number characters or "_",and should start with Chinese/English character.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "trafficControlName"))
 
     @traffic_control_name.setter
     def traffic_control_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTrafficControl, "traffic_control_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "trafficControlName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="trafficControlUnit")
     def traffic_control_unit(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: trafficControlUnit: Traffic control unit, DAY/HOUR/MINUTE.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "trafficControlUnit"))
 
     @traffic_control_unit.setter
     def traffic_control_unit(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTrafficControl, "traffic_control_unit").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "trafficControlUnit", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="appDefault")
     def app_default(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: appDefault: Default APP traffic value.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "appDefault"))
 
     @app_default.setter
     def app_default(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTrafficControl, "app_default").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "appDefault", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: description: Description of the traffic control, less than 180 characters.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTrafficControl, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="special")
     def special(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosTrafficControl.SpecialProperty"]]]]:
         '''
         :Property: special: Special traffic controls.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosTrafficControl.SpecialProperty"]]]], jsii.get(self, "special"))
 
     @special.setter
     def special(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosTrafficControl.SpecialProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTrafficControl, "special").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "special", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="userDefault")
     def user_default(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: userDefault: Default user traffic value.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "userDefault"))
 
     @user_default.setter
     def user_default(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTrafficControl, "user_default").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "userDefault", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-apigateway.RosTrafficControl.SpecialProperty",
         jsii_struct_bases=[],
         name_mapping={
             "special_key": "specialKey",
@@ -7114,14 +7899,19 @@
             traffic_value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param special_key: 
             :param special_type: 
             :param traffic_value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosTrafficControl.SpecialProperty.__init__)
+                check_type(argname="argument special_key", value=special_key, expected_type=type_hints["special_key"])
+                check_type(argname="argument special_type", value=special_type, expected_type=type_hints["special_type"])
+                check_type(argname="argument traffic_value", value=traffic_value, expected_type=type_hints["traffic_value"])
             self._values: typing.Dict[str, typing.Any] = {
                 "special_key": special_key,
                 "special_type": special_type,
                 "traffic_value": traffic_value,
             }
 
         @builtins.property
@@ -7170,119 +7960,143 @@
 ):
     '''A ROS template type:  ``ALIYUN::ApiGateway::TrafficControlBinding``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosTrafficControlBindingProps",
+        props: typing.Union["RosTrafficControlBindingProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::ApiGateway::TrafficControlBinding``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosTrafficControlBinding.__init__)
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
+            type_hints = typing.get_type_hints(RosTrafficControlBinding._render_properties)
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
     @jsii.member(jsii_name="apiIds")
     def api_ids(
         self,
     ) -> typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]:
         '''
         :Property: apiIds: APIs to bind with the traffic control.
         '''
         return typing.cast(typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable], jsii.get(self, "apiIds"))
 
     @api_ids.setter
     def api_ids(
         self,
         value: typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTrafficControlBinding, "api_ids").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "apiIds", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         '''A factory method that creates a new instance of this class from an object containing the properties of this ROS resource.'''
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTrafficControlBinding, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="groupId")
     def group_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: groupId: The id of group.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "groupId"))
 
     @group_id.setter
     def group_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTrafficControlBinding, "group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "groupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="stageName")
     def stage_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: stageName: Bind traffic in this stage.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "stageName"))
 
     @stage_name.setter
     def stage_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTrafficControlBinding, "stage_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "stageName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="trafficControlId")
     def traffic_control_id(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: trafficControlId: The id of traffic control.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "trafficControlId"))
 
     @traffic_control_id.setter
     def traffic_control_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTrafficControlBinding, "traffic_control_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "trafficControlId", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-apigateway.RosTrafficControlBindingProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -7304,14 +8118,20 @@
         '''Properties for defining a ``ALIYUN::ApiGateway::TrafficControlBinding``.
 
         :param api_ids: 
         :param group_id: 
         :param stage_name: 
         :param traffic_control_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosTrafficControlBindingProps.__init__)
+            check_type(argname="argument api_ids", value=api_ids, expected_type=type_hints["api_ids"])
+            check_type(argname="argument group_id", value=group_id, expected_type=type_hints["group_id"])
+            check_type(argname="argument stage_name", value=stage_name, expected_type=type_hints["stage_name"])
+            check_type(argname="argument traffic_control_id", value=traffic_control_id, expected_type=type_hints["traffic_control_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "api_ids": api_ids,
             "group_id": group_id,
             "stage_name": stage_name,
             "traffic_control_id": traffic_control_id,
         }
 
@@ -7385,27 +8205,36 @@
         self,
         *,
         api_default: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
         traffic_control_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         traffic_control_unit: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         app_default: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        special: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosTrafficControl.SpecialProperty]]]] = None,
+        special: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosTrafficControl.SpecialProperty, typing.Dict[str, typing.Any]]]]]] = None,
         user_default: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::ApiGateway::TrafficControl``.
 
         :param api_default: 
         :param traffic_control_name: 
         :param traffic_control_unit: 
         :param app_default: 
         :param description: 
         :param special: 
         :param user_default: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosTrafficControlProps.__init__)
+            check_type(argname="argument api_default", value=api_default, expected_type=type_hints["api_default"])
+            check_type(argname="argument traffic_control_name", value=traffic_control_name, expected_type=type_hints["traffic_control_name"])
+            check_type(argname="argument traffic_control_unit", value=traffic_control_unit, expected_type=type_hints["traffic_control_unit"])
+            check_type(argname="argument app_default", value=app_default, expected_type=type_hints["app_default"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument special", value=special, expected_type=type_hints["special"])
+            check_type(argname="argument user_default", value=user_default, expected_type=type_hints["user_default"])
         self._values: typing.Dict[str, typing.Any] = {
             "api_default": api_default,
             "traffic_control_name": traffic_control_name,
             "traffic_control_unit": traffic_control_unit,
         }
         if app_default is not None:
             self._values["app_default"] = app_default
@@ -7506,109 +8335,133 @@
 ):
     '''A ROS template type:  ``ALIYUN::ApiGateway::VpcAccessConfig``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosVpcAccessConfigProps",
+        props: typing.Union["RosVpcAccessConfigProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::ApiGateway::VpcAccessConfig``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosVpcAccessConfig.__init__)
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
+            type_hints = typing.get_type_hints(RosVpcAccessConfig._render_properties)
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
+            type_hints = typing.get_type_hints(getattr(RosVpcAccessConfig, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceId")
     def instance_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: instanceId: The id of the instance (ECS/SLB).
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "instanceId"))
 
     @instance_id.setter
     def instance_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosVpcAccessConfig, "instance_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="name")
     def name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: name: The name of one VPC access configuration.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "name"))
 
     @name.setter
     def name(self, value: typing.Union[builtins.str, ros_cdk_core.IResolvable]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosVpcAccessConfig, "name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "name", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="port")
     def port(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property: port: The port of the VPC.
         '''
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "port"))
 
     @port.setter
     def port(self, value: typing.Union[jsii.Number, ros_cdk_core.IResolvable]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosVpcAccessConfig, "port").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "port", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vpcId")
     def vpc_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: vpcId: The id of the VPC.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "vpcId"))
 
     @vpc_id.setter
     def vpc_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosVpcAccessConfig, "vpc_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vpcId", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-apigateway.RosVpcAccessConfigProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -7630,14 +8483,20 @@
         '''Properties for defining a ``ALIYUN::ApiGateway::VpcAccessConfig``.
 
         :param instance_id: 
         :param name: 
         :param port: 
         :param vpc_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosVpcAccessConfigProps.__init__)
+            check_type(argname="argument instance_id", value=instance_id, expected_type=type_hints["instance_id"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument port", value=port, expected_type=type_hints["port"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "instance_id": instance_id,
             "name": name,
             "port": port,
             "vpc_id": vpc_id,
         }
 
@@ -7696,31 +8555,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::ApiGateway::Signature``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "SignatureProps",
+        props: typing.Union["SignatureProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::ApiGateway::Signature``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Signature.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSignatureId")
     def attr_signature_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute SignatureId: The id of the created signature.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSignatureId"))
 
 
 class SignatureBinding(
@@ -7730,28 +8595,34 @@
 ):
     '''A ROS resource type:  ``ALIYUN::ApiGateway::SignatureBinding``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "SignatureBindingProps",
+        props: typing.Union["SignatureBindingProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::ApiGateway::SignatureBinding``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(SignatureBinding.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-apigateway.SignatureBindingProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -7773,14 +8644,20 @@
         '''Properties for defining a ``ALIYUN::ApiGateway::SignatureBinding``.
 
         :param api_ids: Property apiIds: APIs to bind with the signature.
         :param group_id: Property groupId: The id of group.
         :param signature_id: Property signatureId: The id of the Signature.
         :param stage_name: Property stageName: Bind signature in this stage.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(SignatureBindingProps.__init__)
+            check_type(argname="argument api_ids", value=api_ids, expected_type=type_hints["api_ids"])
+            check_type(argname="argument group_id", value=group_id, expected_type=type_hints["group_id"])
+            check_type(argname="argument signature_id", value=signature_id, expected_type=type_hints["signature_id"])
+            check_type(argname="argument stage_name", value=stage_name, expected_type=type_hints["stage_name"])
         self._values: typing.Dict[str, typing.Any] = {
             "api_ids": api_ids,
             "group_id": group_id,
             "signature_id": signature_id,
             "stage_name": stage_name,
         }
 
@@ -7845,14 +8722,19 @@
     ) -> None:
         '''Properties for defining a ``ALIYUN::ApiGateway::Signature``.
 
         :param signature_key: Property signatureKey: The key of the signature.
         :param signature_name: Property signatureName: The name of the Signature.Need [4, 50] Chinese\\English\\Number characters or "_",and should start with Chinese/English character.
         :param signature_secret: Property signatureSecret: The secret of the signature.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(SignatureProps.__init__)
+            check_type(argname="argument signature_key", value=signature_key, expected_type=type_hints["signature_key"])
+            check_type(argname="argument signature_name", value=signature_name, expected_type=type_hints["signature_name"])
+            check_type(argname="argument signature_secret", value=signature_secret, expected_type=type_hints["signature_secret"])
         self._values: typing.Dict[str, typing.Any] = {
             "signature_key": signature_key,
             "signature_name": signature_name,
             "signature_secret": signature_secret,
         }
 
     @builtins.property
@@ -7895,28 +8777,34 @@
 ):
     '''A ROS resource type:  ``ALIYUN::ApiGateway::StageConfig``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "StageConfigProps",
+        props: typing.Union["StageConfigProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::ApiGateway::StageConfig``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(StageConfig.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-apigateway.StageConfigProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -7935,14 +8823,19 @@
     ) -> None:
         '''Properties for defining a ``ALIYUN::ApiGateway::StageConfig``.
 
         :param group_id: Property groupId: The id of the Group.
         :param stage_name: Property stageName: The name of the Stage.
         :param variables: Property variables: Variables in the stage, key-value pairs.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(StageConfigProps.__init__)
+            check_type(argname="argument group_id", value=group_id, expected_type=type_hints["group_id"])
+            check_type(argname="argument stage_name", value=stage_name, expected_type=type_hints["stage_name"])
+            check_type(argname="argument variables", value=variables, expected_type=type_hints["variables"])
         self._values: typing.Dict[str, typing.Any] = {
             "group_id": group_id,
             "stage_name": stage_name,
             "variables": variables,
         }
 
     @builtins.property
@@ -7987,31 +8880,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::ApiGateway::TrafficControl``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "TrafficControlProps",
+        props: typing.Union["TrafficControlProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::ApiGateway::TrafficControl``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(TrafficControl.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTrafficControlId")
     def attr_traffic_control_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute TrafficControlId: The id of the traffic control.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTrafficControlId"))
 
 
 class TrafficControlBinding(
@@ -8021,28 +8920,34 @@
 ):
     '''A ROS resource type:  ``ALIYUN::ApiGateway::TrafficControlBinding``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "TrafficControlBindingProps",
+        props: typing.Union["TrafficControlBindingProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::ApiGateway::TrafficControlBinding``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(TrafficControlBinding.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-apigateway.TrafficControlBindingProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -8064,14 +8969,20 @@
         '''Properties for defining a ``ALIYUN::ApiGateway::TrafficControlBinding``.
 
         :param api_ids: Property apiIds: APIs to bind with the traffic control.
         :param group_id: Property groupId: The id of group.
         :param stage_name: Property stageName: Bind traffic in this stage.
         :param traffic_control_id: Property trafficControlId: The id of traffic control.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(TrafficControlBindingProps.__init__)
+            check_type(argname="argument api_ids", value=api_ids, expected_type=type_hints["api_ids"])
+            check_type(argname="argument group_id", value=group_id, expected_type=type_hints["group_id"])
+            check_type(argname="argument stage_name", value=stage_name, expected_type=type_hints["stage_name"])
+            check_type(argname="argument traffic_control_id", value=traffic_control_id, expected_type=type_hints["traffic_control_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "api_ids": api_ids,
             "group_id": group_id,
             "stage_name": stage_name,
             "traffic_control_id": traffic_control_id,
         }
 
@@ -8137,27 +9048,36 @@
         self,
         *,
         api_default: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
         traffic_control_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         traffic_control_unit: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         app_default: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        special: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosTrafficControl.SpecialProperty]]]] = None,
+        special: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosTrafficControl.SpecialProperty, typing.Dict[str, typing.Any]]]]]] = None,
         user_default: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::ApiGateway::TrafficControl``.
 
         :param api_default: Property apiDefault: Default API traffic value.
         :param traffic_control_name: Property trafficControlName: The name of the traffic control.Need [4, 50] Chinese\\English\\Number characters or "_",and should start with Chinese/English character.
         :param traffic_control_unit: Property trafficControlUnit: Traffic control unit, DAY/HOUR/MINUTE.
         :param app_default: Property appDefault: Default APP traffic value.
         :param description: Property description: Description of the traffic control, less than 180 characters.
         :param special: Property special: Special traffic controls.
         :param user_default: Property userDefault: Default user traffic value.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(TrafficControlProps.__init__)
+            check_type(argname="argument api_default", value=api_default, expected_type=type_hints["api_default"])
+            check_type(argname="argument traffic_control_name", value=traffic_control_name, expected_type=type_hints["traffic_control_name"])
+            check_type(argname="argument traffic_control_unit", value=traffic_control_unit, expected_type=type_hints["traffic_control_unit"])
+            check_type(argname="argument app_default", value=app_default, expected_type=type_hints["app_default"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument special", value=special, expected_type=type_hints["special"])
+            check_type(argname="argument user_default", value=user_default, expected_type=type_hints["user_default"])
         self._values: typing.Dict[str, typing.Any] = {
             "api_default": api_default,
             "traffic_control_name": traffic_control_name,
             "traffic_control_unit": traffic_control_unit,
         }
         if app_default is not None:
             self._values["app_default"] = app_default
@@ -8244,28 +9164,34 @@
 ):
     '''A ROS resource type:  ``ALIYUN::ApiGateway::VpcAccessConfig``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "VpcAccessConfigProps",
+        props: typing.Union["VpcAccessConfigProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::ApiGateway::VpcAccessConfig``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(VpcAccessConfig.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-apigateway.VpcAccessConfigProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -8287,14 +9213,20 @@
         '''Properties for defining a ``ALIYUN::ApiGateway::VpcAccessConfig``.
 
         :param instance_id: Property instanceId: The id of the instance (ECS/SLB).
         :param name: Property name: The name of one VPC access configuration.
         :param port: Property port: The port of the VPC.
         :param vpc_id: Property vpcId: The id of the VPC.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(VpcAccessConfigProps.__init__)
+            check_type(argname="argument instance_id", value=instance_id, expected_type=type_hints["instance_id"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument port", value=port, expected_type=type_hints["port"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "instance_id": instance_id,
             "name": name,
             "port": port,
             "vpc_id": vpc_id,
         }
```

### Comparing `ros-cdk-apigateway-1.0.8/src/ros_cdk_apigateway.egg-info/PKG-INFO` & `ros-cdk-apigateway-1.0.9/src/ros_cdk_apigateway.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-apigateway
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS APIGATEWAY Construct Library
```

