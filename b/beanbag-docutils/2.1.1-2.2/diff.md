# Comparing `tmp/beanbag-docutils-2.1.1.tar.gz` & `tmp/beanbag-docutils-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beanbag-docutils-2.1.1.tar", last modified: Wed Mar  1 05:33:49 2023, max compression
+gzip compressed data, was "beanbag-docutils-2.2.tar", last modified: Tue Jun 20 02:55:13 2023, max compression
```

## Comparing `beanbag-docutils-2.1.1.tar` & `beanbag-docutils-2.2.tar`

### file list

```diff
@@ -1,42 +1,46 @@
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-03-01 05:33:49.771869 beanbag-docutils-2.1.1/
--rw-r--r--   0 chipx86    (501) staff       (20)       99 2023-03-01 05:33:49.000000 beanbag-docutils-2.1.1/AUTHORS
--rw-r--r--   0 chipx86    (501) staff       (20)     1058 2023-03-01 05:33:49.000000 beanbag-docutils-2.1.1/COPYING
--rw-r--r--   0 chipx86    (501) staff       (20)     2222 2023-03-01 05:33:49.771938 beanbag-docutils-2.1.1/PKG-INFO
--rw-r--r--   0 chipx86    (501) staff       (20)      992 2023-03-01 05:33:49.000000 beanbag-docutils-2.1.1/README.rst
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-03-01 05:33:49.768949 beanbag-docutils-2.1.1/beanbag_docutils/
--rw-r--r--   0 chipx86    (501) staff       (20)     1585 2023-03-01 05:33:49.000000 beanbag-docutils-2.1.1/beanbag_docutils/__init__.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-03-01 05:33:49.769570 beanbag-docutils-2.1.1/beanbag_docutils/sphinx/
--rw-r--r--   0 chipx86    (501) staff       (20)        0 2023-03-01 05:33:49.000000 beanbag-docutils-2.1.1/beanbag_docutils/sphinx/__init__.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-03-01 05:33:49.770682 beanbag-docutils-2.1.1/beanbag_docutils/sphinx/ext/
--rw-r--r--   0 chipx86    (501) staff       (20)        0 2023-03-01 05:33:49.000000 beanbag-docutils-2.1.1/beanbag_docutils/sphinx/ext/__init__.py
--rw-r--r--   0 chipx86    (501) staff       (20)    24700 2023-03-01 05:33:49.000000 beanbag-docutils-2.1.1/beanbag_docutils/sphinx/ext/autodoc_utils.py
--rw-r--r--   0 chipx86    (501) staff       (20)     2561 2023-03-01 05:33:49.000000 beanbag-docutils-2.1.1/beanbag_docutils/sphinx/ext/collect_files.py
--rw-r--r--   0 chipx86    (501) staff       (20)     1812 2023-03-01 05:33:49.000000 beanbag-docutils-2.1.1/beanbag_docutils/sphinx/ext/django_utils.py
--rw-r--r--   0 chipx86    (501) staff       (20)     3453 2023-03-01 05:33:49.000000 beanbag-docutils-2.1.1/beanbag_docutils/sphinx/ext/extlinks.py
--rw-r--r--   0 chipx86    (501) staff       (20)    11077 2023-03-01 05:33:49.000000 beanbag-docutils-2.1.1/beanbag_docutils/sphinx/ext/github.py
--rw-r--r--   0 chipx86    (501) staff       (20)     7415 2023-03-01 05:33:49.000000 beanbag-docutils-2.1.1/beanbag_docutils/sphinx/ext/http_role.py
--rw-r--r--   0 chipx86    (501) staff       (20)     7949 2023-03-01 05:33:49.000000 beanbag-docutils-2.1.1/beanbag_docutils/sphinx/ext/image_srcsets.py
--rw-r--r--   0 chipx86    (501) staff       (20)     6270 2023-03-01 05:33:49.000000 beanbag-docutils-2.1.1/beanbag_docutils/sphinx/ext/intersphinx_utils.py
--rw-r--r--   0 chipx86    (501) staff       (20)     1714 2023-03-01 05:33:49.000000 beanbag-docutils-2.1.1/beanbag_docutils/sphinx/ext/ref_utils.py
--rw-r--r--   0 chipx86    (501) staff       (20)     3630 2023-03-01 05:33:49.000000 beanbag-docutils-2.1.1/beanbag_docutils/sphinx/ext/retina_images.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-03-01 05:33:49.771597 beanbag-docutils-2.1.1/beanbag_docutils/sphinx/ext/tests/
--rw-r--r--   0 chipx86    (501) staff       (20)        0 2023-03-01 05:33:49.000000 beanbag-docutils-2.1.1/beanbag_docutils/sphinx/ext/tests/__init__.py
--rw-r--r--   0 chipx86    (501) staff       (20)    18742 2023-03-01 05:33:49.000000 beanbag-docutils-2.1.1/beanbag_docutils/sphinx/ext/tests/test_autodoc_utils.py
--rw-r--r--   0 chipx86    (501) staff       (20)     2283 2023-03-01 05:33:49.000000 beanbag-docutils-2.1.1/beanbag_docutils/sphinx/ext/tests/test_django_utils.py
--rw-r--r--   0 chipx86    (501) staff       (20)      873 2023-03-01 05:33:49.000000 beanbag-docutils-2.1.1/beanbag_docutils/sphinx/ext/tests/test_extlinks.py
--rw-r--r--   0 chipx86    (501) staff       (20)    23549 2023-03-01 05:33:49.000000 beanbag-docutils-2.1.1/beanbag_docutils/sphinx/ext/tests/test_github.py
--rw-r--r--   0 chipx86    (501) staff       (20)     2325 2023-03-01 05:33:49.000000 beanbag-docutils-2.1.1/beanbag_docutils/sphinx/ext/tests/test_http_role.py
--rw-r--r--   0 chipx86    (501) staff       (20)     1819 2023-03-01 05:33:49.000000 beanbag-docutils-2.1.1/beanbag_docutils/sphinx/ext/tests/test_image_srcsets.py
--rw-r--r--   0 chipx86    (501) staff       (20)     1304 2023-03-01 05:33:49.000000 beanbag-docutils-2.1.1/beanbag_docutils/sphinx/ext/tests/test_ref_utils.py
--rw-r--r--   0 chipx86    (501) staff       (20)     3985 2023-03-01 05:33:49.000000 beanbag-docutils-2.1.1/beanbag_docutils/sphinx/ext/tests/testcase.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-03-01 05:33:49.771778 beanbag-docutils-2.1.1/beanbag_docutils/sphinx/ext/tests/testdata/
--rw-r--r--   0 chipx86    (501) staff       (20)        0 2023-03-01 05:33:49.000000 beanbag-docutils-2.1.1/beanbag_docutils/sphinx/ext/tests/testdata/__init__.py
--rw-r--r--   0 chipx86    (501) staff       (20)      380 2023-03-01 05:33:49.000000 beanbag-docutils-2.1.1/beanbag_docutils/sphinx/ext/tests/testdata/github_linkcode_module.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-03-01 05:33:49.769474 beanbag-docutils-2.1.1/beanbag_docutils.egg-info/
--rw-r--r--   0 chipx86    (501) staff       (20)     2222 2023-03-01 05:33:49.000000 beanbag-docutils-2.1.1/beanbag_docutils.egg-info/PKG-INFO
--rw-r--r--   0 chipx86    (501) staff       (20)     1369 2023-03-01 05:33:49.000000 beanbag-docutils-2.1.1/beanbag_docutils.egg-info/SOURCES.txt
--rw-r--r--   0 chipx86    (501) staff       (20)        1 2023-03-01 05:33:49.000000 beanbag-docutils-2.1.1/beanbag_docutils.egg-info/dependency_links.txt
--rw-r--r--   0 chipx86    (501) staff       (20)        7 2023-03-01 05:33:49.000000 beanbag-docutils-2.1.1/beanbag_docutils.egg-info/requires.txt
--rw-r--r--   0 chipx86    (501) staff       (20)       17 2023-03-01 05:33:49.000000 beanbag-docutils-2.1.1/beanbag_docutils.egg-info/top_level.txt
--rw-r--r--   0 chipx86    (501) staff       (20)       76 2023-03-01 05:33:49.772138 beanbag-docutils-2.1.1/setup.cfg
--rwxr-xr-x   0 chipx86    (501) staff       (20)     1555 2023-03-01 05:33:49.000000 beanbag-docutils-2.1.1/setup.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-06-20 02:55:13.924128 beanbag-docutils-2.2/
+-rw-r--r--   0 chipx86    (501) staff       (20)       99 2023-06-20 02:55:13.000000 beanbag-docutils-2.2/AUTHORS
+-rw-r--r--   0 chipx86    (501) staff       (20)     1058 2023-06-20 02:55:13.000000 beanbag-docutils-2.2/COPYING
+-rw-r--r--   0 chipx86    (501) staff       (20)     3793 2023-06-20 02:55:13.924205 beanbag-docutils-2.2/PKG-INFO
+-rw-r--r--   0 chipx86    (501) staff       (20)     2437 2023-06-20 02:55:13.000000 beanbag-docutils-2.2/README.rst
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-06-20 02:55:13.920444 beanbag-docutils-2.2/beanbag_docutils/
+-rw-r--r--   0 chipx86    (501) staff       (20)     1585 2023-06-20 02:55:13.000000 beanbag-docutils-2.2/beanbag_docutils/__init__.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-06-20 02:55:13.921120 beanbag-docutils-2.2/beanbag_docutils/sphinx/
+-rw-r--r--   0 chipx86    (501) staff       (20)        0 2023-06-20 02:55:13.000000 beanbag-docutils-2.2/beanbag_docutils/sphinx/__init__.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-06-20 02:55:13.922551 beanbag-docutils-2.2/beanbag_docutils/sphinx/ext/
+-rw-r--r--   0 chipx86    (501) staff       (20)        0 2023-06-20 02:55:13.000000 beanbag-docutils-2.2/beanbag_docutils/sphinx/ext/__init__.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    24702 2023-06-20 02:55:13.000000 beanbag-docutils-2.2/beanbag_docutils/sphinx/ext/autodoc_utils.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     2561 2023-06-20 02:55:13.000000 beanbag-docutils-2.2/beanbag_docutils/sphinx/ext/collect_files.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     1812 2023-06-20 02:55:13.000000 beanbag-docutils-2.2/beanbag_docutils/sphinx/ext/django_utils.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     3453 2023-06-20 02:55:13.000000 beanbag-docutils-2.2/beanbag_docutils/sphinx/ext/extlinks.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    11077 2023-06-20 02:55:13.000000 beanbag-docutils-2.2/beanbag_docutils/sphinx/ext/github.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     7409 2023-06-20 02:55:13.000000 beanbag-docutils-2.2/beanbag_docutils/sphinx/ext/http_role.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     7949 2023-06-20 02:55:13.000000 beanbag-docutils-2.2/beanbag_docutils/sphinx/ext/image_srcsets.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     6270 2023-06-20 02:55:13.000000 beanbag-docutils-2.2/beanbag_docutils/sphinx/ext/intersphinx_utils.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     6055 2023-06-20 02:55:13.000000 beanbag-docutils-2.2/beanbag_docutils/sphinx/ext/json_writer.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     3270 2023-06-20 02:55:13.000000 beanbag-docutils-2.2/beanbag_docutils/sphinx/ext/metadata.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     1714 2023-06-20 02:55:13.000000 beanbag-docutils-2.2/beanbag_docutils/sphinx/ext/ref_utils.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     3630 2023-06-20 02:55:13.000000 beanbag-docutils-2.2/beanbag_docutils/sphinx/ext/retina_images.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-06-20 02:55:13.923811 beanbag-docutils-2.2/beanbag_docutils/sphinx/ext/tests/
+-rw-r--r--   0 chipx86    (501) staff       (20)        0 2023-06-20 02:55:13.000000 beanbag-docutils-2.2/beanbag_docutils/sphinx/ext/tests/__init__.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    18742 2023-06-20 02:55:13.000000 beanbag-docutils-2.2/beanbag_docutils/sphinx/ext/tests/test_autodoc_utils.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     2283 2023-06-20 02:55:13.000000 beanbag-docutils-2.2/beanbag_docutils/sphinx/ext/tests/test_django_utils.py
+-rw-r--r--   0 chipx86    (501) staff       (20)      873 2023-06-20 02:55:13.000000 beanbag-docutils-2.2/beanbag_docutils/sphinx/ext/tests/test_extlinks.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    23549 2023-06-20 02:55:13.000000 beanbag-docutils-2.2/beanbag_docutils/sphinx/ext/tests/test_github.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     2325 2023-06-20 02:55:13.000000 beanbag-docutils-2.2/beanbag_docutils/sphinx/ext/tests/test_http_role.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     1819 2023-06-20 02:55:13.000000 beanbag-docutils-2.2/beanbag_docutils/sphinx/ext/tests/test_image_srcsets.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     5550 2023-06-20 02:55:13.000000 beanbag-docutils-2.2/beanbag_docutils/sphinx/ext/tests/test_json_writer.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     1840 2023-06-20 02:55:13.000000 beanbag-docutils-2.2/beanbag_docutils/sphinx/ext/tests/test_metadata.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     1304 2023-06-20 02:55:13.000000 beanbag-docutils-2.2/beanbag_docutils/sphinx/ext/tests/test_ref_utils.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     5882 2023-06-20 02:55:13.000000 beanbag-docutils-2.2/beanbag_docutils/sphinx/ext/tests/testcase.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-06-20 02:55:13.924014 beanbag-docutils-2.2/beanbag_docutils/sphinx/ext/tests/testdata/
+-rw-r--r--   0 chipx86    (501) staff       (20)        0 2023-06-20 02:55:13.000000 beanbag-docutils-2.2/beanbag_docutils/sphinx/ext/tests/testdata/__init__.py
+-rw-r--r--   0 chipx86    (501) staff       (20)      380 2023-06-20 02:55:13.000000 beanbag-docutils-2.2/beanbag_docutils/sphinx/ext/tests/testdata/github_linkcode_module.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-06-20 02:55:13.921010 beanbag-docutils-2.2/beanbag_docutils.egg-info/
+-rw-r--r--   0 chipx86    (501) staff       (20)     3793 2023-06-20 02:55:13.000000 beanbag-docutils-2.2/beanbag_docutils.egg-info/PKG-INFO
+-rw-r--r--   0 chipx86    (501) staff       (20)     1557 2023-06-20 02:55:13.000000 beanbag-docutils-2.2/beanbag_docutils.egg-info/SOURCES.txt
+-rw-r--r--   0 chipx86    (501) staff       (20)        1 2023-06-20 02:55:13.000000 beanbag-docutils-2.2/beanbag_docutils.egg-info/dependency_links.txt
+-rw-r--r--   0 chipx86    (501) staff       (20)       50 2023-06-20 02:55:13.000000 beanbag-docutils-2.2/beanbag_docutils.egg-info/requires.txt
+-rw-r--r--   0 chipx86    (501) staff       (20)       17 2023-06-20 02:55:13.000000 beanbag-docutils-2.2/beanbag_docutils.egg-info/top_level.txt
+-rw-r--r--   0 chipx86    (501) staff       (20)       76 2023-06-20 02:55:13.924418 beanbag-docutils-2.2/setup.cfg
+-rwxr-xr-x   0 chipx86    (501) staff       (20)     1734 2023-06-20 02:55:13.000000 beanbag-docutils-2.2/setup.py
```

### Comparing `beanbag-docutils-2.1.1/COPYING` & `beanbag-docutils-2.2/COPYING`

 * *Files identical despite different names*

### Comparing `beanbag-docutils-2.1.1/PKG-INFO` & `beanbag-docutils-2.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 Metadata-Version: 2.1
 Name: beanbag-docutils
