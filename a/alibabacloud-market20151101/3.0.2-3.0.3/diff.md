# Comparing `tmp/alibabacloud_market20151101-3.0.2.tar.gz` & `tmp/alibabacloud_market20151101-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_market20151101-3.0.2.tar", last modified: Thu Mar 10 07:36:52 2022, max compression
+gzip compressed data, was "dist/alibabacloud_market20151101-3.0.3.tar", last modified: Tue Jun 20 02:59:35 2023, max compression
```

## Comparing `alibabacloud_market20151101-3.0.2.tar` & `alibabacloud_market20151101-3.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 07:36:52.000000 alibabacloud_market20151101-3.0.2/
--rw-r--r--   0 root         (0) root         (0)      173 2022-03-10 07:36:51.000000 alibabacloud_market20151101-3.0.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2022-03-10 07:36:51.000000 alibabacloud_market20151101-3.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-03-10 07:36:51.000000 alibabacloud_market20151101-3.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2346 2022-03-10 07:36:52.000000 alibabacloud_market20151101-3.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1031 2022-03-10 07:36:51.000000 alibabacloud_market20151101-3.0.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1116 2022-03-10 07:36:51.000000 alibabacloud_market20151101-3.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 07:36:52.000000 alibabacloud_market20151101-3.0.2/alibabacloud_market20151101/
--rw-r--r--   0 root         (0) root         (0)       21 2022-03-10 07:36:51.000000 alibabacloud_market20151101-3.0.2/alibabacloud_market20151101/__init__.py
--rw-r--r--   0 root         (0) root         (0)    61012 2022-03-10 07:36:51.000000 alibabacloud_market20151101-3.0.2/alibabacloud_market20151101/client.py
--rw-r--r--   0 root         (0) root         (0)   162479 2022-03-10 07:36:51.000000 alibabacloud_market20151101-3.0.2/alibabacloud_market20151101/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-10 07:36:52.000000 alibabacloud_market20151101-3.0.2/alibabacloud_market20151101.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2346 2022-03-10 07:36:52.000000 alibabacloud_market20151101-3.0.2/alibabacloud_market20151101.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      444 2022-03-10 07:36:52.000000 alibabacloud_market20151101-3.0.2/alibabacloud_market20151101.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-03-10 07:36:52.000000 alibabacloud_market20151101-3.0.2/alibabacloud_market20151101.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2022-03-10 07:36:52.000000 alibabacloud_market20151101-3.0.2/alibabacloud_market20151101.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       28 2022-03-10 07:36:52.000000 alibabacloud_market20151101-3.0.2/alibabacloud_market20151101.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-03-10 07:36:52.000000 alibabacloud_market20151101-3.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2625 2022-03-10 07:36:51.000000 alibabacloud_market20151101-3.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:59:35.000000 alibabacloud_market20151101-3.0.3/
+-rw-r--r--   0 root         (0) root         (0)      222 2023-06-20 02:59:35.000000 alibabacloud_market20151101-3.0.3/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-20 02:59:35.000000 alibabacloud_market20151101-3.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-20 02:59:35.000000 alibabacloud_market20151101-3.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2346 2023-06-20 02:59:35.000000 alibabacloud_market20151101-3.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1031 2023-06-20 02:59:35.000000 alibabacloud_market20151101-3.0.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1116 2023-06-20 02:59:35.000000 alibabacloud_market20151101-3.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:59:35.000000 alibabacloud_market20151101-3.0.3/alibabacloud_market20151101/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-20 02:59:35.000000 alibabacloud_market20151101-3.0.3/alibabacloud_market20151101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    76634 2023-06-20 02:59:35.000000 alibabacloud_market20151101-3.0.3/alibabacloud_market20151101/client.py
+-rw-r--r--   0 root         (0) root         (0)   200801 2023-06-20 02:59:35.000000 alibabacloud_market20151101-3.0.3/alibabacloud_market20151101/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:59:35.000000 alibabacloud_market20151101-3.0.3/alibabacloud_market20151101.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2346 2023-06-20 02:59:35.000000 alibabacloud_market20151101-3.0.3/alibabacloud_market20151101.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      444 2023-06-20 02:59:35.000000 alibabacloud_market20151101-3.0.3/alibabacloud_market20151101.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 02:59:35.000000 alibabacloud_market20151101-3.0.3/alibabacloud_market20151101.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-06-20 02:59:35.000000 alibabacloud_market20151101-3.0.3/alibabacloud_market20151101.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2023-06-20 02:59:35.000000 alibabacloud_market20151101-3.0.3/alibabacloud_market20151101.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-20 02:59:35.000000 alibabacloud_market20151101-3.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2625 2023-06-20 02:59:35.000000 alibabacloud_market20151101-3.0.3/setup.py
```

### Comparing `alibabacloud_market20151101-3.0.2/LICENSE` & `alibabacloud_market20151101-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_market20151101-3.0.2/PKG-INFO` & `alibabacloud_market20151101-3.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_market20151101
-Version: 3.0.2
+Version: 3.0.3
 Summary: Alibaba Cloud Market (20151101) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_market20151101-3.0.2/README-CN.md` & `alibabacloud_market20151101-3.0.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_market20151101-3.0.2/README.md` & `alibabacloud_market20151101-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_market20151101-3.0.2/alibabacloud_market20151101/client.py` & `alibabacloud_market20151101-3.0.3/alibabacloud_market20151101/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -136,14 +136,100 @@
     async def activate_license_async(
         self,
         request: market_20151101_models.ActivateLicenseRequest,
     ) -> market_20151101_models.ActivateLicenseResponse:
         runtime = util_models.RuntimeOptions()
         return await self.activate_license_with_options_async(request, runtime)
 
