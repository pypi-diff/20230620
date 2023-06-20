# Comparing `tmp/arranges-0.0.4.tar.gz` & `tmp/arranges-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arranges-0.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "arranges-0.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `arranges-0.0.4.tar` & `arranges-0.0.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2724 2023-06-20 07:31:33.656084 arranges-0.0.4/README.md
--rw-r--r--   0        0        0      914 2023-06-20 07:31:33.656084 arranges-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      123 2023-06-20 07:31:33.656084 arranges-0.0.4/src/arranges/__init__.py
--rw-r--r--   0        0        0    12506 2023-06-20 07:31:33.656084 arranges-0.0.4/src/arranges/range.py
--rw-r--r--   0        0        0     3941 2023-06-20 07:31:33.656084 arranges-0.0.4/src/arranges/ranges.py
--rw-r--r--   0        0        0     2304 2023-06-20 07:31:33.656084 arranges-0.0.4/src/arranges/utils.py
--rw-r--r--   0        0        0     3765 1970-01-01 00:00:00.000000 arranges-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     2724 2023-06-20 07:39:41.694887 arranges-0.0.5/README.md
+-rw-r--r--   0        0        0      914 2023-06-20 07:39:41.694887 arranges-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      123 2023-06-20 07:39:41.698887 arranges-0.0.5/src/arranges/__init__.py
+-rw-r--r--   0        0        0    12506 2023-06-20 07:39:41.698887 arranges-0.0.5/src/arranges/range.py
+-rw-r--r--   0        0        0     3941 2023-06-20 07:39:41.698887 arranges-0.0.5/src/arranges/ranges.py
+-rw-r--r--   0        0        0     2304 2023-06-20 07:39:41.698887 arranges-0.0.5/src/arranges/utils.py
+-rw-r--r--   0        0        0     3765 1970-01-01 00:00:00.000000 arranges-0.0.5/PKG-INFO
```

### Comparing `arranges-0.0.4/README.md` & `arranges-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `arranges-0.0.4/pyproject.toml` & `arranges-0.0.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "arranges"
 description = "Mergable range object for use in Pydantic classes"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
     { name = "Gareth Davidson", email = "gaz@bitplane.net" }
 ]
 
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `arranges-0.0.4/src/arranges/range.py` & `arranges-0.0.5/src/arranges/range.py`

 * *Files identical despite different names*

### Comparing `arranges-0.0.4/src/arranges/ranges.py` & `arranges-0.0.5/src/arranges/ranges.py`

 * *Files identical despite different names*

### Comparing `arranges-0.0.4/src/arranges/utils.py` & `arranges-0.0.5/src/arranges/utils.py`

 * *Files identical despite different names*

### Comparing `arranges-0.0.4/PKG-INFO` & `arranges-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arranges
-Version: 0.0.4
+Version: 0.0.5
 Summary: Mergable range object for use in Pydantic classes
 Author-email: Gareth Davidson <gaz@bitplane.net>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Public Domain
 Classifier: Operating System :: OS Independent
```

