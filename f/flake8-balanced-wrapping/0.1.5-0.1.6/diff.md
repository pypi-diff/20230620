# Comparing `tmp/flake8-balanced-wrapping-0.1.5.tar.gz` & `tmp/flake8-balanced-wrapping-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8-balanced-wrapping-0.1.5.tar", last modified: Tue Jun 20 07:16:25 2023, max compression
+gzip compressed data, was "flake8-balanced-wrapping-0.1.6.tar", last modified: Tue Jun 20 07:36:52 2023, max compression
```

## Comparing `flake8-balanced-wrapping-0.1.5.tar` & `flake8-balanced-wrapping-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 07:16:25.813116 flake8-balanced-wrapping-0.1.5/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11339 2023-06-20 07:16:14.000000 flake8-balanced-wrapping-0.1.5/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2256 2023-06-20 07:16:25.813116 flake8-balanced-wrapping-0.1.5/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1242 2023-06-20 07:16:14.000000 flake8-balanced-wrapping-0.1.5/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 07:16:25.813116 flake8-balanced-wrapping-0.1.5/flake8_balanced_wrapping.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2256 2023-06-20 07:16:25.000000 flake8-balanced-wrapping-0.1.5/flake8_balanced_wrapping.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      354 2023-06-20 07:16:25.000000 flake8-balanced-wrapping-0.1.5/flake8_balanced_wrapping.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-20 07:16:25.000000 flake8-balanced-wrapping-0.1.5/flake8_balanced_wrapping.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       79 2023-06-20 07:16:25.000000 flake8-balanced-wrapping-0.1.5/flake8_balanced_wrapping.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-06-20 07:16:25.000000 flake8-balanced-wrapping-0.1.5/flake8_balanced_wrapping.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-06-20 07:16:25.000000 flake8-balanced-wrapping-0.1.5/flake8_balanced_wrapping.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16439 2023-06-20 07:16:14.000000 flake8-balanced-wrapping-0.1.5/flake8_balanced_wrapping.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1031 2023-06-20 07:16:25.813116 flake8-balanced-wrapping-0.1.5/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1631 2023-06-20 07:16:14.000000 flake8-balanced-wrapping-0.1.5/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 07:36:52.631658 flake8-balanced-wrapping-0.1.6/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11339 2023-06-20 07:36:42.000000 flake8-balanced-wrapping-0.1.6/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2256 2023-06-20 07:36:52.631658 flake8-balanced-wrapping-0.1.6/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1242 2023-06-20 07:36:42.000000 flake8-balanced-wrapping-0.1.6/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 07:36:52.631658 flake8-balanced-wrapping-0.1.6/flake8_balanced_wrapping.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2256 2023-06-20 07:36:52.000000 flake8-balanced-wrapping-0.1.6/flake8_balanced_wrapping.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      354 2023-06-20 07:36:52.000000 flake8-balanced-wrapping-0.1.6/flake8_balanced_wrapping.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-20 07:36:52.000000 flake8-balanced-wrapping-0.1.6/flake8_balanced_wrapping.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       79 2023-06-20 07:36:52.000000 flake8-balanced-wrapping-0.1.6/flake8_balanced_wrapping.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-06-20 07:36:52.000000 flake8-balanced-wrapping-0.1.6/flake8_balanced_wrapping.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-06-20 07:36:52.000000 flake8-balanced-wrapping-0.1.6/flake8_balanced_wrapping.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16976 2023-06-20 07:36:42.000000 flake8-balanced-wrapping-0.1.6/flake8_balanced_wrapping.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1031 2023-06-20 07:36:52.631658 flake8-balanced-wrapping-0.1.6/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1631 2023-06-20 07:36:42.000000 flake8-balanced-wrapping-0.1.6/setup.py
```

### Comparing `flake8-balanced-wrapping-0.1.5/LICENSE` & `flake8-balanced-wrapping-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8-balanced-wrapping-0.1.5/PKG-INFO` & `flake8-balanced-wrapping-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-balanced-wrapping
-Version: 0.1.5
+Version: 0.1.6
 Summary: A flake8 plugin that helps you wrap code with visual balance.
 Home-page: https://github.com/PeterJCLaw/flake8-balanced-wrapping
 Author: Peter Law
 Author-email: PeterJCLaw@gmail.com
 License: Apache 2.0
 Project-URL: Issue tracker, https://github.com/PeterJCLaw/flake8-balanced-wrapping/issues
 Platform: UNKNOWN
