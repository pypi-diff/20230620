# Comparing `tmp/vsdenoise-2.3.0.tar.gz` & `tmp/vsdenoise-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsdenoise-2.3.0.tar", last modified: Mon Jun  5 14:32:33 2023, max compression
+gzip compressed data, was "vsdenoise-2.4.0.tar", last modified: Tue Jun 20 15:10:42 2023, max compression
```

## Comparing `vsdenoise-2.3.0.tar` & `vsdenoise-2.4.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:32:33.118652 vsdenoise-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-05 14:32:08.000000 vsdenoise-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-05 14:32:33.118652 vsdenoise-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-05 14:32:08.000000 vsdenoise-2.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-05 14:32:33.118652 vsdenoise-2.3.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1507 2023-06-05 14:32:08.000000 vsdenoise-2.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:32:33.114652 vsdenoise-2.3.0/vsdenoise/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-05 14:32:08.000000 vsdenoise-2.3.0/vsdenoise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-05 14:32:08.000000 vsdenoise-2.3.0/vsdenoise/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    13337 2023-06-05 14:32:08.000000 vsdenoise-2.3.0/vsdenoise/blockmatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    21887 2023-06-05 14:32:08.000000 vsdenoise-2.3.0/vsdenoise/bm3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    10984 2023-06-05 14:32:08.000000 vsdenoise-2.3.0/vsdenoise/ccd.py
--rw-r--r--   0 runner    (1001) docker     (123)    12537 2023-06-05 14:32:08.000000 vsdenoise-2.3.0/vsdenoise/deblock.py
--rw-r--r--   0 runner    (1001) docker     (123)    23153 2023-06-05 14:32:08.000000 vsdenoise-2.3.0/vsdenoise/fft.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-06-05 14:32:08.000000 vsdenoise-2.3.0/vsdenoise/freqs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-06-05 14:32:08.000000 vsdenoise-2.3.0/vsdenoise/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-06-05 14:32:08.000000 vsdenoise-2.3.0/vsdenoise/limit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:32:33.118652 vsdenoise-2.3.0/vsdenoise/mvtools/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-05 14:32:08.000000 vsdenoise-2.3.0/vsdenoise/mvtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17878 2023-06-05 14:32:08.000000 vsdenoise-2.3.0/vsdenoise/mvtools/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-05 14:32:08.000000 vsdenoise-2.3.0/vsdenoise/mvtools/motion.py
--rw-r--r--   0 runner    (1001) docker     (123)    46432 2023-06-05 14:32:08.000000 vsdenoise-2.3.0/vsdenoise/mvtools/mvtools.py
--rw-r--r--   0 runner    (1001) docker     (123)     6023 2023-06-05 14:32:08.000000 vsdenoise-2.3.0/vsdenoise/mvtools/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-05 14:32:08.000000 vsdenoise-2.3.0/vsdenoise/mvtools/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9299 2023-06-05 14:32:08.000000 vsdenoise-2.3.0/vsdenoise/nlm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9762 2023-06-05 14:32:08.000000 vsdenoise-2.3.0/vsdenoise/postprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    41315 2023-06-05 14:32:08.000000 vsdenoise-2.3.0/vsdenoise/prefilters.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 14:32:08.000000 vsdenoise-2.3.0/vsdenoise/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14277 2023-06-05 14:32:08.000000 vsdenoise-2.3.0/vsdenoise/regress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-06-05 14:32:08.000000 vsdenoise-2.3.0/vsdenoise/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:32:33.114652 vsdenoise-2.3.0/vsdenoise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-05 14:32:33.000000 vsdenoise-2.3.0/vsdenoise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-05 14:32:33.000000 vsdenoise-2.3.0/vsdenoise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 14:32:33.000000 vsdenoise-2.3.0/vsdenoise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-05 14:32:33.000000 vsdenoise-2.3.0/vsdenoise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-05 14:32:33.000000 vsdenoise-2.3.0/vsdenoise.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:10:42.663140 vsdenoise-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-20 15:10:20.000000 vsdenoise-2.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-20 15:10:42.663140 vsdenoise-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-20 15:10:20.000000 vsdenoise-2.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-20 15:10:42.663140 vsdenoise-2.4.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1507 2023-06-20 15:10:20.000000 vsdenoise-2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:10:42.663140 vsdenoise-2.4.0/vsdenoise/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-20 15:10:20.000000 vsdenoise-2.4.0/vsdenoise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-20 15:10:20.000000 vsdenoise-2.4.0/vsdenoise/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13337 2023-06-20 15:10:20.000000 vsdenoise-2.4.0/vsdenoise/blockmatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21887 2023-06-20 15:10:20.000000 vsdenoise-2.4.0/vsdenoise/bm3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10984 2023-06-20 15:10:20.000000 vsdenoise-2.4.0/vsdenoise/ccd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13018 2023-06-20 15:10:20.000000 vsdenoise-2.4.0/vsdenoise/deblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23153 2023-06-20 15:10:20.000000 vsdenoise-2.4.0/vsdenoise/fft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-06-20 15:10:20.000000 vsdenoise-2.4.0/vsdenoise/freqs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-06-20 15:10:20.000000 vsdenoise-2.4.0/vsdenoise/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-06-20 15:10:20.000000 vsdenoise-2.4.0/vsdenoise/limit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:10:42.663140 vsdenoise-2.4.0/vsdenoise/mvtools/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-20 15:10:20.000000 vsdenoise-2.4.0/vsdenoise/mvtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17878 2023-06-20 15:10:20.000000 vsdenoise-2.4.0/vsdenoise/mvtools/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-20 15:10:20.000000 vsdenoise-2.4.0/vsdenoise/mvtools/motion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46432 2023-06-20 15:10:20.000000 vsdenoise-2.4.0/vsdenoise/mvtools/mvtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6023 2023-06-20 15:10:20.000000 vsdenoise-2.4.0/vsdenoise/mvtools/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-20 15:10:20.000000 vsdenoise-2.4.0/vsdenoise/mvtools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9834 2023-06-20 15:10:20.000000 vsdenoise-2.4.0/vsdenoise/nlm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9762 2023-06-20 15:10:20.000000 vsdenoise-2.4.0/vsdenoise/postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41350 2023-06-20 15:10:20.000000 vsdenoise-2.4.0/vsdenoise/prefilters.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:10:20.000000 vsdenoise-2.4.0/vsdenoise/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    29523 2023-06-20 15:10:20.000000 vsdenoise-2.4.0/vsdenoise/regress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-06-20 15:10:20.000000 vsdenoise-2.4.0/vsdenoise/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:10:42.663140 vsdenoise-2.4.0/vsdenoise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-20 15:10:42.000000 vsdenoise-2.4.0/vsdenoise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-20 15:10:42.000000 vsdenoise-2.4.0/vsdenoise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:10:42.000000 vsdenoise-2.4.0/vsdenoise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-20 15:10:42.000000 vsdenoise-2.4.0/vsdenoise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-20 15:10:42.000000 vsdenoise-2.4.0/vsdenoise.egg-info/top_level.txt
```

### Comparing `vsdenoise-2.3.0/LICENSE` & `vsdenoise-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vsdenoise-2.3.0/PKG-INFO` & `vsdenoise-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsdenoise
-Version: 2.3.0
+Version: 2.4.0
 Summary: VapourSynth denoising functions
 Author: Irrational Encoding Wizardry
 Author-email: wizards@encode.moe
 Maintainer: Irrational Encoding Wizardry
 Maintainer-email: wizards@encode.moe
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-denoise
 Project-URL: Documentation, https://vsdenoise.encode.moe/en/latest/
