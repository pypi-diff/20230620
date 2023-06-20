# Comparing `tmp/ecglib-1.1.0.tar.gz` & `tmp/ecglib-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecglib-1.1.0.tar", last modified: Tue Jun 20 10:41:45 2023, max compression
+gzip compressed data, was "ecglib-1.1.1.tar", last modified: Tue Jun 20 12:36:28 2023, max compression
```

## Comparing `ecglib-1.1.0.tar` & `ecglib-1.1.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxr-x   0 aram      (1002) aram      (1002)        0 2023-06-20 10:41:45.510172 ecglib-1.1.0/
--rw-rw-r--   0 aram      (1002) aram      (1002)    11335 2023-06-20 10:32:40.000000 ecglib-1.1.0/LICENSE
--rw-rw-r--   0 aram      (1002) aram      (1002)       40 2023-06-20 10:32:40.000000 ecglib-1.1.0/MANIFEST.in
--rw-rw-r--   0 aram      (1002) aram      (1002)      419 2023-06-20 10:41:45.510172 ecglib-1.1.0/PKG-INFO
--rw-rw-r--   0 aram      (1002) aram      (1002)     6997 2023-06-20 10:32:40.000000 ecglib-1.1.0/README.md
--rw-rw-r--   0 aram      (1002) aram      (1002)      745 2023-06-20 10:41:45.510172 ecglib-1.1.0/setup.cfg
--rw-rw-r--   0 aram      (1002) aram      (1002)       37 2023-06-20 10:32:40.000000 ecglib-1.1.0/setup.py
-drwxrwxr-x   0 aram      (1002) aram      (1002)        0 2023-06-20 10:41:45.506172 ecglib-1.1.0/src/
-drwxrwxr-x   0 aram      (1002) aram      (1002)        0 2023-06-20 10:41:45.506172 ecglib-1.1.0/src/ecglib/
--rw-rw-r--   0 aram      (1002) aram      (1002)      167 2023-06-20 10:32:40.000000 ecglib-1.1.0/src/ecglib/__init__.py
-drwxrwxr-x   0 aram      (1002) aram      (1002)        0 2023-06-20 10:41:45.506172 ecglib-1.1.0/src/ecglib/data/
--rw-rw-r--   0 aram      (1002) aram      (1002)      149 2023-06-20 10:32:40.000000 ecglib-1.1.0/src/ecglib/data/__init__.py
--rw-rw-r--   0 aram      (1002) aram      (1002)     7587 2023-06-20 10:32:40.000000 ecglib-1.1.0/src/ecglib/data/datasets.py
--rw-rw-r--   0 aram      (1002) aram      (1002)     4993 2023-06-20 10:32:40.000000 ecglib-1.1.0/src/ecglib/data/ecg_record.py
--rw-rw-r--   0 aram      (1002) aram      (1002)     7247 2023-06-20 10:32:40.000000 ecglib-1.1.0/src/ecglib/data/load_datasets.py
-drwxrwxr-x   0 aram      (1002) aram      (1002)        0 2023-06-20 10:41:45.510172 ecglib-1.1.0/src/ecglib/models/
--rw-rw-r--   0 aram      (1002) aram      (1002)        0 2023-06-20 10:32:40.000000 ecglib-1.1.0/src/ecglib/models/__init__.py
-drwxrwxr-x   0 aram      (1002) aram      (1002)        0 2023-06-20 10:41:45.510172 ecglib-1.1.0/src/ecglib/models/architectures/
--rw-rw-r--   0 aram      (1002) aram      (1002)        0 2023-06-20 10:32:40.000000 ecglib-1.1.0/src/ecglib/models/architectures/__init__.py
--rw-rw-r--   0 aram      (1002) aram      (1002)     2068 2023-06-20 10:32:40.000000 ecglib-1.1.0/src/ecglib/models/architectures/cnn_tabular.py
--rw-rw-r--   0 aram      (1002) aram      (1002)     5809 2023-06-20 10:32:40.000000 ecglib-1.1.0/src/ecglib/models/architectures/densenet1d.py
--rw-rw-r--   0 aram      (1002) aram      (1002)      555 2023-06-20 10:32:40.000000 ecglib-1.1.0/src/ecglib/models/architectures/model_types.py
--rw-rw-r--   0 aram      (1002) aram      (1002)     1809 2023-06-20 10:32:40.000000 ecglib-1.1.0/src/ecglib/models/architectures/registred_models.py
--rw-rw-r--   0 aram      (1002) aram      (1002)     7665 2023-06-20 10:32:40.000000 ecglib-1.1.0/src/ecglib/models/architectures/resnet1d.py
--rw-rw-r--   0 aram      (1002) aram      (1002)     2019 2023-06-20 10:32:40.000000 ecglib-1.1.0/src/ecglib/models/architectures/tabular.py
-drwxrwxr-x   0 aram      (1002) aram      (1002)        0 2023-06-20 10:41:45.510172 ecglib-1.1.0/src/ecglib/models/config/
--rw-rw-r--   0 aram      (1002) aram      (1002)        0 2023-06-20 10:32:40.000000 ecglib-1.1.0/src/ecglib/models/config/__init__.py
--rw-rw-r--   0 aram      (1002) aram      (1002)     2639 2023-06-20 10:32:40.000000 ecglib-1.1.0/src/ecglib/models/config/model_configs.py
--rw-rw-r--   0 aram      (1002) aram      (1002)     1693 2023-06-20 10:32:40.000000 ecglib-1.1.0/src/ecglib/models/config/registred_configs.py
--rw-rw-r--   0 aram      (1002) aram      (1002)     8734 2023-06-20 10:32:40.000000 ecglib-1.1.0/src/ecglib/models/model_builder.py
-drwxrwxr-x   0 aram      (1002) aram      (1002)        0 2023-06-20 10:41:45.510172 ecglib-1.1.0/src/ecglib/models/weights/
--rw-rw-r--   0 aram      (1002) aram      (1002)        0 2023-06-20 10:32:40.000000 ecglib-1.1.0/src/ecglib/models/weights/__init__.py
--rw-rw-r--   0 aram      (1002) aram      (1002)      637 2023-06-20 10:32:40.000000 ecglib-1.1.0/src/ecglib/models/weights/checkpoint.py
--rw-rw-r--   0 aram      (1002) aram      (1002)     3175 2023-06-20 10:32:40.000000 ecglib-1.1.0/src/ecglib/models/weights/model_weights_paths.yaml
-drwxrwxr-x   0 aram      (1002) aram      (1002)        0 2023-06-20 10:41:45.510172 ecglib-1.1.0/src/ecglib/predict/
--rw-rw-r--   0 aram      (1002) aram      (1002)       53 2023-06-20 10:32:40.000000 ecglib-1.1.0/src/ecglib/predict/__init__.py
--rw-rw-r--   0 aram      (1002) aram      (1002)    10332 2023-06-20 10:32:40.000000 ecglib-1.1.0/src/ecglib/predict/predict.py
-drwxrwxr-x   0 aram      (1002) aram      (1002)        0 2023-06-20 10:41:45.510172 ecglib-1.1.0/src/ecglib/preprocessing/
--rw-rw-r--   0 aram      (1002) aram      (1002)      150 2023-06-20 10:32:40.000000 ecglib-1.1.0/src/ecglib/preprocessing/__init__.py
--rw-rw-r--   0 aram      (1002) aram      (1002)     2986 2023-06-20 10:32:40.000000 ecglib-1.1.0/src/ecglib/preprocessing/composition.py
--rw-rw-r--   0 aram      (1002) aram      (1002)     9729 2023-06-20 10:32:40.000000 ecglib-1.1.0/src/ecglib/preprocessing/functional.py
--rw-rw-r--   0 aram      (1002) aram      (1002)    24523 2023-06-20 10:32:40.000000 ecglib-1.1.0/src/ecglib/preprocessing/preprocess.py
-drwxrwxr-x   0 aram      (1002) aram      (1002)        0 2023-06-20 10:41:45.506172 ecglib-1.1.0/src/ecglib.egg-info/
--rw-rw-r--   0 aram      (1002) aram      (1002)      419 2023-06-20 10:41:45.000000 ecglib-1.1.0/src/ecglib.egg-info/PKG-INFO
--rw-rw-r--   0 aram      (1002) aram      (1002)     1217 2023-06-20 10:41:45.000000 ecglib-1.1.0/src/ecglib.egg-info/SOURCES.txt
--rw-rw-r--   0 aram      (1002) aram      (1002)        1 2023-06-20 10:41:45.000000 ecglib-1.1.0/src/ecglib.egg-info/dependency_links.txt
--rw-rw-r--   0 aram      (1002) aram      (1002)      190 2023-06-20 10:41:45.000000 ecglib-1.1.0/src/ecglib.egg-info/requires.txt
--rw-rw-r--   0 aram      (1002) aram      (1002)        7 2023-06-20 10:41:45.000000 ecglib-1.1.0/src/ecglib.egg-info/top_level.txt
+drwxrwxr-x   0 aram      (1002) aram      (1002)        0 2023-06-20 12:36:28.535885 ecglib-1.1.1/
+-rw-rw-r--   0 aram      (1002) aram      (1002)    11335 2023-06-20 10:32:40.000000 ecglib-1.1.1/LICENSE
+-rw-rw-r--   0 aram      (1002) aram      (1002)       40 2023-06-20 10:32:40.000000 ecglib-1.1.1/MANIFEST.in
+-rw-rw-r--   0 aram      (1002) aram      (1002)     7449 2023-06-20 12:36:28.535885 ecglib-1.1.1/PKG-INFO
+-rw-rw-r--   0 aram      (1002) aram      (1002)     6997 2023-06-20 10:32:40.000000 ecglib-1.1.1/README.md
+-rw-rw-r--   0 aram      (1002) aram      (1002)      745 2023-06-20 12:36:28.535885 ecglib-1.1.1/setup.cfg
+-rw-rw-r--   0 aram      (1002) aram      (1002)      213 2023-06-20 12:33:45.000000 ecglib-1.1.1/setup.py
+drwxrwxr-x   0 aram      (1002) aram      (1002)        0 2023-06-20 12:36:28.531885 ecglib-1.1.1/src/
+drwxrwxr-x   0 aram      (1002) aram      (1002)        0 2023-06-20 12:36:28.531885 ecglib-1.1.1/src/ecglib/
+-rw-rw-r--   0 aram      (1002) aram      (1002)      167 2023-06-20 10:32:40.000000 ecglib-1.1.1/src/ecglib/__init__.py
+drwxrwxr-x   0 aram      (1002) aram      (1002)        0 2023-06-20 12:36:28.531885 ecglib-1.1.1/src/ecglib/data/
+-rw-rw-r--   0 aram      (1002) aram      (1002)      149 2023-06-20 10:32:40.000000 ecglib-1.1.1/src/ecglib/data/__init__.py
+-rw-rw-r--   0 aram      (1002) aram      (1002)     7587 2023-06-20 10:32:40.000000 ecglib-1.1.1/src/ecglib/data/datasets.py
+-rw-rw-r--   0 aram      (1002) aram      (1002)     4993 2023-06-20 10:32:40.000000 ecglib-1.1.1/src/ecglib/data/ecg_record.py
+-rw-rw-r--   0 aram      (1002) aram      (1002)     7247 2023-06-20 10:32:40.000000 ecglib-1.1.1/src/ecglib/data/load_datasets.py
+drwxrwxr-x   0 aram      (1002) aram      (1002)        0 2023-06-20 12:36:28.531885 ecglib-1.1.1/src/ecglib/models/
+-rw-rw-r--   0 aram      (1002) aram      (1002)        0 2023-06-20 10:32:40.000000 ecglib-1.1.1/src/ecglib/models/__init__.py
+drwxrwxr-x   0 aram      (1002) aram      (1002)        0 2023-06-20 12:36:28.535885 ecglib-1.1.1/src/ecglib/models/architectures/
+-rw-rw-r--   0 aram      (1002) aram      (1002)        0 2023-06-20 10:32:40.000000 ecglib-1.1.1/src/ecglib/models/architectures/__init__.py
+-rw-rw-r--   0 aram      (1002) aram      (1002)     2068 2023-06-20 10:32:40.000000 ecglib-1.1.1/src/ecglib/models/architectures/cnn_tabular.py
+-rw-rw-r--   0 aram      (1002) aram      (1002)     5809 2023-06-20 10:32:40.000000 ecglib-1.1.1/src/ecglib/models/architectures/densenet1d.py
+-rw-rw-r--   0 aram      (1002) aram      (1002)      555 2023-06-20 10:32:40.000000 ecglib-1.1.1/src/ecglib/models/architectures/model_types.py
+-rw-rw-r--   0 aram      (1002) aram      (1002)     1809 2023-06-20 10:32:40.000000 ecglib-1.1.1/src/ecglib/models/architectures/registred_models.py
+-rw-rw-r--   0 aram      (1002) aram      (1002)     7665 2023-06-20 10:32:40.000000 ecglib-1.1.1/src/ecglib/models/architectures/resnet1d.py
+-rw-rw-r--   0 aram      (1002) aram      (1002)     2019 2023-06-20 10:32:40.000000 ecglib-1.1.1/src/ecglib/models/architectures/tabular.py
+drwxrwxr-x   0 aram      (1002) aram      (1002)        0 2023-06-20 12:36:28.535885 ecglib-1.1.1/src/ecglib/models/config/
+-rw-rw-r--   0 aram      (1002) aram      (1002)        0 2023-06-20 10:32:40.000000 ecglib-1.1.1/src/ecglib/models/config/__init__.py
+-rw-rw-r--   0 aram      (1002) aram      (1002)     2639 2023-06-20 10:32:40.000000 ecglib-1.1.1/src/ecglib/models/config/model_configs.py
+-rw-rw-r--   0 aram      (1002) aram      (1002)     1693 2023-06-20 10:32:40.000000 ecglib-1.1.1/src/ecglib/models/config/registred_configs.py
+-rw-rw-r--   0 aram      (1002) aram      (1002)     8734 2023-06-20 10:32:40.000000 ecglib-1.1.1/src/ecglib/models/model_builder.py
+drwxrwxr-x   0 aram      (1002) aram      (1002)        0 2023-06-20 12:36:28.535885 ecglib-1.1.1/src/ecglib/models/weights/
+-rw-rw-r--   0 aram      (1002) aram      (1002)        0 2023-06-20 10:32:40.000000 ecglib-1.1.1/src/ecglib/models/weights/__init__.py
+-rw-rw-r--   0 aram      (1002) aram      (1002)      637 2023-06-20 10:32:40.000000 ecglib-1.1.1/src/ecglib/models/weights/checkpoint.py
+-rw-rw-r--   0 aram      (1002) aram      (1002)     3175 2023-06-20 10:32:40.000000 ecglib-1.1.1/src/ecglib/models/weights/model_weights_paths.yaml
+drwxrwxr-x   0 aram      (1002) aram      (1002)        0 2023-06-20 12:36:28.535885 ecglib-1.1.1/src/ecglib/predict/
+-rw-rw-r--   0 aram      (1002) aram      (1002)       53 2023-06-20 10:32:40.000000 ecglib-1.1.1/src/ecglib/predict/__init__.py
+-rw-rw-r--   0 aram      (1002) aram      (1002)    10332 2023-06-20 10:32:40.000000 ecglib-1.1.1/src/ecglib/predict/predict.py
+drwxrwxr-x   0 aram      (1002) aram      (1002)        0 2023-06-20 12:36:28.535885 ecglib-1.1.1/src/ecglib/preprocessing/
+-rw-rw-r--   0 aram      (1002) aram      (1002)      150 2023-06-20 10:32:40.000000 ecglib-1.1.1/src/ecglib/preprocessing/__init__.py
+-rw-rw-r--   0 aram      (1002) aram      (1002)     2986 2023-06-20 10:32:40.000000 ecglib-1.1.1/src/ecglib/preprocessing/composition.py
+-rw-rw-r--   0 aram      (1002) aram      (1002)     9729 2023-06-20 10:32:40.000000 ecglib-1.1.1/src/ecglib/preprocessing/functional.py
+-rw-rw-r--   0 aram      (1002) aram      (1002)    24523 2023-06-20 10:32:40.000000 ecglib-1.1.1/src/ecglib/preprocessing/preprocess.py
+drwxrwxr-x   0 aram      (1002) aram      (1002)        0 2023-06-20 12:36:28.531885 ecglib-1.1.1/src/ecglib.egg-info/
+-rw-rw-r--   0 aram      (1002) aram      (1002)     7449 2023-06-20 12:36:28.000000 ecglib-1.1.1/src/ecglib.egg-info/PKG-INFO
+-rw-rw-r--   0 aram      (1002) aram      (1002)     1217 2023-06-20 12:36:28.000000 ecglib-1.1.1/src/ecglib.egg-info/SOURCES.txt
+-rw-rw-r--   0 aram      (1002) aram      (1002)        1 2023-06-20 12:36:28.000000 ecglib-1.1.1/src/ecglib.egg-info/dependency_links.txt
+-rw-rw-r--   0 aram      (1002) aram      (1002)      190 2023-06-20 12:36:28.000000 ecglib-1.1.1/src/ecglib.egg-info/requires.txt
+-rw-rw-r--   0 aram      (1002) aram      (1002)        7 2023-06-20 12:36:28.000000 ecglib-1.1.1/src/ecglib.egg-info/top_level.txt
```

### Comparing `ecglib-1.1.0/LICENSE` & `ecglib-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ecglib-1.1.0/README.md` & `ecglib-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ecglib-1.1.0/setup.cfg` & `ecglib-1.1.1/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ecglib
-version = 1.1.0
+version = 1.1.1
 description = ECG library with pretrained models and tools for ECG analysis
 license = Apache License 2.0
 author = Aram Avetisyan
 author_email = a.a.avetisyan@gmail.com
 keywords = {"ecg analysis", "pytorch", "pretrained models", "ecg preprocessing", "ecg datasets"}
 url = https://github.com/ispras/EcgLib
