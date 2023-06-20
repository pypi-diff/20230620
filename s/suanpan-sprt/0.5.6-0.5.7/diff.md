# Comparing `tmp/suanpan-sprt-0.5.6.tar.gz` & `tmp/suanpan-sprt-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/suanpan-sprt-0.5.6.tar", last modified: Mon Jun 19 06:23:27 2023, max compression
+gzip compressed data, was "dist/suanpan-sprt-0.5.7.tar", last modified: Tue Jun 20 09:26:43 2023, max compression
```

## Comparing `suanpan-sprt-0.5.6.tar` & `suanpan-sprt-0.5.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-06-19 06:23:27.000000 suanpan-sprt-0.5.6/
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      482 2023-06-19 06:23:27.000000 suanpan-sprt-0.5.6/PKG-INFO
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      129 2023-06-02 08:38:14.000000 suanpan-sprt-0.5.6/README.md
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       38 2023-06-19 06:23:27.000000 suanpan-sprt-0.5.6/setup.cfg
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1073 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.6/setup.py
-drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-06-19 06:23:27.000000 suanpan-sprt-0.5.6/sprt/
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      100 2023-03-13 09:36:01.000000 suanpan-sprt-0.5.6/sprt/__init__.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     5190 2023-06-19 06:23:26.000000 suanpan-sprt-0.5.6/sprt/__main__.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     8168 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.6/sprt/arguments.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1280 2023-04-04 09:18:04.000000 suanpan-sprt-0.5.6/sprt/envs.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      242 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.6/sprt/exceptions.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     4321 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.6/sprt/loader.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     2069 2023-04-04 09:18:04.000000 suanpan-sprt-0.5.6/sprt/log.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      880 2023-04-04 09:18:04.000000 suanpan-sprt-0.5.6/sprt/master.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     5229 2023-06-19 06:23:26.000000 suanpan-sprt-0.5.6/sprt/server.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     6456 2023-04-04 09:18:04.000000 suanpan-sprt-0.5.6/sprt/storage.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     3448 2023-04-04 09:18:04.000000 suanpan-sprt-0.5.6/sprt/testing.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1290 2023-06-02 08:38:14.000000 suanpan-sprt-0.5.6/sprt/utils.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       22 2023-06-19 06:23:26.000000 suanpan-sprt-0.5.6/sprt/version.py
-drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-06-19 06:23:27.000000 suanpan-sprt-0.5.6/suanpan_sprt.egg-info/
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      482 2023-06-19 06:23:27.000000 suanpan-sprt-0.5.6/suanpan_sprt.egg-info/PKG-INFO
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      439 2023-06-19 06:23:27.000000 suanpan-sprt-0.5.6/suanpan_sprt.egg-info/SOURCES.txt
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)        1 2023-06-19 06:23:27.000000 suanpan-sprt-0.5.6/suanpan_sprt.egg-info/dependency_links.txt
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       70 2023-06-19 06:23:27.000000 suanpan-sprt-0.5.6/suanpan_sprt.egg-info/entry_points.txt
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      158 2023-06-19 06:23:27.000000 suanpan-sprt-0.5.6/suanpan_sprt.egg-info/requires.txt
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)        5 2023-06-19 06:23:27.000000 suanpan-sprt-0.5.6/suanpan_sprt.egg-info/top_level.txt
+drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-06-20 09:26:43.000000 suanpan-sprt-0.5.7/
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      482 2023-06-20 09:26:43.000000 suanpan-sprt-0.5.7/PKG-INFO
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      129 2023-06-02 08:38:14.000000 suanpan-sprt-0.5.7/README.md
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       38 2023-06-20 09:26:43.000000 suanpan-sprt-0.5.7/setup.cfg
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1073 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.7/setup.py
+drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-06-20 09:26:43.000000 suanpan-sprt-0.5.7/sprt/
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      100 2023-03-13 09:36:01.000000 suanpan-sprt-0.5.7/sprt/__init__.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     5251 2023-06-20 09:26:42.000000 suanpan-sprt-0.5.7/sprt/__main__.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     8168 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.7/sprt/arguments.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1280 2023-04-04 09:18:04.000000 suanpan-sprt-0.5.7/sprt/envs.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      242 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.7/sprt/exceptions.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     4321 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.7/sprt/loader.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     2069 2023-04-04 09:18:04.000000 suanpan-sprt-0.5.7/sprt/log.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      880 2023-04-04 09:18:04.000000 suanpan-sprt-0.5.7/sprt/master.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     5353 2023-06-20 09:26:42.000000 suanpan-sprt-0.5.7/sprt/server.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     6456 2023-04-04 09:18:04.000000 suanpan-sprt-0.5.7/sprt/storage.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     3448 2023-04-04 09:18:04.000000 suanpan-sprt-0.5.7/sprt/testing.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1290 2023-06-02 08:38:14.000000 suanpan-sprt-0.5.7/sprt/utils.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       22 2023-06-20 09:26:42.000000 suanpan-sprt-0.5.7/sprt/version.py
+drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-06-20 09:26:43.000000 suanpan-sprt-0.5.7/suanpan_sprt.egg-info/
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      482 2023-06-20 09:26:43.000000 suanpan-sprt-0.5.7/suanpan_sprt.egg-info/PKG-INFO
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      439 2023-06-20 09:26:43.000000 suanpan-sprt-0.5.7/suanpan_sprt.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)        1 2023-06-20 09:26:43.000000 suanpan-sprt-0.5.7/suanpan_sprt.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       70 2023-06-20 09:26:43.000000 suanpan-sprt-0.5.7/suanpan_sprt.egg-info/entry_points.txt
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      158 2023-06-20 09:26:43.000000 suanpan-sprt-0.5.7/suanpan_sprt.egg-info/requires.txt
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)        5 2023-06-20 09:26:43.000000 suanpan-sprt-0.5.7/suanpan_sprt.egg-info/top_level.txt
```

### Comparing `suanpan-sprt-0.5.6/setup.py` & `suanpan-sprt-0.5.7/setup.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.5.6/sprt/__main__.py` & `suanpan-sprt-0.5.7/sprt/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,15 @@
                 }
             },
         })
 
     signal.signal(signal.SIGTERM, receive_signal)
     signal.signal(signal.SIGINT, receive_signal)
     app = server.create_app(working_dir, log_file, new_log)
