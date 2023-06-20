# Comparing `tmp/live-fast-api-0.0.8.tar.gz` & `tmp/live-fast-api-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "live-fast-api-0.0.8.tar", last modified: Thu Jun 15 21:46:38 2023, max compression
+gzip compressed data, was "live-fast-api-0.0.9.tar", last modified: Tue Jun 20 16:01:27 2023, max compression
```

## Comparing `live-fast-api-0.0.8.tar` & `live-fast-api-0.0.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 21:46:38.153746 live-fast-api-0.0.8/
--rw-rw-rw-   0        0        0      215 2023-06-15 21:46:37.000000 live-fast-api-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     2054 2023-06-15 21:46:38.152746 live-fast-api-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1245 2023-04-12 14:06:13.000000 live-fast-api-0.0.8/README.md
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:14:12.000000 live-fast-api-0.0.8/build.py
-drwxrwxrwx   0        0        0        0 2023-06-15 21:46:38.082776 live-fast-api-0.0.8/live_api/
--rw-rw-rw-   0        0        0      493 2023-03-09 10:59:51.000000 live-fast-api-0.0.8/live_api/__init__.py
--rw-rw-rw-   0        0        0     7565 2023-06-11 21:12:00.000000 live-fast-api-0.0.8/live_api/base.py
--rw-rw-rw-   0        0        0      281 2023-04-12 14:23:43.000000 live-fast-api-0.0.8/live_api/document.py
-drwxrwxrwx   0        0        0        0 2023-06-15 21:46:38.114776 live-fast-api-0.0.8/live_api/endpoints/
--rw-rw-rw-   0        0        0      182 2023-04-12 14:16:43.000000 live-fast-api-0.0.8/live_api/endpoints/__init__.py
--rw-rw-rw-   0        0        0     2599 2023-04-12 14:12:33.000000 live-fast-api-0.0.8/live_api/endpoints/data.py
--rw-rw-rw-   0        0        0    10741 2023-06-13 13:34:08.000000 live-fast-api-0.0.8/live_api/endpoints/engine.py
--rw-rw-rw-   0        0        0     1566 2023-04-12 14:12:33.000000 live-fast-api-0.0.8/live_api/endpoints/exceptions.py
--rw-rw-rw-   0        0        0     1601 2023-04-12 14:15:29.000000 live-fast-api-0.0.8/live_api/endpoints/process.py
-drwxrwxrwx   0        0        0        0 2023-06-15 21:46:38.131773 live-fast-api-0.0.8/live_api/service/
--rw-rw-rw-   0        0        0       92 2023-04-12 14:22:24.000000 live-fast-api-0.0.8/live_api/service/__init__.py
--rw-rw-rw-   0        0        0    19305 2023-06-11 21:25:12.000000 live-fast-api-0.0.8/live_api/service/rest.py
--rw-rw-rw-   0        0        0     2991 2023-04-21 18:19:24.000000 live-fast-api-0.0.8/live_api/service/sockets.py
-drwxrwxrwx   0        0        0        0 2023-06-15 21:46:38.052747 live-fast-api-0.0.8/live_api/source/
-drwxrwxrwx   0        0        0        0 2023-06-15 21:46:38.052747 live-fast-api-0.0.8/live_api/source/assets/
-drwxrwxrwx   0        0        0        0 2023-06-15 21:46:38.136767 live-fast-api-0.0.8/live_api/source/assets/icon/
--rw-rw-rw-   0        0        0     2834 2023-02-04 16:41:18.000000 live-fast-api-0.0.8/live_api/source/assets/icon/icon.ico
--rw-rw-rw-   0        0        0    27619 2023-02-04 16:40:24.000000 live-fast-api-0.0.8/live_api/source/assets/icon/icon.png
-drwxrwxrwx   0        0        0        0 2023-06-15 21:46:38.152746 live-fast-api-0.0.8/live_fast_api.egg-info/
--rw-rw-rw-   0        0        0     2054 2023-06-15 21:46:37.000000 live-fast-api-0.0.8/live_fast_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      641 2023-06-15 21:46:38.000000 live-fast-api-0.0.8/live_fast_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 21:46:37.000000 live-fast-api-0.0.8/live_fast_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       98 2023-06-15 21:46:37.000000 live-fast-api-0.0.8/live_fast_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-15 21:46:37.000000 live-fast-api-0.0.8/live_fast_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      625 2023-06-15 21:46:37.000000 live-fast-api-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0      173 2023-06-15 21:46:37.000000 live-fast-api-0.0.8/requirements-dev.txt
--rw-rw-rw-   0        0        0       69 2023-06-15 21:46:16.000000 live-fast-api-0.0.8/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 21:46:38.153746 live-fast-api-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1580 2023-06-15 21:46:26.000000 live-fast-api-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:01:27.142007 live-fast-api-0.0.9/
+-rw-rw-rw-   0        0        0      215 2023-06-20 16:01:26.000000 live-fast-api-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     2054 2023-06-20 16:01:27.141009 live-fast-api-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1245 2023-04-12 14:06:13.000000 live-fast-api-0.0.9/README.md
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:14:12.000000 live-fast-api-0.0.9/build.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:01:27.082861 live-fast-api-0.0.9/live_api/
+-rw-rw-rw-   0        0        0      493 2023-03-09 10:59:51.000000 live-fast-api-0.0.9/live_api/__init__.py
+-rw-rw-rw-   0        0        0     7565 2023-06-11 21:12:00.000000 live-fast-api-0.0.9/live_api/base.py
+-rw-rw-rw-   0        0        0      281 2023-04-12 14:23:43.000000 live-fast-api-0.0.9/live_api/document.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:01:27.109864 live-fast-api-0.0.9/live_api/endpoints/
+-rw-rw-rw-   0        0        0      182 2023-04-12 14:16:43.000000 live-fast-api-0.0.9/live_api/endpoints/__init__.py
+-rw-rw-rw-   0        0        0     2599 2023-04-12 14:12:33.000000 live-fast-api-0.0.9/live_api/endpoints/data.py
+-rw-rw-rw-   0        0        0     9750 2023-06-20 15:12:12.000000 live-fast-api-0.0.9/live_api/endpoints/engine.py
+-rw-rw-rw-   0        0        0     1566 2023-04-12 14:12:33.000000 live-fast-api-0.0.9/live_api/endpoints/exceptions.py
+-rw-rw-rw-   0        0        0     1601 2023-04-12 14:15:29.000000 live-fast-api-0.0.9/live_api/endpoints/process.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:01:27.120373 live-fast-api-0.0.9/live_api/service/
+-rw-rw-rw-   0        0        0       92 2023-04-12 14:22:24.000000 live-fast-api-0.0.9/live_api/service/__init__.py
+-rw-rw-rw-   0        0        0    19890 2023-06-20 15:51:13.000000 live-fast-api-0.0.9/live_api/service/rest.py
+-rw-rw-rw-   0        0        0     2991 2023-04-21 18:19:24.000000 live-fast-api-0.0.9/live_api/service/sockets.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:01:27.054860 live-fast-api-0.0.9/live_api/source/
+drwxrwxrwx   0        0        0        0 2023-06-20 16:01:27.054860 live-fast-api-0.0.9/live_api/source/assets/
+drwxrwxrwx   0        0        0        0 2023-06-20 16:01:27.126007 live-fast-api-0.0.9/live_api/source/assets/icon/
+-rw-rw-rw-   0        0        0     2834 2023-02-04 16:41:18.000000 live-fast-api-0.0.9/live_api/source/assets/icon/icon.ico
+-rw-rw-rw-   0        0        0    27619 2023-02-04 16:40:24.000000 live-fast-api-0.0.9/live_api/source/assets/icon/icon.png
+drwxrwxrwx   0        0        0        0 2023-06-20 16:01:27.141009 live-fast-api-0.0.9/live_fast_api.egg-info/
+-rw-rw-rw-   0        0        0     2054 2023-06-20 16:01:27.000000 live-fast-api-0.0.9/live_fast_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      641 2023-06-20 16:01:27.000000 live-fast-api-0.0.9/live_fast_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 16:01:27.000000 live-fast-api-0.0.9/live_fast_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2023-06-20 16:01:27.000000 live-fast-api-0.0.9/live_fast_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-20 16:01:27.000000 live-fast-api-0.0.9/live_fast_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      625 2023-06-20 16:01:26.000000 live-fast-api-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       78 2023-06-15 21:47:31.000000 live-fast-api-0.0.9/requirements-dev.txt
+-rw-rw-rw-   0        0        0       69 2023-06-15 21:46:16.000000 live-fast-api-0.0.9/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 16:01:27.142007 live-fast-api-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1580 2023-06-20 16:00:13.000000 live-fast-api-0.0.9/setup.py
```

### Comparing `live-fast-api-0.0.8/PKG-INFO` & `live-fast-api-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: live-fast-api
-Version: 0.0.8
+Version: 0.0.9
 Summary: A framework for developing responsive, live and dynamic REST APIs with python.
 Home-page: https://github.com/Shahaf-F-S/live-api
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `live-fast-api-0.0.8/README.md` & `live-fast-api-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.8/build.py` & `live-fast-api-0.0.9/build.py`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.8/live_api/base.py` & `live-fast-api-0.0.9/live_api/base.py`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.8/live_api/endpoints/data.py` & `live-fast-api-0.0.9/live_api/endpoints/data.py`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.8/live_api/endpoints/engine.py` & `live-fast-api-0.0.9/live_api/endpoints/engine.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,26 @@
-# backend.py
+# engine.py
 
 import datetime as dt
 from functools import wraps
 from typing import (
     List, Any, Union, Dict, Optional,
-    Tuple, Callable, Iterable
+    Tuple, Callable, Iterable, TypeVar, Generic
 )
 
