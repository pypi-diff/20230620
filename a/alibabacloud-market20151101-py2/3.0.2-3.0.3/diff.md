# Comparing `tmp/alibabacloud_market20151101_py2-3.0.2.tar.gz` & `tmp/alibabacloud_market20151101_py2-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_market20151101_py2-3.0.2.tar", last modified: Thu Mar 10 07:36:50 2022, max compression
+gzip compressed data, was "dist/alibabacloud_market20151101_py2-3.0.3.tar", last modified: Tue Jun 20 02:59:02 2023, max compression
```

## Comparing `alibabacloud_market20151101_py2-3.0.2.tar` & `alibabacloud_market20151101_py2-3.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 07:36:50.000000 alibabacloud_market20151101_py2-3.0.2/
--rw-r--r--   0 root         (0) root         (0)      173 2022-03-10 07:36:49.000000 alibabacloud_market20151101_py2-3.0.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2022-03-10 07:36:49.000000 alibabacloud_market20151101_py2-3.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2022-03-10 07:36:49.000000 alibabacloud_market20151101_py2-3.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2490 2022-03-10 07:36:50.000000 alibabacloud_market20151101_py2-3.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1042 2022-03-10 07:36:49.000000 alibabacloud_market20151101_py2-3.0.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1125 2022-03-10 07:36:49.000000 alibabacloud_market20151101_py2-3.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 07:36:50.000000 alibabacloud_market20151101_py2-3.0.2/alibabacloud_market20151101/
--rw-r--r--   0 root         (0) root         (0)       21 2022-03-10 07:36:49.000000 alibabacloud_market20151101_py2-3.0.2/alibabacloud_market20151101/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25597 2022-03-10 07:36:49.000000 alibabacloud_market20151101_py2-3.0.2/alibabacloud_market20151101/client.py
--rw-r--r--   0 root         (0) root         (0)   164296 2022-03-10 07:36:49.000000 alibabacloud_market20151101_py2-3.0.2/alibabacloud_market20151101/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 07:36:50.000000 alibabacloud_market20151101_py2-3.0.2/alibabacloud_market20151101_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2490 2022-03-10 07:36:49.000000 alibabacloud_market20151101_py2-3.0.2/alibabacloud_market20151101_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      464 2022-03-10 07:36:49.000000 alibabacloud_market20151101_py2-3.0.2/alibabacloud_market20151101_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-03-10 07:36:49.000000 alibabacloud_market20151101_py2-3.0.2/alibabacloud_market20151101_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2022-03-10 07:36:49.000000 alibabacloud_market20151101_py2-3.0.2/alibabacloud_market20151101_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       28 2022-03-10 07:36:49.000000 alibabacloud_market20151101_py2-3.0.2/alibabacloud_market20151101_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-03-10 07:36:50.000000 alibabacloud_market20151101_py2-3.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2918 2022-03-10 07:36:49.000000 alibabacloud_market20151101_py2-3.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:59:02.000000 alibabacloud_market20151101_py2-3.0.3/
+-rw-r--r--   0 root         (0) root         (0)      222 2023-06-20 02:59:02.000000 alibabacloud_market20151101_py2-3.0.3/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-06-20 02:59:02.000000 alibabacloud_market20151101_py2-3.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-06-20 02:59:02.000000 alibabacloud_market20151101_py2-3.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2490 2023-06-20 02:59:02.000000 alibabacloud_market20151101_py2-3.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1042 2023-06-20 02:59:02.000000 alibabacloud_market20151101_py2-3.0.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1125 2023-06-20 02:59:02.000000 alibabacloud_market20151101_py2-3.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:59:02.000000 alibabacloud_market20151101_py2-3.0.3/alibabacloud_market20151101/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-20 02:59:02.000000 alibabacloud_market20151101_py2-3.0.3/alibabacloud_market20151101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31737 2023-06-20 02:59:02.000000 alibabacloud_market20151101_py2-3.0.3/alibabacloud_market20151101/client.py
+-rw-r--r--   0 root         (0) root         (0)   202882 2023-06-20 02:59:02.000000 alibabacloud_market20151101_py2-3.0.3/alibabacloud_market20151101/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:59:02.000000 alibabacloud_market20151101_py2-3.0.3/alibabacloud_market20151101_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2490 2023-06-20 02:59:02.000000 alibabacloud_market20151101_py2-3.0.3/alibabacloud_market20151101_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      464 2023-06-20 02:59:02.000000 alibabacloud_market20151101_py2-3.0.3/alibabacloud_market20151101_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 02:59:02.000000 alibabacloud_market20151101_py2-3.0.3/alibabacloud_market20151101_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-06-20 02:59:02.000000 alibabacloud_market20151101_py2-3.0.3/alibabacloud_market20151101_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2023-06-20 02:59:02.000000 alibabacloud_market20151101_py2-3.0.3/alibabacloud_market20151101_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-20 02:59:02.000000 alibabacloud_market20151101_py2-3.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2918 2023-06-20 02:59:02.000000 alibabacloud_market20151101_py2-3.0.3/setup.py
```

### Comparing `alibabacloud_market20151101_py2-3.0.2/LICENSE` & `alibabacloud_market20151101_py2-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_market20151101_py2-3.0.2/PKG-INFO` & `alibabacloud_market20151101_py2-3.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_market20151101_py2
-Version: 3.0.2
+Version: 3.0.3
 Summary: Alibaba Cloud Market (20151101) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_market20151101_py2-3.0.2/README-CN.md` & `alibabacloud_market20151101_py2-3.0.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_market20151101_py2-3.0.2/README.md` & `alibabacloud_market20151101_py2-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_market20151101_py2-3.0.2/alibabacloud_market20151101/client.py` & `alibabacloud_market20151101_py2-3.0.3/alibabacloud_market20151101/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -81,14 +81,50 @@
             self.call_api(params, req, runtime)
         )
 
     def activate_license(self, request):
         runtime = util_models.RuntimeOptions()
         return self.activate_license_with_options(request, runtime)
 
