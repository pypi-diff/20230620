# Comparing `tmp/social_media_card-1.0.0.tar.gz` & `tmp/social_media_card-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "social_media_card-1.0.0.tar", max compression
+gzip compressed data, was "social_media_card-2.0.0.tar", max compression
```

## Comparing `social_media_card-1.0.0.tar` & `social_media_card-2.0.0.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     3628 2023-06-20 18:29:23.841486 social_media_card-1.0.0/README.md
--rw-r--r--   0        0        0     1254 2023-06-20 18:29:23.841486 social_media_card-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3008 2023-06-20 18:29:23.841486 social_media_card-1.0.0/social_media_card/__init__.py
--rw-r--r--   0        0        0     1419 2023-06-20 18:29:23.841486 social_media_card-1.0.0/social_media_card/html_template.py
--rw-r--r--   0        0        0     4751 2023-06-20 18:29:23.841486 social_media_card-1.0.0/social_media_card/image_manip.py
--rw-r--r--   0        0        0     2751 2023-06-20 18:29:23.841486 social_media_card-1.0.0/social_media_card/paths.py
--rw-r--r--   0        0        0     4169 1970-01-01 00:00:00.000000 social_media_card-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3628 2023-06-20 19:07:10.261465 social_media_card-2.0.0/README.md
+-rw-r--r--   0        0        0     1254 2023-06-20 19:07:10.265465 social_media_card-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3008 2023-06-20 19:07:10.265465 social_media_card-2.0.0/social_media_card/__init__.py
+-rw-r--r--   0        0        0     1419 2023-06-20 19:07:10.265465 social_media_card-2.0.0/social_media_card/html_template.py
+-rw-r--r--   0        0        0     4751 2023-06-20 19:07:10.265465 social_media_card-2.0.0/social_media_card/image_manip.py
+-rw-r--r--   0        0        0     2751 2023-06-20 19:07:10.265465 social_media_card-2.0.0/social_media_card/paths.py
+-rw-r--r--   0        0        0        0 2023-06-20 19:07:10.265465 social_media_card-2.0.0/social_media_card/py.typed
+-rw-r--r--   0        0        0     4169 1970-01-01 00:00:00.000000 social_media_card-2.0.0/PKG-INFO
```

### Comparing `social_media_card-1.0.0/README.md` & `social_media_card-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `social_media_card-1.0.0/pyproject.toml` & `social_media_card-2.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "social-media-card"
-version = "1.0.0"
+version = "2.0.0"
 description = "Create clickable images for social media"
 authors = ["Shay Hill <shay_public@hotmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "social_media_card"}]
 
 [tool.poetry.dependencies]
@@ -18,15 +18,15 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.0.0"
+version = "2.0.0"
 tag_format = "$version"
 version_files = [
     "pyproject.toml:^version"
 ]
 
 [tool.pyright]
 include = ["src"]
```

### Comparing `social_media_card-1.0.0/social_media_card/__init__.py` & `social_media_card-2.0.0/social_media_card/__init__.py`

 * *Files identical despite different names*

### Comparing `social_media_card-1.0.0/social_media_card/html_template.py` & `social_media_card-2.0.0/social_media_card/html_template.py`

 * *Files identical despite different names*

### Comparing `social_media_card-1.0.0/social_media_card/image_manip.py` & `social_media_card-2.0.0/social_media_card/image_manip.py`

 * *Files identical despite different names*

### Comparing `social_media_card-1.0.0/social_media_card/paths.py` & `social_media_card-2.0.0/social_media_card/paths.py`

 * *Files identical despite different names*

### Comparing `social_media_card-1.0.0/PKG-INFO` & `social_media_card-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: social-media-card
-Version: 1.0.0
+Version: 2.0.0
 Summary: Create clickable images for social media
 License: MIT
 Author: Shay Hill
 Author-email: shay_public@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: social-media-card Version: 1.0.0 Summary: Create
+Metadata-Version: 2.1 Name: social-media-card Version: 2.0.0 Summary: Create
 clickable images for social media License: MIT Author: Shay Hill Author-email:
 shay_public@hotmail.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Pillow (>=9.5.0,<10.0.0) Description-Content-Type: text/markdown
 # create social media cards for LinkedIn, Facebook, and (untested) Twitter This
```

