# Comparing `tmp/vsscale-1.9.0.tar.gz` & `tmp/vsscale-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsscale-1.9.0.tar", last modified: Mon Jun  5 14:03:02 2023, max compression
+gzip compressed data, was "vsscale-1.9.1.tar", last modified: Tue Jun 20 14:59:20 2023, max compression
```

## Comparing `vsscale-1.9.0.tar` & `vsscale-1.9.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:03:02.544036 vsscale-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-05 14:02:41.000000 vsscale-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-05 14:03:02.544036 vsscale-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-05 14:02:41.000000 vsscale-1.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-05 14:03:02.544036 vsscale-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-05 14:02:41.000000 vsscale-1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:03:02.540036 vsscale-1.9.0/vsscale/
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-05 14:02:41.000000 vsscale-1.9.0/vsscale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-05 14:02:41.000000 vsscale-1.9.0/vsscale/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-05 14:02:41.000000 vsscale-1.9.0/vsscale/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    20260 2023-06-05 14:02:41.000000 vsscale-1.9.0/vsscale/descale.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-05 14:02:41.000000 vsscale-1.9.0/vsscale/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9800 2023-06-05 14:02:41.000000 vsscale-1.9.0/vsscale/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-06-05 14:02:41.000000 vsscale-1.9.0/vsscale/gamma.py
--rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-06-05 14:02:41.000000 vsscale-1.9.0/vsscale/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-06-05 14:02:41.000000 vsscale-1.9.0/vsscale/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 14:02:41.000000 vsscale-1.9.0/vsscale/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13814 2023-06-05 14:02:41.000000 vsscale-1.9.0/vsscale/scale.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:03:02.544036 vsscale-1.9.0/vsscale/shaders/
--rw-r--r--   0 runner    (1001) docker     (123)   246177 2023-06-05 14:02:41.000000 vsscale-1.9.0/vsscale/shaders/FSRCNNX_x2_16-0-4-1.glsl
--rw-r--r--   0 runner    (1001) docker     (123)   362441 2023-06-05 14:02:41.000000 vsscale-1.9.0/vsscale/shaders/FSRCNNX_x2_56-16-4-1.glsl
--rw-r--r--   0 runner    (1001) docker     (123)    70598 2023-06-05 14:02:41.000000 vsscale-1.9.0/vsscale/shaders/FSRCNNX_x2_8-0-4-1.glsl
--rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-06-05 14:02:41.000000 vsscale-1.9.0/vsscale/shaders/SSimDownscaler.glsl
--rw-r--r--   0 runner    (1001) docker     (123)     7316 2023-06-05 14:02:41.000000 vsscale-1.9.0/vsscale/shaders/SSimSuperRes.glsl
--rw-r--r--   0 runner    (1001) docker     (123)     6240 2023-06-05 14:02:41.000000 vsscale-1.9.0/vsscale/shaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-06-05 14:02:41.000000 vsscale-1.9.0/vsscale/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:03:02.544036 vsscale-1.9.0/vsscale.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-05 14:03:02.000000 vsscale-1.9.0/vsscale.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-05 14:03:02.000000 vsscale-1.9.0/vsscale.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 14:03:02.000000 vsscale-1.9.0/vsscale.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-05 14:03:02.000000 vsscale-1.9.0/vsscale.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-05 14:03:02.000000 vsscale-1.9.0/vsscale.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:59:20.342775 vsscale-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-20 14:58:55.000000 vsscale-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-20 14:59:20.342775 vsscale-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-20 14:58:55.000000 vsscale-1.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-20 14:59:20.346775 vsscale-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-20 14:58:55.000000 vsscale-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:59:20.342775 vsscale-1.9.1/vsscale/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-20 14:58:55.000000 vsscale-1.9.1/vsscale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-20 14:58:55.000000 vsscale-1.9.1/vsscale/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-20 14:58:55.000000 vsscale-1.9.1/vsscale/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20260 2023-06-20 14:58:55.000000 vsscale-1.9.1/vsscale/descale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-20 14:58:55.000000 vsscale-1.9.1/vsscale/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9803 2023-06-20 14:58:55.000000 vsscale-1.9.1/vsscale/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-06-20 14:58:55.000000 vsscale-1.9.1/vsscale/gamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-06-20 14:58:55.000000 vsscale-1.9.1/vsscale/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-06-20 14:58:55.000000 vsscale-1.9.1/vsscale/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:58:55.000000 vsscale-1.9.1/vsscale/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13814 2023-06-20 14:58:55.000000 vsscale-1.9.1/vsscale/scale.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:59:20.342775 vsscale-1.9.1/vsscale/shaders/
+-rw-r--r--   0 runner    (1001) docker     (123)   246177 2023-06-20 14:58:55.000000 vsscale-1.9.1/vsscale/shaders/FSRCNNX_x2_16-0-4-1.glsl
+-rw-r--r--   0 runner    (1001) docker     (123)   362441 2023-06-20 14:58:55.000000 vsscale-1.9.1/vsscale/shaders/FSRCNNX_x2_56-16-4-1.glsl
+-rw-r--r--   0 runner    (1001) docker     (123)    70598 2023-06-20 14:58:55.000000 vsscale-1.9.1/vsscale/shaders/FSRCNNX_x2_8-0-4-1.glsl
+-rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-06-20 14:58:55.000000 vsscale-1.9.1/vsscale/shaders/SSimDownscaler.glsl
+-rw-r--r--   0 runner    (1001) docker     (123)     7316 2023-06-20 14:58:55.000000 vsscale-1.9.1/vsscale/shaders/SSimSuperRes.glsl
+-rw-r--r--   0 runner    (1001) docker     (123)     6240 2023-06-20 14:58:55.000000 vsscale-1.9.1/vsscale/shaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-06-20 14:58:55.000000 vsscale-1.9.1/vsscale/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:59:20.342775 vsscale-1.9.1/vsscale.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-20 14:59:20.000000 vsscale-1.9.1/vsscale.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-20 14:59:20.000000 vsscale-1.9.1/vsscale.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 14:59:20.000000 vsscale-1.9.1/vsscale.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-20 14:59:20.000000 vsscale-1.9.1/vsscale.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-20 14:59:20.000000 vsscale-1.9.1/vsscale.egg-info/top_level.txt
```

### Comparing `vsscale-1.9.0/LICENSE` & `vsscale-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vsscale-1.9.0/PKG-INFO` & `vsscale-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsscale
-Version: 1.9.0
+Version: 1.9.1
 Summary: VapourSynth (de)scaling functions
 Author: Setsugen no ao
 Author-email: setsugen@setsugen.dev
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-scale
 Project-URL: Documentation, https://vsscale.encode.moe/en/latest/
