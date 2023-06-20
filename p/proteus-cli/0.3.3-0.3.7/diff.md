# Comparing `tmp/proteus_cli-0.3.3.tar.gz` & `tmp/proteus_cli-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteus_cli-0.3.3.tar", max compression
+gzip compressed data, was "proteus_cli-0.3.7.tar", max compression
```

## Comparing `proteus_cli-0.3.3.tar` & `proteus_cli-0.3.7.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1330 2023-06-15 11:14:40.876516 proteus_cli-0.3.3/cli/__init__.py
--rw-r--r--   0        0        0      384 2023-06-15 11:14:40.876516 proteus_cli-0.3.3/cli/api/__init__.py
--rw-r--r--   0        0        0     1784 2023-06-15 11:14:40.876516 proteus_cli-0.3.3/cli/api/decorators.py
--rw-r--r--   0        0        0      849 2023-06-15 11:14:40.876516 proteus_cli-0.3.3/cli/api/hooks.py
--rw-r--r--   0        0        0        0 2023-06-15 11:14:40.876516 proteus_cli-0.3.3/cli/buckets/__init__.py
--rw-r--r--   0        0        0     1092 2023-06-15 11:14:40.876516 proteus_cli-0.3.3/cli/buckets/commands.py
--rw-r--r--   0        0        0     2621 2023-06-15 11:14:40.876516 proteus_cli-0.3.3/cli/config.py
--rw-r--r--   0        0        0        0 2023-06-15 11:14:40.876516 proteus_cli-0.3.3/cli/datasets/__init__.py
--rw-r--r--   0        0        0     1332 2023-06-15 11:14:40.876516 proteus_cli-0.3.3/cli/datasets/commands.py
--rw-r--r--   0        0        0        0 2023-06-15 11:14:40.876516 proteus_cli-0.3.3/cli/datasets/preprocessor/__init__.py
--rw-r--r--   0        0        0      939 2023-06-15 11:14:40.876516 proteus_cli-0.3.3/cli/datasets/preprocessor/config/__init__.py
--rw-r--r--   0        0        0      323 2023-06-15 11:14:40.876516 proteus_cli-0.3.3/cli/datasets/preprocessor/config/case/__init__.py
--rw-r--r--   0        0        0      958 2023-06-15 11:14:40.876516 proteus_cli-0.3.3/cli/datasets/preprocessor/config/case/cnn_pca.py
--rw-r--r--   0        0        0     3447 2023-06-15 11:14:40.876516 proteus_cli-0.3.3/cli/datasets/preprocessor/config/case/hm.py
--rw-r--r--   0        0        0     3054 2023-06-15 11:14:40.876516 proteus_cli-0.3.3/cli/datasets/preprocessor/config/case/well_model.py
--rw-r--r--   0        0        0      446 2023-06-15 11:14:40.876516 proteus_cli-0.3.3/cli/datasets/preprocessor/config/common/__init__.py
--rw-r--r--   0        0        0     3251 2023-06-15 11:14:40.876516 proteus_cli-0.3.3/cli/datasets/preprocessor/config/common/cnn_pca.py
--rw-r--r--   0        0        0     2009 2023-06-15 11:14:40.876516 proteus_cli-0.3.3/cli/datasets/preprocessor/config/common/hm.py
--rw-r--r--   0        0        0     1542 2023-06-15 11:14:40.876516 proteus_cli-0.3.3/cli/datasets/preprocessor/config/common/well_model.py
--rw-r--r--   0        0        0     2665 2023-06-15 11:14:40.876516 proteus_cli-0.3.3/cli/datasets/preprocessor/config/default.py
--rw-r--r--   0        0        0      418 2023-06-15 11:14:40.876516 proteus_cli-0.3.3/cli/datasets/preprocessor/config/step/__init__.py
--rw-r--r--   0        0        0      125 2023-06-15 11:14:40.876516 proteus_cli-0.3.3/cli/datasets/preprocessor/config/step/cnn_pca.py
--rw-r--r--   0        0        0     2415 2023-06-15 11:14:40.876516 proteus_cli-0.3.3/cli/datasets/preprocessor/config/step/hm.py
--rw-r--r--   0        0        0      128 2023-06-15 11:14:40.876516 proteus_cli-0.3.3/cli/datasets/preprocessor/config/step/well_model.py
--rw-r--r--   0        0        0      673 2023-06-15 11:14:40.876516 proteus_cli-0.3.3/cli/datasets/preprocessor/init_keywords.json
--rw-r--r--   0        0        0    14707 2023-06-15 11:14:40.876516 proteus_cli-0.3.3/cli/datasets/preprocessor/preprocess_functions.py
--rw-r--r--   0        0        0     4944 2023-06-15 11:14:40.876516 proteus_cli-0.3.3/cli/datasets/preprocessor/process_step.py
--rw-r--r--   0        0        0     8656 2023-06-15 11:14:40.876516 proteus_cli-0.3.3/cli/datasets/preprocessor/utils.py
--rw-r--r--   0        0        0      411 2023-06-15 11:14:40.876516 proteus_cli-0.3.3/cli/datasets/preprocessor/well_init_keywords.json
--rw-r--r--   0        0        0        0 2023-06-15 11:14:40.876516 proteus_cli-0.3.3/cli/datasets/sources/__init__.py
--rw-r--r--   0        0        0     6437 2023-06-15 11:14:40.876516 proteus_cli-0.3.3/cli/datasets/sources/az.py
--rw-r--r--   0        0        0      824 2023-06-15 11:14:40.876516 proteus_cli-0.3.3/cli/datasets/sources/common.py
--rw-r--r--   0        0        0     2809 2023-06-15 11:14:40.876516 proteus_cli-0.3.3/cli/datasets/sources/local.py
--rw-r--r--   0        0        0     1783 2023-06-15 11:14:40.876516 proteus_cli-0.3.3/cli/datasets/sources/s3.py
--rw-r--r--   0        0        0     9158 2023-06-15 11:14:40.876516 proteus_cli-0.3.3/cli/datasets/upload.py
--rw-r--r--   0        0        0        0 2023-06-15 11:14:40.876516 proteus_cli-0.3.3/cli/debugger/__init__.py
--rw-r--r--   0        0        0     2265 2023-06-15 11:14:40.876516 proteus_cli-0.3.3/cli/debugger/commands.py
--rw-r--r--   0        0        0     3926 2023-06-15 11:14:40.876516 proteus_cli-0.3.3/cli/debugger/init_keyword_check.py
--rw-r--r--   0        0        0        0 2023-06-15 11:14:40.876516 proteus_cli-0.3.3/cli/debugger/restart_keyword_check.py
--rw-r--r--   0        0        0        0 2023-06-15 11:14:40.876516 proteus_cli-0.3.3/cli/jobs/__init__.py
--rw-r--r--   0        0        0     1283 2023-06-15 11:14:40.876516 proteus_cli-0.3.3/cli/jobs/commands.py
--rw-r--r--   0        0        0     3026 2023-06-15 11:14:40.880517 proteus_cli-0.3.3/cli/jobs/list.py
--rw-r--r--   0        0        0      100 2023-06-15 11:14:40.880517 proteus_cli-0.3.3/cli/runtime.py
--rw-r--r--   0        0        0        0 2023-06-15 11:14:40.880517 proteus_cli-0.3.3/cli/simulations/__init__.py
--rw-r--r--   0        0        0     2460 2023-06-15 11:14:40.880517 proteus_cli-0.3.3/cli/simulations/commands.py
--rw-r--r--   0        0        0     7603 2023-06-15 11:14:40.880517 proteus_cli-0.3.3/cli/simulations/create.py
--rw-r--r--   0        0        0     4119 2023-06-15 11:14:40.880517 proteus_cli-0.3.3/cli/simulations/dependencySolver.py
--rw-r--r--   0        0        0     5190 2023-06-15 11:14:40.880517 proteus_cli-0.3.3/cli/simulations/opm.py
--rw-r--r--   0        0        0      449 2023-06-15 11:14:40.880517 proteus_cli-0.3.3/logging.ini
--rw-r--r--   0        0        0     1530 2023-06-15 11:14:40.880517 proteus_cli-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 proteus_cli-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     3083 2023-06-20 16:50:25.212463 proteus_cli-0.3.7/cli/__init__.py
+-rw-r--r--   0        0        0      384 2023-06-20 16:50:25.212463 proteus_cli-0.3.7/cli/api/__init__.py
+-rw-r--r--   0        0        0     1784 2023-06-20 16:50:25.212463 proteus_cli-0.3.7/cli/api/decorators.py
+-rw-r--r--   0        0        0      849 2023-06-20 16:50:25.212463 proteus_cli-0.3.7/cli/api/hooks.py
+-rw-r--r--   0        0        0        0 2023-06-20 16:50:25.212463 proteus_cli-0.3.7/cli/buckets/__init__.py
+-rw-r--r--   0        0        0     1092 2023-06-20 16:50:25.212463 proteus_cli-0.3.7/cli/buckets/commands.py
+-rw-r--r--   0        0        0     2810 2023-06-20 16:50:25.212463 proteus_cli-0.3.7/cli/config.py
+-rw-r--r--   0        0        0        0 2023-06-20 16:50:25.212463 proteus_cli-0.3.7/cli/datasets/__init__.py
+-rw-r--r--   0        0        0     1332 2023-06-20 16:50:25.212463 proteus_cli-0.3.7/cli/datasets/commands.py
+-rw-r--r--   0        0        0        0 2023-06-20 16:50:25.212463 proteus_cli-0.3.7/cli/datasets/preprocessor/__init__.py
+-rw-r--r--   0        0        0      939 2023-06-20 16:50:25.212463 proteus_cli-0.3.7/cli/datasets/preprocessor/config/__init__.py
+-rw-r--r--   0        0        0      323 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/datasets/preprocessor/config/case/__init__.py
+-rw-r--r--   0        0        0      958 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/datasets/preprocessor/config/case/cnn_pca.py
+-rw-r--r--   0        0        0     3447 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/datasets/preprocessor/config/case/hm.py
+-rw-r--r--   0        0        0     3054 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/datasets/preprocessor/config/case/well_model.py
+-rw-r--r--   0        0        0      446 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/datasets/preprocessor/config/common/__init__.py
+-rw-r--r--   0        0        0     3251 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/datasets/preprocessor/config/common/cnn_pca.py
+-rw-r--r--   0        0        0     2009 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/datasets/preprocessor/config/common/hm.py
+-rw-r--r--   0        0        0     1542 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/datasets/preprocessor/config/common/well_model.py
+-rw-r--r--   0        0        0     2665 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/datasets/preprocessor/config/default.py
+-rw-r--r--   0        0        0      418 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/datasets/preprocessor/config/step/__init__.py
+-rw-r--r--   0        0        0      125 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/datasets/preprocessor/config/step/cnn_pca.py
+-rw-r--r--   0        0        0     2415 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/datasets/preprocessor/config/step/hm.py
+-rw-r--r--   0        0        0      128 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/datasets/preprocessor/config/step/well_model.py
+-rw-r--r--   0        0        0      673 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/datasets/preprocessor/init_keywords.json
+-rw-r--r--   0        0        0    14707 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/datasets/preprocessor/preprocess_functions.py
+-rw-r--r--   0        0        0     4944 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/datasets/preprocessor/process_step.py
+-rw-r--r--   0        0        0     8656 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/datasets/preprocessor/utils.py
+-rw-r--r--   0        0        0      411 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/datasets/preprocessor/well_init_keywords.json
+-rw-r--r--   0        0        0        0 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/datasets/sources/__init__.py
+-rw-r--r--   0        0        0     5927 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/datasets/sources/az.py
+-rw-r--r--   0        0        0      824 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/datasets/sources/common.py
+-rw-r--r--   0        0        0     2809 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/datasets/sources/local.py
+-rw-r--r--   0        0        0     1783 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/datasets/sources/s3.py
+-rw-r--r--   0        0        0     9158 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/datasets/upload.py
+-rw-r--r--   0        0        0        0 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/debugger/__init__.py
+-rw-r--r--   0        0        0     2265 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/debugger/commands.py
+-rw-r--r--   0        0        0     3926 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/debugger/init_keyword_check.py
+-rw-r--r--   0        0        0        0 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/debugger/restart_keyword_check.py
+-rw-r--r--   0        0        0        0 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/jobs/__init__.py
+-rw-r--r--   0        0        0     1283 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/jobs/commands.py
+-rw-r--r--   0        0        0     3026 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/jobs/list.py
+-rw-r--r--   0        0        0      100 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/runtime.py
+-rw-r--r--   0        0        0        0 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/simulations/__init__.py
+-rw-r--r--   0        0        0     2460 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/simulations/commands.py
+-rw-r--r--   0        0        0     7603 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/simulations/create.py
+-rw-r--r--   0        0        0     4119 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/simulations/dependencySolver.py
+-rw-r--r--   0        0        0     5190 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/cli/simulations/opm.py
+-rw-r--r--   0        0        0      449 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/logging.ini
+-rw-r--r--   0        0        0     1530 2023-06-20 16:50:25.216463 proteus_cli-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 proteus_cli-0.3.7/PKG-INFO
```

### Comparing `proteus_cli-0.3.3/cli/api/decorators.py` & `proteus_cli-0.3.7/cli/api/decorators.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.3/cli/api/hooks.py` & `proteus_cli-0.3.7/cli/api/hooks.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.3/cli/buckets/commands.py` & `proteus_cli-0.3.7/cli/buckets/commands.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.3/cli/config.py` & `proteus_cli-0.3.7/cli/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,25 +14,27 @@
     TEMPLATE_NAME = "case_template"
     INPUT_LOC = "input"
     LOG_LOC = "logs"
 
     SLEEP_TIME = 30
     PROMPT = True
     AUTH_HOST = os.getenv("AUTH_HOST", "https://auth.dev.origen.ai")
