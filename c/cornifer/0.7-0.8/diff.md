# Comparing `tmp/cornifer-0.7.tar.gz` & `tmp/cornifer-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cornifer-0.7.tar", last modified: Sun May 28 18:16:47 2023, max compression
+gzip compressed data, was "cornifer-0.8.tar", last modified: Mon Jun 19 23:32:40 2023, max compression
```

## Comparing `cornifer-0.7.tar` & `cornifer-0.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        0 2023-05-28 18:16:47.085758 cornifer-0.7/
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)    35823 2021-08-18 02:15:58.000000 cornifer-0.7/LICENSE
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)      644 2023-05-28 18:16:47.082754 cornifer-0.7/PKG-INFO
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     1376 2022-07-25 17:02:05.000000 cornifer-0.7/README.md
-drwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        0 2023-05-28 18:16:46.343713 cornifer-0.7/lib/
-drwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        0 2023-05-28 18:16:46.525860 cornifer-0.7/lib/Cornifer.egg-info/
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)      644 2023-05-28 18:16:46.000000 cornifer-0.7/lib/Cornifer.egg-info/PKG-INFO
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)      878 2023-05-28 18:16:46.000000 cornifer-0.7/lib/Cornifer.egg-info/SOURCES.txt
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        1 2023-05-28 18:16:46.000000 cornifer-0.7/lib/Cornifer.egg-info/dependency_links.txt
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        1 2022-07-23 17:35:39.000000 cornifer-0.7/lib/Cornifer.egg-info/not-zip-safe
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)       35 2023-05-28 18:16:46.000000 cornifer-0.7/lib/Cornifer.egg-info/requires.txt
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        9 2023-05-28 18:16:46.000000 cornifer-0.7/lib/Cornifer.egg-info/top_level.txt
-drwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        0 2023-05-28 18:16:46.769624 cornifer-0.7/lib/cornifer/
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)      897 2022-09-20 19:30:38.000000 cornifer-0.7/lib/cornifer/__init__.py
-drwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        0 2023-05-28 18:16:46.944561 cornifer-0.7/lib/cornifer/_utilities/
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)    10208 2023-05-26 19:18:06.000000 cornifer-0.7/lib/cornifer/_utilities/__init__.py
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     5859 2023-05-25 21:14:31.000000 cornifer-0.7/lib/cornifer/_utilities/lmdb.py
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     8811 2023-05-24 18:08:21.000000 cornifer-0.7/lib/cornifer/blocks.py
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     1096 2022-08-25 21:25:33.000000 cornifer-0.7/lib/cornifer/errors.py
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)      943 2023-05-12 15:41:02.000000 cornifer-0.7/lib/cornifer/example.py
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     2407 2023-05-10 16:54:32.000000 cornifer-0.7/lib/cornifer/filemetadata.py
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)    13578 2023-05-26 14:59:06.000000 cornifer-0.7/lib/cornifer/info.py
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     1987 2023-05-10 16:57:49.000000 cornifer-0.7/lib/cornifer/regfilestructure.py
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)   128928 2023-05-28 18:02:34.000000 cornifer-0.7/lib/cornifer/registers.py
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)    12329 2023-05-24 18:24:36.000000 cornifer-0.7/lib/cornifer/regloader.py
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)      730 2023-05-28 18:09:24.000000 cornifer-0.7/lib/cornifer/version.py
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)       38 2023-05-28 18:16:47.086755 cornifer-0.7/setup.cfg
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     1897 2022-09-27 16:45:39.000000 cornifer-0.7/setup.py
-drwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        0 2023-05-28 18:16:47.054962 cornifer-0.7/tests/
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     9632 2023-05-12 15:41:02.000000 cornifer-0.7/tests/test_blocks.py
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)    11191 2023-05-12 15:41:02.000000 cornifer-0.7/tests/test_info.py
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     2216 2023-05-26 15:26:43.000000 cornifer-0.7/tests/test_register_file_structure.py
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)   134663 2023-05-28 15:19:05.000000 cornifer-0.7/tests/test_registers.py
+drwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        0 2023-06-19 23:32:40.645084 cornifer-0.8/
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)    35823 2021-08-18 02:15:58.000000 cornifer-0.8/LICENSE
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)      644 2023-06-19 23:32:40.643083 cornifer-0.8/PKG-INFO
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     1376 2022-07-25 17:02:05.000000 cornifer-0.8/README.md
+drwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        0 2023-06-19 23:32:40.183039 cornifer-0.8/lib/
+drwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        0 2023-06-19 23:32:40.317010 cornifer-0.8/lib/Cornifer.egg-info/
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)      644 2023-06-19 23:32:40.000000 cornifer-0.8/lib/Cornifer.egg-info/PKG-INFO
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)      878 2023-06-19 23:32:40.000000 cornifer-0.8/lib/Cornifer.egg-info/SOURCES.txt
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        1 2023-06-19 23:32:40.000000 cornifer-0.8/lib/Cornifer.egg-info/dependency_links.txt
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        1 2022-07-23 17:35:39.000000 cornifer-0.8/lib/Cornifer.egg-info/not-zip-safe
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)       35 2023-06-19 23:32:40.000000 cornifer-0.8/lib/Cornifer.egg-info/requires.txt
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        9 2023-06-19 23:32:40.000000 cornifer-0.8/lib/Cornifer.egg-info/top_level.txt
+drwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        0 2023-06-19 23:32:40.483511 cornifer-0.8/lib/cornifer/
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     4046 2023-06-16 20:01:49.000000 cornifer-0.8/lib/cornifer/__init__.py
+drwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        0 2023-06-19 23:32:40.571175 cornifer-0.8/lib/cornifer/_utilities/
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)    10788 2023-06-16 20:18:33.000000 cornifer-0.8/lib/cornifer/_utilities/__init__.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     5859 2023-05-25 21:14:31.000000 cornifer-0.8/lib/cornifer/_utilities/lmdb.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)    10402 2023-06-19 23:03:27.000000 cornifer-0.8/lib/cornifer/blocks.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     1142 2023-06-14 14:03:06.000000 cornifer-0.8/lib/cornifer/errors.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)      943 2023-05-12 15:41:02.000000 cornifer-0.8/lib/cornifer/example.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     2407 2023-05-10 16:54:32.000000 cornifer-0.8/lib/cornifer/filemetadata.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)    13576 2023-05-30 15:35:39.000000 cornifer-0.8/lib/cornifer/info.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     2045 2023-06-01 18:58:48.000000 cornifer-0.8/lib/cornifer/regfilestructure.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)   131916 2023-06-19 23:13:06.000000 cornifer-0.8/lib/cornifer/registers.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)    12329 2023-05-24 18:24:36.000000 cornifer-0.8/lib/cornifer/regloader.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)      730 2023-06-19 23:15:02.000000 cornifer-0.8/lib/cornifer/version.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)       38 2023-06-19 23:32:40.645084 cornifer-0.8/setup.cfg
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     1897 2022-09-27 16:45:39.000000 cornifer-0.8/setup.py
+drwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        0 2023-06-19 23:32:40.624397 cornifer-0.8/tests/
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     8824 2023-06-19 23:03:26.000000 cornifer-0.8/tests/test_blocks.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)    11191 2023-05-12 15:41:02.000000 cornifer-0.8/tests/test_info.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     2216 2023-05-26 15:26:43.000000 cornifer-0.8/tests/test_register_file_structure.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)   146085 2023-06-19 22:47:41.000000 cornifer-0.8/tests/test_registers.py
```

### Comparing `cornifer-0.7/LICENSE` & `cornifer-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cornifer-0.7/PKG-INFO` & `cornifer-0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cornifer
-Version: 0.7
+Version: 0.8
 Summary: An easy-to-use data manager for experimental mathematics.
 Home-page: https://github.com/automorphis/cornifer
 Author: Michael P. Lane
 Author-email: mlanetheta@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `cornifer-0.7/README.md` & `cornifer-0.8/README.md`

 * *Files identical despite different names*

### Comparing `cornifer-0.7/lib/Cornifer.egg-info/PKG-INFO` & `cornifer-0.8/lib/Cornifer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cornifer
-Version: 0.7
+Version: 0.8
 Summary: An easy-to-use data manager for experimental mathematics.
 Home-page: https://github.com/automorphis/cornifer
 Author: Michael P. Lane
 Author-email: mlanetheta@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `cornifer-0.7/lib/Cornifer.egg-info/SOURCES.txt` & `cornifer-0.8/lib/Cornifer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cornifer-0.7/lib/cornifer/__init__.py` & `cornifer-0.8/lib/cornifer/version.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,12 +9,11 @@
 
     This program is distributed in the hope that it will be useful,
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 """
 
-from .info import ApriInfo, AposInfo
-from .blocks import Block
-from .registers import Register, PickleRegister, NumpyRegister
-from .regloader import search, load
-from .errors import DataNotFoundError, CompressionError, DecompressionError
+CURRENT_VERSION          = "0.8"
+COMPATIBLE_VERSIONS      = ["0.8"]
+
+
```

### Comparing `cornifer-0.7/lib/cornifer/_utilities/__init__.py` & `cornifer-0.8/lib/cornifer/_utilities/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,15 +26,16 @@
 BYTES_PER_KB = 1024
 BYTES_PER_MB = 1024**2
 BYTES_PER_GB = 1024**3
 BYTES_PER_CHAR = 1
 # BASE52 are distinguishable ascii characters (e.g. 1, l are easily confused in some typefaces)
 BASE52 = "2346789abcdefghijmnpqrstuvwxyzABCDEFGHJLMNPQRTUVWXYZ"
 BASE94 = string.ascii_letters + string.digits + string.punctuation
-
+_TXT_FILE_WARNING_MESSAGE = "DO NOT EDIT THIS FILE.\n"
+_TXT_FILE_WARNING_MESSAGE_LEN = len(_TXT_FILE_WARNING_MESSAGE)
 NAME_REGEX = re.compile("[_a-zA-Z]\w*")
 
 try:
     LOCAL_TIMEZONE = datetime.now(timezone(timedelta(0))).astimezone().tzinfo
 
 except RuntimeError:
     LOCAL_TIMEZONE = timezone.utc
@@ -48,14 +49,17 @@
     if int1[1] < 0 or int2[1] < 0:
         raise ValueError
 
     a1,l1 = int1
     a2,l2 = int2
     return a1 <= a2 < a1 + l1 or a1 < a2 + l2 <= a1 + l1 or a2 <= a1 < a2 + l2 or a2 < a1 + l1 <= a2 + l2
 
+def intervals_subset(int1, int2):
+    return int2[0] <= int1[0] and int1[0] + int1[1] <= int2[0] + int2[1]
+
 def random_unique_filename(directory, suffix ="", length = 6, alphabet = BASE52, num_attempts = 10):
 
     directory = Path(directory)
 
     for n in range(num_attempts):
 
         filename =  directory / "".join(random.choices(alphabet, k=length + n))
@@ -67,14 +71,24 @@
             return filename
 
     raise RuntimeError("buy a lottery ticket fr")
 
 def check_has_method(instance, method_name):
     return hasattr(instance.__class__, method_name) and callable(getattr(instance.__class__, method_name))
 
+def write_txt_file(txt, file, overwrite = False):
+
+    with file.open("w" if overwrite else "x") as fh:
+        fh.write(_TXT_FILE_WARNING_MESSAGE + txt)
+
+def read_txt_file(file):
+
+    with file.open("r") as fh:
+        return fh.read()[_TXT_FILE_WARNING_MESSAGE_LEN : ]
+
 # def safe_overwrite_file(filename, new_content):
 #     tempfile = random_unique_filename(filename.parent)
 #     try:
 #         with tempfile.open("w") as fh:
 #             fh.write(new_content)
 #         Path.unlink(filename)
 #         Path.rename(tempfile, filename)
@@ -166,15 +180,15 @@
 
 def is_signed_int(num):
     return isinstance(num, (int, np.int8, np.int16, np.int32, np.int64))
 
 def is_int(num):
     return isinstance(num, (int, np.int8, np.int16, np.int32, np.int64, np.uint8, np.uint16, np.uint32, np.uint64))
 
-def bytify_num(num, num_zeros = None):
+def bytify_int(num, num_zeros = None):
 
     if num_zeros is None:
         return str(num).encode("ASCII")
 
     else:
         return f"{num:0{num_zeros}d}".encode("ASCII")
 
@@ -225,25 +239,25 @@
     """
     :param path: (type `pathlib.Path`)
     :raise FileNotFoundError: If the path could not be resolved.
     :return: (type `pathlib.Path`) Resolved.
     """
 
     try:
-        resolved = path.resolve(True)
+        resolved = path.resolve(True) # True raises FileNotFoundError
 
     except FileNotFoundError:
         raise_error = True
 
     else:
         return resolved
 
     if raise_error:
 
