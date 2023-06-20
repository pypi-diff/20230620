# Comparing `tmp/vsmasktools-1.1.1.tar.gz` & `tmp/vsmasktools-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsmasktools-1.1.1.tar", last modified: Mon Jun  5 20:26:01 2023, max compression
+gzip compressed data, was "vsmasktools-1.1.2.tar", last modified: Tue Jun 20 14:34:44 2023, max compression
```

## Comparing `vsmasktools-1.1.1.tar` & `vsmasktools-1.1.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:26:01.295195 vsmasktools-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-05 20:25:40.000000 vsmasktools-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-05 20:26:01.295195 vsmasktools-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-05 20:25:40.000000 vsmasktools-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-05 20:26:01.295195 vsmasktools-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-05 20:25:40.000000 vsmasktools-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:26:01.291195 vsmasktools-1.1.1/vsmasktools/
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-05 20:25:40.000000 vsmasktools-1.1.1/vsmasktools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-05 20:25:40.000000 vsmasktools-1.1.1/vsmasktools/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-06-05 20:25:40.000000 vsmasktools-1.1.1/vsmasktools/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-06-05 20:25:40.000000 vsmasktools-1.1.1/vsmasktools/details.py
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-06-05 20:25:40.000000 vsmasktools-1.1.1/vsmasktools/diff.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:26:01.295195 vsmasktools-1.1.1/vsmasktools/edge/
--rw-r--r--   0 runner    (1001) docker     (123)    30484 2023-06-05 20:25:40.000000 vsmasktools-1.1.1/vsmasktools/edge/_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-05 20:25:40.000000 vsmasktools-1.1.1/vsmasktools/edge/_2x2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9752 2023-06-05 20:25:40.000000 vsmasktools-1.1.1/vsmasktools/edge/_3x3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-06-05 20:25:40.000000 vsmasktools-1.1.1/vsmasktools/edge/_5x5.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-05 20:25:40.000000 vsmasktools-1.1.1/vsmasktools/edge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16192 2023-06-05 20:25:40.000000 vsmasktools-1.1.1/vsmasktools/edge/_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-06-05 20:25:40.000000 vsmasktools-1.1.1/vsmasktools/edge_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-05 20:25:40.000000 vsmasktools-1.1.1/vsmasktools/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12259 2023-06-05 20:25:40.000000 vsmasktools-1.1.1/vsmasktools/hardsub.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-05 20:25:40.000000 vsmasktools-1.1.1/vsmasktools/masks.py
--rw-r--r--   0 runner    (1001) docker     (123)    15970 2023-06-05 20:25:40.000000 vsmasktools-1.1.1/vsmasktools/morpho.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:25:40.000000 vsmasktools-1.1.1/vsmasktools/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-05 20:25:40.000000 vsmasktools-1.1.1/vsmasktools/spat_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-05 20:25:40.000000 vsmasktools-1.1.1/vsmasktools/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    10974 2023-06-05 20:25:40.000000 vsmasktools-1.1.1/vsmasktools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:26:01.295195 vsmasktools-1.1.1/vsmasktools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-05 20:26:01.000000 vsmasktools-1.1.1/vsmasktools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-05 20:26:01.000000 vsmasktools-1.1.1/vsmasktools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 20:26:01.000000 vsmasktools-1.1.1/vsmasktools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-05 20:26:01.000000 vsmasktools-1.1.1/vsmasktools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-05 20:26:01.000000 vsmasktools-1.1.1/vsmasktools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:34:44.052926 vsmasktools-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-20 14:34:18.000000 vsmasktools-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-20 14:34:44.052926 vsmasktools-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-20 14:34:18.000000 vsmasktools-1.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-20 14:34:44.052926 vsmasktools-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-20 14:34:18.000000 vsmasktools-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:34:44.048926 vsmasktools-1.1.2/vsmasktools/
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-20 14:34:18.000000 vsmasktools-1.1.2/vsmasktools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-20 14:34:18.000000 vsmasktools-1.1.2/vsmasktools/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-06-20 14:34:18.000000 vsmasktools-1.1.2/vsmasktools/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-06-20 14:34:18.000000 vsmasktools-1.1.2/vsmasktools/details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-06-20 14:34:18.000000 vsmasktools-1.1.2/vsmasktools/diff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:34:44.052926 vsmasktools-1.1.2/vsmasktools/edge/
+-rw-r--r--   0 runner    (1001) docker     (123)    30484 2023-06-20 14:34:18.000000 vsmasktools-1.1.2/vsmasktools/edge/_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-20 14:34:18.000000 vsmasktools-1.1.2/vsmasktools/edge/_2x2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9752 2023-06-20 14:34:18.000000 vsmasktools-1.1.2/vsmasktools/edge/_3x3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-06-20 14:34:18.000000 vsmasktools-1.1.2/vsmasktools/edge/_5x5.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-20 14:34:18.000000 vsmasktools-1.1.2/vsmasktools/edge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16268 2023-06-20 14:34:18.000000 vsmasktools-1.1.2/vsmasktools/edge/_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-06-20 14:34:18.000000 vsmasktools-1.1.2/vsmasktools/edge_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-20 14:34:18.000000 vsmasktools-1.1.2/vsmasktools/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12259 2023-06-20 14:34:18.000000 vsmasktools-1.1.2/vsmasktools/hardsub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-20 14:34:18.000000 vsmasktools-1.1.2/vsmasktools/masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15970 2023-06-20 14:34:18.000000 vsmasktools-1.1.2/vsmasktools/morpho.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:34:18.000000 vsmasktools-1.1.2/vsmasktools/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-06-20 14:34:18.000000 vsmasktools-1.1.2/vsmasktools/spat_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-20 14:34:18.000000 vsmasktools-1.1.2/vsmasktools/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10974 2023-06-20 14:34:18.000000 vsmasktools-1.1.2/vsmasktools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:34:44.052926 vsmasktools-1.1.2/vsmasktools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-20 14:34:44.000000 vsmasktools-1.1.2/vsmasktools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-20 14:34:44.000000 vsmasktools-1.1.2/vsmasktools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 14:34:44.000000 vsmasktools-1.1.2/vsmasktools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-20 14:34:44.000000 vsmasktools-1.1.2/vsmasktools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-20 14:34:44.000000 vsmasktools-1.1.2/vsmasktools.egg-info/top_level.txt
```

### Comparing `vsmasktools-1.1.1/LICENSE` & `vsmasktools-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vsmasktools-1.1.1/PKG-INFO` & `vsmasktools-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsmasktools
-Version: 1.1.1
+Version: 1.1.2
 Summary: Various masking tools for VapourSynth
 Author: Irrational Encoding Wizardry
 Author-email: wizards@encode.moe
 Maintainer: Irrational Encoding Wizardry
 Maintainer-email: wizards@encode.moe
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-masktools
 Project-URL: Documentation, https://vsmasktools.encode.moe/en/latest/