```

### Comparing `ecglib-1.1.0/src/ecglib/data/datasets.py` & `ecglib-1.1.1/src/ecglib/data/datasets.py`

 * *Files identical despite different names*

### Comparing `ecglib-1.1.0/src/ecglib/data/ecg_record.py` & `ecglib-1.1.1/src/ecglib/data/ecg_record.py`

 * *Files identical despite different names*

### Comparing `ecglib-1.1.0/src/ecglib/data/load_datasets.py` & `ecglib-1.1.1/src/ecglib/data/load_datasets.py`

 * *Files identical despite different names*

### Comparing `ecglib-1.1.0/src/ecglib/models/architectures/cnn_tabular.py` & `ecglib-1.1.1/src/ecglib/models/architectures/cnn_tabular.py`

 * *Files identical despite different names*

### Comparing `ecglib-1.1.0/src/ecglib/models/architectures/densenet1d.py` & `ecglib-1.1.1/src/ecglib/models/architectures/densenet1d.py`

 * *Files identical despite different names*

### Comparing `ecglib-1.1.0/src/ecglib/models/architectures/model_types.py` & `ecglib-1.1.1/src/ecglib/models/architectures/model_types.py`

 * *Files identical despite different names*

### Comparing `ecglib-1.1.0/src/ecglib/models/architectures/registred_models.py` & `ecglib-1.1.1/src/ecglib/models/architectures/registred_models.py`

 * *Files identical despite different names*

### Comparing `ecglib-1.1.0/src/ecglib/models/architectures/resnet1d.py` & `ecglib-1.1.1/src/ecglib/models/architectures/resnet1d.py`

 * *Files identical despite different names*

### Comparing `ecglib-1.1.0/src/ecglib/models/architectures/tabular.py` & `ecglib-1.1.1/src/ecglib/models/architectures/tabular.py`

 * *Files identical despite different names*

### Comparing `ecglib-1.1.0/src/ecglib/models/config/model_configs.py` & `ecglib-1.1.1/src/ecglib/models/config/model_configs.py`

 * *Files identical despite different names*

### Comparing `ecglib-1.1.0/src/ecglib/models/config/registred_configs.py` & `ecglib-1.1.1/src/ecglib/models/config/registred_configs.py`

 * *Files identical despite different names*

### Comparing `ecglib-1.1.0/src/ecglib/models/model_builder.py` & `ecglib-1.1.1/src/ecglib/models/model_builder.py`

 * *Files identical despite different names*

### Comparing `ecglib-1.1.0/src/ecglib/models/weights/checkpoint.py` & `ecglib-1.1.1/src/ecglib/models/weights/checkpoint.py`

 * *Files identical despite different names*

### Comparing `ecglib-1.1.0/src/ecglib/models/weights/model_weights_paths.yaml` & `ecglib-1.1.1/src/ecglib/models/weights/model_weights_paths.yaml`

 * *Files identical despite different names*

### Comparing `ecglib-1.1.0/src/ecglib/predict/predict.py` & `ecglib-1.1.1/src/ecglib/predict/predict.py`

 * *Files identical despite different names*

### Comparing `ecglib-1.1.0/src/ecglib/preprocessing/composition.py` & `ecglib-1.1.1/src/ecglib/preprocessing/composition.py`

 * *Files identical despite different names*

### Comparing `ecglib-1.1.0/src/ecglib/preprocessing/functional.py` & `ecglib-1.1.1/src/ecglib/preprocessing/functional.py`

 * *Files identical despite different names*

### Comparing `ecglib-1.1.0/src/ecglib/preprocessing/preprocess.py` & `ecglib-1.1.1/src/ecglib/preprocessing/preprocess.py`

 * *Files identical despite different names*

### Comparing `ecglib-1.1.0/src/ecglib.egg-info/SOURCES.txt` & `ecglib-1.1.1/src/ecglib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