-from fastapi.openapi.docs import get_swagger_ui_html
+from fastapi.openapi.docs import get_swagger_ui_html, HTMLResponse
 
 from represent import Modifiers, BaseModel
 
-from live_api.endpoints.process import copy
 from live_api.endpoints.data import DOCS
 
 __all__ = [
     "BaseEndpoint",
     "DocsEndpoint",
     "Record",
-    "DataContainer",
     "valid_endpoints"
 ]
 
 class Record(BaseModel):
     """A class to represent a result object for commands and conditions calls."""
 
     def __init__(
@@ -62,67 +60,19 @@
         self.kwargs.update(kwargs)
         self.returns = returns
     # end collect
 # end Record
 
 Requests = List[Record]
 
-class DataContainer(BaseModel, dict):
-    """A class to represent a data container."""
+_ServiceType = TypeVar("_ServiceType")
+_ReturnType = TypeVar("_ReturnType")
+_ProcessedReturnType = TypeVar("_ProcessedReturnType")
 
-    def __setattr__(self, key: str, value: Any) -> None:
-        """
-        Sets the attribute.
-
-        :param key: The key to the attribute.
-        :param value: The value of the attribute.
-        """
-
-        self[key] = value
-
-        super().__setattr__(key, value)
-    # end __setattr__
-
-    def copy(self):
-        """
-        Copies the data of the model.
-
-        :return: The copy of the model.
-        """
-
-        data: DataContainer = copy(self)
-
-        return data
-    # end copy
-
-    def update(self, config: Dict[str, Any], **kwargs: Any) -> None:
-        """
-        Updates the object's data with the config.
-
-        :param config: The config object.
-        :param kwargs: Any keyword arguments.
-        """
-
-        if isinstance(config, type(self)):
-            config = config.__dict__
-        # end if
-
-        if isinstance(config, dict):
-            for key in self.__dict__.keys():
-                if key in config:
-                    setattr(self, key, config[key])
-                # end if
-            # end for
-        # end if
-
-        super().update(config, **kwargs)
-    # end update
-# end DataContainer
-
-class BaseEndpoint(BaseModel):
+class BaseEndpoint(BaseModel, Generic[_ServiceType, _ReturnType, _ProcessedReturnType]):
     """
     A class to represent an endpoint.
 
     The BaseEndpoint is a command class that is the base of custom
     endpoint classes. Custom endpoint classes inherit from BaseEndpoint
     to add the command to execute when the endpoint is requested
     by a client, through the API of a service object.
@@ -159,25 +109,25 @@
     >>>         ...
     >>>
     >>> endpoint = MyEndpoint(path="/<ENDPOINT PATH IN URL>", methods=[GET])
     # end AnswerEndpoint
     """
 
     modifiers = Modifiers(
-        excluded=["service", "options", "record", "modifiers"]
+        excluded=["options"], hidden=["record", "service"]
     )
 
     PATH: str
     METHODS: List[str]
 
     def __init__(
             self,
             path: Optional[str] = None,
             methods: Optional[Iterable[str]] = None,
-            service: Optional[object] = None,
+            service: Optional[_ServiceType] = None,
             description: Optional[str] = None,
             root: Optional[str] = None,
             options: Optional[Dict[str, Any]] = None
     ) -> None:
         """
         Defines the class attributes.
 
@@ -198,15 +148,15 @@
         self.description = description
 
         self.methods = list(methods or self.METHODS)
 
         self.service = service
     # end __init__
 
-    def __call__(self, *args: Any, **kwargs: Any) -> Dict[str, Union[int, Any]]:
+    def __call__(self, *args: Any, **kwargs: Any) -> Dict[str, Union[int, _ProcessedReturnType]]:
         """
         Returns the function to command the command.
 
         :param name: The intent that activated the command.
         :param message: The message for the intent.
 
         :return: The function to command the command.
@@ -218,53 +168,53 @@
 
         end = dt.datetime.now()
 
         return dict(response=result, time=(end - start).total_seconds())
     # end __call__
 
     @staticmethod
-    def call(instance) -> Callable:
+    def call(instance) -> Callable[..., Dict[str, Union[int, _ProcessedReturnType]]]:
         """
         Returns the function to command the command.
 
         :param instance: An instance of the class.
 
         :return: The function to command the command.
         """
 
         return instance.__call__
     # end __call__
 
-    def process(self, response: Any) -> Any:
+    def process(self, response: Any) -> _ProcessedReturnType:
         """
         Processes the response of the endpoint.
 
         :param response: The endpoint response to process.
 
         :return: The processed response.
         """
 
         dir(self)
 
         return response
     # end process
 
-    def wrap(self, endpoint: Callable[..., Any]) -> Any:
+    def wrap(self, endpoint: Callable[..., Any]) -> Callable[..., _ReturnType]:
         """
         Processes the response of the endpoint.
 
         :param endpoint: The endpoint to process.
 
         :return: The processed response.
         """
 
         dir(self)
 
         @wraps(endpoint)
-        def wrapper(*args: Any, **kwargs: Any) -> Any:
+        def wrapper(*args: Any, **kwargs: Any) -> _ReturnType:
             """
             Returns the response for the API endpoint.
 
             :param args: The positional arguments.
             :param kwargs: Any keyword argument.
 
             :return: The response from the function call.
@@ -292,15 +242,15 @@
 
         :returns: The root path.
         """
 
         return self.root
     # end get_root
 
-    def endpoint(self, *args: Any, **kwargs: Any) -> Any:
+    def endpoint(self, *args: Any, **kwargs: Any) -> _ReturnType:
         """
         Returns the response for the API endpoint.
 
         :param args: The positional arguments.
         :param kwargs: Any keyword argument.
 
         :return: The response from the function call.
@@ -336,15 +286,15 @@
 
         BaseEndpoint.__init__(
             self, path=DOCS, methods=methods, service=service,
             description=description, options=options
         )
     # end __init__
 
-    def endpoint(self) -> Any:
+    def endpoint(self) -> HTMLResponse:
         """
         Returns the response for the API endpoint.
 
         :return: The response from the function call.
         """
 
         return get_swagger_ui_html(
```

### Comparing `live-fast-api-0.0.8/live_api/endpoints/exceptions.py` & `live-fast-api-0.0.9/live_api/endpoints/exceptions.py`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.8/live_api/endpoints/process.py` & `live-fast-api-0.0.9/live_api/endpoints/process.py`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.8/live_api/service/rest.py` & `live-fast-api-0.0.9/live_api/service/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from functools import partial
 import threading
 import datetime as dt
 import copy
 import types
 import functools
 from typing import (
-    Any, Union, Iterable, Optional, Dict, Callable
+    Any, Union, Iterable, Optional, Dict, Callable, TypeVar
 )
 
 from uvicorn import Server, Config as ServiceConfig
 from fastapi import FastAPI, APIRouter
 import fastapi
 
 from live_api.base import terminate_thread, icons
@@ -32,23 +32,27 @@
 
 Port = Union[str, int]
 Host = str
 
 Endpoints = Dict[str, BaseEndpoint]
 EndpointsContainer = Union[Iterable[BaseEndpoint], Endpoints]
 
+_ReturnType = TypeVar("_ReturnType")
+
 def override_signature(
         command: Union[Callable, types.FunctionType], /, *,
-        new: types.FunctionType
-) -> types.FunctionType:
+        new: Union[Callable[..., _ReturnType], types.FunctionType],
+        name: Optional[str] = None
+) -> Union[Callable[..., _ReturnType], types.FunctionType]:
     """
     Overrides the signature of a function.
 
     :param command: The function to override.
     :param new: The function wit the new signature.
+    :param name: The new name for the function.
 
     :return: The old function with the new signature.
     """
 
     attributes = (
         '__module__', '__name__', '__qualname__',
         '__doc__', '__annotations__'
@@ -62,14 +66,18 @@
         Dict[str, Union[int, new.__annotations__['return']]]
     )
 
     command = functools.update_wrapper(command, new, assigned=attributes)
 
     command.__kwdefaults__ = copy.copy(new.__kwdefaults__)
 
+    if isinstance(name, str):
+        command.__name__ = name
+    # end if
+
     return command
 # end override_signature
 
 class RESTService(BaseModel):
     """
     A class to represent a service object.
 
@@ -152,15 +160,17 @@
         :param root: The root to the path.
         :param home: The home endpoint.
         :param debug: The value to create the docs' endpoint for the home endpoint.
         """
 
         self._root = None
 
-        self.endpoints = {}
+        _Base = type(self)
+
+        self.endpoints: Dict[str, BaseEndpoint[_Base]] = {}
 
         if (
             (isinstance(home, bool) and home) or
             (debug and (home is None))
         ):
             home = True
         # end if
@@ -175,17 +185,15 @@
         self.description = description or self.DESCRIPTION
         self.root = root or ""
         self.icon = icon or self.ICON
         self.home = home
         self.name = name or self.NAME
         self.version = version or self.VERSION
 
-        self.endpoints.update(
-            self.valid_endpoints(endpoints)
-        )
+        self.endpoints.update(self.valid_endpoints(endpoints))
 
         for endpoint in self.endpoints.values():
             endpoint.service = self
         # end for
     # end __init__
 
     def __getstate__(self) -> Dict[str, Any]:
@@ -236,14 +244,21 @@
         :param value: The root path.
         """
 
         if value == self._root:
             return
         # end if
 
+        if not hasattr(self, "endpoints"):
+            raise AttributeError(
+                f"{self} must container 'endpoints' "
+                f"attribute before attempting to set 'root'"
+            )
+        # end if
+
         self._root = value
 
         for endpoint in self.endpoints.copy().values():
             endpoint.set_root(self.root)
 
             if endpoint.root:
                 self.endpoints.pop(endpoint.path)
@@ -403,23 +418,23 @@
 
     def remove_all_endpoints(self) -> None:
         """Removes all the endpoints from the service."""
 
         self.endpoints.clear()
     # end remove_all_endpoints
 
-    def set_endpoints(self, endpoints: EndpointsContainer) -> None:
+    def update_endpoints(self, endpoints: EndpointsContainer) -> None:
         """
         Adds the endpoint to the service.
 
         :param endpoints: The commands to run.
         """
 
-        self.endpoints: Endpoints = self.valid_endpoints(endpoints)
-    # end set_endpoints
+        self.endpoints.update(self.valid_endpoints(endpoints))
+    # end update_endpoints
 
     def build(self) -> None:
         """
         Builds the service endpoints.
 
         :returns: The app object.
         """
@@ -436,15 +451,15 @@
         for endpoint in self.endpoints.values():
             endpoint.set_root(self.root)
 
             path = ("/" + endpoint.root if endpoint.root else '') + endpoint.path
 
             command = override_signature(
                 partial(endpoint.__call__, endpoint),
-                new=endpoint.endpoint
+                new=endpoint.endpoint, name=type(endpoint).__name__
             )
 
             try:
                 router.add_api_route(
                     path, command,
                     methods=endpoint.methods, description=endpoint.description,
                     **endpoint.options
```

### Comparing `live-fast-api-0.0.8/live_api/service/sockets.py` & `live-fast-api-0.0.9/live_api/service/sockets.py`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.8/live_api/source/assets/icon/icon.ico` & `live-fast-api-0.0.9/live_api/source/assets/icon/icon.ico`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.8/live_api/source/assets/icon/icon.png` & `live-fast-api-0.0.9/live_api/source/assets/icon/icon.png`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.8/live_fast_api.egg-info/PKG-INFO` & `live-fast-api-0.0.9/live_fast_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: live-fast-api
-Version: 0.0.8
+Version: 0.0.9
 Summary: A framework for developing responsive, live and dynamic REST APIs with python.
 Home-page: https://github.com/Shahaf-F-S/live-api
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `live-fast-api-0.0.8/live_fast_api.egg-info/SOURCES.txt` & `live-fast-api-0.0.9/live_fast_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.8/pyproject.toml` & `live-fast-api-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'live-fast-api'
-version = '0.0.8'
+version = '0.0.9'
 description = 'A framework for developing responsive, live and dynamic REST APIs with python.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `live-fast-api-0.0.8/setup.py` & `live-fast-api-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ],
         include=[
             "live_api/source"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='live-fast-api',
-        version='0.0.8',
+        version='0.0.9',
         description=(
             "A framework for developing responsive, "
             "live and dynamic REST APIs with python."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
         author_email='shahaffrs@gmail.com',
```

