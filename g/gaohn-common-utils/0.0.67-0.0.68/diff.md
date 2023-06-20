# Comparing `tmp/gaohn-common-utils-0.0.67.tar.gz` & `tmp/gaohn-common-utils-0.0.68.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaohn-common-utils-0.0.67.tar", last modified: Tue Jun 20 03:02:02 2023, max compression
+gzip compressed data, was "gaohn-common-utils-0.0.68.tar", last modified: Tue Jun 20 03:13:13 2023, max compression
```

## Comparing `gaohn-common-utils-0.0.67.tar` & `gaohn-common-utils-0.0.68.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:02:02.906041 gaohn-common-utils-0.0.67/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-20 03:01:40.000000 gaohn-common-utils-0.0.67/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-20 03:02:02.906041 gaohn-common-utils-0.0.67/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-06-20 03:01:40.000000 gaohn-common-utils-0.0.67/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:02:02.902041 gaohn-common-utils-0.0.67/common_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 03:01:40.000000 gaohn-common-utils-0.0.67/common_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:02:02.902041 gaohn-common-utils-0.0.67/common_utils/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-20 03:01:40.000000 gaohn-common-utils-0.0.67/common_utils/cloud/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:02:02.902041 gaohn-common-utils-0.0.67/common_utils/cloud/gcp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:02:02.902041 gaohn-common-utils-0.0.67/common_utils/cloud/gcp/database/
--rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-20 03:01:40.000000 gaohn-common-utils-0.0.67/common_utils/cloud/gcp/database/bigquery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:02:02.902041 gaohn-common-utils-0.0.67/common_utils/cloud/gcp/storage/
--rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-06-20 03:01:40.000000 gaohn-common-utils-0.0.67/common_utils/cloud/gcp/storage/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:02:02.902041 gaohn-common-utils-0.0.67/common_utils/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 03:01:40.000000 gaohn-common-utils-0.0.67/common_utils/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 03:01:40.000000 gaohn-common-utils-0.0.67/common_utils/core/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-20 03:01:40.000000 gaohn-common-utils-0.0.67/common_utils/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-06-20 03:01:40.000000 gaohn-common-utils-0.0.67/common_utils/core/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-20 03:01:40.000000 gaohn-common-utils-0.0.67/common_utils/core/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-20 03:01:40.000000 gaohn-common-utils-0.0.67/common_utils/core/file_system_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-06-20 03:01:40.000000 gaohn-common-utils-0.0.67/common_utils/core/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:02:02.902041 gaohn-common-utils-0.0.67/common_utils/data_validator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 03:01:40.000000 gaohn-common-utils-0.0.67/common_utils/data_validator/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-20 03:01:40.000000 gaohn-common-utils-0.0.67/common_utils/data_validator/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:02:02.902041 gaohn-common-utils-0.0.67/common_utils/experiment_tracking/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:02:02.902041 gaohn-common-utils-0.0.67/common_utils/experiment_tracking/promoter/
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-20 03:01:40.000000 gaohn-common-utils-0.0.67/common_utils/experiment_tracking/promoter/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9057 2023-06-20 03:01:40.000000 gaohn-common-utils-0.0.67/common_utils/experiment_tracking/promoter/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:02:02.902041 gaohn-common-utils-0.0.67/common_utils/orchestrator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 03:01:40.000000 gaohn-common-utils-0.0.67/common_utils/orchestrator/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:02:02.902041 gaohn-common-utils-0.0.67/common_utils/versioning/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:02:02.902041 gaohn-common-utils-0.0.67/common_utils/versioning/dvc/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-20 03:01:40.000000 gaohn-common-utils-0.0.67/common_utils/versioning/dvc/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-06-20 03:01:40.000000 gaohn-common-utils-0.0.67/common_utils/versioning/dvc/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:02:02.902041 gaohn-common-utils-0.0.67/common_utils/versioning/git/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 03:01:40.000000 gaohn-common-utils-0.0.67/common_utils/versioning/git/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-20 03:01:40.000000 gaohn-common-utils-0.0.67/common_utils/versioning/git/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:02:02.906041 gaohn-common-utils-0.0.67/gaohn_common_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-20 03:02:02.000000 gaohn-common-utils-0.0.67/gaohn_common_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-20 03:02:02.000000 gaohn-common-utils-0.0.67/gaohn_common_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 03:02:02.000000 gaohn-common-utils-0.0.67/gaohn_common_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-20 03:02:02.000000 gaohn-common-utils-0.0.67/gaohn_common_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-20 03:02:02.000000 gaohn-common-utils-0.0.67/gaohn_common_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-20 03:01:40.000000 gaohn-common-utils-0.0.67/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 03:02:02.906041 gaohn-common-utils-0.0.67/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:13:13.155365 gaohn-common-utils-0.0.68/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-20 03:12:50.000000 gaohn-common-utils-0.0.68/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-20 03:13:13.155365 gaohn-common-utils-0.0.68/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-06-20 03:12:50.000000 gaohn-common-utils-0.0.68/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:13:13.151364 gaohn-common-utils-0.0.68/common_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 03:12:50.000000 gaohn-common-utils-0.0.68/common_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:13:13.151364 gaohn-common-utils-0.0.68/common_utils/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-20 03:12:50.000000 gaohn-common-utils-0.0.68/common_utils/cloud/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:13:13.147364 gaohn-common-utils-0.0.68/common_utils/cloud/gcp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:13:13.151364 gaohn-common-utils-0.0.68/common_utils/cloud/gcp/database/
+-rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-20 03:12:50.000000 gaohn-common-utils-0.0.68/common_utils/cloud/gcp/database/bigquery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:13:13.151364 gaohn-common-utils-0.0.68/common_utils/cloud/gcp/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-06-20 03:12:50.000000 gaohn-common-utils-0.0.68/common_utils/cloud/gcp/storage/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:13:13.151364 gaohn-common-utils-0.0.68/common_utils/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 03:12:50.000000 gaohn-common-utils-0.0.68/common_utils/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 03:12:50.000000 gaohn-common-utils-0.0.68/common_utils/core/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-20 03:12:50.000000 gaohn-common-utils-0.0.68/common_utils/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-06-20 03:12:50.000000 gaohn-common-utils-0.0.68/common_utils/core/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-20 03:12:50.000000 gaohn-common-utils-0.0.68/common_utils/core/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-20 03:12:50.000000 gaohn-common-utils-0.0.68/common_utils/core/file_system_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-06-20 03:12:50.000000 gaohn-common-utils-0.0.68/common_utils/core/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:13:13.151364 gaohn-common-utils-0.0.68/common_utils/data_validator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 03:12:50.000000 gaohn-common-utils-0.0.68/common_utils/data_validator/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-20 03:12:50.000000 gaohn-common-utils-0.0.68/common_utils/data_validator/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:13:13.151364 gaohn-common-utils-0.0.68/common_utils/experiment_tracking/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:13:13.151364 gaohn-common-utils-0.0.68/common_utils/experiment_tracking/promoter/
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-20 03:12:50.000000 gaohn-common-utils-0.0.68/common_utils/experiment_tracking/promoter/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9487 2023-06-20 03:12:50.000000 gaohn-common-utils-0.0.68/common_utils/experiment_tracking/promoter/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:13:13.151364 gaohn-common-utils-0.0.68/common_utils/orchestrator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 03:12:50.000000 gaohn-common-utils-0.0.68/common_utils/orchestrator/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:13:13.151364 gaohn-common-utils-0.0.68/common_utils/versioning/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:13:13.151364 gaohn-common-utils-0.0.68/common_utils/versioning/dvc/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-20 03:12:50.000000 gaohn-common-utils-0.0.68/common_utils/versioning/dvc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-06-20 03:12:50.000000 gaohn-common-utils-0.0.68/common_utils/versioning/dvc/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:13:13.155365 gaohn-common-utils-0.0.68/common_utils/versioning/git/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 03:12:50.000000 gaohn-common-utils-0.0.68/common_utils/versioning/git/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-20 03:12:50.000000 gaohn-common-utils-0.0.68/common_utils/versioning/git/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:13:13.155365 gaohn-common-utils-0.0.68/gaohn_common_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-20 03:13:13.000000 gaohn-common-utils-0.0.68/gaohn_common_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-20 03:13:13.000000 gaohn-common-utils-0.0.68/gaohn_common_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 03:13:13.000000 gaohn-common-utils-0.0.68/gaohn_common_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-20 03:13:13.000000 gaohn-common-utils-0.0.68/gaohn_common_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-20 03:13:13.000000 gaohn-common-utils-0.0.68/gaohn_common_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-20 03:12:50.000000 gaohn-common-utils-0.0.68/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 03:13:13.155365 gaohn-common-utils-0.0.68/setup.cfg
```

### Comparing `gaohn-common-utils-0.0.67/LICENSE` & `gaohn-common-utils-0.0.68/LICENSE`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.67/PKG-INFO` & `gaohn-common-utils-0.0.68/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.67
+Version: 0.0.68
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.67/README.md` & `gaohn-common-utils-0.0.68/README.md`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.67/common_utils/cloud/base.py` & `gaohn-common-utils-0.0.68/common_utils/cloud/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.67/common_utils/cloud/gcp/database/bigquery.py` & `gaohn-common-utils-0.0.68/common_utils/cloud/gcp/database/bigquery.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.67/common_utils/cloud/gcp/storage/gcs.py` & `gaohn-common-utils-0.0.68/common_utils/cloud/gcp/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.67/common_utils/core/base.py` & `gaohn-common-utils-0.0.68/common_utils/core/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.67/common_utils/core/common.py` & `gaohn-common-utils-0.0.68/common_utils/core/common.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.67/common_utils/core/decorators.py` & `gaohn-common-utils-0.0.68/common_utils/core/decorators.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.67/common_utils/core/file_system_utils.py` & `gaohn-common-utils-0.0.68/common_utils/core/file_system_utils.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.67/common_utils/core/logger.py` & `gaohn-common-utils-0.0.68/common_utils/core/logger.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.67/common_utils/data_validator/core.py` & `gaohn-common-utils-0.0.68/common_utils/data_validator/core.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.67/common_utils/experiment_tracking/promoter/base.py` & `gaohn-common-utils-0.0.68/common_utils/experiment_tracking/promoter/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
-from typing import Dict, List
+from typing import Dict, List, Optional
 
 
 @dataclass
 class ModelVersion:
     """
     A class representing a version of an ML model.
 
     This class follows the Value Object pattern, as each instance represents
     a version of a model and its associated properties without a specific
     identity.
 
     NOTE: Be aware of potential namespace conflicts with Mlflow's
-    ModelVersion class.
+    ModelVersion class (ModelVersion).
 
     Single Responsibility Principle is followed, as the class solely
     encapsulates the logic related to a model version.
 
     Attributes
     ----------
     version : int
@@ -26,20 +26,20 @@
         Performance metrics as a dictionary, e.g., {'accuracy': 0.95}.
     stage : str
         Stage of the model version, e.g., 'production'.
     """
 
     version: int
     metrics: Dict[str, float]
