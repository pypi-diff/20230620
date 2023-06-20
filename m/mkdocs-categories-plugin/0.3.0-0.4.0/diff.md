# Comparing `tmp/mkdocs-categories-plugin-0.3.0.tar.gz` & `tmp/mkdocs-categories-plugin-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-categories-plugin-0.3.0.tar", last modified: Fri Apr 14 03:56:25 2023, max compression
+gzip compressed data, was "mkdocs-categories-plugin-0.4.0.tar", last modified: Tue Jun 20 05:01:05 2023, max compression
```

## Comparing `mkdocs-categories-plugin-0.3.0.tar` & `mkdocs-categories-plugin-0.4.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:56:25.674928 mkdocs-categories-plugin-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-14 03:56:15.000000 mkdocs-categories-plugin-0.3.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-04-14 03:56:25.674928 mkdocs-categories-plugin-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-04-14 03:56:15.000000 mkdocs-categories-plugin-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:56:25.670928 mkdocs-categories-plugin-0.3.0/categories/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:56:15.000000 mkdocs-categories-plugin-0.3.0/categories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10425 2023-04-14 03:56:15.000000 mkdocs-categories-plugin-0.3.0/categories/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:56:25.674928 mkdocs-categories-plugin-0.3.0/mkdocs_categories_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-04-14 03:56:25.000000 mkdocs-categories-plugin-0.3.0/mkdocs_categories_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-14 03:56:25.000000 mkdocs-categories-plugin-0.3.0/mkdocs_categories_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 03:56:25.000000 mkdocs-categories-plugin-0.3.0/mkdocs_categories_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-14 03:56:25.000000 mkdocs-categories-plugin-0.3.0/mkdocs_categories_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 03:56:25.000000 mkdocs-categories-plugin-0.3.0/mkdocs_categories_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-14 03:56:25.000000 mkdocs-categories-plugin-0.3.0/mkdocs_categories_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 03:56:25.674928 mkdocs-categories-plugin-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-14 03:56:15.000000 mkdocs-categories-plugin-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:01:05.699943 mkdocs-categories-plugin-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-20 05:00:54.000000 mkdocs-categories-plugin-0.4.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6590 2023-06-20 05:01:05.699943 mkdocs-categories-plugin-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-06-20 05:00:54.000000 mkdocs-categories-plugin-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:01:05.699943 mkdocs-categories-plugin-0.4.0/categories/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:00:54.000000 mkdocs-categories-plugin-0.4.0/categories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10467 2023-06-20 05:00:54.000000 mkdocs-categories-plugin-0.4.0/categories/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:01:05.699943 mkdocs-categories-plugin-0.4.0/mkdocs_categories_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6590 2023-06-20 05:01:05.000000 mkdocs-categories-plugin-0.4.0/mkdocs_categories_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-20 05:01:05.000000 mkdocs-categories-plugin-0.4.0/mkdocs_categories_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 05:01:05.000000 mkdocs-categories-plugin-0.4.0/mkdocs_categories_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-20 05:01:05.000000 mkdocs-categories-plugin-0.4.0/mkdocs_categories_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-20 05:01:05.000000 mkdocs-categories-plugin-0.4.0/mkdocs_categories_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-20 05:01:05.000000 mkdocs-categories-plugin-0.4.0/mkdocs_categories_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 05:01:05.699943 mkdocs-categories-plugin-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-20 05:00:54.000000 mkdocs-categories-plugin-0.4.0/setup.py
```

### Comparing `mkdocs-categories-plugin-0.3.0/LICENSE.md` & `mkdocs-categories-plugin-0.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mkdocs-categories-plugin-0.3.0/PKG-INFO` & `mkdocs-categories-plugin-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: mkdocs-categories-plugin
-Version: 0.3.0
-Summary: An MkDocs plugin allowing for categorization of pages
-Home-page: https://github.com/eddyluten/mkdocs-categories-plugin
-Author: Eddy Luten
-Author-email: eddyluten@gmail.com
-License: MIT
-Keywords: mkdocs python markdown category categories link wiki
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 # mkdocs-categories-plugin
 
 [![PyPI version](https://badge.fury.io/py/mkdocs-categories-plugin.svg)](https://pypi.org/project/mkdocs-categories-plugin/)  [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) ![example workflow](https://github.com/eddyluten/mkdocs-categories-plugin/actions/workflows/pylint.yml/badge.svg) [![Downloads](https://pepy.tech/badge/mkdocs-categories-plugin)](https://pepy.tech/project/mkdocs-categories-plugin)
 
 An MkDocs plugin allowing for categorization of pages in your wiki. This plugin allows for multiple categories per page and will generate a category index page with links to each page within the category.
 
 If you like this MkDocs plugin, you'll probably also like [mkdocs-alias-plugin](https://github.com/EddyLuten/mkdocs-alias-plugin).
@@ -136,14 +119,18 @@
 
 ### `The categories object at URL was not a list, but TYPE`
 
 The page identified did not contain a valid categories configuration object. Please make sure that this is an array of strings.
 
 ## Changelog
 
+### 0.4.0
+
+Fixes sorting categories, child pages, etc. containing numbers by using natural sorting from the `natsort` package rather than the default sorting function.
+
 ### 0.3.0
 
 Added support for subcategories. Python 3.10 or higher is now required.
 
 ### 0.2.1
 
 Patch release: implements a bug fix by @rpmzandwijk reported in [#1](https://github.com/EddyLuten/mkdocs-categories-plugin/issues/1).
```

### Comparing `mkdocs-categories-plugin-0.3.0/README.md` & `mkdocs-categories-plugin-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: mkdocs-categories-plugin
+Version: 0.4.0
+Summary: An MkDocs plugin allowing for categorization of pages
+Home-page: https://github.com/eddyluten/mkdocs-categories-plugin
+Author: Eddy Luten
+Author-email: eddyluten@gmail.com
+License: MIT
+Keywords: mkdocs python markdown category categories link wiki
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
 # mkdocs-categories-plugin
 
 [![PyPI version](https://badge.fury.io/py/mkdocs-categories-plugin.svg)](https://pypi.org/project/mkdocs-categories-plugin/)  [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) ![example workflow](https://github.com/eddyluten/mkdocs-categories-plugin/actions/workflows/pylint.yml/badge.svg) [![Downloads](https://pepy.tech/badge/mkdocs-categories-plugin)](https://pepy.tech/project/mkdocs-categories-plugin)
 
 An MkDocs plugin allowing for categorization of pages in your wiki. This plugin allows for multiple categories per page and will generate a category index page with links to each page within the category.
 
 If you like this MkDocs plugin, you'll probably also like [mkdocs-alias-plugin](https://github.com/EddyLuten/mkdocs-alias-plugin).
@@ -119,14 +136,18 @@
 
 ### `The categories object at URL was not a list, but TYPE`
 
 The page identified did not contain a valid categories configuration object. Please make sure that this is an array of strings.
 
 ## Changelog
 
+### 0.4.0
+
+Fixes sorting categories, child pages, etc. containing numbers by using natural sorting from the `natsort` package rather than the default sorting function.
+
 ### 0.3.0
 
 Added support for subcategories. Python 3.10 or higher is now required.
 
 ### 0.2.1
 
 Patch release: implements a bug fix by @rpmzandwijk reported in [#1](https://github.com/EddyLuten/mkdocs-categories-plugin/issues/1).
```

### Comparing `mkdocs-categories-plugin-0.3.0/categories/plugin.py` & `mkdocs-categories-plugin-0.4.0/categories/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import logging
 import re
 import shutil
 import unicodedata
 from logging import Logger, getLogger
 from pathlib import Path
 
+from natsort import natsorted
 from mkdocs.config import config_options
 from mkdocs.plugins import BasePlugin
 from mkdocs.structure.files import File
 from mkdocs.structure.pages import Page
 from mkdocs.utils import get_markdown_title, get_relative_url, meta
 
 
@@ -97,15 +98,15 @@
         if page.file.url not in self.pages:
             return markdown
         links = list(map(
             lambda c: (
                 f"- [{self.categories[c]['name']}]"
                 f"({relative_url}/{self.categories[c]['slug']}/)"
             ),
-            sorted(self.pages[page.file.url])
+            natsorted(self.pages[page.file.url])
         ))
         return (
             markdown +
             f"\n## {self.config['section_title']}\n\n" +
             "\n".join(links)
         )
 
@@ -171,15 +172,15 @@
                         get_page_title(source, meta_data)
                     )
 
     def generate_index(self, config) -> File:
         """Generates a categories index page if the option is set."""
         joined = "\n".join(map(
             lambda c: f"- [{c['name']}]({str(c['slug'])}/) ({len(c['pages'])})",
-            sorted(self.categories.values(), key=lambda c: c['name'])
+            natsorted(self.categories.values(), key=lambda c: c['name'])
         ))
         with open(self.cat_path / 'index.md', mode="w", encoding='utf-8') as file:
             file.write(
                 "# All Categories\n\n"
                 "\n"
                 f"There are a total of {len(self.categories.keys())} categories(s):\n"
                 "\n"
@@ -201,25 +202,25 @@
 
     def render_child_categories(self, category: dict) -> tuple[bool, str]:
         """Renders the child categories of a category."""
         if len(category['children']) <= 0:
             return False, None
         joined = "\n".join(map(
             lambda c: f"- [{self.categories[c]['name']}](../{self.categories[c]['slug']}/)",
-            sorted(category['children'])
+            natsorted(category['children'])
         ))
         return True, joined
 
     def render_category_pages(self, category: dict) -> tuple[bool, str]:
         """Renders the pages of a category."""
         if len(category['pages']) <= 0:
             return False, None
         joined = "\n".join(map(
             lambda p: f"- [{p['title']}](../../{p['url']})",
-            sorted(category['pages'], key=lambda p: p['title'])
+            natsorted(category['pages'], key=lambda p: p['title'])
         ))
         return True, joined
 
     def render_parent_category(self, category: dict) -> str:
         """Renders the parent category of a category."""
         if not category['parent']:
             return None
```

### Comparing `mkdocs-categories-plugin-0.3.0/mkdocs_categories_plugin.egg-info/PKG-INFO` & `mkdocs-categories-plugin-0.4.0/mkdocs_categories_plugin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-categories-plugin
-Version: 0.3.0
+Version: 0.4.0
 Summary: An MkDocs plugin allowing for categorization of pages
 Home-page: https://github.com/eddyluten/mkdocs-categories-plugin
 Author: Eddy Luten
 Author-email: eddyluten@gmail.com
 License: MIT
 Keywords: mkdocs python markdown category categories link wiki
 Classifier: License :: OSI Approved :: MIT License
@@ -136,14 +136,18 @@
 
 ### `The categories object at URL was not a list, but TYPE`
 
 The page identified did not contain a valid categories configuration object. Please make sure that this is an array of strings.
 
 ## Changelog
 
+### 0.4.0
+
+Fixes sorting categories, child pages, etc. containing numbers by using natural sorting from the `natsort` package rather than the default sorting function.
+
 ### 0.3.0
 
 Added support for subcategories. Python 3.10 or higher is now required.
 
 ### 0.2.1
 
 Patch release: implements a bug fix by @rpmzandwijk reported in [#1](https://github.com/EddyLuten/mkdocs-categories-plugin/issues/1).
```

### Comparing `mkdocs-categories-plugin-0.3.0/setup.py` & `mkdocs-categories-plugin-0.4.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,26 +3,29 @@
 from setuptools import setup, find_packages
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name='mkdocs-categories-plugin',
-    version='0.3.0',
+    version='0.4.0',
     description=
     'An MkDocs plugin allowing for categorization of pages',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords='mkdocs python markdown category categories link wiki',
     url='https://github.com/eddyluten/mkdocs-categories-plugin',
     author='Eddy Luten',
     author_email='eddyluten@gmail.com',
     license='MIT',
     python_requires='>=3.10',
-    install_requires=['mkdocs'],
+    install_requires=[
+        'mkdocs',
+        'natsort>=8.4.0'
+    ],
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3 :: Only',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
     packages=find_packages(exclude=['*.tests']),
```

