# Comparing `tmp/pythorhead-0.2.0.tar.gz` & `tmp/pythorhead-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythorhead-0.2.0.tar", last modified: Mon Jun 19 15:36:06 2023, max compression
+gzip compressed data, was "pythorhead-0.3.0.tar", last modified: Tue Jun 20 09:03:34 2023, max compression
```

## Comparing `pythorhead-0.2.0.tar` & `pythorhead-0.3.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:36:06.477785 pythorhead-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:36:06.473785 pythorhead-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:36:06.473785 pythorhead-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-19 15:35:47.000000 pythorhead-0.2.0/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-19 15:35:47.000000 pythorhead-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-06-19 15:35:53.000000 pythorhead-0.2.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-19 15:35:47.000000 pythorhead-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    40749 2023-06-19 15:36:06.477785 pythorhead-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-19 15:35:47.000000 pythorhead-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   121595 2023-06-19 15:35:47.000000 pythorhead-0.2.0/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-19 15:35:53.000000 pythorhead-0.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:36:06.473785 pythorhead-0.2.0/pythorhead/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-19 15:35:47.000000 pythorhead-0.2.0/pythorhead/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-19 15:35:47.000000 pythorhead-0.2.0/pythorhead/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-19 15:35:47.000000 pythorhead-0.2.0/pythorhead/lemmy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-06-19 15:35:47.000000 pythorhead-0.2.0/pythorhead/post.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-19 15:35:47.000000 pythorhead-0.2.0/pythorhead/requestor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:36:06.477785 pythorhead-0.2.0/pythorhead/types/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-19 15:35:47.000000 pythorhead-0.2.0/pythorhead/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-19 15:35:47.000000 pythorhead-0.2.0/pythorhead/types/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-19 15:35:47.000000 pythorhead-0.2.0/pythorhead/types/listing.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-19 15:35:47.000000 pythorhead-0.2.0/pythorhead/types/sort.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:36:06.473785 pythorhead-0.2.0/pythorhead.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    40749 2023-06-19 15:36:06.000000 pythorhead-0.2.0/pythorhead.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-19 15:36:06.000000 pythorhead-0.2.0/pythorhead.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 15:36:06.000000 pythorhead-0.2.0/pythorhead.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-19 15:36:06.000000 pythorhead-0.2.0/pythorhead.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 15:35:47.000000 pythorhead-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 15:36:06.477785 pythorhead-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:03:34.386103 pythorhead-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:03:34.382103 pythorhead-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:03:34.382103 pythorhead-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-20 09:03:13.000000 pythorhead-0.3.0/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-20 09:03:13.000000 pythorhead-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-06-20 09:03:21.000000 pythorhead-0.3.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-20 09:03:13.000000 pythorhead-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    41047 2023-06-20 09:03:34.386103 pythorhead-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-20 09:03:13.000000 pythorhead-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   121595 2023-06-20 09:03:13.000000 pythorhead-0.3.0/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-20 09:03:21.000000 pythorhead-0.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:03:34.382103 pythorhead-0.3.0/pythorhead/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-20 09:03:13.000000 pythorhead-0.3.0/pythorhead/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-20 09:03:13.000000 pythorhead-0.3.0/pythorhead/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-06-20 09:03:13.000000 pythorhead-0.3.0/pythorhead/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-20 09:03:13.000000 pythorhead-0.3.0/pythorhead/lemmy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-06-20 09:03:13.000000 pythorhead-0.3.0/pythorhead/post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-20 09:03:13.000000 pythorhead-0.3.0/pythorhead/requestor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:03:34.382103 pythorhead-0.3.0/pythorhead/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-20 09:03:13.000000 pythorhead-0.3.0/pythorhead/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-20 09:03:13.000000 pythorhead-0.3.0/pythorhead/types/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-20 09:03:13.000000 pythorhead-0.3.0/pythorhead/types/listing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-20 09:03:13.000000 pythorhead-0.3.0/pythorhead/types/sort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:03:34.382103 pythorhead-0.3.0/pythorhead.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    41047 2023-06-20 09:03:34.000000 pythorhead-0.3.0/pythorhead.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-20 09:03:34.000000 pythorhead-0.3.0/pythorhead.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 09:03:34.000000 pythorhead-0.3.0/pythorhead.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-20 09:03:34.000000 pythorhead-0.3.0/pythorhead.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 09:03:13.000000 pythorhead-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 09:03:34.386103 pythorhead-0.3.0/setup.cfg
```

### Comparing `pythorhead-0.2.0/.github/workflows/pypi.yml` & `pythorhead-0.3.0/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `pythorhead-0.2.0/.gitignore` & `pythorhead-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pythorhead-0.2.0/CHANGELOG.md` & `pythorhead-0.3.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,22 @@
 # Changelog
 
+## [v0.3.0](https://github.com/db0/pythorhead/tree/v0.3.0) (2023-06-20)
+
+[Full Changelog](https://github.com/db0/pythorhead/compare/v0.2.0...v0.3.0)
+
+**Closed issues:**
+
+- Return post id on create? [\#9](https://github.com/db0/pythorhead/issues/9)
+- Dependency on loguru [\#6](https://github.com/db0/pythorhead/issues/6)
+
+**Merged pull requests:**
+
+- Comments [\#11](https://github.com/db0/pythorhead/pull/11) ([NicKoehler](https://github.com/NicKoehler))
+
 ## [v0.2.0](https://github.com/db0/pythorhead/tree/v0.2.0) (2023-06-19)
 
 [Full Changelog](https://github.com/db0/pythorhead/compare/v0.1.1...v0.2.0)
 
 **Closed issues:**
 
 - TypeError: unsupported operand type\(s\) for |: 'type' and 'NoneType' [\#5](https://github.com/db0/pythorhead/issues/5)
```

