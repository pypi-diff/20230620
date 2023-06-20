# Comparing `tmp/playlisterutil-2.0.8.tar.gz` & `tmp/playlisterutil-2.0.9.tar.gz`

## Comparing `playlisterutil-2.0.8.tar` & `playlisterutil-2.0.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 playlisterutil-2.0.8/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 playlisterutil-2.0.8/src/playlisterUtil/__init__.py
--rw-r--r--   0        0        0     5180 2020-02-02 00:00:00.000000 playlisterutil-2.0.8/src/playlisterUtil/playlisterUtil.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 playlisterutil-2.0.8/src/playlisterUtil/setup.py
--rw-r--r--   0        0        0     6492 2020-02-02 00:00:00.000000 playlisterutil-2.0.8/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 playlisterutil-2.0.8/LICENSE
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 playlisterutil-2.0.8/pyproject.toml
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 playlisterutil-2.0.8/PKG-INFO
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 playlisterutil-2.0.9/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 playlisterutil-2.0.9/src/playlisterUtil/__init__.py
+-rw-r--r--   0        0        0     5348 2020-02-02 00:00:00.000000 playlisterutil-2.0.9/src/playlisterUtil/playlisterUtil.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 playlisterutil-2.0.9/src/playlisterUtil/setup.py
+-rw-r--r--   0        0        0     6492 2020-02-02 00:00:00.000000 playlisterutil-2.0.9/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 playlisterutil-2.0.9/LICENSE
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 playlisterutil-2.0.9/pyproject.toml
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 playlisterutil-2.0.9/PKG-INFO
```

### Comparing `playlisterutil-2.0.8/src/playlisterUtil/playlisterUtil.py` & `playlisterutil-2.0.9/src/playlisterUtil/playlisterUtil.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,19 +12,23 @@
             self.data = {
                 'youtube': {
                     'url': '',
                     'title': '',
                     'video_id': '',
                     'mix_id': '',
                     'mix_index': '',
+                    'playlist_name': '',
+                    'playlist_num_songs': '',
+                    'channel_name': '',
                     'duration': '',
                     'license': '',
                     'embeddable': False,
-                    # Determined by duration > 30min and youtube tags
+                    # Determined by duration > 15min and youtube tags
                     'is_multiple_songs': False, 
+                    # Is playlist or mix
                     'is_mix': False,
                 },
                 'spotify': {
                     'api_href': '',
                     'song': {
                         'name': '',
                         'open_url': '',
```

### Comparing `playlisterutil-2.0.8/.gitignore` & `playlisterutil-2.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `playlisterutil-2.0.8/LICENSE` & `playlisterutil-2.0.9/LICENSE`

 * *Files identical despite different names*

