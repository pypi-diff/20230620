# Comparing `tmp/ros-cdk-core-1.0.8.tar.gz` & `tmp/ros-cdk-core-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-core-1.0.8.tar", last modified: Fri May 20 03:32:09 2022, max compression
+gzip compressed data, was "dist/ros-cdk-core-1.0.9.tar", last modified: Thu Jun  9 01:38:47 2022, max compression
```

## Comparing `ros-cdk-core-1.0.8.tar` & `ros-cdk-core-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 03:32:09.000000 ros-cdk-core-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-05-20 03:32:09.000000 ros-cdk-core-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-05-20 03:32:09.000000 ros-cdk-core-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-05-20 03:32:09.000000 ros-cdk-core-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1235 2022-05-20 03:32:09.000000 ros-cdk-core-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      141 2022-05-20 03:32:09.000000 ros-cdk-core-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-05-20 03:32:09.000000 ros-cdk-core-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-05-20 03:32:09.000000 ros-cdk-core-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1851 2022-05-20 03:32:09.000000 ros-cdk-core-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 03:32:09.000000 ros-cdk-core-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 03:32:09.000000 ros-cdk-core-1.0.8/src/ros_cdk_core/
--rw-r--r--   0 root         (0) root         (0)   234846 2022-05-20 03:32:09.000000 ros-cdk-core-1.0.8/src/ros_cdk_core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 03:32:09.000000 ros-cdk-core-1.0.8/src/ros_cdk_core/_jsii/
--rw-r--r--   0 root         (0) root         (0)      410 2022-05-20 03:32:09.000000 ros-cdk-core-1.0.8/src/ros_cdk_core/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)   374394 2022-05-20 03:32:09.000000 ros-cdk-core-1.0.8/src/ros_cdk_core/_jsii/ros-cdk-core@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-20 03:32:09.000000 ros-cdk-core-1.0.8/src/ros_cdk_core/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 03:32:09.000000 ros-cdk-core-1.0.8/src/ros_cdk_core.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1235 2022-05-20 03:32:09.000000 ros-cdk-core-1.0.8/src/ros_cdk_core.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      410 2022-05-20 03:32:09.000000 ros-cdk-core-1.0.8/src/ros_cdk_core.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-20 03:32:09.000000 ros-cdk-core-1.0.8/src/ros_cdk_core.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      130 2022-05-20 03:32:09.000000 ros-cdk-core-1.0.8/src/ros_cdk_core.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2022-05-20 03:32:09.000000 ros-cdk-core-1.0.8/src/ros_cdk_core.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-09 01:38:47.000000 ros-cdk-core-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-06-09 01:38:47.000000 ros-cdk-core-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-06-09 01:38:47.000000 ros-cdk-core-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-06-09 01:38:47.000000 ros-cdk-core-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1235 2022-06-09 01:38:47.000000 ros-cdk-core-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      141 2022-06-09 01:38:47.000000 ros-cdk-core-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      106 2022-06-09 01:38:47.000000 ros-cdk-core-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-06-09 01:38:47.000000 ros-cdk-core-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1851 2022-06-09 01:38:47.000000 ros-cdk-core-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-09 01:38:47.000000 ros-cdk-core-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-09 01:38:47.000000 ros-cdk-core-1.0.9/src/ros_cdk_core/
+-rw-r--r--   0 root         (0) root         (0)   234846 2022-06-09 01:38:47.000000 ros-cdk-core-1.0.9/src/ros_cdk_core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-09 01:38:47.000000 ros-cdk-core-1.0.9/src/ros_cdk_core/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      410 2022-06-09 01:38:47.000000 ros-cdk-core-1.0.9/src/ros_cdk_core/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   374393 2022-06-09 01:38:47.000000 ros-cdk-core-1.0.9/src/ros_cdk_core/_jsii/ros-cdk-core@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-06-09 01:38:47.000000 ros-cdk-core-1.0.9/src/ros_cdk_core/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-09 01:38:47.000000 ros-cdk-core-1.0.9/src/ros_cdk_core.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1235 2022-06-09 01:38:47.000000 ros-cdk-core-1.0.9/src/ros_cdk_core.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      410 2022-06-09 01:38:47.000000 ros-cdk-core-1.0.9/src/ros_cdk_core.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-06-09 01:38:47.000000 ros-cdk-core-1.0.9/src/ros_cdk_core.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      130 2022-06-09 01:38:47.000000 ros-cdk-core-1.0.9/src/ros_cdk_core.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2022-06-09 01:38:47.000000 ros-cdk-core-1.0.9/src/ros_cdk_core.egg-info/top_level.txt
```

### Comparing `ros-cdk-core-1.0.8/LICENSE` & `ros-cdk-core-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-core-1.0.8/PKG-INFO` & `ros-cdk-core-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-core
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: # `@alicloud/ros-cdk-core`
```

### Comparing `ros-cdk-core-1.0.8/setup.py` & `ros-cdk-core-1.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-core",
-    "version": "1.0.8",
+    "version": "1.0.9",
     "description": "Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com",
     "license": "Apache-2.0",
     "url": "https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git",
     "long_description_content_type": "text/markdown",
     "author": "ROS Development Team",
     "bdist_wheel": {
         "universal": true
@@ -22,27 +22,27 @@
     },
     "packages": [
         "ros_cdk_core",
         "ros_cdk_core._jsii"
     ],
     "package_data": {
         "ros_cdk_core._jsii": [
-            "ros-cdk-core@1.0.8.jsii.tgz"
+            "ros-cdk-core@1.0.9.jsii.tgz"
         ],
         "ros_cdk_core": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "constructs>=3.0.4, <4.0.0",
         "jsii>=1.59.0, <2.0.0",
         "publication>=0.0.3",
-        "ros-cdk-assembly-schema>=1.0.8, <2.0.0",
-        "ros-cdk-cxapi>=1.0.8, <2.0.0"
+        "ros-cdk-assembly-schema>=1.0.9, <2.0.0",
+        "ros-cdk-cxapi>=1.0.9, <2.0.0"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
```

### Comparing `ros-cdk-core-1.0.8/src/ros_cdk_core/__init__.py` & `ros-cdk-core-1.0.9/src/ros_cdk_core/__init__.py`

 * *Files identical despite different names*

### Comparing `ros-cdk-core-1.0.8/src/ros_cdk_core.egg-info/PKG-INFO` & `ros-cdk-core-1.0.9/src/ros_cdk_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-core
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: # `@alicloud/ros-cdk-core`
```

