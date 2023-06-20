# Comparing `tmp/kegstand-0.3.2.tar.gz` & `tmp/kegstand-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kegstand-0.3.2.tar", max compression
+gzip compressed data, was "kegstand-0.3.3.tar", max compression
```

## Comparing `kegstand-0.3.2.tar` & `kegstand-0.3.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1077 2023-04-05 20:27:51.475886 kegstand-0.3.2/LICENSE
--rw-r--r--   0        0        0     1141 2023-06-20 17:35:58.318307 kegstand-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      360 2023-06-20 17:35:04.354740 kegstand-0.3.2/src/kegstand/__init__.py
--rw-r--r--   0        0        0     3246 2023-06-20 17:35:08.660812 kegstand-0.3.2/src/kegstand/api.py
--rw-r--r--   0        0        0    10228 2023-06-20 17:35:12.274598 kegstand-0.3.2/src/kegstand/decorators.py
--rw-r--r--   0        0        0     1891 2023-06-20 17:35:15.952831 kegstand-0.3.2/src/kegstand/utils.py
--rw-r--r--   0        0        0      783 1970-01-01 00:00:00.000000 kegstand-0.3.2/setup.py
--rw-r--r--   0        0        0     1045 1970-01-01 00:00:00.000000 kegstand-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-04-05 20:27:51.475886 kegstand-0.3.3/LICENSE
+-rw-r--r--   0        0        0     1141 2023-06-20 21:56:47.295159 kegstand-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      360 2023-06-20 17:35:04.354740 kegstand-0.3.3/src/kegstand/__init__.py
+-rw-r--r--   0        0        0     2831 2023-06-20 21:47:15.563797 kegstand-0.3.3/src/kegstand/api.py
+-rw-r--r--   0        0        0     9982 2023-06-20 21:54:06.742326 kegstand-0.3.3/src/kegstand/decorators.py
+-rw-r--r--   0        0        0     1891 2023-06-20 17:35:15.952831 kegstand-0.3.3/src/kegstand/utils.py
+-rw-r--r--   0        0        0      783 1970-01-01 00:00:00.000000 kegstand-0.3.3/setup.py
+-rw-r--r--   0        0        0     1045 1970-01-01 00:00:00.000000 kegstand-0.3.3/PKG-INFO
```

### Comparing `kegstand-0.3.2/LICENSE` & `kegstand-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kegstand-0.3.2/pyproject.toml` & `kegstand-0.3.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kegstand"
-version = "0.3.2"
+version = "0.3.3"
 description = "The Developer's Toolbelt For Accelerating Mean-Time-To-Party on AWS"
 authors = ["JensRoland <mail@jensroland.com>"]
 license = "MIT"
 repository = "https://github.com/jensroland/kegstand-framework-python"
 homepage = "https://kegstand.dev"
 #readme = "README.md"
 # Keywords description https://python-poetry.org/docs/pyproject/#keywords
```

### Comparing `kegstand-0.3.2/src/kegstand/api.py` & `kegstand-0.3.3/src/kegstand/api.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,18 +10,14 @@
 
 # Class RestApi provides a container for API resources and a method to add
 # resources to the API.
 class RestApi:
     def __init__(self, root: str = None):
         self.resources = []
         if root is not None:
-            # TODO: Check if this is api_src (correct) or api_src/api (incorrect, has to be the parent)
-            logger.info(f"Adding resources 1: {os.path.abspath(root)}")
-            logger.info(f"Adding resources 2: {os.path.dirname(os.path.abspath(root))}")
-            logger.info(f"Adding resources 3: {os.path.dirname(os.path.dirname(os.path.abspath(root)))}")
             source_path = os.path.dirname(os.path.dirname(os.path.abspath(root)))
             logger.info(f"Adding resources from {root} : source_path={source_path}")
             self.find_and_add_resources(source_path)
 
 
     def add_resource(self, resource):
         # Resource is a ApiResource object
