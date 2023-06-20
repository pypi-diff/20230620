# Comparing `tmp/ens_sdk-0.0.2.tar.gz` & `tmp/ens_sdk-0.0.3.tar.gz`

## Comparing `ens_sdk-0.0.2.tar` & `ens_sdk-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 ens_sdk-0.0.2/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ens_sdk-0.0.2/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ens_sdk-0.0.2/src/__init__.py
--rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 ens_sdk-0.0.2/src/ens_sdk/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ens_sdk-0.0.2/src/ens_sdk/utils/__init__.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 ens_sdk-0.0.2/src/ens_sdk/utils/cache.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 ens_sdk-0.0.2/src/ens_sdk/utils/decouple.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 ens_sdk-0.0.2/src/ens_sdk/utils/timezone.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 ens_sdk-0.0.2/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 ens_sdk-0.0.2/LICENSE
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ens_sdk-0.0.2/README.md
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 ens_sdk-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 ens_sdk-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 ens_sdk-0.0.3/.DS_Store
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ens_sdk-0.0.3/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ens_sdk-0.0.3/src/__init__.py
+-rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 ens_sdk-0.0.3/src/ens_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ens_sdk-0.0.3/src/ens_sdk/utils/__init__.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 ens_sdk-0.0.3/src/ens_sdk/utils/cache.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 ens_sdk-0.0.3/src/ens_sdk/utils/decouple.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 ens_sdk-0.0.3/src/ens_sdk/utils/timezone.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 ens_sdk-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 ens_sdk-0.0.3/LICENSE
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ens_sdk-0.0.3/README.md
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 ens_sdk-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 ens_sdk-0.0.3/PKG-INFO
```

### Comparing `ens_sdk-0.0.2/.DS_Store` & `ens_sdk-0.0.3/.DS_Store`

 * *Files identical despite different names*

### Comparing `ens_sdk-0.0.2/src/ens_sdk/__init__.py` & `ens_sdk-0.0.3/src/ens_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `ens_sdk-0.0.2/src/ens_sdk/utils/cache.py` & `ens_sdk-0.0.3/src/ens_sdk/utils/cache.py`

 * *Files identical despite different names*

### Comparing `ens_sdk-0.0.2/LICENSE` & `ens_sdk-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ens_sdk-0.0.2/pyproject.toml` & `ens_sdk-0.0.3/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ens_sdk"
-version = "0.0.2"
+version = "v0.0.3"
 authors = [
   { name="Joseph Daudi", email="joseph@encipher.dev" },
 ]
+dependencies = ['redis', 'pydantic', 'sentry_sdk', 'requests', 'esr-sdk']
 description = "An SDK to simplify connectivity to ENS Services"
 readme = "README.md"
 requires-python = ">=3.9"
-requirements = ['redis', 'pydantic', 'sentry_sdk', 'requests', 'esr-sdk']
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

