# Comparing `tmp/vssource-0.9.3.tar.gz` & `tmp/vssource-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vssource-0.9.3.tar", last modified: Mon Jun  5 20:25:30 2023, max compression
+gzip compressed data, was "vssource-0.9.4.tar", last modified: Tue Jun 20 14:23:46 2023, max compression
```

## Comparing `vssource-0.9.3.tar` & `vssource-0.9.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:25:30.884524 vssource-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-05 20:25:06.000000 vssource-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-05 20:25:30.884524 vssource-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-05 20:25:06.000000 vssource-0.9.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-05 20:25:30.884524 vssource-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-05 20:25:06.000000 vssource-0.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:25:30.880524 vssource-0.9.3/vssource/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-05 20:25:06.000000 vssource-0.9.3/vssource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-05 20:25:06.000000 vssource-0.9.3/vssource/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-05 20:25:06.000000 vssource-0.9.3/vssource/dataclasses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:25:30.880524 vssource-0.9.3/vssource/formats/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-05 20:25:06.000000 vssource-0.9.3/vssource/formats/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:25:30.880524 vssource-0.9.3/vssource/formats/bd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:25:06.000000 vssource-0.9.3/vssource/formats/bd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:25:30.880524 vssource-0.9.3/vssource/formats/dvd/
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-06-05 20:25:06.000000 vssource-0.9.3/vssource/formats/dvd/IsoFile.py
--rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-06-05 20:25:06.000000 vssource-0.9.3/vssource/formats/dvd/IsoFileCore.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-05 20:25:06.000000 vssource-0.9.3/vssource/formats/dvd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:25:30.884524 vssource-0.9.3/vssource/formats/dvd/parsedvd/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-05 20:25:06.000000 vssource-0.9.3/vssource/formats/dvd/parsedvd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-06-05 20:25:06.000000 vssource-0.9.3/vssource/formats/dvd/parsedvd/sector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-06-05 20:25:06.000000 vssource-0.9.3/vssource/formats/dvd/parsedvd/vts_pgci.py
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-06-05 20:25:06.000000 vssource-0.9.3/vssource/funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:25:30.884524 vssource-0.9.3/vssource/indexers/
--rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-06-05 20:25:06.000000 vssource-0.9.3/vssource/indexers/D2VWitch.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-05 20:25:06.000000 vssource-0.9.3/vssource/indexers/DGIndex.py
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-06-05 20:25:06.000000 vssource-0.9.3/vssource/indexers/DGIndexNV.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-05 20:25:06.000000 vssource-0.9.3/vssource/indexers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9148 2023-06-05 20:25:06.000000 vssource-0.9.3/vssource/indexers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-05 20:25:06.000000 vssource-0.9.3/vssource/indexers/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:25:06.000000 vssource-0.9.3/vssource/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-05 20:25:06.000000 vssource-0.9.3/vssource/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:25:30.880524 vssource-0.9.3/vssource.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-05 20:25:30.000000 vssource-0.9.3/vssource.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-05 20:25:30.000000 vssource-0.9.3/vssource.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 20:25:30.000000 vssource-0.9.3/vssource.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-05 20:25:30.000000 vssource-0.9.3/vssource.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-05 20:25:30.000000 vssource-0.9.3/vssource.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:23:46.891149 vssource-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-20 14:23:16.000000 vssource-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-20 14:23:46.891149 vssource-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-20 14:23:16.000000 vssource-0.9.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-20 14:23:46.891149 vssource-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-20 14:23:16.000000 vssource-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:23:46.887149 vssource-0.9.4/vssource/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-20 14:23:16.000000 vssource-0.9.4/vssource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-20 14:23:16.000000 vssource-0.9.4/vssource/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-20 14:23:16.000000 vssource-0.9.4/vssource/dataclasses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:23:46.887149 vssource-0.9.4/vssource/formats/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-20 14:23:16.000000 vssource-0.9.4/vssource/formats/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:23:46.887149 vssource-0.9.4/vssource/formats/bd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:23:16.000000 vssource-0.9.4/vssource/formats/bd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:23:46.887149 vssource-0.9.4/vssource/formats/dvd/
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-06-20 14:23:16.000000 vssource-0.9.4/vssource/formats/dvd/IsoFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-06-20 14:23:16.000000 vssource-0.9.4/vssource/formats/dvd/IsoFileCore.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-20 14:23:16.000000 vssource-0.9.4/vssource/formats/dvd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:23:46.891149 vssource-0.9.4/vssource/formats/dvd/parsedvd/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-20 14:23:16.000000 vssource-0.9.4/vssource/formats/dvd/parsedvd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-06-20 14:23:16.000000 vssource-0.9.4/vssource/formats/dvd/parsedvd/sector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-06-20 14:23:16.000000 vssource-0.9.4/vssource/formats/dvd/parsedvd/vts_pgci.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-06-20 14:23:16.000000 vssource-0.9.4/vssource/funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:23:46.891149 vssource-0.9.4/vssource/indexers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-06-20 14:23:16.000000 vssource-0.9.4/vssource/indexers/D2VWitch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-20 14:23:16.000000 vssource-0.9.4/vssource/indexers/DGIndex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-06-20 14:23:16.000000 vssource-0.9.4/vssource/indexers/DGIndexNV.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-20 14:23:16.000000 vssource-0.9.4/vssource/indexers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9218 2023-06-20 14:23:16.000000 vssource-0.9.4/vssource/indexers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-20 14:23:16.000000 vssource-0.9.4/vssource/indexers/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:23:16.000000 vssource-0.9.4/vssource/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-20 14:23:16.000000 vssource-0.9.4/vssource/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:23:46.887149 vssource-0.9.4/vssource.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-20 14:23:46.000000 vssource-0.9.4/vssource.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-20 14:23:46.000000 vssource-0.9.4/vssource.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 14:23:46.000000 vssource-0.9.4/vssource.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-20 14:23:46.000000 vssource-0.9.4/vssource.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 14:23:46.000000 vssource-0.9.4/vssource.egg-info/top_level.txt
```

### Comparing `vssource-0.9.3/LICENSE` & `vssource-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vssource-0.9.3/PKG-INFO` & `vssource-0.9.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vssource
-Version: 0.9.3
+Version: 0.9.4
 Summary: Vapoursynth Wrapper for DVDs stuff
 Author: Setsugen no ao
 Author-email: setsugen@setsugen.dev
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-source
 Project-URL: Documentation, https://vssource.encode.moe/en/latest/
