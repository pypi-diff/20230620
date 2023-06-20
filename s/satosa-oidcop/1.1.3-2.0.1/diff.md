# Comparing `tmp/satosa_oidcop-1.1.3.tar.gz` & `tmp/satosa_oidcop-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satosa_oidcop-1.1.3.tar", last modified: Tue Jun 20 17:20:57 2023, max compression
+gzip compressed data, was "satosa_oidcop-2.0.1.tar", last modified: Tue Jun 20 17:24:47 2023, max compression
```

## Comparing `satosa_oidcop-1.1.3.tar` & `satosa_oidcop-2.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:20:57.316693 satosa_oidcop-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-20 17:20:24.000000 satosa_oidcop-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-06-20 17:20:57.316693 satosa_oidcop-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-06-20 17:20:24.000000 satosa_oidcop-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:20:57.316693 satosa_oidcop-1.1.3/satosa_oidcop/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 17:20:24.000000 satosa_oidcop-1.1.3/satosa_oidcop/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:20:57.316693 satosa_oidcop-1.1.3/satosa_oidcop/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 17:20:24.000000 satosa_oidcop-1.1.3/satosa_oidcop/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-20 17:20:24.000000 satosa_oidcop-1.1.3/satosa_oidcop/core/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-20 17:20:24.000000 satosa_oidcop-1.1.3/satosa_oidcop/core/claims.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-20 17:20:24.000000 satosa_oidcop-1.1.3/satosa_oidcop/core/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:20:57.316693 satosa_oidcop-1.1.3/satosa_oidcop/core/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 17:20:24.000000 satosa_oidcop-1.1.3/satosa_oidcop/core/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-20 17:20:24.000000 satosa_oidcop-1.1.3/satosa_oidcop/core/storage/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-06-20 17:20:24.000000 satosa_oidcop-1.1.3/satosa_oidcop/core/storage/mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-20 17:20:24.000000 satosa_oidcop-1.1.3/satosa_oidcop/core/user_authn.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-20 17:20:24.000000 satosa_oidcop-1.1.3/satosa_oidcop/core/user_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    29825 2023-06-20 17:20:24.000000 satosa_oidcop-1.1.3/satosa_oidcop/idpy_oidcop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:20:57.316693 satosa_oidcop-1.1.3/satosa_oidcop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-06-20 17:20:57.000000 satosa_oidcop-1.1.3/satosa_oidcop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-20 17:20:57.000000 satosa_oidcop-1.1.3/satosa_oidcop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 17:20:57.000000 satosa_oidcop-1.1.3/satosa_oidcop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-20 17:20:57.000000 satosa_oidcop-1.1.3/satosa_oidcop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-20 17:20:57.000000 satosa_oidcop-1.1.3/satosa_oidcop.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-20 17:20:57.316693 satosa_oidcop-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-20 17:20:24.000000 satosa_oidcop-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:24:47.537452 satosa_oidcop-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-20 17:24:12.000000 satosa_oidcop-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-06-20 17:24:47.537452 satosa_oidcop-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-06-20 17:24:12.000000 satosa_oidcop-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:24:47.537452 satosa_oidcop-2.0.1/satosa_oidcop/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-20 17:24:12.000000 satosa_oidcop-2.0.1/satosa_oidcop/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:24:47.537452 satosa_oidcop-2.0.1/satosa_oidcop/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 17:24:12.000000 satosa_oidcop-2.0.1/satosa_oidcop/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-20 17:24:12.000000 satosa_oidcop-2.0.1/satosa_oidcop/core/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-20 17:24:12.000000 satosa_oidcop-2.0.1/satosa_oidcop/core/claims.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-20 17:24:12.000000 satosa_oidcop-2.0.1/satosa_oidcop/core/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:24:47.537452 satosa_oidcop-2.0.1/satosa_oidcop/core/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 17:24:12.000000 satosa_oidcop-2.0.1/satosa_oidcop/core/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-20 17:24:12.000000 satosa_oidcop-2.0.1/satosa_oidcop/core/storage/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-06-20 17:24:12.000000 satosa_oidcop-2.0.1/satosa_oidcop/core/storage/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-20 17:24:12.000000 satosa_oidcop-2.0.1/satosa_oidcop/core/user_authn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-20 17:24:12.000000 satosa_oidcop-2.0.1/satosa_oidcop/core/user_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31922 2023-06-20 17:24:12.000000 satosa_oidcop-2.0.1/satosa_oidcop/idpy_oidcop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:24:47.537452 satosa_oidcop-2.0.1/satosa_oidcop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-06-20 17:24:47.000000 satosa_oidcop-2.0.1/satosa_oidcop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-20 17:24:47.000000 satosa_oidcop-2.0.1/satosa_oidcop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 17:24:47.000000 satosa_oidcop-2.0.1/satosa_oidcop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-20 17:24:47.000000 satosa_oidcop-2.0.1/satosa_oidcop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-20 17:24:47.000000 satosa_oidcop-2.0.1/satosa_oidcop.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-20 17:24:47.537452 satosa_oidcop-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-20 17:24:12.000000 satosa_oidcop-2.0.1/setup.py
```

### Comparing `satosa_oidcop-1.1.3/LICENSE` & `satosa_oidcop-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `satosa_oidcop-1.1.3/PKG-INFO` & `satosa_oidcop-2.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satosa_oidcop
-Version: 1.1.3
+Version: 2.0.1
 Summary: SATOSA Frontend based on idetity python oidcop
 Home-page: https://github.com/UniversitaDellaCalabria/satosa-oidcop
 Author: Giuseppe De Marco
 Author-email: giuseppe.demarco@unical.it
 License: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -120,17 +120,22 @@
 * [ ] DPoP support
 
 #### Tests
 
 Before you run the tests mind that you've to start a local mongod instance, e.g. with:
 
 ```
