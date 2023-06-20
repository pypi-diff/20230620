# Comparing `tmp/scratchcommunication-1.0.0.tar.gz` & `tmp/scratchcommunication-1.0.1.tar.gz`

## Comparing `scratchcommunication-1.0.0.tar` & `scratchcommunication-1.0.1.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 scratchcommunication-1.0.0/scratchcommunication/__init__.py
--rw-r--r--   0        0        0     9515 2020-02-02 00:00:00.000000 scratchcommunication-1.0.0/scratchcommunication/cloud.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 scratchcommunication-1.0.0/scratchcommunication/exceptions.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 scratchcommunication-1.0.0/scratchcommunication/headers.py
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 scratchcommunication-1.0.0/scratchcommunication/session.py
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 scratchcommunication-1.0.0/LICENSE
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 scratchcommunication-1.0.0/README.md
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 scratchcommunication-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 scratchcommunication-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 scratchcommunication-1.0.1/Pipfile
+-rw-r--r--   0        0        0    29429 2020-02-02 00:00:00.000000 scratchcommunication-1.0.1/Pipfile.lock
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 scratchcommunication-1.0.1/scratchcommunication/__init__.py
+-rw-r--r--   0        0        0     9515 2020-02-02 00:00:00.000000 scratchcommunication-1.0.1/scratchcommunication/cloud.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 scratchcommunication-1.0.1/scratchcommunication/exceptions.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 scratchcommunication-1.0.1/scratchcommunication/headers.py
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 scratchcommunication-1.0.1/scratchcommunication/session.py
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 scratchcommunication-1.0.1/LICENSE
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 scratchcommunication-1.0.1/README.md
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 scratchcommunication-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 scratchcommunication-1.0.1/PKG-INFO
```

### Comparing `scratchcommunication-1.0.0/scratchcommunication/cloud.py` & `scratchcommunication-1.0.1/scratchcommunication/cloud.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-1.0.0/scratchcommunication/session.py` & `scratchcommunication-1.0.1/scratchcommunication/session.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 import warnings
 from .headers import headers
 from .exceptions import InvalidValueError
+from . import cloud
 import requests, json, re
 
 class Session:
     def __init__(self, username : str = None, *, session_id : str):
         self.session_id = session_id
         self.username = username
         self.headers = headers
         self._login()
-    def _login(self) -> None:
+    def _login(self):
+        '''
+        Don't use this
+        '''
         self.cookies = {
             "scratchcsrftoken" : "a",
             "scratchlanguage" : "en",
             "scratchpolicyseen": "true",
             "scratchsessionsid" : self.session_id,
             "accept": "application/json",
             "Content-Type": "application/json",
@@ -23,14 +27,17 @@
             "scratchcsrftoken": "a",
             "scratchlanguage": "en",
         }).json()
         self.xtoken = account["user"]["token"]
         self.headers["X-Token"] = self.xtoken
     @classmethod
     def login(cls, username : str, password : str):
+        '''
+        Login from your username and password.
+        '''
         try:
             return cls(
                 username, session_id=str(re.search('"(.*)"', requests.post(
                     "https://scratch.mit.edu/login/",
                     data=json.dumps({
                         "username": username,
                         "password": password
@@ -40,11 +47,14 @@
                         "scratchcsrftoken": "a",
                         "scratchlanguage": "en"
                     }
                 ).headers["Set-Cookie"]).group())
             )
         except AttributeError:
             raise InvalidValueError("Your login was wrong")
-        except:
-            raise Exception("An error occurred while trying to log in.")
-    def create_cloudrequests_server(self, project_id : int, thread : bool = True):
-        project_id = 1
+        except Exception as e:
+            raise Exception("An error occurred while trying to log in.") from e
+    def create_cloudconnection(self, project_id : int, **kwargs) -> cloud.CloudConnection:
+        '''
+        Create a cloud connection to a project.
+        '''
+        return cloud.CloudConnection(project_id=project_id, session=self, **kwargs)
```

### Comparing `scratchcommunication-1.0.0/LICENSE` & `scratchcommunication-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scratchcommunication-1.0.0/pyproject.toml` & `scratchcommunication-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "scratchcommunication"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Simon Gilde", email="simon.c.gilde@gmail.com" },
 ]
 description = "A python module for communicating with scratch projects"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `scratchcommunication-1.0.0/PKG-INFO` & `scratchcommunication-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchcommunication
-Version: 1.0.0
+Version: 1.0.1
 Summary: A python module for communicating with scratch projects
 Project-URL: Homepage, https://github.com/thecommcraft/scratchcommunication
 Project-URL: Bug Tracker, https://github.com/thecommcraft/scratchcommunication/issues
 Author-email: Simon Gilde <simon.c.gilde@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