```

### Comparing `vsdenoise-2.3.0/README.md` & `vsdenoise-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `vsdenoise-2.3.0/setup.cfg` & `vsdenoise-2.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `vsdenoise-2.3.0/setup.py` & `vsdenoise-2.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `vsdenoise-2.3.0/vsdenoise/blockmatch.py` & `vsdenoise-2.4.0/vsdenoise/blockmatch.py`

 * *Files identical despite different names*

### Comparing `vsdenoise-2.3.0/vsdenoise/bm3d.py` & `vsdenoise-2.4.0/vsdenoise/bm3d.py`

 * *Files 2% similar despite different names*

```diff
@@ -563,28 +563,24 @@
     ...
 
 
 class BM3DCPU(AbstractBM3DCuda, plugin=core.lazy.bm3dcpu):
     ...
 
 
-class AutoBM3DMeta(ABCMeta):
-    def __new__(
-        __mcls: type[Self], __name: str, __bases: tuple[type, ...], __namespace: dict[str, Any], **kwargs: Any
-    ) -> type[AbstractBM3D]:
-        if hasattr(core, 'bm3dcuda_rtc'):
-            return BM3DCudaRTC
-
-        if hasattr(core, 'bm3dcuda'):
-            return BM3DCuda
-
-        if hasattr(core, 'bm3dcpu'):
-            return BM3DCPU
+class BM3D(AbstractBM3D):
+    def __new__(cls, *args: Any, **kwargs: Any) -> AbstractBM3D:  # type: ignore
+        new_cls: type[AbstractBM3D] | None = None
 
-        if hasattr(core, 'bm3d'):
-            return BM3DMawen
-
-        raise CustomRuntimeError('You have no bm3d plugin installed!')
+        if hasattr(core, 'bm3dcuda_rtc'):
+            new_cls = BM3DCudaRTC
+        elif hasattr(core, 'bm3dcuda'):
+            new_cls = BM3DCuda
+        elif hasattr(core, 'bm3dcpu'):
+            new_cls = BM3DCPU
+        elif hasattr(core, 'bm3d'):
+            new_cls = BM3DMawen
 
+        if new_cls is None:
+            raise CustomRuntimeError('You have no bm3d plugin installed!')
 
-class BM3D(AbstractBM3D, metaclass=AutoBM3DMeta):
-    ...
+        return new_cls(*args, **kwargs)
```

