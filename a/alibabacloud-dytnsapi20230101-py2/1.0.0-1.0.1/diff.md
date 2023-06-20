# Comparing `tmp/alibabacloud_dytnsapi20230101_py2-1.0.0.tar.gz` & `tmp/alibabacloud_dytnsapi20230101_py2-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dytnsapi20230101_py2-1.0.0.tar", last modified: Fri Jun 16 08:54:58 2023, max compression
+gzip compressed data, was "dist/alibabacloud_dytnsapi20230101_py2-1.0.1.tar", last modified: Tue Jun 20 03:23:42 2023, max compression
```

## Comparing `alibabacloud_dytnsapi20230101_py2-1.0.0.tar` & `alibabacloud_dytnsapi20230101_py2-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 08:54:58.000000 alibabacloud_dytnsapi20230101_py2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      588 2023-06-16 08:54:58.000000 alibabacloud_dytnsapi20230101_py2-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-06-16 08:54:58.000000 alibabacloud_dytnsapi20230101_py2-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2502 2023-06-16 08:54:58.000000 alibabacloud_dytnsapi20230101_py2-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1048 2023-06-16 08:54:58.000000 alibabacloud_dytnsapi20230101_py2-1.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1131 2023-06-16 08:54:58.000000 alibabacloud_dytnsapi20230101_py2-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 08:54:58.000000 alibabacloud_dytnsapi20230101_py2-1.0.0/alibabacloud_dytnsapi20230101/
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-16 08:54:58.000000 alibabacloud_dytnsapi20230101_py2-1.0.0/alibabacloud_dytnsapi20230101/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1125 2023-06-16 08:54:58.000000 alibabacloud_dytnsapi20230101_py2-1.0.0/alibabacloud_dytnsapi20230101/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 08:54:58.000000 alibabacloud_dytnsapi20230101_py2-1.0.0/alibabacloud_dytnsapi20230101_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2502 2023-06-16 08:54:58.000000 alibabacloud_dytnsapi20230101_py2-1.0.0/alibabacloud_dytnsapi20230101_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      427 2023-06-16 08:54:58.000000 alibabacloud_dytnsapi20230101_py2-1.0.0/alibabacloud_dytnsapi20230101_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 08:54:58.000000 alibabacloud_dytnsapi20230101_py2-1.0.0/alibabacloud_dytnsapi20230101_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      128 2023-06-16 08:54:58.000000 alibabacloud_dytnsapi20230101_py2-1.0.0/alibabacloud_dytnsapi20230101_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-06-16 08:54:58.000000 alibabacloud_dytnsapi20230101_py2-1.0.0/alibabacloud_dytnsapi20230101_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-16 08:54:58.000000 alibabacloud_dytnsapi20230101_py2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2876 2023-06-16 08:54:58.000000 alibabacloud_dytnsapi20230101_py2-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 03:23:42.000000 alibabacloud_dytnsapi20230101_py2-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)       76 2023-06-20 03:23:41.000000 alibabacloud_dytnsapi20230101_py2-1.0.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-06-20 03:23:41.000000 alibabacloud_dytnsapi20230101_py2-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-06-20 03:23:41.000000 alibabacloud_dytnsapi20230101_py2-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2502 2023-06-20 03:23:42.000000 alibabacloud_dytnsapi20230101_py2-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1048 2023-06-20 03:23:41.000000 alibabacloud_dytnsapi20230101_py2-1.0.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-06-20 03:23:41.000000 alibabacloud_dytnsapi20230101_py2-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 03:23:42.000000 alibabacloud_dytnsapi20230101_py2-1.0.1/alibabacloud_dytnsapi20230101/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-20 03:23:41.000000 alibabacloud_dytnsapi20230101_py2-1.0.1/alibabacloud_dytnsapi20230101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5187 2023-06-20 03:23:41.000000 alibabacloud_dytnsapi20230101_py2-1.0.1/alibabacloud_dytnsapi20230101/client.py
+-rw-r--r--   0 root         (0) root         (0)    12752 2023-06-20 03:23:41.000000 alibabacloud_dytnsapi20230101_py2-1.0.1/alibabacloud_dytnsapi20230101/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 03:23:42.000000 alibabacloud_dytnsapi20230101_py2-1.0.1/alibabacloud_dytnsapi20230101_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2502 2023-06-20 03:23:42.000000 alibabacloud_dytnsapi20230101_py2-1.0.1/alibabacloud_dytnsapi20230101_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      480 2023-06-20 03:23:42.000000 alibabacloud_dytnsapi20230101_py2-1.0.1/alibabacloud_dytnsapi20230101_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 03:23:42.000000 alibabacloud_dytnsapi20230101_py2-1.0.1/alibabacloud_dytnsapi20230101_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-06-20 03:23:42.000000 alibabacloud_dytnsapi20230101_py2-1.0.1/alibabacloud_dytnsapi20230101_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-20 03:23:42.000000 alibabacloud_dytnsapi20230101_py2-1.0.1/alibabacloud_dytnsapi20230101_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-20 03:23:42.000000 alibabacloud_dytnsapi20230101_py2-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2928 2023-06-20 03:23:41.000000 alibabacloud_dytnsapi20230101_py2-1.0.1/setup.py
```

### Comparing `alibabacloud_dytnsapi20230101_py2-1.0.0/LICENSE` & `alibabacloud_dytnsapi20230101_py2-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dytnsapi20230101_py2-1.0.0/PKG-INFO` & `alibabacloud_dytnsapi20230101_py2-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dytnsapi20230101_py2
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud Dytnsapi (20230101) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dytnsapi20230101_py2-1.0.0/README-CN.md` & `alibabacloud_dytnsapi20230101_py2-1.0.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dytnsapi20230101_py2-1.0.0/README.md` & `alibabacloud_dytnsapi20230101_py2-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dytnsapi20230101_py2-1.0.0/alibabacloud_dytnsapi20230101_py2.egg-info/PKG-INFO` & `alibabacloud_dytnsapi20230101_py2-1.0.1/alibabacloud_dytnsapi20230101_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dytnsapi20230101-py2
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud Dytnsapi (20230101) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dytnsapi20230101_py2-1.0.0/setup.py` & `alibabacloud_dytnsapi20230101_py2-1.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,29 +21,30 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dytnsapi20230101_py2.
 
-Created on 16/06/2023
+Created on 20/06/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dytnsapi20230101"
 NAME = "alibabacloud_dytnsapi20230101_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dytnsapi (20230101) SDK Library for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python2-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "alibabacloud_tea_util_py2>=0.0.7, <1.0.0",
     "alibabacloud_tea_openapi_py2>=0.1.6, <1.0.0",
+    "alibabacloud_openapi_util_py2>=0.1.1, <1.0.0",
     "alibabacloud_endpoint_util_py2>=0.0.2, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 
 if os.path.exists('./README.md'):
     if sys.version_info.major == 2:
```

