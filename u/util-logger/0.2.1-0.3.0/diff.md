# Comparing `tmp/util_logger-0.2.1.tar.gz` & `tmp/util_logger-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "util_logger-0.2.1.tar", max compression
+gzip compressed data, was "util_logger-0.3.0.tar", max compression
```

## Comparing `util_logger-0.2.1.tar` & `util_logger-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1070 2023-06-20 19:21:32.093686 util_logger-0.2.1/LICENSE.txt
--rw-r--r--   0        0        0     1452 2023-06-20 19:21:32.094635 util_logger-0.2.1/README.md
--rw-r--r--   0        0        0      673 2023-06-20 19:21:48.089930 util_logger-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       22 2023-06-20 19:21:32.094719 util_logger-0.2.1/src/__init__.py
--rw-r--r--   0        0        0     2413 2023-06-20 19:21:32.095049 util_logger-0.2.1/src/logger.py
--rw-r--r--   0        0        0     1825 1970-01-01 00:00:00.000000 util_logger-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-20 19:21:32.093686 util_logger-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     1452 2023-06-20 19:21:32.094635 util_logger-0.3.0/README.md
+-rw-r--r--   0        0        0      695 2023-06-20 19:31:06.228721 util_logger-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       50 2023-06-20 19:31:06.231538 util_logger-0.3.0/src/util_logger/__init__.py
+-rw-r--r--   0        0        0     2413 2023-06-20 19:29:16.887365 util_logger-0.3.0/src/util_logger/logger.py
+-rw-r--r--   0        0        0     1825 1970-01-01 00:00:00.000000 util_logger-0.3.0/PKG-INFO
```

### Comparing `util_logger-0.2.1/LICENSE.txt` & `util_logger-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `util_logger-0.2.1/README.md` & `util_logger-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `util_logger-0.2.1/pyproject.toml` & `util_logger-0.3.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "util_logger"
-version = "0.2.1"
+version = "0.3.0"
 description = "Wrapper package to the logging std module"
 authors = ["tomtenuta <tom@tenuta.io>"]
 readme = "README.md"
-packages = [{ include = "src", from = "." }]
+packages = [{ include = "util_logger", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 
 [tool.poetry.group.dev.dependencies]
 termcolor = "^2.3.0"
 pytest = "^7.3.2"
@@ -20,8 +20,8 @@
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
-[tool.poetry_bumpversion.file."src/__init__.py"]
+[tool.poetry_bumpversion.file."src/util_logger/__init__.py"]
```

### Comparing `util_logger-0.2.1/src/logger.py` & `util_logger-0.3.0/src/util_logger/logger.py`

 * *Files identical despite different names*

### Comparing `util_logger-0.2.1/PKG-INFO` & `util_logger-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: util-logger
-Version: 0.2.1
+Version: 0.3.0
 Summary: Wrapper package to the logging std module
 Author: tomtenuta
 Author-email: tom@tenuta.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

