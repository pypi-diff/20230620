# Comparing `tmp/remotivelabs_cli-0.0.1a3.tar.gz` & `tmp/remotivelabs_cli-0.0.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remotivelabs_cli-0.0.1a3.tar", max compression
+gzip compressed data, was "remotivelabs_cli-0.0.1a4.tar", max compression
```

## Comparing `remotivelabs_cli-0.0.1a3.tar` & `remotivelabs_cli-0.0.1a4.tar`

### file list

```diff
@@ -1,20 +1,23 @@
--rw-r--r--   0        0        0     2092 2023-06-18 17:01:10.908056 remotivelabs_cli-0.0.1a3/README.md
--rw-r--r--   0        0        0      122 2022-10-26 14:05:47.581000 remotivelabs_cli-0.0.1a3/cli/__about__.py
--rw-r--r--   0        0        0       26 2022-10-26 11:41:55.030088 remotivelabs_cli-0.0.1a3/cli/__init__.py
--rw-r--r--   0        0        0     2910 2023-06-19 13:36:54.800059 remotivelabs_cli-0.0.1a3/cli/brokers.py
--rw-r--r--   0        0        0        1 2022-10-24 12:45:02.134227 remotivelabs_cli-0.0.1a3/cli/cloud/__init__.py
--rw-r--r--   0        0        0     3675 2023-06-09 11:46:02.064612 remotivelabs_cli-0.0.1a3/cli/cloud/auth.py
--rw-r--r--   0        0        0     2284 2023-05-30 06:23:51.161239 remotivelabs_cli-0.0.1a3/cli/cloud/brokers.py
--rw-r--r--   0        0        0     1605 2023-06-19 13:52:07.761595 remotivelabs_cli-0.0.1a3/cli/cloud/cloud_cli.py
--rw-r--r--   0        0        0     3132 2023-06-19 13:52:07.776885 remotivelabs_cli-0.0.1a3/cli/cloud/configs.py
--rw-r--r--   0        0        0     6887 2023-06-19 12:26:04.278978 remotivelabs_cli-0.0.1a3/cli/cloud/recordings.py
--rw-r--r--   0        0        0     2861 2023-06-09 09:54:06.620182 remotivelabs_cli-0.0.1a3/cli/cloud/rest_helper.py
--rw-r--r--   0        0        0     1580 2023-06-09 11:33:01.362939 remotivelabs_cli-0.0.1a3/cli/cloud/service_account_keys.py
--rw-r--r--   0        0        0     1176 2023-06-19 13:50:30.024795 remotivelabs_cli-0.0.1a3/cli/cloud/service_accounts.py
--rw-r--r--   0        0        0      141 2022-10-25 14:33:01.608000 remotivelabs_cli-0.0.1a3/cli/lib/__about__.py
--rw-r--r--   0        0        0     4905 2022-10-20 06:14:07.629916 remotivelabs_cli-0.0.1a3/cli/lib/broker.py
--rw-r--r--   0        0        0      292 2023-06-19 13:37:13.805682 remotivelabs_cli-0.0.1a3/cli/remotive.py
--rw-r--r--   0        0        0       77 2023-06-08 06:07:23.995982 remotivelabs_cli-0.0.1a3/cli/requirements.txt
--rw-r--r--   0        0        0       63 2023-03-21 06:24:07.422989 remotivelabs_cli-0.0.1a3/cli/test/test_simple.py
--rw-r--r--   0        0        0      535 2023-06-19 13:52:43.274331 remotivelabs_cli-0.0.1a3/pyproject.toml
--rw-r--r--   0        0        0     2744 1970-01-01 00:00:00.000000 remotivelabs_cli-0.0.1a3/PKG-INFO
+-rw-r--r--   0        0        0      608 2023-06-19 13:55:54.232642 remotivelabs_cli-0.0.1a4/LICENSE
+-rw-r--r--   0        0        0     2092 2023-06-18 17:01:10.908056 remotivelabs_cli-0.0.1a4/README.md
+-rw-r--r--   0        0        0      122 2022-10-26 14:05:47.581000 remotivelabs_cli-0.0.1a4/cli/__about__.py
+-rw-r--r--   0        0        0       26 2022-10-26 11:41:55.030088 remotivelabs_cli-0.0.1a4/cli/__init__.py
+-rw-r--r--   0        0        0     2910 2023-06-19 13:36:54.800059 remotivelabs_cli-0.0.1a4/cli/brokers.py
+-rw-r--r--   0        0        0        1 2022-10-24 12:45:02.134227 remotivelabs_cli-0.0.1a4/cli/cloud/__init__.py
+-rw-r--r--   0        0        0     3875 2023-06-20 11:44:37.485261 remotivelabs_cli-0.0.1a4/cli/cloud/auth.py
+-rw-r--r--   0        0        0     1392 2023-06-20 08:34:18.147931 remotivelabs_cli-0.0.1a4/cli/cloud/auth_keys.py
+-rw-r--r--   0        0        0     2306 2023-06-20 11:51:25.452149 remotivelabs_cli-0.0.1a4/cli/cloud/brokers.py
+-rw-r--r--   0        0        0     1611 2023-06-20 11:54:09.099670 remotivelabs_cli-0.0.1a4/cli/cloud/cloud_cli.py
+-rw-r--r--   0        0        0     3132 2023-06-19 13:52:07.776885 remotivelabs_cli-0.0.1a4/cli/cloud/configs.py
+-rw-r--r--   0        0        0     1083 2023-06-20 12:47:24.741759 remotivelabs_cli-0.0.1a4/cli/cloud/projects.py
+-rw-r--r--   0        0        0     6887 2023-06-19 12:26:04.278978 remotivelabs_cli-0.0.1a4/cli/cloud/recordings.py
+-rw-r--r--   0        0        0     2979 2023-06-20 12:44:49.774042 remotivelabs_cli-0.0.1a4/cli/cloud/rest_helper.py
+-rw-r--r--   0        0        0     1990 2023-06-20 13:21:18.023240 remotivelabs_cli-0.0.1a4/cli/cloud/service_account_keys.py
+-rw-r--r--   0        0        0     1176 2023-06-19 13:50:30.024795 remotivelabs_cli-0.0.1a4/cli/cloud/service_accounts.py
+-rw-r--r--   0        0        0      141 2022-10-25 14:33:01.608000 remotivelabs_cli-0.0.1a4/cli/lib/__about__.py
+-rw-r--r--   0        0        0     4905 2022-10-20 06:14:07.629916 remotivelabs_cli-0.0.1a4/cli/lib/broker.py
+-rw-r--r--   0        0        0      315 2023-06-20 11:51:00.031101 remotivelabs_cli-0.0.1a4/cli/remotive.py
+-rw-r--r--   0        0        0       77 2023-06-08 06:07:23.995982 remotivelabs_cli-0.0.1a4/cli/requirements.txt
+-rw-r--r--   0        0        0       63 2023-03-21 06:24:07.422989 remotivelabs_cli-0.0.1a4/cli/test/test_simple.py
+-rw-r--r--   0        0        0      498 2023-06-20 13:26:20.274638 remotivelabs_cli-0.0.1a4/pyproject.toml
+-rw-r--r--   0        0        0     2744 1970-01-01 00:00:00.000000 remotivelabs_cli-0.0.1a4/PKG-INFO
```

### Comparing `remotivelabs_cli-0.0.1a3/README.md` & `remotivelabs_cli-0.0.1a4/README.md`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a3/cli/brokers.py` & `remotivelabs_cli-0.0.1a4/cli/brokers.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a3/cli/cloud/auth.py` & `remotivelabs_cli-0.0.1a4/cli/cloud/auth.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,27 +4,29 @@
 import time
 import webbrowser
 from http.server import BaseHTTPRequestHandler, HTTPServer
 from pathlib import Path
 from threading import Thread
 import typer
 from . import rest_helper as rest
+from . import auth_keys
 
 app = typer.Typer()
-
+app.add_typer(auth_keys.app, name="keys", help="Manage users personal access keys")
 config_dir_name = str(Path.home()) + "/.config/.remotive/"
 token_file_name = str(Path.home()) + "/.config/.remotive/cloud.secret.token"
 
 
+
 class S(BaseHTTPRequestHandler):
     def _set_response(self):
         self.send_response(200)
-        #self.send_response(301)
-        #self.send_header('Location', 'https://cloud.remotivelabs.com')
-        #self.end_headers()
+        # self.send_response(301)
+        # self.send_header('Location', 'https://cloud.remotivelabs.com')
+        # self.end_headers()
         self.send_header('Content-type', 'text/html')
         self.end_headers()
 
     def log_message(self, format, *args):
         return
 
     def do_GET(self):
@@ -51,34 +53,40 @@
 
 
 @app.command(help="Login to the cloud")
 def login():
     webbrowser.open(f'{rest.base_url}/login?redirectUrl=http://localhost:8089', new=1, autoraise=True)
     start_local_webserver()
 
+@app.command(help="Who am I?")
+def whoami():
+    rest.handle_get('/api/whoami')
 
 @app.command(help="Print access token")
 def print_access_token():
     print(read_token())
 
+
 @app.command(help="List available auth tokens")
 def list():
     for file in os.listdir(config_dir_name):
         print(file)
 
+
 @app.command(help="Show token file")
 def describe(
         file: str = typer.Option(..., help="File name")):
     print(read_file(file))
 
 
+
+
 @app.command(help="Activate the account file")
 def activate(
         file: str = typer.Option(..., help="File name")):
-
     # Best effort to read file
     if os.path.exists(file):
         token_file = json.loads(read_file_with_path(file))
         write_token(token_file['token'])
     elif os.path.exists(str(Path.home()) + f"/.config/.remotive/{file}"):
         token_file = json.loads(read_file(file))
         write_token(token_file['token'])
@@ -102,31 +110,37 @@
 
 def read_token():
     f = open(token_file_name, "r")
     token = f.read()
     f.close()
     return token
 
+
 def read_file_with_path(file):
     f = open(file, "r")
     token = f.read()
     f.close()
     return token
 
+
 def read_file(file):
     f = open(str(Path.home()) + f"/.config/.remotive/{file}", "r")
     token = f.read()
     f.close()
     return token
 
+
 def write_token(token):
     f = open(token_file_name, "w")
     f.write(token)
     f.close()
 
+
+
+
 # Key stuff
 # f = open(str(Path.home())+ "/.remotivelabs/privatekey.json", "r")
 # j = json.loads(f.read())
 # print(j['privateKey'])
 # key = load_pem_private_key(bytes(j['privateKey'],'UTF-8'), None)
 # print(key.key_size)
 #
```