-Version: 2.1.1
+Version: 2.2
 Summary: Sphinx utility modules for Beanbag's documentation format.
 Home-page: https://github.com/beanbaginc/beanbag-docutils
 Maintainer: Christian Hammond
 Maintainer-email: christian@beanbaginc.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Other Environment
+Classifier: Framework :: Sphinx
+Classifier: Framework :: Sphinx :: Extension
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Documentation
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 License-File: COPYING
@@ -43,18 +46,52 @@
 
 .. _Review Board: https://www.reviewboard.org/
 .. _RBCommons: https://www.rbcommons.com/
 .. _Djblets: https://github.com/djblets/djblets/
 .. _RBTools: https://github.com/reviewboard/rbtools/
 
 
+Sphinx Extensions
+=================
+
+Most of the utilities are used with the Sphinx_ documentation system. Amongst
+other enhancements, this package offers:
+
+* A parser for the `Beanbag docstring format`_ (a variation on the `Google
+  docstring format`_), which we use for Python and JavaScript documentation
+* Enhancements for Sphinx's intersphinx_ system to provide per-page
+  intersphinx resolution options (useful for pages, such as release notes,
+  that need to link to different versions of the same docs, such as Django_ or
+  Python)
+* Enhancements to ReStructuredText references to let a reference name span
+  lines (useful for long Python/JavaScript module/class names)
+* Linking code references to GitHub documentation
+* High-DPI image embedding
+* A role for HTTP status codes
+* Access to document-defined metadata in a structured form when parsing
+  documents
+
+
+.. _Beanbag docstring format:
+   https://www.notion.so/reviewboard/Standard-Documentation-Format-4388f594d86547cc949b365cda3cf391
+.. _Django: https://www.djangoproject.com/
+.. _Google docstring format:
+   https://google.github.io/styleguide/pyguide.html#s3.8-comments-and-docstrings
+.. _intersphinx:
+   https://www.sphinx-doc.org/en/master/usage/extensions/intersphinx.html
+.. _our products: https://www.beanbaginc.com/
+.. _ReStructuredText:
+   https://docutils.sourceforge.io/docs/ref/rst/restructuredtext.html
+.. _Sphinx: https://www.sphinx-doc.org/
+
+
 Compatibility
 =============
 
