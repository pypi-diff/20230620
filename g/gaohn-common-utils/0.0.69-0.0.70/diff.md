# Comparing `tmp/gaohn-common-utils-0.0.69.tar.gz` & `tmp/gaohn-common-utils-0.0.70.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaohn-common-utils-0.0.69.tar", last modified: Tue Jun 20 03:26:17 2023, max compression
+gzip compressed data, was "gaohn-common-utils-0.0.70.tar", last modified: Tue Jun 20 03:29:28 2023, max compression
```

## Comparing `gaohn-common-utils-0.0.69.tar` & `gaohn-common-utils-0.0.70.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:26:17.832800 gaohn-common-utils-0.0.69/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-20 03:25:59.000000 gaohn-common-utils-0.0.69/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-20 03:26:17.832800 gaohn-common-utils-0.0.69/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-06-20 03:25:59.000000 gaohn-common-utils-0.0.69/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:26:17.828800 gaohn-common-utils-0.0.69/common_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 03:25:59.000000 gaohn-common-utils-0.0.69/common_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:26:17.828800 gaohn-common-utils-0.0.69/common_utils/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-20 03:25:59.000000 gaohn-common-utils-0.0.69/common_utils/cloud/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:26:17.828800 gaohn-common-utils-0.0.69/common_utils/cloud/gcp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:26:17.828800 gaohn-common-utils-0.0.69/common_utils/cloud/gcp/database/
--rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-20 03:25:59.000000 gaohn-common-utils-0.0.69/common_utils/cloud/gcp/database/bigquery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:26:17.828800 gaohn-common-utils-0.0.69/common_utils/cloud/gcp/storage/
--rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-06-20 03:25:59.000000 gaohn-common-utils-0.0.69/common_utils/cloud/gcp/storage/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:26:17.828800 gaohn-common-utils-0.0.69/common_utils/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 03:25:59.000000 gaohn-common-utils-0.0.69/common_utils/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 03:25:59.000000 gaohn-common-utils-0.0.69/common_utils/core/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-20 03:25:59.000000 gaohn-common-utils-0.0.69/common_utils/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-06-20 03:25:59.000000 gaohn-common-utils-0.0.69/common_utils/core/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-20 03:25:59.000000 gaohn-common-utils-0.0.69/common_utils/core/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-20 03:25:59.000000 gaohn-common-utils-0.0.69/common_utils/core/file_system_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-06-20 03:25:59.000000 gaohn-common-utils-0.0.69/common_utils/core/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:26:17.828800 gaohn-common-utils-0.0.69/common_utils/data_validator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 03:25:59.000000 gaohn-common-utils-0.0.69/common_utils/data_validator/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-20 03:25:59.000000 gaohn-common-utils-0.0.69/common_utils/data_validator/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:26:17.828800 gaohn-common-utils-0.0.69/common_utils/experiment_tracking/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:26:17.828800 gaohn-common-utils-0.0.69/common_utils/experiment_tracking/promoter/
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-20 03:25:59.000000 gaohn-common-utils-0.0.69/common_utils/experiment_tracking/promoter/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9973 2023-06-20 03:25:59.000000 gaohn-common-utils-0.0.69/common_utils/experiment_tracking/promoter/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:26:17.828800 gaohn-common-utils-0.0.69/common_utils/orchestrator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 03:25:59.000000 gaohn-common-utils-0.0.69/common_utils/orchestrator/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:26:17.828800 gaohn-common-utils-0.0.69/common_utils/versioning/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:26:17.832800 gaohn-common-utils-0.0.69/common_utils/versioning/dvc/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-20 03:25:59.000000 gaohn-common-utils-0.0.69/common_utils/versioning/dvc/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-06-20 03:25:59.000000 gaohn-common-utils-0.0.69/common_utils/versioning/dvc/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:26:17.832800 gaohn-common-utils-0.0.69/common_utils/versioning/git/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 03:25:59.000000 gaohn-common-utils-0.0.69/common_utils/versioning/git/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-20 03:25:59.000000 gaohn-common-utils-0.0.69/common_utils/versioning/git/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:26:17.832800 gaohn-common-utils-0.0.69/gaohn_common_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-20 03:26:17.000000 gaohn-common-utils-0.0.69/gaohn_common_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-20 03:26:17.000000 gaohn-common-utils-0.0.69/gaohn_common_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 03:26:17.000000 gaohn-common-utils-0.0.69/gaohn_common_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-20 03:26:17.000000 gaohn-common-utils-0.0.69/gaohn_common_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-20 03:26:17.000000 gaohn-common-utils-0.0.69/gaohn_common_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-20 03:25:59.000000 gaohn-common-utils-0.0.69/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 03:26:17.832800 gaohn-common-utils-0.0.69/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:29:28.846063 gaohn-common-utils-0.0.70/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-20 03:29:08.000000 gaohn-common-utils-0.0.70/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-20 03:29:28.846063 gaohn-common-utils-0.0.70/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-06-20 03:29:08.000000 gaohn-common-utils-0.0.70/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:29:28.838063 gaohn-common-utils-0.0.70/common_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 03:29:08.000000 gaohn-common-utils-0.0.70/common_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:29:28.842063 gaohn-common-utils-0.0.70/common_utils/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-20 03:29:08.000000 gaohn-common-utils-0.0.70/common_utils/cloud/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:29:28.838063 gaohn-common-utils-0.0.70/common_utils/cloud/gcp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:29:28.842063 gaohn-common-utils-0.0.70/common_utils/cloud/gcp/database/
+-rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-20 03:29:08.000000 gaohn-common-utils-0.0.70/common_utils/cloud/gcp/database/bigquery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:29:28.842063 gaohn-common-utils-0.0.70/common_utils/cloud/gcp/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-06-20 03:29:08.000000 gaohn-common-utils-0.0.70/common_utils/cloud/gcp/storage/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:29:28.842063 gaohn-common-utils-0.0.70/common_utils/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 03:29:08.000000 gaohn-common-utils-0.0.70/common_utils/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 03:29:08.000000 gaohn-common-utils-0.0.70/common_utils/core/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-20 03:29:08.000000 gaohn-common-utils-0.0.70/common_utils/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-06-20 03:29:08.000000 gaohn-common-utils-0.0.70/common_utils/core/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-20 03:29:08.000000 gaohn-common-utils-0.0.70/common_utils/core/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-20 03:29:08.000000 gaohn-common-utils-0.0.70/common_utils/core/file_system_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-06-20 03:29:08.000000 gaohn-common-utils-0.0.70/common_utils/core/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:29:28.842063 gaohn-common-utils-0.0.70/common_utils/data_validator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 03:29:08.000000 gaohn-common-utils-0.0.70/common_utils/data_validator/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-20 03:29:08.000000 gaohn-common-utils-0.0.70/common_utils/data_validator/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:29:28.838063 gaohn-common-utils-0.0.70/common_utils/experiment_tracking/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:29:28.842063 gaohn-common-utils-0.0.70/common_utils/experiment_tracking/promoter/
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-20 03:29:08.000000 gaohn-common-utils-0.0.70/common_utils/experiment_tracking/promoter/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9567 2023-06-20 03:29:08.000000 gaohn-common-utils-0.0.70/common_utils/experiment_tracking/promoter/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:29:28.842063 gaohn-common-utils-0.0.70/common_utils/orchestrator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 03:29:08.000000 gaohn-common-utils-0.0.70/common_utils/orchestrator/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:29:28.838063 gaohn-common-utils-0.0.70/common_utils/versioning/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:29:28.842063 gaohn-common-utils-0.0.70/common_utils/versioning/dvc/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-20 03:29:08.000000 gaohn-common-utils-0.0.70/common_utils/versioning/dvc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-06-20 03:29:08.000000 gaohn-common-utils-0.0.70/common_utils/versioning/dvc/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:29:28.842063 gaohn-common-utils-0.0.70/common_utils/versioning/git/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 03:29:08.000000 gaohn-common-utils-0.0.70/common_utils/versioning/git/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-20 03:29:08.000000 gaohn-common-utils-0.0.70/common_utils/versioning/git/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:29:28.842063 gaohn-common-utils-0.0.70/gaohn_common_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-20 03:29:28.000000 gaohn-common-utils-0.0.70/gaohn_common_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-20 03:29:28.000000 gaohn-common-utils-0.0.70/gaohn_common_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 03:29:28.000000 gaohn-common-utils-0.0.70/gaohn_common_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-20 03:29:28.000000 gaohn-common-utils-0.0.70/gaohn_common_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-20 03:29:28.000000 gaohn-common-utils-0.0.70/gaohn_common_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-20 03:29:08.000000 gaohn-common-utils-0.0.70/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 03:29:28.846063 gaohn-common-utils-0.0.70/setup.cfg
```

### Comparing `gaohn-common-utils-0.0.69/LICENSE` & `gaohn-common-utils-0.0.70/LICENSE`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.69/PKG-INFO` & `gaohn-common-utils-0.0.70/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.69
+Version: 0.0.70
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.69/README.md` & `gaohn-common-utils-0.0.70/README.md`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.69/common_utils/cloud/base.py` & `gaohn-common-utils-0.0.70/common_utils/cloud/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.69/common_utils/cloud/gcp/database/bigquery.py` & `gaohn-common-utils-0.0.70/common_utils/cloud/gcp/database/bigquery.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.69/common_utils/cloud/gcp/storage/gcs.py` & `gaohn-common-utils-0.0.70/common_utils/cloud/gcp/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.69/common_utils/core/base.py` & `gaohn-common-utils-0.0.70/common_utils/core/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.69/common_utils/core/common.py` & `gaohn-common-utils-0.0.70/common_utils/core/common.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.69/common_utils/core/decorators.py` & `gaohn-common-utils-0.0.70/common_utils/core/decorators.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.69/common_utils/core/file_system_utils.py` & `gaohn-common-utils-0.0.70/common_utils/core/file_system_utils.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.69/common_utils/core/logger.py` & `gaohn-common-utils-0.0.70/common_utils/core/logger.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.69/common_utils/data_validator/core.py` & `gaohn-common-utils-0.0.70/common_utils/data_validator/core.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.69/common_utils/experiment_tracking/promoter/base.py` & `gaohn-common-utils-0.0.70/common_utils/experiment_tracking/promoter/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     """
 
     version: int
     metrics: Dict[str, float]
     stage: Optional[str] = None
 
 
-class AbstractPromotionManager(ABC):
+class PromotionManager(ABC):
     """
     A base class (interface) for a model promotion manager.
 
     This class outlines the basic methods any concrete promotion manager should implement.
     """
 
     @abstractmethod
```

### Comparing `gaohn-common-utils-0.0.69/common_utils/experiment_tracking/promoter/core.py` & `gaohn-common-utils-0.0.70/common_utils/experiment_tracking/promoter/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,29 +9,20 @@
 
 from typing import List, Literal, Optional
 
 from mlflow.tracking import MlflowClient
 
 from common_utils.core.logger import Logger
 from common_utils.experiment_tracking.promoter.base import (
-    AbstractPromotionManager,
+    PromotionManager,
     ModelVersion,
 )
 
-ModelClient = MlflowClient  # Union[MlflowClient, WandbClient, ...]
 
-# NOTE:
-# 1. MLFlow has a class called ModelVersion and thus it has methods like
-#    data.metrics.get(metric_name) is specifc to client and .version
-#    is specific to the ModelVersion class. Thus, if you need WandbClient
-#    it means you need them to have the same methods as MLFlowClient.
-# 2. Consider just create a
-
-
-class ModelPromotionManager(AbstractPromotionManager):
+class MLFlowPromotionManager(PromotionManager):
     """A class that manages the promotion of machine learning models to production.
 
     This class adheres to several principles of good software design:
 
     1. Single Responsibility Principle (SRP): This class's responsibility is clear -
        managing the promotion of models to production. It maintains the current and
        previous versions of a model, and decides whether to promote a new model
