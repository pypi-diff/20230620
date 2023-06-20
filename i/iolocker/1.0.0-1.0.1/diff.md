# Comparing `tmp/iolocker-1.0.0.tar.gz` & `tmp/iolocker-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iolocker-1.0.0.tar", last modified: Mon Jun 19 17:22:44 2023, max compression
+gzip compressed data, was "iolocker-1.0.1.tar", last modified: Tue Jun 20 10:39:58 2023, max compression
```

## Comparing `iolocker-1.0.0.tar` & `iolocker-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 17:22:44.123188 iolocker-1.0.0/
--rw-rw-rw-   0        0        0     1090 2023-06-16 15:15:34.000000 iolocker-1.0.0/LICENSE
--rw-rw-rw-   0        0        0       14 2022-10-24 07:53:37.000000 iolocker-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1595 2023-06-19 17:22:44.123188 iolocker-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      799 2023-06-19 17:02:14.000000 iolocker-1.0.0/README.md
--rw-rw-rw-   0        0        0       93 2022-08-10 18:07:14.000000 iolocker-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0     1024 2023-06-19 17:22:44.124208 iolocker-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-19 17:22:44.108357 iolocker-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-19 17:22:44.118201 iolocker-1.0.0/src/iolocker/
--rw-rw-rw-   0        0        0      395 2023-06-19 09:49:23.000000 iolocker-1.0.0/src/iolocker/__init__.py
--rw-rw-rw-   0        0        0      877 2023-06-19 10:19:26.000000 iolocker-1.0.0/src/iolocker/constants.py
--rw-rw-rw-   0        0        0     3897 2023-06-19 10:19:26.000000 iolocker-1.0.0/src/iolocker/core.py
--rw-rw-rw-   0        0        0      816 2023-06-19 09:49:23.000000 iolocker-1.0.0/src/iolocker/exceptions.py
--rw-rw-rw-   0        0        0     2426 2023-06-19 16:00:24.000000 iolocker-1.0.0/src/iolocker/handlers.py
-drwxrwxrwx   0        0        0        0 2023-06-19 17:22:44.123188 iolocker-1.0.0/src/iolocker.egg-info/
--rw-rw-rw-   0        0        0     1595 2023-06-19 17:22:44.000000 iolocker-1.0.0/src/iolocker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      392 2023-06-19 17:22:44.000000 iolocker-1.0.0/src/iolocker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 17:22:44.000000 iolocker-1.0.0/src/iolocker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-19 17:22:43.000000 iolocker-1.0.0/src/iolocker.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       46 2023-06-19 17:22:44.000000 iolocker-1.0.0/src/iolocker.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-19 17:22:44.000000 iolocker-1.0.0/src/iolocker.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 10:39:58.027455 iolocker-1.0.1/
+-rw-rw-rw-   0        0        0     1090 2023-06-16 15:15:34.000000 iolocker-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0       14 2022-10-24 07:53:37.000000 iolocker-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1595 2023-06-20 10:39:58.027455 iolocker-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      799 2023-06-19 17:02:14.000000 iolocker-1.0.1/README.md
+-rw-rw-rw-   0        0        0       93 2022-08-10 18:07:14.000000 iolocker-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1024 2023-06-20 10:39:58.043077 iolocker-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-20 10:39:58.011833 iolocker-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-20 10:39:58.027455 iolocker-1.0.1/src/iolocker/
+-rw-rw-rw-   0        0        0      395 2023-06-19 09:49:23.000000 iolocker-1.0.1/src/iolocker/__init__.py
+-rw-rw-rw-   0        0        0      877 2023-06-19 10:19:26.000000 iolocker-1.0.1/src/iolocker/constants.py
+-rw-rw-rw-   0        0        0     3897 2023-06-19 10:19:26.000000 iolocker-1.0.1/src/iolocker/core.py
+-rw-rw-rw-   0        0        0      816 2023-06-19 09:49:23.000000 iolocker-1.0.1/src/iolocker/exceptions.py
+-rw-rw-rw-   0        0        0     2263 2023-06-20 09:28:55.000000 iolocker-1.0.1/src/iolocker/handlers.py
+drwxrwxrwx   0        0        0        0 2023-06-20 10:39:58.027455 iolocker-1.0.1/src/iolocker.egg-info/
+-rw-rw-rw-   0        0        0     1595 2023-06-20 10:39:57.000000 iolocker-1.0.1/src/iolocker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      392 2023-06-20 10:39:58.000000 iolocker-1.0.1/src/iolocker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 10:39:57.000000 iolocker-1.0.1/src/iolocker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-19 17:22:43.000000 iolocker-1.0.1/src/iolocker.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       46 2023-06-20 10:39:57.000000 iolocker-1.0.1/src/iolocker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-20 10:39:57.000000 iolocker-1.0.1/src/iolocker.egg-info/top_level.txt
```

### Comparing `iolocker-1.0.0/LICENSE` & `iolocker-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iolocker-1.0.0/PKG-INFO` & `iolocker-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iolocker
-Version: 1.0.0
+Version: 1.0.1
 Summary: Simple file locker.
 Home-page: https://github.com/ClaudiuDrug/iolocker
 Author: Claudiu DRUG
 Author-email: claudiu.drug@outlook.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/ClaudiuDrug/iolocker/issues
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `iolocker-1.0.0/README.md` & `iolocker-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `iolocker-1.0.0/setup.cfg` & `iolocker-1.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2069 6f6c 6f63 6b65 720d 0a76 6572   = iolocker..ver
-00000020: 7369 6f6e 203d 2031 2e30 2e30 0d0a 6175  sion = 1.0.0..au
+00000020: 7369 6f6e 203d 2031 2e30 2e31 0d0a 6175  sion = 1.0.1..au
 00000030: 7468 6f72 203d 2043 6c61 7564 6975 2044  thor = Claudiu D
 00000040: 5255 470d 0a61 7574 686f 725f 656d 6169  RUG..author_emai
 00000050: 6c20 3d20 636c 6175 6469 752e 6472 7567  l = claudiu.drug
 00000060: 406f 7574 6c6f 6f6b 2e63 6f6d 0d0a 6c69  @outlook.com..li
 00000070: 6365 6e73 6520 3d20 4d49 5420 4c69 6365  cense = MIT Lice
 00000080: 6e73 650d 0a64 6573 6372 6970 7469 6f6e  nse..description
 00000090: 203d 2053 696d 706c 6520 6669 6c65 206c   = Simple file l