```

### Comparing `flake8-balanced-wrapping-0.1.5/README.md` & `flake8-balanced-wrapping-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `flake8-balanced-wrapping-0.1.5/flake8_balanced_wrapping.egg-info/PKG-INFO` & `flake8-balanced-wrapping-0.1.6/flake8_balanced_wrapping.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-balanced-wrapping
-Version: 0.1.5
+Version: 0.1.6
 Summary: A flake8 plugin that helps you wrap code with visual balance.
 Home-page: https://github.com/PeterJCLaw/flake8-balanced-wrapping
 Author: Peter Law
 Author-email: PeterJCLaw@gmail.com
 License: Apache 2.0
 Project-URL: Issue tracker, https://github.com/PeterJCLaw/flake8-balanced-wrapping/issues
 Platform: UNKNOWN
```

### Comparing `flake8-balanced-wrapping-0.1.5/flake8_balanced_wrapping.py` & `flake8-balanced-wrapping-0.1.6/flake8_balanced_wrapping.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import collections
 import dataclasses
 from typing import cast, Iterable, Iterator, Collection, NamedTuple
 from typing_extensions import Protocol
 
 from tuck.ast import Position, _last_token, _first_token
 from asttokens import ASTTokens
-from tuck.wrappers import expression_is_parenthesised
+from tuck.wrappers import get_node_bounds, expression_is_parenthesised
 
 
 class Error(Protocol):
     @property
     def position(self) -> Position:
         ...
 
@@ -80,14 +80,19 @@
 
     @property
     def is_single_line_or_column(self) -> bool:
         return self.is_single_line or self.is_single_column
 
 
 def get_start_position(asttokens: ASTTokens, node: ast.AST) -> Position:
+    if isinstance(node, ast.GeneratorExp):
+        first_token, last_token = get_node_bounds(asttokens, node)
+        if first_token.string == '(' and last_token.string == ')':
+            return Position(*first_token.start)
+
     if (
         isinstance(node, (ast.BoolOp, ast.IfExp)) and
         expression_is_parenthesised(asttokens, node)
     ):
         open_paren = asttokens.prev_token(_first_token(node))
         return Position(*open_paren.start)
 
@@ -99,22 +104,27 @@
     for node in nodes:
         start = get_start_position(asttokens, node)
         if start is not None:
             positions.append(start)
     return positions
 
 
-def get_end_position(node: ast.AST) -> Position:
+def get_end_position(asttokens: ASTTokens, node: ast.AST) -> Position:
+    if isinstance(node, ast.GeneratorExp):
+        first_token, last_token = get_node_bounds(asttokens, node)
+        if first_token.string == '(' and last_token.string == ')':
+            return Position(*last_token.end)
+
     return Position(*_last_token(node).end)
 
 
-def get_end_positions(nodes: Iterable[ast.AST]) -> list[Position]:
+def get_end_positions(asttokens: ASTTokens, nodes: Iterable[ast.AST]) -> list[Position]:
     positions = []
     for node in nodes:
-        end = get_end_position(node)
+        end = get_end_position(asttokens, node)
         if end is not None:
             positions.append(end)
     return positions
 
 
 class Visitor(ast.NodeVisitor):
     def __init__(self, asttokens: ASTTokens) -> None:
@@ -138,15 +148,15 @@
         for x in nodes:
             pos = get_start_position(self.asttokens, x)
             by_line_no[pos.line].append(x)
 
         if include_node_end:
             end_line, end_col = _last_token(node).end
             just_before_end_pos = Position(end_line, end_col - 1)
-            end_positions = get_end_positions(nodes)
+            end_positions = get_end_positions(self.asttokens, nodes)
 
             # Allow hugging, but otherwise add the containing node via its end
             # line too.
             if just_before_end_pos not in end_positions or end_line in by_line_no:
                 by_line_no[end_line].append(node)
 
         return by_line_no
```

### Comparing `flake8-balanced-wrapping-0.1.5/setup.cfg` & `flake8-balanced-wrapping-0.1.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `flake8-balanced-wrapping-0.1.5/setup.py` & `flake8-balanced-wrapping-0.1.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 
 long_description = (Path(__file__).parent / 'README.md').read_text()
 
 setup(
     name='flake8-balanced-wrapping',
-    version='0.1.5',
+    version='0.1.6',
     url='https://github.com/PeterJCLaw/flake8-balanced-wrapping',
     project_urls={
         'Issue tracker': 'https://github.com/PeterJCLaw/flake8-balanced-wrapping/issues',
     },
     description="A flake8 plugin that helps you wrap code with visual balance.",
     long_description=long_description,
     long_description_content_type='text/markdown',
```

