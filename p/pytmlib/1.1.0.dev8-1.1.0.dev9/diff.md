# Comparing `tmp/pytmlib-1.1.0.dev8.tar.gz` & `tmp/pytmlib-1.1.0.dev9.tar.gz`

## Comparing `pytmlib-1.1.0.dev8.tar` & `pytmlib-1.1.0.dev9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/pytmlib/__init__.py
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/pytmlib/abstract_exercise.py
--rw-r--r--   0        0        0     6450 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/pytmlib/api.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/pytmlib/archiver.py
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/pytmlib/context.py
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/pytmlib/create_app.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/pytmlib/decorators.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/pytmlib/exceptions.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/pytmlib/handle_error.py
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/pytmlib/latex.py
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/pytmlib/serializer.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/pytmlib/types.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/pytmlib/output/__init__.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/pytmlib/output/abstract.py
--rw-r--r--   0        0        0     8898 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/pytmlib/output/builder.py
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/pytmlib/output/button.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/pytmlib/output/field.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/pytmlib/output/field_attribute.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/pytmlib/output/field_type_enum.py
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/pytmlib/output/figure.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/pytmlib/output/image.py
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/pytmlib/output/option.py
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/pytmlib/output/option_group.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/pytmlib/output/paragraph.py
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/pytmlib/output/table.py
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/pytmlib/output/table_cell.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/LICENSE
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/README.md
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/pyproject.toml
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/PKG-INFO
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev9/pytmlib/__init__.py
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev9/pytmlib/abstract_exercise.py
+-rw-r--r--   0        0        0     6450 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev9/pytmlib/api.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev9/pytmlib/archiver.py
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev9/pytmlib/context.py
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev9/pytmlib/create_app.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev9/pytmlib/decorators.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev9/pytmlib/exceptions.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev9/pytmlib/handle_error.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev9/pytmlib/latex.py
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev9/pytmlib/serializer.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev9/pytmlib/types.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev9/pytmlib/output/__init__.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev9/pytmlib/output/abstract.py
+-rw-r--r--   0        0        0     8898 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev9/pytmlib/output/builder.py
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev9/pytmlib/output/button.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev9/pytmlib/output/field.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev9/pytmlib/output/field_attribute.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev9/pytmlib/output/field_type_enum.py
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev9/pytmlib/output/figure.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev9/pytmlib/output/image.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev9/pytmlib/output/option.py
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev9/pytmlib/output/option_group.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev9/pytmlib/output/paragraph.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev9/pytmlib/output/table.py
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev9/pytmlib/output/table_cell.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev9/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev9/LICENSE
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev9/README.md
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev9/pyproject.toml
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev9/PKG-INFO
```

### Comparing `pytmlib-1.1.0.dev8/pytmlib/abstract_exercise.py` & `pytmlib-1.1.0.dev9/pytmlib/abstract_exercise.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,26 +7,34 @@
 
 from .context import Context
 from .create_app import create_app
 from .decorators import ENTRYPOINT_MARKER
 from .output import OutputBuilder as Output
 from .types import Action
 
+PYTM_UID_ENV = 'PYTM_UID'
+PYTM_SECRET_ENV = 'PYTM_SECRET'
+HOSTNAME_ENV = 'HOSTNAME'
+
 
 class AbstractExercise(abc.ABC):
-    def __new__(cls, unique_id: str, static_folder_path: str = None, *args, **kwargs):
+    def __new__(cls, unique_id: str = None, static_folder_path: str = None, *args, **kwargs):
         exercise: AbstractExercise = super().__new__(cls, *args, **kwargs)
 
+        unique_id = os.getenv(PYTM_UID_ENV, unique_id)
         secret, fallback = AbstractExercise._get_secret()
         context: Context = Context(unique_id, secret, exercise)
 
         exercise._context = context
 
+        if unique_id is None:
+            logging.warning('missing %s environment variable', PYTM_UID_ENV)
+
         if fallback:
-            logging.warning('missing PYTM_SECRET environment variable')
+            logging.warning('missing %s environment variable', PYTM_SECRET_ENV)
 
         return create_app(context, static_folder_path)
 
     @property
     def output(self) -> Output:
         return self._context.output
 
