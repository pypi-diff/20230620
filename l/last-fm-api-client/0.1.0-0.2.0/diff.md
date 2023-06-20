# Comparing `tmp/last_fm_api_client-0.1.0.tar.gz` & `tmp/last_fm_api_client-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "last_fm_api_client-0.1.0.tar", max compression
+gzip compressed data, was "last_fm_api_client-0.2.0.tar", max compression
```

## Comparing `last_fm_api_client-0.1.0.tar` & `last_fm_api_client-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-05-28 17:55:46.624956 last_fm_api_client-0.1.0/last_fm_api_client/__init__.py
--rw-r--r--   0        0        0    11414 2023-06-03 18:30:38.302558 last_fm_api_client-0.1.0/last_fm_api_client/client.py
--rw-r--r--   0        0        0     8118 2023-06-03 18:22:40.682016 last_fm_api_client-0.1.0/last_fm_api_client/models.py
--rw-r--r--   0        0        0      383 2023-05-28 17:59:30.856779 last_fm_api_client-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      566 2023-06-03 18:28:29.276442 last_fm_api_client-0.1.0/README.md
--rw-r--r--   0        0        0     1016 1970-01-01 00:00:00.000000 last_fm_api_client-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-28 17:55:46.624956 last_fm_api_client-0.2.0/last_fm_api_client/__init__.py
+-rw-r--r--   0        0        0    11414 2023-06-03 18:30:38.302558 last_fm_api_client-0.2.0/last_fm_api_client/client.py
+-rw-r--r--   0        0        0     9801 2023-06-20 18:02:17.528624 last_fm_api_client-0.2.0/last_fm_api_client/models.py
+-rw-r--r--   0        0        0      383 2023-06-20 15:23:51.725038 last_fm_api_client-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      770 2023-06-20 15:23:51.705702 last_fm_api_client-0.2.0/README.md
+-rw-r--r--   0        0        0     1213 1970-01-01 00:00:00.000000 last_fm_api_client-0.2.0/PKG-INFO
```

### Comparing `last_fm_api_client-0.1.0/last_fm_api_client/client.py` & `last_fm_api_client-0.2.0/last_fm_api_client/client.py`

 * *Files identical despite different names*

### Comparing `last_fm_api_client-0.1.0/README.md` & `last_fm_api_client-0.2.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -6,8 +6,15 @@
 
 ### Implemented API methods
 
 The following [Last.FM API methods](https://www.last.fm/api/intro) are implemented:
 * `album.getInfo` - get information about an album
 * `artist.getInfo` - get information about an artist
 * `tag.getInfo` - get information about a tag
-* `user.getRecentTracks` - retrieve scrobbles
+* `user.getRecentTracks` - retrieve scrobbles
+
+### Changelog:
+* `v0.2.0`: Better handling of unset/empty Last.FM values.
+
+   **Breaking changes:**
+  * The field `Album.Tracks` is now optional and may return `None`.
+* `v0.1.0`: Initial release
```

