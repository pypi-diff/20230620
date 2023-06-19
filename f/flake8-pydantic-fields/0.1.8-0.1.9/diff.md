# Comparing `tmp/flake8-pydantic-fields-0.1.8.tar.gz` & `tmp/flake8-pydantic-fields-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8-pydantic-fields-0.1.8.tar", last modified: Thu Feb  2 00:02:05 2023, max compression
+gzip compressed data, was "flake8-pydantic-fields-0.1.9.tar", last modified: Thu Feb  2 00:34:57 2023, max compression
```

## Comparing `flake8-pydantic-fields-0.1.8.tar` & `flake8-pydantic-fields-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 00:02:05.576722 flake8-pydantic-fields-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-02-02 00:02:04.000000 flake8-pydantic-fields-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-02 00:02:04.000000 flake8-pydantic-fields-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-02-02 00:02:05.576722 flake8-pydantic-fields-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-02-02 00:02:04.000000 flake8-pydantic-fields-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 00:02:05.576722 flake8-pydantic-fields-0.1.8/flake8_pydantic_fields.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-02-02 00:02:05.000000 flake8-pydantic-fields-0.1.8/flake8_pydantic_fields.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-02-02 00:02:05.000000 flake8-pydantic-fields-0.1.8/flake8_pydantic_fields.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-02 00:02:05.000000 flake8-pydantic-fields-0.1.8/flake8_pydantic_fields.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-02 00:02:05.000000 flake8-pydantic-fields-0.1.8/flake8_pydantic_fields.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-02 00:02:05.000000 flake8-pydantic-fields-0.1.8/flake8_pydantic_fields.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-02 00:02:05.000000 flake8-pydantic-fields-0.1.8/flake8_pydantic_fields.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8622 2023-02-02 00:02:04.000000 flake8-pydantic-fields-0.1.8/flake8_pydantic_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-02 00:02:04.000000 flake8-pydantic-fields-0.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-02 00:02:05.576722 flake8-pydantic-fields-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-02-02 00:02:04.000000 flake8-pydantic-fields-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 00:34:57.132821 flake8-pydantic-fields-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-02-02 00:34:56.000000 flake8-pydantic-fields-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-02 00:34:56.000000 flake8-pydantic-fields-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-02-02 00:34:57.132821 flake8-pydantic-fields-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-02-02 00:34:56.000000 flake8-pydantic-fields-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 00:34:57.132821 flake8-pydantic-fields-0.1.9/flake8_pydantic_fields.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-02-02 00:34:57.000000 flake8-pydantic-fields-0.1.9/flake8_pydantic_fields.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-02-02 00:34:57.000000 flake8-pydantic-fields-0.1.9/flake8_pydantic_fields.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-02 00:34:57.000000 flake8-pydantic-fields-0.1.9/flake8_pydantic_fields.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-02 00:34:57.000000 flake8-pydantic-fields-0.1.9/flake8_pydantic_fields.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-02 00:34:57.000000 flake8-pydantic-fields-0.1.9/flake8_pydantic_fields.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-02 00:34:57.000000 flake8-pydantic-fields-0.1.9/flake8_pydantic_fields.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8962 2023-02-02 00:34:56.000000 flake8-pydantic-fields-0.1.9/flake8_pydantic_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-02 00:34:56.000000 flake8-pydantic-fields-0.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-02 00:34:57.132821 flake8-pydantic-fields-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-02-02 00:34:56.000000 flake8-pydantic-fields-0.1.9/setup.py
```

### Comparing `flake8-pydantic-fields-0.1.8/LICENSE` & `flake8-pydantic-fields-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8-pydantic-fields-0.1.8/PKG-INFO` & `flake8-pydantic-fields-0.1.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-pydantic-fields
-Version: 0.1.8
+Version: 0.1.9
 Requires-Python: >=3.10,<3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # flake8-pydantic-fields
 
 A flake8 plugin that checks that Pydantic models have default values which are Fields, and that those fields have descriptions. This encourages data documentation.
```

### Comparing `flake8-pydantic-fields-0.1.8/README.md` & `flake8-pydantic-fields-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `flake8-pydantic-fields-0.1.8/flake8_pydantic_fields.egg-info/PKG-INFO` & `flake8-pydantic-fields-0.1.9/flake8_pydantic_fields.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-pydantic-fields
-Version: 0.1.8
+Version: 0.1.9
 Requires-Python: >=3.10,<3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # flake8-pydantic-fields
 
 A flake8 plugin that checks that Pydantic models have default values which are Fields, and that those fields have descriptions. This encourages data documentation.
```

### Comparing `flake8-pydantic-fields-0.1.8/flake8_pydantic_fields.py` & `flake8-pydantic-fields-0.1.9/flake8_pydantic_fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import ast
 from typing import Any, Iterable
 
-VERSION = "0.1.8"
+VERSION = "0.1.9"
 PYDANTIC_MODEL_BASES = ["BaseModel", "GenericModel"]
 VALIDATOR_DECORATOR_NAMES = ["validator", "root_validator"]
 ERRORS = {
     "PF001": "PF001 Found a Pydantic field which has no default",
     "PF002": "PF002 Found a Pydantic field which has a default that is not a Field",
     "PF003": "PF003 Found a Pydantic field which has a Field default with no description",
     "PF004": "PF004 Found a Pydantic field which has a Field default with an empty description",
@@ -121,14 +121,22 @@
             and attribute.name == "__init__"
         ):
             return True
 
     return False
 
 
+def is_typeddict(*, classdef: ast.ClassDef) -> bool:
+    """If a class has a TypedDict base class, it is not a data model."""
+    return any(
+        isinstance(base, ast.Name) and base.id == "TypedDict"
+        for base in classdef.bases
+    )
+
+
 class PydanticFieldChecker(ast.NodeVisitor):
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
         self.current_class_is_candidate = False
         self.errors: list[tuple[int, int, str]] = []
 
     def visit_ClassDef(self, node: ast.ClassDef) -> None:
@@ -138,15 +146,19 @@
                 base_class_indicates_pydantic(classdef=node)
                 or class_contains_only_annassign(classdef=node)
                 or has_validator_method(classdef=node)
                 or has_inner_config_class(classdef=node)
                 or has_classvar_attribute(classdef=node)
                 or no_methods_have_arguments(classdef=node)
             )
-            and not (has_init(classdef=node) or has_dataclass_decorator(classdef=node))
+            and not (
+                has_init(classdef=node)
+                or has_dataclass_decorator(classdef=node)
+                or is_typeddict(classdef=node)
+            )
         )
         self.generic_visit(node)
         self.current_class_is_candidate = False
 
     def visit_FunctionDef(self, node: ast.FunctionDef) -> None:
         self.current_class_is_candidate = False
```

### Comparing `flake8-pydantic-fields-0.1.8/setup.py` & `flake8-pydantic-fields-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     install_requires = f.read().splitlines()
 
 with open("README.md") as f:
     long_description = f.read().strip()
 
 setup(
     name="flake8-pydantic-fields",
-    version="0.1.8",
+    version="0.1.9",
     python_requires=">=3.10,<3.11",
     install_requires=install_requires,
     py_modules=["flake8_pydantic_fields"],
     entry_points={"flake8.extension": "PF00 = flake8_pydantic_fields:Plugin"},
     long_description=long_description,
     long_description_content_type="text/markdown",
 )
```

