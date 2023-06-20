# Comparing `tmp/fusionauth-client-1.8.0rc1.tar.gz` & `tmp/fusionauth-client-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fusionauth-client-1.8.0rc1.tar", last modified: Sun Sep  8 15:20:21 2019, max compression
+gzip compressed data, was "dist/fusionauth-client-1.9.0.tar", last modified: Mon Sep 23 19:06:34 2019, max compression
```

## Comparing `fusionauth-client-1.8.0rc1.tar` & `fusionauth-client-1.9.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 degroff    (501) staff       (20)        0 2019-09-08 15:20:21.000000 fusionauth-client-1.8.0rc1/
--rw-r--r--   0 degroff    (501) staff       (20)     2055 2019-09-08 15:20:21.000000 fusionauth-client-1.8.0rc1/PKG-INFO
--rw-r--r--   0 degroff    (501) staff       (20)     1280 2018-10-30 02:11:50.000000 fusionauth-client-1.8.0rc1/README.md
--rw-r--r--   0 degroff    (501) staff       (20)       38 2019-09-08 15:20:21.000000 fusionauth-client-1.8.0rc1/setup.cfg
--rw-r--r--   0 degroff    (501) staff       (20)      868 2019-09-06 21:37:44.000000 fusionauth-client-1.8.0rc1/setup.py
-drwxr-xr-x   0 degroff    (501) staff       (20)        0 2019-09-08 15:20:21.000000 fusionauth-client-1.8.0rc1/src/
-drwxr-xr-x   0 degroff    (501) staff       (20)        0 2019-09-08 15:20:21.000000 fusionauth-client-1.8.0rc1/src/main/
-drwxr-xr-x   0 degroff    (501) staff       (20)        0 2019-09-08 15:20:21.000000 fusionauth-client-1.8.0rc1/src/main/python/
-drwxr-xr-x   0 degroff    (501) staff       (20)        0 2019-09-08 15:20:21.000000 fusionauth-client-1.8.0rc1/src/main/python/fusionauth/
--rw-r--r--   0 degroff    (501) staff       (20)      154 2019-06-13 17:49:02.000000 fusionauth-client-1.8.0rc1/src/main/python/fusionauth/__init__.py
--rw-r--r--   0 degroff    (501) staff       (20)    83293 2019-09-06 22:11:52.000000 fusionauth-client-1.8.0rc1/src/main/python/fusionauth/fusionauth_client.py
--rw-r--r--   0 degroff    (501) staff       (20)     5913 2018-10-30 01:56:13.000000 fusionauth-client-1.8.0rc1/src/main/python/fusionauth/rest_client.py
-drwxr-xr-x   0 degroff    (501) staff       (20)        0 2019-09-08 15:20:21.000000 fusionauth-client-1.8.0rc1/src/main/python/fusionauth_client.egg-info/
--rw-r--r--   0 degroff    (501) staff       (20)     2055 2019-09-08 15:20:21.000000 fusionauth-client-1.8.0rc1/src/main/python/fusionauth_client.egg-info/PKG-INFO
--rw-r--r--   0 degroff    (501) staff       (20)      497 2019-09-08 15:20:21.000000 fusionauth-client-1.8.0rc1/src/main/python/fusionauth_client.egg-info/SOURCES.txt
--rw-r--r--   0 degroff    (501) staff       (20)        1 2019-09-08 15:20:21.000000 fusionauth-client-1.8.0rc1/src/main/python/fusionauth_client.egg-info/dependency_links.txt
--rw-r--r--   0 degroff    (501) staff       (20)       11 2019-09-08 15:20:21.000000 fusionauth-client-1.8.0rc1/src/main/python/fusionauth_client.egg-info/namespace_packages.txt
--rw-r--r--   0 degroff    (501) staff       (20)        9 2019-09-08 15:20:21.000000 fusionauth-client-1.8.0rc1/src/main/python/fusionauth_client.egg-info/requires.txt
--rw-r--r--   0 degroff    (501) staff       (20)       11 2019-09-08 15:20:21.000000 fusionauth-client-1.8.0rc1/src/main/python/fusionauth_client.egg-info/top_level.txt
+drwxr-xr-x   0 degroff    (501) staff       (20)        0 2019-09-23 19:06:34.000000 fusionauth-client-1.9.0/
+-rw-r--r--   0 degroff    (501) staff       (20)     2052 2019-09-23 19:06:34.000000 fusionauth-client-1.9.0/PKG-INFO
+-rw-r--r--   0 degroff    (501) staff       (20)     1280 2018-10-30 02:11:50.000000 fusionauth-client-1.9.0/README.md
+-rw-r--r--   0 degroff    (501) staff       (20)       38 2019-09-23 19:06:34.000000 fusionauth-client-1.9.0/setup.cfg
+-rw-r--r--   0 degroff    (501) staff       (20)      863 2019-09-18 17:28:35.000000 fusionauth-client-1.9.0/setup.py
+drwxr-xr-x   0 degroff    (501) staff       (20)        0 2019-09-23 19:06:34.000000 fusionauth-client-1.9.0/src/
+drwxr-xr-x   0 degroff    (501) staff       (20)        0 2019-09-23 19:06:34.000000 fusionauth-client-1.9.0/src/main/
+drwxr-xr-x   0 degroff    (501) staff       (20)        0 2019-09-23 19:06:34.000000 fusionauth-client-1.9.0/src/main/python/
+drwxr-xr-x   0 degroff    (501) staff       (20)        0 2019-09-23 19:06:34.000000 fusionauth-client-1.9.0/src/main/python/fusionauth/
+-rw-r--r--   0 degroff    (501) staff       (20)      154 2019-06-13 17:49:02.000000 fusionauth-client-1.9.0/src/main/python/fusionauth/__init__.py
+-rw-r--r--   0 degroff    (501) staff       (20)    83301 2019-09-18 17:28:35.000000 fusionauth-client-1.9.0/src/main/python/fusionauth/fusionauth_client.py
+-rw-r--r--   0 degroff    (501) staff       (20)     5913 2018-10-30 01:56:13.000000 fusionauth-client-1.9.0/src/main/python/fusionauth/rest_client.py
+drwxr-xr-x   0 degroff    (501) staff       (20)        0 2019-09-23 19:06:34.000000 fusionauth-client-1.9.0/src/main/python/fusionauth_client.egg-info/
+-rw-r--r--   0 degroff    (501) staff       (20)     2052 2019-09-23 19:06:34.000000 fusionauth-client-1.9.0/src/main/python/fusionauth_client.egg-info/PKG-INFO
+-rw-r--r--   0 degroff    (501) staff       (20)      497 2019-09-23 19:06:34.000000 fusionauth-client-1.9.0/src/main/python/fusionauth_client.egg-info/SOURCES.txt
+-rw-r--r--   0 degroff    (501) staff       (20)        1 2019-09-23 19:06:34.000000 fusionauth-client-1.9.0/src/main/python/fusionauth_client.egg-info/dependency_links.txt
+-rw-r--r--   0 degroff    (501) staff       (20)       11 2019-09-23 19:06:34.000000 fusionauth-client-1.9.0/src/main/python/fusionauth_client.egg-info/namespace_packages.txt
+-rw-r--r--   0 degroff    (501) staff       (20)        9 2019-09-23 19:06:34.000000 fusionauth-client-1.9.0/src/main/python/fusionauth_client.egg-info/requires.txt
+-rw-r--r--   0 degroff    (501) staff       (20)       11 2019-09-23 19:06:34.000000 fusionauth-client-1.9.0/src/main/python/fusionauth_client.egg-info/top_level.txt
```

### Comparing `fusionauth-client-1.8.0rc1/PKG-INFO` & `fusionauth-client-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusionauth-client
-Version: 1.8.0rc1
+Version: 1.9.0
 Summary: A client library for FusionAuth
 Home-page: https://github.com/FusionAuth/fusionauth-python-client
 Author: Tyler Scott
 Author-email: tyler@inversoft.com
 License: UNKNOWN
 Description: ## FusionAuth Python Client ![semver 2.0.0 compliant](http://img.shields.io/badge/semver-2.0.0-brightgreen.svg?style=flat-square)
         If you're integrating FusionAuth with a Python 3 application, this library will speed up your development time.
