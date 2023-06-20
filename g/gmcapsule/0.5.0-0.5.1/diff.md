# Comparing `tmp/gmcapsule-0.5.0.tar.gz` & `tmp/gmcapsule-0.5.1.tar.gz`

## Comparing `gmcapsule-0.5.0.tar` & `gmcapsule-0.5.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 gmcapsule-0.5.0/example.ini
--rw-r--r--   0        0        0    21684 2020-02-02 00:00:00.000000 gmcapsule-0.5.0/gmcapsule/__init__.py
--rw-r--r--   0        0        0    33472 2020-02-02 00:00:00.000000 gmcapsule-0.5.0/gmcapsule/gemini.py
--rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 gmcapsule-0.5.0/gmcapsule/markdown.py
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 gmcapsule-0.5.0/gmcapsule/modules/10_rewrite.py
--rwxr-xr-x   0        0        0    18619 2020-02-02 00:00:00.000000 gmcapsule-0.5.0/gmcapsule/modules/80_gitview.py
--rw-r--r--   0        0        0     6379 2020-02-02 00:00:00.000000 gmcapsule-0.5.0/gmcapsule/modules/90_cgi.py
--rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 gmcapsule-0.5.0/gmcapsule/modules/99_static.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 gmcapsule-0.5.0/.gitignore
--rw-r--r--   0        0        0     3933 2020-02-02 00:00:00.000000 gmcapsule-0.5.0/README.md
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 gmcapsule-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 gmcapsule-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 gmcapsule-0.5.1/example.ini
+-rw-r--r--   0        0        0    21706 2020-02-02 00:00:00.000000 gmcapsule-0.5.1/gmcapsule/__init__.py
+-rw-r--r--   0        0        0    33433 2020-02-02 00:00:00.000000 gmcapsule-0.5.1/gmcapsule/gemini.py
+-rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 gmcapsule-0.5.1/gmcapsule/markdown.py
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 gmcapsule-0.5.1/gmcapsule/modules/10_rewrite.py
+-rwxr-xr-x   0        0        0    18619 2020-02-02 00:00:00.000000 gmcapsule-0.5.1/gmcapsule/modules/80_gitview.py
+-rw-r--r--   0        0        0     6379 2020-02-02 00:00:00.000000 gmcapsule-0.5.1/gmcapsule/modules/90_cgi.py
+-rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 gmcapsule-0.5.1/gmcapsule/modules/99_static.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 gmcapsule-0.5.1/.gitignore
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 gmcapsule-0.5.1/README.md
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 gmcapsule-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     4927 2020-02-02 00:00:00.000000 gmcapsule-0.5.1/PKG-INFO
```

### Comparing `gmcapsule-0.5.0/example.ini` & `gmcapsule-0.5.1/example.ini`

 * *Files identical despite different names*

### Comparing `gmcapsule-0.5.0/gmcapsule/__init__.py` & `gmcapsule-0.5.1/gmcapsule/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -487,21 +487,21 @@
 import mimetypes
 import os
 import re
 import shlex
 import subprocess
 from pathlib import Path
 
-from .gemini import Server, Cache, Context
+from .gemini import Server, Cache, Context, Identity
 from .markdown import to_gemtext as markdown_to_gemtext
 
 
-__version__ = '0.5.0'
+__version__ = '0.5.1'
 __all__ = [
-    'Config', 'Cache', 'Context',
+    'Config', 'Cache', 'Context', 'Identity',
     'get_mime_type', 'markdown_to_gemtext'
 ]
 
 
 class Config:
     """
     Server configuration.
```

### Comparing `gmcapsule-0.5.0/gmcapsule/gemini.py` & `gmcapsule-0.5.1/gmcapsule/gemini.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,14 @@
     """
     try:
         if is_bytes(data):
             streaming = False
         else:
             streaming = True
             if isinstance(data, Path):
-                print('opening', data)
                 data = open(data, 'rb')
 
         # We may need to retry sending with the exact same buffer,
         # so keep it around until successful.
         BUF_LEN = 32768
         if streaming:
             send_buf = data.read(BUF_LEN)
