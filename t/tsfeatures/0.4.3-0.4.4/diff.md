# Comparing `tmp/tsfeatures-0.4.3.tar.gz` & `tmp/tsfeatures-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsfeatures-0.4.3.tar", last modified: Tue Jun 20 04:17:54 2023, max compression
+gzip compressed data, was "tsfeatures-0.4.4.tar", last modified: Tue Jun 20 08:01:01 2023, max compression
```

## Comparing `tsfeatures-0.4.3.tar` & `tsfeatures-0.4.4.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 04:17:54.307736 tsfeatures-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11336 2023-06-20 04:17:44.000000 tsfeatures-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-06-20 04:17:54.303737 tsfeatures-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-06-20 04:17:44.000000 tsfeatures-0.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 04:17:54.307736 tsfeatures-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-20 04:17:44.000000 tsfeatures-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 04:17:54.299736 tsfeatures-0.4.3/tsfeatures/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-20 04:17:44.000000 tsfeatures-0.4.3/tsfeatures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-06-20 04:17:44.000000 tsfeatures-0.4.3/tsfeatures/compare_with_r.py
--rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-06-20 04:17:44.000000 tsfeatures-0.4.3/tsfeatures/m4_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 04:17:54.303737 tsfeatures-0.4.3/tsfeatures/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-20 04:17:44.000000 tsfeatures-0.4.3/tsfeatures/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10356 2023-06-20 04:17:44.000000 tsfeatures-0.4.3/tsfeatures/metrics/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 04:17:54.303737 tsfeatures-0.4.3/tsfeatures/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 04:17:44.000000 tsfeatures-0.4.3/tsfeatures/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-20 04:17:44.000000 tsfeatures-0.4.3/tsfeatures/tests/test_acf_features.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-20 04:17:44.000000 tsfeatures-0.4.3/tsfeatures/tests/test_arch_stat.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-20 04:17:44.000000 tsfeatures-0.4.3/tsfeatures/tests/test_holt_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-20 04:17:44.000000 tsfeatures-0.4.3/tsfeatures/tests/test_mutability.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-20 04:17:44.000000 tsfeatures-0.4.3/tsfeatures/tests/test_pacf_features.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-20 04:17:44.000000 tsfeatures-0.4.3/tsfeatures/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-20 04:17:44.000000 tsfeatures-0.4.3/tsfeatures/tests/test_sparsity.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-20 04:17:44.000000 tsfeatures-0.4.3/tsfeatures/tests/test_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    29211 2023-06-20 04:17:44.000000 tsfeatures-0.4.3/tsfeatures/tsfeatures.py
--rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-06-20 04:17:44.000000 tsfeatures-0.4.3/tsfeatures/tsfeatures_r.py
--rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-06-20 04:17:44.000000 tsfeatures-0.4.3/tsfeatures/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 04:17:54.299736 tsfeatures-0.4.3/tsfeatures.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-06-20 04:17:54.000000 tsfeatures-0.4.3/tsfeatures.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-20 04:17:54.000000 tsfeatures-0.4.3/tsfeatures.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 04:17:54.000000 tsfeatures-0.4.3/tsfeatures.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-20 04:17:54.000000 tsfeatures-0.4.3/tsfeatures.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-20 04:17:54.000000 tsfeatures-0.4.3/tsfeatures.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:01:01.246237 tsfeatures-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11336 2023-06-20 08:00:51.000000 tsfeatures-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-06-20 08:01:01.246237 tsfeatures-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-06-20 08:00:51.000000 tsfeatures-0.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 08:01:01.246237 tsfeatures-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-20 08:00:51.000000 tsfeatures-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:01:01.246237 tsfeatures-0.4.4/tsfeatures/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-20 08:00:51.000000 tsfeatures-0.4.4/tsfeatures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-06-20 08:00:51.000000 tsfeatures-0.4.4/tsfeatures/compare_with_r.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-06-20 08:00:51.000000 tsfeatures-0.4.4/tsfeatures/m4_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:01:01.246237 tsfeatures-0.4.4/tsfeatures/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-20 08:00:51.000000 tsfeatures-0.4.4/tsfeatures/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10356 2023-06-20 08:00:51.000000 tsfeatures-0.4.4/tsfeatures/metrics/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:01:01.246237 tsfeatures-0.4.4/tsfeatures/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 08:00:51.000000 tsfeatures-0.4.4/tsfeatures/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-20 08:00:51.000000 tsfeatures-0.4.4/tsfeatures/tests/test_acf_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-20 08:00:51.000000 tsfeatures-0.4.4/tsfeatures/tests/test_arch_stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-20 08:00:51.000000 tsfeatures-0.4.4/tsfeatures/tests/test_holt_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-20 08:00:51.000000 tsfeatures-0.4.4/tsfeatures/tests/test_mutability.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-20 08:00:51.000000 tsfeatures-0.4.4/tsfeatures/tests/test_pacf_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-20 08:00:51.000000 tsfeatures-0.4.4/tsfeatures/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-20 08:00:51.000000 tsfeatures-0.4.4/tsfeatures/tests/test_small_ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-20 08:00:51.000000 tsfeatures-0.4.4/tsfeatures/tests/test_sparsity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-20 08:00:51.000000 tsfeatures-0.4.4/tsfeatures/tests/test_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29263 2023-06-20 08:00:51.000000 tsfeatures-0.4.4/tsfeatures/tsfeatures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-06-20 08:00:51.000000 tsfeatures-0.4.4/tsfeatures/tsfeatures_r.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-06-20 08:00:51.000000 tsfeatures-0.4.4/tsfeatures/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:01:01.246237 tsfeatures-0.4.4/tsfeatures.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-06-20 08:01:01.000000 tsfeatures-0.4.4/tsfeatures.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-20 08:01:01.000000 tsfeatures-0.4.4/tsfeatures.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 08:01:01.000000 tsfeatures-0.4.4/tsfeatures.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-20 08:01:01.000000 tsfeatures-0.4.4/tsfeatures.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-20 08:01:01.000000 tsfeatures-0.4.4/tsfeatures.egg-info/top_level.txt
```

### Comparing `tsfeatures-0.4.3/LICENSE` & `tsfeatures-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tsfeatures-0.4.3/PKG-INFO` & `tsfeatures-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsfeatures
-Version: 0.4.3
+Version: 0.4.4
 Summary: Calculates various features from time series data.
 Home-page: https://github.com/Nixtla/tsfeatures
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `tsfeatures-0.4.3/README.md` & `tsfeatures-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `tsfeatures-0.4.3/setup.py` & `tsfeatures-0.4.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tsfeatures",
-    version="0.4.3",
+    version="0.4.4",
     description="Calculates various features from time series data.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Nixtla/tsfeatures",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `tsfeatures-0.4.3/tsfeatures/compare_with_r.py` & `tsfeatures-0.4.4/tsfeatures/compare_with_r.py`

 * *Files identical despite different names*

