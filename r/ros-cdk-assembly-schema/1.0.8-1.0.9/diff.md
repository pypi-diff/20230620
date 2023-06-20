# Comparing `tmp/ros-cdk-assembly-schema-1.0.8.tar.gz` & `tmp/ros-cdk-assembly-schema-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-assembly-schema-1.0.8.tar", last modified: Fri May 20 03:30:37 2022, max compression
+gzip compressed data, was "dist/ros-cdk-assembly-schema-1.0.9.tar", last modified: Thu Jun  9 01:37:33 2022, max compression
```

## Comparing `ros-cdk-assembly-schema-1.0.8.tar` & `ros-cdk-assembly-schema-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 03:30:37.000000 ros-cdk-assembly-schema-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-05-20 03:30:37.000000 ros-cdk-assembly-schema-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-05-20 03:30:37.000000 ros-cdk-assembly-schema-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-05-20 03:30:37.000000 ros-cdk-assembly-schema-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1281 2022-05-20 03:30:37.000000 ros-cdk-assembly-schema-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      176 2022-05-20 03:30:37.000000 ros-cdk-assembly-schema-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-05-20 03:30:37.000000 ros-cdk-assembly-schema-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-05-20 03:30:37.000000 ros-cdk-assembly-schema-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1790 2022-05-20 03:30:37.000000 ros-cdk-assembly-schema-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 03:30:37.000000 ros-cdk-assembly-schema-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 03:30:37.000000 ros-cdk-assembly-schema-1.0.8/src/ros_cdk_assembly_schema/
--rw-r--r--   0 root         (0) root         (0)    40850 2022-05-20 03:30:37.000000 ros-cdk-assembly-schema-1.0.8/src/ros_cdk_assembly_schema/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 03:30:37.000000 ros-cdk-assembly-schema-1.0.8/src/ros_cdk_assembly_schema/_jsii/
--rw-r--r--   0 root         (0) root         (0)      356 2022-05-20 03:30:37.000000 ros-cdk-assembly-schema-1.0.8/src/ros_cdk_assembly_schema/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    96247 2022-05-20 03:30:37.000000 ros-cdk-assembly-schema-1.0.8/src/ros_cdk_assembly_schema/_jsii/ros-cdk-assembly-schema@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-20 03:30:37.000000 ros-cdk-assembly-schema-1.0.8/src/ros_cdk_assembly_schema/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 03:30:37.000000 ros-cdk-assembly-schema-1.0.8/src/ros_cdk_assembly_schema.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1281 2022-05-20 03:30:37.000000 ros-cdk-assembly-schema-1.0.8/src/ros_cdk_assembly_schema.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      520 2022-05-20 03:30:37.000000 ros-cdk-assembly-schema-1.0.8/src/ros_cdk_assembly_schema.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-20 03:30:37.000000 ros-cdk-assembly-schema-1.0.8/src/ros_cdk_assembly_schema.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2022-05-20 03:30:37.000000 ros-cdk-assembly-schema-1.0.8/src/ros_cdk_assembly_schema.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2022-05-20 03:30:37.000000 ros-cdk-assembly-schema-1.0.8/src/ros_cdk_assembly_schema.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-09 01:37:33.000000 ros-cdk-assembly-schema-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-06-09 01:37:33.000000 ros-cdk-assembly-schema-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-06-09 01:37:33.000000 ros-cdk-assembly-schema-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-06-09 01:37:33.000000 ros-cdk-assembly-schema-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1281 2022-06-09 01:37:33.000000 ros-cdk-assembly-schema-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      176 2022-06-09 01:37:33.000000 ros-cdk-assembly-schema-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      106 2022-06-09 01:37:33.000000 ros-cdk-assembly-schema-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-06-09 01:37:33.000000 ros-cdk-assembly-schema-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1790 2022-06-09 01:37:33.000000 ros-cdk-assembly-schema-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-09 01:37:33.000000 ros-cdk-assembly-schema-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-09 01:37:33.000000 ros-cdk-assembly-schema-1.0.9/src/ros_cdk_assembly_schema/
+-rw-r--r--   0 root         (0) root         (0)    40850 2022-06-09 01:37:33.000000 ros-cdk-assembly-schema-1.0.9/src/ros_cdk_assembly_schema/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-09 01:37:33.000000 ros-cdk-assembly-schema-1.0.9/src/ros_cdk_assembly_schema/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      356 2022-06-09 01:37:33.000000 ros-cdk-assembly-schema-1.0.9/src/ros_cdk_assembly_schema/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    96241 2022-06-09 01:37:33.000000 ros-cdk-assembly-schema-1.0.9/src/ros_cdk_assembly_schema/_jsii/ros-cdk-assembly-schema@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-06-09 01:37:33.000000 ros-cdk-assembly-schema-1.0.9/src/ros_cdk_assembly_schema/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-09 01:37:33.000000 ros-cdk-assembly-schema-1.0.9/src/ros_cdk_assembly_schema.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1281 2022-06-09 01:37:33.000000 ros-cdk-assembly-schema-1.0.9/src/ros_cdk_assembly_schema.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      520 2022-06-09 01:37:33.000000 ros-cdk-assembly-schema-1.0.9/src/ros_cdk_assembly_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-06-09 01:37:33.000000 ros-cdk-assembly-schema-1.0.9/src/ros_cdk_assembly_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2022-06-09 01:37:33.000000 ros-cdk-assembly-schema-1.0.9/src/ros_cdk_assembly_schema.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2022-06-09 01:37:33.000000 ros-cdk-assembly-schema-1.0.9/src/ros_cdk_assembly_schema.egg-info/top_level.txt
```

### Comparing `ros-cdk-assembly-schema-1.0.8/LICENSE` & `ros-cdk-assembly-schema-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-assembly-schema-1.0.8/PKG-INFO` & `ros-cdk-assembly-schema-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-assembly-schema
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: # `@alicloud/ros-cdk-assembly-schema`
```

### Comparing `ros-cdk-assembly-schema-1.0.8/setup.py` & `ros-cdk-assembly-schema-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-assembly-schema",
-    "version": "1.0.8",
+    "version": "1.0.9",
     "description": "Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com",
     "license": "Apache-2.0",
     "url": "https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git",
     "long_description_content_type": "text/markdown",
     "author": "ROS Development Team",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "ros_cdk_assembly_schema",
         "ros_cdk_assembly_schema._jsii"
     ],
     "package_data": {
         "ros_cdk_assembly_schema._jsii": [
-            "ros-cdk-assembly-schema@1.0.8.jsii.tgz"
+            "ros-cdk-assembly-schema@1.0.9.jsii.tgz"
         ],
         "ros_cdk_assembly_schema": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `ros-cdk-assembly-schema-1.0.8/src/ros_cdk_assembly_schema/__init__.py` & `ros-cdk-assembly-schema-1.0.9/src/ros_cdk_assembly_schema/__init__.py`

 * *Files identical despite different names*

### Comparing `ros-cdk-assembly-schema-1.0.8/src/ros_cdk_assembly_schema.egg-info/PKG-INFO` & `ros-cdk-assembly-schema-1.0.9/src/ros_cdk_assembly_schema.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-assembly-schema
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: # `@alicloud/ros-cdk-assembly-schema`
```

### Comparing `ros-cdk-assembly-schema-1.0.8/src/ros_cdk_assembly_schema.egg-info/SOURCES.txt` & `ros-cdk-assembly-schema-1.0.9/src/ros_cdk_assembly_schema.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 src/ros_cdk_assembly_schema/py.typed
 src/ros_cdk_assembly_schema.egg-info/PKG-INFO
 src/ros_cdk_assembly_schema.egg-info/SOURCES.txt
 src/ros_cdk_assembly_schema.egg-info/dependency_links.txt
 src/ros_cdk_assembly_schema.egg-info/requires.txt
 src/ros_cdk_assembly_schema.egg-info/top_level.txt
 src/ros_cdk_assembly_schema/_jsii/__init__.py
-src/ros_cdk_assembly_schema/_jsii/ros-cdk-assembly-schema@1.0.8.jsii.tgz
+src/ros_cdk_assembly_schema/_jsii/ros-cdk-assembly-schema@1.0.9.jsii.tgz
```

