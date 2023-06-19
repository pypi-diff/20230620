# Comparing `tmp/responsibleai_tabular_automl-0.3.0.tar.gz` & `tmp/responsibleai_tabular_automl-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "responsibleai_tabular_automl-0.3.0.tar", last modified: Fri May  5 21:47:35 2023, max compression
+gzip compressed data, was "responsibleai_tabular_automl-0.4.0.tar", last modified: Mon Jun 19 23:16:42 2023, max compression
```

## Comparing `responsibleai_tabular_automl-0.3.0.tar` & `responsibleai_tabular_automl-0.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 21:47:35.551896 responsibleai_tabular_automl-0.3.0/
--rw-rw-rw-   0        0        0      778 2023-05-05 21:47:35.551896 responsibleai_tabular_automl-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0      134 2023-01-18 23:36:24.000000 responsibleai_tabular_automl-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 21:47:35.511897 responsibleai_tabular_automl-0.3.0/responsibleai_tabular_automl/
--rw-rw-rw-   0        0        0      284 2023-03-07 22:09:35.000000 responsibleai_tabular_automl-0.3.0/responsibleai_tabular_automl/__init__.py
--rw-rw-rw-   0        0        0     6104 2023-05-04 20:34:24.000000 responsibleai_tabular_automl-0.3.0/responsibleai_tabular_automl/_loggerfactory.py
--rw-rw-rw-   0        0        0    12436 2023-05-05 17:35:09.000000 responsibleai_tabular_automl-0.3.0/responsibleai_tabular_automl/automl_inference_run.py
--rw-rw-rw-   0        0        0    10641 2023-05-05 21:28:52.000000 responsibleai_tabular_automl-0.3.0/responsibleai_tabular_automl/rai_automl.py
--rw-rw-rw-   0        0        0      210 2023-05-05 21:40:10.000000 responsibleai_tabular_automl-0.3.0/responsibleai_tabular_automl/version.py
-drwxrwxrwx   0        0        0        0 2023-05-05 21:47:35.536927 responsibleai_tabular_automl-0.3.0/responsibleai_tabular_automl.egg-info/
--rw-rw-rw-   0        0        0      778 2023-05-05 21:47:35.000000 responsibleai_tabular_automl-0.3.0/responsibleai_tabular_automl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      526 2023-05-05 21:47:35.000000 responsibleai_tabular_automl-0.3.0/responsibleai_tabular_automl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 21:47:35.000000 responsibleai_tabular_automl-0.3.0/responsibleai_tabular_automl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2023-05-05 21:47:35.000000 responsibleai_tabular_automl-0.3.0/responsibleai_tabular_automl.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2023-05-05 21:47:35.000000 responsibleai_tabular_automl-0.3.0/responsibleai_tabular_automl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 21:47:35.551896 responsibleai_tabular_automl-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1399 2023-03-07 22:09:35.000000 responsibleai_tabular_automl-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-05 21:47:35.549897 responsibleai_tabular_automl-0.3.0/tests/
--rw-rw-rw-   0        0        0     1654 2023-05-03 22:59:55.000000 responsibleai_tabular_automl-0.3.0/tests/test_rai_automl.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:16:42.329678 responsibleai_tabular_automl-0.4.0/
+-rw-rw-rw-   0        0        0      778 2023-06-19 23:16:42.329678 responsibleai_tabular_automl-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0      134 2023-01-18 23:36:24.000000 responsibleai_tabular_automl-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 23:16:42.298177 responsibleai_tabular_automl-0.4.0/responsibleai_tabular_automl/
+-rw-rw-rw-   0        0        0      284 2023-03-07 22:09:35.000000 responsibleai_tabular_automl-0.4.0/responsibleai_tabular_automl/__init__.py
+-rw-rw-rw-   0        0        0     6104 2023-05-04 20:34:24.000000 responsibleai_tabular_automl-0.4.0/responsibleai_tabular_automl/_loggerfactory.py
+-rw-rw-rw-   0        0        0    12436 2023-06-19 23:11:29.000000 responsibleai_tabular_automl-0.4.0/responsibleai_tabular_automl/automl_inference_run.py
+-rw-rw-rw-   0        0        0    10641 2023-06-19 23:11:29.000000 responsibleai_tabular_automl-0.4.0/responsibleai_tabular_automl/rai_automl.py
+-rw-rw-rw-   0        0        0      210 2023-06-19 23:11:29.000000 responsibleai_tabular_automl-0.4.0/responsibleai_tabular_automl/version.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:16:42.298177 responsibleai_tabular_automl-0.4.0/responsibleai_tabular_automl.egg-info/
+-rw-rw-rw-   0        0        0      778 2023-06-19 23:16:42.000000 responsibleai_tabular_automl-0.4.0/responsibleai_tabular_automl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      526 2023-06-19 23:16:42.000000 responsibleai_tabular_automl-0.4.0/responsibleai_tabular_automl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 23:16:42.000000 responsibleai_tabular_automl-0.4.0/responsibleai_tabular_automl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-06-19 23:16:42.000000 responsibleai_tabular_automl-0.4.0/responsibleai_tabular_automl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2023-06-19 23:16:42.000000 responsibleai_tabular_automl-0.4.0/responsibleai_tabular_automl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 23:16:42.329678 responsibleai_tabular_automl-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1399 2023-03-07 22:09:35.000000 responsibleai_tabular_automl-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:16:42.298177 responsibleai_tabular_automl-0.4.0/tests/
+-rw-rw-rw-   0        0        0     1654 2023-05-03 22:59:55.000000 responsibleai_tabular_automl-0.4.0/tests/test_rai_automl.py
```

### Comparing `responsibleai_tabular_automl-0.3.0/PKG-INFO` & `responsibleai_tabular_automl-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: responsibleai_tabular_automl
-Version: 0.3.0
+Version: 0.4.0
 Summary: SDK for computing RAI insights for AutoML models.
 Home-page: 
 Author: Gaurav Gupta, Ke Xu
 Author-email: raiwidgets-maintain@microsoft.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `responsibleai_tabular_automl-0.3.0/responsibleai_tabular_automl/_loggerfactory.py` & `responsibleai_tabular_automl-0.4.0/responsibleai_tabular_automl/_loggerfactory.py`

 * *Files identical despite different names*

