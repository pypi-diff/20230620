# Comparing `tmp/alibabacloud_green20220302-1.0.5.tar.gz` & `tmp/alibabacloud_green20220302-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_green20220302-1.0.5.tar", last modified: Wed May 17 06:05:39 2023, max compression
+gzip compressed data, was "dist/alibabacloud_green20220302-1.0.6.tar", last modified: Tue Jun 20 06:11:40 2023, max compression
```

## Comparing `alibabacloud_green20220302-1.0.5.tar` & `alibabacloud_green20220302-1.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:05:39.000000 alibabacloud_green20220302-1.0.5/
--rw-r--r--   0 root         (0) root         (0)      207 2023-05-17 06:05:38.000000 alibabacloud_green20220302-1.0.5/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-05-17 06:05:38.000000 alibabacloud_green20220302-1.0.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-17 06:05:38.000000 alibabacloud_green20220302-1.0.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2340 2023-05-17 06:05:39.000000 alibabacloud_green20220302-1.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1028 2023-05-17 06:05:38.000000 alibabacloud_green20220302-1.0.5/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1113 2023-05-17 06:05:38.000000 alibabacloud_green20220302-1.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:05:39.000000 alibabacloud_green20220302-1.0.5/alibabacloud_green20220302/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-17 06:05:38.000000 alibabacloud_green20220302-1.0.5/alibabacloud_green20220302/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19695 2023-05-17 06:05:38.000000 alibabacloud_green20220302-1.0.5/alibabacloud_green20220302/client.py
--rw-r--r--   0 root         (0) root         (0)    35554 2023-05-17 06:05:38.000000 alibabacloud_green20220302-1.0.5/alibabacloud_green20220302/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:05:39.000000 alibabacloud_green20220302-1.0.5/alibabacloud_green20220302.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2340 2023-05-17 06:05:38.000000 alibabacloud_green20220302-1.0.5/alibabacloud_green20220302.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      436 2023-05-17 06:05:38.000000 alibabacloud_green20220302-1.0.5/alibabacloud_green20220302.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 06:05:38.000000 alibabacloud_green20220302-1.0.5/alibabacloud_green20220302.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-05-17 06:05:38.000000 alibabacloud_green20220302-1.0.5/alibabacloud_green20220302.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-05-17 06:05:38.000000 alibabacloud_green20220302-1.0.5/alibabacloud_green20220302.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-17 06:05:39.000000 alibabacloud_green20220302-1.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2620 2023-05-17 06:05:38.000000 alibabacloud_green20220302-1.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:11:40.000000 alibabacloud_green20220302-1.0.6/
+-rw-r--r--   0 root         (0) root         (0)      264 2023-06-20 06:11:40.000000 alibabacloud_green20220302-1.0.6/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-20 06:11:40.000000 alibabacloud_green20220302-1.0.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-20 06:11:40.000000 alibabacloud_green20220302-1.0.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2340 2023-06-20 06:11:40.000000 alibabacloud_green20220302-1.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1028 2023-06-20 06:11:40.000000 alibabacloud_green20220302-1.0.6/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1113 2023-06-20 06:11:40.000000 alibabacloud_green20220302-1.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:11:40.000000 alibabacloud_green20220302-1.0.6/alibabacloud_green20220302/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-20 06:11:40.000000 alibabacloud_green20220302-1.0.6/alibabacloud_green20220302/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19695 2023-06-20 06:11:40.000000 alibabacloud_green20220302-1.0.6/alibabacloud_green20220302/client.py
+-rw-r--r--   0 root         (0) root         (0)    35811 2023-06-20 06:11:40.000000 alibabacloud_green20220302-1.0.6/alibabacloud_green20220302/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:11:40.000000 alibabacloud_green20220302-1.0.6/alibabacloud_green20220302.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2340 2023-06-20 06:11:40.000000 alibabacloud_green20220302-1.0.6/alibabacloud_green20220302.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      436 2023-06-20 06:11:40.000000 alibabacloud_green20220302-1.0.6/alibabacloud_green20220302.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 06:11:40.000000 alibabacloud_green20220302-1.0.6/alibabacloud_green20220302.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-06-20 06:11:40.000000 alibabacloud_green20220302-1.0.6/alibabacloud_green20220302.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-06-20 06:11:40.000000 alibabacloud_green20220302-1.0.6/alibabacloud_green20220302.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-20 06:11:40.000000 alibabacloud_green20220302-1.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2620 2023-06-20 06:11:40.000000 alibabacloud_green20220302-1.0.6/setup.py
```

### Comparing `alibabacloud_green20220302-1.0.5/LICENSE` & `alibabacloud_green20220302-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_green20220302-1.0.5/PKG-INFO` & `alibabacloud_green20220302-1.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_green20220302
-Version: 1.0.5
+Version: 1.0.6
 Summary: Alibaba Cloud Green (20220302) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_green20220302-1.0.5/README-CN.md` & `alibabacloud_green20220302-1.0.6/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_green20220302-1.0.5/README.md` & `alibabacloud_green20220302-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_green20220302-1.0.5/alibabacloud_green20220302/client.py` & `alibabacloud_green20220302-1.0.6/alibabacloud_green20220302/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_green20220302-1.0.5/alibabacloud_green20220302/models.py` & `alibabacloud_green20220302-1.0.6/alibabacloud_green20220302/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,34 +107,40 @@
         return self
 
 
 class DescribeImageResultExtResponseBodyDataTextInImage(TeaModel):
     def __init__(
         self,
         ocr_datas: List[str] = None,
+        risk_words: List[str] = None,
     ):
         self.ocr_datas = ocr_datas
+        self.risk_words = risk_words
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.ocr_datas is not None:
             result['OcrDatas'] = self.ocr_datas
+        if self.risk_words is not None:
+            result['RiskWords'] = self.risk_words
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('OcrDatas') is not None:
             self.ocr_datas = m.get('OcrDatas')
+        if m.get('RiskWords') is not None:
+            self.risk_words = m.get('RiskWords')
         return self
 
 
 class DescribeImageResultExtResponseBodyData(TeaModel):
     def __init__(
         self,
         custom_image: List[DescribeImageResultExtResponseBodyDataCustomImage] = None,
```

### Comparing `alibabacloud_green20220302-1.0.5/alibabacloud_green20220302.egg-info/PKG-INFO` & `alibabacloud_green20220302-1.0.6/alibabacloud_green20220302.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-green20220302
-Version: 1.0.5
+Version: 1.0.6
 Summary: Alibaba Cloud Green (20220302) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_green20220302-1.0.5/setup.py` & `alibabacloud_green20220302-1.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_green20220302.
 
-Created on 17/05/2023
+Created on 20/06/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_green20220302"
 NAME = "alibabacloud_green20220302" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Green (20220302) SDK Library for Python"
```