@@ -39,13 +47,13 @@
             func = getattr(self, name)
 
             if hasattr(func, ENTRYPOINT_MARKER):
                 yield func
 
     @staticmethod
     def _get_secret() -> Tuple[str, bool]:
-        hostname: str = os.getenv('HOSTNAME', os.name)
+        hostname: str = os.getenv(HOSTNAME_ENV, os.name)
         fallback: uuid = uuid.uuid5(uuid.NAMESPACE_DNS, hostname)
-        secret: str = os.getenv('PYTM_SECRET')
+        secret: str = os.getenv(PYTM_SECRET_ENV)
         use_fallback: bool = secret is None
 
         return str(fallback) if use_fallback else secret, use_fallback
```

### Comparing `pytmlib-1.1.0.dev8/pytmlib/api.py` & `pytmlib-1.1.0.dev9/pytmlib/api.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev8/pytmlib/archiver.py` & `pytmlib-1.1.0.dev9/pytmlib/archiver.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev8/pytmlib/context.py` & `pytmlib-1.1.0.dev9/pytmlib/context.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev8/pytmlib/create_app.py` & `pytmlib-1.1.0.dev9/pytmlib/create_app.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev8/pytmlib/decorators.py` & `pytmlib-1.1.0.dev9/pytmlib/decorators.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev8/pytmlib/handle_error.py` & `pytmlib-1.1.0.dev9/pytmlib/handle_error.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev8/pytmlib/serializer.py` & `pytmlib-1.1.0.dev9/pytmlib/serializer.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev8/pytmlib/output/abstract.py` & `pytmlib-1.1.0.dev9/pytmlib/output/abstract.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev8/pytmlib/output/builder.py` & `pytmlib-1.1.0.dev9/pytmlib/output/builder.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev8/pytmlib/output/button.py` & `pytmlib-1.1.0.dev9/pytmlib/output/button.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev8/pytmlib/output/field.py` & `pytmlib-1.1.0.dev9/pytmlib/output/field.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev8/pytmlib/output/figure.py` & `pytmlib-1.1.0.dev9/pytmlib/output/figure.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev8/pytmlib/output/image.py` & `pytmlib-1.1.0.dev9/pytmlib/output/image.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev8/pytmlib/output/option.py` & `pytmlib-1.1.0.dev9/pytmlib/output/option.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev8/pytmlib/output/option_group.py` & `pytmlib-1.1.0.dev9/pytmlib/output/option_group.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev8/pytmlib/output/paragraph.py` & `pytmlib-1.1.0.dev9/pytmlib/output/paragraph.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev8/pytmlib/output/table.py` & `pytmlib-1.1.0.dev9/pytmlib/output/table.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev8/pytmlib/output/table_cell.py` & `pytmlib-1.1.0.dev9/pytmlib/output/table_cell.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev8/LICENSE` & `pytmlib-1.1.0.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev8/pyproject.toml` & `pytmlib-1.1.0.dev9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pytmlib"
-version = "1.1.0.dev8"
+version = "1.1.0.dev9"
 authors = [
     { name = "Oliver Fabel", email = "oliver.fabel@fhnw.ch" },
 ]
 description = "This is the base library for the Python Tool Manager."
 readme = "README.md"
 license = "MIT"
 requires-python = ">=3.8"
```

### Comparing `pytmlib-1.1.0.dev8/PKG-INFO` & `pytmlib-1.1.0.dev9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytmlib
-Version: 1.1.0.dev8
+Version: 1.1.0.dev9
 Summary: This is the base library for the Python Tool Manager.
 Project-URL: Homepage, https://github.com/ofabel/pytm-bootstrap
 Project-URL: Bug Tracker, https://github.com/ofabel/pytm-bootstrap/issues
 Project-URL: Changelog, https://github.com/ofabel/pytm-bootstrap/blob/main/CHANGELOG.md
 Author-email: Oliver Fabel <oliver.fabel@fhnw.ch>
 License-Expression: MIT
 License-File: LICENSE
```

