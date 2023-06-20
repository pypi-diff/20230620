# Comparing `tmp/gaohn-common-utils-0.0.65.tar.gz` & `tmp/gaohn-common-utils-0.0.67.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaohn-common-utils-0.0.65.tar", last modified: Fri Jun 16 04:05:40 2023, max compression
+gzip compressed data, was "gaohn-common-utils-0.0.67.tar", last modified: Tue Jun 20 03:02:02 2023, max compression
```

## Comparing `gaohn-common-utils-0.0.65.tar` & `gaohn-common-utils-0.0.67.tar`

### file list

```diff
@@ -1,41 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:05:40.081739 gaohn-common-utils-0.0.65/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-16 04:05:20.000000 gaohn-common-utils-0.0.65/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-16 04:05:40.081739 gaohn-common-utils-0.0.65/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-16 04:05:20.000000 gaohn-common-utils-0.0.65/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:05:40.073739 gaohn-common-utils-0.0.65/common_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 04:05:20.000000 gaohn-common-utils-0.0.65/common_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:05:40.073739 gaohn-common-utils-0.0.65/common_utils/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-16 04:05:20.000000 gaohn-common-utils-0.0.65/common_utils/cloud/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:05:40.069739 gaohn-common-utils-0.0.65/common_utils/cloud/gcp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:05:40.073739 gaohn-common-utils-0.0.65/common_utils/cloud/gcp/database/
--rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-16 04:05:20.000000 gaohn-common-utils-0.0.65/common_utils/cloud/gcp/database/bigquery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:05:40.073739 gaohn-common-utils-0.0.65/common_utils/cloud/gcp/storage/
--rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-06-16 04:05:20.000000 gaohn-common-utils-0.0.65/common_utils/cloud/gcp/storage/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:05:40.077739 gaohn-common-utils-0.0.65/common_utils/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 04:05:20.000000 gaohn-common-utils-0.0.65/common_utils/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 04:05:20.000000 gaohn-common-utils-0.0.65/common_utils/core/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-16 04:05:20.000000 gaohn-common-utils-0.0.65/common_utils/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-06-16 04:05:20.000000 gaohn-common-utils-0.0.65/common_utils/core/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-16 04:05:20.000000 gaohn-common-utils-0.0.65/common_utils/core/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-16 04:05:20.000000 gaohn-common-utils-0.0.65/common_utils/core/file_system_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-06-16 04:05:20.000000 gaohn-common-utils-0.0.65/common_utils/core/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:05:40.077739 gaohn-common-utils-0.0.65/common_utils/data_validator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 04:05:20.000000 gaohn-common-utils-0.0.65/common_utils/data_validator/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-16 04:05:20.000000 gaohn-common-utils-0.0.65/common_utils/data_validator/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:05:40.077739 gaohn-common-utils-0.0.65/common_utils/orchestrator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 04:05:20.000000 gaohn-common-utils-0.0.65/common_utils/orchestrator/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:05:40.069739 gaohn-common-utils-0.0.65/common_utils/versioning/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:05:40.077739 gaohn-common-utils-0.0.65/common_utils/versioning/dvc/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-16 04:05:20.000000 gaohn-common-utils-0.0.65/common_utils/versioning/dvc/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-06-16 04:05:20.000000 gaohn-common-utils-0.0.65/common_utils/versioning/dvc/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:05:40.077739 gaohn-common-utils-0.0.65/common_utils/versioning/git/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 04:05:20.000000 gaohn-common-utils-0.0.65/common_utils/versioning/git/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-16 04:05:20.000000 gaohn-common-utils-0.0.65/common_utils/versioning/git/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:05:40.081739 gaohn-common-utils-0.0.65/gaohn_common_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-16 04:05:40.000000 gaohn-common-utils-0.0.65/gaohn_common_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-16 04:05:40.000000 gaohn-common-utils-0.0.65/gaohn_common_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 04:05:40.000000 gaohn-common-utils-0.0.65/gaohn_common_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-16 04:05:40.000000 gaohn-common-utils-0.0.65/gaohn_common_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-16 04:05:40.000000 gaohn-common-utils-0.0.65/gaohn_common_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-16 04:05:20.000000 gaohn-common-utils-0.0.65/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 04:05:40.081739 gaohn-common-utils-0.0.65/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:02:02.906041 gaohn-common-utils-0.0.67/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-20 03:01:40.000000 gaohn-common-utils-0.0.67/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-20 03:02:02.906041 gaohn-common-utils-0.0.67/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-06-20 03:01:40.000000 gaohn-common-utils-0.0.67/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:02:02.902041 gaohn-common-utils-0.0.67/common_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 03:01:40.000000 gaohn-common-utils-0.0.67/common_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:02:02.902041 gaohn-common-utils-0.0.67/common_utils/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-20 03:01:40.000000 gaohn-common-utils-0.0.67/common_utils/cloud/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:02:02.902041 gaohn-common-utils-0.0.67/common_utils/cloud/gcp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:02:02.902041 gaohn-common-utils-0.0.67/common_utils/cloud/gcp/database/
+-rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-20 03:01:40.000000 gaohn-common-utils-0.0.67/common_utils/cloud/gcp/database/bigquery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:02:02.902041 gaohn-common-utils-0.0.67/common_utils/cloud/gcp/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-06-20 03:01:40.000000 gaohn-common-utils-0.0.67/common_utils/cloud/gcp/storage/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:02:02.902041 gaohn-common-utils-0.0.67/common_utils/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 03:01:40.000000 gaohn-common-utils-0.0.67/common_utils/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 03:01:40.000000 gaohn-common-utils-0.0.67/common_utils/core/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-20 03:01:40.000000 gaohn-common-utils-0.0.67/common_utils/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-06-20 03:01:40.000000 gaohn-common-utils-0.0.67/common_utils/core/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-20 03:01:40.000000 gaohn-common-utils-0.0.67/common_utils/core/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-20 03:01:40.000000 gaohn-common-utils-0.0.67/common_utils/core/file_system_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-06-20 03:01:40.000000 gaohn-common-utils-0.0.67/common_utils/core/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:02:02.902041 gaohn-common-utils-0.0.67/common_utils/data_validator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 03:01:40.000000 gaohn-common-utils-0.0.67/common_utils/data_validator/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-20 03:01:40.000000 gaohn-common-utils-0.0.67/common_utils/data_validator/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:02:02.902041 gaohn-common-utils-0.0.67/common_utils/experiment_tracking/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:02:02.902041 gaohn-common-utils-0.0.67/common_utils/experiment_tracking/promoter/
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-20 03:01:40.000000 gaohn-common-utils-0.0.67/common_utils/experiment_tracking/promoter/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9057 2023-06-20 03:01:40.000000 gaohn-common-utils-0.0.67/common_utils/experiment_tracking/promoter/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:02:02.902041 gaohn-common-utils-0.0.67/common_utils/orchestrator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 03:01:40.000000 gaohn-common-utils-0.0.67/common_utils/orchestrator/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:02:02.902041 gaohn-common-utils-0.0.67/common_utils/versioning/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:02:02.902041 gaohn-common-utils-0.0.67/common_utils/versioning/dvc/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-20 03:01:40.000000 gaohn-common-utils-0.0.67/common_utils/versioning/dvc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-06-20 03:01:40.000000 gaohn-common-utils-0.0.67/common_utils/versioning/dvc/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:02:02.902041 gaohn-common-utils-0.0.67/common_utils/versioning/git/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 03:01:40.000000 gaohn-common-utils-0.0.67/common_utils/versioning/git/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-20 03:01:40.000000 gaohn-common-utils-0.0.67/common_utils/versioning/git/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:02:02.906041 gaohn-common-utils-0.0.67/gaohn_common_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-20 03:02:02.000000 gaohn-common-utils-0.0.67/gaohn_common_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-20 03:02:02.000000 gaohn-common-utils-0.0.67/gaohn_common_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 03:02:02.000000 gaohn-common-utils-0.0.67/gaohn_common_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-20 03:02:02.000000 gaohn-common-utils-0.0.67/gaohn_common_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-20 03:02:02.000000 gaohn-common-utils-0.0.67/gaohn_common_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-20 03:01:40.000000 gaohn-common-utils-0.0.67/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 03:02:02.906041 gaohn-common-utils-0.0.67/setup.cfg
```

### Comparing `gaohn-common-utils-0.0.65/LICENSE` & `gaohn-common-utils-0.0.67/LICENSE`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.65/PKG-INFO` & `gaohn-common-utils-0.0.67/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.65
+Version: 0.0.67
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Common Utils
 
-[![Continuous Integration](https://github.com/gao-hongnan/common-utils/actions/workflows/ci.yaml/badge.svg?branch=continuous-integration)](https://github.com/gao-hongnan/common-utils/actions/workflows/ci.yaml)
+[![Continuous Integration](https://github.com/gao-hongnan/common-utils/actions/workflows/continuous_integration.yaml/badge.svg)](https://github.com/gao-hongnan/common-utils/actions/workflows/continuous_integration.yaml)
 
 ## TODOs
 
 1. Use own `Logger` once the class is finalized in all scripts.
 
 ## Continuous Integration
 
@@ -33,15 +33,16 @@
 bash make_venv.sh venv --pyproject --dev && \
 source venv/bin/activate && \
 rm make_venv.sh
 ```
 
 ### Continue on error vs If Always
 
