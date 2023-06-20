# Comparing `tmp/pytket_quantinuum-0.9.0-py3-none-any.whl.zip` & `tmp/pytket_quantinuum-0.9.0rc0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 26964 bytes, number of entries: 14
--rw-r--r--  2.0 unx      886 b- defN 22-Oct-11 15:39 pytket/extensions/quantinuum/__init__.py
--rw-r--r--  2.0 unx       73 b- defN 22-Oct-11 15:39 pytket/extensions/quantinuum/_metadata.py
--rw-r--r--  2.0 unx        0 b- defN 22-Oct-11 15:39 pytket/extensions/quantinuum/py.typed
--rw-r--r--  2.0 unx      773 b- defN 22-Oct-11 15:39 pytket/extensions/quantinuum/backends/__init__.py
--rw-r--r--  2.0 unx    21634 b- defN 22-Oct-11 15:39 pytket/extensions/quantinuum/backends/api_wrappers.py
--rw-r--r--  2.0 unx     1425 b- defN 22-Oct-11 15:39 pytket/extensions/quantinuum/backends/config.py
--rw-r--r--  2.0 unx     3474 b- defN 22-Oct-11 15:39 pytket/extensions/quantinuum/backends/credential_storage.py
--rw-r--r--  2.0 unx     2867 b- defN 22-Oct-11 15:39 pytket/extensions/quantinuum/backends/federated_login.py
--rw-r--r--  2.0 unx    32475 b- defN 22-Oct-11 15:39 pytket/extensions/quantinuum/backends/quantinuum.py
--rw-r--r--  2.0 unx    11357 b- defN 22-Oct-11 15:39 pytket_quantinuum-0.9.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     4333 b- defN 22-Oct-11 15:39 pytket_quantinuum-0.9.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Oct-11 15:39 pytket_quantinuum-0.9.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 22-Oct-11 15:39 pytket_quantinuum-0.9.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1377 b- defN 22-Oct-11 15:39 pytket_quantinuum-0.9.0.dist-info/RECORD
-14 files, 80773 bytes uncompressed, 24594 bytes compressed:  69.6%
+Zip file size: 27039 bytes, number of entries: 14
+-rw-r--r--  2.0 unx      886 b- defN 22-Oct-04 09:48 pytket/extensions/quantinuum/__init__.py
+-rw-r--r--  2.0 unx       76 b- defN 22-Oct-04 09:48 pytket/extensions/quantinuum/_metadata.py
+-rw-r--r--  2.0 unx        0 b- defN 22-Oct-04 09:48 pytket/extensions/quantinuum/py.typed
+-rw-r--r--  2.0 unx      773 b- defN 22-Oct-04 09:48 pytket/extensions/quantinuum/backends/__init__.py
+-rw-r--r--  2.0 unx    21634 b- defN 22-Oct-04 09:48 pytket/extensions/quantinuum/backends/api_wrappers.py
+-rw-r--r--  2.0 unx     1425 b- defN 22-Oct-04 09:48 pytket/extensions/quantinuum/backends/config.py
+-rw-r--r--  2.0 unx     3474 b- defN 22-Oct-04 09:48 pytket/extensions/quantinuum/backends/credential_storage.py
+-rw-r--r--  2.0 unx     2867 b- defN 22-Oct-04 09:48 pytket/extensions/quantinuum/backends/federated_login.py
+-rw-r--r--  2.0 unx    32440 b- defN 22-Oct-04 09:48 pytket/extensions/quantinuum/backends/quantinuum.py
+-rw-r--r--  2.0 unx    11357 b- defN 22-Oct-04 09:48 pytket_quantinuum-0.9.0rc0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4465 b- defN 22-Oct-04 09:48 pytket_quantinuum-0.9.0rc0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 22-Oct-04 09:48 pytket_quantinuum-0.9.0rc0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 22-Oct-04 09:48 pytket_quantinuum-0.9.0rc0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1392 b- defN 22-Oct-04 09:48 pytket_quantinuum-0.9.0rc0.dist-info/RECORD
+14 files, 80888 bytes uncompressed, 24639 bytes compressed:  69.5%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: pytket/extensions/quantinuum/backends/federated_login.py
 Comment: 
 
 Filename: pytket/extensions/quantinuum/backends/quantinuum.py
 Comment: 
 
