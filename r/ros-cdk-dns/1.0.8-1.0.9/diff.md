# Comparing `tmp/ros-cdk-dns-1.0.8.tar.gz` & `tmp/ros-cdk-dns-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-dns-1.0.8.tar", last modified: Thu Jul 14 02:40:49 2022, max compression
+gzip compressed data, was "dist/ros-cdk-dns-1.0.9.tar", last modified: Fri Sep 23 12:14:00 2022, max compression
```

## Comparing `ros-cdk-dns-1.0.8.tar` & `ros-cdk-dns-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:40:49.000000 ros-cdk-dns-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:40:49.000000 ros-cdk-dns-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:40:49.000000 ros-cdk-dns-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:40:49.000000 ros-cdk-dns-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:40:49.000000 ros-cdk-dns-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      179 2022-07-14 02:40:49.000000 ros-cdk-dns-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:40:49.000000 ros-cdk-dns-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:40:49.000000 ros-cdk-dns-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1794 2022-07-14 02:40:49.000000 ros-cdk-dns-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:40:49.000000 ros-cdk-dns-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:40:49.000000 ros-cdk-dns-1.0.8/src/ros_cdk_dns/
--rw-r--r--   0 root         (0) root         (0)    43032 2022-07-14 02:40:49.000000 ros-cdk-dns-1.0.8/src/ros_cdk_dns/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:40:49.000000 ros-cdk-dns-1.0.8/src/ros_cdk_dns/_jsii/
--rw-r--r--   0 root         (0) root         (0)      370 2022-07-14 02:40:49.000000 ros-cdk-dns-1.0.8/src/ros_cdk_dns/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39090 2022-07-14 02:40:49.000000 ros-cdk-dns-1.0.8/src/ros_cdk_dns/_jsii/ros-cdk-dns@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:40:49.000000 ros-cdk-dns-1.0.8/src/ros_cdk_dns/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:40:49.000000 ros-cdk-dns-1.0.8/src/ros_cdk_dns.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:40:49.000000 ros-cdk-dns-1.0.8/src/ros_cdk_dns.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      400 2022-07-14 02:40:49.000000 ros-cdk-dns-1.0.8/src/ros_cdk_dns.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:40:49.000000 ros-cdk-dns-1.0.8/src/ros_cdk_dns.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:40:49.000000 ros-cdk-dns-1.0.8/src/ros_cdk_dns.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-07-14 02:40:49.000000 ros-cdk-dns-1.0.8/src/ros_cdk_dns.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:14:00.000000 ros-cdk-dns-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 12:14:00.000000 ros-cdk-dns-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 12:14:00.000000 ros-cdk-dns-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 12:14:00.000000 ros-cdk-dns-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 12:14:00.000000 ros-cdk-dns-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      179 2022-09-23 12:14:00.000000 ros-cdk-dns-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 12:14:00.000000 ros-cdk-dns-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 12:14:00.000000 ros-cdk-dns-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1823 2022-09-23 12:14:00.000000 ros-cdk-dns-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:14:00.000000 ros-cdk-dns-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:14:00.000000 ros-cdk-dns-1.0.9/src/ros_cdk_dns/
+-rw-r--r--   0 root         (0) root         (0)    53149 2022-09-23 12:14:00.000000 ros-cdk-dns-1.0.9/src/ros_cdk_dns/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:14:00.000000 ros-cdk-dns-1.0.9/src/ros_cdk_dns/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      404 2022-09-23 12:14:00.000000 ros-cdk-dns-1.0.9/src/ros_cdk_dns/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39155 2022-09-23 12:14:00.000000 ros-cdk-dns-1.0.9/src/ros_cdk_dns/_jsii/ros-cdk-dns@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 12:14:00.000000 ros-cdk-dns-1.0.9/src/ros_cdk_dns/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:14:00.000000 ros-cdk-dns-1.0.9/src/ros_cdk_dns.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 12:14:00.000000 ros-cdk-dns-1.0.9/src/ros_cdk_dns.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      400 2022-09-23 12:14:00.000000 ros-cdk-dns-1.0.9/src/ros_cdk_dns.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 12:14:00.000000 ros-cdk-dns-1.0.9/src/ros_cdk_dns.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 12:14:00.000000 ros-cdk-dns-1.0.9/src/ros_cdk_dns.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-09-23 12:14:00.000000 ros-cdk-dns-1.0.9/src/ros_cdk_dns.egg-info/top_level.txt
```

### Comparing `ros-cdk-dns-1.0.8/LICENSE` & `ros-cdk-dns-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-dns-1.0.8/PKG-INFO` & `ros-cdk-dns-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-dns
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS DNS Construct Library
```

### Comparing `ros-cdk-dns-1.0.8/setup.py` & `ros-cdk-dns-1.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-dns",
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
         "ros_cdk_dns",
         "ros_cdk_dns._jsii"
     ],
     "package_data": {
         "ros_cdk_dns._jsii": [
-            "ros-cdk-dns@1.0.8.jsii.tgz"
+            "ros-cdk-dns@1.0.9.jsii.tgz"
         ],
         "ros_cdk_dns": [
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

### Comparing `ros-cdk-dns-1.0.8/src/ros_cdk_dns.egg-info/PKG-INFO` & `ros-cdk-dns-1.0.9/src/ros_cdk_dns.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-dns
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS DNS Construct Library
```

