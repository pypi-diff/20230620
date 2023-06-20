# Comparing `tmp/drukarnia-api-0.1.90.tar.gz` & `tmp/drukarnia-api-0.1.912.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drukarnia-api-0.1.90.tar", last modified: Mon Jun 19 13:13:18 2023, max compression
+gzip compressed data, was "drukarnia-api-0.1.912.tar", last modified: Tue Jun 20 17:23:02 2023, max compression
```

## Comparing `drukarnia-api-0.1.90.tar` & `drukarnia-api-0.1.912.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:13:18.317161 drukarnia-api-0.1.90/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-19 13:13:08.000000 drukarnia-api-0.1.90/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-06-19 13:13:18.313161 drukarnia-api-0.1.90/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-06-19 13:13:08.000000 drukarnia-api-0.1.90/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:13:18.313161 drukarnia-api-0.1.90/drukarnia_api/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-19 13:13:08.000000 drukarnia-api-0.1.90/drukarnia_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-06-19 13:13:08.000000 drukarnia-api-0.1.90/drukarnia_api/article.py
--rw-r--r--   0 runner    (1001) docker     (123)    11263 2023-06-19 13:13:08.000000 drukarnia-api-0.1.90/drukarnia_api/author.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:13:18.313161 drukarnia-api-0.1.90/drukarnia_api/drukarnia_base/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-19 13:13:08.000000 drukarnia-api-0.1.90/drukarnia_api/drukarnia_base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-06-19 13:13:08.000000 drukarnia-api-0.1.90/drukarnia_api/drukarnia_base/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-06-19 13:13:08.000000 drukarnia-api-0.1.90/drukarnia_api/drukarnia_base/element.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-19 13:13:08.000000 drukarnia-api-0.1.90/drukarnia_api/drukarnia_base/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-06-19 13:13:08.000000 drukarnia-api-0.1.90/drukarnia_api/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:13:18.313161 drukarnia-api-0.1.90/drukarnia_api/shortcuts/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-19 13:13:08.000000 drukarnia-api-0.1.90/drukarnia_api/shortcuts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-19 13:13:08.000000 drukarnia-api-0.1.90/drukarnia_api/shortcuts/class_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-06-19 13:13:08.000000 drukarnia-api-0.1.90/drukarnia_api/tag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:13:18.313161 drukarnia-api-0.1.90/drukarnia_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-06-19 13:13:18.000000 drukarnia-api-0.1.90/drukarnia_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-19 13:13:18.000000 drukarnia-api-0.1.90/drukarnia_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 13:13:18.000000 drukarnia-api-0.1.90/drukarnia_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-19 13:13:18.000000 drukarnia-api-0.1.90/drukarnia_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-19 13:13:18.000000 drukarnia-api-0.1.90/drukarnia_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 13:13:18.317161 drukarnia-api-0.1.90/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-06-19 13:13:08.000000 drukarnia-api-0.1.90/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:23:02.287340 drukarnia-api-0.1.912/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-20 17:22:53.000000 drukarnia-api-0.1.912/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-06-20 17:23:02.287340 drukarnia-api-0.1.912/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-06-20 17:22:53.000000 drukarnia-api-0.1.912/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:23:02.287340 drukarnia-api-0.1.912/drukarnia_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-20 17:22:53.000000 drukarnia-api-0.1.912/drukarnia_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10406 2023-06-20 17:22:53.000000 drukarnia-api-0.1.912/drukarnia_api/article.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12060 2023-06-20 17:22:53.000000 drukarnia-api-0.1.912/drukarnia_api/author.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:23:02.287340 drukarnia-api-0.1.912/drukarnia_api/drukarnia_base/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-20 17:22:53.000000 drukarnia-api-0.1.912/drukarnia_api/drukarnia_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-06-20 17:22:53.000000 drukarnia-api-0.1.912/drukarnia_api/drukarnia_base/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-06-20 17:22:53.000000 drukarnia-api-0.1.912/drukarnia_api/drukarnia_base/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-20 17:22:53.000000 drukarnia-api-0.1.912/drukarnia_api/drukarnia_base/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-06-20 17:22:53.000000 drukarnia-api-0.1.912/drukarnia_api/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:23:02.287340 drukarnia-api-0.1.912/drukarnia_api/shortcuts/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-20 17:22:53.000000 drukarnia-api-0.1.912/drukarnia_api/shortcuts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-20 17:22:53.000000 drukarnia-api-0.1.912/drukarnia_api/shortcuts/class_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-06-20 17:22:53.000000 drukarnia-api-0.1.912/drukarnia_api/tag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:23:02.287340 drukarnia-api-0.1.912/drukarnia_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-06-20 17:23:02.000000 drukarnia-api-0.1.912/drukarnia_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-20 17:23:02.000000 drukarnia-api-0.1.912/drukarnia_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 17:23:02.000000 drukarnia-api-0.1.912/drukarnia_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-20 17:23:02.000000 drukarnia-api-0.1.912/drukarnia_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-20 17:23:02.000000 drukarnia-api-0.1.912/drukarnia_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 17:23:02.287340 drukarnia-api-0.1.912/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-20 17:22:53.000000 drukarnia-api-0.1.912/setup.py
```

### Comparing `drukarnia-api-0.1.90/LICENSE` & `drukarnia-api-0.1.912/LICENSE`

 * *Files identical despite different names*

### Comparing `drukarnia-api-0.1.90/PKG-INFO` & `drukarnia-api-0.1.912/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drukarnia-api
-Version: 0.1.90
+Version: 0.1.912
 Summary: wrapper for the Drukarnia API
 Home-page: https://github.com/androu-sys/drukarnia-api
 Author: Andrii Herts
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `drukarnia-api-0.1.90/README.md` & `drukarnia-api-0.1.912/README.md`

 * *Files identical despite different names*