-Filename: pytket_quantinuum-0.9.0.dist-info/LICENSE
+Filename: pytket_quantinuum-0.9.0rc0.dist-info/LICENSE
 Comment: 
 
-Filename: pytket_quantinuum-0.9.0.dist-info/METADATA
+Filename: pytket_quantinuum-0.9.0rc0.dist-info/METADATA
 Comment: 
 
-Filename: pytket_quantinuum-0.9.0.dist-info/WHEEL
+Filename: pytket_quantinuum-0.9.0rc0.dist-info/WHEEL
 Comment: 
 
-Filename: pytket_quantinuum-0.9.0.dist-info/top_level.txt
+Filename: pytket_quantinuum-0.9.0rc0.dist-info/top_level.txt
 Comment: 
 
-Filename: pytket_quantinuum-0.9.0.dist-info/RECORD
+Filename: pytket_quantinuum-0.9.0rc0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pytket/extensions/quantinuum/_metadata.py

```diff
@@ -1,2 +1,2 @@
-__extension_version__ = "0.9.0"
+__extension_version__ = "0.9.0rc0"
 __extension_name__ = "pytket-quantinuum"
```

## pytket/extensions/quantinuum/backends/quantinuum.py

```diff
@@ -365,15 +365,14 @@
             return SequencePass(
                 passlist
                 + [
                     FullPeepholeOptimise(target_2qb_gate=OpType.TK2),
                     NormaliseTK2(),
                     DecomposeTK2(**fidelities),
                     self.rebase_pass(),
-                    ZZPhaseToRz(),
                     RemoveRedundancies(),
                     squash,
                     SimplifyInitial(
                         allow_classical=False, create_all_qubits=True, xcirc=_xcirc
                     ),
                 ]
             )
```

## Comparing `pytket_quantinuum-0.9.0.dist-info/LICENSE` & `pytket_quantinuum-0.9.0rc0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pytket_quantinuum-0.9.0.dist-info/METADATA` & `pytket_quantinuum-0.9.0rc0.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytket-quantinuum
-Version: 0.9.0
+Version: 0.9.0rc0
 Summary: Extension for pytket, providing access to Quantinuum backends
 Author: TKET development team
 Author-email: tket-support@cambridgequantum.com
 License: Apache 2
 Project-URL: Documentation, https://cqcl.github.io/pytket-quantinuum/api/index.html
 Project-URL: Source, https://github.com/CQCL/pytket-quantinuum
 Project-URL: Tracker, https://github.com/CQCL/pytket-quantinuum/issues
