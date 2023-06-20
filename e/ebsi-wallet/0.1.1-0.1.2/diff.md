# Comparing `tmp/ebsi-wallet-0.1.1.tar.gz` & `tmp/ebsi_wallet-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebsi-wallet-0.1.1.tar", max compression
+gzip compressed data, was "ebsi_wallet-0.1.2.tar", max compression
```

## Comparing `ebsi-wallet-0.1.1.tar` & `ebsi_wallet-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0    11368 2022-05-20 09:58:08.963766 ebsi-wallet-0.1.1/LICENSE
--rw-r--r--   0        0        0        0 2022-10-21 11:30:14.293857 ebsi-wallet-0.1.1/ebsi_wallet/__init__.py
--rw-r--r--   0        0        0     4192 2022-10-21 11:29:21.455961 ebsi-wallet-0.1.1/ebsi_wallet/did_jwt/__init__.py
--rw-r--r--   0        0        0     2515 2022-10-21 11:29:23.423242 ebsi-wallet-0.1.1/ebsi_wallet/did_jwt/signer_algorithm.py
--rw-r--r--   0        0        0      805 2022-05-09 15:27:47.484439 ebsi-wallet-0.1.1/ebsi_wallet/did_jwt/util/__init__.py
--rw-r--r--   0        0        0    18274 2022-10-21 11:29:13.620414 ebsi-wallet-0.1.1/ebsi_wallet/did_jwt/util/json_canonicalize/Canonicalize.py
--rw-r--r--   0        0        0     3954 2022-10-21 11:29:18.433253 ebsi-wallet-0.1.1/ebsi_wallet/did_jwt/util/json_canonicalize/NumberToJson.py
--rw-r--r--   0        0        0        0 2022-10-21 11:29:19.937089 ebsi-wallet-0.1.1/ebsi_wallet/did_jwt/util/json_canonicalize/__init__.py
--rw-r--r--   0        0        0     1346 2022-10-21 11:29:26.713261 ebsi-wallet-0.1.1/ebsi_wallet/ebsi_client/__init__.py
--rw-r--r--   0        0        0     1118 2022-10-21 11:29:28.749108 ebsi-wallet-0.1.1/ebsi_wallet/ebsi_did/__init__.py
--rw-r--r--   0        0        0      319 2022-10-21 11:29:41.110568 ebsi-wallet-0.1.1/ebsi_wallet/ebsi_did_resolver/__init__.py
--rw-r--r--   0        0        0      280 2022-10-21 11:29:33.654662 ebsi-wallet-0.1.1/ebsi_wallet/ebsi_did_resolver/constants/__init__.py
--rw-r--r--   0        0        0     1155 2022-10-21 11:29:36.271024 ebsi-wallet-0.1.1/ebsi_wallet/ebsi_did_resolver/validators/__init__.py
--rw-r--r--   0        0        0     3709 2022-10-21 11:29:42.833033 ebsi-wallet-0.1.1/ebsi_wallet/ethereum/__init__.py
--rw-r--r--   0        0        0      436 2022-10-21 11:29:44.883572 ebsi-wallet-0.1.1/ebsi_wallet/ethereum/util.py
--rw-r--r--   0        0        0    25531 2022-10-21 11:30:16.359142 ebsi-wallet-0.1.1/ebsi_wallet/main.py
--rw-r--r--   0        0        0     2764 2022-10-21 11:29:47.934662 ebsi-wallet-0.1.1/ebsi_wallet/siop_auth/__init__.py
--rw-r--r--   0        0        0     2712 2022-10-21 11:29:49.736237 ebsi-wallet-0.1.1/ebsi_wallet/siop_auth/util.py
--rw-r--r--   0        0        0     4220 2022-10-21 11:29:54.539975 ebsi-wallet-0.1.1/ebsi_wallet/util/__init__.py
--rw-r--r--   0        0        0     3363 2022-10-21 11:29:57.336395 ebsi-wallet-0.1.1/ebsi_wallet/util/verifiable_presentation.py
--rw-r--r--   0        0        0     2499 2022-10-21 11:30:00.233535 ebsi-wallet-0.1.1/ebsi_wallet/validators/__init__.py
--rw-r--r--   0        0        0        0 2022-10-21 11:30:05.329867 ebsi-wallet-0.1.1/ebsi_wallet/verifiable_credential/__init__.py
--rw-r--r--   0        0        0      148 2022-10-21 11:30:03.423468 ebsi-wallet-0.1.1/ebsi_wallet/verifiable_credential/validators/__init__.py
--rw-r--r--   0        0        0      536 2022-10-21 11:30:12.254736 ebsi-wallet-0.1.1/ebsi_wallet/verifiable_presentation/__init__.py
--rw-r--r--   0        0        0     1431 2022-10-21 11:30:09.661285 ebsi-wallet-0.1.1/ebsi_wallet/verifiable_presentation/v2/__init__.py
--rw-r--r--   0        0        0      594 2022-10-21 11:34:05.922428 ebsi-wallet-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1427 2022-10-21 11:34:14.337374 ebsi-wallet-0.1.1/setup.py
--rw-r--r--   0        0        0      881 2022-10-21 11:34:14.337531 ebsi-wallet-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11368 2023-01-10 08:28:57.766492 ebsi_wallet-0.1.2/LICENSE
+-rw-r--r--   0        0        0        0 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.2/ebsi_wallet/__init__.py
+-rw-r--r--   0        0        0     4192 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.2/ebsi_wallet/did_jwt/__init__.py
+-rw-r--r--   0        0        0     2515 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.2/ebsi_wallet/did_jwt/signer_algorithm.py
+-rw-r--r--   0        0        0      805 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.2/ebsi_wallet/did_jwt/util/__init__.py
+-rw-r--r--   0        0        0    18274 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.2/ebsi_wallet/did_jwt/util/json_canonicalize/Canonicalize.py
+-rw-r--r--   0        0        0     3954 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.2/ebsi_wallet/did_jwt/util/json_canonicalize/NumberToJson.py
+-rw-r--r--   0        0        0        0 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.2/ebsi_wallet/did_jwt/util/json_canonicalize/__init__.py
+-rw-r--r--   0        0        0     5363 2023-06-20 16:50:47.088113 ebsi_wallet-0.1.2/ebsi_wallet/did_key/__init__.py
+-rw-r--r--   0        0        0     1346 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.2/ebsi_wallet/ebsi_client/__init__.py
+-rw-r--r--   0        0        0     1118 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.2/ebsi_wallet/ebsi_did/__init__.py
+-rw-r--r--   0        0        0      319 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.2/ebsi_wallet/ebsi_did_resolver/__init__.py
+-rw-r--r--   0        0        0      280 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.2/ebsi_wallet/ebsi_did_resolver/constants/__init__.py
+-rw-r--r--   0        0        0     1155 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.2/ebsi_wallet/ebsi_did_resolver/validators/__init__.py
+-rw-r--r--   0        0        0     3709 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.2/ebsi_wallet/ethereum/__init__.py
+-rw-r--r--   0        0        0      436 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.2/ebsi_wallet/ethereum/util.py
+-rw-r--r--   0        0        0    27001 2023-05-01 07:34:47.063782 ebsi_wallet-0.1.2/ebsi_wallet/main.py
+-rw-r--r--   0        0        0     2764 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.2/ebsi_wallet/siop_auth/__init__.py
+-rw-r--r--   0        0        0    15771 2023-06-20 09:52:09.193345 ebsi_wallet-0.1.2/ebsi_wallet/siop_auth/util.py
+-rw-r--r--   0        0        0     4861 2023-06-20 17:08:15.296537 ebsi_wallet-0.1.2/ebsi_wallet/util/__init__.py
+-rw-r--r--   0        0        0     3363 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.2/ebsi_wallet/util/verifiable_presentation.py
+-rw-r--r--   0        0        0     2499 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.2/ebsi_wallet/validators/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.2/ebsi_wallet/verifiable_credential/__init__.py
+-rw-r--r--   0        0        0      148 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.2/ebsi_wallet/verifiable_credential/validators/__init__.py
+-rw-r--r--   0        0        0      536 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.2/ebsi_wallet/verifiable_presentation/__init__.py
+-rw-r--r--   0        0        0     1431 2023-01-10 08:28:57.770491 ebsi_wallet-0.1.2/ebsi_wallet/verifiable_presentation/v2/__init__.py
+-rw-r--r--   0        0        0      645 2023-06-20 17:24:29.488089 ebsi_wallet-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1525 1970-01-01 00:00:00.000000 ebsi_wallet-0.1.2/setup.py
+-rw-r--r--   0        0        0      925 1970-01-01 00:00:00.000000 ebsi_wallet-0.1.2/PKG-INFO
```

### Comparing `ebsi-wallet-0.1.1/LICENSE` & `ebsi_wallet-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ebsi-wallet-0.1.1/ebsi_wallet/did_jwt/__init__.py` & `ebsi_wallet-0.1.2/ebsi_wallet/did_jwt/__init__.py`

 * *Files identical despite different names*

### Comparing `ebsi-wallet-0.1.1/ebsi_wallet/did_jwt/signer_algorithm.py` & `ebsi_wallet-0.1.2/ebsi_wallet/did_jwt/signer_algorithm.py`

 * *Files identical despite different names*

### Comparing `ebsi-wallet-0.1.1/ebsi_wallet/did_jwt/util/__init__.py` & `ebsi_wallet-0.1.2/ebsi_wallet/did_jwt/util/__init__.py`

 * *Files identical despite different names*

### Comparing `ebsi-wallet-0.1.1/ebsi_wallet/did_jwt/util/json_canonicalize/Canonicalize.py` & `ebsi_wallet-0.1.2/ebsi_wallet/did_jwt/util/json_canonicalize/Canonicalize.py`

 * *Files identical despite different names*

### Comparing `ebsi-wallet-0.1.1/ebsi_wallet/did_jwt/util/json_canonicalize/NumberToJson.py` & `ebsi_wallet-0.1.2/ebsi_wallet/did_jwt/util/json_canonicalize/NumberToJson.py`

 * *Files identical despite different names*

### Comparing `ebsi-wallet-0.1.1/ebsi_wallet/ebsi_client/__init__.py` & `ebsi_wallet-0.1.2/ebsi_wallet/ebsi_client/__init__.py`

 * *Files identical despite different names*

### Comparing `ebsi-wallet-0.1.1/ebsi_wallet/ebsi_did/__init__.py` & `ebsi_wallet-0.1.2/ebsi_wallet/ebsi_did/__init__.py`

 * *Files identical despite different names*

### Comparing `ebsi-wallet-0.1.1/ebsi_wallet/ebsi_did_resolver/validators/__init__.py` & `ebsi_wallet-0.1.2/ebsi_wallet/ebsi_did_resolver/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `ebsi-wallet-0.1.1/ebsi_wallet/ethereum/__init__.py` & `ebsi_wallet-0.1.2/ebsi_wallet/ethereum/__init__.py`

 * *Files identical despite different names*