-    stage: str
+    stage: Optional[str] = None
 
 
 class ModelClient(ABC):
     """All subclasses must implement these methods. See MLFlow Client
-    as an example."""
+    as an example (MlflowClient)."""
 
     @abstractmethod
     def get_latest_versions(
         self, model_name: str, stages: List[str]
     ) -> List[ModelVersion]:
         """Get the latest versions of a model."""
```

### Comparing `gaohn-common-utils-0.0.67/common_utils/experiment_tracking/promoter/core.py` & `gaohn-common-utils-0.0.68/common_utils/experiment_tracking/promoter/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 This script handles promoting a model to production.
 Simple logic is if the new model is better than the current production model, then promote it to production.
 Of course in real life, you might want to implement more robust model comparison logic and
 implement a manual approval step before promoting the model to production. Include A/B testing too.
 """
 
-from typing import List, Literal
+from typing import List, Literal, Optional
 
 from common_utils.core.logger import Logger
 from common_utils.experiment_tracking.promoter.base import ModelClient, ModelVersion
 
 
 class ModelPromotionManager:
     """A class that manages the promotion of machine learning models to production.
@@ -62,22 +62,27 @@
     modification (you don't have to change the ModelPromotionManager class to add
     new clients).
     """
 
     def __init__(
         self,
         client: ModelClient,
-        logger: Logger,
         model_name: str,
+        logger: Optional[Logger] = None,
     ) -> None:
         self.client = client