-    PROTEUS_HOST = os.getenv("PROTEUS_HOST", "https://proteus-test.dev.origen.ai")
+    PROTEUS_HOST = os.getenv("PROTEUS_HOST", os.getenv("API_HOST", "https://proteus-test.dev.origen.ai"))
     API_SSL_VERIFY = os.getenv("API_SSL_VERIFY", "1").lower() not in ("0", "false", "f")
-    USERNAME = os.getenv("PROTEUS_USERNAME", None)
-    PASSWORD = os.getenv("PROTEUS_PASSWORD", None)
+    USERNAME = os.getenv("PROTEUS_USERNAME", os.getenv("USERNAME", None))
+    PASSWORD = os.getenv("PROTEUS_PASSWORD", os.getenv("PASSWORD", None))
     REALM = os.getenv("REALM", "origen")
     CLIENT_ID = os.getenv("CLIENT_ID", "proteus-front")
     CLIENT_SECRET = os.getenv("CLIENT_SECRET", None)
 
-    WORKERS_REALM = os.getenv("WORKERS_REALM", "robots")
-    WORKERS_CLIENT_ID = os.getenv("WORKERS_CLIENT_ID", "workers")
-    WORKERS_CLIENT_SECRET = os.getenv("WORKERS_CLIENT_SECRET", None)
+    WORKERS_REALM = os.getenv("WORKERS_REALM", os.getenv("REALM", "robots"))
+    WORKERS_CLIENT_ID = os.getenv("WORKERS_CLIENT_ID", os.getenv("CLIENT_ID", "workers"))
+    WORKERS_CLIENT_SECRET = os.getenv("WORKERS_CLIENT_SECRET", os.getenv("CLIENT_SECRET", None))
+
+    ENTITY_URL = os.getenv("ENTITY_URL", None)
 
     RETRY_INTERVAL = 25  # Seconds
     REFRESH_GAP = 100  # Seconds
     S3_REGION = "eu-west-3"
     WORKERS_COUNT = 5
     WORKERS_DOWNLOAD_COUNT = 10
     AZURE_STORAGE_CONNECTION_STRING = os.getenv("AZURE_STORAGE_CONNECTION_STRING")
