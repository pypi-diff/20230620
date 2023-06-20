# Comparing `tmp/meilisearch_python_async-1.4.0.tar.gz` & `tmp/meilisearch_python_async-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meilisearch_python_async-1.4.0.tar", max compression
+gzip compressed data, was "meilisearch_python_async-1.4.1.tar", max compression
```

## Comparing `meilisearch_python_async-1.4.0.tar` & `meilisearch_python_async-1.4.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1069 2023-06-09 01:38:23.373640 meilisearch_python_async-1.4.0/LICENSE
--rw-r--r--   0        0        0     5759 2023-06-09 01:38:23.373640 meilisearch_python_async-1.4.0/README.md
--rw-r--r--   0        0        0      151 2023-06-09 01:38:23.373640 meilisearch_python_async-1.4.0/meilisearch_python_async/__init__.py
--rw-r--r--   0        0        0     2759 2023-06-09 01:38:23.373640 meilisearch_python_async-1.4.0/meilisearch_python_async/_http_requests.py
--rw-r--r--   0        0        0       18 2023-06-09 01:38:23.373640 meilisearch_python_async-1.4.0/meilisearch_python_async/_version.py
--rw-r--r--   0        0        0    22205 2023-06-09 01:38:23.373640 meilisearch_python_async-1.4.0/meilisearch_python_async/client.py
--rw-r--r--   0        0        0     2085 2023-06-09 01:38:23.373640 meilisearch_python_async-1.4.0/meilisearch_python_async/errors.py
--rw-r--r--   0        0        0    89041 2023-06-09 01:38:23.373640 meilisearch_python_async-1.4.0/meilisearch_python_async/index.py
--rw-r--r--   0        0        0        0 2023-06-09 01:38:23.373640 meilisearch_python_async-1.4.0/meilisearch_python_async/models/__init__.py
--rw-r--r--   0        0        0     1576 2023-06-09 01:38:23.373640 meilisearch_python_async-1.4.0/meilisearch_python_async/models/client.py
--rw-r--r--   0        0        0      202 2023-06-09 01:38:23.373640 meilisearch_python_async-1.4.0/meilisearch_python_async/models/documents.py
--rw-r--r--   0        0        0       95 2023-06-09 01:38:23.373640 meilisearch_python_async-1.4.0/meilisearch_python_async/models/health.py
--rw-r--r--   0        0        0      392 2023-06-09 01:38:23.373640 meilisearch_python_async-1.4.0/meilisearch_python_async/models/index.py
--rw-r--r--   0        0        0     1285 2023-06-09 01:38:23.373640 meilisearch_python_async-1.4.0/meilisearch_python_async/models/search.py
--rw-r--r--   0        0        0     1119 2023-06-09 01:38:23.373640 meilisearch_python_async-1.4.0/meilisearch_python_async/models/settings.py
--rw-r--r--   0        0        0      769 2023-06-09 01:38:23.373640 meilisearch_python_async-1.4.0/meilisearch_python_async/models/task.py
--rw-r--r--   0        0        0      215 2023-06-09 01:38:23.373640 meilisearch_python_async-1.4.0/meilisearch_python_async/models/version.py
--rw-r--r--   0        0        0        0 2023-06-09 01:38:23.373640 meilisearch_python_async-1.4.0/meilisearch_python_async/py.typed
--rw-r--r--   0        0        0    11932 2023-06-09 01:38:23.377640 meilisearch_python_async-1.4.0/meilisearch_python_async/task.py
--rw-r--r--   0        0        0     2286 2023-06-09 01:38:23.377640 meilisearch_python_async-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     6968 1970-01-01 00:00:00.000000 meilisearch_python_async-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-20 15:19:01.840695 meilisearch_python_async-1.4.1/LICENSE
+-rw-r--r--   0        0        0     5759 2023-06-20 15:19:01.840695 meilisearch_python_async-1.4.1/README.md
+-rw-r--r--   0        0        0      151 2023-06-20 15:19:01.844694 meilisearch_python_async-1.4.1/meilisearch_python_async/__init__.py
+-rw-r--r--   0        0        0     2759 2023-06-20 15:19:01.844694 meilisearch_python_async-1.4.1/meilisearch_python_async/_http_requests.py
+-rw-r--r--   0        0        0       18 2023-06-20 15:19:01.844694 meilisearch_python_async-1.4.1/meilisearch_python_async/_version.py
+-rw-r--r--   0        0        0    22205 2023-06-20 15:19:01.844694 meilisearch_python_async-1.4.1/meilisearch_python_async/client.py
+-rw-r--r--   0        0        0     2085 2023-06-20 15:19:01.844694 meilisearch_python_async-1.4.1/meilisearch_python_async/errors.py
+-rw-r--r--   0        0        0    89041 2023-06-20 15:19:01.844694 meilisearch_python_async-1.4.1/meilisearch_python_async/index.py
+-rw-r--r--   0        0        0        0 2023-06-20 15:19:01.844694 meilisearch_python_async-1.4.1/meilisearch_python_async/models/__init__.py
+-rw-r--r--   0        0        0     1576 2023-06-20 15:19:01.844694 meilisearch_python_async-1.4.1/meilisearch_python_async/models/client.py
+-rw-r--r--   0        0        0      202 2023-06-20 15:19:01.844694 meilisearch_python_async-1.4.1/meilisearch_python_async/models/documents.py
+-rw-r--r--   0        0        0       95 2023-06-20 15:19:01.844694 meilisearch_python_async-1.4.1/meilisearch_python_async/models/health.py
+-rw-r--r--   0        0        0      392 2023-06-20 15:19:01.844694 meilisearch_python_async-1.4.1/meilisearch_python_async/models/index.py
+-rw-r--r--   0        0        0     1285 2023-06-20 15:19:01.844694 meilisearch_python_async-1.4.1/meilisearch_python_async/models/search.py
+-rw-r--r--   0        0        0     1119 2023-06-20 15:19:01.844694 meilisearch_python_async-1.4.1/meilisearch_python_async/models/settings.py
+-rw-r--r--   0        0        0      769 2023-06-20 15:19:01.844694 meilisearch_python_async-1.4.1/meilisearch_python_async/models/task.py
+-rw-r--r--   0        0        0      215 2023-06-20 15:19:01.844694 meilisearch_python_async-1.4.1/meilisearch_python_async/models/version.py
+-rw-r--r--   0        0        0        0 2023-06-20 15:19:01.844694 meilisearch_python_async-1.4.1/meilisearch_python_async/py.typed
+-rw-r--r--   0        0        0    11932 2023-06-20 15:19:01.844694 meilisearch_python_async-1.4.1/meilisearch_python_async/task.py
+-rw-r--r--   0        0        0     2286 2023-06-20 15:19:01.848693 meilisearch_python_async-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     6968 1970-01-01 00:00:00.000000 meilisearch_python_async-1.4.1/PKG-INFO
```

### Comparing `meilisearch_python_async-1.4.0/LICENSE` & `meilisearch_python_async-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.0/README.md` & `meilisearch_python_async-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.0/meilisearch_python_async/_http_requests.py` & `meilisearch_python_async-1.4.1/meilisearch_python_async/_http_requests.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.0/meilisearch_python_async/client.py` & `meilisearch_python_async-1.4.1/meilisearch_python_async/client.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.0/meilisearch_python_async/errors.py` & `meilisearch_python_async-1.4.1/meilisearch_python_async/errors.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,24 +28,24 @@
     def __init__(self, error: str, response: Response) -> None:
         self.status_code = response.status_code
         self.code = ""
         self.message = ""
         self.link = ""
         self.error_type = ""
         if response.content:
