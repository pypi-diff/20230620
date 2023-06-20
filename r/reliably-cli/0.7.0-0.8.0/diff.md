# Comparing `tmp/reliably_cli-0.7.0.tar.gz` & `tmp/reliably_cli-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reliably_cli-0.7.0.tar", last modified: Wed Jun 14 09:03:33 2023, max compression
+gzip compressed data, was "reliably_cli-0.8.0.tar", last modified: Tue Jun 20 12:27:10 2023, max compression
```

## Comparing `reliably_cli-0.7.0.tar` & `reliably_cli-0.8.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11357 2023-06-14 09:03:11.431223 reliably_cli-0.7.0/LICENSE
--rw-r--r--   0        0        0     1478 2023-06-14 09:03:11.431223 reliably_cli-0.7.0/README.md
--rw-r--r--   0        0        0     3015 2023-06-14 09:03:33.520431 reliably_cli-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      114 2023-06-14 09:03:11.435223 reliably_cli-0.7.0/reliably_cli/__init__.py
--rw-r--r--   0        0        0      881 2023-06-14 09:03:11.435223 reliably_cli-0.7.0/reliably_cli/__main__.py
--rw-r--r--   0        0        0      166 2023-06-14 09:03:11.435223 reliably_cli-0.7.0/reliably_cli/__version__.py
--rw-r--r--   0        0        0     1221 2023-06-14 09:03:11.435223 reliably_cli-0.7.0/reliably_cli/agent/__init__.py
--rw-r--r--   0        0        0     1545 2023-06-14 09:03:11.435223 reliably_cli-0.7.0/reliably_cli/agent/cli.py
--rw-r--r--   0        0        0     2770 2023-06-14 09:03:11.435223 reliably_cli-0.7.0/reliably_cli/agent/plan/__init__.py
--rw-r--r--   0        0        0     1352 2023-06-14 09:03:11.435223 reliably_cli-0.7.0/reliably_cli/agent/plan/providers/__init__.py
--rw-r--r--   0        0        0     3493 2023-06-14 09:03:11.435223 reliably_cli-0.7.0/reliably_cli/agent/plan/providers/github.py
--rw-r--r--   0        0        0     1215 2023-06-14 09:03:11.435223 reliably_cli-0.7.0/reliably_cli/client.py
--rw-r--r--   0        0        0     1087 2023-06-14 09:03:11.435223 reliably_cli-0.7.0/reliably_cli/config/__init__.py
--rw-r--r--   0        0        0     3552 2023-06-14 09:03:11.435223 reliably_cli-0.7.0/reliably_cli/config/cli.py
--rw-r--r--   0        0        0     2403 2023-06-14 09:03:11.435223 reliably_cli-0.7.0/reliably_cli/config/types.py
--rw-r--r--   0        0        0      566 2023-06-14 09:03:11.435223 reliably_cli-0.7.0/reliably_cli/format.py
--rw-r--r--   0        0        0      126 2023-06-14 09:03:11.435223 reliably_cli-0.7.0/reliably_cli/log.py
--rw-r--r--   0        0        0        0 2023-06-14 09:03:11.435223 reliably_cli-0.7.0/reliably_cli/services/__init__.py
--rw-r--r--   0        0        0      211 2023-06-14 09:03:11.435223 reliably_cli-0.7.0/reliably_cli/services/cli.py
--rw-r--r--   0        0        0     2388 2023-06-14 09:03:11.435223 reliably_cli-0.7.0/reliably_cli/services/org.py
--rw-r--r--   0        0        0    11933 2023-06-14 09:03:11.435223 reliably_cli-0.7.0/reliably_cli/services/plan.py
--rw-r--r--   0        0        0     2690 2023-06-14 09:03:11.439224 reliably_cli-0.7.0/reliably_cli/types.py
--rw-r--r--   0        0        0      662 2023-06-14 09:03:11.439224 reliably_cli-0.7.0/tests/conftest.py
--rw-r--r--   0        0        0      581 2023-06-14 09:03:11.439224 reliably_cli-0.7.0/tests/test_cli.py
--rw-r--r--   0        0        0     3573 1970-01-01 00:00:00.000000 reliably_cli-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-20 12:26:50.065176 reliably_cli-0.8.0/LICENSE
+-rw-r--r--   0        0        0     1478 2023-06-20 12:26:50.065176 reliably_cli-0.8.0/README.md
+-rw-r--r--   0        0        0     3015 2023-06-20 12:27:10.061474 reliably_cli-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      114 2023-06-20 12:26:50.065176 reliably_cli-0.8.0/reliably_cli/__init__.py
+-rw-r--r--   0        0        0      881 2023-06-20 12:26:50.065176 reliably_cli-0.8.0/reliably_cli/__main__.py
+-rw-r--r--   0        0        0      166 2023-06-20 12:26:50.069176 reliably_cli-0.8.0/reliably_cli/__version__.py
+-rw-r--r--   0        0        0     1221 2023-06-20 12:26:50.069176 reliably_cli-0.8.0/reliably_cli/agent/__init__.py
+-rw-r--r--   0        0        0     1545 2023-06-20 12:26:50.069176 reliably_cli-0.8.0/reliably_cli/agent/cli.py
+-rw-r--r--   0        0        0     2770 2023-06-20 12:26:50.069176 reliably_cli-0.8.0/reliably_cli/agent/plan/__init__.py
+-rw-r--r--   0        0        0     1352 2023-06-20 12:26:50.069176 reliably_cli-0.8.0/reliably_cli/agent/plan/providers/__init__.py
+-rw-r--r--   0        0        0     3493 2023-06-20 12:26:50.069176 reliably_cli-0.8.0/reliably_cli/agent/plan/providers/github.py
+-rw-r--r--   0        0        0     1215 2023-06-20 12:26:50.069176 reliably_cli-0.8.0/reliably_cli/client.py
+-rw-r--r--   0        0        0     1087 2023-06-20 12:26:50.069176 reliably_cli-0.8.0/reliably_cli/config/__init__.py
+-rw-r--r--   0        0        0     3552 2023-06-20 12:26:50.069176 reliably_cli-0.8.0/reliably_cli/config/cli.py
+-rw-r--r--   0        0        0     2403 2023-06-20 12:26:50.069176 reliably_cli-0.8.0/reliably_cli/config/types.py
+-rw-r--r--   0        0        0      566 2023-06-20 12:26:50.069176 reliably_cli-0.8.0/reliably_cli/format.py
+-rw-r--r--   0        0        0      126 2023-06-20 12:26:50.069176 reliably_cli-0.8.0/reliably_cli/log.py
+-rw-r--r--   0        0        0        0 2023-06-20 12:26:50.069176 reliably_cli-0.8.0/reliably_cli/services/__init__.py
+-rw-r--r--   0        0        0      211 2023-06-20 12:26:50.069176 reliably_cli-0.8.0/reliably_cli/services/cli.py
+-rw-r--r--   0        0        0     2388 2023-06-20 12:26:50.069176 reliably_cli-0.8.0/reliably_cli/services/org.py
+-rw-r--r--   0        0        0    12455 2023-06-20 12:26:50.069176 reliably_cli-0.8.0/reliably_cli/services/plan.py
+-rw-r--r--   0        0        0     2690 2023-06-20 12:26:50.069176 reliably_cli-0.8.0/reliably_cli/types.py
+-rw-r--r--   0        0        0      662 2023-06-20 12:26:50.069176 reliably_cli-0.8.0/tests/conftest.py
+-rw-r--r--   0        0        0      581 2023-06-20 12:26:50.069176 reliably_cli-0.8.0/tests/test_cli.py
+-rw-r--r--   0        0        0     3573 1970-01-01 00:00:00.000000 reliably_cli-0.8.0/PKG-INFO
```

### Comparing `reliably_cli-0.7.0/LICENSE` & `reliably_cli-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.7.0/README.md` & `reliably_cli-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.7.0/pyproject.toml` & `reliably_cli-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     "rich>=13.3.1",
     "chaostoolkit-addons>=0.4.0",
     "chaostoolkit>=1.15.0",
     "chaostoolkit-lib>=1.33.1",
     "chaostoolkit-reliably>=0.22.0",
     "orjson>=3.8.10",
 ]