### Comparing `drukarnia-api-0.1.90/drukarnia_api/article.py` & `drukarnia-api-0.1.912/drukarnia_api/article.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from aiohttp import ClientSession
 
 from drukarnia_api.drukarnia_base import DrukarniaElement
 from drukarnia_api.shortcuts import data2authors, data2articles, data2tags
 
 from typing import TYPE_CHECKING, Tuple, Dict, List
 
-if TYPE_CHECKING:   # always False, used for type hints
+if TYPE_CHECKING:  # always False, used for type hints
     from drukarnia_api.author import Author
     from drukarnia_api.tag import Tag
 
 
 class Article(DrukarniaElement):
     def __init__(self, slug: str = None, article_id: str = None, *args, **kwargs):
         """
@@ -24,95 +24,97 @@
     @DrukarniaElement._control_attr('article_id')
     @DrukarniaElement._is_authenticated
     async def post_comment(self, comment_text: str) -> str:
         """
         Posts a comment on the article and returns the ID of the posted comment.
         """
 
-        posted_comment_id = await self.post('/api/articles/{_id}/comments'.format(_id=self.article_id),
-                                            {'comment': comment_text}, output='read')
+        posted_comment_id = await self.request('post', '/api/articles/{_id}/comments'.format(_id=self.article_id),
+                                               data={'comment': comment_text}, output='read')
         return str(posted_comment_id)
 
     @DrukarniaElement._control_attr('article_id')
     @DrukarniaElement._is_authenticated
     async def reply2comment(self, comment_text: str, comment_id: str, root_comment: str,
                             root_comment_owner: str, reply2user: str) -> str:
         """
         Posts a reply to a comment and returns the ID of the new comment.
         """
 
-        new_comment_id = await self.post(
-            f'/api/articles/{self.article_id}/comments/{comment_id}/replies',
-            {
-                "comment": comment_text, "replyToComment": comment_id, "rootComment": root_comment,
-                "rootCommentOwner": root_comment_owner, "replyToUser": reply2user
-            },
-            output='read'
-        )
+        new_comment_id = await self.request('post',
+                                            f'/api/articles/{self.article_id}/comments/{comment_id}/replies',
+                                            data={
+                                                  "comment": comment_text, "replyToComment": comment_id,
+                                                  "rootComment": root_comment,
+                                                  "rootCommentOwner": root_comment_owner, "replyToUser": reply2user
+                                                },
+                                            output='read'
+                                            )
 
-        return str(new_comment_id)
+        return new_comment_id.decode('utf-8')
 
     @DrukarniaElement._control_attr('article_id')
     @DrukarniaElement._is_authenticated
     async def delete_comment(self, comment_id: str) -> None:
         """
         Deletes a comment from the article.
         """
 
-        await self.delete(f'/api/articles/{self.article_id}/comments/{comment_id}', [])
+        await self.request('delete', f'/api/articles/{self.article_id}/comments/{comment_id}')
 
     @DrukarniaElement._control_attr('article_id')
     @DrukarniaElement._is_authenticated
-    async def like_comment(self, comment_id: str, delete: bool = False) -> None:
+    async def like_comment(self, comment_id: str, unlike: bool = False) -> None:
         """
         Likes or unlikes a comment based on the 'delete' parameter.
         """
 
-        if delete:
-            await self.delete(f'/api/articles/{self.article_id}/comments/{comment_id}/likes', [])
+        if unlike:
+            await self.request('delete', f'/api/articles/{self.article_id}/comments/{comment_id}/likes')
 
         else:
-            await self.post(f'/api/articles/{self.article_id}/comments/{comment_id}/likes', {}, [])
+            await self.request('post', f'/api/articles/{self.article_id}/comments/{comment_id}/likes')
 
     @DrukarniaElement._control_attr('article_id')
     @DrukarniaElement._is_authenticated
     async def like_article(self, n_likes: int) -> None:
         """
         Likes the article with the specified number of likes.
         """
 
         if not (0 <= n_likes <= 10):
             raise ValueError('Number of likes must be greater or equal to zero and lower or equal to ten')
 
-        await self.post(f'/api/articles/{self.article_id}/like', {'likes': n_likes}, 'read')
+        await self.request('post', f'/api/articles/{self.article_id}/like', data={'likes': n_likes})
 
     @DrukarniaElement._control_attr('article_id')
     @DrukarniaElement._is_authenticated
     async def bookmark(self, section_id: str = '', unbookmark: bool = False) -> None:
         """
         Adds or removes the article from bookmarks based on the 'unbookmark' parameter.
         """
 
         if unbookmark:
-            await self.delete(f'/api/articles/{self.article_id}/bookmarks', [])
+            await self.request('delete', f'/api/articles/{self.article_id}/bookmarks')
 
         elif not section_id:
-            raise ValueError('section_id must be passed to bookmark')
+            raise ValueError('section_id must be passed for bookmarking')
 
         else:
-            await self.post('/api/articles/bookmarks', {"article": self.article_id, "list": section_id}, [])
+            await self.request('post', '/api/articles/bookmarks',
+                               data={"article": self.article_id, "list": section_id})
 
     @DrukarniaElement._control_attr('slug')
     async def collect_data(self, return_: bool = False) -> Dict or None:
         """
         Collects the article's data and updates the object's attributes.
         If 'return_' is True, returns the collected data.
         """
 
-        data = await self.get(f'/api/articles/{self.slug}', output='json')
+        data = await self.request('get', f'/api/articles/{self.slug}', output='json')
 
         self._update_data(data)
 
         if return_:
             return data
 
     @property
@@ -144,23 +146,21 @@
     def relationships(self) -> Dict:
         """
         Retrieves the relationships of the article.
         """
         return self._get_basetype_from_data('relationships', dict)
 
     @property
-    @DrukarniaElement._is_authenticated
     def is_bookmarked(self) -> bool:
         """
         Checks if the article is bookmarked.
         """
         return self._get_basetype_from_data('isBookmarked', bool)
 
     @property
-    @DrukarniaElement._is_authenticated
     def is_liked(self) -> bool:
         """
         Checks if the article is liked.
         """
         return self._get_basetype_from_data('isLiked', bool)
 
     @property
```

### Comparing `drukarnia-api-0.1.90/drukarnia_api/author.py` & `drukarnia-api-0.1.912/drukarnia_api/author.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,35 +20,39 @@
 
         self._update_data({'username': username, '_id': author_id})
 
     async def login(self, email: str, password: str) -> None:
         """
         Log in the author with the provided email and password.
         """
+
         # Make a POST request to log in the author
-        headers, info = await self.post('/api/users/login',
-                                        data={'password': password, 'email': email},
-                                        output=['headers', 'json'])
+        headers, info = await self.request('post',
+                                           '/api/users/login',
+                                           data={"password": password, "email": email},
+                                           output=['headers', 'json'])
 
         if self.author_id and (self.author_id != info['user']['_id']):
             raise ValueError('You are trying to log into an unrelated author.')
 
         elif self.username and (self.username != info['user']['username']):
             raise ValueError('You are trying to log into an unrelated author.')
 
         elif not (self.author_id or self.username):
             warn("We weren't able to identify any relationship between the current Author data and the Drukarnia "
                  "User you are trying to log into. It may cause unexpected and fatal errors. Please consider "
                  "initializing the Author class with the same username and _id as your Drukarnia User.")
 
+        self._update_data(info['user'])
+
         headers = str(headers)
         token = re.search(r'refreshToken=(.*?);', headers).group(1)
         device_id = re.search(r'deviceId=(.*?);', headers).group(1)
 
-        self.session.headers.update({'Cookie': f'deviceId={device_id}; token={token};'})
+        self._update_headers({'Cookie': f'deviceId={device_id}; token={token};'})
 
     @DrukarniaElement._control_attr('author_id')
     async def get_followers(self, create_authors: bool = True, offset: int = 0, results_per_page: int = 20,
                             n_collect: int = None, *args, **kwargs) -> Tuple['Author'] or Tuple[Dict]:
         """
         Get the followers of the author.
         """
@@ -85,139 +89,155 @@
         Get the notifications of the author.
         """
         return await self.multi_page_request('/api/notifications',
                                              offset, results_per_page, n_collect,
                                              *args, **kwargs)
 
     @DrukarniaElement._is_authenticated