-            self.message = f" Error message: {response.json().get('message') or ''}."
+            self.message = f"Error message: {response.json().get('message') or ''}"
             self.code = f"{response.json().get('code') or ''}"
             self.error_type = f"{response.json().get('type') or ''}"
-            self.link = f" Error documentation: {response.json().get('link') or ''}"
+            self.link = f"Error documentation: {response.json().get('link') or ''}"
         else:
             self.message = error
         super().__init__(self.message)
 
     def __str__(self) -> str:
-        return f"MeilisearchApiError.{self.code}{self.message}{self.error_type}{self.link}"
+        return f"MeilisearchApiError.{self.code} {self.message} {self.error_type} {self.link}"
 
 
 class MeilisearchCommunicationError(MeilisearchError):
     """Error when connecting to Meilisearch."""
 
     def __str__(self) -> str:
         return f"MeilisearchCommunicationError, {self.message}"
```

### Comparing `meilisearch_python_async-1.4.0/meilisearch_python_async/index.py` & `meilisearch_python_async-1.4.1/meilisearch_python_async/index.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.0/meilisearch_python_async/models/client.py` & `meilisearch_python_async-1.4.1/meilisearch_python_async/models/client.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.0/meilisearch_python_async/models/search.py` & `meilisearch_python_async-1.4.1/meilisearch_python_async/models/search.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.0/meilisearch_python_async/models/settings.py` & `meilisearch_python_async-1.4.1/meilisearch_python_async/models/settings.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.0/meilisearch_python_async/models/task.py` & `meilisearch_python_async-1.4.1/meilisearch_python_async/models/task.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.0/meilisearch_python_async/task.py` & `meilisearch_python_async-1.4.1/meilisearch_python_async/task.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.0/pyproject.toml` & `meilisearch_python_async-1.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "meilisearch-python-async"
-version = "1.4.0"
+version = "1.4.1"
 description = "A Python async client for the Meilisearch API"
 authors = ["Paul Sanders <psanders1@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/sanders41/meilisearch-python-async"
 homepage = "https://github.com/sanders41/meilisearch-python-async"
 documentation = "https://meilisearch-python-async.paulsanders.dev"
```

### Comparing `meilisearch_python_async-1.4.0/PKG-INFO` & `meilisearch_python_async-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meilisearch-python-async
-Version: 1.4.0
+Version: 1.4.1
 Summary: A Python async client for the Meilisearch API
 Home-page: https://github.com/sanders41/meilisearch-python-async
 License: MIT
 Keywords: meilisearch,async,python
 Author: Paul Sanders
 Author-email: psanders1@gmail.com
 Requires-Python: >=3.7,<4.0
```