### Comparing `ebsi-wallet-0.1.1/ebsi_wallet/main.py` & `ebsi_wallet-0.1.2/ebsi_wallet/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,49 +21,55 @@
 )
 from ebsi_wallet.util.verifiable_presentation import create_vp_jwt
 
 console = Console()
 
 app_config = {
     "conformance": {
-        "api": "https://api.conformance.intebsi.xyz",
+        "api": "https://api-conformance.ebsi.eu",
         "endpoints": {
             "issuer-initiate-v1": "/conformance/v1/issuer-mock/initiate",
             "issuer-authorize-v1": "/conformance/v1/issuer-mock/authorize",
             "issuer-initiate-v2": "/conformance/v2/issuer-mock/initiate",
             "issuer-authorize-v2": "/conformance/v2/issuer-mock/authorize",
+            "issuer-initiate-v3": "/conformance/v3/issuer-mock/initiate",
+            "issuer-authorize-v3": "/conformance/v3/issuer-mock/authorize",
             "issuer-token-v1": "/conformance/v1/issuer-mock/token",
             "issuer-token-v2": "/conformance/v2/issuer-mock/token",
+            "issuer-token-v3": "/conformance/v3/issuer-mock/token",
             "issuer-credential-v1": "/conformance/v1/issuer-mock/credential",
             "issuer-credential-v2": "/conformance/v2/issuer-mock/credential",
+            "issuer-credential-v3": "/conformance/v3/issuer-mock/credential",
             "verifier-auth-request-v1": "/conformance/v1/verifier-mock/authentication-requests",
             "verifier-auth-request-v2": "/conformance/v2/verifier-mock/authentication-requests",
+            "verifier-auth-request-v3": "/conformance/v3/verifier-mock/authentication-requests",
             "verifier-auth-response-v1": "/conformance/v1/verifier-mock/authentication-responses",
             "verifier-auth-response-v2": "/conformance/v2/verifier-mock/authentication-responses",
+            "verifier-auth-response-v3": "/conformance/v3/verifier-mock/authentication-responses",
         },
         "onboarding": {
-            "api": "https://api.conformance.intebsi.xyz",
+            "api": "https://api-conformance.ebsi.eu",
             "endpoints": {
                 "post": {
                     "authentication-requests": "/users-onboarding/v1/authentication-requests",
                     "sessions": "/users-onboarding/v1/sessions",
                     "authentication-responses": "/users-onboarding/v1/authentication-responses",
                 }
             },
         },
         "authorisation": {
-            "api": "https://api.conformance.intebsi.xyz",
+            "api": "https://api-conformance.ebsi.eu",
             "endpoints": {
                 "post": {
                     "siop-authentication-requests": "/authorisation/v1/authentication-requests"
                 }
             },
         },
         "did": {
-            "api": "https://api.conformance.intebsi.xyz",
+            "api": "https://api-conformance.ebsi.eu",
             "endpoints": {"post": {"identifiers": "/did-registry/v2/identifiers"}},
         },
     }
 }
 
 
 async def authorisation(method, headers, options):
