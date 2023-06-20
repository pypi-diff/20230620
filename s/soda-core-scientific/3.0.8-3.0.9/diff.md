# Comparing `tmp/soda-core-scientific-3.0.8.tar.gz` & `tmp/soda-core-scientific-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda-core-scientific-3.0.8.tar", last modified: Wed Sep 21 19:41:52 2022, max compression
+gzip compressed data, was "soda-core-scientific-3.0.9.tar", last modified: Tue Sep 27 20:20:01 2022, max compression
```

## Comparing `soda-core-scientific-3.0.8.tar` & `soda-core-scientific-3.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:52.387367 soda-core-scientific-3.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-09-21 19:41:52.387367 soda-core-scientific-3.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-21 19:41:52.387367 soda-core-scientific-3.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1149 2022-09-21 19:41:14.000000 soda-core-scientific-3.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:52.383367 soda-core-scientific-3.0.8/soda/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:52.383367 soda-core-scientific-3.0.8/soda/scientific/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:52.387367 soda-core-scientific-3.0.8/soda/scientific/anomaly_detection/
--rw-r--r--   0 runner    (1001) docker     (121)     9557 2022-09-21 19:41:14.000000 soda-core-scientific-3.0.8/soda/scientific/anomaly_detection/anomaly_detector.py
--rw-r--r--   0 runner    (1001) docker     (121)     1167 2022-09-21 19:41:14.000000 soda-core-scientific-3.0.8/soda/scientific/anomaly_detection/detector_config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     7531 2022-09-21 19:41:14.000000 soda-core-scientific-3.0.8/soda/scientific/anomaly_detection/feedback_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:52.387367 soda-core-scientific-3.0.8/soda/scientific/anomaly_detection/models/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:14.000000 soda-core-scientific-3.0.8/soda/scientific/anomaly_detection/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4161 2022-09-21 19:41:14.000000 soda-core-scientific-3.0.8/soda/scientific/anomaly_detection/models/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    21889 2022-09-21 19:41:14.000000 soda-core-scientific-3.0.8/soda/scientific/anomaly_detection/models/prophet_model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:52.387367 soda-core-scientific-3.0.8/soda/scientific/common/
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-09-21 19:41:14.000000 soda-core-scientific-3.0.8/soda/scientific/common/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:52.387367 soda-core-scientific-3.0.8/soda/scientific/distribution/
--rw-r--r--   0 runner    (1001) docker     (121)    12338 2022-09-21 19:41:14.000000 soda-core-scientific-3.0.8/soda/scientific/distribution/comparison.py
--rw-r--r--   0 runner    (1001) docker     (121)     1841 2022-09-21 19:41:14.000000 soda-core-scientific-3.0.8/soda/scientific/distribution/generate_dro.py
--rw-r--r--   0 runner    (1001) docker     (121)     2920 2022-09-21 19:41:14.000000 soda-core-scientific-3.0.8/soda/scientific/distribution/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:52.387367 soda-core-scientific-3.0.8/soda_core_scientific.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-09-21 19:41:52.000000 soda-core-scientific-3.0.8/soda_core_scientific.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      715 2022-09-21 19:41:52.000000 soda-core-scientific-3.0.8/soda_core_scientific.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-21 19:41:52.000000 soda-core-scientific-3.0.8/soda_core_scientific.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-09-21 19:41:52.000000 soda-core-scientific-3.0.8/soda_core_scientific.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-09-21 19:41:52.000000 soda-core-scientific-3.0.8/soda_core_scientific.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:20:01.780087 soda-core-scientific-3.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-09-27 20:20:01.780087 soda-core-scientific-3.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-27 20:20:01.780087 soda-core-scientific-3.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1149 2022-09-27 20:19:27.000000 soda-core-scientific-3.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:20:01.780087 soda-core-scientific-3.0.9/soda/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:20:01.780087 soda-core-scientific-3.0.9/soda/scientific/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:20:01.780087 soda-core-scientific-3.0.9/soda/scientific/anomaly_detection/
+-rw-r--r--   0 runner    (1001) docker     (121)     9557 2022-09-27 20:19:27.000000 soda-core-scientific-3.0.9/soda/scientific/anomaly_detection/anomaly_detector.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1167 2022-09-27 20:19:27.000000 soda-core-scientific-3.0.9/soda/scientific/anomaly_detection/detector_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     7531 2022-09-27 20:19:27.000000 soda-core-scientific-3.0.9/soda/scientific/anomaly_detection/feedback_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:20:01.780087 soda-core-scientific-3.0.9/soda/scientific/anomaly_detection/models/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-27 20:19:27.000000 soda-core-scientific-3.0.9/soda/scientific/anomaly_detection/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4161 2022-09-27 20:19:27.000000 soda-core-scientific-3.0.9/soda/scientific/anomaly_detection/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21889 2022-09-27 20:19:27.000000 soda-core-scientific-3.0.9/soda/scientific/anomaly_detection/models/prophet_model.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:20:01.780087 soda-core-scientific-3.0.9/soda/scientific/common/
+-rw-r--r--   0 runner    (1001) docker     (121)      134 2022-09-27 20:19:27.000000 soda-core-scientific-3.0.9/soda/scientific/common/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:20:01.780087 soda-core-scientific-3.0.9/soda/scientific/distribution/
+-rw-r--r--   0 runner    (1001) docker     (121)    12338 2022-09-27 20:19:27.000000 soda-core-scientific-3.0.9/soda/scientific/distribution/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1841 2022-09-27 20:19:27.000000 soda-core-scientific-3.0.9/soda/scientific/distribution/generate_dro.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2920 2022-09-27 20:19:27.000000 soda-core-scientific-3.0.9/soda/scientific/distribution/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:20:01.780087 soda-core-scientific-3.0.9/soda_core_scientific.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-09-27 20:20:01.000000 soda-core-scientific-3.0.9/soda_core_scientific.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      715 2022-09-27 20:20:01.000000 soda-core-scientific-3.0.9/soda_core_scientific.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-27 20:20:01.000000 soda-core-scientific-3.0.9/soda_core_scientific.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      164 2022-09-27 20:20:01.000000 soda-core-scientific-3.0.9/soda_core_scientific.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2022-09-27 20:20:01.000000 soda-core-scientific-3.0.9/soda_core_scientific.egg-info/top_level.txt
```

### Comparing `soda-core-scientific-3.0.8/setup.py` & `soda-core-scientific-3.0.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 if sys.version_info < (3, 8):
     print("Error: Soda SQL requires at least Python 3.8")
     print("Error: Please upgrade your Python version to 3.8 or later")
     sys.exit(1)
 
 package_name = "soda-core-scientific"
