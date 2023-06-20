# Comparing `tmp/proteus_cli-0.3.7.tar.gz` & `tmp/proteus_cli-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteus_cli-0.3.7.tar", max compression
+gzip compressed data, was "proteus_cli-0.3.8.tar", max compression
```

## Comparing `proteus_cli-0.3.7.tar` & `proteus_cli-0.3.8.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     3083 2023-06-20 16:50:25.212463 proteus_cli-0.3.7/cli/__init__.py
--rw-r--r--   0        0        0      384 2023-06-20 16:50:25.212463 proteus_cli-0.3.7/cli/api/__init__.py
--rw-r--r--   0        0        0     1784 2023-06-20 16:50:25.212463 proteus_cli-0.3.7/cli/api/decorators.py
--rw-r--r--   0        0        0      849 2023-06-20 16:50:25.212463 proteus_cli-0.3.7/cli/api/hooks.py
--rw-r--r--   0        0        0        0 2023-06-20 16:50:25.212463 proteus_cli-0.3.7/cli/buckets/__init__.py
--rw-r--r--   0        0        0     1092 2023-06-20 16:50:25.212463 proteus_cli-0.3.7/cli/buckets/commands.py
--rw-r--r--   0        0        0     2810 2023-06-20 16:50:25.212463 proteus_cli-0.3.7/cli/config.py
--rw-r--r--   0        0        0        0 2023-06-20 16:50:25.212463 proteus_cli-0.3.7/cli/datasets/__init__.py
--rw-r--r--   0        0        0     1332 2023-06-20 16:50:25.212463 proteus_cli-0.3.7/cli/datasets/commands.py
--rw-r--r--   0        0        0        0 2023-06-20 16:50:25.212463 proteus_cli-0.3.7/cli/datasets/preprocessor/__init__.py
--rw-r--r--   0        0        0      939 2023-06-20 16:50:25.212463 proteus_cli-0.3.7/cli/datasets/preprocessor/config/__init__.py
--rw-r--r--   0        0        0      323 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/datasets/preprocessor/config/case/__init__.py
--rw-r--r--   0        0        0      958 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/datasets/preprocessor/config/case/cnn_pca.py
--rw-r--r--   0        0        0     3447 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/datasets/preprocessor/config/case/hm.py
--rw-r--r--   0        0        0     3054 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/datasets/preprocessor/config/case/well_model.py
--rw-r--r--   0        0        0      446 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/datasets/preprocessor/config/common/__init__.py
--rw-r--r--   0        0        0     3251 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/datasets/preprocessor/config/common/cnn_pca.py
--rw-r--r--   0        0        0     2009 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/datasets/preprocessor/config/common/hm.py
--rw-r--r--   0        0        0     1542 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/datasets/preprocessor/config/common/well_model.py
--rw-r--r--   0        0        0     2665 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/datasets/preprocessor/config/default.py
--rw-r--r--   0        0        0      418 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/datasets/preprocessor/config/step/__init__.py
--rw-r--r--   0        0        0      125 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/datasets/preprocessor/config/step/cnn_pca.py
--rw-r--r--   0        0        0     2415 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/datasets/preprocessor/config/step/hm.py
--rw-r--r--   0        0        0      128 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/datasets/preprocessor/config/step/well_model.py
--rw-r--r--   0        0        0      673 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/datasets/preprocessor/init_keywords.json
--rw-r--r--   0        0        0    14707 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/datasets/preprocessor/preprocess_functions.py
--rw-r--r--   0        0        0     4944 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/datasets/preprocessor/process_step.py
--rw-r--r--   0        0        0     8656 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/datasets/preprocessor/utils.py
--rw-r--r--   0        0        0      411 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/datasets/preprocessor/well_init_keywords.json
--rw-r--r--   0        0        0        0 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/datasets/sources/__init__.py
--rw-r--r--   0        0        0     5927 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/datasets/sources/az.py
--rw-r--r--   0        0        0      824 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/datasets/sources/common.py
--rw-r--r--   0        0        0     2809 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/datasets/sources/local.py
--rw-r--r--   0        0        0     1783 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/datasets/sources/s3.py
--rw-r--r--   0        0        0     9158 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/datasets/upload.py
--rw-r--r--   0        0        0        0 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/debugger/__init__.py
--rw-r--r--   0        0        0     2265 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/debugger/commands.py
--rw-r--r--   0        0        0     3926 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/debugger/init_keyword_check.py
--rw-r--r--   0        0        0        0 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/debugger/restart_keyword_check.py
--rw-r--r--   0        0        0        0 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/jobs/__init__.py
--rw-r--r--   0        0        0     1283 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/jobs/commands.py
--rw-r--r--   0        0        0     3026 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/jobs/list.py
--rw-r--r--   0        0        0      100 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/runtime.py
--rw-r--r--   0        0        0        0 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/simulations/__init__.py
--rw-r--r--   0        0        0     2460 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/simulations/commands.py
--rw-r--r--   0        0        0     7603 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/simulations/create.py
--rw-r--r--   0        0        0     4119 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/simulations/dependencySolver.py
--rw-r--r--   0        0        0     5190 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/simulations/opm.py
--rw-r--r--   0        0        0      449 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/logging.ini
--rw-r--r--   0        0        0     1530 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/pyproject.toml
--rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 proteus_cli-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0     3083 2023-06-20 17:12:06.060060 proteus_cli-0.3.8/cli/__init__.py
+-rw-r--r--   0        0        0      384 2023-06-20 17:12:06.060060 proteus_cli-0.3.8/cli/api/__init__.py
+-rw-r--r--   0        0        0     1784 2023-06-20 17:12:06.060060 proteus_cli-0.3.8/cli/api/decorators.py
+-rw-r--r--   0        0        0      849 2023-06-20 17:12:06.060060 proteus_cli-0.3.8/cli/api/hooks.py
+-rw-r--r--   0        0        0        0 2023-06-20 17:12:06.060060 proteus_cli-0.3.8/cli/buckets/__init__.py
+-rw-r--r--   0        0        0     1092 2023-06-20 17:12:06.060060 proteus_cli-0.3.8/cli/buckets/commands.py
+-rw-r--r--   0        0        0     2810 2023-06-20 17:12:06.060060 proteus_cli-0.3.8/cli/config.py
+-rw-r--r--   0        0        0        0 2023-06-20 17:12:06.060060 proteus_cli-0.3.8/cli/datasets/__init__.py
+-rw-r--r--   0        0        0     1332 2023-06-20 17:12:06.060060 proteus_cli-0.3.8/cli/datasets/commands.py
+-rw-r--r--   0        0        0        0 2023-06-20 17:12:06.060060 proteus_cli-0.3.8/cli/datasets/preprocessor/__init__.py
+-rw-r--r--   0        0        0      939 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/datasets/preprocessor/config/__init__.py
+-rw-r--r--   0        0        0      323 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/datasets/preprocessor/config/case/__init__.py
+-rw-r--r--   0        0        0      958 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/datasets/preprocessor/config/case/cnn_pca.py
+-rw-r--r--   0        0        0     3447 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/datasets/preprocessor/config/case/hm.py
+-rw-r--r--   0        0        0     3054 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/datasets/preprocessor/config/case/well_model.py
+-rw-r--r--   0        0        0      446 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/datasets/preprocessor/config/common/__init__.py
+-rw-r--r--   0        0        0     3251 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/datasets/preprocessor/config/common/cnn_pca.py
+-rw-r--r--   0        0        0     2009 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/datasets/preprocessor/config/common/hm.py
+-rw-r--r--   0        0        0     1542 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/datasets/preprocessor/config/common/well_model.py
+-rw-r--r--   0        0        0     2665 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/datasets/preprocessor/config/default.py
+-rw-r--r--   0        0        0      418 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/datasets/preprocessor/config/step/__init__.py
+-rw-r--r--   0        0        0      125 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/datasets/preprocessor/config/step/cnn_pca.py
+-rw-r--r--   0        0        0     2415 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/datasets/preprocessor/config/step/hm.py
+-rw-r--r--   0        0        0      128 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/datasets/preprocessor/config/step/well_model.py
+-rw-r--r--   0        0        0      673 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/datasets/preprocessor/init_keywords.json
+-rw-r--r--   0        0        0    14707 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/datasets/preprocessor/preprocess_functions.py
+-rw-r--r--   0        0        0     4944 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/datasets/preprocessor/process_step.py
+-rw-r--r--   0        0        0     8656 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/datasets/preprocessor/utils.py
+-rw-r--r--   0        0        0      411 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/datasets/preprocessor/well_init_keywords.json
+-rw-r--r--   0        0        0        0 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/datasets/sources/__init__.py
+-rw-r--r--   0        0        0     5927 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/datasets/sources/az.py
+-rw-r--r--   0        0        0      824 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/datasets/sources/common.py
+-rw-r--r--   0        0        0     2809 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/datasets/sources/local.py
+-rw-r--r--   0        0        0     1783 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/datasets/sources/s3.py
+-rw-r--r--   0        0        0     9158 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/datasets/upload.py
+-rw-r--r--   0        0        0        0 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/debugger/__init__.py
+-rw-r--r--   0        0        0     2265 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/debugger/commands.py
+-rw-r--r--   0        0        0     3926 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/debugger/init_keyword_check.py
+-rw-r--r--   0        0        0        0 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/debugger/restart_keyword_check.py
+-rw-r--r--   0        0        0        0 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/jobs/__init__.py
+-rw-r--r--   0        0        0     1283 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/jobs/commands.py
+-rw-r--r--   0        0        0     3026 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/jobs/list.py
+-rw-r--r--   0        0        0      100 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/runtime.py
+-rw-r--r--   0        0        0        0 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/simulations/__init__.py
+-rw-r--r--   0        0        0     2460 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/simulations/commands.py
+-rw-r--r--   0        0        0     7603 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/simulations/create.py
+-rw-r--r--   0        0        0     4119 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/simulations/dependencySolver.py
+-rw-r--r--   0        0        0     5190 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/simulations/opm.py
+-rw-r--r--   0        0        0      449 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/logging.ini
+-rw-r--r--   0        0        0     1530 2023-06-20 17:12:06.068058 proteus_cli-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 proteus_cli-0.3.8/PKG-INFO
```

### Comparing `proteus_cli-0.3.7/cli/__init__.py` & `proteus_cli-0.3.8/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.7/cli/api/decorators.py` & `proteus_cli-0.3.8/cli/api/decorators.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.7/cli/api/hooks.py` & `proteus_cli-0.3.8/cli/api/hooks.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.7/cli/buckets/commands.py` & `proteus_cli-0.3.8/cli/buckets/commands.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.7/cli/config.py` & `proteus_cli-0.3.8/cli/config.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.7/cli/datasets/commands.py` & `proteus_cli-0.3.8/cli/datasets/commands.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.7/cli/datasets/preprocessor/config/__init__.py` & `proteus_cli-0.3.8/cli/datasets/preprocessor/config/__init__.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.7/cli/datasets/preprocessor/config/case/cnn_pca.py` & `proteus_cli-0.3.8/cli/datasets/preprocessor/config/case/cnn_pca.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.7/cli/datasets/preprocessor/config/case/hm.py` & `proteus_cli-0.3.8/cli/datasets/preprocessor/config/case/hm.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.7/cli/datasets/preprocessor/config/case/well_model.py` & `proteus_cli-0.3.8/cli/datasets/preprocessor/config/case/well_model.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.7/cli/datasets/preprocessor/config/common/cnn_pca.py` & `proteus_cli-0.3.8/cli/datasets/preprocessor/config/common/cnn_pca.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.7/cli/datasets/preprocessor/config/common/hm.py` & `proteus_cli-0.3.8/cli/datasets/preprocessor/config/common/hm.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.7/cli/datasets/preprocessor/config/common/well_model.py` & `proteus_cli-0.3.8/cli/datasets/preprocessor/config/common/well_model.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.7/cli/datasets/preprocessor/config/default.py` & `proteus_cli-0.3.8/cli/datasets/preprocessor/config/default.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.7/cli/datasets/preprocessor/config/step/hm.py` & `proteus_cli-0.3.8/cli/datasets/preprocessor/config/step/hm.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.7/cli/datasets/preprocessor/init_keywords.json` & `proteus_cli-0.3.8/cli/datasets/preprocessor/init_keywords.json`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.7/cli/datasets/preprocessor/preprocess_functions.py` & `proteus_cli-0.3.8/cli/datasets/preprocessor/preprocess_functions.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.7/cli/datasets/preprocessor/process_step.py` & `proteus_cli-0.3.8/cli/datasets/preprocessor/process_step.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.7/cli/datasets/preprocessor/utils.py` & `proteus_cli-0.3.8/cli/datasets/preprocessor/utils.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.7/cli/datasets/sources/az.py` & `proteus_cli-0.3.8/cli/datasets/sources/az.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.7/cli/datasets/sources/common.py` & `proteus_cli-0.3.8/cli/datasets/sources/common.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.7/cli/datasets/sources/local.py` & `proteus_cli-0.3.8/cli/datasets/sources/local.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.7/cli/datasets/sources/s3.py` & `proteus_cli-0.3.8/cli/datasets/sources/s3.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.7/cli/datasets/upload.py` & `proteus_cli-0.3.8/cli/datasets/upload.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.7/cli/debugger/commands.py` & `proteus_cli-0.3.8/cli/debugger/commands.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.7/cli/debugger/init_keyword_check.py` & `proteus_cli-0.3.8/cli/debugger/init_keyword_check.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.7/cli/jobs/commands.py` & `proteus_cli-0.3.8/cli/jobs/commands.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.7/cli/jobs/list.py` & `proteus_cli-0.3.8/cli/jobs/list.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.7/cli/simulations/commands.py` & `proteus_cli-0.3.8/cli/simulations/commands.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.7/cli/simulations/create.py` & `proteus_cli-0.3.8/cli/simulations/create.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.7/cli/simulations/dependencySolver.py` & `proteus_cli-0.3.8/cli/simulations/dependencySolver.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.7/cli/simulations/opm.py` & `proteus_cli-0.3.8/cli/simulations/opm.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.7/pyproject.toml` & `proteus_cli-0.3.8/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "proteus-cli"
-version = "0.3.7"
+version = "0.3.8"
 description = ""
 authors = []
 packages = [
     {include="cli"},
     {include="logging.ini"}
 ]
```

### Comparing `proteus_cli-0.3.7/PKG-INFO` & `proteus_cli-0.3.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proteus-cli
-Version: 0.3.7
+Version: 0.3.8
 Summary: 
 Requires-Python: >=3.8,<3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Dist: azure-identity (>=1.12.0,<2.0.0)
 Requires-Dist: azure-storage-blob (>=12.8.1,<13.0.0)
 Requires-Dist: boto3 (>=1.17.79,<2.0.0)
```

