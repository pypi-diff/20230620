# Comparing `tmp/domini-0.8.0.tar.gz` & `tmp/domini-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domini-0.8.0.tar", max compression
+gzip compressed data, was "domini-0.8.1.tar", max compression
```

## Comparing `domini-0.8.0.tar` & `domini-0.8.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35066 2022-09-30 02:05:07.299772 domini-0.8.0/LICENSE
--rw-r--r--   0        0        0     2070 2023-06-08 23:04:06.895144 domini-0.8.0/README.md
--rw-r--r--   0        0        0        0 2023-04-15 00:46:21.435310 domini-0.8.0/domini/__init__.py
--rw-r--r--   0        0        0       19 2023-06-08 14:31:26.952321 domini-0.8.0/domini/html/__init__.py
--rw-r--r--   0        0        0     2139 2023-06-08 22:40:23.979848 domini-0.8.0/domini/html/events.py
--rw-r--r--   0        0        0    16293 2023-06-08 14:49:43.940214 domini-0.8.0/domini/html/tags.py
--rw-r--r--   0        0        0      418 2023-06-08 23:04:35.254714 domini-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     2699 1970-01-01 00:00:00.000000 domini-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    35066 2022-09-30 02:05:07.299772 domini-0.8.1/LICENSE
+-rw-r--r--   0        0        0     2070 2023-06-08 23:04:06.895144 domini-0.8.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-15 00:46:21.435310 domini-0.8.1/domini/__init__.py
+-rw-r--r--   0        0        0       19 2023-06-08 14:31:26.952321 domini-0.8.1/domini/html/__init__.py
+-rw-r--r--   0        0        0     2139 2023-06-08 22:40:23.979848 domini-0.8.1/domini/html/events.py
+-rw-r--r--   0        0        0    16294 2023-06-20 15:40:16.828970 domini-0.8.1/domini/html/tags.py
+-rw-r--r--   0        0        0      418 2023-06-20 15:41:24.028094 domini-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     2699 1970-01-01 00:00:00.000000 domini-0.8.1/PKG-INFO
```

### Comparing `domini-0.8.0/LICENSE` & `domini-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `domini-0.8.0/README.md` & `domini-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `domini-0.8.0/domini/html/events.py` & `domini-0.8.1/domini/html/events.py`

 * *Files identical despite different names*

### Comparing `domini-0.8.0/domini/html/tags.py` & `domini-0.8.1/domini/html/tags.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
         Return a copy with the children added.
         """
 
         # Create a copy of the element
         copy = type(self)(*self.attrs, **self.kwattrs)
         
         if self.children is not None:
-            copy.add(self.children)
+            copy.add(*self.children)
 
         # Add children
 
         # o) Strings and HTML tags are obviously singular
         if isinstance(content, (str, HTMLTag)):
             return copy.add(content)
```

### Comparing `domini-0.8.0/PKG-INFO` & `domini-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domini
-Version: 0.8.0
+Version: 0.8.1
 Summary: Create HTML documents using Pythonic syntax that mimics the real deal.
 Home-page: https://gitlab.com/deepadmax/domini
 License: GPL-3.0-or-later
 Author: Maximillian Strand
 Author-email: maxi@millian.se
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

