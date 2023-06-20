# Comparing `tmp/graphene_django_plus-5.0.tar.gz` & `tmp/graphene_django_plus-5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphene_django_plus-5.0.tar", max compression
+gzip compressed data, was "graphene_django_plus-5.1.tar", max compression
```

## Comparing `graphene_django_plus-5.0.tar` & `graphene_django_plus-5.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1077 2023-02-28 16:40:44.025170 graphene_django_plus-5.0/LICENSE
--rw-r--r--   0        0        0    10975 2023-02-28 16:40:44.025170 graphene_django_plus-5.0/README.md
--rw-r--r--   0        0        0        0 2023-02-28 16:40:44.025170 graphene_django_plus-5.0/graphene_django_plus/__init__.py
--rw-r--r--   0        0        0      338 2023-02-28 16:40:44.025170 graphene_django_plus-5.0/graphene_django_plus/exceptions.py
--rw-r--r--   0        0        0     1526 2023-02-28 16:40:44.025170 graphene_django_plus-5.0/graphene_django_plus/fields.py
--rw-r--r--   0        0        0     1894 2023-02-28 16:40:44.025170 graphene_django_plus-5.0/graphene_django_plus/input_types.py
--rw-r--r--   0        0        0     8790 2023-02-28 16:40:44.025170 graphene_django_plus-5.0/graphene_django_plus/models.py
--rw-r--r--   0        0        0    24058 2023-02-28 16:40:44.025170 graphene_django_plus-5.0/graphene_django_plus/mutations.py
--rw-r--r--   0        0        0     1564 2023-02-28 16:40:44.025170 graphene_django_plus-5.0/graphene_django_plus/perms.py
--rw-r--r--   0        0        0      911 2023-02-28 16:40:44.025170 graphene_django_plus-5.0/graphene_django_plus/queries.py
--rw-r--r--   0        0        0     5371 2023-02-28 16:40:44.025170 graphene_django_plus-5.0/graphene_django_plus/schema.py
--rw-r--r--   0        0        0     3874 2023-02-28 16:40:44.029170 graphene_django_plus-5.0/graphene_django_plus/settings.py
--rw-r--r--   0        0        0    15238 2023-02-28 16:40:44.029170 graphene_django_plus-5.0/graphene_django_plus/types.py
--rw-r--r--   0        0        0     5772 2023-02-28 16:40:44.029170 graphene_django_plus-5.0/graphene_django_plus/utils.py
--rw-r--r--   0        0        0     1980 2023-02-28 16:40:44.029170 graphene_django_plus-5.0/graphene_django_plus/views.py
--rw-r--r--   0        0        0     3099 2023-02-28 16:40:44.029170 graphene_django_plus-5.0/pyproject.toml
--rw-r--r--   0        0        0    12558 1970-01-01 00:00:00.000000 graphene_django_plus-5.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-06-20 18:09:55.916748 graphene_django_plus-5.1/LICENSE
+-rw-r--r--   0        0        0    10975 2023-06-20 18:09:55.916748 graphene_django_plus-5.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-20 18:09:55.916748 graphene_django_plus-5.1/graphene_django_plus/__init__.py
+-rw-r--r--   0        0        0      338 2023-06-20 18:09:55.916748 graphene_django_plus-5.1/graphene_django_plus/exceptions.py
+-rw-r--r--   0        0        0     1526 2023-06-20 18:09:55.916748 graphene_django_plus-5.1/graphene_django_plus/fields.py
+-rw-r--r--   0        0        0     1894 2023-06-20 18:09:55.916748 graphene_django_plus-5.1/graphene_django_plus/input_types.py
+-rw-r--r--   0        0        0     8790 2023-06-20 18:09:55.916748 graphene_django_plus-5.1/graphene_django_plus/models.py
+-rw-r--r--   0        0        0    24058 2023-06-20 18:09:55.916748 graphene_django_plus-5.1/graphene_django_plus/mutations.py
+-rw-r--r--   0        0        0     1564 2023-06-20 18:09:55.916748 graphene_django_plus-5.1/graphene_django_plus/perms.py
+-rw-r--r--   0        0        0      911 2023-06-20 18:09:55.916748 graphene_django_plus-5.1/graphene_django_plus/queries.py
+-rw-r--r--   0        0        0     5289 2023-06-20 18:09:55.916748 graphene_django_plus-5.1/graphene_django_plus/schema.py
+-rw-r--r--   0        0        0     3874 2023-06-20 18:09:55.916748 graphene_django_plus-5.1/graphene_django_plus/settings.py
+-rw-r--r--   0        0        0    15238 2023-06-20 18:09:55.916748 graphene_django_plus-5.1/graphene_django_plus/types.py
+-rw-r--r--   0        0        0     5772 2023-06-20 18:09:55.916748 graphene_django_plus-5.1/graphene_django_plus/utils.py
+-rw-r--r--   0        0        0     1980 2023-06-20 18:09:55.916748 graphene_django_plus-5.1/graphene_django_plus/views.py
+-rw-r--r--   0        0        0     3044 2023-06-20 18:09:55.920748 graphene_django_plus-5.1/pyproject.toml
+-rw-r--r--   0        0        0    12301 1970-01-01 00:00:00.000000 graphene_django_plus-5.1/PKG-INFO
```

### Comparing `graphene_django_plus-5.0/LICENSE` & `graphene_django_plus-5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `graphene_django_plus-5.0/README.md` & `graphene_django_plus-5.1/README.md`

 * *Files identical despite different names*

