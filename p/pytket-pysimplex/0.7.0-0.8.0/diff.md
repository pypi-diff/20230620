# Comparing `tmp/pytket_pysimplex-0.7.0-py3-none-any.whl.zip` & `tmp/pytket_pysimplex-0.8.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 11113 bytes, number of entries: 10
--rw-r--r--  2.0 unx      842 b- defN 22-Nov-25 16:41 pytket/extensions/pysimplex/__init__.py
--rw-r--r--  2.0 unx       72 b- defN 22-Nov-25 16:42 pytket/extensions/pysimplex/_metadata.py
--rw-r--r--  2.0 unx        0 b- defN 22-Nov-25 16:41 pytket/extensions/pysimplex/py.typed
--rw-r--r--  2.0 unx      724 b- defN 22-Nov-25 16:41 pytket/extensions/pysimplex/backends/__init__.py
--rw-r--r--  2.0 unx     6225 b- defN 22-Nov-25 16:41 pytket/extensions/pysimplex/backends/simplex_backend.py
--rw-r--r--  2.0 unx    11357 b- defN 22-Nov-25 16:42 pytket_pysimplex-0.7.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     4010 b- defN 22-Nov-25 16:42 pytket_pysimplex-0.7.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Nov-25 16:42 pytket_pysimplex-0.7.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 22-Nov-25 16:42 pytket_pysimplex-0.7.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      927 b- defN 22-Nov-25 16:42 pytket_pysimplex-0.7.0.dist-info/RECORD
-10 files, 24256 bytes uncompressed, 9487 bytes compressed:  60.9%
+Zip file size: 11108 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      842 b- defN 23-Jun-20 16:56 pytket/extensions/pysimplex/__init__.py
+-rw-r--r--  2.0 unx       72 b- defN 23-Jun-20 16:56 pytket/extensions/pysimplex/_metadata.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-20 16:56 pytket/extensions/pysimplex/py.typed
+-rw-r--r--  2.0 unx      724 b- defN 23-Jun-20 16:56 pytket/extensions/pysimplex/backends/__init__.py
+-rw-r--r--  2.0 unx     6225 b- defN 23-Jun-20 16:56 pytket/extensions/pysimplex/backends/simplex_backend.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jun-20 16:56 pytket_pysimplex-0.8.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3956 b- defN 23-Jun-20 16:56 pytket_pysimplex-0.8.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-20 16:56 pytket_pysimplex-0.8.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-20 16:56 pytket_pysimplex-0.8.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      927 b- defN 23-Jun-20 16:56 pytket_pysimplex-0.8.0.dist-info/RECORD
+10 files, 24202 bytes uncompressed, 9482 bytes compressed:  60.8%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: pytket/extensions/pysimplex/backends/__init__.py
 Comment: 
 
 Filename: pytket/extensions/pysimplex/backends/simplex_backend.py
 Comment: 
 
-Filename: pytket_pysimplex-0.7.0.dist-info/LICENSE
+Filename: pytket_pysimplex-0.8.0.dist-info/LICENSE
 Comment: 
 
-Filename: pytket_pysimplex-0.7.0.dist-info/METADATA
+Filename: pytket_pysimplex-0.8.0.dist-info/METADATA
 Comment: 
 
-Filename: pytket_pysimplex-0.7.0.dist-info/WHEEL
+Filename: pytket_pysimplex-0.8.0.dist-info/WHEEL
 Comment: 
 
-Filename: pytket_pysimplex-0.7.0.dist-info/top_level.txt
+Filename: pytket_pysimplex-0.8.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pytket_pysimplex-0.7.0.dist-info/RECORD
+Filename: pytket_pysimplex-0.8.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pytket/extensions/pysimplex/__init__.py

```diff
@@ -1,8 +1,8 @@
-# Copyright 2020-2022 Cambridge Quantum Computing
+# Copyright 2020-2023 Cambridge Quantum Computing
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

## pytket/extensions/pysimplex/_metadata.py

```diff
@@ -1,2 +1,2 @@
-__extension_version__ = "0.7.0"
+__extension_version__ = "0.8.0"
 __extension_name__ = "pytket-pysimplex"
```

## pytket/extensions/pysimplex/backends/__init__.py

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2022 Cambridge Quantum Computing
+# Copyright 2019-2023 Cambridge Quantum Computing
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

## pytket/extensions/pysimplex/backends/simplex_backend.py

```diff
@@ -1,8 +1,8 @@
-# Copyright 2020-2022 Cambridge Quantum Computing
+# Copyright 2020-2023 Cambridge Quantum Computing
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

## Comparing `pytket_pysimplex-0.7.0.dist-info/LICENSE` & `pytket_pysimplex-0.8.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pytket_pysimplex-0.7.0.dist-info/METADATA` & `pytket_pysimplex-0.8.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: pytket-pysimplex
-Version: 0.7.0
+Version: 0.8.0
 Summary: Extension for pytket, providing access to the pysimplex Clifford simulator
 Author: TKET development team
 Author-email: tket-support@cambridgequantum.com
 License: Apache 2
 Project-URL: Documentation, https://cqcl.github.io/pytket-pysimplex/api/index.html
 Project-URL: Source, https://github.com/CQCL/pytket-pysimplex
 Project-URL: Tracker, https://github.com/CQCL/pytket-pysimplex/issues
 Classifier: Environment :: Console
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pytket (~=1.9)
+Requires-Dist: pytket (~=1.16)
 Requires-Dist: pysimplex (~=1.4)
 
 # Pytket Extensions
 
 This repository contains the pytket-pysimplex extension, using Quantinuum's
 [pytket](https://cqcl.github.io/tket/pytket/api/index.html) quantum SDK.
 
@@ -36,15 +35,15 @@
 with tket, a quantum computing toolkit and optimisation compiler developed by Quantinuum.
 
 `pytket-pysimplex` is an extension to `pytket` that allows `pytket` circuits to
 be simulated using pysimplex.
 
 ## Getting started
 
-`pytket-pysimplex` is available for Python 3.8, 3.9 and 3.10, on Linux, MacOS
+`pytket-pysimplex` is available for Python 3.9 and 3.10, on Linux, MacOS
 and Windows. To install, run:
 
 ```pip install pytket-pysimplex```
 
 This will install `pytket` if it isn't already installed, and add new classes
 and methods into the `pytket.extensions` namespace.
```