-version = "0.7.0"
+version = "0.8.0"
 
 [project.license]
 text = "Apache-2.0"
 
 [project.urls]
 Homepage = "https://reliably.com/"
 Repository = "https://github.com/reliablyhq/cli"
```

### Comparing `reliably_cli-0.7.0/reliably_cli/__main__.py` & `reliably_cli-0.8.0/reliably_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.7.0/reliably_cli/agent/__init__.py` & `reliably_cli-0.8.0/reliably_cli/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.7.0/reliably_cli/agent/cli.py` & `reliably_cli-0.8.0/reliably_cli/agent/cli.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.7.0/reliably_cli/agent/plan/__init__.py` & `reliably_cli-0.8.0/reliably_cli/agent/plan/__init__.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.7.0/reliably_cli/agent/plan/providers/__init__.py` & `reliably_cli-0.8.0/reliably_cli/agent/plan/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.7.0/reliably_cli/agent/plan/providers/github.py` & `reliably_cli-0.8.0/reliably_cli/agent/plan/providers/github.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.7.0/reliably_cli/client.py` & `reliably_cli-0.8.0/reliably_cli/client.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.7.0/reliably_cli/config/__init__.py` & `reliably_cli-0.8.0/reliably_cli/config/__init__.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.7.0/reliably_cli/config/cli.py` & `reliably_cli-0.8.0/reliably_cli/config/cli.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.7.0/reliably_cli/config/types.py` & `reliably_cli-0.8.0/reliably_cli/config/types.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.7.0/reliably_cli/format.py` & `reliably_cli-0.8.0/reliably_cli/format.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.7.0/reliably_cli/services/org.py` & `reliably_cli-0.8.0/reliably_cli/services/org.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.7.0/reliably_cli/services/plan.py` & `reliably_cli-0.8.0/reliably_cli/services/plan.py`

 * *Files 8% similar despite different names*

```diff
@@ -82,18 +82,19 @@
 ) -> None:
     """
     Execute a plan
     """
     ensure_config_is_set()
 
     p = load_plan(plan_id)
