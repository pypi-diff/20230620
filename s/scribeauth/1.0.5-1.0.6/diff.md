# Comparing `tmp/scribeauth-1.0.5-py3-none-any.whl.zip` & `tmp/scribeauth-1.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 8050 bytes, number of entries: 9
+Zip file size: 8053 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat       66 b- defN 23-May-17 09:44 scribeauth/__init__.py
--rw-rw-rw-  2.0 fat      521 b- defN 23-Jun-12 14:20 scribeauth/__main__.py
--rw-rw-rw-  2.0 fat    14380 b- defN 23-Jun-14 18:03 scribeauth/scribeauth.py
+-rw-rw-rw-  2.0 fat      664 b- defN 23-Jun-20 10:33 scribeauth/__main__.py
+-rw-rw-rw-  2.0 fat    14309 b- defN 23-Jun-20 10:12 scribeauth/scribeauth.py
 -rw-rw-rw-  2.0 fat     1351 b- defN 23-May-15 17:21 scribeauth/scribeauthfederation.py
--rw-rw-rw-  2.0 fat     1097 b- defN 23-Jun-14 18:04 scribeauth-1.0.5.dist-info/LICENSE.md
--rw-rw-rw-  2.0 fat     5073 b- defN 23-Jun-14 18:04 scribeauth-1.0.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-14 18:04 scribeauth-1.0.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Jun-14 18:04 scribeauth-1.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      732 b- defN 23-Jun-14 18:04 scribeauth-1.0.5.dist-info/RECORD
-9 files, 23323 bytes uncompressed, 6786 bytes compressed:  70.9%
+-rw-rw-rw-  2.0 fat     1097 b- defN 23-Jun-20 10:34 scribeauth-1.0.6.dist-info/LICENSE.md
+-rw-rw-rw-  2.0 fat     5008 b- defN 23-Jun-20 10:34 scribeauth-1.0.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-20 10:34 scribeauth-1.0.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Jun-20 10:34 scribeauth-1.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      732 b- defN 23-Jun-20 10:34 scribeauth-1.0.6.dist-info/RECORD
+9 files, 23330 bytes uncompressed, 6789 bytes compressed:  70.9%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: scribeauth/scribeauth.py
 Comment: 
 
 Filename: scribeauth/scribeauthfederation.py
 Comment: 
 
-Filename: scribeauth-1.0.5.dist-info/LICENSE.md
+Filename: scribeauth-1.0.6.dist-info/LICENSE.md
 Comment: 
 
-Filename: scribeauth-1.0.5.dist-info/METADATA
+Filename: scribeauth-1.0.6.dist-info/METADATA
 Comment: 
 
-Filename: scribeauth-1.0.5.dist-info/WHEEL
+Filename: scribeauth-1.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: scribeauth-1.0.5.dist-info/top_level.txt
+Filename: scribeauth-1.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: scribeauth-1.0.5.dist-info/RECORD
+Filename: scribeauth-1.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## scribeauth/__main__.py

```diff
@@ -1,13 +1,14 @@
 import argparse
 from scribeauth import ScribeAuth
 
 if __name__ == '__main__':
 
     parser = argparse.ArgumentParser('scribeauth')
     parser.add_argument('--client_id', help='Client ID provided by Scribe', type=str)
+    parser.add_argument('--user_pool_id', help='User pool ID provided by Scribe', type=str)
     parser.add_argument('--username', help='Username', type=str)
     parser.add_argument('--password', help='Password', type=str)
     args = parser.parse_args()
-    auth = ScribeAuth(args.client_id)
+    auth = ScribeAuth({'client_id': args.client_id, 'user_pool_id': args.user_pool_id})
     tokens = auth.get_tokens(username=args.username, password=args.password)
     print(tokens)
```

## scribeauth/scribeauth.py

