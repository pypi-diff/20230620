# Comparing `tmp/fal_serverless-0.6.34.tar.gz` & `tmp/fal_serverless-0.6.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fal_serverless-0.6.34.tar", max compression
+gzip compressed data, was "fal_serverless-0.6.35.tar", max compression
```

## Comparing `fal_serverless-0.6.34.tar` & `fal_serverless-0.6.35.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      213 2023-06-12 16:47:30.829636 fal_serverless-0.6.34/README.md
--rw-r--r--   0        0        0     1006 2023-06-12 16:47:53.626225 fal_serverless-0.6.34/pyproject.toml
--rw-r--r--   0        0        0      335 2023-06-12 16:47:30.829636 fal_serverless-0.6.34/src/fal_serverless/__init__.py
--rw-r--r--   0        0        0    17568 2023-06-12 16:47:30.829636 fal_serverless-0.6.34/src/fal_serverless/api.py
--rw-r--r--   0        0        0     2593 2023-06-12 16:47:30.829636 fal_serverless-0.6.34/src/fal_serverless/auth/__init__.py
--rw-r--r--   0        0        0     5426 2023-06-12 16:47:30.829636 fal_serverless-0.6.34/src/fal_serverless/auth/auth0.py
--rw-r--r--   0        0        0     1786 2023-06-12 16:47:30.829636 fal_serverless-0.6.34/src/fal_serverless/auth/local.py
--rw-r--r--   0        0        0    15633 2023-06-12 16:47:30.829636 fal_serverless-0.6.34/src/fal_serverless/cli.py
--rw-r--r--   0        0        0      132 2023-06-12 16:47:30.829636 fal_serverless-0.6.34/src/fal_serverless/console/__init__.py
--rw-r--r--   0        0        0      108 2023-06-12 16:47:30.829636 fal_serverless-0.6.34/src/fal_serverless/console/icons.py
--rw-r--r--   0        0        0      485 2023-06-12 16:47:30.829636 fal_serverless-0.6.34/src/fal_serverless/console/ux.py
--rw-r--r--   0        0        0      172 2023-06-12 16:47:45.242028 fal_serverless-0.6.34/src/fal_serverless/env.py
--rw-r--r--   0        0        0      938 2023-06-12 16:47:30.829636 fal_serverless-0.6.34/src/fal_serverless/exceptions/__init__.py
--rw-r--r--   0        0        0      412 2023-06-12 16:47:30.829636 fal_serverless-0.6.34/src/fal_serverless/exceptions/_base.py
--rw-r--r--   0        0        0      353 2023-06-12 16:47:30.829636 fal_serverless-0.6.34/src/fal_serverless/exceptions/auth.py
--rw-r--r--   0        0        0     1435 2023-06-12 16:47:30.829636 fal_serverless-0.6.34/src/fal_serverless/exceptions/handlers.py
--rw-r--r--   0        0        0      326 2023-06-12 16:47:30.829636 fal_serverless-0.6.34/src/fal_serverless/flags.py
--rw-r--r--   0        0        0     1649 2023-06-12 16:47:30.829636 fal_serverless-0.6.34/src/fal_serverless/logging/__init__.py
--rw-r--r--   0        0        0     2574 2023-06-12 16:47:30.829636 fal_serverless-0.6.34/src/fal_serverless/logging/datadog.py
--rw-r--r--   0        0        0     2122 2023-06-12 16:47:30.829636 fal_serverless-0.6.34/src/fal_serverless/logging/isolate.py
--rw-r--r--   0        0        0      386 2023-06-12 16:47:30.829636 fal_serverless-0.6.34/src/fal_serverless/logging/style.py
--rw-r--r--   0        0        0     1785 2023-06-12 16:47:30.829636 fal_serverless-0.6.34/src/fal_serverless/logging/trace.py
--rw-r--r--   0        0        0      643 2023-06-12 16:47:30.829636 fal_serverless-0.6.34/src/fal_serverless/logging/user.py
--rw-r--r--   0        0        0    16029 2023-06-12 16:47:30.829636 fal_serverless-0.6.34/src/fal_serverless/sdk.py
--rw-r--r--   0        0        0     6533 2023-06-12 16:47:30.829636 fal_serverless-0.6.34/src/fal_serverless/sync.py
--rw-r--r--   0        0        0     1778 1970-01-01 00:00:00.000000 fal_serverless-0.6.34/setup.py
--rw-r--r--   0        0        0     1608 1970-01-01 00:00:00.000000 fal_serverless-0.6.34/PKG-INFO
+-rw-r--r--   0        0        0      213 2023-06-20 00:21:31.515343 fal_serverless-0.6.35/README.md
+-rw-r--r--   0        0        0     1013 2023-06-20 00:21:51.807364 fal_serverless-0.6.35/pyproject.toml
+-rw-r--r--   0        0        0      335 2023-06-20 00:21:31.515343 fal_serverless-0.6.35/src/fal_serverless/__init__.py
+-rw-r--r--   0        0        0    17568 2023-06-20 00:21:31.515343 fal_serverless-0.6.35/src/fal_serverless/api.py
+-rw-r--r--   0        0        0     2593 2023-06-20 00:21:31.515343 fal_serverless-0.6.35/src/fal_serverless/auth/__init__.py
+-rw-r--r--   0        0        0     5426 2023-06-20 00:21:31.515343 fal_serverless-0.6.35/src/fal_serverless/auth/auth0.py
+-rw-r--r--   0        0        0     1786 2023-06-20 00:21:31.515343 fal_serverless-0.6.35/src/fal_serverless/auth/local.py
+-rw-r--r--   0        0        0    15650 2023-06-20 00:21:31.515343 fal_serverless-0.6.35/src/fal_serverless/cli.py
+-rw-r--r--   0        0        0      132 2023-06-20 00:21:31.515343 fal_serverless-0.6.35/src/fal_serverless/console/__init__.py
+-rw-r--r--   0        0        0      108 2023-06-20 00:21:31.515343 fal_serverless-0.6.35/src/fal_serverless/console/icons.py
+-rw-r--r--   0        0        0      485 2023-06-20 00:21:31.515343 fal_serverless-0.6.35/src/fal_serverless/console/ux.py
+-rw-r--r--   0        0        0      172 2023-06-20 00:21:44.471356 fal_serverless-0.6.35/src/fal_serverless/env.py
+-rw-r--r--   0        0        0      938 2023-06-20 00:21:31.515343 fal_serverless-0.6.35/src/fal_serverless/exceptions/__init__.py
+-rw-r--r--   0        0        0      412 2023-06-20 00:21:31.515343 fal_serverless-0.6.35/src/fal_serverless/exceptions/_base.py
+-rw-r--r--   0        0        0      353 2023-06-20 00:21:31.515343 fal_serverless-0.6.35/src/fal_serverless/exceptions/auth.py
+-rw-r--r--   0        0        0     1435 2023-06-20 00:21:31.515343 fal_serverless-0.6.35/src/fal_serverless/exceptions/handlers.py
+-rw-r--r--   0        0        0      326 2023-06-20 00:21:31.515343 fal_serverless-0.6.35/src/fal_serverless/flags.py
+-rw-r--r--   0        0        0     1649 2023-06-20 00:21:31.515343 fal_serverless-0.6.35/src/fal_serverless/logging/__init__.py
+-rw-r--r--   0        0        0     2574 2023-06-20 00:21:31.515343 fal_serverless-0.6.35/src/fal_serverless/logging/datadog.py
+-rw-r--r--   0        0        0     2122 2023-06-20 00:21:31.515343 fal_serverless-0.6.35/src/fal_serverless/logging/isolate.py
+-rw-r--r--   0        0        0      386 2023-06-20 00:21:31.515343 fal_serverless-0.6.35/src/fal_serverless/logging/style.py
+-rw-r--r--   0        0        0     1785 2023-06-20 00:21:31.515343 fal_serverless-0.6.35/src/fal_serverless/logging/trace.py
+-rw-r--r--   0        0        0      643 2023-06-20 00:21:31.515343 fal_serverless-0.6.35/src/fal_serverless/logging/user.py
+-rw-r--r--   0        0        0    16374 2023-06-20 00:21:31.515343 fal_serverless-0.6.35/src/fal_serverless/sdk.py
+-rw-r--r--   0        0        0     6533 2023-06-20 00:21:31.515343 fal_serverless-0.6.35/src/fal_serverless/sync.py
+-rw-r--r--   0        0        0     1783 1970-01-01 00:00:00.000000 fal_serverless-0.6.35/setup.py
+-rw-r--r--   0        0        0     1613 1970-01-01 00:00:00.000000 fal_serverless-0.6.35/PKG-INFO
```

### Comparing `fal_serverless-0.6.34/pyproject.toml` & `fal_serverless-0.6.35/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "fal_serverless"
-version = "0.6.34"
+version = "0.6.35"
 description = "fal Serverless is an easy-to-use Serverless Python Framework"
 authors = ["Features & Labels <hello@fal.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 auth0-python = "^4.1.0"
 requests = "^2.28.1"
 isolate = {version = ">=0.12.2, <1.0", extras = ["build"]}
 grpcio = "^1.50.0"
-dill = "0.3.5.1"
-isolate-proto = "^0.0.30"
+dill = ">=0.3.6,<0.3.7"
+isolate-proto = "^0.0.31"
 typing-extensions = "4.4"
 click = "^8.1.3"
 structlog = "^22.3.0"
 datadog-api-client = "2.12.0"
 opentelemetry-api = "^1.15.0"
 opentelemetry-sdk = "^1.15.0"
 grpc-interceptor = "^0.15.0"
```

### Comparing `fal_serverless-0.6.34/src/fal_serverless/api.py` & `fal_serverless-0.6.35/src/fal_serverless/api.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.34/src/fal_serverless/auth/__init__.py` & `fal_serverless-0.6.35/src/fal_serverless/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.34/src/fal_serverless/auth/auth0.py` & `fal_serverless-0.6.35/src/fal_serverless/auth/auth0.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.34/src/fal_serverless/auth/local.py` & `fal_serverless-0.6.35/src/fal_serverless/auth/local.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.34/src/fal_serverless/cli.py` & `fal_serverless-0.6.35/src/fal_serverless/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 import grpc
 from fal_serverless import api, sdk
 from fal_serverless.console import console
 from fal_serverless.exceptions import ApplicationExceptionHandler
 from fal_serverless.logging import get_logger, set_debug_logging
 from fal_serverless.logging.isolate import IsolateLogPrinter
 from fal_serverless.logging.trace import get_tracer
-from fal_serverless.sync import get_latest_logs
 from rich.table import Table
 
 DEFAULT_HOST = "api.alpha.fal.ai"
 HOST_ENVVAR = "FAL_HOST"
 
 DEFAULT_PORT = "443"
 PORT_ENVVAR = "FAL_PORT"
@@ -333,22 +332,26 @@
         console.print(cron_id)
 
 
 @function_cli.command("logs")
 @click.option("--lines", default=100)
 @click.option("--url", default=None)
 @click.pass_obj
-def get_logs(host: api.FalServerlessHost, lines: int | None, url: str | None):
+def get_logs(
+    host: api.FalServerlessHost, lines: int | None = 100, url: str | None = None
+):
     if url:
         url = remove_http_and_port_from_url(url)
-    latest_logs = get_latest_logs(lines, url)
-    latest_logs.reverse()
+    logs = host._connection.get_logs(lines=lines, url=url)
+    if not logs:
+        console.print("No logs found")
+        return
     log_printer = IsolateLogPrinter(debug=True)
-    for log in latest_logs:
-        log_printer.print_dict(log)
+    for log in logs:
+        log_printer.print(log)
 
 
 ##### Alias group #####
 @click.group
 @click.option("--host", default=DEFAULT_HOST, envvar=HOST_ENVVAR)
 @click.option("--port", default=DEFAULT_PORT, envvar=PORT_ENVVAR, hidden=True)
 @click.pass_context
```

### Comparing `fal_serverless-0.6.34/src/fal_serverless/exceptions/__init__.py` & `fal_serverless-0.6.35/src/fal_serverless/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.34/src/fal_serverless/exceptions/handlers.py` & `fal_serverless-0.6.35/src/fal_serverless/exceptions/handlers.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.34/src/fal_serverless/logging/__init__.py` & `fal_serverless-0.6.35/src/fal_serverless/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.34/src/fal_serverless/logging/datadog.py` & `fal_serverless-0.6.35/src/fal_serverless/logging/datadog.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.34/src/fal_serverless/logging/isolate.py` & `fal_serverless-0.6.35/src/fal_serverless/logging/isolate.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.34/src/fal_serverless/logging/trace.py` & `fal_serverless-0.6.35/src/fal_serverless/logging/trace.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.34/src/fal_serverless/logging/user.py` & `fal_serverless-0.6.35/src/fal_serverless/logging/user.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.34/src/fal_serverless/sdk.py` & `fal_serverless-0.6.35/src/fal_serverless/sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -491,14 +491,23 @@
     def get_activation_logs(self, cron_id: str, activation_id: str) -> list[Log]:
         request = isolate_proto.GetActivationLogsRequest(
             cron_id=cron_id, activation_id=activation_id
         )
         response = self.stub.GetActivationLogs(request)
         return [from_grpc(log) for log in response.logs]
 
+    def get_logs(
+        self, lines: int | None = None, url: str | None = None
+    ) -> Iterator[Log]:
+
+        filter = isolate_proto.LogsFilter(lines=lines, url=url)
+        request = isolate_proto.GetLogsRequest(filter=filter)
+        for partial_result in self.stub.GetLogs(request):
+            yield from_grpc(partial_result.log_entry)
+
     def list_worker_status(self, user_id: str | None = None) -> list[WorkerStatus]:
         request = isolate_proto.WorkerStatusListRequest(user_id=user_id)
         response = self.stub.WorkerStatusList(request)
         return [
             WorkerStatus(
                 ws.worker_id,
                 isolate_proto.datetime_from_timestamp(ws.start_time),
```

### Comparing `fal_serverless-0.6.34/src/fal_serverless/sync.py` & `fal_serverless-0.6.35/src/fal_serverless/sync.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.34/setup.py` & `fal_serverless-0.6.35/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 {'': ['*']}
 
 install_requires = \
 ['auth0-python>=4.1.0,<5.0.0',
  'click>=8.1.3,<9.0.0',
  'colorama>=0.4.6,<0.5.0',
  'datadog-api-client==2.12.0',
- 'dill==0.3.5.1',
+ 'dill>=0.3.6,<0.3.7',
  'grpc-interceptor>=0.15.0,<0.16.0',
  'grpcio>=1.50.0,<2.0.0',
- 'isolate-proto>=0.0.30,<0.0.31',
+ 'isolate-proto>=0.0.31,<0.0.32',
  'isolate[build]>=0.12.2,<1.0',
  'opentelemetry-api>=1.15.0,<2.0.0',
  'opentelemetry-sdk>=1.15.0,<2.0.0',
  'packaging>=21.3',
  'pathspec>=0.11.1,<0.12.0',
  'portalocker>=2.7.0,<3.0.0',
  'requests>=2.28.1,<3.0.0',
@@ -38,15 +38,15 @@
 {':python_version < "3.10"': ['importlib-metadata>=4.4']}
 
 entry_points = \
 {'console_scripts': ['fal-serverless = fal_serverless.cli:cli']}
 
 setup_kwargs = {
     'name': 'fal-serverless',
-    'version': '0.6.34',
+    'version': '0.6.35',
     'description': 'fal Serverless is an easy-to-use Serverless Python Framework',
     'long_description': '# fal-serverless\n\nLibrary to run, serve or schedule your Python functions in the cloud with any machine type you may need.\n\nCheck out to the [docs](https://docs.fal.ai/fal-serverless/quickstart) for more details.\n',
     'author': 'Features & Labels',
     'author_email': 'hello@fal.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `fal_serverless-0.6.34/PKG-INFO` & `fal_serverless-0.6.35/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: fal-serverless
-Version: 0.6.34
+Version: 0.6.35
 Summary: fal Serverless is an easy-to-use Serverless Python Framework
 Author: Features & Labels
 Author-email: hello@fal.ai
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: auth0-python (>=4.1.0,<5.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: datadog-api-client (==2.12.0)
-Requires-Dist: dill (==0.3.5.1)
+Requires-Dist: dill (>=0.3.6,<0.3.7)
 Requires-Dist: grpc-interceptor (>=0.15.0,<0.16.0)
 Requires-Dist: grpcio (>=1.50.0,<2.0.0)
 Requires-Dist: importlib-metadata (>=4.4) ; python_version < "3.10"
-Requires-Dist: isolate-proto (>=0.0.30,<0.0.31)
+Requires-Dist: isolate-proto (>=0.0.31,<0.0.32)
 Requires-Dist: isolate[build] (>=0.12.2,<1.0)
 Requires-Dist: opentelemetry-api (>=1.15.0,<2.0.0)
 Requires-Dist: opentelemetry-sdk (>=1.15.0,<2.0.0)
 Requires-Dist: packaging (>=21.3)
 Requires-Dist: pathspec (>=0.11.1,<0.12.0)
 Requires-Dist: portalocker (>=2.7.0,<3.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
```

