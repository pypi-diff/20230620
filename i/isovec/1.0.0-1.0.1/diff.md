# Comparing `tmp/isovec-1.0.0.tar.gz` & `tmp/isovec-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isovec-1.0.0.tar", last modified: Wed Jun 14 20:39:55 2023, max compression
+gzip compressed data, was "isovec-1.0.1.tar", last modified: Tue Jun 20 11:52:44 2023, max compression
```

## Comparing `isovec-1.0.0.tar` & `isovec-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 20:39:55.579680 isovec-1.0.0/
--rw-rw-rw-   0        0        0     1088 2023-02-25 12:24:32.000000 isovec-1.0.0/LICENSE
--rw-rw-rw-   0        0        0    10905 2023-06-14 20:39:55.575678 isovec-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     8943 2023-06-14 20:39:18.000000 isovec-1.0.0/README.md
--rw-rw-rw-   0        0        0      966 2023-06-14 20:38:05.000000 isovec-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-14 20:39:55.579680 isovec-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-14 20:39:55.485824 isovec-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-14 20:39:55.555680 isovec-1.0.0/src/isovec/
--rw-rw-rw-   0        0        0     6376 2023-06-14 14:05:45.000000 isovec-1.0.0/src/isovec/Element.py
--rw-rw-rw-   0        0        0     3255 2023-06-11 17:54:14.000000 isovec-1.0.0/src/isovec/Isotope.py
--rw-rw-rw-   0        0        0     3994 2023-06-11 18:01:58.000000 isovec-1.0.0/src/isovec/Mixture.py
--rw-rw-rw-   0        0        0     5100 2023-06-11 18:02:42.000000 isovec-1.0.0/src/isovec/Molecule.py
--rw-rw-rw-   0        0        0      219 2023-06-11 11:00:02.000000 isovec-1.0.0/src/isovec/__init__.py
--rw-rw-rw-   0        0        0     1527 2023-05-23 20:40:44.000000 isovec-1.0.0/src/isovec/conversion.py
--rw-rw-rw-   0        0        0    21330 2023-06-14 14:12:04.000000 isovec-1.0.0/src/isovec/elements.py
--rw-rw-rw-   0        0        0      173 2023-06-14 14:03:23.000000 isovec-1.0.0/src/isovec/exceptions.py
--rw-rw-rw-   0        0        0    21141 2023-05-23 19:45:40.000000 isovec-1.0.0/src/isovec/isotopes.py
--rw-rw-rw-   0        0        0      109 2023-05-23 19:42:08.000000 isovec-1.0.0/src/isovec/printer.py
-drwxrwxrwx   0        0        0        0 2023-06-14 20:39:55.571678 isovec-1.0.0/src/isovec.egg-info/
--rw-rw-rw-   0        0        0    10905 2023-06-14 20:39:55.000000 isovec-1.0.0/src/isovec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      398 2023-06-14 20:39:55.000000 isovec-1.0.0/src/isovec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 20:39:55.000000 isovec-1.0.0/src/isovec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-14 20:39:55.000000 isovec-1.0.0/src/isovec.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 11:52:44.038947 isovec-1.0.1/
+-rw-rw-rw-   0        0        0      473 2023-06-20 11:44:39.000000 isovec-1.0.1/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1088 2023-02-25 13:24:32.000000 isovec-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0       20 2023-06-20 11:39:46.000000 isovec-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    11118 2023-06-20 11:52:44.037952 isovec-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     9093 2023-06-20 11:51:58.000000 isovec-1.0.1/README.md
+-rw-rw-rw-   0        0        0     1024 2023-06-20 11:49:18.000000 isovec-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-20 11:52:44.039944 isovec-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-20 11:52:43.887050 isovec-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-20 11:52:44.012079 isovec-1.0.1/src/isovec/
+-rw-rw-rw-   0        0        0     6376 2023-06-14 14:05:46.000000 isovec-1.0.1/src/isovec/Element.py
+-rw-rw-rw-   0        0        0     3255 2023-06-11 17:54:14.000000 isovec-1.0.1/src/isovec/Isotope.py
+-rw-rw-rw-   0        0        0     3994 2023-06-11 18:01:58.000000 isovec-1.0.1/src/isovec/Mixture.py
+-rw-rw-rw-   0        0        0     5100 2023-06-11 18:02:42.000000 isovec-1.0.1/src/isovec/Molecule.py
+-rw-rw-rw-   0        0        0      206 2023-06-20 11:28:10.000000 isovec-1.0.1/src/isovec/__init__.py
+-rw-rw-rw-   0        0        0     2499 2023-06-20 11:31:29.000000 isovec-1.0.1/src/isovec/conversion.py
+-rw-rw-rw-   0        0        0    21330 2023-06-14 14:12:06.000000 isovec-1.0.1/src/isovec/elements.py
+-rw-rw-rw-   0        0        0      173 2023-06-14 14:03:24.000000 isovec-1.0.1/src/isovec/exceptions.py
+-rw-rw-rw-   0        0        0    21141 2023-05-23 19:45:40.000000 isovec-1.0.1/src/isovec/isotopes.py
+-rw-rw-rw-   0        0        0      109 2023-05-23 19:42:08.000000 isovec-1.0.1/src/isovec/printer.py
+drwxrwxrwx   0        0        0        0 2023-06-20 11:52:44.033276 isovec-1.0.1/src/isovec.egg-info/
+-rw-rw-rw-   0        0        0    11118 2023-06-20 11:52:43.000000 isovec-1.0.1/src/isovec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      423 2023-06-20 11:52:43.000000 isovec-1.0.1/src/isovec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 11:52:43.000000 isovec-1.0.1/src/isovec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-20 11:52:43.000000 isovec-1.0.1/src/isovec.egg-info/top_level.txt
```

### Comparing `isovec-1.0.0/LICENSE` & `isovec-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `isovec-1.0.0/PKG-INFO` & `isovec-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: isovec
-Version: 1.0.0
-Summary: A package to calculate isotopic composition of (custom) Elements, Molecules and Alloys.
+Version: 1.0.1
+Summary: A package to calculate isotopic composition of (custom) Elements, Molecules and Mixtures.
 Author-email: Julius Mercz <julius.mercz@tum.de>
 License: MIT License
         
         Copyright (c) 2023 Julius Mercz
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -20,15 +20,16 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
-Keywords: isotope,element,molecule,alloy,composition,weight,atomic
+Project-URL: PyPI, https://pypi.org/project/isovec/
+Keywords: isotope,element,molecule,mixture,alloy,composition,weight,atomic
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Typing :: Typed
@@ -238,10 +239,14 @@
   O-16: 2.0921E-01
   O-17: 7.9694E-05
   O-18: 4.2993E-04
    [...]
 ```
 
 