### Comparing `pythorhead-0.2.0/LICENSE` & `pythorhead-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pythorhead-0.2.0/PKG-INFO` & `pythorhead-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythorhead
-Version: 0.2.0
+Version: 0.3.0
 Summary: A python library for interacting with Lemmy API
 Author-email: db0 <mail@dbzer0.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -677,17 +677,33 @@
 
 # Pythörhead
 
 A python library for interacting with Lemmy
 
 ![pythorhead logo](https://raw.githubusercontent.com/db0/pythorhead/main/logo.png)
 
-# Sample Usage
+# Sample Post Usage
 
 ```python
 from pythorhead import Lemmy
 
 lemmy = Lemmy("https://lemmy.dbzer0.com")
 lemmy.log_in("username", "password")
 community_id = lemmy.discover_community("botart")
 lemmy.post.create(community_id, "Hello Lemmy World")
 ```
+
+# Sample Comment Usage
+
+```python
+from pythorhead import Lemmy
+
+lemmy = Lemmy("https://lemmy.dbzer0.com")
+lemmy.log_in("username", "password")
+
+# getting the first post id
+post_id = lemmy.post.list()[0]["post"]["id"]
+
+# leave a comment
+lemmy.comment.create(post_id, "Hello Lemmy World")
+
+```
```

### Comparing `pythorhead-0.2.0/logo.png` & `pythorhead-0.3.0/logo.png`

 * *Files identical despite different names*

### Comparing `pythorhead-0.2.0/pyproject.toml` & `pythorhead-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "pythorhead"
 description = "A python library for interacting with Lemmy API"
 authors = [
     {name = "db0", email = "mail@dbzer0.com"},
 ]
-version = "v0.2.0"
+version = "v0.3.0"
 readme = "README.md"
 requires-python = ">=3.8,<3.11"
 license = { file="LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU Affero General Public License v3",
     "Operating System :: OS Independent",
```

### Comparing `pythorhead-0.2.0/pythorhead/auth.py` & `pythorhead-0.3.0/pythorhead/auth.py`

 * *Files identical despite different names*

### Comparing `pythorhead-0.2.0/pythorhead/lemmy.py` & `pythorhead-0.3.0/pythorhead/lemmy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import logging
-
 from typing import Optional
 
+from pythorhead.comment import Comment
 from pythorhead.post import Post
-from pythorhead.requestor import Requestor, Request
+from pythorhead.requestor import Request, Requestor
 
 logging.basicConfig(format="%(asctime)s - %(name)s - %(levelname)s - %(message)s")
 
 
 class Lemmy:
     post: Post
+    comment: Comment
     _known_communities = {}
     _requestor: Requestor
 
     def __init__(self, api_base_url: str) -> None:
         self._requestor = Requestor()
         self._requestor.set_api_base_url(f"{api_base_url}/api/v3")
         self.post = Post()
+        self.comment = Comment()
 
     def log_in(self, username_or_email: str, password: str) -> bool:
         return self._requestor.log_in(username_or_email, password)
 
     def discover_community(self, community_name: str) -> Optional[int]:
         if community_name in self._known_communities:
             return self._known_communities[community_name]
```

### Comparing `pythorhead-0.2.0/pythorhead/post.py` & `pythorhead-0.3.0/pythorhead/post.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from typing import Any, Literal, Optional, List
+from typing import Any, List, Literal, Optional
 
-from pythorhead.types import FeatureType, ListingType, SortType
-from pythorhead.requestor import Requestor, Request
+from pythorhead.requestor import Request, Requestor
+from pythorhead.types import FeatureType, ListingType, PostSortType
 
 
 class Post:
     def __init__(self):
         self._requestor = Requestor()
 
     def get(
@@ -35,15 +35,15 @@
     def list(  # noqa: A003
         self,
         community_id: Optional[int] = None,
         community_name: Optional[str] = None,
         limit: Optional[int] = None,
         page: Optional[int] = None,
         saved_only: Optional[bool] = None,
-        sort: Optional[SortType] = None,
+        sort: Optional[PostSortType] = None,
         type_: Optional[ListingType] = None,
     ) -> List[dict]:
         """
 
         Get posts, with various filters.
 
         Args:
@@ -198,15 +198,15 @@
         if language_id is not None:
             edit_post["language_id"] = language_id
 
         return self._requestor.request(Request.PUT, "/post", json=edit_post)
 
     def like(self, post_id: int, score: Literal[-1, 0, 1]) -> Optional[dict]:
         """
-        Like a post
+        Like / Dislike a post
 
         Args:
             post_id (int)
             score (int)
 
         Returns:
             Optional[dict]: post data if successful
@@ -216,15 +216,15 @@
             "score": score,
         }
         return self._requestor.request(Request.POST, "/post/like", json=like_post)
 
     def save(self, post_id: int, saved: bool) -> Optional[dict]:
         """
 
-        Save / Unsave a post
+        Add / Remove a post to saved posts
 
         Args:
             post_id (int)
             saved (bool)
 
         Returns:
             Optional[dict]: post data if successful
```

### Comparing `pythorhead-0.2.0/pythorhead/requestor.py` & `pythorhead-0.3.0/pythorhead/requestor.py`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-import requests
 import logging
-
 from enum import Enum
 from typing import Optional
-from pythorhead.auth import Authentication
 
+import requests
+
+from pythorhead.auth import Authentication
 
 logger = logging.getLogger(__name__)
 
 
 class Request(Enum):
     GET = "GET"
     PUT = "PUT"
```

### Comparing `pythorhead-0.2.0/pythorhead.egg-info/PKG-INFO` & `pythorhead-0.3.0/pythorhead.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythorhead
-Version: 0.2.0
+Version: 0.3.0
 Summary: A python library for interacting with Lemmy API
 Author-email: db0 <mail@dbzer0.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -677,17 +677,33 @@
 
 # Pythörhead
 
 A python library for interacting with Lemmy
 
 ![pythorhead logo](https://raw.githubusercontent.com/db0/pythorhead/main/logo.png)
 
-# Sample Usage
+# Sample Post Usage
 
 ```python
 from pythorhead import Lemmy
 
 lemmy = Lemmy("https://lemmy.dbzer0.com")
 lemmy.log_in("username", "password")
 community_id = lemmy.discover_community("botart")
 lemmy.post.create(community_id, "Hello Lemmy World")
 ```
+
+# Sample Comment Usage
+
+```python
+from pythorhead import Lemmy
+
+lemmy = Lemmy("https://lemmy.dbzer0.com")
+lemmy.log_in("username", "password")
+
+# getting the first post id
+post_id = lemmy.post.list()[0]["post"]["id"]
+
+# leave a comment
+lemmy.comment.create(post_id, "Hello Lemmy World")
+
+```
```