-    async def get_reads_history(self, offset: int = 0, results_per_page: int = 20,
-                                n_collect: int = None, *args, **kwargs) -> List[Dict]:
+    async def get_reads_history(self, create_articles: bool = True, offset: int = 0,
+                                results_per_page: int = 20, n_collect: int = None,
+                                *args, **kwargs) -> List[Dict] or List['Article']:
         """
         Get the reading history of the author.
         """
-        return await self.multi_page_request('/api/stats/reads/history',
-                                             offset, results_per_page, n_collect,
-                                             *args, **kwargs)
+        articles = await self.multi_page_request('/api/stats/reads/history',
+                                                 offset, results_per_page, n_collect,
+                                                 *args, **kwargs)
+
+        if create_articles:
+            articles = await data2articles(articles, self.session)
+
+        return articles
 
     @DrukarniaElement._is_authenticated
-    async def get_sections(self, preview: bool = True, *args, **kwargs) -> Dict or List:
+    async def get_sections(self, preview: bool = True, **kwargs) -> List[dict]:
         """
         Get the sections of the author's articles.
         """
-        return await self.get(f'/api/articles/bookmarks/lists?preview={str(preview).lower()}',
-                              output='json', *args, **kwargs)
+        return await self.request('get', f'/api/articles/bookmarks/lists?preview={str(preview).lower()}',
+                                  output='json', **kwargs)
 
     @DrukarniaElement._is_authenticated
