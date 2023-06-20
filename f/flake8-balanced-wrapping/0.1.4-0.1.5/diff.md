# Comparing `tmp/flake8-balanced-wrapping-0.1.4.tar.gz` & `tmp/flake8-balanced-wrapping-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8-balanced-wrapping-0.1.4.tar", last modified: Sun Jun 18 18:55:17 2023, max compression
+gzip compressed data, was "flake8-balanced-wrapping-0.1.5.tar", last modified: Tue Jun 20 07:16:25 2023, max compression
```

## Comparing `flake8-balanced-wrapping-0.1.4.tar` & `flake8-balanced-wrapping-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-18 18:55:17.925705 flake8-balanced-wrapping-0.1.4/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11339 2023-06-18 18:55:06.000000 flake8-balanced-wrapping-0.1.4/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2256 2023-06-18 18:55:17.925705 flake8-balanced-wrapping-0.1.4/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1242 2023-06-18 18:55:06.000000 flake8-balanced-wrapping-0.1.4/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-18 18:55:17.925705 flake8-balanced-wrapping-0.1.4/flake8_balanced_wrapping.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2256 2023-06-18 18:55:17.000000 flake8-balanced-wrapping-0.1.4/flake8_balanced_wrapping.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      354 2023-06-18 18:55:17.000000 flake8-balanced-wrapping-0.1.4/flake8_balanced_wrapping.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-18 18:55:17.000000 flake8-balanced-wrapping-0.1.4/flake8_balanced_wrapping.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       79 2023-06-18 18:55:17.000000 flake8-balanced-wrapping-0.1.4/flake8_balanced_wrapping.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-06-18 18:55:17.000000 flake8-balanced-wrapping-0.1.4/flake8_balanced_wrapping.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-06-18 18:55:17.000000 flake8-balanced-wrapping-0.1.4/flake8_balanced_wrapping.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15837 2023-06-18 18:55:06.000000 flake8-balanced-wrapping-0.1.4/flake8_balanced_wrapping.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1006 2023-06-18 18:55:17.929705 flake8-balanced-wrapping-0.1.4/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1631 2023-06-18 18:55:06.000000 flake8-balanced-wrapping-0.1.4/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 07:16:25.813116 flake8-balanced-wrapping-0.1.5/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11339 2023-06-20 07:16:14.000000 flake8-balanced-wrapping-0.1.5/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2256 2023-06-20 07:16:25.813116 flake8-balanced-wrapping-0.1.5/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1242 2023-06-20 07:16:14.000000 flake8-balanced-wrapping-0.1.5/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 07:16:25.813116 flake8-balanced-wrapping-0.1.5/flake8_balanced_wrapping.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2256 2023-06-20 07:16:25.000000 flake8-balanced-wrapping-0.1.5/flake8_balanced_wrapping.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      354 2023-06-20 07:16:25.000000 flake8-balanced-wrapping-0.1.5/flake8_balanced_wrapping.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-20 07:16:25.000000 flake8-balanced-wrapping-0.1.5/flake8_balanced_wrapping.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       79 2023-06-20 07:16:25.000000 flake8-balanced-wrapping-0.1.5/flake8_balanced_wrapping.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-06-20 07:16:25.000000 flake8-balanced-wrapping-0.1.5/flake8_balanced_wrapping.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-06-20 07:16:25.000000 flake8-balanced-wrapping-0.1.5/flake8_balanced_wrapping.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16439 2023-06-20 07:16:14.000000 flake8-balanced-wrapping-0.1.5/flake8_balanced_wrapping.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1031 2023-06-20 07:16:25.813116 flake8-balanced-wrapping-0.1.5/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1631 2023-06-20 07:16:14.000000 flake8-balanced-wrapping-0.1.5/setup.py
```

### Comparing `flake8-balanced-wrapping-0.1.4/LICENSE` & `flake8-balanced-wrapping-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8-balanced-wrapping-0.1.4/PKG-INFO` & `flake8-balanced-wrapping-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-balanced-wrapping
-Version: 0.1.4
+Version: 0.1.5
 Summary: A flake8 plugin that helps you wrap code with visual balance.
 Home-page: https://github.com/PeterJCLaw/flake8-balanced-wrapping
 Author: Peter Law
 Author-email: PeterJCLaw@gmail.com
 License: Apache 2.0
 Project-URL: Issue tracker, https://github.com/PeterJCLaw/flake8-balanced-wrapping/issues
 Platform: UNKNOWN
