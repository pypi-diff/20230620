# Comparing `tmp/logfire-python-0.0.3.tar.gz` & `tmp/logfire-python-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logfire-python-0.0.3.tar", last modified: Tue Jun  6 06:55:00 2023, max compression
+gzip compressed data, was "logfire-python-0.0.4.tar", last modified: Tue Jun 20 11:50:08 2023, max compression
```

## Comparing `logfire-python-0.0.3.tar` & `logfire-python-0.0.4.tar`

### file list

```diff
@@ -1,32 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 06:55:00.001047 logfire-python-0.0.3/
--rw-rw-rw-   0        0        0      741 2023-04-12 02:48:20.000000 logfire-python-0.0.3/LICENSE.md
--rw-rw-rw-   0        0        0      106 2023-04-12 06:15:33.000000 logfire-python-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     3861 2023-06-06 06:55:00.000046 logfire-python-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2672 2023-04-12 03:58:47.000000 logfire-python-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 06:54:59.981473 logfire-python-0.0.3/logfire/
--rw-rw-rw-   0        0        0      260 2023-04-12 03:28:58.000000 logfire-python-0.0.3/logfire/__init__.py
--rw-rw-rw-   0        0        0      141 2023-04-12 03:31:13.000000 logfire-python-0.0.3/logfire/compat.py
--rw-rw-rw-   0        0        0     2998 2023-04-12 03:31:03.000000 logfire-python-0.0.3/logfire/flusher.py
--rw-rw-rw-   0        0        0      968 2023-04-12 03:30:53.000000 logfire-python-0.0.3/logfire/formatter.py
--rw-rw-rw-   0        0        0     2441 2023-04-12 03:30:43.000000 logfire-python-0.0.3/logfire/frame.py
--rw-rw-rw-   0        0        0     2680 2023-06-06 06:50:37.000000 logfire-python-0.0.3/logfire/handler.py
--rw-rw-rw-   0        0        0     1156 2023-04-12 03:30:18.000000 logfire-python-0.0.3/logfire/helpers.py
--rw-rw-rw-   0        0        0      588 2023-04-12 03:30:07.000000 logfire-python-0.0.3/logfire/uploader.py
-drwxrwxrwx   0        0        0        0 2023-06-06 06:54:59.991983 logfire-python-0.0.3/logfire_python.egg-info/
--rw-rw-rw-   0        0        0     3861 2023-06-06 06:54:59.000000 logfire-python-0.0.3/logfire_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      566 2023-06-06 06:54:59.000000 logfire-python-0.0.3/logfire_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 06:54:59.000000 logfire-python-0.0.3/logfire_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       98 2023-06-06 06:54:59.000000 logfire-python-0.0.3/logfire_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-06 06:54:59.000000 logfire-python-0.0.3/logfire_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1357 2023-06-06 06:53:53.000000 logfire-python-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      222 2023-04-12 07:58:34.000000 logfire-python-0.0.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 06:55:00.001047 logfire-python-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0       54 2023-04-12 05:19:07.000000 logfire-python-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-06 06:54:59.999046 logfire-python-0.0.3/tests/
--rw-rw-rw-   0        0        0        0 2023-04-11 14:45:50.000000 logfire-python-0.0.3/tests/__init__.py
--rw-rw-rw-   0        0        0     5206 2023-06-06 06:50:49.000000 logfire-python-0.0.3/tests/test_flusher.py
--rw-rw-rw-   0        0        0     5264 2023-04-11 15:02:08.000000 logfire-python-0.0.3/tests/test_formatter.py
--rw-rw-rw-   0        0        0     1955 2023-04-11 15:02:30.000000 logfire-python-0.0.3/tests/test_frame.py
--rw-rw-rw-   0        0        0     4337 2023-04-11 15:02:51.000000 logfire-python-0.0.3/tests/test_handler.py
--rw-rw-rw-   0        0        0     1846 2023-04-11 15:03:14.000000 logfire-python-0.0.3/tests/test_helpers.py
--rw-rw-rw-   0        0        0     1059 2023-04-11 15:03:40.000000 logfire-python-0.0.3/tests/test_uploader.py
+drwxrwxrwx   0        0        0        0 2023-06-20 11:50:08.558169 logfire-python-0.0.4/
+-rw-rw-rw-   0        0        0      741 2023-04-12 02:48:20.000000 logfire-python-0.0.4/LICENSE.md
+-rw-rw-rw-   0        0        0      106 2023-04-12 06:15:33.000000 logfire-python-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     3861 2023-06-20 11:50:08.557170 logfire-python-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2672 2023-04-12 03:58:47.000000 logfire-python-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 11:50:08.525171 logfire-python-0.0.4/logfire/
+-rw-rw-rw-   0        0        0      260 2023-04-12 03:28:58.000000 logfire-python-0.0.4/logfire/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 11:50:08.533172 logfire-python-0.0.4/logfire/__pycache__/
+-rw-rw-rw-   0        0        0      539 2023-06-20 11:04:18.000000 logfire-python-0.0.4/logfire/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      406 2023-06-20 11:04:18.000000 logfire-python-0.0.4/logfire/__pycache__/compat.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3574 2023-06-20 11:04:18.000000 logfire-python-0.0.4/logfire/__pycache__/flusher.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1462 2023-06-20 11:04:18.000000 logfire-python-0.0.4/logfire/__pycache__/formatter.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3687 2023-06-20 11:47:36.000000 logfire-python-0.0.4/logfire/__pycache__/frame.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3811 2023-06-20 11:04:18.000000 logfire-python-0.0.4/logfire/__pycache__/handler.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2627 2023-06-20 11:04:18.000000 logfire-python-0.0.4/logfire/__pycache__/helpers.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1367 2023-06-20 11:04:18.000000 logfire-python-0.0.4/logfire/__pycache__/uploader.cpython-311.pyc
+-rw-rw-rw-   0        0        0      141 2023-04-12 03:31:13.000000 logfire-python-0.0.4/logfire/compat.py
+-rw-rw-rw-   0        0        0     2998 2023-04-12 03:31:03.000000 logfire-python-0.0.4/logfire/flusher.py
+-rw-rw-rw-   0        0        0      968 2023-04-12 03:30:53.000000 logfire-python-0.0.4/logfire/formatter.py
+-rw-rw-rw-   0        0        0     2642 2023-06-20 11:47:33.000000 logfire-python-0.0.4/logfire/frame.py
+-rw-rw-rw-   0        0        0     2733 2023-06-20 10:58:13.000000 logfire-python-0.0.4/logfire/handler.py
+-rw-rw-rw-   0        0        0     1156 2023-04-12 03:30:18.000000 logfire-python-0.0.4/logfire/helpers.py
+-rw-rw-rw-   0        0        0      588 2023-04-12 03:30:07.000000 logfire-python-0.0.4/logfire/uploader.py
+drwxrwxrwx   0        0        0        0 2023-06-20 11:50:08.553169 logfire-python-0.0.4/logfire_python.egg-info/
+-rw-rw-rw-   0        0        0     3861 2023-06-20 11:50:08.000000 logfire-python-0.0.4/logfire_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      919 2023-06-20 11:50:08.000000 logfire-python-0.0.4/logfire_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 11:50:08.000000 logfire-python-0.0.4/logfire_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       98 2023-06-20 11:50:08.000000 logfire-python-0.0.4/logfire_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-20 11:50:08.000000 logfire-python-0.0.4/logfire_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1357 2023-06-20 11:49:52.000000 logfire-python-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      222 2023-04-12 07:58:34.000000 logfire-python-0.0.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 11:50:08.558169 logfire-python-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0       54 2023-04-12 05:19:07.000000 logfire-python-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 11:50:08.557170 logfire-python-0.0.4/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-11 14:45:50.000000 logfire-python-0.0.4/tests/__init__.py
+-rw-rw-rw-   0        0        0     5206 2023-06-06 06:50:49.000000 logfire-python-0.0.4/tests/test_flusher.py
+-rw-rw-rw-   0        0        0     5264 2023-04-11 15:02:08.000000 logfire-python-0.0.4/tests/test_formatter.py
+-rw-rw-rw-   0        0        0     1955 2023-04-11 15:02:30.000000 logfire-python-0.0.4/tests/test_frame.py
+-rw-rw-rw-   0        0        0     4337 2023-04-11 15:02:51.000000 logfire-python-0.0.4/tests/test_handler.py
+-rw-rw-rw-   0        0        0     1846 2023-04-11 15:03:14.000000 logfire-python-0.0.4/tests/test_helpers.py
+-rw-rw-rw-   0        0        0     1059 2023-04-11 15:03:40.000000 logfire-python-0.0.4/tests/test_uploader.py
```

### Comparing `logfire-python-0.0.3/LICENSE.md` & `logfire-python-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `logfire-python-0.0.3/PKG-INFO` & `logfire-python-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logfire-python
-Version: 0.0.3
+Version: 0.0.4
 Summary: Logfire.sh client library
 Author-email: Logfire <support@logfire.sh>
 Project-URL: Homepage, https://github.com/logfire-sh/logfire-python
 Keywords: api,logfire,logging,client
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Operating System :: OS Independent
```