-    async def create_section(self, name: str, **kwargs) -> str:
+    async def create_section(self, name: str, **kwargs) -> List[Dict]:
         """
         Create a new section for the author's articles.
         """
-        section_id = await self.post('/api/articles/bookmarks/lists', data={"name": name}, output='read', **kwargs)
+        section_id = await self.request('get',
+                                        '/api/articles/bookmarks/lists',
+                                        data={"name": name},
+                                        output='read', **kwargs)
 
-        return str(section_id)
+        return section_id.decode('utf-8')
 
     @DrukarniaElement._is_authenticated
     async def delete_section(self, section_id: str, **kwargs) -> None:
         """
         Delete a section for the author's articles.
         """
-        await self.delete(f'/api/articles/bookmarks/lists/{section_id}', **kwargs)
+        await self.request('delete', f'/api/articles/bookmarks/lists/{section_id}', **kwargs)
 
     @DrukarniaElement._is_authenticated
     async def subscribe_author(self, author_id: str, unsubscribe: bool = False) -> None:
         """
         Subscribe or unsubscribe to/from an author.
         """
+
         if unsubscribe:
-            await self.delete(f'/api/relationships/subscribe/{author_id}')
+            await self.request('delete', f'/api/relationships/subscribe/{author_id}')
             return None
 
