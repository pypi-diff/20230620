# Comparing `tmp/array_api_compat-1.2.tar.gz` & `tmp/array_api_compat-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "array_api_compat-1.2.tar", last modified: Mon Apr  3 20:48:01 2023, max compression
+gzip compressed data, was "array_api_compat-1.3.tar", last modified: Tue Jun 20 18:05:58 2023, max compression
```

## Comparing `array_api_compat-1.2.tar` & `array_api_compat-1.3.tar`

### file list

```diff
@@ -1,35 +1,40 @@
-drwxr-xr-x   0 aaronmeurer   (501) staff       (20)        0 2023-04-03 20:48:01.975062 array_api_compat-1.2/
--rw-r--r--   0 aaronmeurer   (501) staff       (20)     1097 2022-09-26 22:13:49.000000 array_api_compat-1.2/LICENSE
--rw-r--r--   0 aaronmeurer   (501) staff       (20)    12926 2023-04-03 20:48:01.974682 array_api_compat-1.2/PKG-INFO
--rw-r--r--   0 aaronmeurer   (501) staff       (20)    12393 2023-03-11 07:06:20.000000 array_api_compat-1.2/README.md
-drwxr-xr-x   0 aaronmeurer   (501) staff       (20)        0 2023-04-03 20:48:01.962661 array_api_compat-1.2/array_api_compat/
--rw-r--r--   0 aaronmeurer   (501) staff       (20)      944 2023-03-31 22:44:32.000000 array_api_compat-1.2/array_api_compat/__init__.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)      987 2022-12-05 23:02:55.000000 array_api_compat-1.2/array_api_compat/_internal.py
-drwxr-xr-x   0 aaronmeurer   (501) staff       (20)        0 2023-04-03 20:48:01.967604 array_api_compat-1.2/array_api_compat/common/
--rw-r--r--   0 aaronmeurer   (501) staff       (20)       24 2022-12-05 23:02:55.000000 array_api_compat-1.2/array_api_compat/common/__init__.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)    15799 2023-03-21 21:19:45.000000 array_api_compat-1.2/array_api_compat/common/_aliases.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)     8122 2023-03-11 07:06:20.000000 array_api_compat-1.2/array_api_compat/common/_helpers.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)     5889 2023-03-06 20:47:39.000000 array_api_compat-1.2/array_api_compat/common/_linalg.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)      388 2022-12-05 23:02:55.000000 array_api_compat-1.2/array_api_compat/common/_typing.py
-drwxr-xr-x   0 aaronmeurer   (501) staff       (20)        0 2023-04-03 20:48:01.970238 array_api_compat-1.2/array_api_compat/cupy/
--rw-r--r--   0 aaronmeurer   (501) staff       (20)      397 2023-03-21 21:19:45.000000 array_api_compat-1.2/array_api_compat/cupy/__init__.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)     2297 2023-03-21 21:19:45.000000 array_api_compat-1.2/array_api_compat/cupy/_aliases.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)      617 2022-12-05 23:02:55.000000 array_api_compat-1.2/array_api_compat/cupy/_typing.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)     1125 2023-03-06 20:47:39.000000 array_api_compat-1.2/array_api_compat/cupy/linalg.py
-drwxr-xr-x   0 aaronmeurer   (501) staff       (20)        0 2023-04-03 20:48:01.972366 array_api_compat-1.2/array_api_compat/numpy/
--rw-r--r--   0 aaronmeurer   (501) staff       (20)      596 2022-12-05 23:02:55.000000 array_api_compat-1.2/array_api_compat/numpy/__init__.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)     2301 2023-03-21 21:19:45.000000 array_api_compat-1.2/array_api_compat/numpy/_aliases.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)      618 2022-12-05 23:02:55.000000 array_api_compat-1.2/array_api_compat/numpy/_typing.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)      956 2023-03-17 23:19:38.000000 array_api_compat-1.2/array_api_compat/numpy/linalg.py
-drwxr-xr-x   0 aaronmeurer   (501) staff       (20)        0 2023-04-03 20:48:01.973981 array_api_compat-1.2/array_api_compat/torch/
--rw-r--r--   0 aaronmeurer   (501) staff       (20)      518 2023-03-21 21:19:45.000000 array_api_compat-1.2/array_api_compat/torch/__init__.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)    24987 2023-03-21 21:19:45.000000 array_api_compat-1.2/array_api_compat/torch/_aliases.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)     2099 2023-03-31 22:38:34.000000 array_api_compat-1.2/array_api_compat/torch/linalg.py
-drwxr-xr-x   0 aaronmeurer   (501) staff       (20)        0 2023-04-03 20:48:01.964679 array_api_compat-1.2/array_api_compat.egg-info/
--rw-r--r--   0 aaronmeurer   (501) staff       (20)    12926 2023-04-03 20:48:01.000000 array_api_compat-1.2/array_api_compat.egg-info/PKG-INFO
--rw-r--r--   0 aaronmeurer   (501) staff       (20)      835 2023-04-03 20:48:01.000000 array_api_compat-1.2/array_api_compat.egg-info/SOURCES.txt
--rw-r--r--   0 aaronmeurer   (501) staff       (20)        1 2023-04-03 20:48:01.000000 array_api_compat-1.2/array_api_compat.egg-info/dependency_links.txt
--rw-r--r--   0 aaronmeurer   (501) staff       (20)       28 2023-04-03 20:48:01.000000 array_api_compat-1.2/array_api_compat.egg-info/requires.txt
--rw-r--r--   0 aaronmeurer   (501) staff       (20)       17 2023-04-03 20:48:01.000000 array_api_compat-1.2/array_api_compat.egg-info/top_level.txt
--rw-r--r--   0 aaronmeurer   (501) staff       (20)       38 2023-04-03 20:48:01.975171 array_api_compat-1.2/setup.cfg
--rw-r--r--   0 aaronmeurer   (501) staff       (20)      859 2023-01-02 23:36:35.000000 array_api_compat-1.2/setup.py
+drwxr-xr-x   0 aaronmeurer   (501) staff       (20)        0 2023-06-20 18:05:58.540820 array_api_compat-1.3/
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)     1097 2022-09-26 22:13:49.000000 array_api_compat-1.3/LICENSE
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)    12723 2023-06-20 18:05:58.540493 array_api_compat-1.3/PKG-INFO
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)    12190 2023-06-20 17:59:02.000000 array_api_compat-1.3/README.md
+drwxr-xr-x   0 aaronmeurer   (501) staff       (20)        0 2023-06-20 18:05:58.528658 array_api_compat-1.3/array_api_compat/
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)      944 2023-06-20 18:00:17.000000 array_api_compat-1.3/array_api_compat/__init__.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)      987 2022-12-05 23:02:55.000000 array_api_compat-1.3/array_api_compat/_internal.py
+drwxr-xr-x   0 aaronmeurer   (501) staff       (20)        0 2023-06-20 18:05:58.532442 array_api_compat-1.3/array_api_compat/common/
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)       24 2022-12-05 23:02:55.000000 array_api_compat-1.3/array_api_compat/common/__init__.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)    16001 2023-06-20 16:24:09.000000 array_api_compat-1.3/array_api_compat/common/_aliases.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)     8312 2023-06-16 22:26:06.000000 array_api_compat-1.3/array_api_compat/common/_helpers.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)     6073 2023-06-20 16:24:09.000000 array_api_compat-1.3/array_api_compat/common/_linalg.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)      388 2022-12-05 23:02:55.000000 array_api_compat-1.3/array_api_compat/common/_typing.py
+drwxr-xr-x   0 aaronmeurer   (501) staff       (20)        0 2023-06-20 18:05:58.534255 array_api_compat-1.3/array_api_compat/cupy/
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)      397 2023-06-20 16:24:09.000000 array_api_compat-1.3/array_api_compat/cupy/__init__.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)     2297 2023-03-21 21:19:45.000000 array_api_compat-1.3/array_api_compat/cupy/_aliases.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)      617 2022-12-05 23:02:55.000000 array_api_compat-1.3/array_api_compat/cupy/_typing.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)     1125 2023-03-06 20:47:39.000000 array_api_compat-1.3/array_api_compat/cupy/linalg.py
+drwxr-xr-x   0 aaronmeurer   (501) staff       (20)        0 2023-06-20 18:05:58.536174 array_api_compat-1.3/array_api_compat/numpy/
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)      596 2023-06-20 16:24:09.000000 array_api_compat-1.3/array_api_compat/numpy/__init__.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)     2301 2023-03-21 21:19:45.000000 array_api_compat-1.3/array_api_compat/numpy/_aliases.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)      618 2022-12-05 23:02:55.000000 array_api_compat-1.3/array_api_compat/numpy/_typing.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)      956 2023-03-17 23:19:38.000000 array_api_compat-1.3/array_api_compat/numpy/linalg.py
+drwxr-xr-x   0 aaronmeurer   (501) staff       (20)        0 2023-06-20 18:05:58.537483 array_api_compat-1.3/array_api_compat/torch/
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)      518 2023-06-20 16:24:09.000000 array_api_compat-1.3/array_api_compat/torch/__init__.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)    26377 2023-06-20 16:24:09.000000 array_api_compat-1.3/array_api_compat/torch/_aliases.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)     2099 2023-03-31 22:38:34.000000 array_api_compat-1.3/array_api_compat/torch/linalg.py
+drwxr-xr-x   0 aaronmeurer   (501) staff       (20)        0 2023-06-20 18:05:58.530661 array_api_compat-1.3/array_api_compat.egg-info/
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)    12723 2023-06-20 18:05:58.000000 array_api_compat-1.3/array_api_compat.egg-info/PKG-INFO
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)      932 2023-06-20 18:05:58.000000 array_api_compat-1.3/array_api_compat.egg-info/SOURCES.txt
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)        1 2023-06-20 18:05:58.000000 array_api_compat-1.3/array_api_compat.egg-info/dependency_links.txt
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)       28 2023-06-20 18:05:58.000000 array_api_compat-1.3/array_api_compat.egg-info/requires.txt
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)       17 2023-06-20 18:05:58.000000 array_api_compat-1.3/array_api_compat.egg-info/top_level.txt
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)       38 2023-06-20 18:05:58.540913 array_api_compat-1.3/setup.cfg
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)      859 2023-01-02 23:36:35.000000 array_api_compat-1.3/setup.py
+drwxr-xr-x   0 aaronmeurer   (501) staff       (20)        0 2023-06-20 18:05:58.539855 array_api_compat-1.3/tests/
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)     1322 2023-05-02 22:44:40.000000 array_api_compat-1.3/tests/test_array_namespace.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)      914 2023-06-16 22:26:06.000000 array_api_compat-1.3/tests/test_common.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)     3584 2023-03-21 21:19:45.000000 array_api_compat-1.3/tests/test_isdtype.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)      404 2023-03-06 20:47:39.000000 array_api_compat-1.3/tests/test_vendoring.py
```

### Comparing `array_api_compat-1.2/LICENSE` & `array_api_compat-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.2/PKG-INFO` & `array_api_compat-1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: array_api_compat
-Version: 1.2
+Version: 1.3
 Summary: A wrapper around NumPy and other array libraries to make them compatible with the Array API standard
 Home-page: https://data-apis.org/array-api-compat/
 Author: Consortium for Python Data API Standards
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,19 +23,16 @@
 
 Note that some of the functionality in this library is backwards incompatible
 with the corresponding wrapped libraries. The end-goal is to eventually make
 each array library itself fully compatible with the array API, but this
 requires making backwards incompatible changes in many cases, so this will
 take some time.
 
