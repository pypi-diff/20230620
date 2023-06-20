# Comparing `tmp/fastdeploy-2.2.7rc4.tar.gz` & `tmp/fastdeploy-2.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastdeploy-2.2.7rc4.tar", last modified: Tue Mar 21 10:42:39 2023, max compression
+gzip compressed data, was "fastdeploy-2.2.8.tar", last modified: Thu Apr 20 07:36:41 2023, max compression
```

## Comparing `fastdeploy-2.2.7rc4.tar` & `fastdeploy-2.2.8.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 10:42:39.431656 fastdeploy-2.2.7rc4/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-21 10:35:52.000000 fastdeploy-2.2.7rc4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-03-21 10:35:52.000000 fastdeploy-2.2.7rc4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-03-21 10:42:39.427656 fastdeploy-2.2.7rc4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-03-21 10:35:52.000000 fastdeploy-2.2.7rc4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 10:42:39.427656 fastdeploy-2.2.7rc4/fastdeploy/
--rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-03-21 10:35:52.000000 fastdeploy-2.2.7rc4/fastdeploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-03-21 10:35:52.000000 fastdeploy-2.2.7rc4/fastdeploy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-03-21 10:35:52.000000 fastdeploy-2.2.7rc4/fastdeploy/_app.py
--rw-r--r--   0 runner    (1001) docker     (123)    11284 2023-03-21 10:35:52.000000 fastdeploy-2.2.7rc4/fastdeploy/_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-03-21 10:35:52.000000 fastdeploy-2.2.7rc4/fastdeploy/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9201 2023-03-21 10:35:52.000000 fastdeploy-2.2.7rc4/fastdeploy/_ws.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 10:42:39.427656 fastdeploy-2.2.7rc4/fastdeploy/fastdeploy-ui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 10:42:39.427656 fastdeploy-2.2.7rc4/fastdeploy/fastdeploy-ui/build/
--rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-03-21 10:42:29.000000 fastdeploy-2.2.7rc4/fastdeploy/fastdeploy-ui/build/bundle.css
--rw-r--r--   0 runner    (1001) docker     (123)   180407 2023-03-21 10:42:29.000000 fastdeploy-2.2.7rc4/fastdeploy/fastdeploy-ui/build/bundle.js
--rw-r--r--   0 runner    (1001) docker     (123)   353573 2023-03-21 10:42:29.000000 fastdeploy-2.2.7rc4/fastdeploy/fastdeploy-ui/build/bundle.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-03-21 10:35:52.000000 fastdeploy-2.2.7rc4/fastdeploy/fastdeploy-ui/favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-03-21 10:35:52.000000 fastdeploy-2.2.7rc4/fastdeploy/fastdeploy-ui/global.css
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-03-21 10:35:52.000000 fastdeploy-2.2.7rc4/fastdeploy/fastdeploy-ui/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 10:42:39.427656 fastdeploy-2.2.7rc4/fastdeploy-ui/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-21 10:35:52.000000 fastdeploy-2.2.7rc4/fastdeploy-ui/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-03-21 10:35:52.000000 fastdeploy-2.2.7rc4/fastdeploy-ui/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   108863 2023-03-21 10:35:52.000000 fastdeploy-2.2.7rc4/fastdeploy-ui/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-03-21 10:35:52.000000 fastdeploy-2.2.7rc4/fastdeploy-ui/package.json
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-03-21 10:35:52.000000 fastdeploy-2.2.7rc4/fastdeploy-ui/rollup.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 10:42:39.427656 fastdeploy-2.2.7rc4/fastdeploy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-03-21 10:42:39.000000 fastdeploy-2.2.7rc4/fastdeploy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-03-21 10:42:39.000000 fastdeploy-2.2.7rc4/fastdeploy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 10:42:39.000000 fastdeploy-2.2.7rc4/fastdeploy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-21 10:42:39.000000 fastdeploy-2.2.7rc4/fastdeploy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-21 10:42:39.000000 fastdeploy-2.2.7rc4/fastdeploy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-21 10:42:39.000000 fastdeploy-2.2.7rc4/fastdeploy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-21 10:42:39.431656 fastdeploy-2.2.7rc4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-03-21 10:35:52.000000 fastdeploy-2.2.7rc4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:36:41.923997 fastdeploy-2.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-20 07:29:08.000000 fastdeploy-2.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-20 07:29:08.000000 fastdeploy-2.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-04-20 07:36:41.923997 fastdeploy-2.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-04-20 07:29:08.000000 fastdeploy-2.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:36:41.923997 fastdeploy-2.2.8/fastdeploy/
+-rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-04-20 07:29:08.000000 fastdeploy-2.2.8/fastdeploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-04-20 07:29:08.000000 fastdeploy-2.2.8/fastdeploy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12869 2023-04-20 07:29:08.000000 fastdeploy-2.2.8/fastdeploy/_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11284 2023-04-20 07:29:08.000000 fastdeploy-2.2.8/fastdeploy/_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-04-20 07:29:08.000000 fastdeploy-2.2.8/fastdeploy/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9201 2023-04-20 07:29:08.000000 fastdeploy-2.2.8/fastdeploy/_ws.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:36:41.923997 fastdeploy-2.2.8/fastdeploy/fastdeploy-ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:36:41.923997 fastdeploy-2.2.8/fastdeploy/fastdeploy-ui/build/
+-rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-04-20 07:36:31.000000 fastdeploy-2.2.8/fastdeploy/fastdeploy-ui/build/bundle.css
+-rw-r--r--   0 runner    (1001) docker     (123)   180407 2023-04-20 07:36:31.000000 fastdeploy-2.2.8/fastdeploy/fastdeploy-ui/build/bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)   353573 2023-04-20 07:36:31.000000 fastdeploy-2.2.8/fastdeploy/fastdeploy-ui/build/bundle.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-04-20 07:29:08.000000 fastdeploy-2.2.8/fastdeploy/fastdeploy-ui/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-20 07:29:08.000000 fastdeploy-2.2.8/fastdeploy/fastdeploy-ui/global.css
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-20 07:29:08.000000 fastdeploy-2.2.8/fastdeploy/fastdeploy-ui/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:36:41.923997 fastdeploy-2.2.8/fastdeploy-ui/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-20 07:29:08.000000 fastdeploy-2.2.8/fastdeploy-ui/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-04-20 07:29:08.000000 fastdeploy-2.2.8/fastdeploy-ui/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   108863 2023-04-20 07:29:08.000000 fastdeploy-2.2.8/fastdeploy-ui/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-20 07:29:08.000000 fastdeploy-2.2.8/fastdeploy-ui/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-20 07:29:08.000000 fastdeploy-2.2.8/fastdeploy-ui/rollup.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:36:41.923997 fastdeploy-2.2.8/fastdeploy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-04-20 07:36:41.000000 fastdeploy-2.2.8/fastdeploy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-20 07:36:41.000000 fastdeploy-2.2.8/fastdeploy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 07:36:41.000000 fastdeploy-2.2.8/fastdeploy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-20 07:36:41.000000 fastdeploy-2.2.8/fastdeploy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-20 07:36:41.000000 fastdeploy-2.2.8/fastdeploy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-20 07:36:41.000000 fastdeploy-2.2.8/fastdeploy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 07:36:41.923997 fastdeploy-2.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-04-20 07:29:08.000000 fastdeploy-2.2.8/setup.py
```

### Comparing `fastdeploy-2.2.7rc4/LICENSE` & `fastdeploy-2.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fastdeploy-2.2.7rc4/PKG-INFO` & `fastdeploy-2.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastdeploy
-Version: 2.2.7rc4
+Version: 2.2.8
 Summary: Deploy DL/ ML inference pipelines with minimal extra code. 
 Home-page: https://github.com/notAI-tech/fastDeploy
 Author: BEDAPUDI PRANEETH
 Author-email: praneeth@bpraneeth.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `fastdeploy-2.2.7rc4/README.md` & `fastdeploy-2.2.8/README.md`

 * *Files identical despite different names*