```

### Comparing `proteus_cli-0.3.3/cli/datasets/commands.py` & `proteus_cli-0.3.7/cli/datasets/commands.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.3/cli/datasets/preprocessor/config/__init__.py` & `proteus_cli-0.3.7/cli/datasets/preprocessor/config/__init__.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.3/cli/datasets/preprocessor/config/case/cnn_pca.py` & `proteus_cli-0.3.7/cli/datasets/preprocessor/config/case/cnn_pca.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.3/cli/datasets/preprocessor/config/case/hm.py` & `proteus_cli-0.3.7/cli/datasets/preprocessor/config/case/hm.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.3/cli/datasets/preprocessor/config/case/well_model.py` & `proteus_cli-0.3.7/cli/datasets/preprocessor/config/case/well_model.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.3/cli/datasets/preprocessor/config/common/cnn_pca.py` & `proteus_cli-0.3.7/cli/datasets/preprocessor/config/common/cnn_pca.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.3/cli/datasets/preprocessor/config/common/hm.py` & `proteus_cli-0.3.7/cli/datasets/preprocessor/config/common/hm.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.3/cli/datasets/preprocessor/config/common/well_model.py` & `proteus_cli-0.3.7/cli/datasets/preprocessor/config/common/well_model.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.3/cli/datasets/preprocessor/config/default.py` & `proteus_cli-0.3.7/cli/datasets/preprocessor/config/default.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.3/cli/datasets/preprocessor/config/step/hm.py` & `proteus_cli-0.3.7/cli/datasets/preprocessor/config/step/hm.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.3/cli/datasets/preprocessor/init_keywords.json` & `proteus_cli-0.3.7/cli/datasets/preprocessor/init_keywords.json`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.3/cli/datasets/preprocessor/preprocess_functions.py` & `proteus_cli-0.3.7/cli/datasets/preprocessor/preprocess_functions.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.3/cli/datasets/preprocessor/process_step.py` & `proteus_cli-0.3.7/cli/datasets/preprocessor/process_step.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.3/cli/datasets/preprocessor/utils.py` & `proteus_cli-0.3.7/cli/datasets/preprocessor/utils.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.3/cli/datasets/sources/az.py` & `proteus_cli-0.3.7/cli/datasets/sources/az.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,183 +1,165 @@
 import re
-
-# from azure.storage.blob._models import BlobProperties as AzureBlobProperties
+from functools import lru_cache
 from io import BytesIO
 
-from azure.storage.blob import ContainerClient
 from azure.core.credentials import AzureSasCredential
 from azure.core.exceptions import HttpResponseError, ClientAuthenticationError
 from azure.identity import DefaultAzureCredential
+from azure.storage.blob import ContainerClient
 
+from cli.config import config
 from .common import Source, SourcedItem
 from ... import proteus
-from cli.config import config
 
 AZURE_SAS_TOKEN = config.AZURE_SAS_TOKEN
 
 CONTENT_CHUNK_SIZE = 10 * 1024 * 1024
 
 
 class AZSource(Source):
     URI_re = re.compile(
         r"^https:\/\/(?P<bucket_name>.*\.windows\.net)\/" r"(?P<container_name>[^\/]*)(\/)?(?P<prefix>.*)?$"
     )
 
+    SAS_TOKEN_COMPONENTS = {"sv", "se", "sr", "sp"}
+
+    CLIENT_INIT_PARAMS = {"max_single_get_size": 256 * 1024 * 1024, "max_chunk_get_size": 128 * 1024 * 1024}
+    MAX_CONCURRENCY = 10
+
     def __init__(self, uri):
         super().__init__(uri)
         match = self.URI_re.match(uri.rstrip("/"))
         assert match is not None, f"{uri} must be an s3 URI"
         container_name = match.groupdict()["container_name"]
         storage_url = f'https://{match.groupdict()["bucket_name"]}'
 
+        errors = []
+
+        # Check first if the URI include credentials as SAS url
+        url_sas_token = next(iter(uri.split("?")[1:]), "")
+        url_sas_token_components = set(x.split("=")[0] for x in url_sas_token.split("&") if x)
+
+        if self.SAS_TOKEN_COMPONENTS.intersection(url_sas_token_components) == self.SAS_TOKEN_COMPONENTS:
+            self.container_client = ContainerClient.from_container_url(
+                f"{storage_url}/{container_name}?" + uri.split("?")[1], **self.CLIENT_INIT_PARAMS
+            )
+            try:
+                next(self.container_client.list_blobs())
+                return
+            except ClientAuthenticationError as e:
+                errors.append(e)
+
+        # Try to see if there is a general SAS token
+        if AZURE_SAS_TOKEN:
+            self.container_client = ContainerClient(
+                storage_url,
+                credential=AzureSasCredential(AZURE_SAS_TOKEN),
+                container_name=container_name,
+                **self.CLIENT_INIT_PARAMS,
+            )
+
+            try:
+                next(self.container_client.list_blobs())
+                return
+            except ClientAuthenticationError as e:
+                errors.append(e)
+
+        # Finally try default azure credentials
         auth_methods = [
             "exclude_environment_credential",
             "exclude_cli_credential",
             "exclude_shared_token_cache_credential",
             "exclude_visual_studio_code_credential",
             "exclude_interactive_browser_credential",
             "exclude_powershell_credential",
             "exclude_managed_identity_credential",
         ]
 
-        if AZURE_SAS_TOKEN:
-            self.container_client = ContainerClient(
-                storage_url,
-                credential=AzureSasCredential(AZURE_SAS_TOKEN),
-                container_name=container_name,
-            )
-            return
-
-        errors = []
-        login_successful = False
         for auth_method in auth_methods:
             try:
                 flags = {auth: True for auth in auth_methods}
                 flags[auth_method] = False
+
                 self.container_client = ContainerClient(
                     storage_url,
                     credential=DefaultAzureCredential(**flags),
                     container_name=container_name,
+                    **self.CLIENT_INIT_PARAMS,
                 )
-                self.container_client.exists()
-                login_successful = True
-                break
+
+                next(self.container_client.list_blobs())
+
+                return
             except ClientAuthenticationError as e:
                 errors.append(e)
 
-        if not login_successful:
-            for error in errors:
-                proteus.logger.error(error)
-            raise RuntimeError("Cannot authenticate into azure")
+        for error in errors:
+            proteus.logger.error(error)
+
+        raise RuntimeError("Cannot authenticate into azure")
 
     @proteus.may_insist_up_to(5, 1)
     def list_contents(self, starts_with="", ends_with=None):
         bucket_uri = self.uri
-        match = self.URI_re.match(bucket_uri.rstrip("/"))
+        match = self.URI_re.match(bucket_uri.split("?")[0].rstrip("/"))
         assert match is not None, f"{bucket_uri} must be an s3 URI"
         prefix = match.groupdict()["prefix"]
         try:
-            for item in self.container_client.list_blobs(name_starts_with=prefix + starts_with):
+            for item in self._list_blobs_with_cache(name_starts_with=prefix + starts_with):
                 item_name = f'/{item["name"]}'
                 assert item_name.startswith(f"/{prefix}{starts_with}".replace("//", "/"))
                 if ends_with is None or item_name.endswith(ends_with):
                     yield SourcedItem(item, item_name, self, item.size)
         except HttpResponseError:
             proteus.logger.error(
                 "Missing Azure credentials to perform this operation, please "
                 "provide a SAS token or provide another authentication method on Azure"
             )
             raise
 
+    _blob_cache = {}
+
+    @lru_cache(maxsize=50000)
+    def _list_blobs_with_cache(self, name_starts_with):
+        items = self._blob_cache.get(name_starts_with)
+
+        if not items:
+            items = list(self.container_client.list_blobs(name_starts_with=name_starts_with))
+            self._blob_cache[name_starts_with] = items
+
+        return items
+
     def open(self, reference):
         reference_path = reference.get("name")
         file_size = reference["size"]
         modified = reference["last_modified"]
 
         stream = BytesIO()
-        streamdownloader = self.container_client.download_blob(reference.get("name"), max_concurrency=4)
+        streamdownloader = self._download_blob(reference)
         streamdownloader.download_to_stream(stream)
         stream.seek(0)
         return reference_path, file_size, modified, stream
 
     @proteus.may_insist_up_to(5, 1)
     def _download_blob(self, reference):
         return self.container_client.download_blob(
-            reference.get("name"), max_concurrency=3, read_timeout=8000, timeout=8000
+            reference.get("name"),
+            max_concurrency=self.MAX_CONCURRENCY,
+            read_timeout=8000,
+            timeout=8000,
+            length=getattr(reference, "size", None),
+            offset=0,
         )
 
     def download(self, reference):
         return self._download_blob(reference).readall()
 
     def chunks(self, reference):
-        with AZObjectFile(
-            mode="r", size=reference.size, container_client=self.container_client, reference_path=reference.get("name")
-        ) as f:
-            for chunk in f:
-                yield chunk
-
-
-class AZObjectFile:
-    """An ObjectFile in object storage that can be opened and closed.
-    See Objects.open()"""
-
-    def __init__(self, mode, size, container_client=None, reference_path=None):
-        """Initialize the Object object with a name and a blob_client
-        mode is w or r, size is the blob size.
-        """
-        self.container_client = container_client
-        self.reference_path = reference_path
-        self.block_list = []
-        self.mode = mode
-        self.__open__ = True
-        self.pos = 0
-        self.size = size
-
-    def close(self):
-        """Finalise the object"""
-        self.__open__ = False
-
-    def __del__(self):
-        if self.__open__:
-            self.close()
-
-    def __enter__(self):
-        return self
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        if self.__open__:
-            self.close()
-
-    def __iter__(self):
-        self.pos = 0
-
-        return self
-
-    @proteus.may_insist_up_to(5, delay_in_secs=1)
-    def __next__(self):
-        data = BytesIO()
-        if self.pos >= self.size:
-            raise StopIteration()
-        elif self.pos + CONTENT_CHUNK_SIZE > self.size:
-            size = self.size - self.pos
-        else:
-            size = CONTENT_CHUNK_SIZE
-        self.container_client.download_blob(self.reference_path, offset=self.pos, length=size).download_to_stream(
-            data, max_concurrency=16
-        )
-        self.pos += size
-        return data.getvalue()
+        stream = self._download_blob(reference)
 
-    def read(self, size=CONTENT_CHUNK_SIZE):
-        if size is None:
-            return self.container_client.download_blob(self.reference_path).readall()
-        else:
-            if self.pos >= self.size:
-                return ""
-            elif self.pos + size > self.size:
-                size = self.size - self.pos
-            data = BytesIO()
-            self.container_client.download_blob(self.reference_path, offset=self.pos, length=size).download_to_stream(
-                data, max_concurrency=4
-            )
-            self.pos += size
-            return data.getvalue()
+        for chunk in stream.chunks():
+            yield chunk
+
+    def fastcopy(self, reference, destination):
+        # TODO: Maybe fastcopy can use azcopy?
+        return False
```

