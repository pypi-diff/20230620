# Comparing `tmp/d20-securityLayer-2.0.0a6.tar.gz` & `tmp/d20-securityLayer-2.0.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\d20\tools\libs\security_layer_python_arangodb\dist\.tmp-nbq7dyr7\d20-securityLayer-2.0.0a6.tar", last modified: Tue Jun 20 02:59:00 2023, max compression
+gzip compressed data, was "D:\d20\tools\libs\security_layer_python_arangodb\dist\.tmp-r12bei2s\d20-securityLayer-2.0.0a7.tar", last modified: Tue Jun 20 03:01:36 2023, max compression
```

## Comparing `d20-securityLayer-2.0.0a6.tar` & `d20-securityLayer-2.0.0a7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 02:59:00.135808 d20-securityLayer-2.0.0a6/
--rw-rw-rw-   0        0        0     1064 2021-09-22 23:30:22.000000 d20-securityLayer-2.0.0a6/LICENSE
--rw-rw-rw-   0        0        0      677 2023-06-20 02:59:00.133799 d20-securityLayer-2.0.0a6/PKG-INFO
--rw-rw-rw-   0        0        0      105 2021-06-18 21:41:10.000000 d20-securityLayer-2.0.0a6/README.md
--rw-rw-rw-   0        0        0      108 2021-09-22 23:14:25.000000 d20-securityLayer-2.0.0a6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-20 02:59:00.135808 d20-securityLayer-2.0.0a6/setup.cfg
--rw-rw-rw-   0        0        0      964 2023-06-20 02:58:44.000000 d20-securityLayer-2.0.0a6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-20 02:59:00.079534 d20-securityLayer-2.0.0a6/src/
-drwxrwxrwx   0        0        0        0 2023-06-20 02:59:00.104001 d20-securityLayer-2.0.0a6/src/d20_securityLayer.egg-info/
--rw-rw-rw-   0        0        0      677 2023-06-20 02:59:00.000000 d20-securityLayer-2.0.0a6/src/d20_securityLayer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      511 2023-06-20 02:59:00.000000 d20-securityLayer-2.0.0a6/src/d20_securityLayer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 02:59:00.000000 d20-securityLayer-2.0.0a6/src/d20_securityLayer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-06-20 02:59:00.000000 d20-securityLayer-2.0.0a6/src/d20_securityLayer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-20 02:59:00.000000 d20-securityLayer-2.0.0a6/src/d20_securityLayer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-20 02:59:00.132817 d20-securityLayer-2.0.0a6/src/securityLayer/
--rw-rw-rw-   0        0        0    10081 2023-05-12 01:22:57.000000 d20-securityLayer-2.0.0a6/src/securityLayer/AccessControl.py
--rw-rw-rw-   0        0        0      233 2023-05-16 00:25:53.000000 d20-securityLayer-2.0.0a6/src/securityLayer/AuthAnswer.py
--rw-rw-rw-   0        0        0     9697 2023-05-16 02:42:02.000000 d20-securityLayer-2.0.0a6/src/securityLayer/Error.py
--rw-rw-rw-   0        0        0    16797 2023-06-07 23:54:37.000000 d20-securityLayer-2.0.0a6/src/securityLayer/SSO.py
--rw-rw-rw-   0        0        0    15246 2023-06-20 02:58:26.000000 d20-securityLayer-2.0.0a6/src/securityLayer/SecurityLayer.py
--rw-rw-rw-   0        0        0      125 2023-01-02 23:20:55.000000 d20-securityLayer-2.0.0a6/src/securityLayer/__init__.py
--rw-rw-rw-   0        0        0      156 2023-06-20 02:58:40.000000 d20-securityLayer-2.0.0a6/src/securityLayer/__version__.py
--rw-rw-rw-   0        0        0       55 2021-09-23 23:27:01.000000 d20-securityLayer-2.0.0a6/src/securityLayer/default.py
+drwxrwxrwx   0        0        0        0 2023-06-20 03:01:36.468690 d20-securityLayer-2.0.0a7/
+-rw-rw-rw-   0        0        0     1064 2021-09-22 23:30:22.000000 d20-securityLayer-2.0.0a7/LICENSE
+-rw-rw-rw-   0        0        0      677 2023-06-20 03:01:36.467689 d20-securityLayer-2.0.0a7/PKG-INFO
+-rw-rw-rw-   0        0        0      105 2021-06-18 21:41:10.000000 d20-securityLayer-2.0.0a7/README.md
+-rw-rw-rw-   0        0        0      108 2021-09-22 23:14:25.000000 d20-securityLayer-2.0.0a7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-20 03:01:36.468690 d20-securityLayer-2.0.0a7/setup.cfg
+-rw-rw-rw-   0        0        0      964 2023-06-20 03:01:17.000000 d20-securityLayer-2.0.0a7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 03:01:36.407952 d20-securityLayer-2.0.0a7/src/
+drwxrwxrwx   0        0        0        0 2023-06-20 03:01:36.437120 d20-securityLayer-2.0.0a7/src/d20_securityLayer.egg-info/
+-rw-rw-rw-   0        0        0      677 2023-06-20 03:01:36.000000 d20-securityLayer-2.0.0a7/src/d20_securityLayer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      511 2023-06-20 03:01:36.000000 d20-securityLayer-2.0.0a7/src/d20_securityLayer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 03:01:36.000000 d20-securityLayer-2.0.0a7/src/d20_securityLayer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-06-20 03:01:36.000000 d20-securityLayer-2.0.0a7/src/d20_securityLayer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-20 03:01:36.000000 d20-securityLayer-2.0.0a7/src/d20_securityLayer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 03:01:36.466689 d20-securityLayer-2.0.0a7/src/securityLayer/
+-rw-rw-rw-   0        0        0    10081 2023-05-12 01:22:57.000000 d20-securityLayer-2.0.0a7/src/securityLayer/AccessControl.py
+-rw-rw-rw-   0        0        0      233 2023-05-16 00:25:53.000000 d20-securityLayer-2.0.0a7/src/securityLayer/AuthAnswer.py
+-rw-rw-rw-   0        0        0     9697 2023-05-16 02:42:02.000000 d20-securityLayer-2.0.0a7/src/securityLayer/Error.py
+-rw-rw-rw-   0        0        0    16797 2023-06-07 23:54:37.000000 d20-securityLayer-2.0.0a7/src/securityLayer/SSO.py
+-rw-rw-rw-   0        0        0    15275 2023-06-20 03:01:13.000000 d20-securityLayer-2.0.0a7/src/securityLayer/SecurityLayer.py
+-rw-rw-rw-   0        0        0      125 2023-01-02 23:20:55.000000 d20-securityLayer-2.0.0a7/src/securityLayer/__init__.py
+-rw-rw-rw-   0        0        0      156 2023-06-20 03:01:19.000000 d20-securityLayer-2.0.0a7/src/securityLayer/__version__.py
+-rw-rw-rw-   0        0        0       55 2021-09-23 23:27:01.000000 d20-securityLayer-2.0.0a7/src/securityLayer/default.py
```

### Comparing `d20-securityLayer-2.0.0a6/LICENSE` & `d20-securityLayer-2.0.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `d20-securityLayer-2.0.0a6/PKG-INFO` & `d20-securityLayer-2.0.0a7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: d20-securityLayer
-Version: 2.0.0a6
+Version: 2.0.0a7
 Summary: A simple access manager
 Home-page: https://github.com/d20services/security_layer_python_arangodb
 Author: Alex Sánchez Vega
 Author-email: alex@d20.services
 Project-URL: Bug Tracker, https://github.com/d20services/security_layer_python_arangodb/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `d20-securityLayer-2.0.0a6/setup.py` & `d20-securityLayer-2.0.0a7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="d20-securityLayer",