### Comparing `vsdenoise-2.3.0/vsdenoise/ccd.py` & `vsdenoise-2.4.0/vsdenoise/ccd.py`

 * *Files identical despite different names*

### Comparing `vsdenoise-2.3.0/vsdenoise/deblock.py` & `vsdenoise-2.4.0/vsdenoise/deblock.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 
 __all__ = [
     'dpir', 'dpir_mask'
 ]
 
 
 class _dpir(CustomStrEnum):
-    DEBLOCK = 'deblock'
-    DENOISE = 'denoise'
+    DEBLOCK: _dpir = 'deblock'  # type: ignore
+    DENOISE: _dpir = 'denoise'  # type: ignore
 
     def __call__(
         self, clip: vs.VideoNode, strength: SupportsFloat | vs.VideoNode | None | tuple[
             SupportsFloat | vs.VideoNode | None, SupportsFloat | vs.VideoNode | None
         ] = 10, matrix: MatrixT | None = None, cuda: bool | Literal['trt'] | None = None, i444: bool = False,
         tiles: int | tuple[int, int] | None = None, overlap: int | tuple[int, int] | None = 8,
         zones: list[tuple[FrameRangeN | FrameRangesN | None, SupportsFloat | vs.VideoNode | None]] | None = None,
@@ -44,14 +44,17 @@
             if clip.format.num_planes > 1:
                 args = (matrix, cuda, i444, tiles, overlap, zones, fp16, num_streams, device_id, kernel)
                 return join(dpir(get_y(clip), strength[0], *args), dpir(clip, strength[1], *args))
             strength = strength[0]
 
         kernel = Kernel.ensure_obj(kernel)
 
+        if not strength:
+            return kernel.resample(clip, clip.format.replace(subsampling_w=0, subsampling_h=0)) if i444 else clip
+
         bit_depth = get_depth(clip)
         is_rgb, is_gray = (clip.format.color_family is f for f in (vs.RGB, vs.GRAY))
 
         if self.value == 'deblock':
             model = DPIRModel.drunet_deblocking_grayscale if is_gray else DPIRModel.drunet_deblocking_color
         else:  # elif self.value == 'denoise':
             model = DPIRModel.drunet_color if not is_gray else DPIRModel.drunet_gray
@@ -71,17 +74,15 @@
 
         if fp16 is None:
             fp16 = fp16_available
 
         def _get_strength_clip(clip: vs.VideoNode, strength: SupportsFloat) -> vs.VideoNode:
             return clip.std.BlankClip(format=vs.GRAYH if fp16 else vs.GRAYS, color=float(strength) / 255, keep=True)
 
-        if isinstance(strength, vs.VideoNode):
-            str_clip: vs.VideoNode = strength  # type: ignore
-
+        def _norm_str_clip(str_clip: vs.VideoNode) -> vs.VideoNode:
             assert (fmt := str_clip.format)
 
             InvalidColorFamilyError.check(
                 fmt, vs.GRAY, func, '"strength" must be of {correct} color family, not {wrong}!'
             )
 
             if fmt.id == vs.GRAY8:
@@ -93,15 +94,18 @@
 
             if str_clip.width != clip.width or str_clip.height != clip.height:
                 str_clip = kernel.scale(str_clip, clip.width, clip.height)  # type: ignore
 
             if str_clip.num_frames != clip.num_frames:
                 raise LengthMismatchError(func, '`strength` must be of the same length as \'clip\'')
 
-            strength = str_clip
+            return str_clip
+
+        if isinstance(strength, vs.VideoNode):
+            strength = _norm_str_clip(strength)  # type: ignore
         elif isinstance(strength, SupportsFloat):
             strength = float(strength)
         else:
             raise UnsupportedVideoFormatError('`strength` must be a float or a GRAYS clip', func)
 
         if not is_rgb:
             targ_matrix = Matrix.from_param(matrix) or Matrix.from_video(clip)
@@ -181,15 +185,15 @@
                         no_dpir_zones.append(ranges)  # type: ignore
 
                     continue
 
                 rstr_clip: vs.VideoNode
 
                 if isinstance(zstr, vs.VideoNode):
-                    rstr_clip = zstr  # type: ignore
+                    rstr_clip = _norm_str_clip(zstr)  # type: ignore
                 else:
                     zstr = float(zstr)  # type: ignore
 
                     if zstr not in cache_strength_clips:
                         cache_strength_clips[zstr] = _get_strength_clip(clip_rgb, zstr)
 
                     rstr_clip = cache_strength_clips[zstr]
@@ -198,14 +202,18 @@
 
                 for rrange in lranges:
                     if rrange:
                         dpir_zones[rrange] = rstr_clip
 
             if len(dpir_zones) <= 2:
                 for rrange, sclip in dpir_zones.items():
+                    if to_pad:
+                        sclip = Point(src_width=d_width, src_height=d_height).scale(
+                            sclip, d_width, d_height, (-mod_h, -mod_w)
+                        )
                     zoned_strength_clip = replace_ranges(zoned_strength_clip, sclip, rrange)
             else:
                 dpir_ranges_zones = {
                     range(*(
                         (r, r + 1) if isinstance(r, int) else (r[0] or 0, r[1] + 1 if r[1] else clip.num_frames)
                     )): sclip for r, sclip in dpir_zones.items()
                 }
```

### Comparing `vsdenoise-2.3.0/vsdenoise/fft.py` & `vsdenoise-2.4.0/vsdenoise/fft.py`

 * *Files identical despite different names*

### Comparing `vsdenoise-2.3.0/vsdenoise/freqs.py` & `vsdenoise-2.4.0/vsdenoise/freqs.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     'frequency_merge'
 ]
 
 
 def frequency_merge(
     *_clips: vs.VideoNode | Iterable[vs.VideoNode], tr: int = 0,
     mode_high: MeanMode = MeanMode.LEHMER, mode_low: MeanMode = MeanMode.ARITHMETIC,
-    mode_tr: MeanMode | None = None, lowpass: GenericVSFunction | list[GenericVSFunction] = DFTTest(sigma=5).denoise,
+    mode_tr: MeanMode | None = None, lowpass: GenericVSFunction | list[GenericVSFunction] = DFTTest.denoise,
     mean_diff: bool = False, planes: PlanesT = None, mv_args: KwargsT | None = None,
     **kwargs: Any
 ) -> vs.VideoNode:
     clips = flatten_vnodes(_clips)
     n_clips = len(clips)
 
     mv_args = mv_args or KwargsT()
