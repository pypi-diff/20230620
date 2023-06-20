# Comparing `tmp/playlisterutil-2.0.9.tar.gz` & `tmp/playlisterutil-3.0.0.tar.gz`

## Comparing `playlisterutil-2.0.9.tar` & `playlisterutil-3.0.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 playlisterutil-2.0.9/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 playlisterutil-2.0.9/src/playlisterUtil/__init__.py
--rw-r--r--   0        0        0     5348 2020-02-02 00:00:00.000000 playlisterutil-2.0.9/src/playlisterUtil/playlisterUtil.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 playlisterutil-2.0.9/src/playlisterUtil/setup.py
--rw-r--r--   0        0        0     6492 2020-02-02 00:00:00.000000 playlisterutil-2.0.9/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 playlisterutil-2.0.9/LICENSE
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 playlisterutil-2.0.9/pyproject.toml
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 playlisterutil-2.0.9/PKG-INFO
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 playlisterutil-3.0.0/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 playlisterutil-3.0.0/src/playlisterUtil/__init__.py
+-rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 playlisterutil-3.0.0/src/playlisterUtil/playlisterUtil.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 playlisterutil-3.0.0/src/playlisterUtil/setup.py
+-rw-r--r--   0        0        0     6492 2020-02-02 00:00:00.000000 playlisterutil-3.0.0/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 playlisterutil-3.0.0/LICENSE
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 playlisterutil-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 playlisterutil-3.0.0/PKG-INFO
```

### Comparing `playlisterutil-2.0.9/src/playlisterUtil/playlisterUtil.py` & `playlisterutil-3.0.0/src/playlisterUtil/playlisterUtil.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,53 +11,54 @@
         elif dictionary is None:
             self.data = {
                 'youtube': {
                     'url': '',
                     'title': '',
                     'video_id': '',
                     'mix_id': '',
-                    'mix_index': '',
-                    'playlist_name': '',
-                    'playlist_num_songs': '',
+                    'mix_index': -1,
+                    'mix_name': '',
+                    'mix_num_songs': '',
                     'channel_name': '',
-                    'duration': '',
+                    # Duration in seconds
+                    'duration': -1,
                     'license': '',
                     'embeddable': False,
                     # Determined by duration > 15min and youtube tags
                     'is_multiple_songs': False, 
                     # Is playlist or mix
-                    'is_mix': False,
+                    'mix_type': '',
                 },
                 'spotify': {
-                    'api_href': '',
                     'song': {
                         'name': '',
                         'open_url': '',
                         'preview_url': '',
                         'api_url': '',
-                        'duration': 0,
+                        # Duration in seconds
+                        'duration': -1,
                     },
                     'artist': {
                         'open_url': '',
                         'api_url': '',
                         'name': '',
                     },
                     'album': {
                         'name': '',
                         'image_url': '',
                         'open_url': '',
                         'api_url': '',
-                        'duration': 0
+                        'duration': -1
                     }
 
                 },
                 'createdAt': "",
                 'startedProcessing': "",
                 'finishedProcessing': "",
-                'id': 0,
+                'id': -1,
                 # 0 not processed, 1 in process, 2 processed
                 'processed': 0,
                 # 0 didn't succeed, 1 succeed
                 'success': 0,
                 'retries': 0
             }
```

### Comparing `playlisterutil-2.0.9/.gitignore` & `playlisterutil-3.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `playlisterutil-2.0.9/LICENSE` & `playlisterutil-3.0.0/LICENSE`

 * *Files identical despite different names*