-docker run --rm -e ALLOW_EMPTY_PASSWORD=yes -e MONGODB_ENABLE_JOURNAL=false -p 27017:27017 --name mongodb bitnami/mongodb:latest
+sudo docker run --rm -e ALLOW_EMPTY_PASSWORD=yes -e MONGODB_ENABLE_JOURNAL=false -p 27017:27017 --name mongodb bitnami/mongodb:latest
 ```
 
+If you like you can use mongo-express as a management UI over the local mongo instance:
+````
+sudo docker run -e ME_CONFIG_MONGODB_SERVER=$MONGOHOST-OR-DOCKER-BRIDGE-LIKE-172.17.0.1 -p 8081:8081 mongo-express
+````
+
 Then run the tests:
 
 ````
 pip install pytest pytest-cov
 pytest --cov=satosa_oidcop -v --cov-report term --cov-fail-under=95 tests/
 ````
```

### Comparing `satosa_oidcop-1.1.3/README.md` & `satosa_oidcop-2.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -106,17 +106,22 @@
 * [ ] DPoP support
 
 #### Tests
 
 Before you run the tests mind that you've to start a local mongod instance, e.g. with:
 
 ```
-docker run --rm -e ALLOW_EMPTY_PASSWORD=yes -e MONGODB_ENABLE_JOURNAL=false -p 27017:27017 --name mongodb bitnami/mongodb:latest
+sudo docker run --rm -e ALLOW_EMPTY_PASSWORD=yes -e MONGODB_ENABLE_JOURNAL=false -p 27017:27017 --name mongodb bitnami/mongodb:latest
 ```
 
+If you like you can use mongo-express as a management UI over the local mongo instance:
+````
+sudo docker run -e ME_CONFIG_MONGODB_SERVER=$MONGOHOST-OR-DOCKER-BRIDGE-LIKE-172.17.0.1 -p 8081:8081 mongo-express
+````
+
 Then run the tests:
 
 ````
 pip install pytest pytest-cov
 pytest --cov=satosa_oidcop -v --cov-report term --cov-fail-under=95 tests/
 ````
```

### Comparing `satosa_oidcop-1.1.3/satosa_oidcop/core/application.py` & `satosa_oidcop-2.0.1/satosa_oidcop/core/application.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import os
 
-from oidcop.configure import OPConfiguration
-from oidcop.server import Server
-from oidcop.util import importer
+from idpyoidc.server.configure import OPConfiguration
+from idpyoidc.server import Server
+from idpyoidc.server.util import importer
 
 
 folder = os.path.dirname(os.path.realpath(__file__))
 logger = logging.getLogger(__name__)
 
 
 def oidc_provider_init_app(config, name="oidc_op", **kwargs):
```

### Comparing `satosa_oidcop-1.1.3/satosa_oidcop/core/claims.py` & `satosa_oidcop-2.0.1/satosa_oidcop/core/claims.py`

 * *Files identical despite different names*

### Comparing `satosa_oidcop-1.1.3/satosa_oidcop/core/storage/base.py` & `satosa_oidcop-2.0.1/satosa_oidcop/core/storage/base.py`

 * *Files identical despite different names*

### Comparing `satosa_oidcop-1.1.3/satosa_oidcop/core/storage/mongo.py` & `satosa_oidcop-2.0.1/satosa_oidcop/core/storage/mongo.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 import base64
 import copy
 import datetime
 import json
 import logging