+    app.logger.info(f'use {log_file} {log_level} {new_log}')
 
     config = Config()
     config.bind = [f'{host}:{port}']
     app.logger.info(f'python runtime running on {host}:{port}')
     asyncio.run(serve(app, config))
```

### Comparing `suanpan-sprt-0.5.6/sprt/arguments.py` & `suanpan-sprt-0.5.7/sprt/arguments.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.5.6/sprt/envs.py` & `suanpan-sprt-0.5.7/sprt/envs.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.5.6/sprt/loader.py` & `suanpan-sprt-0.5.7/sprt/loader.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.5.6/sprt/log.py` & `suanpan-sprt-0.5.7/sprt/log.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.5.6/sprt/master.py` & `suanpan-sprt-0.5.7/sprt/master.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.5.6/sprt/server.py` & `suanpan-sprt-0.5.7/sprt/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,17 @@
 
     @app.post("/")
     @validate_request(FunctionParams)
     @validate_response(FunctionResponse)
     async def handle_post(data: FunctionParams) -> FunctionResponse:
         node_id = data.context.node_id
         if new_log:
-            log_name = log_path / f'{logfile_prefix[0]}-{logfile_prefix[1]}-{node_id}'
+            log_dir = log_path / f'{logfile_prefix[0]}-{logfile_prefix[1]}-{node_id}'
+            log_dir.mkdir(parents=True, exist_ok=True)
+            log_name = log_dir / f'app-{logfile_prefix[0]}-{node_id}'
         else:
             log_name = log_path / node_id
         if utils.should_log_rollover(str(log_name)):
             utils.do_log_rollover(str(log_name))
         with open(log_path / node_id, 'a', encoding='utf8') as f:
             with redirect_stdout(f), redirect_stderr(f), node_context(node_id):
                 function = None
```

### Comparing `suanpan-sprt-0.5.6/sprt/storage.py` & `suanpan-sprt-0.5.7/sprt/storage.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.5.6/sprt/testing.py` & `suanpan-sprt-0.5.7/sprt/testing.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.5.6/sprt/utils.py` & `suanpan-sprt-0.5.7/sprt/utils.py`

 * *Files identical despite different names*