### Comparing `fastdeploy-2.2.7rc4/fastdeploy/__init__.py` & `fastdeploy-2.2.8/fastdeploy/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         help="Path to your recipe folder; env: RECIPE",
         required=True,
     )
 
     parser.add_argument(
         "--mode",
         type=str,
-        help='One of, ["loop", "rest", "websocket", "build_rest"]; env: MODE',
+        help='One of, ["loop", "rest", "websocket", "build_rest", "build_rest_no_loop"]; env: MODE',
         required=True,
     )
 
     parser.add_argument(
         "--queue_dir",
         type=str,
         help='Defaults to "--recipe" folder; end: QUEUE_DIR',
@@ -61,14 +61,18 @@
     )
 
     args = parser.parse_args()
 
     QUEUE_DIR = os.path.join(os.path.abspath(args.recipe), "fastdeploy_dbs")
 
     MODE = args.mode
+    if MODE == "build_no_loop_rest":
+        MODE = "build_rest"
+        os.environ["NO_LOOP"] = True
+
     RECIPE = os.path.abspath(args.recipe)
     BASE = args.base
     DOCKER_ARGS = args.docker_args
     if not DOCKER_ARGS:
         DOCKER_ARGS = ""
 
 if os.path.exists(RECIPE):
@@ -185,17 +189,23 @@
     )
 
     dockerfile_lines.append(
         f'ENTRYPOINT {os.getenv("ENTRYPOINT", ["/bin/sh", "-c"])} \n'.replace("'", '"')
     )
 
     if mode == "build_rest":