+
+from idpyoidc.server.exception import NoSuchGrant
 import pymongo
 
 from .base import SatosaOidcStorage
-from oidcop.session.manager import SessionManager
+from idpyoidc.server.session.manager import SessionManager
 
 logger = logging.getLogger(__name__)
 
 
 class Mongodb(SatosaOidcStorage):
     session_attr_map = {
-        "oidcop.session.info.UserSessionInfo": "sub",
-        "oidcop.session.info.ClientSessionInfo": "client_id",
-        "oidcop.session.grant.Grant": "grant_id",
+        "idpyoidc.server.session.info.UserSessionInfo": "sub",
+        "idpyoidc.server.session.info.ClientSessionInfo": "client_id",
+        "idpyoidc.server.session.grant.Grant": "grant_id",
     }
     token_attr_map = {
-        "oidcop.session.token.AuthorizationCode": "authorization_code",
-        "oidcop.session.token.AccessToken": "access_token",
-        "oidcop.session.token.RefreshToken": "refresh_token",
-        "oidcop.session.token.IDToken": "id_token",
+        "idpyoidc.server.session.token.AuthorizationCode": "authorization_code",
+        "idpyoidc.server.session.token.AccessToken": "access_token",
+        "idpyoidc.server.session.token.RefreshToken": "refresh_token",
+        "idpyoidc.server.session.token.IDToken": "id_token",
     }
 
     def __init__(self, storage_conf: dict, url: str, connection_params: dict = None):
         self.storage_conf = storage_conf
         self.url = url
         self.connection_params = connection_params
 
@@ -59,29 +61,29 @@
             "sid_encrypted": "",
             "authorization_code": "",
             "access_token": "",
             "id_token": "",
             "refresh_token": "",
             "claims": claims or {},
             "dump": json.dumps(_db),
-            "key": ses_man_dump["key"],
-            "salt": ses_man_dump["salt"],
+            "key": ses_man_dump['crypt_config']['kwargs']["password"],
+            "salt": ses_man_dump['crypt_config']['kwargs']["salt"]
         }
 
         for k, v in _db.items():
             # TODO: ask to roland to have something better than this
-            if len(k) > 128 and ";;" not in k and v[0] == "oidcop.session.grant.Grant":
+            if len(k) > 128 and ";;" not in k and v[0] == "idpyoidc.server.session.grant.Grant":
                 data["sid_encrypted"] = k
                 continue
-
+    
             classname = v[0]
             field_name = self.session_attr_map[classname]
             if field_name == "sub":
-                data["client_id"] = v[1]["subordinate"][0]
-                data[field_name] = v[1]["user_id"]
+                data["client_id"] = list(_db.keys())[1].split(";")[-1]
+                data[field_name] = _db[list(_db.keys())[2]][1]['sub']
             elif field_name == "client_id":
                 data["grant_id"] = v[1]["subordinate"][0]
             elif field_name == "grant_id":
                 _exp_time = datetime.datetime.fromtimestamp(v[1]["expires_at"])
                 data["expires_at"] = _exp_time
                 data["revoked"] = v[1]["revoked"]
                 # data['sub'] = v[1]['sub']
@@ -108,15 +110,15 @@
             self.session_db.insert_one(data)
 
     def load_session_from_db(
         self, parse_req, http_headers: dict, session_manager: SessionManager, **kwargs
     ) -> dict:
         """
         This method detects some usefull elements for doing a lookup in the session storage
-        then loads the session inmemory
+        then loads the session in-memory
 
         It doesn't want to do any validation but only loading a session inmemory
         Security validation will be made later by oidcop in process_request
         """
         data = {}
         _q = {}
         http_authz = http_headers.get("headers", {}).get("authorization", "")
@@ -152,28 +154,30 @@
         res = self.session_db.find_one(_q)
         if res:
             data["key"] = res["key"]
             data["salt"] = res["salt"]
             data["db"] = json.loads(res["dump"])
             session_manager.flush()
             session_manager.load(data)
+        elif 'client_id' in _q:
+            raise NoSuchGrant('The client has not been issued the grant')
         return data
 
     def get_claims_from_sid(self, sid: str):
         self._connect()
         res = self.session_db.find_one({"sid": sid})
         if res:
             return res["claims"]
 
     def insert_client(self, client_data: dict):
         _client_data = copy.deepcopy(client_data)
         self._connect()
         client_id = _client_data["client_id"]
         if self.get_client_by_id(client_id):