```

### Comparing `vsmasktools-1.1.1/README.md` & `vsmasktools-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `vsmasktools-1.1.1/setup.cfg` & `vsmasktools-1.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `vsmasktools-1.1.1/setup.py` & `vsmasktools-1.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `vsmasktools-1.1.1/vsmasktools/__init__.py` & `vsmasktools-1.1.2/vsmasktools/__init__.py`

 * *Files identical despite different names*

### Comparing `vsmasktools-1.1.1/vsmasktools/abstract.py` & `vsmasktools-1.1.2/vsmasktools/abstract.py`

 * *Files identical despite different names*

### Comparing `vsmasktools-1.1.1/vsmasktools/details.py` & `vsmasktools-1.1.2/vsmasktools/details.py`

 * *Files identical despite different names*

### Comparing `vsmasktools-1.1.1/vsmasktools/diff.py` & `vsmasktools-1.1.2/vsmasktools/diff.py`

 * *Files identical despite different names*

### Comparing `vsmasktools-1.1.1/vsmasktools/edge/_1d.py` & `vsmasktools-1.1.2/vsmasktools/edge/_1d.py`

 * *Files identical despite different names*

### Comparing `vsmasktools-1.1.1/vsmasktools/edge/_3x3.py` & `vsmasktools-1.1.2/vsmasktools/edge/_3x3.py`

 * *Files identical despite different names*

