# Comparing `tmp/pylemmy-0.0.1.tar.gz` & `tmp/pylemmy-0.0.2.tar.gz`

## Comparing `pylemmy-0.0.1.tar` & `pylemmy-0.0.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 pylemmy-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 pylemmy-0.0.1/mkdocs.yml
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 pylemmy-0.0.1/.github/workflows/docs.yaml
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 pylemmy-0.0.1/.github/workflows/integration.yml
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 pylemmy-0.0.1/.github/workflows/lint.yaml
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 pylemmy-0.0.1/.github/workflows/publish.yaml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 pylemmy-0.0.1/docs/index.md
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pylemmy-0.0.1/docs/api/lemmy.md
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pylemmy-0.0.1/docs/api/utils.md
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pylemmy-0.0.1/docs/api/models/comment.md
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pylemmy-0.0.1/docs/api/models/community.md
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pylemmy-0.0.1/docs/api/models/post.md
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 pylemmy-0.0.1/examples/lmgtfy.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 pylemmy-0.0.1/pylemmy/__about__.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pylemmy-0.0.1/pylemmy/__init__.py
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 pylemmy-0.0.1/pylemmy/endpoints.py
--rw-r--r--   0        0        0     7107 2020-02-02 00:00:00.000000 pylemmy-0.0.1/pylemmy/lemmy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pylemmy-0.0.1/pylemmy/py.typed
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 pylemmy-0.0.1/pylemmy/utils.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pylemmy-0.0.1/pylemmy/api/__init__.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 pylemmy-0.0.1/pylemmy/api/auth.py
--rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 pylemmy-0.0.1/pylemmy/api/comment.py
--rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 pylemmy-0.0.1/pylemmy/api/community.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 pylemmy-0.0.1/pylemmy/api/listing.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 pylemmy-0.0.1/pylemmy/api/person.py
--rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 pylemmy-0.0.1/pylemmy/api/post.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 pylemmy-0.0.1/pylemmy/api/site.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 pylemmy-0.0.1/pylemmy/api/utils.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 pylemmy-0.0.1/pylemmy/models/__init__.py
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 pylemmy-0.0.1/pylemmy/models/comment.py
--rw-r--r--   0        0        0     4422 2020-02-02 00:00:00.000000 pylemmy-0.0.1/pylemmy/models/community.py
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 pylemmy-0.0.1/pylemmy/models/post.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pylemmy-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 pylemmy-0.0.1/tests/integration/__init__.py
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 pylemmy-0.0.1/tests/integration/docker-compose.yml
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 pylemmy-0.0.1/tests/integration/lemmy.hjson
--rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 pylemmy-0.0.1/tests/integration/test_api.py
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 pylemmy-0.0.1/tests/integration/test_lemmy.py
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 pylemmy-0.0.1/.gitignore
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 pylemmy-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 pylemmy-0.0.1/README.md
--rw-r--r--   0        0        0     4102 2020-02-02 00:00:00.000000 pylemmy-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 pylemmy-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 pylemmy-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 pylemmy-0.0.2/mkdocs.yml
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 pylemmy-0.0.2/.github/workflows/docs.yaml
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 pylemmy-0.0.2/.github/workflows/integration.yml
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 pylemmy-0.0.2/.github/workflows/lint.yaml
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 pylemmy-0.0.2/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 pylemmy-0.0.2/docs/index.md
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pylemmy-0.0.2/docs/api/lemmy.md
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pylemmy-0.0.2/docs/api/utils.md
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pylemmy-0.0.2/docs/api/models/comment.md
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pylemmy-0.0.2/docs/api/models/community.md
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pylemmy-0.0.2/docs/api/models/post.md
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 pylemmy-0.0.2/examples/lmgtfy.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 pylemmy-0.0.2/pylemmy/__about__.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pylemmy-0.0.2/pylemmy/__init__.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 pylemmy-0.0.2/pylemmy/endpoints.py
+-rw-r--r--   0        0        0     7579 2020-02-02 00:00:00.000000 pylemmy-0.0.2/pylemmy/lemmy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pylemmy-0.0.2/pylemmy/py.typed
+-rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 pylemmy-0.0.2/pylemmy/utils.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pylemmy-0.0.2/pylemmy/api/__init__.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 pylemmy-0.0.2/pylemmy/api/auth.py
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 pylemmy-0.0.2/pylemmy/api/comment.py
+-rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 pylemmy-0.0.2/pylemmy/api/community.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 pylemmy-0.0.2/pylemmy/api/listing.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 pylemmy-0.0.2/pylemmy/api/person.py
+-rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 pylemmy-0.0.2/pylemmy/api/post.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 pylemmy-0.0.2/pylemmy/api/site.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 pylemmy-0.0.2/pylemmy/api/utils.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 pylemmy-0.0.2/pylemmy/models/__init__.py
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 pylemmy-0.0.2/pylemmy/models/comment.py
+-rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 pylemmy-0.0.2/pylemmy/models/community.py
+-rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 pylemmy-0.0.2/pylemmy/models/post.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pylemmy-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 pylemmy-0.0.2/tests/integration/__init__.py
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 pylemmy-0.0.2/tests/integration/docker-compose.yml
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 pylemmy-0.0.2/tests/integration/lemmy.hjson
+-rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 pylemmy-0.0.2/tests/integration/test_api.py
+-rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 pylemmy-0.0.2/tests/integration/test_lemmy.py
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 pylemmy-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 pylemmy-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 pylemmy-0.0.2/README.md
+-rw-r--r--   0        0        0     4088 2020-02-02 00:00:00.000000 pylemmy-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 pylemmy-0.0.2/PKG-INFO
```

### Comparing `pylemmy-0.0.1/mkdocs.yml` & `pylemmy-0.0.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.1/.github/workflows/docs.yaml` & `pylemmy-0.0.2/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.1/.github/workflows/publish.yaml` & `pylemmy-0.0.2/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.1/docs/index.md` & `pylemmy-0.0.2/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 # pylemmy
 
