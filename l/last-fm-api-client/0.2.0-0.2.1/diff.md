# Comparing `tmp/last_fm_api_client-0.2.0.tar.gz` & `tmp/last_fm_api_client-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "last_fm_api_client-0.2.0.tar", max compression
+gzip compressed data, was "last_fm_api_client-0.2.1.tar", max compression
```

## Comparing `last_fm_api_client-0.2.0.tar` & `last_fm_api_client-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-05-28 17:55:46.624956 last_fm_api_client-0.2.0/last_fm_api_client/__init__.py
--rw-r--r--   0        0        0    11414 2023-06-03 18:30:38.302558 last_fm_api_client-0.2.0/last_fm_api_client/client.py
--rw-r--r--   0        0        0     9801 2023-06-20 18:02:17.528624 last_fm_api_client-0.2.0/last_fm_api_client/models.py
--rw-r--r--   0        0        0      383 2023-06-20 15:23:51.725038 last_fm_api_client-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      770 2023-06-20 15:23:51.705702 last_fm_api_client-0.2.0/README.md
--rw-r--r--   0        0        0     1213 1970-01-01 00:00:00.000000 last_fm_api_client-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-28 17:55:46.624956 last_fm_api_client-0.2.1/last_fm_api_client/__init__.py
+-rw-r--r--   0        0        0    11414 2023-06-03 18:30:38.302558 last_fm_api_client-0.2.1/last_fm_api_client/client.py
+-rw-r--r--   0        0        0     9989 2023-06-20 18:26:06.148746 last_fm_api_client-0.2.1/last_fm_api_client/models.py
+-rw-r--r--   0        0        0      383 2023-06-20 18:26:06.155528 last_fm_api_client-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      871 2023-06-20 18:26:06.142712 last_fm_api_client-0.2.1/README.md
+-rw-r--r--   0        0        0     1312 1970-01-01 00:00:00.000000 last_fm_api_client-0.2.1/PKG-INFO
```

### Comparing `last_fm_api_client-0.2.0/last_fm_api_client/client.py` & `last_fm_api_client-0.2.1/last_fm_api_client/client.py`

 * *Files identical despite different names*

### Comparing `last_fm_api_client-0.2.0/last_fm_api_client/models.py` & `last_fm_api_client-0.2.1/last_fm_api_client/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,16 +57,18 @@
     """Represents a certain date."""
     timestamp: datetime.datetime = Field(alias="uts")
     text: str = Field(alias="#text")
     _normalize_timestamp = validator("timestamp", allow_reuse=True, pre=True)(convert_unix_timestamp_to_datetime)
 
 class UndetailedMetadata(BaseModel):
     """Represents data for an undetailed album or artist in Last.FM that only includes two keys: #text and mbid."""
-    text: str = Field(alias="#text")
+    text: Optional[str] = Field(alias="#text")
     mbid: Optional[str]
+    _normalize_text = validator("text", allow_reuse=True)(convert_empty_string_to_none)
+    _normalize_mbid = validator("mbid", allow_reuse=True)(convert_empty_string_to_none)
 
 class LinkMetadata(BaseModel):
     """Represents data for a link in the Last.Fm page"""
     href: str
     text: Optional[str] = Field(alias="#text")
     rel: Optional[str]
```

### Comparing `last_fm_api_client-0.2.0/PKG-INFO` & `last_fm_api_client-0.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: last-fm-api-client
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Author: William04A
 Author-email: 35110380+William04A@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -23,12 +23,14 @@
 The following [Last.FM API methods](https://www.last.fm/api/intro) are implemented:
 * `album.getInfo` - get information about an album
 * `artist.getInfo` - get information about an artist
 * `tag.getInfo` - get information about a tag
 * `user.getRecentTracks` - retrieve scrobbles
 
 ### Changelog:
+* `v0.2.1`: Fixed empty album text being converted to None.
 * `v0.2.0`: Better handling of unset/empty Last.FM values.
 
    **Breaking changes:**
   * The field `Album.Tracks` is now optional and may return `None`.
+  * Same applies for all image fields.
 * `v0.1.0`: Initial release
```

