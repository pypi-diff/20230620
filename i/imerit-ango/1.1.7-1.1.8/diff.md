# Comparing `tmp/imerit-ango-1.1.7.tar.gz` & `tmp/imerit-ango-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imerit-ango-1.1.7.tar", last modified: Fri Jun 16 09:27:20 2023, max compression
+gzip compressed data, was "imerit-ango-1.1.8.tar", last modified: Tue Jun 20 08:19:17 2023, max compression
```

## Comparing `imerit-ango-1.1.7.tar` & `imerit-ango-1.1.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-16 09:27:20.553299 imerit-ango-1.1.7/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1665 2023-06-16 09:27:20.553299 imerit-ango-1.1.7/PKG-INFO
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1305 2023-01-23 13:16:24.000000 imerit-ango-1.1.7/README.md
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-16 09:27:20.553299 imerit-ango-1.1.7/imerit_ango/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-06-16 09:20:50.000000 imerit-ango-1.1.7/imerit_ango/__init__.py
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-16 09:27:20.553299 imerit-ango-1.1.7/imerit_ango/models/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-06-16 09:20:50.000000 imerit-ango-1.1.7/imerit_ango/models/__init__.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)       93 2023-06-16 09:20:50.000000 imerit-ango-1.1.7/imerit_ango/models/enums.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     5452 2023-06-16 09:20:50.000000 imerit-ango-1.1.7/imerit_ango/models/label_category.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1304 2023-06-16 09:20:50.000000 imerit-ango-1.1.7/imerit_ango/plugin_logger.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     6129 2023-06-16 09:25:36.000000 imerit-ango-1.1.7/imerit_ango/plugins.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)    14443 2023-06-16 09:20:50.000000 imerit-ango-1.1.7/imerit_ango/sdk.py
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-16 09:27:20.553299 imerit-ango-1.1.7/imerit_ango.egg-info/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1665 2023-06-16 09:27:20.000000 imerit-ango-1.1.7/imerit_ango.egg-info/PKG-INFO
--rw-rw-r--   0 ofk       (1000) ofk       (1000)      383 2023-06-16 09:27:20.000000 imerit-ango-1.1.7/imerit_ango.egg-info/SOURCES.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        1 2023-06-16 09:27:20.000000 imerit-ango-1.1.7/imerit_ango.egg-info/dependency_links.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)      137 2023-06-16 09:27:20.000000 imerit-ango-1.1.7/imerit_ango.egg-info/requires.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)       12 2023-06-16 09:27:20.000000 imerit-ango-1.1.7/imerit_ango.egg-info/top_level.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)       38 2023-06-16 09:27:20.553299 imerit-ango-1.1.7/setup.cfg
--rw-rw-r--   0 ofk       (1000) ofk       (1000)      892 2023-06-16 09:26:57.000000 imerit-ango-1.1.7/setup.py
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-20 08:19:17.962220 imerit-ango-1.1.8/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1665 2023-06-20 08:19:17.962220 imerit-ango-1.1.8/PKG-INFO
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1305 2023-01-23 13:16:24.000000 imerit-ango-1.1.8/README.md
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-20 08:19:17.962220 imerit-ango-1.1.8/imerit_ango/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-06-19 08:05:54.000000 imerit-ango-1.1.8/imerit_ango/__init__.py
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-20 08:19:17.962220 imerit-ango-1.1.8/imerit_ango/models/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-06-19 08:05:54.000000 imerit-ango-1.1.8/imerit_ango/models/__init__.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)       93 2023-06-19 08:05:54.000000 imerit-ango-1.1.8/imerit_ango/models/enums.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     5452 2023-06-19 08:05:54.000000 imerit-ango-1.1.8/imerit_ango/models/label_category.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1304 2023-06-19 08:05:54.000000 imerit-ango-1.1.8/imerit_ango/plugin_logger.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     6155 2023-06-20 08:18:03.000000 imerit-ango-1.1.8/imerit_ango/plugins.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)    14443 2023-06-20 08:18:36.000000 imerit-ango-1.1.8/imerit_ango/sdk.py
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-20 08:19:17.962220 imerit-ango-1.1.8/imerit_ango.egg-info/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1665 2023-06-20 08:19:17.000000 imerit-ango-1.1.8/imerit_ango.egg-info/PKG-INFO
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)      383 2023-06-20 08:19:17.000000 imerit-ango-1.1.8/imerit_ango.egg-info/SOURCES.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        1 2023-06-20 08:19:17.000000 imerit-ango-1.1.8/imerit_ango.egg-info/dependency_links.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)      137 2023-06-20 08:19:17.000000 imerit-ango-1.1.8/imerit_ango.egg-info/requires.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)       12 2023-06-20 08:19:17.000000 imerit-ango-1.1.8/imerit_ango.egg-info/top_level.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)       38 2023-06-20 08:19:17.962220 imerit-ango-1.1.8/setup.cfg
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)      892 2023-06-20 08:18:45.000000 imerit-ango-1.1.8/setup.py
```

### Comparing `imerit-ango-1.1.7/PKG-INFO` & `imerit-ango-1.1.8/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imerit-ango
-Version: 1.1.7
+Version: 1.1.8
 Summary: Ango-Hub SDK
 Author: Faruk Karakaya
 Author-email: <faruk@ango.ai>
 License: UNKNOWN
 Keywords: imerit_ango,ango-hub,imerit_ango sdk,Ango,Ango-hub
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `imerit-ango-1.1.7/README.md` & `imerit-ango-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `imerit-ango-1.1.7/imerit_ango/models/label_category.py` & `imerit-ango-1.1.8/imerit_ango/models/label_category.py`

 * *Files identical despite different names*

### Comparing `imerit-ango-1.1.7/imerit_ango/plugin_logger.py` & `imerit-ango-1.1.8/imerit_ango/plugin_logger.py`

 * *Files identical despite different names*

### Comparing `imerit-ango-1.1.7/imerit_ango/plugins.py` & `imerit-ango-1.1.8/imerit_ango/plugins.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,15 +164,15 @@
         super().__init__(id, secret, callback)
 
 
 def _connect(plugin, host):
     try:
         sio = socketio.Client(logger=logging.getLogger("plugin"), reconnection=False)
         sio.register_namespace(plugin)
-        sio.connect(host, namespaces=["/plugin"])
+        sio.connect(host, namespaces=["/plugin"], transports=["websocket"])
     except Exception as e:
         logging.getLogger().critical(e)
         os._exit(1)
 
 
 def run(plugin, host="https://plugin.imerit.ango.ai"):
     _connect(plugin, host)
```

### Comparing `imerit-ango-1.1.7/imerit_ango/sdk.py` & `imerit-ango-1.1.8/imerit_ango/sdk.py`

 * *Files identical despite different names*

### Comparing `imerit-ango-1.1.7/imerit_ango.egg-info/PKG-INFO` & `imerit-ango-1.1.8/imerit_ango.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imerit-ango
-Version: 1.1.7
+Version: 1.1.8
 Summary: Ango-Hub SDK
 Author: Faruk Karakaya
 Author-email: <faruk@ango.ai>
 License: UNKNOWN
 Keywords: imerit_ango,ango-hub,imerit_ango sdk,Ango,Ango-hub
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `imerit-ango-1.1.7/setup.py` & `imerit-ango-1.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="imerit-ango",
-    version="1.1.7",
+    version="1.1.8",
     author="Faruk Karakaya",
     author_email="<faruk@ango.ai>",
     description="Ango-Hub SDK",
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```

