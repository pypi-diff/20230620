# Comparing `tmp/utilki-0.4.3.tar.gz` & `tmp/utilki-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utilki-0.4.3.tar", max compression
+gzip compressed data, was "utilki-0.4.4.tar", max compression
```

## Comparing `utilki-0.4.3.tar` & `utilki-0.4.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1064 2023-06-09 15:57:24.421282 utilki-0.4.3/README.md
--rw-r--r--   0        0        0      525 2023-06-09 15:57:24.421282 utilki-0.4.3/pyproject.toml
--rw-r--r--   0        0        0      269 2023-06-09 15:57:24.421282 utilki-0.4.3/utilki/__init__.py
--rw-r--r--   0        0        0     2184 2023-06-09 15:57:24.421282 utilki-0.4.3/utilki/cli.py
--rw-r--r--   0        0        0     5273 2023-06-09 15:57:24.421282 utilki-0.4.3/utilki/log_utils.py
--rw-r--r--   0        0        0     6437 2023-06-09 15:57:24.421282 utilki-0.4.3/utilki/task_mixin.py
--rw-r--r--   0        0        0     1659 1970-01-01 00:00:00.000000 utilki-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-20 13:42:18.372101 utilki-0.4.4/README.md
+-rw-r--r--   0        0        0      525 2023-06-20 13:42:18.372101 utilki-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0      269 2023-06-20 13:42:18.372101 utilki-0.4.4/utilki/__init__.py
+-rw-r--r--   0        0        0     2184 2023-06-20 13:42:18.372101 utilki-0.4.4/utilki/cli.py
+-rw-r--r--   0        0        0     5273 2023-06-20 13:42:18.372101 utilki-0.4.4/utilki/log_utils.py
+-rw-r--r--   0        0        0     6698 2023-06-20 13:42:18.372101 utilki-0.4.4/utilki/task_mixin.py
+-rw-r--r--   0        0        0     1659 1970-01-01 00:00:00.000000 utilki-0.4.4/PKG-INFO
```

### Comparing `utilki-0.4.3/README.md` & `utilki-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `utilki-0.4.3/pyproject.toml` & `utilki-0.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "utilki"
-version = "0.4.3"
+version = "0.4.4"
 description = "A collection of useful utilities"
 readme = "README.md"
 authors = ["Khaidar Bikmaev <khaidar@bikmaev.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.7"
 click = "^8.1.3"
```

### Comparing `utilki-0.4.3/utilki/cli.py` & `utilki-0.4.4/utilki/cli.py`

 * *Files identical despite different names*

### Comparing `utilki-0.4.3/utilki/log_utils.py` & `utilki-0.4.4/utilki/log_utils.py`

 * *Files identical despite different names*

### Comparing `utilki-0.4.3/utilki/task_mixin.py` & `utilki-0.4.4/utilki/task_mixin.py`

 * *Files 3% similar despite different names*

```diff
@@ -108,14 +108,21 @@
                 return value
         elif type_ in [int, str, float, bool]:
             if isinstance(value, type_):
                 return value
         else:
             raise TypeError("Invalid type")
 
+    def update(self, param_dict: Dict[str, Any]):
+        for param, value in param_dict.items():
+            if hasattr(self, param):
+                setattr(self, param, value)
+            else:
+                raise ValueError(f"Invalid parameter {param}")
+
 
 def parse_bool(param):
     if param in ["True", "true", True]:
         return True
     elif param in ["False", "false", False]:
         return False
     else:
```

### Comparing `utilki-0.4.3/PKG-INFO` & `utilki-0.4.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utilki
-Version: 0.4.3
+Version: 0.4.4
 Summary: A collection of useful utilities
 Author: Khaidar Bikmaev
 Author-email: khaidar@bikmaev.com
 Requires-Python: >=3.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

