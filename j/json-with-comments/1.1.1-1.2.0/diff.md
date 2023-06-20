# Comparing `tmp/json-with-comments-1.1.1.tar.gz` & `tmp/json_with_comments-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json-with-comments-1.1.1.tar", max compression
+gzip compressed data, was "json_with_comments-1.2.0.tar", max compression
```

## Comparing `json-with-comments-1.1.1.tar` & `json_with_comments-1.2.0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     3163 2022-12-06 02:38:25.528529 json-with-comments-1.1.1/jsonc/__init__.py
--rw-r--r--   0        0        0     1088 2022-07-20 23:36:52.080807 json-with-comments-1.1.1/LICENSE
--rw-r--r--   0        0        0      680 2022-12-06 02:35:40.105549 json-with-comments-1.1.1/pyproject.toml
--rw-r--r--   0        0        0      983 2022-07-24 23:24:41.732329 json-with-comments-1.1.1/README.md
--rw-r--r--   0        0        0     1695 1970-01-01 00:00:00.000000 json-with-comments-1.1.1/setup.py
--rw-r--r--   0        0        0     1772 1970-01-01 00:00:00.000000 json-with-comments-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     9619 2023-06-20 19:48:47.418131 json_with_comments-1.2.0/jsonc/__init__.py
+-rw-r--r--   0        0        0     1088 2023-04-21 14:37:42.998515 json_with_comments-1.2.0/LICENSE
+-rw-r--r--   0        0        0      684 2023-06-20 19:46:34.318451 json_with_comments-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      983 2023-04-21 14:37:42.999515 json_with_comments-1.2.0/README.md
+-rw-r--r--   0        0        0     1824 1970-01-01 00:00:00.000000 json_with_comments-1.2.0/PKG-INFO
```

### Comparing `json-with-comments-1.1.1/LICENSE` & `json_with_comments-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `json-with-comments-1.1.1/pyproject.toml` & `json_with_comments-1.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "json-with-comments"
-version = "1.1.1"
+version = "1.2.0"
 description = "JSON with Comments for Python"
 license = "MIT"
 authors = ["Takumasa Nakamura <n.takumasa@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/n-takumasa/json-with-comments"
 classifiers = [
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 packages = [
     { include = "jsonc" },
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.7, <3.12"
+python = ">=3.7, <3.13"
 tomli = { version = "^2.0.1", python = "<3.11" }
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
-tox = "^3.27.0"
+tox = ">=3.27,<5.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `json-with-comments-1.1.1/README.md` & `json_with_comments-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `json-with-comments-1.1.1/PKG-INFO` & `json_with_comments-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: json-with-comments
-Version: 1.1.1
+Version: 1.2.0
 Summary: JSON with Comments for Python
 Home-page: https://github.com/n-takumasa/json-with-comments
 License: MIT
 Author: Takumasa Nakamura
 Author-email: n.takumasa@gmail.com
-Requires-Python: >=3.7,<3.12
+Requires-Python: >=3.7,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: tomli (>=2.0.1,<3.0.0); python_version < "3.11"
+Requires-Dist: tomli (>=2.0.1,<3.0.0) ; python_version < "3.11"
 Project-URL: Repository, https://github.com/n-takumasa/json-with-comments
 Description-Content-Type: text/markdown
 
 # JSON with Comments for Python
 [![pypi version](https://img.shields.io/pypi/v/json-with-comments.svg)](https://pypi.python.org/project/json-with-comments)
 [![Python package](https://github.com/n-takumasa/json-with-comments/actions/workflows/python-package.yml/badge.svg)](https://github.com/n-takumasa/json-with-comments/actions/workflows/python-package.yml)
 [![Python Versions](https://img.shields.io/pypi/pyversions/json-with-comments.svg)](https://pypi.org/project/json-with-comments/)
```

