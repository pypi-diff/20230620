# Comparing `tmp/vsexprtools-1.4.5.tar.gz` & `tmp/vsexprtools-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsexprtools-1.4.5.tar", last modified: Mon Jun  5 13:58:53 2023, max compression
+gzip compressed data, was "vsexprtools-1.4.6.tar", last modified: Tue Jun 20 14:31:32 2023, max compression
```

## Comparing `vsexprtools-1.4.5.tar` & `vsexprtools-1.4.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:58:53.353233 vsexprtools-1.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-05 13:58:30.000000 vsexprtools-1.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-05 13:58:53.353233 vsexprtools-1.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-05 13:58:30.000000 vsexprtools-1.4.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-05 13:58:53.353233 vsexprtools-1.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-05 13:58:30.000000 vsexprtools-1.4.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:58:53.353233 vsexprtools-1.4.5/vsexprtools/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-05 13:58:30.000000 vsexprtools-1.4.5/vsexprtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-05 13:58:30.000000 vsexprtools-1.4.5/vsexprtools/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    11313 2023-06-05 13:58:30.000000 vsexprtools-1.4.5/vsexprtools/exprop.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-06-05 13:58:30.000000 vsexprtools-1.4.5/vsexprtools/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-06-05 13:58:30.000000 vsexprtools-1.4.5/vsexprtools/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-06-05 13:58:30.000000 vsexprtools-1.4.5/vsexprtools/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-05 13:58:30.000000 vsexprtools-1.4.5/vsexprtools/polyfills.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 13:58:30.000000 vsexprtools-1.4.5/vsexprtools/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8260 2023-06-05 13:58:30.000000 vsexprtools-1.4.5/vsexprtools/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11311 2023-06-05 13:58:30.000000 vsexprtools-1.4.5/vsexprtools/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:58:53.353233 vsexprtools-1.4.5/vsexprtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-05 13:58:53.000000 vsexprtools-1.4.5/vsexprtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-05 13:58:53.000000 vsexprtools-1.4.5/vsexprtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 13:58:53.000000 vsexprtools-1.4.5/vsexprtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-05 13:58:53.000000 vsexprtools-1.4.5/vsexprtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-05 13:58:53.000000 vsexprtools-1.4.5/vsexprtools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:31:32.796507 vsexprtools-1.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-20 14:31:00.000000 vsexprtools-1.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-20 14:31:32.796507 vsexprtools-1.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-20 14:31:00.000000 vsexprtools-1.4.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-20 14:31:32.796507 vsexprtools-1.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-20 14:31:00.000000 vsexprtools-1.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:31:32.792507 vsexprtools-1.4.6/vsexprtools/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-20 14:31:00.000000 vsexprtools-1.4.6/vsexprtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-20 14:31:00.000000 vsexprtools-1.4.6/vsexprtools/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11313 2023-06-20 14:31:00.000000 vsexprtools-1.4.6/vsexprtools/exprop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-06-20 14:31:00.000000 vsexprtools-1.4.6/vsexprtools/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-06-20 14:31:00.000000 vsexprtools-1.4.6/vsexprtools/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-06-20 14:31:00.000000 vsexprtools-1.4.6/vsexprtools/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-20 14:31:00.000000 vsexprtools-1.4.6/vsexprtools/polyfills.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:31:00.000000 vsexprtools-1.4.6/vsexprtools/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-06-20 14:31:00.000000 vsexprtools-1.4.6/vsexprtools/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11311 2023-06-20 14:31:00.000000 vsexprtools-1.4.6/vsexprtools/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:31:32.796507 vsexprtools-1.4.6/vsexprtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-20 14:31:32.000000 vsexprtools-1.4.6/vsexprtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-20 14:31:32.000000 vsexprtools-1.4.6/vsexprtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 14:31:32.000000 vsexprtools-1.4.6/vsexprtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-20 14:31:32.000000 vsexprtools-1.4.6/vsexprtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-20 14:31:32.000000 vsexprtools-1.4.6/vsexprtools.egg-info/top_level.txt
```

### Comparing `vsexprtools-1.4.5/LICENSE` & `vsexprtools-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vsexprtools-1.4.5/PKG-INFO` & `vsexprtools-1.4.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsexprtools
-Version: 1.4.5
+Version: 1.4.6
 Summary: VapourSynth functions and helpers for writing RPN expressions.
 Author: Setsugen no ao
 Author-email: setsugen@setsugen.dev
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-exprtools
 Project-URL: Documentation, https://vsexprtools.encode.moe/en/latest/
```

### Comparing `vsexprtools-1.4.5/setup.cfg` & `vsexprtools-1.4.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `vsexprtools-1.4.5/setup.py` & `vsexprtools-1.4.6/setup.py`

 * *Files identical despite different names*

### Comparing `vsexprtools-1.4.5/vsexprtools/exprop.py` & `vsexprtools-1.4.6/vsexprtools/exprop.py`

 * *Files identical despite different names*

### Comparing `vsexprtools-1.4.5/vsexprtools/funcs.py` & `vsexprtools-1.4.6/vsexprtools/funcs.py`

 * *Files identical despite different names*

### Comparing `vsexprtools-1.4.5/vsexprtools/manager.py` & `vsexprtools-1.4.6/vsexprtools/manager.py`

 * *Files identical despite different names*

### Comparing `vsexprtools-1.4.5/vsexprtools/operators.py` & `vsexprtools-1.4.6/vsexprtools/operators.py`

 * *Files identical despite different names*

### Comparing `vsexprtools-1.4.5/vsexprtools/polyfills.py` & `vsexprtools-1.4.6/vsexprtools/polyfills.py`

 * *Files identical despite different names*

### Comparing `vsexprtools-1.4.5/vsexprtools/util.py` & `vsexprtools-1.4.6/vsexprtools/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,27 @@
     'ExprVars', 'ExprVarsT', 'ExprVarRangeT', 'bitdepth_aware_tokenize_expr',
     # VS helpers
     'norm_expr_planes'
 ]
 
 
 class _complexpr_available:
+    @property
+    def fp16(self) -> bool:
+        from .funcs import expr_func
+
+        if not hasattr(self, '_fp16_available'):
+            try:
+                expr_func(core.std.BlankClip(format=vs.GRAYH), 'x dup *')
+                self._fp16_available = True
+            except Exception:
+                self._fp16_available = False
+
+        return self._fp16_available
+
     def __bool__(self) -> bool:
         try:
             return bool(core.akarin.Expr)
         except AttributeError:
             ...
 
         return False
```

### Comparing `vsexprtools-1.4.5/vsexprtools/variables.py` & `vsexprtools-1.4.6/vsexprtools/variables.py`

 * *Files identical despite different names*

### Comparing `vsexprtools-1.4.5/vsexprtools.egg-info/PKG-INFO` & `vsexprtools-1.4.6/vsexprtools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsexprtools
-Version: 1.4.5
+Version: 1.4.6
 Summary: VapourSynth functions and helpers for writing RPN expressions.
 Author: Setsugen no ao
 Author-email: setsugen@setsugen.dev
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-exprtools
 Project-URL: Documentation, https://vsexprtools.encode.moe/en/latest/
```

