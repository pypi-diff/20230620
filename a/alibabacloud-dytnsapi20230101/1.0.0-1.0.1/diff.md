# Comparing `tmp/alibabacloud_dytnsapi20230101-1.0.0.tar.gz` & `tmp/alibabacloud_dytnsapi20230101-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dytnsapi20230101-1.0.0.tar", last modified: Fri Jun 16 08:55:41 2023, max compression
+gzip compressed data, was "dist/alibabacloud_dytnsapi20230101-1.0.1.tar", last modified: Tue Jun 20 03:24:08 2023, max compression
```

## Comparing `alibabacloud_dytnsapi20230101-1.0.0.tar` & `alibabacloud_dytnsapi20230101-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 08:55:41.000000 alibabacloud_dytnsapi20230101-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      600 2023-06-16 08:55:40.000000 alibabacloud_dytnsapi20230101-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-16 08:55:40.000000 alibabacloud_dytnsapi20230101-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2358 2023-06-16 08:55:41.000000 alibabacloud_dytnsapi20230101-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1037 2023-06-16 08:55:40.000000 alibabacloud_dytnsapi20230101-1.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1122 2023-06-16 08:55:40.000000 alibabacloud_dytnsapi20230101-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 08:55:41.000000 alibabacloud_dytnsapi20230101-1.0.0/alibabacloud_dytnsapi20230101/
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-16 08:55:40.000000 alibabacloud_dytnsapi20230101-1.0.0/alibabacloud_dytnsapi20230101/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1332 2023-06-16 08:55:40.000000 alibabacloud_dytnsapi20230101-1.0.0/alibabacloud_dytnsapi20230101/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 08:55:41.000000 alibabacloud_dytnsapi20230101-1.0.0/alibabacloud_dytnsapi20230101.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2358 2023-06-16 08:55:41.000000 alibabacloud_dytnsapi20230101-1.0.0/alibabacloud_dytnsapi20230101.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      407 2023-06-16 08:55:41.000000 alibabacloud_dytnsapi20230101-1.0.0/alibabacloud_dytnsapi20230101.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 08:55:41.000000 alibabacloud_dytnsapi20230101-1.0.0/alibabacloud_dytnsapi20230101.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      116 2023-06-16 08:55:41.000000 alibabacloud_dytnsapi20230101-1.0.0/alibabacloud_dytnsapi20230101.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-06-16 08:55:41.000000 alibabacloud_dytnsapi20230101-1.0.0/alibabacloud_dytnsapi20230101.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-16 08:55:41.000000 alibabacloud_dytnsapi20230101-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2587 2023-06-16 08:55:40.000000 alibabacloud_dytnsapi20230101-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 03:24:08.000000 alibabacloud_dytnsapi20230101-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)       76 2023-06-20 03:24:07.000000 alibabacloud_dytnsapi20230101-1.0.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-20 03:24:07.000000 alibabacloud_dytnsapi20230101-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-20 03:24:07.000000 alibabacloud_dytnsapi20230101-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-06-20 03:24:08.000000 alibabacloud_dytnsapi20230101-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1037 2023-06-20 03:24:07.000000 alibabacloud_dytnsapi20230101-1.0.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1122 2023-06-20 03:24:07.000000 alibabacloud_dytnsapi20230101-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 03:24:08.000000 alibabacloud_dytnsapi20230101-1.0.1/alibabacloud_dytnsapi20230101/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-20 03:24:07.000000 alibabacloud_dytnsapi20230101-1.0.1/alibabacloud_dytnsapi20230101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10605 2023-06-20 03:24:07.000000 alibabacloud_dytnsapi20230101-1.0.1/alibabacloud_dytnsapi20230101/client.py
+-rw-r--r--   0 root         (0) root         (0)    12594 2023-06-20 03:24:07.000000 alibabacloud_dytnsapi20230101-1.0.1/alibabacloud_dytnsapi20230101/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 03:24:08.000000 alibabacloud_dytnsapi20230101-1.0.1/alibabacloud_dytnsapi20230101.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-06-20 03:24:07.000000 alibabacloud_dytnsapi20230101-1.0.1/alibabacloud_dytnsapi20230101.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2023-06-20 03:24:07.000000 alibabacloud_dytnsapi20230101-1.0.1/alibabacloud_dytnsapi20230101.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 03:24:07.000000 alibabacloud_dytnsapi20230101-1.0.1/alibabacloud_dytnsapi20230101.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-06-20 03:24:07.000000 alibabacloud_dytnsapi20230101-1.0.1/alibabacloud_dytnsapi20230101.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-20 03:24:07.000000 alibabacloud_dytnsapi20230101-1.0.1/alibabacloud_dytnsapi20230101.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-20 03:24:08.000000 alibabacloud_dytnsapi20230101-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2635 2023-06-20 03:24:07.000000 alibabacloud_dytnsapi20230101-1.0.1/setup.py
```

### Comparing `alibabacloud_dytnsapi20230101-1.0.0/LICENSE` & `alibabacloud_dytnsapi20230101-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dytnsapi20230101-1.0.0/PKG-INFO` & `alibabacloud_dytnsapi20230101-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dytnsapi20230101
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud Dytnsapi (20230101) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dytnsapi20230101-1.0.0/README-CN.md` & `alibabacloud_dytnsapi20230101-1.0.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dytnsapi20230101-1.0.0/README.md` & `alibabacloud_dytnsapi20230101-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dytnsapi20230101-1.0.0/alibabacloud_dytnsapi20230101.egg-info/PKG-INFO` & `alibabacloud_dytnsapi20230101-1.0.1/alibabacloud_dytnsapi20230101.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dytnsapi20230101
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud Dytnsapi (20230101) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dytnsapi20230101-1.0.0/setup.py` & `alibabacloud_dytnsapi20230101-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,29 +20,30 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dytnsapi20230101.
 
-Created on 16/06/2023
+Created on 20/06/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dytnsapi20230101"
 NAME = "alibabacloud_dytnsapi20230101" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dytnsapi (20230101) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "alibabacloud_tea_util>=0.3.8, <1.0.0",
     "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
+    "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