-pylemmy enables simple access to [Lemmy](https://join-lemmy.org/)'s API with Python.
+[![PyPI - Version](https://img.shields.io/pypi/v/pylemmy.svg)](https://pypi.org/project/pylemmy)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pylemmy.svg)](https://pypi.org/project/pylemmy)
+
+-----
+
+**Table of Contents**
+
+- [Installation](#installation)
+- [Usage](#usage)
+- [License](#license)
 
 ## Installation
 
-```commandline
+```console
 pip install pylemmy
 ```
 
 ## Usage
 
 Simple example of running a Python function on new posts, as they are created.
 
@@ -18,16 +27,19 @@
 def process_post(post):
     ...
 
 lemmy = Lemmy(
     lemmy_url="http://127.0.0.1:8536",
     username="lemmy",
     password="lemmylemmy",
-    user_agent="LMGTFY (by u/USERNAME)",
+    user_agent="custom user agent (by u/USERNAME)",
 )
 
 community = lemmy.get_community("test")
 for post in community.stream.get_posts():
     process_post(post)
 ```
 
-For more examples, see [the examples directory on GitHub](https://github.com/dcferreira/pylemmy/tree/main/examples).
+## License
+
+`pylemmy` is distributed under the terms of the 
+[MIT](https://spdx.org/licenses/MIT.html) license.
```

### Comparing `pylemmy-0.0.1/examples/lmgtfy.py` & `pylemmy-0.0.2/examples/lmgtfy.py`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.1/pylemmy/lemmy.py` & `pylemmy-0.0.2/pylemmy/lemmy.py`

 * *Files 5% similar despite different names*

```diff
@@ -93,23 +93,36 @@
         """Get the jwt session token."""
         jwt = self.login().jwt
         if jwt is None:
             msg = "No jwt token was found, try logging in again."
             raise RuntimeError(msg)
         return jwt
 
+    def get_token_optional(self) -> Optional[str]:
+        """Get the jwt session token if it exists, or `None`.
+
+        This should be used for requests that don't need authentication.
+        """
+        if self.username is None or self.password is None:
+            return None
+        return self.get_token()
+
     def get_community(self, community: Union[str, int]) -> Community:
         """Get a community by id or name.
 
         :param community: Either a community id (int) or name (str).
         """
         if isinstance(community, str):
-            payload = api.community.GetCommunity(auth=self.get_token(), name=community)
+            payload = api.community.GetCommunity(
+                auth=self.get_token_optional(), name=community
+            )
         elif isinstance(community, int):
-            payload = api.community.GetCommunity(auth=self.get_token(), id=community)
+            payload = api.community.GetCommunity(
+                auth=self.get_token_optional(), id=community
+            )
         else:
             raise ValueError()
 
         result = self.get_request(LemmyAPI.Community, params=payload)
         parsed_result = api.community.GetCommunityResponse(**result)
         return Community(self, parsed_result.community_view)
 
@@ -131,32 +144,36 @@
 
     def list_communities(self, **kwargs) -> List[Community]:
         """List the communities in the current Lemmy instance.
 
         :param kwargs: See optional arguments in [ListCommunities](
         https://join-lemmy.org/api/interfaces/ListCommunities.html).
         """
-        payload = api.community.ListCommunities(auth=self.get_token(), **kwargs)
+        payload = api.community.ListCommunities(
+            auth=self.get_token_optional(), **kwargs
+        )
         result = self.get_request(LemmyAPI.ListCommunities, params=payload)
         parsed_result = api.community.ListCommunitiesResponse(**result)
 
         return [Community(self, view) for view in parsed_result.communities]
 
     def get_post(
         self, *, post_id: Optional[int] = None, comment_id: Optional[int] = None
     ) -> Post:
         """Get a post from its id.
 
         :param post_id: Id of the post.
         :param comment_id: Id of the comment.
         """
         if post_id is not None:
-            payload = api.post.GetPost(auth=self.get_token(), id=post_id)
+            payload = api.post.GetPost(auth=self.get_token_optional(), id=post_id)
         elif comment_id is not None:
-            payload = api.post.GetPost(auth=self.get_token(), comment_id=comment_id)
+            payload = api.post.GetPost(
+                auth=self.get_token_optional(), comment_id=comment_id
+            )
         else:
             msg = "Need to give either a post id or a comment id."
             raise ValueError(msg)
 
         result = self.get_request(LemmyAPI.Post, params=payload)
         parsed_result = api.post.GetPostResponse(**result)
```

### Comparing `pylemmy-0.0.1/pylemmy/utils.py` & `pylemmy-0.0.2/pylemmy/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,25 +31,25 @@
     """
     found_keys = set()
     count = 0
     last_key: str = ""
 
     wait_time = min_wait_time
     while True:
-        if limit is not None and count >= limit:
-            break
         first_key = last_key
         results = function(**function_kwargs)
         for r in filter(filter_fn, results):
             unique_key = unique_key_fn(r)
             if unique_key not in found_keys:
                 last_key = unique_key
                 yield r
+                count += 1
+                if limit is not None and count >= limit:
+                    return
                 found_keys.add(unique_key)
 
         if first_key == last_key:  # no new results
             wait_time = min(2 * wait_time, max_wait_time)
         else:
             wait_time = min_wait_time
 
         time.sleep(wait_time)
-        count += 1
```

### Comparing `pylemmy-0.0.1/pylemmy/api/comment.py` & `pylemmy-0.0.2/pylemmy/api/comment.py`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.1/pylemmy/api/community.py` & `pylemmy-0.0.2/pylemmy/api/community.py`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.1/pylemmy/api/post.py` & `pylemmy-0.0.2/pylemmy/api/post.py`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.1/pylemmy/models/comment.py` & `pylemmy-0.0.2/pylemmy/models/comment.py`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.1/pylemmy/models/community.py` & `pylemmy-0.0.2/pylemmy/models/community.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,29 +49,29 @@
     def get_posts(self, **kwargs) -> List[Post]:
         """Gets a list of Posts from this community.
 
         :param kwargs: See optional arguments in [GetPosts](
         https://join-lemmy.org/api/interfaces/GetPosts.html).
         """
         payload = api.post.GetPosts(
-            auth=self.lemmy.get_token(), community_id=self.safe.id, **kwargs
+            auth=self.lemmy.get_token_optional(), community_id=self.safe.id, **kwargs
         )
         result = self.lemmy.get_request(LemmyAPI.GetPosts, params=payload)
         parsed_result = api.post.GetPostsResponse(**result)
 
         return [Post(self.lemmy, post, community=self) for post in parsed_result.posts]
 
     def get_comments(self, **kwargs) -> List[Comment]:
         """Gets a list of Comments from this community.
 
         :param kwargs: See optional arguments in [GetComments](
         https://join-lemmy.org/api/interfaces/GetComments.html).
         """
         payload = api.comment.GetComments(
-            auth=self.lemmy.get_token(), community_id=self.safe.id, **kwargs
+            auth=self.lemmy.get_token_optional(), community_id=self.safe.id, **kwargs
         )
         result = self.lemmy.get_request(LemmyAPI.GetComments, params=payload)
         parsed_result = api.comment.GetCommentsResponse(**result)
 
         return [Comment(self.lemmy, comment) for comment in parsed_result.comments]
 
     @property
@@ -113,22 +113,22 @@
         """Get a stream of Posts in the Community.
 
         :param kwargs: See the arguments in
         [stream_generator][pylemmy.utils.stream_generator].
         """
         return stream_generator(
             self.community.get_posts,
-            lambda x: str(x.post_view.post_request.ap_id),
+            lambda x: str(x.post_view.post.ap_id),
             **kwargs,
         )
 
     def get_comments(self, **kwargs):
         """Get a stream of Comments in the Community.
 
         :param kwargs: See the arguments in
         [stream_generator][pylemmy.utils.stream_generator].
         """
         return stream_generator(
             self.community.get_comments,
-            lambda x: str(x.comment_view.Comment.ap_id),
+            lambda x: str(x.comment_view.comment.ap_id),
             **kwargs,
         )
```

### Comparing `pylemmy-0.0.1/pylemmy/models/post.py` & `pylemmy-0.0.2/pylemmy/models/post.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,17 @@
     def get_comments(self, **kwargs) -> List[Comment]:
         """Get Comments under this Post.
 
         :param kwargs: See optional arguments in [GetComments](
         https://join-lemmy.org/api/interfaces/GetComments.html).
         """
         payload = api.comment.GetComments(
-            auth=self.lemmy.get_token(), post_id=self.post_view.post.id, **kwargs
+            auth=self.lemmy.get_token_optional(),
+            post_id=self.post_view.post.id,
+            **kwargs,
         )
         result = self.lemmy.get_request(LemmyAPI.GetComments, params=payload)
         parsed_result = api.comment.GetCommentsResponse(**result)
 
         return [
             Comment(self.lemmy, comment, post=self, community=self._community)
             for comment in parsed_result.comments
```

### Comparing `pylemmy-0.0.1/tests/integration/docker-compose.yml` & `pylemmy-0.0.2/tests/integration/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.1/tests/integration/lemmy.hjson` & `pylemmy-0.0.2/tests/integration/lemmy.hjson`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.1/tests/integration/test_api.py` & `pylemmy-0.0.2/tests/integration/test_api.py`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.1/.gitignore` & `pylemmy-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.1/LICENSE.txt` & `pylemmy-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.1/pyproject.toml` & `pylemmy-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 dependencies = [
     "pydantic>=1.7",
     "requests>=2.18",
     "loguru>=0.3",
 ]
 
 [project.urls]
-Documentation = "https://github.com/dcferreira/pylemmy#readme"
+Documentation = "https://dcferreira.com/pylemmy"
 Issues = "https://github.com/dcferreira/pylemmy/issues"
 Source = "https://github.com/dcferreira/pylemmy"
 
 [tool.hatch.version]
 path = "pylemmy/__about__.py"
 
 [tool.hatch.envs.default]
```

### Comparing `pylemmy-0.0.1/PKG-INFO` & `pylemmy-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pylemmy
-Version: 0.0.1
+Version: 0.0.2
 Summary: pylemmy enables simple access to Lemmy's API with Python
-Project-URL: Documentation, https://github.com/dcferreira/pylemmy#readme
+Project-URL: Documentation, https://dcferreira.com/pylemmy
 Project-URL: Issues, https://github.com/dcferreira/pylemmy/issues
 Project-URL: Source, https://github.com/dcferreira/pylemmy
 Author-email: Daniel Ferreira <daniel.ferreira.1@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
@@ -52,15 +52,15 @@
 def process_post(post):
     ...
 
 lemmy = Lemmy(
     lemmy_url="http://127.0.0.1:8536",
     username="lemmy",
     password="lemmylemmy",
-    user_agent="LMGTFY (by u/USERNAME)",
+    user_agent="custom user agent (by u/USERNAME)",
 )
 
 community = lemmy.get_community("test")
 for post in community.stream.get_posts():
     process_post(post)
 ```
```