### Comparing `remotivelabs_cli-0.0.1a3/cli/cloud/brokers.py` & `remotivelabs_cli-0.0.1a4/cli/cloud/brokers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import typer
 import json
 from rich.progress import Progress, SpinnerColumn, TextColumn
 from . import rest_helper as rest
-
+from rich import print
 app = typer.Typer()
 
 
 @app.command("list", help="Lists brokers in project")
 def list(project: str = typer.Option(..., help="Project ID", envvar='REMOTIVE_CLOUD_PROJECT')):
     rest.handle_get(f"/api/project/{project}/brokers")
```

### Comparing `remotivelabs_cli-0.0.1a3/cli/cloud/cloud_cli.py` & `remotivelabs_cli-0.0.1a4/cli/cloud/cloud_cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 import typer
 
-from . import recordings, brokers, configs, auth, service_accounts
+from . import recordings, brokers, configs, auth, service_accounts, projects
 from . import rest_helper as rest
 
 app = typer.Typer()
 
 
-@app.command(help="Who am I?")
-def whoami():
-    rest.handle_get('/api/whoami')
-
-
 @app.command(help="List licenses for an organisation")
 def licenses(
         organisation: str = typer.Option(..., help="Organisation ID", envvar='REMOTIVE_CLOUD_ORGANISATION'),
         filter: str = typer.Option("all", help="all, valid, expired")
 ):
     rest.handle_get(f"/api/bu/{organisation}/licenses", {'filter': filter})
 
