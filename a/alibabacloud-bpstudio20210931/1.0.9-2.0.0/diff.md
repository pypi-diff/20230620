# Comparing `tmp/alibabacloud_bpstudio20210931-1.0.9.tar.gz` & `tmp/alibabacloud_bpstudio20210931-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_bpstudio20210931-1.0.9.tar", last modified: Tue Mar 14 05:24:45 2023, max compression
+gzip compressed data, was "dist/alibabacloud_bpstudio20210931-2.0.0.tar", last modified: Tue Jun 20 06:00:45 2023, max compression
```

## Comparing `alibabacloud_bpstudio20210931-1.0.9.tar` & `alibabacloud_bpstudio20210931-2.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 05:24:45.000000 alibabacloud_bpstudio20210931-1.0.9/
--rw-r--r--   0 root         (0) root         (0)      307 2023-03-14 05:24:45.000000 alibabacloud_bpstudio20210931-1.0.9/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-03-14 05:24:45.000000 alibabacloud_bpstudio20210931-1.0.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-03-14 05:24:45.000000 alibabacloud_bpstudio20210931-1.0.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2358 2023-03-14 05:24:45.000000 alibabacloud_bpstudio20210931-1.0.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1037 2023-03-14 05:24:45.000000 alibabacloud_bpstudio20210931-1.0.9/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1122 2023-03-14 05:24:45.000000 alibabacloud_bpstudio20210931-1.0.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 05:24:45.000000 alibabacloud_bpstudio20210931-1.0.9/alibabacloud_bpstudio20210931/
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-14 05:24:45.000000 alibabacloud_bpstudio20210931-1.0.9/alibabacloud_bpstudio20210931/__init__.py
--rw-r--r--   0 root         (0) root         (0)    47984 2023-03-14 05:24:45.000000 alibabacloud_bpstudio20210931-1.0.9/alibabacloud_bpstudio20210931/client.py
--rw-r--r--   0 root         (0) root         (0)    85024 2023-03-14 05:24:45.000000 alibabacloud_bpstudio20210931-1.0.9/alibabacloud_bpstudio20210931/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 05:24:45.000000 alibabacloud_bpstudio20210931-1.0.9/alibabacloud_bpstudio20210931.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2358 2023-03-14 05:24:45.000000 alibabacloud_bpstudio20210931-1.0.9/alibabacloud_bpstudio20210931.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      460 2023-03-14 05:24:45.000000 alibabacloud_bpstudio20210931-1.0.9/alibabacloud_bpstudio20210931.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-14 05:24:45.000000 alibabacloud_bpstudio20210931-1.0.9/alibabacloud_bpstudio20210931.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-03-14 05:24:45.000000 alibabacloud_bpstudio20210931-1.0.9/alibabacloud_bpstudio20210931.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-03-14 05:24:45.000000 alibabacloud_bpstudio20210931-1.0.9/alibabacloud_bpstudio20210931.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-03-14 05:24:45.000000 alibabacloud_bpstudio20210931-1.0.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2635 2023-03-14 05:24:45.000000 alibabacloud_bpstudio20210931-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:00:45.000000 alibabacloud_bpstudio20210931-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)      448 2023-06-20 06:00:44.000000 alibabacloud_bpstudio20210931-2.0.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-20 06:00:44.000000 alibabacloud_bpstudio20210931-2.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-20 06:00:44.000000 alibabacloud_bpstudio20210931-2.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-06-20 06:00:45.000000 alibabacloud_bpstudio20210931-2.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1037 2023-06-20 06:00:44.000000 alibabacloud_bpstudio20210931-2.0.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1122 2023-06-20 06:00:44.000000 alibabacloud_bpstudio20210931-2.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:00:45.000000 alibabacloud_bpstudio20210931-2.0.0/alibabacloud_bpstudio20210931/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-20 06:00:44.000000 alibabacloud_bpstudio20210931-2.0.0/alibabacloud_bpstudio20210931/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56618 2023-06-20 06:00:44.000000 alibabacloud_bpstudio20210931-2.0.0/alibabacloud_bpstudio20210931/client.py
+-rw-r--r--   0 root         (0) root         (0)   118755 2023-06-20 06:00:44.000000 alibabacloud_bpstudio20210931-2.0.0/alibabacloud_bpstudio20210931/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:00:45.000000 alibabacloud_bpstudio20210931-2.0.0/alibabacloud_bpstudio20210931.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-06-20 06:00:45.000000 alibabacloud_bpstudio20210931-2.0.0/alibabacloud_bpstudio20210931.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2023-06-20 06:00:45.000000 alibabacloud_bpstudio20210931-2.0.0/alibabacloud_bpstudio20210931.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 06:00:45.000000 alibabacloud_bpstudio20210931-2.0.0/alibabacloud_bpstudio20210931.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-06-20 06:00:45.000000 alibabacloud_bpstudio20210931-2.0.0/alibabacloud_bpstudio20210931.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-20 06:00:45.000000 alibabacloud_bpstudio20210931-2.0.0/alibabacloud_bpstudio20210931.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-20 06:00:45.000000 alibabacloud_bpstudio20210931-2.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2635 2023-06-20 06:00:44.000000 alibabacloud_bpstudio20210931-2.0.0/setup.py
```

### Comparing `alibabacloud_bpstudio20210931-1.0.9/LICENSE` & `alibabacloud_bpstudio20210931-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_bpstudio20210931-1.0.9/PKG-INFO` & `alibabacloud_bpstudio20210931-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_bpstudio20210931
-Version: 1.0.9
+Version: 2.0.0
 Summary: Alibaba Cloud BPStudio (20210931) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_bpstudio20210931-1.0.9/README-CN.md` & `alibabacloud_bpstudio20210931-2.0.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_bpstudio20210931-1.0.9/README.md` & `alibabacloud_bpstudio20210931-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_bpstudio20210931-1.0.9/alibabacloud_bpstudio20210931/client.py` & `alibabacloud_bpstudio20210931-2.0.0/alibabacloud_bpstudio20210931/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -857,14 +857,110 @@
     async def list_application_async(
         self,
         request: bpstudio_20210931_models.ListApplicationRequest,
     ) -> bpstudio_20210931_models.ListApplicationResponse:
         runtime = util_models.RuntimeOptions()
         return await self.list_application_with_options_async(request, runtime)
 