```diff
@@ -59,51 +59,38 @@
 class UnknownException(Exception):
     pass
 
 def is_complete_credentials(cred: Credentials) -> bool:
     return 'AccessKeyId' in cred and 'SecretKey' in cred and 'SessionToken' in cred
 
 class ScribeAuth:
-    def __init__(self, param: Union[Unpack[PoolConfiguration], str]):
+    def __init__(self, param: PoolConfiguration):
         """Construct an authorisation client.
 
         Args
         ----
-        Union[Unpack[PoolConfiguration], str]
-        A parameter that can either be an instance of PoolConfiguration or a string.
-        
-        ---
-
         PoolConfiguration:
+
         ---
         client_id -- The client ID of the application provided by Scribe.
         
         user_pool_id -- The user pool ID provided by Scribe.
         
         identity_pool_id -- The identity pool ID provided by Scribe.
-
-        ---
-
-        str:
-        ---
-        client_id -- The client ID of the application provided by Scribe.
         """
         config = Config(signature_version=botocore.UNSIGNED)
         self.client_unsigned = boto3.client(
             'cognito-idp', config=config, region_name='eu-west-2')
         self.client_signed = boto3.client(
             'cognito-idp', region_name='eu-west-2')
-        self.fed_client = boto3.client('cognito-identity', region_name='eu-west-2')
-        if isinstance(param, str):
-            self.client_id = param
-        else:
-            self.client_id = param.get('client_id')
-            self.user_pool_id = param.get('user_pool_id')
-            self.identity_pool_id = param.get('identity_pool_id')
-
+        self.client_id = param.get('client_id')
+        self.user_pool_id = param.get('user_pool_id')
+        self.identity_pool_id = param.get('identity_pool_id')
+        if(param.get('identity_pool_id')):
+            self.fed_client = boto3.client('cognito-identity', region_name='eu-west-2')
 
     def change_password(self, username: str, password: str, new_password: str) -> bool: # pragma: no cover
         """Creates a new password for a user.
 
         Args
         ----
         username -- Username (usually an email address).
@@ -125,15 +112,15 @@
                     access_token = auth_result.get('AccessToken')
                     self.__change_password_cognito(
                         password, new_password, access_token)
                     return True
                 except Exception as err:
                     raise err
             else:
-                if not self.client_id:
+                if not hasattr(self, 'client_id'):
                     raise MissingIdException("Missing client ID")
                 session = response_initiate.get("Session")
                 challenge_parameters = response_initiate.get("ChallengeParameters")
                 user_id_SRP = challenge_parameters.get("USER_ID_FOR_SRP")
                 required_attributes = challenge_parameters.get("requiredAttributes")
                 try:
                     self.__respond_to_auth_challenge(
@@ -232,18 +219,18 @@
         ----
         id_token -- Id token to use.
 
         Returns
         -------
         str
         """
-        if not self.user_pool_id:
+        if not hasattr(self, 'user_pool_id'):
             raise MissingIdException('Missing user pool ID')
-        if not self.identity_pool_id:
-            raise MissingIdException('Missing federated pool ID')
+        if not hasattr(self, 'fed_client'):
+            raise MissingIdException('Federated pool ID is not provided. Create a new ScribeAuth object using identity_pool_id')
         try:
             response = self.fed_client.get_id(
                 IdentityPoolId=self.identity_pool_id,
                 Logins={
                     f'cognito-idp.eu-west-2.amazonaws.com/{self.user_pool_id}': id_token
                 }
             )
@@ -267,16 +254,18 @@
 
         id_token -- Id token to use.
 
         Returns
         -------
         Credentials -- Dictionary {"AccessKeyId": "str", "SecretKey": "str", "SessionToken": "str", "Expiration": "str"}
         """
-        if not self.user_pool_id:
+        if not hasattr(self, 'user_pool_id'):
             raise MissingIdException('Missing user pool ID')
+        if not hasattr(self, 'fed_client'):
+            raise MissingIdException('Federated pool ID is not provided. Create a new ScribeAuth object using identity_pool_id')
         try:
             response = self.fed_client.get_credentials_for_identity(
                 IdentityId=id,
                 Logins={
                     f'cognito-idp.eu-west-2.amazonaws.com/{self.user_pool_id}': id_token
                 }
             )
@@ -330,15 +319,16 @@
                     'access_token': result.get('AccessToken'),
                     'id_token': result.get('IdToken')
                 }
             except:
                 raise UnauthorizedException("Username and/or Password are incorrect. Could not get tokens")
         else:
             raise UnauthorizedException("Username and/or Password are missing. Could not get tokens")
-       
+ 
+ 
     def __get_tokens_with_refresh(self, refresh_token: str):
         try:
             auth_result = 'AuthenticationResult'
             response = self.client_signed.initiate_auth(ClientId=self.client_id, AuthFlow='REFRESH_TOKEN', AuthParameters={'REFRESH_TOKEN': refresh_token})
             result = response.get(auth_result)
             return {
                 'refresh_token': refresh_token,
```

