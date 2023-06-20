# Comparing `tmp/vsdehalo-1.7.1.tar.gz` & `tmp/vsdehalo-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsdehalo-1.7.1.tar", last modified: Mon Jun  5 14:33:46 2023, max compression
+gzip compressed data, was "vsdehalo-1.7.2.tar", last modified: Tue Jun 20 15:27:16 2023, max compression
```

## Comparing `vsdehalo-1.7.1.tar` & `vsdehalo-1.7.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:33:46.603425 vsdehalo-1.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-05 14:33:24.000000 vsdehalo-1.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-05 14:33:46.603425 vsdehalo-1.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-05 14:33:24.000000 vsdehalo-1.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-05 14:33:46.603425 vsdehalo-1.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-05 14:33:24.000000 vsdehalo-1.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:33:46.603425 vsdehalo-1.7.1/vsdehalo/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-05 14:33:24.000000 vsdehalo-1.7.1/vsdehalo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-05 14:33:24.000000 vsdehalo-1.7.1/vsdehalo/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    31378 2023-06-05 14:33:24.000000 vsdehalo-1.7.1/vsdehalo/alpha.py
--rw-r--r--   0 runner    (1001) docker     (123)     7299 2023-06-05 14:33:24.000000 vsdehalo-1.7.1/vsdehalo/denoise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-05 14:33:24.000000 vsdehalo-1.7.1/vsdehalo/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 14:33:24.000000 vsdehalo-1.7.1/vsdehalo/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7536 2023-06-05 14:33:24.000000 vsdehalo-1.7.1/vsdehalo/vine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-06-05 14:33:24.000000 vsdehalo-1.7.1/vsdehalo/warp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:33:46.603425 vsdehalo-1.7.1/vsdehalo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-05 14:33:46.000000 vsdehalo-1.7.1/vsdehalo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-05 14:33:46.000000 vsdehalo-1.7.1/vsdehalo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 14:33:46.000000 vsdehalo-1.7.1/vsdehalo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-05 14:33:46.000000 vsdehalo-1.7.1/vsdehalo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-05 14:33:46.000000 vsdehalo-1.7.1/vsdehalo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:27:16.369732 vsdehalo-1.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-20 15:26:54.000000 vsdehalo-1.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-20 15:27:16.369732 vsdehalo-1.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-20 15:26:54.000000 vsdehalo-1.7.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-20 15:27:16.369732 vsdehalo-1.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-20 15:26:54.000000 vsdehalo-1.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:27:16.369732 vsdehalo-1.7.2/vsdehalo/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-20 15:26:54.000000 vsdehalo-1.7.2/vsdehalo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-20 15:26:54.000000 vsdehalo-1.7.2/vsdehalo/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31303 2023-06-20 15:26:54.000000 vsdehalo-1.7.2/vsdehalo/alpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7299 2023-06-20 15:26:54.000000 vsdehalo-1.7.2/vsdehalo/denoise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-20 15:26:54.000000 vsdehalo-1.7.2/vsdehalo/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:26:54.000000 vsdehalo-1.7.2/vsdehalo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7536 2023-06-20 15:26:54.000000 vsdehalo-1.7.2/vsdehalo/vine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-06-20 15:26:54.000000 vsdehalo-1.7.2/vsdehalo/warp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:27:16.369732 vsdehalo-1.7.2/vsdehalo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-20 15:27:16.000000 vsdehalo-1.7.2/vsdehalo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-20 15:27:16.000000 vsdehalo-1.7.2/vsdehalo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:27:16.000000 vsdehalo-1.7.2/vsdehalo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-20 15:27:16.000000 vsdehalo-1.7.2/vsdehalo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 15:27:16.000000 vsdehalo-1.7.2/vsdehalo.egg-info/top_level.txt
```

### Comparing `vsdehalo-1.7.1/LICENSE` & `vsdehalo-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vsdehalo-1.7.1/PKG-INFO` & `vsdehalo-1.7.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsdehalo
-Version: 1.7.1
+Version: 1.7.2
 Summary: Collection of dehaloing VapourSynth functions
 Author: Setsugen no ao
 Author-email: setsugen@setsugen.dev
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-dehalo
 Project-URL: Documentation, https://vsdehalo.encode.moe/en/latest/
```

### Comparing `vsdehalo-1.7.1/setup.cfg` & `vsdehalo-1.7.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `vsdehalo-1.7.1/setup.py` & `vsdehalo-1.7.2/setup.py`

 * *Files identical despite different names*

### Comparing `vsdehalo-1.7.1/vsdehalo/alpha.py` & `vsdehalo-1.7.2/vsdehalo/alpha.py`

 * *Files 1% similar despite different names*

```diff
@@ -673,20 +673,18 @@
     dehalo_mask = RemoveGrainMode.MINMAX_MEDIAN_OPP(dehalo_mask)
 
     if brz:
         dmask_expr = f"x {scale_value(abs(brz), 32, y)} {'>' if brz < 0.0 else '>'} 0 x 2 * ?"
     else:
         dmask_expr = 'x 2 *'
 
-    dehalo_mask = norm_expr(dehalo_mask, dmask_expr, func.norm_planes)
+    dehalo_mask = norm_expr(dehalo_mask, dmask_expr)
 
-    fine_edge_mask = fine_dehalo.mask(norm_expr([y_mask, ymask_ref0], 'y x -'), planes=func.norm_planes)
-    dehalo_mask = norm_expr(
-        [dehalo_mask, y_mask, ymask_ref0, fine_edge_mask], 'y z + 2 / x < x and x abs a ?', func.norm_planes
-    )
+    fine_edge_mask = fine_dehalo.mask(norm_expr([y_mask, ymask_ref0], 'y x -'))
+    dehalo_mask = norm_expr([dehalo_mask, y_mask, ymask_ref0, fine_edge_mask], 'y z + 2 / x < x and x abs a ?')
     dehalo_mask = RemoveGrainMode.EDGE_CLIP_STRONG(dehalo_mask)
 
     actual_dehalo = dehalo_sigma(
         func.work_clip, pre_ss=1 + pre_ss, sigma=sigma, ss=ss - 0.5 * pre_ss, planes=func.norm_planes, **kwargs
     )
     dehalo_ref = fine_dehalo(func.work_clip, planes=func.norm_planes, **fdehalo_kwargs)
```

### Comparing `vsdehalo-1.7.1/vsdehalo/denoise.py` & `vsdehalo-1.7.2/vsdehalo/denoise.py`

 * *Files identical despite different names*

### Comparing `vsdehalo-1.7.1/vsdehalo/mask.py` & `vsdehalo-1.7.2/vsdehalo/mask.py`

 * *Files identical despite different names*

### Comparing `vsdehalo-1.7.1/vsdehalo/vine.py` & `vsdehalo-1.7.2/vsdehalo/vine.py`

 * *Files identical despite different names*

### Comparing `vsdehalo-1.7.1/vsdehalo/warp.py` & `vsdehalo-1.7.2/vsdehalo/warp.py`

 * *Files identical despite different names*

### Comparing `vsdehalo-1.7.1/vsdehalo.egg-info/PKG-INFO` & `vsdehalo-1.7.2/vsdehalo.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsdehalo
-Version: 1.7.1
+Version: 1.7.2
 Summary: Collection of dehaloing VapourSynth functions
 Author: Setsugen no ao
 Author-email: setsugen@setsugen.dev
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-dehalo
 Project-URL: Documentation, https://vsdehalo.encode.moe/en/latest/
```

