# Comparing `tmp/kadaster_kikinzage_client-0.1.5.tar.gz` & `tmp/kadaster_kikinzage_client-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kadaster_kikinzage_client-0.1.5.tar", max compression
+gzip compressed data, was "kadaster_kikinzage_client-0.1.6.tar", max compression
```

## Comparing `kadaster_kikinzage_client-0.1.5.tar` & `kadaster_kikinzage_client-0.1.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1071 2023-06-16 12:34:44.020569 kadaster_kikinzage_client-0.1.5/LICENSE
--rw-r--r--   0        0        0     4027 2023-06-16 12:34:44.020569 kadaster_kikinzage_client-0.1.5/README.md
--rw-r--r--   0        0        0     2113 2023-06-16 12:35:02.385155 kadaster_kikinzage_client-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       45 2023-06-16 12:34:44.024570 kadaster_kikinzage_client-0.1.5/src/kikinzage/__init__.py
--rw-r--r--   0        0        0     2274 2023-06-16 12:34:44.024570 kadaster_kikinzage_client-0.1.5/src/kikinzage/__main__.py
--rw-r--r--   0        0        0      302 2023-06-16 12:34:44.024570 kadaster_kikinzage_client-0.1.5/src/kikinzage/client/__init__.py
--rw-r--r--   0        0        0     2379 2023-06-16 12:34:44.024570 kadaster_kikinzage_client-0.1.5/src/kikinzage/client/asyncio.py
--rw-r--r--   0        0        0     9405 2023-06-16 12:34:44.024570 kadaster_kikinzage_client-0.1.5/src/kikinzage/client/base.py
--rw-r--r--   0        0        0     5365 2023-06-16 12:34:44.024570 kadaster_kikinzage_client-0.1.5/src/kikinzage/client/default.py
--rw-r--r--   0        0        0      610 2023-06-16 12:34:44.024570 kadaster_kikinzage_client-0.1.5/src/kikinzage/client/errors.py
--rw-r--r--   0        0        0      182 2023-06-16 12:34:44.024570 kadaster_kikinzage_client-0.1.5/src/kikinzage/client/utils.py
--rw-r--r--   0        0        0      401 2023-06-16 12:34:44.024570 kadaster_kikinzage_client-0.1.5/src/kikinzage/models/__init__.py
--rw-r--r--   0        0        0     2927 2023-06-16 12:34:44.024570 kadaster_kikinzage_client-0.1.5/src/kikinzage/models/adres.py
--rw-r--r--   0        0        0    11899 2023-06-16 12:34:44.024570 kadaster_kikinzage_client-0.1.5/src/kikinzage/models/collectie.py
--rw-r--r--   0        0        0     5786 2023-06-16 12:34:44.024570 kadaster_kikinzage_client-0.1.5/src/kikinzage/models/eigendomsinformatie.py
--rw-r--r--   0        0        0     1445 2023-06-16 12:34:44.024570 kadaster_kikinzage_client-0.1.5/src/kikinzage/models/enum.py
--rw-r--r--   0        0        0     8739 2023-06-16 12:34:44.024570 kadaster_kikinzage_client-0.1.5/src/kikinzage/models/generated.py
--rw-r--r--   0        0        0      613 2023-06-16 12:34:44.024570 kadaster_kikinzage_client-0.1.5/src/kikinzage/models/misc.py
--rw-r--r--   0        0        0     3452 2023-06-16 12:34:44.024570 kadaster_kikinzage_client-0.1.5/src/kikinzage/models/persoon.py
--rw-r--r--   0        0        0     4030 2023-06-16 12:34:44.024570 kadaster_kikinzage_client-0.1.5/src/kikinzage/models/product.py
--rw-r--r--   0        0        0     2361 2023-06-16 12:34:44.024570 kadaster_kikinzage_client-0.1.5/src/kikinzage/models/stukken.py
--rw-r--r--   0        0        0     1195 2023-06-16 12:34:44.024570 kadaster_kikinzage_client-0.1.5/src/kikinzage/models/zekerheid.py
--rw-r--r--   0        0        0        0 2023-06-16 12:34:44.024570 kadaster_kikinzage_client-0.1.5/src/kikinzage/py.typed
--rw-r--r--   0        0        0     5083 1970-01-01 00:00:00.000000 kadaster_kikinzage_client-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-20 12:16:47.768472 kadaster_kikinzage_client-0.1.6/LICENSE
+-rw-r--r--   0        0        0     4027 2023-06-20 12:16:47.768472 kadaster_kikinzage_client-0.1.6/README.md
+-rw-r--r--   0        0        0     2113 2023-06-20 12:17:02.372542 kadaster_kikinzage_client-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0       45 2023-06-20 12:16:47.772472 kadaster_kikinzage_client-0.1.6/src/kikinzage/__init__.py
+-rw-r--r--   0        0        0     2274 2023-06-20 12:16:47.772472 kadaster_kikinzage_client-0.1.6/src/kikinzage/__main__.py
+-rw-r--r--   0        0        0      302 2023-06-20 12:16:47.772472 kadaster_kikinzage_client-0.1.6/src/kikinzage/client/__init__.py
+-rw-r--r--   0        0        0    13244 2023-06-20 12:16:47.772472 kadaster_kikinzage_client-0.1.6/src/kikinzage/client/asyncio.py
+-rw-r--r--   0        0        0    16611 2023-06-20 12:16:47.772472 kadaster_kikinzage_client-0.1.6/src/kikinzage/client/base.py
+-rw-r--r--   0        0        0    12666 2023-06-20 12:16:47.772472 kadaster_kikinzage_client-0.1.6/src/kikinzage/client/default.py
+-rw-r--r--   0        0        0      610 2023-06-20 12:16:47.772472 kadaster_kikinzage_client-0.1.6/src/kikinzage/client/errors.py
+-rw-r--r--   0        0        0      188 2023-06-20 12:16:47.772472 kadaster_kikinzage_client-0.1.6/src/kikinzage/client/utils.py
+-rw-r--r--   0        0        0      401 2023-06-20 12:16:47.772472 kadaster_kikinzage_client-0.1.6/src/kikinzage/models/__init__.py
+-rw-r--r--   0        0        0     2927 2023-06-20 12:16:47.772472 kadaster_kikinzage_client-0.1.6/src/kikinzage/models/adres.py
+-rw-r--r--   0        0        0    11899 2023-06-20 12:16:47.772472 kadaster_kikinzage_client-0.1.6/src/kikinzage/models/collectie.py
+-rw-r--r--   0        0        0     5786 2023-06-20 12:16:47.772472 kadaster_kikinzage_client-0.1.6/src/kikinzage/models/eigendomsinformatie.py
+-rw-r--r--   0        0        0     1445 2023-06-20 12:16:47.772472 kadaster_kikinzage_client-0.1.6/src/kikinzage/models/enum.py
+-rw-r--r--   0        0        0     8739 2023-06-20 12:16:47.772472 kadaster_kikinzage_client-0.1.6/src/kikinzage/models/generated.py
+-rw-r--r--   0        0        0      613 2023-06-20 12:16:47.772472 kadaster_kikinzage_client-0.1.6/src/kikinzage/models/misc.py
+-rw-r--r--   0        0        0     3452 2023-06-20 12:16:47.772472 kadaster_kikinzage_client-0.1.6/src/kikinzage/models/persoon.py
+-rw-r--r--   0        0        0     4030 2023-06-20 12:16:47.772472 kadaster_kikinzage_client-0.1.6/src/kikinzage/models/product.py
+-rw-r--r--   0        0        0     2361 2023-06-20 12:16:47.772472 kadaster_kikinzage_client-0.1.6/src/kikinzage/models/stukken.py
+-rw-r--r--   0        0        0     1195 2023-06-20 12:16:47.772472 kadaster_kikinzage_client-0.1.6/src/kikinzage/models/zekerheid.py
+-rw-r--r--   0        0        0        0 2023-06-20 12:16:47.772472 kadaster_kikinzage_client-0.1.6/src/kikinzage/py.typed
+-rw-r--r--   0        0        0     5083 1970-01-01 00:00:00.000000 kadaster_kikinzage_client-0.1.6/PKG-INFO
```

### Comparing `kadaster_kikinzage_client-0.1.5/LICENSE` & `kadaster_kikinzage_client-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.5/README.md` & `kadaster_kikinzage_client-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.5/pyproject.toml` & `kadaster_kikinzage_client-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kadaster-kikinzage-client"
-version = "0.1.5"
+version = "0.1.6"
 description = " Kadaster - KIK Inzage API Python client"
 authors = ["Jelmer Draaijer <info@jelmert.nl>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/foarsitter/kadaster-kik-inzage-api-python-client"
 repository = "https://github.com/foarsitter/kadaster-kik-inzage-api-python-client"
 documentation = "https://kadaster-kik-inzage-api-python-client.readthedocs.io"
```

### Comparing `kadaster_kikinzage_client-0.1.5/src/kikinzage/__main__.py` & `kadaster_kikinzage_client-0.1.6/src/kikinzage/__main__.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.5/src/kikinzage/client/errors.py` & `kadaster_kikinzage_client-0.1.6/src/kikinzage/client/errors.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.5/src/kikinzage/models/adres.py` & `kadaster_kikinzage_client-0.1.6/src/kikinzage/models/adres.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.5/src/kikinzage/models/collectie.py` & `kadaster_kikinzage_client-0.1.6/src/kikinzage/models/collectie.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.5/src/kikinzage/models/eigendomsinformatie.py` & `kadaster_kikinzage_client-0.1.6/src/kikinzage/models/eigendomsinformatie.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.5/src/kikinzage/models/enum.py` & `kadaster_kikinzage_client-0.1.6/src/kikinzage/models/enum.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.5/src/kikinzage/models/generated.py` & `kadaster_kikinzage_client-0.1.6/src/kikinzage/models/generated.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.5/src/kikinzage/models/misc.py` & `kadaster_kikinzage_client-0.1.6/src/kikinzage/models/misc.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.5/src/kikinzage/models/persoon.py` & `kadaster_kikinzage_client-0.1.6/src/kikinzage/models/persoon.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.5/src/kikinzage/models/product.py` & `kadaster_kikinzage_client-0.1.6/src/kikinzage/models/product.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.5/src/kikinzage/models/stukken.py` & `kadaster_kikinzage_client-0.1.6/src/kikinzage/models/stukken.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.5/src/kikinzage/models/zekerheid.py` & `kadaster_kikinzage_client-0.1.6/src/kikinzage/models/zekerheid.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.5/PKG-INFO` & `kadaster_kikinzage_client-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kadaster-kikinzage-client
-Version: 0.1.5
+Version: 0.1.6
 Summary:  Kadaster - KIK Inzage API Python client
 Home-page: https://github.com/foarsitter/kadaster-kik-inzage-api-python-client
 License: MIT
 Author: Jelmer Draaijer
 Author-email: info@jelmert.nl
 Requires-Python: >=3.8.1
 Classifier: Development Status :: 4 - Beta
```

