# Comparing `tmp/vbpdf-0.1.8.tar.gz` & `tmp/vbpdf-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbpdf-0.1.8.tar", max compression
+gzip compressed data, was "vbpdf-0.1.9.tar", max compression
```

## Comparing `vbpdf-0.1.8.tar` & `vbpdf-0.1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     2364 2023-03-18 17:28:09.929910 vbpdf-0.1.8/README.md
--rw-r--r--   0        0        0      556 2023-03-28 11:32:54.817272 vbpdf-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-18 03:58:18.949908 vbpdf-0.1.8/vbpdf/__init__.py
--rw-r--r--   0        0        0       47 2023-03-18 03:59:34.812782 vbpdf-0.1.8/vbpdf/__main__.py
--rw-r--r--   0        0        0     1384 2023-03-22 17:37:56.479143 vbpdf-0.1.8/vbpdf/addbg.py
--rw-r--r--   0        0        0     1335 2023-03-28 06:42:24.480344 vbpdf-0.1.8/vbpdf/blur.py
--rw-r--r--   0        0        0     2044 2023-03-18 12:48:37.740668 vbpdf-0.1.8/vbpdf/functions_pdf.py
--rw-r--r--   0        0        0     1562 2023-03-28 11:30:53.119572 vbpdf-0.1.8/vbpdf/instagram.py
--rw-r--r--   0        0        0      517 2023-03-28 11:32:42.893420 vbpdf-0.1.8/vbpdf/main.py
--rw-r--r--   0        0        0     2827 2023-03-18 05:38:17.629570 vbpdf-0.1.8/vbpdf/overlay.py
--rw-r--r--   0        0        0      971 2023-03-18 11:01:19.443240 vbpdf-0.1.8/vbpdf/split.py
--rw-r--r--   0        0        0     1622 2023-03-28 06:42:34.145004 vbpdf-0.1.8/vbpdf/stack.py
--rw-r--r--   0        0        0     2085 2023-03-18 12:50:12.452825 vbpdf-0.1.8/vbpdf/topng.py
--rw-r--r--   0        0        0     2902 1970-01-01 00:00:00.000000 vbpdf-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     2364 2023-03-18 17:28:09.929910 vbpdf-0.1.9/README.md
+-rw-r--r--   0        0        0      556 2023-03-28 11:34:23.028601 vbpdf-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-18 03:58:18.949908 vbpdf-0.1.9/vbpdf/__init__.py
+-rw-r--r--   0        0        0       47 2023-03-18 03:59:34.812782 vbpdf-0.1.9/vbpdf/__main__.py
+-rw-r--r--   0        0        0     1384 2023-03-22 17:37:56.479143 vbpdf-0.1.9/vbpdf/addbg.py
+-rw-r--r--   0        0        0     1335 2023-03-28 06:42:24.480344 vbpdf-0.1.9/vbpdf/blur.py
+-rw-r--r--   0        0        0     2044 2023-03-18 12:48:37.740668 vbpdf-0.1.9/vbpdf/functions_pdf.py
+-rw-r--r--   0        0        0     1586 2023-03-28 11:34:15.242860 vbpdf-0.1.9/vbpdf/instagram.py
+-rw-r--r--   0        0        0      517 2023-03-28 11:32:42.893420 vbpdf-0.1.9/vbpdf/main.py
+-rw-r--r--   0        0        0     2827 2023-03-18 05:38:17.629570 vbpdf-0.1.9/vbpdf/overlay.py
+-rw-r--r--   0        0        0      971 2023-03-18 11:01:19.443240 vbpdf-0.1.9/vbpdf/split.py
+-rw-r--r--   0        0        0     1622 2023-03-28 06:42:34.145004 vbpdf-0.1.9/vbpdf/stack.py
+-rw-r--r--   0        0        0     2085 2023-03-18 12:50:12.452825 vbpdf-0.1.9/vbpdf/topng.py
+-rw-r--r--   0        0        0     2902 1970-01-01 00:00:00.000000 vbpdf-0.1.9/PKG-INFO
```

### Comparing `vbpdf-0.1.8/README.md` & `vbpdf-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `vbpdf-0.1.8/pyproject.toml` & `vbpdf-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vbpdf"
-version = "0.1.8"
+version = "0.1.9"
 description = "Added addbg for adding background image to png."
 authors = ["vaibhavblayer <vaibhavblayer@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/vaibhavblayer/vbpdf"
 repository = "https://github.com/vaibhavblayer/vbpdf"
 keywords = ["split pdf", "annotate pdf", "pdftopng", "png", "pdf"]
```

### Comparing `vbpdf-0.1.8/vbpdf/addbg.py` & `vbpdf-0.1.9/vbpdf/addbg.py`

 * *Files identical despite different names*

### Comparing `vbpdf-0.1.8/vbpdf/blur.py` & `vbpdf-0.1.9/vbpdf/blur.py`

 * *Files identical despite different names*

### Comparing `vbpdf-0.1.8/vbpdf/functions_pdf.py` & `vbpdf-0.1.9/vbpdf/functions_pdf.py`

 * *Files identical despite different names*

### Comparing `vbpdf-0.1.8/vbpdf/instagram.py` & `vbpdf-0.1.9/vbpdf/instagram.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import PyPDF2
 import time
 from rich.console import Console
 from .functions_pdf import pages_pdf
 from .functions_pdf import extract_png_pdf
 from .blur import blur
 from .stack import stack
-
+from .topng import topng
 
 
 @click.command(
         help="Converts pdf pages into pngs"
         )
 @click.option(
         '-i',
```

### Comparing `vbpdf-0.1.8/vbpdf/main.py` & `vbpdf-0.1.9/vbpdf/main.py`

 * *Files identical despite different names*

### Comparing `vbpdf-0.1.8/vbpdf/overlay.py` & `vbpdf-0.1.9/vbpdf/overlay.py`

 * *Files identical despite different names*

### Comparing `vbpdf-0.1.8/vbpdf/split.py` & `vbpdf-0.1.9/vbpdf/split.py`

 * *Files identical despite different names*

### Comparing `vbpdf-0.1.8/vbpdf/stack.py` & `vbpdf-0.1.9/vbpdf/stack.py`

 * *Files identical despite different names*

### Comparing `vbpdf-0.1.8/vbpdf/topng.py` & `vbpdf-0.1.9/vbpdf/topng.py`

 * *Files identical despite different names*

### Comparing `vbpdf-0.1.8/PKG-INFO` & `vbpdf-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vbpdf
-Version: 0.1.8
+Version: 0.1.9
 Summary: Added addbg for adding background image to png.
 Home-page: https://github.com/vaibhavblayer/vbpdf
 Keywords: split pdf,annotate pdf,pdftopng,png,pdf
 Author: vaibhavblayer
 Author-email: vaibhavblayer@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
```

