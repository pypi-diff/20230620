# Comparing `tmp/pytmlib-1.1.0.dev7.tar.gz` & `tmp/pytmlib-1.1.0.dev8.tar.gz`

## Comparing `pytmlib-1.1.0.dev7.tar` & `pytmlib-1.1.0.dev8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev7/pytmlib/__init__.py
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev7/pytmlib/abstract_exercise.py
--rw-r--r--   0        0        0     6270 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev7/pytmlib/api.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev7/pytmlib/archiver.py
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev7/pytmlib/context.py
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev7/pytmlib/create_app.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev7/pytmlib/decorators.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev7/pytmlib/exceptions.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev7/pytmlib/handle_error.py
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev7/pytmlib/latex.py
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev7/pytmlib/serializer.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev7/pytmlib/types.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev7/pytmlib/output/__init__.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev7/pytmlib/output/abstract.py
--rw-r--r--   0        0        0     8898 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev7/pytmlib/output/builder.py
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev7/pytmlib/output/button.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev7/pytmlib/output/field.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev7/pytmlib/output/field_attribute.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev7/pytmlib/output/field_type_enum.py
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev7/pytmlib/output/figure.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev7/pytmlib/output/image.py
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev7/pytmlib/output/option.py
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev7/pytmlib/output/option_group.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev7/pytmlib/output/paragraph.py
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev7/pytmlib/output/table.py
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev7/pytmlib/output/table_cell.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev7/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev7/LICENSE
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev7/README.md
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev7/pyproject.toml
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev7/PKG-INFO
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/pytmlib/__init__.py
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/pytmlib/abstract_exercise.py
+-rw-r--r--   0        0        0     6450 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/pytmlib/api.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/pytmlib/archiver.py
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/pytmlib/context.py
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/pytmlib/create_app.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/pytmlib/decorators.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/pytmlib/exceptions.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/pytmlib/handle_error.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/pytmlib/latex.py
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/pytmlib/serializer.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/pytmlib/types.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/pytmlib/output/__init__.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/pytmlib/output/abstract.py
+-rw-r--r--   0        0        0     8898 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/pytmlib/output/builder.py
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/pytmlib/output/button.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/pytmlib/output/field.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/pytmlib/output/field_attribute.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/pytmlib/output/field_type_enum.py
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/pytmlib/output/figure.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/pytmlib/output/image.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/pytmlib/output/option.py
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/pytmlib/output/option_group.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/pytmlib/output/paragraph.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/pytmlib/output/table.py
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/pytmlib/output/table_cell.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/LICENSE
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/README.md
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/pyproject.toml
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev8/PKG-INFO
```

### Comparing `pytmlib-1.1.0.dev7/pytmlib/abstract_exercise.py` & `pytmlib-1.1.0.dev8/pytmlib/abstract_exercise.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import abc
 import logging
 import os
 import uuid
-from typing import List
+from typing import Iterable
 from typing import Tuple
 
 from .context import Context
 from .create_app import create_app
 from .decorators import ENTRYPOINT_MARKER
 from .output import OutputBuilder as Output
-from .types import Entrypoint
+from .types import Action
 
 
 class AbstractExercise(abc.ABC):
     def __new__(cls, unique_id: str, static_folder_path: str = None, *args, **kwargs):
         exercise: AbstractExercise = super().__new__(cls, *args, **kwargs)
 
         secret, fallback = AbstractExercise._get_secret()
@@ -30,23 +30,20 @@
     def output(self) -> Output:
         return self._context.output
 
     @abc.abstractmethod
     def start(self) -> Output:
         pass
 
-    def get_entrypoints(self) -> List[Entrypoint]:
-        entrypoints = []
+    def get_entrypoints(self) -> Iterable[Action]:
         for name in dir(self):
             func = getattr(self, name)
 
             if hasattr(func, ENTRYPOINT_MARKER):