+    def list_tag_resources_with_options(
+        self,
+        request: bpstudio_20210931_models.ListTagResourcesRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> bpstudio_20210931_models.ListTagResourcesResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.client_token):
+            body['ClientToken'] = request.client_token
+        if not UtilClient.is_unset(request.next_token):
+            body['NextToken'] = request.next_token
+        if not UtilClient.is_unset(request.region_id):
+            body['RegionId'] = request.region_id
+        body_flat = {}
+        if not UtilClient.is_unset(request.resource_id):
+            body_flat['ResourceId'] = request.resource_id
+        if not UtilClient.is_unset(request.resource_type):
+            body['ResourceType'] = request.resource_type
+        if not UtilClient.is_unset(request.tag):
+            body_flat['Tag'] = request.tag
+        body = TeaCore.merge(body,
+            OpenApiUtilClient.query(body_flat))
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='ListTagResources',
+            version='2021-09-31',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            bpstudio_20210931_models.ListTagResourcesResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def list_tag_resources_with_options_async(
+        self,
+        request: bpstudio_20210931_models.ListTagResourcesRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> bpstudio_20210931_models.ListTagResourcesResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.client_token):
+            body['ClientToken'] = request.client_token
+        if not UtilClient.is_unset(request.next_token):
+            body['NextToken'] = request.next_token
+        if not UtilClient.is_unset(request.region_id):
+            body['RegionId'] = request.region_id
+        body_flat = {}
+        if not UtilClient.is_unset(request.resource_id):
+            body_flat['ResourceId'] = request.resource_id
+        if not UtilClient.is_unset(request.resource_type):
+            body['ResourceType'] = request.resource_type
+        if not UtilClient.is_unset(request.tag):
+            body_flat['Tag'] = request.tag
+        body = TeaCore.merge(body,
+            OpenApiUtilClient.query(body_flat))
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='ListTagResources',
+            version='2021-09-31',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            bpstudio_20210931_models.ListTagResourcesResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def list_tag_resources(
+        self,
+        request: bpstudio_20210931_models.ListTagResourcesRequest,
+    ) -> bpstudio_20210931_models.ListTagResourcesResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.list_tag_resources_with_options(request, runtime)
+
+    async def list_tag_resources_async(
+        self,
+        request: bpstudio_20210931_models.ListTagResourcesRequest,
+    ) -> bpstudio_20210931_models.ListTagResourcesResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.list_tag_resources_with_options_async(request, runtime)
+
     def list_template_with_options(
         self,
         request: bpstudio_20210931_models.ListTemplateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> bpstudio_20210931_models.ListTemplateResponse:
         UtilClient.validate_model(request)
         body = {}
@@ -1176,7 +1272,109 @@
 
     async def valuate_application_async(
         self,
         request: bpstudio_20210931_models.ValuateApplicationRequest,
     ) -> bpstudio_20210931_models.ValuateApplicationResponse:
         runtime = util_models.RuntimeOptions()
         return await self.valuate_application_with_options_async(request, runtime)
+
+    def valuate_template_with_options(
+        self,
+        tmp_req: bpstudio_20210931_models.ValuateTemplateRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> bpstudio_20210931_models.ValuateTemplateResponse:
+        UtilClient.validate_model(tmp_req)
+        request = bpstudio_20210931_models.ValuateTemplateShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.instances):
+            request.instances_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.instances, 'Instances', 'json')
+        if not UtilClient.is_unset(tmp_req.variables):
+            request.variables_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.variables, 'Variables', 'json')
+        body = {}
+        if not UtilClient.is_unset(request.area_id):
+            body['AreaId'] = request.area_id
+        if not UtilClient.is_unset(request.client_token):
+            body['ClientToken'] = request.client_token
+        if not UtilClient.is_unset(request.instances_shrink):
+            body['Instances'] = request.instances_shrink
+        if not UtilClient.is_unset(request.resource_group_id):
+            body['ResourceGroupId'] = request.resource_group_id
+        if not UtilClient.is_unset(request.template_id):
+            body['TemplateId'] = request.template_id
+        if not UtilClient.is_unset(request.variables_shrink):
+            body['Variables'] = request.variables_shrink
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='ValuateTemplate',
+            version='2021-09-31',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            bpstudio_20210931_models.ValuateTemplateResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def valuate_template_with_options_async(
+        self,
+        tmp_req: bpstudio_20210931_models.ValuateTemplateRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> bpstudio_20210931_models.ValuateTemplateResponse:
+        UtilClient.validate_model(tmp_req)
+        request = bpstudio_20210931_models.ValuateTemplateShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.instances):
+            request.instances_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.instances, 'Instances', 'json')
+        if not UtilClient.is_unset(tmp_req.variables):
+            request.variables_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.variables, 'Variables', 'json')
+        body = {}
+        if not UtilClient.is_unset(request.area_id):
+            body['AreaId'] = request.area_id
+        if not UtilClient.is_unset(request.client_token):
+            body['ClientToken'] = request.client_token
+        if not UtilClient.is_unset(request.instances_shrink):
+            body['Instances'] = request.instances_shrink
+        if not UtilClient.is_unset(request.resource_group_id):
+            body['ResourceGroupId'] = request.resource_group_id
+        if not UtilClient.is_unset(request.template_id):
+            body['TemplateId'] = request.template_id
+        if not UtilClient.is_unset(request.variables_shrink):
+            body['Variables'] = request.variables_shrink
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='ValuateTemplate',
+            version='2021-09-31',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            bpstudio_20210931_models.ValuateTemplateResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def valuate_template(
+        self,
+        request: bpstudio_20210931_models.ValuateTemplateRequest,
+    ) -> bpstudio_20210931_models.ValuateTemplateResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.valuate_template_with_options(request, runtime)
+
+    async def valuate_template_async(
+        self,
+        request: bpstudio_20210931_models.ValuateTemplateRequest,
+    ) -> bpstudio_20210931_models.ValuateTemplateResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.valuate_template_with_options_async(request, runtime)
```

### Comparing `alibabacloud_bpstudio20210931-1.0.9/alibabacloud_bpstudio20210931.egg-info/PKG-INFO` & `alibabacloud_bpstudio20210931-2.0.0/alibabacloud_bpstudio20210931.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-bpstudio20210931
-Version: 1.0.9
+Version: 2.0.0
 Summary: Alibaba Cloud BPStudio (20210931) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_bpstudio20210931-1.0.9/setup.py` & `alibabacloud_bpstudio20210931-2.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_bpstudio20210931.
 
-Created on 14/03/2023
+Created on 20/06/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_bpstudio20210931"
 NAME = "alibabacloud_bpstudio20210931" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud BPStudio (20210931) SDK Library for Python"
```