```

### Comparing `fusionauth-client-1.8.0rc1/README.md` & `fusionauth-client-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `fusionauth-client-1.8.0rc1/setup.py` & `fusionauth-client-1.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="fusionauth-client",
-    version="1.8.0-RC.1",
+    version="1.9.0",
     author="Tyler Scott",
     author_email="tyler@inversoft.com",
     description="A client library for FusionAuth",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/FusionAuth/fusionauth-python-client",
     packages=find_packages(where='src/main/python'),
```

### Comparing `fusionauth-client-1.8.0rc1/src/main/python/fusionauth/fusionauth_client.py` & `fusionauth-client-1.9.0/src/main/python/fusionauth/fusionauth_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -739,15 +739,15 @@
         both the secret and a Base32 encoded form of the secret which can be shown to a User when using a 2 Step Authentication
         application such as Google Authenticator.
 
         Attributes:
             encoded_jwt: The encoded JWT (access token).
         """
         return self.start().uri('/api/two-factor/secret') \
-            .authorization("JWT " + encoded_jwt)
+            .authorization("JWT " + encoded_jwt) \
             .get() \
             .go()
 
     def identity_provider_login(self, request):
         """
         Handles login via third-parties including Social login, external OAuth and OpenID Connect, and other
         login systems.
@@ -798,15 +798,15 @@
         obtained a valid token from authentication.
 
         Attributes:
             application_id: The Application Id for which you are requesting a new access token be issued.
             encoded_jwt: The encoded JWT (access token).
         """
         return self.start().uri('/api/jwt/issue') \
-            .authorization("JWT " + encoded_jwt)
+            .authorization("JWT " + encoded_jwt) \
             .url_parameter('applicationId', application_id) \
             .get() \
             .go()
 
     def login(self, request):
         """
         Authenticates a user to FusionAuth. 