@@ -33,22 +29,14 @@
         # Expects a folder structure like this:
         # api/
         #   [resource_name].py which exposes a resource object named `api`
         # api/public/
         #   [resource_name].py which exposes a resource object named `api`
         resource_module_folders = find_resource_modules(api_source_root)
 
-        # Output all modules found, each module contains:
-        logger.info("Kegstand framework: Found the following resource modules:")
-        for resource in resource_module_folders:
-            logger.info(f" - Name: {resource['name']}")
-            logger.info(f"   Module path: {resource['module_path']}")
-            logger.info(f"   Fromlist: {resource['fromlist']}")
-            logger.info(f"   Is public: {resource['is_public']}")
-
         for resource_module_folder in resource_module_folders:
             # Import the resource module
             resource_module = __import__(resource_module_folder['module_path'], fromlist=resource_module_folder['fromlist'])
             # Get the resource object from the module and add it to the API
             self.add_resource(getattr(resource_module, 'api'))
 
         return self.resources
@@ -63,14 +51,21 @@
             for resource in self.resources:
                 if event["path"].startswith(resource.prefix):
                     method, params = resource.get_matching_route(event["httpMethod"], event["path"])
                     if method is not None:
                         break
 
             if method is None:
-                logger.error(f'No matching route found for {event["httpMethod"]} {event["path"]}')
+                logger.error(f"No matching route found for {event['httpMethod']} {event['path']}")
                 return api_response({"error": f"Not found: {event['httpMethod']} {event['path']}"}, 404)
 
+            # Check if the method is public and if not, check that the user is authenticated
+            if not method["is_public"]:
+                # Check that the user is authenticated
+                if "authorizer" not in event["requestContext"]:
+                    logger.error("User is not authenticated")
+                    return api_response({"error": f"User is not authenticated"}, 401)
+
             # Call the method's handler function
             return method["handler"](params, event, context)
 
         return handler
```

### Comparing `kegstand-0.3.2/src/kegstand/decorators.py` & `kegstand-0.3.3/src/kegstand/decorators.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,66 +14,66 @@
 # resource's base prefix.
 class ApiResource:
     def __init__(self, prefix: str, method_defaults: dict = None):
         self.prefix = prefix
         self.methods = []
         self.method_defaults = method_defaults or {}
 
-    def get(self, route: str = '/', **kwargs):
-        return self._method_decorator('GET', route, **{**self.method_defaults, **kwargs})
+    def get(self, route: str = "/", **kwargs):
+        return self._method_decorator("GET", route, **{**self.method_defaults, **kwargs})
 
-    def post(self, route: str = '/', **kwargs):
-        return self._method_decorator('POST', route, **{**self.method_defaults, **kwargs})
+    def post(self, route: str = "/", **kwargs):
+        return self._method_decorator("POST", route, **{**self.method_defaults, **kwargs})
 
-    def put(self, route: str = '/', **kwargs):
-        return self._method_decorator('PUT', route, **{**self.method_defaults, **kwargs})
+    def put(self, route: str = "/", **kwargs):
+        return self._method_decorator("PUT", route, **{**self.method_defaults, **kwargs})
 
-    def delete(self, route: str = '/', **kwargs):
-        return self._method_decorator('DELETE', route, **{**self.method_defaults, **kwargs})
+    def delete(self, route: str = "/", **kwargs):
+        return self._method_decorator("DELETE", route, **{**self.method_defaults, **kwargs})
 
     # Route contains the path to the resource method, relative to the resource's prefix
     # and may include dynamic segments (e.g. `/:id`).
     def _method_decorator(self, method: str, route: str, **kwargs):
         def decorator(func):
             @wraps(func)
             def wrapper(params, event, context):
-                if event['httpMethod'] != method:
-                    return api_response({'error': f'Method not allowed for prefix {self.prefix}'}, 405)
+                if event["httpMethod"] != method:
+                    return api_response({"error": f"Method not allowed for prefix {self.prefix}"}, 405)
 
                 try:
-                    data = json.loads(event['body']) if event['body'] else {}
+                    data = json.loads(event["body"]) if event["body"] else {}
                 except json.JSONDecodeError:
-                    return api_response({'error': 'Invalid JSON data provided'}, 400)
+                    return api_response({"error": "Invalid JSON data provided"}, 400)
 
                 try:
                     # Authorization
                     # Defaults to checking for a valid requestContext
                     auth_conditions = kwargs.get("auth", Auth())
                     if type(auth_conditions) is not list:
                         auth_conditions = [auth_conditions]
 
                     # Validate each auth condition
                     for auth_condition in auth_conditions:
                         if not auth_condition.evaluate(event):
-                            return api_response({'error': 'Unauthorized'}, 401)
+                            return api_response({"error": "Unauthorized"}, 401)
 
-                    # If the func has a 'claims' argument, then we have to pass
+                    # If the func has a "claims" argument, then we have to pass
                     # in the authorized user properties (claims) from the authorizer
                     claims = None
-                    if 'claims' in inspect.signature(func).parameters:
-                        if 'authorizer' not in event['requestContext']:
-                            return api_response({'error': 'Unauthorized (missing authorizer context)'}, 401)
-                        claims = event['requestContext']['authorizer']['claims']
+                    if "claims" in inspect.signature(func).parameters:
+                        if "authorizer" not in event["requestContext"] or "claims" not in event["requestContext"]["authorizer"]:
+                            return api_response({"error": "Unauthorized (missing authorizer context)"}, 401)
+                        claims = event["requestContext"]["authorizer"]["claims"]
 
                     # Other injected arguments
-                    # If the func has a 'query' argument, then we have to pass
+                    # If the func has a "query" argument, then we have to pass
                     # in the query string parameters from the event
                     query = None