-* beanbag-docutils 2.x supports Python 3.6-3.11.
+* beanbag-docutils 2.x supports Python 3.6-3.12 and Sphinx 1.8-7.x.
 * beanbag-docutils 1.x supports Python 2.7 and 3.6-3.10.
 
 
 Getting Started
 ===============
 
 To install the package, run:
```

### Comparing `beanbag-docutils-2.1.1/beanbag_docutils/__init__.py` & `beanbag-docutils-2.2/beanbag_docutils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #: The version of beanbag_docutils.
 #:
 #: This is in the format of:
 #:
 #:   (Major, Minor, Micro, alpha/beta/rc/final, Release Number, Released)
 #:
-VERSION = (2, 1, 1, 'final', 0, True)
+VERSION = (2, 2, 0, 'final', 0, True)
 
 
 def get_version_string():
     """Return the version as a human-readable string.
 
     Returns:
         unicode:
```

### Comparing `beanbag-docutils-2.1.1/beanbag_docutils/sphinx/ext/autodoc_utils.py` & `beanbag-docutils-2.2/beanbag_docutils/sphinx/ext/autodoc_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,15 @@
     def _convert_type_spec(type_part, type_aliases):
         try:
             return type_aliases[type_part]
         except KeyError:
             if type_part == 'None':
                 return ':obj:`None`'
             else:
-                return f':class:`{type_part}`'
+                return ':class:`%s`' % type_part
 
 
 class BeanbagDocstring(GoogleDocstring):
     """Docstring parser for the Beanbag documentation.
 
     This is based on the Google docstring format used by Napoleon, but with
     a few additions:
