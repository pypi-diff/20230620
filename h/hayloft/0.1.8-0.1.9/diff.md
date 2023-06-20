# Comparing `tmp/hayloft-0.1.8.tar.gz` & `tmp/hayloft-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hayloft-0.1.8.tar", max compression
+gzip compressed data, was "hayloft-0.1.9.tar", max compression
```

## Comparing `hayloft-0.1.8.tar` & `hayloft-0.1.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1074 2023-06-13 15:27:24.809402 hayloft-0.1.8/LICENSE
--rw-r--r--   0        0        0      908 2023-06-18 15:56:02.291486 hayloft-0.1.8/README.md
--rw-r--r--   0        0        0        0 2023-06-13 15:23:56.017734 hayloft-0.1.8/hayloft/__init__.py
--rw-r--r--   0        0        0     3269 2023-06-18 15:54:20.457801 hayloft-0.1.8/hayloft/app.py
--rw-r--r--   0        0        0      669 2023-06-19 12:12:50.488202 hayloft-0.1.8/hayloft/logger.py
--rw-r--r--   0        0        0    18224 2023-06-18 15:55:10.311304 hayloft-0.1.8/hayloft/public/assets/index-7630e259.css
--rw-r--r--   0        0        0   175056 2023-06-18 15:55:10.311304 hayloft-0.1.8/hayloft/public/assets/index-be461c13.js
--rw-r--r--   0        0        0      384 2023-06-18 15:55:15.047987 hayloft-0.1.8/hayloft/public/index.html
--rw-r--r--   0        0        0     1367 2023-06-13 15:26:48.605765 hayloft-0.1.8/hayloft/schema.py
--rw-r--r--   0        0        0      430 2023-06-19 12:15:27.918544 hayloft-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1492 1970-01-01 00:00:00.000000 hayloft-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-13 15:27:24.809402 hayloft-0.1.9/LICENSE
+-rw-r--r--   0        0        0      908 2023-06-18 15:56:02.291486 hayloft-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2023-06-13 15:23:56.017734 hayloft-0.1.9/hayloft/__init__.py
+-rw-r--r--   0        0        0     3269 2023-06-18 15:54:20.457801 hayloft-0.1.9/hayloft/app.py
+-rw-r--r--   0        0        0      669 2023-06-19 12:12:50.488202 hayloft-0.1.9/hayloft/logger.py
+-rw-r--r--   0        0        0    18224 2023-06-18 15:55:10.311304 hayloft-0.1.9/hayloft/public/assets/index-7630e259.css
+-rw-r--r--   0        0        0   175056 2023-06-18 15:55:10.311304 hayloft-0.1.9/hayloft/public/assets/index-be461c13.js
+-rw-r--r--   0        0        0      384 2023-06-18 15:55:15.047987 hayloft-0.1.9/hayloft/public/index.html
+-rw-r--r--   0        0        0     1367 2023-06-13 15:26:48.605765 hayloft-0.1.9/hayloft/schema.py
+-rw-r--r--   0        0        0      550 2023-06-20 09:58:23.191032 hayloft-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1761 1970-01-01 00:00:00.000000 hayloft-0.1.9/PKG-INFO
```

### Comparing `hayloft-0.1.8/LICENSE` & `hayloft-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hayloft-0.1.8/README.md` & `hayloft-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `hayloft-0.1.8/hayloft/app.py` & `hayloft-0.1.9/hayloft/app.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.1.8/hayloft/logger.py` & `hayloft-0.1.9/hayloft/logger.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.1.8/hayloft/public/assets/index-7630e259.css` & `hayloft-0.1.9/hayloft/public/assets/index-7630e259.css`

 * *Files identical despite different names*

### Comparing `hayloft-0.1.8/hayloft/public/assets/index-be461c13.js` & `hayloft-0.1.9/hayloft/public/assets/index-be461c13.js`

 * *Files identical despite different names*

### Comparing `hayloft-0.1.8/hayloft/schema.py` & `hayloft-0.1.9/hayloft/schema.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.1.8/PKG-INFO` & `hayloft-0.1.9/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 Metadata-Version: 2.1
 Name: hayloft
-Version: 0.1.8
+Version: 0.1.9
 Summary: UI tool for LLM frameworks
+Home-page: https://github.com/eturchenkov/hayloft
 License: MIT
-Requires-Python: >=3.10,<4.0
+Keywords: llm framework,llm app tracking,ui for llm app
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: flask (>=2.3.2,<3.0.0)
 Requires-Dist: flask-cors (>=3.0.10,<4.0.0)
-Requires-Dist: flask-sqlalchemy (>=3.0.3,<4.0.0)
+Requires-Dist: flask-sqlalchemy (>=3.0.4,<4.0.0)
 Requires-Dist: nanoid (>=2.0.0,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
+Project-URL: Repository, https://github.com/eturchenkov/hayloft
 Description-Content-Type: text/markdown
 
 # Hayloft
 
 UI tool for LLM frameworks to make easy prompt/completion tracking, store and comparison of different sessions.
 
 Install package with pip
```

