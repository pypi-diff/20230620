# Comparing `tmp/d20-securityLayer-2.0.0a7.tar.gz` & `tmp/d20-securityLayer-2.0.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\d20\tools\libs\security_layer_python_arangodb\dist\.tmp-r12bei2s\d20-securityLayer-2.0.0a7.tar", last modified: Tue Jun 20 03:01:36 2023, max compression
+gzip compressed data, was "D:\d20\tools\libs\security_layer_python_arangodb\dist\.tmp-evjxy3hg\d20-securityLayer-2.0.0a8.tar", last modified: Tue Jun 20 03:07:46 2023, max compression
```

## Comparing `d20-securityLayer-2.0.0a7.tar` & `d20-securityLayer-2.0.0a8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 03:01:36.468690 d20-securityLayer-2.0.0a7/
--rw-rw-rw-   0        0        0     1064 2021-09-22 23:30:22.000000 d20-securityLayer-2.0.0a7/LICENSE
--rw-rw-rw-   0        0        0      677 2023-06-20 03:01:36.467689 d20-securityLayer-2.0.0a7/PKG-INFO
--rw-rw-rw-   0        0        0      105 2021-06-18 21:41:10.000000 d20-securityLayer-2.0.0a7/README.md
--rw-rw-rw-   0        0        0      108 2021-09-22 23:14:25.000000 d20-securityLayer-2.0.0a7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-20 03:01:36.468690 d20-securityLayer-2.0.0a7/setup.cfg
--rw-rw-rw-   0        0        0      964 2023-06-20 03:01:17.000000 d20-securityLayer-2.0.0a7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-20 03:01:36.407952 d20-securityLayer-2.0.0a7/src/
-drwxrwxrwx   0        0        0        0 2023-06-20 03:01:36.437120 d20-securityLayer-2.0.0a7/src/d20_securityLayer.egg-info/
--rw-rw-rw-   0        0        0      677 2023-06-20 03:01:36.000000 d20-securityLayer-2.0.0a7/src/d20_securityLayer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      511 2023-06-20 03:01:36.000000 d20-securityLayer-2.0.0a7/src/d20_securityLayer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 03:01:36.000000 d20-securityLayer-2.0.0a7/src/d20_securityLayer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-06-20 03:01:36.000000 d20-securityLayer-2.0.0a7/src/d20_securityLayer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-20 03:01:36.000000 d20-securityLayer-2.0.0a7/src/d20_securityLayer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-20 03:01:36.466689 d20-securityLayer-2.0.0a7/src/securityLayer/
--rw-rw-rw-   0        0        0    10081 2023-05-12 01:22:57.000000 d20-securityLayer-2.0.0a7/src/securityLayer/AccessControl.py
--rw-rw-rw-   0        0        0      233 2023-05-16 00:25:53.000000 d20-securityLayer-2.0.0a7/src/securityLayer/AuthAnswer.py
--rw-rw-rw-   0        0        0     9697 2023-05-16 02:42:02.000000 d20-securityLayer-2.0.0a7/src/securityLayer/Error.py
--rw-rw-rw-   0        0        0    16797 2023-06-07 23:54:37.000000 d20-securityLayer-2.0.0a7/src/securityLayer/SSO.py
--rw-rw-rw-   0        0        0    15275 2023-06-20 03:01:13.000000 d20-securityLayer-2.0.0a7/src/securityLayer/SecurityLayer.py
--rw-rw-rw-   0        0        0      125 2023-01-02 23:20:55.000000 d20-securityLayer-2.0.0a7/src/securityLayer/__init__.py
--rw-rw-rw-   0        0        0      156 2023-06-20 03:01:19.000000 d20-securityLayer-2.0.0a7/src/securityLayer/__version__.py
--rw-rw-rw-   0        0        0       55 2021-09-23 23:27:01.000000 d20-securityLayer-2.0.0a7/src/securityLayer/default.py
+drwxrwxrwx   0        0        0        0 2023-06-20 03:07:46.301811 d20-securityLayer-2.0.0a8/
+-rw-rw-rw-   0        0        0     1064 2021-09-22 23:30:22.000000 d20-securityLayer-2.0.0a8/LICENSE
+-rw-rw-rw-   0        0        0      677 2023-06-20 03:07:46.299270 d20-securityLayer-2.0.0a8/PKG-INFO
+-rw-rw-rw-   0        0        0      105 2021-06-18 21:41:10.000000 d20-securityLayer-2.0.0a8/README.md
+-rw-rw-rw-   0        0        0      108 2021-09-22 23:14:25.000000 d20-securityLayer-2.0.0a8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-20 03:07:46.301811 d20-securityLayer-2.0.0a8/setup.cfg
+-rw-rw-rw-   0        0        0      964 2023-06-20 03:07:08.000000 d20-securityLayer-2.0.0a8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 03:07:46.227762 d20-securityLayer-2.0.0a8/src/
+drwxrwxrwx   0        0        0        0 2023-06-20 03:07:46.255530 d20-securityLayer-2.0.0a8/src/d20_securityLayer.egg-info/
+-rw-rw-rw-   0        0        0      677 2023-06-20 03:07:46.000000 d20-securityLayer-2.0.0a8/src/d20_securityLayer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      511 2023-06-20 03:07:46.000000 d20-securityLayer-2.0.0a8/src/d20_securityLayer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 03:07:46.000000 d20-securityLayer-2.0.0a8/src/d20_securityLayer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-06-20 03:07:46.000000 d20-securityLayer-2.0.0a8/src/d20_securityLayer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-20 03:07:46.000000 d20-securityLayer-2.0.0a8/src/d20_securityLayer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 03:07:46.298299 d20-securityLayer-2.0.0a8/src/securityLayer/
+-rw-rw-rw-   0        0        0    10081 2023-06-20 03:06:54.000000 d20-securityLayer-2.0.0a8/src/securityLayer/AccessControl.py
+-rw-rw-rw-   0        0        0      233 2023-05-16 00:25:53.000000 d20-securityLayer-2.0.0a8/src/securityLayer/AuthAnswer.py
+-rw-rw-rw-   0        0        0     9697 2023-05-16 02:42:02.000000 d20-securityLayer-2.0.0a8/src/securityLayer/Error.py
+-rw-rw-rw-   0        0        0    16797 2023-06-07 23:54:37.000000 d20-securityLayer-2.0.0a8/src/securityLayer/SSO.py
+-rw-rw-rw-   0        0        0    15275 2023-06-20 03:06:27.000000 d20-securityLayer-2.0.0a8/src/securityLayer/SecurityLayer.py
+-rw-rw-rw-   0        0        0      125 2023-01-02 23:20:55.000000 d20-securityLayer-2.0.0a8/src/securityLayer/__init__.py
+-rw-rw-rw-   0        0        0      156 2023-06-20 03:07:02.000000 d20-securityLayer-2.0.0a8/src/securityLayer/__version__.py
+-rw-rw-rw-   0        0        0       55 2021-09-23 23:27:01.000000 d20-securityLayer-2.0.0a8/src/securityLayer/default.py
```

### Comparing `d20-securityLayer-2.0.0a7/LICENSE` & `d20-securityLayer-2.0.0a8/LICENSE`

 * *Files identical despite different names*

### Comparing `d20-securityLayer-2.0.0a7/PKG-INFO` & `d20-securityLayer-2.0.0a8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: d20-securityLayer
-Version: 2.0.0a7
+Version: 2.0.0a8
 Summary: A simple access manager
 Home-page: https://github.com/d20services/security_layer_python_arangodb
 Author: Alex Sánchez Vega
 Author-email: alex@d20.services
 Project-URL: Bug Tracker, https://github.com/d20services/security_layer_python_arangodb/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `d20-securityLayer-2.0.0a7/setup.py` & `d20-securityLayer-2.0.0a8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="d20-securityLayer",