```

### Comparing `flake8-balanced-wrapping-0.1.4/README.md` & `flake8-balanced-wrapping-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `flake8-balanced-wrapping-0.1.4/flake8_balanced_wrapping.egg-info/PKG-INFO` & `flake8-balanced-wrapping-0.1.5/flake8_balanced_wrapping.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-balanced-wrapping
-Version: 0.1.4
+Version: 0.1.5
 Summary: A flake8 plugin that helps you wrap code with visual balance.
 Home-page: https://github.com/PeterJCLaw/flake8-balanced-wrapping
 Author: Peter Law
 Author-email: PeterJCLaw@gmail.com
 License: Apache 2.0
 Project-URL: Issue tracker, https://github.com/PeterJCLaw/flake8-balanced-wrapping/issues
 Platform: UNKNOWN
```

### Comparing `flake8-balanced-wrapping-0.1.4/flake8_balanced_wrapping.py` & `flake8-balanced-wrapping-0.1.5/flake8_balanced_wrapping.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,22 +79,29 @@
     most_common_line_number: int
 
     @property
     def is_single_line_or_column(self) -> bool:
         return self.is_single_line or self.is_single_column
 
 
-def get_start_position(node: ast.AST) -> Position:
+def get_start_position(asttokens: ASTTokens, node: ast.AST) -> Position:
+    if (
+        isinstance(node, (ast.BoolOp, ast.IfExp)) and
+        expression_is_parenthesised(asttokens, node)
+    ):
+        open_paren = asttokens.prev_token(_first_token(node))
+        return Position(*open_paren.start)
+
     return Position.from_node_start(node)
 
 
-def get_start_positions(nodes: Iterable[ast.AST]) -> list[Position]:
+def get_start_positions(asttokens: ASTTokens, nodes: Iterable[ast.AST]) -> list[Position]:
     positions = []
     for node in nodes:
-        start = get_start_position(node)
+        start = get_start_position(asttokens, node)
         if start is not None:
             positions.append(start)
     return positions
 
 
 def get_end_position(node: ast.AST) -> Position:
     return Position(*_last_token(node).end)
@@ -125,15 +132,15 @@
     ) -> dict[int, list[ast.AST]]:
         by_line_no = collections.defaultdict(list)
 
         if include_node_start:
             by_line_no[reference.line].append(node)
 
         for x in nodes:
-            pos = get_start_position(x)
+            pos = get_start_position(self.asttokens, x)
             by_line_no[pos.line].append(x)
 
         if include_node_end:
             end_line, end_col = _last_token(node).end
             just_before_end_pos = Position(end_line, end_col - 1)
             end_positions = get_end_positions(nodes)
 
@@ -158,15 +165,15 @@
 
     def _record_error(
         self,
         node: ast.AST,
         nodes: list[ast.AST],
         error_type: type[UnderWrappedError] | type[OverWrappedError] = UnderWrappedError,
     ) -> None:
-        positions = get_start_positions(nodes)
+        positions = get_start_positions(self.asttokens, nodes)
         assert positions
         self.errors.append(error_type(node, positions))
 
     def _check_under_wrapping(
         self,
         node: ast.AST,
         reference: Position,
@@ -283,15 +290,18 @@
                 #        kwarg='',
                 #    )
                 #
                 # which we want to allow users to allow if they want.
                 summary = self._summarise_lines(by_line_no)
 
                 if not summary.is_single_line_or_column:
-                    positions = get_start_positions(by_line_no[summary.most_common_line_number])
+                    positions = get_start_positions(
+                        self.asttokens,
+                        by_line_no[summary.most_common_line_number],
+                    )
                     assert positions
                     self.errors.append(CallUnderWrappedError(node, positions))
 
         self.generic_visit(node)
 
     def visit_Dict(self, node: ast.Dict) -> None:
         by_line_no = self._get_nodes_by_line_number(
@@ -336,16 +346,16 @@
             [node.body, node.test, node.orelse],
             include_node_end=False,
             include_node_start=False,
         )
 
         if expression_is_parenthesised(self.asttokens, node):
             # Also account for the parens
-            open_paren = self.asttokens.prev_token(_first_token(node.body))
-            close_paren = self.asttokens.next_token(_last_token(node.orelse))
+            open_paren = self.asttokens.prev_token(_first_token(node))
+            close_paren = self.asttokens.next_token(_last_token(node))
 
             open_line = open_paren.start[0]
             close_line = close_paren.start[0]
 
             if open_line in by_line_no or close_line in by_line_no:
                 by_line_no[open_line].append(node)
                 by_line_no[close_line].append(node)
@@ -428,31 +438,39 @@
                 node,
                 [node, *node.values],
                 error_type=OverWrappedError,
             )
 
         elif expression_is_parenthesised(self.asttokens, node):
             # Also account for the parens
-            first_token = self.asttokens.prev_token(_first_token(node))
-            last_token = self.asttokens.next_token(_last_token(node))
+            open_paren = self.asttokens.prev_token(_first_token(node))
+            close_paren = self.asttokens.next_token(_last_token(node))
 
-            if first_token.start[0] in by_line_no or last_token.start[0] in by_line_no:
-                by_line_no[first_token.line].append(node)
-                by_line_no[last_token.line].append(node)
+            open_line = open_paren.start[0]
+            close_line = close_paren.start[0]
+
+            if (
+                open_line != close_line and
+                (open_line in by_line_no or close_line in by_line_no)
+            ):
+                by_line_no[open_line].append(node)
+                by_line_no[close_line].append(node)
 
                 self._record_error(
                     node,
                     [node, *node.values],
                     error_type=OverWrappedError,
                 )
 
         self.generic_visit(node)
 
     def visit_UnaryOp(self, node: ast.UnaryOp) -> None:
-        if node.lineno != node.operand.lineno:
+        operand_start = get_start_position(self.asttokens, node.operand)
+
+        if node.lineno != operand_start.line:
             self._record_error(
                 node,
                 [node, node.operand],
                 error_type=OverWrappedError,
             )
 
         self.generic_visit(node)
@@ -468,15 +486,15 @@
         self.generic_visit(node)
 
     def visit_Compare(self, node: ast.Compare) -> None:
         self._check_over_wrapping(
             node,
             Position.from_node_start(node.left),
             [node.left, *node.comparators],
-            include_node_end=True,
+            include_node_end=False,
             include_node_start=True,
         )
         self.generic_visit(node)
 
 
 def check(asttokens: ASTTokens) -> list[Error]:
     visitor = Visitor(asttokens)
```

### Comparing `flake8-balanced-wrapping-0.1.4/setup.cfg` & `flake8-balanced-wrapping-0.1.5/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 	build,
 	debian,
 	script
 ignore = 
 	C401
 	W504
 max_line_length = 105
+noqa-require-code = true
 
 [isort]
 atomic = True
 balanced_wrapping = True
 combine_as_imports = True
 include_trailing_comma = True
 length_sort = True
```

### Comparing `flake8-balanced-wrapping-0.1.4/setup.py` & `flake8-balanced-wrapping-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 
 long_description = (Path(__file__).parent / 'README.md').read_text()
 
 setup(
     name='flake8-balanced-wrapping',
-    version='0.1.4',
+    version='0.1.5',
     url='https://github.com/PeterJCLaw/flake8-balanced-wrapping',
     project_urls={
         'Issue tracker': 'https://github.com/PeterJCLaw/flake8-balanced-wrapping/issues',
     },
     description="A flake8 plugin that helps you wrap code with visual balance.",
     long_description=long_description,
     long_description_content_type='text/markdown',
```