+    tempdir = tempfile.TemporaryDirectory()
 
     context = {}
     if not skip_context:
-        context = store_plan_context(p)
+        context = store_plan_context(p, tempdir.name)
 
     settings = get_settings()
 
     if os.getenv("RELIABLY_HOST") is None:
         os.environ["RELIABLY_HOST"] = settings.service.host.replace(
             "https://", ""
         )
@@ -107,15 +108,14 @@
 
     experiment_id = p.definition.experiments[0]
     base_url = f"{settings.service.host}/api/v1/organization"
     base_url = f"{base_url}/{settings.organization.id}"
     experiment_url = f"{base_url}/experiments/{experiment_id}/raw"
 
     if load_environment:
-        tempdir = tempfile.TemporaryDirectory()
         load_environment_into_memory(p, tempdir.name)
 
     with console.status("Executing..."):
         if set_status:
             send_status(p.id, "running")
 
         with reconfigure_chaostoolkit_logger(log_file, log_stdout):
@@ -154,20 +154,33 @@
             elif r.status_code > 399:
                 console.print(f"unexpected error: {r.status_code}: {r.json()}")
                 raise typer.Exit(code=1)
 
             return Plan.parse_obj(r.json())
 
 
-def store_plan_context(plan: Plan) -> dict[str, Any]:
+def store_plan_context(plan: Plan, target_dir: str) -> dict[str, Any]:
     global_controls = {}
 
     with console.status("Storing context..."):
         with api_client() as client:
             for int_id in plan.definition.integrations:
+                r = client.get(f"/integrations/{int_id}")
+                if r.status_code > 399:
+                    console.print(
+                        f"Plan references integration {int_id} which does "
+                        "not exist"
+                    )
+                    continue
+
+                control = r.json()
+                env_id = control.get("environment_id")
+                if env_id:
+                    load_environment(env_id, target_dir)
+
                 r = client.get(f"/integrations/{int_id}/control")
                 control = r.json()
                 if control:
                     ctrl_name = control.pop("name")
                     provider = control.get("provider", {})
                     if "secrets" in provider and provider["secrets"] is None:
                         del provider["secrets"]
