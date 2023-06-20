# Comparing `tmp/pydita_ast-0.1.0.tar.gz` & `tmp/pydita_ast-0.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydita_ast-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pydita_ast-0.1.dev0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pydita_ast-0.1.0.tar` & `pydita_ast-0.1.dev0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1089 2023-06-20 17:07:07.385641 pydita_ast-0.1.0/LICENSE
--rw-r--r--   0        0        0     3150 2023-06-20 17:07:07.385641 pydita_ast-0.1.0/README.rst
--rw-r--r--   0        0        0     2036 2023-06-20 17:07:07.389641 pydita_ast-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      286 2023-06-20 17:07:07.389641 pydita_ast-0.1.0/src/pydita_ast/__init__.py
--rw-r--r--   0        0        0    75667 2023-06-20 17:07:07.389641 pydita_ast-0.1.0/src/pydita_ast/ast_tree.py
--rw-r--r--   0        0        0     5289 2023-06-20 17:07:07.389641 pydita_ast-0.1.0/src/pydita_ast/custom_functions.py
--rw-r--r--   0        0        0     4726 2023-06-20 17:07:07.389641 pydita_ast-0.1.0/src/pydita_ast/directory_format.py
--rw-r--r--   0        0        0    10341 2023-06-20 17:07:07.389641 pydita_ast-0.1.0/src/pydita_ast/load_xml_doc.py
--rw-r--r--   0        0        0     1726 2023-06-20 17:07:07.389641 pydita_ast-0.1.0/src/pydita_ast/version_variables.py
--rw-r--r--   0        0        0    11698 2023-06-20 17:07:07.389641 pydita_ast-0.1.0/src/pydita_ast/writer.py
--rw-r--r--   0        0        0     5292 1970-01-01 00:00:00.000000 pydita_ast-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-06-20 14:52:54.879382 pydita_ast-0.1.dev0/LICENSE
+-rw-r--r--   0        0        0     3150 2023-06-20 14:52:54.879382 pydita_ast-0.1.dev0/README.rst
+-rw-r--r--   0        0        0     2039 2023-06-20 14:52:54.879382 pydita_ast-0.1.dev0/pyproject.toml
+-rw-r--r--   0        0        0      286 2023-06-20 14:52:54.879382 pydita_ast-0.1.dev0/src/pydita_ast/__init__.py
+-rw-r--r--   0        0        0    75667 2023-06-20 14:52:54.879382 pydita_ast-0.1.dev0/src/pydita_ast/ast_tree.py
+-rw-r--r--   0        0        0     5289 2023-06-20 14:52:54.879382 pydita_ast-0.1.dev0/src/pydita_ast/custom_functions.py
+-rw-r--r--   0        0        0     4726 2023-06-20 14:52:54.879382 pydita_ast-0.1.dev0/src/pydita_ast/directory_format.py
+-rw-r--r--   0        0        0    10341 2023-06-20 14:52:54.879382 pydita_ast-0.1.dev0/src/pydita_ast/load_xml_doc.py
+-rw-r--r--   0        0        0     1726 2023-06-20 14:52:54.879382 pydita_ast-0.1.dev0/src/pydita_ast/version_variables.py
+-rw-r--r--   0        0        0    11698 2023-06-20 14:52:54.879382 pydita_ast-0.1.dev0/src/pydita_ast/writer.py
+-rw-r--r--   0        0        0     5295 1970-01-01 00:00:00.000000 pydita_ast-0.1.dev0/PKG-INFO
```

### Comparing `pydita_ast-0.1.0/LICENSE` & `pydita_ast-0.1.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydita_ast-0.1.0/README.rst` & `pydita_ast-0.1.dev0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 Getting started
 ---------------
 
 Install the ``pydita-ast`` package with:
 
 .. code:: bash
 
-    python -m pip install pydita-ast
+    python -m pip install pydita_ast
 
 
 It is recommended to organize the XML documentation as follow:
 
 .. image:: ./doc/source/user_guide/images/diags/graphviz-diag_directory.png
    :width: 450
    :align: center
```

### Comparing `pydita_ast-0.1.0/pyproject.toml` & `pydita_ast-0.1.dev0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 # Check https://flit.readthedocs.io/en/latest/pyproject_toml.html for all available sections
-name = "pydita-ast"
-version = "0.1.0"
+name = "pydita_ast"
+version = "0.1.dev0"
 description = "PyDita AST converter."
 readme = "README.rst"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 authors = [
     {name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"},
 ]
```

### Comparing `pydita_ast-0.1.0/src/pydita_ast/ast_tree.py` & `pydita_ast-0.1.dev0/src/pydita_ast/ast_tree.py`

 * *Files identical despite different names*

### Comparing `pydita_ast-0.1.0/src/pydita_ast/custom_functions.py` & `pydita_ast-0.1.dev0/src/pydita_ast/custom_functions.py`

 * *Files identical despite different names*

### Comparing `pydita_ast-0.1.0/src/pydita_ast/directory_format.py` & `pydita_ast-0.1.dev0/src/pydita_ast/directory_format.py`

 * *Files identical despite different names*

### Comparing `pydita_ast-0.1.0/src/pydita_ast/load_xml_doc.py` & `pydita_ast-0.1.dev0/src/pydita_ast/load_xml_doc.py`

 * *Files identical despite different names*

### Comparing `pydita_ast-0.1.0/src/pydita_ast/version_variables.py` & `pydita_ast-0.1.dev0/src/pydita_ast/version_variables.py`

 * *Files identical despite different names*

### Comparing `pydita_ast-0.1.0/src/pydita_ast/writer.py` & `pydita_ast-0.1.dev0/src/pydita_ast/writer.py`

 * *Files identical despite different names*

### Comparing `pydita_ast-0.1.0/PKG-INFO` & `pydita_ast-0.1.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pydita-ast
-Version: 0.1.0
+Name: pydita_ast
+Version: 0.1.dev0
 Summary: PyDita AST converter.
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: PyAnsys developers <pyansys.maintainers@ansys.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -92,15 +92,15 @@
 Getting started
 ---------------
 
 Install the ``pydita-ast`` package with:
 
 .. code:: bash
 
-    python -m pip install pydita-ast
+    python -m pip install pydita_ast
 
 
 It is recommended to organize the XML documentation as follow:
 
 .. image:: ./doc/source/user_guide/images/diags/graphviz-diag_directory.png
    :width: 450
    :align: center
```

