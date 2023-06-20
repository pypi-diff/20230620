# Comparing `tmp/ane-1.0.5-py3.10.egg` & `tmp/ane-1.0.6-py3.11.egg`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4098 bytes, number of entries: 8
--rw-r--r--  2.0 unx      123 b- defN 23-Mar-24 13:33 EGG-INFO/PKG-INFO
--rw-r--r--  2.0 unx      158 b- defN 23-Mar-24 13:33 EGG-INFO/SOURCES.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Mar-24 13:33 EGG-INFO/dependency_links.txt
--rw-r--r--  2.0 unx        6 b- defN 23-Mar-24 13:33 EGG-INFO/requires.txt
--rw-r--r--  2.0 unx        4 b- defN 23-Mar-24 13:33 EGG-INFO/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Mar-24 13:33 EGG-INFO/zip-safe
--rw-r--r--  2.0 unx     2404 b- defN 23-Mar-24 09:47 ane/__init__.py
--rw-r--r--  2.0 unx     3899 b- defN 23-Mar-24 13:33 ane/__pycache__/__init__.cpython-310.pyc
-8 files, 6596 bytes uncompressed, 3106 bytes compressed:  52.9%
+Zip file size: 5913 bytes, number of entries: 8
+-rw-r--r--  2.0 unx      123 b- defN 23-Jun-20 14:03 EGG-INFO/PKG-INFO
+-rw-r--r--  2.0 unx      158 b- defN 23-Jun-20 14:03 EGG-INFO/SOURCES.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-20 14:03 EGG-INFO/dependency_links.txt
+-rw-r--r--  2.0 unx       16 b- defN 23-Jun-20 14:03 EGG-INFO/requires.txt
+-rw-r--r--  2.0 unx        4 b- defN 23-Jun-20 14:03 EGG-INFO/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-20 14:03 EGG-INFO/zip-safe
+-rw-r--r--  2.0 unx     2604 b- defN 23-Jun-20 13:59 ane/__init__.py
+-rw-r--r--  2.0 unx     7788 b- defN 23-Jun-20 14:03 ane/__pycache__/__init__.cpython-311.pyc
+8 files, 10695 bytes uncompressed, 4921 bytes compressed:  54.0%
```

## zipnote «TEMP»/diffoscope_q_cgxlbm_/tmp62m819rk_.zip

```diff
@@ -15,11 +15,11 @@
 
 Filename: EGG-INFO/zip-safe
 Comment: 
 
 Filename: ane/__init__.py
 Comment: 
 
-Filename: ane/__pycache__/__init__.cpython-310.pyc
+Filename: ane/__pycache__/__init__.cpython-311.pyc
 Comment: 
 
 Zip file comment:
```

## EGG-INFO/PKG-INFO

```diff
@@ -1,6 +1,6 @@
 Metadata-Version: 2.1
 Name: ane
-Version: 1.0.5
+Version: 1.0.6
 Summary: ANE driver interface
 Author: Eileen Yoon
 Author-email: eyn@gmx.com
```

## EGG-INFO/requires.txt

```diff
@@ -1 +1,2 @@
+construct
 numpy
```

## ane/__init__.py

```diff
@@ -1,51 +1,50 @@
 #!/usr/bin/python3
 
 # SPDX-License-Identifier: MIT
 # Copyright 2022 Eileen Yoon <eyn@gmx.com>
 
-import os
 import atexit
 import ctypes
 import numpy as np
-from ctypes import c_void_p, c_ulong
+from ctypes import c_void_p
+from construct import Struct, Array, Int32ul, Int64ul
 
-class Driver:
-	def __init__(self, path):
-		self.lib = ctypes.cdll.LoadLibrary(path)
+class _Driver:
+	def __init__(self, lib_path):
+		self.lib = ctypes.cdll.LoadLibrary(lib_path)
 		self.lib.pyane_init.restype = c_void_p
+		self.lib.pyane_init.argtypes = [ctypes.c_char_p, ctypes.c_int]
 		self.lib.pyane_free.argtypes = [c_void_p]
 		self.lib.pyane_exec.argtypes = [c_void_p]
 		self.lib.pyane_send.argtypes = [c_void_p] + [c_void_p] * 0x20
 		self.lib.pyane_read.argtypes = [c_void_p] + [c_void_p] * 0x20
-		self.lib.pyane_info.argtypes = [c_void_p] + [ctypes.POINTER(c_ulong)] * (2 + (2 * 0x20 * 6))
 		self.handles = {}
 		atexit.register(self.cleanup)
 
 	def cleanup(self):
 		for handle in self.handles:
 			self.lib.pyane_free(handle)
 
-	def register(self):
-		handle = self.lib.pyane_init()
+	def register(self, path, dev_id):
+		handle = self.lib.pyane_init(path.encode('ascii'), dev_id)
 		if (handle == None): raise RuntimeError("driver error")
 		self.handles[handle] = handle
 		return handle
 
-class Model:
-	def __init__(self, path):
-		self.driver = Driver(os.path.abspath(path))
-		self.handle = self.driver.register()
-		counts, nchws = [c_ulong(), c_ulong()], [c_ulong() for x in range(2 * 0x20 * 6)]
-		self.driver.lib.pyane_info(self.handle, *[ctypes.byref(x) for x in counts + nchws])
-		self.src_count, self.dst_count = counts[0].value, counts[1].value
-		self.src_nchw = tuple([tuple(x.value for x in nchws[n*6:(n+1)*6]) for n in range(self.src_count)])
-		self.dst_nchw = tuple([tuple(x.value for x in nchws[n*6:(n+1)*6]) for n in range(0x20, 0x20 + self.dst_count)])
+class model:
+	def __init__(self, path, dev_id=0, lib_path="/usr/lib/libane_python.so"):
+		self.driver = _Driver(lib_path)
+		self.handle = self.driver.register(path, dev_id)
+		fmt = Struct("size" / Int64ul,"td_size" / Int32ul, "td_count" / Int32ul, "tsk_size" / Int64ul, "krn_size" / Int64ul, "src_count" / Int32ul, "dst_count" / Int32ul, "tiles" / Array(0x20, Int32ul), "nchw" / Array(0x20 * 6, Int64ul))
+		res = fmt.parse(open(path, "rb").read()[:fmt.sizeof()])
+		self.src_count, self.dst_count = res.src_count, res.dst_count
+		self.dst_nchw, self.src_nchw = [tuple([tuple(x for x in res.nchw[(base+n)*6:(base+n+1)*6]) for n in range(count)]) for (base, count) in ((4, res.dst_count), (4 + res.dst_count, res.src_count))]
 		self.outputs = [ctypes.create_string_buffer(((nchw[0]*nchw[1]*nchw[4]) + 0x3fff) & -0x4000) for nchw in self.dst_nchw]
-		self.inputs_pad, self.outputs_pad = [b''] * (0x20 - self.src_count), [b''] * (0x20 - self.dst_count)
+		self.inputs_pad, self.outputs_pad = [b''] * (0x20 - res.src_count), [b''] * (0x20 - res.dst_count)
 
 	def predict(self, inarrs):  # list of numpy arrays
 		assert(len(inarrs) == self.src_count)
 		assert(all(((arr.dtype == np.float16) and (arr.shape == self.src_nchw[idx][:4])) for idx,arr in enumerate(inarrs)))
 		self.driver.lib.pyane_send(self.handle, *[arr.tobytes(order='C') for arr in inarrs], *self.inputs_pad)
 		self.driver.lib.pyane_exec(self.handle)
 		self.driver.lib.pyane_read(self.handle, *self.outputs, *self.outputs_pad)
```