### Comparing `logfire-python-0.0.3/README.md` & `logfire-python-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `logfire-python-0.0.3/logfire/flusher.py` & `logfire-python-0.0.4/logfire/flusher.py`

 * *Files identical despite different names*

### Comparing `logfire-python-0.0.3/logfire/formatter.py` & `logfire-python-0.0.4/logfire/formatter.py`

 * *Files identical despite different names*

### Comparing `logfire-python-0.0.3/logfire/frame.py` & `logfire-python-0.0.4/logfire/frame.py`

 * *Files 11% similar despite different names*

```diff
@@ -44,21 +44,30 @@
 def _parse_custom_events(record, include_extra_attributes):
     default_keys = {
         'args', 'asctime', 'created', 'exc_info', 'exc_text', 'pathname',
         'funcName', 'levelname', 'levelno', 'lineno', 'module', 'msecs',
         'message', 'msg', 'name', 'pathname', 'process', 'processName',
         'relativeCreated', 'thread', 'threadName'
     }
+    extra_keys = {
+        'filename', 'stack_info'
+    }
     events = {}
+    extra = {}
     for key, val in record.__dict__.items():
         if key in default_keys:
             continue
         if not include_extra_attributes and not isinstance(val, dict):
             continue
-        events[key] = val
+        if key not in extra_keys:
+            extra[key] = val
+        else:
+            events[key] = val
+    if extra :
+        events["extra"] = extra
     return events
 
 
 def _levelname(level):
     return {
         'debug': 'debug',
         'info': 'info',
```

