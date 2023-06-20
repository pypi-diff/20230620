# Comparing `tmp/markyp-html-0.2306.1.tar.gz` & `tmp/markyp-html-0.2306.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markyp-html-0.2306.1.tar", last modified: Tue Jun 20 11:59:03 2023, max compression
+gzip compressed data, was "markyp-html-0.2306.2.tar", last modified: Tue Jun 20 12:31:13 2023, max compression
```

## Comparing `markyp-html-0.2306.1.tar` & `markyp-html-0.2306.2.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-20 11:59:03.454526 markyp-html-0.2306.1/
--rw-rw-r--   0 peter     (1000) peter     (1000)     1067 2023-06-19 14:29:32.000000 markyp-html-0.2306.1/LICENSE
--rw-rw-r--   0 peter     (1000) peter     (1000)     6297 2023-06-20 11:59:03.454526 markyp-html-0.2306.1/PKG-INFO
--rw-rw-r--   0 peter     (1000) peter     (1000)     5188 2023-06-19 14:29:32.000000 markyp-html-0.2306.1/README.md
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-20 11:59:03.450526 markyp-html-0.2306.1/markyp_html/
--rw-rw-r--   0 peter     (1000) peter     (1000)     7414 2023-06-20 11:58:32.000000 markyp-html-0.2306.1/markyp_html/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3401 2023-06-19 14:29:32.000000 markyp-html-0.2306.1/markyp_html/block.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1400 2023-06-19 14:29:32.000000 markyp-html-0.2306.1/markyp_html/entities.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     7192 2023-06-19 14:29:32.000000 markyp-html-0.2306.1/markyp_html/forms.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     5951 2023-06-19 14:29:32.000000 markyp-html-0.2306.1/markyp_html/inline.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1146 2023-06-19 14:29:32.000000 markyp-html-0.2306.1/markyp_html/lists.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1555 2023-06-19 14:29:32.000000 markyp-html-0.2306.1/markyp_html/tables.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     5792 2023-06-19 14:29:32.000000 markyp-html-0.2306.1/markyp_html/text.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-20 11:59:03.450526 markyp-html-0.2306.1/markyp_html.egg-info/
--rw-rw-r--   0 peter     (1000) peter     (1000)     6297 2023-06-20 11:59:03.000000 markyp-html-0.2306.1/markyp_html.egg-info/PKG-INFO
--rw-rw-r--   0 peter     (1000) peter     (1000)      530 2023-06-20 11:59:03.000000 markyp-html-0.2306.1/markyp_html.egg-info/SOURCES.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)        1 2023-06-20 11:59:03.000000 markyp-html-0.2306.1/markyp_html.egg-info/dependency_links.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)       15 2023-06-20 11:59:03.000000 markyp-html-0.2306.1/markyp_html.egg-info/requires.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)       12 2023-06-20 11:59:03.000000 markyp-html-0.2306.1/markyp_html.egg-info/top_level.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)       38 2023-06-20 11:59:03.454526 markyp-html-0.2306.1/setup.cfg
--rw-rw-r--   0 peter     (1000) peter     (1000)     2589 2023-06-19 14:29:32.000000 markyp-html-0.2306.1/setup.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-20 11:59:03.454526 markyp-html-0.2306.1/test/
--rw-rw-r--   0 peter     (1000) peter     (1000)     2663 2023-06-19 14:29:32.000000 markyp-html-0.2306.1/test/test_block.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1017 2023-06-19 14:29:32.000000 markyp-html-0.2306.1/test/test_entities.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3311 2023-06-19 14:29:32.000000 markyp-html-0.2306.1/test/test_forms.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     4835 2023-06-19 14:29:32.000000 markyp-html-0.2306.1/test/test_init.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3906 2023-06-19 14:29:32.000000 markyp-html-0.2306.1/test/test_inline.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      915 2023-06-19 14:29:32.000000 markyp-html-0.2306.1/test/test_lists.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1370 2023-06-19 14:29:32.000000 markyp-html-0.2306.1/test/test_tables.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1579 2023-06-19 14:29:32.000000 markyp-html-0.2306.1/test/test_text.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-20 12:31:13.668322 markyp-html-0.2306.2/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1067 2023-06-19 14:29:32.000000 markyp-html-0.2306.2/LICENSE
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6297 2023-06-20 12:31:13.668322 markyp-html-0.2306.2/PKG-INFO
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5188 2023-06-19 14:29:32.000000 markyp-html-0.2306.2/README.md
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-20 12:31:13.664322 markyp-html-0.2306.2/markyp_html/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     7414 2023-06-20 12:30:51.000000 markyp-html-0.2306.2/markyp_html/__init__.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3401 2023-06-19 14:29:32.000000 markyp-html-0.2306.2/markyp_html/block.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1400 2023-06-19 14:29:32.000000 markyp-html-0.2306.2/markyp_html/entities.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     7192 2023-06-19 14:29:32.000000 markyp-html-0.2306.2/markyp_html/forms.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5951 2023-06-19 14:29:32.000000 markyp-html-0.2306.2/markyp_html/inline.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1146 2023-06-19 14:29:32.000000 markyp-html-0.2306.2/markyp_html/lists.py
+-rw-r--r--   0 peter     (1000) peter     (1000)        0 2023-06-19 14:29:55.000000 markyp-html-0.2306.2/markyp_html/py.typed
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1555 2023-06-19 14:29:32.000000 markyp-html-0.2306.2/markyp_html/tables.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5792 2023-06-19 14:29:32.000000 markyp-html-0.2306.2/markyp_html/text.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-20 12:31:13.664322 markyp-html-0.2306.2/markyp_html.egg-info/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6297 2023-06-20 12:31:13.000000 markyp-html-0.2306.2/markyp_html.egg-info/PKG-INFO
+-rw-rw-r--   0 peter     (1000) peter     (1000)      551 2023-06-20 12:31:13.000000 markyp-html-0.2306.2/markyp_html.egg-info/SOURCES.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)        1 2023-06-20 12:31:13.000000 markyp-html-0.2306.2/markyp_html.egg-info/dependency_links.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)       15 2023-06-20 12:31:13.000000 markyp-html-0.2306.2/markyp_html.egg-info/requires.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)       12 2023-06-20 12:31:13.000000 markyp-html-0.2306.2/markyp_html.egg-info/top_level.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)       38 2023-06-20 12:31:13.668322 markyp-html-0.2306.2/setup.cfg
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2637 2023-06-20 12:30:10.000000 markyp-html-0.2306.2/setup.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-20 12:31:13.668322 markyp-html-0.2306.2/test/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2663 2023-06-19 14:29:32.000000 markyp-html-0.2306.2/test/test_block.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1017 2023-06-19 14:29:32.000000 markyp-html-0.2306.2/test/test_entities.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3311 2023-06-19 14:29:32.000000 markyp-html-0.2306.2/test/test_forms.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4835 2023-06-19 14:29:32.000000 markyp-html-0.2306.2/test/test_init.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3906 2023-06-19 14:29:32.000000 markyp-html-0.2306.2/test/test_inline.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      915 2023-06-19 14:29:32.000000 markyp-html-0.2306.2/test/test_lists.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1370 2023-06-19 14:29:32.000000 markyp-html-0.2306.2/test/test_tables.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1579 2023-06-19 14:29:32.000000 markyp-html-0.2306.2/test/test_text.py
```

### Comparing `markyp-html-0.2306.1/LICENSE` & `markyp-html-0.2306.2/LICENSE`

 * *Files identical despite different names*

### Comparing `markyp-html-0.2306.1/PKG-INFO` & `markyp-html-0.2306.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markyp-html
-Version: 0.2306.1
+Version: 0.2306.2
 Summary: HTML element implementations based on markyp.
 Home-page: https://github.com/volfpeter/markyp-html
 Author: Peter Volf
 Author-email: do.volfp@gmail.com
 License: MIT
 Keywords: html markup generator utility
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `markyp-html-0.2306.1/README.md` & `markyp-html-0.2306.2/README.md`

 * *Files identical despite different names*