### Comparing `proteus_cli-0.3.3/cli/datasets/sources/common.py` & `proteus_cli-0.3.7/cli/datasets/sources/common.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.3/cli/datasets/sources/local.py` & `proteus_cli-0.3.7/cli/datasets/sources/local.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.3/cli/datasets/sources/s3.py` & `proteus_cli-0.3.7/cli/datasets/sources/s3.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.3/cli/datasets/upload.py` & `proteus_cli-0.3.7/cli/datasets/upload.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.3/cli/debugger/commands.py` & `proteus_cli-0.3.7/cli/debugger/commands.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.3/cli/debugger/init_keyword_check.py` & `proteus_cli-0.3.7/cli/debugger/init_keyword_check.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.3/cli/jobs/commands.py` & `proteus_cli-0.3.7/cli/jobs/commands.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.3/cli/jobs/list.py` & `proteus_cli-0.3.7/cli/jobs/list.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.3/cli/simulations/commands.py` & `proteus_cli-0.3.7/cli/simulations/commands.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.3/cli/simulations/create.py` & `proteus_cli-0.3.7/cli/simulations/create.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.3/cli/simulations/dependencySolver.py` & `proteus_cli-0.3.7/cli/simulations/dependencySolver.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.3/cli/simulations/opm.py` & `proteus_cli-0.3.7/cli/simulations/opm.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.3/pyproject.toml` & `proteus_cli-0.3.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "proteus-cli"
-version = "0.3.3"
+version = "0.3.7"
 description = ""
 authors = []
 packages = [
     {include="cli"},
     {include="logging.ini"}
 ]
 
