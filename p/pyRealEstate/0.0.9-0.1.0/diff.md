# Comparing `tmp/pyRealEstate-0.0.9.tar.gz` & `tmp/pyRealEstate-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyRealEstate-0.0.9.tar", last modified: Thu Jun  8 12:52:35 2023, max compression
+gzip compressed data, was "pyRealEstate-0.1.0.tar", last modified: Tue Jun 20 19:00:39 2023, max compression
```

## Comparing `pyRealEstate-0.0.9.tar` & `pyRealEstate-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:52:35.453393 pyRealEstate-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-08 12:52:16.000000 pyRealEstate-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-08 12:52:35.453393 pyRealEstate-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-08 12:52:16.000000 pyRealEstate-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:52:35.453393 pyRealEstate-0.0.9/pyRealEstate/
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-08 12:52:16.000000 pyRealEstate-0.0.9/pyRealEstate/Pre_Processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-06-08 12:52:16.000000 pyRealEstate-0.0.9/pyRealEstate/RealEstateMetrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-08 12:52:16.000000 pyRealEstate-0.0.9/pyRealEstate/Time_Trending.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 12:52:16.000000 pyRealEstate-0.0.9/pyRealEstate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:52:35.453393 pyRealEstate-0.0.9/pyRealEstate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-08 12:52:35.000000 pyRealEstate-0.0.9/pyRealEstate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-08 12:52:35.000000 pyRealEstate-0.0.9/pyRealEstate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 12:52:35.000000 pyRealEstate-0.0.9/pyRealEstate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-08 12:52:35.000000 pyRealEstate-0.0.9/pyRealEstate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-08 12:52:35.000000 pyRealEstate-0.0.9/pyRealEstate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-08 12:52:16.000000 pyRealEstate-0.0.9/pypi_description.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-08 12:52:16.000000 pyRealEstate-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-08 12:52:35.453393 pyRealEstate-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:00:39.082808 pyRealEstate-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-20 19:00:23.000000 pyRealEstate-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-20 19:00:39.082808 pyRealEstate-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-06-20 19:00:23.000000 pyRealEstate-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:00:39.082808 pyRealEstate-0.1.0/pyRealEstate/
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-20 19:00:23.000000 pyRealEstate-0.1.0/pyRealEstate/Pre_Processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-06-20 19:00:23.000000 pyRealEstate-0.1.0/pyRealEstate/RealEstateMetrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-06-20 19:00:23.000000 pyRealEstate-0.1.0/pyRealEstate/Time_Trending.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 19:00:23.000000 pyRealEstate-0.1.0/pyRealEstate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:00:39.082808 pyRealEstate-0.1.0/pyRealEstate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-20 19:00:39.000000 pyRealEstate-0.1.0/pyRealEstate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-20 19:00:39.000000 pyRealEstate-0.1.0/pyRealEstate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 19:00:39.000000 pyRealEstate-0.1.0/pyRealEstate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-20 19:00:39.000000 pyRealEstate-0.1.0/pyRealEstate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-20 19:00:39.000000 pyRealEstate-0.1.0/pyRealEstate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-20 19:00:23.000000 pyRealEstate-0.1.0/pypi_description.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-20 19:00:23.000000 pyRealEstate-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-20 19:00:39.082808 pyRealEstate-0.1.0/setup.cfg
```

### Comparing `pyRealEstate-0.0.9/LICENSE` & `pyRealEstate-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyRealEstate-0.0.9/PKG-INFO` & `pyRealEstate-0.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyRealEstate
-Version: 0.0.9
+Version: 0.1.0
 Summary: package to assist with data analytics in real estate
 Home-page: https://github.com/Joshua-Data-Wizard/PyRealEstate/tree/main
 Author: Joshua Jorgensen
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.4
```

### Comparing `pyRealEstate-0.0.9/pyRealEstate/Pre_Processing.py` & `pyRealEstate-0.1.0/pyRealEstate/Pre_Processing.py`

 * *Files identical despite different names*

### Comparing `pyRealEstate-0.0.9/pyRealEstate/RealEstateMetrics.py` & `pyRealEstate-0.1.0/pyRealEstate/RealEstateMetrics.py`

 * *Files identical despite different names*

### Comparing `pyRealEstate-0.0.9/pyRealEstate/Time_Trending.py` & `pyRealEstate-0.1.0/pyRealEstate/Time_Trending.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 import pandas as pd 
 import statsmodels.api as sm
 import matplotlib.pyplot as plt
 
 
-class SPPSF_Polyniomial_Time_Model :
+class SPPSF_Polynomial_Time_Model :
 
 
   def fit( self ,SPPSF_ , Time_ , return_model =False ):
     #Creates df for SPPSF and Months
     modelData = pd.DataFrame({
                               'SPPSF' : SPPSF_ , 
                               'const' : 1,
```

### Comparing `pyRealEstate-0.0.9/pyRealEstate.egg-info/PKG-INFO` & `pyRealEstate-0.1.0/pyRealEstate.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyRealEstate
-Version: 0.0.9
+Version: 0.1.0
 Summary: package to assist with data analytics in real estate
 Home-page: https://github.com/Joshua-Data-Wizard/PyRealEstate/tree/main
 Author: Joshua Jorgensen
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.4
```

### Comparing `pyRealEstate-0.0.9/pypi_description.md` & `pyRealEstate-0.1.0/pypi_description.md`

 * *Files identical despite different names*

### Comparing `pyRealEstate-0.0.9/setup.cfg` & `pyRealEstate-0.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyRealEstate
-version = 0.0.9
+version = 0.1.0
 author = Joshua Jorgensen
 description = package to assist with data analytics in real estate
 long_description = file: pypi_description.md
 long_description_content_type = text/markdown
 url = https://github.com/Joshua-Data-Wizard/PyRealEstate/tree/main
 classifiers = 
 	Programming Language :: Python :: 3
```