```

### Comparing `vsscale-1.9.0/setup.cfg` & `vsscale-1.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `vsscale-1.9.0/setup.py` & `vsscale-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `vsscale-1.9.0/vsscale/base.py` & `vsscale-1.9.1/vsscale/base.py`

 * *Files identical despite different names*

### Comparing `vsscale-1.9.0/vsscale/descale.py` & `vsscale-1.9.1/vsscale/descale.py`

 * *Files identical despite different names*

### Comparing `vsscale-1.9.0/vsscale/exceptions.py` & `vsscale-1.9.1/vsscale/exceptions.py`

 * *Files identical despite different names*

### Comparing `vsscale-1.9.0/vsscale/funcs.py` & `vsscale-1.9.1/vsscale/funcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,15 @@
         else:
             merged = smooth.std.Merge(ref, merge_weight)
 
             if isinstance(self.limit, RepairMode):
                 merged = repair(merged, smooth, self.limit)
 
         if self.operator is not None:
-            merge2 = combine([smooth, ref], ExprOp.MIN)
+            merge2 = combine([smooth, ref], self.operator)
 
             if self.masked:
                 merged = merged.std.MaskedMerge(merge2, ringing_mask(smooth))
             else:
                 merged = merge2
         elif self.masked:
             merged.std.MaskedMerge(smooth, ringing_mask(smooth))