### Comparing `tsfeatures-0.4.3/tsfeatures/m4_data.py` & `tsfeatures-0.4.4/tsfeatures/m4_data.py`

 * *Files identical despite different names*

### Comparing `tsfeatures-0.4.3/tsfeatures/metrics/metrics.py` & `tsfeatures-0.4.4/tsfeatures/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `tsfeatures-0.4.3/tsfeatures/tests/test_acf_features.py` & `tsfeatures-0.4.4/tsfeatures/tests/test_acf_features.py`

 * *Files identical despite different names*

### Comparing `tsfeatures-0.4.3/tsfeatures/tests/test_holt_parameters.py` & `tsfeatures-0.4.4/tsfeatures/tests/test_holt_parameters.py`

 * *Files identical despite different names*

### Comparing `tsfeatures-0.4.3/tsfeatures/tests/test_mutability.py` & `tsfeatures-0.4.4/tsfeatures/tests/test_mutability.py`

 * *Files identical despite different names*

### Comparing `tsfeatures-0.4.3/tsfeatures/tests/test_pipeline.py` & `tsfeatures-0.4.4/tsfeatures/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `tsfeatures-0.4.3/tsfeatures/tests/test_sparsity.py` & `tsfeatures-0.4.4/tsfeatures/tests/test_sparsity.py`

 * *Files identical despite different names*

### Comparing `tsfeatures-0.4.3/tsfeatures/tests/test_statistics.py` & `tsfeatures-0.4.4/tsfeatures/tests/test_statistics.py`

 * *Files identical despite different names*

### Comparing `tsfeatures-0.4.3/tsfeatures/tsfeatures.py` & `tsfeatures-0.4.4/tsfeatures/tsfeatures.py`

 * *Files 0% similar despite different names*

```diff
@@ -755,15 +755,18 @@
     # Compute measures of linearity and curvature
     time = np.arange(n) + 1
     poly_m = poly(time, 2)
     time_x = add_constant(poly_m)
     coefs = OLS(trend0, time_x).fit().params
 
     linearity = coefs[1]
-    curvature = -coefs[2]
+    try:
+        curvature = -coefs[2]
+    except:
+        curvature = np.nan
     # ACF features
     acfremainder = acf_features(remainder, m)
     # Assemble features
     output = {
         'nperiods': nperiods,
         'seasonal_period': m,
         'trend': trend,
```

### Comparing `tsfeatures-0.4.3/tsfeatures/tsfeatures_r.py` & `tsfeatures-0.4.4/tsfeatures/tsfeatures_r.py`

 * *Files identical despite different names*

### Comparing `tsfeatures-0.4.3/tsfeatures/utils.py` & `tsfeatures-0.4.4/tsfeatures/utils.py`

 * *Files identical despite different names*

### Comparing `tsfeatures-0.4.3/tsfeatures.egg-info/PKG-INFO` & `tsfeatures-0.4.4/tsfeatures.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsfeatures
-Version: 0.4.3
+Version: 0.4.4
 Summary: Calculates various features from time series data.
 Home-page: https://github.com/Nixtla/tsfeatures
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `tsfeatures-0.4.3/tsfeatures.egg-info/SOURCES.txt` & `tsfeatures-0.4.4/tsfeatures.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -17,9 +17,10 @@
 tsfeatures/tests/__init__.py
 tsfeatures/tests/test_acf_features.py
 tsfeatures/tests/test_arch_stat.py
 tsfeatures/tests/test_holt_parameters.py
 tsfeatures/tests/test_mutability.py
 tsfeatures/tests/test_pacf_features.py
 tsfeatures/tests/test_pipeline.py
+tsfeatures/tests/test_small_ts.py
 tsfeatures/tests/test_sparsity.py
 tsfeatures/tests/test_statistics.py
```