```

### Comparing `beanbag-docutils-2.1.1/beanbag_docutils/sphinx/ext/collect_files.py` & `beanbag-docutils-2.2/beanbag_docutils/sphinx/ext/collect_files.py`

 * *Files identical despite different names*

### Comparing `beanbag-docutils-2.1.1/beanbag_docutils/sphinx/ext/django_utils.py` & `beanbag-docutils-2.2/beanbag_docutils/sphinx/ext/django_utils.py`

 * *Files identical despite different names*

### Comparing `beanbag-docutils-2.1.1/beanbag_docutils/sphinx/ext/extlinks.py` & `beanbag-docutils-2.2/beanbag_docutils/sphinx/ext/extlinks.py`

 * *Files identical despite different names*

### Comparing `beanbag-docutils-2.1.1/beanbag_docutils/sphinx/ext/github.py` & `beanbag-docutils-2.2/beanbag_docutils/sphinx/ext/github.py`

 * *Files identical despite different names*

### Comparing `beanbag-docutils-2.1.1/beanbag_docutils/sphinx/ext/http_role.py` & `beanbag-docutils-2.2/beanbag_docutils/sphinx/ext/http_role.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,15 +229,15 @@
     return [node], []
 
 
 def setup(app):
     """Set up the Sphinx extension.
 
     This registers the :rst:role:`http` role,
-    :rst:directive:`http-status-codes-format` directive, and the configuration
+    :rst:dir:`http-status-codes-format` directive, and the configuration
     settings for specifying the format and URL for linking to HTTP status
     codes.
 
     Args:
         app (sphinx.application.Sphinx):
             The Sphinx application to register roles and configuration on.
     """