@@ -17,15 +17,15 @@
 boto3 = "^1.17.79"
 tqdm = "^4.61.0"
 tabulate = "^0.8.9"
 azure-storage-blob = "^12.8.1"
 readchar = "^3.0.4"
 azure-identity = "^1.12.0"
 markupsafe = "2.0.1"
-proteus-runtime = "0.2.24"
+proteus-runtime = "0.2.29"
 proteus-preprocessing = "0.2.15"
 
 [tool.poetry.dev-dependencies]
 black = "^22.1.0"
 pre-commit = "^2.9.3"
 pytest-mock = "^3.5.1"
 requests-mock = "^1.8.0"
```

### Comparing `proteus_cli-0.3.3/PKG-INFO` & `proteus_cli-0.3.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: proteus-cli
-Version: 0.3.3
+Version: 0.3.7
 Summary: 
 Requires-Python: >=3.8,<3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Dist: azure-identity (>=1.12.0,<2.0.0)
 Requires-Dist: azure-storage-blob (>=12.8.1,<13.0.0)
 Requires-Dist: boto3 (>=1.17.79,<2.0.0)
 Requires-Dist: click (>=8.0.0,<9.0.0)
 Requires-Dist: cryptography (>=3.3.2,<4.0.0)
 Requires-Dist: jwt (>=1.2.0,<2.0.0)
 Requires-Dist: markupsafe (==2.0.1)
 Requires-Dist: proteus-preprocessing (==0.2.15)
-Requires-Dist: proteus-runtime (==0.2.24)
+Requires-Dist: proteus-runtime (==0.2.29)
 Requires-Dist: pycryptodome (>=3.10.1,<4.0.0)
 Requires-Dist: readchar (>=3.0.4,<4.0.0)
 Requires-Dist: tabulate (>=0.8.9,<0.9.0)
 Requires-Dist: tqdm (>=4.61.0,<5.0.0)
```