```

### Comparing `vssource-0.9.3/README.md` & `vssource-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `vssource-0.9.3/setup.cfg` & `vssource-0.9.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `vssource-0.9.3/setup.py` & `vssource-0.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `vssource-0.9.3/vssource/dataclasses.py` & `vssource-0.9.4/vssource/dataclasses.py`

 * *Files identical despite different names*

### Comparing `vssource-0.9.3/vssource/formats/dvd/IsoFile.py` & `vssource-0.9.4/vssource/formats/dvd/IsoFile.py`

 * *Files identical despite different names*

### Comparing `vssource-0.9.3/vssource/formats/dvd/IsoFileCore.py` & `vssource-0.9.4/vssource/formats/dvd/IsoFileCore.py`

 * *Files identical despite different names*

### Comparing `vssource-0.9.3/vssource/formats/dvd/parsedvd/sector.py` & `vssource-0.9.4/vssource/formats/dvd/parsedvd/sector.py`

 * *Files identical despite different names*

### Comparing `vssource-0.9.3/vssource/formats/dvd/parsedvd/vts_pgci.py` & `vssource-0.9.4/vssource/formats/dvd/parsedvd/vts_pgci.py`

 * *Files identical despite different names*

### Comparing `vssource-0.9.3/vssource/indexers/D2VWitch.py` & `vssource-0.9.4/vssource/indexers/D2VWitch.py`

 * *Files identical despite different names*

### Comparing `vssource-0.9.3/vssource/indexers/DGIndex.py` & `vssource-0.9.4/vssource/indexers/DGIndex.py`

 * *Files identical despite different names*

### Comparing `vssource-0.9.3/vssource/indexers/DGIndexNV.py` & `vssource-0.9.4/vssource/indexers/DGIndexNV.py`

 * *Files identical despite different names*

### Comparing `vssource-0.9.3/vssource/indexers/base.py` & `vssource-0.9.4/vssource/indexers/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import shutil
 import subprocess
 import tempfile
 from abc import ABC, abstractmethod
 from hashlib import md5
+from os import name as os_name
 from typing import Any, Callable, ClassVar, Iterable, Literal, Protocol, Sequence
 
 from vstools import (
     MISSING, ChromaLocationT, ColorRangeT, CustomRuntimeError, DataType, FieldBasedT, MatrixT, MissingT, PrimariesT,
     SPath, SPathLike, TransferT, core, initialize_clip, inject_self, to_arr, vs
 )
 
@@ -143,15 +144,15 @@
 
     @abstractmethod
     def update_video_filenames(self, index_path: SPath, filepaths: list[SPath]) -> None:
         raise NotImplementedError
 
     def _get_bin_path(self) -> SPath:
         if not (bin_path := shutil.which(str(self.bin_path))):
-            raise FileNotFoundError(f'Indexer: `{self.bin_path}` was not found!')
+            raise FileNotFoundError(f'Indexer: `{self.bin_path}` was not found{" in PATH" if os_name == "nt" else ""}!')
         return SPath(bin_path)
 
     def _run_index(self, files: list[SPath], output: SPath, cmd_args: Sequence[str]) -> None:
         output.mkdirp()
 
         proc = subprocess.Popen(
             list(map(str, self.get_cmd(files, output) + list(cmd_args) + list(self._default_args))),
```

### Comparing `vssource-0.9.3/vssource/utils.py` & `vssource-0.9.4/vssource/utils.py`

 * *Files identical despite different names*

### Comparing `vssource-0.9.3/vssource.egg-info/PKG-INFO` & `vssource-0.9.4/vssource.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vssource
-Version: 0.9.3
+Version: 0.9.4
 Summary: Vapoursynth Wrapper for DVDs stuff
 Author: Setsugen no ao
 Author-email: setsugen@setsugen.dev
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-source
 Project-URL: Documentation, https://vssource.encode.moe/en/latest/
```

### Comparing `vssource-0.9.3/vssource.egg-info/SOURCES.txt` & `vssource-0.9.4/vssource.egg-info/SOURCES.txt`

 * *Files identical despite different names*

