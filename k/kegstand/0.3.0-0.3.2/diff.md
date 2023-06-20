# Comparing `tmp/kegstand-0.3.0.tar.gz` & `tmp/kegstand-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kegstand-0.3.0.tar", max compression
+gzip compressed data, was "kegstand-0.3.2.tar", max compression
```

## Comparing `kegstand-0.3.0.tar` & `kegstand-0.3.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1077 2023-04-05 20:27:51.475886 kegstand-0.3.0/LICENSE
--rw-r--r--   0        0        0     1141 2023-04-29 19:34:52.696904 kegstand-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      394 2023-04-08 13:29:40.180072 kegstand-0.3.0/src/kegstand/__init__.py
--rw-r--r--   0        0        0     2086 2023-04-29 19:06:48.437560 kegstand-0.3.0/src/kegstand/api.py
--rw-r--r--   0        0        0     9928 2023-04-08 13:23:20.126106 kegstand-0.3.0/src/kegstand/decorators.py
--rw-r--r--   0        0        0     1255 2023-04-29 20:18:40.463405 kegstand-0.3.0/src/kegstand/utils.py
--rw-r--r--   0        0        0      783 1970-01-01 00:00:00.000000 kegstand-0.3.0/setup.py
--rw-r--r--   0        0        0     1045 1970-01-01 00:00:00.000000 kegstand-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-04-05 20:27:51.475886 kegstand-0.3.2/LICENSE
+-rw-r--r--   0        0        0     1141 2023-06-20 17:35:58.318307 kegstand-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      360 2023-06-20 17:35:04.354740 kegstand-0.3.2/src/kegstand/__init__.py
+-rw-r--r--   0        0        0     3246 2023-06-20 17:35:08.660812 kegstand-0.3.2/src/kegstand/api.py
+-rw-r--r--   0        0        0    10228 2023-06-20 17:35:12.274598 kegstand-0.3.2/src/kegstand/decorators.py
+-rw-r--r--   0        0        0     1891 2023-06-20 17:35:15.952831 kegstand-0.3.2/src/kegstand/utils.py
+-rw-r--r--   0        0        0      783 1970-01-01 00:00:00.000000 kegstand-0.3.2/setup.py
+-rw-r--r--   0        0        0     1045 1970-01-01 00:00:00.000000 kegstand-0.3.2/PKG-INFO
```

### Comparing `kegstand-0.3.0/LICENSE` & `kegstand-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kegstand-0.3.0/pyproject.toml` & `kegstand-0.3.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kegstand"
-version = "0.3.0"
+version = "0.3.2"
 description = "The Developer's Toolbelt For Accelerating Mean-Time-To-Party on AWS"
 authors = ["JensRoland <mail@jensroland.com>"]
 license = "MIT"
 repository = "https://github.com/jensroland/kegstand-framework-python"
 homepage = "https://kegstand.dev"
 #readme = "README.md"
 # Keywords description https://python-poetry.org/docs/pyproject/#keywords
```

### Comparing `kegstand-0.3.0/src/kegstand/api.py` & `kegstand-0.3.2/src/kegstand/api.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,49 +10,67 @@
 
 # Class RestApi provides a container for API resources and a method to add
 # resources to the API.
 class RestApi:
     def __init__(self, root: str = None):
         self.resources = []
         if root is not None:
-            source_path = os.path.dirname(os.path.abspath(root))
-            logger.info(f'Adding resources from {root} : source_path={source_path}')
+            # TODO: Check if this is api_src (correct) or api_src/api (incorrect, has to be the parent)
+            logger.info(f"Adding resources 1: {os.path.abspath(root)}")
+            logger.info(f"Adding resources 2: {os.path.dirname(os.path.abspath(root))}")
+            logger.info(f"Adding resources 3: {os.path.dirname(os.path.dirname(os.path.abspath(root)))}")
+            source_path = os.path.dirname(os.path.dirname(os.path.abspath(root)))
+            logger.info(f"Adding resources from {root} : source_path={source_path}")
             self.find_and_add_resources(source_path)
 
 
     def add_resource(self, resource):
         # Resource is a ApiResource object
         self.resources.append(resource)
 
 
     def find_and_add_resources(self, api_source_root: str):
         # Look through folder structure, importing and adding resources to the API.
         # Expects a folder structure like this:
         # api/
         #   [resource_name].py which exposes a resource object named `api`
+        # api/public/
+        #   [resource_name].py which exposes a resource object named `api`
         resource_module_folders = find_resource_modules(api_source_root)