-        self.logger = logger
-
         self.model_name = model_name
 
+        if logger is None:
+            self.logger = Logger(
+                module_name=__name__, propagate=False, log_root_dir=None, log_file=None
+            ).logger
+        else:
+            self.logger = logger
+
     def _check_if_there_exists_production_model(self) -> Literal[True, False]:
         return len(self._get_all_production_models()) > 0
 
     def _get_all_production_models(self) -> List:
         production_models = self.client.get_latest_versions(
             self.model_name, stages=["Production"]
         )
@@ -97,14 +102,15 @@
         # get the latest production model
         latest_production_model = sorted_production_models[0]
         run_id = latest_production_model.run_id
         run = self.client.get_run(run_id)
         return ModelVersion(
             version=latest_production_model.version,
             metrics=run.data.metrics,
+            stage=latest_production_model.current_stage,
         )
 
     def _find_best_model_for_production(
         self, metric_name: str = "test_f1"
     ) -> ModelVersion:
         """
         Find the best model to promote to production based on the metric score.
@@ -118,15 +124,15 @@
             )
             for version in model_versions
         ]
         model_versions_metrics = [x for x in model_versions_metrics if x[1] is not None]
         best_model_version, best_model_metrics = max(
             model_versions_metrics, key=lambda x: x[1]
         )
-        return ModelVersion(best_model_version, best_model_metrics)
+        return ModelVersion(best_model_version, best_model_metrics, "Production")
 
     def _compare_models(
         self,
         model1: ModelVersion,
         model2: ModelVersion,
         metric_name: str = "test_f1",
     ) -> bool:
@@ -185,19 +191,22 @@
             non_production_latest_model = self.client.get_latest_versions(
                 self.model_name, stages=["None"]
             )[0]
 
             # get the model version number and metrics
             latest_curr_model_version = non_production_latest_model.version
             latest_curr_model_run_id = non_production_latest_model.run_id
+            latest_curr_model_stage = non_production_latest_model.current_stage
             latest_curr_model_run = self.client.get_run(latest_curr_model_run_id)
 
             latest_curr_model_metrics = latest_curr_model_run.data.metrics
             latest_curr_model: ModelVersion = ModelVersion(
-                version=latest_curr_model_version, metrics=latest_curr_model_metrics
+                version=latest_curr_model_version,
+                metrics=latest_curr_model_metrics,
+                stage=latest_curr_model_stage,
             )
 
             if not self._compare_models(
                 model1=latest_curr_model, model2=latest_production_model
             ):
                 self.logger.info(
                     f"Model {self.model_name} version {latest_curr_model_version} does not outperform the current production model."
```

### Comparing `gaohn-common-utils-0.0.67/common_utils/versioning/dvc/core.py` & `gaohn-common-utils-0.0.68/common_utils/versioning/dvc/core.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.67/common_utils/versioning/git/core.py` & `gaohn-common-utils-0.0.68/common_utils/versioning/git/core.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.67/gaohn_common_utils.egg-info/PKG-INFO` & `gaohn-common-utils-0.0.68/gaohn_common_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.67
+Version: 0.0.68
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.67/gaohn_common_utils.egg-info/SOURCES.txt` & `gaohn-common-utils-0.0.68/gaohn_common_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.67/pyproject.toml` & `gaohn-common-utils-0.0.68/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gaohn-common-utils"
-version = "0.0.67"
+version = "0.0.68"
 authors = [
   { name="Gao Hongnan", email="hongnangao@gmail.com" },
 ]
 description = "A small utility package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

