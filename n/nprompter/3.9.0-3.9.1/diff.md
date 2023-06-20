# Comparing `tmp/nprompter-3.9.0.tar.gz` & `tmp/nprompter-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nprompter-3.9.0.tar", max compression
+gzip compressed data, was "nprompter-3.9.1.tar", max compression
```

## Comparing `nprompter-3.9.0.tar` & `nprompter-3.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0       56 2023-06-18 07:25:18.963411 nprompter-3.9.0/nprompter/__init__.py
--rw-r--r--   0        0        0     3736 2023-06-18 07:25:18.963411 nprompter-3.9.0/nprompter/__main__.py
--rw-r--r--   0        0        0        0 2023-06-18 07:25:18.963411 nprompter-3.9.0/nprompter/api/__init__.py
--rw-r--r--   0        0        0     2092 2023-06-18 07:25:18.963411 nprompter-3.9.0/nprompter/api/notion_client.py
--rw-r--r--   0        0        0        0 2023-06-18 07:25:18.963411 nprompter-3.9.0/nprompter/cli/__init__.py
--rw-r--r--   0        0        0      144 2023-06-18 07:25:18.963411 nprompter-3.9.0/nprompter/cli/defaults.py
--rw-r--r--   0        0        0      907 2023-06-18 07:25:18.963411 nprompter-3.9.0/nprompter/cli/helpers.py
--rw-r--r--   0        0        0        0 2023-06-18 07:25:18.963411 nprompter-3.9.0/nprompter/processing/__init__.py
--rw-r--r--   0        0        0     8053 2023-06-18 07:25:18.963411 nprompter-3.9.0/nprompter/processing/processor.py
--rw-r--r--   0        0        0        0 2023-06-18 07:25:18.963411 nprompter-3.9.0/nprompter/web/__init__.py
--rw-r--r--   0        0        0    31041 2023-06-18 07:25:18.963411 nprompter-3.9.0/nprompter/web/assets/android-chrome-192x192.png
--rw-r--r--   0        0        0   128229 2023-06-18 07:25:18.963411 nprompter-3.9.0/nprompter/web/assets/android-chrome-512x512.png
--rw-r--r--   0        0        0     7204 2023-06-18 07:25:18.963411 nprompter-3.9.0/nprompter/web/assets/app.js
--rw-r--r--   0        0        0    29064 2023-06-18 07:25:18.963411 nprompter-3.9.0/nprompter/web/assets/apple-touch-icon.png
--rw-r--r--   0        0        0      845 2023-06-18 07:25:18.963411 nprompter-3.9.0/nprompter/web/assets/favicon-16x16.png
--rw-r--r--   0        0        0     2274 2023-06-18 07:25:18.963411 nprompter-3.9.0/nprompter/web/assets/favicon-32x32.png
--rw-r--r--   0        0        0    15406 2023-06-18 07:25:18.963411 nprompter-3.9.0/nprompter/web/assets/favicon.ico
--rw-r--r--   0        0        0      263 2023-06-18 07:25:18.963411 nprompter-3.9.0/nprompter/web/assets/site.webmanifest
--rw-r--r--   0        0        0      512 2023-06-18 07:25:18.963411 nprompter-3.9.0/nprompter/web/nprompter.toml
--rw-r--r--   0        0        0     1265 2023-06-18 07:25:18.963411 nprompter-3.9.0/nprompter/web/templates/base.html
--rw-r--r--   0        0        0      365 2023-06-18 07:25:18.963411 nprompter-3.9.0/nprompter/web/templates/index.html
--rw-r--r--   0        0        0     4512 2023-06-18 07:25:18.963411 nprompter-3.9.0/nprompter/web/templates/nprompter.css
--rw-r--r--   0        0        0      172 2023-06-18 07:25:18.963411 nprompter-3.9.0/nprompter/web/templates/script.html
--rw-r--r--   0        0        0     1435 2023-06-18 07:25:18.963411 nprompter-3.9.0/nprompter/web/templates/settings.js
--rw-r--r--   0        0        0     1379 2023-06-18 07:25:18.967411 nprompter-3.9.0/pyproject.toml
--rw-r--r--   0        0        0     1008 2023-06-18 07:26:03.383093 nprompter-3.9.0/setup.py
--rw-r--r--   0        0        0      688 2023-06-18 07:26:03.383386 nprompter-3.9.0/PKG-INFO
+-rw-r--r--   0        0        0       56 2023-06-20 07:36:36.421952 nprompter-3.9.1/nprompter/__init__.py
+-rw-r--r--   0        0        0     3736 2023-06-20 07:36:36.421952 nprompter-3.9.1/nprompter/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-20 07:36:36.421952 nprompter-3.9.1/nprompter/api/__init__.py
+-rw-r--r--   0        0        0     2092 2023-06-20 07:36:36.421952 nprompter-3.9.1/nprompter/api/notion_client.py
+-rw-r--r--   0        0        0        0 2023-06-20 07:36:36.421952 nprompter-3.9.1/nprompter/cli/__init__.py
+-rw-r--r--   0        0        0      144 2023-06-20 07:36:36.421952 nprompter-3.9.1/nprompter/cli/defaults.py
+-rw-r--r--   0        0        0      907 2023-06-20 07:36:36.421952 nprompter-3.9.1/nprompter/cli/helpers.py
+-rw-r--r--   0        0        0        0 2023-06-20 07:36:36.421952 nprompter-3.9.1/nprompter/processing/__init__.py
+-rw-r--r--   0        0        0     8053 2023-06-20 07:36:36.421952 nprompter-3.9.1/nprompter/processing/processor.py
+-rw-r--r--   0        0        0        0 2023-06-20 07:36:36.421952 nprompter-3.9.1/nprompter/web/__init__.py
+-rw-r--r--   0        0        0    31041 2023-06-20 07:36:36.421952 nprompter-3.9.1/nprompter/web/assets/android-chrome-192x192.png
+-rw-r--r--   0        0        0   128229 2023-06-20 07:36:36.425952 nprompter-3.9.1/nprompter/web/assets/android-chrome-512x512.png
+-rw-r--r--   0        0        0     7204 2023-06-20 07:36:36.425952 nprompter-3.9.1/nprompter/web/assets/app.js
+-rw-r--r--   0        0        0    29064 2023-06-20 07:36:36.425952 nprompter-3.9.1/nprompter/web/assets/apple-touch-icon.png
+-rw-r--r--   0        0        0      845 2023-06-20 07:36:36.425952 nprompter-3.9.1/nprompter/web/assets/favicon-16x16.png
+-rw-r--r--   0        0        0     2274 2023-06-20 07:36:36.425952 nprompter-3.9.1/nprompter/web/assets/favicon-32x32.png
+-rw-r--r--   0        0        0    15406 2023-06-20 07:36:36.425952 nprompter-3.9.1/nprompter/web/assets/favicon.ico
+-rw-r--r--   0        0        0      263 2023-06-20 07:36:36.425952 nprompter-3.9.1/nprompter/web/assets/site.webmanifest
+-rw-r--r--   0        0        0      512 2023-06-20 07:36:36.425952 nprompter-3.9.1/nprompter/web/nprompter.toml
+-rw-r--r--   0        0        0     1265 2023-06-20 07:36:36.425952 nprompter-3.9.1/nprompter/web/templates/base.html
+-rw-r--r--   0        0        0      365 2023-06-20 07:36:36.425952 nprompter-3.9.1/nprompter/web/templates/index.html
+-rw-r--r--   0        0        0     4512 2023-06-20 07:36:36.425952 nprompter-3.9.1/nprompter/web/templates/nprompter.css
+-rw-r--r--   0        0        0      172 2023-06-20 07:36:36.425952 nprompter-3.9.1/nprompter/web/templates/script.html
+-rw-r--r--   0        0        0     1435 2023-06-20 07:36:36.425952 nprompter-3.9.1/nprompter/web/templates/settings.js
+-rw-r--r--   0        0        0     1364 2023-06-20 07:36:36.425952 nprompter-3.9.1/pyproject.toml
+-rw-r--r--   0        0        0     1016 1970-01-01 00:00:00.000000 nprompter-3.9.1/setup.py
+-rw-r--r--   0        0        0      739 1970-01-01 00:00:00.000000 nprompter-3.9.1/PKG-INFO
```

### Comparing `nprompter-3.9.0/nprompter/__main__.py` & `nprompter-3.9.1/nprompter/__main__.py`

 * *Files identical despite different names*

### Comparing `nprompter-3.9.0/nprompter/api/notion_client.py` & `nprompter-3.9.1/nprompter/api/notion_client.py`

 * *Files identical despite different names*

### Comparing `nprompter-3.9.0/nprompter/cli/helpers.py` & `nprompter-3.9.1/nprompter/cli/helpers.py`

 * *Files identical despite different names*

### Comparing `nprompter-3.9.0/nprompter/processing/processor.py` & `nprompter-3.9.1/nprompter/processing/processor.py`

 * *Files identical despite different names*

### Comparing `nprompter-3.9.0/nprompter/web/assets/android-chrome-192x192.png` & `nprompter-3.9.1/nprompter/web/assets/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `nprompter-3.9.0/nprompter/web/assets/android-chrome-512x512.png` & `nprompter-3.9.1/nprompter/web/assets/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `nprompter-3.9.0/nprompter/web/assets/app.js` & `nprompter-3.9.1/nprompter/web/assets/app.js`

 * *Files identical despite different names*

### Comparing `nprompter-3.9.0/nprompter/web/assets/apple-touch-icon.png` & `nprompter-3.9.1/nprompter/web/assets/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `nprompter-3.9.0/nprompter/web/assets/favicon-16x16.png` & `nprompter-3.9.1/nprompter/web/assets/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `nprompter-3.9.0/nprompter/web/assets/favicon-32x32.png` & `nprompter-3.9.1/nprompter/web/assets/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `nprompter-3.9.0/nprompter/web/assets/favicon.ico` & `nprompter-3.9.1/nprompter/web/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `nprompter-3.9.0/nprompter/web/nprompter.toml` & `nprompter-3.9.1/nprompter/web/nprompter.toml`

 * *Files identical despite different names*

### Comparing `nprompter-3.9.0/nprompter/web/templates/base.html` & `nprompter-3.9.1/nprompter/web/templates/base.html`

 * *Files identical despite different names*

### Comparing `nprompter-3.9.0/nprompter/web/templates/nprompter.css` & `nprompter-3.9.1/nprompter/web/templates/nprompter.css`

 * *Files identical despite different names*

### Comparing `nprompter-3.9.0/nprompter/web/templates/settings.js` & `nprompter-3.9.1/nprompter/web/templates/settings.js`

 * *Files identical despite different names*

### Comparing `nprompter-3.9.0/pyproject.toml` & `nprompter-3.9.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nprompter"
-version = "3.9.0"
+version = "3.9.1"
 description = "A web based teleprompter that uses Notion as a storage backend"
 authors = ["Antonio Feregrino <antonio.feregrino@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.scripts]
 nprompter = 'nprompter.__main__:app'
 
@@ -13,24 +13,23 @@
 Jinja2 = "^3.1.2"
 python = "^3.8"
 python-slugify = "^6.1.2"
 requests = "^2.28.0"
 tomli = "^2.0.1"
 typer = "^0.4.1"
 
-[tool.poetry.dev-dependencies]
-Sphinx = "^5.2.3"
+[tool.poetry.group.dev.dependencies]
 black = "^22.3.0"
 bump2version = "^1.0.1"
 commitizen = "^2.37.0"
 isort = "^5.10.1"
+mkdocs-material = "^9.1.16"
 myst-parser = "^0.18.1"
 pyproject-flake8 = "^0.0.1-alpha.4"
 pytest = "^7.1.3"
-sphinxext-opengraph = "^0.6.3"
 
 [tool.black]
 line-length = 120
 exclude = '''
 (
   /(
       \.eggs         # exclude a few common directories in the
```

### Comparing `nprompter-3.9.0/setup.py` & `nprompter-3.9.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,22 +19,22 @@
  'typer>=0.4.1,<0.5.0']
 
 entry_points = \
 {'console_scripts': ['nprompter = nprompter.__main__:app']}
 
 setup_kwargs = {
     'name': 'nprompter',
-    'version': '3.9.0',
+    'version': '3.9.1',
     'description': 'A web based teleprompter that uses Notion as a storage backend',
-    'long_description': None,
+    'long_description': 'None',
     'author': 'Antonio Feregrino',
     'author_email': 'antonio.feregrino@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.8,<4.0',
 }
```

### Comparing `nprompter-3.9.0/PKG-INFO` & `nprompter-3.9.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: nprompter
-Version: 3.9.0
+Version: 3.9.1
 Summary: A web based teleprompter that uses Notion as a storage backend
 License: MIT
 Author: Antonio Feregrino
 Author-email: antonio.feregrino@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: python-slugify (>=6.1.2,<7.0.0)
 Requires-Dist: requests (>=2.28.0,<3.0.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Requires-Dist: typer (>=0.4.1,<0.5.0)
```