-                entrypoints.append(func)
-
-        return entrypoints
+                yield func
 
     @staticmethod
     def _get_secret() -> Tuple[str, bool]:
         hostname: str = os.getenv('HOSTNAME', os.name)
         fallback: uuid = uuid.uuid5(uuid.NAMESPACE_DNS, hostname)
         secret: str = os.getenv('PYTM_SECRET')
         use_fallback: bool = secret is None
```

### Comparing `pytmlib-1.1.0.dev7/pytmlib/api.py` & `pytmlib-1.1.0.dev8/pytmlib/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,18 +10,19 @@
 from flask import Response
 from flask import jsonify
 from flask import request
 from flask_cors import CORS
 
 from .archiver import Archiver
 from .context import Context
+from .decorators import ENTRYPOINT_TITLE
 from .exceptions import EntrypointNotFound
 from .exceptions import MethodCallException
 from .output.button import ButtonOutput
-from .types import Entrypoint
+from .types import Action
 
 if TYPE_CHECKING:
     from .output import OutputBuilder
 
 
 class API:
     def __init__(self, context: Context):
@@ -40,15 +41,15 @@
         result: 'OutputBuilder' = self._call_method(self.context.exercise.start)
         json: dict = result.to_json()
         envelop = self._wrap_with_envelop(json)
 
         return jsonify(envelop)
 
     def handle_entrypoint(self, entrypoint: str) -> Response:
-        method: Entrypoint = self._get_entrypoint_by_name(entrypoint)
+        method: Action = self._get_entrypoint_by_name(entrypoint)
         result: 'OutputBuilder' = self._call_method(method)
         json: dict = result.to_json()
         envelop = self._wrap_with_envelop(json)
 
         return jsonify(envelop)
 
     def handle_entrypoints(self) -> Response:
@@ -60,15 +61,15 @@
         json: list = [self._map_entrypoint_to_json(entrypoint) for entrypoint in entrypoints]
 
         envelop = self._wrap_with_envelop(json)
 
         return jsonify(envelop)
 
     def handle_action(self, action: str) -> Response:
-        method: Entrypoint = getattr(self.context.exercise, action, None)
+        method: Action = getattr(self.context.exercise, action, None)
         envelop_in: dict = request.json
         result: 'OutputBuilder' = self._call_action(method, envelop_in)
         json: dict = result.to_json()
         envelop_out: dict = self._wrap_with_envelop(json)
 
         return jsonify(envelop_out)
 
@@ -97,15 +98,15 @@
 
     def _wrap_with_envelop(self, payload: Union[list, dict, str, int, float]) -> dict:
         return {
             'exercise_id': self.context.unique_id,
             'payload': payload
         }
 
-    def _call_action(self, method: Entrypoint, envelop: dict) -> 'OutputBuilder':
+    def _call_action(self, method: Action, envelop: dict) -> 'OutputBuilder':
         method_signature: Signature = signature(method)
         available_arguments: dict = envelop.pop('payload')
         additional_parameters: dict = self._get_additional_parameters(envelop)
         applicable_arguments: dict = {**additional_parameters, **available_arguments}
         arguments: dict = {}
 
         for key in method_signature.parameters.keys():
@@ -139,27 +140,28 @@
         # apply standard arguments
         if parameter.kind == Parameter.POSITIONAL_OR_KEYWORD:
             arguments[name] = applicable_arguments.pop(name)
         # apply kwargs
         elif parameter.kind == Parameter.VAR_KEYWORD:
             arguments.update(**applicable_arguments)
 
-    def _get_entrypoint_by_name(self, name: str) -> Entrypoint:
+    def _get_entrypoint_by_name(self, name: str) -> Action:
         for entrypoint in self.context.exercise.get_entrypoints():
             if entrypoint.__name__ == name:
                 return entrypoint
         raise EntrypointNotFound
 
     @staticmethod