@@ -1820,15 +1820,15 @@
         """
         Retrieves the user for the given Id. This method does not use an API key, instead it uses a JSON Web Token (JWT) for authentication.
 
         Attributes:
             encoded_jwt: The encoded JWT (access token).
         """
         return self.start().uri('/api/user') \
-            .authorization("JWT " + encoded_jwt)
+            .authorization("JWT " + encoded_jwt) \
             .get() \
             .go()
 
     def retrieve_webhook(self, webhook_id):
         """
         Retrieves the webhook for the given Id. If you pass in null for the id, this will return all the webhooks.
 
@@ -2273,15 +2273,15 @@
         <p>
         This API may be used to verify the JWT as well as decode the encoded JWT into human readable identity claims.
 
         Attributes:
             encoded_jwt: The encoded JWT (access token).
         """
         return self.start().uri('/api/jwt/validate') \
-            .authorization("JWT " + encoded_jwt)
+            .authorization("JWT " + encoded_jwt) \
             .get() \
             .go()
 
     def verify_email(self, verification_id):
         """
         Confirms a email verification. The Id given is usually from an email sent to the user.
```

### Comparing `fusionauth-client-1.8.0rc1/src/main/python/fusionauth/rest_client.py` & `fusionauth-client-1.9.0/src/main/python/fusionauth/rest_client.py`

 * *Files identical despite different names*

### Comparing `fusionauth-client-1.8.0rc1/src/main/python/fusionauth_client.egg-info/PKG-INFO` & `fusionauth-client-1.9.0/src/main/python/fusionauth_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusionauth-client
-Version: 1.8.0rc1
+Version: 1.9.0
 Summary: A client library for FusionAuth
 Home-page: https://github.com/FusionAuth/fusionauth-python-client
 Author: Tyler Scott
 Author-email: tyler@inversoft.com
 License: UNKNOWN
 Description: ## FusionAuth Python Client ![semver 2.0.0 compliant](http://img.shields.io/badge/semver-2.0.0-brightgreen.svg?style=flat-square)
         If you're integrating FusionAuth with a Python 3 application, this library will speed up your development time.
```