-        dockerfile_lines.append(
-            f'CMD ["ulimit -n 1000000 && python3 -m fastdeploy --recipe {recipe_base_name} --mode loop & python3 -m fastdeploy --recipe {recipe_base_name} --mode rest"] \n'
-        )
+        if os.getenv("NO_LOOP"):
+            dockerfile_lines.append(
+                f'CMD ["ulimit -n 1000000 && NO_LOOP=true python3 -m fastdeploy --recipe {recipe_base_name} --mode rest"] \n'
+            )
+
+        else:
+            dockerfile_lines.append(
+                f'CMD ["ulimit -n 1000000 && python3 -m fastdeploy --recipe {recipe_base_name} --mode loop & python3 -m fastdeploy --recipe {recipe_base_name} --mode rest"] \n'
+            )
     elif mode == "build_websocket":
         dockerfile_lines.append(
             f'CMD ["ulimit -n 1000000 && python3 -m fastdeploy --recipe {recipe_base_name} --mode loop & python3 -m fastdeploy --recipe {recipe_base_name} --mode websocket"] \n'
         )
 
     dockerfile_path = os.path.join(RECIPE, "fastDeploy.auto_dockerfile")
     _dockerignore_f = open(os.path.join(RECIPE, ".dockerignore"), "w")
```

### Comparing `fastdeploy-2.2.7rc4/fastdeploy/__main__.py` & `fastdeploy-2.2.8/fastdeploy/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         help="Path to your recipe folder; env: RECIPE",
         required=True,
     )
 
     parser.add_argument(
         "--mode",
         type=str,
-        help='One of, ["loop", "rest", "websocket", "build_rest"]; env: MODE',
+        help='One of, ["loop", "rest", "websocket", "build_rest", "build_rest_no_loop"]; env: MODE',
         required=True,
     )
 
     parser.add_argument(
         "--queue_dir",
         type=str,
         help='Defaults to "--recipe" folder; end: QUEUE_DIR',
@@ -61,14 +61,18 @@
     )
 
     args = parser.parse_args()
 
     QUEUE_DIR = os.path.join(os.path.abspath(args.recipe), "fastdeploy_dbs")
 
     MODE = args.mode
+    if MODE == "build_no_loop_rest":
+        MODE = "build_rest"
+        os.environ["NO_LOOP"] = True
+
     RECIPE = os.path.abspath(args.recipe)
     BASE = args.base
     DOCKER_ARGS = args.docker_args
     if not DOCKER_ARGS:
         DOCKER_ARGS = ""
 
 if os.path.exists(RECIPE):
@@ -185,17 +189,23 @@
     )
 
     dockerfile_lines.append(
         f'ENTRYPOINT {os.getenv("ENTRYPOINT", ["/bin/sh", "-c"])} \n'.replace("'", '"')
     )
 
     if mode == "build_rest":
-        dockerfile_lines.append(
-            f'CMD ["ulimit -n 1000000 && python3 -m fastdeploy --recipe {recipe_base_name} --mode loop & python3 -m fastdeploy --recipe {recipe_base_name} --mode rest"] \n'
-        )
+        if os.getenv("NO_LOOP"):
+            dockerfile_lines.append(
+                f'CMD ["ulimit -n 1000000 && NO_LOOP=true python3 -m fastdeploy --recipe {recipe_base_name} --mode rest"] \n'
+            )
+
+        else:
+            dockerfile_lines.append(
+                f'CMD ["ulimit -n 1000000 && python3 -m fastdeploy --recipe {recipe_base_name} --mode loop & python3 -m fastdeploy --recipe {recipe_base_name} --mode rest"] \n'
+            )
     elif mode == "build_websocket":
         dockerfile_lines.append(
             f'CMD ["ulimit -n 1000000 && python3 -m fastdeploy --recipe {recipe_base_name} --mode loop & python3 -m fastdeploy --recipe {recipe_base_name} --mode websocket"] \n'
         )
 
     dockerfile_path = os.path.join(RECIPE, "fastDeploy.auto_dockerfile")
     _dockerignore_f = open(os.path.join(RECIPE, ".dockerignore"), "w")
