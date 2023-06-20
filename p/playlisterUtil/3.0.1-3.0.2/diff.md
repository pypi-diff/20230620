# Comparing `tmp/playlisterutil-3.0.1.tar.gz` & `tmp/playlisterutil-3.0.2.tar.gz`

## Comparing `playlisterutil-3.0.1.tar` & `playlisterutil-3.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 playlisterutil-3.0.1/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 playlisterutil-3.0.1/src/playlisterUtil/__init__.py
--rw-r--r--   0        0        0     5353 2020-02-02 00:00:00.000000 playlisterutil-3.0.1/src/playlisterUtil/playlisterUtil.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 playlisterutil-3.0.1/src/playlisterUtil/setup.py
--rw-r--r--   0        0        0     6492 2020-02-02 00:00:00.000000 playlisterutil-3.0.1/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 playlisterutil-3.0.1/LICENSE
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 playlisterutil-3.0.1/pyproject.toml
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 playlisterutil-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 playlisterutil-3.0.2/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 playlisterutil-3.0.2/src/playlisterUtil/__init__.py
+-rw-r--r--   0        0        0     5045 2020-02-02 00:00:00.000000 playlisterutil-3.0.2/src/playlisterUtil/playlisterUtil.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 playlisterutil-3.0.2/src/playlisterUtil/setup.py
+-rw-r--r--   0        0        0     6492 2020-02-02 00:00:00.000000 playlisterutil-3.0.2/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 playlisterutil-3.0.2/LICENSE
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 playlisterutil-3.0.2/pyproject.toml
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 playlisterutil-3.0.2/PKG-INFO
```

### Comparing `playlisterutil-3.0.1/src/playlisterUtil/playlisterUtil.py` & `playlisterutil-3.0.2/src/playlisterUtil/playlisterUtil.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,53 +15,46 @@
                     'title': '',
                     'video_id': '',
                     'mix_id': '',
                     'mix_index': -1,
                     'mix_name': '',
                     'mix_num_songs': '',
                     'channel_name': '',
-                    # Duration in seconds
                     'duration': -1,
                     'license': '',
                     'embeddable': False,
-                    # Determined by duration > 15min and youtube tags
-                    'is_multiple_songs': False, 
-                    # Is playlist or mix
+                    'is_multiple_songs': False,
                     'mix_type': '',
                 },
                 'spotify': {
                     'song': {
                         'name': '',
                         'open_url': '',
                         'preview_url': '',
                         'api_url': '',
-                        # Duration in seconds
                         'duration': -1,
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
                         'duration': -1
                     }
-
                 },
-                'createdAt': "",
-                'startedProcessing': "",
-                'finishedProcessing': "",
+                'createdAt': '',
+                'startedProcessing': '',
+                'finishedProcessing': '',
                 'id': -1,
-                # 0 not processed, 1 in process, 2 processed
                 'processed': 0,
-                # 0 didn't succeed, 1 succeed
                 'success': 0,
                 'retries': 0
             }
 
     def get_value(self, key, default=None):
         keys = key.split('.')
         value = self.data
```

### Comparing `playlisterutil-3.0.1/.gitignore` & `playlisterutil-3.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `playlisterutil-3.0.1/LICENSE` & `playlisterutil-3.0.2/LICENSE`

 * *Files identical despite different names*

