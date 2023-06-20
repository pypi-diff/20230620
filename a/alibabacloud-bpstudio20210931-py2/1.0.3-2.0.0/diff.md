# Comparing `tmp/alibabacloud_bpstudio20210931_py2-1.0.3.tar.gz` & `tmp/alibabacloud_bpstudio20210931_py2-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_bpstudio20210931_py2-1.0.3.tar", last modified: Mon May 22 09:08:04 2023, max compression
+gzip compressed data, was "dist/alibabacloud_bpstudio20210931_py2-2.0.0.tar", last modified: Tue Jun 20 05:59:37 2023, max compression
```

## Comparing `alibabacloud_bpstudio20210931_py2-1.0.3.tar` & `alibabacloud_bpstudio20210931_py2-2.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:08:04.000000 alibabacloud_bpstudio20210931_py2-1.0.3/
--rw-r--r--   0 root         (0) root         (0)      123 2023-05-22 09:08:04.000000 alibabacloud_bpstudio20210931_py2-1.0.3/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-05-22 09:08:04.000000 alibabacloud_bpstudio20210931_py2-1.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-05-22 09:08:04.000000 alibabacloud_bpstudio20210931_py2-1.0.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2502 2023-05-22 09:08:04.000000 alibabacloud_bpstudio20210931_py2-1.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1048 2023-05-22 09:08:04.000000 alibabacloud_bpstudio20210931_py2-1.0.3/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1131 2023-05-22 09:08:04.000000 alibabacloud_bpstudio20210931_py2-1.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:08:04.000000 alibabacloud_bpstudio20210931_py2-1.0.3/alibabacloud_bpstudio20210931/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-22 09:08:04.000000 alibabacloud_bpstudio20210931_py2-1.0.3/alibabacloud_bpstudio20210931/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21867 2023-05-22 09:08:04.000000 alibabacloud_bpstudio20210931_py2-1.0.3/alibabacloud_bpstudio20210931/client.py
--rw-r--r--   0 root         (0) root         (0)   104364 2023-05-22 09:08:04.000000 alibabacloud_bpstudio20210931_py2-1.0.3/alibabacloud_bpstudio20210931/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:08:04.000000 alibabacloud_bpstudio20210931_py2-1.0.3/alibabacloud_bpstudio20210931_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2502 2023-05-22 09:08:04.000000 alibabacloud_bpstudio20210931_py2-1.0.3/alibabacloud_bpstudio20210931_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      480 2023-05-22 09:08:04.000000 alibabacloud_bpstudio20210931_py2-1.0.3/alibabacloud_bpstudio20210931_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 09:08:04.000000 alibabacloud_bpstudio20210931_py2-1.0.3/alibabacloud_bpstudio20210931_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-05-22 09:08:04.000000 alibabacloud_bpstudio20210931_py2-1.0.3/alibabacloud_bpstudio20210931_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-05-22 09:08:04.000000 alibabacloud_bpstudio20210931_py2-1.0.3/alibabacloud_bpstudio20210931_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-22 09:08:04.000000 alibabacloud_bpstudio20210931_py2-1.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2928 2023-05-22 09:08:04.000000 alibabacloud_bpstudio20210931_py2-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 05:59:37.000000 alibabacloud_bpstudio20210931_py2-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)      180 2023-06-20 05:59:36.000000 alibabacloud_bpstudio20210931_py2-2.0.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-06-20 05:59:36.000000 alibabacloud_bpstudio20210931_py2-2.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-06-20 05:59:36.000000 alibabacloud_bpstudio20210931_py2-2.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2502 2023-06-20 05:59:37.000000 alibabacloud_bpstudio20210931_py2-2.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1048 2023-06-20 05:59:36.000000 alibabacloud_bpstudio20210931_py2-2.0.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-06-20 05:59:36.000000 alibabacloud_bpstudio20210931_py2-2.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 05:59:37.000000 alibabacloud_bpstudio20210931_py2-2.0.0/alibabacloud_bpstudio20210931/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-20 05:59:36.000000 alibabacloud_bpstudio20210931_py2-2.0.0/alibabacloud_bpstudio20210931/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23930 2023-06-20 05:59:36.000000 alibabacloud_bpstudio20210931_py2-2.0.0/alibabacloud_bpstudio20210931/client.py
+-rw-r--r--   0 root         (0) root         (0)   119210 2023-06-20 05:59:36.000000 alibabacloud_bpstudio20210931_py2-2.0.0/alibabacloud_bpstudio20210931/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 05:59:37.000000 alibabacloud_bpstudio20210931_py2-2.0.0/alibabacloud_bpstudio20210931_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2502 2023-06-20 05:59:37.000000 alibabacloud_bpstudio20210931_py2-2.0.0/alibabacloud_bpstudio20210931_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      480 2023-06-20 05:59:37.000000 alibabacloud_bpstudio20210931_py2-2.0.0/alibabacloud_bpstudio20210931_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 05:59:37.000000 alibabacloud_bpstudio20210931_py2-2.0.0/alibabacloud_bpstudio20210931_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-06-20 05:59:37.000000 alibabacloud_bpstudio20210931_py2-2.0.0/alibabacloud_bpstudio20210931_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-20 05:59:37.000000 alibabacloud_bpstudio20210931_py2-2.0.0/alibabacloud_bpstudio20210931_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-20 05:59:37.000000 alibabacloud_bpstudio20210931_py2-2.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2928 2023-06-20 05:59:36.000000 alibabacloud_bpstudio20210931_py2-2.0.0/setup.py
```

### Comparing `alibabacloud_bpstudio20210931_py2-1.0.3/LICENSE` & `alibabacloud_bpstudio20210931_py2-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_bpstudio20210931_py2-1.0.3/PKG-INFO` & `alibabacloud_bpstudio20210931_py2-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_bpstudio20210931_py2
-Version: 1.0.3
+Version: 2.0.0
 Summary: Alibaba Cloud BPStudio (20210931) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_bpstudio20210931_py2-1.0.3/README-CN.md` & `alibabacloud_bpstudio20210931_py2-2.0.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_bpstudio20210931_py2-1.0.3/README.md` & `alibabacloud_bpstudio20210931_py2-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_bpstudio20210931_py2-1.0.3/alibabacloud_bpstudio20210931/client.py` & `alibabacloud_bpstudio20210931_py2-2.0.0/alibabacloud_bpstudio20210931/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -538,7 +538,51 @@
             bpstudio_20210931_models.ValuateApplicationResponse(),
             self.call_api(params, req, runtime)
         )
 
     def valuate_application(self, request):
         runtime = util_models.RuntimeOptions()
         return self.valuate_application_with_options(request, runtime)
