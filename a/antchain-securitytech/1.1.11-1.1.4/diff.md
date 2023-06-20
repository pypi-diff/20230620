# Comparing `tmp/antchain_securitytech-1.1.11.tar.gz` & `tmp/antchain_securitytech-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_securitytech-1.1.11.tar", last modified: Tue Jun 20 03:00:04 2023, max compression
+gzip compressed data, was "dist/antchain_securitytech-1.1.4.tar", last modified: Wed May 24 02:53:36 2023, max compression
```

## Comparing `antchain_securitytech-1.1.11.tar` & `antchain_securitytech-1.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 03:00:04.000000 antchain_securitytech-1.1.11/
--rw-r--r--   0 root         (0) root         (0)      600 2023-06-20 03:00:03.000000 antchain_securitytech-1.1.11/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-20 03:00:03.000000 antchain_securitytech-1.1.11/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2217 2023-06-20 03:00:04.000000 antchain_securitytech-1.1.11/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      831 2023-06-20 03:00:03.000000 antchain_securitytech-1.1.11/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1017 2023-06-20 03:00:03.000000 antchain_securitytech-1.1.11/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 03:00:04.000000 antchain_securitytech-1.1.11/antchain_sdk_securitytech/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-20 03:00:03.000000 antchain_securitytech-1.1.11/antchain_sdk_securitytech/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44817 2023-06-20 03:00:03.000000 antchain_securitytech-1.1.11/antchain_sdk_securitytech/client.py
--rw-r--r--   0 root         (0) root         (0)    69392 2023-06-20 03:00:03.000000 antchain_securitytech-1.1.11/antchain_sdk_securitytech/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 03:00:04.000000 antchain_securitytech-1.1.11/antchain_securitytech.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2217 2023-06-20 03:00:04.000000 antchain_securitytech-1.1.11/antchain_securitytech.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      395 2023-06-20 03:00:04.000000 antchain_securitytech-1.1.11/antchain_securitytech.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 03:00:04.000000 antchain_securitytech-1.1.11/antchain_securitytech.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-06-20 03:00:04.000000 antchain_securitytech-1.1.11/antchain_securitytech.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-06-20 03:00:04.000000 antchain_securitytech-1.1.11/antchain_securitytech.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-20 03:00:04.000000 antchain_securitytech-1.1.11/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2533 2023-06-20 03:00:03.000000 antchain_securitytech-1.1.11/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 02:53:36.000000 antchain_securitytech-1.1.4/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-24 02:53:35.000000 antchain_securitytech-1.1.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-24 02:53:35.000000 antchain_securitytech-1.1.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2216 2023-05-24 02:53:36.000000 antchain_securitytech-1.1.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      831 2023-05-24 02:53:35.000000 antchain_securitytech-1.1.4/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-05-24 02:53:35.000000 antchain_securitytech-1.1.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 02:53:36.000000 antchain_securitytech-1.1.4/antchain_sdk_securitytech/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-24 02:53:35.000000 antchain_securitytech-1.1.4/antchain_sdk_securitytech/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26551 2023-05-24 02:53:35.000000 antchain_securitytech-1.1.4/antchain_sdk_securitytech/client.py
+-rw-r--r--   0 root         (0) root         (0)    44321 2023-05-24 02:53:35.000000 antchain_securitytech-1.1.4/antchain_sdk_securitytech/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 02:53:36.000000 antchain_securitytech-1.1.4/antchain_securitytech.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2216 2023-05-24 02:53:36.000000 antchain_securitytech-1.1.4/antchain_securitytech.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      395 2023-05-24 02:53:36.000000 antchain_securitytech-1.1.4/antchain_securitytech.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 02:53:36.000000 antchain_securitytech-1.1.4/antchain_securitytech.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-05-24 02:53:36.000000 antchain_securitytech-1.1.4/antchain_securitytech.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-05-24 02:53:36.000000 antchain_securitytech-1.1.4/antchain_securitytech.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-24 02:53:36.000000 antchain_securitytech-1.1.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2533 2023-05-24 02:53:35.000000 antchain_securitytech-1.1.4/setup.py
```

### Comparing `antchain_securitytech-1.1.11/LICENSE` & `antchain_securitytech-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_securitytech-1.1.11/PKG-INFO` & `antchain_securitytech-1.1.4/antchain_securitytech.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: antchain_securitytech
-Version: 1.1.11
+Name: antchain-securitytech
+Version: 1.1.4
 Summary: Ant Chain SECURITYTECH SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_securitytech-1.1.11/README-CN.md` & `antchain_securitytech-1.1.4/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_securitytech-1.1.11/README.md` & `antchain_securitytech-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `antchain_securitytech-1.1.11/antchain_sdk_securitytech/client.py` & `antchain_securitytech-1.1.4/antchain_sdk_securitytech/client.py`

 * *Files 23% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.1.11',