-    def _call_method(method: Entrypoint, **kwargs) -> 'OutputBuilder':
+    def _call_method(method: Action, **kwargs) -> 'OutputBuilder':
         try:
             return method(**kwargs)
         except BaseException as reason:
             raise MethodCallException() from reason
 
     @staticmethod
-    def _map_entrypoint_to_json(entrypoint: Entrypoint) -> dict:
+    def _map_entrypoint_to_json(entrypoint: Action) -> dict:
         name: str = entrypoint.__name__
-        title: Optional[str] = entrypoint.__doc__
-        title = title if title is None else title.strip()
+        title: str = getattr(entrypoint, ENTRYPOINT_TITLE, name[0].upper() + name[1:])
+        description: Optional[str] = entrypoint.__doc__
+        description = description if description is None else description.strip().splitlines(False).pop(0)
 
-        return dict(name=name, title=title)
+        return dict(name=name, title=title, description=description)
```

### Comparing `pytmlib-1.1.0.dev7/pytmlib/archiver.py` & `pytmlib-1.1.0.dev8/pytmlib/archiver.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev7/pytmlib/context.py` & `pytmlib-1.1.0.dev8/pytmlib/context.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev7/pytmlib/create_app.py` & `pytmlib-1.1.0.dev8/pytmlib/create_app.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev7/pytmlib/handle_error.py` & `pytmlib-1.1.0.dev8/pytmlib/handle_error.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev7/pytmlib/serializer.py` & `pytmlib-1.1.0.dev8/pytmlib/serializer.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev7/pytmlib/output/abstract.py` & `pytmlib-1.1.0.dev8/pytmlib/output/abstract.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev7/pytmlib/output/builder.py` & `pytmlib-1.1.0.dev8/pytmlib/output/builder.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev7/pytmlib/output/button.py` & `pytmlib-1.1.0.dev8/pytmlib/output/button.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev7/pytmlib/output/field.py` & `pytmlib-1.1.0.dev8/pytmlib/output/field.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev7/pytmlib/output/figure.py` & `pytmlib-1.1.0.dev8/pytmlib/output/figure.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev7/pytmlib/output/image.py` & `pytmlib-1.1.0.dev8/pytmlib/output/image.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev7/pytmlib/output/option.py` & `pytmlib-1.1.0.dev8/pytmlib/output/option.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev7/pytmlib/output/option_group.py` & `pytmlib-1.1.0.dev8/pytmlib/output/option_group.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev7/pytmlib/output/paragraph.py` & `pytmlib-1.1.0.dev8/pytmlib/output/paragraph.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev7/pytmlib/output/table.py` & `pytmlib-1.1.0.dev8/pytmlib/output/table.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev7/pytmlib/output/table_cell.py` & `pytmlib-1.1.0.dev8/pytmlib/output/table_cell.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev7/LICENSE` & `pytmlib-1.1.0.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev7/pyproject.toml` & `pytmlib-1.1.0.dev8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pytmlib"
-version = "1.1.0.dev7"
+version = "1.1.0.dev8"
 authors = [
     { name = "Oliver Fabel", email = "oliver.fabel@fhnw.ch" },
 ]
 description = "This is the base library for the Python Tool Manager."
 readme = "README.md"
 license = "MIT"
 requires-python = ">=3.8"
```

### Comparing `pytmlib-1.1.0.dev7/PKG-INFO` & `pytmlib-1.1.0.dev8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytmlib
-Version: 1.1.0.dev7
+Version: 1.1.0.dev8
 Summary: This is the base library for the Python Tool Manager.
 Project-URL: Homepage, https://github.com/ofabel/pytm-bootstrap
 Project-URL: Bug Tracker, https://github.com/ofabel/pytm-bootstrap/issues
 Project-URL: Changelog, https://github.com/ofabel/pytm-bootstrap/blob/main/CHANGELOG.md
 Author-email: Oliver Fabel <oliver.fabel@fhnw.ch>
 License-Expression: MIT
 License-File: LICENSE
```

