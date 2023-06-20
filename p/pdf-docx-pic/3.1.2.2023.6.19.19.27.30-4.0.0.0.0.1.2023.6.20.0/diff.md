# Comparing `tmp/pdf-docx-pic-3.1.2.2023.6.19.19.27.30.tar.gz` & `tmp/pdf_docx_pic-4.0.0.0.0.1.2023.6.20.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdf-docx-pic-3.1.2.2023.6.19.19.27.30.tar", last modified: Mon Jun 19 11:33:02 2023, max compression
+gzip compressed data, was "pdf_docx_pic-4.0.0.0.0.1.2023.6.20.0.tar", last modified: Tue Jun 20 07:33:40 2023, max compression
```

## Comparing `pdf-docx-pic-3.1.2.2023.6.19.19.27.30.tar` & `pdf_docx_pic-4.0.0.0.0.1.2023.6.20.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 11:33:02.445795 pdf-docx-pic-3.1.2.2023.6.19.19.27.30/
--rw-rw-rw-   0        0        0     1330 2023-06-19 11:33:02.444795 pdf-docx-pic-3.1.2.2023.6.19.19.27.30/PKG-INFO
--rw-rw-rw-   0        0        0      416 2023-06-19 09:02:11.000000 pdf-docx-pic-3.1.2.2023.6.19.19.27.30/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-19 11:33:02.434592 pdf-docx-pic-3.1.2.2023.6.19.19.27.30/pdf-docx-pic/
--rw-rw-rw-   0        0        0        0 2023-06-17 02:49:27.000000 pdf-docx-pic-3.1.2.2023.6.19.19.27.30/pdf-docx-pic/__init__.py
--rw-rw-rw-   0        0        0     6432 2023-06-17 02:22:45.000000 pdf-docx-pic-3.1.2.2023.6.19.19.27.30/pdf-docx-pic/main.py
-drwxrwxrwx   0        0        0        0 2023-06-19 11:33:02.442794 pdf-docx-pic-3.1.2.2023.6.19.19.27.30/pdf_docx_pic.egg-info/
--rw-rw-rw-   0        0        0     1330 2023-06-19 11:33:02.000000 pdf-docx-pic-3.1.2.2023.6.19.19.27.30/pdf_docx_pic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-06-19 11:33:02.000000 pdf-docx-pic-3.1.2.2023.6.19.19.27.30/pdf_docx_pic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 11:33:02.000000 pdf-docx-pic-3.1.2.2023.6.19.19.27.30/pdf_docx_pic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      128 2023-06-19 11:33:02.000000 pdf-docx-pic-3.1.2.2023.6.19.19.27.30/pdf_docx_pic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-19 11:33:02.000000 pdf-docx-pic-3.1.2.2023.6.19.19.27.30/pdf_docx_pic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 11:33:02.445795 pdf-docx-pic-3.1.2.2023.6.19.19.27.30/setup.cfg
--rw-rw-rw-   0        0        0     1644 2023-06-19 11:27:48.000000 pdf-docx-pic-3.1.2.2023.6.19.19.27.30/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 07:33:40.015903 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.0/
+-rw-rw-rw-   0        0        0     1453 2023-06-20 07:33:40.015903 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.0/PKG-INFO
+-rw-rw-rw-   0        0        0      416 2023-06-19 09:02:11.000000 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-20 07:33:40.000256 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.0/pdf-docx-pic/
+-rw-rw-rw-   0        0        0        0 2023-06-17 02:49:27.000000 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.0/pdf-docx-pic/__init__.py
+-rw-rw-rw-   0        0        0     6432 2023-06-17 02:22:45.000000 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.0/pdf-docx-pic/main.py
+drwxrwxrwx   0        0        0        0 2023-06-20 07:33:40.015903 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.0/pdf_docx_pic.egg-info/
+-rw-rw-rw-   0        0        0     1453 2023-06-20 07:33:39.000000 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.0/pdf_docx_pic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-06-20 07:33:39.000000 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.0/pdf_docx_pic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 07:33:39.000000 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.0/pdf_docx_pic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      135 2023-06-20 07:33:39.000000 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.0/pdf_docx_pic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-20 07:33:39.000000 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.0/pdf_docx_pic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 07:33:40.015903 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.0/setup.cfg
+-rw-rw-rw-   0        0        0     1773 2023-06-20 07:33:07.000000 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.0/setup.py
```

### Comparing `pdf-docx-pic-3.1.2.2023.6.19.19.27.30/PKG-INFO` & `pdf_docx_pic-4.0.0.0.0.1.2023.6.20.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
-Name: pdf-docx-pic
-Version: 3.1.2.2023.6.19.19.27.30
+Name: pdf_docx_pic
+Version: 4.0.0.0.0.1.2023.6.20.0
+Classifier: Development Status :: 4 - Beta
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: GPU
 Classifier: Framework :: Jupyter :: JupyterLab :: 4
 Classifier: Framework :: Django :: 4.2
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows :: Windows 7
+Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Mime Renderers
 Classifier: Operating System :: Microsoft :: Windows :: Windows 8
 Classifier: Operating System :: Microsoft :: Windows :: Windows 8.1
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: Operating System :: POSIX
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Programming Language :: Python :: 2.6
```

### Comparing `pdf-docx-pic-3.1.2.2023.6.19.19.27.30/pdf-docx-pic/main.py` & `pdf_docx_pic-4.0.0.0.0.1.2023.6.20.0/pdf-docx-pic/main.py`

 * *Files identical despite different names*

### Comparing `pdf-docx-pic-3.1.2.2023.6.19.19.27.30/pdf_docx_pic.egg-info/PKG-INFO` & `pdf_docx_pic-4.0.0.0.0.1.2023.6.20.0/pdf_docx_pic.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: pdf-docx-pic
-Version: 3.1.2.2023.6.19.19.27.30
+Version: 4.0.0.0.0.1.2023.6.20.0
+Classifier: Development Status :: 4 - Beta
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: GPU
 Classifier: Framework :: Jupyter :: JupyterLab :: 4
 Classifier: Framework :: Django :: 4.2
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows :: Windows 7
+Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Mime Renderers
 Classifier: Operating System :: Microsoft :: Windows :: Windows 8
 Classifier: Operating System :: Microsoft :: Windows :: Windows 8.1
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: Operating System :: POSIX
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Programming Language :: Python :: 2.6
```

### Comparing `pdf-docx-pic-3.1.2.2023.6.19.19.27.30/setup.py` & `pdf_docx_pic-4.0.0.0.0.1.2023.6.20.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from setuptools import *
 
 setup(
-    name = "pdf-docx-pic",
-    version = "3.1.2.2023.6.19.19.27.30",
+    name = "pdf_docx_pic",
+    version = "4.0.0.0.0.1.2023.6.20.0",
     packages = find_packages(),
     classifiers = [
+        "Development Status :: 4 - Beta",
         "Development Status :: 5 - Production/Stable",
         "Environment :: GPU",
         "Framework :: Jupyter :: JupyterLab :: 4",
         "Framework :: Django :: 4.2",
         "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
         "License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows :: Windows 7",
+        "Framework :: Jupyter :: JupyterLab :: Extensions :: Mime Renderers",
         "Operating System :: Microsoft :: Windows :: Windows 8",
         "Operating System :: Microsoft :: Windows :: Windows 8.1",
         "Operating System :: Microsoft :: Windows :: Windows 10",
         "Operating System :: Microsoft :: Windows :: Windows 11",
         "Operating System :: POSIX",
         "Natural Language :: Chinese (Simplified)",
         "Programming Language :: Python :: 2.6",
@@ -25,15 +27,15 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
     ],
     install_requires = [
-        "ttkbootstrap>=1.10, <1.11",
-        "pdf2docx!=0.5.4, >=0.5.2", 
-        "docx2pdf>=0.1.8", 
-        "PyMuPDF>=1.22.1", 
-        "Pillow>=9.3.0, <10.0", 
-        "wheel!=0.38.2, >=0.38, <0.41",
+        "ttkbootstrap>=1.10.1, <1.11",
+        "pdf2docx>=0.5.5, <0.6.0", 
+        "docx2pdf>=0.1.8, <0.2.0", 
+        "PyMuPDF>=1.22.1, <1.23", 
+        "Pillow>=9.5.0, <10.0", 
+        "wheel>=0.38.2, <0.41",
     ]
 )
```