+
+    def valuate_template_with_options(self, tmp_req, runtime):
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
+    def valuate_template(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.valuate_template_with_options(request, runtime)
```

### Comparing `alibabacloud_bpstudio20210931_py2-1.0.3/alibabacloud_bpstudio20210931/models.py` & `alibabacloud_bpstudio20210931_py2-2.0.0/alibabacloud_bpstudio20210931/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -1019,15 +1019,15 @@
             self.status = m.get('Status')
         return self
 
 
 class GetApplicationResponseBodyData(TeaModel):
     def __init__(self, application_id=None, checklist=None, create_time=None, description=None, error=None,
                  image_url=None, name=None, price_list=None, resource_group_id=None, resource_list=None, status=None,
-                 template_id=None, topo_url=None):
+                 template_id=None):
         # The description of the application.
         self.application_id = application_id  # type: str
         # The resource tag.
         self.checklist = checklist  # type: list[GetApplicationResponseBodyDataChecklist]
         # The URL of the application topology image.
         self.create_time = create_time  # type: str
         # The message returned for the request.
@@ -1044,16 +1044,14 @@
         self.resource_group_id = resource_group_id  # type: str
         # The resource specification.
         self.resource_list = resource_list  # type: list[GetApplicationResponseBodyDataResourceList]
         # Verification passed
         self.status = status  # type: str
         # CADT application
         self.template_id = template_id  # type: str
-        # The ID of the application.
-        self.topo_url = topo_url  # type: str
 
     def validate(self):
         if self.checklist:
             for k in self.checklist:
                 if k:
                     k.validate()
         if self.price_list:
