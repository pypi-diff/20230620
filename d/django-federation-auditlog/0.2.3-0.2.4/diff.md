# Comparing `tmp/django_federation_auditlog-0.2.3.tar.gz` & `tmp/django_federation_auditlog-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_federation_auditlog-0.2.3.tar", max compression
+gzip compressed data, was "django_federation_auditlog-0.2.4.tar", max compression
```

## Comparing `django_federation_auditlog-0.2.3.tar` & `django_federation_auditlog-0.2.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1432 2023-06-15 20:35:58.385636 django_federation_auditlog-0.2.3/README.md
--rw-r--r--   0        0        0        0 2023-06-15 20:35:58.385636 django_federation_auditlog-0.2.3/django_federation_auditlog/__init__.py
--rw-r--r--   0        0        0      799 2023-06-15 20:35:58.389636 django_federation_auditlog-0.2.3/django_federation_auditlog/admin.py
--rw-r--r--   0        0        0      127 2023-06-15 20:35:58.389636 django_federation_auditlog-0.2.3/django_federation_auditlog/apps.py
--rw-r--r--   0        0        0     5513 2023-06-15 20:35:58.389636 django_federation_auditlog-0.2.3/django_federation_auditlog/diff.py
--rw-r--r--   0        0        0     4175 2023-06-15 20:35:58.389636 django_federation_auditlog-0.2.3/django_federation_auditlog/middleware.py
--rw-r--r--   0        0        0     3212 2023-06-15 20:35:58.389636 django_federation_auditlog-0.2.3/django_federation_auditlog/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-06-15 20:35:58.389636 django_federation_auditlog-0.2.3/django_federation_auditlog/migrations/__init__.py
--rw-r--r--   0        0        0     2373 2023-06-15 20:35:58.389636 django_federation_auditlog-0.2.3/django_federation_auditlog/mixins.py
--rw-r--r--   0        0        0    15062 2023-06-15 20:35:58.389636 django_federation_auditlog-0.2.3/django_federation_auditlog/models.py
--rw-r--r--   0        0        0     2084 2023-06-15 20:35:58.389636 django_federation_auditlog-0.2.3/django_federation_auditlog/receivers.py
--rw-r--r--   0        0        0     4720 2023-06-15 20:35:58.389636 django_federation_auditlog-0.2.3/django_federation_auditlog/registry.py
--rw-r--r--   0        0        0       60 2023-06-15 20:35:58.389636 django_federation_auditlog-0.2.3/django_federation_auditlog/tests.py
--rw-r--r--   0        0        0      742 2023-06-15 20:35:58.389636 django_federation_auditlog-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     2091 1970-01-01 00:00:00.000000 django_federation_auditlog-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     2542 2023-06-20 20:03:52.117219 django_federation_auditlog-0.2.4/README.md
+-rw-r--r--   0        0        0       22 2023-06-20 20:03:52.117219 django_federation_auditlog-0.2.4/django_federation_auditlog/__init__.py
+-rw-r--r--   0        0        0      799 2023-06-20 20:03:52.117219 django_federation_auditlog-0.2.4/django_federation_auditlog/admin.py
+-rw-r--r--   0        0        0      127 2023-06-20 20:03:52.117219 django_federation_auditlog-0.2.4/django_federation_auditlog/apps.py
+-rw-r--r--   0        0        0     5513 2023-06-20 20:03:52.117219 django_federation_auditlog-0.2.4/django_federation_auditlog/diff.py
+-rw-r--r--   0        0        0     4175 2023-06-20 20:03:52.117219 django_federation_auditlog-0.2.4/django_federation_auditlog/middleware.py
+-rw-r--r--   0        0        0     3212 2023-06-20 20:03:52.117219 django_federation_auditlog-0.2.4/django_federation_auditlog/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-06-20 20:03:52.117219 django_federation_auditlog-0.2.4/django_federation_auditlog/migrations/__init__.py
+-rw-r--r--   0        0        0     2373 2023-06-20 20:03:52.117219 django_federation_auditlog-0.2.4/django_federation_auditlog/mixins.py
+-rw-r--r--   0        0        0    15062 2023-06-20 20:03:52.117219 django_federation_auditlog-0.2.4/django_federation_auditlog/models.py
+-rw-r--r--   0        0        0     2084 2023-06-20 20:03:52.117219 django_federation_auditlog-0.2.4/django_federation_auditlog/receivers.py
+-rw-r--r--   0        0        0     4720 2023-06-20 20:03:52.117219 django_federation_auditlog-0.2.4/django_federation_auditlog/registry.py
+-rw-r--r--   0        0        0       60 2023-06-20 20:03:52.117219 django_federation_auditlog-0.2.4/django_federation_auditlog/tests.py
+-rw-r--r--   0        0        0      742 2023-06-20 20:03:52.117219 django_federation_auditlog-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     3201 1970-01-01 00:00:00.000000 django_federation_auditlog-0.2.4/PKG-INFO
```

### Comparing `django_federation_auditlog-0.2.3/README.md` & `django_federation_auditlog-0.2.4/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -61,8 +61,48 @@
 class MyModel(models.Model):
     pass
     # Model definition goes here
 
 auditlog.register(MyModel)
 ```
 
-It is recommended to place the register code (auditlog.register(MyModel)) at the bottom of your models.py file.
+It is recommended to place the register code (auditlog.register(MyModel)) at the bottom of your models.py file.
+
+## Including Fields
+
+If ```include_fields``` is specified, only the fields with the given names will be included in the generated log entries.
+
+For example, to include only the field ```name``` from class MyModel, use:
+
+```python
+from django.db import models
+
+from django_federation_auditlog.registry import auditlog
+
+class MyModel(models.Model):
+    name = models.CharField()
+    description = models.CharField()
+    # Model definition goes here
+
+auditlog.register(MyModel, include_fields=["name"])
+```
+
+## Excluding fields
+
+Fields that are excluded will not trigger saving a new log entry and will not show up in the recorded changes.
+
+If ```exclude_fields``` is specified the fields with the given names will not be included in the generated log entries.
+
+For example, to exclude the field ```description```, use:
+
+```python
+from django.db import models
+
+from django_federation_auditlog.registry import auditlog
+
+class MyModel(models.Model):
+    name = models.CharField()
+    description = models.CharField()
+    # Model definition goes here
+
+auditlog.register(MyModel, exclude_fields=["description"])
+```
```