+## Changelog
+
+For a history of changes, refer to the file `CHANGELOG.md` in the source distribution available under "Navigation/Download files".
+
 ## References
 
 1. Coursey, J.S., Schwab, D.J., Tsai, J.J., and Dragoset, R.A. (2015), Atomic Weights and Isotopic Compositions (version 4.1). [Online] Available: http://physics.nist.gov/Comp [Accessed 23 November 2022]. National Institute of Standards and Technology, Gaithersburg, MD.
```

### Comparing `isovec-1.0.0/README.md` & `isovec-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -200,10 +200,14 @@
   O-16: 2.0921E-01
   O-17: 7.9694E-05
   O-18: 4.2993E-04
    [...]
 ```
 
 
+## Changelog
+
+For a history of changes, refer to the file `CHANGELOG.md` in the source distribution available under "Navigation/Download files".
+
 ## References
 
 1. Coursey, J.S., Schwab, D.J., Tsai, J.J., and Dragoset, R.A. (2015), Atomic Weights and Isotopic Compositions (version 4.1). [Online] Available: http://physics.nist.gov/Comp [Accessed 23 November 2022]. National Institute of Standards and Technology, Gaithersburg, MD.
```

### Comparing `isovec-1.0.0/pyproject.toml` & `isovec-1.0.1/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -8,31 +8,32 @@
 where = ["src"]
 include = ["isovec*"]
 exclude = ["extension*"]
 
 
 [project]
 name = "isovec"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
     { name="Julius Mercz", email="julius.mercz@tum.de" }
 ]
-description = "A package to calculate isotopic composition of (custom) Elements, Molecules and Alloys."
+description = "A package to calculate isotopic composition of (custom) Elements, Molecules and Mixtures."
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.9"
-keywords = ["isotope", "element", "molecule", "alloy", "composition", "weight", "atomic"]
+keywords = ["isotope", "element", "molecule", "mixture", "alloy", "composition", "weight", "atomic"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Topic :: Scientific/Engineering :: Physics",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
     "Typing :: Typed"
 ]
 dependencies = [
     
 ]
 
 
-[project.urls]
+[project.urls]
+"PyPI" = "https://pypi.org/project/isovec/"
```

### Comparing `isovec-1.0.0/src/isovec/Element.py` & `isovec-1.0.1/src/isovec/Element.py`

 * *Files identical despite different names*

### Comparing `isovec-1.0.0/src/isovec/Isotope.py` & `isovec-1.0.1/src/isovec/Isotope.py`

 * *Files identical despite different names*

### Comparing `isovec-1.0.0/src/isovec/Mixture.py` & `isovec-1.0.1/src/isovec/Mixture.py`

 * *Files identical despite different names*

### Comparing `isovec-1.0.0/src/isovec/Molecule.py` & `isovec-1.0.1/src/isovec/Molecule.py`

 * *Files identical despite different names*

### Comparing `isovec-1.0.0/src/isovec/elements.py` & `isovec-1.0.1/src/isovec/elements.py`

 * *Files identical despite different names*

### Comparing `isovec-1.0.0/src/isovec/isotopes.py` & `isovec-1.0.1/src/isovec/isotopes.py`

 * *Files identical despite different names*

### Comparing `isovec-1.0.0/src/isovec.egg-info/PKG-INFO` & `isovec-1.0.1/src/isovec.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: isovec
-Version: 1.0.0
-Summary: A package to calculate isotopic composition of (custom) Elements, Molecules and Alloys.
+Version: 1.0.1
+Summary: A package to calculate isotopic composition of (custom) Elements, Molecules and Mixtures.
 Author-email: Julius Mercz <julius.mercz@tum.de>
 License: MIT License
         
         Copyright (c) 2023 Julius Mercz
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -20,15 +20,16 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
-Keywords: isotope,element,molecule,alloy,composition,weight,atomic
+Project-URL: PyPI, https://pypi.org/project/isovec/
+Keywords: isotope,element,molecule,mixture,alloy,composition,weight,atomic
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Typing :: Typed
@@ -238,10 +239,14 @@
   O-16: 2.0921E-01
   O-17: 7.9694E-05
   O-18: 4.2993E-04
    [...]
 ```
 
 
+## Changelog
+
+For a history of changes, refer to the file `CHANGELOG.md` in the source distribution available under "Navigation/Download files".
+
 ## References
 
 1. Coursey, J.S., Schwab, D.J., Tsai, J.J., and Dragoset, R.A. (2015), Atomic Weights and Isotopic Compositions (version 4.1). [Online] Available: http://physics.nist.gov/Comp [Accessed 23 November 2022]. National Institute of Standards and Technology, Gaithersburg, MD.
```