-        await self.post(f'/api/relationships/subscribe/{author_id}')
+        await self.request('post', f'/api/relationships/subscribe/{author_id}')
 
     @DrukarniaElement._is_authenticated
     async def subscribe_tag(self, tag_id: str, unsubscribe: bool = False) -> None:
         """
         Subscribe or unsubscribe to/from a tag.
         """
         if unsubscribe:
-            await self.delete(f'/api/preferences/tags/{tag_id}')
+            await self.request('delete', f'/api/preferences/tags/{tag_id}')
             return None
 
-        await self.put(f'/api/preferences/tags/{tag_id}')
+        await self.request('put', f'/api/preferences/tags/{tag_id}')
 
     @DrukarniaElement._is_authenticated
     async def block_tag(self, tag_id: str, unblock: bool = False) -> None:
         """
         Block or unblock an author.
         """
         if unblock:
-            await self.put(f'/api/preferences/tags/{tag_id}/block', data={"isBlocked": 'false'})
+            await self.request('put', f'/api/preferences/tags/{tag_id}/block', data={"isBlocked": False})
             return None
 
-        await self.put(f'/api/preferences/tags/{tag_id}/block', data={"isBlocked": 'true'})
+        await self.request('put', f'/api/preferences/tags/{tag_id}/block', data={"isBlocked": True})
 
     @DrukarniaElement._is_authenticated
     async def block_author(self, author_id: str, unblock: bool = False) -> None:
         """
         Block or unblock an author.
         """
         if unblock:
-            await self.patch(f'/api/relationships/block/{author_id}')
+            await self.request('patch', f'/api/relationships/block/{author_id}')
             return None
 
-        await self.put(f'/api/relationships/block/{author_id}')
+        await self.request('put', f'/api/relationships/block/{author_id}')
 
     @DrukarniaElement._is_authenticated
-    async def get_blocked(self) -> List or Dict:
+    async def get_blocked(self, create_authors: bool = False) -> List[Dict] or Tuple['Author']:
         """
         Get the authors blocked by the current author.
         """
-        return await self.get('/api/relationships/blocked')
+
+        authors = await self.request('get', '/api/relationships/blocked', output='json')
+
+        if create_authors:
+            authors = await data2authors(authors, self.session)
+
+        return authors
 
     @DrukarniaElement._is_authenticated
     async def change_password(self, old_password: str, new_password: str, **kwargs) -> None:
         """
         Change the author's password.
         """
-        await self.patch(f'/api/users/login/password',
-                         data={"oldPassword": old_password, "newPassword": new_password},
-                         output='read', **kwargs)
+        await self.request('patch', f'/api/users/login/password',
+                           data={"oldPassword": old_password, "newPassword": new_password},
+                           output='read', **kwargs)
 
     @DrukarniaElement._is_authenticated
     async def change_user_info(self, name: str = None, description: str = None, username: str = None,
                                description_short: str = None, socials: dict = None, donate_url: str = None) -> str:
         """
         Change the author's user information.
         """
         info2patch = {"name": name, "description": description, "username": username,
                       "descriptionShort": description_short,
                       "socials": socials, "donateUrl": donate_url}
 
         info2patch = {key: value for key, value in info2patch.items() if value is not None}
 
-        response = await self.patch('/api/users', data=info2patch, output='read')
-        return str(response)
+        response = await self.request('patch', '/api/users', data=info2patch, output='read')
+        return response.decode('utf-8')
 
     @DrukarniaElement._is_authenticated
     async def change_email(self, current_password: str, new_email: str, **kwargs) -> None:
         """
         Change the author's email.
         """
-        await self.patch(f'/api/users/login/email',
-                         data={"currentPassword": current_password, "newEmail": new_email},
-                         output='read', **kwargs)
+        await self.request('patch', f'/api/users/login/email',
+                           data={"currentPassword": current_password, "newEmail": new_email},
+                           **kwargs)
 
     @DrukarniaElement._control_attr('username')
     async def collect_data(self, return_: bool = False) -> Dict or None:
         """
         Collect the author's data and update the object's attributes.
         """
 
-        data = await self.get('/api/users/profile/{username}'.format(username=self.username),
-                              output='json')
+        data = await self.request('get', '/api/users/profile/{username}'.format(username=self.username),
+                                  output='json')
 
         self._update_data(data)
 
         if return_:
             return data
 
     @property