-            logger.warning(
+            logger.debug(
                 f"OIDC Client {client_id} already present in the client db")
             return
         self.client_db.insert_one(_client_data)
 
     def get_client_creds_from_basic_auth(self, request_authorization: str):
         cred = base64.b64decode(
             request_authorization.replace("Basic ", "").encode())
@@ -189,21 +193,25 @@
 
         if len(cred) == 2:
             client_id = cred[0]
             return client_id
 
     def get_client_by_basic_auth(self, request_authorization: str):
         cred = self.get_client_creds_from_basic_auth(request_authorization)
-
+        
         if len(cred) == 2:
             client_id = cred[0]
             client_secret = cred[1]
 
             self._connect()
             return self.client_db.find_one(
                 {"client_id": client_id, "client_secret": client_secret}
             )
 
+    def get_client_by_bearer_token(self, request_authorization: str):
+        access_token = request_authorization.replace("Bearer ", "")
+        return self.session_db.find_one({"access_token": access_token})
+
     def get_registered_clients_id(self):
         self._connect()
         res = self.client_db.distinct("client_id")
         return res
```

### Comparing `satosa_oidcop-1.1.3/satosa_oidcop/core/user_authn.py` & `satosa_oidcop-2.0.1/satosa_oidcop/core/user_authn.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from oidcop.user_authn.user import UserAuthnMethod
+from idpyoidc.server.user_authn.user import UserAuthnMethod
 
 
 class SatosaAuthnMethod(UserAuthnMethod):
     """
     Dummy approach to get SATOSA working with oidcop as it is
     """
```

### Comparing `satosa_oidcop-1.1.3/satosa_oidcop/core/user_info.py` & `satosa_oidcop-2.0.1/satosa_oidcop/core/user_info.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from oidcop.user_info import UserInfo
+from idpyoidc.server.user_info import UserInfo
 
 
 class UserInfoDict:
     def __init__(self, claims: dict):
         self.claims = claims
 
     def __getitem__(self, key):
```

### Comparing `satosa_oidcop-1.1.3/satosa_oidcop/idpy_oidcop.py` & `satosa_oidcop-2.0.1/satosa_oidcop/idpy_oidcop.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,37 +3,37 @@
 """
 import base64
 import logging
 import os
 from urllib.parse import urlencode
 
 from cryptojwt.key_jar import KeyJar
-from oidcmsg.oauth2 import ResponseMessage
-from oidcmsg.oidc import AccessTokenRequest
-from oidcmsg.oidc import AuthorizationErrorResponse
-from oidcmsg.oidc import AuthnToken
-from oidcmsg.oidc import TokenErrorResponse
-from oidcmsg.oidc import AuthorizationRequest
-from oidcop.authn_event import create_authn_event
-from oidcop.exception import InvalidClient
-from oidcop.exception import UnAuthorizedClient
-from oidcop.exception import UnknownClient
-from oidcop.token.exception import UnknownToken
-from oidcop.oidc.registration import random_client_id
-
-import satosa.logging_util as lu
+from idpyoidc.message.oauth2 import ResponseMessage
+from idpyoidc.message.oidc import AccessTokenRequest
+from idpyoidc.message.oidc import AuthnToken
+from idpyoidc.message.oidc import AuthorizationErrorResponse
+from idpyoidc.message.oidc import AuthorizationRequest
+from idpyoidc.message.oidc import TokenErrorResponse
+from idpyoidc.server.authn_event import create_authn_event
+from idpyoidc.server.exception import ClientAuthenticationError
+from idpyoidc.server.exception import NoSuchGrant
+from idpyoidc.server.exception import InvalidClient
+from idpyoidc.server.exception import UnAuthorizedClient
+from idpyoidc.server.exception import UnknownClient
+from idpyoidc.server.oidc.registration import random_client_id
 from satosa.context import Context
-from satosa.internal import InternalData
 from satosa.frontends.base import FrontendModule
+from satosa.internal import InternalData
+import satosa.logging_util as lu
 from satosa.response import SeeOther
+
 from .core.application import oidcop_application as oidcop_app
 from .core.claims import combine_claim_values
 from .core.response import JsonResponse
 
-
 IGNORED_HEADERS = ["cookie", "user-agent"]
 logger = logging.getLogger(__name__)
 
 
 class ExtendedContext(Context):  # pragma: no cover
     def __init__(self, **kwargs):
         super().__init__()
@@ -47,53 +47,72 @@
     """
     Interoperability class between satosa and oidcop
     """
 
     def __init__(self):  # pragma: no cover
         self.app = None
 
+    def get_client_info(self, client_id, context):
+        _cinfo = context.cdb.get(client_id)
+        if _cinfo:
+            return _cinfo
+
+        _cinfo = self.app.storage.get_client_by_id(client_id)
+        if _cinfo:
+            context.cdb = {client_id: _cinfo}
+
+        return _cinfo
+
     def _load_cdb(self, context: ExtendedContext, client_id: str = None) -> dict:
         """
         gets client_id from local storage and updates the client DB
         """
         if client_id:
             client_id = client_id
         elif context.request and isinstance(context.request, dict):
             client_id = context.request.get("client_id")
 
-        client = {}
-        _ec = self.app.server.server_get("endpoint_context")
+        _ec = self.app.server.context
 
         if client_id:
             client = self.app.storage.get_client_by_id(client_id)
         elif "Basic " in getattr(context, "request_authorization", ""):
             # here even for introspection endpoint
             client = (
-                self.app.storage.get_client_by_basic_auth(
-                    context.request_authorization)
-                or {}
+                    self.app.storage.get_client_by_basic_auth(
+                        context.request_authorization)
+                    or {}
             )
             client_id = client.get("client_id")
         elif context.request and context.request.get(
-            "client_assertion"
+                "client_assertion"
         ):  # pragma: no cover
             # this is not a validation just a client detection
             # validation is demanded later to oidcop parse_request
 
             ####
             # WARNING: private_key_jwt can't be supported in SATOSA directly to token endpoint
             # because the user MUST always pass through the authorization endpoint
             ####
             token = AuthnToken().from_jwt(
                 txt=context.request["client_assertion"],
                 keyjar=KeyJar(),  # keyless keyjar
-                verify=False,  # otherwise keyjar would contains the issuer key
+                verify=False,  # otherwise keyjar would contain the issuer key
             )
             client_id = token.get("iss")
             client = self.app.storage.get_client_by_id(client_id)
+            
+        elif "Bearer " in getattr(context, "request_authorization", ""):
+            client = (
+                    self.app.storage.get_client_by_bearer_token(
+                        context.request_authorization)
+                    or {}
+            )
+            client_id = client.get("client_id")
+            
         else:  # pragma: no cover
             _ec.cdb = {}
             _msg = f"Client {client_id} not found!"
             logger.warning(_msg)
             raise InvalidClient(_msg)
 
         if client:
@@ -149,57 +168,63 @@
         if getattr(context, "request_authorization", None):
             http_headers["headers"].update(
                 {"authorization": context.request_authorization}
             )
         return http_headers
 
     def store_session_to_db(self, claims=None):
-        sman = self.app.server.server_get("endpoint_context").session_manager
+        sman = self.app.server.context.session_manager
         self.app.storage.store_session_to_db(sman, claims)
         logger.debug(f"Stored oidcop session to db: {sman.dump()}")
 
     def load_session_from_db(self, parse_req, http_headers):
-        sman = self.app.server.server_get("endpoint_context").session_manager
+        sman = self.app.server.context.session_manager
         claims = self.app.storage.load_session_from_db(
             parse_req, http_headers, sman)
         logger.debug(f"Loaded oidcop session from db: {sman.dump()}")
+        
         return claims
 
     def _flush_endpoint_context_memory(self):
         """
         each OAuth2/OIDC request loads an oidcop session in memory
         this method will simply free the memory from any loaded session
         """
-        _ec = self.app.server.server_get("endpoint_context")
+        _ec = self.app.server.context
         sman = _ec.session_manager
         sman.flush()
 
     def _load_session(self, parse_req, endpoint, http_headers):
         """
         actions to perform before an endpoint handles a new http request
         """
         self._flush_endpoint_context_memory()
         self.load_session_from_db(parse_req, http_headers)
 
     def _parse_request(
-        self, endpoint, context: ExtendedContext, http_headers: dict = None
+            self, endpoint, context: ExtendedContext, http_headers: dict = None
     ):
         """
         Returns a parsed OAuth2/OIDC request,
         used by Authorization, Token, Userinfo and Introspection enpoints views
         """
         http_headers = http_headers or self._get_http_headers(context)
         try:
             parse_req = endpoint.parse_request(
-                context.request, http_info=http_headers)
-        except (InvalidClient, UnknownClient, UnAuthorizedClient) as err:
+                context.request, http_info=http_headers,
+            )
+        except (
+                InvalidClient,
+                UnknownClient,
+                UnAuthorizedClient,
+                ClientAuthenticationError,
+        ) as err:
             logger.error(err)
             response = JsonResponse(
-                {"error": "unauthorized_client",
-                    "error_description": str(err)},
+                {"error": "unauthorized_client", "error_description": str(err)},
                 status="403",
             )
             return self.send_response(response)
         return parse_req
 
     def _process_request(self, endpoint, context: Context, parse_req, http_headers):
         """
@@ -228,31 +253,31 @@
     def _log_request(self, context: ExtendedContext, msg: str, level: str = "info"):
         _msg = f"{msg}: {context.request}"
         logline = lu.LOG_FMT.format(
             id=lu.get_session_id(context.state), message=_msg)
         getattr(logger, level)(logline)
 
     def handle_error(
-        self, msg: str = None, excp: Exception = None, status: str = "403"
+            self, msg: str = None, excp: Exception = None, status: str = "403"
     ):  # pragma: no cover
         _msg = f'Something went wrong ... {excp or ""}'
         msg = msg or _msg
         logger.error(msg)
         response = JsonResponse(msg, status=status)
         return self.send_response(response)
 
     def send_response(self, response):
         self._flush_endpoint_context_memory()
         return response
 
     def dump_clients(self):  # pragma: no cover
-        return self.app.server.server_get("endpoint_context").cdb
+        return self.app.server.context.cdb
 
     def dump_sessions(self):  # pragma: no cover
-        return self.app.server.server_get("endpoint_context").session_manager.dump()
+        return self.app.server.context.session_manager.dump()
 
 
 class OidcOpEndpoints(OidcOpUtils):
     """Handles all the oidc endpoint"""
 
     def jwks_endpoint(self, context: Context):
         """
@@ -324,32 +349,32 @@
                         "error": "unauthorized_client",
                         "error_description": "unknown client",
                     }
                 )
             )
 
         raw_request = AccessTokenRequest().from_urlencoded(urlencode(context.request))
-        self._load_session(raw_request, endpoint, http_headers)
-        # in token endpoint we cannot parse a request without having loaded cdb and session first
         try:
-            parse_req = self._parse_request(
-                endpoint, context, http_headers=http_headers
-            )
-        except UnknownToken:
-            return self.send_response(
-                JsonResponse(
-                    {"error": "invalid_token", "error_description": "Unknown Token"},
-                    status="403",
-                )
+            self._load_session(raw_request, endpoint, http_headers)
+        except NoSuchGrant:
+            _response = JsonResponse(
+                {
+                    "error": "invalid_request",
+                    "error_description": "Not owner of token",
+                },
+                status="403",
             )
+            return self.send_response(_response)
+
+        # in token endpoint we cannot parse a request without having loaded cdb and session first
+        parse_req = self._parse_request(endpoint, context, http_headers=http_headers)
 
-        ec = endpoint.server_get("endpoint_context")
+        ec = endpoint.upstream_get("context")
         self._load_claims(ec)
-        proc_req = self._process_request(
-            endpoint, context, parse_req, http_headers)
+        proc_req = self._process_request(endpoint, context, parse_req, http_headers)
         # flush as soon as possible, otherwise in case of an exception it would be
         # stored in the object ... until a next .load would happen ...
         ec.userinfo.flush()
 
         if isinstance(proc_req, JsonResponse):  # pragma: no cover
             return self.send_response(proc_req)
         elif isinstance(proc_req, TokenErrorResponse):
@@ -370,21 +395,56 @@
         return self.send_response(response)
 
     def userinfo_endpoint(self, context: ExtendedContext):
         self._log_request(context, "Userinfo endpoint request")
         endpoint = self.app.server.endpoint["userinfo"]
         http_headers = self._get_http_headers(context)
 
-        # everything depends by bearer access token here
+        # everything depends on bearer access token here
         self._load_session({}, endpoint, http_headers)
+        
+        # not load the client from the session using the bearer token
+        if self.dump_sessions():
+            # load cdb from authz bearer token
+            try:
+                self._load_cdb(context)
+            except Exception:
+                logger.warning(
+                    f"Userinfo endpoint request without any loadable client"
+                )
+                return self.send_response(
+                    JsonResponse(
+                        {"error": "invalid_client", "error_description": "<client not found>"},
+                        status="403",
+                    )
+                )
+        else:
+            logger.warning(
+                f"Userinfo endpoint request without any loadable sessions"
+            )
+            return self.send_response(
+                JsonResponse(
+                    {"error": "invalid_token", "error_description": "<no loadable session>"},
+                    status="403",
+                )
+            )
 
-        parse_req = self._parse_request(
-            endpoint, context, http_headers=http_headers)
+        try:
+            parse_req = self._parse_request(
+                endpoint, context, http_headers=http_headers
+            )
+        except KeyError:
+            return self.send_response(
+                JsonResponse(
+                    {"error": "invalid_token", "error_description": "<TOKEN>"},
+                    status="403",
+                )
+            )
 
-        ec = endpoint.server_get("endpoint_context")
+        ec = endpoint.upstream_get("context")
         self._load_claims(ec)
         proc_req = self._process_request(
             endpoint, context, parse_req, http_headers)
         # flush as soon as possible, otherwise in case of an exception it would be
         # stored in the object ... until a next .load would happen ...
         ec.userinfo.flush()
 
@@ -406,21 +466,25 @@
         self.store_session_to_db()
         return self.send_response(response)
 
     def _load_claims(self, endpoint_context):
         claims = {}
         sman = endpoint_context.session_manager
         for k, v in sman.dump()["db"].items():
-            if v[0] == "oidcop.session.grant.Grant":
+            if v[0] == "idpyoidc.server.session.grant.Grant":
                 sid = k
                 claims = self.app.storage.get_claims_from_sid(sid)
                 break
             else:  # pragma: no cover
-                logger.warning(
-                    "Can't find any suitable sid/claims from stored session")
+                continue
+
+        if not claims:
+            logger.warning(
+                "Can't find any suitable sid/claims from stored session"
+            )
 
         # That's a patchy runtime definition of userinfo db configuration
         endpoint_context.userinfo.load(claims)
 
     def registration_read_endpoint(self, context: Context):
         """
         The Client Configuration Endpoint is an OAuth 2.0 Protected Resource
@@ -498,15 +562,15 @@
 
 class OidcOpFrontend(FrontendModule, OidcOpEndpoints):
     """
     OpenID Connect frontend module based on idpy oidcop
     """
 
     def __init__(
-        self, auth_req_callback_func, internal_attributes, conf, base_url, name
+            self, auth_req_callback_func, internal_attributes, conf, base_url, name
     ):
         super().__init__(auth_req_callback_func, internal_attributes, base_url, name)
         self.app = oidcop_app(conf)
         # Why not
         # self.config = self.app.server.conf
         self.config = self.app.srv_config
         jwks_public_path = self.config["key_conf"]["public_path"]
@@ -568,15 +632,15 @@
             # this should be for humans if auth code flow
             # and JsonResponse for other flows ...
             self.handle_error(excp=excp)
 
         context.state[self.name] = {"oidc_request": context.request}
 
         client_id = parse_req.get("client_id")
-        _client_conf = endpoint.server_get("endpoint_context").cdb[client_id]
+        _client_conf = endpoint.upstream_get("context").cdb[client_id]
         client_name = _client_conf.get("client_name")
         subject_type = _client_conf.get("subject_type", "pairwise")
         if client_name:
             requester_name = [{"lang": "en", "text": client_name}]
         else:  # pragma: no cover
             requester_name = None
 
@@ -649,15 +713,15 @@
             uid=sub,
             salt=base64.b64encode(os.urandom(self.app.salt_size)).decode(),
             # TODO
             # authn_info=auth_args['authn_class_ref'],
             # authn_time=auth_args['iat']
         )
 
