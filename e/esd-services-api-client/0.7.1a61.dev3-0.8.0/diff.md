# Comparing `tmp/esd_services_api_client-0.7.1a61.dev3.tar.gz` & `tmp/esd_services_api_client-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esd_services_api_client-0.7.1a61.dev3.tar", max compression
+gzip compressed data, was "esd_services_api_client-0.8.0.tar", max compression
```

## Comparing `esd_services_api_client-0.7.1a61.dev3.tar` & `esd_services_api_client-0.8.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    10693 2023-06-16 13:03:51.676208 esd_services_api_client-0.7.1a61.dev3/LICENSE
--rw-r--r--   0        0        0      111 2023-06-16 13:03:51.676208 esd_services_api_client-0.7.1a61.dev3/README.md
--rw-r--r--   0        0        0      598 2023-06-16 13:03:51.676208 esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/__init__.py
--rw-r--r--   0        0        0       31 2023-06-16 13:04:12.476672 esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/_version.py
--rw-r--r--   0        0        0      743 2023-06-16 13:03:51.676208 esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/beast/__init__.py
--rw-r--r--   0        0        0     2666 2023-06-16 13:03:51.676208 esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/beast/_auth.py
--rw-r--r--   0        0        0    10369 2023-06-16 13:03:51.676208 esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/beast/_connector.py
--rw-r--r--   0        0        0     9442 2023-06-16 13:03:51.676208 esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/beast/_models.py
--rw-r--r--   0        0        0     2221 2023-06-16 13:03:51.676208 esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/boxer/README.md
--rw-r--r--   0        0        0      780 2023-06-16 13:03:51.676208 esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/boxer/__init__.py
--rw-r--r--   0        0        0     5214 2023-06-16 13:03:51.676208 esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/boxer/_auth.py
--rw-r--r--   0        0        0      976 2023-06-16 13:03:51.676208 esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/boxer/_base.py
--rw-r--r--   0        0        0     8272 2023-06-16 13:03:51.676208 esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/boxer/_connector.py
--rw-r--r--   0        0        0     1736 2023-06-16 13:03:51.676208 esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/boxer/_helpers.py
--rw-r--r--   0        0        0     3105 2023-06-16 13:03:51.676208 esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/boxer/_models.py
--rw-r--r--   0        0        0      598 2023-06-16 13:03:51.676208 esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/common/__init__.py
--rw-r--r--   0        0        0      787 2023-06-16 13:03:51.676208 esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/crystal/__init__.py
--rw-r--r--   0        0        0      832 2023-06-16 13:03:51.676208 esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/crystal/_api_versions.py
--rw-r--r--   0        0        0    12015 2023-06-16 13:03:51.676208 esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/crystal/_connector.py
--rw-r--r--   0        0        0     4025 2023-06-16 13:03:51.676208 esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/crystal/_models.py
--rw-r--r--   0        0        0      958 2023-06-16 13:04:12.476672 esd_services_api_client-0.7.1a61.dev3/pyproject.toml
--rw-r--r--   0        0        0     1085 1970-01-01 00:00:00.000000 esd_services_api_client-0.7.1a61.dev3/PKG-INFO
+-rw-r--r--   0        0        0    10693 2023-06-20 13:22:24.363952 esd_services_api_client-0.8.0/LICENSE
+-rw-r--r--   0        0        0      111 2023-06-20 13:22:24.363952 esd_services_api_client-0.8.0/README.md
+-rw-r--r--   0        0        0      598 2023-06-20 13:22:24.363952 esd_services_api_client-0.8.0/esd_services_api_client/__init__.py
+-rw-r--r--   0        0        0       22 2023-06-20 13:22:39.136227 esd_services_api_client-0.8.0/esd_services_api_client/_version.py
+-rw-r--r--   0        0        0      743 2023-06-20 13:22:24.363952 esd_services_api_client-0.8.0/esd_services_api_client/beast/__init__.py
+-rw-r--r--   0        0        0     2666 2023-06-20 13:22:24.367952 esd_services_api_client-0.8.0/esd_services_api_client/beast/_auth.py
+-rw-r--r--   0        0        0    10369 2023-06-20 13:22:24.367952 esd_services_api_client-0.8.0/esd_services_api_client/beast/_connector.py
+-rw-r--r--   0        0        0     9442 2023-06-20 13:22:24.367952 esd_services_api_client-0.8.0/esd_services_api_client/beast/_models.py
+-rw-r--r--   0        0        0     2221 2023-06-20 13:22:24.367952 esd_services_api_client-0.8.0/esd_services_api_client/boxer/README.md
+-rw-r--r--   0        0        0      780 2023-06-20 13:22:24.367952 esd_services_api_client-0.8.0/esd_services_api_client/boxer/__init__.py
+-rw-r--r--   0        0        0     5214 2023-06-20 13:22:24.367952 esd_services_api_client-0.8.0/esd_services_api_client/boxer/_auth.py
+-rw-r--r--   0        0        0      976 2023-06-20 13:22:24.367952 esd_services_api_client-0.8.0/esd_services_api_client/boxer/_base.py
+-rw-r--r--   0        0        0     8272 2023-06-20 13:22:24.367952 esd_services_api_client-0.8.0/esd_services_api_client/boxer/_connector.py
+-rw-r--r--   0        0        0     1736 2023-06-20 13:22:24.367952 esd_services_api_client-0.8.0/esd_services_api_client/boxer/_helpers.py
+-rw-r--r--   0        0        0     3105 2023-06-20 13:22:24.367952 esd_services_api_client-0.8.0/esd_services_api_client/boxer/_models.py
+-rw-r--r--   0        0        0      598 2023-06-20 13:22:24.367952 esd_services_api_client-0.8.0/esd_services_api_client/common/__init__.py
+-rw-r--r--   0        0        0      787 2023-06-20 13:22:24.367952 esd_services_api_client-0.8.0/esd_services_api_client/crystal/__init__.py
+-rw-r--r--   0        0        0      832 2023-06-20 13:22:24.367952 esd_services_api_client-0.8.0/esd_services_api_client/crystal/_api_versions.py
+-rw-r--r--   0        0        0    12015 2023-06-20 13:22:24.367952 esd_services_api_client-0.8.0/esd_services_api_client/crystal/_connector.py
+-rw-r--r--   0        0        0     4025 2023-06-20 13:22:24.367952 esd_services_api_client-0.8.0/esd_services_api_client/crystal/_models.py
+-rw-r--r--   0        0        0      949 2023-06-20 13:22:39.136227 esd_services_api_client-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     1077 1970-01-01 00:00:00.000000 esd_services_api_client-0.8.0/PKG-INFO
```

### Comparing `esd_services_api_client-0.7.1a61.dev3/LICENSE` & `esd_services_api_client-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/__init__.py` & `esd_services_api_client-0.8.0/esd_services_api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/beast/__init__.py` & `esd_services_api_client-0.8.0/esd_services_api_client/beast/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/beast/_auth.py` & `esd_services_api_client-0.8.0/esd_services_api_client/beast/_auth.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/beast/_connector.py` & `esd_services_api_client-0.8.0/esd_services_api_client/beast/_connector.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/beast/_models.py` & `esd_services_api_client-0.8.0/esd_services_api_client/beast/_models.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/boxer/README.md` & `esd_services_api_client-0.8.0/esd_services_api_client/boxer/README.md`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/boxer/__init__.py` & `esd_services_api_client-0.8.0/esd_services_api_client/boxer/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/boxer/_auth.py` & `esd_services_api_client-0.8.0/esd_services_api_client/boxer/_auth.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/boxer/_base.py` & `esd_services_api_client-0.8.0/esd_services_api_client/boxer/_base.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/boxer/_connector.py` & `esd_services_api_client-0.8.0/esd_services_api_client/boxer/_connector.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/boxer/_helpers.py` & `esd_services_api_client-0.8.0/esd_services_api_client/boxer/_helpers.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/boxer/_models.py` & `esd_services_api_client-0.8.0/esd_services_api_client/boxer/_models.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/common/__init__.py` & `esd_services_api_client-0.8.0/esd_services_api_client/common/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/crystal/__init__.py` & `esd_services_api_client-0.8.0/esd_services_api_client/crystal/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/crystal/_api_versions.py` & `esd_services_api_client-0.8.0/esd_services_api_client/crystal/_api_versions.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/crystal/_connector.py` & `esd_services_api_client-0.8.0/esd_services_api_client/crystal/_connector.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/crystal/_models.py` & `esd_services_api_client-0.8.0/esd_services_api_client/crystal/_models.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.7.1a61.dev3/pyproject.toml` & `esd_services_api_client-0.8.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "esd-services-api-client"
-version = "v0.7.1a61.dev3"
+version = "0.8.0"
 description = "Python clients for ESD services"
 authors = ["ECCO Sneaks & Data <esdsupport@ecco.com>"]
 maintainers = ['GZU <gzu@ecco.com>', 'JRB <ext-jrb@ecco.com>', 'VISA <visa@ecco.com>']
 readme = "README.md"
 license = 'Apache 2.0'
 repository = 'https://github.com/SneaksAndData/esd-services-api-client'
```

### Comparing `esd_services_api_client-0.7.1a61.dev3/PKG-INFO` & `esd_services_api_client-0.8.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esd-services-api-client
-Version: 0.7.1a61.dev3
+Version: 0.8.0
 Summary: Python clients for ESD services
 Home-page: https://github.com/SneaksAndData/esd-services-api-client
 License: Apache 2.0
 Author: ECCO Sneaks & Data
 Author-email: esdsupport@ecco.com
 Maintainer: GZU
 Maintainer-email: gzu@ecco.com
```

