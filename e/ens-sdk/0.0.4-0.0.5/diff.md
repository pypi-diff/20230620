# Comparing `tmp/ens_sdk-0.0.4.tar.gz` & `tmp/ens_sdk-0.0.5.tar.gz`

## Comparing `ens_sdk-0.0.4.tar` & `ens_sdk-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 ens_sdk-0.0.4/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ens_sdk-0.0.4/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ens_sdk-0.0.4/src/__init__.py
--rw-r--r--   0        0        0     4274 2020-02-02 00:00:00.000000 ens_sdk-0.0.4/src/ens_sdk/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ens_sdk-0.0.4/src/ens_sdk/utils/__init__.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 ens_sdk-0.0.4/src/ens_sdk/utils/cache.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 ens_sdk-0.0.4/src/ens_sdk/utils/decouple.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 ens_sdk-0.0.4/src/ens_sdk/utils/timezone.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 ens_sdk-0.0.4/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 ens_sdk-0.0.4/LICENSE
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ens_sdk-0.0.4/README.md
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 ens_sdk-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 ens_sdk-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 ens_sdk-0.0.5/.DS_Store
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ens_sdk-0.0.5/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ens_sdk-0.0.5/src/__init__.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 ens_sdk-0.0.5/src/ens_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ens_sdk-0.0.5/src/ens_sdk/utils/__init__.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 ens_sdk-0.0.5/src/ens_sdk/utils/cache.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 ens_sdk-0.0.5/src/ens_sdk/utils/decouple.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 ens_sdk-0.0.5/src/ens_sdk/utils/timezone.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 ens_sdk-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 ens_sdk-0.0.5/LICENSE
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ens_sdk-0.0.5/README.md
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 ens_sdk-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 ens_sdk-0.0.5/PKG-INFO
```

### Comparing `ens_sdk-0.0.4/.DS_Store` & `ens_sdk-0.0.5/.DS_Store`

 * *Files identical despite different names*

### Comparing `ens_sdk-0.0.4/src/ens_sdk/__init__.py` & `ens_sdk-0.0.5/src/ens_sdk/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import base64
 import json
 from datetime import timedelta, datetime
 
 import requests
 import sentry_sdk
 
-from utils.cache import Cache
-from utils.decouple import config
-from utils.timezone import make_aware
+from .utils.cache import Cache
+from .utils.decouple import config
+from .utils.timezone import make_aware
 
 
 class ENS:
 
     def __init__(self):
         self._CLIENT_ID = config('ENCIPHER_CLIENT_ID')
         self._CLIENT_SECRET = config('ENCIPHER_CLIENT_SECRET')
```

### Comparing `ens_sdk-0.0.4/src/ens_sdk/utils/cache.py` & `ens_sdk-0.0.5/src/ens_sdk/utils/cache.py`

 * *Files identical despite different names*

### Comparing `ens_sdk-0.0.4/LICENSE` & `ens_sdk-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ens_sdk-0.0.4/pyproject.toml` & `ens_sdk-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ens_sdk"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Joseph Daudi", email="joseph@encipher.dev" },
 ]
 dependencies = ['redis', 'pydantic', 'sentry_sdk', 'requests', 'esr-sdk', 'pytz']
 description = "An SDK to simplify connectivity to ENS Services"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `ens_sdk-0.0.4/PKG-INFO` & `ens_sdk-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ens_sdk
-Version: 0.0.4
+Version: 0.0.5
 Summary: An SDK to simplify connectivity to ENS Services
 Project-URL: Homepage, https://github.com/enciphertz/encipher-notificaition-service-python-sdk
 Project-URL: Bug Tracker, https://github.com/enciphertz/encipher-notificaition-service-python-sdk/issues
 Author-email: Joseph Daudi <joseph@encipher.dev>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