```

### Comparing `gmcapsule-0.5.0/gmcapsule/markdown.py` & `gmcapsule-0.5.1/gmcapsule/markdown.py`

 * *Files identical despite different names*

### Comparing `gmcapsule-0.5.0/gmcapsule/modules/10_rewrite.py` & `gmcapsule-0.5.1/gmcapsule/modules/10_rewrite.py`

 * *Files identical despite different names*

### Comparing `gmcapsule-0.5.0/gmcapsule/modules/80_gitview.py` & `gmcapsule-0.5.1/gmcapsule/modules/80_gitview.py`

 * *Files identical despite different names*

### Comparing `gmcapsule-0.5.0/gmcapsule/modules/90_cgi.py` & `gmcapsule-0.5.1/gmcapsule/modules/90_cgi.py`

 * *Files identical despite different names*

### Comparing `gmcapsule-0.5.0/gmcapsule/modules/99_static.py` & `gmcapsule-0.5.1/gmcapsule/modules/99_static.py`

 * *Files identical despite different names*

### Comparing `gmcapsule-0.5.0/README.md` & `gmcapsule-0.5.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -51,14 +51,18 @@
 
 * Added `processes` to the `[server]` section to configure how many request handler processes are started.
 * Extension modules can register new protocols in addition to the built-in Gemini and Titan.
 * SIGHUP causes the configuration file to be reloaded and workers to be restarted. The listening socket remains open, so the socket and TLS parameters cannot be changed.
 * API change: Extension modules get initialized separately in each worker thread. Instead of a `Capsule`, the extension module `init` method is passed a `Context`. `Capsule` is no longer available as global state.
 * API change: `Identity` no longer contains OpenSSL objects for the certificate and public key. Instead, they are provided as serialized in DER format.
 
+v0.5.1:
+
+* `Identity` class is available when importing the `gmcapsule` module.
+
 ### v0.4
 
 * Added built-in module "rewrite" that matches regular expressions against the request path and can rewrite the path or return a custom status for redirection, "Gone" messages, or other exceptional situations.
 * Extension module load order is determined after locating all modules from all directories. Previously, the order was local to each directory.
 * Added a new configuration section `[priority]` for overriding default module priorities determined from file names. This is useful for changing the priority of the built-in modules.
 
 v0.4.1:
```

### Comparing `gmcapsule-0.5.0/pyproject.toml` & `gmcapsule-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gmcapsule-0.5.0/PKG-INFO` & `gmcapsule-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmcapsule
-Version: 0.5.0
+Version: 0.5.1
 Summary: Extensible Gemini/Titan server
 Project-URL: Home-page, https://geminispace.org/gmcapsule/
 Project-URL: Documentation, https://geminispace.org/gmcapsule/gmcapsule.html
 Project-URL: Source, https://codeberg.org/skyjake/gmcapsule
 Project-URL: Issues, https://codeberg.org/skyjake/gmcapsule/issues
 Author-email: Jaakko Keränen <jaakko.keranen@iki.fi>
 Keywords: gemini,internet,server,titan
@@ -73,14 +73,18 @@
 
 * Added `processes` to the `[server]` section to configure how many request handler processes are started.
 * Extension modules can register new protocols in addition to the built-in Gemini and Titan.
 * SIGHUP causes the configuration file to be reloaded and workers to be restarted. The listening socket remains open, so the socket and TLS parameters cannot be changed.
 * API change: Extension modules get initialized separately in each worker thread. Instead of a `Capsule`, the extension module `init` method is passed a `Context`. `Capsule` is no longer available as global state.
 * API change: `Identity` no longer contains OpenSSL objects for the certificate and public key. Instead, they are provided as serialized in DER format.
 
+v0.5.1:
+
+* `Identity` class is available when importing the `gmcapsule` module.
+
 ### v0.4
 
 * Added built-in module "rewrite" that matches regular expressions against the request path and can rewrite the path or return a custom status for redirection, "Gone" messages, or other exceptional situations.
 * Extension module load order is determined after locating all modules from all directories. Previously, the order was local to each directory.
 * Added a new configuration section `[priority]` for overriding default module priorities determined from file names. This is useful for changing the priority of the built-in modules.
 
 v0.4.1:
```