### Comparing `graphene_django_plus-5.0/graphene_django_plus/fields.py` & `graphene_django_plus-5.1/graphene_django_plus/fields.py`

 * *Files identical despite different names*

### Comparing `graphene_django_plus-5.0/graphene_django_plus/input_types.py` & `graphene_django_plus-5.1/graphene_django_plus/input_types.py`

 * *Files identical despite different names*

### Comparing `graphene_django_plus-5.0/graphene_django_plus/models.py` & `graphene_django_plus-5.1/graphene_django_plus/models.py`

 * *Files identical despite different names*

### Comparing `graphene_django_plus-5.0/graphene_django_plus/mutations.py` & `graphene_django_plus-5.1/graphene_django_plus/mutations.py`

 * *Files identical despite different names*

### Comparing `graphene_django_plus-5.0/graphene_django_plus/perms.py` & `graphene_django_plus-5.1/graphene_django_plus/perms.py`

 * *Files identical despite different names*

### Comparing `graphene_django_plus-5.0/graphene_django_plus/queries.py` & `graphene_django_plus-5.1/graphene_django_plus/queries.py`

 * *Files identical despite different names*

### Comparing `graphene_django_plus-5.0/graphene_django_plus/schema.py` & `graphene_django_plus-5.1/graphene_django_plus/schema.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,12 @@
 import functools
 
 from django.db import models
 import graphene
-from graphene_django.compat import (
-    ArrayField,
-    HStoreField,
-    JSONField,
-    PGJSONField,
-    RangeField,
-)
+from graphene_django.compat import ArrayField, HStoreField, RangeField
 from graphene_django.registry import get_global_registry
 
 _registry = get_global_registry()
 
 
 class FieldKind(graphene.Enum):
     """Field kind."""
@@ -205,14 +199,13 @@
 @get_field_schema.register(RangeField)
 def get_field_schema_array(field, registry=None):
     d = get_field_schema(field.base_field)
     d["multiple"] = True
     return d
 
 
-@get_field_schema.register(PGJSONField)
-@get_field_schema.register(JSONField)
+@get_field_schema.register(models.JSONField)
 @get_field_schema.register(HStoreField)
 def get_field_schema_pg(field, registry=None):
     return {
         "kind": FieldKind.JSON,
     }
