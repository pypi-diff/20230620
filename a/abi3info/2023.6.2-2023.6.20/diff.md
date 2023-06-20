# Comparing `tmp/abi3info-2023.6.2.tar.gz` & `tmp/abi3info-2023.6.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abi3info-2023.6.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "abi3info-2023.6.20.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `abi3info-2023.6.2.tar` & `abi3info-2023.6.20.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1109 2023-06-02 22:35:00.674314 abi3info-2023.6.2/LICENSE
--rw-r--r--   0        0        0     1915 2023-06-02 22:35:00.674314 abi3info-2023.6.2/README.md
--rw-r--r--   0        0        0     1038 2023-06-02 22:35:00.674314 abi3info-2023.6.2/abi3info/__init__.py
--rw-r--r--   0        0        0   190471 2023-06-02 22:35:00.674314 abi3info-2023.6.2/abi3info/_internal.py
--rw-r--r--   0        0        0     7791 2023-06-02 22:35:00.674314 abi3info-2023.6.2/abi3info/models.py
--rw-r--r--   0        0        0     1885 2023-06-02 22:35:00.674314 abi3info-2023.6.2/pyproject.toml
--rw-r--r--   0        0        0     3461 1970-01-01 00:00:00.000000 abi3info-2023.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1109 2023-06-20 13:56:23.663293 abi3info-2023.6.20/LICENSE
+-rw-r--r--   0        0        0     1915 2023-06-20 13:56:23.663293 abi3info-2023.6.20/README.md
+-rw-r--r--   0        0        0     1038 2023-06-20 13:56:23.663293 abi3info-2023.6.20/abi3info/__init__.py
+-rw-r--r--   0        0        0   189917 2023-06-20 13:56:23.663293 abi3info-2023.6.20/abi3info/_internal.py
+-rw-r--r--   0        0        0     7791 2023-06-20 13:56:23.663293 abi3info-2023.6.20/abi3info/models.py
+-rw-r--r--   0        0        0     1885 2023-06-20 13:56:23.663293 abi3info-2023.6.20/pyproject.toml
+-rw-r--r--   0        0        0     3462 1970-01-01 00:00:00.000000 abi3info-2023.6.20/PKG-INFO
```

### Comparing `abi3info-2023.6.2/LICENSE` & `abi3info-2023.6.20/LICENSE`

 * *Files identical despite different names*

### Comparing `abi3info-2023.6.2/README.md` & `abi3info-2023.6.20/README.md`

 * *Files identical despite different names*

### Comparing `abi3info-2023.6.2/abi3info/__init__.py` & `abi3info-2023.6.20/abi3info/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     Function,
     Macro,
     Struct,
     Symbol,
     Typedef,
 )
 
-__version__ = "2023.06.02"
+__version__ = "2023.06.20"
 """
 The current version of abi3info.
 """
 
 DATAS: Final[dict[Symbol, Data]] = _DATAS
 """
 Data object members of the limited API and stable ABI.
```

### Comparing `abi3info-2023.6.2/abi3info/_internal.py` & `abi3info-2023.6.20/abi3info/_internal.py`

 * *Files 1% similar despite different names*

```diff
@@ -4433,33 +4433,19 @@
     ),
     Symbol(name="PyType_GetTypeDataSize"): Function(
         symbol=Symbol(name="PyType_GetTypeDataSize"),
         added=PyVersion(major=3, minor=12),
         ifdef=None,
         abi_only=False,
     ),
-    Symbol(name="_Py_IncRefTotal_DO_NOT_USE_THIS"): Function(
-        symbol=Symbol(name="_Py_IncRefTotal_DO_NOT_USE_THIS"),
-        added=PyVersion(major=3, minor=12),
-        ifdef=FeatureMacro(
-            name="Py_REF_DEBUG",
-            doc="when Python is compiled in debug mode (with Py_REF_DEBUG)",
-            windows="maybe",
-        ),
-        abi_only=True,
-    ),
-    Symbol(name="_Py_DecRefTotal_DO_NOT_USE_THIS"): Function(
-        symbol=Symbol(name="_Py_DecRefTotal_DO_NOT_USE_THIS"),
-        added=PyVersion(major=3, minor=12),
-        ifdef=FeatureMacro(
-            name="Py_REF_DEBUG",
-            doc="when Python is compiled in debug mode (with Py_REF_DEBUG)",
-            windows="maybe",
-        ),
-        abi_only=True,
+    Symbol(name="PyImport_AddModuleRef"): Function(
+        symbol=Symbol(name="PyImport_AddModuleRef"),
+        added=PyVersion(major=3, minor=13),
+        ifdef=None,
+        abi_only=False,
     ),
 }
 _MACROS: Final[dict[str, Macro]] = {
     "Py_tp_dealloc": Macro(name="Py_tp_dealloc", added=PyVersion(major=3, minor=2)),
     "Py_tp_getattr": Macro(name="Py_tp_getattr", added=PyVersion(major=3, minor=2)),
     "Py_tp_setattr": Macro(name="Py_tp_setattr", added=PyVersion(major=3, minor=2)),
     "Py_tp_repr": Macro(name="Py_tp_repr", added=PyVersion(major=3, minor=2)),
```

### Comparing `abi3info-2023.6.2/abi3info/models.py` & `abi3info-2023.6.20/abi3info/models.py`

 * *Files identical despite different names*

### Comparing `abi3info-2023.6.2/pyproject.toml` & `abi3info-2023.6.20/pyproject.toml`

 * *Files identical despite different names*

### Comparing `abi3info-2023.6.2/PKG-INFO` & `abi3info-2023.6.20/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abi3info
-Version: 2023.6.2
+Version: 2023.6.20
 Summary: A library for abi3 and other CPython API information
 Author-email: William Woodruff <william@yossarian.net>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
```