@@ -129,18 +135,41 @@
 
     assert method_fn is not None, "Method not found"
 
     return await method_fn()
 
 
 async def conformance(method, headers=None, options=None):
+
+    async def issuer_initiate_v3():
+        credential_type = options.get("credential_type", "diploma")
+        flow_type = options.get("flow_type", "cross-device")
+        conformance = options.get("conformance")
+
+        url = (
+            app_config["conformance"]["api"]
+            + app_config["conformance"]["endpoints"]["issuer-initiate-v3"]
+            + f"?credential_type={credential_type}"
+            + f"&flow_type={flow_type}"
+            + f"&conformance={conformance}"
+        )
+        response = await http_call_text(url, "GET", data=None, headers=headers)
+        return response
+
     async def issuer_initiate():
+        credential_type = options.get("credential_type", "diploma")
+        flow_type = options.get("flow_type", "cross-device")
+        conformance = options.get("conformance")
+
         url = (
             app_config["conformance"]["api"]
             + app_config["conformance"]["endpoints"]["issuer-initiate-v2"]
+            + f"?credential_type={credential_type}"
+            + f"&flow_type={flow_type}"
+            + f"&conformance={conformance}"
         )
         response = await http_call_text(url, "GET", data=None, headers=headers)
         return response
 
     async def issuer_authorize():
         credential_type = options.get("credential_type")
 
