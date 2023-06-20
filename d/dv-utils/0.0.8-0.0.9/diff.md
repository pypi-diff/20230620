# Comparing `tmp/dv_utils-0.0.8.tar.gz` & `tmp/dv_utils-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dv_utils-0.0.8.tar", max compression
+gzip compressed data, was "dv_utils-0.0.9.tar", max compression
```

## Comparing `dv_utils-0.0.8.tar` & `dv_utils-0.0.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      622 2022-09-23 12:38:21.911471 dv_utils-0.0.8/README.md
--rw-r--r--   0        0        0      328 2022-08-05 13:44:21.474630 dv_utils-0.0.8/dv_utils/__init__.py
--rw-r--r--   0        0        0      452 2023-04-26 10:45:42.041117 dv_utils-0.0.8/dv_utils/__main__.py
--rw-r--r--   0        0        0     3239 2023-02-20 08:24:19.300581 dv_utils-0.0.8/dv_utils/client.py
--rw-r--r--   0        0        0      996 2023-04-26 11:03:06.397525 dv_utils-0.0.8/dv_utils/listener.py
--rw-r--r--   0        0        0     1913 2023-04-26 11:01:57.641223 dv_utils-0.0.8/dv_utils/log_utils.py
--rw-r--r--   0        0        0     1521 2022-08-05 13:05:56.151683 dv_utils-0.0.8/dv_utils/process.py
--rw-r--r--   0        0        0     3284 2023-02-16 13:40:18.447939 dv_utils-0.0.8/dv_utils/redis.py
--rw-r--r--   0        0        0     1413 2022-08-05 13:04:09.726787 dv_utils-0.0.8/dv_utils/settings.py
--rw-r--r--   0        0        0     1186 2023-04-26 11:03:34.453649 dv_utils-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1514 1970-01-01 00:00:00.000000 dv_utils-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      622 2022-09-23 12:38:21.911471 dv_utils-0.0.9/README.md
+-rw-r--r--   0        0        0      328 2022-08-05 13:44:21.474630 dv_utils-0.0.9/dv_utils/__init__.py
+-rw-r--r--   0        0        0      452 2023-04-26 10:45:42.041117 dv_utils-0.0.9/dv_utils/__main__.py
+-rw-r--r--   0        0        0     3239 2023-02-20 08:24:19.300581 dv_utils-0.0.9/dv_utils/client.py
+-rw-r--r--   0        0        0      995 2023-04-26 11:52:29.464558 dv_utils-0.0.9/dv_utils/listener.py
+-rw-r--r--   0        0        0     1913 2023-04-26 11:01:57.641223 dv_utils-0.0.9/dv_utils/log_utils.py
+-rw-r--r--   0        0        0     1521 2022-08-05 13:05:56.151683 dv_utils-0.0.9/dv_utils/process.py
+-rw-r--r--   0        0        0     3284 2023-02-16 13:40:18.447939 dv_utils-0.0.9/dv_utils/redis.py
+-rw-r--r--   0        0        0     1413 2022-08-05 13:04:09.726787 dv_utils-0.0.9/dv_utils/settings.py
+-rw-r--r--   0        0        0     1186 2023-04-26 11:52:51.472718 dv_utils-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1514 1970-01-01 00:00:00.000000 dv_utils-0.0.9/PKG-INFO
```

### Comparing `dv_utils-0.0.8/README.md` & `dv_utils-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `dv_utils-0.0.8/dv_utils/client.py` & `dv_utils-0.0.9/dv_utils/client.py`

 * *Files identical despite different names*

### Comparing `dv_utils-0.0.8/dv_utils/listener.py` & `dv_utils-0.0.9/dv_utils/listener.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     def __init__(
         self, event_processor: Callable[[dict], Any] = process_event_dummy, daemon=False
     ):
         # Instantiate the local Datavillage Redis queue
         redis_queue = RedisQueue()
         redis_queue.create_consummer_group()
 
-        audit_log(log="Algo Event Listener starting", app="algo"):
+        audit_log(log="Algo Event Listener starting", app="algo")
 
 
         if daemon:
             # listen continously and process all incoming events
             # the listen loop stops by default after 1h
             redis_queue.listen(event_processor)
         else:
```

### Comparing `dv_utils-0.0.8/dv_utils/log_utils.py` & `dv_utils-0.0.9/dv_utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `dv_utils-0.0.8/dv_utils/process.py` & `dv_utils-0.0.9/dv_utils/process.py`

 * *Files identical despite different names*

### Comparing `dv_utils-0.0.8/dv_utils/redis.py` & `dv_utils-0.0.9/dv_utils/redis.py`

 * *Files identical despite different names*

### Comparing `dv_utils-0.0.8/dv_utils/settings.py` & `dv_utils-0.0.9/dv_utils/settings.py`

 * *Files identical despite different names*

### Comparing `dv_utils-0.0.8/pyproject.toml` & `dv_utils-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry>=0.12", "setuptools>=40.8.0"]
 build-backend = "poetry.masonry.api"
 
 [tool]
 [tool.poetry]
 name = "dv-utils"
-version = "0.0.8"
+version = "0.0.9"
 description = "DataVillage Python utils for interaction with the middleware and building algo processing code"
 authors = ["Loic Quertenmont <loic@deeperanalytics.be>"]
 readme = "README.md"
 repository = "https://github.com/datavillage-me/dv-utils"
 
 [tool.poetry.dependencies]
 python = ">=3.10.4,<4"
```

### Comparing `dv_utils-0.0.8/PKG-INFO` & `dv_utils-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dv-utils
-Version: 0.0.8
+Version: 0.0.9
 Summary: DataVillage Python utils for interaction with the middleware and building algo processing code
 Home-page: https://github.com/datavillage-me/dv-utils
 Author: Loic Quertenmont
 Author-email: loic@deeperanalytics.be
 Requires-Python: >=3.10.4,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

