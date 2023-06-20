# Comparing `tmp/vsdeband-1.0.1.tar.gz` & `tmp/vsdeband-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsdeband-1.0.1.tar", last modified: Mon Jun  5 14:34:30 2023, max compression
+gzip compressed data, was "vsdeband-1.0.2.tar", last modified: Tue Jun 20 15:28:47 2023, max compression
```

## Comparing `vsdeband-1.0.1.tar` & `vsdeband-1.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:34:30.341065 vsdeband-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-05 14:34:04.000000 vsdeband-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-05 14:34:30.341065 vsdeband-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-05 14:34:04.000000 vsdeband-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-05 14:34:30.341065 vsdeband-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-05 14:34:04.000000 vsdeband-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:34:30.341065 vsdeband-1.0.1/vsdeband/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-05 14:34:04.000000 vsdeband-1.0.1/vsdeband/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-05 14:34:04.000000 vsdeband-1.0.1/vsdeband/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-05 14:34:04.000000 vsdeband-1.0.1/vsdeband/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-06-05 14:34:04.000000 vsdeband-1.0.1/vsdeband/f3kdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-06-05 14:34:04.000000 vsdeband-1.0.1/vsdeband/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-06-05 14:34:04.000000 vsdeband-1.0.1/vsdeband/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-05 14:34:04.000000 vsdeband-1.0.1/vsdeband/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)    23962 2023-06-05 14:34:04.000000 vsdeband-1.0.1/vsdeband/noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-06-05 14:34:04.000000 vsdeband-1.0.1/vsdeband/placebo.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 14:34:04.000000 vsdeband-1.0.1/vsdeband/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-05 14:34:04.000000 vsdeband-1.0.1/vsdeband/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:34:30.341065 vsdeband-1.0.1/vsdeband.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-05 14:34:30.000000 vsdeband-1.0.1/vsdeband.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-05 14:34:30.000000 vsdeband-1.0.1/vsdeband.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 14:34:30.000000 vsdeband-1.0.1/vsdeband.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-05 14:34:30.000000 vsdeband-1.0.1/vsdeband.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-05 14:34:30.000000 vsdeband-1.0.1/vsdeband.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:28:47.045302 vsdeband-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-20 15:28:21.000000 vsdeband-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-20 15:28:47.045302 vsdeband-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-20 15:28:21.000000 vsdeband-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-20 15:28:47.045302 vsdeband-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-20 15:28:21.000000 vsdeband-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:28:47.041302 vsdeband-1.0.2/vsdeband/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-20 15:28:21.000000 vsdeband-1.0.2/vsdeband/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-20 15:28:21.000000 vsdeband-1.0.2/vsdeband/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-20 15:28:21.000000 vsdeband-1.0.2/vsdeband/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-06-20 15:28:21.000000 vsdeband-1.0.2/vsdeband/f3kdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-06-20 15:28:21.000000 vsdeband-1.0.2/vsdeband/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-06-20 15:28:21.000000 vsdeband-1.0.2/vsdeband/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-20 15:28:21.000000 vsdeband-1.0.2/vsdeband/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23962 2023-06-20 15:28:21.000000 vsdeband-1.0.2/vsdeband/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-06-20 15:28:21.000000 vsdeband-1.0.2/vsdeband/placebo.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:28:21.000000 vsdeband-1.0.2/vsdeband/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-20 15:28:21.000000 vsdeband-1.0.2/vsdeband/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:28:47.045302 vsdeband-1.0.2/vsdeband.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-20 15:28:47.000000 vsdeband-1.0.2/vsdeband.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-20 15:28:47.000000 vsdeband-1.0.2/vsdeband.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:28:47.000000 vsdeband-1.0.2/vsdeband.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-20 15:28:47.000000 vsdeband-1.0.2/vsdeband.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 15:28:47.000000 vsdeband-1.0.2/vsdeband.egg-info/top_level.txt
```

### Comparing `vsdeband-1.0.1/LICENSE` & `vsdeband-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vsdeband-1.0.1/PKG-INFO` & `vsdeband-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsdeband
-Version: 1.0.1
+Version: 1.0.2
 Summary: VapourSynth Debanding Functions Collection
 Author: Irrational Encoding Wizardry
 Author-email: wizards@encode.moe
 Maintainer: Irrational Encoding Wizardry
 Maintainer-email: wizards@encode.moe
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-deband
 Project-URL: Documentation, https://vsdeband.encode.moe/en/latest/
```

### Comparing `vsdeband-1.0.1/setup.cfg` & `vsdeband-1.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `vsdeband-1.0.1/setup.py` & `vsdeband-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `vsdeband-1.0.1/vsdeband/f3kdb.py` & `vsdeband-1.0.2/vsdeband/f3kdb.py`

 * *Files identical despite different names*

### Comparing `vsdeband-1.0.1/vsdeband/filters.py` & `vsdeband-1.0.2/vsdeband/filters.py`

 * *Files identical despite different names*

### Comparing `vsdeband-1.0.1/vsdeband/funcs.py` & `vsdeband-1.0.2/vsdeband/funcs.py`

 * *Files identical despite different names*

### Comparing `vsdeband-1.0.1/vsdeband/mask.py` & `vsdeband-1.0.2/vsdeband/mask.py`

 * *Files identical despite different names*

### Comparing `vsdeband-1.0.1/vsdeband/noise.py` & `vsdeband-1.0.2/vsdeband/noise.py`

 * *Files identical despite different names*

### Comparing `vsdeband-1.0.1/vsdeband/placebo.py` & `vsdeband-1.0.2/vsdeband/placebo.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     iterations: int | None = None
 
     dither: PlaceboDither | None = None
 
     @inject_self
     def deband(  # type: ignore[override]
         self, clip: vs.VideoNode, radius: float = 16.0, thr: float | list[float] = 4.0,
-        iterations: int = 1, grain: float | list[float] = 0.0, dither: PlaceboDither = PlaceboDither.DEFAULT
+        iterations: int = 4, grain: float | list[float] = 0.0, dither: PlaceboDither = PlaceboDither.DEFAULT
     ) -> vs.VideoNode:
         """
         Main deband function, wrapper for `placebo.Deband <https:/github.com/Lypheo/vs-placebo#vs-placebo>`_
 
         :param clip:            Source clip
         :param radius:          The debanding filter's initial radius.
                                 The radius increases linearly for each iteration.
```

### Comparing `vsdeband-1.0.1/vsdeband.egg-info/PKG-INFO` & `vsdeband-1.0.2/vsdeband.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsdeband
-Version: 1.0.1
+Version: 1.0.2
 Summary: VapourSynth Debanding Functions Collection
 Author: Irrational Encoding Wizardry
 Author-email: wizards@encode.moe
 Maintainer: Irrational Encoding Wizardry
 Maintainer-email: wizards@encode.moe
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-deband
 Project-URL: Documentation, https://vsdeband.encode.moe/en/latest/
```

