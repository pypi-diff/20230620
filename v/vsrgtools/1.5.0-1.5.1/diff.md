# Comparing `tmp/vsrgtools-1.5.0.tar.gz` & `tmp/vsrgtools-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsrgtools-1.5.0.tar", last modified: Mon Jun  5 14:00:51 2023, max compression
+gzip compressed data, was "vsrgtools-1.5.1.tar", last modified: Tue Jun 20 14:31:05 2023, max compression
```

## Comparing `vsrgtools-1.5.0.tar` & `vsrgtools-1.5.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:00:51.233498 vsrgtools-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-05 14:00:30.000000 vsrgtools-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-05 14:00:51.233498 vsrgtools-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-05 14:00:30.000000 vsrgtools-1.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-05 14:00:51.233498 vsrgtools-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-05 14:00:30.000000 vsrgtools-1.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:00:51.233498 vsrgtools-1.5.0/vsrgtools/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-05 14:00:30.000000 vsrgtools-1.5.0/vsrgtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-05 14:00:30.000000 vsrgtools-1.5.0/vsrgtools/_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:00:51.233498 vsrgtools-1.5.0/vsrgtools/aka_expr/
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-06-05 14:00:30.000000 vsrgtools-1.5.0/vsrgtools/aka_expr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-06-05 14:00:30.000000 vsrgtools-1.5.0/vsrgtools/aka_expr/_rg.py
--rw-r--r--   0 runner    (1001) docker     (123)    14266 2023-06-05 14:00:30.000000 vsrgtools-1.5.0/vsrgtools/aka_expr/_rp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-06-05 14:00:30.000000 vsrgtools-1.5.0/vsrgtools/bilateral.cu
--rw-r--r--   0 runner    (1001) docker     (123)    14017 2023-06-05 14:00:30.000000 vsrgtools-1.5.0/vsrgtools/blur.py
--rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-06-05 14:00:30.000000 vsrgtools-1.5.0/vsrgtools/contra.py
--rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-06-05 14:00:30.000000 vsrgtools-1.5.0/vsrgtools/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-06-05 14:00:30.000000 vsrgtools-1.5.0/vsrgtools/freqs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-05 14:00:30.000000 vsrgtools-1.5.0/vsrgtools/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-06-05 14:00:30.000000 vsrgtools-1.5.0/vsrgtools/limit.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 14:00:30.000000 vsrgtools-1.5.0/vsrgtools/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-06-05 14:00:30.000000 vsrgtools-1.5.0/vsrgtools/rgtools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-06-05 14:00:30.000000 vsrgtools-1.5.0/vsrgtools/sharp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-05 14:00:30.000000 vsrgtools-1.5.0/vsrgtools/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:00:51.233498 vsrgtools-1.5.0/vsrgtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-05 14:00:51.000000 vsrgtools-1.5.0/vsrgtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-05 14:00:51.000000 vsrgtools-1.5.0/vsrgtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 14:00:51.000000 vsrgtools-1.5.0/vsrgtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-05 14:00:51.000000 vsrgtools-1.5.0/vsrgtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-05 14:00:51.000000 vsrgtools-1.5.0/vsrgtools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:31:05.446424 vsrgtools-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-20 14:30:43.000000 vsrgtools-1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-20 14:31:05.446424 vsrgtools-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-20 14:30:43.000000 vsrgtools-1.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-20 14:31:05.446424 vsrgtools-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-20 14:30:43.000000 vsrgtools-1.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:31:05.442423 vsrgtools-1.5.1/vsrgtools/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-20 14:30:43.000000 vsrgtools-1.5.1/vsrgtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-20 14:30:43.000000 vsrgtools-1.5.1/vsrgtools/_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:31:05.442423 vsrgtools-1.5.1/vsrgtools/aka_expr/
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-06-20 14:30:43.000000 vsrgtools-1.5.1/vsrgtools/aka_expr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-06-20 14:30:43.000000 vsrgtools-1.5.1/vsrgtools/aka_expr/_rg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14266 2023-06-20 14:30:43.000000 vsrgtools-1.5.1/vsrgtools/aka_expr/_rp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-06-20 14:30:43.000000 vsrgtools-1.5.1/vsrgtools/bilateral.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    14356 2023-06-20 14:30:43.000000 vsrgtools-1.5.1/vsrgtools/blur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-06-20 14:30:43.000000 vsrgtools-1.5.1/vsrgtools/contra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-06-20 14:30:43.000000 vsrgtools-1.5.1/vsrgtools/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-06-20 14:30:43.000000 vsrgtools-1.5.1/vsrgtools/freqs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-20 14:30:43.000000 vsrgtools-1.5.1/vsrgtools/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-06-20 14:30:43.000000 vsrgtools-1.5.1/vsrgtools/limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:30:43.000000 vsrgtools-1.5.1/vsrgtools/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-06-20 14:30:43.000000 vsrgtools-1.5.1/vsrgtools/rgtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-06-20 14:30:43.000000 vsrgtools-1.5.1/vsrgtools/sharp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-20 14:30:43.000000 vsrgtools-1.5.1/vsrgtools/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:31:05.442423 vsrgtools-1.5.1/vsrgtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-20 14:31:05.000000 vsrgtools-1.5.1/vsrgtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-20 14:31:05.000000 vsrgtools-1.5.1/vsrgtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 14:31:05.000000 vsrgtools-1.5.1/vsrgtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-20 14:31:05.000000 vsrgtools-1.5.1/vsrgtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-20 14:31:05.000000 vsrgtools-1.5.1/vsrgtools.egg-info/top_level.txt
```

### Comparing `vsrgtools-1.5.0/LICENSE` & `vsrgtools-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vsrgtools-1.5.0/PKG-INFO` & `vsrgtools-1.5.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsrgtools
-Version: 1.5.0
+Version: 1.5.1
 Summary: Wrapper for RGVS, RGSF, and various other functions
 Author: Irrational Encoding Wizardry
 Author-email: wizards@encode.moe
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-rgtools
 Project-URL: Documentation, https://vsrgtools.encode.moe/en/latest/
