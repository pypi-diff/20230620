# Comparing `tmp/pytest-richtrace-0.1.0.tar.gz` & `tmp/pytest_richtrace-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-richtrace-0.1.0.tar", max compression
+gzip compressed data, was "pytest_richtrace-0.2.0.tar", max compression
```

## Comparing `pytest-richtrace-0.1.0.tar` & `pytest_richtrace-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,14 @@
--rw-r--r--   0        0        0      427 2022-11-05 16:27:28.401007 pytest-richtrace-0.1.0/ReadMe.md
--rw-r--r--   0        0        0      547 2022-11-04 13:48:41.438947 pytest-richtrace-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    13630 2022-11-05 16:27:28.403007 pytest-richtrace-0.1.0/src/pytest_richtrace/__init__.py
--rw-r--r--   0        0        0     1252 1970-01-01 00:00:00.000000 pytest-richtrace-0.1.0/setup.py
--rw-r--r--   0        0        0      855 1970-01-01 00:00:00.000000 pytest-richtrace-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1352 2023-06-02 10:50:35.098255 pytest_richtrace-0.2.0/ReadMe.md
+-rw-r--r--   0        0        0      892 2023-06-20 19:08:36.679744 pytest_richtrace-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1431 2023-06-02 10:50:35.114255 pytest_richtrace-0.2.0/src/pytest_richtrace/__init__.py
+-rw-r--r--   0        0        0     7081 2023-06-02 10:50:35.115255 pytest_richtrace-0.2.0/src/pytest_richtrace/collection_observer.py
+-rw-r--r--   0        0        0     2972 2023-06-02 10:50:35.123255 pytest_richtrace-0.2.0/src/pytest_richtrace/console.py
+-rw-r--r--   0        0        0     3671 2023-06-02 10:50:35.123255 pytest_richtrace-0.2.0/src/pytest_richtrace/event.py
+-rw-r--r--   0        0        0     1637 2023-06-02 10:50:35.123255 pytest_richtrace-0.2.0/src/pytest_richtrace/events.py
+-rw-r--r--   0        0        0       55 2023-06-02 10:50:35.123255 pytest_richtrace-0.2.0/src/pytest_richtrace/item.py
+-rw-r--r--   0        0        0     7713 2023-06-02 10:50:35.115255 pytest_richtrace-0.2.0/src/pytest_richtrace/plugin.py
+-rw-r--r--   0        0        0        0 2023-06-02 10:50:35.123255 pytest_richtrace-0.2.0/src/pytest_richtrace/py.typed
+-rw-r--r--   0        0        0     4998 2023-06-02 10:50:35.123255 pytest_richtrace-0.2.0/src/pytest_richtrace/results.py
+-rw-r--r--   0        0        0    27850 2023-06-02 10:50:35.124255 pytest_richtrace-0.2.0/src/pytest_richtrace/rich_reporter.py
+-rw-r--r--   0        0        0     6604 2023-06-02 10:50:35.123255 pytest_richtrace-0.2.0/src/pytest_richtrace/test_execution_observer.py
+-rw-r--r--   0        0        0     1915 1970-01-01 00:00:00.000000 pytest_richtrace-0.2.0/PKG-INFO
```

### Comparing `pytest-richtrace-0.1.0/pyproject.toml` & `pytest_richtrace-0.2.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,33 @@
 [tool.poetry]
 name = "pytest-richtrace"
-version = "0.1.0"
-description = ""
+version = "0.2.0"
+description = "A pytest plugin that displays the names and information of the pytest hook functions as they are executed."
 authors = ["Simon Kennedy <sffjunkie+code@gmail.com>"]
+license = "Apache-2.0"
 readme = "ReadMe.md"
-packages = [{ include = "pytest_richtrace", from = "src" }]
+packages = [
+    { include = "pytest_richtrace", from = "src" },
+    { include = "pytest_richtrace/py.typed", from = "src" },
+]
 
-[tool.poetry.dependencies]
-python = "^3.9"
-rich = "^12.6.0"
-pytest = "^7.2.0"
+[tool.poetry.plugins]
+pytest11 = { pytest_richtrace = "pytest_richtrace" }
 
+[tool.poetry.dependencies]
+python = "^3.11"
+rich = "^13.3.5"
+pydantic = { version = ">=2.0a1", allow-prereleases = true }
 
 [tool.poetry.group.dev.dependencies]
-black = { version = "^22.10.0", allow-prereleases = true }
+mkdocs = "^1.4.3"
+mypy = "^1.3.0"
+pytest = "^7.3.1"
+mkdocs-material = "^9.1.13"
+pre-commit = "^3.3.2"
 
-[tool.poetry.plugins."pytest11"]
-"pytest-richtrace" = "pytest_richtrace"
+[tool.pytest.ini_options]
+testpaths = ["tests/rich_trace"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

