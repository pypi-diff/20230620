# Comparing `tmp/zoom_python-0.1.0.tar.gz` & `tmp/zoom_python-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zoom_python-0.1.0.tar", max compression
+gzip compressed data, was "zoom_python-0.1.1.tar", max compression
```

## Comparing `zoom_python-0.1.0.tar` & `zoom_python-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1065 2023-06-02 13:51:23.092062 zoom_python-0.1.0/LICENSE
--rw-r--r--   0        0        0     2660 2023-06-02 13:51:23.092172 zoom_python-0.1.0/README.md
--rw-r--r--   0        0        0      384 2023-06-02 13:51:23.092267 zoom_python-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-02 13:51:23.092351 zoom_python-0.1.0/zoom/__init__.py
--rw-r--r--   0        0        0     6058 2023-06-02 13:51:23.092501 zoom_python-0.1.0/zoom/client.py
--rw-r--r--   0        0        0      190 2023-06-02 13:51:23.092581 zoom_python-0.1.0/zoom/exceptions.py
--rw-r--r--   0        0        0     3300 1970-01-01 00:00:00.000000 zoom_python-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-02 13:51:23.092062 zoom_python-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2818 2023-06-20 17:51:19.438019 zoom_python-0.1.1/README.md
+-rw-r--r--   0        0        0      384 2023-06-20 17:51:19.438211 zoom_python-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-02 13:51:23.092351 zoom_python-0.1.1/zoom/__init__.py
+-rw-r--r--   0        0        0     6227 2023-06-20 17:51:19.438418 zoom_python-0.1.1/zoom/client.py
+-rw-r--r--   0        0        0      190 2023-06-02 13:51:23.092581 zoom_python-0.1.1/zoom/exceptions.py
+-rw-r--r--   0        0        0     3458 1970-01-01 00:00:00.000000 zoom_python-0.1.1/PKG-INFO
```

### Comparing `zoom_python-0.1.0/LICENSE` & `zoom_python-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zoom_python-0.1.0/README.md` & `zoom_python-0.1.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 
 # zoom-python
