# Comparing `tmp/sbmlmath-0.0.0.tar.gz` & `tmp/sbmlmath-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sbmlmath-0.0.0.tar", last modified: Thu Mar 23 09:53:43 2023, max compression
+gzip compressed data, was "sbmlmath-0.0.1.tar", last modified: Tue Jun 20 06:19:09 2023, max compression
```

## Comparing `sbmlmath-0.0.0.tar` & `sbmlmath-0.0.1.tar`

### file list

```diff
@@ -1,27 +1,32 @@
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2023-03-23 09:53:43.241479 sbmlmath-0.0.0/
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2023-03-23 09:53:43.237479 sbmlmath-0.0.0/.github/
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2023-03-23 09:53:43.237479 sbmlmath-0.0.0/.github/workflows/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1209 2023-03-23 09:34:07.000000 sbmlmath-0.0.0/.github/workflows/ci.yaml
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)       37 2023-03-23 09:37:52.000000 sbmlmath-0.0.0/.gitignore
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1462 2023-03-23 09:22:44.000000 sbmlmath-0.0.0/LICENSE
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1240 2023-03-23 09:53:43.241479 sbmlmath-0.0.0/PKG-INFO
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      979 2023-03-23 09:49:35.000000 sbmlmath-0.0.0/README.md
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      504 2023-03-23 09:26:42.000000 sbmlmath-0.0.0/pyproject.toml
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2023-03-23 09:53:43.237479 sbmlmath-0.0.0/sbmlmath/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      932 2023-03-23 09:16:23.000000 sbmlmath-0.0.0/sbmlmath/__init__.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    16085 2023-03-23 09:47:19.000000 sbmlmath-0.0.0/sbmlmath/mathml_parser.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     3282 2023-03-23 09:11:13.000000 sbmlmath-0.0.0/sbmlmath/mathml_printer.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1668 2023-03-22 14:10:30.000000 sbmlmath-0.0.0/sbmlmath/species_symbol.py
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2023-03-23 09:53:43.237479 sbmlmath-0.0.0/sbmlmath.egg-info/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1240 2023-03-23 09:53:43.000000 sbmlmath-0.0.0/sbmlmath.egg-info/PKG-INFO
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      468 2023-03-23 09:53:43.000000 sbmlmath-0.0.0/sbmlmath.egg-info/SOURCES.txt
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)        1 2023-03-23 09:53:43.000000 sbmlmath-0.0.0/sbmlmath.egg-info/dependency_links.txt
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)       46 2023-03-23 09:53:43.000000 sbmlmath-0.0.0/sbmlmath.egg-info/requires.txt
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)        9 2023-03-23 09:53:43.000000 sbmlmath-0.0.0/sbmlmath.egg-info/top_level.txt
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)       38 2023-03-23 09:53:43.241479 sbmlmath-0.0.0/setup.cfg
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2023-03-23 09:53:43.241479 sbmlmath-0.0.0/tests/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1353 2023-03-23 09:34:43.000000 sbmlmath-0.0.0/tests/test_mathml_parser_sbml_semantic_suite.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1395 2023-03-23 09:49:22.000000 sbmlmath-0.0.0/tests/test_misc.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      803 2023-03-23 09:15:49.000000 sbmlmath-0.0.0/tests/test_parser.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1083 2023-03-23 09:15:49.000000 sbmlmath-0.0.0/tests/test_printer.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     4034 2023-03-23 09:15:49.000000 sbmlmath-0.0.0/tests/test_species_symbol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 06:19:09.577337 sbmlmath-0.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 06:19:09.573337 sbmlmath-0.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 06:19:09.573337 sbmlmath-0.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-20 06:19:00.000000 sbmlmath-0.0.1/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-20 06:19:00.000000 sbmlmath-0.0.1/.github/workflows/deploy_release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-20 06:19:00.000000 sbmlmath-0.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-20 06:19:00.000000 sbmlmath-0.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-20 06:19:00.000000 sbmlmath-0.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-20 06:19:09.577337 sbmlmath-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-20 06:19:00.000000 sbmlmath-0.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-20 06:19:00.000000 sbmlmath-0.0.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 06:19:09.573337 sbmlmath-0.0.1/sbmlmath/
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-20 06:19:00.000000 sbmlmath-0.0.1/sbmlmath/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-06-20 06:19:00.000000 sbmlmath-0.0.1/sbmlmath/cfunction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-20 06:19:00.000000 sbmlmath-0.0.1/sbmlmath/csymbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17053 2023-06-20 06:19:00.000000 sbmlmath-0.0.1/sbmlmath/mathml_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-06-20 06:19:00.000000 sbmlmath-0.0.1/sbmlmath/mathml_printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-20 06:19:00.000000 sbmlmath-0.0.1/sbmlmath/species_symbol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 06:19:09.577337 sbmlmath-0.0.1/sbmlmath.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-20 06:19:09.000000 sbmlmath-0.0.1/sbmlmath.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-20 06:19:09.000000 sbmlmath-0.0.1/sbmlmath.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 06:19:09.000000 sbmlmath-0.0.1/sbmlmath.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-20 06:19:09.000000 sbmlmath-0.0.1/sbmlmath.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 06:19:09.000000 sbmlmath-0.0.1/sbmlmath.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 06:19:09.577337 sbmlmath-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 06:19:09.577337 sbmlmath-0.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-20 06:19:00.000000 sbmlmath-0.0.1/tests/test_csymbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-20 06:19:00.000000 sbmlmath-0.0.1/tests/test_mathml_parser_sbml_semantic_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-06-20 06:19:00.000000 sbmlmath-0.0.1/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-20 06:19:00.000000 sbmlmath-0.0.1/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-20 06:19:00.000000 sbmlmath-0.0.1/tests/test_printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-06-20 06:19:00.000000 sbmlmath-0.0.1/tests/test_species_symbol.py
```

### Comparing `sbmlmath-0.0.0/.github/workflows/ci.yaml` & `sbmlmath-0.0.1/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `sbmlmath-0.0.0/LICENSE` & `sbmlmath-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sbmlmath-0.0.0/PKG-INFO` & `sbmlmath-0.0.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 Metadata-Version: 2.1
 Name: sbmlmath
-Version: 0.0.0
+Version: 0.0.1
 Summary: SBML Math <-> SymPy
 Author-email: Daniel Weindl <sci@danielweindl.de>
 License: BSD-3-Clause
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # sbmlmath - a Python library for handling SBML MathML
 
-This is Python library for interconverting [SymPy](https://github.com/sympy/sympy/) 
-expressions and [SBML](https://sbml.org/) MathML. 
-SBML uses a subset of [MathML](https://www.w3.org/Math/) that this library 
-tries to support. This is not (intended to be) a general MathML parser. 
+This is Python library for interconverting [SymPy](https://github.com/sympy/sympy/)
+expressions and [SBML](https://sbml.org/) MathML.
+SBML uses a subset of [MathML](https://www.w3.org/Math/) that this library
+tries to support. This is not (intended to be) a general MathML parser.
 
 Main functionality:
 
 * sympy -> SBML MathML
 * SBML MathML -> sympy
-  * in particular for cases where `sympy.sympify(libsbml.formulaToL3String(...))` 
+  * in particular for cases where `sympy.sympify(libsbml.formulaToL3String(...))`
     won't do the job
   * retaining unit annotations and other `<ci>` attributes
 
 **NOTE: This is under development and the API is to be considered unstable**
 
 ## Usage
 
 ```python