### Comparing `vsmasktools-1.1.1/vsmasktools/edge/_5x5.py` & `vsmasktools-1.1.2/vsmasktools/edge/_5x5.py`

 * *Files identical despite different names*

### Comparing `vsmasktools-1.1.1/vsmasktools/edge/_abstract.py` & `vsmasktools-1.1.2/vsmasktools/edge/_abstract.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 
 from abc import ABC, abstractmethod
 from enum import Enum, IntFlag, auto
 from typing import Any, ClassVar, NoReturn, Sequence, TypeAlias
 
 from vsexprtools import ExprOp, ExprToken, norm_expr
 from vstools import (
-    ColorRange, CustomRuntimeError, CustomValueError, FuncExceptT, PlanesT, T, check_variable, core, get_lowest_values,
-    get_peak_value, get_peak_values, get_subclasses, inject_self, join, normalize_planes, plane, scale_value, vs
+    ColorRange, CustomRuntimeError, CustomValueError, FuncExceptT, KwargsT, PlanesT, T, check_variable, core,
+    get_lowest_values, get_peak_value, get_peak_values, get_subclasses, inject_self, join, normalize_planes, plane,
+    scale_value, vs
 )
 
 from ..exceptions import UnknownEdgeDetectError, UnknownRidgeDetectError
 
 __all__ = [
     'EdgeDetect', 'EdgeDetectT',
     'RidgeDetect', 'RidgeDetectT',
@@ -124,14 +125,16 @@
 
         return new_edge_detect
 
 
 class EdgeDetect(ABC):
     """Abstract edge detection interface."""
 
+    kwargs: KwargsT | None = None
+
     def __init__(self, **kwargs: Any) -> None:
         super().__init__()
 
         self.kwargs = kwargs
 
     @classmethod
     def from_param(
@@ -171,15 +174,16 @@
         lthr: float = 0.0, hthr: float | None = None,
         multi: float = 1.0,
         clamp: bool | tuple[float, float] | list[tuple[float, float]] = False,
         feature: _Feature = _Feature.EDGE, planes: PlanesT | tuple[PlanesT, bool] = None, **kwargs: Any
     ) -> vs.VideoNode:
         assert check_variable(clip, self.__class__)
 
-        kwargs = self.kwargs | kwargs
+        if self.kwargs:
+            kwargs = self.kwargs | kwargs
 
         peak = get_peak_value(clip)
         hthr = 1.0 if hthr is None else hthr
 
         lthr, hthr = scale_value(lthr, 32, clip), scale_value(hthr, 32, clip)
 
         discard_planes = False
```

### Comparing `vsmasktools-1.1.1/vsmasktools/edge_funcs.py` & `vsmasktools-1.1.2/vsmasktools/edge_funcs.py`

 * *Files identical despite different names*

### Comparing `vsmasktools-1.1.1/vsmasktools/exceptions.py` & `vsmasktools-1.1.2/vsmasktools/exceptions.py`

 * *Files identical despite different names*

### Comparing `vsmasktools-1.1.1/vsmasktools/hardsub.py` & `vsmasktools-1.1.2/vsmasktools/hardsub.py`

 * *Files identical despite different names*

### Comparing `vsmasktools-1.1.1/vsmasktools/masks.py` & `vsmasktools-1.1.2/vsmasktools/masks.py`

 * *Files identical despite different names*

### Comparing `vsmasktools-1.1.1/vsmasktools/morpho.py` & `vsmasktools-1.1.2/vsmasktools/morpho.py`

 * *Files identical despite different names*

### Comparing `vsmasktools-1.1.1/vsmasktools/spat_funcs.py` & `vsmasktools-1.1.2/vsmasktools/spat_funcs.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 from __future__ import annotations
 
 from typing import Sequence, overload
 
 from vsexprtools import ExprOp, ExprVars, complexpr_available, norm_expr
 from vsrgtools import box_blur, gauss_blur
 from vstools import (
-    ColorRange, CustomRuntimeError, DitherType, FuncExceptT, StrList, check_variable, core, depth, get_lowest_value,
-    get_peak_value, get_sample_type, get_y, plane, scale_value, vs
+    ColorRange, CustomRuntimeError, DitherType, FuncExceptT, StrList, check_variable, core, depth, fallback,
+    get_lowest_value, get_peak_value, get_sample_type, get_y, plane, scale_8bit, scale_value, vs
 )
 
+from .edge import MinMax
+from .morpho import Morpho
+
 __all__ = [
     'adg_mask',
     'retinex',
-    'flat_mask'
+    'flat_mask',
+    'texture_mask'
 ]
 
 
 @overload
 def adg_mask(  # type: ignore
     clip: vs.VideoNode, luma_scaling: float = 8.0, relative: bool = False, func: FuncExceptT | None = None
 ) -> vs.VideoNode:
@@ -143,7 +147,49 @@
     luma = get_y(src)
 
     blur = gauss_blur(luma, radius * 0.361083333) if gauss else box_blur(luma, radius)
 
     mask = depth(luma, 8).abrz.AdaptiveBinarize(depth(blur, 8), scale_value(thr, 32, 8))
 
     return depth(mask, luma, dither_type=DitherType.NONE, range_in=ColorRange.FULL, range_out=ColorRange.FULL)
+
+
+def texture_mask(
+    clip: vs.VideoNode, rady: int = 2, radc: int | None = None,
+    blur: int | float = 8, thr: float = 0.2,
+    stages: list[tuple[int, int]] = [(60, 2), (40, 4), (20, 2)],
+    points: list[tuple[bool, float]] = [(False, 1.75), (True, 2.5), (True, 5), (False, 10)]
+) -> vs.VideoNode:
+    levels = [x for x, _ in points]
+    _points = [scale_value(x, 8, clip) for _, x in points]
+
+    qm, peak = len(points), get_peak_value(clip)
+
+    rmask = MinMax(rady, fallback(radc, rady)).edgemask(clip, lthr=0)
+
+    emask = clip.std.Prewitt()
+
+    rm_txt = ExprOp.MIN(rmask, (
+        Morpho.minimum(Morpho.binarize(emask, scale_8bit(32, thr), 1.0, 0), iterations=it)
+        for thr, it in stages
+    ))
+
+    expr = [f'x {_points[0]} < x {_points[-1]} > or 0']
+
+    for x in range(len(_points) - 1):
+        if _points[x + 1] < _points[-1]:
+            expr.append(f'x {_points[x+1]} <=')
+
+        if levels[x] == levels[x + 1]:
+            expr.append(f'{peak if levels[x] else 0}')
+        else:
+            mean = peak * (levels[x + 1] - levels[x]) / (_points[x + 1] - _points[x])
+            expr.append(f'x {_points[x]} - {mean} * {peak * levels[x]} +')
+
+    weighted = norm_expr(rm_txt, [expr, ExprOp.TERN * (qm - 1)])
+
+    if isinstance(blur, float):
+        weighted = gauss_blur(weighted, blur)
+    else:
+        weighted = box_blur(weighted, blur)
+
+    return norm_expr(weighted, f'x {peak * thr} - {1 / (1 - thr)} *')
```

### Comparing `vsmasktools-1.1.1/vsmasktools/types.py` & `vsmasktools-1.1.2/vsmasktools/types.py`

 * *Files identical despite different names*

### Comparing `vsmasktools-1.1.1/vsmasktools/utils.py` & `vsmasktools-1.1.2/vsmasktools/utils.py`

 * *Files identical despite different names*

### Comparing `vsmasktools-1.1.1/vsmasktools.egg-info/PKG-INFO` & `vsmasktools-1.1.2/vsmasktools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsmasktools
-Version: 1.1.1
+Version: 1.1.2
 Summary: Various masking tools for VapourSynth
 Author: Irrational Encoding Wizardry
 Author-email: wizards@encode.moe
 Maintainer: Irrational Encoding Wizardry
 Maintainer-email: wizards@encode.moe
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-masktools
 Project-URL: Documentation, https://vsmasktools.encode.moe/en/latest/
```

### Comparing `vsmasktools-1.1.1/vsmasktools.egg-info/SOURCES.txt` & `vsmasktools-1.1.2/vsmasktools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

