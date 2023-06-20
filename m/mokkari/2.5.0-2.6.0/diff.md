# Comparing `tmp/mokkari-2.5.0.tar.gz` & `tmp/mokkari-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mokkari-2.5.0.tar", max compression
+gzip compressed data, was "mokkari-2.6.0.tar", max compression
```

## Comparing `mokkari-2.5.0.tar` & `mokkari-2.6.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0    35149 2023-05-20 15:15:39.131600 mokkari-2.5.0/LICENSE
--rw-r--r--   0        0        0     1946 2023-05-20 15:15:39.131600 mokkari-2.5.0/README.rst
--rw-r--r--   0        0        0     1250 2023-05-20 15:15:39.131600 mokkari-2.5.0/mokkari/__init__.py
--rw-r--r--   0        0        0     2960 2023-05-20 15:15:39.131600 mokkari-2.5.0/mokkari/arc.py
--rw-r--r--   0        0        0     3553 2023-05-20 15:15:39.131600 mokkari-2.5.0/mokkari/character.py
--rw-r--r--   0        0        0     3338 2023-05-20 15:15:39.131600 mokkari-2.5.0/mokkari/creator.py
--rw-r--r--   0        0        0      750 2023-05-20 15:15:39.131600 mokkari-2.5.0/mokkari/exceptions.py
--rw-r--r--   0        0        0     1148 2023-05-20 15:15:39.131600 mokkari-2.5.0/mokkari/genre.py
--rw-r--r--   0        0        0     9157 2023-05-20 15:15:39.131600 mokkari-2.5.0/mokkari/issue.py
--rw-r--r--   0        0        0     3257 2023-05-20 15:15:39.131600 mokkari-2.5.0/mokkari/publisher.py
--rw-r--r--   0        0        0     1148 2023-05-20 15:15:39.131600 mokkari-2.5.0/mokkari/rating.py
--rw-r--r--   0        0        0     1213 2023-05-20 15:15:39.131600 mokkari-2.5.0/mokkari/reprint.py
--rw-r--r--   0        0        0     7499 2023-05-20 15:15:39.131600 mokkari-2.5.0/mokkari/series.py
--rw-r--r--   0        0        0    14359 2023-05-20 15:15:39.131600 mokkari-2.5.0/mokkari/session.py
--rw-r--r--   0        0        0     2103 2023-05-20 15:15:39.131600 mokkari-2.5.0/mokkari/sqlite_cache.py
--rw-r--r--   0        0        0     3138 2023-05-20 15:15:39.131600 mokkari-2.5.0/mokkari/team.py
--rw-r--r--   0        0        0     1259 2023-05-20 15:15:39.131600 mokkari-2.5.0/mokkari/variant.py
--rw-r--r--   0        0        0     2334 2023-05-20 15:15:39.131600 mokkari-2.5.0/pyproject.toml
--rw-r--r--   0        0        0      544 2023-05-20 15:15:39.131600 mokkari-2.5.0/tests/README.md
--rw-r--r--   0        0        0       25 2023-05-20 15:15:39.131600 mokkari-2.5.0/tests/__init__.py
--rw-r--r--   0        0        0      734 2023-05-20 15:15:39.131600 mokkari-2.5.0/tests/conftest.py
--rw-r--r--   0        0        0     2590 2023-05-20 15:15:39.131600 mokkari-2.5.0/tests/test_arcs.py
--rw-r--r--   0        0        0     2075 2023-05-20 15:15:39.131600 mokkari-2.5.0/tests/test_cache.py
--rw-r--r--   0        0        0     3087 2023-05-20 15:15:39.131600 mokkari-2.5.0/tests/test_characters.py
--rw-r--r--   0        0        0     2594 2023-05-20 15:15:39.131600 mokkari-2.5.0/tests/test_creator.py
--rw-r--r--   0        0        0      659 2023-05-20 15:15:39.131600 mokkari-2.5.0/tests/test_init.py
--rw-r--r--   0        0        0    10082 2023-05-20 15:15:39.135600 mokkari-2.5.0/tests/test_issues.py
--rw-r--r--   0        0        0     2476 2023-05-20 15:15:39.135600 mokkari-2.5.0/tests/test_publishers.py
--rw-r--r--   0        0        0      714 2023-05-20 15:15:39.135600 mokkari-2.5.0/tests/test_role.py
--rw-r--r--   0        0        0     4091 2023-05-20 15:15:39.135600 mokkari-2.5.0/tests/test_series.py
--rw-r--r--   0        0        0      734 2023-05-20 15:15:39.135600 mokkari-2.5.0/tests/test_series_type.py
--rw-r--r--   0        0        0     2648 2023-05-20 15:15:39.135600 mokkari-2.5.0/tests/test_teams.py
--rw-r--r--   0        0        0   544768 2023-05-20 15:15:39.135600 mokkari-2.5.0/tests/testing_mock.sqlite
--rw-r--r--   0        0        0     3464 1970-01-01 00:00:00.000000 mokkari-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-20 18:43:00.250085 mokkari-2.6.0/LICENSE
+-rw-r--r--   0        0        0     1946 2023-06-20 18:43:00.250085 mokkari-2.6.0/README.rst
+-rw-r--r--   0        0        0     1250 2023-06-20 18:43:00.250085 mokkari-2.6.0/mokkari/__init__.py
+-rw-r--r--   0        0        0     2960 2023-06-20 18:43:00.250085 mokkari-2.6.0/mokkari/arc.py
+-rw-r--r--   0        0        0     3553 2023-06-20 18:43:00.250085 mokkari-2.6.0/mokkari/character.py
+-rw-r--r--   0        0        0     3338 2023-06-20 18:43:00.250085 mokkari-2.6.0/mokkari/creator.py
+-rw-r--r--   0        0        0      750 2023-06-20 18:43:00.250085 mokkari-2.6.0/mokkari/exceptions.py
+-rw-r--r--   0        0        0     1148 2023-06-20 18:43:00.250085 mokkari-2.6.0/mokkari/genre.py
+-rw-r--r--   0        0        0     9325 2023-06-20 18:43:00.250085 mokkari-2.6.0/mokkari/issue.py
+-rw-r--r--   0        0        0     3257 2023-06-20 18:43:00.250085 mokkari-2.6.0/mokkari/publisher.py
+-rw-r--r--   0        0        0     1148 2023-06-20 18:43:00.250085 mokkari-2.6.0/mokkari/rating.py
+-rw-r--r--   0        0        0     1213 2023-06-20 18:43:00.250085 mokkari-2.6.0/mokkari/reprint.py
+-rw-r--r--   0        0        0     7499 2023-06-20 18:43:00.250085 mokkari-2.6.0/mokkari/series.py
+-rw-r--r--   0        0        0    14359 2023-06-20 18:43:00.250085 mokkari-2.6.0/mokkari/session.py
+-rw-r--r--   0        0        0     2103 2023-06-20 18:43:00.250085 mokkari-2.6.0/mokkari/sqlite_cache.py
+-rw-r--r--   0        0        0     3138 2023-06-20 18:43:00.250085 mokkari-2.6.0/mokkari/team.py
+-rw-r--r--   0        0        0     1259 2023-06-20 18:43:00.250085 mokkari-2.6.0/mokkari/variant.py
+-rw-r--r--   0        0        0     2380 2023-06-20 18:43:00.250085 mokkari-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0      544 2023-06-20 18:43:00.250085 mokkari-2.6.0/tests/README.md
+-rw-r--r--   0        0        0       25 2023-06-20 18:43:00.250085 mokkari-2.6.0/tests/__init__.py
+-rw-r--r--   0        0        0      734 2023-06-20 18:43:00.250085 mokkari-2.6.0/tests/conftest.py
+-rw-r--r--   0        0        0     2590 2023-06-20 18:43:00.250085 mokkari-2.6.0/tests/test_arcs.py
+-rw-r--r--   0        0        0     2075 2023-06-20 18:43:00.250085 mokkari-2.6.0/tests/test_cache.py
+-rw-r--r--   0        0        0     3087 2023-06-20 18:43:00.250085 mokkari-2.6.0/tests/test_characters.py
+-rw-r--r--   0        0        0     2594 2023-06-20 18:43:00.250085 mokkari-2.6.0/tests/test_creator.py
+-rw-r--r--   0        0        0      659 2023-06-20 18:43:00.250085 mokkari-2.6.0/tests/test_init.py
+-rw-r--r--   0        0        0    10082 2023-06-20 18:43:00.254085 mokkari-2.6.0/tests/test_issues.py
+-rw-r--r--   0        0        0     2476 2023-06-20 18:43:00.254085 mokkari-2.6.0/tests/test_publishers.py
+-rw-r--r--   0        0        0      714 2023-06-20 18:43:00.254085 mokkari-2.6.0/tests/test_role.py
+-rw-r--r--   0        0        0     4091 2023-06-20 18:43:00.254085 mokkari-2.6.0/tests/test_series.py
+-rw-r--r--   0        0        0      734 2023-06-20 18:43:00.254085 mokkari-2.6.0/tests/test_series_type.py
+-rw-r--r--   0        0        0     2648 2023-06-20 18:43:00.254085 mokkari-2.6.0/tests/test_teams.py
+-rw-r--r--   0        0        0   544768 2023-06-20 18:43:00.254085 mokkari-2.6.0/tests/testing_mock.sqlite
+-rw-r--r--   0        0        0     3464 1970-01-01 00:00:00.000000 mokkari-2.6.0/PKG-INFO
```

### Comparing `mokkari-2.5.0/LICENSE` & `mokkari-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mokkari-2.5.0/README.rst` & `mokkari-2.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `mokkari-2.5.0/mokkari/__init__.py` & `mokkari-2.6.0/mokkari/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Project entry file."""
 
 # Keep this at beginning of file to prevent circular import with session
-__version__ = "2.5.0"
+__version__ = "2.6.0"
 
 from typing import Optional
 
 from mokkari import exceptions, session, sqlite_cache
 
 
 def api(
```

