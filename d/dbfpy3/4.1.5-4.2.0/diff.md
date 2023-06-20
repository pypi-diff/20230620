# Comparing `tmp/dbfpy3-4.1.5.tar.gz` & `tmp/dbfpy3-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbfpy3-4.1.5.tar", last modified: Fri Jan 15 15:16:39 2021, max compression
+gzip compressed data, was "dbfpy3-4.2.0.tar", last modified: Tue Jun 20 15:08:47 2023, max compression
```

## Comparing `dbfpy3-4.1.5.tar` & `dbfpy3-4.2.0.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 15:16:39.233495 dbfpy3-4.1.5/
--rw-r--r--   0 runner    (1001) docker     (116)     3515 2021-01-15 15:16:36.000000 dbfpy3-4.1.5/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (116)       89 2021-01-15 15:16:36.000000 dbfpy3-4.1.5/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1067 2021-01-15 15:16:36.000000 dbfpy3-4.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      242 2021-01-15 15:16:36.000000 dbfpy3-4.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     1996 2021-01-15 15:16:39.233495 dbfpy3-4.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      568 2021-01-15 15:16:36.000000 dbfpy3-4.1.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 15:16:39.229495 dbfpy3-4.1.5/dbfpy3/
--rw-r--r--   0 runner    (1001) docker     (116)      200 2021-01-15 15:16:36.000000 dbfpy3-4.1.5/dbfpy3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3917 2021-01-15 15:16:36.000000 dbfpy3-4.1.5/dbfpy3/code_page.py
--rw-r--r--   0 runner    (1001) docker     (116)     7842 2021-01-15 15:16:36.000000 dbfpy3-4.1.5/dbfpy3/dbf.py
--rw-r--r--   0 runner    (1001) docker     (116)       19 2021-01-15 15:16:36.000000 dbfpy3-4.1.5/dbfpy3/dbfpy3.py
--rw-r--r--   0 runner    (1001) docker     (116)    15383 2021-01-15 15:16:36.000000 dbfpy3-4.1.5/dbfpy3/fields.py
--rw-r--r--   0 runner    (1001) docker     (116)    12528 2021-01-15 15:16:36.000000 dbfpy3-4.1.5/dbfpy3/header.py
--rw-r--r--   0 runner    (1001) docker     (116)     5462 2021-01-15 15:16:36.000000 dbfpy3-4.1.5/dbfpy3/memo.py
--rw-r--r--   0 runner    (1001) docker     (116)     5722 2021-01-15 15:16:36.000000 dbfpy3-4.1.5/dbfpy3/record.py
--rw-r--r--   0 runner    (1001) docker     (116)     4766 2021-01-15 15:16:36.000000 dbfpy3-4.1.5/dbfpy3/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 15:16:39.229495 dbfpy3-4.1.5/dbfpy3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     1996 2021-01-15 15:16:39.000000 dbfpy3-4.1.5/dbfpy3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      624 2021-01-15 15:16:39.000000 dbfpy3-4.1.5/dbfpy3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-15 15:16:39.000000 dbfpy3-4.1.5/dbfpy3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-15 15:16:39.000000 dbfpy3-4.1.5/dbfpy3.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)        7 2021-01-15 15:16:39.000000 dbfpy3-4.1.5/dbfpy3.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 15:16:39.233495 dbfpy3-4.1.5/docs/
--rw-r--r--   0 runner    (1001) docker     (116)      607 2021-01-15 15:16:36.000000 dbfpy3-4.1.5/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (116)     4753 2021-01-15 15:16:36.000000 dbfpy3-4.1.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (116)       33 2021-01-15 15:16:36.000000 dbfpy3-4.1.5/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (116)       28 2021-01-15 15:16:36.000000 dbfpy3-4.1.5/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (116)      292 2021-01-15 15:16:36.000000 dbfpy3-4.1.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1110 2021-01-15 15:16:36.000000 dbfpy3-4.1.5/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (116)      768 2021-01-15 15:16:36.000000 dbfpy3-4.1.5/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (116)       27 2021-01-15 15:16:36.000000 dbfpy3-4.1.5/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (116)       67 2021-01-15 15:16:36.000000 dbfpy3-4.1.5/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (116)      389 2021-01-15 15:16:39.233495 dbfpy3-4.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1570 2021-01-15 15:16:36.000000 dbfpy3-4.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 15:16:39.233495 dbfpy3-4.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (116)       36 2021-01-15 15:16:36.000000 dbfpy3-4.1.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      205 2021-01-15 15:16:36.000000 dbfpy3-4.1.5/tests/env.py
--rw-r--r--   0 runner    (1001) docker     (116)     1036 2021-01-15 15:16:36.000000 dbfpy3-4.1.5/tests/test_code_page.py
--rw-r--r--   0 runner    (1001) docker     (116)      382 2021-01-15 15:16:36.000000 dbfpy3-4.1.5/tests/test_dbfpy3.py
--rw-r--r--   0 runner    (1001) docker     (116)     6512 2021-01-15 15:16:36.000000 dbfpy3-4.1.5/tests/test_fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:08:47.585961 dbfpy3-4.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-06-20 15:08:43.000000 dbfpy3-4.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-20 15:08:43.000000 dbfpy3-4.2.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-20 15:08:43.000000 dbfpy3-4.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-20 15:08:43.000000 dbfpy3-4.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-20 15:08:47.585961 dbfpy3-4.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-20 15:08:43.000000 dbfpy3-4.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:08:47.585961 dbfpy3-4.2.0/dbfpy3/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-20 15:08:43.000000 dbfpy3-4.2.0/dbfpy3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-06-20 15:08:43.000000 dbfpy3-4.2.0/dbfpy3/code_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7842 2023-06-20 15:08:43.000000 dbfpy3-4.2.0/dbfpy3/dbf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-20 15:08:43.000000 dbfpy3-4.2.0/dbfpy3/dbfpy3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-06-20 15:08:43.000000 dbfpy3-4.2.0/dbfpy3/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12528 2023-06-20 15:08:43.000000 dbfpy3-4.2.0/dbfpy3/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-06-20 15:08:43.000000 dbfpy3-4.2.0/dbfpy3/memo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-06-20 15:08:43.000000 dbfpy3-4.2.0/dbfpy3/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-06-20 15:08:43.000000 dbfpy3-4.2.0/dbfpy3/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:08:47.585961 dbfpy3-4.2.0/dbfpy3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-20 15:08:47.000000 dbfpy3-4.2.0/dbfpy3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-20 15:08:47.000000 dbfpy3-4.2.0/dbfpy3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:08:47.000000 dbfpy3-4.2.0/dbfpy3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:08:47.000000 dbfpy3-4.2.0/dbfpy3.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 15:08:47.000000 dbfpy3-4.2.0/dbfpy3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:08:47.585961 dbfpy3-4.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-20 15:08:43.000000 dbfpy3-4.2.0/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4753 2023-06-20 15:08:43.000000 dbfpy3-4.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-20 15:08:43.000000 dbfpy3-4.2.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-20 15:08:43.000000 dbfpy3-4.2.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-20 15:08:43.000000 dbfpy3-4.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-20 15:08:43.000000 dbfpy3-4.2.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-20 15:08:43.000000 dbfpy3-4.2.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-20 15:08:43.000000 dbfpy3-4.2.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-20 15:08:43.000000 dbfpy3-4.2.0/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-20 15:08:47.585961 dbfpy3-4.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-20 15:08:43.000000 dbfpy3-4.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:08:47.585961 dbfpy3-4.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-20 15:08:43.000000 dbfpy3-4.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-20 15:08:43.000000 dbfpy3-4.2.0/tests/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-20 15:08:43.000000 dbfpy3-4.2.0/tests/test_code_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-20 15:08:43.000000 dbfpy3-4.2.0/tests/test_dbfpy3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-06-20 15:08:43.000000 dbfpy3-4.2.0/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-20 15:08:43.000000 dbfpy3-4.2.0/tests/test_memo.py
```

### Comparing `dbfpy3-4.1.5/CONTRIBUTING.rst` & `dbfpy3-4.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dbfpy3-4.1.5/LICENSE` & `dbfpy3-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbfpy3-4.1.5/PKG-INFO` & `dbfpy3-4.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,74 +1,73 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: dbfpy3
-Version: 4.1.5
-Summary: Port to Python 3 and released at PyPi by Frank Xu.
- dbfpy is a python-only module for reading and writing DBF-files.
- It was created by Jeff Kunce and then modified by Hans Fiby
- and Yaroslav Samchuk.  Dbfpy was ported to Python 3.x by James Douglass. 
+Version: 4.2.0
+Summary: Port to Python 3. Dbfpy is a python-only module for reading and writing DBF-files.
 Home-page: https://github.com/frankyxhl/dbfpy3
 Author: Frank Xu
 Author-email: franky.xhl@gmail.com
 License: MIT license
