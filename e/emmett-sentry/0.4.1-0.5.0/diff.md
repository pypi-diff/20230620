# Comparing `tmp/emmett_sentry-0.4.1.tar.gz` & `tmp/emmett_sentry-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emmett_sentry-0.4.1.tar", max compression
+gzip compressed data, was "emmett_sentry-0.5.0.tar", max compression
```

## Comparing `emmett_sentry-0.4.1.tar` & `emmett_sentry-0.5.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1486 2023-05-04 13:55:35.593865 emmett_sentry-0.4.1/LICENSE
--rw-r--r--   0        0        0     1475 2023-05-04 13:55:35.593865 emmett_sentry-0.4.1/README.md
--rw-r--r--   0        0        0       24 2023-05-04 13:55:35.593865 emmett_sentry-0.4.1/emmett_sentry/__init__.py
--rw-r--r--   0        0        0       22 2023-05-04 13:55:35.593865 emmett_sentry-0.4.1/emmett_sentry/__version__.py
--rw-r--r--   0        0        0     2469 2023-05-04 13:55:35.593865 emmett_sentry-0.4.1/emmett_sentry/ext.py
--rw-r--r--   0        0        0     7866 2023-05-04 13:55:35.593865 emmett_sentry-0.4.1/emmett_sentry/helpers.py
--rw-r--r--   0        0        0     1298 2023-05-04 13:55:35.593865 emmett_sentry-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     2243 1970-01-01 00:00:00.000000 emmett_sentry-0.4.1/setup.py
--rw-r--r--   0        0        0     2946 1970-01-01 00:00:00.000000 emmett_sentry-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1486 2023-06-20 12:42:07.333167 emmett_sentry-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1845 2023-06-20 12:42:07.333167 emmett_sentry-0.5.0/README.md
+-rw-r--r--   0        0        0       31 2023-06-20 12:42:07.333167 emmett_sentry-0.5.0/emmett_sentry/__init__.py
+-rw-r--r--   0        0        0       22 2023-06-20 12:42:07.333167 emmett_sentry-0.5.0/emmett_sentry/__version__.py
+-rw-r--r--   0        0        0     3415 2023-06-20 12:42:07.333167 emmett_sentry-0.5.0/emmett_sentry/ext.py
+-rw-r--r--   0        0        0     7322 2023-06-20 12:42:07.333167 emmett_sentry-0.5.0/emmett_sentry/helpers.py
+-rw-r--r--   0        0        0     5197 2023-06-20 12:42:07.333167 emmett_sentry-0.5.0/emmett_sentry/instrument.py
+-rw-r--r--   0        0        0     1296 2023-06-20 12:42:07.333167 emmett_sentry-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2621 1970-01-01 00:00:00.000000 emmett_sentry-0.5.0/setup.py
+-rw-r--r--   0        0        0     3313 1970-01-01 00:00:00.000000 emmett_sentry-0.5.0/PKG-INFO
```

### Comparing `emmett_sentry-0.4.1/LICENSE` & `emmett_sentry-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `emmett_sentry-0.4.1/README.md` & `emmett_sentry-0.5.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -24,19 +24,25 @@
 
 | param | default | description |
 | --- | --- | --- |
 | dsn | | Sentry project's DSN |
 | environment | development | Application environment |
 | release | | Application release |
 | auto\_load | `True` | Automatically inject extension on routes |
-| enable\_tracing | `False` | Enable tracing on routes |
 | sample\_rate | 1 | Error sampling rate |
-| traces\_sample\_rate | | Traces sampling rate |
-| trace\_websockets | `False` | Enable tracing on websocket routes |
+| integrations | | List of integrations to pass to the SDK |
+| enable\_tracing | `False` | Enable tracing on routes |
+| tracing\_sample\_rate | | Traces sampling rate |
 | tracing\_exclude\_routes | | List of specific routes to exclude from tracing | 
+| trace\_websockets | `False` | Enable tracing on websocket routes |
+| trace\_orm | `True` | Enable tracing on ORM queries |
+| trace\_templates | `True` | Enable tracing on templates rendering |
+| trace\_sessions | `True` | Enable tracing on sessions load/store |
+| trace\_cache | `True` | Enable tracing on cache get/set |
+| trace\_pipes | `False` | Enable tracing on pipes |
 
 ## Usage
 
 The extension exposes two methods to manually track events:
 
 - exception
 - message
```