```

### Comparing `fastdeploy-2.2.7rc4/fastdeploy/_app.py` & `fastdeploy-2.2.8/fastdeploy/_app.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,22 +15,25 @@
 import logging
 import datetime
 import mimetypes
 from functools import partial
 
 from . import _utils
 
-_utils.logger.info(f"Waiting for warmup, batch size search to finish.")
-
-while "LAST_PREDICTOR_SEQUENCE" not in _utils.META_INDEX:
-    time.sleep(5)
+if "LAST_PREDICTOR_SEQUENCE" not in _utils.META_INDEX:
+    _utils.logger.info(f"Waiting for warmup, batch size search to finish.")
+    while "LAST_PREDICTOR_SEQUENCE" not in _utils.META_INDEX:
+        time.sleep(5)
 
 LAST_PREDICTOR_SEQUENCE = _utils.META_INDEX["LAST_PREDICTOR_SEQUENCE"]
 
-while f"example_{LAST_PREDICTOR_SEQUENCE}" not in _utils.META_INDEX:
+while (
+    f"example_{LAST_PREDICTOR_SEQUENCE}" not in _utils.META_INDEX
+    or f"time_per_example_{LAST_PREDICTOR_SEQUENCE}" not in _utils.META_INDEX
+):
     time.sleep(5)
 
 ONLY_ASYNC = os.getenv("ONLY_ASYNC", False)
 
 TIME_PER_EXAMPLE = sum(
     [
         _utils.META_INDEX[f"time_per_example_{_}"]
@@ -40,14 +43,21 @@
 IS_FILE_INPUT = _utils.META_INDEX["IS_FILE_INPUT"]
 
 REQUEST_INDEX, RESULTS_INDEX = _utils.get_request_index_results_index(
     None, is_first=True, is_last=True
 )
 print(REQUEST_INDEX.directory, RESULTS_INDEX.directory)
 
+NO_LOOP_MODE = False
+if os.getenv("NO_LOOP").lower() == "true":
+    NO_LOOP_MODE = True
+
+if NO_LOOP_MODE:
+    from predictor import predictor
+
 
 def wait_and_read_pred(unique_id):
     """
     Waits for and reads result for unique_id.
 
     :param unique_id: unique_id of the input
 
@@ -152,35 +162,39 @@
 
                                 _temp_file.write(chunk)
                             _temp_file.flush()
                             _temp_file.close()
 
                             in_data.append(_temp_file_path)
 
-                _utils.META_INDEX["TO_PROCESS_COUNT"] += len(in_data)
-
-                _metrics = {}
-                _metrics["received"] = time.time()
-                _metrics["in_data"] = in_data
-                _utils.METRICS_INDEX[unique_id] = _metrics
-
-                REQUEST_INDEX[unique_id] = (
-                    in_data,
-                    [_extra_options_for_predictor.get(_) for _ in _in_file_names],
-                )
-
-                if is_async_request:
-                    resp.media = {"unique_id": unique_id, "success": True}
+                if NO_LOOP_MODE:
+                    resp.media = {"success": True, "prediction": predictor(in_data)}
                     resp.status = falcon.HTTP_200
                 else:
-                    resp.media, resp.status = wait_and_read_pred(unique_id)
+                    _utils.META_INDEX["TO_PROCESS_COUNT"] += len(in_data)
 
-                _metrics = _utils.METRICS_INDEX[unique_id]
-                _metrics["responded"] = time.time()
-                _utils.METRICS_INDEX[unique_id] = _metrics
+                    _metrics = {}
+                    _metrics["received"] = time.time()
+                    _metrics["in_data"] = in_data
+                    _utils.METRICS_INDEX[unique_id] = _metrics
+
+                    REQUEST_INDEX[unique_id] = (
+                        in_data,
+                        [_extra_options_for_predictor.get(_) for _ in _in_file_names],
+                    )
+
+                    if is_async_request:
+                        resp.media = {"unique_id": unique_id, "success": True}
+                        resp.status = falcon.HTTP_200
+                    else:
+                        resp.media, resp.status = wait_and_read_pred(unique_id)
+
+                    _metrics = _utils.METRICS_INDEX[unique_id]
+                    _metrics["responded"] = time.time()
+                    _utils.METRICS_INDEX[unique_id] = _metrics
 
         except Exception as ex:
             _utils.logger.exception(ex, exc_info=True)
             resp.media = {"success": False, "reason": "malformed request"}
             resp.status = falcon.HTTP_400
```

### Comparing `fastdeploy-2.2.7rc4/fastdeploy/_loop.py` & `fastdeploy-2.2.8/fastdeploy/_loop.py`

 * *Files identical despite different names*

### Comparing `fastdeploy-2.2.7rc4/fastdeploy/_utils.py` & `fastdeploy-2.2.8/fastdeploy/_utils.py`

 * *Files identical despite different names*

### Comparing `fastdeploy-2.2.7rc4/fastdeploy/_ws.py` & `fastdeploy-2.2.8/fastdeploy/_ws.py`

 * *Files identical despite different names*

### Comparing `fastdeploy-2.2.7rc4/fastdeploy/fastdeploy-ui/build/bundle.css` & `fastdeploy-2.2.8/fastdeploy/fastdeploy-ui/build/bundle.css`

 * *Files identical despite different names*

### Comparing `fastdeploy-2.2.7rc4/fastdeploy/fastdeploy-ui/build/bundle.js` & `fastdeploy-2.2.8/fastdeploy/fastdeploy-ui/build/bundle.js`

 * *Files identical despite different names*

### Comparing `fastdeploy-2.2.7rc4/fastdeploy/fastdeploy-ui/build/bundle.js.map` & `fastdeploy-2.2.8/fastdeploy/fastdeploy-ui/build/bundle.js.map`

 * *Files identical despite different names*

### Comparing `fastdeploy-2.2.7rc4/fastdeploy/fastdeploy-ui/favicon.png` & `fastdeploy-2.2.8/fastdeploy/fastdeploy-ui/favicon.png`

 * *Files identical despite different names*

### Comparing `fastdeploy-2.2.7rc4/fastdeploy/fastdeploy-ui/global.css` & `fastdeploy-2.2.8/fastdeploy/fastdeploy-ui/global.css`

 * *Files identical despite different names*

### Comparing `fastdeploy-2.2.7rc4/fastdeploy-ui/README.md` & `fastdeploy-2.2.8/fastdeploy-ui/README.md`

 * *Files identical despite different names*

### Comparing `fastdeploy-2.2.7rc4/fastdeploy-ui/package-lock.json` & `fastdeploy-2.2.8/fastdeploy-ui/package-lock.json`

 * *Files identical despite different names*

### Comparing `fastdeploy-2.2.7rc4/fastdeploy-ui/package.json` & `fastdeploy-2.2.8/fastdeploy-ui/package.json`

 * *Files identical despite different names*

### Comparing `fastdeploy-2.2.7rc4/fastdeploy-ui/rollup.config.js` & `fastdeploy-2.2.8/fastdeploy-ui/rollup.config.js`

 * *Files identical despite different names*

### Comparing `fastdeploy-2.2.7rc4/fastdeploy.egg-info/PKG-INFO` & `fastdeploy-2.2.8/fastdeploy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastdeploy
-Version: 2.2.7rc4
+Version: 2.2.8
 Summary: Deploy DL/ ML inference pipelines with minimal extra code. 
 Home-page: https://github.com/notAI-tech/fastDeploy
 Author: BEDAPUDI PRANEETH
 Author-email: praneeth@bpraneeth.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `fastdeploy-2.2.7rc4/fastdeploy.egg-info/SOURCES.txt` & `fastdeploy-2.2.8/fastdeploy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastdeploy-2.2.7rc4/setup.py` & `fastdeploy-2.2.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = "fastdeploy"
 DESCRIPTION = "Deploy DL/ ML inference pipelines with minimal extra code. "
 URL = "https://github.com/notAI-tech/fastDeploy"
 EMAIL = "praneeth@bpraneeth.com"
 AUTHOR = "BEDAPUDI PRANEETH"
 REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "2.2.7rc4"
+VERSION = "2.2.8"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "requests",
     "falcon",
     "diskcache",
     "ujson",
```

