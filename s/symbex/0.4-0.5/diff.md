# Comparing `tmp/symbex-0.4.tar.gz` & `tmp/symbex-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symbex-0.4.tar", last modified: Mon Jun 19 18:08:06 2023, max compression
+gzip compressed data, was "symbex-0.5.tar", last modified: Tue Jun 20 11:51:30 2023, max compression
```

## Comparing `symbex-0.4.tar` & `symbex-0.5.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:08:06.508515 symbex-0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-19 18:07:51.000000 symbex-0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-06-19 18:08:06.508515 symbex-0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-06-19 18:07:51.000000 symbex-0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 18:08:06.508515 symbex-0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-19 18:07:51.000000 symbex-0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:08:06.508515 symbex-0.4/symbex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 18:07:51.000000 symbex-0.4/symbex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-19 18:07:51.000000 symbex-0.4/symbex/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-19 18:07:51.000000 symbex-0.4/symbex/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-06-19 18:07:51.000000 symbex-0.4/symbex/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:08:06.508515 symbex-0.4/symbex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-06-19 18:08:06.000000 symbex-0.4/symbex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-19 18:08:06.000000 symbex-0.4/symbex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 18:08:06.000000 symbex-0.4/symbex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-19 18:08:06.000000 symbex-0.4/symbex.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-19 18:08:06.000000 symbex-0.4/symbex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-19 18:08:06.000000 symbex-0.4/symbex.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:08:06.508515 symbex-0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-06-19 18:07:51.000000 symbex-0.4/tests/test_symbex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-06-19 18:07:51.000000 symbex-0.4/tests/test_symbols.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:51:30.299520 symbex-0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-20 11:51:15.000000 symbex-0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-06-20 11:51:30.299520 symbex-0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9614 2023-06-20 11:51:15.000000 symbex-0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 11:51:30.299520 symbex-0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-20 11:51:15.000000 symbex-0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:51:30.299520 symbex-0.5/symbex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 11:51:15.000000 symbex-0.5/symbex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-20 11:51:15.000000 symbex-0.5/symbex/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-06-20 11:51:15.000000 symbex-0.5/symbex/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9408 2023-06-20 11:51:15.000000 symbex-0.5/symbex/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:51:30.299520 symbex-0.5/symbex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-06-20 11:51:30.000000 symbex-0.5/symbex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-20 11:51:30.000000 symbex-0.5/symbex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 11:51:30.000000 symbex-0.5/symbex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-20 11:51:30.000000 symbex-0.5/symbex.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-20 11:51:30.000000 symbex-0.5/symbex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 11:51:30.000000 symbex-0.5/symbex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:51:30.299520 symbex-0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-06-20 11:51:15.000000 symbex-0.5/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-06-20 11:51:15.000000 symbex-0.5/tests/test_symbex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-06-20 11:51:15.000000 symbex-0.5/tests/test_symbols.py
```

### Comparing `symbex-0.4/LICENSE` & `symbex-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `symbex-0.4/setup.py` & `symbex-0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "0.4"
+VERSION = "0.5"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
```

### Comparing `symbex-0.4/symbex/lib.py` & `symbex-0.5/symbex/lib.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import fnmatch
 import ast
 from ast import literal_eval, parse, AST, AsyncFunctionDef, FunctionDef, ClassDef
 import codecs
+from dataclasses import dataclass
 from itertools import zip_longest
 import re
 from typing import Iterable, List, Optional, Tuple
 
 
 def find_symbol_nodes(
     code: str, filename: str, symbols: Iterable[str]
@@ -226,7 +227,59 @@
             content = f.read()
     except LookupError:
         # If the detected encoding is not valid, try again with utf-8
         with codecs.open(path, "r", encoding=default_encoding) as f:
             content = f.read()
 
     return content
+
+
+@dataclass
+class TypeSummary:
+    fully: bool
+    partially: bool
+
+
+def type_summary(node: AST) -> Optional[TypeSummary]:
+    if not isinstance(node, (FunctionDef, AsyncFunctionDef)):
+        return None
+    all_args = [
+        *node.args.posonlyargs,
+        *node.args.args,
+        *node.args.kwonlyargs,
+    ]
+    num_arguments = len(all_args)
+    has_untyped_self = False
+    typed_args = []
+    first = True
+    for arg in all_args:
+        # Special case if the first argument is self - note that we do not
+        # check that we are a class method but ideally we would do that
+        if first and arg.arg == "self":
+            has_untyped_self = True
+            continue
+        if arg.annotation:
+            typed_args.append(arg)
+        first = False
+
+    return_is_typed = bool(node.returns)
+
+    partially = len(typed_args) > 0 or return_is_typed
+    fully = False
+    if len(typed_args) == num_arguments and return_is_typed:
+        fully = True
+    # Something is fully typed if either EVERY arg is typed
+    # or all arguments except for the untyped self are typed
+    if has_untyped_self and len(typed_args) == num_arguments - 1 and return_is_typed:
+        fully = True
+    # Another special case: __init__() doesn't need a return type
+    if node.name == "__init__":
+        if (has_untyped_self and len(typed_args) == num_arguments - 1) or len(
+            typed_args
+        ) == num_arguments:
+            # Doesn't matter if we have a return type
+            fully = True
+
+    return TypeSummary(
+        fully=fully,
+        partially=partially,
+    )
```

### Comparing `symbex-0.4/tests/test_symbex.py` & `symbex-0.5/tests/test_symbex.py`

 * *Files identical despite different names*

### Comparing `symbex-0.4/tests/test_symbols.py` & `symbex-0.5/tests/test_symbols.py`

 * *Files identical despite different names*

