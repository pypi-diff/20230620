# Comparing `tmp/webexception-0.1.0.tar.gz` & `tmp/webexception-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webexception-0.1.0.tar", max compression
+gzip compressed data, was "webexception-1.0.0.tar", max compression
```

## Comparing `webexception-0.1.0.tar` & `webexception-1.0.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     6185 2023-06-20 15:11:48.458636 webexception-0.1.0/README.md
--rw-r--r--   0        0        0      566 2023-06-20 15:13:04.693830 webexception-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-20 15:13:03.845839 webexception-0.1.0/webexception/__init__.py
--rw-r--r--   0        0        0      109 2023-06-20 15:13:27.433588 webexception-0.1.0/webexception/webexception.py
--rw-r--r--   0        0        0     6478 1970-01-01 00:00:00.000000 webexception-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     6185 2023-06-20 15:11:48.458636 webexception-1.0.0/README.md
+-rw-r--r--   0        0        0      566 2023-06-20 16:01:43.389139 webexception-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-20 15:13:03.845839 webexception-1.0.0/webexception/__init__.py
+-rw-r--r--   0        0        0      664 2023-06-20 16:00:55.717895 webexception-1.0.0/webexception/webexception.py
+-rw-r--r--   0        0        0     6478 1970-01-01 00:00:00.000000 webexception-1.0.0/PKG-INFO
```

### Comparing `webexception-0.1.0/README.md` & `webexception-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `webexception-0.1.0/pyproject.toml` & `webexception-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "webexception"
-version = "0.1.0"
+version = "1.0.0"
 description = ""
 authors = ["Marco Bartel <bsimpson888@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `webexception-0.1.0/PKG-INFO` & `webexception-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webexception
-Version: 0.1.0
+Version: 1.0.0
 Summary: 
 Author: Marco Bartel
 Author-email: bsimpson888@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