+
+        # Output all modules found, each module contains:
+        logger.info("Kegstand framework: Found the following resource modules:")
+        for resource in resource_module_folders:
+            logger.info(f" - Name: {resource['name']}")
+            logger.info(f"   Module path: {resource['module_path']}")
+            logger.info(f"   Fromlist: {resource['fromlist']}")
+            logger.info(f"   Is public: {resource['is_public']}")
+
         for resource_module_folder in resource_module_folders:
             # Import the resource module
             resource_module = __import__(resource_module_folder['module_path'], fromlist=resource_module_folder['fromlist'])
             # Get the resource object from the module and add it to the API
             self.add_resource(getattr(resource_module, 'api'))
 
         return self.resources
 
 
     def export(self):
         # Export the API as a single Lambda-compatible handler function
         def handler(event, context):
+            logger.debug(f"event={event}")
+            logger.debug(f"context={context}")
             method = None
             for resource in self.resources:
-                if event['path'].startswith(resource.prefix):
-                    method, params = resource.get_matching_route(event['httpMethod'], event['path'])
+                if event["path"].startswith(resource.prefix):
+                    method, params = resource.get_matching_route(event["httpMethod"], event["path"])
                     if method is not None:
                         break
 
             if method is None:
-                return api_response({'error': 'Not found'}, 404)
+                logger.error(f'No matching route found for {event["httpMethod"]} {event["path"]}')
+                return api_response({"error": f"Not found: {event['httpMethod']} {event['path']}"}, 404)
 
             # Call the method's handler function
-            return method['handler'](params, event, context)
+            return method["handler"](params, event, context)
 
         return handler
```

### Comparing `kegstand-0.3.0/src/kegstand/decorators.py` & `kegstand-0.3.2/src/kegstand/decorators.py`

 * *Files 5% similar despite different names*

```diff
@@ -82,26 +82,31 @@
                     )
 
                 except ApiError as e:
                     return e.to_api_response()
 
                 return api_response(response, 200)
 
+            # Read auth configuration and add it to the method config object
+            auth_conditions = kwargs.get("auth", Auth())
+            if type(auth_conditions) is not list:
+                auth_conditions = [auth_conditions]
+
             self.methods.append({
                 'route': route,
                 'full_route': self.prefix + route,
                 'method': method,
-                'handler': wrapper
+                'handler': wrapper,
+                'auth': auth_conditions,
             })
 
             return wrapper
         
         return decorator
 
-
     def _call_func_with_arguments(self, method, func, params, **kwargs):
         # Calls different function signatures depending on different method types
         # and whether or not claims are present:
         #   - func()
         #   - func(params=params)
         #   - func(query=query)
         #   - func(params=params, query=query)
@@ -229,27 +234,27 @@
         claims = event['requestContext']['authorizer']['claims']
         for condition in self.conditions:
             if not condition(claims):
                 return False
         return True
 
 
-class PublicAccess(Auth):
-    def __init__(self):
-        Auth.__init__(self)
-        self.conditions.append(lambda claims: True)
-
-    def evaluate(self, _event):
-        return True
-
-    # Override all the Auth methods to raise an error
-    def __getattr__(self, name):
-        def method(*args, **kwargs):
-            raise Exception("Public access does not support claims")
-        return method
+# class PublicAccess(Auth):
+#     def __init__(self):
+#         Auth.__init__(self)
+#         self.conditions.append(lambda claims: True)
+
+#     def evaluate(self, _event):
+#         return True
+
+#     # Override all the Auth methods to raise an error
+#     def __getattr__(self, name):
+#         def method(*args, **kwargs):
+#             raise Exception("Public access does not support claims")
+#         return method
 
 
 def claim(claim_key):
     instance = Auth()
     return instance._claim(claim_key)
```

### Comparing `kegstand-0.3.0/setup.py` & `kegstand-0.3.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['aws-lambda-powertools[aws-sdk]>=2.10.0,<3.0.0', 'pyjwt>=2.1.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'kegstand',
-    'version': '0.3.0',
+    'version': '0.3.2',
     'description': "The Developer's Toolbelt For Accelerating Mean-Time-To-Party on AWS",
     'long_description': 'None',
     'author': 'JensRoland',
     'author_email': 'mail@jensroland.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://kegstand.dev',
```

### Comparing `kegstand-0.3.0/PKG-INFO` & `kegstand-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kegstand
-Version: 0.3.0
+Version: 0.3.2
 Summary: The Developer's Toolbelt For Accelerating Mean-Time-To-Party on AWS
 Home-page: https://kegstand.dev
 License: MIT
 Author: JensRoland
 Author-email: mail@jensroland.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