```

### Comparing `iolocker-1.0.0/src/iolocker/constants.py` & `iolocker-1.0.1/src/iolocker/constants.py`

 * *Files identical despite different names*

### Comparing `iolocker-1.0.0/src/iolocker/core.py` & `iolocker-1.0.1/src/iolocker/core.py`

 * *Files identical despite different names*

### Comparing `iolocker-1.0.0/src/iolocker/exceptions.py` & `iolocker-1.0.1/src/iolocker/exceptions.py`

 * *Files identical despite different names*

### Comparing `iolocker-1.0.0/src/iolocker/handlers.py` & `iolocker-1.0.1/src/iolocker/handlers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,64 +1,60 @@
 # -*- coding: UTF-8 -*-
 
 from abc import ABC, abstractmethod
-from typing import IO
+from typing import Union, IO, TextIO, BinaryIO
 
 from .constants import LOCK
 from .core import lock, unlock
 from .exceptions import LockFlagsError
 
 __all__ = ["Handler", "FileLocker"]
 
+Handle = Union[IO, TextIO, BinaryIO]
+
 
 class Handler(ABC):
     """Base abstract handler."""
 
     def __init__(self, *args, **kwargs):
         self._args, self._kwargs = args, kwargs
 
-    def __enter__(self) -> IO:
+    def __enter__(self) -> Handle:
         if not hasattr(self, "_handle"):
-            self._handle: IO = self.acquire(*self._args, **self._kwargs)
+            self._handle: Handle = self.acquire(*self._args, **self._kwargs)
         return self._handle
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         if hasattr(self, "_handle"):
             self.release(self._handle)
             del self._handle
 
     def __delete__(self, instance):
         instance.release()
 
     @abstractmethod
     def acquire(self, *args, **kwargs):
-        raise NotImplementedError(
-            f"Method 'acquire()' was not implemented "
-            f"in child class {self.__class__.__name__}!"
-        )
+        raise NotImplementedError
 
     @abstractmethod
     def release(self, *args, **kwargs):
-        raise NotImplementedError(
-            f"Method 'release()' was not implemented "
-            f"in child class {self.__class__.__name__}!"
-        )
+        raise NotImplementedError
 
 
 class FileLocker(Handler):
     """File locker."""
 
     _flags: dict = {
         "w": LOCK.EX,
         "a": LOCK.EX,
         "x": LOCK.EX,
         "r": LOCK.SH,
     }
 
-    def acquire(self, handle: IO, flags: LOCK = None) -> IO:
+    def acquire(self, handle: Handle, flags: LOCK = None) -> Handle:
         """
         Acquire a lock on the given `handle`.
         If `flags` are not provided it will try to guess
         them by reading the handle's operating mode.
 
         :param handle: The file handle.
         :param flags: The flags to be used to lock the handle.
@@ -71,16 +67,16 @@
 
         elif (mode == "w") and (flags in (LOCK.SH | LOCK.NB)):
             raise LockFlagsError(f"Wrong flags used on this operating mode of the handle (`{mode}`)!")
 
         lock(handle, flags)
         return handle
 
-    def release(self, handle: IO):
+    def release(self, handle: Handle):
         """Unlock the file handle."""
         unlock(handle)
 
     @staticmethod
-    def _get_mode(handle: IO) -> str:
+    def _get_mode(handle: Handle) -> str:
         """Return the handle's operating mode."""
         mode = handle.mode
         return mode.strip("tb+")
```

### Comparing `iolocker-1.0.0/src/iolocker.egg-info/PKG-INFO` & `iolocker-1.0.1/src/iolocker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iolocker
-Version: 1.0.0
+Version: 1.0.1
 Summary: Simple file locker.
 Home-page: https://github.com/ClaudiuDrug/iolocker
 Author: Claudiu DRUG
 Author-email: claudiu.drug@outlook.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/ClaudiuDrug/iolocker/issues
 Classifier: Programming Language :: Python :: 3.7
```