-Currently all libraries here are implemented against the 2021.12 version of
-the standard. Support for the [2022.12
-version](https://data-apis.org/array-api/2022.12/changelog.html), which adds
-complex number support as well as several additional functions, will be added
-later this year.
+Currently all libraries here are implemented against the [2022.22
+version](https://data-apis.org/array-api/2022.22/) of the standard.
 
 ## Usage
 
 The typical usage of this library will be to get the corresponding array API
 compliant namespace from the input arrays using `array_namespace()`, like
 
 ```py
@@ -188,16 +185,14 @@
 
 - The `x.size` attribute on `torch.Tensor` is a function that behaves
   differently from
   [`x.size`](https://data-apis.org/array-api/draft/API_specification/generated/array_api.array.size.html)
   in the spec. Use the `size(x)` helper function as a portable workaround (see
   above).
 
-- The `linalg` extension is not yet implemented.
-
 - PyTorch does not have unsigned integer types other than `uint8`, and no
   attempt is made to implement them here.
 
 - PyTorch has type promotion semantics that differ from the array API
   specification for 0-D tensor objects. The array functions in this wrapper
   library do work around this, but the operators on the Tensor object do not,
   as no operators or methods on the Tensor object are modified. If this is a
```

### Comparing `array_api_compat-1.2/README.md` & `array_api_compat-1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,16 @@
 
 Note that some of the functionality in this library is backwards incompatible
 with the corresponding wrapped libraries. The end-goal is to eventually make
 each array library itself fully compatible with the array API, but this
 requires making backwards incompatible changes in many cases, so this will
 take some time.
 
-Currently all libraries here are implemented against the 2021.12 version of
-the standard. Support for the [2022.12
-version](https://data-apis.org/array-api/2022.12/changelog.html), which adds
-complex number support as well as several additional functions, will be added
-later this year.
+Currently all libraries here are implemented against the [2022.22
+version](https://data-apis.org/array-api/2022.22/) of the standard.
 
 ## Usage
 
 The typical usage of this library will be to get the corresponding array API
 compliant namespace from the input arrays using `array_namespace()`, like
 
 ```py
@@ -173,16 +170,14 @@
 
 - The `x.size` attribute on `torch.Tensor` is a function that behaves
   differently from
   [`x.size`](https://data-apis.org/array-api/draft/API_specification/generated/array_api.array.size.html)
   in the spec. Use the `size(x)` helper function as a portable workaround (see
   above).
 
-- The `linalg` extension is not yet implemented.
-
 - PyTorch does not have unsigned integer types other than `uint8`, and no
   attempt is made to implement them here.
 
 - PyTorch has type promotion semantics that differ from the array API
   specification for 0-D tensor objects. The array functions in this wrapper
   library do work around this, but the operators on the Tensor object do not,
   as no operators or methods on the Tensor object are modified. If this is a
```

### Comparing `array_api_compat-1.2/array_api_compat/__init__.py` & `array_api_compat-1.3/array_api_compat/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,10 +13,10 @@
 separate Array object, but rather just uses numpy.ndarray directly.
 
 Library authors using the Array API may wish to test against numpy.array_api
 to ensure they are not using functionality outside of the standard, but prefer
 this implementation for the default when working with NumPy arrays.
 
 """
-__version__ = '1.2'
+__version__ = '1.3'
 
 from .common import *
```

### Comparing `array_api_compat-1.2/array_api_compat/_internal.py` & `array_api_compat-1.3/array_api_compat/_internal.py`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.2/array_api_compat/common/_aliases.py` & `array_api_compat-1.3/array_api_compat/common/_aliases.py`

 * *Files 2% similar despite different names*

```diff
@@ -327,25 +327,26 @@
             copy = True
         if copy in COPY_TRUE:
             return xp.array(obj, copy=True, dtype=dtype)
         return obj
 
     return xp.asarray(obj, dtype=dtype, **kwargs)
 
-# xp.reshape calls the keyword argument 'newshape' instead of 'shape'
+# np.reshape calls the keyword argument 'newshape' instead of 'shape'
 def reshape(x: ndarray,
             /,
             shape: Tuple[int, ...],
             xp, copy: Optional[bool] = None,
             **kwargs) -> ndarray:
     if copy is True:
         x = x.copy()
     elif copy is False:
-        x.shape = shape
-        return x
+        y = x.view()
+        y.shape = shape
+        return y
     return xp.reshape(x, shape, **kwargs)
 
 # The descending keyword is new in sort and argsort, and 'kind' replaced with
 # 'stable'
 def argsort(
     x: ndarray, /, xp, *, axis: int = -1, descending: bool = False, stable: bool = True,
     **kwargs,
@@ -392,31 +393,37 @@
     xp,
     *,
     axis: Optional[Union[int, Tuple[int, ...]]] = None,
     dtype: Optional[Dtype] = None,
     keepdims: bool = False,
     **kwargs,
 ) -> ndarray:
-    # `xp.sum` already upcasts integers, but not floats
-    if dtype is None and x.dtype == xp.float32:
-        dtype = xp.float64
+    # `xp.sum` already upcasts integers, but not floats or complexes
+    if dtype is None:
+        if x.dtype == xp.float32:
+            dtype = xp.float64
+        elif x.dtype == xp.complex64:
+            dtype = xp.complex128
     return xp.sum(x, axis=axis, dtype=dtype, keepdims=keepdims, **kwargs)
 
 def prod(
     x: ndarray,
     /,
     xp,
     *,
     axis: Optional[Union[int, Tuple[int, ...]]] = None,
     dtype: Optional[Dtype] = None,
     keepdims: bool = False,
     **kwargs,
 ) -> ndarray:
-    if dtype is None and x.dtype == xp.float32:
-        dtype = xp.float64
+    if dtype is None:
+        if x.dtype == xp.float32:
+            dtype = xp.float64
+        elif x.dtype == xp.complex64:
+            dtype = xp.complex128
     return xp.prod(x, dtype=dtype, axis=axis, keepdims=keepdims, **kwargs)
 
 # ceil, floor, and trunc return integers for integer inputs
 
 def ceil(x: ndarray, /, xp, **kwargs) -> ndarray:
     if xp.issubdtype(x.dtype, xp.integer):
         return x
```

### Comparing `array_api_compat-1.2/array_api_compat/common/_helpers.py` & `array_api_compat-1.3/array_api_compat/common/_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,14 +150,19 @@
     import cupy as cp
     from cupy.cuda import Device as _Device
     from cupy.cuda import stream as stream_module
     from cupy_backends.cuda.api import runtime
 
     if device == x.device:
         return x
+    elif device == "cpu":
+        # allowing us to use `to_device(x, "cpu")`
+        # is useful for portable test swapping between
+        # host and device backends
+        return x.get()
     elif not isinstance(device, _Device):
         raise ValueError(f"Unsupported device {device!r}")
     else:
         # see cupy/cupy#5985 for the reason how we handle device/stream here
         prev_device = runtime.getDevice()
         prev_stream: stream_module.Stream = None
         if stream is not None:
```

### Comparing `array_api_compat-1.2/array_api_compat/common/_linalg.py` & `array_api_compat-1.3/array_api_compat/common/_linalg.py`

 * *Files 4% similar despite different names*

```diff
@@ -132,15 +132,20 @@
 
 # xp.diagonal and xp.trace operate on the first two axes whereas these
 # operates on the last two
 
 def diagonal(x: ndarray, /, xp, *, offset: int = 0, **kwargs) -> ndarray:
     return xp.diagonal(x, offset=offset, axis1=-2, axis2=-1, **kwargs)
 
-def trace(x: ndarray, /, xp, *, offset: int = 0, **kwargs) -> ndarray:
-    return xp.asarray(xp.trace(x, offset=offset, axis1=-2, axis2=-1, **kwargs))
+def trace(x: ndarray, /, xp, *, offset: int = 0, dtype=None, **kwargs) -> ndarray:
+    if dtype is None:
+        if x.dtype == xp.float32:
+            dtype = xp.float64
+        elif x.dtype == xp.complex64:
+            dtype = xp.complex128
+    return xp.asarray(xp.trace(x, offset=offset, dtype=dtype, axis1=-2, axis2=-1, **kwargs))
 
 __all__ = ['cross', 'matmul', 'outer', 'tensordot', 'EighResult',
            'QRResult', 'SlogdetResult', 'SVDResult', 'eigh', 'qr', 'slogdet',
            'svd', 'cholesky', 'matrix_rank', 'pinv', 'matrix_norm',
            'matrix_transpose', 'svdvals', 'vecdot', 'vector_norm', 'diagonal',
            'trace']
```

### Comparing `array_api_compat-1.2/array_api_compat/cupy/_aliases.py` & `array_api_compat-1.3/array_api_compat/cupy/_aliases.py`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.2/array_api_compat/cupy/_typing.py` & `array_api_compat-1.3/array_api_compat/cupy/_typing.py`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.2/array_api_compat/cupy/linalg.py` & `array_api_compat-1.3/array_api_compat/cupy/linalg.py`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.2/array_api_compat/numpy/__init__.py` & `array_api_compat-1.3/array_api_compat/numpy/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,8 +15,8 @@
 # dynamically so that the library can be vendored.
 __import__(__package__ + '.linalg')
 
 from .linalg import matrix_transpose, vecdot
 
 from ..common._helpers import *
 
-__array_api_version__ = '2021.12'
+__array_api_version__ = '2022.12'
```

### Comparing `array_api_compat-1.2/array_api_compat/numpy/_aliases.py` & `array_api_compat-1.3/array_api_compat/numpy/_aliases.py`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.2/array_api_compat/numpy/_typing.py` & `array_api_compat-1.3/array_api_compat/numpy/_typing.py`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.2/array_api_compat/numpy/linalg.py` & `array_api_compat-1.3/array_api_compat/numpy/linalg.py`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.2/array_api_compat/torch/_aliases.py` & `array_api_compat-1.3/array_api_compat/torch/_aliases.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 }
 
 _array_api_dtypes = {
     torch.bool,
     *_int_dtypes,
     torch.float32,
     torch.float64,
+    torch.complex64,
+    torch.complex128,
 }
 
 _promotion_table  = {
     # bool
     (torch.bool, torch.bool): torch.bool,
     # ints
     (torch.int8, torch.int8): torch.int8,
@@ -66,14 +68,24 @@
     (torch.uint8, torch.int32): torch.int32,
     (torch.uint8, torch.int64): torch.int64,
     # floats
     (torch.float32, torch.float32): torch.float32,
     (torch.float32, torch.float64): torch.float64,
     (torch.float64, torch.float32): torch.float64,
     (torch.float64, torch.float64): torch.float64,
+    # complexes
+    (torch.complex64, torch.complex64): torch.complex64,
+    (torch.complex64, torch.complex128): torch.complex128,
+    (torch.complex128, torch.complex64): torch.complex128,
+    (torch.complex128, torch.complex128): torch.complex128,
+    # Mixed float and complex
+    (torch.float32, torch.complex64): torch.complex64,
+    (torch.float32, torch.complex128): torch.complex128,
+    (torch.float64, torch.complex64): torch.complex128,
+    (torch.float64, torch.complex128): torch.complex128,
 }
 
 
 def _two_arg(f):
     @wraps(f)
     def _f(x1, x2, /, **kwargs):
         x1, x2 = _fix_promotion(x1, x2)
@@ -125,15 +137,14 @@
 
 def can_cast(from_: Union[Dtype, array], to: Dtype, /) -> bool:
     if not isinstance(from_, torch.dtype):
         from_ = from_.dtype
     return torch.can_cast(from_, to)
 
 # Basic renames
-permute_dims = torch.permute
 bitwise_invert = torch.bitwise_not
 
 # Two-arg elementwise functions
 # These require a wrapper to do the correct type promotion on 0-D tensors
 add = _two_arg(torch.add)
 atan2 = _two_arg(torch.atan2)
 bitwise_and = _two_arg(torch.bitwise_and)
@@ -435,34 +446,52 @@
     axes = _normalize_axes(axis, x.ndim)
     # Remove this once pytorch 1.14 is released with the above PR #89017.
     sequence = [a - i for i, a in enumerate(axes)]
     for a in sequence:
         x = torch.squeeze(x, a)
     return x
 
+# torch.broadcast_to uses size instead of shape
+def broadcast_to(x: array, /, shape: Tuple[int, ...], **kwargs) -> array:
+    return torch.broadcast_to(x, shape, **kwargs)
+
+# torch.permute uses dims instead of axes
+def permute_dims(x: array, /, axes: Tuple[int, ...]) -> array:
+    return torch.permute(x, axes)
+
 # The axis parameter doesn't work for flip() and roll()
 # https://github.com/pytorch/pytorch/issues/71210. Also torch.flip() doesn't
 # accept axis=None
-def flip(x: array, /, *, axis: Optional[Union[int, Tuple[int, ...]]] = None) -> array:
+def flip(x: array, /, *, axis: Optional[Union[int, Tuple[int, ...]]] = None, **kwargs) -> array:
     if axis is None:
         axis = tuple(range(x.ndim))
     # torch.flip doesn't accept dim as an int but the method does
     # https://github.com/pytorch/pytorch/issues/18095
-    return x.flip(axis)
+    return x.flip(axis, **kwargs)
 
-def roll(x: array, /, shift: Union[int, Tuple[int, ...]], *, axis: Optional[Union[int, Tuple[int, ...]]] = None) -> array:
-    return torch.roll(x, shift, axis)
+def roll(x: array, /, shift: Union[int, Tuple[int, ...]], *, axis: Optional[Union[int, Tuple[int, ...]]] = None, **kwargs) -> array:
+    return torch.roll(x, shift, axis, **kwargs)
 
 def nonzero(x: array, /, **kwargs) -> Tuple[array, ...]:
     return torch.nonzero(x, as_tuple=True, **kwargs)
 
 def where(condition: array, x1: array, x2: array, /) -> array:
     x1, x2 = _fix_promotion(x1, x2)
     return torch.where(condition, x1, x2)
 
+# torch.reshape doesn't have the copy keyword
+def reshape(x: array,
+            /,
+            shape: Tuple[int, ...],
+            copy: Optional[bool] = None,
+            **kwargs) -> array:
+    if copy is not None:
+        raise NotImplementedError("torch.reshape doesn't yet support the copy keyword")
+    return torch.reshape(x, shape, **kwargs)
+
 # torch.arange doesn't support returning empty arrays
 # (https://github.com/pytorch/pytorch/issues/70915), and doesn't support some
 # keyword argument combinations
 # (https://github.com/pytorch/pytorch/issues/70914)
 def arange(start: Union[int, float],
            /,
            stop: Optional[Union[int, float]] = None,
@@ -648,19 +677,22 @@
         elif kind == 'numeric':
             return isdtype(dtype, ('integral', 'real floating', 'complex floating'))
         else:
             raise ValueError(f"Unrecognized data type kind: {kind!r}")
     else:
         return dtype == kind
 
+def take(x: array, indices: array, /, *, axis: int, **kwargs) -> array:
+    return torch.index_select(x, axis, indices, **kwargs)
+
 __all__ = ['result_type', 'can_cast', 'permute_dims', 'bitwise_invert', 'add',
            'atan2', 'bitwise_and', 'bitwise_left_shift', 'bitwise_or',
            'bitwise_right_shift', 'bitwise_xor', 'divide', 'equal',
            'floor_divide', 'greater', 'greater_equal', 'less', 'less_equal',
            'logaddexp', 'multiply', 'not_equal', 'pow', 'remainder',
            'subtract', 'max', 'min', 'sort', 'prod', 'sum', 'any', 'all',
-           'mean', 'std', 'var', 'concat', 'squeeze', 'flip', 'roll',
-           'nonzero', 'where', 'arange', 'eye', 'linspace', 'full', 'ones',
-           'zeros', 'empty', 'tril', 'triu', 'expand_dims', 'astype',
+           'mean', 'std', 'var', 'concat', 'squeeze', 'broadcast_to', 'flip', 'roll',
+           'nonzero', 'where', 'reshape', 'arange', 'eye', 'linspace', 'full',
+           'ones', 'zeros', 'empty', 'tril', 'triu', 'expand_dims', 'astype',
            'broadcast_arrays', 'unique_all', 'unique_counts',
            'unique_inverse', 'unique_values', 'matmul', 'matrix_transpose',
-           'vecdot', 'tensordot', 'isdtype']
+           'vecdot', 'tensordot', 'isdtype', 'take']
```

### Comparing `array_api_compat-1.2/array_api_compat/torch/linalg.py` & `array_api_compat-1.3/array_api_compat/torch/linalg.py`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.2/array_api_compat.egg-info/PKG-INFO` & `array_api_compat-1.3/array_api_compat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: array-api-compat
-Version: 1.2
+Version: 1.3
 Summary: A wrapper around NumPy and other array libraries to make them compatible with the Array API standard
 Home-page: https://data-apis.org/array-api-compat/
 Author: Consortium for Python Data API Standards
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,19 +23,16 @@
 
 Note that some of the functionality in this library is backwards incompatible
 with the corresponding wrapped libraries. The end-goal is to eventually make
 each array library itself fully compatible with the array API, but this
 requires making backwards incompatible changes in many cases, so this will
 take some time.
 
-Currently all libraries here are implemented against the 2021.12 version of
-the standard. Support for the [2022.12
-version](https://data-apis.org/array-api/2022.12/changelog.html), which adds
-complex number support as well as several additional functions, will be added
-later this year.
+Currently all libraries here are implemented against the [2022.22
+version](https://data-apis.org/array-api/2022.22/) of the standard.
 
 ## Usage
 
 The typical usage of this library will be to get the corresponding array API
 compliant namespace from the input arrays using `array_namespace()`, like
 
 ```py
@@ -188,16 +185,14 @@
 
 - The `x.size` attribute on `torch.Tensor` is a function that behaves
   differently from
   [`x.size`](https://data-apis.org/array-api/draft/API_specification/generated/array_api.array.size.html)
   in the spec. Use the `size(x)` helper function as a portable workaround (see
   above).
 
-- The `linalg` extension is not yet implemented.
-
 - PyTorch does not have unsigned integer types other than `uint8`, and no
   attempt is made to implement them here.
 
 - PyTorch has type promotion semantics that differ from the array API
   specification for 0-D tensor objects. The array functions in this wrapper
   library do work around this, but the operators on the Tensor object do not,
   as no operators or methods on the Tensor object are modified. If this is a
```

### Comparing `array_api_compat-1.2/array_api_compat.egg-info/SOURCES.txt` & `array_api_compat-1.3/array_api_compat.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -19,8 +19,12 @@
 array_api_compat/cupy/linalg.py
 array_api_compat/numpy/__init__.py
 array_api_compat/numpy/_aliases.py
 array_api_compat/numpy/_typing.py
 array_api_compat/numpy/linalg.py
 array_api_compat/torch/__init__.py
 array_api_compat/torch/_aliases.py
-array_api_compat/torch/linalg.py
+array_api_compat/torch/linalg.py
+tests/test_array_namespace.py
+tests/test_common.py
+tests/test_isdtype.py
+tests/test_vendoring.py
```

### Comparing `array_api_compat-1.2/setup.py` & `array_api_compat-1.3/setup.py`

 * *Files identical despite different names*

