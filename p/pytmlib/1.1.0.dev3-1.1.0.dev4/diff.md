# Comparing `tmp/pytmlib-1.1.0.dev3.tar.gz` & `tmp/pytmlib-1.1.0.dev4.tar.gz`

## Comparing `pytmlib-1.1.0.dev3.tar` & `pytmlib-1.1.0.dev4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/pytmlib/__init__.py
--rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/pytmlib/abstract_exercise.py
--rw-r--r--   0        0        0     6046 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/pytmlib/api.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/pytmlib/archiver.py
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/pytmlib/context.py
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/pytmlib/create_app.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/pytmlib/exceptions.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/pytmlib/handle_error.py
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/pytmlib/latex.py
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/pytmlib/serializer.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/pytmlib/output/__init__.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/pytmlib/output/abstract.py
--rw-r--r--   0        0        0     8898 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/pytmlib/output/builder.py
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/pytmlib/output/button.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/pytmlib/output/field.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/pytmlib/output/field_attribute.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/pytmlib/output/field_type_enum.py
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/pytmlib/output/figure.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/pytmlib/output/image.py
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/pytmlib/output/option.py
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/pytmlib/output/option_group.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/pytmlib/output/paragraph.py
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/pytmlib/output/table.py
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/pytmlib/output/table_cell.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/LICENSE
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/README.md
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/pyproject.toml
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/PKG-INFO
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev4/pytmlib/__init__.py
+-rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev4/pytmlib/abstract_exercise.py
+-rw-r--r--   0        0        0     6039 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev4/pytmlib/api.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev4/pytmlib/archiver.py
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev4/pytmlib/context.py
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev4/pytmlib/create_app.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev4/pytmlib/exceptions.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev4/pytmlib/handle_error.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev4/pytmlib/latex.py
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev4/pytmlib/serializer.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev4/pytmlib/output/__init__.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev4/pytmlib/output/abstract.py
+-rw-r--r--   0        0        0     8898 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev4/pytmlib/output/builder.py
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev4/pytmlib/output/button.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev4/pytmlib/output/field.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev4/pytmlib/output/field_attribute.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev4/pytmlib/output/field_type_enum.py
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev4/pytmlib/output/figure.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev4/pytmlib/output/image.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev4/pytmlib/output/option.py
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev4/pytmlib/output/option_group.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev4/pytmlib/output/paragraph.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev4/pytmlib/output/table.py
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev4/pytmlib/output/table_cell.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev4/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev4/LICENSE
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev4/README.md
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev4/pyproject.toml
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev4/PKG-INFO
```

### Comparing `pytmlib-1.1.0.dev3/pytmlib/abstract_exercise.py` & `pytmlib-1.1.0.dev4/pytmlib/abstract_exercise.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev3/pytmlib/api.py` & `pytmlib-1.1.0.dev4/pytmlib/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
     def handle_entrypoints(self) -> Response:
         try:
             entrypoints = self.context.exercise.entrypoints()
         except BaseException as reason:
             raise MethodCallException() from reason
 
-        json: list = [{'name': entrypoint.__name__, 'title': entrypoint.__doc__.trim()} for entrypoint in entrypoints]
+        json: list = [{'name': entrypoint.__name__, 'title': entrypoint.__doc__} for entrypoint in entrypoints]
 
         envelop = self._wrap_with_envelop(json)
 
         return jsonify(envelop)
 
     def handle_action(self, action: str) -> Response:
         method: Callable[..., 'OutputBuilder'] = getattr(self.context.exercise, action, None)
```

### Comparing `pytmlib-1.1.0.dev3/pytmlib/archiver.py` & `pytmlib-1.1.0.dev4/pytmlib/archiver.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev3/pytmlib/context.py` & `pytmlib-1.1.0.dev4/pytmlib/context.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev3/pytmlib/create_app.py` & `pytmlib-1.1.0.dev4/pytmlib/create_app.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev3/pytmlib/handle_error.py` & `pytmlib-1.1.0.dev4/pytmlib/handle_error.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev3/pytmlib/serializer.py` & `pytmlib-1.1.0.dev4/pytmlib/serializer.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev3/pytmlib/output/abstract.py` & `pytmlib-1.1.0.dev4/pytmlib/output/abstract.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev3/pytmlib/output/builder.py` & `pytmlib-1.1.0.dev4/pytmlib/output/builder.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev3/pytmlib/output/button.py` & `pytmlib-1.1.0.dev4/pytmlib/output/button.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev3/pytmlib/output/field.py` & `pytmlib-1.1.0.dev4/pytmlib/output/field.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev3/pytmlib/output/figure.py` & `pytmlib-1.1.0.dev4/pytmlib/output/figure.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev3/pytmlib/output/image.py` & `pytmlib-1.1.0.dev4/pytmlib/output/image.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev3/pytmlib/output/option.py` & `pytmlib-1.1.0.dev4/pytmlib/output/option.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev3/pytmlib/output/option_group.py` & `pytmlib-1.1.0.dev4/pytmlib/output/option_group.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev3/pytmlib/output/paragraph.py` & `pytmlib-1.1.0.dev4/pytmlib/output/paragraph.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev3/pytmlib/output/table.py` & `pytmlib-1.1.0.dev4/pytmlib/output/table.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev3/pytmlib/output/table_cell.py` & `pytmlib-1.1.0.dev4/pytmlib/output/table_cell.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev3/LICENSE` & `pytmlib-1.1.0.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev3/pyproject.toml` & `pytmlib-1.1.0.dev4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pytmlib"
-version = "1.1.0.dev3"
+version = "1.1.0.dev4"
 authors = [
     { name = "Oliver Fabel", email = "oliver.fabel@fhnw.ch" },
 ]
 description = "This is the base library for the Python Tool Manager."
 readme = "README.md"
 license = "MIT"
 requires-python = ">=3.8"
```

### Comparing `pytmlib-1.1.0.dev3/PKG-INFO` & `pytmlib-1.1.0.dev4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytmlib
-Version: 1.1.0.dev3
+Version: 1.1.0.dev4
 Summary: This is the base library for the Python Tool Manager.
 Project-URL: Homepage, https://github.com/ofabel/pytm-bootstrap
 Project-URL: Bug Tracker, https://github.com/ofabel/pytm-bootstrap/issues
 Project-URL: Changelog, https://github.com/ofabel/pytm-bootstrap/blob/main/CHANGELOG.md
 Author-email: Oliver Fabel <oliver.fabel@fhnw.ch>
 License-Expression: MIT
 License-File: LICENSE
```

