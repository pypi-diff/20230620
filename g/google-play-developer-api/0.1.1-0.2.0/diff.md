# Comparing `tmp/google_play_developer_api-0.1.1.tar.gz` & `tmp/google_play_developer_api-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google_play_developer_api-0.1.1.tar", max compression
+gzip compressed data, was "google_play_developer_api-0.2.0.tar", max compression
```

## Comparing `google_play_developer_api-0.1.1.tar` & `google_play_developer_api-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1062 2023-06-19 10:18:41.965065 google_play_developer_api-0.1.1/LICENSE
--rw-r--r--   0        0        0      820 2023-06-19 10:18:41.965065 google_play_developer_api-0.1.1/README.md
--rw-r--r--   0        0        0       71 2023-06-19 10:18:41.965065 google_play_developer_api-0.1.1/google_play_developer_api/__init__.py
--rw-r--r--   0        0        0      381 2023-06-19 10:18:41.965065 google_play_developer_api-0.1.1/google_play_developer_api/example.py
--rw-r--r--   0        0        0     2588 2023-06-19 10:18:41.965065 google_play_developer_api-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       37 2023-06-19 10:18:41.965065 google_play_developer_api-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0      420 2023-06-19 10:18:41.965065 google_play_developer_api-0.1.1/tests/test_app.py
--rw-r--r--   0        0        0     2805 1970-01-01 00:00:00.000000 google_play_developer_api-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-20 03:03:49.762734 google_play_developer_api-0.2.0/LICENSE
+-rw-r--r--   0        0        0      829 2023-06-20 03:03:49.762734 google_play_developer_api-0.2.0/README.md
+-rw-r--r--   0        0        0       71 2023-06-20 03:03:49.762734 google_play_developer_api-0.2.0/google_play_developer_api/__init__.py
+-rw-r--r--   0        0        0      381 2023-06-20 03:03:49.762734 google_play_developer_api-0.2.0/google_play_developer_api/example.py
+-rw-r--r--   0        0        0     2597 2023-06-20 03:03:49.762734 google_play_developer_api-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       37 2023-06-20 03:03:49.762734 google_play_developer_api-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      420 2023-06-20 03:03:49.762734 google_play_developer_api-0.2.0/tests/test_app.py
+-rw-r--r--   0        0        0     2823 1970-01-01 00:00:00.000000 google_play_developer_api-0.2.0/PKG-INFO
```

### Comparing `google_play_developer_api-0.1.1/LICENSE` & `google_play_developer_api-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google_play_developer_api-0.1.1/README.md` & `google_play_developer_api-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # google-play-developer-api
 
 [![release](https://img.shields.io/pypi/v/google-play-developer-api.svg)](https://pypi.org/project/google-play-developer-api/)
 [![docs](https://img.shields.io/website/https/ikameglobal.github.io/google-play-developer-api/index.html.svg?label=docs&down_message=unavailable&up_message=available)](https://ikameglobal.github.io/google-play-developer-api)
 [![develop](https://github.com/ikameglobal/google-play-developer-api/actions/workflows/dev.yml/badge.svg)](https://github.com/ikameglobal/google-play-developer-api/actions/workflows/dev.yml)
 [![main](https://github.com/ikameglobal/google-play-developer-api/actions/workflows/release.yml/badge.svg)](https://github.com/ikameglobal/google-play-developer-api/actions/workflows/release.yml)
 
-Wrapper
+Wrapper for APIs
 
 ## Features
 
 * Something
 * Something else
```

### Comparing `google_play_developer_api-0.1.1/pyproject.toml` & `google_play_developer_api-0.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool]
 [tool.poetry]
 name = "google-play-developer-api"
-version = "0.1.1"
+version = "0.2.0"
 homepage = "https://github.com/ikameglobal/google-play-developer-api"
-description = "Wrapper"
+description = "Wrapper for APIs"
 authors = ["ikameglobal <minhpc@ikameglobal.com>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
     'Development Status :: 2 - Pre-Alpha',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: MIT License',
```

### Comparing `google_play_developer_api-0.1.1/PKG-INFO` & `google_play_developer_api-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: google-play-developer-api
-Version: 0.1.1
-Summary: Wrapper
+Version: 0.2.0
+Summary: Wrapper for APIs
 Home-page: https://github.com/ikameglobal/google-play-developer-api
 License: MIT
 Author: ikameglobal
 Author-email: minhpc@ikameglobal.com
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -44,14 +44,14 @@
 # google-play-developer-api
 
 [![release](https://img.shields.io/pypi/v/google-play-developer-api.svg)](https://pypi.org/project/google-play-developer-api/)
 [![docs](https://img.shields.io/website/https/ikameglobal.github.io/google-play-developer-api/index.html.svg?label=docs&down_message=unavailable&up_message=available)](https://ikameglobal.github.io/google-play-developer-api)
 [![develop](https://github.com/ikameglobal/google-play-developer-api/actions/workflows/dev.yml/badge.svg)](https://github.com/ikameglobal/google-play-developer-api/actions/workflows/dev.yml)
 [![main](https://github.com/ikameglobal/google-play-developer-api/actions/workflows/release.yml/badge.svg)](https://github.com/ikameglobal/google-play-developer-api/actions/workflows/release.yml)
 
-Wrapper
+Wrapper for APIs
 
 ## Features
 
 * Something
 * Something else
```

