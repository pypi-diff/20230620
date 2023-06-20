# Comparing `tmp/datawise-0.0.15.tar.gz` & `tmp/datawise-0.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datawise-0.0.15.tar", max compression
+gzip compressed data, was "datawise-0.0.16.tar", max compression
```

## Comparing `datawise-0.0.15.tar` & `datawise-0.0.16.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-06-16 12:22:48.812559 datawise-0.0.15/LICENSE
--rw-r--r--   0        0        0     6818 2023-06-20 04:10:21.992731 datawise-0.0.15/README.md
--rw-r--r--   0        0        0     5433 2023-06-20 04:01:43.116353 datawise-0.0.15/datawise/__init__.py
--rw-r--r--   0        0        0      481 2023-06-18 12:46:33.125357 datawise-0.0.15/datawise/exceptions.py
--rw-r--r--   0        0        0      634 2023-06-20 04:04:41.402374 datawise-0.0.15/pyproject.toml
--rw-r--r--   0        0        0     7421 1970-01-01 00:00:00.000000 datawise-0.0.15/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-16 12:22:48.812559 datawise-0.0.16/LICENSE
+-rw-r--r--   0        0        0     6818 2023-06-20 04:10:21.992731 datawise-0.0.16/README.md
+-rw-r--r--   0        0        0     5600 2023-06-20 11:36:16.459385 datawise-0.0.16/datawise/__init__.py
+-rw-r--r--   0        0        0      636 2023-06-20 11:29:08.510434 datawise-0.0.16/datawise/exceptions.py
+-rw-r--r--   0        0        0      634 2023-06-20 11:46:57.003406 datawise-0.0.16/pyproject.toml
+-rw-r--r--   0        0        0     7421 1970-01-01 00:00:00.000000 datawise-0.0.16/PKG-INFO
```

### Comparing `datawise-0.0.15/LICENSE` & `datawise-0.0.16/LICENSE`

 * *Files identical despite different names*

### Comparing `datawise-0.0.15/README.md` & `datawise-0.0.16/README.md`

 * *Files identical despite different names*

### Comparing `datawise-0.0.15/datawise/__init__.py` & `datawise-0.0.16/datawise/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import logging
 import os
 import requests
 
-from .exceptions import AuthorizationError, DataWiseInternalError, TranslationError
+from .exceptions import AuthorizationError, BadRequestError, DataWiseInternalError, TranslationError
 from dotenv import load_dotenv
 from requests.exceptions import RequestException
 from retry import retry
 
 
 class DataWise:
   """Creates a new DataWise API client."""
@@ -57,15 +57,16 @@
       data=json.dumps(data), 
       headers={
         "Authorization": "Bearer " + self.api_key,
         "content-type": "application/json"
       }
     )
 
-    if (response.status_code == 400): raise AuthorizationError()
+    if (response.status_code == 400): raise BadRequestError(response.text)
+    if (response.status_code == 401): raise AuthorizationError()
     if (response.status_code >= 500): raise DataWiseInternalError()
 
     python_code = response.json()
 
     import pandas as pd
     import numpy as np
     globals = { "np": np, "pd": pd }
@@ -123,15 +124,16 @@
       data=json.dumps(data), 
       headers={
         "Authorization": "Bearer " + self.api_key,
         "content-type": "application/json"
       }
     )
 
-    if (response.status_code == 400): raise AuthorizationError()
+    if (response.status_code == 400): raise BadRequestError(response.text)
+    if (response.status_code == 401): raise AuthorizationError()
     if (response.status_code >= 500): raise DataWiseInternalError()
 
     python_code = response.json()
 
     import matplotlib.pyplot as plt
     import seaborn as sns
     globals = { "plt": plt, "sns": sns }
```

### Comparing `datawise-0.0.15/pyproject.toml` & `datawise-0.0.16/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datawise"
-version = "0.0.15"
+version = "0.0.16"
 description = "DataWise is your co-pilot for performing data analysis and visualization in Python."
 authors = ["DataWise Team"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9.0"
 python-dotenv = "^1.0.0"
```

### Comparing `datawise-0.0.15/PKG-INFO` & `datawise-0.0.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datawise
-Version: 0.0.15
+Version: 0.0.16
 Summary: DataWise is your co-pilot for performing data analysis and visualization in Python.
 Author: DataWise Team
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