-                    if 'query' in inspect.signature(func).parameters:
-                        query = event['queryStringParameters'] or {}
+                    if "query" in inspect.signature(func).parameters:
+                        query = event["queryStringParameters"] or {}
 
                     # Call the function with the authorized user properties
                     response = self._call_func_with_arguments(
                         method,
                         func,
                         params,
                         query=query,
@@ -88,19 +88,19 @@
 
             # Read auth configuration and add it to the method config object
             auth_conditions = kwargs.get("auth", Auth())
             if type(auth_conditions) is not list:
                 auth_conditions = [auth_conditions]
 
             self.methods.append({
-                'route': route,
-                'full_route': self.prefix + route,
-                'method': method,
-                'handler': wrapper,
-                'auth': auth_conditions,
+                "route": route,
+                "full_route": self.prefix + route,
+                "method": method,
+                "handler": wrapper,
+                "auth": auth_conditions,
             })
 
             return wrapper
         
         return decorator
 
     def _call_func_with_arguments(self, method, func, params, **kwargs):
@@ -115,24 +115,24 @@
         #   - func(params=params, query=query, data=data, claims=claims)
         #   - etc.
         #
         # May raise ApiError
         func_kwargs = {}
         if len(params) > 0:
             func_kwargs["params"] = params
-        if method in ['POST', 'PUT', 'PATCH']:
-            func_kwargs["data"] = kwargs.get('data', {})
+        if method in ["POST", "PUT", "PATCH"]:
+            func_kwargs["data"] = kwargs.get("data", {})
 
-        # Add querystring parameters if a 'query' parameter was passed in
-        query = kwargs.get('query', None)
+        # Add querystring parameters if a "query" parameter was passed in
+        query = kwargs.get("query", None)
         if query is not None:
             func_kwargs["query"] = query
 
-        # Add authorized user properties (claims) if a 'claims' parameter was passed in
-        claims = kwargs.get('claims', None)
+        # Add authorized user properties (claims) if a "claims" parameter was passed in
+        claims = kwargs.get("claims", None)
         if claims is not None:
             func_kwargs["claims"] = claims
 
         return func(**func_kwargs)
 
 
     def get_matching_route(self, httpMethod: str, request_uri: str):
@@ -142,38 +142,38 @@
                 return method, params
         
         return None, None
 
 
     def _route_matcher(self, httpMethod, request_uri, method):
         # If the method doesn't match, the routes don't match
-        if httpMethod != method['method']:
+        if httpMethod != method["method"]:
             return None
         
         # Split the request_uri into segments
         # Remove trailing slash if present (/hello/world/ -> /hello/world)
-        if request_uri.endswith('/'):
+        if request_uri.endswith("/"):
             request_uri = request_uri[:-1]
-        segments = request_uri.split('/')
+        segments = request_uri.split("/")
 
         # And same for the method's full route
-        method_route = method['full_route']
-        if method_route.endswith('/'):
+        method_route = method["full_route"]
+        if method_route.endswith("/"):
             method_route = method_route[:-1]
-        method_segments = method_route.split('/')
+        method_segments = method_route.split("/")
 
         # If the number of segments doesn't match, the routes don't match
         if len(segments) != len(method_segments):
             return None
 
         # Loop through the segments and compare them
         route_params = {}
         for i in range(len(segments)):
             # If the segment is a dynamic segment, it matches
-            if method_segments[i].startswith(':'):
+            if method_segments[i].startswith(":"):
                 route_params[method_segments[i][1:]] = unquote_plus(segments[i])
                 continue
 
             # If the segment doesn't match, the routes don't match
             if segments[i] != method_segments[i]:
                 return None
 
@@ -225,50 +225,38 @@
         return self
 
     def not_in_collection(self, collection):
         self.conditions.append(lambda claims: claims.get(self.current_claim, None) not in collection)
         return self
 
     def evaluate(self, event):
-        if 'authorizer' not in event['requestContext']:
+        if len(self.conditions) == 0:
+            return True
+
+        if "authorizer" not in event["requestContext"] or "claims" not in event["requestContext"]["authorizer"]:
             return False
-        claims = event['requestContext']['authorizer']['claims']
+        claims = event["requestContext"]["authorizer"]["claims"]
         for condition in self.conditions:
             if not condition(claims):
                 return False
         return True
 
 
-# class PublicAccess(Auth):
-#     def __init__(self):
-#         Auth.__init__(self)
-#         self.conditions.append(lambda claims: True)
-
-#     def evaluate(self, _event):
-#         return True
-
-#     # Override all the Auth methods to raise an error
-#     def __getattr__(self, name):
-#         def method(*args, **kwargs):
-#             raise Exception("Public access does not support claims")
-#         return method
-
-
 def claim(claim_key):
     instance = Auth()
     return instance._claim(claim_key)
 
 
 class ApiError(Exception):
     def __init__(self, error_message, status_code: int = 400):
         Exception.__init__(self)
         self.error_message = error_message
         self.status_code = status_code
         logger.warning(f"API Error (status {status_code}): {error_message}")
 
     def to_dict(self):
         rv = dict()
-        rv['error'] = self.error_message
+        rv["error"] = self.error_message
         return rv
 
     def to_api_response(self):
         return api_response(self.to_dict(), self.status_code)
```

### Comparing `kegstand-0.3.2/src/kegstand/utils.py` & `kegstand-0.3.3/src/kegstand/utils.py`

 * *Files identical despite different names*

### Comparing `kegstand-0.3.2/setup.py` & `kegstand-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['aws-lambda-powertools[aws-sdk]>=2.10.0,<3.0.0', 'pyjwt>=2.1.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'kegstand',
-    'version': '0.3.2',
+    'version': '0.3.3',
     'description': "The Developer's Toolbelt For Accelerating Mean-Time-To-Party on AWS",
     'long_description': 'None',
     'author': 'JensRoland',
     'author_email': 'mail@jensroland.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://kegstand.dev',
```

### Comparing `kegstand-0.3.2/PKG-INFO` & `kegstand-0.3.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kegstand
-Version: 0.3.2
+Version: 0.3.3
 Summary: The Developer's Toolbelt For Accelerating Mean-Time-To-Party on AWS
 Home-page: https://kegstand.dev
 License: MIT
 Author: JensRoland
 Author-email: mail@jensroland.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

