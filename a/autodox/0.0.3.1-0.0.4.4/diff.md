# Comparing `tmp/autodox-0.0.3.1.tar.gz` & `tmp/autodox-0.0.4.4.tar.gz`

## Comparing `autodox-0.0.3.1.tar` & `autodox-0.0.4.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 autodox-0.0.3.1/autodox/__init__.py
--rw-r--r--   0        0        0    16545 2020-02-02 00:00:00.000000 autodox-0.0.3.1/autodox/functions.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 autodox-0.0.3.1/tests/context.py
--rw-r--r--   0        0        0     5851 2020-02-02 00:00:00.000000 autodox-0.0.3.1/tests/test_hooks.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 autodox-0.0.3.1/.gitignore
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 autodox-0.0.3.1/license
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 autodox-0.0.3.1/pyproject.toml
--rw-r--r--   0        0        0     7100 2020-02-02 00:00:00.000000 autodox-0.0.3.1/readme.md
--rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 autodox-0.0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 autodox-0.0.4.4/autodox/__init__.py
+-rw-r--r--   0        0        0    18443 2020-02-02 00:00:00.000000 autodox-0.0.4.4/autodox/functions.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 autodox-0.0.4.4/tests/context.py
+-rw-r--r--   0        0        0     5851 2020-02-02 00:00:00.000000 autodox-0.0.4.4/tests/test_hooks.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 autodox-0.0.4.4/.gitignore
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 autodox-0.0.4.4/license
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 autodox-0.0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     7100 2020-02-02 00:00:00.000000 autodox-0.0.4.4/readme.md
+-rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 autodox-0.0.4.4/PKG-INFO
```

### Comparing `autodox-0.0.3.1/autodox/functions.py` & `autodox-0.0.4.4/autodox/functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from enum import Enum, auto
-from types import ModuleType
+from types import ModuleType, MethodType, FunctionType
 from typing import Any, Callable
 
 
 
 class Event(Enum):
     AFTER_HEADER = auto()
     AFTER_PARAGRAPH = auto()
@@ -222,39 +222,44 @@
 def dox_a_function(function: Callable, options: dict = {}) -> str:
     """Collects some information about a function and returns it
         formatted as specified in the options or as a list.
     """
     function, options = _invoke_handler(Event.BEFORE_FUNCTION, function, options)
     header_level = options['header_level'] if 'header_level' in options else 0
     format = options['format'] if 'format' in options else 'list'
+    prepend = options['prepend'] if 'prepend' in options else ''
 
     name = function.__name__ if hasattr(function, '__name__') else '{unknown/unnamed}'
     annotations = function.__annotations__ if hasattr(function, '__annotations__') else {}
     return_annotation = annotations['return'] if 'return' in annotations else None
     annotations = [
         f'{key}: {value.__name__ if hasattr(value, "__name__") else str(value)}'
         for key, value in annotations.items()
         if key != 'return'
     ]
-    defaults = [*function.__defaults__] if function.__defaults__ else []
+
+    if hasattr(function, '__defaults__') and function.__defaults__:
+        defaults = [*function.__defaults__]
+    else:
+        defaults = []
     offset = len(annotations) - len(defaults)
     if offset < 0:
         offset = 0
 
     if annotations and defaults:
         for i in range(len(defaults)):
             if defaults[i] == '':
                 annotations[i+offset] += f" = ''"
             else:
                 annotations[i+offset] += f' = {defaults[i]}'
 
     annotations = ', '.join(annotations) or ''
     docstring = function.__doc__ if hasattr(function, '__doc__') else None
 
-    signature = f'`{name}({annotations})'
+    signature = f'`{prepend}{name}({annotations})'
     if return_annotation:
         if hasattr(return_annotation, '__name__'):
             return_annotation = return_annotation.__name__
         signature += f' -> {return_annotation}'
     signature += ':` '
 
     doc = ''
@@ -316,15 +321,15 @@
                 doc += _list(f'{name} - {value.__doc__}')
             else:
                 doc += _list(name)
 
     return doc
 
 
-def _dox_methods(methods: dict, options: dict = {}) -> str:
+def _dox_methods(cls: type, methods: dict, options: dict = {}) -> str:
     """Format a collection of methods/functions."""
     header_level = options['header_level'] if 'header_level' in options else 0
     header_level += 1
     suboptions = {**options, 'header_level': header_level}
     format = options['method_format'] if 'method_format' in options else 'header'
     doc = ''
 
@@ -341,28 +346,43 @@
     publics = {
         name: value
         for name, value in methods.items()
         if name not in dunders and name not in privates
     }
 
     if publics:
-        for _, value in publics.items():
-            doc += dox_a_function(value, {**suboptions, 'format': format})
+        for name, value in publics.items():
+            if isinstance(value, classmethod):
+                doc += dox_a_function(value, {**suboptions, 'format': format, 'prepend': '@classmethod '})
+            elif isinstance(cls.__dict__[name], staticmethod):
+                doc += dox_a_function(value, {**suboptions, 'format': format, 'prepend': '@staticmethod '})
+            else:
+                doc += dox_a_function(value, {**suboptions, 'format': format})
 
     if privates:
         for _, value in privates.items():
             doc += dox_a_function(value, {**suboptions, 'format': format})
 
     if dunders:
         for _, value in dunders.items():
             doc += dox_a_function(value, {**suboptions, 'format': format})
 
     return doc
 
 