-Description: Python 3 modules for accessing .dbf files
-        ------------------------------------------
-        
-        Port to Python 3 and released at PyPi by Frank Xu.
-        
-        ### Features
-        
-        * Support FoxPro
-        * Support memo
-        * Code page
-        
-        ### TODO
-        
-        * Write test
-        * dBase compatible
-        
-        ### Install
-        
-        Run `python -m pip install dbfpy3`
-        
-        
-        ---
-        
-        ### NOT FULLY TEST YET
-        
-        ### USE AT YOUR OWN RISK
-        
-        ### NO WARRANTIES WHATSOEVER
-        
-        ---
-        
-        steelywing <https://github.com/steelywing/dbfpy>
-        
-        Jeff Kunce <kuncej@mail.conservation.state.mo.us>
-        
-        http://starship.python.net/crew/jjkunce/
-        
-        Hans Fiby <hans@fiby.at>
-        
-        http://www.fiby.at
-        
-        
-        =======
-        History
-        =======
-        
-        0.1.0 (2020-12-26)
-        ------------------
-        
-        * First release on PyPI.
-        
 Keywords: dbfpy3
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.5
+License-File: LICENSE
+
+Python 3 modules for accessing .dbf files
+------------------------------------------
+
+Port to Python 3 and released at PyPi by Frank Xu.
+
+### Features
+
+* Support FoxPro
+* Support memo
+* Code page
+
+### TODO
+
+* Write test
+* dBase compatible
+
+### Install
+
+Run `pip install dbfpy3`
+
+
+---
+
+### NOT FULLY TEST YET
+
+### USE AT YOUR OWN RISK
+
+### NO WARRANTIES WHATSOEVER
+
+---
+
+steelywing <https://github.com/steelywing/dbfpy>
+
+Jeff Kunce <kuncej@mail.conservation.state.mo.us>
+
+Hans Fiby <hans@fiby.at>
+
+Frank Xu <https://github.com/frankyxhl/dbfpy3>
+
+Zdeněk Böhm <https://github.com/zbohm>
+
+=======
+History
+=======
+
+0.1.0 (2020-12-26)
+------------------
+
+* First release on PyPI.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dbfpy3-4.1.5/README.rst` & `dbfpy3-4.2.0/README.rst`

 * *Files 21% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 ### TODO
 
 * Write test
 * dBase compatible
 
 ### Install
 
-Run `python -m pip install dbfpy3`
+Run `pip install dbfpy3`
 
 
 ---
 
 ### NOT FULLY TEST YET
 
 ### USE AT YOUR OWN RISK
@@ -29,12 +29,12 @@
 
 ---
 
 steelywing <https://github.com/steelywing/dbfpy>
 
 Jeff Kunce <kuncej@mail.conservation.state.mo.us>
 
-http://starship.python.net/crew/jjkunce/
-
 Hans Fiby <hans@fiby.at>
 
-http://www.fiby.at
+Frank Xu <https://github.com/frankyxhl/dbfpy3>
+
+Zdeněk Böhm <https://github.com/zbohm>
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dbfpy3-4.1.5/dbfpy3/code_page.py` & `dbfpy3-4.2.0/dbfpy3/code_page.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,12 +100,12 @@
         for code_page, (encoding, name) in code_pages.items():
             if encoding == target_encoding:
                 self.code_page = code_page
                 break
         else:
             self.code_page = 0
             print("Could not find encodings. Here is list:")
-            for code, (code_page, name) in code_pages:
+            for code, (code_page, name) in code_pages.items():
                 print(hex(code), code_page, name)
 
     def __str__(self):
         return self.encoding
```