+                    'sdk_version': '1.1.4',
                     '_prod_code': 'SECURITYTECH',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.1.11',
+                    'sdk_version': '1.1.4',
                     '_prod_code': 'SECURITYTECH',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -387,350 +387,14 @@
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             securitytech_models.ExecEkytInsureResponse(),
             await self.do_request_async('1.0', 'antsecuritytech.gateway.ekyt.insure.exec', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
-    def init_iifaa_device(
-        self,
-        request: securitytech_models.InitIifaaDeviceRequest,
-    ) -> securitytech_models.InitIifaaDeviceResponse:
-        """
-        Description: 设备激活
-        Summary: 可信设备认证设备初始化，设备激活
-        """
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return self.init_iifaa_device_ex(request, headers, runtime)
-
-    async def init_iifaa_device_async(
-        self,
-        request: securitytech_models.InitIifaaDeviceRequest,
-    ) -> securitytech_models.InitIifaaDeviceResponse:
-        """
-        Description: 设备激活
-        Summary: 可信设备认证设备初始化，设备激活
-        """
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return await self.init_iifaa_device_ex_async(request, headers, runtime)
-
-    def init_iifaa_device_ex(
-        self,
-        request: securitytech_models.InitIifaaDeviceRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> securitytech_models.InitIifaaDeviceResponse:
-        """
-        Description: 设备激活
-        Summary: 可信设备认证设备初始化，设备激活
-        """
-        UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            securitytech_models.InitIifaaDeviceResponse(),
-            self.do_request('1.0', 'antsecuritytech.gateway.iifaa.device.init', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
-        )
-
-    async def init_iifaa_device_ex_async(
-        self,
-        request: securitytech_models.InitIifaaDeviceRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> securitytech_models.InitIifaaDeviceResponse:
-        """
-        Description: 设备激活
-        Summary: 可信设备认证设备初始化，设备激活
-        """
-        UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            securitytech_models.InitIifaaDeviceResponse(),
-            await self.do_request_async('1.0', 'antsecuritytech.gateway.iifaa.device.init', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
-        )
-
-    def recognize_iifaa_device(
-        self,
-        request: securitytech_models.RecognizeIifaaDeviceRequest,
-    ) -> securitytech_models.RecognizeIifaaDeviceResponse:
-        """
-        Description: 可信设备认证风险咨询，获取预认证数据
-        Summary: 可信设备认证风险咨询，获取预认证数据
-        """
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return self.recognize_iifaa_device_ex(request, headers, runtime)
-
-    async def recognize_iifaa_device_async(
-        self,
-        request: securitytech_models.RecognizeIifaaDeviceRequest,
-    ) -> securitytech_models.RecognizeIifaaDeviceResponse:
-        """
-        Description: 可信设备认证风险咨询，获取预认证数据
-        Summary: 可信设备认证风险咨询，获取预认证数据
-        """
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return await self.recognize_iifaa_device_ex_async(request, headers, runtime)
-
-    def recognize_iifaa_device_ex(
-        self,
-        request: securitytech_models.RecognizeIifaaDeviceRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> securitytech_models.RecognizeIifaaDeviceResponse:
-        """
-        Description: 可信设备认证风险咨询，获取预认证数据
-        Summary: 可信设备认证风险咨询，获取预认证数据
-        """
-        UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            securitytech_models.RecognizeIifaaDeviceResponse(),
-            self.do_request('1.0', 'antsecuritytech.gateway.iifaa.device.recognize', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
-        )
-
-    async def recognize_iifaa_device_ex_async(
-        self,
-        request: securitytech_models.RecognizeIifaaDeviceRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> securitytech_models.RecognizeIifaaDeviceResponse:
-        """
-        Description: 可信设备认证风险咨询，获取预认证数据
-        Summary: 可信设备认证风险咨询，获取预认证数据
-        """
-        UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            securitytech_models.RecognizeIifaaDeviceResponse(),
-            await self.do_request_async('1.0', 'antsecuritytech.gateway.iifaa.device.recognize', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
-        )
-
-    def verify_iifaa_device(
-        self,
-        request: securitytech_models.VerifyIifaaDeviceRequest,
-    ) -> securitytech_models.VerifyIifaaDeviceResponse:
-        """
-        Description: 可信设备认证，设备验证
-        Summary: 可信设备认证，设备验证
-        """
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return self.verify_iifaa_device_ex(request, headers, runtime)
-
-    async def verify_iifaa_device_async(
-        self,
-        request: securitytech_models.VerifyIifaaDeviceRequest,
-    ) -> securitytech_models.VerifyIifaaDeviceResponse:
-        """
-        Description: 可信设备认证，设备验证
-        Summary: 可信设备认证，设备验证
-        """
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return await self.verify_iifaa_device_ex_async(request, headers, runtime)
-
-    def verify_iifaa_device_ex(
-        self,
-        request: securitytech_models.VerifyIifaaDeviceRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> securitytech_models.VerifyIifaaDeviceResponse:
-        """
-        Description: 可信设备认证，设备验证
-        Summary: 可信设备认证，设备验证
-        """
-        UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            securitytech_models.VerifyIifaaDeviceResponse(),
-            self.do_request('1.0', 'antsecuritytech.gateway.iifaa.device.verify', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
-        )
-
-    async def verify_iifaa_device_ex_async(
-        self,
-        request: securitytech_models.VerifyIifaaDeviceRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> securitytech_models.VerifyIifaaDeviceResponse:
-        """
-        Description: 可信设备认证，设备验证
-        Summary: 可信设备认证，设备验证
-        """
-        UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            securitytech_models.VerifyIifaaDeviceResponse(),
-            await self.do_request_async('1.0', 'antsecuritytech.gateway.iifaa.device.verify', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
-        )
-
-    def register_iifaa_corp(
-        self,
-        request: securitytech_models.RegisterIifaaCorpRequest,
-    ) -> securitytech_models.RegisterIifaaCorpResponse:
-        """
-        Description: 可信设备认证，产商注册
-        Summary: 可信设备认证，产商注册
-        """
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return self.register_iifaa_corp_ex(request, headers, runtime)
-
-    async def register_iifaa_corp_async(
-        self,
-        request: securitytech_models.RegisterIifaaCorpRequest,
-    ) -> securitytech_models.RegisterIifaaCorpResponse:
-        """
-        Description: 可信设备认证，产商注册
-        Summary: 可信设备认证，产商注册
-        """
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return await self.register_iifaa_corp_ex_async(request, headers, runtime)
-
-    def register_iifaa_corp_ex(
-        self,
-        request: securitytech_models.RegisterIifaaCorpRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> securitytech_models.RegisterIifaaCorpResponse:
-        """
-        Description: 可信设备认证，产商注册
-        Summary: 可信设备认证，产商注册
-        """
-        UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            securitytech_models.RegisterIifaaCorpResponse(),
-            self.do_request('1.0', 'antsecuritytech.gateway.iifaa.corp.register', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
-        )
-
-    async def register_iifaa_corp_ex_async(
-        self,
-        request: securitytech_models.RegisterIifaaCorpRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> securitytech_models.RegisterIifaaCorpResponse:
-        """
-        Description: 可信设备认证，产商注册
-        Summary: 可信设备认证，产商注册
-        """
-        UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            securitytech_models.RegisterIifaaCorpResponse(),
-            await self.do_request_async('1.0', 'antsecuritytech.gateway.iifaa.corp.register', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
-        )
-
-    def deprecate_iifaa_device(
-        self,
-        request: securitytech_models.DeprecateIifaaDeviceRequest,
-    ) -> securitytech_models.DeprecateIifaaDeviceResponse:
-        """
-        Description: 可信设备认证，擦除设备信息
-        Summary: 可信设备认证，擦除设备信息
-        """
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return self.deprecate_iifaa_device_ex(request, headers, runtime)
-
-    async def deprecate_iifaa_device_async(
-        self,
-        request: securitytech_models.DeprecateIifaaDeviceRequest,
-    ) -> securitytech_models.DeprecateIifaaDeviceResponse:
-        """
-        Description: 可信设备认证，擦除设备信息
-        Summary: 可信设备认证，擦除设备信息
-        """
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return await self.deprecate_iifaa_device_ex_async(request, headers, runtime)
-
-    def deprecate_iifaa_device_ex(
-        self,
-        request: securitytech_models.DeprecateIifaaDeviceRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> securitytech_models.DeprecateIifaaDeviceResponse:
-        """
-        Description: 可信设备认证，擦除设备信息
-        Summary: 可信设备认证，擦除设备信息
-        """
-        UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            securitytech_models.DeprecateIifaaDeviceResponse(),
-            self.do_request('1.0', 'antsecuritytech.gateway.iifaa.device.deprecate', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
-        )
-
-    async def deprecate_iifaa_device_ex_async(
-        self,
-        request: securitytech_models.DeprecateIifaaDeviceRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> securitytech_models.DeprecateIifaaDeviceResponse:
-        """
-        Description: 可信设备认证，擦除设备信息
-        Summary: 可信设备认证，擦除设备信息
-        """
-        UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            securitytech_models.DeprecateIifaaDeviceResponse(),
-            await self.do_request_async('1.0', 'antsecuritytech.gateway.iifaa.device.deprecate', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
-        )
-
-    def exec_iifaa_insure(
-        self,
-        request: securitytech_models.ExecIifaaInsureRequest,
-    ) -> securitytech_models.ExecIifaaInsureResponse:
-        """
-        Description: 租凭住房保险产品，接口开放给租房平台
-        Summary: 租凭住房保险产品，接口开放给租房平台
-        """
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return self.exec_iifaa_insure_ex(request, headers, runtime)
-
-    async def exec_iifaa_insure_async(
-        self,
-        request: securitytech_models.ExecIifaaInsureRequest,
-    ) -> securitytech_models.ExecIifaaInsureResponse:
-        """
-        Description: 租凭住房保险产品，接口开放给租房平台
-        Summary: 租凭住房保险产品，接口开放给租房平台
-        """
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return await self.exec_iifaa_insure_ex_async(request, headers, runtime)
-
-    def exec_iifaa_insure_ex(
-        self,
-        request: securitytech_models.ExecIifaaInsureRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> securitytech_models.ExecIifaaInsureResponse:
-        """
-        Description: 租凭住房保险产品，接口开放给租房平台
-        Summary: 租凭住房保险产品，接口开放给租房平台
-        """
-        UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            securitytech_models.ExecIifaaInsureResponse(),
-            self.do_request('1.0', 'antsecuritytech.gateway.iifaa.insure.exec', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
-        )
-
-    async def exec_iifaa_insure_ex_async(
-        self,
-        request: securitytech_models.ExecIifaaInsureRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> securitytech_models.ExecIifaaInsureResponse:
-        """
-        Description: 租凭住房保险产品，接口开放给租房平台
-        Summary: 租凭住房保险产品，接口开放给租房平台
-        """
-        UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            securitytech_models.ExecIifaaInsureResponse(),
-            await self.do_request_async('1.0', 'antsecuritytech.gateway.iifaa.insure.exec', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
-        )
-
     def create_bssecpic(
         self,
         request: securitytech_models.CreateBssecpicRequest,
     ) -> securitytech_models.CreateBssecpicResponse:
         """
         Description: 蓝盾安全图片生成
         Summary: 蓝盾安全图片生成
@@ -946,119 +610,7 @@
         Summary: 人脸盾Web查询
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             securitytech_models.QueryFaceshieldWebResponse(),
             await self.do_request_async('1.0', 'antsecuritytech.gateway.faceshield.web.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
-
-    def run_xhunter_spi(
-        self,
-        request: securitytech_models.RunXhunterSpiRequest,
-    ) -> securitytech_models.RunXhunterSpiResponse:
-        """
-        Description: 巡检商业化
-        Summary: 巡检商业化
-        """
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return self.run_xhunter_spi_ex(request, headers, runtime)
-
-    async def run_xhunter_spi_async(
-        self,
-        request: securitytech_models.RunXhunterSpiRequest,
-    ) -> securitytech_models.RunXhunterSpiResponse:
-        """
-        Description: 巡检商业化
-        Summary: 巡检商业化
-        """
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return await self.run_xhunter_spi_ex_async(request, headers, runtime)
-
-    def run_xhunter_spi_ex(
-        self,
-        request: securitytech_models.RunXhunterSpiRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> securitytech_models.RunXhunterSpiResponse:
-        """
-        Description: 巡检商业化
-        Summary: 巡检商业化
-        """
-        UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            securitytech_models.RunXhunterSpiResponse(),
-            self.do_request('1.0', 'antsecuritytech.gateway.xhunter.spi.run', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
-        )
-
-    async def run_xhunter_spi_ex_async(
-        self,
-        request: securitytech_models.RunXhunterSpiRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> securitytech_models.RunXhunterSpiResponse:
-        """
-        Description: 巡检商业化
-        Summary: 巡检商业化
-        """
-        UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            securitytech_models.RunXhunterSpiResponse(),
-            await self.do_request_async('1.0', 'antsecuritytech.gateway.xhunter.spi.run', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
-        )
-
-    def query_cct_picture(
-        self,
-        request: securitytech_models.QueryCctPictureRequest,
-    ) -> securitytech_models.QueryCctPictureResponse:
-        """
-        Description: 内容安全图片同步检测
-        Summary: 内容安全图片同步检测
-        """
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return self.query_cct_picture_ex(request, headers, runtime)
-
-    async def query_cct_picture_async(
-        self,
-        request: securitytech_models.QueryCctPictureRequest,
-    ) -> securitytech_models.QueryCctPictureResponse:
-        """
-        Description: 内容安全图片同步检测
-        Summary: 内容安全图片同步检测
-        """
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return await self.query_cct_picture_ex_async(request, headers, runtime)
-
-    def query_cct_picture_ex(
-        self,
-        request: securitytech_models.QueryCctPictureRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> securitytech_models.QueryCctPictureResponse:
-        """
-        Description: 内容安全图片同步检测
-        Summary: 内容安全图片同步检测
-        """
-        UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            securitytech_models.QueryCctPictureResponse(),
-            self.do_request('1.0', 'antsecuritytech.gateway.cct.picture.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
-        )
-
-    async def query_cct_picture_ex_async(
-        self,
-        request: securitytech_models.QueryCctPictureRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> securitytech_models.QueryCctPictureResponse:
-        """
-        Description: 内容安全图片同步检测
-        Summary: 内容安全图片同步检测
-        """
-        UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            securitytech_models.QueryCctPictureResponse(),
-            await self.do_request_async('1.0', 'antsecuritytech.gateway.cct.picture.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
-        )
```

### Comparing `antchain_securitytech-1.1.11/antchain_securitytech.egg-info/PKG-INFO` & `antchain_securitytech-1.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: antchain-securitytech
-Version: 1.1.11
+Name: antchain_securitytech
+Version: 1.1.4
 Summary: Ant Chain SECURITYTECH SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_securitytech-1.1.11/setup.py` & `antchain_securitytech-1.1.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_securitytech.
 
-Created on 20/06/2023
+Created on 24/05/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_securitytech"
 NAME = "antchain_securitytech" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain SECURITYTECH SDK Library for Python"
```