@@ -183,42 +196,46 @@
 
 
 def load_environment_into_memory(plan: Plan, target_dir: str) -> None:
     with console.status("Loading environment..."):
         if not plan.definition.environment:
             return None
 
-        with api_client() as client:
-            env_id = str(plan.definition.environment.id)
-            r = client.get(f"/environments/{env_id}/clear")
-            env = Environment.parse_obj(r.json())
-            if env:
-                path_mapping = {}
-                for s in env.secrets.__root__:
-                    if isinstance(s, EnvironmentSecretAsFile):
-                        new_path = Path(target_dir, s.path.lstrip("/"))
-                        new_path.parent.mkdir(mode=0o710, parents=True)
-                        new_path.write_text(s.value.get_secret_value())
-                        new_path.chmod(0o770)
-
-                        path_mapping[s.path] = str(new_path)
-
-                for e in env.envvars.__root__:
-                    if e.value in path_mapping:
-                        os.environ[e.var_name] = path_mapping[e.value]
-                    else:
-                        os.environ[e.var_name] = e.value
+        env_id = str(plan.definition.environment.id)
+        load_environment(env_id, target_dir)
+
 
-                for s in env.secrets.__root__:
-                    if isinstance(s, EnvironmentSecret):
-                        v = s.value.get_secret_value()
-                        if v in path_mapping:
-                            os.environ[s.var_name] = path_mapping[v]
-                        else:
-                            os.environ[s.var_name] = v
+def load_environment(environment_id: str, target_dir: str) -> None:
+    with api_client() as client:
+        r = client.get(f"/environments/{environment_id}/clear")
+        env = Environment.parse_obj(r.json())
+        if env:
+            path_mapping = {}
+            for s in env.secrets.__root__:
+                if isinstance(s, EnvironmentSecretAsFile):
+                    new_path = Path(target_dir, s.path.lstrip("/"))
+                    new_path.parent.mkdir(mode=0o710, parents=True)
+                    new_path.write_text(s.value.get_secret_value())
+                    new_path.chmod(0o770)
+
+                    path_mapping[s.path] = str(new_path)
+
+            for e in env.envvars.__root__:
+                if e.value in path_mapping:
+                    os.environ[e.var_name] = path_mapping[e.value]
+                else:
+                    os.environ[e.var_name] = e.value
+
+            for s in env.secrets.__root__:
+                if isinstance(s, EnvironmentSecret):
+                    v = s.value.get_secret_value()
+                    if v in path_mapping:
+                        os.environ[s.var_name] = path_mapping[v]
+                    else:
+                        os.environ[s.var_name] = v
 
 
 def send_status(plan_id: UUID, status: str, error: str | None = None) -> None:
     with api_client() as client:
         payload = {"status": status, "error": error}
         r = client.put(f"/plans/{str(plan_id)}/status", json=payload)
         if r.status_code == 404:
```

### Comparing `reliably_cli-0.7.0/reliably_cli/types.py` & `reliably_cli-0.8.0/reliably_cli/types.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.7.0/tests/conftest.py` & `reliably_cli-0.8.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.7.0/tests/test_cli.py` & `reliably_cli-0.8.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.7.0/PKG-INFO` & `reliably_cli-0.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reliably-cli
-Version: 0.7.0
+Version: 0.8.0
 Summary: Reliably CLI
 Author-Email: Sylvain Hellegouarch <sylvain@reliably.com>
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: reliably-cli Version: 0.7.0 Summary: Reliably CLI
+Metadata-Version: 2.1 Name: reliably-cli Version: 0.8.0 Summary: Reliably CLI
 Author-Email: Sylvain Hellegouarch
 reliably.com> License: Apache-2.0 Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Development Status :: 4 - Beta Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: Utilities Project-URL: Homepage, https://reliably.com/
```

