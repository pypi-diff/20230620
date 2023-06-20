# Comparing `tmp/mlserver-xgboost-1.3.4rc2.tar.gz` & `tmp/mlserver-xgboost-1.4.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlserver-xgboost-1.3.4rc2.tar", last modified: Tue Jun 20 09:09:26 2023, max compression
+gzip compressed data, was "mlserver-xgboost-1.4.0.dev2.tar", last modified: Thu May  4 09:30:37 2023, max compression
```

## Comparing `mlserver-xgboost-1.3.4rc2.tar` & `mlserver-xgboost-1.4.0.dev2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:09:26.100738 mlserver-xgboost-1.3.4rc2/
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-06-20 09:08:50.000000 mlserver-xgboost-1.3.4rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-06-20 09:09:26.100738 mlserver-xgboost-1.3.4rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-06-20 09:08:50.000000 mlserver-xgboost-1.3.4rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:09:26.096738 mlserver-xgboost-1.3.4rc2/mlserver_xgboost/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-20 09:08:50.000000 mlserver-xgboost-1.3.4rc2/mlserver_xgboost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-20 09:08:50.000000 mlserver-xgboost-1.3.4rc2/mlserver_xgboost/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-06-20 09:08:50.000000 mlserver-xgboost-1.3.4rc2/mlserver_xgboost/xgboost.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:09:26.100738 mlserver-xgboost-1.3.4rc2/mlserver_xgboost.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-06-20 09:09:25.000000 mlserver-xgboost-1.3.4rc2/mlserver_xgboost.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-20 09:09:26.000000 mlserver-xgboost-1.3.4rc2/mlserver_xgboost.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 09:09:25.000000 mlserver-xgboost-1.3.4rc2/mlserver_xgboost.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-20 09:09:25.000000 mlserver-xgboost-1.3.4rc2/mlserver_xgboost.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-20 09:09:25.000000 mlserver-xgboost-1.3.4rc2/mlserver_xgboost.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 09:09:26.100738 mlserver-xgboost-1.3.4rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-20 09:08:50.000000 mlserver-xgboost-1.3.4rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:37.289166 mlserver-xgboost-1.4.0.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-05-04 09:29:57.000000 mlserver-xgboost-1.4.0.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-04 09:30:37.289166 mlserver-xgboost-1.4.0.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-04 09:29:57.000000 mlserver-xgboost-1.4.0.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:37.289166 mlserver-xgboost-1.4.0.dev2/mlserver_xgboost/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-04 09:29:57.000000 mlserver-xgboost-1.4.0.dev2/mlserver_xgboost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-04 09:29:57.000000 mlserver-xgboost-1.4.0.dev2/mlserver_xgboost/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-05-04 09:29:57.000000 mlserver-xgboost-1.4.0.dev2/mlserver_xgboost/xgboost.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:37.289166 mlserver-xgboost-1.4.0.dev2/mlserver_xgboost.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-04 09:30:36.000000 mlserver-xgboost-1.4.0.dev2/mlserver_xgboost.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-04 09:30:37.000000 mlserver-xgboost-1.4.0.dev2/mlserver_xgboost.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 09:30:36.000000 mlserver-xgboost-1.4.0.dev2/mlserver_xgboost.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-04 09:30:36.000000 mlserver-xgboost-1.4.0.dev2/mlserver_xgboost.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-04 09:30:36.000000 mlserver-xgboost-1.4.0.dev2/mlserver_xgboost.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 09:30:37.289166 mlserver-xgboost-1.4.0.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-04 09:29:57.000000 mlserver-xgboost-1.4.0.dev2/setup.py
```

### Comparing `mlserver-xgboost-1.3.4rc2/LICENSE` & `mlserver-xgboost-1.4.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `mlserver-xgboost-1.3.4rc2/mlserver_xgboost/xgboost.py` & `mlserver-xgboost-1.4.0.dev2/mlserver_xgboost/xgboost.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     ResponseOutput,
 )
 
 PREDICT_OUTPUT = "predict"
 PREDICT_PROBA_OUTPUT = "predict_proba"
 VALID_OUTPUTS = [PREDICT_OUTPUT, PREDICT_PROBA_OUTPUT]
 
-WELLKNOWN_MODEL_FILENAMES = ["model.bst", "model.json", "model.ubj"]
+WELLKNOWN_MODEL_FILENAMES = ["model.bst", "model.json"]
 
 
 def _load_sklearn_interface(model_uri: str) -> XGBModel:
     try:
         regressor = xgb.XGBRegressor()
         regressor.load_model(model_uri)
         return regressor
```

### Comparing `mlserver-xgboost-1.3.4rc2/setup.py` & `mlserver-xgboost-1.4.0.dev2/setup.py`

 * *Files identical despite different names*