-package_version = "3.0.8"
+package_version = "3.0.9"
 description = "Soda Core Scientific Package"
 requires = [
     f"soda-core=={package_version}",
     "wheel",
     "pydantic>=1.8.1,<2.0.0",
     "scipy>=1.8.0",
     "inflection==0.5.1",
```

### Comparing `soda-core-scientific-3.0.8/soda/scientific/anomaly_detection/anomaly_detector.py` & `soda-core-scientific-3.0.9/soda/scientific/anomaly_detection/anomaly_detector.py`

 * *Files identical despite different names*

### Comparing `soda-core-scientific-3.0.8/soda/scientific/anomaly_detection/detector_config.yaml` & `soda-core-scientific-3.0.9/soda/scientific/anomaly_detection/detector_config.yaml`

 * *Files identical despite different names*

### Comparing `soda-core-scientific-3.0.8/soda/scientific/anomaly_detection/feedback_processor.py` & `soda-core-scientific-3.0.9/soda/scientific/anomaly_detection/feedback_processor.py`

 * *Files identical despite different names*

### Comparing `soda-core-scientific-3.0.8/soda/scientific/anomaly_detection/models/base.py` & `soda-core-scientific-3.0.9/soda/scientific/anomaly_detection/models/base.py`

 * *Files identical despite different names*

### Comparing `soda-core-scientific-3.0.8/soda/scientific/anomaly_detection/models/prophet_model.py` & `soda-core-scientific-3.0.9/soda/scientific/anomaly_detection/models/prophet_model.py`

 * *Files identical despite different names*

### Comparing `soda-core-scientific-3.0.8/soda/scientific/distribution/comparison.py` & `soda-core-scientific-3.0.9/soda/scientific/distribution/comparison.py`

 * *Files identical despite different names*

### Comparing `soda-core-scientific-3.0.8/soda/scientific/distribution/generate_dro.py` & `soda-core-scientific-3.0.9/soda/scientific/distribution/generate_dro.py`

 * *Files identical despite different names*

### Comparing `soda-core-scientific-3.0.8/soda/scientific/distribution/utils.py` & `soda-core-scientific-3.0.9/soda/scientific/distribution/utils.py`

 * *Files identical despite different names*

### Comparing `soda-core-scientific-3.0.8/soda_core_scientific.egg-info/SOURCES.txt` & `soda-core-scientific-3.0.9/soda_core_scientific.egg-info/SOURCES.txt`

 * *Files identical despite different names*