### Comparing `django_federation_auditlog-0.2.3/django_federation_auditlog/admin.py` & `django_federation_auditlog-0.2.4/django_federation_auditlog/admin.py`

 * *Files identical despite different names*

### Comparing `django_federation_auditlog-0.2.3/django_federation_auditlog/diff.py` & `django_federation_auditlog-0.2.4/django_federation_auditlog/diff.py`

 * *Files identical despite different names*

### Comparing `django_federation_auditlog-0.2.3/django_federation_auditlog/middleware.py` & `django_federation_auditlog-0.2.4/django_federation_auditlog/middleware.py`

 * *Files identical despite different names*

### Comparing `django_federation_auditlog-0.2.3/django_federation_auditlog/migrations/0001_initial.py` & `django_federation_auditlog-0.2.4/django_federation_auditlog/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_federation_auditlog-0.2.3/django_federation_auditlog/mixins.py` & `django_federation_auditlog-0.2.4/django_federation_auditlog/mixins.py`

 * *Files identical despite different names*

### Comparing `django_federation_auditlog-0.2.3/django_federation_auditlog/models.py` & `django_federation_auditlog-0.2.4/django_federation_auditlog/models.py`

 * *Files identical despite different names*

### Comparing `django_federation_auditlog-0.2.3/django_federation_auditlog/receivers.py` & `django_federation_auditlog-0.2.4/django_federation_auditlog/receivers.py`

 * *Files identical despite different names*

### Comparing `django_federation_auditlog-0.2.3/django_federation_auditlog/registry.py` & `django_federation_auditlog-0.2.4/django_federation_auditlog/registry.py`

 * *Files identical despite different names*

### Comparing `django_federation_auditlog-0.2.3/pyproject.toml` & `django_federation_auditlog-0.2.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-federation-auditlog"
-version = "0.2.3"
+version = "0.2.4"
 description = ""
 authors = ["Anderson Marques <anderson89marques@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 djangorestframework = "==3.11.1"
```

### Comparing `django_federation_auditlog-0.2.3/PKG-INFO` & `django_federation_auditlog-0.2.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-federation-auditlog
-Version: 0.2.3
+Version: 0.2.4
 Summary: 
 Author: Anderson Marques
 Author-email: anderson89marques@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -80,7 +80,47 @@
     pass
     # Model definition goes here
 
 auditlog.register(MyModel)
 ```
 
 It is recommended to place the register code (auditlog.register(MyModel)) at the bottom of your models.py file.
+
+## Including Fields
+
+If ```include_fields``` is specified, only the fields with the given names will be included in the generated log entries.
+
+For example, to include only the field ```name``` from class MyModel, use:
+
+```python
+from django.db import models
+
+from django_federation_auditlog.registry import auditlog
+
+class MyModel(models.Model):
+    name = models.CharField()
+    description = models.CharField()
+    # Model definition goes here
+
+auditlog.register(MyModel, include_fields=["name"])
+```
+
+## Excluding fields
+
+Fields that are excluded will not trigger saving a new log entry and will not show up in the recorded changes.
+
+If ```exclude_fields``` is specified the fields with the given names will not be included in the generated log entries.
+
+For example, to exclude the field ```description```, use:
+
+```python
+from django.db import models
+
+from django_federation_auditlog.registry import auditlog
+
+class MyModel(models.Model):
+    name = models.CharField()
+    description = models.CharField()
+    # Model definition goes here
+
+auditlog.register(MyModel, exclude_fields=["description"])
+```
```