```

### Comparing `graphene_django_plus-5.0/graphene_django_plus/settings.py` & `graphene_django_plus-5.1/graphene_django_plus/settings.py`

 * *Files identical despite different names*

### Comparing `graphene_django_plus-5.0/graphene_django_plus/types.py` & `graphene_django_plus-5.1/graphene_django_plus/types.py`

 * *Files identical despite different names*

### Comparing `graphene_django_plus-5.0/graphene_django_plus/utils.py` & `graphene_django_plus-5.1/graphene_django_plus/utils.py`

 * *Files identical despite different names*

### Comparing `graphene_django_plus-5.0/graphene_django_plus/views.py` & `graphene_django_plus-5.1/graphene_django_plus/views.py`

 * *Files identical despite different names*

### Comparing `graphene_django_plus-5.0/pyproject.toml` & `graphene_django_plus-5.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 [tool.poetry]
 name = "graphene-django-plus"
-version = "5.0"
+version = "5.1"
 description = "Tools to easily create permissioned CRUD endpoints in graphene."
 authors = ["Thiago Bellini Ribeiro <thiago@bellini.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/0soft/graphene-django-plus"
 repository = "https://github.com/0soft/graphene-django-plus"
 documentation = "https://graphene-django-plus.readthedocs.io"
 keywords = ["graphene", "django", "graphql", "crud", "permissions"]
 classifiers = [
-    "Development Status :: 5 - Production/Stable",
-    "Environment :: Web Environment",
-    "Intended Audience :: Developers",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Framework :: Django",
-    "Framework :: Django :: 2.2",
-    "Framework :: Django :: 3.0",
-    "Framework :: Django :: 3.1",
-    "Framework :: Django :: 3.2",
-    "Framework :: Django :: 4.0",
-    "Framework :: Django :: 4.1",
+  "Development Status :: 5 - Production/Stable",
+  "Environment :: Web Environment",
+  "Intended Audience :: Developers",
+  "License :: OSI Approved :: MIT License",
+  "Operating System :: OS Independent",
+  "Programming Language :: Python",
+  "Programming Language :: Python :: 3",
+  "Programming Language :: Python :: 3.8",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Framework :: Django",
+  "Framework :: Django :: 3.2",
+  "Framework :: Django :: 4.0",
+  "Framework :: Django :: 4.1",
+  "Framework :: Django :: 4.2",
 ]
 packages = [{ include = "graphene_django_plus" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
+django = ">=3.2"
+graphene-django = ">=3.1.2"
 
 [tool.poetry.dev-dependencies]
 black = "^22.3.0"
 codecov = "^2.1.11"
 django = "^4.1.7"
 django-filter = "^22.1"
 django-guardian = "^2.3.0"
@@ -46,15 +46,15 @@
 flake8-bugbear = "^22.1.11"
 flake8-builtins = "^1.5.3"
 flake8-comprehensions = "^3.7.0"
 flake8-polyfill = "^1.0.2"
 flake8-return = "^1.1.3"
 flake8-simplify = "^0.19.2"
 graphene = "^3.2.1"
-graphene-django = "^3.0.0"
+graphene-django = "^3.1.2"
 graphene-django-optimizer = { git = "https://github.com/bellini666/graphene-django-optimizer.git" }
 mock = "^5.0.1"
 pytest = "^7.1.2"
 pytest-cov = "^4.0.0"
 pytest-env = "^0.8.1"
 pytest-django = "^4.2.0"
 pytest-mock = "^3.6.1"
```

### Comparing `graphene_django_plus-5.0/PKG-INFO` & `graphene_django_plus-5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,35 @@
 Metadata-Version: 2.1
 Name: graphene-django-plus
-Version: 5.0
+Version: 5.1
 Summary: Tools to easily create permissioned CRUD endpoints in graphene.
 Home-page: https://github.com/0soft/graphene-django-plus
 License: MIT
 Keywords: graphene,django,graphql,crud,permissions
 Author: Thiago Bellini Ribeiro
 Author-email: thiago@bellini.dev
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: django (>=3.2)
+Requires-Dist: graphene-django (>=3.1.2)
 Project-URL: Documentation, https://graphene-django-plus.readthedocs.io
 Project-URL: Repository, https://github.com/0soft/graphene-django-plus
 Description-Content-Type: text/markdown
 
 # graphene-django-plus
 
 [![build status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2F0soft%2Fgraphene-django-plus%2Fbadge%3Fref%3Dmaster&style=flat)](https://actions-badge.atrox.dev/0soft/graphene-django-plus/goto?ref=master)
```