### Comparing `logfire-python-0.0.3/logfire/handler.py` & `logfire-python-0.0.4/logfire/handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 
 from .compat import queue
 from .helpers import DEFAULT_CONTEXT
 from .flusher import FlushWorker
 from .uploader import Uploader
 from .frame import create_frame
 
-DEFAULT_HOST = 'https://in.logfire.sh'
+DEFAULT_HOST = 'http://localhost:8888/logfire.sh'
+# DEFAULT_HOST = 'https://in.logfire.sh'
 DEFAULT_BUFFER_CAPACITY = 1000
 DEFAULT_FLUSH_INTERVAL = 1
 DEFAULT_RAISE_EXCEPTIONS = False
 DEFAULT_DROP_EXTRA_EVENTS = True
 DEFAULT_INCLUDE_EXTRA_ATTRIBUTES = True
```

### Comparing `logfire-python-0.0.3/logfire/helpers.py` & `logfire-python-0.0.4/logfire/helpers.py`

 * *Files identical despite different names*

### Comparing `logfire-python-0.0.3/logfire/uploader.py` & `logfire-python-0.0.4/logfire/uploader.py`

 * *Files identical despite different names*

### Comparing `logfire-python-0.0.3/logfire_python.egg-info/PKG-INFO` & `logfire-python-0.0.4/logfire_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logfire-python
-Version: 0.0.3
+Version: 0.0.4
 Summary: Logfire.sh client library
 Author-email: Logfire <support@logfire.sh>
 Project-URL: Homepage, https://github.com/logfire-sh/logfire-python
 Keywords: api,logfire,logging,client
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Operating System :: OS Independent
```

### Comparing `logfire-python-0.0.3/logfire_python.egg-info/SOURCES.txt` & `logfire-python-0.0.4/logfire_python.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -8,14 +8,22 @@
 logfire/compat.py
 logfire/flusher.py
 logfire/formatter.py
 logfire/frame.py
 logfire/handler.py
 logfire/helpers.py
 logfire/uploader.py
+logfire/__pycache__/__init__.cpython-311.pyc
+logfire/__pycache__/compat.cpython-311.pyc
+logfire/__pycache__/flusher.cpython-311.pyc
+logfire/__pycache__/formatter.cpython-311.pyc
+logfire/__pycache__/frame.cpython-311.pyc
+logfire/__pycache__/handler.cpython-311.pyc
+logfire/__pycache__/helpers.cpython-311.pyc
+logfire/__pycache__/uploader.cpython-311.pyc
 logfire_python.egg-info/PKG-INFO
 logfire_python.egg-info/SOURCES.txt
 logfire_python.egg-info/dependency_links.txt
 logfire_python.egg-info/requires.txt
 logfire_python.egg-info/top_level.txt
 tests/__init__.py
 tests/test_flusher.py
```

### Comparing `logfire-python-0.0.3/pyproject.toml` & `logfire-python-0.0.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "logfire-python"
-version = "0.0.3"
+version = "0.0.4"
 description = "Logfire.sh client library"
 readme = "README.md"
 authors = [{ name = "Logfire", email = "support@logfire.sh" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: ISC License (ISCL)",
```

### Comparing `logfire-python-0.0.3/tests/test_flusher.py` & `logfire-python-0.0.4/tests/test_flusher.py`

 * *Files identical despite different names*

### Comparing `logfire-python-0.0.3/tests/test_formatter.py` & `logfire-python-0.0.4/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `logfire-python-0.0.3/tests/test_frame.py` & `logfire-python-0.0.4/tests/test_frame.py`

 * *Files identical despite different names*

### Comparing `logfire-python-0.0.3/tests/test_handler.py` & `logfire-python-0.0.4/tests/test_handler.py`

 * *Files identical despite different names*

### Comparing `logfire-python-0.0.3/tests/test_helpers.py` & `logfire-python-0.0.4/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `logfire-python-0.0.3/tests/test_uploader.py` & `logfire-python-0.0.4/tests/test_uploader.py`

 * *Files identical despite different names*

