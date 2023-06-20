# Comparing `tmp/pytket_stim-0.8.0-py3-none-any.whl.zip` & `tmp/pytket_stim-0.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 5764 bytes, number of entries: 9
--rw-r--r--  2.0 unx      834 b- defN 22-Mar-14 12:27 pytket/extensions/stim/__init__.py
--rw-r--r--  2.0 unx       67 b- defN 22-Mar-14 12:33 pytket/extensions/stim/_metadata.py
--rw-r--r--  2.0 unx        0 b- defN 22-Mar-14 12:27 pytket/extensions/stim/py.typed
--rw-r--r--  2.0 unx      713 b- defN 22-Mar-14 12:27 pytket/extensions/stim/backends/__init__.py
--rw-r--r--  2.0 unx     5664 b- defN 22-Mar-14 12:27 pytket/extensions/stim/backends/stim_backend.py
--rw-r--r--  2.0 unx     1435 b- defN 22-Mar-14 12:33 pytket_stim-0.8.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Mar-14 12:33 pytket_stim-0.8.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 22-Mar-14 12:33 pytket_stim-0.8.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      781 b- defN 22-Mar-14 12:33 pytket_stim-0.8.0.dist-info/RECORD
-9 files, 9593 bytes uncompressed, 4390 bytes compressed:  54.2%
+Zip file size: 5763 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      834 b- defN 22-Apr-12 12:55 pytket/extensions/stim/__init__.py
+-rw-r--r--  2.0 unx       67 b- defN 22-Apr-12 13:04 pytket/extensions/stim/_metadata.py
+-rw-r--r--  2.0 unx        0 b- defN 22-Apr-12 12:55 pytket/extensions/stim/py.typed
+-rw-r--r--  2.0 unx      713 b- defN 22-Apr-12 12:55 pytket/extensions/stim/backends/__init__.py
+-rw-r--r--  2.0 unx     5664 b- defN 22-Apr-12 12:55 pytket/extensions/stim/backends/stim_backend.py
+-rw-r--r--  2.0 unx     1435 b- defN 22-Apr-12 13:04 pytket_stim-0.9.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 22-Apr-12 13:04 pytket_stim-0.9.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 22-Apr-12 13:04 pytket_stim-0.9.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      781 b- defN 22-Apr-12 13:04 pytket_stim-0.9.0.dist-info/RECORD
+9 files, 9593 bytes uncompressed, 4389 bytes compressed:  54.2%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: pytket/extensions/stim/backends/__init__.py
 Comment: 
 
 Filename: pytket/extensions/stim/backends/stim_backend.py
 Comment: 
 
-Filename: pytket_stim-0.8.0.dist-info/METADATA
+Filename: pytket_stim-0.9.0.dist-info/METADATA
 Comment: 
 
-Filename: pytket_stim-0.8.0.dist-info/WHEEL
+Filename: pytket_stim-0.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: pytket_stim-0.8.0.dist-info/top_level.txt
+Filename: pytket_stim-0.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pytket_stim-0.8.0.dist-info/RECORD
+Filename: pytket_stim-0.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pytket/extensions/stim/_metadata.py

```diff
@@ -1,2 +1,2 @@
-__extension_version__ = "0.8.0"
+__extension_version__ = "0.9.0"
 __extension_name__ = "pytket-stim"
```

## Comparing `pytket_stim-0.8.0.dist-info/METADATA` & `pytket_stim-0.9.0.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytket-stim
-Version: 0.8.0
+Version: 0.9.0
 Summary: Extension for pytket, providing access to the Stim Clifford simulator
 Home-page: https://github.com/CQCL/pytket-extensions
 Author: Alec Edgington
 Author-email: alec.edgington@cambridgequantum.com
 License: Apache 2
 Platform: UNKNOWN
 Classifier: Environment :: Console
@@ -16,15 +16,15 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: pytket (~=1.0)
+Requires-Dist: pytket (~=1.1)
 Requires-Dist: stim (~=1.4)
 
 # pytket-stim
 
 [Pytket](https://cqcl.github.io/pytket) is a Python module for interfacing
 with CQC tket, a set of quantum programming tools.
```

