# Comparing `tmp/arranges-0.0.3.tar.gz` & `tmp/arranges-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arranges-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "arranges-0.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `arranges-0.0.3.tar` & `arranges-0.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2723 2023-06-20 07:09:26.402300 arranges-0.0.3/README.md
--rw-r--r--   0        0        0      914 2023-06-20 07:11:17.027430 arranges-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      123 2023-06-20 07:09:26.402300 arranges-0.0.3/src/arranges/__init__.py
--rw-r--r--   0        0        0    12506 2023-06-20 07:09:26.402300 arranges-0.0.3/src/arranges/range.py
--rw-r--r--   0        0        0     3941 2023-06-20 07:09:26.402300 arranges-0.0.3/src/arranges/ranges.py
--rw-r--r--   0        0        0     2304 2023-06-20 07:09:26.402300 arranges-0.0.3/src/arranges/utils.py
--rw-r--r--   0        0        0     3764 1970-01-01 00:00:00.000000 arranges-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     2724 2023-06-20 07:31:33.656084 arranges-0.0.4/README.md
+-rw-r--r--   0        0        0      914 2023-06-20 07:31:33.656084 arranges-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      123 2023-06-20 07:31:33.656084 arranges-0.0.4/src/arranges/__init__.py
+-rw-r--r--   0        0        0    12506 2023-06-20 07:31:33.656084 arranges-0.0.4/src/arranges/range.py
+-rw-r--r--   0        0        0     3941 2023-06-20 07:31:33.656084 arranges-0.0.4/src/arranges/ranges.py
+-rw-r--r--   0        0        0     2304 2023-06-20 07:31:33.656084 arranges-0.0.4/src/arranges/utils.py
+-rw-r--r--   0        0        0     3765 1970-01-01 00:00:00.000000 arranges-0.0.4/PKG-INFO
```

### Comparing `arranges-0.0.3/README.md` & `arranges-0.0.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 Type `make help` to see the other options, or run the one-liner scripts in the
 `./build` dir if you want to run steps without all that fancy caching nonsense.
 
 ## Usage
 
 * [RTFM](https://bitplane.github.io/arranges/)
 * Read [the tests](../arranges/tests/), which have full coverage.
-* [Read the API docs](../docs/api.md)
+* [Read the pydocs](../docs/pydocs.md)
 
 ## License
 
 Free as in freedom from legalese; the [WTFPL with a warranty clause](../LICENSE).
 
 Political note: I don't want to live in a world where lawyers tell me how to
 speak. If you don't trust me enough to use the WTFPL then you shouldn't be
```

### Comparing `arranges-0.0.3/pyproject.toml` & `arranges-0.0.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "arranges"
 description = "Mergable range object for use in Pydantic classes"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
     { name = "Gareth Davidson", email = "gaz@bitplane.net" }
 ]
 
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `arranges-0.0.3/src/arranges/range.py` & `arranges-0.0.4/src/arranges/range.py`

 * *Files identical despite different names*

### Comparing `arranges-0.0.3/src/arranges/ranges.py` & `arranges-0.0.4/src/arranges/ranges.py`

 * *Files identical despite different names*

### Comparing `arranges-0.0.3/src/arranges/utils.py` & `arranges-0.0.4/src/arranges/utils.py`

 * *Files identical despite different names*

### Comparing `arranges-0.0.3/PKG-INFO` & `arranges-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arranges
-Version: 0.0.3
+Version: 0.0.4
 Summary: Mergable range object for use in Pydantic classes
 Author-email: Gareth Davidson <gaz@bitplane.net>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Public Domain
 Classifier: Operating System :: OS Independent
@@ -80,15 +80,15 @@
 Type `make help` to see the other options, or run the one-liner scripts in the
 `./build` dir if you want to run steps without all that fancy caching nonsense.
 
 ## Usage
 
 * [RTFM](https://bitplane.github.io/arranges/)
 * Read [the tests](../arranges/tests/), which have full coverage.
-* [Read the API docs](../docs/api.md)
+* [Read the pydocs](../docs/pydocs.md)
 
 ## License
 
 Free as in freedom from legalese; the [WTFPL with a warranty clause](../LICENSE).
 
 Political note: I don't want to live in a world where lawyers tell me how to
 speak. If you don't trust me enough to use the WTFPL then you shouldn't be
```

