# Comparing `tmp/ros-cdk-bastionhost-1.0.13.tar.gz` & `tmp/ros-cdk-bastionhost-1.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-bastionhost-1.0.13.tar", last modified: Wed Apr 26 07:23:46 2023, max compression
+gzip compressed data, was "dist/ros-cdk-bastionhost-1.0.14.tar", last modified: Tue Jun 20 02:08:07 2023, max compression
```

## Comparing `ros-cdk-bastionhost-1.0.13.tar` & `ros-cdk-bastionhost-1.0.14.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:23:46.000000 ros-cdk-bastionhost-1.0.13/
--rw-r--r--   0 root         (0) root         (0)    10279 2023-04-26 07:23:46.000000 ros-cdk-bastionhost-1.0.13/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-04-26 07:23:46.000000 ros-cdk-bastionhost-1.0.13/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2023-04-26 07:23:46.000000 ros-cdk-bastionhost-1.0.13/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1324 2023-04-26 07:23:46.000000 ros-cdk-bastionhost-1.0.13/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      203 2023-04-26 07:23:46.000000 ros-cdk-bastionhost-1.0.13/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-04-26 07:23:46.000000 ros-cdk-bastionhost-1.0.13/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 07:23:46.000000 ros-cdk-bastionhost-1.0.13/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1923 2023-04-26 07:23:46.000000 ros-cdk-bastionhost-1.0.13/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:23:46.000000 ros-cdk-bastionhost-1.0.13/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:23:46.000000 ros-cdk-bastionhost-1.0.13/src/ros_cdk_bastionhost/
--rw-r--r--   0 root         (0) root         (0)    43509 2023-04-26 07:23:46.000000 ros-cdk-bastionhost-1.0.13/src/ros_cdk_bastionhost/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:23:46.000000 ros-cdk-bastionhost-1.0.13/src/ros_cdk_bastionhost/_jsii/
--rw-r--r--   0 root         (0) root         (0)      435 2023-04-26 07:23:46.000000 ros-cdk-bastionhost-1.0.13/src/ros_cdk_bastionhost/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    34033 2023-04-26 07:23:46.000000 ros-cdk-bastionhost-1.0.13/src/ros_cdk_bastionhost/_jsii/ros-cdk-bastionhost@1.0.13.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 07:23:46.000000 ros-cdk-bastionhost-1.0.13/src/ros_cdk_bastionhost/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:23:46.000000 ros-cdk-bastionhost-1.0.13/src/ros_cdk_bastionhost.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1324 2023-04-26 07:23:46.000000 ros-cdk-bastionhost-1.0.13/src/ros_cdk_bastionhost.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      481 2023-04-26 07:23:46.000000 ros-cdk-bastionhost-1.0.13/src/ros_cdk_bastionhost.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 07:23:46.000000 ros-cdk-bastionhost-1.0.13/src/ros_cdk_bastionhost.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      109 2023-04-26 07:23:46.000000 ros-cdk-bastionhost-1.0.13/src/ros_cdk_bastionhost.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-04-26 07:23:46.000000 ros-cdk-bastionhost-1.0.13/src/ros_cdk_bastionhost.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:08:07.000000 ros-cdk-bastionhost-1.0.14/
+-rw-r--r--   0 root         (0) root         (0)    10279 2023-06-20 02:08:07.000000 ros-cdk-bastionhost-1.0.14/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2023-06-20 02:08:07.000000 ros-cdk-bastionhost-1.0.14/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2023-06-20 02:08:07.000000 ros-cdk-bastionhost-1.0.14/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1324 2023-06-20 02:08:07.000000 ros-cdk-bastionhost-1.0.14/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      203 2023-06-20 02:08:07.000000 ros-cdk-bastionhost-1.0.14/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2023-06-20 02:08:07.000000 ros-cdk-bastionhost-1.0.14/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-20 02:08:07.000000 ros-cdk-bastionhost-1.0.14/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1923 2023-06-20 02:08:07.000000 ros-cdk-bastionhost-1.0.14/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:08:07.000000 ros-cdk-bastionhost-1.0.14/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:08:07.000000 ros-cdk-bastionhost-1.0.14/src/ros_cdk_bastionhost/
+-rw-r--r--   0 root         (0) root         (0)    43509 2023-06-20 02:08:07.000000 ros-cdk-bastionhost-1.0.14/src/ros_cdk_bastionhost/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:08:07.000000 ros-cdk-bastionhost-1.0.14/src/ros_cdk_bastionhost/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      435 2023-06-20 02:08:07.000000 ros-cdk-bastionhost-1.0.14/src/ros_cdk_bastionhost/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    34035 2023-06-20 02:08:07.000000 ros-cdk-bastionhost-1.0.14/src/ros_cdk_bastionhost/_jsii/ros-cdk-bastionhost@1.0.14.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 02:08:07.000000 ros-cdk-bastionhost-1.0.14/src/ros_cdk_bastionhost/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:08:07.000000 ros-cdk-bastionhost-1.0.14/src/ros_cdk_bastionhost.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1324 2023-06-20 02:08:07.000000 ros-cdk-bastionhost-1.0.14/src/ros_cdk_bastionhost.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      481 2023-06-20 02:08:07.000000 ros-cdk-bastionhost-1.0.14/src/ros_cdk_bastionhost.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 02:08:07.000000 ros-cdk-bastionhost-1.0.14/src/ros_cdk_bastionhost.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2023-06-20 02:08:07.000000 ros-cdk-bastionhost-1.0.14/src/ros_cdk_bastionhost.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-20 02:08:07.000000 ros-cdk-bastionhost-1.0.14/src/ros_cdk_bastionhost.egg-info/top_level.txt
```

### Comparing `ros-cdk-bastionhost-1.0.13/LICENSE` & `ros-cdk-bastionhost-1.0.14/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-bastionhost-1.0.13/PKG-INFO` & `ros-cdk-bastionhost-1.0.14/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-bastionhost
-Version: 1.0.13
+Version: 1.0.14
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS BASTIONHOST Construct Library
```

### Comparing `ros-cdk-bastionhost-1.0.13/setup.py` & `ros-cdk-bastionhost-1.0.14/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-bastionhost",
-    "version": "1.0.13",
+    "version": "1.0.14",
     "description": "Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com",
     "license": "Apache-2.0",
     "url": "https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git",
     "long_description_content_type": "text/markdown",
     "author": "ROS Development Team",
     "bdist_wheel": {
         "universal": true
@@ -22,24 +22,24 @@
     },
     "packages": [
         "ros_cdk_bastionhost",
         "ros_cdk_bastionhost._jsii"
     ],
     "package_data": {
         "ros_cdk_bastionhost._jsii": [
-            "ros-cdk-bastionhost@1.0.13.jsii.tgz"
+            "ros-cdk-bastionhost@1.0.14.jsii.tgz"
         ],
         "ros_cdk_bastionhost": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "constructs>=3.0.4, <4.0.0",
-        "jsii>=1.80.0, <2.0.0",
+        "jsii>=1.84.0, <2.0.0",
         "publication>=0.0.3",
         "ros-cdk-core>=1.0.6, <2.0.0",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
```

### Comparing `ros-cdk-bastionhost-1.0.13/src/ros_cdk_bastionhost/__init__.py` & `ros-cdk-bastionhost-1.0.14/src/ros_cdk_bastionhost/__init__.py`

 * *Files identical despite different names*

### Comparing `ros-cdk-bastionhost-1.0.13/src/ros_cdk_bastionhost.egg-info/PKG-INFO` & `ros-cdk-bastionhost-1.0.14/src/ros_cdk_bastionhost.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-bastionhost
-Version: 1.0.13
+Version: 1.0.14
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS BASTIONHOST Construct Library
```