```

### Comparing `drukarnia-api-0.1.90/drukarnia_api/drukarnia_base/element.py` & `drukarnia-api-0.1.912/drukarnia_api/drukarnia_base/element.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Any, Callable
 from warnings import warn
 from datetime import datetime
+import inspect
 from drukarnia_api.drukarnia_base.connection import Connection
 from drukarnia_api.drukarnia_base.exceptions import DrukarniaElementDataError
 
 
 class DrukarniaElement(Connection):
     """
     A class representing a printing element in a printing shop.
@@ -25,19 +26,22 @@
             default (Any): The default value if the key is not found. If set to 'auto', the default value will be
                            an instance of the specified type.
 
         Returns:
             Any: The value from the author data dictionary casted to the specified type or the default value.
 
         """
+
         if default == 'auto':
             default = type_()
 
+        check = lambda el1: el1 is default if default is None else el1 == default
+
         n = self._access_data(key, default)
-        return type_(n) if n != default else n
+        return type_(n) if check(n) else n
 
     def _get_datetime_from_author_data(self, key: str):
         """
         Get a datetime object from the specified key in the author data dictionary.
 
         Args:
             key (str): The key to access the value in the author data dictionary.
```

### Comparing `drukarnia-api-0.1.90/drukarnia_api/drukarnia_base/exceptions.py` & `drukarnia-api-0.1.912/drukarnia_api/drukarnia_base/exceptions.py`

 * *Files identical despite different names*

### Comparing `drukarnia-api-0.1.90/drukarnia_api/search.py` & `drukarnia-api-0.1.912/drukarnia_api/search.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,22 +40,31 @@
                                                  offset, results_per_page, n_collect, *args, **kwargs)
 
         if create_articles:
             articles = await data2articles(articles, self.session)
 
         return articles
 
-    async def find_tags(self, query: str, create_tags: bool = True,
-                        offset: int = 0, results_per_page: int = 20, n_collect: int = None,
-                        *args, **kwargs) -> Tuple['Tag'] or Tuple[Dict]:
+    async def find_tags(self, query: str, create_tags: bool = True, get_articles: bool = False,
+                        create_articles: bool = True, offset: int = 0, results_per_page: int = 20,
+                        n_collect: int = None, *args, **kwargs) -> Tuple['Tag'] or Tuple[Dict]:
         """
         Search for tags.
         """
 
         # Make a request to get articles
-        tags = await self.multi_page_request(f'/api/articles/search/tags?text={query}',
-                                             offset, results_per_page, n_collect, *args, **kwargs)
+        tags, articles = await self.multi_page_request(f'/api/articles/search/tags?text={query}',
+                                                       list_key=['tags', 'articles'],
+                                                       offset=offset,
+                                                       results_per_page=results_per_page,
+                                                       n_collect=n_collect, *args, **kwargs)
+
+        if get_articles:
+            if create_articles:
+                articles = await data2articles(articles, self.session)
+
+            return tags, articles
 
         if create_tags:
             tags = await data2tags(tags, self.session)
 
         return tags
```

### Comparing `drukarnia-api-0.1.90/drukarnia_api/shortcuts/class_generator.py` & `drukarnia-api-0.1.912/drukarnia_api/shortcuts/class_generator.py`

 * *Files identical despite different names*

### Comparing `drukarnia-api-0.1.90/drukarnia_api.egg-info/PKG-INFO` & `drukarnia-api-0.1.912/drukarnia_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drukarnia-api
-Version: 0.1.90
+Version: 0.1.912
 Summary: wrapper for the Drukarnia API
 Home-page: https://github.com/androu-sys/drukarnia-api
 Author: Andrii Herts
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `drukarnia-api-0.1.90/drukarnia_api.egg-info/SOURCES.txt` & `drukarnia-api-0.1.912/drukarnia_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drukarnia-api-0.1.90/setup.py` & `drukarnia-api-0.1.912/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # Get requirements
 with open(path.join(HERE, 'requirements.txt')) as f:
     requirements = f.read().splitlines()
 
 # This call to setup() does all the work
 setup(
     name="drukarnia-api",
-    version="0.1.90",
+    version="0.1.912",
     description="wrapper for the Drukarnia API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/androu-sys/drukarnia-api",
     author="Andrii Herts",
     license="MIT",
     classifiers=[
```