-See [here](https://stackoverflow.com/questions/58858429/how-to-run-a-github-actions-step-even-if-the-previous-step-fails-while-still-f/58859404#58859404).
+See
+[here](https://stackoverflow.com/questions/58858429/how-to-run-a-github-actions-step-even-if-the-previous-step-fails-while-still-f/58859404#58859404).
 
 ### Run Bandit Security Check
 
 ```bash
 bash ./scripts/devops/ci/ci_security_bandit.sh \
   --severity-level=low \
   --format=json \
@@ -95,10 +96,43 @@
 
 ## Run Integration Test
 
 ### Run System Test
 
 ### Run Acceptance Test
 
-https://madewithml.com/courses/mlops/testing/
+See [madewithml](https://madewithml.com/courses/mlops/testing/).
 
 ### Run Data Test (Great Expectations)
+
+### Run Markdown Lint
+
+```bash
+npm install -g markdownlint-cli && \
+touch .markdownlint.json && \
+```
+
+```bash
+npm install --save-dev --save-exact prettier
+```
+
+```bash
+# prettier
+function pr() {
+  if [ -z "$1" ]; then
+    echo "Error: TARGET_DIR is mandatory."
+    return 1
+  fi
+
+  TARGET_DIR="$1"
+  prettier "$TARGET_DIR" --write \
+    --prose-wrap always \
+    --print-width 80 \
+    --tab-width 4 \
+    --use-tabs true
+}
+```
+
+```bash
+pr <TARGET_MARKDOWN_FILE>
+markdownlint --fix <TARGET_MARKDOWN_FILE>
+```
```

### Comparing `gaohn-common-utils-0.0.65/common_utils/cloud/base.py` & `gaohn-common-utils-0.0.67/common_utils/cloud/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.65/common_utils/cloud/gcp/database/bigquery.py` & `gaohn-common-utils-0.0.67/common_utils/cloud/gcp/database/bigquery.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.65/common_utils/cloud/gcp/storage/gcs.py` & `gaohn-common-utils-0.0.67/common_utils/cloud/gcp/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.65/common_utils/core/base.py` & `gaohn-common-utils-0.0.67/common_utils/core/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.65/common_utils/core/common.py` & `gaohn-common-utils-0.0.67/common_utils/core/common.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.65/common_utils/core/decorators.py` & `gaohn-common-utils-0.0.67/common_utils/core/decorators.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.65/common_utils/core/file_system_utils.py` & `gaohn-common-utils-0.0.67/common_utils/core/file_system_utils.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.65/common_utils/core/logger.py` & `gaohn-common-utils-0.0.67/common_utils/core/logger.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.65/common_utils/data_validator/core.py` & `gaohn-common-utils-0.0.67/common_utils/data_validator/core.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.65/common_utils/versioning/dvc/core.py` & `gaohn-common-utils-0.0.67/common_utils/versioning/dvc/core.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.65/common_utils/versioning/git/core.py` & `gaohn-common-utils-0.0.67/common_utils/versioning/git/core.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.65/gaohn_common_utils.egg-info/PKG-INFO` & `gaohn-common-utils-0.0.67/gaohn_common_utils.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.65
+Version: 0.0.67
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Common Utils
 
-[![Continuous Integration](https://github.com/gao-hongnan/common-utils/actions/workflows/ci.yaml/badge.svg?branch=continuous-integration)](https://github.com/gao-hongnan/common-utils/actions/workflows/ci.yaml)
+[![Continuous Integration](https://github.com/gao-hongnan/common-utils/actions/workflows/continuous_integration.yaml/badge.svg)](https://github.com/gao-hongnan/common-utils/actions/workflows/continuous_integration.yaml)
 
 ## TODOs
 
 1. Use own `Logger` once the class is finalized in all scripts.
 
 ## Continuous Integration
 
@@ -33,15 +33,16 @@
 bash make_venv.sh venv --pyproject --dev && \
 source venv/bin/activate && \
 rm make_venv.sh
 ```
 
 ### Continue on error vs If Always
 
-See [here](https://stackoverflow.com/questions/58858429/how-to-run-a-github-actions-step-even-if-the-previous-step-fails-while-still-f/58859404#58859404).
+See
+[here](https://stackoverflow.com/questions/58858429/how-to-run-a-github-actions-step-even-if-the-previous-step-fails-while-still-f/58859404#58859404).
 
 ### Run Bandit Security Check
 
 ```bash
 bash ./scripts/devops/ci/ci_security_bandit.sh \
   --severity-level=low \
   --format=json \
@@ -95,10 +96,43 @@
 
 ## Run Integration Test
 
 ### Run System Test
 
 ### Run Acceptance Test
 
-https://madewithml.com/courses/mlops/testing/
+See [madewithml](https://madewithml.com/courses/mlops/testing/).
 
 ### Run Data Test (Great Expectations)
+
+### Run Markdown Lint
+
+```bash
+npm install -g markdownlint-cli && \
+touch .markdownlint.json && \
+```
+
+```bash
+npm install --save-dev --save-exact prettier
+```
+
+```bash
+# prettier
+function pr() {
+  if [ -z "$1" ]; then
+    echo "Error: TARGET_DIR is mandatory."
+    return 1
+  fi
+
+  TARGET_DIR="$1"
+  prettier "$TARGET_DIR" --write \
+    --prose-wrap always \
+    --print-width 80 \
+    --tab-width 4 \
+    --use-tabs true
+}
+```
+
+```bash
+pr <TARGET_MARKDOWN_FILE>
+markdownlint --fix <TARGET_MARKDOWN_FILE>
+```
```

### Comparing `gaohn-common-utils-0.0.65/gaohn_common_utils.egg-info/SOURCES.txt` & `gaohn-common-utils-0.0.67/gaohn_common_utils.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 common_utils/core/base.py
 common_utils/core/common.py
 common_utils/core/decorators.py
 common_utils/core/file_system_utils.py
 common_utils/core/logger.py
 common_utils/data_validator/base.py
 common_utils/data_validator/core.py
+common_utils/experiment_tracking/promoter/base.py
+common_utils/experiment_tracking/promoter/core.py
 common_utils/orchestrator/base.py
 common_utils/versioning/dvc/base.py
 common_utils/versioning/dvc/core.py
 common_utils/versioning/git/base.py
 common_utils/versioning/git/core.py
 gaohn_common_utils.egg-info/PKG-INFO
 gaohn_common_utils.egg-info/SOURCES.txt
```

### Comparing `gaohn-common-utils-0.0.65/pyproject.toml` & `gaohn-common-utils-0.0.67/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gaohn-common-utils"
-version = "0.0.65"
+version = "0.0.67"
 authors = [
   { name="Gao Hongnan", email="hongnangao@gmail.com" },
 ]
 description = "A small utility package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