@@ -1097,16 +1095,14 @@
         if self.resource_list is not None:
             for k in self.resource_list:
                 result['ResourceList'].append(k.to_map() if k else None)
         if self.status is not None:
             result['Status'] = self.status
         if self.template_id is not None:
             result['TemplateId'] = self.template_id
-        if self.topo_url is not None:
-            result['TopoURL'] = self.topo_url
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('ApplicationId') is not None:
             self.application_id = m.get('ApplicationId')
         self.checklist = []
@@ -1136,16 +1132,14 @@
             for k in m.get('ResourceList'):
                 temp_model = GetApplicationResponseBodyDataResourceList()
                 self.resource_list.append(temp_model.from_map(k))
         if m.get('Status') is not None:
             self.status = m.get('Status')
         if m.get('TemplateId') is not None:
             self.template_id = m.get('TemplateId')
-        if m.get('TopoURL') is not None:
-            self.topo_url = m.get('TopoURL')
         return self
 
 
 class GetApplicationResponseBody(TeaModel):
     def __init__(self, code=None, data=None, message=None, request_id=None):
         # The deployment result.
         self.code = code  # type: int
@@ -1487,22 +1481,21 @@
         if m.get('Variable') is not None:
             self.variable = m.get('Variable')
         return self
 
 
 class GetTemplateResponseBodyData(TeaModel):
     def __init__(self, create_time=None, description=None, image_url=None, name=None, resource_group_id=None,
-                 template_id=None, topo_url=None, variables=None):
+                 template_id=None, variables=None):
         self.create_time = create_time  # type: str
         self.description = description  # type: str
         self.image_url = image_url  # type: str
         self.name = name  # type: str
         self.resource_group_id = resource_group_id  # type: str
         self.template_id = template_id  # type: str
-        self.topo_url = topo_url  # type: str
         self.variables = variables  # type: list[GetTemplateResponseBodyDataVariables]
 
     def validate(self):
         if self.variables:
             for k in self.variables:
                 if k:
                     k.validate()
@@ -1521,16 +1514,14 @@
             result['ImageURL'] = self.image_url
         if self.name is not None:
             result['Name'] = self.name
         if self.resource_group_id is not None:
             result['ResourceGroupId'] = self.resource_group_id
         if self.template_id is not None:
             result['TemplateId'] = self.template_id
-        if self.topo_url is not None:
-            result['TopoURL'] = self.topo_url
         result['Variables'] = []
         if self.variables is not None:
             for k in self.variables:
                 result['Variables'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m=None):
@@ -1543,16 +1534,14 @@
             self.image_url = m.get('ImageURL')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('ResourceGroupId') is not None:
             self.resource_group_id = m.get('ResourceGroupId')
         if m.get('TemplateId') is not None:
             self.template_id = m.get('TemplateId')
-        if m.get('TopoURL') is not None:
-            self.topo_url = m.get('TopoURL')
         self.variables = []
         if m.get('Variables') is not None:
             for k in m.get('Variables'):
                 temp_model = GetTemplateResponseBodyDataVariables()
                 self.variables.append(temp_model.from_map(k))
         return self
 
@@ -1852,22 +1841,21 @@
         if m.get('Status') is not None:
             self.status = m.get('Status')
         return self
 
 
 class ListApplicationResponseBodyData(TeaModel):
     def __init__(self, application_id=None, create_time=None, image_url=None, name=None, resource_group_id=None,
-                 status=None, topo_url=None):
+                 status=None):
         self.application_id = application_id  # type: str
         self.create_time = create_time  # type: str
         self.image_url = image_url  # type: str
         self.name = name  # type: str
         self.resource_group_id = resource_group_id  # type: str
         self.status = status  # type: str
-        self.topo_url = topo_url  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListApplicationResponseBodyData, self).to_map()
         if _map is not None:
@@ -1882,16 +1870,14 @@
             result['ImageURL'] = self.image_url
         if self.name is not None:
             result['Name'] = self.name
         if self.resource_group_id is not None:
             result['ResourceGroupId'] = self.resource_group_id
         if self.status is not None:
             result['Status'] = self.status
-        if self.topo_url is not None:
-            result['TopoURL'] = self.topo_url
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('ApplicationId') is not None:
             self.application_id = m.get('ApplicationId')
         if m.get('CreateTime') is not None:
@@ -1900,16 +1886,14 @@
             self.image_url = m.get('ImageURL')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('ResourceGroupId') is not None:
             self.resource_group_id = m.get('ResourceGroupId')
         if m.get('Status') is not None:
             self.status = m.get('Status')
-        if m.get('TopoURL') is not None:
-            self.topo_url = m.get('TopoURL')
         return self
 
 
 class ListApplicationResponseBody(TeaModel):
     def __init__(self, code=None, data=None, message=None, next_token=None, request_id=None, total_count=None):
         self.code = code  # type: int
         self.data = data  # type: list[ListApplicationResponseBodyData]
@@ -2003,15 +1987,17 @@
             temp_model = ListApplicationResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListTagResourcesRequestTag(TeaModel):
     def __init__(self, key=None, value=None):
+        # The key of the tag.
         self.key = key  # type: str
+        # The value of the tag.
         self.value = value  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListTagResourcesRequestTag, self).to_map()
@@ -2033,19 +2019,25 @@
             self.value = m.get('Value')
         return self
 
 
 class ListTagResourcesRequest(TeaModel):
     def __init__(self, client_token=None, next_token=None, region_id=None, resource_id=None, resource_type=None,
                  tag=None):
+        # The client token that is used to ensure the idempotence of the request.
         self.client_token = client_token  # type: str
+        # The pagination token that is used in the next request to retrieve a new page of results.
         self.next_token = next_token  # type: str
+        # The ID of the region.
         self.region_id = region_id  # type: str
+        # The resource IDs. You can specify a maximum number of 50 IDs.
         self.resource_id = resource_id  # type: list[str]
+        # The resource type.
         self.resource_type = resource_type  # type: str
+        # The tags. A maximum of 20 tags are supported.
         self.tag = tag  # type: list[ListTagResourcesRequestTag]
 
     def validate(self):
         if self.tag:
             for k in self.tag:
                 if k:
                     k.validate()
@@ -2090,17 +2082,21 @@
                 temp_model = ListTagResourcesRequestTag()
                 self.tag.append(temp_model.from_map(k))
         return self
 
 
 class ListTagResourcesResponseBodyTagResources(TeaModel):
     def __init__(self, resource_id=None, resource_type=None, tag_key=None, tag_value=None):
+        # The ID of the resource.
         self.resource_id = resource_id  # type: str
+        # The resource type. Valid values: application and template.
         self.resource_type = resource_type  # type: str
+        # The key of the tag.
         self.tag_key = tag_key  # type: str
+        # The value of the tag.
         self.tag_value = tag_value  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListTagResourcesResponseBodyTagResources, self).to_map()
@@ -2129,19 +2125,23 @@
         if m.get('TagValue') is not None:
             self.tag_value = m.get('TagValue')
         return self
 
 
 class ListTagResourcesResponseBody(TeaModel):
     def __init__(self, code=None, message=None, next_token=None, request_id=None, tag_resources=None):
+        # The HTTP status code. A value of 200 indicates that the request is successful.
         self.code = code  # type: str
+        # The error message returned if the request failed.
         self.message = message  # type: str
+        # The returned value of NextToken is a pagination token, which can be used in the next request to retrieve a new page of results. If the NextToken parameter is empty, no next page exists.
         self.next_token = next_token  # type: str
+        # The request ID.
         self.request_id = request_id  # type: str
-        # TagResource
+        # The tags that are added to the resources.
         self.tag_resources = tag_resources  # type: list[ListTagResourcesResponseBodyTagResources]
 
     def validate(self):
         if self.tag_resources:
             for k in self.tag_resources:
                 if k:
                     k.validate()
@@ -2286,31 +2286,29 @@
         if m.get('Type') is not None:
             self.type = m.get('Type')
         return self
 
 
 class ListTemplateResponseBodyData(TeaModel):
     def __init__(self, create_time=None, image_url=None, name=None, resource_group_id=None, tag_id=None,
-                 tag_name=None, template_id=None, topo_url=None):
+                 tag_name=None, template_id=None):
         # The time when the template was created.
         self.create_time = create_time  # type: str
         # The URL of the architecture image.
         self.image_url = image_url  # type: str
         # The name of the template.
         self.name = name  # type: str
         # The ID of the resource group.
         self.resource_group_id = resource_group_id  # type: str
         # The ID of the tag that is added to the template.
         self.tag_id = tag_id  # type: int
         # The name of the tag that is added to the template.
         self.tag_name = tag_name  # type: str
         # The ID of the template.
         self.template_id = template_id  # type: str
