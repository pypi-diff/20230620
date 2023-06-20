# Comparing `tmp/subplots_from_axsize-0.1.1.tar.gz` & `tmp/subplots_from_axsize-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subplots_from_axsize-0.1.1.tar", max compression
+gzip compressed data, was "subplots_from_axsize-0.1.3.tar", max compression
```

## Comparing `subplots_from_axsize-0.1.1.tar` & `subplots_from_axsize-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1505 2023-06-15 13:41:52.549659 subplots_from_axsize-0.1.1/LICENSE
--rw-r--r--   0        0        0       77 2023-06-17 17:56:09.932773 subplots_from_axsize-0.1.1/README.md
--rw-r--r--   0        0        0      396 2023-06-19 09:07:28.921701 subplots_from_axsize-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       76 2023-06-15 14:07:27.491712 subplots_from_axsize-0.1.1/src/subplots_from_axsize/__init__.py
--rw-r--r--   0        0        0     2954 2023-06-17 17:53:53.828390 subplots_from_axsize-0.1.1/src/subplots_from_axsize/_subplots_from_axsize.py
--rw-r--r--   0        0        0      623 1970-01-01 00:00:00.000000 subplots_from_axsize-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1505 2023-06-15 13:41:52.549659 subplots_from_axsize-0.1.3/LICENSE
+-rw-r--r--   0        0        0       77 2023-06-17 17:56:09.932773 subplots_from_axsize-0.1.3/README.md
+-rw-r--r--   0        0        0      394 2023-06-20 21:28:01.922554 subplots_from_axsize-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       76 2023-06-15 14:07:27.491712 subplots_from_axsize-0.1.3/src/subplots_from_axsize/__init__.py
+-rw-r--r--   0        0        0     3221 2023-06-20 21:28:49.176177 subplots_from_axsize-0.1.3/src/subplots_from_axsize/_subplots_from_axsize.py
+-rw-r--r--   0        0        0      619 1970-01-01 00:00:00.000000 subplots_from_axsize-0.1.3/PKG-INFO
```

### Comparing `subplots_from_axsize-0.1.1/LICENSE` & `subplots_from_axsize-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `subplots_from_axsize-0.1.1/src/subplots_from_axsize/_subplots_from_axsize.py` & `subplots_from_axsize-0.1.3/src/subplots_from_axsize/_subplots_from_axsize.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Implementation of subplots_from_axsize()"""
 
 from collections.abc import Iterable
+from typing import Optional, Tuple, Union
 
 import matplotlib.pyplot as plt
 import mpl_toolkits.axes_grid1 as ag
 import numpy as np
 
 
 def _list_or_float(x):
@@ -20,20 +21,25 @@
 
     n1 = int(n) if n is not None else None
     n2 = len(axs) if isinstance(axs, list) else None
     n3 = len(ds) + 1 if isinstance(ds, list) else None
 
     ns = {n1, n2, n3} - {None}
 
-    assert len(ns) < 2, f"Inconsistent {row_or_col} count.\n{n = }, {axs = }, {ds = }"
+    assert len(ns) < 2, (
+        f"Inconsistent {row_or_col} count.\n"
+        f"declared: {n}\n"
+        f"ax sizes: {axs}\n"
+        f"spaces: {ds}"
+    )
 
     if len(ns) == 0:
         n = 1
     else:
-        n, = ns
+        (n,) = ns
         assert isinstance(n, int)
 
     if not isinstance(axs, list):
         assert isinstance(axs, float)
         axs = n * [axs]
 
     if not isinstance(ds, list):
@@ -44,36 +50,32 @@
 
 
 def _make_sizes(start, axs, end, spaces):
     n = len(axs)
     assert len(spaces) == n - 1
 
     # interleave ax sizes and spaces
-    ds = [start] + [
-        l
-        for pair in zip(axs, spaces + [end])  # same lengths!
-        for l in pair
-    ]
+    ds = [start] + [l for pair in zip(axs, spaces + [end]) for l in pair]
 
     sizes = [ag.Size.Fixed(d) for d in ds]
 
     return sizes, sum(ds)
 
 
 def subplots_from_axsize(
-    axsize=(3, 2),
-    nrows=None,
-    ncols=None,
-    top=0.1,
-    bottom=0.5,
-    left=0.5,
-    right=0.1,
-    hspace=0.5,
-    wspace=0.5,
-    squeeze=True,
+    nrows: Optional[int] = None,
+    ncols: Optional[int] = None,
+    axsize: Tuple[Union[float, list[float]], Union[float, list[float]]] = (4, 3),
+    top: float = 0.1,
+    bottom: float = 0.5,
+    left: float = 0.6,
+    right: float = 0.2,
+    hspace: Union[float, list[float]] = 0.5,
+    wspace: Union[float, list[float]] = 0.5,
+    squeeze: bool = True,
 ):
     """
     Similar to plt.subplots() but uses fixed instead of relative sizes.
     This allows for more control over the final axes sizes.
 
     Examples:
     fig, axs = subplots_from_axsize(axsize=(3, 2), nrows=2) creates a figure with two axes of size (3, 2)
```

### Comparing `subplots_from_axsize-0.1.1/PKG-INFO` & `subplots_from_axsize-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: subplots-from-axsize
-Version: 0.1.1
+Version: 0.1.3
 Summary: 
 Author: Frederic Grabowski
 Author-email: grabowski.frederic@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
+Requires-Dist: matplotlib (>=3.5,<4.0)
 Requires-Dist: pytest (>=7.3.2,<8.0.0)
 Description-Content-Type: text/markdown
 
 # subplots-from-axsize
 matplotlib subplots() but axsize= instead of figsize=
```

