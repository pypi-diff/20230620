# Comparing `tmp/pdf_docx_pic-4.0.0.0.0.1.2023.6.20.0.tar.gz` & `tmp/pdf_docx_pic-4.0.0.0.0.1.2023.6.20.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdf_docx_pic-4.0.0.0.0.1.2023.6.20.0.tar", last modified: Tue Jun 20 07:33:40 2023, max compression
+gzip compressed data, was "pdf_docx_pic-4.0.0.0.0.1.2023.6.20.1.tar", last modified: Tue Jun 20 07:37:21 2023, max compression
```

## Comparing `pdf_docx_pic-4.0.0.0.0.1.2023.6.20.0.tar` & `pdf_docx_pic-4.0.0.0.0.1.2023.6.20.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 07:33:40.015903 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.0/
--rw-rw-rw-   0        0        0     1453 2023-06-20 07:33:40.015903 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.0/PKG-INFO
--rw-rw-rw-   0        0        0      416 2023-06-19 09:02:11.000000 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-20 07:33:40.000256 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.0/pdf-docx-pic/
--rw-rw-rw-   0        0        0        0 2023-06-17 02:49:27.000000 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.0/pdf-docx-pic/__init__.py
--rw-rw-rw-   0        0        0     6432 2023-06-17 02:22:45.000000 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.0/pdf-docx-pic/main.py
-drwxrwxrwx   0        0        0        0 2023-06-20 07:33:40.015903 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.0/pdf_docx_pic.egg-info/
--rw-rw-rw-   0        0        0     1453 2023-06-20 07:33:39.000000 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.0/pdf_docx_pic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-06-20 07:33:39.000000 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.0/pdf_docx_pic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 07:33:39.000000 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.0/pdf_docx_pic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      135 2023-06-20 07:33:39.000000 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.0/pdf_docx_pic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-20 07:33:39.000000 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.0/pdf_docx_pic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-20 07:33:40.015903 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.0/setup.cfg
--rw-rw-rw-   0        0        0     1773 2023-06-20 07:33:07.000000 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 07:37:21.957773 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.1/
+-rw-rw-rw-   0        0        0     1469 2023-06-20 07:37:21.957773 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.1/PKG-INFO
+-rw-rw-rw-   0        0        0      416 2023-06-19 09:02:11.000000 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-20 07:37:21.942118 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.1/pdf-docx-pic/
+-rw-rw-rw-   0        0        0        0 2023-06-17 02:49:27.000000 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.1/pdf-docx-pic/__init__.py
+-rw-rw-rw-   0        0        0     6432 2023-06-17 02:22:45.000000 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.1/pdf-docx-pic/main.py
+drwxrwxrwx   0        0        0        0 2023-06-20 07:37:21.957773 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.1/pdf_docx_pic.egg-info/
+-rw-rw-rw-   0        0        0     1469 2023-06-20 07:37:21.000000 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.1/pdf_docx_pic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-06-20 07:37:21.000000 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.1/pdf_docx_pic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 07:37:21.000000 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.1/pdf_docx_pic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      135 2023-06-20 07:37:21.000000 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.1/pdf_docx_pic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-20 07:37:21.000000 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.1/pdf_docx_pic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 07:37:21.957773 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.1/setup.cfg
+-rw-rw-rw-   0        0        0     1814 2023-06-20 07:37:05.000000 pdf_docx_pic-4.0.0.0.0.1.2023.6.20.1/setup.py
```

### Comparing `pdf_docx_pic-4.0.0.0.0.1.2023.6.20.0/PKG-INFO` & `pdf_docx_pic-4.0.0.0.0.1.2023.6.20.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdf_docx_pic
-Version: 4.0.0.0.0.1.2023.6.20.0
+Version: 4.0.0.0.0.1.2023.6.20.1
 Classifier: Development Status :: 4 - Beta
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: GPU
 Classifier: Framework :: Jupyter :: JupyterLab :: 4
 Classifier: Framework :: Django :: 4.2
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)
@@ -21,7 +21,9 @@
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
+
+.\README.rst
```

### Comparing `pdf_docx_pic-4.0.0.0.0.1.2023.6.20.0/pdf-docx-pic/main.py` & `pdf_docx_pic-4.0.0.0.0.1.2023.6.20.1/pdf-docx-pic/main.py`

 * *Files identical despite different names*

### Comparing `pdf_docx_pic-4.0.0.0.0.1.2023.6.20.0/pdf_docx_pic.egg-info/PKG-INFO` & `pdf_docx_pic-4.0.0.0.0.1.2023.6.20.1/pdf_docx_pic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdf-docx-pic
-Version: 4.0.0.0.0.1.2023.6.20.0
+Version: 4.0.0.0.0.1.2023.6.20.1
 Classifier: Development Status :: 4 - Beta
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: GPU
 Classifier: Framework :: Jupyter :: JupyterLab :: 4
 Classifier: Framework :: Django :: 4.2
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)
@@ -21,7 +21,9 @@
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
+
+.\README.rst
```

### Comparing `pdf_docx_pic-4.0.0.0.0.1.2023.6.20.0/setup.py` & `pdf_docx_pic-4.0.0.0.0.1.2023.6.20.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import *
 
 setup(
     name = "pdf_docx_pic",
-    version = "4.0.0.0.0.1.2023.6.20.0",
+    version = "4.0.0.0.0.1.2023.6.20.1",
     packages = find_packages(),
     classifiers = [
         "Development Status :: 4 - Beta",
         "Development Status :: 5 - Production/Stable",
         "Environment :: GPU",
         "Framework :: Jupyter :: JupyterLab :: 4",
         "Framework :: Django :: 4.2",
@@ -33,9 +33,10 @@
     install_requires = [
         "ttkbootstrap>=1.10.1, <1.11",
         "pdf2docx>=0.5.5, <0.6.0", 
         "docx2pdf>=0.1.8, <0.2.0", 
         "PyMuPDF>=1.22.1, <1.23", 
         "Pillow>=9.5.0, <10.0", 
         "wheel>=0.38.2, <0.41",
-    ]
+    ],
+    long_description = ".\\README.rst"
 )
```