```

### Comparing `vsrgtools-1.5.0/setup.cfg` & `vsrgtools-1.5.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `vsrgtools-1.5.0/setup.py` & `vsrgtools-1.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `vsrgtools-1.5.0/vsrgtools/aka_expr/__init__.py` & `vsrgtools-1.5.1/vsrgtools/aka_expr/__init__.py`

 * *Files identical despite different names*

### Comparing `vsrgtools-1.5.0/vsrgtools/aka_expr/_rg.py` & `vsrgtools-1.5.1/vsrgtools/aka_expr/_rg.py`

 * *Files identical despite different names*

### Comparing `vsrgtools-1.5.0/vsrgtools/aka_expr/_rp.py` & `vsrgtools-1.5.1/vsrgtools/aka_expr/_rp.py`

 * *Files identical despite different names*

### Comparing `vsrgtools-1.5.0/vsrgtools/bilateral.cu` & `vsrgtools-1.5.1/vsrgtools/bilateral.cu`

 * *Files identical despite different names*

### Comparing `vsrgtools-1.5.0/vsrgtools/blur.py` & `vsrgtools-1.5.1/vsrgtools/blur.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,23 +63,32 @@
 
     if isinstance(radius, list):
         return normalize_radius(clip, box_blur, radius, planes, passes=passes)
 
     if not radius:
         return clip
 
-    if radius > 12:
+    fp16 = clip.format.sample_type == vs.FLOAT and clip.format.bits_per_sample == 16
+
+    if radius > 12 and not fp16:
         blurred = clip.std.BoxBlur(planes, radius, passes, radius, passes)
     else:
         matrix_size = radius * 2 | 1
+
+        if fp16:
+            matrix_size **= 2
+
         blurred = clip
         for _ in range(passes):
-            blurred = blurred.std.Convolution(
-                [1] * matrix_size, planes=planes, mode=ConvMode.SQUARE
-            )
+            if fp16:
+                blurred = norm_expr(blurred, [
+                    ExprOp.matrix('x', radius), ExprOp.ADD * (matrix_size - 1), matrix_size, ExprOp.DIV
+                ], planes)
+            else:
+                blurred = blurred.std.Convolution([1] * matrix_size, planes=planes, mode=ConvMode.SQUARE)
 
     return blurred
 
 
 def side_box_blur(
     clip: vs.VideoNode, radius: int | list[int] = 1, planes: PlanesT = None,
     inverse: bool = False
```

### Comparing `vsrgtools-1.5.0/vsrgtools/contra.py` & `vsrgtools-1.5.1/vsrgtools/contra.py`

 * *Files identical despite different names*

### Comparing `vsrgtools-1.5.0/vsrgtools/enum.py` & `vsrgtools-1.5.1/vsrgtools/enum.py`

 * *Files identical despite different names*

### Comparing `vsrgtools-1.5.0/vsrgtools/freqs.py` & `vsrgtools-1.5.1/vsrgtools/freqs.py`

 * *Files identical despite different names*

### Comparing `vsrgtools-1.5.0/vsrgtools/func.py` & `vsrgtools-1.5.1/vsrgtools/func.py`

 * *Files identical despite different names*

### Comparing `vsrgtools-1.5.0/vsrgtools/limit.py` & `vsrgtools-1.5.1/vsrgtools/limit.py`

 * *Files identical despite different names*

### Comparing `vsrgtools-1.5.0/vsrgtools/rgtools.py` & `vsrgtools-1.5.1/vsrgtools/rgtools.py`

 * *Files identical despite different names*

### Comparing `vsrgtools-1.5.0/vsrgtools/sharp.py` & `vsrgtools-1.5.1/vsrgtools/sharp.py`

 * *Files identical despite different names*

### Comparing `vsrgtools-1.5.0/vsrgtools/util.py` & `vsrgtools-1.5.1/vsrgtools/util.py`

 * *Files identical despite different names*

### Comparing `vsrgtools-1.5.0/vsrgtools.egg-info/PKG-INFO` & `vsrgtools-1.5.1/vsrgtools.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsrgtools
-Version: 1.5.0
+Version: 1.5.1
 Summary: Wrapper for RGVS, RGSF, and various other functions
 Author: Irrational Encoding Wizardry
 Author-email: wizards@encode.moe
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-rgtools
 Project-URL: Documentation, https://vsrgtools.encode.moe/en/latest/
```

### Comparing `vsrgtools-1.5.0/vsrgtools.egg-info/SOURCES.txt` & `vsrgtools-1.5.1/vsrgtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