@@ -18,26 +18,28 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pytket (~=1.7)
+Requires-Dist: pytket (~=1.6)
 Requires-Dist: requests (>=2.2)
 Requires-Dist: types-requests
 Requires-Dist: websockets (>=7.0)
 Requires-Dist: nest-asyncio (>=1.2)
 Requires-Dist: pyjwt (~=2.4)
 Requires-Dist: msal (~=1.18)
 
 # Pytket Extensions
 
 This repository contains the pytket-quantinuum extension, using Quantinuum's
 [pytket](https://cqcl.github.io/tket/pytket/api/index.html) quantum SDK.
+The other pytket extensions can be found [here](https://github.com/CQCL/pytket-extensions)
+
 
 # pytket-quantinuum
 
 [Pytket](https://cqcl.github.io/tket/pytket/api/index.html) is a python module for interfacing
 with tket, a quantum computing toolkit and optimisation compiler developed by Quantinuum.
 
 `pytket-quantinuum` is an extension to `pytket` that allows `pytket` circuits to
@@ -94,16 +96,17 @@
 complicated, but it should be sufficient to run the script `modules/mypy-check`
 (passing as a single argument the root directory of the module to test). The
 script requires `mypy` 0.800 or above.
 
 #### Linting
 
 We use [pylint](https://pypi.org/project/pylint/) on the CI to check compliance
-with a set of style requirements (listed in `.pylintrc`). You should run
-`pylint` over any changed files before submitting a PR, to catch any issues.
+with a set of style requirements (listed in `modules/.pylintrc`). You should run
+`pylint` over any changed files from the `modules` directory before submitting a
+PR, to catch any issues.
 
 ### Tests
 
 To run the tests for a module:
 
 1. `cd` into that module's `tests` directory;
 2. ensure you have installed `pytest`, `hypothesis`, and any modules listed in
```

## Comparing `pytket_quantinuum-0.9.0.dist-info/RECORD` & `pytket_quantinuum-0.9.0rc0.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 pytket/extensions/quantinuum/__init__.py,sha256=BowFQeNj96tSsIuj4NDUqHwA2PmYijYNF1Pohtii24I,886
-pytket/extensions/quantinuum/_metadata.py,sha256=VaA9c3sNzdk-zYCx0FHoJaCOJ30FvuFutIj_1fdFVzI,73
+pytket/extensions/quantinuum/_metadata.py,sha256=IuLfVdKPkdVSGZH_z-ldNiLFTzbTWrc12WtPHznww8I,76
 pytket/extensions/quantinuum/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pytket/extensions/quantinuum/backends/__init__.py,sha256=ZBvcwMVxcHVzHsCOmtLDgbklqBhMDVNpB0VXGPGtpkk,773
 pytket/extensions/quantinuum/backends/api_wrappers.py,sha256=qWR87Q8Mckw6fEm_dMgFAyhsUT72vTsqBugg0FVzVl8,21634
 pytket/extensions/quantinuum/backends/config.py,sha256=ZITTMIDtQGxM8IMC_PP1RVrRcUktZExeVD8jCbk4zTw,1425
 pytket/extensions/quantinuum/backends/credential_storage.py,sha256=tX-WsGlWTA6ZUBIGfvCzA6koTbzJdtpYNqAXmgVXxdQ,3474
 pytket/extensions/quantinuum/backends/federated_login.py,sha256=Qda8Hp_QkBQU6nBqlW1sEYBXpKJEB7CIa98TWyRLZuk,2867
-pytket/extensions/quantinuum/backends/quantinuum.py,sha256=KniY0iIukYYJTuXdJOamK3g7z8Bcm9IJ5ci3rCZwAgg,32475
-pytket_quantinuum-0.9.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-pytket_quantinuum-0.9.0.dist-info/METADATA,sha256=MucxgUafNukdWQJ8JIIRg1MRAKi-LxEPUVEcuAXmu84,4333
-pytket_quantinuum-0.9.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pytket_quantinuum-0.9.0.dist-info/top_level.txt,sha256=GsvCQQpJ7P8Vrx4ydtbjs36yufXiD59vSbbQFtFgcQ0,7
-pytket_quantinuum-0.9.0.dist-info/RECORD,,
+pytket/extensions/quantinuum/backends/quantinuum.py,sha256=rWFWWyqGfexS0HwTCV2WjS_dpP80by5gIY2g_t7KNUg,32440
+pytket_quantinuum-0.9.0rc0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+pytket_quantinuum-0.9.0rc0.dist-info/METADATA,sha256=0P5vG0I8CkXp0EiCy9SiEXAa6vQzDD_fka6S5QOSgtU,4465
+pytket_quantinuum-0.9.0rc0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+pytket_quantinuum-0.9.0rc0.dist-info/top_level.txt,sha256=GsvCQQpJ7P8Vrx4ydtbjs36yufXiD59vSbbQFtFgcQ0,7
+pytket_quantinuum-0.9.0rc0.dist-info/RECORD,,
```