-![](https://img.shields.io/badge/version-0.1.0-success) ![](https://img.shields.io/badge/Python-3.8%20|%203.9%20|%203.10%20|%203.11-4B8BBE?logo=python&logoColor=white)  
+![](https://img.shields.io/badge/version-0.1.1-success) ![](https://img.shields.io/badge/Python-3.8%20|%203.9%20|%203.10%20|%203.11-4B8BBE?logo=python&logoColor=white)  
 
 *zoom-python* is an API wrapper for Zoom, written in Python.  
 This library uses Oauth2 for authentication.
 ## Installing
 ```
 pip install zoom-python
 ```
 ### Usage
 ```python
 from zoom.client import Client
-client = Client(client_id, client_secret)
+client = Client(client_id, client_secret, redirect_uri=None)
 ```
 To obtain and set an access token, follow this instructions:
 1. **Get authorization URL**
 ```python
-url = client.authorization_url(redirect_uri)
+url = client.authorization_url(code_challenge, redirect_uri=None, state=None)
+# redirect_uri required if not given in Client.
 ```
 2. **Get access token using code**
 ```python
-response = client.get_access_token(code)
+response = client.get_access_token(code, code_verifier)
+# code_verifier is the same code_challenge
 ```
 3. **Set access token**
 ```python
 client.set_token(access_token)
 ```
 If your access token expired, you can get a new one using refresh token:
 ```python
```

### Comparing `zoom_python-0.1.0/zoom/client.py` & `zoom_python-0.1.1/zoom/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,29 +13,39 @@
     headers = {"Content-Type": "application/json", "Accept": "application/json"}
 
     def __init__(self, client_id=None, client_secret=None, redirect_uri=None):
         self.CLIENT_ID = client_id
         self.CLIENT_SECRET = client_secret
         self.REDIRECT_URI = redirect_uri
 
-    def authorization_url(self, redirect_uri=None, state=None):
+    def authorization_url(self, code_challenge, redirect_uri=None, state=None):
         if redirect_uri is not None:
             self.REDIRECT_URI = redirect_uri
-        params = {"client_id": self.CLIENT_ID, "redirect_uri": self.REDIRECT_URI, "response_type": "code"}
+        params = {
+            "client_id": self.CLIENT_ID,
+            "redirect_uri": self.REDIRECT_URI,
+            "response_type": "code",
+            "code_challenge": code_challenge,
+        }
         if state:
             params["state"] = state
         return self.AUTH_URL + "authorize?" + urlencode(params)
 
     def auth_headers(self):
         encoded_credentials = base64.b64encode(f"{self.CLIENT_ID}:{self.CLIENT_SECRET}".encode("utf-8")).decode("utf-8")
         self.headers["Authorization"] = f"Basic {encoded_credentials}"
         self.headers["Content-Type"] = "application/x-www-form-urlencoded"
 
-    def get_access_token(self, code):
-        body = {"code": code, "grant_type": "authorization_code", "redirect_uri": self.REDIRECT_URI}
+    def get_access_token(self, code, code_verifier):
+        body = {
+            "code": code,
+            "grant_type": "authorization_code",
+            "redirect_uri": self.REDIRECT_URI,
+            "code_verifier": code_verifier,
+        }
         self.auth_headers()
         return self.post("token", auth_url=True, data=body)
 
     def refresh_access_token(self, refresh_token):
         body = {"refresh_token": refresh_token, "grant_type": "refresh_token"}
         self.auth_headers()
         return self.post("token", auth_url=True, data=body)
@@ -93,16 +103,14 @@
         no_of_employees: str = None,
         purchasing_time_frame: str = None,
         role_in_purchase_process: str = None,
         language: str = None,
         auto_approve: bool = None,
     ):
         args = locals()
-        print(type(args))
-        print(args)
         body = self.set_form_data(args)
         return self.post(f"meetings/{meeting_id}/registrants", data=json.dumps(body))
 
     def add_webinar_registrant(
         self,
         webinar_id,
         email: str,
```

### Comparing `zoom_python-0.1.0/PKG-INFO` & `zoom_python-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zoom-python
-Version: 0.1.0
+Version: 0.1.1
 Summary: API wrapper for Zoom written in Python
 License: MIT
 Author: Juan Carlos Rios
 Author-email: juankrios15@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -14,35 +14,37 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: requests (>=2.26.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 
 # zoom-python
-![](https://img.shields.io/badge/version-0.1.0-success) ![](https://img.shields.io/badge/Python-3.8%20|%203.9%20|%203.10%20|%203.11-4B8BBE?logo=python&logoColor=white)  
+![](https://img.shields.io/badge/version-0.1.1-success) ![](https://img.shields.io/badge/Python-3.8%20|%203.9%20|%203.10%20|%203.11-4B8BBE?logo=python&logoColor=white)  
 
 *zoom-python* is an API wrapper for Zoom, written in Python.  
 This library uses Oauth2 for authentication.
 ## Installing
 ```
 pip install zoom-python
 ```
 ### Usage
 ```python
 from zoom.client import Client
-client = Client(client_id, client_secret)
+client = Client(client_id, client_secret, redirect_uri=None)
 ```
 To obtain and set an access token, follow this instructions:
 1. **Get authorization URL**
 ```python
-url = client.authorization_url(redirect_uri)
+url = client.authorization_url(code_challenge, redirect_uri=None, state=None)
+# redirect_uri required if not given in Client.
 ```
 2. **Get access token using code**
 ```python
-response = client.get_access_token(code)
+response = client.get_access_token(code, code_verifier)
+# code_verifier is the same code_challenge
 ```
 3. **Set access token**
 ```python
 client.set_token(access_token)
 ```
 If your access token expired, you can get a new one using refresh token:
 ```python
```