### Comparing `dbfpy3-4.1.5/dbfpy3/dbf.py` & `dbfpy3-4.2.0/dbfpy3/dbf.py`

 * *Files identical despite different names*

### Comparing `dbfpy3-4.1.5/dbfpy3/fields.py` & `dbfpy3-4.2.0/dbfpy3/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -412,15 +412,17 @@
         return super().decode(value).decode(encoding)
 
     def encode(self, value, encoding=locale.getpreferredencoding()):
         """Return raw data string encoded from a ``value``.
 
         Note: this is an internal method.
         """
-        return super().encode(value.encode(encoding))
+        if isinstance(value, str):
+            value = value.encode(encoding)
+        return super().encode(value)
 
 
 class DbfPictureField(DbfGeneralField):
     """Definition of the picture field."""
 
     # not implement yet
     type_code = b'P'
```

### Comparing `dbfpy3-4.1.5/dbfpy3/header.py` & `dbfpy3-4.2.0/dbfpy3/header.py`

 * *Files identical despite different names*

### Comparing `dbfpy3-4.1.5/dbfpy3/memo.py` & `dbfpy3-4.2.0/dbfpy3/memo.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,18 +82,18 @@
             # http://msdn.microsoft.com/en-US/library/d6e1ah7y%28v=VS.80%29.aspx
             elif blocksize == 0:
                 self.blocksize = 1
             elif blocksize <= 32:
                 self.blocksize = 512 * blocksize
             else:
                 self.blocksize = blocksize