-        _ec = endpoint.server_get("endpoint_context")
+        _ec = endpoint.upstream_get("context")
         _token_usage_rules = _ec.authn_broker.get_method_by_id("user")
 
         session_manager = _ec.session_manager
         client = self.app.storage.get_client_by_id(client_id)
         client_subject_type = client.get("subject_type", "public")
         _session_id = session_manager.create_session(
             authn_event=authn_event,
@@ -666,15 +730,15 @@
             client_id=client_id,
             sub_type=client_subject_type,
             token_usage_rules=_token_usage_rules,
         )
 
         try:
             # _args is a dict that contains:
-            #  - oidcmsg.oidc.AuthorizationResponse
+            #  - idpyoidc.message.oidc.AuthorizationResponse
             #  - session_id
             #  - cookie (only need for logout -> not yet supported by Satosa)
             _args = endpoint.authz_part2(
                 user=sub,
                 session_id=_session_id,
                 request=parse_req,
                 authn_event=authn_event,
@@ -684,36 +748,36 @@
             return self.handle_error(excp=excp)
         except Exception as excp:  # pragma: no cover
             return self.handle_error(excp=excp)
 
         if isinstance(_args, ResponseMessage) and "error" in _args:  # pragma: no cover
             return self.send_response(JsonResponse(_args, status="403"))
         elif isinstance(
-            _args.get("response_args"), AuthorizationErrorResponse
+                _args.get("response_args"), AuthorizationErrorResponse
         ):  # pragma: no cover
             rargs = _args.get("response_args")
             logger.error(rargs)
             response = JsonResponse(rargs.to_json(), status="403")
             return self.send_response(response)
 
         info = endpoint.do_response(request=parse_req, **proc_req)
         info_response = info["response"]
         _response_placement = info.get(
             "response_placement", endpoint.response_placement
         )
         if _response_placement == "url":
             data = _args["response_args"].to_dict()
-            redirect_url = info_response + f"{urlencode(data)}"
+            redirect_url = info_response + f"?{urlencode(data)}"
             logger.debug(f"Redirect to: {redirect_url}")
             resp = SeeOther(redirect_url)
         else:  # pragma: no cover
             self._flush_endpoint_context_memory()
             raise NotImplementedError()
 
-        # I don't flush inmem db because it will be flushed by handle_authn_response
+        # I don't flush in-mem db because it will be flushed by handle_authn_response
         return resp
 
     def handle_authn_response(self, context: ExtendedContext, internal_resp):
         """
         See super class method satosa.frontends.base.FrontendModule#handle_authn_response
         :type context: satosa.context.Context
         :type internal_resp: satosa.internal.InternalData
@@ -742,15 +806,16 @@
         auth_req = AuthorizationRequest().from_urlencoded(
             urlencode(exception.state[self.name]["oidc_request"])
         )
         msg = exception.message
         error_resp = AuthorizationErrorResponse(
             error="access_denied",
             error_description=msg,
-            # If the client sent us a state parameter, we should reflect it back according to the spec
+            # If the client sent us a state parameter, we should reflect it back according to the
+            # spec
             **({"state": auth_req["state"]} if "state" in auth_req else {}),
         )
         logline = lu.LOG_FMT.format(
             id=lu.get_session_id(exception.state), message=msg)
         logger.info(logline)
         return SeeOther(
             error_resp.request(
```

### Comparing `satosa_oidcop-1.1.3/satosa_oidcop.egg-info/PKG-INFO` & `satosa_oidcop-2.0.1/satosa_oidcop.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satosa-oidcop
-Version: 1.1.3
+Version: 2.0.1
 Summary: SATOSA Frontend based on idetity python oidcop
 Home-page: https://github.com/UniversitaDellaCalabria/satosa-oidcop
 Author: Giuseppe De Marco
 Author-email: giuseppe.demarco@unical.it
 License: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -120,17 +120,22 @@
 * [ ] DPoP support
 
 #### Tests
 
 Before you run the tests mind that you've to start a local mongod instance, e.g. with:
 
 ```
-docker run --rm -e ALLOW_EMPTY_PASSWORD=yes -e MONGODB_ENABLE_JOURNAL=false -p 27017:27017 --name mongodb bitnami/mongodb:latest
+sudo docker run --rm -e ALLOW_EMPTY_PASSWORD=yes -e MONGODB_ENABLE_JOURNAL=false -p 27017:27017 --name mongodb bitnami/mongodb:latest
 ```
 
+If you like you can use mongo-express as a management UI over the local mongo instance:
+````
+sudo docker run -e ME_CONFIG_MONGODB_SERVER=$MONGOHOST-OR-DOCKER-BRIDGE-LIKE-172.17.0.1 -p 8081:8081 mongo-express
+````
+
 Then run the tests:
 
 ````
 pip install pytest pytest-cov
 pytest --cov=satosa_oidcop -v --cov-report term --cov-fail-under=95 tests/
 ````
```

### Comparing `satosa_oidcop-1.1.3/satosa_oidcop.egg-info/SOURCES.txt` & `satosa_oidcop-2.0.1/satosa_oidcop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `satosa_oidcop-1.1.3/setup.py` & `satosa_oidcop-2.0.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,11 +26,11 @@
     package_data={f"{_pkg_name}": [
             i.replace(f'{_pkg_name}/', '')
             for i in glob(f'{_pkg_name}/**', recursive=True)
         ]
     },
     install_requires=[
         "satosa>=8.0.0",
-        "pymongo>=3.11,<=4.0.1",
-        "oidcop>=2.3.3,<=2.3.4"
+        "pymongo>=3.11,<=4.3",
+        "idpyoidc>=2.0.0,<=2.1.0"
     ],
 )
```