@@ -34,16 +29,17 @@
 @app.command(help="List users in an organisation")
 def users(
         organisation: str = typer.Option(..., help="Organisation ID", envvar='REMOTIVE_CLOUD_ORGANISATION'),
 ):
     rest.handle_get(f"/api/bu/{organisation}/users")
 
 
+app.add_typer(projects.app, name="projects", help="Manage projects")
+app.add_typer(auth.app, name="auth", help="Manage access to cloud resources")
 app.add_typer(brokers.app, name="brokers", help="Manage cloud broker lifecycle")
 app.add_typer(recordings.app, name="recordings", help="Manage recordings")
-app.add_typer(configs.app, name="configs", help="Manage signal databases")
-app.add_typer(auth.app, name="auth", help="Manage access to cloud resources")
+app.add_typer(configs.app, name="signal-databases", help="Manage signal databases")
 app.add_typer(service_accounts.app, name="service-accounts", help="Manage project service account keys")
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `remotivelabs_cli-0.0.1a3/cli/cloud/configs.py` & `remotivelabs_cli-0.0.1a4/cli/cloud/configs.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a3/cli/cloud/recordings.py` & `remotivelabs_cli-0.0.1a4/cli/cloud/recordings.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a3/cli/cloud/rest_helper.py` & `remotivelabs_cli-0.0.1a4/cli/cloud/rest_helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import requests
 import os
 import json
 import logging
 from pathlib import Path
 from os.path import exists
-
+#from rich import print
 import typer
 
 if 'REMOTIVE_CLOUD_HTTP_LOGGING' in os.environ:
     logging.basicConfig()
     logging.getLogger().setLevel(logging.DEBUG)
     requests_log = logging.getLogger("requests.packages.urllib3")
     requests_log.setLevel(logging.DEBUG)
@@ -47,17 +47,21 @@
     f = open(str(Path.home()) + "/.config/.remotive/cloud.secret.token", "r")
     token = f.read()
     os.environ['REMOTIVE_CLOUD_AUTH_TOKEN'] = token
     global headers
     headers = {"Authorization": "Bearer " + token.strip()}
 
 
-def handle_get(url, params={}):
+def handle_get(url, params={},return_response: bool = False):
     ensure_auth_token()
     r = requests.get(f'{base_url}{url}', headers=headers, params=params)
+
+    if return_response:
+        return r
+
     if r.status_code == 200:
         print(json.dumps(r.json()))
     else:
         sys.stderr.write(f'Got status code: {r.status_code}\n')
         sys.stderr.write(r.text + "\n")
 
 
@@ -93,7 +97,8 @@
     if r.status_code == 200:
         print(r.text)
         # print(json.dumps(r.json()))
     elif r.status_code == 204:
         print(r.status_code)
     else:
         print(f'Got status code: {r.status_code}')
+        print(r.text)
```

