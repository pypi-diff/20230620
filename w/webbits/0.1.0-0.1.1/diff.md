# Comparing `tmp/webbits-0.1.0.tar.gz` & `tmp/webbits-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webbits-0.1.0.tar", max compression
+gzip compressed data, was "webbits-0.1.1.tar", max compression
```

## Comparing `webbits-0.1.0.tar` & `webbits-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0      583 2023-04-10 12:10:20.977228 webbits-0.1.0/LICENSE
--rw-r--r--   0        0        0     1058 2023-04-10 13:33:19.027798 webbits-0.1.0/README.md
--rw-r--r--   0        0        0     3153 2023-05-30 11:06:45.873825 webbits-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      128 2023-04-10 12:10:21.004779 webbits-0.1.0/src/webbits/__init__.py
--rw-r--r--   0        0        0       71 2023-03-15 21:35:37.681297 webbits-0.1.0/src/webbits/html/__init__.py
--rw-r--r--   0        0        0     4825 2023-03-15 17:28:40.505466 webbits-0.1.0/src/webbits/html/_constants.py
--rw-r--r--   0        0        0     4299 2023-04-13 15:12:15.426207 webbits-0.1.0/src/webbits/html/_elements.py
--rw-r--r--   0        0        0      856 2023-04-14 16:44:37.288016 webbits-0.1.0/src/webbits/html/_h.py
--rw-r--r--   0        0        0      202 2023-04-14 17:11:32.128852 webbits-0.1.0/src/webbits/lib.py
--rw-r--r--   0        0        0       37 2023-04-10 12:10:20.994654 webbits-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      804 2023-04-14 16:44:18.864188 webbits-0.1.0/tests/test_h.py
--rw-r--r--   0        0        0     2562 2023-04-14 16:44:53.605035 webbits-0.1.0/tests/test_html.py
--rw-r--r--   0        0        0     1786 1970-01-01 00:00:00.000000 webbits-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      583 2023-04-10 12:10:20.977228 webbits-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3612 2023-05-30 13:23:23.815412 webbits-0.1.1/README.md
+-rw-r--r--   0        0        0     3153 2023-06-20 09:13:31.331231 webbits-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      128 2023-04-10 12:10:21.004779 webbits-0.1.1/src/webbits/__init__.py
+-rw-r--r--   0        0        0       71 2023-03-15 21:35:37.681297 webbits-0.1.1/src/webbits/html/__init__.py
+-rw-r--r--   0        0        0     4825 2023-03-15 17:28:40.505466 webbits-0.1.1/src/webbits/html/_constants.py
+-rw-r--r--   0        0        0     4299 2023-04-13 15:12:15.426207 webbits-0.1.1/src/webbits/html/_elements.py
+-rw-r--r--   0        0        0      856 2023-04-14 16:44:37.288016 webbits-0.1.1/src/webbits/html/_h.py
+-rw-r--r--   0        0        0      202 2023-04-14 17:11:32.128852 webbits-0.1.1/src/webbits/lib.py
+-rw-r--r--   0        0        0       37 2023-04-10 12:10:20.994654 webbits-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0      804 2023-04-14 16:44:18.864188 webbits-0.1.1/tests/test_h.py
+-rw-r--r--   0        0        0     2562 2023-04-14 16:44:53.605035 webbits-0.1.1/tests/test_html.py
+-rw-r--r--   0        0        0      952 2023-06-07 12:34:30.010747 webbits-0.1.1/tests/text_new_dsl.py
+-rw-r--r--   0        0        0     4340 1970-01-01 00:00:00.000000 webbits-0.1.1/PKG-INFO
```

### Comparing `webbits-0.1.0/LICENSE` & `webbits-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `webbits-0.1.0/pyproject.toml` & `webbits-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "webbits"
-version = "0.1.0"
+version = "0.1.1"
 homepage = "https://github.com/sfermigier/webbits"
 description = "Top-level package for Webbits."
 authors = ["Abilian SAS <sf@abilian.com>"]
 readme = "README.md"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
     'Intended Audience :: Developers',
```

### Comparing `webbits-0.1.0/src/webbits/html/_constants.py` & `webbits-0.1.1/src/webbits/html/_constants.py`

 * *Files identical despite different names*

### Comparing `webbits-0.1.0/src/webbits/html/_elements.py` & `webbits-0.1.1/src/webbits/html/_elements.py`

 * *Files identical despite different names*

### Comparing `webbits-0.1.0/src/webbits/html/_h.py` & `webbits-0.1.1/src/webbits/html/_h.py`

 * *Files identical despite different names*

### Comparing `webbits-0.1.0/tests/test_h.py` & `webbits-0.1.1/tests/test_h.py`

 * *Files identical despite different names*

### Comparing `webbits-0.1.0/tests/test_html.py` & `webbits-0.1.1/tests/test_html.py`

 * *Files identical despite different names*