### Comparing `mokkari-2.5.0/mokkari/arc.py` & `mokkari-2.6.0/mokkari/arc.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.5.0/mokkari/character.py` & `mokkari-2.6.0/mokkari/character.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.5.0/mokkari/creator.py` & `mokkari-2.6.0/mokkari/creator.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.5.0/mokkari/exceptions.py` & `mokkari-2.6.0/mokkari/exceptions.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.5.0/mokkari/genre.py` & `mokkari-2.6.0/mokkari/genre.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.5.0/mokkari/issue.py` & `mokkari-2.6.0/mokkari/issue.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,14 +162,15 @@
         price (decimal): The price of the issue.
         rating (Rating): The issue rating.
         sku (str): Stock keeping unit for the issue.
         upc (str): UPC barcode for the issue.
         page_count (int): Number of pages for the issue.
         desc (str): Summary description for the issue.
         image (url): The url for a cover image associated with the issue.
+        cover_hash (str): A Perceptual hash string for the cover image.
         arcs (list[:obj:`Arc`]): A list of story arcs.
         credits (list[:obj:`Credit`]): A list of creator credits for the issue.
         characters (list[:obj:`Character`]): A list of characters who appear in the issue.
         teams (list[:obj:`Team`]): A list of teams who appear in the issue.
         reprints (list[:obj:`Reprint`]): A list of reprinted issue contained in the issue.
         issue_name (str): The name used to identified the issue.
         variants (list[:obj:`Variant`]): A list of variant covers for the issue.