## Comparing `scribeauth-1.0.5.dist-info/LICENSE.md` & `scribeauth-1.0.6.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `scribeauth-1.0.5.dist-info/METADATA` & `scribeauth-1.0.6.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,130 +1,134 @@
-Metadata-Version: 2.1
-Name: scribeauth
-Version: 1.0.5
-Summary: Library to authenticate to Scribe's platform
-Home-page: https://github.com/ScribeLabsAI/ScribeAuth
-Author: Ailin Venerus
-Author-email: ailin@scribelabs.ai
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Security
-Classifier: Typing :: Typed
-Requires-Python: >=3.10.0
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-Requires-Dist: boto3
-Requires-Dist: typing-extensions
-
-# Scribe Auth
-
-Most calls to Scribe's API require authentication and authorization. This library simplifies this process.
-
-You first need a Scribe account and a client ID. Both can be requested at support[atsign]scribelabs[dotsign]ai or through Intercom on https://platform.scribelabs.ai if you already have a Scribe account.
-
-This library interacts directly with our authentication provider [AWS Cognito](https://aws.amazon.com/cognito/) meaning that your username and password never transit through our servers.
-
-## Installation
-
-```bash
-pip install scribeauth
-```
-
-This library requires Python >= 3.10 that supports typing.
-
-## Methods
-
-### 1. Changing password
-
-```python
-from scribeauth import ScribeAuth
-access = ScribeAuth(client_id)
-access.change_password('username', 'password', 'new_password')
-```
-
-### 2. Recovering an account in case of forgotten password
-
-```python
-from scribeauth import ScribeAuth
-access = ScribeAuth(client_id)
-access.forgot_password('username', 'password', 'confirmation_code')
-```
-
-### 3. Get or generate tokens
-
-##### With username and password
-
-```python
-from scribeauth import ScribeAuth
-access = ScribeAuth(client_id)
-access.get_tokens(username='username', password='password')
-```
-
-##### With refresh token
-
-```python
-from scribeauth import ScribeAuth
-access = ScribeAuth(client_id)
-access.get_tokens(refresh_token='refresh_token')
-```
-
-### 4. Revoking a refresh token
-
-```python
-from scribeauth import ScribeAuth
-access = ScribeAuth(client_id)
-access.revoke_refresh_token('refresh_token')
-```
-
-### 5. Getting federated id
-
-```python
-from scribeauth import ScribeAuth
-access = ScribeAuth({'client_id': your_client_id, 'user_pool_id': your_user_pool_id, 'identity_pool_id': your_identity_pool_id})
-access.get_federated_id('your_id_token')
-```
-
-### 6. Getting federated credentials
-
-```python
-from scribeauth import ScribeAuth
-access = ScribeAuth({'client_id': your_client_id, 'user_pool_id': your_user_pool_id, 'identity_pool_id': your_identity_pool_id})
-access.get_federated_credentials('your_federated_id', 'your_id_token')
-```
-
-### 7. Getting signature for request
-
-```python
-from scribeauth import ScribeAuth
-access = ScribeAuth({'client_id': your_client_id, 'user_pool_id': your_user_pool_id, 'identity_pool_id': your_identity_pool_id})
-access.get_signature_for_request(request='your_request', credentials='your_federated_credentials')
-```
-
-## Flow
-
-- If you never have accessed your Scribe account, it probably still contains the temporary password we generated for you. You can change it directly on the [platform](https://platform.scribelabs.ai) or with the `change_password` method. You won't be able to access anything else until the temporary password has been changed.
-
-- Once the account is up and running, you can request new tokens with `get_tokens`. You will initially have to provide your username and password. The access and id tokens are valid for up to 30 minutes. The refresh token is valid for 30 days.
-
-- While you have a valid refresh token, you can request fresh access and id tokens with `get_tokens` but using the refresh token this time, so you're not sending your username and password over the wire anymore.
-
-- In case you suspect that your refresh token has been leaked, you can revoke it with `revoke_token`. This will also invalidate any access/id token that has been issued with it. In order to get a new one, you'll need to use your username and password again.
-
-- You can get your federated id by using `get_federated_id` and providing your id token. The federated id will allow you to use `get_federated_credentials` to get an access key id, secret key and session token.
-
-- Every API call to be made to Scribe's API Gateway needs to have a signature. You can get the signature for your request by using `get_signature_for_request`. Provide the request you'll be using and your credentials (use `get_federated_credentials` to get them).
-
-## Command line
-
-You can also use the package as follows for quick access to tokens:
-
-```bash
-python -m scribeauth --client_id clientid --username username --password password
-```
-
----
-
-To flag an issue, open a ticket on [Github](https://github.com/ScribeLabsAI/ScribeAuth/issues) and contact us on Intercom through the platform.
+Metadata-Version: 2.1
+Name: scribeauth
+Version: 1.0.6
+Summary: Library to authenticate to Scribe's platform
+Home-page: https://github.com/ScribeLabsAI/ScribeAuth
+Author: Ailin Venerus
+Author-email: ailin@scribelabs.ai
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Security
+Classifier: Typing :: Typed
+Requires-Python: >=3.10.0
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+Requires-Dist: boto3
+Requires-Dist: typing-extensions
+
+# Scribe Auth
+
+Most calls to Scribe's API require authentication and authorization. This library simplifies this process.
+
+You first need a Scribe account and a client ID. Both can be requested at support[atsign]scribelabs[dotsign]ai or through Intercom on https://platform.scribelabs.ai if you already have a Scribe account.
+
+This library interacts directly with our authentication provider [AWS Cognito](https://aws.amazon.com/cognito/) meaning that your username and password never transit through our servers.
+
+## Installation
+
+```bash
+pip install scribeauth
+```
+
+This library requires Python >= 3.10 that supports typing.
+
+## Methods
+
+### 1. Changing password
+
+```python
+from scribeauth import ScribeAuth
+access = ScribeAuth(client_id)
+access.change_password('username', 'password', 'new_password')
+```
+
+### 2. Recovering an account in case of forgotten password
+
+```python
+from scribeauth import ScribeAuth
+access = ScribeAuth(client_id)
+access.forgot_password('username', 'password', 'confirmation_code')
+```
+
+### 3. Get or generate tokens
+
+##### With username and password
+
+```python
+from scribeauth import ScribeAuth
+access = ScribeAuth(client_id)
+access.get_tokens(username='username', password='password')
+```
+
+##### With refresh token
+
+```python
+from scribeauth import ScribeAuth
+access = ScribeAuth(client_id)
+access.get_tokens(refresh_token='refresh_token')
+```
+
+### 4. Revoking a refresh token
+
+```python
+from scribeauth import ScribeAuth
+access = ScribeAuth(client_id)
+access.revoke_refresh_token('refresh_token')
+```
+
+### 5. Getting federated id
+
+```python
+from scribeauth import ScribeAuth
+access = ScribeAuth({'client_id': your_client_id, 'user_pool_id': your_user_pool_id, 'identity_pool_id': your_identity_pool_id})
+access.get_federated_id('your_id_token')
+```
+
+### 6. Getting federated credentials
+
+```python
+from scribeauth import ScribeAuth
+access = ScribeAuth({'client_id': your_client_id, 'user_pool_id': your_user_pool_id, 'identity_pool_id': your_identity_pool_id})
+access.get_federated_credentials('your_federated_id', 'your_id_token')
+```
+
+### 7. Getting signature for request
+
+```python
+from scribeauth import ScribeAuth
+access = ScribeAuth({'client_id': your_client_id, 'user_pool_id': your_user_pool_id, 'identity_pool_id': your_identity_pool_id})
+access.get_signature_for_request(request='your_request', credentials='your_federated_credentials')
+```
+
+## Flow
+
+- If you never have accessed your Scribe account, it probably still contains the temporary password we generated for you. You can change it directly on the [platform](https://platform.scribelabs.ai) or with the `change_password` method. You won't be able to access anything else until the temporary password has been changed.
+
+- Once the account is up and running, you can request new tokens with `get_tokens`. You will initially have to provide your username and password. The access and id tokens are valid for up to 30 minutes. The refresh token is valid for 30 days.
+
+- While you have a valid refresh token, you can request fresh access and id tokens with `get_tokens` but using the refresh token this time, so you're not sending your username and password over the wire anymore.
+
+- In case you suspect that your refresh token has been leaked, you can revoke it with `revoke_token`. This will also invalidate any access/id token that has been issued with it. In order to get a new one, you'll need to use your username and password again.
+
+- You can get your federated id by using `get_federated_id` and providing your id token. The federated id will allow you to use `get_federated_credentials` to get an access key id, secret key and session token.
+
+- Every API call to be made to Scribe's API Gateway needs to have a signature. You can get the signature for your request by using `get_signature_for_request`. Provide the request you'll be using and your credentials (use `get_federated_credentials` to get them).
+
+## Command line
+
+You can also use the package as follows for quick access to tokens:
+
+```bash
+python -m scribeauth --client_id clientid --user_pool_id user_pool_id --username username --password password
+```
+
+---
+
+To flag an issue, open a ticket on [Github](https://github.com/ScribeLabsAI/ScribeAuth/issues) and contact us on Intercom through the platform.
+
+
```

