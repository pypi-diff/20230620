# Comparing `tmp/playlisterutil-2.0.5.tar.gz` & `tmp/playlisterutil-2.0.6.tar.gz`

## Comparing `playlisterutil-2.0.5.tar` & `playlisterutil-2.0.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 playlisterutil-2.0.5/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 playlisterutil-2.0.5/src/playlisterUtil/__init__.py
--rw-r--r--   0        0        0     4801 2020-02-02 00:00:00.000000 playlisterutil-2.0.5/src/playlisterUtil/playlisterUtil.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 playlisterutil-2.0.5/src/playlisterUtil/setup.py
--rw-r--r--   0        0        0     6492 2020-02-02 00:00:00.000000 playlisterutil-2.0.5/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 playlisterutil-2.0.5/LICENSE
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 playlisterutil-2.0.5/pyproject.toml
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 playlisterutil-2.0.5/PKG-INFO
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 playlisterutil-2.0.6/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 playlisterutil-2.0.6/src/playlisterUtil/__init__.py
+-rw-r--r--   0        0        0     5051 2020-02-02 00:00:00.000000 playlisterutil-2.0.6/src/playlisterUtil/playlisterUtil.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 playlisterutil-2.0.6/src/playlisterUtil/setup.py
+-rw-r--r--   0        0        0     6492 2020-02-02 00:00:00.000000 playlisterutil-2.0.6/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 playlisterutil-2.0.6/LICENSE
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 playlisterutil-2.0.6/pyproject.toml
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 playlisterutil-2.0.6/PKG-INFO
```

### Comparing `playlisterutil-2.0.5/src/playlisterUtil/playlisterUtil.py` & `playlisterutil-2.0.6/src/playlisterUtil/playlisterUtil.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,65 +1,65 @@
 import os
 import pymongo
 
 def get_mongo_uri() -> str :
     return f"mongodb://{os.environ.get('MONGO_USER')}:{os.environ.get('MONGO_PASS')}@{os.environ.get('MONGO_SVC_ADDRESS')}/{os.environ.get('MONGO_DB')}" 
 
 class MongoDoc:
-    def __init__(self):
-        self.data = {
-            'youtube': {
-                'url': '',
-                'title': '',
-                'video_id': '',
-                'mix_id': '',
-                'mix_index': '',
-                'duration': '',
-                'license': '',
-                'embeddable': False,
-                # Determined by duration > 30min and youtube tags
-                'is_multiple_songs': False, 
-                'is_mix': False,
-            },
-            'spotify': {
-                'api_href': '',
-                'song': {
-                    'name': '',
-                    'open_url': '',
-                    'preview_url': '',
-                    'api_url': '',
-                    'duration': 0,
+    def __init__(self, dictionary=None):
+        if type(dictionary) is dict:
+            self.data = dictionary
+        elif dictionary is None:
+            self.data = {
+                'youtube': {
+                    'url': '',
+                    'title': '',
+                    'video_id': '',
+                    'mix_id': '',
+                    'mix_index': '',
+                    'duration': '',
+                    'license': '',
+                    'embeddable': False,
+                    # Determined by duration > 30min and youtube tags
+                    'is_multiple_songs': False, 
+                    'is_mix': False,
                 },
-                'artist': {
-                    'open_url': '',
-                    'api_url': '',
-                    'name': '',
-                },
-                'album': {
-                    'name': '',
-                    'image_url': '',
-                    'open_url': '',
-                    'api_url': '',
-                    'duration': 0
-                }
-
-            },
-            'createdAt': "",
-            'startedProcessing': "",
-            'finishedProcessing': "",
-            'id': 0,
-            # 0 not processed, 1 in process, 2 processed
-            'processed': 0,
-            # 0 didn't succeed, 1 succeed
-            'success': 0,
-            'retries': 0
-        }
+                'spotify': {
+                    'api_href': '',
+                    'song': {
+                        'name': '',
+                        'open_url': '',
+                        'preview_url': '',
+                        'api_url': '',
+                        'duration': 0,
+                    },
+                    'artist': {
+                        'open_url': '',
+                        'api_url': '',
+                        'name': '',
+                    },
+                    'album': {
+                        'name': '',
+                        'image_url': '',
+                        'open_url': '',
+                        'api_url': '',
+                        'duration': 0
+                    }
 
-    def __init__(self, dict):
-        self.data = dict
+                },
+                'createdAt': "",
+                'startedProcessing': "",
+                'finishedProcessing': "",
+                'id': 0,
+                # 0 not processed, 1 in process, 2 processed
+                'processed': 0,
+                # 0 didn't succeed, 1 succeed
+                'success': 0,
+                'retries': 0
+            }
 
     def get_value(self, key, default=None):
         keys = key.split('.')
         value = self.data
         for k in keys:
             value = value.get(k)
             if value is None:
```

### Comparing `playlisterutil-2.0.5/.gitignore` & `playlisterutil-2.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `playlisterutil-2.0.5/LICENSE` & `playlisterutil-2.0.6/LICENSE`

 * *Files identical despite different names*