+def _get_all_annocations(cls: type) -> dict:
+    """Collects all annotations from a class hierarchy."""
+    annotations = cls.__annotations__ if hasattr(cls, '__annotations__') else {}
+    parent = cls.__base__ if hasattr(cls, '__base__') else None
+    if parent:
+        if hasattr(parent, '__annotations__'):
+            annotations = {**_get_all_annocations(parent.__annotations__), **annotations}
+    return annotations
+
+
 def dox_a_class(cls: type, options: dict = {}) -> str:
     """Collects some information about a class and returns a formatted
         str. Any names specified in options['exclude_names'] and any
         types specified in options['exclude_types'] will be excluded.
         Private and dunder methods/properties will be included if
         options['include_private'] or options['include_dunder'] are
         specified, respectively.
@@ -374,30 +394,28 @@
     include_dunder = 'include_dunder' in options
     suboptions = {**options, 'header_level': header_level + 1}
 
     parent = cls.__base__ if hasattr(cls, '__base__') else None
 
     properties = {}
     methods = {}
-    annotations = cls.__annotations__ if hasattr(cls, '__annotations__') else {}
+    annotations = _get_all_annocations(cls)
 
     if parent:
-        if hasattr(parent, '__annotations__'):
-            annotations = {**parent.__annotations__, **annotations}
         parent = parent.__name__ if hasattr(parent, '__name__') else str(parent)
 
     for name, item in cls.__dict__.items():
         if name[:1] == '_' and not (include_private or include_dunder):
             continue
         if name[:2] == '__' and not include_dunder:
             continue
         if name in exclude_names:
             continue
 
-        if type(item) is type(dox_a_function):
+        if type(item) in (MethodType, FunctionType, staticmethod, classmethod):
             methods[name] = item
 
         if type(item) is property:
             properties[name] = item
 
     name = cls.__name__ if hasattr(cls, '__name__') else '{unknown/unnamed class}'
     if name in exclude_names:
@@ -412,27 +430,46 @@
 
     if properties:
         doc += _header('Properties', header_level + 1)
         doc += _dox_properties(properties, header_level)
 
     if methods:
         doc += _header('Methods', header_level + 1)
-        doc += _dox_methods(methods, suboptions)
+        doc += _dox_methods(cls, methods, suboptions)
 
     return _invoke_handler(Event.AFTER_CLASS, doc)
 
 
+def _cli_help(name: str) -> int:
+    print(f'Usage: {name} [package[.module]] [options] ')
+    print('\t-exclude_name=str: exclude the given name (or csv of names)')
+    print('\t-exclude_type=str: exclude the given type (or csv of types)')
+    print('\t-header_level=int: number of hashtags to prepend to headers')
+    print('\t-package=str: name of package if not using the . notation')
+    print('\t-function_format=str: choose one of "header", "paragraph", or "list"')
+    print('\t-method_format=type: choose one of "header", "paragraph", or "list"')
+    print('\t-value_format=type: choose one of "header", "paragraph", or "list"')
+    print('\t-include_private: includes things prefaced with "_"')
+    print('\t-include_dunder: includes things prefaced with "__"')
+    print('\t-include_submodules: includes submodules')
+    print('\t-document_submodules: runs module documentation for submodules')
+    return 0
+
+
 def main_cli() -> int:
     """Entry point for pip installed wrapper function to invoke via CLI."""
     from importlib import import_module
     from sys import argv
     _settings = {}
     _module = ''
 
     for arg in argv[1:]:
+        if arg in ('--help', '-help', '-?', '-h', '?'):
+            return _cli_help(argv[0])
+
         if arg[:14] == '-exclude_name=':
             if 'exclude_names' not in _settings:
                 _settings['exclude_names'] = []
             _settings['exclude_names'].extend(arg[14:].split(','))
         elif arg[:14] == '-exclude_type=':
             if 'exclude_types' not in _settings:
                 _settings['exclude_types'] = []
```

### Comparing `autodox-0.0.3.1/tests/test_hooks.py` & `autodox-0.0.4.4/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `autodox-0.0.3.1/license` & `autodox-0.0.4.4/license`

 * *Files identical despite different names*

### Comparing `autodox-0.0.3.1/pyproject.toml` & `autodox-0.0.4.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "autodox"
-version = "0.0.3.1"
+version = "0.0.4.4"
 authors = [
   { name="k98kurz", email="k98kurz@gmail.com" },
 ]
 description = "Tool for generating documentation automatically from code annotations, types, and docstrings."
 readme = "readme.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `autodox-0.0.3.1/readme.md` & `autodox-0.0.4.4/readme.md`

 * *Files identical despite different names*

### Comparing `autodox-0.0.3.1/PKG-INFO` & `autodox-0.0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autodox
-Version: 0.0.3.1
+Version: 0.0.4.4
 Summary: Tool for generating documentation automatically from code annotations, types, and docstrings.
 Project-URL: Homepage, https://github.com/k98kurz/autodox
 Project-URL: Bug Tracker, https://github.com/k98kurz/autodox/issues
 Author-email: k98kurz <k98kurz@gmail.com>
 License-File: license
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: ISC License (ISCL)
```