+    def auto_renew_instance_with_options(
+        self,
+        request: market_20151101_models.AutoRenewInstanceRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> market_20151101_models.AutoRenewInstanceResponse:
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
+    async def auto_renew_instance_with_options_async(
+        self,
+        request: market_20151101_models.AutoRenewInstanceRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> market_20151101_models.AutoRenewInstanceResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def auto_renew_instance(
+        self,
+        request: market_20151101_models.AutoRenewInstanceRequest,
+    ) -> market_20151101_models.AutoRenewInstanceResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.auto_renew_instance_with_options(request, runtime)
+
+    async def auto_renew_instance_async(
+        self,
+        request: market_20151101_models.AutoRenewInstanceRequest,
+    ) -> market_20151101_models.AutoRenewInstanceResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.auto_renew_instance_with_options_async(request, runtime)
+
     def create_order_with_options(
         self,
         request: market_20151101_models.CreateOrderRequest,
         runtime: util_models.RuntimeOptions,
     ) -> market_20151101_models.CreateOrderResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -226,14 +312,150 @@
     async def create_order_async(
         self,
         request: market_20151101_models.CreateOrderRequest,
     ) -> market_20151101_models.CreateOrderResponse:
         runtime = util_models.RuntimeOptions()
         return await self.create_order_with_options_async(request, runtime)
 
+    def cross_account_verify_token_with_options(
+        self,
+        request: market_20151101_models.CrossAccountVerifyTokenRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> market_20151101_models.CrossAccountVerifyTokenResponse:
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
+    async def cross_account_verify_token_with_options_async(
+        self,
+        request: market_20151101_models.CrossAccountVerifyTokenRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> market_20151101_models.CrossAccountVerifyTokenResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def cross_account_verify_token(
+        self,
+        request: market_20151101_models.CrossAccountVerifyTokenRequest,
+    ) -> market_20151101_models.CrossAccountVerifyTokenResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.cross_account_verify_token_with_options(request, runtime)
+
+    async def cross_account_verify_token_async(
+        self,
+        request: market_20151101_models.CrossAccountVerifyTokenRequest,
+    ) -> market_20151101_models.CrossAccountVerifyTokenResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.cross_account_verify_token_with_options_async(request, runtime)
+
+    def describe_api_metering_with_options(
+        self,
+        request: market_20151101_models.DescribeApiMeteringRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> market_20151101_models.DescribeApiMeteringResponse:
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
+    async def describe_api_metering_with_options_async(
+        self,
+        request: market_20151101_models.DescribeApiMeteringRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> market_20151101_models.DescribeApiMeteringResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_api_metering(
+        self,
+        request: market_20151101_models.DescribeApiMeteringRequest,
+    ) -> market_20151101_models.DescribeApiMeteringResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_api_metering_with_options(request, runtime)
+
+    async def describe_api_metering_async(
+        self,
+        request: market_20151101_models.DescribeApiMeteringRequest,
+    ) -> market_20151101_models.DescribeApiMeteringResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_api_metering_with_options_async(request, runtime)
+
     def describe_current_node_info_with_options(
         self,
         request: market_20151101_models.DescribeCurrentNodeInfoRequest,
         runtime: util_models.RuntimeOptions,
     ) -> market_20151101_models.DescribeCurrentNodeInfoResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -296,14 +518,158 @@
     async def describe_current_node_info_async(
         self,
         request: market_20151101_models.DescribeCurrentNodeInfoRequest,
     ) -> market_20151101_models.DescribeCurrentNodeInfoResponse:
         runtime = util_models.RuntimeOptions()
         return await self.describe_current_node_info_with_options_async(request, runtime)
 
+    def describe_distribution_products_with_options(
+        self,
+        request: market_20151101_models.DescribeDistributionProductsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> market_20151101_models.DescribeDistributionProductsResponse:
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
+    async def describe_distribution_products_with_options_async(
+        self,
+        request: market_20151101_models.DescribeDistributionProductsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> market_20151101_models.DescribeDistributionProductsResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_distribution_products(
+        self,
+        request: market_20151101_models.DescribeDistributionProductsRequest,
+    ) -> market_20151101_models.DescribeDistributionProductsResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_distribution_products_with_options(request, runtime)
+
+    async def describe_distribution_products_async(
+        self,
+        request: market_20151101_models.DescribeDistributionProductsRequest,
+    ) -> market_20151101_models.DescribeDistributionProductsResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_distribution_products_with_options_async(request, runtime)
+
+    def describe_distribution_products_link_with_options(
+        self,
+        tmp_req: market_20151101_models.DescribeDistributionProductsLinkRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> market_20151101_models.DescribeDistributionProductsLinkResponse:
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
+    async def describe_distribution_products_link_with_options_async(
+        self,
+        tmp_req: market_20151101_models.DescribeDistributionProductsLinkRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> market_20151101_models.DescribeDistributionProductsLinkResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_distribution_products_link(
+        self,
+        request: market_20151101_models.DescribeDistributionProductsLinkRequest,
+    ) -> market_20151101_models.DescribeDistributionProductsLinkResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_distribution_products_link_with_options(request, runtime)
+
+    async def describe_distribution_products_link_async(
+        self,
+        request: market_20151101_models.DescribeDistributionProductsLinkRequest,
+    ) -> market_20151101_models.DescribeDistributionProductsLinkResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_distribution_products_link_with_options_async(request, runtime)
+
     def describe_instance_with_options(
         self,
         request: market_20151101_models.DescribeInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> market_20151101_models.DescribeInstanceResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -1053,14 +1419,22 @@
         return await self.describe_project_messages_with_options_async(request, runtime)
 
     def describe_project_nodes_with_options(
         self,
         request: market_20151101_models.DescribeProjectNodesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> market_20151101_models.DescribeProjectNodesResponse:
+        """
+        *\
+        **\
+        
+        @param request: DescribeProjectNodesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeProjectNodesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -1081,14 +1455,22 @@
         )
 
     async def describe_project_nodes_with_options_async(
         self,
         request: market_20151101_models.DescribeProjectNodesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> market_20151101_models.DescribeProjectNodesResponse:
+        """
+        *\
+        **\
+        
+        @param request: DescribeProjectNodesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeProjectNodesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -1108,21 +1490,35 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_project_nodes(
         self,
         request: market_20151101_models.DescribeProjectNodesRequest,
     ) -> market_20151101_models.DescribeProjectNodesResponse:
+        """
+        *\
+        **\
+        
+        @param request: DescribeProjectNodesRequest
+        @return: DescribeProjectNodesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_project_nodes_with_options(request, runtime)
 
     async def describe_project_nodes_async(
         self,
         request: market_20151101_models.DescribeProjectNodesRequest,
     ) -> market_20151101_models.DescribeProjectNodesResponse:
+        """
+        *\
+        **\
+        
+        @param request: DescribeProjectNodesRequest
+        @return: DescribeProjectNodesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_project_nodes_with_options_async(request, runtime)
 
     def describe_project_operate_logs_with_options(
         self,
         request: market_20151101_models.DescribeProjectOperateLogsRequest,
         runtime: util_models.RuntimeOptions,
```

### Comparing `alibabacloud_market20151101-3.0.2/alibabacloud_market20151101/models.py` & `alibabacloud_market20151101-3.0.3/alibabacloud_market20151101/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -70,47 +70,188 @@
         return self
 
 
 class ActivateLicenseResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: ActivateLicenseResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        auto_renew_cycle: str = None,
+        auto_renew_duration: int = None,
+        order_biz_id: int = None,
+        owner_id: int = None,
+        type: str = None,
+    ):
+        self.auto_renew_cycle = auto_renew_cycle
+        self.auto_renew_duration = auto_renew_duration
+        self.order_biz_id = order_biz_id
+        self.owner_id = owner_id
+        self.type = type
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        data: bool = None,
+        request_id: str = None,
+        success: bool = None,
+    ):
+        self.data = data
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: AutoRenewInstanceResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
     def __init__(
         self,
         client_token: str = None,
         commodity: str = None,
         order_souce: str = None,
         order_type: str = None,
@@ -232,47 +373,454 @@
         return self
 
 
 class CreateOrderResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: CreateOrderResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        token: str = None,
+    ):
+        self.token = token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.token is not None:
+            result['Token'] = self.token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Token') is not None:
+            self.token = m.get('Token')
+        return self
+
+
+class CrossAccountVerifyTokenResponseBodyResult(TeaModel):
+    def __init__(
+        self,
+        auth_roles: List[str] = None,
+        auth_time: int = None,
+        name: str = None,
+        uid: str = None,
+    ):
+        self.auth_roles = auth_roles
+        self.auth_time = auth_time
+        self.name = name
+        self.uid = uid
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        code: str = None,
+        message: str = None,
+        request_id: str = None,
+        result: CrossAccountVerifyTokenResponseBodyResult = None,
+        success: bool = None,
+    ):
+        self.code = code
+        self.message = message
+        # RequestId
+        self.request_id = request_id
+        self.result = result
+        self.success = success
+
+    def validate(self):
+        if self.result:
+            self.result.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: CrossAccountVerifyTokenResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        page_num: int = None,
+        product_code: str = None,
+        type: int = None,
+    ):
+        self.page_num = page_num
+        self.product_code = product_code
+        self.type = type
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        aliyun_pk: int = None,
+        product_code: str = None,
+        product_name: str = None,
+        total_quota: int = None,
+        total_usage: int = None,
+        unit: str = None,
+    ):
+        self.aliyun_pk = aliyun_pk
+        self.product_code = product_code
+        self.product_name = product_name
+        self.total_quota = total_quota
+        self.total_usage = total_usage
+        self.unit = unit
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        code: str = None,
+        count: int = None,
+        fatal: bool = None,
+        message: str = None,
+        page_number: int = None,
+        page_size: int = None,
+        request_id: str = None,
+        result: List[DescribeApiMeteringResponseBodyResult] = None,
+        success: bool = None,
+        version: str = None,
+    ):
+        self.code = code
+        self.count = count
+        # fatal
+        self.fatal = fatal
+        self.message = message
+        self.page_number = page_number
+        self.page_size = page_size
+        self.request_id = request_id
+        self.result = result
+        self.success = success
+        self.version = version
+
+    def validate(self):
+        if self.result:
+            for k in self.result:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribeApiMeteringResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
     def __init__(
         self,
         instance_id: str = None,
     ):
         self.instance_id = instance_id
 
@@ -454,47 +1002,533 @@
         return self
 
 
 class DescribeCurrentNodeInfoResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeCurrentNodeInfoResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        key: str = None,
+        value: str = None,
+    ):
+        self.key = key
+        self.value = value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
+class DescribeDistributionProductsRequest(TeaModel):
+    def __init__(
+        self,
+        filter: List[DescribeDistributionProductsRequestFilter] = None,
+        page_number: int = None,
+        page_size: int = None,
+    ):
+        self.filter = filter
+        self.page_number = page_number
+        self.page_size = page_size
+
+    def validate(self):
+        if self.filter:
+            for k in self.filter:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        code: str = None,
+        first_category_name: str = None,
+        image_url: str = None,
+        name: str = None,
+        price: str = None,
+        score: str = None,
+        second_category_name: str = None,
+        short_description: str = None,
+        submission_radio: str = None,
+        supplier_name: str = None,
+        supplier_uid: str = None,
+        trade_count: str = None,
+        type: str = None,
+        user_comment_count: str = None,
+    ):
+        self.code = code
+        self.first_category_name = first_category_name
+        self.image_url = image_url
+        self.name = name
+        self.price = price
+        self.score = score
+        self.second_category_name = second_category_name
+        self.short_description = short_description
+        self.submission_radio = submission_radio
+        self.supplier_name = supplier_name
+        self.supplier_uid = supplier_uid
+        self.trade_count = trade_count
+        self.type = type
+        self.user_comment_count = user_comment_count
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        page_number: int = None,
+        page_size: int = None,
+        request_id: str = None,
+        results: List[DescribeDistributionProductsResponseBodyResults] = None,
+        total_count: int = None,
+    ):
+        self.page_number = page_number
+        self.page_size = page_size
+        self.request_id = request_id
+        self.results = results
+        self.total_count = total_count
+
+    def validate(self):
+        if self.results:
+            for k in self.results:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribeDistributionProductsResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        codes: List[str] = None,
+    ):
+        self.codes = codes
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.codes is not None:
+            result['Codes'] = self.codes
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Codes') is not None:
+            self.codes = m.get('Codes')
+        return self
+
+
+class DescribeDistributionProductsLinkShrinkRequest(TeaModel):
+    def __init__(
+        self,
+        codes_shrink: str = None,
+    ):
+        self.codes_shrink = codes_shrink
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.codes_shrink is not None:
+            result['Codes'] = self.codes_shrink
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Codes') is not None:
+            self.codes_shrink = m.get('Codes')
+        return self
+
+
+class DescribeDistributionProductsLinkResponseBodyResult(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        name: str = None,
+        url: str = None,
+    ):
+        self.code = code
+        self.name = name
+        self.url = url
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        request_id: str = None,
+        result: List[DescribeDistributionProductsLinkResponseBodyResult] = None,
+        success: bool = None,
+        total_count: int = None,
+    ):
+        # Id of the request
+        self.request_id = request_id
+        self.result = result
+        self.success = success
+        self.total_count = total_count
+
+    def validate(self):
+        if self.result:
+            for k in self.result:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribeDistributionProductsLinkResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
     def __init__(
         self,
         instance_id: str = None,
         order_type: str = None,
         owner_id: int = None,
     ):
@@ -825,14 +1859,15 @@
         return self
 
 
 class DescribeInstanceResponseBody(TeaModel):
     def __init__(
         self,
         app_json: str = None,
+        auto_renewal: str = None,
         began_on: int = None,
         component_json: str = None,
         constraints: str = None,
         created_on: int = None,
         end_on: int = None,
         extend_json: str = None,
         host_json: str = None,
@@ -845,14 +1880,15 @@
         product_sku_code: str = None,
         product_type: str = None,
         relational_data: DescribeInstanceResponseBodyRelationalData = None,
         status: str = None,
         supplier_name: str = None,
     ):
         self.app_json = app_json
+        self.auto_renewal = auto_renewal
         self.began_on = began_on
         self.component_json = component_json
         self.constraints = constraints
         self.created_on = created_on
         self.end_on = end_on
         self.extend_json = extend_json
         self.host_json = host_json
@@ -878,14 +1914,16 @@
         _map = super().to_map()
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
@@ -920,14 +1958,16 @@
             result['SupplierName'] = self.supplier_name
         return result
 
     def from_map(self, m: dict = None):
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
@@ -965,41 +2005,48 @@
         return self
 
 
 class DescribeInstanceResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeInstanceResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -1264,41 +2311,48 @@
         return self
 
 
 class DescribeInstancesResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeInstancesResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -1574,41 +2628,48 @@
         return self
 
 
 class DescribeLicenseResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeLicenseResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -1850,41 +2911,48 @@
         return self
 
 
 class DescribeOrderResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeOrderResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -2190,54 +3258,62 @@
         return self
 
 
 class DescribePriceResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribePriceResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
     def __init__(
         self,
         ali_uid: str = None,
         code: str = None,
         query_draft: bool = None,
     ):
+        # AliUid
         self.ali_uid = ali_uid
         self.code = code
         self.query_draft = query_draft
 
     def validate(self):
         pass
 
@@ -3091,41 +4167,48 @@
         return self
 
 
 class DescribeProductResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeProductResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -3419,41 +4502,48 @@
         return self
 
 
 class DescribeProductsResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeProductsResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -3641,41 +4731,48 @@
         return self
 
 
 class DescribeProjectAttachmentsResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeProjectAttachmentsResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -3869,41 +4966,48 @@
         return self
 
 
 class DescribeProjectInfoResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeProjectInfoResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -4043,41 +5147,48 @@
         return self
 
 
 class DescribeProjectMessagesResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeProjectMessagesResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -4271,41 +5382,48 @@
         return self
 
 
 class DescribeProjectNodesResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeProjectNodesResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -4433,41 +5551,48 @@
         return self
 
 
 class DescribeProjectOperateLogsResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeProjectOperateLogsResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -4554,41 +5679,48 @@
         return self
 
 
 class FinishCurrentProjectNodeResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: FinishCurrentProjectNodeResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -4669,41 +5801,48 @@
         return self
 
 
 class PauseProjectResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: PauseProjectResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -4766,41 +5905,48 @@
         return self
 
 
 class PushMeteringDataResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: PushMeteringDataResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -4881,41 +6027,48 @@
         return self
 
 
 class ResumeProjectResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: ResumeProjectResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -4996,40 +6149,47 @@
         return self
 
 
 class RollbackCurrentProjectNodeResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: RollbackCurrentProjectNodeResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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

### Comparing `alibabacloud_market20151101-3.0.2/alibabacloud_market20151101.egg-info/PKG-INFO` & `alibabacloud_market20151101-3.0.3/alibabacloud_market20151101.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-market20151101
-Version: 3.0.2
+Version: 3.0.3
 Summary: Alibaba Cloud Market (20151101) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_market20151101-3.0.2/setup.py` & `alibabacloud_market20151101-3.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_market20151101.
 
-Created on 10/03/2022
+Created on 20/06/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_market20151101"
 NAME = "alibabacloud_market20151101" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Market (20151101) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.5, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.1, <1.0.0",
-    "alibabacloud_openapi_util>=0.1.6, <1.0.0",
+    "alibabacloud_tea_util>=0.3.8, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
+    "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