```

### Comparing `vsscale-1.9.0/vsscale/gamma.py` & `vsscale-1.9.1/vsscale/gamma.py`

 * *Files identical despite different names*

### Comparing `vsscale-1.9.0/vsscale/helpers.py` & `vsscale-1.9.1/vsscale/helpers.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,15 +10,18 @@
 from vstools import F_VD, KwargsT, MatrixT, fallback, get_w, mod2, plane, vs
 
 from .types import Resolution
 
 __all__ = [
     'GenericScaler',
     'scale_var_clip',
-    'fdescale_args'
+    'fdescale_args',
+    'descale_args',
+
+    'ScalingArgs'
 ]
 
 
 class _GeneriScaleNoShift(Protocol):
     def __call__(self, clip: vs.VideoNode, width: int, height: int, *args: Any, **kwds: Any) -> vs.VideoNode:
         ...
 
@@ -117,26 +120,31 @@
 
     def ensure_scaler(self, scaler: ScalerT) -> Scaler:
         from dataclasses import is_dataclass, replace
 
         scaler_obj = Scaler.ensure_obj(scaler, self.__class__)
 
         if is_dataclass(scaler_obj):
+            from inspect import Signature
+
             kwargs = dict()
 
-            if hasattr(scaler_obj, 'kernel'):
+            init_keys = Signature.from_callable(scaler_obj.__init__).parameters.keys()
+
+            if 'kernel' in init_keys:
                 kwargs.update(kernel=self.kernel or scaler_obj.kernel)
 
-            if hasattr(scaler_obj, 'scaler'):
+            if 'scaler' in init_keys:
                 kwargs.update(scaler=self.scaler or scaler_obj.scaler)
 
-            if hasattr(scaler_obj, 'shifter'):
+            if 'shifter' in init_keys:
                 kwargs.update(shifter=self.shifter or scaler_obj.shifter)
 
