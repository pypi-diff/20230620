# Comparing `tmp/markyp-html-0.1910.0.tar.gz` & `tmp/markyp-html-0.2306.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/markyp-html-0.1910.0.tar", last modified: Mon Oct 14 17:52:42 2019, max compression
+gzip compressed data, was "markyp-html-0.2306.0.tar", last modified: Mon Jun 19 14:32:08 2023, max compression
```

## Comparing `markyp-html-0.1910.0.tar` & `markyp-html-0.2306.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2019-10-14 17:52:42.000000 markyp-html-0.1910.0/
--rw-r--r--   0 peter      (501) staff       (20)     6943 2019-10-14 17:52:42.000000 markyp-html-0.1910.0/PKG-INFO
--rw-r--r--   0 peter      (501) staff       (20)     5033 2019-06-17 19:58:42.000000 markyp-html-0.1910.0/README.md
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2019-10-14 17:52:42.000000 markyp-html-0.1910.0/markyp_html/
--rw-r--r--   0 peter      (501) staff       (20)     7420 2019-10-14 15:34:05.000000 markyp-html-0.1910.0/markyp_html/__init__.py
--rw-r--r--   0 peter      (501) staff       (20)     3401 2019-04-25 12:47:56.000000 markyp-html-0.1910.0/markyp_html/block.py
--rw-r--r--   0 peter      (501) staff       (20)     1326 2019-06-02 09:22:08.000000 markyp-html-0.1910.0/markyp_html/entities.py
--rw-r--r--   0 peter      (501) staff       (20)     7192 2019-05-04 08:40:51.000000 markyp-html-0.1910.0/markyp_html/forms.py
--rw-r--r--   0 peter      (501) staff       (20)     5951 2019-04-25 20:55:20.000000 markyp-html-0.1910.0/markyp_html/inline.py
--rw-r--r--   0 peter      (501) staff       (20)     1146 2019-04-20 11:54:52.000000 markyp-html-0.1910.0/markyp_html/lists.py
--rw-r--r--   0 peter      (501) staff       (20)     1555 2019-04-20 11:55:39.000000 markyp-html-0.1910.0/markyp_html/tables.py
--rw-r--r--   0 peter      (501) staff       (20)     5792 2019-04-20 11:56:23.000000 markyp-html-0.1910.0/markyp_html/text.py
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2019-10-14 17:52:42.000000 markyp-html-0.1910.0/markyp_html.egg-info/
--rw-r--r--   0 peter      (501) staff       (20)     6943 2019-10-14 17:52:42.000000 markyp-html-0.1910.0/markyp_html.egg-info/PKG-INFO
--rw-r--r--   0 peter      (501) staff       (20)      522 2019-10-14 17:52:42.000000 markyp-html-0.1910.0/markyp_html.egg-info/SOURCES.txt
--rw-r--r--   0 peter      (501) staff       (20)        1 2019-10-14 17:52:42.000000 markyp-html-0.1910.0/markyp_html.egg-info/dependency_links.txt
--rw-r--r--   0 peter      (501) staff       (20)       15 2019-10-14 17:52:42.000000 markyp-html-0.1910.0/markyp_html.egg-info/requires.txt
--rw-r--r--   0 peter      (501) staff       (20)       12 2019-10-14 17:52:42.000000 markyp-html-0.1910.0/markyp_html.egg-info/top_level.txt
--rw-r--r--   0 peter      (501) staff       (20)       38 2019-10-14 17:52:42.000000 markyp-html-0.1910.0/setup.cfg
--rw-r--r--   0 peter      (501) staff       (20)     2589 2019-10-14 13:33:27.000000 markyp-html-0.1910.0/setup.py
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2019-10-14 17:52:42.000000 markyp-html-0.1910.0/test/
--rw-r--r--   0 peter      (501) staff       (20)     2663 2019-04-25 12:49:13.000000 markyp-html-0.1910.0/test/test_block.py
--rw-r--r--   0 peter      (501) staff       (20)     1409 2019-04-03 10:08:15.000000 markyp-html-0.1910.0/test/test_entities.py
--rw-r--r--   0 peter      (501) staff       (20)     3311 2019-05-05 19:08:30.000000 markyp-html-0.1910.0/test/test_forms.py
--rw-r--r--   0 peter      (501) staff       (20)     4835 2019-04-08 16:27:53.000000 markyp-html-0.1910.0/test/test_init.py
--rw-r--r--   0 peter      (501) staff       (20)     3906 2019-04-25 20:55:35.000000 markyp-html-0.1910.0/test/test_inline.py
--rw-r--r--   0 peter      (501) staff       (20)      915 2019-03-25 21:01:05.000000 markyp-html-0.1910.0/test/test_lists.py
--rw-r--r--   0 peter      (501) staff       (20)     1370 2019-03-25 21:15:33.000000 markyp-html-0.1910.0/test/test_tables.py
--rw-r--r--   0 peter      (501) staff       (20)     1579 2019-04-20 15:40:07.000000 markyp-html-0.1910.0/test/test_text.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-19 14:32:08.279081 markyp-html-0.2306.0/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1067 2023-06-19 14:29:32.000000 markyp-html-0.2306.0/LICENSE
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6297 2023-06-19 14:32:08.279081 markyp-html-0.2306.0/PKG-INFO
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5188 2023-06-19 14:29:32.000000 markyp-html-0.2306.0/README.md
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-19 14:32:08.279081 markyp-html-0.2306.0/markyp_html/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     7414 2023-06-19 14:30:22.000000 markyp-html-0.2306.0/markyp_html/__init__.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3401 2023-06-19 14:29:32.000000 markyp-html-0.2306.0/markyp_html/block.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1400 2023-06-19 14:29:32.000000 markyp-html-0.2306.0/markyp_html/entities.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     7192 2023-06-19 14:29:32.000000 markyp-html-0.2306.0/markyp_html/forms.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5951 2023-06-19 14:29:32.000000 markyp-html-0.2306.0/markyp_html/inline.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1146 2023-06-19 14:29:32.000000 markyp-html-0.2306.0/markyp_html/lists.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1555 2023-06-19 14:29:32.000000 markyp-html-0.2306.0/markyp_html/tables.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5792 2023-06-19 14:29:32.000000 markyp-html-0.2306.0/markyp_html/text.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-19 14:32:08.279081 markyp-html-0.2306.0/markyp_html.egg-info/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6297 2023-06-19 14:32:08.000000 markyp-html-0.2306.0/markyp_html.egg-info/PKG-INFO
+-rw-rw-r--   0 peter     (1000) peter     (1000)      530 2023-06-19 14:32:08.000000 markyp-html-0.2306.0/markyp_html.egg-info/SOURCES.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)        1 2023-06-19 14:32:08.000000 markyp-html-0.2306.0/markyp_html.egg-info/dependency_links.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)       15 2023-06-19 14:32:08.000000 markyp-html-0.2306.0/markyp_html.egg-info/requires.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)       12 2023-06-19 14:32:08.000000 markyp-html-0.2306.0/markyp_html.egg-info/top_level.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)       38 2023-06-19 14:32:08.279081 markyp-html-0.2306.0/setup.cfg
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2589 2023-06-19 14:29:32.000000 markyp-html-0.2306.0/setup.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-19 14:32:08.279081 markyp-html-0.2306.0/test/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2663 2023-06-19 14:29:32.000000 markyp-html-0.2306.0/test/test_block.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1017 2023-06-19 14:29:32.000000 markyp-html-0.2306.0/test/test_entities.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3311 2023-06-19 14:29:32.000000 markyp-html-0.2306.0/test/test_forms.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4835 2023-06-19 14:29:32.000000 markyp-html-0.2306.0/test/test_init.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3906 2023-06-19 14:29:32.000000 markyp-html-0.2306.0/test/test_inline.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      915 2023-06-19 14:29:32.000000 markyp-html-0.2306.0/test/test_lists.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1370 2023-06-19 14:29:32.000000 markyp-html-0.2306.0/test/test_tables.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1579 2023-06-19 14:29:32.000000 markyp-html-0.2306.0/test/test_text.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `markyp-html-0.1910.0/README.md` & `markyp-html-0.2306.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -53,18 +53,19 @@
 print(html)
 ```
 
 ## `markyp-html` extensions
 
 `markyp-html` is built on [markyp](https://github.com/volfpeter/markyp). In general, extensions follow the `markyp-{domain-or-extension-name}` naming convention.
 
-Here is a list of extension built on top of `markyp-html`:
+Here is a list of extensions built on top of `markyp-html`:
 
-- `markyp-highlightjs`: Code highlighting in HTML using `highlight.js` at https://github.com/volfpeter/markyp-highlightjs, contribution is welcome.
 - `markyp-bootstrap4`: Bootstrap 4 implementation at https://github.com/volfpeter/markyp-bootstrap4, contribution is welcome.
+- `markyp-fontawesome`: Font Awesome icons for `markyp-html`-based web pages at https://github.com/volfpeter/markyp-fontawesome, contribution is welcome.
+- `markyp-highlightjs`: Code highlighting in HTML using `highlight.js` at https://github.com/volfpeter/markyp-highlightjs, contribution is welcome.
 
 If you have created an open source `markyp-html` extension, please let us know and we will include your project in this list.
 
 ## Community guidelines
 
 In general, please treat each other with respect and follow the below guidelines to interact with the project:
```

### Comparing `markyp-html-0.1910.0/markyp_html/__init__.py` & `markyp-html-0.2306.0/markyp_html/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 The base elements that are required in all HTML documents.
 """
 
-from typing import Dict, Optional, Sequence, Union
+from typing import Optional, Sequence, Union
 
 from markyp import ElementType, IElement
 from markyp.elements import Element, ElementSequence, StandaloneElement, StringElement
 from markyp.formatters import format_properties
 
 
 __author__ = "Peter Volf"
 __copyright__ = "Copyright 2019, Peter Volf"
 __email__ = "do.volfp@gmail.com"
 __license__ = "MIT"
 __url__ = "https://github.com/volfpeter/markyp-html"
-__version__ = "0.1910.0"
+__version__ = "0.2306.0"
 
 
 __all__ = ("DOCTYPE", "html", "head", "body", "base", "title", "link", "meta", "script", "style")
 
 
 class DOCTYPE(IElement):
     """
```

### Comparing `markyp-html-0.1910.0/markyp_html/block.py` & `markyp-html-0.2306.0/markyp_html/block.py`

 * *Files identical despite different names*

### Comparing `markyp-html-0.1910.0/markyp_html/forms.py` & `markyp-html-0.2306.0/markyp_html/forms.py`

 * *Files identical despite different names*

### Comparing `markyp-html-0.1910.0/markyp_html/inline.py` & `markyp-html-0.2306.0/markyp_html/inline.py`

 * *Files identical despite different names*

### Comparing `markyp-html-0.1910.0/markyp_html/lists.py` & `markyp-html-0.2306.0/markyp_html/lists.py`

 * *Files identical despite different names*

### Comparing `markyp-html-0.1910.0/markyp_html/tables.py` & `markyp-html-0.2306.0/markyp_html/tables.py`

 * *Files identical despite different names*

### Comparing `markyp-html-0.1910.0/markyp_html/text.py` & `markyp-html-0.2306.0/markyp_html/text.py`

 * *Files identical despite different names*

### Comparing `markyp-html-0.1910.0/markyp_html.egg-info/SOURCES.txt` & `markyp-html-0.2306.0/markyp_html.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 markyp_html/__init__.py
 markyp_html/block.py
 markyp_html/entities.py
 markyp_html/forms.py
 markyp_html/inline.py
```

### Comparing `markyp-html-0.1910.0/setup.py` & `markyp-html-0.2306.0/setup.py`

 * *Files identical despite different names*

### Comparing `markyp-html-0.1910.0/test/test_block.py` & `markyp-html-0.2306.0/test/test_block.py`

 * *Files identical despite different names*

### Comparing `markyp-html-0.1910.0/test/test_forms.py` & `markyp-html-0.2306.0/test/test_forms.py`

 * *Files identical despite different names*

### Comparing `markyp-html-0.1910.0/test/test_init.py` & `markyp-html-0.2306.0/test/test_init.py`

 * *Files identical despite different names*

### Comparing `markyp-html-0.1910.0/test/test_inline.py` & `markyp-html-0.2306.0/test/test_inline.py`

 * *Files identical despite different names*

### Comparing `markyp-html-0.1910.0/test/test_lists.py` & `markyp-html-0.2306.0/test/test_lists.py`

 * *Files identical despite different names*

### Comparing `markyp-html-0.1910.0/test/test_tables.py` & `markyp-html-0.2306.0/test/test_tables.py`

 * *Files identical despite different names*

### Comparing `markyp-html-0.1910.0/test/test_text.py` & `markyp-html-0.2306.0/test/test_text.py`

 * *Files identical despite different names*