@@ -228,14 +229,18 @@
     .. versionchanged:: 2.3.3
 
         - Added ``resource_url`` field.
 
     .. versionadded:: 2.4.0
 
         - Added ``cv_id`` field.
+
+    .. versionadded:: 2.6.0
+
+        - Add ``cover_hash`` field.
     """
 
     id = fields.Int()
     publisher = fields.Nested(PublisherSchema)
     series = fields.Nested(SeriesSchema)
     number = fields.Str()
     collection_title = fields.Str(allow_none=True, data_key="title")
@@ -245,14 +250,15 @@
     price = fields.Decimal(places=2, allow_none=True)
     rating = fields.Nested(RatingSchema)
     sku = fields.Str()
     upc = fields.Str()
     page_count = fields.Int(allow_none=True, data_key="page")
     desc = fields.Str(allow_none=True)
     image = fields.URL(allow_none=True)
+    cover_hash = fields.Str()
     arcs = fields.Nested(ArcSchema, many=True)
     credits = fields.Nested(CreditsSchema, many=True)
     characters = fields.Nested(CharacterSchema, many=True)
     teams = fields.Nested(TeamSchema, many=True)
     reprints = fields.Nested(ReprintSchema, many=True)
     issue_name = fields.Str(data_key="issue")
     variants = fields.Nested(VariantSchema, many=True)
```

### Comparing `mokkari-2.5.0/mokkari/publisher.py` & `mokkari-2.6.0/mokkari/publisher.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.5.0/mokkari/rating.py` & `mokkari-2.6.0/mokkari/rating.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.5.0/mokkari/reprint.py` & `mokkari-2.6.0/mokkari/reprint.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.5.0/mokkari/series.py` & `mokkari-2.6.0/mokkari/series.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.5.0/mokkari/session.py` & `mokkari-2.6.0/mokkari/session.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.5.0/mokkari/sqlite_cache.py` & `mokkari-2.6.0/mokkari/sqlite_cache.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.5.0/mokkari/team.py` & `mokkari-2.6.0/mokkari/team.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.5.0/mokkari/variant.py` & `mokkari-2.6.0/mokkari/variant.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.5.0/pyproject.toml` & `mokkari-2.6.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mokkari"
-version = "2.5.0"
+version = "2.6.0"
 description = "Python wrapper for Metron API"
 authors = ["Brian Pepple <bdpepple@gmail.com>"]
 license = "GPL-3.0-or-later"
 maintainers = ["Brian Pepple <bdpepple@gmail.com>"]
 readme = "README.rst"
 packages = [
 	{ include = "mokkari" },
@@ -17,14 +17,15 @@
     "Environment :: Console",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Natural Language :: English",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Internet",
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: POSIX",
     "Operating System :: POSIX :: BSD",
     "Operating System :: POSIX :: Linux",
     "Operating System :: Microsoft :: Windows",
 ]
```

### Comparing `mokkari-2.5.0/tests/README.md` & `mokkari-2.6.0/tests/README.md`

 * *Files identical despite different names*

### Comparing `mokkari-2.5.0/tests/conftest.py` & `mokkari-2.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.5.0/tests/test_arcs.py` & `mokkari-2.6.0/tests/test_arcs.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.5.0/tests/test_cache.py` & `mokkari-2.6.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.5.0/tests/test_characters.py` & `mokkari-2.6.0/tests/test_characters.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.5.0/tests/test_creator.py` & `mokkari-2.6.0/tests/test_creator.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.5.0/tests/test_init.py` & `mokkari-2.6.0/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.5.0/tests/test_issues.py` & `mokkari-2.6.0/tests/test_issues.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.5.0/tests/test_publishers.py` & `mokkari-2.6.0/tests/test_publishers.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.5.0/tests/test_role.py` & `mokkari-2.6.0/tests/test_role.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.5.0/tests/test_series.py` & `mokkari-2.6.0/tests/test_series.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.5.0/tests/test_series_type.py` & `mokkari-2.6.0/tests/test_series_type.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.5.0/tests/test_teams.py` & `mokkari-2.6.0/tests/test_teams.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.5.0/tests/testing_mock.sqlite` & `mokkari-2.6.0/tests/testing_mock.sqlite`

 * *Files identical despite different names*

### Comparing `mokkari-2.5.0/PKG-INFO` & `mokkari-2.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mokkari
-Version: 2.5.0
+Version: 2.6.0
 Summary: Python wrapper for Metron API
 License: GPL-3.0-or-later
 Keywords: comics,comic,metadata
 Author: Brian Pepple
 Author-email: bdpepple@gmail.com
 Maintainer: Brian Pepple
 Maintainer-email: bdpepple@gmail.com
```

