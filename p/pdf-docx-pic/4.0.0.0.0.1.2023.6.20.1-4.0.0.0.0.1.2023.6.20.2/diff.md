# Comparing `tmp/pdf_docx_pic-4.0.0.0.0.1.2023.6.20.1.tar.gz` & `tmp/pdf_docx_pic-4.0.0.0.0.1.2023.6.20.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdf_docx_pic-4.0.0.0.0.1.2023.6.20.1.tar", last modified: Tue Jun 20 07:37:21 2023, max compression
+gzip compressed data, was "pdf_docx_pic-4.0.0.0.0.1.2023.6.20.2.tar", last modified: Tue Jun 20 07:40:27 2023, max compression
```

## Comparing `pdf_docx_pic-4.0.0.0.0.1.2023.6.20.1.tar` & `pdf_docx_pic-4.0.0.0.0.1.2023.6.20.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 07:37:21.957773 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.1/
--rw-rw-rw-   0        0        0     1469 2023-06-20 07:37:21.957773 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.1/PKG-INFO
--rw-rw-rw-   0        0        0      416 2023-06-19 09:02:11.000000 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-20 07:37:21.942118 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.1/pdf-docx-pic/
--rw-rw-rw-   0        0        0        0 2023-06-17 02:49:27.000000 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.1/pdf-docx-pic/__init__.py
--rw-rw-rw-   0        0        0     6432 2023-06-17 02:22:45.000000 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.1/pdf-docx-pic/main.py
-drwxrwxrwx   0        0        0        0 2023-06-20 07:37:21.957773 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.1/pdf_docx_pic.egg-info/
--rw-rw-rw-   0        0        0     1469 2023-06-20 07:37:21.000000 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.1/pdf_docx_pic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-06-20 07:37:21.000000 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.1/pdf_docx_pic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 07:37:21.000000 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.1/pdf_docx_pic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      135 2023-06-20 07:37:21.000000 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.1/pdf_docx_pic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-20 07:37:21.000000 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.1/pdf_docx_pic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-20 07:37:21.957773 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.1/setup.cfg
--rw-rw-rw-   0        0        0     1814 2023-06-20 07:37:05.000000 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 07:40:27.845877 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.2/
+-rw-rw-rw-   0        0        0     1871 2023-06-20 07:40:27.845877 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.2/PKG-INFO
+-rw-rw-rw-   0        0        0      416 2023-06-19 09:02:11.000000 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-20 07:40:27.830241 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.2/pdf-docx-pic/
+-rw-rw-rw-   0        0        0        0 2023-06-17 02:49:27.000000 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.2/pdf-docx-pic/__init__.py
+-rw-rw-rw-   0        0        0     6432 2023-06-17 02:22:45.000000 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.2/pdf-docx-pic/main.py
+drwxrwxrwx   0        0        0        0 2023-06-20 07:40:27.845877 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.2/pdf_docx_pic.egg-info/
+-rw-rw-rw-   0        0        0     1871 2023-06-20 07:40:27.000000 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.2/pdf_docx_pic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-06-20 07:40:27.000000 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.2/pdf_docx_pic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 07:40:27.000000 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.2/pdf_docx_pic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      135 2023-06-20 07:40:27.000000 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.2/pdf_docx_pic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-20 07:40:27.000000 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.2/pdf_docx_pic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 07:40:27.845877 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.2/setup.cfg
+-rw-rw-rw-   0        0        0     1866 2023-06-20 07:40:14.000000 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.2/setup.py
```

### Comparing `pdf_docx_pic-4.0.0.0.0.1.2023.6.20.1/pdf-docx-pic/main.py` & `pdf_docx_pic-4.0.0.0.0.1.2023.6.20.2/pdf-docx-pic/main.py`

 * *Files identical despite different names*

### Comparing `pdf_docx_pic-4.0.0.0.0.1.2023.6.20.1/setup.py` & `pdf_docx_pic-4.0.0.0.0.1.2023.6.20.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from setuptools import *
 
+a = open(".\\README.rst", mode='r', encoding = 'UTF-8').read()
+
 setup(
     name = "pdf_docx_pic",
-    version = "4.0.0.0.0.1.2023.6.20.1",
+    version = "4.0.0.0.0.1.2023.6.20.2",
     packages = find_packages(),
     classifiers = [
         "Development Status :: 4 - Beta",
         "Development Status :: 5 - Production/Stable",
         "Environment :: GPU",
         "Framework :: Jupyter :: JupyterLab :: 4",
         "Framework :: Django :: 4.2",
@@ -34,9 +36,9 @@
         "ttkbootstrap>=1.10.1, <1.11",
         "pdf2docx>=0.5.5, <0.6.0", 
         "docx2pdf>=0.1.8, <0.2.0", 
         "PyMuPDF>=1.22.1, <1.23", 
         "Pillow>=9.5.0, <10.0", 
         "wheel>=0.38.2, <0.41",
     ],
-    long_description = ".\\README.rst"
+    long_description = a
 )
```