-        # The URL of the template topology image.
-        self.topo_url = topo_url  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListTemplateResponseBodyData, self).to_map()
         if _map is not None:
@@ -2327,16 +2325,14 @@
             result['ResourceGroupId'] = self.resource_group_id
         if self.tag_id is not None:
             result['TagId'] = self.tag_id
         if self.tag_name is not None:
             result['TagName'] = self.tag_name
         if self.template_id is not None:
             result['TemplateId'] = self.template_id
-        if self.topo_url is not None:
-            result['TopoURL'] = self.topo_url
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('CreateTime') is not None:
             self.create_time = m.get('CreateTime')
         if m.get('ImageURL') is not None:
@@ -2347,16 +2343,14 @@
             self.resource_group_id = m.get('ResourceGroupId')
         if m.get('TagId') is not None:
             self.tag_id = m.get('TagId')
         if m.get('TagName') is not None:
             self.tag_name = m.get('TagName')
         if m.get('TemplateId') is not None:
             self.template_id = m.get('TemplateId')
-        if m.get('TopoURL') is not None:
-            self.topo_url = m.get('TopoURL')
         return self
 
 
 class ListTemplateResponseBody(TeaModel):
     def __init__(self, code=None, data=None, message=None, next_token=None, request_id=None, total_count=None):
         # The HTTP status code.
         self.code = code  # type: int