+    def auto_renew_instance_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.auto_renew_cycle):
+            body['AutoRenewCycle'] = request.auto_renew_cycle
+        if not UtilClient.is_unset(request.auto_renew_duration):
+            body['AutoRenewDuration'] = request.auto_renew_duration
+        if not UtilClient.is_unset(request.order_biz_id):
+            body['OrderBizId'] = request.order_biz_id
+        if not UtilClient.is_unset(request.owner_id):
+            body['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.type):
+            body['Type'] = request.type
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='AutoRenewInstance',
+            version='2015-11-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            market_20151101_models.AutoRenewInstanceResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def auto_renew_instance(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.auto_renew_instance_with_options(request, runtime)
+
     def create_order_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.commodity):
             query['Commodity'] = request.commodity
@@ -119,14 +155,68 @@
             self.call_api(params, req, runtime)
         )
 
     def create_order(self, request):
         runtime = util_models.RuntimeOptions()
         return self.create_order_with_options(request, runtime)
 
+    def cross_account_verify_token_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.token):
+            body['Token'] = request.token
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='CrossAccountVerifyToken',
+            version='2015-11-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            market_20151101_models.CrossAccountVerifyTokenResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def cross_account_verify_token(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.cross_account_verify_token_with_options(request, runtime)
+
+    def describe_api_metering_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = OpenApiUtilClient.query(UtilClient.to_map(request))
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeApiMetering',
+            version='2015-11-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='GET',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            market_20151101_models.DescribeApiMeteringResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def describe_api_metering(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.describe_api_metering_with_options(request, runtime)
+
     def describe_current_node_info_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
@@ -147,14 +237,72 @@
             self.call_api(params, req, runtime)
         )
 
     def describe_current_node_info(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_current_node_info_with_options(request, runtime)
 
+    def describe_distribution_products_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = OpenApiUtilClient.query(UtilClient.to_map(request))
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeDistributionProducts',
+            version='2015-11-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='GET',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            market_20151101_models.DescribeDistributionProductsResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def describe_distribution_products(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.describe_distribution_products_with_options(request, runtime)
+
+    def describe_distribution_products_link_with_options(self, tmp_req, runtime):
+        UtilClient.validate_model(tmp_req)
+        request = market_20151101_models.DescribeDistributionProductsLinkShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.codes):
+            request.codes_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.codes, 'Codes', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.codes_shrink):
+            query['Codes'] = request.codes_shrink
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeDistributionProductsLink',
+            version='2015-11-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            market_20151101_models.DescribeDistributionProductsLinkResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def describe_distribution_products_link(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.describe_distribution_products_link_with_options(request, runtime)
+
     def describe_instance_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.order_type):
             query['OrderType'] = request.order_type
