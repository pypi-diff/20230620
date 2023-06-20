# Comparing `tmp/pytmlib-1.1.0.dev5.tar.gz` & `tmp/pytmlib-1.1.0.dev6.tar.gz`

## Comparing `pytmlib-1.1.0.dev5.tar` & `pytmlib-1.1.0.dev6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev5/pytmlib/__init__.py
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev5/pytmlib/abstract_exercise.py
--rw-r--r--   0        0        0     5968 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev5/pytmlib/api.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev5/pytmlib/archiver.py
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev5/pytmlib/context.py
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev5/pytmlib/create_app.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev5/pytmlib/decorators.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev5/pytmlib/exceptions.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev5/pytmlib/handle_error.py
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev5/pytmlib/latex.py
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev5/pytmlib/serializer.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev5/pytmlib/types.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev5/pytmlib/output/__init__.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev5/pytmlib/output/abstract.py
--rw-r--r--   0        0        0     8898 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev5/pytmlib/output/builder.py
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev5/pytmlib/output/button.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev5/pytmlib/output/field.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev5/pytmlib/output/field_attribute.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev5/pytmlib/output/field_type_enum.py
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev5/pytmlib/output/figure.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev5/pytmlib/output/image.py
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev5/pytmlib/output/option.py
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev5/pytmlib/output/option_group.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev5/pytmlib/output/paragraph.py
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev5/pytmlib/output/table.py
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev5/pytmlib/output/table_cell.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev5/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev5/LICENSE
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev5/README.md
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev5/pyproject.toml
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev5/PKG-INFO
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev6/pytmlib/__init__.py
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev6/pytmlib/abstract_exercise.py
+-rw-r--r--   0        0        0     5983 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev6/pytmlib/api.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev6/pytmlib/archiver.py
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev6/pytmlib/context.py
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev6/pytmlib/create_app.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev6/pytmlib/decorators.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev6/pytmlib/exceptions.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev6/pytmlib/handle_error.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev6/pytmlib/latex.py
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev6/pytmlib/serializer.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev6/pytmlib/types.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev6/pytmlib/output/__init__.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev6/pytmlib/output/abstract.py
+-rw-r--r--   0        0        0     8898 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev6/pytmlib/output/builder.py
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev6/pytmlib/output/button.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev6/pytmlib/output/field.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev6/pytmlib/output/field_attribute.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev6/pytmlib/output/field_type_enum.py
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev6/pytmlib/output/figure.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev6/pytmlib/output/image.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev6/pytmlib/output/option.py
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev6/pytmlib/output/option_group.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev6/pytmlib/output/paragraph.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev6/pytmlib/output/table.py
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev6/pytmlib/output/table_cell.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev6/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev6/LICENSE
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev6/README.md
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev6/pyproject.toml
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev6/PKG-INFO
```

### Comparing `pytmlib-1.1.0.dev5/pytmlib/abstract_exercise.py` & `pytmlib-1.1.0.dev6/pytmlib/abstract_exercise.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev5/pytmlib/api.py` & `pytmlib-1.1.0.dev6/pytmlib/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,15 +139,15 @@
         if parameter.kind == Parameter.POSITIONAL_OR_KEYWORD:
             arguments[name] = applicable_arguments.pop(name)
         # apply kwargs
         elif parameter.kind == Parameter.VAR_KEYWORD:
             arguments.update(**applicable_arguments)
 
     def _get_entrypoint_by_name(self, name: str) -> Entrypoint:
-        for entrypoint in self.context.entrypoints:
+        for entrypoint in self.context.exercise.get_entrypoints():
             if entrypoint.__name__ == name:
                 return entrypoint
         raise EntrypointNotFound
 
     @staticmethod
     def _call_method(method: Entrypoint, **kwargs) -> 'OutputBuilder':
         try:
```

### Comparing `pytmlib-1.1.0.dev5/pytmlib/archiver.py` & `pytmlib-1.1.0.dev6/pytmlib/archiver.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev5/pytmlib/create_app.py` & `pytmlib-1.1.0.dev6/pytmlib/create_app.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev5/pytmlib/handle_error.py` & `pytmlib-1.1.0.dev6/pytmlib/handle_error.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev5/pytmlib/serializer.py` & `pytmlib-1.1.0.dev6/pytmlib/serializer.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev5/pytmlib/output/abstract.py` & `pytmlib-1.1.0.dev6/pytmlib/output/abstract.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev5/pytmlib/output/builder.py` & `pytmlib-1.1.0.dev6/pytmlib/output/builder.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev5/pytmlib/output/button.py` & `pytmlib-1.1.0.dev6/pytmlib/output/button.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev5/pytmlib/output/field.py` & `pytmlib-1.1.0.dev6/pytmlib/output/field.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev5/pytmlib/output/figure.py` & `pytmlib-1.1.0.dev6/pytmlib/output/figure.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev5/pytmlib/output/image.py` & `pytmlib-1.1.0.dev6/pytmlib/output/image.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev5/pytmlib/output/option.py` & `pytmlib-1.1.0.dev6/pytmlib/output/option.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev5/pytmlib/output/option_group.py` & `pytmlib-1.1.0.dev6/pytmlib/output/option_group.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev5/pytmlib/output/paragraph.py` & `pytmlib-1.1.0.dev6/pytmlib/output/paragraph.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev5/pytmlib/output/table.py` & `pytmlib-1.1.0.dev6/pytmlib/output/table.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev5/pytmlib/output/table_cell.py` & `pytmlib-1.1.0.dev6/pytmlib/output/table_cell.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev5/LICENSE` & `pytmlib-1.1.0.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev5/pyproject.toml` & `pytmlib-1.1.0.dev6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pytmlib"
-version = "1.1.0.dev5"
+version = "1.1.0.dev6"
 authors = [
     { name = "Oliver Fabel", email = "oliver.fabel@fhnw.ch" },
 ]
 description = "This is the base library for the Python Tool Manager."
 readme = "README.md"
 license = "MIT"
 requires-python = ">=3.8"
```

### Comparing `pytmlib-1.1.0.dev5/PKG-INFO` & `pytmlib-1.1.0.dev6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytmlib
-Version: 1.1.0.dev5
+Version: 1.1.0.dev6
 Summary: This is the base library for the Python Tool Manager.
 Project-URL: Homepage, https://github.com/ofabel/pytm-bootstrap
 Project-URL: Bug Tracker, https://github.com/ofabel/pytm-bootstrap/issues
 Project-URL: Changelog, https://github.com/ofabel/pytm-bootstrap/blob/main/CHANGELOG.md
 Author-email: Oliver Fabel <oliver.fabel@fhnw.ch>
 License-Expression: MIT
 License-File: LICENSE
```