### Comparing `markyp-html-0.2306.1/markyp_html/__init__.py` & `markyp-html-0.2306.2/markyp_html/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 __author__ = "Peter Volf"
 __copyright__ = "Copyright 2019, Peter Volf"
 __email__ = "do.volfp@gmail.com"
 __license__ = "MIT"
 __url__ = "https://github.com/volfpeter/markyp-html"
-__version__ = "0.2306.1"
+__version__ = "0.2306.2"
 
 
 __all__ = ("DOCTYPE", "html", "head", "body", "base", "title", "link", "meta", "script", "style")
 
 
 class DOCTYPE(IElement):
     """
```

### Comparing `markyp-html-0.2306.1/markyp_html/block.py` & `markyp-html-0.2306.2/markyp_html/block.py`

 * *Files identical despite different names*

### Comparing `markyp-html-0.2306.1/markyp_html/entities.py` & `markyp-html-0.2306.2/markyp_html/entities.py`

 * *Files identical despite different names*

### Comparing `markyp-html-0.2306.1/markyp_html/forms.py` & `markyp-html-0.2306.2/markyp_html/forms.py`

 * *Files identical despite different names*

### Comparing `markyp-html-0.2306.1/markyp_html/inline.py` & `markyp-html-0.2306.2/markyp_html/inline.py`

 * *Files identical despite different names*

### Comparing `markyp-html-0.2306.1/markyp_html/lists.py` & `markyp-html-0.2306.2/markyp_html/lists.py`

 * *Files identical despite different names*

### Comparing `markyp-html-0.2306.1/markyp_html/tables.py` & `markyp-html-0.2306.2/markyp_html/tables.py`

 * *Files identical despite different names*

### Comparing `markyp-html-0.2306.1/markyp_html/text.py` & `markyp-html-0.2306.2/markyp_html/text.py`

 * *Files identical despite different names*

### Comparing `markyp-html-0.2306.1/markyp_html.egg-info/PKG-INFO` & `markyp-html-0.2306.2/markyp_html.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markyp-html
-Version: 0.2306.1
+Version: 0.2306.2
 Summary: HTML element implementations based on markyp.
 Home-page: https://github.com/volfpeter/markyp-html
 Author: Peter Volf
 Author-email: do.volfp@gmail.com
 License: MIT
 Keywords: html markup generator utility
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `markyp-html-0.2306.1/markyp_html.egg-info/SOURCES.txt` & `markyp-html-0.2306.2/markyp_html.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 setup.py
 markyp_html/__init__.py
 markyp_html/block.py
 markyp_html/entities.py
 markyp_html/forms.py
 markyp_html/inline.py
 markyp_html/lists.py
+markyp_html/py.typed
 markyp_html/tables.py
 markyp_html/text.py
 markyp_html.egg-info/PKG-INFO
 markyp_html.egg-info/SOURCES.txt
 markyp_html.egg-info/dependency_links.txt
 markyp_html.egg-info/requires.txt
 markyp_html.egg-info/top_level.txt
```

### Comparing `markyp-html-0.2306.1/setup.py` & `markyp-html-0.2306.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,10 +58,11 @@
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Text Processing :: Markup :: HTML",
         "Topic :: Utilities",
         "Typing :: Typed"
     ],
     keywords="html markup generator utility",
     packages=find_packages(exclude=["test"]),
+    package_data={"markyp_html": ["py.typed"]},
     python_requires=">=3.6",
     install_requires=requirements
 )
```

### Comparing `markyp-html-0.2306.1/test/test_block.py` & `markyp-html-0.2306.2/test/test_block.py`

 * *Files identical despite different names*

### Comparing `markyp-html-0.2306.1/test/test_entities.py` & `markyp-html-0.2306.2/test/test_entities.py`

 * *Files identical despite different names*

### Comparing `markyp-html-0.2306.1/test/test_forms.py` & `markyp-html-0.2306.2/test/test_forms.py`

 * *Files identical despite different names*

### Comparing `markyp-html-0.2306.1/test/test_init.py` & `markyp-html-0.2306.2/test/test_init.py`

 * *Files identical despite different names*

### Comparing `markyp-html-0.2306.1/test/test_inline.py` & `markyp-html-0.2306.2/test/test_inline.py`

 * *Files identical despite different names*

### Comparing `markyp-html-0.2306.1/test/test_lists.py` & `markyp-html-0.2306.2/test/test_lists.py`

 * *Files identical despite different names*

### Comparing `markyp-html-0.2306.1/test/test_tables.py` & `markyp-html-0.2306.2/test/test_tables.py`

 * *Files identical despite different names*

### Comparing `markyp-html-0.2306.1/test/test_text.py` & `markyp-html-0.2306.2/test/test_text.py`

 * *Files identical despite different names*

