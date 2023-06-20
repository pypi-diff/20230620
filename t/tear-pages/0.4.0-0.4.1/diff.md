# Comparing `tmp/tear-pages-0.4.0.tar.gz` & `tmp/tear-pages-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tear-pages-0.4.0.tar", last modified: Wed Dec 11 08:14:39 2019, max compression
+gzip compressed data, was "tear-pages-0.4.1.tar", last modified: Tue Jun 20 05:12:54 2023, max compression
```

## Comparing `tear-pages-0.4.0.tar` & `tear-pages-0.4.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxr-xr-x   0 fr        (1000) fr        (1000)        0 2019-12-11 08:14:39.000000 tear-pages-0.4.0/
--rw-r--r--   0 fr        (1000) fr        (1000)    35131 2018-10-18 09:47:29.000000 tear-pages-0.4.0/LICENSE
--rw-r--r--   0 fr        (1000) fr        (1000)      272 2019-12-11 08:14:39.000000 tear-pages-0.4.0/PKG-INFO
--rw-r--r--   0 fr        (1000) fr        (1000)      776 2018-10-18 09:47:29.000000 tear-pages-0.4.0/README.md
--rw-r--r--   0 fr        (1000) fr        (1000)       15 2018-10-18 09:47:29.000000 tear-pages-0.4.0/requirements.txt
--rw-r--r--   0 fr        (1000) fr        (1000)      481 2018-10-18 09:47:29.000000 tear-pages-0.4.0/setup.py
--rwxr-xr-x   0 fr        (1000) fr        (1000)     3056 2019-12-11 08:09:41.000000 tear-pages-0.4.0/tearpages.py
+drwxr-xr-x   0 fr        (1000) fr        (1000)        0 2023-06-20 05:12:54.201698 tear-pages-0.4.1/
+-rw-r--r--   0 fr        (1000) fr        (1000)    35131 2022-10-13 08:27:22.000000 tear-pages-0.4.1/LICENSE
+-rw-r--r--   0 fr        (1000) fr        (1000)       54 2022-10-13 08:27:22.000000 tear-pages-0.4.1/MANIFEST.in
+-rw-r--r--   0 fr        (1000) fr        (1000)      255 2023-06-20 05:12:54.201698 tear-pages-0.4.1/PKG-INFO
+-rw-r--r--   0 fr        (1000) fr        (1000)      776 2022-10-13 08:27:22.000000 tear-pages-0.4.1/README.md
+-rw-r--r--   0 fr        (1000) fr        (1000)       14 2023-06-20 05:10:36.000000 tear-pages-0.4.1/requirements.txt
+-rw-r--r--   0 fr        (1000) fr        (1000)       38 2023-06-20 05:12:54.201698 tear-pages-0.4.1/setup.cfg
+-rw-r--r--   0 fr        (1000) fr        (1000)      481 2022-10-13 08:27:22.000000 tear-pages-0.4.1/setup.py
+drwxr-xr-x   0 fr        (1000) fr        (1000)        0 2023-06-20 05:12:54.201698 tear-pages-0.4.1/tear_pages.egg-info/
+-rw-r--r--   0 fr        (1000) fr        (1000)      255 2023-06-20 05:12:54.000000 tear-pages-0.4.1/tear_pages.egg-info/PKG-INFO
+-rw-r--r--   0 fr        (1000) fr        (1000)      237 2023-06-20 05:12:54.000000 tear-pages-0.4.1/tear_pages.egg-info/SOURCES.txt
+-rw-r--r--   0 fr        (1000) fr        (1000)        1 2023-06-20 05:12:54.000000 tear-pages-0.4.1/tear_pages.egg-info/dependency_links.txt
+-rw-r--r--   0 fr        (1000) fr        (1000)       15 2023-06-20 05:12:54.000000 tear-pages-0.4.1/tear_pages.egg-info/requires.txt
+-rw-r--r--   0 fr        (1000) fr        (1000)       10 2023-06-20 05:12:54.000000 tear-pages-0.4.1/tear_pages.egg-info/top_level.txt
+-rwxr-xr-x   0 fr        (1000) fr        (1000)     3057 2023-06-20 05:10:36.000000 tear-pages-0.4.1/tearpages.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tear-pages-0.4.0/LICENSE` & `tear-pages-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tear-pages-0.4.0/README.md` & `tear-pages-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `tear-pages-0.4.0/tearpages.py` & `tear-pages-0.4.1/tearpages.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 # License: GPLv3
 
 import argparse
 import logging
 import shutil
 import tempfile
 from PyPDF2 import PdfFileWriter, PdfFileReader
-from PyPDF2.utils import PdfReadError
+from PyPDF2.errors import PdfReadError
 
-__version__ = '0.4.0'
+__version__ = '0.4.1'
 
 
 def fixPdf(pdfFile, destination):
     """
     Fix malformed pdf files when data are present after '%%EOF'
 
     :param pdfFile: PDF filepath
```