```

### Comparing `beanbag-docutils-2.1.1/beanbag_docutils/sphinx/ext/image_srcsets.py` & `beanbag-docutils-2.2/beanbag_docutils/sphinx/ext/image_srcsets.py`

 * *Files identical despite different names*

### Comparing `beanbag-docutils-2.1.1/beanbag_docutils/sphinx/ext/intersphinx_utils.py` & `beanbag-docutils-2.2/beanbag_docutils/sphinx/ext/intersphinx_utils.py`

 * *Files identical despite different names*

### Comparing `beanbag-docutils-2.1.1/beanbag_docutils/sphinx/ext/ref_utils.py` & `beanbag-docutils-2.2/beanbag_docutils/sphinx/ext/ref_utils.py`

 * *Files identical despite different names*

### Comparing `beanbag-docutils-2.1.1/beanbag_docutils/sphinx/ext/retina_images.py` & `beanbag-docutils-2.2/beanbag_docutils/sphinx/ext/retina_images.py`

 * *Files identical despite different names*

### Comparing `beanbag-docutils-2.1.1/beanbag_docutils/sphinx/ext/tests/test_autodoc_utils.py` & `beanbag-docutils-2.2/beanbag_docutils/sphinx/ext/tests/test_autodoc_utils.py`

 * *Files identical despite different names*

### Comparing `beanbag-docutils-2.1.1/beanbag_docutils/sphinx/ext/tests/test_django_utils.py` & `beanbag-docutils-2.2/beanbag_docutils/sphinx/ext/tests/test_django_utils.py`

 * *Files identical despite different names*

### Comparing `beanbag-docutils-2.1.1/beanbag_docutils/sphinx/ext/tests/test_extlinks.py` & `beanbag-docutils-2.2/beanbag_docutils/sphinx/ext/tests/test_extlinks.py`

 * *Files identical despite different names*

### Comparing `beanbag-docutils-2.1.1/beanbag_docutils/sphinx/ext/tests/test_github.py` & `beanbag-docutils-2.2/beanbag_docutils/sphinx/ext/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `beanbag-docutils-2.1.1/beanbag_docutils/sphinx/ext/tests/test_http_role.py` & `beanbag-docutils-2.2/beanbag_docutils/sphinx/ext/tests/test_http_role.py`

 * *Files identical despite different names*