@@ -288,15 +317,17 @@
         )
 
         if client.did_version == "v1":
 
             if headers:
                 headers["Content-Type"] = "application/json"
 
-            credential_url = "https://api.conformance.intebsi.xyz/conformance/v1/issuer-mock/credential"
+            credential_url = (
+                "https://api-conformance.ebsi.eu/conformance/v1/issuer-mock/credential"
+            )
 
             payload = {
                 "type": "https://api.test.intebsi.xyz/trusted-schemas-registry/v1/schemas/0x1ee207961aba4a8ba018bacf3aaa338df9884d52e993468297e775a585abe4d8",
                 "format": "jwt_vc",
                 "did": client.ebsi_did.did,
                 "proof": {
                     "type": "JWS",
@@ -486,14 +517,15 @@
                 authentication_response_url, "POST", data=payload_str, headers=headers
             )
 
             return vp_status
 
     switcher = {
         "issuerInitiate": issuer_initiate,
+        "issuerInitiateV3": issuer_initiate_v3,
         "issuerAuthorize": issuer_authorize,
         "issuerToken": issuer_token,
         "issuerCredential": issuer_credential,
         "verifierAuthRequest": verifier_auth_request,
         "verifierAuthResponse": verifier_auth_response,
     }
```

### Comparing `ebsi-wallet-0.1.1/ebsi_wallet/siop_auth/__init__.py` & `ebsi_wallet-0.1.2/ebsi_wallet/siop_auth/__init__.py`

 * *Files identical despite different names*

### Comparing `ebsi-wallet-0.1.1/ebsi_wallet/util/__init__.py` & `ebsi_wallet-0.1.2/ebsi_wallet/util/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import asyncio
 import base64
 import datetime
+import os
+import typing
+import json
 from urllib.parse import parse_qs, urlparse
 
 import aiohttp
 
 
 def pad_base64(data):
     """
@@ -150,7 +153,22 @@
     """
 
     parsed_url = urlparse(url)
 
     query_string = parsed_url.query
 
     return parse_qs(query_string)
+
+def generate_random_salt() -> str:
+    # Generate a random salt with 16 bytes (128 bits)
+    salt = os.urandom(16)
+
+    # Convert the salt to hexadecimal representation
+    salt_hex = salt.hex()
+
+    return salt_hex
+
+def generate_disclosure_content_and_base64(claim_key: str, claims: dict) -> typing.Tuple[str, str]:
+    claim_salt = generate_random_salt()
+    claim_disclosure = [claim_salt, claim_key, claims[claim_key]]
+    claim_disclosure_base64 = base64.urlsafe_b64encode(json.dumps(claim_disclosure).encode('utf-8')).decode('utf-8').rstrip("=")
+    return claim_disclosure, claim_disclosure_base64
```

### Comparing `ebsi-wallet-0.1.1/ebsi_wallet/util/verifiable_presentation.py` & `ebsi_wallet-0.1.2/ebsi_wallet/util/verifiable_presentation.py`

 * *Files identical despite different names*

### Comparing `ebsi-wallet-0.1.1/ebsi_wallet/validators/__init__.py` & `ebsi_wallet-0.1.2/ebsi_wallet/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `ebsi-wallet-0.1.1/ebsi_wallet/verifiable_presentation/__init__.py` & `ebsi_wallet-0.1.2/ebsi_wallet/verifiable_presentation/__init__.py`

 * *Files identical despite different names*

### Comparing `ebsi-wallet-0.1.1/ebsi_wallet/verifiable_presentation/v2/__init__.py` & `ebsi_wallet-0.1.2/ebsi_wallet/verifiable_presentation/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `ebsi-wallet-0.1.1/pyproject.toml` & `ebsi_wallet-0.1.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 [tool.poetry]
 name = "ebsi-wallet"
-version = "0.1.1"
+version = "0.1.2"
 description = "EBSI Python SDK"
 authors = ["George J Padayatti <george.padayatti@igrant.io>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.11"
+python = ">=3.8.1,<3.11"
 jwcrypto = "^1.3.1"
 py-multibase = "^1.0.3"
 coincurve = "^17.0.0"
 aiohttp = "^3.8.1"
 sslcrypto = "^5.3"
 rich = "^12.5.1"
 jsonschema = "^4.14.0"
 base58 = "1.0.3"
 eth-keys = "^0.4.0"
 PyJWT = "^2.4.0"
 pysha3 = "^1.0.2"
+multiformats = "^0.2.1"
+cryptography = "^41.0.1"
 
 [tool.poetry.dev-dependencies]
 jupyter = "^1.0.0"
 notebook = "^6.4.12"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `ebsi-wallet-0.1.1/setup.py` & `ebsi_wallet-0.1.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from setuptools import setup
 
 packages = \
 ['ebsi_wallet',
  'ebsi_wallet.did_jwt',
  'ebsi_wallet.did_jwt.util',
  'ebsi_wallet.did_jwt.util.json_canonicalize',
+ 'ebsi_wallet.did_key',
  'ebsi_wallet.ebsi_client',
  'ebsi_wallet.ebsi_did',
  'ebsi_wallet.ebsi_did_resolver',
  'ebsi_wallet.ebsi_did_resolver.constants',
  'ebsi_wallet.ebsi_did_resolver.validators',
  'ebsi_wallet.ethereum',
  'ebsi_wallet.siop_auth',
@@ -24,33 +25,35 @@
 {'': ['*']}
 
 install_requires = \
 ['PyJWT>=2.4.0,<3.0.0',
  'aiohttp>=3.8.1,<4.0.0',
  'base58==1.0.3',
  'coincurve>=17.0.0,<18.0.0',
+ 'cryptography>=41.0.1,<42.0.0',
  'eth-keys>=0.4.0,<0.5.0',
  'jsonschema>=4.14.0,<5.0.0',
  'jwcrypto>=1.3.1,<2.0.0',
+ 'multiformats>=0.2.1,<0.3.0',
  'py-multibase>=1.0.3,<2.0.0',
  'pysha3>=1.0.2,<2.0.0',
  'rich>=12.5.1,<13.0.0',
  'sslcrypto>=5.3,<6.0']
 
 setup_kwargs = {
     'name': 'ebsi-wallet',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'EBSI Python SDK',
-    'long_description': None,
+    'long_description': 'None',
     'author': 'George J Padayatti',
     'author_email': 'george.padayatti@igrant.io',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.8,<3.11',
+    'python_requires': '>=3.8.1,<3.11',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `ebsi-wallet-0.1.1/PKG-INFO` & `ebsi_wallet-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: ebsi-wallet
-Version: 0.1.1
+Version: 0.1.2
 Summary: EBSI Python SDK
 License: MIT
 Author: George J Padayatti
 Author-email: george.padayatti@igrant.io
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: PyJWT (>=2.4.0,<3.0.0)
 Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
 Requires-Dist: base58 (==1.0.3)
 Requires-Dist: coincurve (>=17.0.0,<18.0.0)
+Requires-Dist: cryptography (>=41.0.1,<42.0.0)
 Requires-Dist: eth-keys (>=0.4.0,<0.5.0)
 Requires-Dist: jsonschema (>=4.14.0,<5.0.0)
 Requires-Dist: jwcrypto (>=1.3.1,<2.0.0)
+Requires-Dist: multiformats (>=0.2.1,<0.3.0)
 Requires-Dist: py-multibase (>=1.0.3,<2.0.0)
 Requires-Dist: pysha3 (>=1.0.2,<2.0.0)
 Requires-Dist: rich (>=12.5.1,<13.0.0)
 Requires-Dist: sslcrypto (>=5.3,<6.0)
```

