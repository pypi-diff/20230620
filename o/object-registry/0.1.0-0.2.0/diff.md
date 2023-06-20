# Comparing `tmp/object_registry-0.1.0.tar.gz` & `tmp/object_registry-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "object_registry-0.1.0.tar", max compression
+gzip compressed data, was "object_registry-0.2.0.tar", max compression
```

## Comparing `object_registry-0.1.0.tar` & `object_registry-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    35093 2023-06-18 14:46:21.918955 object_registry-0.1.0/LICENSE
--rw-r--r--   0        0        0      618 2023-06-18 14:00:45.865151 object_registry-0.1.0/README.md
--rw-r--r--   0        0        0     1720 2023-06-19 15:18:40.336089 object_registry-0.1.0/object_registry/__init__.py
--rw-r--r--   0        0        0      459 2023-06-19 15:24:45.970521 object_registry-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1203 1970-01-01 00:00:00.000000 object_registry-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35093 2023-06-18 14:46:21.918955 object_registry-0.2.0/LICENSE
+-rw-r--r--   0        0        0      618 2023-06-18 14:00:45.865151 object_registry-0.2.0/README.md
+-rw-r--r--   0        0        0     1512 2023-06-20 00:07:13.544118 object_registry-0.2.0/object_registry/__init__.py
+-rw-r--r--   0        0        0      459 2023-06-19 23:49:21.403205 object_registry-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1203 1970-01-01 00:00:00.000000 object_registry-0.2.0/PKG-INFO
```

### Comparing `object_registry-0.1.0/LICENSE` & `object_registry-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `object_registry-0.1.0/README.md` & `object_registry-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `object_registry-0.1.0/object_registry/__init__.py` & `object_registry-0.2.0/object_registry/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,64 +1,58 @@
 from __future__ import annotations
 
 import weakref
 
 
-_registries: dict[type, dict[int, weakref.ReferenceType[ObjectRegistry]]] = {}
+_registered: dict[int, weakref.ReferenceType[ObjectRegistry]] = {}
 
 
 class ObjectRegistry:
     """
     Objects of the inheriting class are tracked in a registry.
 
     The registry stores weak references to objects,
     allowing objects to be garbage collected when
     they are no longer referenced elsewhere in the code.
     If an object is deleted or its reference becomes invalid,
     it is automatically unregistered from the registry.
     """
 
-    def __init_subclass__(cls) -> None:
-        """
-        Add class to registry to track its instantiated objects.
-        """
-        _registries[cls] = {}
-    
     def __new__(cls, *args, **kwargs) -> ObjectRegistry:
         """
         Register object upon creation.
         """
         obj = super().__new__(cls, *args, **kwargs)
-        _registries[cls][id(obj)] = weakref.ref(obj)
+        _registered[id(obj)] = weakref.ref(obj)
         return obj
 
     def __del__(self) -> None:
         """
         Unregister object upon deletion.
         """
         try:
-            del _registries[type(self)][id(self)]
+            del _registered[id(self)]
         except KeyError:
             pass
 
 
     @classmethod
     def from_id(cls, object_id: int, /) -> ObjectRegistry:
         """
         Get object by ID.
         """
         
         obj = None
 
-        if object_id in _registries[cls]:
+        if object_id in _registered:
             # Attempt to follow the weak reference.
-            obj = _registries[cls][object_id]()
+            obj = _registered[object_id]()
 
             if obj is None:
                 # If the reference has been invalidated,
                 # delete and unregister the stray object.
-                del _registries[cls][object_id]
+                del _registered[object_id]
 
         if obj is None:
             raise KeyError(f'No object by ID {object_id}.')
 
         return obj
```

### Comparing `object_registry-0.1.0/PKG-INFO` & `object_registry-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: object-registry
-Version: 0.1.0
+Version: 0.2.0
 Summary: Keep track of all instantiated objects of a class.
 Home-page: https://gitlab.com/deepadmax/object-registry
 License: GPL-3.0-or-later
 Author: Maximillian Strand
 Author-email: maxi@millian.se
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