### Comparing `beanbag-docutils-2.1.1/beanbag_docutils/sphinx/ext/tests/test_image_srcsets.py` & `beanbag-docutils-2.2/beanbag_docutils/sphinx/ext/tests/test_image_srcsets.py`

 * *Files identical despite different names*

### Comparing `beanbag-docutils-2.1.1/beanbag_docutils/sphinx/ext/tests/test_ref_utils.py` & `beanbag-docutils-2.2/beanbag_docutils/sphinx/ext/tests/test_ref_utils.py`

 * *Files identical despite different names*

### Comparing `beanbag-docutils-2.1.1/beanbag_docutils/sphinx/ext/tests/testcase.py` & `beanbag-docutils-2.2/beanbag_docutils/sphinx/ext/tests/testcase.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Base test case support for Sphinx extensions."""
 
 import os
-import shutil
-import tempfile
 from contextlib import contextmanager
 from unittest import TestCase
+from typing import Dict, Iterator
 
+import six
 from sphinx_testing.util import TestApp, docutils_namespace
 
 import beanbag_docutils
 
 
 _theme_path = os.path.abspath(os.path.join(beanbag_docutils.__file__,
                                            '..', '..', 'tests', 'sphinx',
@@ -75,60 +75,122 @@
                     'app': app,
                     'config': app.config,
                     'srcdir': app.srcdir,
                 }
             finally:
                 app.cleanup()
 
-    def render_doc(self, doc_content, config={}, builder_name='html',
-                   extra_files={}):
-        """Render a ReST document to a string.
+    @contextmanager
+    def rendered_docs(
+        self,
+        files={},            # type: Dict
+        config={},           # type: Dict
+        builder_name='html'  # type: str
+    ):  # type: (...) -> Iterator[str]
+        """Render ReST documents and yield the directory for processing.
 
         This will set up a Sphinx environment, based on the extensions and
         configuration provided by the consumer, and perform a render of the
-        given ReST content. The resulting string will be a rendered version
-        of just that content.
+        given ReST files. The caller can then inspect the files within the
+        environment.
+
+        Version Added:
+            2.2
 
         Args:
-            doc_content (unicode):
-                The ReST content to render.
+            files (dict):
+                A mapping of filenames and contents to write.
+
+                All contents are byte strings.
 
             config (dict, optional):
                 Additional configuration to set for the render.
 
-        Returns:
+            builder_name (unicode, optional):
+                The name of the builder to use.
+
+        Context:
             unicode:
-            The rendered content.
         """
-        if builder_name == 'html':
-            out_filename = 'contents.html'
-        else:
-            raise ValueError('"%s" is not a supported builder name'
-                             % builder_name)
-
         with self.with_sphinx_env(config=config,
                                   builder_name=builder_name) as ctx:
             srcdir = ctx['srcdir']
 
             old_cwd = os.getcwd()
             os.chdir(srcdir)
 
             try:
-                with open('contents.rst', 'w') as fp:
-                    fp.write(doc_content)
-
-                for path, contents in extra_files.items():
+                for path, contents in files.items():
                     dirname = os.path.dirname(path)
 
-                    if not os.path.exists(dirname):
+                    if dirname and not os.path.exists(dirname):
                         os.makedirs(dirname)
 
-                    with open(path, 'wb') as fp:
-                        fp.write(contents)
+                    if isinstance(contents, bytes):
+                        with open(path, 'wb') as fp:
+                            fp.write(contents)
+                    else:
+                        assert isinstance(contents, six.text_type)
+
+                        with open(path, 'w') as fp:
+                            fp.write(contents)
 
                 app = ctx['app']
                 app.build()
 
-                with open(app.outdir / out_filename, 'r') as fp:
-                    return fp.read().strip()
+                yield str(app.outdir)
             finally:
                 os.chdir(old_cwd)
+
+    def render_doc(
+        self,
+        doc_content: str,
+        config={},
+        builder_name='html',
+        extra_files={}
+    ):  # type: (...) -> str
+        """Render a ReST document to a string.
+
+        This will set up a Sphinx environment, based on the extensions and
+        configuration provided by the consumer, and perform a render of the
+        given ReST content. The resulting string will be a rendered version
+        of just that content.
+
+        Args:
+            doc_content (unicode):
+                The ReST content to render.
+
+            config (dict, optional):
+                Additional configuration to set for the render.
+
+            builder_name (unicode, optional):
+                The name of the builder to use.
+
+            extra_files (dict):
+                A mapping of extra filenames and contents to write.
+
+        Returns:
+            unicode:
+            The rendered content.
+
+        Raises:
+            ValueError:
+                ``builder_name`` wasn't a valid value.
+        """
+        if builder_name == 'html':
+            out_filename = 'contents.html'
+        elif builder_name == 'json':
+            out_filename = 'contents.fjson'
+        else:
+            raise ValueError('"%s" is not a supported builder name'
+                             % builder_name)
+
+        files = {
+            'contents.rst': doc_content,
+        }
+        files.update(extra_files)
+
+        with self.rendered_docs(files=files,
+                                config=config,
+                                builder_name=builder_name) as build_dir:
+            with open(os.path.join(build_dir, out_filename), 'r') as fp:
+                return fp.read().strip()
```

### Comparing `beanbag-docutils-2.1.1/beanbag_docutils.egg-info/PKG-INFO` & `beanbag-docutils-2.2/beanbag_docutils.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 Metadata-Version: 2.1
 Name: beanbag-docutils
-Version: 2.1.1
+Version: 2.2
 Summary: Sphinx utility modules for Beanbag's documentation format.
 Home-page: https://github.com/beanbaginc/beanbag-docutils
 Maintainer: Christian Hammond
 Maintainer-email: christian@beanbaginc.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Other Environment
+Classifier: Framework :: Sphinx
+Classifier: Framework :: Sphinx :: Extension
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Documentation
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 License-File: COPYING
@@ -43,18 +46,52 @@
 
 .. _Review Board: https://www.reviewboard.org/
 .. _RBCommons: https://www.rbcommons.com/
 .. _Djblets: https://github.com/djblets/djblets/
 .. _RBTools: https://github.com/reviewboard/rbtools/
 
 
+Sphinx Extensions
+=================
+
+Most of the utilities are used with the Sphinx_ documentation system. Amongst
+other enhancements, this package offers:
+
+* A parser for the `Beanbag docstring format`_ (a variation on the `Google
+  docstring format`_), which we use for Python and JavaScript documentation
+* Enhancements for Sphinx's intersphinx_ system to provide per-page
+  intersphinx resolution options (useful for pages, such as release notes,
+  that need to link to different versions of the same docs, such as Django_ or
+  Python)
+* Enhancements to ReStructuredText references to let a reference name span
+  lines (useful for long Python/JavaScript module/class names)
+* Linking code references to GitHub documentation
+* High-DPI image embedding
+* A role for HTTP status codes
+* Access to document-defined metadata in a structured form when parsing
+  documents
+
+
+.. _Beanbag docstring format:
+   https://www.notion.so/reviewboard/Standard-Documentation-Format-4388f594d86547cc949b365cda3cf391
+.. _Django: https://www.djangoproject.com/
+.. _Google docstring format:
+   https://google.github.io/styleguide/pyguide.html#s3.8-comments-and-docstrings
+.. _intersphinx:
+   https://www.sphinx-doc.org/en/master/usage/extensions/intersphinx.html
+.. _our products: https://www.beanbaginc.com/
+.. _ReStructuredText:
+   https://docutils.sourceforge.io/docs/ref/rst/restructuredtext.html
+.. _Sphinx: https://www.sphinx-doc.org/
+
+
 Compatibility
 =============
 
-* beanbag-docutils 2.x supports Python 3.6-3.11.
+* beanbag-docutils 2.x supports Python 3.6-3.12 and Sphinx 1.8-7.x.
 * beanbag-docutils 1.x supports Python 2.7 and 3.6-3.10.
 
 
 Getting Started
 ===============
 
 To install the package, run:
```

### Comparing `beanbag-docutils-2.1.1/beanbag_docutils.egg-info/SOURCES.txt` & `beanbag-docutils-2.2/beanbag_docutils.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,20 +15,24 @@
 beanbag_docutils/sphinx/ext/collect_files.py
 beanbag_docutils/sphinx/ext/django_utils.py
 beanbag_docutils/sphinx/ext/extlinks.py
 beanbag_docutils/sphinx/ext/github.py
 beanbag_docutils/sphinx/ext/http_role.py
 beanbag_docutils/sphinx/ext/image_srcsets.py
 beanbag_docutils/sphinx/ext/intersphinx_utils.py
+beanbag_docutils/sphinx/ext/json_writer.py
+beanbag_docutils/sphinx/ext/metadata.py
 beanbag_docutils/sphinx/ext/ref_utils.py
 beanbag_docutils/sphinx/ext/retina_images.py
 beanbag_docutils/sphinx/ext/tests/__init__.py
 beanbag_docutils/sphinx/ext/tests/test_autodoc_utils.py
 beanbag_docutils/sphinx/ext/tests/test_django_utils.py
 beanbag_docutils/sphinx/ext/tests/test_extlinks.py
 beanbag_docutils/sphinx/ext/tests/test_github.py
 beanbag_docutils/sphinx/ext/tests/test_http_role.py
 beanbag_docutils/sphinx/ext/tests/test_image_srcsets.py
+beanbag_docutils/sphinx/ext/tests/test_json_writer.py
+beanbag_docutils/sphinx/ext/tests/test_metadata.py
 beanbag_docutils/sphinx/ext/tests/test_ref_utils.py
 beanbag_docutils/sphinx/ext/tests/testcase.py
 beanbag_docutils/sphinx/ext/tests/testdata/__init__.py
 beanbag_docutils/sphinx/ext/tests/testdata/github_linkcode_module.py
```

### Comparing `beanbag-docutils-2.1.1/setup.py` & `beanbag-docutils-2.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,31 +19,35 @@
     description="Sphinx utility modules for Beanbag's documentation format.",
     long_description=readme,
     url='https://github.com/beanbaginc/beanbag-docutils',
     maintainer='Christian Hammond',
     maintainer_email='christian@beanbaginc.com',
     packages=find_packages(),
     install_requires=[
-        'Sphinx',
+        'Sphinx>=1.8,<=7.999',
+        'sphinxcontrib-serializinghtml',
     ],
     python_requires='>=3.6',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Other Environment',
+        'Framework :: Sphinx',
+        'Framework :: Sphinx :: Extension',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Topic :: Documentation',
         'Topic :: Documentation :: Sphinx',
         'Topic :: Software Development',
         'Topic :: Software Development :: Documentation',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ]
 )
```