-            scaler_obj = replace(scaler_obj, **kwargs)
+            if kwargs:
+                scaler_obj = replace(scaler_obj, **kwargs)
 
         return scaler_obj
 
 
 def scale_var_clip(
     clip: vs.VideoNode,
     width: int | Callable[[Resolution], int] | None, height: int | Callable[[Resolution], int],
@@ -197,14 +205,93 @@
         out_clip = clip
     else:
         out_clip = clip.std.BlankClip(width, height)
 
     return out_clip.std.FrameEval(_eval_scale, clip, clip)
 
 
+@dataclass
+class ScalingArgs:
+    width: int
+    height: int
+    src_width: float
+    src_height: float
+    src_top: float
+    src_left: float
+    mode: str = 'hw'
+
+    base_clip: vs.VideoNode | None = None
+
+    def _do(self) -> tuple[bool, bool]:
+        return 'h' in self.mode.lower(), 'w' in self.mode.lower()
+
+    def _up_rate(self, clip: vs.VideoNode | None = None) -> tuple[float, float]:
+        if clip is None:
+            return 1.0, 1.0
+
+        assert self.base_clip
+
+        return clip.height / self.base_clip.height, clip.width / self.base_clip.width
+
+    def kwargs(self, clip: vs.VideoNode | None = None) -> KwargsT:
+        kwargs = KwargsT()
+        do_h, do_w = self._do()
+        up_rate_h, up_rate_w = self._up_rate(clip)
+
+        if do_h:
+            kwargs.update(
+                src_height=self.src_height * up_rate_h,
+                src_top=self.src_top * up_rate_h
+            )
+
+        if do_w:
+            kwargs.update(
+                src_width=self.src_width * up_rate_w,
+                src_left=self.src_left * up_rate_w
+            )
+
+        return kwargs
+
+
+def descale_args(
+    clip: vs.VideoNode,
+    src_height: float, src_width: float | None = None,
+    base_height: int | None = None, base_width: int | None = None,
+    crop_top: int = 0, crop_bottom: int = 0,
+    crop_left: int = 0, crop_right: int = 0,
+    mode: str = 'hw'
+) -> ScalingArgs:
+    base_height = fallback(base_height, mod2(ceil(src_height)))
+    base_width = fallback(base_width, get_w(base_height, clip, 2))
+
+    ratio = src_height / (clip.height + crop_top + crop_bottom)
+    src_width = fallback(src_width, ratio * (clip.width + crop_left + crop_right))
+
+    margin_left = (base_width - src_width) / 2 + ratio * crop_left
+    margin_right = (base_width - src_width) / 2 + ratio * crop_right
+    cropped_width = base_width - floor(margin_left) - floor(margin_right)
+
+    margin_top = (base_height - src_height) / 2 + ratio * crop_top
+    margin_bottom = (base_height - src_height) / 2 + ratio * crop_bottom
+    cropped_height = base_height - floor(margin_top) - floor(margin_bottom)
+
+    cropped_src_width = ratio * clip.width
+    cropped_src_left = margin_left - floor(margin_left)
+
+    cropped_src_height = ratio * clip.height
+    cropped_src_top = margin_top - floor(margin_top)
+
+    return ScalingArgs(
+        cropped_width, cropped_height,
+        cropped_src_width, cropped_src_height,
+        cropped_src_top, cropped_src_left,
+        mode, clip
+    )
+
+
 def fdescale_args(
     clip: vs.VideoNode, src_height: float,
     base_height: int | None = None, base_width: int | None = None,
     src_top: float | None = None, src_left: float | None = None,
     src_width: float | None = None, mode: str = 'hw', up_rate: float = 2.0
 ) -> tuple[KwargsT, KwargsT]:
     base_height = fallback(base_height, mod2(ceil(src_height)))
```

### Comparing `vsscale-1.9.0/vsscale/mask.py` & `vsscale-1.9.1/vsscale/mask.py`

 * *Files identical despite different names*

### Comparing `vsscale-1.9.0/vsscale/scale.py` & `vsscale-1.9.1/vsscale/scale.py`

 * *Files identical despite different names*

### Comparing `vsscale-1.9.0/vsscale/shaders/FSRCNNX_x2_16-0-4-1.glsl` & `vsscale-1.9.1/vsscale/shaders/FSRCNNX_x2_16-0-4-1.glsl`

 * *Files identical despite different names*

### Comparing `vsscale-1.9.0/vsscale/shaders/FSRCNNX_x2_56-16-4-1.glsl` & `vsscale-1.9.1/vsscale/shaders/FSRCNNX_x2_56-16-4-1.glsl`

 * *Files identical despite different names*

### Comparing `vsscale-1.9.0/vsscale/shaders/FSRCNNX_x2_8-0-4-1.glsl` & `vsscale-1.9.1/vsscale/shaders/FSRCNNX_x2_8-0-4-1.glsl`

 * *Files identical despite different names*

### Comparing `vsscale-1.9.0/vsscale/shaders/SSimDownscaler.glsl` & `vsscale-1.9.1/vsscale/shaders/SSimDownscaler.glsl`

 * *Files identical despite different names*

### Comparing `vsscale-1.9.0/vsscale/shaders/SSimSuperRes.glsl` & `vsscale-1.9.1/vsscale/shaders/SSimSuperRes.glsl`

 * *Files identical despite different names*

### Comparing `vsscale-1.9.0/vsscale/shaders.py` & `vsscale-1.9.1/vsscale/shaders.py`

 * *Files identical despite different names*

### Comparing `vsscale-1.9.0/vsscale/types.py` & `vsscale-1.9.1/vsscale/types.py`

 * *Files identical despite different names*

### Comparing `vsscale-1.9.0/vsscale.egg-info/PKG-INFO` & `vsscale-1.9.1/vsscale.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsscale
-Version: 1.9.0
+Version: 1.9.1
 Summary: VapourSynth (de)scaling functions
 Author: Setsugen no ao
 Author-email: setsugen@setsugen.dev
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-scale
 Project-URL: Documentation, https://vsscale.encode.moe/en/latest/
```

### Comparing `vsscale-1.9.0/vsscale.egg-info/SOURCES.txt` & `vsscale-1.9.1/vsscale.egg-info/SOURCES.txt`

 * *Files identical despite different names*

