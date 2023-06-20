# Comparing `tmp/ango-1.1.5.tar.gz` & `tmp/ango-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ango-1.1.5.tar", last modified: Fri Jun 16 09:28:07 2023, max compression
+gzip compressed data, was "ango-1.1.6.tar", last modified: Tue Jun 20 08:20:02 2023, max compression
```

## Comparing `ango-1.1.5.tar` & `ango-1.1.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-16 09:28:07.489078 ango-1.1.5/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1644 2023-06-16 09:28:07.489078 ango-1.1.5/PKG-INFO
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1305 2023-01-23 13:16:24.000000 ango-1.1.5/README.md
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-16 09:28:07.489078 ango-1.1.5/ango/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-06-16 09:27:24.000000 ango-1.1.5/ango/__init__.py
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-16 09:28:07.489078 ango-1.1.5/ango/models/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-06-16 09:27:24.000000 ango-1.1.5/ango/models/__init__.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)       93 2023-06-16 09:27:24.000000 ango-1.1.5/ango/models/enums.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     5445 2023-06-16 09:27:24.000000 ango-1.1.5/ango/models/label_category.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1304 2023-06-16 09:27:24.000000 ango-1.1.5/ango/plugin_logger.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     6055 2023-06-16 09:27:58.000000 ango-1.1.5/ango/plugins.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)    14965 2023-06-16 09:27:24.000000 ango-1.1.5/ango/sdk.py
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-16 09:28:07.489078 ango-1.1.5/ango.egg-info/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1644 2023-06-16 09:28:07.000000 ango-1.1.5/ango.egg-info/PKG-INFO
--rw-rw-r--   0 ofk       (1000) ofk       (1000)      299 2023-06-16 09:28:07.000000 ango-1.1.5/ango.egg-info/SOURCES.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        1 2023-06-16 09:28:07.000000 ango-1.1.5/ango.egg-info/dependency_links.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)      137 2023-06-16 09:28:07.000000 ango-1.1.5/ango.egg-info/requires.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        5 2023-06-16 09:28:07.000000 ango-1.1.5/ango.egg-info/top_level.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)       38 2023-06-16 09:28:07.489078 ango-1.1.5/setup.cfg
--rw-rw-r--   0 ofk       (1000) ofk       (1000)      871 2023-06-16 09:27:24.000000 ango-1.1.5/setup.py
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-20 08:20:02.410423 ango-1.1.6/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1644 2023-06-20 08:20:02.410423 ango-1.1.6/PKG-INFO
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1305 2023-01-23 13:16:24.000000 ango-1.1.6/README.md
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-20 08:20:02.410423 ango-1.1.6/ango/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-06-20 08:19:44.000000 ango-1.1.6/ango/__init__.py
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-20 08:20:02.410423 ango-1.1.6/ango/models/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-06-20 08:19:44.000000 ango-1.1.6/ango/models/__init__.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)       93 2023-06-20 08:19:44.000000 ango-1.1.6/ango/models/enums.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     5445 2023-06-20 08:19:44.000000 ango-1.1.6/ango/models/label_category.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1304 2023-06-20 08:19:44.000000 ango-1.1.6/ango/plugin_logger.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     6081 2023-06-20 08:19:51.000000 ango-1.1.6/ango/plugins.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)    14965 2023-06-20 08:19:44.000000 ango-1.1.6/ango/sdk.py
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-20 08:20:02.410423 ango-1.1.6/ango.egg-info/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1644 2023-06-20 08:20:02.000000 ango-1.1.6/ango.egg-info/PKG-INFO
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)      299 2023-06-20 08:20:02.000000 ango-1.1.6/ango.egg-info/SOURCES.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        1 2023-06-20 08:20:02.000000 ango-1.1.6/ango.egg-info/dependency_links.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)      137 2023-06-20 08:20:02.000000 ango-1.1.6/ango.egg-info/requires.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        5 2023-06-20 08:20:02.000000 ango-1.1.6/ango.egg-info/top_level.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)       38 2023-06-20 08:20:02.410423 ango-1.1.6/setup.cfg
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)      871 2023-06-20 08:19:57.000000 ango-1.1.6/setup.py
```

### Comparing `ango-1.1.5/PKG-INFO` & `ango-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ango
-Version: 1.1.5
+Version: 1.1.6
 Summary: Ango-Hub SDK
 Author: Faruk Karakaya
 Author-email: <faruk@ango.ai>
 License: UNKNOWN
 Keywords: ango,ango-hub,ango sdk,Ango,Ango-hub
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ango-1.1.5/README.md` & `ango-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `ango-1.1.5/ango/models/label_category.py` & `ango-1.1.6/ango/models/label_category.py`

 * *Files identical despite different names*

### Comparing `ango-1.1.5/ango/plugin_logger.py` & `ango-1.1.6/ango/plugin_logger.py`

 * *Files identical despite different names*

### Comparing `ango-1.1.5/ango/plugins.py` & `ango-1.1.6/ango/plugins.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,15 @@
     def __init__(self, id: str, secret: str, callback: Callable):
         super().__init__(id, secret, callback)
 
 def _connect(plugin, host):
     try:
         sio = socketio.Client(logger=logging.getLogger("plugin"), reconnection=False)
         sio.register_namespace(plugin)
-        sio.connect(host, namespaces=["/plugin"])
+        sio.connect(host, namespaces=["/plugin"], transports=["websocket"])
     except Exception as e:
         logging.getLogger("plugin").critical(e)
         os._exit(1)
 
 def run(plugin, host="https://api.ango.ai"):
     _connect(plugin, host)
     try:
```

### Comparing `ango-1.1.5/ango/sdk.py` & `ango-1.1.6/ango/sdk.py`

 * *Files identical despite different names*

### Comparing `ango-1.1.5/ango.egg-info/PKG-INFO` & `ango-1.1.6/ango.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ango
-Version: 1.1.5
+Version: 1.1.6
 Summary: Ango-Hub SDK
 Author: Faruk Karakaya
 Author-email: <faruk@ango.ai>
 License: UNKNOWN
 Keywords: ango,ango-hub,ango sdk,Ango,Ango-hub
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ango-1.1.5/setup.py` & `ango-1.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="ango",
-    version="1.1.5",
+    version="1.1.6",
     author="Faruk Karakaya",
     author_email="<faruk@ango.ai>",
     description="Ango-Hub SDK",
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```