### Comparing `responsibleai_tabular_automl-0.3.0/responsibleai_tabular_automl/automl_inference_run.py` & `responsibleai_tabular_automl-0.4.0/responsibleai_tabular_automl/automl_inference_run.py`

 * *Files identical despite different names*

### Comparing `responsibleai_tabular_automl-0.3.0/responsibleai_tabular_automl/rai_automl.py` & `responsibleai_tabular_automl-0.4.0/responsibleai_tabular_automl/rai_automl.py`

 * *Files identical despite different names*

### Comparing `responsibleai_tabular_automl-0.3.0/responsibleai_tabular_automl.egg-info/PKG-INFO` & `responsibleai_tabular_automl-0.4.0/responsibleai_tabular_automl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: responsibleai-tabular-automl
-Version: 0.3.0
+Version: 0.4.0
 Summary: SDK for computing RAI insights for AutoML models.
 Home-page: 
 Author: Gaurav Gupta, Ke Xu
 Author-email: raiwidgets-maintain@microsoft.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `responsibleai_tabular_automl-0.3.0/responsibleai_tabular_automl.egg-info/SOURCES.txt` & `responsibleai_tabular_automl-0.4.0/responsibleai_tabular_automl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `responsibleai_tabular_automl-0.3.0/setup.py` & `responsibleai_tabular_automl-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `responsibleai_tabular_automl-0.3.0/tests/test_rai_automl.py` & `responsibleai_tabular_automl-0.4.0/tests/test_rai_automl.py`

 * *Files identical despite different names*