@@ -75,15 +66,15 @@
     open for extension (you can add support for new types of clients) but closed for
     modification (you don't have to change the ModelPromotionManager class to add
     new clients).
     """
 
     def __init__(
         self,
-        client: ModelClient,
+        client: MlflowClient,
         model_name: str,
         logger: Optional[Logger] = None,
     ) -> None:
         self.client = client
         self.model_name = model_name
 
         if logger is None:
```

### Comparing `gaohn-common-utils-0.0.69/common_utils/versioning/dvc/core.py` & `gaohn-common-utils-0.0.70/common_utils/versioning/dvc/core.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.69/common_utils/versioning/git/core.py` & `gaohn-common-utils-0.0.70/common_utils/versioning/git/core.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.69/gaohn_common_utils.egg-info/PKG-INFO` & `gaohn-common-utils-0.0.70/gaohn_common_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.69
+Version: 0.0.70
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.69/gaohn_common_utils.egg-info/SOURCES.txt` & `gaohn-common-utils-0.0.70/gaohn_common_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.69/pyproject.toml` & `gaohn-common-utils-0.0.70/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gaohn-common-utils"
-version = "0.0.69"
+version = "0.0.70"
 authors = [
   { name="Gao Hongnan", email="hongnangao@gmail.com" },
 ]
 description = "A small utility package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```