-    version="2.0.0a7",
+    version="2.0.0a8",
     author="Alex Sánchez Vega",
     author_email="alex@d20.services",
     description="A simple access manager",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/d20services/security_layer_python_arangodb",
     project_urls={
```

### Comparing `d20-securityLayer-2.0.0a7/src/d20_securityLayer.egg-info/PKG-INFO` & `d20-securityLayer-2.0.0a8/src/d20_securityLayer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: d20-securityLayer
-Version: 2.0.0a7
+Version: 2.0.0a8
 Summary: A simple access manager
 Home-page: https://github.com/d20services/security_layer_python_arangodb
 Author: Alex Sánchez Vega
 Author-email: alex@d20.services
 Project-URL: Bug Tracker, https://github.com/d20services/security_layer_python_arangodb/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `d20-securityLayer-2.0.0a7/src/securityLayer/AccessControl.py` & `d20-securityLayer-2.0.0a8/src/securityLayer/AccessControl.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
             token.auth()
         except HTTPError:
             token_id = jr.get('otp')
             otp = SecurityLayer.OneTimeAccess(data= {'_key': token_id, 'username': jr['username']})
             try:
                 otp.find()
                 token = SecurityLayer.UserToken(data={'username': jr.get('username'), 'oauth': jr.get('oauth'), 'oauth_client': token.get('apiuser'), 'scopes': jr.get('scopes'), 'userid': otp.get('userid')})
-                token.create()
+                token.insert()
             except HTTPError as e:
                 AuthAnswer(False, error= e())           
     elif (kwargs.get('oauth', False) == True or kwargs.get('TPAMI', False) == True or kwargs.get('file_req', False) == True) and access_code != '':
         try:
             token = break_access_token(access_code)
         except:
             return AuthAnswer(False, error= SSOInvalidUserTokenError())
```

### Comparing `d20-securityLayer-2.0.0a7/src/securityLayer/Error.py` & `d20-securityLayer-2.0.0a8/src/securityLayer/Error.py`

 * *Files identical despite different names*

### Comparing `d20-securityLayer-2.0.0a7/src/securityLayer/SSO.py` & `d20-securityLayer-2.0.0a8/src/securityLayer/SSO.py`

 * *Files identical despite different names*

### Comparing `d20-securityLayer-2.0.0a7/src/securityLayer/SecurityLayer.py` & `d20-securityLayer-2.0.0a8/src/securityLayer/SecurityLayer.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,21 +35,21 @@
             self.collection = 'PasswordRecoveryTokens'
 
         def make(self):
             self.attributes = ['_key', 'created', 'updated', 'valid_thru', 'active', 'userid', 'username']
             for key in self.attributes:
                 setattr(self, key, None)
 
-        def create(self):
+        def insert(self):
             p = Metadata.Parameter()
             p.load('psswdrec_lifespawn')
             psswdrec_lifespawn = p.get('value')
             self.valid_thru = self.created + datetime.timedelta(minutes=psswdrec_lifespawn)
             self.active = True
-            return super().create()
+            return super().insert()
 
         def load(self):
             query = [{"dim":"_key", 'op':'==', 'val': self._key},
                      {"dim":"active", 'op':'==', 'val': True},
                      {"dim":"userid", 'op':'==', 'val': self.userid}]
             try:
                 self.search(query_list=query, limit=1)
@@ -73,21 +73,21 @@
             self.collection = 'OTP'
 
         def make(self):
             self.attributes = ['_key', 'created', 'updated', 'valid_thru', 'active', 'userid', 'username']
             for key in self.attributes:
                 setattr(self, key, None)
 
-        def create(self):
+        def insert(self):
             p = Metadata.Parameter()
             p.load('otp_lifespawn')            
             otp_lifespawn = p.get('value')
             self.valid_thru = self.created + datetime.timedelta(minutes=otp_lifespawn)
             self.active = True
-            return super().create()
+            return super().insert()
 
         def load(self):
             query = [{"dim":"_key", 'op':'==', 'val': self._key},
                      {"dim":"active", 'op':'==', 'val': True},
                      {"dim":"userid", 'op':'==', 'val': self.userid}]
             try:
                 self.search(query_list=query, limit=1)
@@ -117,25 +117,25 @@
         
         def auth(self):
             user = SecurityLayer.UserAccess(data={"username" : self.get('userid'), 'password' : self.get('password')})
             self.password = None
             
             if user.auth()==True:
                 self.userid = user.get('_key')
-                self.create()
+                self.insert()
             else: 
                 raise SSOInvalidCredentialsError
 
-        def create(self):
+        def insert(self):
             p = Metadata.Parameter()
             p.load('user_token_lifespawn')
             user_token_lifespawn = p.get('value')
             self.valid_thru = self.created + datetime.timedelta(minutes=user_token_lifespawn)
             self.active = True
-            return super().create()
+            return super().insert()
 
         def find(self):
             query = [{"dim":"_key", 'op':'==', 'val': self._key},
                      {"dim":"oauth" if self.get('oauth') != True else "active", 'op':'==', 'val': True},
                      {"dim":"userid", 'op':'==', 'val': self.userid}]
             try:
                 self.search(query_list=query, limit=1)
@@ -172,18 +172,18 @@
             self.attributes = ['_key', 'password', 'username', 'created', 'updated']
             for key in self.attributes:
                 setattr(self, key, None)
         
         def auth(self):
             return self.verify_password()
 
-        def create(self):
+        def insert(self):
             self.password = self.hash_password()
             self.active = True
-            return super().create()
+            return super().insert()
             
         def verify_password(self):
             self.load(self.get('username'))
             stored_password = self.get("password")
             self.id = self.get("_key")
             salt = stored_password[:64]
             stored_password = stored_password[64:]
@@ -233,19 +233,19 @@
 
         def auth(self):
             api_access = SecurityLayer.APIAccess(data={"username" : self.get('apiuser'), 'password' : self.get('apisecret')})
             self.password = None
             if api_access.auth()==True:
                 self.build_from_access(api_access)
                 self._key = None
-                self.create()
+                self.insert()
             else:
                 raise SSOInvalidCredentialsError
 
-        def create(self):
+        def insert(self):
             if self.get('origin') == None or self.get('origin') == '':
                 self.origin = ['NoCors']
             if not isinstance(self.get('origin'), list):
                 self.origin = [self.get('origin')]
             if not isinstance(self.get('oauth_urls'), list):
                 self.oauth_urls = [self.get('oauth_urls')]
             if self.get('permalink') == True:
@@ -253,15 +253,15 @@
             else:
                 p = Metadata.Parameter()
                 p.load('api_token_lifespawn')
                 api_token_lifespawn = p.get('value')
                 self.valid_thru = self.created + datetime.timedelta(minutes=api_token_lifespawn)
             self.active = True
             self.deleted = False
-            return super().create()
+            return super().insert()
 
         def find(self):
             self.id = self.get('_key')
             origin = self.get('origin')
             self.load()
             if origin == None or origin == '':
                 origin = 'NoCors'
@@ -341,10 +341,10 @@
         def update(self):
             if self.password != None and self.password != '':
                 self.password = self.hash_password()
             else:
                 self.password = None
             return super().update()
 
-        def create(self):
+        def insert(self):
             self.password = self.hash_password()
-            return super().create()
+            return super().insert()
```