@@ -454,14 +602,25 @@
         )
 
     def describe_project_messages(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_project_messages_with_options(request, runtime)
 
     def describe_project_nodes_with_options(self, request, runtime):
+        """
+        *\
+        **\
+        
+
+        @param request: DescribeProjectNodesRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: DescribeProjectNodesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -478,14 +637,23 @@
         )
         return TeaCore.from_map(
             market_20151101_models.DescribeProjectNodesResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_project_nodes(self, request):
+        """
+        *\
+        **\
+        
+
+        @param request: DescribeProjectNodesRequest
+
+        @return: DescribeProjectNodesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_project_nodes_with_options(request, runtime)
 
     def describe_project_operate_logs_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
```

### Comparing `alibabacloud_market20151101_py2-3.0.2/alibabacloud_market20151101/models.py` & `alibabacloud_market20151101_py2-3.0.3/alibabacloud_market20151101/models.py`

 * *Files 15% similar despite different names*

```diff
@@ -58,46 +58,169 @@
             self.request_id = m.get('RequestId')
         if m.get('Success') is not None:
             self.success = m.get('Success')
         return self
 
 
 class ActivateLicenseResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: ActivateLicenseResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ActivateLicenseResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ActivateLicenseResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class AutoRenewInstanceRequest(TeaModel):
+    def __init__(self, auto_renew_cycle=None, auto_renew_duration=None, order_biz_id=None, owner_id=None, type=None):
+        self.auto_renew_cycle = auto_renew_cycle  # type: str
+        self.auto_renew_duration = auto_renew_duration  # type: int
+        self.order_biz_id = order_biz_id  # type: long
+        self.owner_id = owner_id  # type: long
+        self.type = type  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(AutoRenewInstanceRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auto_renew_cycle is not None:
+            result['AutoRenewCycle'] = self.auto_renew_cycle
+        if self.auto_renew_duration is not None:
+            result['AutoRenewDuration'] = self.auto_renew_duration
+        if self.order_biz_id is not None:
+            result['OrderBizId'] = self.order_biz_id
+        if self.owner_id is not None:
+            result['OwnerId'] = self.owner_id
+        if self.type is not None:
+            result['Type'] = self.type
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('AutoRenewCycle') is not None:
+            self.auto_renew_cycle = m.get('AutoRenewCycle')
+        if m.get('AutoRenewDuration') is not None:
+            self.auto_renew_duration = m.get('AutoRenewDuration')
+        if m.get('OrderBizId') is not None:
+            self.order_biz_id = m.get('OrderBizId')
+        if m.get('OwnerId') is not None:
+            self.owner_id = m.get('OwnerId')
+        if m.get('Type') is not None:
+            self.type = m.get('Type')
+        return self
+
+
+class AutoRenewInstanceResponseBody(TeaModel):
+    def __init__(self, data=None, request_id=None, success=None):
+        self.data = data  # type: bool
+        self.request_id = request_id  # type: str
+        self.success = success  # type: bool
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(AutoRenewInstanceResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.data is not None:
+            result['Data'] = self.data
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Data') is not None:
+            self.data = m.get('Data')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class AutoRenewInstanceResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: AutoRenewInstanceResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(AutoRenewInstanceResponse, self).to_map()
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
+            temp_model = AutoRenewInstanceResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class CreateOrderRequest(TeaModel):
     def __init__(self, client_token=None, commodity=None, order_souce=None, order_type=None, owner_id=None,
                  payment_type=None):
         self.client_token = client_token  # type: str
         self.commodity = commodity  # type: str
         self.order_souce = order_souce  # type: str
         self.order_type = order_type  # type: str
@@ -201,46 +324,403 @@
             self.order_id = m.get('OrderId')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class CreateOrderResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: CreateOrderResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(CreateOrderResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateOrderResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CrossAccountVerifyTokenRequest(TeaModel):
+    def __init__(self, token=None):
+        self.token = token  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CrossAccountVerifyTokenRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.token is not None:
+            result['Token'] = self.token
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Token') is not None:
+            self.token = m.get('Token')
+        return self
+
+
+class CrossAccountVerifyTokenResponseBodyResult(TeaModel):
+    def __init__(self, auth_roles=None, auth_time=None, name=None, uid=None):
+        self.auth_roles = auth_roles  # type: list[str]
+        self.auth_time = auth_time  # type: long
+        self.name = name  # type: str
+        self.uid = uid  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CrossAccountVerifyTokenResponseBodyResult, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_roles is not None:
+            result['AuthRoles'] = self.auth_roles
+        if self.auth_time is not None:
+            result['AuthTime'] = self.auth_time
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.uid is not None:
+            result['Uid'] = self.uid
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('AuthRoles') is not None:
+            self.auth_roles = m.get('AuthRoles')
+        if m.get('AuthTime') is not None:
+            self.auth_time = m.get('AuthTime')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('Uid') is not None:
+            self.uid = m.get('Uid')
+        return self
+
+
+class CrossAccountVerifyTokenResponseBody(TeaModel):
+    def __init__(self, code=None, message=None, request_id=None, result=None, success=None):
+        self.code = code  # type: str
+        self.message = message  # type: str
+        # RequestId
+        self.request_id = request_id  # type: str
+        self.result = result  # type: CrossAccountVerifyTokenResponseBodyResult
+        self.success = success  # type: bool
+
+    def validate(self):
+        if self.result:
+            self.result.validate()
+
+    def to_map(self):
+        _map = super(CrossAccountVerifyTokenResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.result is not None:
+            result['Result'] = self.result.to_map()
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Result') is not None:
+            temp_model = CrossAccountVerifyTokenResponseBodyResult()
+            self.result = temp_model.from_map(m['Result'])
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class CrossAccountVerifyTokenResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: CrossAccountVerifyTokenResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(CrossAccountVerifyTokenResponse, self).to_map()
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
+            temp_model = CrossAccountVerifyTokenResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class DescribeApiMeteringRequest(TeaModel):
+    def __init__(self, page_num=None, product_code=None, type=None):
+        self.page_num = page_num  # type: int
+        self.product_code = product_code  # type: str
+        self.type = type  # type: int
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeApiMeteringRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.page_num is not None:
+            result['pageNum'] = self.page_num
+        if self.product_code is not None:
+            result['productCode'] = self.product_code
+        if self.type is not None:
+            result['type'] = self.type
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('pageNum') is not None:
+            self.page_num = m.get('pageNum')
+        if m.get('productCode') is not None:
+            self.product_code = m.get('productCode')
+        if m.get('type') is not None:
+            self.type = m.get('type')
+        return self
+
+
+class DescribeApiMeteringResponseBodyResult(TeaModel):
+    def __init__(self, aliyun_pk=None, product_code=None, product_name=None, total_quota=None, total_usage=None,
+                 unit=None):
+        self.aliyun_pk = aliyun_pk  # type: long
+        self.product_code = product_code  # type: str
+        self.product_name = product_name  # type: str
+        self.total_quota = total_quota  # type: long
+        self.total_usage = total_usage  # type: long
+        self.unit = unit  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeApiMeteringResponseBodyResult, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.aliyun_pk is not None:
+            result['AliyunPk'] = self.aliyun_pk
+        if self.product_code is not None:
+            result['ProductCode'] = self.product_code
+        if self.product_name is not None:
+            result['ProductName'] = self.product_name
+        if self.total_quota is not None:
+            result['TotalQuota'] = self.total_quota
+        if self.total_usage is not None:
+            result['TotalUsage'] = self.total_usage
+        if self.unit is not None:
+            result['Unit'] = self.unit
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('AliyunPk') is not None:
+            self.aliyun_pk = m.get('AliyunPk')
+        if m.get('ProductCode') is not None:
+            self.product_code = m.get('ProductCode')
+        if m.get('ProductName') is not None:
+            self.product_name = m.get('ProductName')
+        if m.get('TotalQuota') is not None:
+            self.total_quota = m.get('TotalQuota')
+        if m.get('TotalUsage') is not None:
+            self.total_usage = m.get('TotalUsage')
+        if m.get('Unit') is not None:
+            self.unit = m.get('Unit')
+        return self
+
+
+class DescribeApiMeteringResponseBody(TeaModel):
+    def __init__(self, code=None, count=None, fatal=None, message=None, page_number=None, page_size=None,
+                 request_id=None, result=None, success=None, version=None):
+        self.code = code  # type: str
+        self.count = count  # type: long
+        # fatal
+        self.fatal = fatal  # type: bool
+        self.message = message  # type: str
+        self.page_number = page_number  # type: long
+        self.page_size = page_size  # type: long
+        self.request_id = request_id  # type: str
+        self.result = result  # type: list[DescribeApiMeteringResponseBodyResult]
+        self.success = success  # type: bool
+        self.version = version  # type: str
+
+    def validate(self):
+        if self.result:
+            for k in self.result:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DescribeApiMeteringResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.count is not None:
+            result['Count'] = self.count
+        if self.fatal is not None:
+            result['Fatal'] = self.fatal
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        result['Result'] = []
+        if self.result is not None:
+            for k in self.result:
+                result['Result'].append(k.to_map() if k else None)
+        if self.success is not None:
+            result['Success'] = self.success
+        if self.version is not None:
+            result['Version'] = self.version
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Count') is not None:
+            self.count = m.get('Count')
+        if m.get('Fatal') is not None:
+            self.fatal = m.get('Fatal')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        self.result = []
+        if m.get('Result') is not None:
+            for k in m.get('Result'):
+                temp_model = DescribeApiMeteringResponseBodyResult()
+                self.result.append(temp_model.from_map(k))
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        if m.get('Version') is not None:
+            self.version = m.get('Version')
+        return self
+
+
+class DescribeApiMeteringResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DescribeApiMeteringResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DescribeApiMeteringResponse, self).to_map()
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
+            temp_model = DescribeApiMeteringResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DescribeCurrentNodeInfoRequest(TeaModel):
     def __init__(self, instance_id=None):
         self.instance_id = instance_id  # type: str
 
     def validate(self):
         pass
 
@@ -396,46 +876,474 @@
             self.result = temp_model.from_map(m['Result'])
         if m.get('Success') is not None:
             self.success = m.get('Success')
         return self
 
 
 class DescribeCurrentNodeInfoResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DescribeCurrentNodeInfoResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeCurrentNodeInfoResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeCurrentNodeInfoResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DescribeDistributionProductsRequestFilter(TeaModel):
+    def __init__(self, key=None, value=None):
+        self.key = key  # type: str
+        self.value = value  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeDistributionProductsRequestFilter, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.key is not None:
+            result['Key'] = self.key
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
+class DescribeDistributionProductsRequest(TeaModel):
+    def __init__(self, filter=None, page_number=None, page_size=None):
+        self.filter = filter  # type: list[DescribeDistributionProductsRequestFilter]
+        self.page_number = page_number  # type: long
+        self.page_size = page_size  # type: long
+
+    def validate(self):
+        if self.filter:
+            for k in self.filter:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DescribeDistributionProductsRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['Filter'] = []
+        if self.filter is not None:
+            for k in self.filter:
+                result['Filter'].append(k.to_map() if k else None)
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        self.filter = []
+        if m.get('Filter') is not None:
+            for k in m.get('Filter'):
+                temp_model = DescribeDistributionProductsRequestFilter()
+                self.filter.append(temp_model.from_map(k))
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        return self
+
+
+class DescribeDistributionProductsResponseBodyResults(TeaModel):
+    def __init__(self, code=None, first_category_name=None, image_url=None, name=None, price=None, score=None,
+                 second_category_name=None, short_description=None, submission_radio=None, supplier_name=None, supplier_uid=None,
+                 trade_count=None, type=None, user_comment_count=None):
+        self.code = code  # type: str
+        self.first_category_name = first_category_name  # type: str
+        self.image_url = image_url  # type: str
+        self.name = name  # type: str
+        self.price = price  # type: str
+        self.score = score  # type: str
+        self.second_category_name = second_category_name  # type: str
+        self.short_description = short_description  # type: str
+        self.submission_radio = submission_radio  # type: str
+        self.supplier_name = supplier_name  # type: str
+        self.supplier_uid = supplier_uid  # type: str
+        self.trade_count = trade_count  # type: str
+        self.type = type  # type: str
+        self.user_comment_count = user_comment_count  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeDistributionProductsResponseBodyResults, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.first_category_name is not None:
+            result['FirstCategoryName'] = self.first_category_name
+        if self.image_url is not None:
+            result['ImageUrl'] = self.image_url
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.price is not None:
+            result['Price'] = self.price
+        if self.score is not None:
+            result['Score'] = self.score
+        if self.second_category_name is not None:
+            result['SecondCategoryName'] = self.second_category_name
+        if self.short_description is not None:
+            result['ShortDescription'] = self.short_description
+        if self.submission_radio is not None:
+            result['SubmissionRadio'] = self.submission_radio
+        if self.supplier_name is not None:
+            result['SupplierName'] = self.supplier_name
+        if self.supplier_uid is not None:
+            result['SupplierUId'] = self.supplier_uid
+        if self.trade_count is not None:
+            result['TradeCount'] = self.trade_count
+        if self.type is not None:
+            result['Type'] = self.type
+        if self.user_comment_count is not None:
+            result['UserCommentCount'] = self.user_comment_count
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('FirstCategoryName') is not None:
+            self.first_category_name = m.get('FirstCategoryName')
+        if m.get('ImageUrl') is not None:
+            self.image_url = m.get('ImageUrl')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('Price') is not None:
+            self.price = m.get('Price')
+        if m.get('Score') is not None:
+            self.score = m.get('Score')
+        if m.get('SecondCategoryName') is not None:
+            self.second_category_name = m.get('SecondCategoryName')
+        if m.get('ShortDescription') is not None:
+            self.short_description = m.get('ShortDescription')
+        if m.get('SubmissionRadio') is not None:
+            self.submission_radio = m.get('SubmissionRadio')
+        if m.get('SupplierName') is not None:
+            self.supplier_name = m.get('SupplierName')
+        if m.get('SupplierUId') is not None:
+            self.supplier_uid = m.get('SupplierUId')
+        if m.get('TradeCount') is not None:
+            self.trade_count = m.get('TradeCount')
+        if m.get('Type') is not None:
+            self.type = m.get('Type')
+        if m.get('UserCommentCount') is not None:
+            self.user_comment_count = m.get('UserCommentCount')
+        return self
+
+
+class DescribeDistributionProductsResponseBody(TeaModel):
+    def __init__(self, page_number=None, page_size=None, request_id=None, results=None, total_count=None):
+        self.page_number = page_number  # type: int
+        self.page_size = page_size  # type: int
+        self.request_id = request_id  # type: str
+        self.results = results  # type: list[DescribeDistributionProductsResponseBodyResults]
+        self.total_count = total_count  # type: int
+
+    def validate(self):
+        if self.results:
+            for k in self.results:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DescribeDistributionProductsResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        result['Results'] = []
+        if self.results is not None:
+            for k in self.results:
+                result['Results'].append(k.to_map() if k else None)
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        self.results = []
+        if m.get('Results') is not None:
+            for k in m.get('Results'):
+                temp_model = DescribeDistributionProductsResponseBodyResults()
+                self.results.append(temp_model.from_map(k))
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class DescribeDistributionProductsResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DescribeDistributionProductsResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DescribeDistributionProductsResponse, self).to_map()
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
+            temp_model = DescribeDistributionProductsResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class DescribeDistributionProductsLinkRequest(TeaModel):
+    def __init__(self, codes=None):
+        self.codes = codes  # type: list[str]
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeDistributionProductsLinkRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.codes is not None:
+            result['Codes'] = self.codes
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Codes') is not None:
+            self.codes = m.get('Codes')
+        return self
+
+
+class DescribeDistributionProductsLinkShrinkRequest(TeaModel):
+    def __init__(self, codes_shrink=None):
+        self.codes_shrink = codes_shrink  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeDistributionProductsLinkShrinkRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.codes_shrink is not None:
+            result['Codes'] = self.codes_shrink
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Codes') is not None:
+            self.codes_shrink = m.get('Codes')
+        return self
+
+
+class DescribeDistributionProductsLinkResponseBodyResult(TeaModel):
+    def __init__(self, code=None, name=None, url=None):
+        self.code = code  # type: str
+        self.name = name  # type: str
+        self.url = url  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeDistributionProductsLinkResponseBodyResult, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.url is not None:
+            result['Url'] = self.url
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('Url') is not None:
+            self.url = m.get('Url')
+        return self
+
+
+class DescribeDistributionProductsLinkResponseBody(TeaModel):
+    def __init__(self, request_id=None, result=None, success=None, total_count=None):
+        # Id of the request
+        self.request_id = request_id  # type: str
+        self.result = result  # type: list[DescribeDistributionProductsLinkResponseBodyResult]
+        self.success = success  # type: bool
+        self.total_count = total_count  # type: long
+
+    def validate(self):
+        if self.result:
+            for k in self.result:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DescribeDistributionProductsLinkResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        result['Result'] = []
+        if self.result is not None:
+            for k in self.result:
+                result['Result'].append(k.to_map() if k else None)
+        if self.success is not None:
+            result['Success'] = self.success
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        self.result = []
+        if m.get('Result') is not None:
+            for k in m.get('Result'):
+                temp_model = DescribeDistributionProductsLinkResponseBodyResult()
+                self.result.append(temp_model.from_map(k))
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class DescribeDistributionProductsLinkResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DescribeDistributionProductsLinkResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DescribeDistributionProductsLinkResponse, self).to_map()
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
+            temp_model = DescribeDistributionProductsLinkResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DescribeInstanceRequest(TeaModel):
     def __init__(self, instance_id=None, order_type=None, owner_id=None):
         self.instance_id = instance_id  # type: str
         self.order_type = order_type  # type: str
         self.owner_id = owner_id  # type: long
 
     def validate(self):
@@ -724,19 +1632,20 @@
         m = m or dict()
         if m.get('ServiceStatus') is not None:
             self.service_status = m.get('ServiceStatus')
         return self
 
 
 class DescribeInstanceResponseBody(TeaModel):
-    def __init__(self, app_json=None, began_on=None, component_json=None, constraints=None, created_on=None,
-                 end_on=None, extend_json=None, host_json=None, instance_id=None, is_trial=None, modules=None,
+    def __init__(self, app_json=None, auto_renewal=None, began_on=None, component_json=None, constraints=None,
+                 created_on=None, end_on=None, extend_json=None, host_json=None, instance_id=None, is_trial=None, modules=None,
                  order_id=None, product_code=None, product_name=None, product_sku_code=None, product_type=None,
                  relational_data=None, status=None, supplier_name=None):
         self.app_json = app_json  # type: str
+        self.auto_renewal = auto_renewal  # type: str
         self.began_on = began_on  # type: long
         self.component_json = component_json  # type: str
         self.constraints = constraints  # type: str
         self.created_on = created_on  # type: long
         self.end_on = end_on  # type: long
         self.extend_json = extend_json  # type: str
         self.host_json = host_json  # type: str
@@ -762,14 +1671,16 @@
         _map = super(DescribeInstanceResponseBody, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.app_json is not None:
             result['AppJson'] = self.app_json
+        if self.auto_renewal is not None:
+            result['AutoRenewal'] = self.auto_renewal
         if self.began_on is not None:
             result['BeganOn'] = self.began_on
         if self.component_json is not None:
             result['ComponentJson'] = self.component_json
         if self.constraints is not None:
             result['Constraints'] = self.constraints
         if self.created_on is not None:
@@ -804,14 +1715,16 @@
             result['SupplierName'] = self.supplier_name
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('AppJson') is not None:
             self.app_json = m.get('AppJson')
+        if m.get('AutoRenewal') is not None:
+            self.auto_renewal = m.get('AutoRenewal')
         if m.get('BeganOn') is not None:
             self.began_on = m.get('BeganOn')
         if m.get('ComponentJson') is not None:
             self.component_json = m.get('ComponentJson')
         if m.get('Constraints') is not None:
             self.constraints = m.get('Constraints')
         if m.get('CreatedOn') is not None:
@@ -846,40 +1759,46 @@
             self.status = m.get('Status')
         if m.get('SupplierName') is not None:
             self.supplier_name = m.get('SupplierName')
         return self
 
 
 class DescribeInstanceResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DescribeInstanceResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeInstanceResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeInstanceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeInstancesRequest(TeaModel):
@@ -1107,40 +2026,46 @@
             self.request_id = m.get('RequestId')
         if m.get('TotalCount') is not None:
             self.total_count = m.get('TotalCount')
         return self
 
 
 class DescribeInstancesResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DescribeInstancesResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeInstancesResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeInstancesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeLicenseRequest(TeaModel):
@@ -1381,40 +2306,46 @@
             self.license = temp_model.from_map(m['License'])
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class DescribeLicenseResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DescribeLicenseResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeLicenseResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeLicenseResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeOrderRequest(TeaModel):
@@ -1624,40 +2555,46 @@
             self.supplier_telephones = temp_model.from_map(m['SupplierTelephones'])
         if m.get('TotalPrice') is not None:
             self.total_price = m.get('TotalPrice')
         return self
 
 
 class DescribeOrderResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DescribeOrderResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeOrderResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeOrderResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribePriceRequest(TeaModel):
@@ -1925,48 +2862,55 @@
             self.promotion_rules = temp_model.from_map(m['PromotionRules'])
         if m.get('TradePrice') is not None:
             self.trade_price = m.get('TradePrice')
         return self
 
 
 class DescribePriceResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DescribePriceResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribePriceResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribePriceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeProductRequest(TeaModel):
     def __init__(self, ali_uid=None, code=None, query_draft=None):
+        # AliUid
         self.ali_uid = ali_uid  # type: str
         self.code = code  # type: str
         self.query_draft = query_draft  # type: bool
 
     def validate(self):
         pass
 
@@ -2722,40 +3666,46 @@
             self.type = m.get('Type')
         if m.get('UseCount') is not None:
             self.use_count = m.get('UseCount')
         return self
 
 
 class DescribeProductResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DescribeProductResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeProductResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeProductResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeProductsRequestFilter(TeaModel):
@@ -3010,40 +3960,46 @@
             self.request_id = m.get('RequestId')
         if m.get('TotalCount') is not None:
             self.total_count = m.get('TotalCount')
         return self
 
 
 class DescribeProductsResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DescribeProductsResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeProductsResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeProductsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeProjectAttachmentsRequest(TeaModel):
@@ -3205,40 +4161,46 @@
                 self.result.append(temp_model.from_map(k))
         if m.get('Success') is not None:
             self.success = m.get('Success')
         return self
 
 
 class DescribeProjectAttachmentsResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DescribeProjectAttachmentsResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeProjectAttachmentsResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeProjectAttachmentsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeProjectInfoRequest(TeaModel):
@@ -3405,40 +4367,46 @@
             self.result = temp_model.from_map(m['Result'])
         if m.get('Success') is not None:
             self.success = m.get('Success')
         return self
 
 
 class DescribeProjectInfoResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DescribeProjectInfoResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeProjectInfoResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeProjectInfoResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeProjectMessagesRequest(TeaModel):
@@ -3558,40 +4526,46 @@
             self.success = m.get('Success')
         if m.get('TotalCount') is not None:
             self.total_count = m.get('TotalCount')
         return self
 
 
 class DescribeProjectMessagesResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DescribeProjectMessagesResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeProjectMessagesResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeProjectMessagesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeProjectNodesRequest(TeaModel):
@@ -3759,40 +4733,46 @@
                 self.result.append(temp_model.from_map(k))
         if m.get('Success') is not None:
             self.success = m.get('Success')
         return self
 
 
 class DescribeProjectNodesResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DescribeProjectNodesResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeProjectNodesResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeProjectNodesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeProjectOperateLogsRequest(TeaModel):
@@ -3902,40 +4882,46 @@
                 self.result.append(temp_model.from_map(k))
         if m.get('Success') is not None:
             self.success = m.get('Success')
         return self
 
 
 class DescribeProjectOperateLogsResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DescribeProjectOperateLogsResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeProjectOperateLogsResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeProjectOperateLogsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class FinishCurrentProjectNodeRequest(TeaModel):
@@ -4008,40 +4994,46 @@
             self.result = m.get('Result')
         if m.get('Success') is not None:
             self.success = m.get('Success')
         return self
 
 
 class FinishCurrentProjectNodeResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: FinishCurrentProjectNodeResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(FinishCurrentProjectNodeResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = FinishCurrentProjectNodeResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class PauseProjectRequest(TeaModel):
@@ -4109,40 +5101,46 @@
             self.result = m.get('Result')
         if m.get('Success') is not None:
             self.success = m.get('Success')
         return self
 
 
 class PauseProjectResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: PauseProjectResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(PauseProjectResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = PauseProjectResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class PushMeteringDataRequest(TeaModel):
@@ -4195,40 +5193,46 @@
             self.request_id = m.get('RequestId')
         if m.get('Success') is not None:
             self.success = m.get('Success')
         return self
 
 
 class PushMeteringDataResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: PushMeteringDataResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(PushMeteringDataResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = PushMeteringDataResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ResumeProjectRequest(TeaModel):
@@ -4296,40 +5300,46 @@
             self.result = m.get('Result')
         if m.get('Success') is not None:
             self.success = m.get('Success')
         return self
 
 
 class ResumeProjectResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: ResumeProjectResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ResumeProjectResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ResumeProjectResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RollbackCurrentProjectNodeRequest(TeaModel):
@@ -4397,39 +5407,45 @@
             self.result = m.get('Result')
         if m.get('Success') is not None:
             self.success = m.get('Success')
         return self
 
 
 class RollbackCurrentProjectNodeResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: RollbackCurrentProjectNodeResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(RollbackCurrentProjectNodeResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = RollbackCurrentProjectNodeResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
```

### Comparing `alibabacloud_market20151101_py2-3.0.2/alibabacloud_market20151101_py2.egg-info/PKG-INFO` & `alibabacloud_market20151101_py2-3.0.3/alibabacloud_market20151101_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-market20151101-py2
-Version: 3.0.2
+Version: 3.0.3
 Summary: Alibaba Cloud Market (20151101) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_market20151101_py2-3.0.2/setup.py` & `alibabacloud_market20151101_py2-3.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,30 +21,30 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_market20151101_py2.
 
-Created on 10/03/2022
+Created on 20/06/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_market20151101"
 NAME = "alibabacloud_market20151101_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Market (20151101) SDK Library for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python2-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util_py2>=0.0.5, <1.0.0",
-    "alibabacloud_tea_openapi_py2>=0.1.1, <1.0.0",
-    "alibabacloud_openapi_util_py2>=0.0.8, <1.0.0",
+    "alibabacloud_tea_util_py2>=0.0.7, <1.0.0",
+    "alibabacloud_tea_openapi_py2>=0.1.6, <1.0.0",
+    "alibabacloud_openapi_util_py2>=0.1.1, <1.0.0",
     "alibabacloud_endpoint_util_py2>=0.0.2, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 
 if os.path.exists('./README.md'):
     if sys.version_info.major == 2:
```