-from sbmlmath import MyMathMLContentPrinter, SBMLMathMLParser
+from sbmlmath import SBMLMathMLPrinter, SBMLMathMLParser
 import sympy as sp
 
 sympy_expr = sp.sympify("A ** B + exp(C) * D")
-mathml = MyMathMLContentPrinter().doprint(sympy_expr)
+mathml = SBMLMathMLPrinter().doprint(sympy_expr)
 print(mathml)
 
 cycled_sympy = SBMLMathMLParser().parse_str(mathml)
 print(cycled_sympy)
 assert sympy_expr == cycled_sympy
 ```
```

### Comparing `sbmlmath-0.0.0/README.md` & `sbmlmath-0.0.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # sbmlmath - a Python library for handling SBML MathML
 
-This is Python library for interconverting [SymPy](https://github.com/sympy/sympy/) 
-expressions and [SBML](https://sbml.org/) MathML. 
-SBML uses a subset of [MathML](https://www.w3.org/Math/) that this library 
-tries to support. This is not (intended to be) a general MathML parser. 
+This is Python library for interconverting [SymPy](https://github.com/sympy/sympy/)
+expressions and [SBML](https://sbml.org/) MathML.
+SBML uses a subset of [MathML](https://www.w3.org/Math/) that this library
+tries to support. This is not (intended to be) a general MathML parser.
 
 Main functionality:
 
 * sympy -> SBML MathML
 * SBML MathML -> sympy
-  * in particular for cases where `sympy.sympify(libsbml.formulaToL3String(...))` 
+  * in particular for cases where `sympy.sympify(libsbml.formulaToL3String(...))`
     won't do the job
   * retaining unit annotations and other `<ci>` attributes
 
 **NOTE: This is under development and the API is to be considered unstable**
 
 ## Usage
 
 ```python
-from sbmlmath import MyMathMLContentPrinter, SBMLMathMLParser
+from sbmlmath import SBMLMathMLPrinter, SBMLMathMLParser
 import sympy as sp
 
 sympy_expr = sp.sympify("A ** B + exp(C) * D")
-mathml = MyMathMLContentPrinter().doprint(sympy_expr)
+mathml = SBMLMathMLPrinter().doprint(sympy_expr)
 print(mathml)
 
 cycled_sympy = SBMLMathMLParser().parse_str(mathml)
 print(cycled_sympy)
 assert sympy_expr == cycled_sympy
 ```
```

### Comparing `sbmlmath-0.0.0/sbmlmath/__init__.py` & `sbmlmath-0.0.1/sbmlmath/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,47 @@
 from typing import Union
 
 import libsbml
 import sympy as sp
 
 from .mathml_parser import SBMLMathMLParser
-from .mathml_printer import MyMathMLContentPrinter
+from .mathml_printer import SBMLMathMLPrinter
 from .species_symbol import SpeciesSymbol
+from .csymbol import *
+from .cfunction import *
+
+
+__all__ = [
+    "SBMLMathMLParser",
+    "SBMLMathMLPrinter",
+    "SpeciesSymbol",
+    "TimeSymbol",
+    "sympy_to_sbml_math",
+    "sbml_math_to_sympy",
+    *csymbol.__all__,
+    *cfunction.__all__,
+]
 
 
 def sympy_to_sbml_math(sp_expr: sp.Expr) -> libsbml.ASTNode:
     """Convert sympy expression to SBML math ASTNode"""
-    mathml = MyMathMLContentPrinter().doprint(sp_expr)
+    mathml = SBMLMathMLPrinter().doprint(sp_expr)
 
     if ast_node := libsbml.readMathMLFromString(mathml):
         return ast_node
 
     raise ValueError(
-        f"Unknown error handling math expression:\n{sp_expr}\n"
-        f"{mathml}"
+        f"Unknown error handling math expression:\n{sp_expr}\n" f"{mathml}"
     )
 
 
 def sbml_math_to_sympy(
-        sbml_obj: Union[libsbml.SBase, libsbml.ASTNode]
+    sbml_obj: Union[libsbml.SBase, libsbml.ASTNode]
 ) -> sp.Expr:
     """Convert SBML MathML to sympy using the custom MathML parser"""
-    ast_node = sbml_obj if isinstance(sbml_obj, libsbml.ASTNode) \
+    ast_node = (
+        sbml_obj
+        if isinstance(sbml_obj, libsbml.ASTNode)
         else sbml_obj.getMath()
+    )
     mathml = libsbml.writeMathMLToString(ast_node)
     return SBMLMathMLParser().parse_str(mathml)
-
```

### Comparing `sbmlmath-0.0.0/sbmlmath/mathml_parser.py` & `sbmlmath-0.0.1/sbmlmath/mathml_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 """SBML mathml to sympy."""
 import contextlib
 import operator as operators
 from functools import reduce
 from io import BytesIO
-
+from typing import Union
 import sympy as sp
 from lxml import etree
 from pint import UnitRegistry
 from sympy.logic.boolalg import Boolean, BooleanFalse, BooleanTrue
 
 from .species_symbol import SpeciesSymbol
+from .csymbol import CSymbol
+from .cfunction import CFunction
+
+__all__ = ["SBMLMathMLParser"]
+
 
 mathml_ns = "http://www.w3.org/1998/Math/MathML"
 _ureg = UnitRegistry()
 _ureg.Quantity.name = property(fget=lambda s: f"({s})")
-_ureg.Quantity_sympy_ = lambda s: sp.sympify(f'{s.m}*{s.u:~}')
+_ureg.Quantity_sympy_ = lambda s: sp.sympify(f"{s.m}*{s.u:~}")
 
 mathml_op_sympy_trigonometric = {
     f"{{{mathml_ns}}}sin": sp.sin,
     f"{{{mathml_ns}}}cos": sp.cos,
     f"{{{mathml_ns}}}tan": sp.tan,
     f"{{{mathml_ns}}}sec": sp.sec,
     f"{{{mathml_ns}}}csc": sp.csc,
@@ -45,23 +50,28 @@
 mathml_op_sympy_boolean = {
     f"{{{mathml_ns}}}and": sp.And,
     f"{{{mathml_ns}}}or": sp.Or,
     f"{{{mathml_ns}}}xor": sp.Xor,
 }
 
 mathml_op_sympy = {
-    f"{{{mathml_ns}}}times":
-        lambda *args: reduce(operators.mul, args, sp.Integer(1)),
-    f"{{{mathml_ns}}}power": lambda base, exponent: base ** exponent,
-    f"{{{mathml_ns}}}eq": sp.Equality,
-    f"{{{mathml_ns}}}neq": sp.Unequality,
-    f"{{{mathml_ns}}}lt": sp.StrictLessThan,
-    f"{{{mathml_ns}}}gt": sp.StrictGreaterThan,
-    f"{{{mathml_ns}}}geq": sp.GreaterThan,
-    f"{{{mathml_ns}}}leq": sp.LessThan,
+    f"{{{mathml_ns}}}times": lambda *args: reduce(
+        operators.mul, args, sp.Integer(1)
+    ),
+    f"{{{mathml_ns}}}power": lambda base, exponent: base**exponent,
+    f"{{{mathml_ns}}}eq": lambda *args: sp.Equality(*args, evaluate=False),
+    f"{{{mathml_ns}}}neq": lambda *args: sp.Unequality(*args, evaluate=False),
+    f"{{{mathml_ns}}}lt": lambda *args: sp.StrictLessThan(
+        *args, evaluate=False
+    ),
+    f"{{{mathml_ns}}}gt": lambda *args: sp.StrictGreaterThan(
+        *args, evaluate=False
+    ),
+    f"{{{mathml_ns}}}geq": lambda *args: sp.GreaterThan(*args, evaluate=False),
+    f"{{{mathml_ns}}}leq": lambda *args: sp.LessThan(*args, evaluate=False),
     f"{{{mathml_ns}}}max": sp.Max,
     f"{{{mathml_ns}}}min": sp.Min,
     f"{{{mathml_ns}}}abs": sp.Abs,
     f"{{{mathml_ns}}}exp": sp.exp,
     f"{{{mathml_ns}}}ceiling": sp.ceiling,
     f"{{{mathml_ns}}}floor": sp.floor,
     f"{{{mathml_ns}}}factorial": sp.factorial,
@@ -85,15 +95,15 @@
     f"{{{mathml_ns}}}floor",
     f"{{{mathml_ns}}}factorial",
     f"{{{mathml_ns}}}ln",
     f"{{{mathml_ns}}}not",
     f"{{{mathml_ns}}}min",
     f"{{{mathml_ns}}}max",
     f"{{{mathml_ns}}}root",
-    *mathml_op_sympy_trigonometric
+    *mathml_op_sympy_trigonometric,
 }
 # n-ary functions
 n_ary = {
     f"{{{mathml_ns}}}times",
     f"{{{mathml_ns}}}plus",
     *mathml_op_sympy_boolean,
     f"{{{mathml_ns}}}lt",
@@ -119,50 +129,59 @@
     """MathML parser for sympy, restricted to the SBML subset of MathML 2.0
 
     SBML spec:
     https://raw.githubusercontent.com/combine-org/combine-specifications/main/specifications/files/sbml.level-3.version-2.core.release-2.pdf
     section 3.4
     """
 
-    def __init__(self, ureg: UnitRegistry = None):
+    def __init__(
+        self,
+        level: Union[int, str] = 3,
+        version: Union[int, str] = 2,
+        ureg: UnitRegistry = None,
+        floats_as_rationals=True,
+    ):
         self.ureg = ureg or _ureg or UnitRegistry()
-        # TODO configurable version
+        self.sbml_core_ns = (
+            f"http://www.sbml.org/sbml/level{level}/version{version}/core"
+        )
         #  TODO {prefix=>url}
-        self.sbml_core_ns = \
-            'http://www.sbml.org/sbml/level3/version2/core'
-        self.sbml_multi_ns = \
-            'http://www.sbml.org/sbml/level3/version1/multi/version1'
+        self.sbml_multi_ns = (
+            # L3V2 doesn't work
+            f"http://www.sbml.org/sbml/level{level}/version1/multi/version1"
+        )
+        self.floats_as_rationals = floats_as_rationals
 
     def parse_file(self, file_like) -> sp.Expr:
         element_tree = etree.parse(file_like)
         for element in element_tree.iter():
             if element.tag == f"{{{mathml_ns}}}math":
                 continue
 
             return self._parse_element(element)
 
     def parse_str(self, mathml: str):
-        # (fragile) workaround for libsbml dropping xmlns declarations for
-        #  namespaces other than 'sbml'
-        if "multi:" in mathml and 'xmlns:multi' not in mathml:
+        # (fragile) workaround for libsbml<5.20.0 dropping xmlns declarations
+        #  for namespaces other than 'sbml'
+        if "multi:" in mathml and "xmlns:multi" not in mathml:
             math_element = '<math xmlns="http://www.w3.org/1998/Math/MathML"'
             mathml = mathml.replace(
                 math_element,
-                f'{math_element} xmlns:multi="{self.sbml_multi_ns}"'
+                f'{math_element} xmlns:multi="{self.sbml_multi_ns}"',
             )
         # end
 
         return self.parse_file(file_like=BytesIO(mathml.encode()))
 
     def _parse_element(self, element: etree._Element) -> sp.Expr:
         mathml_prefix = f"{{{mathml_ns}}}"
         if not element.tag.startswith(mathml_prefix):
             raise AssertionError(element.tag)
 
-        stripped_tag = element.tag[len(mathml_prefix):]
+        stripped_tag = element.tag[len(mathml_prefix) :]
 
         handler = f"handle_{stripped_tag}"
         if handler := getattr(self, handler, None):
             try:
                 return handler(element)
             except NotImplementedError:
                 raise
@@ -177,46 +196,58 @@
 
     def handle_apply(self, element: etree._Element) -> sp.Expr:
         """Handle <apply>"""
         operator, *operands = element
         sym_operands = list(map(self._parse_element, operands))
 
         # TODO cleanup; doesn't check properly if compatible with 2 args
-        if operator.tag not in (f"{{{mathml_ns}}}csymbol",
-                                f"{{{mathml_ns}}}ci") \
-                and (len(operands) == 1 and operator.tag not in unary
-                     or len(operands) > 2 and operator.tag not in n_ary):
+        if operator.tag not in (
+            f"{{{mathml_ns}}}csymbol",
+            f"{{{mathml_ns}}}ci",
+        ) and (
+            len(operands) == 1
+            and operator.tag not in unary
+            or len(operands) > 2
+            and operator.tag not in n_ary
+        ):
             raise AssertionError(
                 f"Unknown arity for {operator.tag} ({operands}"
             )
 
         if operator.tag.startswith(f"{{{mathml_ns}}}"):
-            stripped_tag = operator.tag[len(f"{{{mathml_ns}}}"):]
-            if len(operands) == 1 \
-                    and stripped_tag in {'plus', 'times', 'and', 'or',
-                                         'xor', 'min', 'max'}:
+            stripped_tag = operator.tag[len(f"{{{mathml_ns}}}") :]
+            if len(operands) == 1 and stripped_tag in {
+                "plus",
+                "times",
+                "and",
+                "or",
+                "xor",
+                "min",
+                "max",
+            }:
                 return sym_operands[0]
 
-            if stripped_tag in ("gt", "lt", "leq", "geq", "eq") \
-                    and len(operands) >= 3:
+            if (
+                stripped_tag in ("gt", "lt", "leq", "geq", "eq")
+                and len(operands) >= 3
+            ):
                 # n-ary relational operators:
                 #  a < b < c cannot directory be represented in sympy.
                 #  either change to `a < b and b < c`, to be sympy-evaluatable,
                 #  or to Function('MathML_Lt')(a, b, c), which will cycle
                 #  (although potentially collide with other functions with
                 #  that name), but which cannot be evaluated in sympy.
                 #  The Function-approach won't work when used in piecewise
                 #  -> "Second argument must be a Boolean, not `lt`"
                 #  Therefore, chain expressions with `and`.
                 sym_operator = mathml_op_sympy[operator.tag]
                 expr = True
                 for i in range(len(sym_operands) - 1):
                     expr = sp.And(
-                        expr, sym_operator(sym_operands[i],
-                                           sym_operands[i + 1])
+                        expr, sym_operator(sym_operands[i], sym_operands[i + 1])
                     )
                 return expr
 
         # TODO: need to handle boolean->{int,float} conversion via
         #  `Piecewise((1, expr),(0,True))`
         #  {int,float} -> bool
         #  `Piecewise((True, expr != 0),(False,True))`
@@ -267,84 +298,87 @@
             # so we use modulo instead. this won't cycle.
             # a // b = (a - a mod b) / b
             assert len(operands) == 2
             a, b = sym_operands
             return (a - a % b) / b
 
         if operator.tag == f"{{{mathml_ns}}}csymbol":
-            # TODO store definitionURL somewhere?
-            # TODO need to be able to distinguish between lambdas referenced
-            #  through ci and functions from csymbols
-            assert operator.attrib['encoding'] == "text"
-            return sp.Function(operator.text.strip())(*sym_operands)
+            # examples: rateOf, delay, distributions from distrib package
+            assert operator.attrib["encoding"] == "text"
+            return CFunction(
+                operator.text.strip(),
+                definition_url=operator.attrib["definitionURL"],
+            )(*sym_operands)
 
         if operator.tag == f"{{{mathml_ns}}}ci":
             assert not operator.attrib
-            return sp.Function(operator.text.strip())(*sym_operands)
+            return sp.Function(operator.text.strip(), real=True)(*sym_operands)
 
         raise NotImplementedError(f"Unsupported operator {operator.tag}.")
 
     def handle_ci(self, element: etree._Element) -> sp.Expr:
         """Handle identifiers."""
         handled_attrs = {
             # TODO: remove after fixing xmlns in model
-            'multi:representationType',
-            'multi:speciesReference',
-            f'{{{self.sbml_multi_ns}}}representationType',
-            f'{{{self.sbml_multi_ns}}}speciesReference',
+            "multi:representationType",
+            "multi:speciesReference",
+            f"{{{self.sbml_multi_ns}}}representationType",
+            f"{{{self.sbml_multi_ns}}}speciesReference",
         }
         if unhandled_attrs := (set(element.attrib.keys()) - handled_attrs):
             raise NotImplementedError(
-                f"Unhandled <ci> attributes: {unhandled_attrs}")
+                f"Unhandled <ci> attributes: {unhandled_attrs}"
+            )
 
         representation_type = element.attrib.get(
-            f'{{{self.sbml_multi_ns}}}representationType', None) \
-                              or element.attrib.get('multi:representationType', None)
+            f"{{{self.sbml_multi_ns}}}representationType", None
+        ) or element.attrib.get("multi:representationType", None)
         species_reference = element.attrib.get(
-            f'{{{self.sbml_multi_ns}}}speciesReference', None) \
-                            or element.attrib.get('multi:speciesReference',
-                                                  None)
+            f"{{{self.sbml_multi_ns}}}speciesReference", None
+        ) or element.attrib.get("multi:speciesReference", None)
         symbol_name = element.text.strip()
         if representation_type or species_reference:
             return SpeciesSymbol(
                 name=symbol_name,
                 representation_type=representation_type,
                 species_reference=species_reference,
             )
         return sp.Symbol(symbol_name)
 
     def handle_cn(self, element: etree._Element) -> sp.Expr:
         """Handle numbers."""
         handled_attrs = {
-            'type',
-            f'{{{self.sbml_core_ns}}}units',
+            "type",
+            f"{{{self.sbml_core_ns}}}units",
         }
         if unhandled_attrs := (set(element.attrib.keys()) - handled_attrs):
             raise NotImplementedError(
-                f"Unhandled <cn> attributes: {unhandled_attrs}")
-        dtype = element.attrib.get('type', 'real')
+                f"Unhandled <cn> attributes: {unhandled_attrs}"
+            )
+        dtype = element.attrib.get("type", "real")
         converter = {
-            'real':
-                lambda element: sp.Float(element.text),
-            'integer':
-                lambda element: sp.Integer(element.text),
-            'rational':
-                lambda element: sp.Rational(element.text, element[0].tail),
-            'e-notation':
+            "real": (lambda element: sp.Rational(element.text))
+            if self.floats_as_rationals
+            else lambda element: sp.Float(element.text),
+            "integer": lambda element: sp.Integer(element.text),
+            "rational": lambda element: sp.Rational(
+                element.text, element[0].tail
+            ),
+            "e-notation":
             # this won't cycle. we don't have a corresponding
             #  representation in sympy
-                lambda element: sp.Float(
-                    float(element.text) * 10 ** int(element[0].tail)
-                ),
+            lambda element: sp.Float(
+                float(element.text) * 10 ** int(element[0].tail)
+            ),
         }.get(dtype)
         if not converter:
             raise NotImplementedError(f"Unhandled type: {dtype}")
         obj = converter(element)
 
-        if units := element.attrib.get(f'{{{self.sbml_core_ns}}}units', None):
+        if units := element.attrib.get(f"{{{self.sbml_core_ns}}}units", None):
             if units not in self.ureg:
                 # TODO fixme: replace rhs by base units
                 #  this requires access to the underlying SBML model to access
                 #  unit definitions. they should be parsed during __init__.
                 #  base units defined in SBML can be handled without a model,
                 #  as they are not allowed to be redefined (are they?).
                 #  should start from an empty UnitRegistry, as sbml could
@@ -364,25 +398,30 @@
                 assert len(e) == 2
                 cond = self._parse_element(e[1])
                 if not isinstance(cond, Boolean):
                     raise NotImplementedError(
                         "Cannot handle non-boolean piecewise conditions: "
                         f"{cond}"
                     )
-                expr_cond_pairs.append((self._parse_element(e[0]), cond), )
+                expr_cond_pairs.append(
+                    (self._parse_element(e[0]), cond),
+                )
             elif e.tag == f"{{{mathml_ns}}}otherwise":
                 # may occur only as last condition
                 assert e is element[-1]
                 assert len(e) == 1
-                expr_cond_pairs.append((self._parse_element(e[0]), True), )
+                expr_cond_pairs.append(
+                    (self._parse_element(e[0]), True),
+                )
             else:
                 raise AssertionError(e.tag)
-        return sp.Piecewise(*expr_cond_pairs)
+        return sp.Piecewise(*expr_cond_pairs, evaluate=False)
 
     def handle_lambda(self, element: etree._Element) -> sp.Expr:
+        # See https://www.w3.org/TR/MathML2/chapter4.html#id.4.2.1.7
         # collect arguments / bound variables
         args = []
         for e in element[:-1]:
             assert e.tag == f"{{{mathml_ns}}}bvar"
             assert len(e) == 1
             args.append(self._parse_element(e[0]))
 
@@ -394,16 +433,20 @@
         return self._parse_element(element[0])
 
     def handle_logbase(self, element: etree._Element) -> sp.Expr:
         assert len(element) == 1
         return self._parse_element(element[0])
 
     def handle_csymbol(self, element: etree._Element) -> sp.Expr:
-        assert element.attrib['encoding'] == "text"
-        return sp.Dummy(element.text.strip())
+        assert element.attrib["encoding"] == "text"
+        return CSymbol(
+            element.text.strip(),
+            encoding=element.attrib["encoding"],
+            definition_url=element.attrib["definitionURL"],
+        )
 
 
 def _bool2num(x):
     if isinstance(x, BooleanFalse):
         return sp.Integer(0)
     if isinstance(x, BooleanTrue):
         return sp.Integer(1)
```

### Comparing `sbmlmath-0.0.0/sbmlmath/species_symbol.py` & `sbmlmath-0.0.1/sbmlmath/species_symbol.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """SBML MathML related functionality"""
 from typing import Literal, Optional
 
 import sympy as sp
 
+__all__ = ["SpeciesSymbol"]
+
 
 class SpeciesSymbol(sp.Dummy):
     """
     Represents a <ci> element containing a species.
 
     Represents e.g.:
     ``<ci multi:representationType="sum"> bla </ci>``
@@ -16,22 +18,23 @@
     Subclassed from sympy.Dummy to avoid caching issues, due to using the same
     name but with different meanings.
 
     representation_type: SBML-multi spec 3.26.2
     species_reference: SBML-multi spec 3.26.1. ID of a species reference in the
         same reaction.
     """
+
     _cache = {}
 
     def __new__(
-            cls, *args,
-            representation_type:
-            Optional[Literal['sum', 'numericValue']] = None,
-            species_reference: str = None,
-            **kwargs
+        cls,
+        *args,
+        representation_type: Optional[Literal["sum", "numericValue"]] = None,
+        species_reference: str = None,
+        **kwargs,
     ):
         # Cache instances.
         # If not done: (SpeciesSymbol("A") == SpeciesSymbol("A")) == False
         if not (name := kwargs.get("name")):
             name = args[0]
         cache_key = (name, representation_type, species_reference)
         if cached := cls._cache.get(cache_key):
@@ -42,13 +45,19 @@
         obj.species_reference = species_reference
 
         cls._cache[cache_key] = obj
 
         return obj
 
     def __repr__(self):
-        rt = f"representation_type={self.representation_type},"\
-            if self.representation_type else ""
-        sr = f"species_reference={self.species_reference}," \
-            if self.species_reference else ""
+        rt = (
+            f"representation_type={self.representation_type},"
+            if self.representation_type
+            else ""
+        )
+        sr = (
+            f"species_reference={self.species_reference},"
+            if self.species_reference
+            else ""
+        )
 
         return f"<{self.name}({rt}{sr})>"
```

### Comparing `sbmlmath-0.0.0/sbmlmath.egg-info/PKG-INFO` & `sbmlmath-0.0.1/sbmlmath.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 Metadata-Version: 2.1
 Name: sbmlmath
-Version: 0.0.0
+Version: 0.0.1
 Summary: SBML Math <-> SymPy
 Author-email: Daniel Weindl <sci@danielweindl.de>
 License: BSD-3-Clause
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # sbmlmath - a Python library for handling SBML MathML
 
-This is Python library for interconverting [SymPy](https://github.com/sympy/sympy/) 
-expressions and [SBML](https://sbml.org/) MathML. 
-SBML uses a subset of [MathML](https://www.w3.org/Math/) that this library 
-tries to support. This is not (intended to be) a general MathML parser. 
+This is Python library for interconverting [SymPy](https://github.com/sympy/sympy/)
+expressions and [SBML](https://sbml.org/) MathML.
+SBML uses a subset of [MathML](https://www.w3.org/Math/) that this library
+tries to support. This is not (intended to be) a general MathML parser.
 
 Main functionality:
 
 * sympy -> SBML MathML
 * SBML MathML -> sympy
-  * in particular for cases where `sympy.sympify(libsbml.formulaToL3String(...))` 
+  * in particular for cases where `sympy.sympify(libsbml.formulaToL3String(...))`
     won't do the job
   * retaining unit annotations and other `<ci>` attributes
 
 **NOTE: This is under development and the API is to be considered unstable**
 
 ## Usage
 
 ```python
-from sbmlmath import MyMathMLContentPrinter, SBMLMathMLParser
+from sbmlmath import SBMLMathMLPrinter, SBMLMathMLParser
 import sympy as sp
 
 sympy_expr = sp.sympify("A ** B + exp(C) * D")
-mathml = MyMathMLContentPrinter().doprint(sympy_expr)
+mathml = SBMLMathMLPrinter().doprint(sympy_expr)
 print(mathml)
 
 cycled_sympy = SBMLMathMLParser().parse_str(mathml)
 print(cycled_sympy)
 assert sympy_expr == cycled_sympy
 ```
```

### Comparing `sbmlmath-0.0.0/tests/test_mathml_parser_sbml_semantic_suite.py` & `sbmlmath-0.0.1/tests/test_mathml_parser_sbml_semantic_suite.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,39 +6,40 @@
 from pathlib import Path
 
 import libsbml
 import pytest
 
 from sbmlmath import SBMLMathMLParser
 
-sbml_test_suite_root = os.environ.get('SBML_TEST_SUITE_ROOT', '')
+sbml_test_suite_root = os.environ.get("SBML_TEST_SUITE_ROOT", "")
 if not sbml_test_suite_root:
     pytest.skip("$SBML_TEST_SUITE_ROOT not set", allow_module_level=True)
 
-cases_root = Path(sbml_test_suite_root, 'cases', 'semantic')
+cases_root = Path(sbml_test_suite_root, "cases", "semantic")
 cases = sorted(cases_root.rglob("*-sbml-l3v2.xml"))
 assert len(cases)
+
+
 @pytest.mark.parametrize(
-    ('sbml_file', ),
-    [[file] for file in cases],
-    ids=map(lambda x: x.stem, cases)
+    ("sbml_file",), [[file] for file in cases], ids=map(lambda x: x.stem, cases)
 )
 def test_sbml(sbml_file):
     print()
     print(sbml_file)
 
     # load file, try to parse all math elements
     sbml_reader = libsbml.SBMLReader()
     sbml_doc = sbml_reader.readSBMLFromFile(str(sbml_file))
     sbml_model = sbml_doc.getModel()
 
     parser = SBMLMathMLParser()
     for element in sbml_model.getListOfAllElements():
-        if (get_math := getattr(element, 'getMath', None)) \
-                and (mathml := libsbml.writeMathMLToString(get_math())):
+        if (get_math := getattr(element, "getMath", None)) and (
+            mathml := libsbml.writeMathMLToString(get_math())
+        ):
             print(element.getId())
             print(mathml)
             try:
                 sym = parser.parse_str(mathml)
                 print(sym)
             except NotImplementedError as e:
                 pytest.skip(str(e))
```

### Comparing `sbmlmath-0.0.0/tests/test_parser.py` & `sbmlmath-0.0.1/tests/test_parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import libsbml
 import pytest
 import sympy as sp
 from sbmlmath import *
 
+
 # https://sbml.org/software/libsbml/5.18.0/docs/formatted/python-api/classlibsbml_1_1_a_s_t_node.html
 @pytest.mark.parametrize(
-    ('formula_str',),
+    ("formula_str",),
     (
-            ("1 + a",),
-            ("1.0 + a",),
-            ("2.5 * x / 12",),
-            ("(3 + a) * b",),
-            ("5 - y * 3",),
-            ("sqrt(y)",),
-            ("pow(a, b)",),
-            ("-a",),
-            ("-a - b",),
-            # ("log(a) + log(x, y)",),
-    )
+        ("1 + a",),
+        ("1.0 + a",),
+        ("2.5 * x / 12",),
+        ("(3 + a) * b",),
+        ("5 - y * 3",),
+        ("sqrt(y)",),
+        ("pow(a, b)",),
+        ("-a",),
+        ("-a - b",),
+        # ("log(a) + log(x, y)",),
+    ),
 )
 def test_mathmlparser_vs_sympify(formula_str):
     ast_node = libsbml.parseL3Formula(formula_str)
     mathml = libsbml.writeMathMLToString(ast_node)
-    parser = SBMLMathMLParser()
+    parser = SBMLMathMLParser(floats_as_rationals=False)
     sym_expr = parser.parse_str(mathml)
     print(sym_expr)
     assert sym_expr == sp.sympify(formula_str)
-
```

### Comparing `sbmlmath-0.0.0/tests/test_species_symbol.py` & `sbmlmath-0.0.1/tests/test_species_symbol.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,69 +1,67 @@
-import libsbml
-import pytest
-import sympy as sp
 from sbmlmath import *
 
 
 def test_species_symbol_equality():
     sym1 = SpeciesSymbol("A", representation_type="sum")
     sym2 = SpeciesSymbol("A", species_reference="ref_to_A")
 
     # ensure they are not considered equal
     assert sym1 is not sym2
     assert sym1 != sym2
 
     # Test caching works
-    assert SpeciesSymbol("A", representation_type="sum") \
-           == SpeciesSymbol("A", representation_type="sum")
-    assert SpeciesSymbol("A", representation_type="sum") \
-           is SpeciesSymbol("A", representation_type="sum")
+    assert SpeciesSymbol("A", representation_type="sum") == SpeciesSymbol(
+        "A", representation_type="sum"
+    )
+    assert SpeciesSymbol("A", representation_type="sum") is SpeciesSymbol(
+        "A", representation_type="sum"
+    )
     assert SpeciesSymbol("A") is SpeciesSymbol("A")
 
 
 def test_species_symbol_operations():
     sym1 = SpeciesSymbol("A", representation_type="sum")
     sym2 = SpeciesSymbol("A", species_reference="ref_to_A")
 
     expr = sym1 + sym2
-    mathml = MyMathMLContentPrinter().doprint(expr)
+    mathml = SBMLMathMLPrinter().doprint(expr)
     assert mathml == (
         '<?xml version="1.0" encoding="UTF-8"?>\n'
         '<math xmlns="http://www.w3.org/1998/Math/MathML" '
-        'xmlns:sbml="http://www.sbml.org/sbml/level3/version2/core" '
         'xmlns:multi="http://www.sbml.org/sbml/level3/version1/multi/version1">\n'
         '<apply><plus/><ci multi:representationType="sum">A</ci>'
         '<ci multi:speciesReference="ref_to_A">A</ci></apply>'
-        '</math>'
+        "</math>"
     )
 
     expr = sym1 * sym2
-    mathml = MyMathMLContentPrinter().doprint(expr)
+    mathml = SBMLMathMLPrinter().doprint(expr)
     assert mathml == (
         '<?xml version="1.0" encoding="UTF-8"?>\n'
         '<math xmlns="http://www.w3.org/1998/Math/MathML" '
-        'xmlns:sbml="http://www.sbml.org/sbml/level3/version2/core" '
         'xmlns:multi="http://www.sbml.org/sbml/level3/version1/multi/version1">\n'
         '<apply><times/><ci multi:representationType="sum">A</ci>'
         '<ci multi:speciesReference="ref_to_A">A</ci></apply>'
-        '</math>'
+        "</math>"
     )
 
     expr = sym1 + sym1 + sym2 * sym2
-    mathml = MyMathMLContentPrinter().doprint(expr)
+    mathml = SBMLMathMLPrinter().doprint(expr)
     assert mathml == (
         '<?xml version="1.0" encoding="UTF-8"?>\n'
         '<math xmlns="http://www.w3.org/1998/Math/MathML" '
         'xmlns:sbml="http://www.sbml.org/sbml/level3/version2/core" '
         'xmlns:multi="http://www.sbml.org/sbml/level3/version1/multi/version1">\n'
-        '<apply><plus/><apply><times/><cn sbml:units="dimensionless">2</cn>'
+        "<apply><plus/><apply><times/>"
+        '<cn type="integer" sbml:units="dimensionless">2</cn>'
         '<ci multi:representationType="sum">A</ci></apply>'
         '<apply><power/><ci multi:speciesReference="ref_to_A">A</ci>'
-        '<cn sbml:units="dimensionless">2</cn></apply></apply>'
-        '</math>'
+        '<cn type="integer" sbml:units="dimensionless">2</cn></apply></apply>'
+        "</math>"
     )
 
     # check subs() works
     assert (-1 + sym1).subs(sym1, 1) == 0
 
     # test mathml -> sympy
     mathml_exp = (
@@ -71,27 +69,26 @@
         '<math xmlns="http://www.w3.org/1998/Math/MathML" '
         'xmlns:sbml="http://www.sbml.org/sbml/level3/version2/core" '
         'xmlns:multi="http://www.sbml.org/sbml/level3/version1/multi/version1">\n'
         '<apply><plus/><apply><times/><cn sbml:units="dimensionless">2</cn>'
         '<ci multi:representationType="sum">A</ci></apply>'
         '<apply><power/><ci multi:speciesReference="ref_to_A">A</ci>'
         '<cn sbml:units="dimensionless">2</cn></apply></apply>'
-        '</math>'
+        "</math>"
     )
-    sym_expr = SBMLMathMLParser().parse_str(mathml_exp)
-    mathml_act = MyMathMLContentPrinter().doprint(sym_expr)
+    sym_expr = SBMLMathMLParser(floats_as_rationals=False).parse_str(mathml_exp)
+    mathml_act = SBMLMathMLPrinter().doprint(sym_expr)
 
     # not an exact match, but close enough, for now
     #  TODO - some term re-ordering occurs
     #  TODO - integer / double handling is not happening
     assert mathml_act == (
         '<?xml version="1.0" encoding="UTF-8"?>\n'
         '<math xmlns="http://www.w3.org/1998/Math/MathML" '
         'xmlns:sbml="http://www.sbml.org/sbml/level3/version2/core" '
         'xmlns:multi="http://www.sbml.org/sbml/level3/version1/multi/version1">\n'
-        '<apply><plus/><apply><power/>'
+        "<apply><plus/><apply><power/>"
         '<ci multi:speciesReference="ref_to_A">A</ci>'
         '<cn sbml:units="dimensionless">2.0</cn></apply>'
         '<apply><times/><cn sbml:units="dimensionless">2.0</cn>'
         '<ci multi:representationType="sum">A</ci></apply></apply></math>'
     )
-
```