-        resolved = path.resolve(False)
+        resolved = path.resolve(False) # False suppressed FileNotFoundError
 
         for parent in reversed(resolved.parents):
 
             if not parent.exists():
                 raise FileNotFoundError(
                     f"Resolved path : `{resolved}`\n" +
                     f"The file or directory `{str(parent)}` could not be found."
```

### Comparing `cornifer-0.7/lib/cornifer/_utilities/lmdb.py` & `cornifer-0.8/lib/cornifer/_utilities/lmdb.py`

 * *Files identical despite different names*

### Comparing `cornifer-0.7/lib/cornifer/errors.py` & `cornifer-0.8/lib/cornifer/errors.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,14 +13,16 @@
     GNU General Public License for more details.
 """
 
 NOT_ABSOLUTE_ERROR_MESSAGE = (
     "The path `{0}` is not absolute."
 )
 
+class BlockNotOpenError(RuntimeError):pass
+
 class RegisterError(RuntimeError):pass
 
 class RegisterRecoveryError(RegisterError):pass
 
 class RegisterAlreadyOpenError(RegisterError):
     def __init__(self):
         super().__init__("This register is already opened.")
```

### Comparing `cornifer-0.7/lib/cornifer/example.py` & `cornifer-0.8/lib/cornifer/example.py`

 * *Files identical despite different names*

### Comparing `cornifer-0.7/lib/cornifer/filemetadata.py` & `cornifer-0.8/lib/cornifer/filemetadata.py`

 * *Files identical despite different names*

### Comparing `cornifer-0.7/lib/cornifer/info.py` & `cornifer-0.8/lib/cornifer/info.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,15 +161,14 @@
         self._memoize_json = False
         self._encoder = _Info._default_encoder
 
     @classmethod
     def _check_reserved_kws(cls, kwargs):
 
         if any(kw in kwargs for kw in cls._reserved_kws):
-
             raise ValueError(
                 "The following keyword-argument keys are reserved. Choose a different key.\n" +
                 f"{', '.join(cls._reserved_kws)}"
             )
 
     @classmethod
     def from_json(cls, json_str, decoder = None):
```

### Comparing `cornifer-0.7/lib/cornifer/regfilestructure.py` & `cornifer-0.8/lib/cornifer/regfilestructure.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 """
 
 from cornifer.errors import NOT_ABSOLUTE_ERROR_MESSAGE
 from cornifer._utilities import BASE52
 
 REG_FILENAME           = "register"
 VERSION_FILEPATH       = f"{REG_FILENAME}/version.txt"
+SHORTHAND_FILEPATH     = f"{REG_FILENAME}/shorthand.txt"
 MSG_FILEPATH           = f"{REG_FILENAME}/message.txt"
 CLS_FILEPATH           = f"{REG_FILENAME}/class.txt"
 DATABASE_FILEPATH      = f"{REG_FILENAME}/database"
 MAP_SIZE_FILEPATH      = f"{REG_FILENAME}/mapsize.txt"
 
 LOCAL_DIR_CHARS        = BASE52
 COMPRESSED_FILE_SUFFIX = ".zip"
```

### Comparing `cornifer-0.7/lib/cornifer/registers.py` & `cornifer-0.8/lib/cornifer/registers.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,40 +9,38 @@
 
     This program is distributed in the hope that it will be useful,
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 """
 
-import inspect
-import math
 import pickle
 import shutil
 import warnings
 import zipfile
 from contextlib import contextmanager, ExitStack
-from itertools import count
 from pathlib import Path
 from abc import ABC, abstractmethod
 
 import lmdb
 import numpy as np
 
 from .errors import DataNotFoundError, RegisterAlreadyOpenError, RegisterError, CompressionError, \
-    DecompressionError, NOT_ABSOLUTE_ERROR_MESSAGE, RegisterRecoveryError
+    DecompressionError, NOT_ABSOLUTE_ERROR_MESSAGE, RegisterRecoveryError, BlockNotOpenError
 from .info import ApriInfo, AposInfo, _InfoJsonEncoder, _InfoJsonDecoder, _Info
-from .blocks import Block, MemmapBlock, ReleaseBlock
+from .blocks import Block, MemmapBlock
 from .filemetadata import FileMetadata
 from ._utilities import random_unique_filename, is_int, resolve_path, BYTES_PER_MB, is_deletable, check_type, \
-    check_return_int_None_default, check_Path, check_return_int, bytify_num, intify_bytes
+    check_return_int_None_default, check_Path, check_return_int, bytify_int, intify_bytes, intervals_overlap, \
+    write_txt_file, read_txt_file, intervals_subset
 from ._utilities.lmdb import lmdb_has_key, lmdb_prefix_iter, open_lmdb, lmdb_count_keys, \
-    ReversibleTransaction, is_transaction, lmdb_prefix_list
+    ReversibleTransaction, is_transaction
 from .regfilestructure import VERSION_FILEPATH, LOCAL_DIR_CHARS, \
     COMPRESSED_FILE_SUFFIX, MSG_FILEPATH, CLS_FILEPATH, check_reg_structure, DATABASE_FILEPATH, \
-    REG_FILENAME, MAP_SIZE_FILEPATH
+    REG_FILENAME, MAP_SIZE_FILEPATH, SHORTHAND_FILEPATH
 from .version import CURRENT_VERSION, COMPATIBLE_VERSIONS
 
 _NO_DEBUG = 0
 _debug = _NO_DEBUG
 
 #################################
 #            LMDB KEYS          #
@@ -102,23 +100,23 @@
     else:
         return f"No {type_} `Block` found with the following data: {str(apri)}."
 
 _NOT_CREATED_ERROR_MESSAGE = (
     "The `Register` database has not been created. You must do `with reg.open() as reg:` at least once before " +
     "calling the method `{0}`."
 )
-
 _MEMORY_FULL_ERROR_MESSAGE = (
     "Exceeded max `Register` size of {0} Bytes. Please increase the max size using the method `increase_reg_size`."
 )
-
 _REG_ALREADY_ADDED_ERROR_MESSAGE = "Already added as subregister."
-
 _NO_APRI_ERROR_MESSAGE = "The following `ApriInfo` is not known to this `Register` : {0}"
-
+_RAM_BLOCK_NOT_OPEN_ERROR_MESSAGE = (
+    "Closed RAM `Block` with the following data (it is good practice to always keep all RAM `Block`s open) : {0}, "
+    "startn = {1}."
+)
 
 #################################
 #           CONSTANTS           #
 
 _START_N_TAIL_LENGTH_DEFAULT   = 12
 _LENGTH_LENGTH_DEFAULT         = 7
 _MAX_LENGTH_DEFAULT            = 10 ** _LENGTH_LENGTH_DEFAULT - 1
@@ -128,42 +126,43 @@
 _MAX_NUM_APRI                  = 10**_MAX_NUM_APRI_LENGTH
 
 class Register(ABC):
 
     #################################
     #     PUBLIC INITIALIZATION     #
 
-    def __init__(self, saves_dir, msg, initial_reg_size = None):
+    def __init__(self, saves_dir, shorthand, msg, initial_reg_size = None):
         """
-        :param saves_dir: (type `str`)
-        :param msg: (type `str`) A brief message describing this `Register`.
+        :param saves_dir: (type `str`) Directory where this `Register` is saved.
+        :param shorthand: (type `str`) A word or short phrase describing this `Register`.
+        :param msg: (type `str`) A more detailed message describing this `Register`.
         :param initial_reg_size: (type `int`, default 5) Size in bytes. You may wish to set this lower
         than 5 MB if you do not expect to add many disk `Block`s to your register and you are concerned about disk
         memory. If your `Register` exceeds `initial_register_size`, then you can adjust the database size later via the
         method `increase_reg_size`. If you are on a non-Windows system, there is no harm in setting this value
         to be very large (e.g. 1 TB).
         """
 
         check_Path(saves_dir, "saves_dir")
+        check_type(shorthand, "shorthand", str)
         check_type(msg, "msg", str)
         initial_reg_size = check_return_int_None_default(
             initial_reg_size, "initial_reg_size", _INITIAL_REGISTER_SIZE_DEFAULT
         )
 
         if initial_reg_size <= 0:
             raise ValueError("`initial_reg_size` must be positive.")
 
         self.saves_dir = resolve_path(Path(saves_dir))
 
         if not self.saves_dir.is_dir():
-            raise FileNotFoundError(
-                f"You must create the file `{str(self.saves_dir)}` before calling " +
-                f"`{self.__class__.__name__}(\"{str(self.saves_dir)}\", \"{msg}\")`."
-            )
+            raise NotADirectoryError(f"The path `{str(self.saves_dir)}` exists but is not a directory.")
 
+        self._shorthand = shorthand
+        self._shorthand_filepath = None
         self._msg = msg
         self._msg_filepath = None
 
         self._local_dir = None
         self._local_dir_bytes = None
         self._subreg_bytes = None
 
@@ -187,15 +186,15 @@
 
         self._ram_blks = {}
 
         self._created = False
 
     def __init_subclass__(cls, **kwargs):
 
-        super().__init_subclass__()
+        super().__init_subclass__(**kwargs)
         Register._constructors[cls.__name__] = cls
 
     #################################
     #     PROTEC INITIALIZATION     #
 
     _constructors = {}
 
@@ -221,16 +220,15 @@
 
         if Register._instance_exists(local_dir):
             # return the `Register` that has already been opened
             return Register._get_instance(local_dir)
 
         else:
 
-            with (local_dir / CLS_FILEPATH).open("r") as fh:
-                cls_name = fh.readline().strip()
+            cls_name = read_txt_file(local_dir / CLS_FILEPATH)
 
             if cls_name == "Register":
                 raise TypeError(
                     "`Register` is an abstract class, meaning that `Register` itself cannot be instantiated, " +
                     "only its concrete subclasses."
                 )
 
@@ -238,26 +236,20 @@
 
             if con is None:
                 raise TypeError(
                     f"`Register` is not aware of a subclass called `{cls_name}`. Please be sure that `{cls_name}` "
                     f"properly subclasses `Register` and that `{cls_name}` is in the namespace by importing it."
                 )
 
-            with (local_dir / MSG_FILEPATH).open("r") as fh:
-                msg = fh.read()
-
-            with (local_dir / MAP_SIZE_FILEPATH).open("r") as fh:
-                map_size = int(fh.readline().strip())
-
-            reg = con(local_dir.parent, msg, map_size)
+            shorthand = read_txt_file(local_dir / SHORTHAND_FILEPATH)
+            msg = read_txt_file(local_dir / MSG_FILEPATH)
+            map_size = int(read_txt_file(local_dir / MAP_SIZE_FILEPATH))
+            reg = con(local_dir.parent, shorthand, msg, map_size)
             reg._set_local_dir(local_dir)
-
-            with (local_dir / VERSION_FILEPATH).open("r") as fh:
-                reg._version = fh.readline().strip()
-
+            reg._version = read_txt_file(local_dir / VERSION_FILEPATH)
             return reg
 
     @staticmethod
     def _add_instance(local_dir, reg):
         """
         :param local_dir: (type `pathlib.Path`) Absolute.
         :param reg: (type `Register`)
@@ -311,61 +303,56 @@
         if not self._created:
             raise RegisterError(_NOT_CREATED_ERROR_MESSAGE.format("__hash__"))
 
         else:
             return hash(str(self._local_dir)) + hash(type(self))
 
     def __str__(self):
-        return self._msg
-
-    def __repr__(self):
-        return f"{self.__class__.__name__}(\"{str(self.saves_dir)}\", \"{self._msg}\")"
-
-    def __contains__(self, apri):
-
-        self._check_open_raise("__contains__")
 
-        if any(blk.apri() == apri for blk in self._ram_blks):
-            return True
+        if self._created:
+            return f'{self._shorthand} ({self._local_dir}): "{self._msg}"'
 
         else:
+            return f'{self._shorthand}: "{self._msg}"'
 
-            with self._db.begin() as txn:
-
-                try:
-                    apri_json = relational_encode_info(self, apri, txn)
+    def __repr__(self):
+        return f'{self.__class__.__name__}("{str(self.saves_dir)}", "{self._shorthand}", "{self._msg}", {self._db_map_size})'
 
-                except DataNotFoundError:
-                    return False
+    def set_shorthand(self, shorthand):
 
-                key = _APRI_ID_KEY_PREFIX + apri_json
-                return lmdb_has_key(txn, key)
+        check_type(shorthand, "shorthand", str)
 
-    def __iter__(self):
-        return iter(self.apris())
+        if self._created:
 
-    def set_msg(self, message):
-        """Give this `Register` a brief description.
+            self._check_readwrite_raise("set_shorthand")
+            write_txt_file(shorthand, self._shorthand_filepath, True)
 
-        WARNING: This method OVERWRITES the current msg. In order to append a new msg to the current one, do
-        something like the following:
+        self._shorthand = shorthand
 
-            old_message = str(reg)
-            new_message = old_message + " Hello!"
-            reg.set_msg(new_message)
+    def set_msg(self, message, append = False):
+        """Give this `Register` a detailed description.
 
         :param message: (type `str`)
+        :param append: (type `bool`, default `False`) Set to `True` to append the new message to the old one.
         """
 
         check_type(message, "message", str)
-        self._msg = message
+
+        if append:
+            new_msg = self._msg + message
+
+        else:
+            new_msg = message
 
         if self._created:
-            with self._msg_filepath.open("w") as fh:
-                fh.write(message)
+
+            self._check_readwrite_raise("set_msg")
+            write_txt_file(new_msg, self._msg_filepath, True)
+
+        self._msg = new_msg
 
     def set_startn_info(self, head = None, tail_len = None):
         """Set the range of the `startn` parameters of disk `Block`s belonging to this `Register`.
 
         Reset to default `head` and `tail_len` by omitting the parameters.
 
         If the `startn` parameter is very large (of order more than trillions), then the `Register` database can
@@ -383,15 +370,14 @@
         :param head: (type `int`, optional) Non-negative. If omitted, resets this `Register` to the default `head`.
         :param tail_len: (type `int`) Positive. If omitted, resets this `Register` to the default `tail_len`.
         """
 
         # DEBUG : 1, 2
 
         self._check_open_raise("set_startn_info")
-
         self._check_readwrite_raise("set_startn_info")
 
         if head is not None and not is_int(head):
             raise TypeError("`head` must be of type `int`.")
 
         elif head is not None:
             head = int(head)
@@ -443,22 +429,22 @@
 
             with self._db.begin(write = True) as rw_txn:
 
                 with self._db.begin() as ro_txn:
 
                     with lmdb_prefix_iter(ro_txn, _BLK_KEY_PREFIX) as it:
 
-                        rw_txn.put(_START_N_HEAD_KEY, bytify_num(head))
-                        rw_txn.put(_START_N_TAIL_LENGTH_KEY, bytify_num(tail_len))
+                        rw_txn.put(_START_N_HEAD_KEY, bytify_int(head))
+                        rw_txn.put(_START_N_TAIL_LENGTH_KEY, bytify_int(tail_len))
 
                         for key, val in it:
 
                             _, startn, _ = self._convert_disk_block_key(_BLK_KEY_PREFIX_LEN, key)
                             apri_id, _, length_bytes = self._split_disk_block_key(_BLK_KEY_PREFIX_LEN, key)
-                            new_startn_bytes = bytify_num(startn % new_mod, tail_len)
+                            new_startn_bytes = bytify_int(startn % new_mod, tail_len)
                             new_key = Register._join_disk_block_data(
                                 _BLK_KEY_PREFIX, apri_id, new_startn_bytes, length_bytes
                             )
 
                             if key != new_key:
 
                                 rw_txn.put(new_key, val)
@@ -482,27 +468,19 @@
             # set local directory info and create levelDB database
             local_dir = random_unique_filename(self.saves_dir, length = 4, alphabet = LOCAL_DIR_CHARS)
 
             try:
 
                 local_dir.mkdir()
                 (local_dir / REG_FILENAME).mkdir()
-
-                with (local_dir / MSG_FILEPATH).open("x") as fh:
-                    fh.write(self._msg)
-
-                with (local_dir / VERSION_FILEPATH).open("x") as fh:
-                    fh.write(self._version + "\nDO NOT EDIT THIS FILE. CALL THE FUNCTION `updateRegVersion` INSTEAD.")
-
-                with (local_dir / CLS_FILEPATH).open("x") as fh:
-                    fh.write(str(type(self).__name__) + "\nDO NOT EDIT THIS FILE.")
-
-                with (local_dir / MAP_SIZE_FILEPATH).open("x") as fh:
-                    fh.write(str(self._db_map_size) + "\nDO NOT EDIT THIS FILE. CALL THE FUNCTION `increase_reg_size` INSTEAD.")
-
+                write_txt_file(self._shorthand, local_dir / SHORTHAND_FILEPATH)
+                write_txt_file(self._msg, local_dir / MSG_FILEPATH)
+                write_txt_file(self._version, local_dir / VERSION_FILEPATH)
+                write_txt_file(str(type(self).__name__), local_dir / CLS_FILEPATH)
+                write_txt_file(str(self._db_map_size), local_dir / MAP_SIZE_FILEPATH)
                 (local_dir / DATABASE_FILEPATH).mkdir()
                 self._set_local_dir(local_dir)
                 self._db = open_lmdb(self._db_filepath, self._db_map_size, False)
 
                 try:
 
                     with self._db.begin(write = True) as txn:
@@ -514,14 +492,15 @@
 
                 except lmdb.MapFullError as e:
                     raise RegisterError(_MEMORY_FULL_ERROR_MESSAGE.format(self._db_map_size)) from e
 
                 Register._add_instance(local_dir, self)
                 yiel = self
                 yiel._opened = True
+                yiel._readonly = readonly
 
             except BaseException as e:
 
                 if local_dir.is_dir():
                     shutil.rmtree(local_dir)
 
                 raise e
@@ -537,94 +516,52 @@
 
         try:
             yield yiel
 
         finally:
             yiel._close_created()
 
-    @staticmethod
-    @contextmanager
-    def opens(*regs, **kwargs):
-
-        if (len(kwargs) == 1 and 'readonlys' not in kwargs) or len(kwargs) > 1:
-            raise KeyError("`opens` only takes one keyword-argument, `readonlys`.")
-
-        if len(kwargs) == 1:
-            readonlys = kwargs['readonlys']
-
-        else:
-            readonlys = None
-
-        if readonlys is not None and not isinstance(readonlys, (list, tuple)):
-            raise TypeError("`readonlys` must be of type `list` or `tuple`.")
-
-        for reg in regs:
-
-            if not isinstance(reg, Register):
-                raise TypeError("Each element of `regs` must be of type `Register`.")
-
-        if readonlys is not None:
-
-            for readonly in readonlys:
-
-                if not isinstance(readonly, bool):
-                    raise TypeError("Each element of `readonlys` must be of type `bool`.")
-
-        if readonlys is not None and len(regs) != len(readonlys):
-            raise ValueError("`regs` and `readonlys` must have the same length.")
-
-        if readonlys is None:
-            readonlys = (False,) * len(regs)
-
-        stack = ExitStack()
-        yld = []
-
-        with stack:
-
-            for reg, readonly in zip(regs, readonlys):
-                yld.append(stack.enter_context(reg.open(readonly = readonly)))
-
-            yield tuple(yld)
-
     def increase_reg_size(self, num_bytes):
         """WARNING: DO NOT CALL THIS METHOD FROM MORE THAN ONE PYTHON PROCESS AT A TIME. You are safe if you call it
         from only one Python process. You are safe if you have multiple Python processes running and call it from only
         ONE of them. But do NOT call it from multiple processes at once. Doing so may result in catastrophic loss of
         data.
 
         :param num_bytes: (type `int`) Positive.
         """
 
         self._check_open_raise("increase_reg_size")
+        self._check_readwrite_raise("increase_reg_size")
 
         if not is_int(num_bytes):
             raise TypeError("`num_bytes` must be of type `int`.")
 
         if num_bytes <= 0:
             raise ValueError("`num_bytes` must be positive.")
 
         if num_bytes <= self._db_map_size:
             raise ValueError("`num_bytes` must be larger than the current `Register` size.")
 
         self._db.set_mapsize(num_bytes)
         self._db_map_size = num_bytes
-
-        with self._db_map_size_filepath.open("w") as fh:
-            fh.write(str(self._db_map_size))
+        write_txt_file(str(self._db_map_size), self._db_map_size_filepath, True)
 
     def reg_size(self):
         return self._db_map_size
 
     def ident(self):
 
         if not self._created:
             raise RegisterError(_NOT_CREATED_ERROR_MESSAGE.format("ident"))
 
         return str(self._local_dir)
 
+    def shorthand(self):
+        return self._shorthand
+
     #################################
     #    PROTEC REGISTER METHODS    #
 
     def _open_created(self, readonly):
 
         if Register._instance_exists(self._local_dir):
             ret = Register._get_instance(self._local_dir)
@@ -635,15 +572,14 @@
         if not ret._created:
             raise RegisterError(_NOT_CREATED_ERROR_MESSAGE.format("_open_created"))
 
         if ret._db is not None and ret._opened:
             raise RegisterAlreadyOpenError()
 
         ret._readonly = readonly
-
         ret._db = open_lmdb(ret._db_filepath, ret._db_map_size, readonly)
 
         with ret._db.begin() as txn:
             ret._length_length = int(txn.get(_LENGTH_LENGTH_KEY))
 
         ret._max_length = 10 ** ret._length_length - 1
         ret._opened = True
@@ -730,29 +666,23 @@
             raise ValueError(
                 "The `local_dir` argument must be a sub-directory of `reg.savesDir`.\n" +
                 f"`local_dir.parent`    : {str(local_dir.parent)}\n"
                 f"`reg.savesDir` : {str(self.saves_dir)}"
             )
 
         check_reg_structure(local_dir)
-
         self._created = True
-
         self._local_dir = local_dir
         self._local_dir_bytes = str(self._local_dir).encode("ASCII")
-
         self._db_filepath = self._local_dir / DATABASE_FILEPATH
-
-        self._subreg_bytes = (
-            _SUB_KEY_PREFIX + self._local_dir_bytes
-        )
-
+        self._subreg_bytes = _SUB_KEY_PREFIX + self._local_dir_bytes
         self._version_filepath = local_dir / VERSION_FILEPATH
         self._msg_filepath = local_dir / MSG_FILEPATH
         self._cls_filepath = local_dir / CLS_FILEPATH
+        self._shorthand_filepath = local_dir / SHORTHAND_FILEPATH
         self._db_map_size_filepath = local_dir / MAP_SIZE_FILEPATH
 
     def _has_compatible_version(self):
         return self._version in COMPATIBLE_VERSIONS
     #
     # def _db_is_closed(self):
     #
@@ -927,14 +857,37 @@
 
             if isinstance(e, lmdb.MapFullError):
                 raise RegisterError(_MEMORY_FULL_ERROR_MESSAGE.format(self._db_map_size)) from e
 
             else:
                 raise e
 
+    def __contains__(self, apri):
+
+        self._check_open_raise("__contains__")
+
+        if any(blk.apri() == apri for blk in self._ram_blks):
+            return True
+
+        else:
+
+            with self._db.begin() as txn:
+
+                try:
+                    apri_json = relational_encode_info(self, apri, txn)
+
+                except DataNotFoundError:
+                    return False
+
+                key = _APRI_ID_KEY_PREFIX + apri_json
+                return lmdb_has_key(txn, key)
+
+    def __iter__(self):
+        return iter(self.apris())
+
     #################################
     #      PROTEC APRI METHODS      #
 
     def _apris_helper(self, diskonly, recursively, root_call):
 
         ret = []
 
@@ -1085,23 +1038,23 @@
             warnings.warn(f"Long `ApriInfo` result in disk memory inefficiency. Long `ApriInfo`: {str(apri)}.")
 
     @staticmethod
     def _get_new_apri_id(txn, reserved):
 
         for next_id_num in range(int(txn.get(_CURR_ID_KEY)), _MAX_NUM_APRI):
 
-            next_id = bytify_num(next_id_num, _MAX_NUM_APRI_LENGTH)
+            next_id = bytify_int(next_id_num, _MAX_NUM_APRI_LENGTH)
 
             if next_id not in reserved:
                 break
 
         else:
             raise RegisterError(f"Too many apris added to this `Register`, the limit is {_MAX_NUM_APRI}.")
 
-        txn.put(_CURR_ID_KEY, bytify_num(next_id_num + 1, _MAX_NUM_APRI_LENGTH))
+        txn.put(_CURR_ID_KEY, bytify_int(next_id_num + 1, _MAX_NUM_APRI_LENGTH))
         return next_id
 
     def _rmv_apri_txn(self, apri, force, txn):
 
         apris = []
         aposs = []
         blk_datas = []
@@ -1552,63 +1505,80 @@
         :param filename: (type `pathlib.Path`) Where to remove the raw data.
         :raises DataNotFoundError: If the data could not be cleaned because it doesn't exist.
         """
 
         if not filename.is_absolute():
             raise ValueError(NOT_ABSOLUTE_ERROR_MESSAGE.format(filename))
 
-        filename.unlink()
+        try:
+            filename.unlink()
+
+        except FileNotFoundError as e:
+            raise DataNotFoundError from e
 
     @classmethod
     @abstractmethod
     def with_suffix(cls, filename):
         """Adds a suffix to a filename and returns it.
 
         :param filename: (type `pathlib.Path`)
         :return: (type `pathlib.Path`)
         """
 
-    def add_disk_blk(self, blk, exists_ok = False, ret_metadata = False, **kwargs):
+    def add_disk_blk(self, blk, exists_ok = False, dups_ok = True, ret_metadata = False, **kwargs):
         """Save a `Block` to disk and link it with this `Register`.
 
         :param blk: (type `Block`)
         :param ret_metadata: (type `bool`, default `False`) Whether to return a `File_Metadata` object, which
         contains file creation date/time and size of dumped data to the disk.
         :raises RegisterError: If a duplicate `Block` already exists in this `Register`.
         """
 
         #DEBUG : 1, 2, 3, 4, 5
 
         self._check_open_raise("add_disk_blk")
         self._check_readwrite_raise("add_disk_blk")
+        Register._check_blk_open_raise(blk, "add_disk_blk")
         check_type(blk, "blk", Block)
         check_type(exists_ok, "exists_ok", bool)
+        check_type(dups_ok, "dups_ok", bool)
         check_type(ret_metadata, "ret_metadata", bool)
         startn_head = blk.startn() // self._startn_tail_mod
 
         if startn_head != self._startn_head :
 
             raise IndexError(
                 "The `startn_` for the passed `Block` does not have the correct head:\n"
-                f"`tail_len`       : {self._startn_tail_length}\n"
+                f"`tail_len`      : {self._startn_tail_length}\n"
                 f"expected `head` : {self._startn_head}\n"
-                f"`startn_`       : {blk.startn()}\n"
-                f"`startn_` head  : {startn_head}\n"
+                f"`startn`        : {blk.startn()}\n"
+                f"`startn` head   : {startn_head}\n"
                 "Please see the method `set_startn_info` to troubleshoot this error."
             )
 
         if len(blk) > self._max_length:
             raise ValueError
 
         if _debug == 1:
             raise KeyboardInterrupt
 
         txn = None
         filename = None
 
+        if not dups_ok and blk.apri() in self:
+
+            int_ = (blk.startn(), len(blk))
+
+            for t in self.intervals(blk.apri(), False, True, False):
+
+                if intervals_overlap(t, int_):
+                    raise RegisterError(
+                        "Attempted to add a `Block` with duplicate indices. Set `dups_ok` to `True` to suppress."
+                    )
+
         if _debug == 2:
             raise KeyboardInterrupt
 
         try:
 
             with ReversibleTransaction(self._db).begin(write = True) as txn:
 
@@ -1657,47 +1627,40 @@
 
         if ret_metadata:
             return self.blk_metadata(blk.apri(), blk.startn(), len(blk), False)
 
         else:
             return None
 
-    def append_disk_blk(self, blk, exists_ok = False, ret_metadata = False, **kwargs):
+    def append_disk_blk(self, blk, ret_metadata = False, **kwargs):
         """Add a `Block` to disk and link it with this `Register`.
 
-        If no disk `Block`s with the same `ApriInfo` as `blk` have previously been added to disk, then `blk` will be
-        added to this `Register` via the method `add_disk_blk`. If not, then `startn_` will be set to one more than the
-        largest index among all disk `Block`s with the same `ApriInfo` as `blk`.
+        If no disk `Block`s with the same `ApriInfo` as `blk` have previously been added to disk, then `startn` is set
+        to 0.. If not, then `startn` will be set to one more than the largest index among all disk `Block`s with the
+        same `ApriInfo` as `blk`.
 
         :param blk: (type `Block`)
         :param ret_metadata: (type `bool`, default `False`) Whether to return a `File_Metadata` object, which
         contains file creation date/time and size of dumped data to the disk.
         :raises RegisterError: If a duplicate `Block` already exists in this `Register`.
         """
 
+        self._check_open_raise("append_disk_blk")
+        self._check_readwrite_raise("append_disk_blk")
+        Register._check_blk_open_raise(blk, "append_disk_blk")
         check_type(blk, "blk", Block)
-        check_type(exists_ok, "exists_ok", bool)
         check_type(ret_metadata, "ret_metadata", bool)
 
         if self.num_blks(blk.apri(), diskonly = True) == 0:
-            return self.add_disk_blk(blk, exists_ok, ret_metadata, **kwargs)
+            return self.add_disk_blk(blk, ret_metadata, **kwargs)
 
         else:
 
-            startn = 0
-
-            for key, _ in self._iter_disk_blk_pairs(_BLK_KEY_PREFIX, blk.apri(), None):
-
-                _, _startn, _length = self._convert_disk_block_key(_BLK_KEY_PREFIX_LEN, key)
-
-                if startn < _startn + _length:
-                    startn = _startn + _length
-
-            blk.set_startn(startn)
-            return self.add_disk_blk(blk, exists_ok, ret_metadata, **kwargs)
+            blk.set_startn(self.maxn(blk.apri()) + 1)
+            return self.add_disk_blk(blk, ret_metadata, **kwargs)
 
     def rmv_disk_blk(self, apri, startn = None, length = None, missing_ok = False, recursively = False, **kwargs):
         """Delete a disk `Block` and unlink it with this `Register`.
 
         :param apri: (type `ApriInfo`)
         :param startn: (type `int`) Non-negative.
         :param length: (type `int`) Non-negative.
@@ -1728,84 +1691,84 @@
 
         else:
 
             if _debug == 1:
                 raise KeyboardInterrupt
 
             txn = None
-            blkFilename = None
-            comprFilename = None
+            blk_filename = None
+            compr_filename = None
 
             if _debug == 2:
                 raise KeyboardInterrupt
 
             try:
 
                 if _debug == 3:
                     raise KeyboardInterrupt
 
                 with ReversibleTransaction(self._db).begin(write = True) as txn:
 
                     if _debug == 4:
                         raise KeyboardInterrupt
 
-                    blkFilename, comprFilename = self._rmv_disk_blk_txn(apri, startn_, length_, txn)
+                    blk_filename, compr_filename = self._rmv_disk_blk_txn(apri, startn_, length_, txn)
 
                     if _debug == 5:
                         raise KeyboardInterrupt
 
                 if _debug == 6:
                     raise KeyboardInterrupt
 
-                if not is_deletable(blkFilename):
-                    raise OSError(f"Cannot delete `Block` file `{str(blkFilename)}`.")
+                if not is_deletable(blk_filename):
+                    raise OSError(f"Cannot delete `Block` file `{str(blk_filename)}`.")
 
                 if _debug == 7:
                     raise KeyboardInterrupt
 
-                if comprFilename is not None and not is_deletable(comprFilename):
-                    raise OSError(f"Cannot delete compressed `Block` file `{str(comprFilename)}`.")
+                if compr_filename is not None and not is_deletable(compr_filename):
+                    raise OSError(f"Cannot delete compressed `Block` file `{str(compr_filename)}`.")
 
                 if _debug == 8:
                     raise KeyboardInterrupt
 
-                if comprFilename is not None:
+                if compr_filename is not None:
 
-                    blkFilename.unlink()
+                    blk_filename.unlink()
 
                     if _debug == 9:
                         raise KeyboardInterrupt
 
-                    comprFilename.unlink()
+                    compr_filename.unlink()
 
                 else:
-                    type(self).clean_disk_data(blkFilename, **kwargs)
+                    type(self).clean_disk_data(blk_filename, **kwargs)
 
                 return
 
             except BaseException as e:
 
                 FAIL_NO_RECOVER_ERROR_MESSAGE = "Could not successfully recover from a failed disk `Block` remove!"
 
                 try:
 
-                    if comprFilename is not None:
+                    if compr_filename is not None:
 
-                        if blkFilename is not None and comprFilename.exists():
+                        if blk_filename is not None and compr_filename.exists():
 
                             try:
-                                blkFilename.touch()
+                                blk_filename.touch()
 
                             except FileExistsError:
                                 pass
 
                         else:
                             raise RegisterRecoveryError(FAIL_NO_RECOVER_ERROR_MESSAGE) from e
 
-                    elif blkFilename is not None and not blkFilename.exists():
+                    elif blk_filename is not None and not blk_filename.exists():
                         raise RegisterRecoveryError(FAIL_NO_RECOVER_ERROR_MESSAGE) from e
 
                     if txn is not None:
 
                         with self._db.begin(write = True) as txn_:
                             txn.reverse(txn_)
 
@@ -2183,14 +2146,20 @@
     #
     #     :param hashing: (type `bool`)
     #     """
 
     #################################
     #    PROTEC DISK BLK METHODS    #
 
+    @staticmethod
+    def _check_blk_open_raise(blk, method_name):
+
+        if not blk._entered:
+            raise BlockNotOpenError(f"You must do `with blk:` before you call `reg.{method_name}()`.")
+
     def _add_disk_blk_txn(self, blk, txn):
 
         # DEBUG : 6,7,8,9, 10
 
         apris = [apri for _, apri in blk.apri().iter_inner_info() if isinstance(apri, ApriInfo)]
 
         if _debug == 6:
@@ -2241,28 +2210,26 @@
 
             return filename
 
         else:
 
             raise RegisterError(
                 f"Duplicate `Block` with the following data already exists in this `Register`: " +
-                f"{str(blk.apri())}, startn_ = {blk.startn()}, length_ = {len(blk)}."
+                f"{str(blk.apri())}, startn = {blk.startn()}, length = {len(blk)}."
             )
 
     def _rmv_disk_blk_txn(self, apri, startn, length, txn):
 
         if _debug == 12:
             raise KeyboardInterrupt
-
         # raises DataNotFoundError
         self._get_id_by_apri(apri, None, False, txn, None)
 
         if _debug == 13:
             raise KeyboardInterrupt
-
         # raises RegisterError and DataNotFoundError
         blk_key, compressed_key = self._check_blk_compressed_keys_raise(None, None, apri, None, startn, length, txn)
 
         if _debug == 14:
             raise KeyboardInterrupt
 
         blk_filename, compr_filename = self._check_blk_compressed_files_raise(
@@ -2305,16 +2272,16 @@
         :return: (type `bytes`)
         """
 
         if apri is None and apri_json is None:
             raise ValueError
 
         id_ = self._get_id_by_apri(apri, apri_json, missing_ok, txn, None)
-        tail = bytify_num(startn % self._startn_tail_mod, self._startn_tail_length)
-        op_length = bytify_num(self._max_length - length, self._length_length)
+        tail = bytify_int(startn % self._startn_tail_mod, self._startn_tail_length)
+        op_length = bytify_int(self._max_length - length, self._length_length)
 
         return (
                 prefix   +
                 id_      + _KEY_SEP +
                 tail     + _KEY_SEP +
                 op_length
         )
@@ -2491,30 +2458,40 @@
 
     #################################
     #    PUBLIC RAM BLK METHODS     #
 
     def add_ram_blk(self, blk):
 
         self._check_open_raise("add_ram_blk")
+        self._check_readwrite_raise("add_ram_blk")
+        Register._check_blk_open_raise(blk, "add_ram_blk")
         check_type(blk, "blk", Block)
 
         if blk.apri() not in self._ram_blks.keys():
             self._ram_blks[blk.apri()] = [blk]
 
         elif len(self._ram_blks[blk.apri()]) == 0:
             self._ram_blks[blk.apri()].append(blk)
 
         else:
 
             for i, blk_ in enumerate(self._ram_blks[blk.apri()]):
 
+                try:
+                    blk_len = len(blk_)
+
+                except BlockNotOpenError as e:
+                    raise BlockNotOpenError(
+                        _RAM_BLOCK_NOT_OPEN_ERROR_MESSAGE.format(blk_.apri(), blk_.startn())
+                    ) from e
+
                 if blk_ is blk:
                     break
 
-                elif blk.startn() < blk_.startn() or (blk.startn() == blk_.startn() and len(blk) > len(blk_)):
+                elif blk.startn() < blk_.startn() or (blk.startn() == blk_.startn() and len(blk) > blk_len):
 
                     self._ram_blks[blk.apri()].insert(i, blk)
                     break
 
             else:
                 self._ram_blks[blk.apri()].append(blk)
 
@@ -2547,14 +2524,15 @@
 
     #################################
     #    PROTEC RAM BLK METHODS     #
 
     #################################
     # PUBLIC RAM & DISK BLK METHODS #
 
+    @contextmanager
     def blk_by_n(self, apri, n, diskonly = False, recursively = False, ret_metadata = False, **kwargs):
 
         self._check_open_raise("blk_by_n")
         check_type(apri, "apri", ApriInfo)
         n = check_return_int(n, "n")
         check_type(diskonly, "diskonly", bool)
         check_type(recursively, "recursively", bool)
@@ -2572,34 +2550,42 @@
                 raise
 
         else:
 
             for startn, length in self.intervals(apri, combine = False, diskonly = diskonly, recursively = False):
 
                 if startn <= n < startn + length:
-                    return self.blk(apri, startn, length, diskonly, False, ret_metadata, **kwargs)
+
+                    with self.blk(apri, startn, length, diskonly, False, ret_metadata, **kwargs) as blk:
+
+                        yield blk
+                        return
 
         if recursively:
 
             for subreg in self._iter_subregs():
 
                 with subreg._recursive_open(True) as subreg:
 
                     try:
-                        return subreg.blk_by_n(apri, n, diskonly, True, ret_metadata, **kwargs)
+
+                        with subreg.blk_by_n(apri, n, diskonly, True, ret_metadata, **kwargs) as blk:
+
+                            yield blk
+                            return
 
                     except DataNotFoundError:
                         pass
 
         raise DataNotFoundError(_blk_not_found_err_msg(diskonly, apri, n))
 
+    @contextmanager
     def blk(self, apri, startn = None, length = None, diskonly = False, recursively = False, ret_metadata = False, **kwargs):
 
         self._check_open_raise("blk")
-
         check_type(apri, "apri", ApriInfo)
         startn = check_return_int_None_default(startn, "startn", None)
         length = check_return_int_None_default(length, "length", None)
         check_type(diskonly, "diskonly", bool)
         check_type(recursively, "recursively", bool)
         check_type(ret_metadata, "ret_metadata", bool)
 
@@ -2621,21 +2607,31 @@
 
             startn_, length_ = self._resolve_startn_length(apri, startn, length, diskonly)
 
             if not diskonly and apri in self._ram_blks.keys():
 
                 for blk in self._ram_blks[apri]:
 
-                    if blk.startn() == startn_ and len(blk) == length_:
+                    try:
+                        blk_len = len(blk)
+
+                    except BlockNotOpenError as e:
+                        raise BlockNotOpenError(_RAM_BLOCK_NOT_OPEN_ERROR_MESSAGE.format(apri, blk.startn())) from e
+
+                    if blk.startn() == startn_ and blk_len == length_:
 
                         if ret_metadata:
-                            return blk, None
+
+                            yield blk, None
+                            return
 
                         else:
-                            return blk
+
+                            yield blk
+                            return
 
             try:
                 blk_key, compressed_key = self._check_blk_compressed_keys_raise(None, None, apri, None, startn_, length_)
 
             except DataNotFoundError:
                 pass
 
@@ -2651,37 +2647,63 @@
                         )
 
                 blk_filename, _ = self._check_blk_compressed_files_raise(blk_key, compressed_key, apri, startn_, length_)
                 blk_filename = self._local_dir / blk_filename
                 data = type(self).load_disk_data(blk_filename, **kwargs)
                 blk = Block(data, apri, startn_)
 
-                if ret_metadata:
-                    return blk, FileMetadata.from_path(blk_filename)
+                with blk:
 
-                else:
-                    return blk
+                    if ret_metadata:
+                        yield blk, FileMetadata.from_path(blk_filename)
+
+                    else:
+                        yield blk
+
+                return
 
         if recursively:
 
             for subreg in self._iter_subregs():
 
                 with subreg._recursive_open(True) as subreg:
 
                     try:
-                        return subreg.blk(apri, startn, length, ret_metadata, ret_metadata=True)
+
+                        with subreg.blk(apri, startn, length, ret_metadata, ret_metadata=True) as blk:
+                            yield blk
+
+                        return
 
                     except DataNotFoundError:
                         pass
 
         raise DataNotFoundError(
             _blk_not_found_err_msg(diskonly, str(apri), None, startn, length)
         )
 
     def blks(self, apri, diskonly = False, recursively = False, ret_metadata = False, **kwargs):
+        """Iterate over all `Block`s with `apri`.
+
+        This is a convenience method that should be used only for simple data manipulation. This method opens
+        only one `Block` at a time; each is closed automatically before the next `Block` is yielded (hence it is
+        not necessary to use a `with` clause).
+
+        The following idiom is equivalent to `for blk in reg.blks(apri):`
+
+            for startn, length in self.intervals(apri):
+                with reg.blk(startn, length) as blk:
+                    ...
+
+        :param apri: (type `ApriInfo`)
+        :param diskonly: (type `bool`, default `False`)
+        :param recursively: (type `bool`, default `False`)
+        :param ret_metadata: (type `bool`, default `False`)
+        :return:
+        """
 
         self._check_open_raise("blks")
         check_type(apri, "apri", ApriInfo)
         check_type(diskonly, "diskonly", bool)
         check_type(recursively, "recursively", bool)
         check_type(ret_metadata, "ret_metadata", bool)
 
@@ -2694,40 +2716,48 @@
                 raise
 
         else:
 
             for startn, length in self.intervals(apri, combine = False, diskonly = diskonly, recursively = recursively):
 
                 try:
-                    yield self.blk(apri, startn, length, diskonly, False, ret_metadata, **kwargs)
+
+                    with self.blk(apri, startn, length, diskonly, False, ret_metadata, **kwargs) as blk:
+                        yield blk
 
                 except DataNotFoundError:
                     pass
 
         if recursively:
 
             for subreg in self._iter_subregs():
 
                 with subreg._recursive_open(True) as subreg:
                     yield from subreg.blks(apri, diskonly, True, ret_metadata, **kwargs)
 
+    @contextmanager
     def __getitem__(self, apri_n_diskonly_recursively):
-        return self.get(*Register._resolve_apri_n_diskonly_recursively(apri_n_diskonly_recursively))
 
+        with self.get(*Register._resolve_apri_n_diskonly_recursively(apri_n_diskonly_recursively)) as yield_:
+            yield yield_
+
+    @contextmanager
     def get(self, apri, n, diskonly = False, recursively = False, **kwargs):
 
         self._check_open_raise("get")
 
+        n_slice = isinstance(n, slice)
+
         if not isinstance(apri, ApriInfo):
             raise TypeError("The first argument to `reg[]` must be an `ApriInfo.")
 
-        if not is_int(n) and not isinstance(n, slice):
+        if not is_int(n) and n_slice:
             raise TypeError("The second argument to `reg[]` must be an `int` or a `slice`.")
 
-        elif is_int(n):
+        elif not n_slice:
             n = int(n)
 
         else:
 
             _n = [None]*3
 
             if n.start is not None and not is_int(n.start):
@@ -2752,15 +2782,15 @@
 
         if not isinstance(diskonly, bool):
             raise TypeError("The second argument of `reg[]` must be of type `bool`.")
 
         if not isinstance(recursively, bool):
             raise TypeError("The third argument of `reg[]` must be of type `bool`.")
 
-        if isinstance(n, slice):
+        if n_slice:
 
             if n.start is not None and n.start < 0:
                 raise ValueError("Start index cannot be negative.")
 
             if n.stop is not None and n.stop < 0:
                 raise ValueError("Stop index cannot be negative.")
 
@@ -2770,27 +2800,23 @@
         except DataNotFoundError:
 
             if not recursively:
                 raise
 
         else:
 
-            if isinstance(n, slice):
-                # return iterator if given slice
-                return _ElementIter(self, apri, n, diskonly, recursively, kwargs)
-
-            else:
+            if n_slice:
 
-                blk = self.blk_by_n(apri, n, diskonly, recursively, False, **kwargs)
-                ret = blk[n]
+                yield _element_iter(self, apri, n, diskonly, recursively, kwargs)
+                return
 
-                if isinstance(blk, ReleaseBlock):
-                    blk.release()
+            else:
 
-                return ret
+                with self.blk_by_n(apri, n, diskonly, recursively, False, **kwargs) as blk:
+                    yield blk.segment()
 
         if recursively:
 
             for subreg in self._iter_subregs():
 
                 with subreg._recursive_open(True) as subreg:
 
@@ -2951,14 +2977,50 @@
 
         if ret == -1:
             raise DataNotFoundError(_blk_not_found_err_msg(diskonly, apri))
 
         else:
             return ret
 
+    def contains_index(self, apri, index, diskonly = False, recursively = False):
+
+        check_type(apri, "apri", ApriInfo)
+        index = check_return_int(index, "index")
+        check_type(diskonly, "diskonly", bool)
+        check_type(recursively, "recursively", bool)
+
+        if index < 0:
+            raise ValueError("`index` must be non-negative.")
+
+        for startn, length in self.intervals(apri, False, diskonly, recursively):
+
+            if startn <= index < startn + length:
+                return True
+
+        else:
+            return False
+
+    def contains_interval(self, apri, startn, length, diskonly = False, recursively = False):
+
+        check_type(apri, "apri", ApriInfo)
+        startn = check_return_int(startn, "startn")
+        length = check_return_int(length, "length")
+        check_type(diskonly, "diskonly", bool)
+        check_type(recursively, "recursively", bool)
+
+        int1 = (startn, length)
+
+        for int2 in self.intervals(apri, True, diskonly, recursively):
+
+            if intervals_overlap(int1, int2):
+                return intervals_subset(int1, int2)
+
+        else:
+            return False
+
     #################################
     # PROTEC RAM & DISK BLK METHODS #
 
     @staticmethod
     def _resolve_apri_n_diskonly_recursively(apri_n_diskonly_recursively):
 
         if not isinstance(apri_n_diskonly_recursively, tuple) or len(apri_n_diskonly_recursively) <= 1:
@@ -2997,25 +3059,42 @@
 
         if startn is None and length is not None:
             raise ValueError(f"If you specify a `Block` length, you must also specify a `startn`.")
 
         elif startn is not None and length is not None:
             return startn, length
 
-        if not diskonly and apri in self._ram_blks.keys():
+        if not diskonly and apri in self._ram_blks.keys() and len(self._ram_blks[apri]) > 0:
 
             if startn is not None and length is None:
 
                 for blk in self._ram_blks[apri]:
 
+                    try:
+                        blk_len = len(blk)
+
+                    except BlockNotOpenError as e:
+                        raise BlockNotOpenError(
+                            _RAM_BLOCK_NOT_OPEN_ERROR_MESSAGE.format(blk.apri(), blk.startn())
+                        ) from e
+
                     if blk.startn() == startn:
-                        return startn, len(blk)
+                        return startn, blk_len
 
             else:
-                return self._ram_blks[apri][0].startn(), len(self._ram_blks[apri][0])
+
+                blk = self._ram_blks[apri][0]
+
+                try:
+                    blk_len = len(blk)
+
+                except BlockNotOpenError as e:
+                    raise BlockNotOpenError(_RAM_BLOCK_NOT_OPEN_ERROR_MESSAGE.format(blk.apri(), blk.starn())) from e
+
+                return blk.startn(), blk_len
 
         if startn is not None and length is None:
 
             key = self._get_disk_blk_key(_BLK_KEY_PREFIX, apri, None, startn, 1, False, txn) # raises DataNotFoundError
             first_key_sep_index = key.find(_KEY_SEP)
             second_key_sep_index = key.find(_KEY_SEP, first_key_sep_index + 1)
             prefix = key [ : second_key_sep_index + 1]
@@ -3057,15 +3136,24 @@
                         raise
 
                 else:
 
                     if not diskonly and apri in self._ram_blks.keys():
 
                         for blk in self._ram_blks[apri]:
-                            yield blk.startn(), len(blk)
+
+                            try:
+                                blk_len = len(blk)
+
+                            except BlockNotOpenError as e:
+                                raise BlockNotOpenError(
+                                    _RAM_BLOCK_NOT_OPEN_ERROR_MESSAGE.format(apri, blk.startn())
+                                ) from e
+
+                            yield blk.startn(), blk_len
 
                     try:
 
                         for key, _ in self._iter_disk_blk_pairs(_BLK_KEY_PREFIX, apri, None, txn):
                             yield self._convert_disk_block_key(_BLK_KEY_PREFIX_LEN, key, apri, txn)[1:]
 
                     except DataNotFoundError:
@@ -3231,53 +3319,62 @@
                         return subreg.set(apri, n, value, diskonly, recursively, mmap_mode = mmap_mode, **kwargs)
 
                     except DataNotFoundError:
                         pass
 
         raise DataNotFoundError(_blk_not_found_err_msg(diskonly, str(apri), n))
 
-
+    @contextmanager
     def blk(self, apri, startn = None, length = None, diskonly = False, recursively = False, ret_metadata = False, **kwargs):
         """
         :param apri: (type `ApriInfo`)
         :param startn: (type `int`)
         :param length: (type `length_`) non-negative
         :param ret_metadata: (type `bool`, default `False`) Whether to return a `File_Metadata` object, which
         contains file creation date/time and size of dumped saved on the disk.
         :param recursively: (type `bool`, default `False`) Search all subregisters for the `Block`.
         :param mmap_mode: (type `str`, optional) Load the Numpy file using memory mapping, see
         https://numpy.org/doc/stable/reference/generated/numpy.memmap.html#numpy.memmap for more information.
         :return: (type `File_Metadata`) If `ret_metadata is True`.
         """
 
-        ret = super().blk(apri, startn, length, diskonly, recursively, ret_metadata, **kwargs)
+        with super().blk(apri, startn, length, diskonly, recursively, ret_metadata, **kwargs) as ret:
 
-        if ret_metadata:
-            blk = ret[0]
+            if ret_metadata:
+                blk = ret[0]
 
-        else:
-            blk = ret
+            else:
+                blk = ret
 
-        if isinstance(blk.segment(), np.memmap):
-            blk = MemmapBlock(blk.segment(), blk.apri(), blk.startn())
+            if issubclass(blk.segment_type, np.memmap):
 
-        if ret_metadata:
-            return blk, ret[1]
+                with MemmapBlock.cast(blk) as blk:
 
-        else:
-            return blk
+                    if ret_metadata:
+                        yield blk, ret[1]
+
+                    else:
+                        yield blk
+
+            else:
+
+                if ret_metadata:
+                    yield blk, ret[1]
+
+                else:
+                    yield blk
 
     def concat_disk_blks(self, apri, startn = None, length = None, delete = False, ret_metadata = False):
         """Concatenate several `Block`s into a single `Block` along axis 0 and save the new one to the disk.
 
         If `delete = True`, then the smaller `Block`s are deleted automatically.
 
         The interval `range(startn, startn + length)` must be the disjoint union of intervals of the form
         `range(blk.startn(), blk.startn() + len(blk))`, where `blk` is a disk `Block` with `ApriInfo`
-        given by `info`.
+        given by `apri`.
 
         Length-0 `Block`s are ignored.
 
         If `startn` is not specified, it is taken to be the smallest `startn` of any `Block` saved to this
         `Register`. If `length` is not specified, it is taken to be the length of the largest
         contiguous set of indices that start with `startn`. If `startn` is not specified but `length` is, a
         ValueError is raised.
@@ -3453,161 +3550,114 @@
             if ret_metadata:
                 return self.blk_metadata(apri, *intervals_to_get)
 
             else:
                 return None
 
         blks = []
+        metadata = []
         fixed_shape = None
-        ref_blk = None
+        ref_blk_startn = None
+        ref_blk_len = None
         failure_reinsert_indices = []
         combined_blk = None
 
         try:
+            # All blocks will be opened and will remain open until they are concatenated
+            stack = ExitStack()
 
-            for startn_, length_ in intervals_to_get:
-                # check that blocks have the correct shape
-
-                blk = self.blk(apri, startn_, length_, True, False, False, mmap_mode="r")
-                blks.append(blk)
-
-                if fixed_shape is None:
+            with stack:
 
-                    fixed_shape = blk.segment().shape[1:]
-                    ref_blk = blk
+                for startn_, length_ in intervals_to_get:
 
-                elif fixed_shape != blk.segment().shape[1:]:
+                    blk = stack.enter_context(self.blk(apri, startn_, length_, True, False, False, mmap_mode="r"))
+                    blks.append(blk)
+                    metadata.append((startn_, length_))
+                    # check that all shapes are correct
+                    if fixed_shape is None:
+                        # initialize correct shape
+                        fixed_shape = blk.segment().shape[1:]
+                        ref_blk_startn = blk.startn()
+                        ref_blk_len = len(blk)
 
-                    raise ValueError(
-                        "Cannot combine the following two `Block`s because all axes other than axis 0 must have the same " +
-                        "shape:\n" +
-                        f"{str(apri)}, startn = {ref_blk.startn()}, length = {len(ref_blk)}\n, shape = " +
-                        f"{str(fixed_shape)}\n" +
-                        f"{str(apri)}, startn = {startn_}, length = {length_}\n, shape = " +
-                        f"{str(blk.segment().shape)}\n"
+                    elif fixed_shape != blk.segment().shape[1:]:
+                        raise ValueError(
+                            "Cannot combine the following two `Block`s because all axes other than axis 0 must have the"
+                            " same shape:\n"
+                            f"{str(apri)}, startn = {ref_blk_startn}, length = {ref_blk_len}\n, shape = "
+                            f"{str(fixed_shape)}\n"
+                            f"{str(apri)}, startn = {startn_}, length = {length_}\n, shape = "
+                            f"{str(blk.segment().shape)}"
+                        )
 
-                    )
+                combined_blk = np.concatenate([blk.segment() for blk in blks], axis=0)
+                combined_blk = Block(combined_blk, apri, startn)
 
-            combined_blk = np.concatenate([blk.segment() for blk in blks], axis=0)
-            combined_blk = Block(combined_blk, apri, startn)
-            ret = self.add_disk_blk(combined_blk, ret_metadata)
+                with combined_blk:
+                    ret = self.add_disk_blk(combined_blk, ret_metadata)
 
-            if _debug == 1:
-                raise KeyboardInterrupt
+                if _debug == 1:
+                    raise KeyboardInterrupt
 
             if delete:
 
-                for blk in blks:
+                for startn_, length_ in metadata:
 
-                    startn_ = blk.startn()
-                    length_ = len(blk)
-                    blk.release()
                     self.rmv_disk_blk(apri, startn_, length_, False)
                     failure_reinsert_indices.append((startn_, length_))
 
                     if _debug == 2:
                         raise KeyboardInterrupt
 
         except BaseException as e:
 
             try:
 
                 if combined_blk is not None and isinstance(combined_blk, Block) and delete:
 
-                    for startn_, length_ in failure_reinsert_indices:
-                        self.add_disk_blk(combined_blk[startn_: startn_ + length_])
+                    with combined_blk:
 
-            except BaseException:
-                raise RegisterRecoveryError(_FAIL_NO_RECOVER_ERROR_MESSAGE)
-
-            else:
-                raise e
-
-        finally:
+                        for startn_, length_ in failure_reinsert_indices:
 
-            for blk in blks:
-                blk.release()
+                            reinsert_blk = Block(combined_blk[startn_: startn_ + length_], apri, startn_)
 
-        return ret
+                            with reinsert_blk:
+                                self.add_disk_blk(combined_blk[startn_: startn_ + length_])
 
-class _ElementIter:
+            except BaseException as ee:
+                raise RegisterRecoveryError(_FAIL_NO_RECOVER_ERROR_MESSAGE) from ee
 
-    def __init__(self, reg, apri, slc, diskonly, recursively, kwargs):
-
-        self.reg = reg
-        self.apri = apri
-        self.step = slc.step if slc.step else 1
-        self.stop = slc.stop
-        self.diskonly = diskonly
-        self.recursively = recursively
-        self.kwargs = kwargs
-        self.curr_blk = None
-        self.intervals = None
-        self.curr_n = slc.start if slc.start else 0
-
-    def update_intervals_calculated(self):
-
-        self.intervals = list(
-            self.reg.intervals(self.apri, combine = False, diskonly = self.diskonly, recursively = self.recursively)
-        )
-
-    def get_next_blk(self):
-
-        if self.curr_blk is not None and isinstance(self.curr_blk, ReleaseBlock):
-            self.curr_blk.release()
-
-        return self.reg.blk_by_n(self.apri, self.curr_n, self.diskonly, self.recursively, False, **self.kwargs)
-
-    def __iter__(self):
-        return self
-
-    def __next__(self):
-
-        if self.stop is not None and self.curr_n >= self.stop:
-            raise StopIteration
-
-        elif self.curr_blk is None:
-
-            self.update_intervals_calculated()
-
-            if len(self.intervals) == 0:
-                raise StopIteration
-
-            self.curr_n = max(self.intervals[0][0], self.curr_n)
-
-            try:
-                self.curr_blk = self.get_next_blk()
-
-            except DataNotFoundError:
-                raise StopIteration
+            else:
+                raise e
 
-        elif self.curr_n not in self.curr_blk:
+        return ret
 
-            try:
-                self.curr_blk = self.get_next_blk()
+def _element_iter(reg, apri, slice_, diskonly, recursively, kwargs):
 
-            except DataNotFoundError:
+    n = slice_.start if slice_.start is not None else 0
+    stop = slice_.stop
+    step = slice_.step if slice_.step is not None else 1
 
-                self.update_intervals_calculated()
+    while True:
 
-                for startn, length in self.intervals:
+        try:
+            blk_contextmanager = reg.blk_by_n(apri, n, diskonly, recursively, False, **kwargs)
 
-                    if startn > self.curr_n:
+        except DataNotFoundError:
+            return
 
-                        self.curr_n += math.ceil( (startn - self.curr_n) / self.step ) * self.step
-                        break
+        with blk_contextmanager as blk:
 
-                else:
-                    raise StopIteration
+            while n < stop and n in blk:
 
-                self.curr_blk = self.get_next_blk()
+                yield blk[n]
+                n += step
 
-        ret = self.curr_blk[self.curr_n]
-        self.curr_n += self.step
-        return ret
+            if n >= stop:
+                return
 
 class _CopyRegister(Register):
 
     @classmethod
     def with_suffix(cls, filename):
         return filename
 
@@ -3623,18 +3673,16 @@
         shutil.copyfile(data, filename)
         return filename
 
     @classmethod
     def load_disk_data(cls, filename, **kwargs):
         raise NotImplementedError
 
-    def set_cls_name(self, clsName):
-
-        with self._cls_filepath.open() as fh:
-            fh.write(clsName)
+    def set_cls_name(self, cls_name):
+        write_txt_file(cls_name, self._cls_filepath)
 
 ###################
 # RELATIONAL INFO #
 ###################
 
 _RELATIONAL_APRI_PREFIX = (_APRI_ID_KEY_PREFIX + _KEY_SEP).decode("ASCII")
 _RELATIONAL_APRI_PREFIX_LEN = len(_RELATIONAL_APRI_PREFIX)
```

### Comparing `cornifer-0.7/lib/cornifer/regloader.py` & `cornifer-0.8/lib/cornifer/regloader.py`

 * *Files identical despite different names*

### Comparing `cornifer-0.7/setup.py` & `cornifer-0.8/setup.py`

 * *Files identical despite different names*

### Comparing `cornifer-0.7/tests/test_info.py` & `cornifer-0.8/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `cornifer-0.7/tests/test_register_file_structure.py` & `cornifer-0.8/tests/test_register_file_structure.py`

 * *Files identical despite different names*

### Comparing `cornifer-0.7/tests/test_registers.py` & `cornifer-0.8/tests/test_registers.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,25 +4,26 @@
 from itertools import product, chain
 from pathlib import Path
 from unittest import TestCase
 
 import cornifer
 import numpy as np
 
-from cornifer import NumpyRegister, Register, Block, load
+from cornifer import NumpyRegister, Register, Block, load, open_blks, open_regs
 from cornifer.info import ApriInfo, AposInfo
 from cornifer._utilities import random_unique_filename
 from cornifer.errors import RegisterAlreadyOpenError, DataNotFoundError, RegisterError, CompressionError, \
     DecompressionError, RegisterRecoveryError
 from cornifer.regfilestructure import REG_FILENAME, VERSION_FILEPATH, MSG_FILEPATH, CLS_FILEPATH, \
     DATABASE_FILEPATH, MAP_SIZE_FILEPATH
 from cornifer.registers import _BLK_KEY_PREFIX, _KEY_SEP, \
     _APRI_ID_KEY_PREFIX, _ID_APRI_KEY_PREFIX, _START_N_HEAD_KEY, _START_N_TAIL_LENGTH_KEY, _SUB_KEY_PREFIX, \
     _COMPRESSED_KEY_PREFIX, _IS_NOT_COMPRESSED_VAL, _BLK_KEY_PREFIX_LEN, _SUB_VAL, _APOS_KEY_PREFIX, _NO_DEBUG, \
-    _START_N_TAIL_LENGTH_DEFAULT, _LENGTH_LENGTH_KEY, _LENGTH_LENGTH_DEFAULT, _CURR_ID_KEY
+    _START_N_TAIL_LENGTH_DEFAULT, _LENGTH_LENGTH_KEY, _LENGTH_LENGTH_DEFAULT, _CURR_ID_KEY, \
+    _INITIAL_REGISTER_SIZE_DEFAULT
 from cornifer._utilities.lmdb import lmdb_has_key, lmdb_prefix_iter, lmdb_count_keys, open_lmdb
 from cornifer.version import CURRENT_VERSION
 
 """
 PUBLIC READ-WRITE METHODS FOR LMDB:
  - set_startn_info
  - open
@@ -151,46 +152,53 @@
     @classmethod
     def load_disk_data(cls, filename, **kwargs): pass
 
     @classmethod
     def clean_disk_data(cls, filename, **kwargs):pass
 
 def data(blk):
-    return blk.apri(), blk.startn(), len(blk)
+
+    with blk:
+        return blk.apri(), blk.startn(), len(blk)
 
 class Test_Register(TestCase):
 
     def setUp(self):
         if SAVES_DIR.is_dir():
             shutil.rmtree(SAVES_DIR)
         SAVES_DIR.mkdir()
 
     def tearDown(self):
+
         if SAVES_DIR.is_dir():
             shutil.rmtree(SAVES_DIR)
+
         Register._instances.clear()
 
     def test___init__(self):
 
         shutil.rmtree(SAVES_DIR)
 
         with self.assertRaises(FileNotFoundError):
-            Testy_Register(SAVES_DIR, "tests")
+            Testy_Register(SAVES_DIR, "sh", "tests")
 
         SAVES_DIR.mkdir()
 
         with self.assertRaises(TypeError):
-            Testy_Register(SAVES_DIR, 0)
+            Testy_Register(SAVES_DIR, "sh", 0)
+
+        with self.assertRaises(TypeError):
+            Testy_Register(0, "sh", "sup")
 
         with self.assertRaises(TypeError):
-            Testy_Register(0, "sup")
+            Testy_Register(SAVES_DIR, 0, "sup")
 
-        self.assertFalse(Testy_Register(SAVES_DIR, "sup")._created)
+        self.assertFalse(Testy_Register(SAVES_DIR, "sh", "sup")._created)
 
-        self.assertEqual(Testy_Register(SAVES_DIR, "sup")._version, CURRENT_VERSION)
+        self.assertEqual(Testy_Register(SAVES_DIR, "sh", "sup")._version, CURRENT_VERSION)
 
     # def test_add_subclass(self):
     #
     #     with self.assertRaisesRegex(TypeError, "must be a class"):
     #         Register.add_subclass(0)
     #
     #     class Hello:pass
@@ -258,51 +266,57 @@
         #     self.assertEqual(
         #         split[1:],
         #         Register._split_disk_block_key(_BLK_KEY_PREFIX_LEN, Register._join_disk_block_data(*split))
         #     )
 
     def test___str__(self):
 
+        reg = Testy_Register(SAVES_DIR, "sh", "hello")
+        self.assertEqual(
+            str(reg),
+            f"sh: \"hello\""
+        )
+        with reg.open() as reg:pass
         self.assertEqual(
-            str(Testy_Register(SAVES_DIR, "hello")),
-            "hello"
+            str(reg),
+            f"sh ({reg._local_dir}): \"hello\""
         )
 
     def test___repr__(self):
 
         self.assertEqual(
-            repr(Testy_Register(SAVES_DIR, "hello")),
-            f"Testy_Register(\"{str(SAVES_DIR)}\", \"hello\")"
+            repr(Testy_Register(SAVES_DIR, "sh", "hello")),
+            f"Testy_Register(\"{str(SAVES_DIR)}\", \"sh\", \"hello\", {_INITIAL_REGISTER_SIZE_DEFAULT})"
         )
 
     def test__check_open_raise_uncreated(self):
 
-        reg = Testy_Register(SAVES_DIR, "hey")
+        reg = Testy_Register(SAVES_DIR, "sh", "hey")
 
         with self.assertRaisesRegex(RegisterError, "tests"):
             reg._check_open_raise("tests")
 
     def test__set_local_dir(self):
 
         # tests that error is raised when `local_dir` is not a sub-dir of `savesDir`
         local_dir = SAVES_DIR / "bad" / "test_local_dir"
-        reg = Testy_Register(SAVES_DIR, "sup")
+        reg = Testy_Register(SAVES_DIR, "sh", "sup")
         with self.assertRaisesRegex(ValueError, "sub-directory"):
             reg._set_local_dir(local_dir)
 
         # tests that error is raised when `Register` has not been created
         local_dir = SAVES_DIR / "test_local_dir"
-        reg = Testy_Register(SAVES_DIR, "sup")
+        reg = Testy_Register(SAVES_DIR, "sh", "sup")
         with self.assertRaisesRegex(FileNotFoundError, "database"):
             reg._set_local_dir(local_dir)
 
         # tests that newly created register has the correct filestructure and instance attributes
         # register database must be manually created for this tests case
         local_dir = SAVES_DIR / "test_local_dir"
-        reg = Testy_Register(SAVES_DIR, "sup")
+        reg = Testy_Register(SAVES_DIR, "sh", "sup")
         local_dir.mkdir()
         (local_dir / REG_FILENAME).mkdir(exist_ok = False)
         (local_dir / VERSION_FILEPATH).touch(exist_ok = False)
         (local_dir / MSG_FILEPATH).touch(exist_ok = False)
         (local_dir / CLS_FILEPATH).touch(exist_ok = False)
         (local_dir / DATABASE_FILEPATH).mkdir(exist_ok = False)
         (local_dir / MAP_SIZE_FILEPATH).touch(exist_ok = False)
@@ -335,104 +349,96 @@
             )
 
         finally:
             reg._db.close()
 
     def test___hash___uncreated(self):
         with self.assertRaisesRegex(RegisterError, "__hash__"):
-            hash(Testy_Register(SAVES_DIR, "hey"))
+            hash(Testy_Register(SAVES_DIR, "sh", "hey"))
 
     def test___eq___uncreated(self):
         with self.assertRaises(RegisterError):
-            Testy_Register(SAVES_DIR, "hey") == Testy_Register(SAVES_DIR, "sup")
+            Testy_Register(SAVES_DIR, "sh", "hey") == Testy_Register(SAVES_DIR, "sh", "sup")
 
     def test_add_ram_block(self):
 
-        reg = Testy_Register(SAVES_DIR, "msg")
+        reg = Testy_Register(SAVES_DIR, "sh", "msg")
         blk = Block([], ApriInfo(name ="tests"))
 
-        reg = Testy_Register(SAVES_DIR, "msg")
+        reg = Testy_Register(SAVES_DIR, "sh", "msg")
         blk1 = Block([], ApriInfo(name ="tests"))
-
-        with reg.open() as reg:
-            reg.add_ram_blk(blk1)
-
-        self.assertEqual(
-            1,
-            len(reg._ram_blks)
-        )
-
-        self.assertEqual(
-            1,
-            len(reg._ram_blks[ApriInfo(name ="tests")])
-        )
-
         blk2 = Block([], ApriInfo(name = "testy"))
+        blk3 = Block([], ApriInfo(name="testy"))
+        blk4 = Block([1], ApriInfo(name="testy"))
 
         with reg.open() as reg:
-            reg.add_ram_blk(blk2)
-
-        self.assertEqual(
-            2,
-            len(reg._ram_blks)
-        )
-
-        self.assertEqual(
-            1,
-            len(reg._ram_blks[ApriInfo(name ="tests")])
-        )
-
-        self.assertEqual(
-            1,
-            len(reg._ram_blks[ApriInfo(name ="testy")])
-        )
-
-        blk3 = Block([], ApriInfo(name = "testy"))
-
-        with reg.open() as reg:
-            reg.add_ram_blk(blk3)
 
-        self.assertEqual(
-            2,
-            len(reg._ram_blks)
-        )
+            with blk1:
 
-        self.assertEqual(
-            1,
-            len(reg._ram_blks[ApriInfo(name="tests")])
-        )
+                reg.add_ram_blk(blk1)
+                self.assertEqual(
+                    1,
+                    len(reg._ram_blks)
+                )
+                self.assertEqual(
+                    1,
+                    len(reg._ram_blks[ApriInfo(name ="tests")])
+                )
 
-        self.assertEqual(
-            2,
-            len(reg._ram_blks[ApriInfo(name="testy")])
-        )
+                with blk2:
 
-        blk4 = Block([1], ApriInfo(name ="testy"))
+                    reg.add_ram_blk(blk2)
+                    self.assertEqual(
+                        2,
+                        len(reg._ram_blks)
+                    )
+                    self.assertEqual(
+                        1,
+                        len(reg._ram_blks[ApriInfo(name ="tests")])
+                    )
+                    self.assertEqual(
+                        1,
+                        len(reg._ram_blks[ApriInfo(name ="testy")])
+                    )
 
-        with reg.open() as reg:
-            reg.add_ram_blk(blk4)
+                    with blk3:
 
-        self.assertEqual(
-            2,
-            len(reg._ram_blks)
-        )
+                        reg.add_ram_blk(blk3)
+                        self.assertEqual(
+                            2,
+                            len(reg._ram_blks)
+                        )
+                        self.assertEqual(
+                            1,
+                            len(reg._ram_blks[ApriInfo(name="tests")])
+                        )
+                        self.assertEqual(
+                            2,
+                            len(reg._ram_blks[ApriInfo(name="testy")])
+                        )
 
-        self.assertEqual(
-            1,
-            len(reg._ram_blks[ApriInfo(name="tests")])
-        )
+                        with blk4:
 
-        self.assertEqual(
-            3,
-            len(reg._ram_blks[ApriInfo(name="testy")])
-        )
+                            reg.add_ram_blk(blk4)
+                            self.assertEqual(
+                                2,
+                                len(reg._ram_blks)
+                            )
+                            self.assertEqual(
+                                1,
+                                len(reg._ram_blks[ApriInfo(name="tests")])
+                            )
+                            self.assertEqual(
+                                3,
+                                len(reg._ram_blks[ApriInfo(name="testy")])
+                            )
 
     def test_open_uncreated(self):
 
-        reg = Testy_Register(SAVES_DIR, "hey")
+        reg = Testy_Register(SAVES_DIR, "sh", "hey")
 
         with reg.open() as reg:
             self.assertTrue(reg._opened)
 
         self.assertTrue(reg._created)
 
         keyvals = {
@@ -464,57 +470,62 @@
 
         finally:
             if db is not None:
                 db.close()
 
     def test_remove_ram_block(self):
 
-        reg = NumpyRegister(SAVES_DIR, "msg")
+        reg = NumpyRegister(SAVES_DIR, "sh", "msg")
         blk1 = Block([], ApriInfo(name ="name1"))
 
         with reg.open() as reg:
 
-            reg.add_ram_blk(blk1)
-            reg.rmv_ram_blk(blk1)
-            self.assertEqual(
-                0,
-                len(reg._ram_blks)
-            )
+            with blk1:
 
-            reg.add_ram_blk(blk1)
-            reg.rmv_ram_blk(blk1)
-            self.assertEqual(
-                0,
-                len(reg._ram_blks)
-            )
+                reg.add_ram_blk(blk1)
+                reg.rmv_ram_blk(blk1)
+                self.assertEqual(
+                    0,
+                    len(reg._ram_blks)
+                )
 
-            reg.add_ram_blk(blk1)
-            blk2 = Block([], ApriInfo(name ="name2"))
-            reg.add_ram_blk(blk2)
-            reg.rmv_ram_blk(blk1)
-            self.assertEqual(
-                1,
-                len(reg._ram_blks)
-            )
-            self.assertIs(
-                blk2,
-                reg._ram_blks[blk2.apri()][0]
-            )
+                reg.add_ram_blk(blk1)
+                reg.rmv_ram_blk(blk1)
+                self.assertEqual(
+                    0,
+                    len(reg._ram_blks)
+                )
 
-            reg.rmv_ram_blk(blk2)
-            self.assertEqual(
-                0,
-                len(reg._ram_blks)
-            )
+                reg.add_ram_blk(blk1)
+                blk2 = Block([], ApriInfo(name ="name2"))
+
+                with blk2:
+
+                    reg.add_ram_blk(blk2)
+                    reg.rmv_ram_blk(blk1)
+                    self.assertEqual(
+                        1,
+                        len(reg._ram_blks)
+                    )
+                    self.assertIs(
+                        blk2,
+                        reg._ram_blks[blk2.apri()][0]
+                    )
+
+                    reg.rmv_ram_blk(blk2)
+                    self.assertEqual(
+                        0,
+                        len(reg._ram_blks)
+                    )
 
     def test___hash___created(self):
 
         # create two `Register`s
-        reg1 = Testy_Register(SAVES_DIR, "msg")
-        reg2 = Testy_Register(SAVES_DIR, "msg")
+        reg1 = Testy_Register(SAVES_DIR, "sh", "msg")
+        reg2 = Testy_Register(SAVES_DIR, "sh", "msg")
         with reg1.open() as reg1:pass
         with reg2.open() as reg2:pass
 
         self.assertEqual(
             hash(reg1),
             hash(reg1)
         )
@@ -526,42 +537,42 @@
 
         self.assertNotEqual(
             hash(reg1),
             hash(reg2)
         )
 
         # manually change the `_localDir` to force equality
-        reg2 = Testy_Register(SAVES_DIR, "msg")
+        reg2 = Testy_Register(SAVES_DIR, "sh", "msg")
         reg2._set_local_dir(reg1._local_dir)
         self.assertEqual(
             hash(reg2),
             hash(reg1)
         )
 
         # a different `Register` derived type should change the hash value
-        reg2 = Testy_Register2(SAVES_DIR, "msg")
+        reg2 = Testy_Register2(SAVES_DIR, "sh", "msg")
         reg2._set_local_dir(reg1._local_dir)
         self.assertNotEqual(
             hash(reg2),
             hash(reg1)
         )
 
         # relative paths should work as expected
-        reg2 = Testy_Register(SAVES_DIR, "msg")
+        reg2 = Testy_Register(SAVES_DIR, "sh", "msg")
         reg2._set_local_dir(".." / SAVES_DIR / reg1._local_dir)
         self.assertEqual(
             hash(reg2),
             hash(reg1)
         )
 
     def test___eq___created(self):
 
         # open two `Register`s
-        reg1 = Testy_Register(SAVES_DIR, "msg")
-        reg2 = Testy_Register(SAVES_DIR, "msg")
+        reg1 = Testy_Register(SAVES_DIR, "sh", "msg")
+        reg2 = Testy_Register(SAVES_DIR, "sh", "msg")
         with reg1.open() as reg1:pass
         with reg2.open() as reg2:pass
 
         self.assertEqual(
             reg1,
             reg1
         )
@@ -573,70 +584,70 @@
 
         self.assertNotEqual(
             reg1,
             reg2
         )
 
         # manually change the `_localDir` to force equality
-        reg2 = Testy_Register(SAVES_DIR, "msg")
+        reg2 = Testy_Register(SAVES_DIR, "sh", "msg")
         reg2._set_local_dir(reg1._local_dir)
         self.assertEqual(
             reg2,
             reg1
         )
 
         # tests a different `Register` derived type
-        reg2 = Testy_Register2(SAVES_DIR, "msg")
+        reg2 = Testy_Register2(SAVES_DIR, "sh", "msg")
         reg2._set_local_dir(reg1._local_dir)
         self.assertNotEqual(
             reg2,
             reg1
         )
 
         # tests that relative paths work as expected
-        reg2 = Testy_Register(SAVES_DIR, "msg")
+        reg2 = Testy_Register(SAVES_DIR, "sh", "msg")
         reg2._set_local_dir(".." / SAVES_DIR / reg1._local_dir)
         self.assertEqual(
             reg2,
             reg1
         )
 
     def test__check_open_raise_created(self):
 
-        reg = Testy_Register(SAVES_DIR, "hi")
+        reg = Testy_Register(SAVES_DIR, "sh", "hi")
         with self.assertRaisesRegex(RegisterError, "xyz"):
             reg._check_open_raise("xyz")
 
-        reg = Testy_Register(SAVES_DIR, "hi")
+        reg = Testy_Register(SAVES_DIR, "sh", "hi")
         with reg.open() as reg:
             try:
                 reg._check_open_raise("xyz")
             except RegisterError:
                 self.fail("the register is open")
 
-        reg = Testy_Register(SAVES_DIR, "hi")
+        reg = Testy_Register(SAVES_DIR, "sh", "hi")
         with reg.open() as reg:pass
         with self.assertRaisesRegex(RegisterError, "xyz"):
             reg._check_open_raise("xyz")
 
     def test__get_id_by_apri_new(self):
 
-        reg = Testy_Register(SAVES_DIR, "hi")
+        reg = Testy_Register(SAVES_DIR, "sh", "hi")
 
         with self.assertRaises(ValueError):
             reg._get_id_by_apri(None, None, True)
 
         with self.assertRaises(ValueError):
             reg._get_id_by_apri(None, None, False)
 
         apri1 = ApriInfo(name ="hi")
         apri2 = ApriInfo(name ="hello")
         apri3 = ApriInfo(name ="sup")
         apri4 = ApriInfo(name ="hey")
-        reg = Testy_Register(SAVES_DIR, "hi")
+        reg = Testy_Register(SAVES_DIR, "sh", "hi")
 
         with reg.open() as reg:
 
 
             _id1 = reg._get_id_by_apri(apri1, None, True)
 
             self.assertEqual(
@@ -678,131 +689,142 @@
             )
 
             with self.assertRaises(DataNotFoundError):
                 reg._get_id_by_apri(apri4, None, False)
 
     def test__get_instance(self):
 
-        reg1 = Testy_Register(SAVES_DIR, "msg")
+        reg1 = Testy_Register(SAVES_DIR, "sh", "msg")
 
 
         with reg1.open() as reg1: pass
-        reg2 = Testy_Register(SAVES_DIR, "msg")
+        reg2 = Testy_Register(SAVES_DIR, "sh", "msg")
         reg2._set_local_dir(reg1._local_dir)
 
         self.assertIs(
             reg1,
             Register._get_instance(reg2._local_dir)
         )
 
         self.assertIs(
             reg1,
             Register._get_instance(reg1._local_dir)
         )
 
     def test_set_message(self):
 
-        reg = Testy_Register(SAVES_DIR, "testy")
+        reg = Testy_Register(SAVES_DIR, "sh", "testy")
 
         try:
             reg.set_msg("yes")
 
         except RegisterError as e:
             if "has not been opened" in str(e):
                 self.fail("the register doesn't need to be open for set_msg")
             else:
                 raise e
 
         self.assertEqual(
-            "yes",
+            "sh: \"yes\"",
             str(reg)
         )
-
         with reg.open() as reg:pass
-
         reg.set_msg("no")
 
         self.assertEqual(
-            "no",
+            f"sh ({reg._local_dir}): \"no\"",
             str(reg)
         )
 
-        with reg._msg_filepath.open("r") as fh:
-            self.assertEqual(
-                "no",
-                fh.read()
-            )
-
     def test_add_disk_block(self):
 
-        reg = Testy_Register(SAVES_DIR, "sup")
+        reg = Testy_Register(SAVES_DIR, "sh", "sup")
         blk = Block([], ApriInfo(name ="hi"))
+
         with self.assertRaisesRegex(RegisterError, "open.*add_disk_blk"):
-            reg.add_disk_blk(blk)
 
-        reg = Testy_Register(SAVES_DIR, "hello")
-        blk = Block([], ApriInfo(name ="hi"), 10 ** 50)
+            with blk:
+                reg.add_disk_blk(blk)
+
+        reg = Testy_Register(SAVES_DIR, "sh", "hello")
         with reg.open() as reg:
+
             with self.assertRaisesRegex(IndexError, "correct head"):
-                reg.add_disk_blk(blk)
 
-        reg = Testy_Register(SAVES_DIR, "hello")
+                with Block([], ApriInfo(name ="hi"), 10 ** 50) as blk:
+                    reg.add_disk_blk(blk)
+
+        reg = Testy_Register(SAVES_DIR, "sh", "hello")
         too_large = reg._startn_tail_mod
-        blk = Block([], ApriInfo(name ="hi"), too_large)
+
         with reg.open() as reg:
+
             with self.assertRaisesRegex(IndexError, "correct head"):
-                reg.add_disk_blk(blk)
 
-        reg = Testy_Register(SAVES_DIR, "hello")
+                with Block([], ApriInfo(name ="hi"), too_large) as blk:
+                    reg.add_disk_blk(blk)
+
+        reg = Testy_Register(SAVES_DIR, "sh", "hello")
         too_large = reg._startn_tail_mod
-        blk = Block([], ApriInfo(name ="hi"), too_large - 1)
+
         with reg.open() as reg:
+
             try:
-                reg.add_disk_blk(blk)
+
+                with Block([], ApriInfo(name ="hi"), too_large - 1) as blk:
+                    reg.add_disk_blk(blk)
+
             except IndexError:
                 self.fail("index is not too large")
 
-        reg = Testy_Register(SAVES_DIR, "hi")
+        reg = Testy_Register(SAVES_DIR, "sh", "hi")
         blk1 = Block([], ApriInfo(name ="hello"))
         blk2 = Block([1], ApriInfo(name ="hello"))
         blk3 = Block([], ApriInfo(name ="hi"))
         blk4 = Block([], ApriInfo(name ="hello"))
         blk5 = Block([], ApriInfo(sir ="hey", maam ="hi"))
         blk6 = Block([], ApriInfo(maam="hi", sir ="hey"))
+
         with reg.open() as reg:
 
-            reg.add_disk_blk(blk1)
+            with blk1:
+                reg.add_disk_blk(blk1)
+
             self.assertEqual(
                 1,
                 lmdb_count_keys(reg._db, _BLK_KEY_PREFIX)
             )
             self.assertEqual(
                 1,
                 lmdb_count_keys(reg._db, _APRI_ID_KEY_PREFIX)
             )
             self.assertEqual(
                 1,
                 lmdb_count_keys(reg._db, _ID_APRI_KEY_PREFIX)
             )
 
-            reg.add_disk_blk(blk2)
+            with blk2:
+                reg.add_disk_blk(blk2)
+
             self.assertEqual(
                 2,
                 lmdb_count_keys(reg._db, _BLK_KEY_PREFIX)
             )
             self.assertEqual(
                 1,
                 lmdb_count_keys(reg._db, _APRI_ID_KEY_PREFIX)
             )
             self.assertEqual(
                 1,
                 lmdb_count_keys(reg._db, _ID_APRI_KEY_PREFIX)
             )
 
-            reg.add_disk_blk(blk3)
+            with blk3:
+                reg.add_disk_blk(blk3)
+
             self.assertEqual(
                 3,
                 lmdb_count_keys(reg._db, _BLK_KEY_PREFIX)
             )
             self.assertEqual(
                 2,
                 lmdb_count_keys(reg._db, _APRI_ID_KEY_PREFIX)
@@ -810,43 +832,52 @@
             self.assertEqual(
                 2,
                 lmdb_count_keys(reg._db, _ID_APRI_KEY_PREFIX)
             )
 
             try:
                 with self.assertRaisesRegex(RegisterError, "[dD]uplicate"):
-                    reg.add_disk_blk(blk4)
+
+                    with blk4:
+                        reg.add_disk_blk(blk4)
 
             except AssertionError:
                 raise
 
-            reg.add_disk_blk(blk5)
+            with blk5:
+                reg.add_disk_blk(blk5)
 
             with self.assertRaisesRegex(RegisterError, "[dD]uplicate"):
-                reg.add_disk_blk(blk6)
+
+                with blk6:
+                    reg.add_disk_blk(blk6)
 
         with self.assertRaisesRegex(RegisterError, "read-only"):
+
             with reg.open(readonly= True) as reg:
-                reg.add_disk_blk(blk)
 
-        reg = NumpyRegister(SAVES_DIR, "no")
+                with blk:
+                    reg.add_disk_blk(blk)
+
+        reg = NumpyRegister(SAVES_DIR, "sh", "no")
 
         with reg.open() as reg:
 
-            reg.add_disk_blk(Block(np.arange(30), ApriInfo(maybe ="maybe")))
+            with Block(np.arange(30), ApriInfo(maybe ="maybe")) as blk:
+                reg.add_disk_blk(blk)
 
             for debug in [1,2,3,4,5,6,7,8,9,10]:
 
                 apri = ApriInfo(none ="all")
-                blk = Block(np.arange(14), apri, 0)
-
                 cornifer.registers._debug = debug
 
                 with self.assertRaises(KeyboardInterrupt):
-                    reg.add_disk_blk(blk)
+
+                    with Block(np.arange(14), apri, 0) as blk:
+                        reg.add_disk_blk(blk)
 
                 cornifer.registers._debug = _NO_DEBUG
 
                 try:
                     self.assertEqual(
                         1,
                         lmdb_count_keys(reg._db, _BLK_KEY_PREFIX)
@@ -873,25 +904,30 @@
                     self.assertEqual(
                         1,
                         sum(1 for d in reg._local_dir.iterdir() if d.is_file())
                     )
                 except AssertionError:
                     raise
 
-                self.assertTrue(np.all(
-                    np.arange(30) ==
-                    reg.blk(ApriInfo(maybe="maybe"), 0, 30).segment()
-                ))
+                blk = reg.blk(ApriInfo(maybe="maybe"), 0, 30)
+
+                with blk as blk:
+                    self.assertTrue(np.all(
+                        np.arange(30) ==
+                        blk.segment()
+                    ))
 
                 with self.assertRaises(DataNotFoundError):
-                    reg.blk(ApriInfo(none="all"), 0, 14)
+
+                    with reg.blk(ApriInfo(none="all"), 0, 14) as blk:
+                        pass
 
     def test__get_apri_json_by_id(self):
 
-        reg = Testy_Register(SAVES_DIR, "hello")
+        reg = Testy_Register(SAVES_DIR, "sh", "hello")
         with reg.open() as reg:
             apri1 = ApriInfo(name ="hi")
             _id1 = reg._get_id_by_apri(apri1, None, True)
 
             self.assertIsInstance(
                 _id1,
                 bytes
@@ -906,35 +942,38 @@
             self.assertEqual(
                 apri2,
                 ApriInfo.from_json(reg._get_apri_json_by_id(_id2).decode("ASCII"))
             )
 
     def test_apri_infos_no_recursive(self):
 
-        reg = Testy_Register(SAVES_DIR, "msg")
+        reg = Testy_Register(SAVES_DIR, "sh", "msg")
+
         with self.assertRaisesRegex(RegisterError, "apris"):
             reg.apris()
 
-        reg = Testy_Register(SAVES_DIR, "msg")
+        reg = Testy_Register(SAVES_DIR, "sh", "msg")
+
         with reg.open() as reg:
 
             apri1 = ApriInfo(name ="hello")
             reg._get_id_by_apri(apri1, None, True)
             self.assertEqual(
                 1,
                 len(list(reg.apris()))
             )
             self.assertEqual(
                 apri1,
                 list(reg.apris())[0]
             )
 
             apri2 = ApriInfo(name ="hey")
-            blk = Block([], apri2)
-            reg.add_ram_blk(blk)
+
+            with Block([], apri2) as blk:
+                reg.add_ram_blk(blk)
 
             self.assertEqual(
                 2,
                 len(list(reg.apris()))
             )
             self.assertIn(
                 apri1,
@@ -943,25 +982,25 @@
             self.assertIn(
                 apri2,
                 list(reg.apris())
             )
 
     def test__open_created(self):
 
-        reg = Testy_Register(SAVES_DIR, "testy")
+        reg = Testy_Register(SAVES_DIR, "sh", "testy")
         with reg.open() as reg: pass
         with reg.open() as reg:
             self.assertTrue(reg._opened)
             with self.assertRaises(RegisterAlreadyOpenError):
                 with reg.open() as reg: pass
 
-        reg1 = Testy_Register(SAVES_DIR, "testy")
+        reg1 = Testy_Register(SAVES_DIR, "sh", "testy")
         with reg1.open() as reg1: pass
 
-        reg2 = Testy_Register(SAVES_DIR, "testy")
+        reg2 = Testy_Register(SAVES_DIR, "sh", "testy")
 
         reg2._set_local_dir(reg1._local_dir)
 
         self.assertEqual(
             reg1,
             reg2
         )
@@ -974,15 +1013,15 @@
             self.assertIs(
                 reg1,
                 reg2
             )
 
     def test__get_id_by_apri(self):
 
-        reg = Testy_Register(SAVES_DIR, "hello")
+        reg = Testy_Register(SAVES_DIR, "sh", "hello")
         apri1 = ApriInfo(name ="hello")
         with reg.open() as reg:
             _id1 = reg._get_id_by_apri(apri1, None, True)
             _id2 = reg._get_id_by_apri(apri1, None, True)
             self.assertIsInstance(
                 _id2,
                 bytes
@@ -996,63 +1035,86 @@
             self.assertEqual(
                 _id1,
                 _id3
             )
 
     def test__convert_disk_block_key_no_head(self):
 
-        reg = Testy_Register(SAVES_DIR, "sup")
+        reg = Testy_Register(SAVES_DIR, "sh", "sup")
+
         with reg.open() as reg:
 
             apri1 = ApriInfo(name ="hey")
             blk1 = Block([], apri1)
-            reg.add_disk_blk(blk1)
+
+            with blk1:
+                reg.add_disk_blk(blk1)
+
             with lmdb_prefix_iter(reg._db, _BLK_KEY_PREFIX) as it:
+
                 for curr_key,_ in it: pass
+
             self.assertEqual(
                 (apri1, 0, 0),
                 reg._convert_disk_block_key(_BLK_KEY_PREFIX_LEN, curr_key)
             )
             self.assertEqual(
                 (apri1, 0, 0),
                 reg._convert_disk_block_key(_BLK_KEY_PREFIX_LEN, curr_key, apri1)
             )
             old_keys = {curr_key}
 
             blk2 = Block(list(range(10)), apri1)
-            reg.add_disk_blk(blk2)
+
+            with blk2:
+                reg.add_disk_blk(blk2)
+
             with lmdb_prefix_iter(reg._db, _BLK_KEY_PREFIX) as it:
+
                 for key,_val in it:
+
                     if key not in old_keys:
                         curr_key = key
+
             self.assertEqual(
                 (apri1, 0, 10),
                 reg._convert_disk_block_key(_BLK_KEY_PREFIX_LEN, curr_key)
             )
             old_keys.add(curr_key)
 
             apri2 = ApriInfo(name ="hello")
             blk3 = Block(list(range(100)), apri2, 10)
-            reg.add_disk_blk(blk3)
+
+            with blk3:
+                reg.add_disk_blk(blk3)
+
             with lmdb_prefix_iter(reg._db, _BLK_KEY_PREFIX) as it:
+
                 for key,_val in it:
+
                     if key not in old_keys:
                         curr_key = key
+
             self.assertEqual(
                 (apri2, 10, 100),
                 reg._convert_disk_block_key(_BLK_KEY_PREFIX_LEN, curr_key)
             )
             old_keys.add(curr_key)
-
             blk4 = Block(list(range(100)), apri2)
-            reg.add_disk_blk(blk4)
+
+            with blk4:
+                reg.add_disk_blk(blk4)
+
             with lmdb_prefix_iter(reg._db, _BLK_KEY_PREFIX) as it:
+
                 for key,_val in it:
+
                     if key not in old_keys:
                         curr_key = key
+
             self.assertEqual(
                 (apri2, 0, 100),
                 reg._convert_disk_block_key(_BLK_KEY_PREFIX_LEN, curr_key)
             )
 
     def check_reg_set_start_n_info(self, reg, mod, head, tail_length):
         self.assertEqual(
@@ -1093,105 +1155,131 @@
         self.assertEqual(
             length,
             _length
         )
 
     def test_set_start_n_info(self):
 
-        reg = Testy_Register(SAVES_DIR, "hello")
+        reg = Testy_Register(SAVES_DIR, "sh", "hello")
+
         with self.assertRaisesRegex(RegisterError, "set_startn_info"):
             reg.set_startn_info(10, 3)
 
-        reg = Testy_Register(SAVES_DIR, "hello")
+        reg = Testy_Register(SAVES_DIR, "sh", "hello")
+
         with reg.open() as reg:
+
             with self.assertRaisesRegex(TypeError, "int"):
                 reg.set_startn_info(10, 3.5)
 
-        reg = Testy_Register(SAVES_DIR, "hello")
+        reg = Testy_Register(SAVES_DIR, "sh", "hello")
+
         with reg.open() as reg:
+
             with self.assertRaisesRegex(TypeError, "int"):
                 reg.set_startn_info(10.5, 3)
 
-        reg = Testy_Register(SAVES_DIR, "hello")
+        reg = Testy_Register(SAVES_DIR, "sh", "hello")
+
         with reg.open() as reg:
+
             with self.assertRaisesRegex(ValueError, "non-negative"):
                 reg.set_startn_info(-1, 3)
 
-        reg = Testy_Register(SAVES_DIR, "hello")
+        reg = Testy_Register(SAVES_DIR, "sh", "hello")
+
         with reg.open() as reg:
+
             try:
                 reg.set_startn_info(0, 3)
+
             except ValueError:
                 self.fail("head can be 0")
 
-        reg = Testy_Register(SAVES_DIR, "hello")
+        reg = Testy_Register(SAVES_DIR, "sh", "hello")
+
         with reg.open() as reg:
+
             with self.assertRaisesRegex(ValueError, "positive"):
                 reg.set_startn_info(0, -1)
 
-        reg = Testy_Register(SAVES_DIR, "hello")
+        reg = Testy_Register(SAVES_DIR, "sh", "hello")
+
         with reg.open() as reg:
+
             with self.assertRaisesRegex(ValueError, "positive"):
                 reg.set_startn_info(0, 0)
 
 
         for head, tail_length in product([0, 1, 10, 100, 1100, 450], [1,2,3,4,5]):
-
             # check set works
-            reg = Testy_Register(SAVES_DIR, "hello")
+            reg = Testy_Register(SAVES_DIR, "sh",  "hello")
+
             with reg.open() as reg:
 
                 try:
                     reg.set_startn_info(head, tail_length)
 
                 except ValueError:
                     self.fail(f"head = {head}, tail_length = {tail_length} are okay")
 
                 with reg._db.begin() as txn:
+
                     self.assertEqual(
                         str(head).encode("ASCII"),
                         txn.get(_START_N_HEAD_KEY)
                     )
-
                     self.assertEqual(
                         str(tail_length).encode("ASCII"),
                         txn.get(_START_N_TAIL_LENGTH_KEY)
                     )
-
             # check read-only mode doesn't work
             with reg.open(readonly= True) as reg:
+
                 with self.assertRaisesRegex(RegisterError, "read-only"):
                     reg.set_startn_info(head, tail_length)
 
             # tests make sure ValueError is thrown for small smart_n
             # 0 and head * 10 ** tail_len - 1 are the two possible extremes of the small start_n
             if head > 0:
+
                 for start_n in [0, head * 10 ** tail_length - 1]:
-                    reg = Testy_Register(SAVES_DIR, "hello")
+
+                    reg = Testy_Register(SAVES_DIR, "sh",  "hello")
+
                     with reg.open() as reg:
+
                             blk = Block([], ApriInfo(name ="hi"), start_n)
-                            reg.add_disk_blk(blk)
+
+                            with blk:
+                                reg.add_disk_blk(blk)
+
                             with self.assertRaisesRegex(ValueError, "correct head"):
                                 reg.set_startn_info(head, tail_length)
-
                             # make sure it exits safely
                             self.check_reg_set_start_n_info(
                                 reg,
                                 10 ** _START_N_TAIL_LENGTH_DEFAULT, 0, _START_N_TAIL_LENGTH_DEFAULT
                             )
 
             # tests to make sure a few permissible start_n work
             smallest = head * 10 ** tail_length
             largest = smallest + 10 ** tail_length  - 1
+
             for start_n in [smallest, smallest + 1, smallest + 2, largest -2, largest -1, largest]:
-                reg = Testy_Register(SAVES_DIR, "hello")
+
+                reg = Testy_Register(SAVES_DIR, "sh",  "hello")
                 apri = ApriInfo(name="hi")
+
                 with reg.open() as reg:
+
                     blk = Block([], apri,start_n)
-                    reg.add_disk_blk(blk)
+
+                    with blk:
+                        reg.add_disk_blk(blk)
 
                     for debug in [0, 1, 2]:
 
                         if debug == _NO_DEBUG:
                             reg.set_startn_info(head, tail_length)
 
                         else:
@@ -1211,25 +1299,29 @@
                         with lmdb_prefix_iter(reg._db, _BLK_KEY_PREFIX) as it:
                             for curr_key,_ in it:pass
 
                         self.check_key_set_start_n_info(
                             reg, curr_key,
                             apri, start_n, 0
                         )
-
             # tests to make sure `largest + 1` etc do not work
             for start_n in [largest + 1, largest + 10, largest + 100, largest + 1000]:
-                reg = Testy_Register(SAVES_DIR, "hello")
+
+                reg = Testy_Register(SAVES_DIR, "sh",  "hello")
                 apri = ApriInfo(name="hi")
+
                 with reg.open() as reg:
+
                     blk = Block([], apri, start_n)
-                    reg.add_disk_blk(blk)
+
+                    with blk:
+                        reg.add_disk_blk(blk)
+
                     with self.assertRaisesRegex(ValueError, "correct head"):
                         reg.set_startn_info(head, tail_length)
-
                     # make sure it exits safely
                     self.check_reg_set_start_n_info(
                         reg,
                         10 ** _START_N_TAIL_LENGTH_DEFAULT, 0, _START_N_TAIL_LENGTH_DEFAULT
                     )
 
     def check__iter_disk_block_pairs(self, t, apri, start_n, length):
@@ -1260,130 +1352,155 @@
         self.assertEqual(
             length,
             t[2]
         )
 
     def test__iter_disk_block_pairs(self):
 
-        reg = Testy_Register(SAVES_DIR, "HI")
+        reg = Testy_Register(SAVES_DIR, "sh",  "HI")
+
         with reg.open() as reg:
-            apri1 = ApriInfo(name ="abc")
-            apri2 = ApriInfo(name ="xyz")
+
+            apri1 = ApriInfo(name = "abc")
             blk1 = Block(list(range(50)), apri1, 0)
             blk2 = Block(list(range(50)), apri1, 50)
-            blk3 = Block(list(range(500)), apri2, 1000)
 
-            reg.add_disk_blk(blk1)
+            with blk1:
+                reg.add_disk_blk(blk1)
+
             total = 0
+
             for i, t in chain(
                 enumerate(reg._iter_disk_blk_pairs(_BLK_KEY_PREFIX, apri1, None)),
                 enumerate(reg._iter_disk_blk_pairs(_BLK_KEY_PREFIX, None, apri1.to_json().encode("ASCII")))
             ):
+
                 total += 1
+
                 if i == 0:
+
                     t = reg._convert_disk_block_key(_BLK_KEY_PREFIX_LEN, t[0], apri1)
                     self.check__iter_disk_block_pairs(t, apri1, 0, 50)
+
                 else:
                     self.fail()
+
             if total != 2:
                 self.fail(str(total))
 
-            reg.add_disk_blk(blk2)
+            with blk2:
+                reg.add_disk_blk(blk2)
+
             total = 0
+
             for i, t in chain(
                 enumerate(reg._iter_disk_blk_pairs(_BLK_KEY_PREFIX, apri1, None)),
                 enumerate(reg._iter_disk_blk_pairs(_BLK_KEY_PREFIX, None, apri1.to_json().encode("ASCII")))
             ):
+
                 total += 1
+
                 if i == 0:
+
                     t = reg._convert_disk_block_key(_BLK_KEY_PREFIX_LEN, t[0], apri1)
                     self.check__iter_disk_block_pairs(t, apri1, 0, 50)
+
                 elif i == 1:
+
                     t = reg._convert_disk_block_key(_BLK_KEY_PREFIX_LEN, t[0], apri1)
                     self.check__iter_disk_block_pairs(t, apri1, 50, 50)
+
                 else:
                     self.fail()
+
             if total != 4:
                 self.fail(str(total))
 
             total = 0
+
             for i, t in chain(
                 enumerate(reg._iter_disk_blk_pairs(_BLK_KEY_PREFIX, apri1, None)),
                 enumerate(reg._iter_disk_blk_pairs(_BLK_KEY_PREFIX, None, apri1.to_json().encode("ASCII")))
             ):
+
                 total += 1
+
                 if i == 0:
+
                     t = reg._convert_disk_block_key(_BLK_KEY_PREFIX_LEN, t[0], apri1)
                     self.check__iter_disk_block_pairs(t, apri1, 0, 50)
+
                 elif i == 1:
+
                     t = reg._convert_disk_block_key(_BLK_KEY_PREFIX_LEN, t[0], apri1)
                     self.check__iter_disk_block_pairs(t, apri1, 50, 50)
+
                 else:
                     self.fail()
 
             if total != 4:
                 self.fail()
 
     def test_open(self):
 
-        reg1 = Testy_Register(SAVES_DIR, "msg")
+        reg1 = Testy_Register(SAVES_DIR, "sh",  "msg")
         with reg1.open() as reg2:pass
         self.assertIs(
             reg1,
             reg2
         )
 
         try:
             with reg1.open() as reg1:pass
 
         except RegisterError:
             self.fail()
 
-        reg2 = Testy_Register(SAVES_DIR, "hello")
+        reg2 = Testy_Register(SAVES_DIR, "sh",  "hello")
         with reg2.open() as reg2:pass
-        reg3 = Testy_Register(SAVES_DIR, "hello")
+        reg3 = Testy_Register(SAVES_DIR, "sh",  "hello")
         reg3._set_local_dir(reg2._local_dir)
         with reg3.open() as reg4:pass
         self.assertIs(
             reg4,
             reg2
         )
 
-        reg4 = Testy_Register(SAVES_DIR, "sup")
+        reg4 = Testy_Register(SAVES_DIR, "sh",  "sup")
         with self.assertRaisesRegex(ValueError, "read-only"):
             with reg4.open(readonly= True) as reg:pass
 
     def test__recursive_open(self):
 
         # must be created
-        reg1 = Testy_Register(SAVES_DIR, "hello")
+        reg1 = Testy_Register(SAVES_DIR, "sh",  "hello")
 
         with self.assertRaises(RegisterError):
             with reg1._recursive_open(False):pass
 
         # must be created
-        reg2 = Testy_Register(SAVES_DIR, "hello")
+        reg2 = Testy_Register(SAVES_DIR, "sh",  "hello")
         with reg2.open() as reg2:pass
         with reg2._recursive_open(False) as reg3:pass
 
         self.assertIs(
             reg2,
             reg3
         )
 
-        reg3 = Testy_Register(SAVES_DIR, "hello")
+        reg3 = Testy_Register(SAVES_DIR, "sh",  "hello")
         reg3._set_local_dir(reg2._local_dir)
         with reg3._recursive_open(False) as reg4:pass
 
         self.assertIs(
             reg2,
             reg4
         )
 
-        reg5 = Testy_Register(SAVES_DIR, "hi")
+        reg5 = Testy_Register(SAVES_DIR, "sh",  "hi")
 
         with reg5.open() as reg5:
 
             try:
                 with reg5._recursive_open(False):pass
 
             except RegisterError:
@@ -1394,15 +1511,15 @@
                     reg5._opened
                 )
 
         self.assertFalse(
             reg5._opened
         )
 
-        reg6 = Testy_Register(SAVES_DIR, "supp")
+        reg6 = Testy_Register(SAVES_DIR, "sh",  "supp")
 
         with reg6.open() as reg6: pass
 
         with reg6.open(readonly= True) as reg6:
 
             with self.assertRaisesRegex(ValueError, "read-only"):
                 with reg6._recursive_open(False):pass
@@ -1435,95 +1552,101 @@
             key = reg._get_disk_blk_key(_BLK_KEY_PREFIX, apri, None, start_n, length, False)
             with reg._db.begin() as txn:
                 filename = Path(txn.get(key).decode("ASCII"))
             self.assertTrue((reg._local_dir / filename).exists())
 
     def test_remove_disk_block(self):
 
-        reg1 = Testy_Register(SAVES_DIR, "hi")
+        reg1 = Testy_Register(SAVES_DIR, "sh",  "hi")
 
         with self.assertRaisesRegex(RegisterError, "open.*rmv_disk_blk"):
             reg1.rmv_disk_blk(ApriInfo(name ="fooopy doooopy"), 0, 0)
 
         with reg1.open() as reg1:
 
             apri1 = ApriInfo(name ="fooopy doooopy")
-            blk1 = Block(list(range(50)), apri1)
-            reg1.add_disk_blk(blk1)
-            self._remove_disk_block_helper(reg1, [(apri1, 0, 50)])
 
+            with Block(list(range(50)), apri1) as blk1:
+                reg1.add_disk_blk(blk1)
+
+            self._remove_disk_block_helper(reg1, [(apri1, 0, 50)])
             reg1.rmv_disk_blk(apri1, 0, 50)
             self._remove_disk_block_helper(reg1, [])
 
-            reg1.add_disk_blk(blk1)
+            with blk1:
+                reg1.add_disk_blk(blk1)
+
             apri2 = ApriInfo(name ="fooopy doooopy2")
-            blk2 = Block(list(range(100)), apri2, 1000)
-            reg1.add_disk_blk(blk2)
+
+            with Block(list(range(100)), apri2, 1000) as blk2:
+                reg1.add_disk_blk(blk2)
+
             self._remove_disk_block_helper(reg1, [(apri1, 0, 50), (apri2, 1000, 100)])
 
             reg1.rmv_disk_blk(apri2, 1000, 100)
             self._remove_disk_block_helper(reg1, [(apri1, 0, 50)])
 
             reg1.rmv_disk_blk(apri1, 0, 50)
             self._remove_disk_block_helper(reg1, [])
 
         with self.assertRaisesRegex(RegisterError, "read-write"):
             with reg1.open(readonly= True) as reg1:
                 reg1.rmv_disk_blk(apri1, 0, 0)
 
         # add the same block to two registers
-        reg1 = Testy_Register(SAVES_DIR, "hello")
-        reg2 = Testy_Register(SAVES_DIR, "sup")
+        reg1 = Testy_Register(SAVES_DIR, "sh",  "hello")
+        reg2 = Testy_Register(SAVES_DIR, "sh",  "sup")
         apri = ApriInfo(name ="hi")
-        blk = Block([], apri)
 
-        with reg1.open() as reg1:
-            reg1.add_disk_blk(blk)
+        with Block([], apri) as blk:
 
-        with reg2.open() as reg2:
-            reg2.add_disk_blk(blk)
+            with reg1.open() as reg1:
+                reg1.add_disk_blk(blk)
+
+            with reg2.open() as reg2:
+                reg2.add_disk_blk(blk)
 
         with reg1.open() as reg1:
+
             reg1.rmv_disk_blk(apri, 0, 0)
             self._remove_disk_block_helper(reg1, [])
 
         with reg2.open() as reg2:
             self._remove_disk_block_helper(reg2, [(apri, 0, 0)])
 
-        reg = NumpyRegister(SAVES_DIR, "hello")
+        reg = NumpyRegister(SAVES_DIR, "sh", "hello")
 
         with reg.open() as reg:
 
             apri = ApriInfo(no ="yes")
-            blk = Block(np.arange(14), apri)
 
-            reg.add_disk_blk(blk)
+            with Block(np.arange(14), apri) as blk:
+                reg.add_disk_blk(blk)
 
             apri = ApriInfo(maybe ="maybe")
-            blk = Block(np.arange(20), apri)
 
-            reg.add_disk_blk(blk)
+            with Block(np.arange(20), apri) as blk:
+                reg.add_disk_blk(blk)
 
             for compress in range(2):
 
                 for debug in [1,2,3,4,5,6,7,8,9,   12,13,14,15,16,17]:
 
                     if debug >= 9 and compress == 1 or debug == 9 and compress == 0:
                         continue
 
                     if compress == 1:
-                        reg.compress(blk.apri(), blk.startn(), len(blk))
+
+                        with blk:
+                            reg.compress(blk.apri(), blk.startn(), len(blk))
 
                     cornifer.registers._debug = debug
 
-                    try:
-                        with self.assertRaises(KeyboardInterrupt):
-                            reg.rmv_disk_blk(ApriInfo(maybe ="maybe"), 0, 20)
-                    except (RegisterRecoveryError, AssertionError):
-                        raise
+                    with self.assertRaises(KeyboardInterrupt):
+                        reg.rmv_disk_blk(ApriInfo(maybe ="maybe"), 0, 20)
 
                     cornifer.registers._debug = _NO_DEBUG
 
                     self.assertEqual(
                         2,
                         lmdb_count_keys(reg._db, _BLK_KEY_PREFIX)
                     )
@@ -1548,29 +1671,33 @@
                             2 + compress,
                             sum(1 for d in reg._local_dir.iterdir() if d.is_file())
                         )
                     except AssertionError:
                         raise
 
                     if compress == 1:
-                        reg.decompress(blk.apri(), blk.startn(), len(blk))
 
-                    self.assertTrue(np.all(
-                        np.arange(14) ==
-                        reg.blk(ApriInfo(no="yes"), 0, 14).segment()
-                    ))
+                        with blk:
+                            reg.decompress(blk.apri(), blk.startn(), len(blk))
 
-                    self.assertTrue(np.all(
-                        np.arange(20) ==
-                        reg.blk(ApriInfo(maybe="maybe"), 0, 20).segment()
-                    ))
+                    with reg.blk(ApriInfo(no="yes"), 0, 14) as blk:
+                        self.assertTrue(np.all(
+                            np.arange(14) ==
+                            blk.segment()
+                        ))
+
+                    with reg.blk(ApriInfo(maybe="maybe"), 0, 20) as blk:
+                        self.assertTrue(np.all(
+                            np.arange(20) ==
+                            blk.segment()
+                        ))
 
     def test_set_apos_info(self):
 
-        reg = Testy_Register(SAVES_DIR, "hello")
+        reg = Testy_Register(SAVES_DIR, "sh",  "hello")
 
         with self.assertRaisesRegex(RegisterError, "open.*set_apos"):
             reg.set_apos(ApriInfo(no ="no"), AposInfo(yes ="yes"))
 
         with reg.open() as reg:
 
             try:
@@ -1624,15 +1751,15 @@
 
         with reg.open(readonly= True) as reg:
             with self.assertRaisesRegex(RegisterError, "read-write"):
                 reg.set_apos(ApriInfo(no="no"), AposInfo(yes="yes"))
 
     def test_apos_info(self):
 
-        reg = Testy_Register(SAVES_DIR, "hello")
+        reg = Testy_Register(SAVES_DIR, "sh",  "hello")
 
         with self.assertRaisesRegex(RegisterError, "open.*apos"):
             reg.apos(ApriInfo(no ="no"))
 
         with reg.open() as reg:
 
             apri = ApriInfo(no ="yes")
@@ -1675,15 +1802,15 @@
                     raise e
 
             except Exception as e:
                 raise e
 
     def test_remove_apos_info(self):
 
-        reg = Testy_Register(SAVES_DIR, "hello")
+        reg = Testy_Register(SAVES_DIR, "sh",  "hello")
 
         with self.assertRaisesRegex(RegisterError, "open.*rmv_apos"):
             reg.rmv_apos(ApriInfo(no ="no"))
 
         with reg.open() as reg:
 
             apri1 = ApriInfo(no ="yes")
@@ -1745,108 +1872,142 @@
 
         with reg.open(readonly= True) as reg:
             with self.assertRaisesRegex(RegisterError, "read-write"):
                 reg.rmv_apos(apri1)
 
     def test_disk_blocks_no_recursive(self):
 
-        reg = NumpyRegister(SAVES_DIR, "HI")
+        reg = NumpyRegister(SAVES_DIR, "sh", "HI")
+
         with reg.open() as reg:
+
             apri1 = ApriInfo(name ="abc")
             apri2 = ApriInfo(name ="xyz")
             blk1 = Block(np.arange(50), apri1, 0)
             blk2 = Block(np.arange(50), apri1, 50)
             blk3 = Block(np.arange(500), apri2, 1000)
 
-            reg.add_disk_blk(blk1)
-            total = 0
-            for i, blk in enumerate(reg.blks(apri1)):
-                total += 1
-                if i == 0:
-                    self.assertEqual(
-                        blk1,
-                        blk
-                    )
-                else:
-                    self.fail()
+            with blk1:
+
+                reg.add_disk_blk(blk1)
+                total = 0
+
+                for i, blk in enumerate(reg.blks(apri1)):
+
+                    total += 1
+
+                    if i == 0:
+
+                        self.assertEqual(
+                            blk1,
+                            blk
+                        )
+
+                    else:
+                        self.fail()
+
             self.assertEqual(
                 1,
                 total
             )
 
-            reg.add_disk_blk(blk2)
-            total = 0
-            for i, blk in enumerate(reg.blks(apri1)):
-                total += 1
-                if i == 0:
-                    self.assertEqual(
-                        blk1,
-                        blk
-                    )
-                elif i == 1:
-                    self.assertEqual(
-                        blk2,
-                        blk
-                    )
-                else:
-                    self.fail()
-            self.assertEqual(
-                2,
-                total
-            )
+            with open_blks(blk1, blk2):
+
+                reg.add_disk_blk(blk2)
+                total = 0
+
+                for i, blk in enumerate(reg.blks(apri1)):
+
+                    total += 1
+
+                    if i == 0:
+
+                        self.assertEqual(
+                            blk1,
+                            blk
+                        )
+
+                    elif i == 1:
+                        self.assertEqual(
+                            blk2,
+                            blk
+                        )
+
+                    else:
+                        self.fail()
 
-            reg.add_disk_blk(blk3)
-            total = 0
-            for i, blk in enumerate(reg.blks(apri1)):
-                total += 1
-                if i == 0:
-                    self.assertEqual(
-                        blk1,
-                        blk
-                    )
-                elif i == 1:
-                    self.assertEqual(
-                        blk2,
-                        blk
-                    )
-                else:
-                    self.fail()
             self.assertEqual(
                 2,
                 total
             )
-            total = 0
-            for i,blk in enumerate(reg.blks(apri2)):
-                total += 1
-                if i == 0:
-                    self.assertEqual(
-                        blk3,
-                        blk
-                    )
-                else:
-                    self.fail()
-            self.assertEqual(
-                1,
-                total
-            )
+
+            with open_blks(blk1, blk2, blk3):
+
+                reg.add_disk_blk(blk3)
+                total = 0
+
+                for i, blk in enumerate(reg.blks(apri1)):
+
+                    total += 1
+
+                    if i == 0:
+                        self.assertEqual(
+                            blk1,
+                            blk
+                        )
+
+                    elif i == 1:
+                        self.assertEqual(
+                            blk2,
+                            blk
+                        )
+                    else:
+                        self.fail()
+
+                self.assertEqual(
+                    2,
+                    total
+                )
+
+            with blk3:
+
+                total = 0
+
+                for i,blk in enumerate(reg.blks(apri2)):
+
+                    total += 1
+
+                    if i == 0:
+                        self.assertEqual(
+                            blk3,
+                            blk
+                        )
+
+                    else:
+                        self.fail()
+
+                self.assertEqual(
+                    1,
+                    total
+                )
 
     def test__iter_subregisters(self):
 
-        reg = Testy_Register(SAVES_DIR, "hello")
+        reg = Testy_Register(SAVES_DIR, "sh",  "hello")
         with reg.open() as reg:
             total = 0
             for i,_ in enumerate(reg._iter_subregs()):
                 total += 1
             self.assertEqual(
                 0,
                 total
             )
 
 
-        reg = Testy_Register(SAVES_DIR, "hello")
+        reg = Testy_Register(SAVES_DIR, "sh",  "hello")
 
         with reg.open() as reg:
 
             with reg._db.begin(write = True) as txn:
                 txn.put(reg._get_subreg_key(), _SUB_VAL)
 
             total = 0
@@ -1860,17 +2021,17 @@
                 else:
                     self.fail()
             self.assertEqual(
                 1,
                 total
             )
 
-        reg1 = Testy_Register(SAVES_DIR, "hello")
-        reg2 = Testy_Register(SAVES_DIR, "hello")
-        reg3 = Testy_Register(SAVES_DIR, "hello")
+        reg1 = Testy_Register(SAVES_DIR, "sh",  "hello")
+        reg2 = Testy_Register(SAVES_DIR, "sh",  "hello")
+        reg3 = Testy_Register(SAVES_DIR, "sh",  "hello")
 
         with reg2.open():pass
         with reg3.open():pass
 
         with reg1.open() as reg:
 
             with reg1._db.begin(write=True) as txn:
@@ -1892,17 +2053,17 @@
                 2,
                 total
             )
             self.assertFalse(
                 regs[0] is regs[1]
             )
 
-        reg1 = Testy_Register(SAVES_DIR, "hello")
-        reg2 = Testy_Register(SAVES_DIR, "hello")
-        reg3 = Testy_Register(SAVES_DIR, "hello")
+        reg1 = Testy_Register(SAVES_DIR, "sh",  "hello")
+        reg2 = Testy_Register(SAVES_DIR, "sh",  "hello")
+        reg3 = Testy_Register(SAVES_DIR, "sh",  "hello")
         with reg3.open():pass
 
         with reg2.open():
 
             with reg2._db.begin(write=True) as txn:
                 txn.put(reg3._get_subreg_key(), _SUB_VAL)
 
@@ -1940,327 +2101,426 @@
                 else:
                     self.fail()
             self.assertEqual(
                 1,
                 total
             )
 
-    def test_blkByN(self):
+    def test_blk_by_n(self):
+
+        reg = Testy_Register(SAVES_DIR, "sh",  "hello")
 
-        reg = Testy_Register(SAVES_DIR, "hello")
         with self.assertRaisesRegex(RegisterError, "open.*blk_by_n"):
-            reg.blk_by_n(ApriInfo(name ="no"), -1)
 
-        reg = Testy_Register(SAVES_DIR, "hello")
+            with reg.blk_by_n(ApriInfo(name ="no"), -1):
+                pass
+
+        reg = Testy_Register(SAVES_DIR, "sh",  "hello")
+
         with self.assertRaisesRegex(IndexError, "non-negative"):
+
             with reg.open() as reg:
-                reg.blk_by_n(ApriInfo(name ="no"), -1)
 
-        reg = Testy_Register(SAVES_DIR, "hello")
+                with reg.blk_by_n(ApriInfo(name ="no"), -1):
+                    pass
+
+        reg = Testy_Register(SAVES_DIR, "sh",  "hello")
         apri = ApriInfo(name ="list")
         blk1 = Block(list(range(1000)), apri)
-        with reg.open() as reg:
-            reg.add_ram_blk(blk1)
-            for n in [0, 10, 500, 990, 999]:
-                self.assertIs(
-                    blk1,
-                    reg.blk_by_n(apri, n)
-                )
-            with self.assertRaises(DataNotFoundError):
-                reg.blk_by_n(apri, 1000)
 
-        blk2 = Block(list(range(1000, 2000)), apri, 1000)
         with reg.open() as reg:
-            reg.add_ram_blk(blk2)
-            for n in [1000, 1010, 1990, 1999]:
-                self.assertIs(
-                    blk2,
-                    reg.blk_by_n(apri, n)
-                )
 
-        reg = Testy_Register(SAVES_DIR, "whatever")
+            with blk1:
+
+                reg.add_ram_blk(blk1)
+
+                for n in [0, 10, 500, 990, 999]:
 
+                    with reg.blk_by_n(apri, n) as blk:
+                        self.assertIs(
+                            blk1,
+                            blk
+                        )
+
+                with self.assertRaises(DataNotFoundError):
+
+                    with reg.blk_by_n(apri, 1000):
+                        pass
+
+                blk2 = Block(list(range(1000, 2000)), apri, 1000)
+
+                with blk2:
+
+                    reg.add_ram_blk(blk2)
+
+                    for n in [1000, 1010, 1990, 1999]:
+
+                        with reg.blk_by_n(apri, n) as blk:
+                            self.assertIs(
+                                blk2,
+                                blk
+                            )
+
+        reg = Testy_Register(SAVES_DIR, "sh",  "whatever")
         apri = ApriInfo(name ="whatev")
-        with reg.open() as reg: pass
+
+        with reg.open() as reg:
+            pass
+
         with self.assertRaisesRegex(RegisterError, "open.*blk_by_n"):
-            for _ in reg.blk_by_n(apri, 0): pass
+
+            with reg.blk_by_n(apri, 0):
+                pass
 
         apri1 = ApriInfo(name ="foomy")
         apri2 = ApriInfo(name ="doomy")
         blk1 = Block(list(range(10)), apri1)
         blk2 = Block(list(range(20)), apri1, 10)
         blk3 = Block(list(range(14)), apri2, 50)
         blk4 = Block(list(range(100)), apri2, 120)
         blk5 = Block(list(range(120)), apri2, 1000)
-        reg1 = Testy_Register(SAVES_DIR, "helllo")
-        reg2 = Testy_Register(SAVES_DIR, "suuup")
-
-        with reg1.open() as reg1:
-
-            reg1.add_ram_blk(blk1)
-            reg1.add_ram_blk(blk2)
-            reg1.add_ram_blk(blk3)
-
-        with reg2.open() as reg2:
+        reg1 = Testy_Register(SAVES_DIR, "sh",  "helllo")
+        reg2 = Testy_Register(SAVES_DIR, "sh",  "suuup")
 
-            reg2.add_ram_blk(blk4)
-            reg2.add_ram_blk(blk5)
+        with open_regs(reg1, reg2) as (reg1, reg2):
 
+            with open_blks(blk1, blk2, blk3, blk4, blk5):
 
-        tests = [
-            (reg1, (apri1,    0, True ), blk1),
-            (reg1, (apri1,    0, False), blk1),
-            (reg1, (apri1,    9, True ), blk1),
-            (reg1, (apri1,    9, False), blk1),
-            (reg1, (apri1,   10, True ), blk2),
-            (reg1, (apri1,   10, False), blk2),
-            (reg1, (apri1,   29, True ), blk2),
-            (reg1, (apri1,   29, False), blk2),
-            (reg1, (apri2,   50, True ), blk3),
-            (reg1, (apri2,   50, False), blk3),
-            (reg1, (apri2,   63, True ), blk3),
-            (reg1, (apri2,   63, False), blk3),
-            (reg2, (apri2,  120, True ), blk4),
-            (reg2, (apri2,  219, True ), blk4),
-            (reg2, (apri2, 1000, True ), blk5),
-            (reg2, (apri2, 1119, True ), blk5)
-        ]
+                reg1.add_ram_blk(blk1)
+                reg1.add_ram_blk(blk2)
+                reg1.add_ram_blk(blk3)
+                reg2.add_ram_blk(blk4)
+                reg2.add_ram_blk(blk5)
+
+                tests = [
+                    (reg1, (apri1,    0, True ), blk1),
+                    (reg1, (apri1,    0, False), blk1),
+                    (reg1, (apri1,    9, True ), blk1),
+                    (reg1, (apri1,    9, False), blk1),
+                    (reg1, (apri1,   10, True ), blk2),
+                    (reg1, (apri1,   10, False), blk2),
+                    (reg1, (apri1,   29, True ), blk2),
+                    (reg1, (apri1,   29, False), blk2),
+                    (reg1, (apri2,   50, True ), blk3),
+                    (reg1, (apri2,   50, False), blk3),
+                    (reg1, (apri2,   63, True ), blk3),
+                    (reg1, (apri2,   63, False), blk3),
+                    (reg2, (apri2,  120, True ), blk4),
+                    (reg2, (apri2,  219, True ), blk4),
+                    (reg2, (apri2, 1000, True ), blk5),
+                    (reg2, (apri2, 1119, True ), blk5)
+                ]
+
+                for reg, args, blk in tests:
+
+                    with reg.blk_by_n(*args[:2]) as blk_:
+                        self.assertIs(
+                            blk,
+                            blk_
+                        )
 
-        for reg, args, blk in tests:
-            with reg.open() as reg:
-                try:
-                    self.assertIs(
-                        blk,
-                        reg.blk_by_n(*args[:2])
-                    )
-                except:
-                    raise
+        reg = NumpyRegister(SAVES_DIR, "sh", "hello")
 
-        reg = NumpyRegister(SAVES_DIR, "hello")
         with self.assertRaises(RegisterError):
-            reg.blk_by_n(ApriInfo(name="no"), 50)
 
-        reg = NumpyRegister(SAVES_DIR, "hello")
+            with reg.blk_by_n(ApriInfo(name="no"), 50):
+                pass
+
+        reg = NumpyRegister(SAVES_DIR, "sh", "hello")
         apri1 = ApriInfo(name ="sup")
         apri2 = ApriInfo(name ="hi")
         blk1 = Block(np.arange(75), apri1)
         blk2 = Block(np.arange(125), apri1, 75)
         blk3 = Block(np.arange(1000), apri2, 100)
         blk4 = Block(np.arange(100), apri2, 2000)
+
         with reg.open() as reg:
-            reg.add_disk_blk(blk1)
-            reg.add_disk_blk(blk2)
-            reg.add_disk_blk(blk3)
-            reg.add_disk_blk(blk4)
-            for n in [0, 1, 2, 72, 73, 74]:
-                self.assertEqual(
-                    blk1,
-                    reg.blk_by_n(apri1, n)
-                )
-            for n in [75, 76, 77, 197, 198, 199]:
-                self.assertEqual(
-                    blk2,
-                    reg.blk_by_n(apri1, n)
-                )
-            for n in [-2, -1]:
-                with self.assertRaisesRegex(IndexError, "non-negative"):
-                    reg.blk_by_n(apri1, n)
-            for n in [200, 201, 1000]:
-                with self.assertRaises(DataNotFoundError):
-                    reg.blk_by_n(apri1, n)
+
+            with open_blks(blk1, blk2, blk3, blk4):
+
+                reg.add_disk_blk(blk1)
+                reg.add_disk_blk(blk2)
+                reg.add_disk_blk(blk3)
+                reg.add_disk_blk(blk4)
+
+                for n in [0, 1, 2, 72, 73, 74]:
+
+                    with reg.blk_by_n(apri1, n) as blk:
+                        self.assertEqual(
+                            blk1,
+                            blk
+                        )
+
+                for n in [75, 76, 77, 197, 198, 199]:
+
+                    with reg.blk_by_n(apri1, n) as blk:
+                        self.assertEqual(
+                            blk2,
+                            blk
+                        )
+
+                for n in [-2, -1]:
+
+                    with self.assertRaisesRegex(IndexError, "non-negative"):
+
+                        with reg.blk_by_n(apri1, n):
+                            pass
+
+                for n in [200, 201, 1000]:
+
+                    with self.assertRaises(DataNotFoundError):
+
+                        with reg.blk_by_n(apri1, n):
+                            pass
 
     def test_blk(self):
 
-        reg = NumpyRegister(SAVES_DIR, "hello")
+        reg = NumpyRegister(SAVES_DIR, "sh", "hello")
+
         with self.assertRaisesRegex(RegisterError, "blk"):
-            reg.blk(ApriInfo(name="i am the octopus"), 0, 0)
 
-        reg = NumpyRegister(SAVES_DIR, "hello")
+            with reg.blk(ApriInfo(name="i am the octopus"), 0, 0):
+                pass
+
+        reg = NumpyRegister(SAVES_DIR, "sh", "hello")
+
         with reg.open() as reg:
+
             apri1 = ApriInfo(name ="i am the octopus")
-            blk1 = Block(np.arange(100), apri1)
-            reg.add_disk_blk(blk1)
 
-            self.assertEqual(
-                blk1,
-                reg.blk(apri1, 0, 100)
-            )
+            with Block(np.arange(100), apri1) as blk1:
 
-            blk2 = Block(np.arange(100,200), apri1, 100)
-            reg.add_disk_blk(blk2)
+                reg.add_disk_blk(blk1)
 
-            self.assertEqual(
-                blk2,
-                reg.blk(apri1, 100, 100)
-            )
+                with reg.blk(apri1, 0, 100) as blk:
+                    self.assertEqual(
+                        blk1,
+                        blk
+                    )
 
-            self.assertEqual(
-                blk1,
-                reg.blk(apri1, 0, 100)
-            )
+            with Block(np.arange(100,200), apri1, 100) as blk2:
+
+                reg.add_disk_blk(blk2)
+
+                with reg.blk(apri1, 100, 100) as blk:
+                    self.assertEqual(
+                        blk2,
+                        blk
+                    )
+
+            with blk1:
+
+                with reg.blk(apri1, 0, 100) as blk:
+                    self.assertEqual(
+                        blk1,
+                        blk
+                    )
 
             apri2 = ApriInfo(name ="hello")
-            blk3 = Block(np.arange(3000,4000), apri2, 2000)
-            reg.add_disk_blk(blk3)
 
-            self.assertEqual(
-                blk3,
-                reg.blk(apri2, 2000, 1000)
-            )
+            with Block(np.arange(3000,4000), apri2, 2000) as blk3:
 
-            self.assertEqual(
-                blk2,
-                reg.blk(apri1, 100, 100)
-            )
+                reg.add_disk_blk(blk3)
 
-            self.assertEqual(
-                blk1,
-                reg.blk(apri1, 0, 100)
-            )
+                with reg.blk(apri2, 2000, 1000) as blk:
+                    self.assertEqual(
+                        blk3,
+                        blk
+                    )
+
+            with open_blks(blk1, blk2, reg.blk(apri1, 100, 100), reg.blk(apri1, 0, 100)) as (blk1, blk2, blk3, blk4):
+
+                self.assertEqual(
+                    blk2,
+                    blk3
+                )
+
+                self.assertEqual(
+                    blk1,
+                    blk4
+                )
 
             for metadata in [
                 (apri1, 0, 200), (apri1, 1, 99), (apri1, 5, 100), (apri1, 1, 100),
                 (apri2, 2000, 999), (apri2, 2000, 1001), (apri2, 1999, 1000),
                 (ApriInfo(name ="noooo"), 0, 100)
             ]:
                 with self.assertRaises(DataNotFoundError):
-                    reg.blk(*metadata)
+
+                    with reg.blk(*metadata):
+                        pass
 
             apri3 = ApriInfo(
                 name = "'''i love quotes'''and'' backslashes\\\\",
                 num = '\\\"double\\quotes\' are cool too"'
             )
             blk = Block(np.arange(69, 420), apri3)
-            reg.add_disk_blk(blk)
 
-            self.assertEqual(
-                blk,
-                reg.blk(apri3, 0, 420 - 69)
-            )
+            with blk:
 
-        reg = NumpyRegister(SAVES_DIR, "tests")
+                reg.add_disk_blk(blk)
 
+                with reg.blk(apri3, 0, 420 - 69) as blk2:
+                    self.assertEqual(
+                        blk,
+                        blk2
+                    )
+
+        reg = NumpyRegister(SAVES_DIR, "sh", "tests")
         apri1 = ApriInfo(descr ="hey")
 
         with self.assertRaisesRegex(RegisterError, "open.*blk"):
-            reg.blk(apri1)
+
+            with reg.blk(apri1):
+                pass
 
         with reg.open() as reg:
 
             with self.assertRaisesRegex(TypeError, "ApriInfo"):
-                reg.blk("kitty kat")
+
+                with reg.blk("kitty kat"):
+                    pass
 
             with self.assertRaisesRegex(TypeError, "int"):
-                reg.blk(apri1, "puppy dawg")
+
+                with reg.blk(apri1, "puppy dawg"):
+                    pass
 
             with self.assertRaisesRegex(TypeError, "int"):
-                reg.blk(apri1, 0, "bunny wunny")
+
+                with reg.blk(apri1, 0, "bunny wunny"):
+                    pass
 
             with self.assertRaisesRegex(ValueError, "non-negative"):
-                reg.blk(apri1, -1)
+
+                with reg.blk(apri1, -1):
+                    pass
 
             with self.assertRaisesRegex(ValueError, "non-negative"):
-                reg.blk(apri1, 0, -1)
+
+                with reg.blk(apri1, 0, -1):
+                    pass
 
             with self.assertRaises(ValueError):
-                reg.blk(apri1, length=-1)
 
-            reg.add_disk_blk(Block(list(range(50)), apri1))
+                with reg.blk(apri1, length=-1):
+                    pass
 
-            self.assertTrue(np.all(
-                reg.blk(apri1).segment() == np.arange(50)
-            ))
+            with Block(list(range(50)), apri1) as blk:
+                reg.add_disk_blk(blk)
 
-            self.assertTrue(np.all(
-                reg.blk(apri1, 0).segment() == np.arange(50)
-            ))
+            with reg.blk(apri1) as blk:
+                self.assertTrue(np.all(
+                    blk.segment() == np.arange(50)
+                ))
 
-            self.assertTrue(np.all(
-                reg.blk(apri1, 0, 50).segment() == np.arange(50)
-            ))
+            with reg.blk(apri1) as blk:
+                self.assertTrue(np.all(
+                    blk.segment() == np.arange(50)
+                ))
 
-            reg.add_disk_blk(Block(list(range(51)), apri1))
+            with reg.blk(apri1, 0, 50) as blk:
+                self.assertTrue(np.all(
+                    blk.segment() == np.arange(50)
+                ))
 
-            self.assertTrue(np.all(
-                reg.blk(apri1).segment() == np.arange(51)
-            ))
+            with Block(list(range(51)), apri1) as blk:
+                reg.add_disk_blk(blk)
 
-            self.assertTrue(np.all(
-                reg.blk(apri1, 0).segment() == np.arange(51)
-            ))
+            with reg.blk(apri1) as blk:
+                self.assertTrue(np.all(
+                    blk.segment() == np.arange(51)
+                ))
 
-            self.assertTrue(np.all(
-                reg.blk(apri1, 0, 51).segment() == np.arange(51)
-            ))
+            with reg.blk(apri1, 0) as blk:
+                self.assertTrue(np.all(
+                    blk.segment() == np.arange(51)
+                ))
 
-            self.assertTrue(np.all(
-                reg.blk(apri1, 0, 50).segment() == np.arange(50)
-            ))
+            with reg.blk(apri1, 0, 51) as blk:
+                self.assertTrue(np.all(
+                    blk.segment() == np.arange(51)
+                ))
 
-            reg.add_disk_blk(Block(list(range(100)), apri1, 1))
+            with reg.blk(apri1, 0, 50) as blk:
+                self.assertTrue(np.all(
+                    blk.segment() == np.arange(50)
+                ))
 
-            self.assertTrue(np.all(
-                reg.blk(apri1).segment() == np.arange(51)
-            ))
+            with Block(list(range(100)), apri1, 1) as blk:
+                reg.add_disk_blk(blk)
 
-            self.assertTrue(np.all(
-                reg.blk(apri1, 0).segment() == np.arange(51)
-            ))
+            with reg.blk(apri1) as blk:
+                self.assertTrue(np.all(
+                    blk.segment() == np.arange(51)
+                ))
 
-            self.assertTrue(np.all(
-                reg.blk(apri1, 0, 51).segment() == np.arange(51)
-            ))
+            with reg.blk(apri1, 0) as blk:
+                self.assertTrue(np.all(
+                    blk.segment() == np.arange(51)
+                ))
 
-            self.assertTrue(np.all(
-                reg.blk(apri1, 0, 50).segment() == np.arange(50)
-            ))
+            with reg.blk(apri1, 0, 51) as blk:
+                self.assertTrue(np.all(
+                    blk.segment() == np.arange(51)
+                ))
 
-            self.assertTrue(np.all(
-                reg.blk(apri1, 1, 100).segment() == np.arange(100)
-            ))
+            with reg.blk(apri1, 0, 50) as blk:
+                self.assertTrue(np.all(
+                    blk.segment() == np.arange(50)
+                ))
 
-            blk1 = Block(list(range(5)), apri1)
-            reg.add_ram_blk(blk1)
+            with reg.blk(apri1, 1, 100) as blk:
+                self.assertTrue(np.all(
+                    blk.segment() == np.arange(100)
+                ))
 
-            self.assertIs(
-                blk1,
-                reg.blk(apri1)
-            )
+            with Block(list(range(5)), apri1) as blk1:
 
-            self.assertIs(
-                blk1,
-                reg.blk(apri1, 0)
-            )
+                reg.add_ram_blk(blk1)
 
-            self.assertIs(
-                blk1,
-                reg.blk(apri1, 0, 5)
-            )
+                with reg.blk(apri1) as blk:
+                    self.assertIs(
+                        blk1,
+                        blk
+                    )
+
+                with reg.blk(apri1, 0) as blk:
+                    self.assertIs(
+                        blk1,
+                        blk
+                    )
+
+                with reg.blk(apri1, 0, 5) as blk:
+                    self.assertIs(
+                        blk1,
+                        blk
+                    )
 
     def test__check_no_cycles_from(self):
 
-        reg = Testy_Register(SAVES_DIR, "hello")
+        reg = Testy_Register(SAVES_DIR, "sh",  "hello")
         with self.assertRaises(RegisterError):
             reg._check_no_cycles_from(reg)
 
-        reg = Testy_Register(SAVES_DIR, "hello")
+        reg = Testy_Register(SAVES_DIR, "sh",  "hello")
         with reg.open() as reg:pass
 
         # loop
         self.assertFalse(
             reg._check_no_cycles_from(reg)
         )
 
-        reg1 = Testy_Register(SAVES_DIR, "hello")
-        reg2 = Testy_Register(SAVES_DIR, "hello")
-        reg3 = Testy_Register(SAVES_DIR, "hello")
-        reg4 = Testy_Register(SAVES_DIR, "hello")
-        reg5 = Testy_Register(SAVES_DIR, "hello")
-        reg6 = Testy_Register(SAVES_DIR, "hello")
-        reg7 = Testy_Register(SAVES_DIR, "hello")
+        reg1 = Testy_Register(SAVES_DIR, "sh",  "hello")
+        reg2 = Testy_Register(SAVES_DIR, "sh",  "hello")
+        reg3 = Testy_Register(SAVES_DIR, "sh",  "hello")
+        reg4 = Testy_Register(SAVES_DIR, "sh",  "hello")
+        reg5 = Testy_Register(SAVES_DIR, "sh",  "hello")
+        reg6 = Testy_Register(SAVES_DIR, "sh",  "hello")
+        reg7 = Testy_Register(SAVES_DIR, "sh",  "hello")
         with reg1.open(): pass
         with reg2.open(): pass
         with reg3.open(): pass
         with reg4.open(): pass
         with reg5.open(): pass
         with reg6.open(): pass
         with reg7.open(): pass
@@ -2550,15 +2810,15 @@
             reg3._check_no_cycles_from(reg7)
         )
 
         # long path (0 -> 1 -> ... -> N)
 
         N = 10
 
-        regs = [NumpyRegister(SAVES_DIR, f"{i}") for i in range(N + 2)]
+        regs = [NumpyRegister(SAVES_DIR, "sh", f"{i}") for i in range(N + 2)]
 
         for reg in regs:
             with reg.open():pass
 
         for i in range(N):
             with regs[i].open() as reg:
                 with reg._db.begin(write=True) as txn:
@@ -2594,28 +2854,28 @@
             regi = eval(f"reg{i}")
             regj = eval(f"reg{j}")
 
             self.assertTrue(regi._check_no_cycles_from(regj))
 
     def test_add_subregister(self):
 
-        reg1 = Testy_Register(SAVES_DIR, "hello")
-        reg2 = Testy_Register(SAVES_DIR, "hello")
+        reg1 = Testy_Register(SAVES_DIR, "sh",  "hello")
+        reg2 = Testy_Register(SAVES_DIR, "sh",  "hello")
         with self.assertRaisesRegex(RegisterError, "open.*add_subreg"):
             reg1.add_subreg(reg2)
 
-        reg1 = Testy_Register(SAVES_DIR, "hello")
-        reg2 = Testy_Register(SAVES_DIR, "hello")
+        reg1 = Testy_Register(SAVES_DIR, "sh",  "hello")
+        reg2 = Testy_Register(SAVES_DIR, "sh",  "hello")
         with reg1.open() as reg1:
             with self.assertRaisesRegex(RegisterError, "add_subreg"):
                 reg1.add_subreg(reg2)
 
-        reg1 = Testy_Register(SAVES_DIR, "hello")
-        reg2 = Testy_Register(SAVES_DIR, "hello")
-        reg3 = Testy_Register(SAVES_DIR, "hello")
+        reg1 = Testy_Register(SAVES_DIR, "sh",  "hello")
+        reg2 = Testy_Register(SAVES_DIR, "sh",  "hello")
+        reg3 = Testy_Register(SAVES_DIR, "sh",  "hello")
         with reg2.open(): pass
         with reg1.open() as reg1:
             try:
                 reg1.add_subreg(reg2)
             except RegisterError:
                 self.fail()
 
@@ -2632,17 +2892,17 @@
                 self.fail()
         with reg1.open() as reg1:
             try:
                 reg1.add_subreg(reg3)
             except RegisterError:
                 self.fail()
 
-        reg1 = Testy_Register(SAVES_DIR, "hello")
-        reg2 = Testy_Register(SAVES_DIR, "hello")
-        reg3 = Testy_Register(SAVES_DIR, "hello")
+        reg1 = Testy_Register(SAVES_DIR, "sh",  "hello")
+        reg2 = Testy_Register(SAVES_DIR, "sh",  "hello")
+        reg3 = Testy_Register(SAVES_DIR, "sh",  "hello")
         with reg3.open(): pass
         with reg2.open() as reg2:
             try:
                 reg2.add_subreg(reg3)
             except RegisterError:
                 self.fail()
         with reg1.open() as reg1:
@@ -2650,16 +2910,16 @@
                 reg1.add_subreg(reg2)
             except RegisterError:
                 self.fail()
         with reg3.open() as reg3:
             with self.assertRaises(RegisterError):
                 reg3.add_subreg(reg1)
 
-        reg1 = Testy_Register(SAVES_DIR, "hello")
-        reg2 = Testy_Register(SAVES_DIR, "hello")
+        reg1 = Testy_Register(SAVES_DIR, "sh",  "hello")
+        reg2 = Testy_Register(SAVES_DIR, "sh",  "hello")
 
         with reg1.open():pass
         with reg2.open():pass
 
         with reg1.open() as reg1:
 
             for debug in [1,2]:
@@ -2674,17 +2934,17 @@
                 self.assertEqual(
                     0,
                     lmdb_count_keys(reg1._db, _SUB_KEY_PREFIX)
                 )
 
     def test_remove_subregister(self):
 
-        reg1 = Testy_Register(SAVES_DIR, "hello")
-        reg2 = Testy_Register(SAVES_DIR, "hello")
-        reg3 = Testy_Register(SAVES_DIR, "hello")
+        reg1 = Testy_Register(SAVES_DIR, "sh",  "hello")
+        reg2 = Testy_Register(SAVES_DIR, "sh",  "hello")
+        reg3 = Testy_Register(SAVES_DIR, "sh",  "hello")
 
         with reg1.open():pass
         with reg2.open():pass
 
         with self.assertRaisesRegex(RegisterError, "open.*rmv_subreg"):
             reg1.rmv_subreg(reg2)
 
@@ -2740,159 +3000,183 @@
         with self.assertRaisesRegex(RegisterError, "read-write"):
 
             with reg1.open(readonly= True) as reg1:
                 reg1.rmv_subreg(reg2)
 
     def test_blks(self):
 
-        reg = Testy_Register(SAVES_DIR, "whatever")
+        reg = Testy_Register(SAVES_DIR, "sh",  "whatever")
         apri = ApriInfo(name ="whatev")
 
         with self.assertRaisesRegex(RegisterError, "open.*blks"):
             list(reg.blks(apri))
 
-        reg = Testy_Register(SAVES_DIR, "whatever")
+        reg = Testy_Register(SAVES_DIR, "sh",  "whatever")
         apri1 = ApriInfo(name ="foomy")
         apri2 = ApriInfo(name ="doomy")
         blk1 = Block(list(range(10)), apri1)
         blk2 = Block(list(range(20)), apri1, 10)
         blk3 = Block(list(range(14)), apri2, 50)
         blk4 = Block(list(range(100)), apri2, 120)
         blk5 = Block(list(range(120)), apri2, 1000)
-        reg1 = Testy_Register(SAVES_DIR, "helllo")
-        reg2 = Testy_Register(SAVES_DIR, "suuup")
+        reg1 = Testy_Register(SAVES_DIR, "sh",  "helllo")
+        reg2 = Testy_Register(SAVES_DIR, "sh",  "suuup")
 
-        with reg1.open() as reg1:
+        with open_blks(blk1, blk2, blk3, blk4, blk5):
 
-            reg1.add_ram_blk(blk1)
-            reg1.add_ram_blk(blk2)
-            reg1.add_ram_blk(blk3)
+            with open_regs(reg1, reg2) as (reg1, reg2):
 
-        with reg2.open() as reg2:
+                reg1.add_ram_blk(blk1)
+                reg1.add_ram_blk(blk2)
+                reg1.add_ram_blk(blk3)
+                reg2.add_ram_blk(blk4)
+                reg2.add_ram_blk(blk5)
+                total = 0
 
-            reg2.add_ram_blk(blk4)
-            reg2.add_ram_blk(blk5)
+                for i, blk in enumerate(reg1.blks(apri1)):
 
-        with reg1.open() as reg1:
+                    total += 1
 
-            total = 0
-            for i, blk in enumerate(reg1.blks(apri1)):
-                total += 1
-                if i == 0:
-                    self.assertIs(
-                        blk1,
-                        blk
-                    )
-                elif i == 1:
-                    self.assertIs(
-                        blk2,
-                        blk
-                    )
-                else:
-                    self.fail()
+                    if i == 0:
+                        self.assertIs(
+                            blk1,
+                            blk
+                        )
 
-            self.assertEqual(
-                2,
-                total
-            )
+                    elif i == 1:
+                        self.assertIs(
+                            blk2,
+                            blk
+                        )
 
-        with reg2.open(): pass
-        with reg1.open() as reg1:
-            reg1.add_subreg(reg2)
-            total = 0
-            for i, blk in enumerate(reg1.blks(apri1, recursively = True)):
-                total += 1
-                if i == 0:
-                    self.assertIs(
-                        blk1,
-                        blk
-                    )
-                elif i == 1:
-                    self.assertIs(
-                        blk2,
-                        blk
-                    )
-                else:
-                    self.fail()
-            self.assertEqual(
-                2,
-                total
-            )
+                    else:
+                        self.fail()
 
-            total = 0
-            for i, blk in enumerate(reg1.blks(apri2, recursively = True)):
-                total += 1
-                if i == 0:
-                    self.assertIs(
-                        blk3,
-                        blk
-                    )
-                elif i == 1:
-                    self.assertIs(
-                        blk4,
-                        blk
-                    )
-                elif i == 2:
-                    self.assertIs(
-                        blk5,
-                        blk
-                    )
-                else:
-                    self.fail()
-            self.assertEqual(
-                3,
-                total
-            )
+                self.assertEqual(
+                    2,
+                    total
+                )
+
+            with reg2.open():
+                pass
+
+            with reg1.open() as reg1:
+
+                reg1.add_subreg(reg2)
+                total = 0
 
-        reg = Testy_Register(SAVES_DIR, "msg")
+                for i, blk in enumerate(reg1.blks(apri1, recursively = True)):
+
+                    total += 1
+
+                    if i == 0:
+                        self.assertIs(
+                            blk1,
+                            blk
+                        )
+
+                    elif i == 1:
+                        self.assertIs(
+                            blk2,
+                            blk
+                        )
+
+                    else:
+                        self.fail()
+
+                self.assertEqual(
+                    2,
+                    total
+                )
+                total = 0
+
+                for i, blk in enumerate(reg1.blks(apri2, recursively = True)):
+
+                    total += 1
+
+                    if i == 0:
+                        self.assertIs(
+                            blk3,
+                            blk
+                        )
+
+                    elif i == 1:
+                        self.assertIs(
+                            blk4,
+                            blk
+                        )
+
+                    elif i == 2:
+                        self.assertIs(
+                            blk5,
+                            blk
+                        )
+
+                    else:
+                        self.fail()
+
+                self.assertEqual(
+                    3,
+                    total
+                )
+
+        reg = Testy_Register(SAVES_DIR, "sh",  "msg")
         apri1 = ApriInfo(name="hey")
         blk1 = Block([], apri1)
 
-        with reg.open() as reg:
+        with blk1:
 
-            reg.add_ram_blk(blk1)
-            self.assertEqual(
-                1,
-                len(list(reg.blks(apri1)))
-            )
-            self.assertEqual(
-                blk1,
-                list(reg.blks(apri1))[0]
-            )
+            with reg.open() as reg:
 
-            apri2 = ApriInfo(name ="hello")
-            blk2 = Block(list(range(10)), apri2)
-            reg.add_ram_blk(blk2)
-            self.assertEqual(
-                1,
-                len(list(reg.blks(apri2)))
-            )
-            self.assertEqual(
-                blk2,
-                list(reg.blks(apri2))[0]
-            )
+                reg.add_ram_blk(blk1)
+                self.assertEqual(
+                    1,
+                    len(list(reg.blks(apri1)))
+                )
+                self.assertEqual(
+                    blk1,
+                    list(reg.blks(apri1))[0]
+                )
 
-            blk3 = Block(list(range(10)), apri2, 1)
-            reg.add_ram_blk(blk3)
-            self.assertEqual(
-                2,
-                len(list(reg.blks(apri2)))
-            )
-            self.assertIn(
-                blk2,
-                reg.blks(apri2)
-            )
-            self.assertIn(
-                blk3,
-                reg.blks(apri2)
-            )
+                apri2 = ApriInfo(name ="hello")
+                blk2 = Block(list(range(10)), apri2)
+
+                with blk2:
+
+                    reg.add_ram_blk(blk2)
+                    self.assertEqual(
+                        1,
+                        len(list(reg.blks(apri2)))
+                    )
+                    self.assertEqual(
+                        blk2,
+                        list(reg.blks(apri2))[0]
+                    )
+
+                    blk3 = Block(list(range(10)), apri2, 1)
+
+                    with blk3:
+
+                        reg.add_ram_blk(blk3)
+                        self.assertEqual(
+                            2,
+                            len(list(reg.blks(apri2)))
+                        )
+                        self.assertIn(
+                            blk2,
+                            reg.blks(apri2)
+                        )
+                        self.assertIn(
+                            blk3,
+                            reg.blks(apri2)
+                        )
 
     def test_intervals(self):
 
-        reg = Testy_Register(SAVES_DIR, "sup")
+        reg = Testy_Register(SAVES_DIR, "sh",  "sup")
 
         apri1 = ApriInfo(descr ="hello")
         apri2 = ApriInfo(descr ="hey")
 
         with self.assertRaisesRegex(RegisterError, "open.*intervals"):
             list(reg.intervals(apri1))
 
@@ -2902,39 +3186,43 @@
 
                 with self.assertRaisesRegex(DataNotFoundError, "ApriInfo"):
                     list(reg.intervals(apri, combine=False, diskonly=True))
 
 
         with reg.open() as reg:
 
-            reg.add_disk_blk(Block(list(range(50)), apri1))
+            with Block(list(range(50)), apri1) as blk:
+                reg.add_disk_blk(blk)
 
             self.assertEqual(
                 [(0, 50)],
                 list(reg.intervals(apri1, combine=False, diskonly=True))
             )
 
             with self.assertRaisesRegex(DataNotFoundError, "ApriInfo"):
                 list(reg.intervals(apri2, combine=False, diskonly=True))
 
-            reg.add_disk_blk(Block(list(range(100)), apri1))
+            with Block(list(range(100)), apri1) as blk:
+                reg.add_disk_blk(blk)
 
             self.assertEqual(
                 [(0, 100), (0, 50)],
                 list(reg.intervals(apri1, combine=False, diskonly=True))
             )
 
-            reg.add_disk_blk(Block(list(range(1000)), apri1, 1))
+            with Block(list(range(1000)), apri1, 1) as blk:
+                reg.add_disk_blk(blk)
 
             self.assertEqual(
                 [(0, 100), (0, 50), (1, 1000)],
                 list(reg.intervals(apri1, combine=False, diskonly=True))
             )
 
-            reg.add_disk_blk(Block(list(range(420)), apri2, 69))
+            with Block(list(range(420)), apri2, 69) as blk:
+                reg.add_disk_blk(blk)
 
             self.assertEqual(
                 [(0, 100), (0, 50), (1, 1000)],
                 list(reg.intervals(apri1, combine=False, diskonly=True))
             )
 
             self.assertEqual(
@@ -2944,28 +3232,30 @@
 
         # blk = Block(list(range(50)), )
 
     def test__iter_ram_and_disk_block_datas(self):pass
 
     def test_apri_infos(self):
 
-        reg = Testy_Register(SAVES_DIR, "tests")
+        reg = Testy_Register(SAVES_DIR, "sh",  "tests")
 
         with self.assertRaisesRegex(RegisterError, "open.*apris"):
             reg.apris()
 
-        for i in range(200):
+        for i in range(10):
 
             apri1 = ApriInfo(name = i)
             apri2 = ApriInfo(name =f"{i}")
 
             with reg.open() as reg:
 
-                reg.add_disk_blk(Block([1], apri1))
-                reg.add_ram_blk(Block([1], apri2))
+                with open_blks(Block([1], apri1), Block([1], apri2)) as (blk1, blk2):
+
+                    reg.add_disk_blk(blk1)
+                    reg.add_ram_blk(blk2)
 
                 get = reg.apris()
 
             self.assertEqual(
                 2*(i+1),
                 len(get)
             )
@@ -3026,15 +3316,15 @@
         data_key = reg._get_disk_blk_key(_BLK_KEY_PREFIX, apri, None, start_n, length, False)
 
         with reg._db.begin() as txn:
             return txn.get(data_key)
 
     def test_compress(self):
 
-        reg2 = NumpyRegister(SAVES_DIR, "testy2")
+        reg2 = NumpyRegister(SAVES_DIR, "sh", "testy2")
 
         with self.assertRaisesRegex(RegisterError, "open.*compress"):
             reg2.compress(ApriInfo(num = 0))
 
         apri1 = ApriInfo(descr ="sup")
         apri2 = ApriInfo(descr ="hey")
         apris = [apri1, apri1, apri2]
@@ -3044,17 +3334,20 @@
         length2 = 1000000
         blk2 = Block(np.arange(length2), apri1)
         length3 = 2000
         blk3 = Block(np.arange(length3), apri2)
         lengths = [length1, length2, length3]
 
         with reg2.open() as reg2:
-            reg2.add_disk_blk(blk1)
-            reg2.add_disk_blk(blk2)
-            reg2.add_disk_blk(blk3)
+
+            with open_blks(blk1, blk2, blk3):
+
+                reg2.add_disk_blk(blk1)
+                reg2.add_disk_blk(blk2)
+                reg2.add_disk_blk(blk3)
 
             for i, (apri, length) in enumerate(zip(apris, lengths)):
 
                 data_file_bytes = self._is_not_compressed_helper(reg2, apri, 0, length)
                 reg2.compress(apri, 0, length)
                 self._is_compressed_helper(reg2, apri, 0, length, data_file_bytes)
 
@@ -3067,60 +3360,61 @@
                 with self.assertRaisesRegex(CompressionError, expected):
                     reg2.compress(apri, 0, length)
 
         with self.assertRaisesRegex(RegisterError, "read-write"):
             with reg2.open(readonly= True) as reg2:
                 reg2.compress(ApriInfo(num = 0))
 
-        reg = NumpyRegister(SAVES_DIR, "no")
+        reg = NumpyRegister(SAVES_DIR, "sh", "no")
 
         with reg.open() as reg:
 
             apri = ApriInfo(num = 7)
             blk = Block(np.arange(40), apri)
-            reg.add_disk_blk(blk)
+
+            with blk:
+                reg.add_disk_blk(blk)
 
             for debug in [1,2,3,4]:
 
                 cornifer.registers._debug = debug
 
                 with self.assertRaises(KeyboardInterrupt):
                     reg.compress(apri)
 
                 cornifer.registers._debug = _NO_DEBUG
 
                 self._is_not_compressed_helper(reg, apri, 0, 40)
 
     def test_decompress(self):
 
-        reg1 = NumpyRegister(SAVES_DIR, "lol")
-
+        reg1 = NumpyRegister(SAVES_DIR, "sh", "lol")
         apri1 = ApriInfo(descr ="LOL")
         apri2 = ApriInfo(decr ="HAHA")
         apris = [apri1, apri1, apri2]
 
         with self.assertRaisesRegex(RegisterError, "open.*decompress"):
             reg1.decompress(apri1)
 
         lengths = [50, 500, 5000]
         start_ns = [0, 0, 1000]
-
         data = [np.arange(length) for length in lengths]
-
         blks = [Block(*t) for t in zip(data, apris, start_ns)]
-
         data_files_bytes = []
 
         with reg1.open() as reg1:
 
             for blk in blks:
-                reg1.add_disk_blk(blk)
-                data_files_bytes.append(
-                    self._is_not_compressed_helper(reg1, blk.apri(), blk.startn(), len(blk))
-                )
+
+                with blk:
+
+                    reg1.add_disk_blk(blk)
+                    data_files_bytes.append(
+                        self._is_not_compressed_helper(reg1, blk.apri(), blk.startn(), len(blk))
+                    )
 
             for t in zip(apris, start_ns, lengths):
                 reg1.compress(*t)
 
             for i, t in enumerate(zip(apris, start_ns, lengths)):
 
                 reg1.decompress(*t)
@@ -3128,32 +3422,35 @@
                 self._is_not_compressed_helper(reg1, *t)
 
                 for _t in zip(apris[i+1:], start_ns[i+1:], lengths[i+1:], data_files_bytes[i+1:]):
 
                     self._is_compressed_helper(reg1, *_t)
 
                 expected = str(t[0]).replace("(", "\\(").replace(")", "\\)") + f".*startn.*0.*length.*{t[2]}"
+
                 with self.assertRaisesRegex(DecompressionError, expected):
                     reg1.decompress(*t)
 
         with self.assertRaisesRegex(RegisterError, "read-only"):
 
             with reg1.open(readonly= True) as reg1:
                 reg1.decompress(apri1)
 
-        reg2 = NumpyRegister(SAVES_DIR, "hi")
+        reg2 = NumpyRegister(SAVES_DIR, "sh", "hi")
 
         with reg2.open() as reg2:
 
             apri = ApriInfo(hi ="hello")
             blk1 = Block(np.arange(15), apri)
             blk2 = Block(np.arange(15, 30), apri, 15)
 
-            reg2.add_disk_blk(blk1)
-            reg2.add_disk_blk(blk2)
+            with open_blks(blk1, blk2):
+
+                reg2.add_disk_blk(blk1)
+                reg2.add_disk_blk(blk2)
 
             reg2.compress(apri, 0, 15)
             reg2.compress(apri, 15, 15)
 
             for debug in [1, 2, 3, 4]:
 
                 cornifer.registers._debug = debug
@@ -3307,15 +3604,15 @@
     #
     #         self._is_not_compressed_helper(reg, apri1, 0, 10000)
     #         self._is_not_compressed_helper(reg, apri1, 0, 1000)
     #         self._is_not_compressed_helper(reg, apri1, 42069, 30000)
 
     def test_change_apri_info(self):
 
-        reg = Testy_Register(SAVES_DIR, "msg")
+        reg = Testy_Register(SAVES_DIR, "sh",  "msg")
 
         with self.assertRaisesRegex(RegisterError, "open.*change_apri"):
             reg.change_apri(ApriInfo(i = 0), ApriInfo(j=0))
 
         with reg.open() as reg:
 
             old_apri = ApriInfo(sup ="hey")
@@ -3362,15 +3659,15 @@
                 reg
             )
 
         with reg.open(readonly= True) as reg:
             with self.assertRaisesRegex(RegisterError, "read-write"):
                 reg.change_apri(old_apri, new_apri)
 
-        reg = NumpyRegister(SAVES_DIR, "hello")
+        reg = NumpyRegister(SAVES_DIR, "sh", "hello")
 
         with reg.open() as reg:
 
             old_apri = ApriInfo(sup ="hey")
             other_apri = ApriInfo(sir ="maam", respective = old_apri)
             new_apri = ApriInfo(hello ="hi")
             new_other_apri = ApriInfo(respective = new_apri, sir ="maam")
@@ -3513,15 +3810,17 @@
                 lmdb_count_keys(reg._db, _ID_APRI_KEY_PREFIX)
             )
 
 
             # change to an info that already exists in the register
 
             blk = Block(np.arange(100), other_apri)
-            reg.add_disk_blk(blk)
+
+            with blk:
+                reg.add_disk_blk(blk)
 
             reg.change_apri(old_apri, other_apri)
 
             other_other_apri = ApriInfo(sir ="maam", respective = other_apri)
 
             with self.assertRaisesRegex(DataNotFoundError, r"AposInfo.*" + re.escape(str(old_apri))):
                 reg.apos(old_apri)
@@ -3538,18 +3837,21 @@
             )
 
             self.assertEqual(
                 apos2,
                 reg.apos(other_other_apri)
             )
 
-            self.assertEqual(
-                Block(np.arange(100), other_other_apri),
-                reg.blk(other_other_apri)
-            )
+            with reg.blk(other_other_apri) as blk:
+
+                with Block(np.arange(100), other_other_apri) as blk_:
+                    self.assertEqual(
+                        blk_,
+                        blk
+                    )
 
             self.assertIn(
                 other_apri,
                 reg
             )
 
             self.assertIn(
@@ -3600,23 +3902,25 @@
             )
 
             # change to an info that creates duplicate keys
 
             with self.assertRaisesRegex(ValueError, "[dD]uplicate"):
                 reg.change_apri(other_other_apri, other_apri)
 
-        reg = NumpyRegister(SAVES_DIR, "hello")
+        reg = NumpyRegister(SAVES_DIR, "sh", "hello")
 
         with reg.open() as reg:
 
             apri1 = ApriInfo(hi ="hello")
             apri2 = ApriInfo(num = 7, respective = apri1)
 
             reg.set_apos(apri1, AposInfo(no ="yes"))
-            reg.add_disk_blk(Block(np.arange(10), apri2))
+
+            with Block(np.arange(10), apri2) as blk:
+                reg.add_disk_blk(blk)
 
             for debug in [1,2,3]:
 
                 cornifer.registers._debug = debug
 
                 with self.assertRaises(KeyboardInterrupt):
                     reg.change_apri(apri1, ApriInfo(sup ="hey"), False)
@@ -3624,18 +3928,19 @@
                 cornifer.registers._debug = _NO_DEBUG
 
                 self.assertEqual(
                     AposInfo(no ="yes"),
                     reg.apos(ApriInfo(hi ="hello"))
                 )
 
-                self.assertTrue(np.all(
-                    np.arange(10) ==
-                    reg.blk(ApriInfo(num=7, respective=ApriInfo(hi="hello")), 0, 10).segment()
-                ))
+                with reg.blk(ApriInfo(num=7, respective=ApriInfo(hi="hello")), 0, 10) as blk:
+                    self.assertTrue(np.all(
+                        np.arange(10) ==
+                        blk.segment()
+                    ))
 
                 self.assertIn(
                     ApriInfo(hi ="hello"),
                     reg
                 )
 
                 self.assertIn(
@@ -3678,37 +3983,37 @@
                 self.assertEqual(
                     2,
                     lmdb_count_keys(reg._db, _ID_APRI_KEY_PREFIX)
                 )
 
     def test_concatenate_disk_blocks(self):
 
-        reg = NumpyRegister(SAVES_DIR, "hello")
+        reg = NumpyRegister(SAVES_DIR, "sh", "hello")
 
         with self.assertRaisesRegex(RegisterError, "open.*concat_disk_blks"):
             reg.concat_disk_blks(ApriInfo(_ ="_"), 0, 0)
 
         with reg.open() as reg:
 
             apri = ApriInfo(hi ="hello")
-
             blk1 = Block(np.arange(100), apri)
             blk2 = Block(np.arange(100, 200), apri, 100)
 
-            reg.add_disk_blk(blk1)
-            reg.add_disk_blk(blk2)
+            with open_blks(blk1, blk2):
+
+                reg.add_disk_blk(blk1)
+                reg.add_disk_blk(blk2)
 
             with self.assertRaisesRegex(ValueError, "right size"):
                 reg.concat_disk_blks(apri, 0, 150, True)
 
             self.assertEqual(
                 2,
                 lmdb_count_keys(reg._db, _BLK_KEY_PREFIX)
             )
-
             self.assertEqual(
                 2,
                 lmdb_count_keys(reg._db, _COMPRESSED_KEY_PREFIX)
             )
 
             with self.assertRaisesRegex(ValueError, "right size"):
                 reg.concat_disk_blks(apri, 1, 200)
@@ -3716,15 +4021,14 @@
             with self.assertRaisesRegex(ValueError, "right size"):
                 reg.concat_disk_blks(apri, 0, 199)
 
             self.assertEqual(
                 2,
                 lmdb_count_keys(reg._db, _BLK_KEY_PREFIX)
             )
-
             self.assertEqual(
                 2,
                 lmdb_count_keys(reg._db, _COMPRESSED_KEY_PREFIX)
             )
 
             try:
                 reg.concat_disk_blks(apri, 0, 200, True)
@@ -3732,280 +4036,390 @@
             except:
                 self.fail("concat_disk_blks call should have succeeded")
 
             self.assertEqual(
                 1,
                 lmdb_count_keys(reg._db, _BLK_KEY_PREFIX)
             )
-
             self.assertEqual(
                 1,
                 lmdb_count_keys(reg._db, _COMPRESSED_KEY_PREFIX)
             )
 
-            self.assertEqual(
-                Block(np.arange(200), apri),
-                reg.blk(apri, 0, 200)
-            )
+            with reg.blk(apri, 0, 200) as blk:
 
-            self.assertEqual(
-                Block(np.arange(200), apri),
-                reg.blk(apri)
-            )
+                self.assertEqual(
+                    0,
+                    blk.startn()
+                )
+                self.assertTrue(np.all(
+                    blk.segment() ==
+                    np.arange(200)
+                ))
+
+            with reg.blk(apri) as blk:
+
+                self.assertEqual(
+                    0,
+                    blk.startn()
+                )
+                self.assertTrue(np.all(
+                    blk.segment() ==
+                    np.arange(200)
+                ))
 
             try:
                 # this shouldn't do anything
                 reg.concat_disk_blks(apri)
 
             except Exception as e:
                 self.fail("combine call should have worked.")
 
             self.assertEqual(
                 1,
                 lmdb_count_keys(reg._db, _BLK_KEY_PREFIX)
             )
-
             self.assertEqual(
                 1,
                 lmdb_count_keys(reg._db, _COMPRESSED_KEY_PREFIX)
             )
 
-            self.assertEqual(
-                Block(np.arange(200), apri),
-                reg.blk(apri, 0, 200)
-            )
+            with reg.blk(apri, 0, 200) as blk:
 
-            self.assertEqual(
-                Block(np.arange(200), apri),
-                reg.blk(apri)
-            )
+                self.assertEqual(
+                    0,
+                    blk.startn()
+                )
+                self.assertTrue(np.all(
+                    blk.segment() ==
+                    np.arange(200)
+                ))
 
-            blk3 = Block(np.arange(200, 4000), apri, 200)
+            with reg.blk(apri) as blk:
+
+                self.assertEqual(
+                    0,
+                    blk.startn()
+                )
+                self.assertTrue(np.all(
+                    blk.segment() ==
+                    np.arange(200)
+                ))
 
-            reg.add_disk_blk(blk3)
+            with Block(np.arange(200, 4000), apri, 200) as blk3:
+                reg.add_disk_blk(blk3)
 
             reg.concat_disk_blks(apri, delete = True)
-
             self.assertEqual(
                 1,
                 lmdb_count_keys(reg._db, _BLK_KEY_PREFIX)
             )
-
             self.assertEqual(
                 1,
                 lmdb_count_keys(reg._db, _COMPRESSED_KEY_PREFIX)
             )
 
-            self.assertEqual(
-                Block(np.arange(4000), apri),
-                reg.blk(apri, 0, 4000)
-            )
+            with reg.blk(apri, 0, 4000) as blk:
 
-            self.assertEqual(
-                Block(np.arange(4000), apri),
-                reg.blk(apri)
-            )
+                self.assertEqual(
+                    0,
+                    blk.startn()
+                )
+                self.assertTrue(np.all(
+                    blk.segment() ==
+                    np.arange(4000)
+                ))
 
-            blk4 = Block(np.arange(4001, 4005), apri, 4001)
+            with reg.blk(apri) as blk:
 
-            reg.add_disk_blk(blk4)
+                self.assertEqual(
+                    0,
+                    blk.startn()
+                )
+                self.assertTrue(np.all(
+                    blk.segment() ==
+                    np.arange(4000)
+                ))
 
+            with Block(np.arange(4001, 4005), apri, 4001) as blk4:
+                reg.add_disk_blk(blk4)
             # this shouldn't do anything
             reg.concat_disk_blks(apri)
-
             self.assertEqual(
                 2,
                 lmdb_count_keys(reg._db, _BLK_KEY_PREFIX)
             )
-
             self.assertEqual(
                 2,
                 lmdb_count_keys(reg._db, _COMPRESSED_KEY_PREFIX)
             )
 
-            self.assertEqual(
-                Block(np.arange(4000), apri),
-                reg.blk(apri, 0, 4000)
-            )
+            with reg.blk(apri, 0, 4000) as blk:
 
-            self.assertEqual(
-                Block(np.arange(4000), apri),
-                reg.blk(apri)
-            )
+                self.assertEqual(
+                    0,
+                    blk.startn()
+                )
+                self.assertTrue(np.all(
+                    blk.segment() ==
+                    np.arange(4000)
+                ))
+
+            with reg.blk(apri) as blk:
+
+                self.assertEqual(
+                    0,
+                    blk.startn()
+                )
+                self.assertTrue(np.all(
+                    blk.segment() ==
+                    np.arange(4000)
+                ))
 
             with self.assertRaisesRegex(DataNotFoundError, "4000"):
                 reg.concat_disk_blks(apri, 0, 4001)
 
             with self.assertRaisesRegex(DataNotFoundError, "4000.*4000"):
                 reg.concat_disk_blks(apri, 0, 4005)
 
-            blk5 = Block(np.arange(3999, 4001), apri, 3999)
-
-            reg.add_disk_blk(blk5)
+            with Block(np.arange(3999, 4001), apri, 3999) as blk5:
+                reg.add_disk_blk(blk5)
 
             with self.assertRaisesRegex(ValueError, "[oO]verlap"):
                 reg.concat_disk_blks(apri, 0, 4001)
 
             blk6 = Block(np.arange(4005, 4100), apri, 4005)
             blk7 = Block(np.arange(4100, 4200), apri, 4100)
             blk8 = Block(np.arange(4200, 4201), apri, 4200)
 
-            reg.add_disk_blk(blk6)
-            reg.add_disk_blk(blk7)
-            reg.add_disk_blk(blk8)
+            with open_blks(blk6, blk7, blk8):
+
+                reg.add_disk_blk(blk6)
+                reg.add_disk_blk(blk7)
+                reg.add_disk_blk(blk8)
 
             reg.concat_disk_blks(apri, 4005, delete = True)
 
             self.assertEqual(
                 4,
                 lmdb_count_keys(reg._db, _BLK_KEY_PREFIX)
             )
 
             self.assertEqual(
                 4,
                 lmdb_count_keys(reg._db, _COMPRESSED_KEY_PREFIX)
             )
 
-            self.assertEqual(
-                Block(np.arange(4005, 4201), apri, 4005),
-                reg.blk(apri, 4005, 4201 - 4005)
-            )
+            with reg.blk(apri, 4005, 4201 - 4005) as blk:
 
-            self.assertEqual(
-                Block(np.arange(4005, 4201), apri, 4005),
-                reg.blk(apri, 4005)
-            )
+                self.assertEqual(
+                    4005,
+                    blk.startn()
+                )
+                self.assertTrue(np.all(
+                    blk.segment() ==
+                    np.arange(4005, 4201)
+                ))
 
-            self.assertEqual(
-                Block(np.arange(4000), apri),
-                reg.blk(apri)
-            )
+            with reg.blk(apri, 4005) as blk:
+
+                self.assertEqual(
+                    4005,
+                    blk.startn()
+                )
+                self.assertTrue(np.all(
+                    blk.segment() ==
+                    np.arange(4005, 4201)
+                ))
 
-            blk9 = Block(np.arange(4201, 4201), apri, 4201)
-            reg.add_disk_blk(blk9)
+            with reg.blk(apri) as blk:
 
-            reg.concat_disk_blks(apri, 4005, delete = True)
+                self.assertEqual(
+                    0,
+                    blk.startn()
+                )
+                self.assertTrue(np.all(
+                    blk.segment() ==
+                    np.arange(4000)
+                ))
 
+            with Block(np.arange(4201, 4201), apri, 4201) as blk9:
+                reg.add_disk_blk(blk9)
+
+            reg.concat_disk_blks(apri, 4005, delete = True)
             self.assertEqual(
                 5,
                 lmdb_count_keys(reg._db, _BLK_KEY_PREFIX)
             )
-
             self.assertEqual(
                 5,
                 lmdb_count_keys(reg._db, _COMPRESSED_KEY_PREFIX)
             )
 
-            self.assertEqual(
-                Block(np.arange(4005, 4201), apri, 4005),
-                reg.blk(apri, 4005, 4201 - 4005)
-            )
+            with reg.blk(apri, 4005, 4201 - 4005) as blk:
 
-            self.assertEqual(
-                Block(np.arange(4005, 4201), apri, 4005),
-                reg.blk(apri, 4005)
-            )
+                self.assertEqual(
+                    4005,
+                    blk.startn()
+                )
+                self.assertTrue(np.all(
+                    blk.segment() ==
+                    np.arange(4005, 4201)
+                ))
 
-            self.assertEqual(
-                Block(np.arange(4000), apri),
-                reg.blk(apri)
-            )
+            with reg.blk(apri, 4005) as blk:
 
-            self.assertEqual(
-                Block(np.arange(4201, 4201), apri, 4201),
-                reg.blk(apri, 4201, 0)
-            )
+                self.assertEqual(
+                    4005,
+                    blk.startn()
+                )
+                self.assertTrue(np.all(
+                    blk.segment() ==
+                    np.arange(4005, 4201)
+                ))
 
-            blk10 = Block(np.arange(0, 0), apri, 0)
-            reg.add_disk_blk(blk10)
+            with reg.blk(apri) as blk:
 
-            reg.rmv_disk_blk(apri, 3999, 2)
+                self.assertEqual(
+                    0,
+                    blk.startn()
+                )
+                self.assertTrue(np.all(
+                    blk.segment() ==
+                    np.arange(4000)
+                ))
 
-            reg.concat_disk_blks(apri, delete = True)
+            with reg.blk(apri, 4201, 0) as blk:
+
+                self.assertEqual(
+                    4201,
+                    blk.startn()
+                )
+                self.assertTrue(np.all(
+                    blk.segment() ==
+                    np.arange(4201, 4201)
+                ))
 
+            with Block(np.arange(0, 0), apri, 0) as blk10:
+                reg.add_disk_blk(blk10)
+
+            reg.rmv_disk_blk(apri, 3999, 2)
+            reg.concat_disk_blks(apri, delete = True)
             self.assertEqual(
                 5,
                 lmdb_count_keys(reg._db, _BLK_KEY_PREFIX)
             )
-
             self.assertEqual(
                 5,
                 lmdb_count_keys(reg._db, _COMPRESSED_KEY_PREFIX)
             )
 
-            self.assertEqual(
-                Block(np.arange(4005, 4201), apri, 4005),
-                reg.blk(apri, 4005, 4201 - 4005)
-            )
+            with reg.blk(apri, 4005, 4201 - 4005) as blk:
 
-            self.assertEqual(
-                Block(np.arange(4005, 4201), apri, 4005),
-                reg.blk(apri, 4005)
-            )
+                self.assertEqual(
+                    4005,
+                    blk.startn()
+                )
+                self.assertTrue(np.all(
+                    blk.segment() ==
+                    np.arange(4005, 4201)
+                ))
 
-            self.assertEqual(
-                Block(np.arange(4000), apri),
-                reg.blk(apri)
-            )
+            with reg.blk(apri, 4005) as blk:
 
-            self.assertEqual(
-                Block(np.arange(4201, 4201), apri, 4201),
-                reg.blk(apri, 4201, 0)
-            )
+                self.assertEqual(
+                    4005,
+                    blk.startn()
+                )
+                self.assertTrue(np.all(
+                    blk.segment() ==
+                    np.arange(4005, 4201)
+                ))
 
-            self.assertEqual(
-                Block(np.arange(0, 0), apri, 0),
-                reg.blk(apri, 0, 0)
-            )
+            with reg.blk(apri) as blk:
+
+                self.assertEqual(
+                    0,
+                    blk.startn()
+                )
+                self.assertTrue(np.all(
+                    blk.segment() ==
+                    np.arange(4000)
+                ))
+
+            with reg.blk(apri, 4201, 0) as blk:
+
+                self.assertEqual(
+                    4201,
+                    blk.startn()
+                )
+                self.assertTrue(np.all(
+                    blk.segment() ==
+                    np.arange(4201, 4201)
+                ))
 
+            with reg.blk(apri, 0, 0) as blk:
+
+                self.assertEqual(
+                    0,
+                    blk.startn()
+                )
+                self.assertTrue(np.all(
+                    blk.segment() ==
+                    np.arange(0, 0)
+                ))
 
         with reg.open(readonly= True) as reg:
             with self.assertRaisesRegex(RegisterError, "[rR]ead-write"):
                 reg.concat_disk_blks(ApriInfo(_="_"), 0, 0)
 
     def _composite_helper(self, reg, block_datas, apris):
 
         with reg._db.begin() as txn:
 
             # check blocks
             for data, (seg, compressed) in block_datas.items():
 
-                try:
-                    filename = (txn
-                                .get(reg._get_disk_blk_key(_BLK_KEY_PREFIX, data[0], None, data[1], data[2], False))
-                                .decode("ASCII")
-                    )
-                except:
-                    raise
-
+                filename = (txn
+                            .get(reg._get_disk_blk_key(_BLK_KEY_PREFIX, data[0], None, data[1], data[2], False))
+                            .decode("ASCII")
+                )
                 filename = reg._local_dir / filename
-
                 self.assertTrue(filename.is_file())
-
                 val = txn.get(reg._get_disk_blk_key(_COMPRESSED_KEY_PREFIX, data[0], None, data[1], data[2], False))
-
                 self.assertEqual(
                     compressed,
                     val != _IS_NOT_COMPRESSED_VAL
                 )
 
                 if val == _IS_NOT_COMPRESSED_VAL:
 
-                    self.assertEqual(
-                        Block(seg, *data[:2]),
-                        reg.blk(*data)
-                    )
+                    with reg.blk(*data) as blk:
+
+                        self.assertEqual(
+                            blk.apri(),
+                            data[0]
+                        )
+                        self.assertEqual(
+                            blk.startn(),
+                            data[1]
+                        )
+                        self.assertTrue(np.all(
+                            blk.segment() ==
+                            seg
+                        ))
 
                 else:
 
                     with self.assertRaises(CompressionError):
-                        reg.blk(*data)
 
-                    filename = reg._local_dir / val.decode("ASCII")
+                        with reg.blk(*data) as blk:
+                            pass
 
+                    filename = reg._local_dir / val.decode("ASCII")
                     self.assertTrue(filename.is_file())
 
             self.assertEqual(
                 len(block_datas),
                 lmdb_count_keys(txn, _BLK_KEY_PREFIX)
             )
 
@@ -4017,15 +4431,14 @@
         for apri in apris:
 
             self.assertEqual(
                 sum(_apri == apri for _apri,_,_ in block_datas),
                 reg.num_blks(apri)
             )
 
-
         # check info
         all_apri = reg.apris()
 
         for apri in apris:
 
             self.assertIn(
                 apri, reg
@@ -4084,51 +4497,57 @@
         # combine disk blocks
         # increase register size
         # change info info back
 
         block_datas = {}
         apris = []
 
-        reg = NumpyRegister(SAVES_DIR, "hello")
+        reg = NumpyRegister(SAVES_DIR, "sh", "hello")
 
         with reg.open() as reg:
 
             inner_apri = ApriInfo(descr ="\\\\hello", num = 7)
             apri = ApriInfo(descr ="\\'hi\"", respective = inner_apri)
             apris.append(inner_apri)
             apris.append(apri)
             seg = np.arange(69, 420)
             blk = Block(seg, apri, 1337)
-            reg.add_disk_blk(blk)
+
+            with blk:
+                reg.add_disk_blk(blk)
+
             block_datas[data(blk)] = [seg, False]
 
             self._composite_helper(reg, block_datas, apris)
 
             seg = np.arange(69, 69)
             blk = Block(seg, apri, 1337)
-            reg.add_disk_blk(blk)
-            block_datas[data(blk)] = [seg, False]
 
-            self._composite_helper(reg, block_datas, apris)
+            with blk:
+                reg.add_disk_blk(blk)
 
-            apri = ApriInfo(descr ="Apri_Info.fromJson(hi = \"lol\")", respective = inner_apri)
+            block_datas[data(blk)] = [seg, False]
+            self._composite_helper(reg, block_datas, apris)
+            apri = ApriInfo(descr ="ApriInfo.from_json(hi = \"lol\")", respective = inner_apri)
             apris.append(apri)
             seg = np.arange(69., 420.)
             blk = Block(seg, apri, 1337)
-            reg.add_disk_blk(blk)
-            block_datas[data(blk)] = [seg, False]
 
+            with blk:
+                reg.add_disk_blk(blk)
+
+            block_datas[data(blk)] = [seg, False]
             self._composite_helper(reg, block_datas, apris)
 
             for start_n, length in reg.intervals(
-                    ApriInfo(descr="Apri_Info.fromJson(hi = \"lol\")", respective=inner_apri)):
-                reg.compress(ApriInfo(descr ="Apri_Info.fromJson(hi = \"lol\")", respective = inner_apri), start_n, length)
+                    ApriInfo(descr="ApriInfo.from_json(hi = \"lol\")", respective=inner_apri)):
+                reg.compress(ApriInfo(descr ="ApriInfo.from_json(hi = \"lol\")", respective = inner_apri), start_n, length)
 
             _set_block_datas_compressed(block_datas,
-                ApriInfo(descr ="Apri_Info.fromJson(hi = \"lol\")", respective = inner_apri)
+                ApriInfo(descr ="ApriInfo.from_json(hi = \"lol\")", respective = inner_apri)
             )
 
             self._composite_helper(reg, block_datas, apris)
 
             for start_n, length in reg.intervals(ApriInfo(descr="\\'hi\"", respective=inner_apri)):
                 reg.compress(ApriInfo(descr ="\\'hi\"", respective = inner_apri), start_n, length)
 
@@ -4163,56 +4582,59 @@
 
             self._composite_helper(reg, block_datas, apris)
 
             with self.assertRaises(ValueError):
                 reg.rmv_apri(inner_apri)
 
             reg.decompress(
-                ApriInfo(descr ="Apri_Info.fromJson(hi = \"lol\")", respective = inner_apri),
+                ApriInfo(descr ="ApriInfo.from_json(hi = \"lol\")", respective = inner_apri),
                 1337,
                 420 - 69
             )
 
             _set_block_datas_compressed(
                 block_datas,
-                ApriInfo(descr ="Apri_Info.fromJson(hi = \"lol\")", respective = inner_apri),
+                ApriInfo(descr ="ApriInfo.from_json(hi = \"lol\")", respective = inner_apri),
                 compressed = False
             )
 
             self._composite_helper(reg, block_datas, apris)
 
             new_message = "\\\\new msg\"\"\\'"
             reg.set_msg(new_message)
 
             self.assertEqual(
-                new_message,
-                str(reg)
+                str(reg),
+                f'sh ({reg._local_dir}): "\\\\new msg""\\\'"'
             )
 
         self.assertEqual(
-            new_message,
-            str(reg)
+            str(reg),
+            f'sh ({reg._local_dir}): "\\\\new msg""\\\'"'
         )
 
         reg = load(reg._local_dir)
 
         with reg.open() as reg:
 
             inner_inner_apri = ApriInfo(inner_apri = inner_apri)
-            apri = ApriInfo(inner_apri = inner_inner_apri, love ="Apos_Info(num = 6)")
+            apri = ApriInfo(inner_apri = inner_inner_apri, love ="AposInfo(num = 6)")
             apris.append(apri)
             apris.append(inner_inner_apri)
 
             datas = [(10, 34), (10 + 34, 8832), (10 + 34 + 8832, 0), (10 + 34 + 8832, 54), (10 + 34 + 8832 + 54, 0)]
 
             for start_n, length in datas:
 
                 seg = np.arange(length, 2 * length)
                 blk = Block(seg, apri, start_n)
-                reg.add_disk_blk(blk)
+
+                with blk:
+                    reg.add_disk_blk(blk)
+
                 block_datas[data(blk)] = [seg, False]
 
                 self._composite_helper(reg, block_datas, apris)
 
             with self.assertRaisesRegex(ValueError, re.escape(str(apri))):
                 reg.rmv_apri(inner_inner_apri)
 
@@ -4252,45 +4674,52 @@
 
             start_n = 10 ** 17
 
             for i in range(5):
 
                 apri = ApriInfo(longg ="boi")
                 blk = Block(np.arange(start_n + i*1000, start_n + (i+1)*1000, dtype = np.int64), apri, start_n + i*1000)
-                reg.add_disk_blk(blk)
+
+                with blk:
+                    reg.add_disk_blk(blk)
 
             with self.assertRaisesRegex(IndexError, "head"):
-                reg.add_disk_blk(Block([], apri))
+
+                with Block([], apri) as blk:
+                    reg.add_disk_blk(blk)
 
             for start_n, length in reg.intervals(apri):
                 reg.rmv_disk_blk(apri, start_n, length)
 
             reg.set_startn_info()
-
             reg.increase_reg_size(reg.reg_size() + 1)
 
             with self.assertRaises(ValueError):
                 reg.increase_reg_size(reg.reg_size() - 1)
 
     def test_remove_apri_info(self):
 
-        reg = NumpyRegister(SAVES_DIR, "sup")
+        reg = NumpyRegister(SAVES_DIR, "sh", "sup")
 
         with self.assertRaisesRegex(RegisterError, "open.*rmv_apri"):
             reg.rmv_apri(ApriInfo(no ="yes"))
 
         with reg.open() as reg:
 
             apri1 = ApriInfo(hello ="hi")
             apri2 = ApriInfo(sup ="hey")
             apri3 = ApriInfo(respective = apri1)
 
-            reg.add_disk_blk(Block(np.arange(15), apri1))
+            with Block(np.arange(15), apri1) as blk:
+                reg.add_disk_blk(blk)
+
             reg.set_apos(apri2, AposInfo(num = 7))
-            reg.add_disk_blk(Block(np.arange(15, 30), apri3, 15))
+
+            with Block(np.arange(15, 30), apri3, 15) as blk:
+                reg.add_disk_blk(blk)
 
             for i in [1,2,3]:
 
                 apri = eval(f"apri{i}")
 
                 with self.assertRaises(ValueError):
                     reg.rmv_apri(apri)
@@ -4322,18 +4751,15 @@
                     )
 
                     self.assertIn(
                         _apri,
                         get
                     )
 
-            try:
-                reg.rmv_disk_blk(apri1, 0, 15)
-            except DataNotFoundError:
-                raise
+            reg.rmv_disk_blk(apri1, 0, 15)
 
             for i in [1,2,3]:
 
                 apri = eval(f"apri{i}")
 
                 with self.assertRaises(ValueError):
                     reg.rmv_apri(apri)
```