### Comparing `remotivelabs_cli-0.0.1a3/cli/cloud/service_account_keys.py` & `remotivelabs_cli-0.0.1a4/cli/cloud/service_account_keys.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,13 +31,21 @@
 @app.command(name="list", help="List service-account keys")
 def list_keys(
         service_account: str = typer.Option(..., help="Service account name"),
         project: str = typer.Option(..., help="Project ID", envvar='REMOTIVE_CLOUD_PROJECT')):
     rest.handle_get(f"/api/project/{project}/admin/accounts/{service_account}/keys")
 
 
+@app.command(name="revoke", help="Revoke service account key")
+def revoke(
+        service_account: str = typer.Option(..., help="Service account name"),
+        key_name: str = typer.Option(..., help="Key name"),
+        project: str = typer.Option(..., help="Project ID", envvar='REMOTIVE_CLOUD_PROJECT')):
+    rest.handle_delete(f"/api/project/{project}/admin/accounts/{service_account}/keys/{key_name}")
+
+
 def write_token(file, token):
     path = str(Path.home()) + f"/.config/.remotive/{file}"
     f = open(path, "w")
     f.write(token)
     f.close()
     print(f"Secret token written to {path}")
```

### Comparing `remotivelabs_cli-0.0.1a3/cli/cloud/service_accounts.py` & `remotivelabs_cli-0.0.1a4/cli/cloud/service_accounts.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a3/cli/lib/broker.py` & `remotivelabs_cli-0.0.1a4/cli/lib/broker.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a3/PKG-INFO` & `remotivelabs_cli-0.0.1a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotivelabs-cli
-Version: 0.0.1a3
+Version: 0.0.1a4
 Summary: 
 Author: Johan Rask
 Author-email: johan.rask@remotivelabs.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