```

### Comparing `vsdenoise-2.3.0/vsdenoise/funcs.py` & `vsdenoise-2.4.0/vsdenoise/funcs.py`

 * *Files identical despite different names*

### Comparing `vsdenoise-2.3.0/vsdenoise/limit.py` & `vsdenoise-2.4.0/vsdenoise/limit.py`

 * *Files identical despite different names*

### Comparing `vsdenoise-2.3.0/vsdenoise/mvtools/enums.py` & `vsdenoise-2.4.0/vsdenoise/mvtools/enums.py`

 * *Files identical despite different names*

### Comparing `vsdenoise-2.3.0/vsdenoise/mvtools/motion.py` & `vsdenoise-2.4.0/vsdenoise/mvtools/motion.py`

 * *Files identical despite different names*

### Comparing `vsdenoise-2.3.0/vsdenoise/mvtools/mvtools.py` & `vsdenoise-2.4.0/vsdenoise/mvtools/mvtools.py`

 * *Files identical despite different names*

### Comparing `vsdenoise-2.3.0/vsdenoise/mvtools/presets.py` & `vsdenoise-2.4.0/vsdenoise/mvtools/presets.py`

 * *Files identical despite different names*

### Comparing `vsdenoise-2.3.0/vsdenoise/mvtools/utils.py` & `vsdenoise-2.4.0/vsdenoise/mvtools/utils.py`

 * *Files identical despite different names*

### Comparing `vsdenoise-2.3.0/vsdenoise/nlm.py` & `vsdenoise-2.4.0/vsdenoise/nlm.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 This module implements a wrapper for non local means denoisers
 """
 
 from __future__ import annotations
 
 import warnings
 from enum import auto
-from typing import TYPE_CHECKING, Any, Literal, NamedTuple, Sequence, overload
+from typing import TYPE_CHECKING, Any, Callable, Literal, NamedTuple, Sequence, overload
 
 from vstools import (
     CustomEnum, CustomIntEnum, CustomValueError, KwargsT, PlanesT, check_variable, core, join, normalize_planes,
     normalize_seq, to_arr, vs
 )
 
 __all__ = [
@@ -123,23 +123,42 @@
         self: DeviceTypeWithInfo | DeviceType, clip: vs.VideoNode,
         h: float | None = None, d: int | None = None, a: int | None = None, s: int | None = None,
         channels: str | None = None, wmode: int | None = None, wref: float | None = None,
         ref: vs.VideoNode | None = None, **kwargs: Any
     ) -> vs.VideoNode:
         if self == DeviceType.AUTO and hasattr(core, 'nlm_cuda'):
             self = DeviceType.CUDA
-        elif self == DeviceType.CUDA and not hasattr(core, 'nlm_cuda'):
+
+        if self == DeviceType.CUDA and not hasattr(core, 'nlm_cuda'):
             raise CustomValueError("You can't use cuda device type, you are missing the nlm_cuda plugin!")
 
+        funcs = list[Callable[..., vs.VideoNode]]()
+
         if self == DeviceType.CUDA:
-            return core.nlm_cuda.NLMeans(  # type: ignore
-                clip, d, a, s, h, channels, wmode, wref, ref, **(self.kwargs | kwargs)
-            )
+            funcs.append(core.proxied.nlm_cuda.NLMeans)
+        else:
+            funcs.extend([core.proxied.knlm.KNLMeansCL, core.proxied.nlm_ispc.NLMeans])
+
+        exceptions = list[Exception]()
+
+        for func in funcs:
+            try:
+                return func(clip, d, a, s, h, channels, wmode, wref, ref, **(self.kwargs | kwargs))
+            except Exception as _e:
+                exceptions.append(_e)
+
+        for x in (True, False):
+            for e in exceptions:
+                if not isinstance(e, AttributeError):
+                    if 'no compatible opencl' not in str(e):
+                        if x:
+                            continue
+                    raise e from None
 
-        return core.knlm.KNLMeansCL(clip, d, a, s, h, channels, wmode, wref, ref, **(self.kwargs | kwargs))
+        raise next(iter(exceptions))
 
 
 class DeviceType(DeviceTypeWithInfo, CustomEnum):
     """Enum representing available OpenCL device on which to run the plugin."""
 
     ACCELERATOR = 'accelerator'
     """Dedicated OpenCL accelerators."""
```

### Comparing `vsdenoise-2.3.0/vsdenoise/postprocess.py` & `vsdenoise-2.4.0/vsdenoise/postprocess.py`

 * *Files identical despite different names*

### Comparing `vsdenoise-2.3.0/vsdenoise/prefilters.py` & `vsdenoise-2.4.0/vsdenoise/prefilters.py`

 * *Files 1% similar despite different names*

```diff
@@ -757,17 +757,19 @@
 class PrefilterPartial(PrefBase):  # type: ignore
     def __init__(self, prefilter: Prefilter, planes: PlanesT, **kwargs: Any) -> None:
         self.prefilter = prefilter
         self.planes = planes
         self.kwargs = kwargs
 
     def __call__(  # type: ignore
-        self, clip: vs.VideoNode, /, planes: PlanesT = None, **kwargs: Any
+        self, clip: vs.VideoNode, /, planes: PlanesT | MissingT = MISSING, **kwargs: Any
     ) -> vs.VideoNode:
-        return self.prefilter(clip, planes=fallback(planes, self.planes), **kwargs | self.kwargs)  # type: ignore
+        return self.prefilter(
+            clip, planes=self.planes if planes is MISSING else planes, **kwargs | self.kwargs
+        )
 
 
 class MultiPrefilter(PrefBase):  # type: ignore
     def __init__(self, *prefilters: Prefilter) -> None:
         self.prefilters = prefilters
 
     def __call__(self, clip: vs.VideoNode, /, **kwargs: Any) -> vs.VideoNode:  # type: ignore
```

### Comparing `vsdenoise-2.3.0/vsdenoise/types.py` & `vsdenoise-2.4.0/vsdenoise/types.py`

 * *Files identical despite different names*

### Comparing `vsdenoise-2.3.0/vsdenoise.egg-info/PKG-INFO` & `vsdenoise-2.4.0/vsdenoise.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsdenoise
-Version: 2.3.0
+Version: 2.4.0
 Summary: VapourSynth denoising functions
 Author: Irrational Encoding Wizardry
 Author-email: wizards@encode.moe
 Maintainer: Irrational Encoding Wizardry
 Maintainer-email: wizards@encode.moe
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-denoise
 Project-URL: Documentation, https://vsdenoise.encode.moe/en/latest/
```

### Comparing `vsdenoise-2.3.0/vsdenoise.egg-info/SOURCES.txt` & `vsdenoise-2.4.0/vsdenoise.egg-info/SOURCES.txt`

 * *Files identical despite different names*