-            self.tail = 512 / self.blocksize
+            self.tail = 512 // self.blocksize
             self.stream.write(
                 struct.pack(">LHH", self.tail, 0, self.blocksize)
-                + "\0" * 8 + "\x03" + "\0" * 495)
+                + b"\0" * 8 + b"\x03" + b"\0" * 495)
         else:
             (self.tail, _zero, self.blocksize) = struct.unpack(">LHH",
                 self.stream.read(8))
             if not self.is_fpt:
                 # In DBT files, block size is fixed to 512 bytes
                 self.blocksize = 512
```

### Comparing `dbfpy3-4.1.5/dbfpy3/record.py` & `dbfpy3-4.2.0/dbfpy3/record.py`

 * *Files identical despite different names*

### Comparing `dbfpy3-4.1.5/dbfpy3/utils.py` & `dbfpy3-4.2.0/dbfpy3/utils.py`

 * *Files identical despite different names*

### Comparing `dbfpy3-4.1.5/dbfpy3.egg-info/PKG-INFO` & `dbfpy3-4.2.0/dbfpy3.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,74 +1,73 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: dbfpy3
-Version: 4.1.5
-Summary: Port to Python 3 and released at PyPi by Frank Xu.
- dbfpy is a python-only module for reading and writing DBF-files.
- It was created by Jeff Kunce and then modified by Hans Fiby
- and Yaroslav Samchuk.  Dbfpy was ported to Python 3.x by James Douglass. 
+Version: 4.2.0
+Summary: Port to Python 3. Dbfpy is a python-only module for reading and writing DBF-files.
 Home-page: https://github.com/frankyxhl/dbfpy3
 Author: Frank Xu
 Author-email: franky.xhl@gmail.com
 License: MIT license
-Description: Python 3 modules for accessing .dbf files
-        ------------------------------------------
-        
-        Port to Python 3 and released at PyPi by Frank Xu.
-        
-        ### Features
-        
-        * Support FoxPro
-        * Support memo
-        * Code page
-        
-        ### TODO
-        
-        * Write test
-        * dBase compatible
-        
-        ### Install
-        
-        Run `python -m pip install dbfpy3`
-        
-        
-        ---
-        
-        ### NOT FULLY TEST YET
-        
-        ### USE AT YOUR OWN RISK
-        
-        ### NO WARRANTIES WHATSOEVER
-        
-        ---
-        
-        steelywing <https://github.com/steelywing/dbfpy>
-        
-        Jeff Kunce <kuncej@mail.conservation.state.mo.us>
-        
-        http://starship.python.net/crew/jjkunce/
-        
-        Hans Fiby <hans@fiby.at>
-        
-        http://www.fiby.at
-        
-        
-        =======
-        History
-        =======
-        
-        0.1.0 (2020-12-26)
-        ------------------
-        
-        * First release on PyPI.
-        
 Keywords: dbfpy3
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.5
+License-File: LICENSE
+
+Python 3 modules for accessing .dbf files
+------------------------------------------
+
+Port to Python 3 and released at PyPi by Frank Xu.
+
+### Features
+
+* Support FoxPro
+* Support memo
+* Code page
+
+### TODO
+
+* Write test
+* dBase compatible
+
+### Install
+
+Run `pip install dbfpy3`
+
+
+---
+
+### NOT FULLY TEST YET
+
+### USE AT YOUR OWN RISK
+
+### NO WARRANTIES WHATSOEVER
+
+---
+
+steelywing <https://github.com/steelywing/dbfpy>
+
+Jeff Kunce <kuncej@mail.conservation.state.mo.us>
+
+Hans Fiby <hans@fiby.at>
+
+Frank Xu <https://github.com/frankyxhl/dbfpy3>
+
+Zdeněk Böhm <https://github.com/zbohm>
+
+=======
+History
+=======
+
+0.1.0 (2020-12-26)
+------------------
+
+* First release on PyPI.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dbfpy3-4.1.5/dbfpy3.egg-info/SOURCES.txt` & `dbfpy3-4.2.0/dbfpy3.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -28,8 +28,9 @@
 docs/make.bat
 docs/readme.rst
 docs/usage.rst
 tests/__init__.py
 tests/env.py
 tests/test_code_page.py
 tests/test_dbfpy3.py