### Comparing `emmett_sentry-0.4.1/emmett_sentry/helpers.py` & `emmett_sentry-0.5.0/emmett_sentry/helpers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-# -*- coding: utf-8 -*-
-"""
-    emmett_sentry.helpers
-    ---------------------
-
-    Provides Sentry extension helpers
-
-    :copyright: 2020 Giovanni Barillari
-    :license: BSD-3-Clause
-"""
-
 import urllib
 
 from functools import wraps
 
 from emmett import current
 from emmett.asgi.wrappers import Request as ASGIRequest, Websocket as ASGIWebsocket
 from emmett.http import HTTPResponse
@@ -98,111 +87,109 @@
 
     return event
 
 
 def _build_http_dispatcher_wrapper_err(ext, dispatch_method):
     @wraps(dispatch_method)
     async def wrap(*args, **kwargs):
-        with Hub(Hub.current) as hub:
-            with hub.push_scope() as scope:
-                scope.add_event_processor(_process_http)
-                for key, builder in ext._scopes.items():
-                    scope.set_extra(key, await builder())
+        hub = Hub.current
+        with hub.push_scope() as scope:
+            scope.add_event_processor(_process_http)
+            for key, builder in ext._scopes.items():
+                scope.set_extra(key, await builder())
+            try:
+                return await dispatch_method(*args, **kwargs)
+            except HTTPResponse:
+                raise
+            except Exception as exc:
+                scope.set_extra(
+                    "body_params",
+                    await current.request.body_params
+                )
+                _capture_exception(hub, exc)
+                raise
+    return wrap
+
+
+def _build_http_dispatcher_wrapper_txn(ext, dispatch_method):
+    @wraps(dispatch_method)
+    async def wrap(*args, **kwargs):
+        hub = Hub.current
+        with hub.push_scope() as scope:
+            scope.add_event_processor(_process_http)
+            for key, builder in ext._scopes.items():
+                scope.set_extra(key, await builder())
+
+            proto = (
+                "rsgi" if hasattr(current.request._scope, "rsgi_version") else "asgi"
+            )
+            txn = Transaction.continue_from_headers(
+                current.request.headers,
+                op="http.server"
+            )
+            txn.set_tag(f"{proto}.type", "http")
+
+            with hub.start_transaction(txn):
                 try:
                     return await dispatch_method(*args, **kwargs)
                 except HTTPResponse:
                     raise
                 except Exception as exc:
                     scope.set_extra(
                         "body_params",
                         await current.request.body_params
                     )
                     _capture_exception(hub, exc)
                     raise
     return wrap
 
 
-def _build_http_dispatcher_wrapper_txn(ext, dispatch_method):
+def _build_ws_dispatcher_wrapper_err(ext, dispatch_method):
     @wraps(dispatch_method)
     async def wrap(*args, **kwargs):
-        with Hub(Hub.current) as hub:
-            with hub.push_scope() as scope:
-                scope.add_event_processor(_process_http)
-                for key, builder in ext._scopes.items():
-                    scope.set_extra(key, await builder())
-
-                proto = (
-                    "rsgi" if hasattr(current.request._scope, "rsgi_version") else
-                    "asgi"
-                )
-                txn = Transaction.continue_from_headers(
-                    current.request.headers,
-                    op="http.server"
-                )
-                txn.set_tag(f"{proto}.type", "http")
-
-                with hub.start_transaction(txn):
-                    try:
-                        return await dispatch_method(*args, **kwargs)
-                    except HTTPResponse:
-                        raise
-                    except Exception as exc:
-                        scope.set_extra(
-                            "body_params",
-                            await current.request.body_params
-                        )
-                        _capture_exception(hub, exc)
-                        raise
+        hub = Hub.current
+        with hub.push_scope() as scope:
+            scope.add_event_processor(_process_ws)
+            for key, builder in ext._scopes.items():
+                scope.set_extra(key, await builder())
+            try:
+                return await dispatch_method(*args, **kwargs)
+            except Exception as exc:
+                _capture_exception(hub, exc)
+                raise
     return wrap
 
 
-def _build_ws_dispatcher_wrapper_err(ext, dispatch_method):
+def _build_ws_dispatcher_wrapper_txn(ext, dispatch_method):
     @wraps(dispatch_method)
     async def wrap(*args, **kwargs):
-        with Hub(Hub.current) as hub:
-            with hub.push_scope() as scope:
-                scope.add_event_processor(_process_ws)
-                for key, builder in ext._scopes.items():
-                    scope.set_extra(key, await builder())
+        hub = Hub.current
+        with hub.push_scope() as scope:
+            scope.add_event_processor(_process_ws)
+            for key, builder in ext._scopes.items():
+                scope.set_extra(key, await builder())
+
+            proto = (
+                "rsgi" if hasattr(current.websocket._scope, "rsgi_version") else "asgi"
+            )
+            txn = Transaction.continue_from_headers(
+                current.websocket.headers,
+                op="websocket.server"
+            )
+            txn.set_tag(f"{proto}.type", "websocket")
+
+            with hub.start_transaction(txn):
                 try:
                     return await dispatch_method(*args, **kwargs)
                 except Exception as exc:
                     _capture_exception(hub, exc)
                     raise
     return wrap
 
 