@@ -2793,7 +2787,394 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ValuateApplicationResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ValuateTemplateRequestInstances(TeaModel):
+    def __init__(self, id=None, node_name=None, node_type=None):
+        self.id = id  # type: str
+        self.node_name = node_name  # type: str
+        self.node_type = node_type  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ValuateTemplateRequestInstances, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.id is not None:
+            result['Id'] = self.id
+        if self.node_name is not None:
+            result['NodeName'] = self.node_name
+        if self.node_type is not None:
+            result['NodeType'] = self.node_type
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Id') is not None:
+            self.id = m.get('Id')
+        if m.get('NodeName') is not None:
+            self.node_name = m.get('NodeName')
+        if m.get('NodeType') is not None:
+            self.node_type = m.get('NodeType')
+        return self
+
+
+class ValuateTemplateRequest(TeaModel):
+    def __init__(self, area_id=None, client_token=None, instances=None, resource_group_id=None, template_id=None,
+                 variables=None):
+        self.area_id = area_id  # type: str
+        self.client_token = client_token  # type: str
+        self.instances = instances  # type: list[ValuateTemplateRequestInstances]
+        self.resource_group_id = resource_group_id  # type: str
+        self.template_id = template_id  # type: str
+        self.variables = variables  # type: dict[str, str]
+
+    def validate(self):
+        if self.instances:
+            for k in self.instances:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(ValuateTemplateRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.area_id is not None:
+            result['AreaId'] = self.area_id
+        if self.client_token is not None:
+            result['ClientToken'] = self.client_token
+        result['Instances'] = []
+        if self.instances is not None:
+            for k in self.instances:
+                result['Instances'].append(k.to_map() if k else None)
+        if self.resource_group_id is not None:
+            result['ResourceGroupId'] = self.resource_group_id
+        if self.template_id is not None:
+            result['TemplateId'] = self.template_id
+        if self.variables is not None:
+            result['Variables'] = self.variables
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('AreaId') is not None:
+            self.area_id = m.get('AreaId')
+        if m.get('ClientToken') is not None:
+            self.client_token = m.get('ClientToken')
+        self.instances = []
+        if m.get('Instances') is not None:
+            for k in m.get('Instances'):
+                temp_model = ValuateTemplateRequestInstances()
+                self.instances.append(temp_model.from_map(k))
+        if m.get('ResourceGroupId') is not None:
+            self.resource_group_id = m.get('ResourceGroupId')
+        if m.get('TemplateId') is not None:
+            self.template_id = m.get('TemplateId')
+        if m.get('Variables') is not None:
+            self.variables = m.get('Variables')
+        return self
+
+
+class ValuateTemplateShrinkRequest(TeaModel):
+    def __init__(self, area_id=None, client_token=None, instances_shrink=None, resource_group_id=None,
+                 template_id=None, variables_shrink=None):
+        self.area_id = area_id  # type: str
+        self.client_token = client_token  # type: str
+        self.instances_shrink = instances_shrink  # type: str
+        self.resource_group_id = resource_group_id  # type: str
+        self.template_id = template_id  # type: str
+        self.variables_shrink = variables_shrink  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ValuateTemplateShrinkRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.area_id is not None:
+            result['AreaId'] = self.area_id
+        if self.client_token is not None:
+            result['ClientToken'] = self.client_token
+        if self.instances_shrink is not None:
+            result['Instances'] = self.instances_shrink
+        if self.resource_group_id is not None:
+            result['ResourceGroupId'] = self.resource_group_id
+        if self.template_id is not None:
+            result['TemplateId'] = self.template_id
+        if self.variables_shrink is not None:
+            result['Variables'] = self.variables_shrink
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('AreaId') is not None:
+            self.area_id = m.get('AreaId')
+        if m.get('ClientToken') is not None:
+            self.client_token = m.get('ClientToken')
+        if m.get('Instances') is not None:
+            self.instances_shrink = m.get('Instances')
+        if m.get('ResourceGroupId') is not None:
+            self.resource_group_id = m.get('ResourceGroupId')
+        if m.get('TemplateId') is not None:
+            self.template_id = m.get('TemplateId')
+        if m.get('Variables') is not None:
+            self.variables_shrink = m.get('Variables')
+        return self
+
+
+class ValuateTemplateResponseBodyDataResourceListPriceList(TeaModel):
+    def __init__(self, discount_amount=None, error=None, node_type=None, original_price=None, price_unit=None,
+                 promotion_name=None, resource_id=None, trade_price=None, type=None):
+        self.discount_amount = discount_amount  # type: float
+        self.error = error  # type: str
+        self.node_type = node_type  # type: str
+        self.original_price = original_price  # type: float
+        self.price_unit = price_unit  # type: str
+        self.promotion_name = promotion_name  # type: str
+        self.resource_id = resource_id  # type: str
+        self.trade_price = trade_price  # type: float
+        self.type = type  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ValuateTemplateResponseBodyDataResourceListPriceList, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.discount_amount is not None:
+            result['DiscountAmount'] = self.discount_amount
+        if self.error is not None:
+            result['Error'] = self.error
+        if self.node_type is not None:
+            result['NodeType'] = self.node_type
+        if self.original_price is not None:
+            result['OriginalPrice'] = self.original_price
+        if self.price_unit is not None:
+            result['PriceUnit'] = self.price_unit
+        if self.promotion_name is not None:
+            result['PromotionName'] = self.promotion_name
+        if self.resource_id is not None:
+            result['ResourceId'] = self.resource_id
+        if self.trade_price is not None:
+            result['TradePrice'] = self.trade_price
+        if self.type is not None:
+            result['Type'] = self.type
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('DiscountAmount') is not None:
+            self.discount_amount = m.get('DiscountAmount')
+        if m.get('Error') is not None:
+            self.error = m.get('Error')
+        if m.get('NodeType') is not None:
+            self.node_type = m.get('NodeType')
+        if m.get('OriginalPrice') is not None:
+            self.original_price = m.get('OriginalPrice')
+        if m.get('PriceUnit') is not None:
+            self.price_unit = m.get('PriceUnit')
+        if m.get('PromotionName') is not None:
+            self.promotion_name = m.get('PromotionName')
+        if m.get('ResourceId') is not None:
+            self.resource_id = m.get('ResourceId')
+        if m.get('TradePrice') is not None:
+            self.trade_price = m.get('TradePrice')
+        if m.get('Type') is not None:
+            self.type = m.get('Type')
+        return self
+
+
+class ValuateTemplateResponseBodyDataResourceList(TeaModel):
+    def __init__(self, discount_amount=None, error=None, node_type=None, original_price=None, price_list=None,
+                 price_unit=None, promotion_name=None, trade_price=None):
+        self.discount_amount = discount_amount  # type: float
+        self.error = error  # type: str
+        self.node_type = node_type  # type: str
+        self.original_price = original_price  # type: float
+        self.price_list = price_list  # type: list[ValuateTemplateResponseBodyDataResourceListPriceList]
+        self.price_unit = price_unit  # type: str
+        self.promotion_name = promotion_name  # type: str
+        self.trade_price = trade_price  # type: float
+
+    def validate(self):
+        if self.price_list:
+            for k in self.price_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(ValuateTemplateResponseBodyDataResourceList, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.discount_amount is not None:
+            result['DiscountAmount'] = self.discount_amount
+        if self.error is not None:
+            result['Error'] = self.error
+        if self.node_type is not None:
+            result['NodeType'] = self.node_type
+        if self.original_price is not None:
+            result['OriginalPrice'] = self.original_price
+        result['PriceList'] = []
+        if self.price_list is not None:
+            for k in self.price_list:
+                result['PriceList'].append(k.to_map() if k else None)
+        if self.price_unit is not None:
+            result['PriceUnit'] = self.price_unit
+        if self.promotion_name is not None:
+            result['PromotionName'] = self.promotion_name
+        if self.trade_price is not None:
+            result['TradePrice'] = self.trade_price
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('DiscountAmount') is not None:
+            self.discount_amount = m.get('DiscountAmount')
+        if m.get('Error') is not None:
+            self.error = m.get('Error')
+        if m.get('NodeType') is not None:
+            self.node_type = m.get('NodeType')
+        if m.get('OriginalPrice') is not None:
+            self.original_price = m.get('OriginalPrice')
+        self.price_list = []
+        if m.get('PriceList') is not None:
+            for k in m.get('PriceList'):
+                temp_model = ValuateTemplateResponseBodyDataResourceListPriceList()
+                self.price_list.append(temp_model.from_map(k))
+        if m.get('PriceUnit') is not None:
+            self.price_unit = m.get('PriceUnit')
+        if m.get('PromotionName') is not None:
+            self.promotion_name = m.get('PromotionName')
+        if m.get('TradePrice') is not None:
+            self.trade_price = m.get('TradePrice')
+        return self
+
+
+class ValuateTemplateResponseBodyData(TeaModel):
+    def __init__(self, resource_list=None):
+        self.resource_list = resource_list  # type: list[ValuateTemplateResponseBodyDataResourceList]
+
+    def validate(self):
+        if self.resource_list:
+            for k in self.resource_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(ValuateTemplateResponseBodyData, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['ResourceList'] = []
+        if self.resource_list is not None:
+            for k in self.resource_list:
+                result['ResourceList'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        self.resource_list = []
+        if m.get('ResourceList') is not None:
+            for k in m.get('ResourceList'):
+                temp_model = ValuateTemplateResponseBodyDataResourceList()
+                self.resource_list.append(temp_model.from_map(k))
+        return self
+
+
+class ValuateTemplateResponseBody(TeaModel):
+    def __init__(self, code=None, data=None, message=None, request_id=None):
+        self.code = code  # type: str
+        self.data = data  # type: ValuateTemplateResponseBodyData
+        self.message = message  # type: str
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super(ValuateTemplateResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Data') is not None:
+            temp_model = ValuateTemplateResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class ValuateTemplateResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: ValuateTemplateResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(ValuateTemplateResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ValuateTemplateResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
```

### Comparing `alibabacloud_bpstudio20210931_py2-1.0.3/alibabacloud_bpstudio20210931_py2.egg-info/PKG-INFO` & `alibabacloud_bpstudio20210931_py2-2.0.0/alibabacloud_bpstudio20210931_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-bpstudio20210931-py2
-Version: 1.0.3
+Version: 2.0.0
 Summary: Alibaba Cloud BPStudio (20210931) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_bpstudio20210931_py2-1.0.3/setup.py` & `alibabacloud_bpstudio20210931_py2-2.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_bpstudio20210931_py2.
 
-Created on 22/05/2023
+Created on 20/06/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_bpstudio20210931"
 NAME = "alibabacloud_bpstudio20210931_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud BPStudio (20210931) SDK Library for Python2"
```