-tests/test_fields.py
+tests/test_fields.py
+tests/test_memo.py
```

### Comparing `dbfpy3-4.1.5/docs/Makefile` & `dbfpy3-4.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dbfpy3-4.1.5/docs/conf.py` & `dbfpy3-4.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dbfpy3-4.1.5/docs/installation.rst` & `dbfpy3-4.2.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `dbfpy3-4.1.5/docs/make.bat` & `dbfpy3-4.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dbfpy3-4.1.5/setup.py` & `dbfpy3-4.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,24 +25,27 @@
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9'
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
     ],
-    description="Port to Python 3 and released at PyPi by Frank Xu.\n dbfpy is a python-only module for reading and writing DBF-files.\n It was created by Jeff Kunce and then modified by Hans Fiby\n and Yaroslav Samchuk.  Dbfpy was ported to Python 3.x by James Douglass. ",
+    description="Port to Python 3. Dbfpy is a python-only module for reading and writing DBF-files.\n It was created by Jeff Kunce and then modified by Hans Fiby\n and Yaroslav Samchuk.  Dbfpy was ported to Python 3.x by James Douglass and released at PyPi by Frank X and released at PyPi by Frank Xuu.  ",
     install_requires=requirements,
     license="MIT license",
     long_description=readme + '\n\n' + history,
     include_package_data=True,
     keywords='dbfpy3',
     name='dbfpy3',
     packages=find_packages(include=['dbfpy3', 'dbfpy3.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/frankyxhl/dbfpy3',
-    version='4.1.5',
+    version='4.2.0',
     zip_safe=False,
 )
```

### Comparing `dbfpy3-4.1.5/tests/test_code_page.py` & `dbfpy3-4.2.0/tests/test_code_page.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 __author__ = 'Wing'
 
 import locale
 import unittest
-import env
-from dbfpy.code_page import CodePage
+from dbfpy3.code_page import CodePage
 
 
 class CodePageTest(unittest.TestCase):
     def setUp(self):
         self.code_page = CodePage()
 
     def tearDown(self):
```

### Comparing `dbfpy3-4.1.5/tests/test_fields.py` & `dbfpy3-4.2.0/tests/test_fields.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,40 @@
 __author__ = 'Wing'
 
-import unittest
 import struct
-import env
-from dbfpy import fields
+import unittest
+from io import BytesIO
+
+from dbfpy3 import fields
 
 
 # Implement DbfField
 class _DbfField(fields.DbfField):
     type_code = ' '
     fixed_length = 0
     default_value = 0
 
 
 class FieldsTest(unittest.TestCase):
 
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
-
     def test_field_name(self):
         dbf_field = _DbfField(b'NAME')
         self.assertEqual(dbf_field.name, b'NAME')
         dbf_field.name = b'ID'
         self.assertEqual(dbf_field.name, b'ID')
 
     def test_field_name_upper_case(self):
         dbf_field = _DbfField(b'item')
         self.assertEqual(dbf_field.name, b'ITEM')
 
     def test_field_name_max_length(self):
         dbf_field = _DbfField(b'NAME')
-        # max length 10 bytes
-        with self.assertRaises(ValueError):
-            dbf_field.name = b'N' * 11
+        # max length 20 bytes
+        with self.assertRaisesRegex(ValueError, "field name 'b'NNNNNNNNNNNNNNNNNNNNN'' must less than 20 bytes"):
+            dbf_field.name = b'N' * 21
 
     def test_numeric_field(self):
         field = fields.DbfNumericField(b'NUM', 10, decimal_count=2)
         self.assertEqual(field.name, b'NUM')
         self.assertEqual(field.length, 10)
         self.assertEqual(field.decimal_count, 2)
 
@@ -176,9 +171,23 @@
         self.assertEqual(field.to_bytes(), field_string)
 
         # test parse length
         field_string.pop()
         with self.assertRaises(ValueError):
             fields.DbfFields.parse(bytes(field_string))
 
+
+class DbfMemoFieldTest(unittest.TestCase):
+
+    def test_encode_str(self):
+        field = fields.DbfMemoField(b'NAME')
+        field.file = BytesIO()
+        self.assertEqual(field.encode('test'), b'\x04\x00\x00\x00')
+
+    def test_encode_bytes(self):
+        field = fields.DbfMemoField(b'NAME')
+        field.file = BytesIO()
+        self.assertEqual(field.encode(b'test'), b'\x04\x00\x00\x00')
+
+
 if __name__ == '__main__':
     unittest.main()
```