-def _build_ws_dispatcher_wrapper_txn(ext, dispatch_method):
-    @wraps(dispatch_method)
-    async def wrap(*args, **kwargs):
-        with Hub(Hub.current) as hub:
-            with hub.push_scope() as scope:
-                scope.add_event_processor(_process_ws)
-                for key, builder in ext._scopes.items():
-                    scope.set_extra(key, await builder())
-
-                proto = (
-                    "rsgi" if hasattr(current.websocket._scope, "rsgi_version") else
-                    "asgi"
-                )
-                txn = Transaction.continue_from_headers(
-                    current.websocket.headers,
-                    op="websocket.server"
-                )
-                txn.set_tag(f"{proto}.type", "websocket")
-
-                with hub.start_transaction(txn):
-                    try:
-                        return await dispatch_method(*args, **kwargs)
-                    except Exception as exc:
-                        _capture_exception(hub, exc)
-                        raise
-    return wrap
-
-
 def _build_routing_rec_http(ext, rec_cls):
     def _routing_rec_http(router, name, match, dispatch):
         wrapper = (
             _build_http_dispatcher_wrapper_txn if (
                 ext.config.enable_tracing and
                 name not in ext._tracing_excluded_routes
             ) else _build_http_dispatcher_wrapper_err
```

### Comparing `emmett_sentry-0.4.1/pyproject.toml` & `emmett_sentry-0.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "emmett-sentry"
-version = "0.4.1"
+version = "0.5.0"
 description = "Sentry extension for Emmett framework"
 authors = ["Giovanni Barillari <g@baro.dev>"]
 license = "BSD-3-Clause"
 
 readme = "README.md"
 homepage = "https://github.com/emmett-framework/sentry"
 repository = "https://github.com/emmett-framework/sentry"
@@ -29,15 +29,15 @@
 include = [
     "LICENSE"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 emmett = "^2.5.0"
-sentry-sdk = "^1.20.0"
+sentry-sdk = "~1.25"
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.urls]
 "Issue Tracker" = "https://github.com/emmett-framework/sentry/issues"
 
 [build-system]
```

### Comparing `emmett_sentry-0.4.1/setup.py` & `emmett_sentry-0.5.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 packages = \
 ['emmett_sentry']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['emmett>=2.5.0,<3.0.0', 'sentry-sdk>=1.20.0,<2.0.0']
+['emmett>=2.5.0,<3.0.0', 'sentry-sdk>=1.25,<1.26']
 
 setup_kwargs = {
     'name': 'emmett-sentry',
-    'version': '0.4.1',
+    'version': '0.5.0',
     'description': 'Sentry extension for Emmett framework',
-    'long_description': '# Emmett-Sentry\n\nEmmett-Sentry is an [Emmett framework](https://emmett.sh) extension integrating [Sentry](https://sentry.io) monitoring platform.\n\n[![pip version](https://img.shields.io/pypi/v/emmett-sentry.svg?style=flat)](https://pypi.python.org/pypi/emmett-sentry) \n\n## Installation\n\nYou can install Emmett-Sentry using pip:\n\n    pip install emmett-sentry\n\nAnd add it to your Emmett application:\n\n```python\nfrom emmett_sentry import Sentry\n\nsentry = app.use_extension(Sentry)\n```\n\n## Configuration\n\nHere is the complete list of parameters of the extension configuration:\n\n| param | default | description |\n| --- | --- | --- |\n| dsn | | Sentry project\'s DSN |\n| environment | development | Application environment |\n| release | | Application release |\n| auto\\_load | `True` | Automatically inject extension on routes |\n| enable\\_tracing | `False` | Enable tracing on routes |\n| sample\\_rate | 1 | Error sampling rate |\n| traces\\_sample\\_rate | | Traces sampling rate |\n| trace\\_websockets | `False` | Enable tracing on websocket routes |\n| tracing\\_exclude\\_routes | | List of specific routes to exclude from tracing | \n\n## Usage\n\nThe extension exposes two methods to manually track events:\n\n- exception\n- message\n\nYou call these methods directly within your code:\n\n```python\n# track an error\ntry:\n    1 / 0\nexcept Exception:\n    sentry.exception()\n\n# track a message\nsentry.message("some event", level="info")\n```\n\n## License\n\nEmmett-Sentry is released under BSD license.\n',
+    'long_description': '# Emmett-Sentry\n\nEmmett-Sentry is an [Emmett framework](https://emmett.sh) extension integrating [Sentry](https://sentry.io) monitoring platform.\n\n[![pip version](https://img.shields.io/pypi/v/emmett-sentry.svg?style=flat)](https://pypi.python.org/pypi/emmett-sentry) \n\n## Installation\n\nYou can install Emmett-Sentry using pip:\n\n    pip install emmett-sentry\n\nAnd add it to your Emmett application:\n\n```python\nfrom emmett_sentry import Sentry\n\nsentry = app.use_extension(Sentry)\n```\n\n## Configuration\n\nHere is the complete list of parameters of the extension configuration:\n\n| param | default | description |\n| --- | --- | --- |\n| dsn | | Sentry project\'s DSN |\n| environment | development | Application environment |\n| release | | Application release |\n| auto\\_load | `True` | Automatically inject extension on routes |\n| sample\\_rate | 1 | Error sampling rate |\n| integrations | | List of integrations to pass to the SDK |\n| enable\\_tracing | `False` | Enable tracing on routes |\n| tracing\\_sample\\_rate | | Traces sampling rate |\n| tracing\\_exclude\\_routes | | List of specific routes to exclude from tracing | \n| trace\\_websockets | `False` | Enable tracing on websocket routes |\n| trace\\_orm | `True` | Enable tracing on ORM queries |\n| trace\\_templates | `True` | Enable tracing on templates rendering |\n| trace\\_sessions | `True` | Enable tracing on sessions load/store |\n| trace\\_cache | `True` | Enable tracing on cache get/set |\n| trace\\_pipes | `False` | Enable tracing on pipes |\n\n## Usage\n\nThe extension exposes two methods to manually track events:\n\n- exception\n- message\n\nYou call these methods directly within your code:\n\n```python\n# track an error\ntry:\n    1 / 0\nexcept Exception:\n    sentry.exception()\n\n# track a message\nsentry.message("some event", level="info")\n```\n\n## License\n\nEmmett-Sentry is released under BSD license.\n',
     'author': 'Giovanni Barillari',
     'author_email': 'g@baro.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/emmett-framework/sentry',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `emmett_sentry-0.4.1/PKG-INFO` & `emmett_sentry-0.5.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emmett-sentry
-Version: 0.4.1
+Version: 0.5.0
 Summary: Sentry extension for Emmett framework
 Home-page: https://github.com/emmett-framework/sentry
 License: BSD-3-Clause
 Keywords: sentry,logging,emmett
 Author: Giovanni Barillari
 Author-email: g@baro.dev
 Requires-Python: >=3.8,<4.0
@@ -23,15 +23,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: emmett (>=2.5.0,<3.0.0)
-Requires-Dist: sentry-sdk (>=1.20.0,<2.0.0)
+Requires-Dist: sentry-sdk (>=1.25,<1.26)
 Project-URL: Issue Tracker, https://github.com/emmett-framework/sentry/issues
 Project-URL: Repository, https://github.com/emmett-framework/sentry
 Description-Content-Type: text/markdown
 
 # Emmett-Sentry
 
 Emmett-Sentry is an [Emmett framework](https://emmett.sh) extension integrating [Sentry](https://sentry.io) monitoring platform.
@@ -58,19 +58,25 @@
 
 | param | default | description |
 | --- | --- | --- |
 | dsn | | Sentry project's DSN |
 | environment | development | Application environment |
 | release | | Application release |
 | auto\_load | `True` | Automatically inject extension on routes |
-| enable\_tracing | `False` | Enable tracing on routes |
 | sample\_rate | 1 | Error sampling rate |
-| traces\_sample\_rate | | Traces sampling rate |
-| trace\_websockets | `False` | Enable tracing on websocket routes |
+| integrations | | List of integrations to pass to the SDK |
+| enable\_tracing | `False` | Enable tracing on routes |
+| tracing\_sample\_rate | | Traces sampling rate |
 | tracing\_exclude\_routes | | List of specific routes to exclude from tracing | 
+| trace\_websockets | `False` | Enable tracing on websocket routes |
+| trace\_orm | `True` | Enable tracing on ORM queries |
+| trace\_templates | `True` | Enable tracing on templates rendering |
+| trace\_sessions | `True` | Enable tracing on sessions load/store |
+| trace\_cache | `True` | Enable tracing on cache get/set |
+| trace\_pipes | `False` | Enable tracing on pipes |
 
 ## Usage
 
 The extension exposes two methods to manually track events:
 
 - exception
 - message
```