-    version="2.0.0a6",
+    version="2.0.0a7",
     author="Alex Sánchez Vega",
     author_email="alex@d20.services",
     description="A simple access manager",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/d20services/security_layer_python_arangodb",
     project_urls={
```

### Comparing `d20-securityLayer-2.0.0a6/src/d20_securityLayer.egg-info/PKG-INFO` & `d20-securityLayer-2.0.0a7/src/d20_securityLayer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: d20-securityLayer
-Version: 2.0.0a6
+Version: 2.0.0a7
 Summary: A simple access manager
 Home-page: https://github.com/d20services/security_layer_python_arangodb
 Author: Alex Sánchez Vega
 Author-email: alex@d20.services
 Project-URL: Bug Tracker, https://github.com/d20services/security_layer_python_arangodb/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `d20-securityLayer-2.0.0a6/src/securityLayer/AccessControl.py` & `d20-securityLayer-2.0.0a7/src/securityLayer/AccessControl.py`

 * *Files identical despite different names*

### Comparing `d20-securityLayer-2.0.0a6/src/securityLayer/Error.py` & `d20-securityLayer-2.0.0a7/src/securityLayer/Error.py`

 * *Files identical despite different names*

### Comparing `d20-securityLayer-2.0.0a6/src/securityLayer/SSO.py` & `d20-securityLayer-2.0.0a7/src/securityLayer/SSO.py`

 * *Files identical despite different names*

### Comparing `d20-securityLayer-2.0.0a6/src/securityLayer/SecurityLayer.py` & `d20-securityLayer-2.0.0a7/src/securityLayer/SecurityLayer.py`

 * *Files 0% similar despite different names*

```diff
@@ -315,15 +315,15 @@
             
         def verify_password(self):
             try:
                 self.load(self.get('username'))
             except:
                 query = [{"dim":"username", 'op':'==', 'val': self.get('username')}]
                 self.search(query_list=query)
-                self.set(data=self.found[0])
+                self.set(id=self.found[0].get('_key'),data=self.found[0])
             stored_password = self.get("password")
             self.id = self.get("_key")
             salt = stored_password[:64]
             stored_password = stored_password[64:]
             pwdhash = hashlib.pbkdf2_hmac('sha512', 
                                         self.get('password').encode('utf-8'), 
                                         salt.encode('ascii'),
```

