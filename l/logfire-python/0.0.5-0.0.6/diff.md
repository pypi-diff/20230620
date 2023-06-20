# Comparing `tmp/logfire-python-0.0.5.tar.gz` & `tmp/logfire-python-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logfire-python-0.0.5.tar", last modified: Tue Jun 20 11:54:18 2023, max compression
+gzip compressed data, was "logfire-python-0.0.6.tar", last modified: Tue Jun 20 12:20:07 2023, max compression
```

## Comparing `logfire-python-0.0.5.tar` & `logfire-python-0.0.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 11:54:18.321285 logfire-python-0.0.5/
--rw-rw-rw-   0        0        0      741 2023-04-12 02:48:20.000000 logfire-python-0.0.5/LICENSE.md
--rw-rw-rw-   0        0        0      106 2023-04-12 06:15:33.000000 logfire-python-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     3861 2023-06-20 11:54:18.321285 logfire-python-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2672 2023-04-12 03:58:47.000000 logfire-python-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 11:54:18.305282 logfire-python-0.0.5/logfire/
--rw-rw-rw-   0        0        0      260 2023-04-12 03:28:58.000000 logfire-python-0.0.5/logfire/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 11:54:18.309285 logfire-python-0.0.5/logfire/__pycache__/
--rw-rw-rw-   0        0        0      539 2023-06-20 11:04:18.000000 logfire-python-0.0.5/logfire/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0      406 2023-06-20 11:04:18.000000 logfire-python-0.0.5/logfire/__pycache__/compat.cpython-311.pyc
--rw-rw-rw-   0        0        0     3574 2023-06-20 11:04:18.000000 logfire-python-0.0.5/logfire/__pycache__/flusher.cpython-311.pyc
--rw-rw-rw-   0        0        0     1462 2023-06-20 11:04:18.000000 logfire-python-0.0.5/logfire/__pycache__/formatter.cpython-311.pyc
--rw-rw-rw-   0        0        0     3687 2023-06-20 11:47:36.000000 logfire-python-0.0.5/logfire/__pycache__/frame.cpython-311.pyc
--rw-rw-rw-   0        0        0     3811 2023-06-20 11:04:18.000000 logfire-python-0.0.5/logfire/__pycache__/handler.cpython-311.pyc
--rw-rw-rw-   0        0        0     2627 2023-06-20 11:04:18.000000 logfire-python-0.0.5/logfire/__pycache__/helpers.cpython-311.pyc
--rw-rw-rw-   0        0        0     1367 2023-06-20 11:04:18.000000 logfire-python-0.0.5/logfire/__pycache__/uploader.cpython-311.pyc
--rw-rw-rw-   0        0        0      141 2023-04-12 03:31:13.000000 logfire-python-0.0.5/logfire/compat.py
--rw-rw-rw-   0        0        0     2998 2023-04-12 03:31:03.000000 logfire-python-0.0.5/logfire/flusher.py
--rw-rw-rw-   0        0        0      968 2023-04-12 03:30:53.000000 logfire-python-0.0.5/logfire/formatter.py
--rw-rw-rw-   0        0        0     2642 2023-06-20 11:47:33.000000 logfire-python-0.0.5/logfire/frame.py
--rw-rw-rw-   0        0        0     2680 2023-06-20 11:54:06.000000 logfire-python-0.0.5/logfire/handler.py
--rw-rw-rw-   0        0        0     1156 2023-04-12 03:30:18.000000 logfire-python-0.0.5/logfire/helpers.py
--rw-rw-rw-   0        0        0      588 2023-04-12 03:30:07.000000 logfire-python-0.0.5/logfire/uploader.py
-drwxrwxrwx   0        0        0        0 2023-06-20 11:54:18.316285 logfire-python-0.0.5/logfire_python.egg-info/
--rw-rw-rw-   0        0        0     3861 2023-06-20 11:54:18.000000 logfire-python-0.0.5/logfire_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      919 2023-06-20 11:54:18.000000 logfire-python-0.0.5/logfire_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 11:54:18.000000 logfire-python-0.0.5/logfire_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       98 2023-06-20 11:54:18.000000 logfire-python-0.0.5/logfire_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-20 11:54:18.000000 logfire-python-0.0.5/logfire_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1357 2023-06-20 11:53:42.000000 logfire-python-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0      222 2023-04-12 07:58:34.000000 logfire-python-0.0.5/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-20 11:54:18.322284 logfire-python-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0       54 2023-04-12 05:19:07.000000 logfire-python-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-20 11:54:18.320285 logfire-python-0.0.5/tests/
--rw-rw-rw-   0        0        0        0 2023-04-11 14:45:50.000000 logfire-python-0.0.5/tests/__init__.py
--rw-rw-rw-   0        0        0     5206 2023-06-06 06:50:49.000000 logfire-python-0.0.5/tests/test_flusher.py
--rw-rw-rw-   0        0        0     5264 2023-04-11 15:02:08.000000 logfire-python-0.0.5/tests/test_formatter.py
--rw-rw-rw-   0        0        0     1955 2023-04-11 15:02:30.000000 logfire-python-0.0.5/tests/test_frame.py
--rw-rw-rw-   0        0        0     4337 2023-04-11 15:02:51.000000 logfire-python-0.0.5/tests/test_handler.py
--rw-rw-rw-   0        0        0     1846 2023-04-11 15:03:14.000000 logfire-python-0.0.5/tests/test_helpers.py
--rw-rw-rw-   0        0        0     1059 2023-04-11 15:03:40.000000 logfire-python-0.0.5/tests/test_uploader.py
+drwxrwxrwx   0        0        0        0 2023-06-20 12:20:07.894217 logfire-python-0.0.6/
+-rw-rw-rw-   0        0        0      741 2023-04-12 02:48:20.000000 logfire-python-0.0.6/LICENSE.md
+-rw-rw-rw-   0        0        0      106 2023-04-12 06:15:33.000000 logfire-python-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     3861 2023-06-20 12:20:07.894217 logfire-python-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2672 2023-04-12 03:58:47.000000 logfire-python-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 12:20:07.879212 logfire-python-0.0.6/logfire/
+-rw-rw-rw-   0        0        0      260 2023-04-12 03:28:58.000000 logfire-python-0.0.6/logfire/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 12:20:07.883219 logfire-python-0.0.6/logfire/__pycache__/
+-rw-rw-rw-   0        0        0      539 2023-06-20 11:04:18.000000 logfire-python-0.0.6/logfire/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      406 2023-06-20 11:04:18.000000 logfire-python-0.0.6/logfire/__pycache__/compat.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3574 2023-06-20 11:04:18.000000 logfire-python-0.0.6/logfire/__pycache__/flusher.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1462 2023-06-20 11:04:18.000000 logfire-python-0.0.6/logfire/__pycache__/formatter.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3849 2023-06-20 12:14:04.000000 logfire-python-0.0.6/logfire/__pycache__/frame.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3811 2023-06-20 12:03:55.000000 logfire-python-0.0.6/logfire/__pycache__/handler.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2627 2023-06-20 11:04:18.000000 logfire-python-0.0.6/logfire/__pycache__/helpers.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1367 2023-06-20 11:04:18.000000 logfire-python-0.0.6/logfire/__pycache__/uploader.cpython-311.pyc
+-rw-rw-rw-   0        0        0      141 2023-04-12 03:31:13.000000 logfire-python-0.0.6/logfire/compat.py
+-rw-rw-rw-   0        0        0     2998 2023-04-12 03:31:03.000000 logfire-python-0.0.6/logfire/flusher.py
+-rw-rw-rw-   0        0        0      968 2023-04-12 03:30:53.000000 logfire-python-0.0.6/logfire/formatter.py
+-rw-rw-rw-   0        0        0     2759 2023-06-20 12:14:00.000000 logfire-python-0.0.6/logfire/frame.py
+-rw-rw-rw-   0        0        0     2680 2023-06-20 12:19:35.000000 logfire-python-0.0.6/logfire/handler.py
+-rw-rw-rw-   0        0        0     1156 2023-04-12 03:30:18.000000 logfire-python-0.0.6/logfire/helpers.py
+-rw-rw-rw-   0        0        0      588 2023-04-12 03:30:07.000000 logfire-python-0.0.6/logfire/uploader.py
+drwxrwxrwx   0        0        0        0 2023-06-20 12:20:07.891219 logfire-python-0.0.6/logfire_python.egg-info/
+-rw-rw-rw-   0        0        0     3861 2023-06-20 12:20:07.000000 logfire-python-0.0.6/logfire_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      919 2023-06-20 12:20:07.000000 logfire-python-0.0.6/logfire_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 12:20:07.000000 logfire-python-0.0.6/logfire_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       98 2023-06-20 12:20:07.000000 logfire-python-0.0.6/logfire_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-20 12:20:07.000000 logfire-python-0.0.6/logfire_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1357 2023-06-20 12:20:03.000000 logfire-python-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0      222 2023-04-12 07:58:34.000000 logfire-python-0.0.6/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 12:20:07.894217 logfire-python-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0       54 2023-04-12 05:19:07.000000 logfire-python-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 12:20:07.894217 logfire-python-0.0.6/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-11 14:45:50.000000 logfire-python-0.0.6/tests/__init__.py
+-rw-rw-rw-   0        0        0     5206 2023-06-06 06:50:49.000000 logfire-python-0.0.6/tests/test_flusher.py
+-rw-rw-rw-   0        0        0     5264 2023-04-11 15:02:08.000000 logfire-python-0.0.6/tests/test_formatter.py
+-rw-rw-rw-   0        0        0     1955 2023-04-11 15:02:30.000000 logfire-python-0.0.6/tests/test_frame.py
+-rw-rw-rw-   0        0        0     4337 2023-04-11 15:02:51.000000 logfire-python-0.0.6/tests/test_handler.py
+-rw-rw-rw-   0        0        0     1846 2023-04-11 15:03:14.000000 logfire-python-0.0.6/tests/test_helpers.py
+-rw-rw-rw-   0        0        0     1059 2023-04-11 15:03:40.000000 logfire-python-0.0.6/tests/test_uploader.py
```

### Comparing `logfire-python-0.0.5/LICENSE.md` & `logfire-python-0.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `logfire-python-0.0.5/PKG-INFO` & `logfire-python-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logfire-python
-Version: 0.0.5
+Version: 0.0.6
 Summary: Logfire.sh client library
 Author-email: Logfire <support@logfire.sh>
 Project-URL: Homepage, https://github.com/logfire-sh/logfire-python
 Keywords: api,logfire,logging,client
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Operating System :: OS Independent
```

### Comparing `logfire-python-0.0.5/README.md` & `logfire-python-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `logfire-python-0.0.5/logfire/__pycache__/__init__.cpython-311.pyc` & `logfire-python-0.0.6/logfire/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `logfire-python-0.0.5/logfire/__pycache__/flusher.cpython-311.pyc` & `logfire-python-0.0.6/logfire/__pycache__/flusher.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `logfire-python-0.0.5/logfire/__pycache__/formatter.cpython-311.pyc` & `logfire-python-0.0.6/logfire/__pycache__/formatter.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `logfire-python-0.0.5/logfire/__pycache__/frame.cpython-311.pyc` & `logfire-python-0.0.6/logfire/__pycache__/frame.cpython-311.pyc`

 * *Files 10% similar despite different names*

#### Python bytecode

```diff
@@ -1,19 +1,20 @@
 magic:    0xa70d0d0a
-moddate:  0xd5919164 (Tue Jun 20 11:47:33 2023 UTC)
-files sz: 2642
+moddate:  0x08989164 (Tue Jun 20 12:14:00 2023 UTC)
+files sz: 2759
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
       0x9700640064016c006d015a016d025a020100640064026c036d035a0301
-      00640064036c046d055a050100640064046c065a06640b640684015a0764
-      0784005a08640884005a09640984005a0a640a84005a0b64045300
+      00640064036c045a04640064046c056d065a060100640064036c075a0764
+      0b640684015a08640784005a09640884005a0a640984005a0b640a84005a
+      0c64035300
      0           0 RESUME                   0
    
      2           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('print_function', 'unicode_literals'))
                  6 IMPORT_NAME              0 (__future__)
                  8 IMPORT_FROM              1 (print_function)
                 10 STORE_NAME               1 (print_function)
@@ -24,54 +25,59 @@
      3          18 LOAD_CONST               0 (0)
                 20 LOAD_CONST               2 (('datetime',))
                 22 IMPORT_NAME              3 (datetime)
                 24 IMPORT_FROM              3 (datetime)
                 26 STORE_NAME               3 (datetime)
                 28 POP_TOP
    
-     5          30 LOAD_CONST               0 (0)
-                32 LOAD_CONST               3 (('path',))
-                34 IMPORT_NAME              4 (os)
-                36 IMPORT_FROM              5 (path)
-                38 STORE_NAME               5 (path)
-                40 POP_TOP
+     4          30 LOAD_CONST               0 (0)
+                32 LOAD_CONST               3 (None)
+                34 IMPORT_NAME              4 (json)
+                36 STORE_NAME               4 (json)
    
-     6          42 LOAD_CONST               0 (0)
-                44 LOAD_CONST               4 (None)
-                46 IMPORT_NAME              6 (__main__)
-                48 STORE_NAME               6 (__main__)
+     6          38 LOAD_CONST               0 (0)
+                40 LOAD_CONST               4 (('path',))
+                42 IMPORT_NAME              5 (os)
+                44 IMPORT_FROM              6 (path)
+                46 STORE_NAME               6 (path)
+                48 POP_TOP
    
-     8          50 LOAD_CONST              11 ((False,))
-                52 LOAD_CONST               6 (<code object create_frame, file "D:\constient\logfire\logfire-python-source\logfire\frame.py", line 8>)
-                54 MAKE_FUNCTION            1 (defaults)
-                56 STORE_NAME               7 (create_frame)
+     7          50 LOAD_CONST               0 (0)
+                52 LOAD_CONST               3 (None)
+                54 IMPORT_NAME              7 (__main__)
+                56 STORE_NAME               7 (__main__)
    
-    44          58 LOAD_CONST               7 (<code object _parse_custom_events, file "D:\constient\logfire\logfire-python-source\logfire\frame.py", line 44>)
-                60 MAKE_FUNCTION            0
-                62 STORE_NAME               8 (_parse_custom_events)
+     9          58 LOAD_CONST              11 ((False,))
+                60 LOAD_CONST               6 (<code object create_frame, file "D:\constient\logfire\logfire-python-source\logfire\frame.py", line 9>)
+                62 MAKE_FUNCTION            1 (defaults)
+                64 STORE_NAME               8 (create_frame)
    
-    70          64 LOAD_CONST               8 (<code object _levelname, file "D:\constient\logfire\logfire-python-source\logfire\frame.py", line 70>)
-                66 MAKE_FUNCTION            0
-                68 STORE_NAME               9 (_levelname)
+    45          66 LOAD_CONST               7 (<code object _parse_custom_events, file "D:\constient\logfire\logfire-python-source\logfire\frame.py", line 45>)
+                68 MAKE_FUNCTION            0
+                70 STORE_NAME               9 (_parse_custom_events)
    
-    80          70 LOAD_CONST               9 (<code object _relative_to_main_module_if_possible, file "D:\constient\logfire\logfire-python-source\logfire\frame.py", line 80>)
-                72 MAKE_FUNCTION            0
-                74 STORE_NAME              10 (_relative_to_main_module_if_possible)
+    74          72 LOAD_CONST               8 (<code object _levelname, file "D:\constient\logfire\logfire-python-source\logfire\frame.py", line 74>)
+                74 MAKE_FUNCTION            0
+                76 STORE_NAME              10 (_levelname)
    
-    84          76 LOAD_CONST              10 (<code object _relative_to_main_module, file "D:\constient\logfire\logfire-python-source\logfire\frame.py", line 84>)
-                78 MAKE_FUNCTION            0
-                80 STORE_NAME              11 (_relative_to_main_module)
-                82 LOAD_CONST               4 (None)
-                84 RETURN_VALUE
+    84          78 LOAD_CONST               9 (<code object _relative_to_main_module_if_possible, file "D:\constient\logfire\logfire-python-source\logfire\frame.py", line 84>)
+                80 MAKE_FUNCTION            0
+                82 STORE_NAME              11 (_relative_to_main_module_if_possible)
+   
+    88          84 LOAD_CONST              10 (<code object _relative_to_main_module, file "D:\constient\logfire\logfire-python-source\logfire\frame.py", line 88>)
+                86 MAKE_FUNCTION            0
+                88 STORE_NAME              12 (_relative_to_main_module)
+                90 LOAD_CONST               3 (None)
+                92 RETURN_VALUE
    consts
       0
       ('print_function', 'unicode_literals')
       ('datetime',)
-      ('path',)
       None
+      ('path',)
       False
       code
          argcount  : 4
          nlocals   : 11
          stacksize : 6
          flags     : 3
          code
@@ -95,24 +101,24 @@
             0000007c02a0080000000000000000000000000000000000000000a60000
             00ab00000000000000000072277c07a00900000000000000000000000000
             000000000000007c02a00a00000000000000000000000000000000000000
             00a6000000ab000000000000000000a6010000ab01000000000000000001
             007417000000000000000000007c007c03a6020000ab0200000000000000
             007d0a7c0a72157c05a00900000000000000000000000000000000000000
             007c0aa6010000ab01000000000000000001007c055300
-           8           0 RESUME                   0
+           9           0 RESUME                   0
          
-           9           2 LOAD_FAST                0 (record)
+          10           2 LOAD_FAST                0 (record)
                        4 LOAD_ATTR                0 (__dict__)
                       14 STORE_FAST               4 (r)
          
-          10          16 BUILD_MAP                0
+          11          16 BUILD_MAP                0
                       18 STORE_FAST               5 (frame)
          
-          13          20 LOAD_CONST               1 ('{}+00:00')
+          14          20 LOAD_CONST               1 ('{}+00:00')
                       22 LOAD_METHOD              1 (format)
                       44 LOAD_GLOBAL              5 (NULL + datetime)
                       56 LOAD_ATTR                3 (utcfromtimestamp)
                       66 LOAD_FAST                4 (r)
                       68 LOAD_CONST               2 ('created')
                       70 BINARY_SUBSCR
                       80 PRECALL                  1
@@ -122,157 +128,157 @@
                      120 CALL                     0
                      130 PRECALL                  1
                      134 CALL                     1
                      144 LOAD_FAST                5 (frame)
                      146 LOAD_CONST               3 ('dt')
                      148 STORE_SUBSCR
          
-          14         152 LOAD_GLOBAL             11 (NULL + _levelname)
+          15         152 LOAD_GLOBAL             11 (NULL + _levelname)
                      164 LOAD_FAST                4 (r)
                      166 LOAD_CONST               4 ('levelname')
                      168 BINARY_SUBSCR
                      178 PRECALL                  1
                      182 CALL                     1
                      192 COPY                     1
                      194 LOAD_FAST                5 (frame)
                      196 LOAD_CONST               5 ('level')
                      198 STORE_SUBSCR
                      202 STORE_FAST               6 (level)
          
-          15         204 LOAD_GLOBAL             13 (NULL + int)
+          16         204 LOAD_GLOBAL             13 (NULL + int)
                      216 LOAD_FAST                4 (r)
                      218 LOAD_CONST               6 ('levelno')
                      220 BINARY_SUBSCR
                      230 LOAD_CONST               7 (10)
                      232 BINARY_OP               11 (/)
                      236 PRECALL                  1
                      240 CALL                     1
                      250 LOAD_FAST                5 (frame)
                      252 LOAD_CONST               8 ('severity')
                      254 STORE_SUBSCR
          
-          16         258 LOAD_FAST                1 (message)
+          17         258 LOAD_FAST                1 (message)
                      260 LOAD_FAST                5 (frame)
                      262 LOAD_CONST               9 ('message')
                      264 STORE_SUBSCR
          
-          17         268 BUILD_MAP                0
+          18         268 BUILD_MAP                0
                      270 COPY                     1
                      272 LOAD_FAST                5 (frame)
                      274 LOAD_CONST              10 ('context')
                      276 STORE_SUBSCR
                      280 STORE_FAST               7 (ctx)
          
-          20         282 BUILD_MAP                0
+          21         282 BUILD_MAP                0
                      284 COPY                     1
                      286 LOAD_FAST                7 (ctx)
                      288 LOAD_CONST              11 ('runtime')
                      290 STORE_SUBSCR
                      294 STORE_FAST               8 (runtime)
          
-          21         296 LOAD_FAST                4 (r)
+          22         296 LOAD_FAST                4 (r)
                      298 LOAD_CONST              12 ('funcName')
                      300 BINARY_SUBSCR
                      310 LOAD_FAST                8 (runtime)
                      312 LOAD_CONST              13 ('function')
                      314 STORE_SUBSCR
          
-          22         318 LOAD_GLOBAL             15 (NULL + _relative_to_main_module_if_possible)
+          23         318 LOAD_GLOBAL             15 (NULL + _relative_to_main_module_if_possible)
                      330 LOAD_FAST                4 (r)
                      332 LOAD_CONST              14 ('pathname')
                      334 BINARY_SUBSCR
                      344 PRECALL                  1
                      348 CALL                     1
                      358 LOAD_FAST                8 (runtime)
                      360 LOAD_CONST              15 ('file')
                      362 STORE_SUBSCR
          
-          23         366 LOAD_FAST                4 (r)
+          24         366 LOAD_FAST                4 (r)
                      368 LOAD_CONST              16 ('lineno')
                      370 BINARY_SUBSCR
                      380 LOAD_FAST                8 (runtime)
                      382 LOAD_CONST              17 ('line')
                      384 STORE_SUBSCR
          
-          24         388 LOAD_FAST                4 (r)
+          25         388 LOAD_FAST                4 (r)
                      390 LOAD_CONST              18 ('thread')
                      392 BINARY_SUBSCR
                      402 LOAD_FAST                8 (runtime)
                      404 LOAD_CONST              19 ('thread_id')
                      406 STORE_SUBSCR
          
-          25         410 LOAD_FAST                4 (r)
+          26         410 LOAD_FAST                4 (r)
                      412 LOAD_CONST              20 ('threadName')
                      414 BINARY_SUBSCR
                      424 LOAD_FAST                8 (runtime)
                      426 LOAD_CONST              21 ('thread_name')
                      428 STORE_SUBSCR
          
-          26         432 LOAD_FAST                4 (r)
+          27         432 LOAD_FAST                4 (r)
                      434 LOAD_CONST              22 ('name')
                      436 BINARY_SUBSCR
                      446 LOAD_FAST                8 (runtime)
                      448 LOAD_CONST              23 ('logger_name')
                      450 STORE_SUBSCR
          
-          29         454 BUILD_MAP                0
+          30         454 BUILD_MAP                0
                      456 COPY                     1
                      458 LOAD_FAST                7 (ctx)
                      460 LOAD_CONST              24 ('system')
                      462 STORE_SUBSCR
                      466 STORE_FAST               9 (system)
          
-          30         468 LOAD_FAST                4 (r)
+          31         468 LOAD_FAST                4 (r)
                      470 LOAD_CONST              25 ('process')
                      472 BINARY_SUBSCR
                      482 LOAD_FAST                9 (system)
                      484 LOAD_CONST              26 ('pid')
                      486 STORE_SUBSCR
          
-          31         490 LOAD_FAST                4 (r)
+          32         490 LOAD_FAST                4 (r)
                      492 LOAD_CONST              27 ('processName')
                      494 BINARY_SUBSCR
                      504 LOAD_FAST                9 (system)
                      506 LOAD_CONST              28 ('process_name')
                      508 STORE_SUBSCR
          
-          34         512 LOAD_FAST                2 (context)
+          35         512 LOAD_FAST                2 (context)
                      514 LOAD_METHOD              8 (exists)
                      536 PRECALL                  0
                      540 CALL                     0
                      550 POP_JUMP_FORWARD_IF_FALSE    39 (to 630)
          
-          35         552 LOAD_FAST                7 (ctx)
+          36         552 LOAD_FAST                7 (ctx)
                      554 LOAD_METHOD              9 (update)
                      576 LOAD_FAST                2 (context)
                      578 LOAD_METHOD             10 (collapse)
                      600 PRECALL                  0
                      604 CALL                     0
                      614 PRECALL                  1
                      618 CALL                     1
                      628 POP_TOP
          
-          37     >>  630 LOAD_GLOBAL             23 (NULL + _parse_custom_events)
+          38     >>  630 LOAD_GLOBAL             23 (NULL + _parse_custom_events)
                      642 LOAD_FAST                0 (record)
                      644 LOAD_FAST                3 (include_extra_attributes)
                      646 PRECALL                  2
                      650 CALL                     2
                      660 STORE_FAST              10 (events)
          
-          38         662 LOAD_FAST               10 (events)
+          39         662 LOAD_FAST               10 (events)
                      664 POP_JUMP_FORWARD_IF_FALSE    21 (to 708)
          
-          39         666 LOAD_FAST                5 (frame)
+          40         666 LOAD_FAST                5 (frame)
                      668 LOAD_METHOD              9 (update)
                      690 LOAD_FAST               10 (events)
                      692 PRECALL                  1
                      696 CALL                     1
                      706 POP_TOP
          
-          41     >>  708 LOAD_FAST                5 (frame)
+          42     >>  708 LOAD_FAST                5 (frame)
                      710 RETURN_VALUE
          consts
             None
             '{}+00:00'
             'created'
             'dt'
             'levelname'
@@ -302,152 +308,172 @@
             'process_name'
          names      ('__dict__', 'format', 'datetime', 'utcfromtimestamp', 'isoformat', '_levelname', 'int', '_relative_to_main_module_if_possible', 'exists', 'update', 'collapse', '_parse_custom_events')
          varnames   ('record', 'message', 'context', 'include_extra_attributes', 'r', 'frame', 'level', 'ctx', 'runtime', 'system', 'events')
          freevars   ()
          cellvars   ()
          filename   'D:\\constient\\logfire\\logfire-python-source\\logfire\\frame.py'
          name       'create_frame'
-         firstlineno 8
+         firstlineno 9
          lnotab
             0x02010e0104038401340136010a010e030e011601300116011601160116
             030e011601160328014e02200104012a02
       code
          argcount  : 2
          nlocals   : 8
          stacksize : 5
          flags     : 3
          code
             0x970068006401a3017d026402640368027d0369007d0469007d057c006a
             000000000000000000a00100000000000000000000000000000000000000
-            00a6000000ab00000000000000000044005d315c0200007d067d077c067c
+            00a6000000ab00000000000000000044005d5e5c0200007d067d077c067c
             02760072018c0a7c0173167405000000000000000000007c077406000000
             00000000000000a6020000ab02000000000000000073018c227c067c0376
-            0172067c077c057c063c0000008c2c7c077c047c063c0000008c327c0572
+            0172337405000000000000000000007c07740600000000000000000000a6
+            020000ab02000000000000000072187409000000000000000000006a0500
+            000000000000007c07a6010000ab0100000000000000007c057c063c0000
+            008c537c077c057c063c0000008c597c077c047c063c0000008c5f7c0572
             057c057c0464043c0000007c045300
-          44           0 RESUME                   0
+          45           0 RESUME                   0
          
-          45           2 BUILD_SET                0
+          46           2 BUILD_SET                0
                        4 LOAD_CONST               1 (frozenset({'processName', 'threadName', 'exc_text', 'thread', 'pathname', 'exc_info', 'process', 'module', 'msg', 'lineno', 'funcName', 'name', 'msecs', 'levelno', 'message', 'created', 'relativeCreated', 'asctime', 'levelname', 'args'}))
                        6 SET_UPDATE               1
                        8 STORE_FAST               2 (default_keys)
          
-          52          10 LOAD_CONST               2 ('filename')
+          53          10 LOAD_CONST               2 ('filename')
                       12 LOAD_CONST               3 ('stack_info')
          
-          51          14 BUILD_SET                2
+          52          14 BUILD_SET                2
                       16 STORE_FAST               3 (extra_keys)
          
-          54          18 BUILD_MAP                0
+          55          18 BUILD_MAP                0
                       20 STORE_FAST               4 (events)
          
-          55          22 BUILD_MAP                0
+          56          22 BUILD_MAP                0
                       24 STORE_FAST               5 (extra)
          
-          56          26 LOAD_FAST                0 (record)
+          57          26 LOAD_FAST                0 (record)
                       28 LOAD_ATTR                0 (__dict__)
                       38 LOAD_METHOD              1 (items)
                       60 PRECALL                  0
                       64 CALL                     0
                       74 GET_ITER
-                 >>   76 FOR_ITER                49 (to 176)
+                 >>   76 FOR_ITER                94 (to 266)
                       78 UNPACK_SEQUENCE          2
                       82 STORE_FAST               6 (key)
                       84 STORE_FAST               7 (val)
          
-          57          86 LOAD_FAST                6 (key)
+          58          86 LOAD_FAST                6 (key)
                       88 LOAD_FAST                2 (default_keys)
                       90 CONTAINS_OP              0
                       92 POP_JUMP_FORWARD_IF_FALSE     1 (to 96)
          
-          58          94 JUMP_BACKWARD           10 (to 76)
+          59          94 JUMP_BACKWARD           10 (to 76)
          
-          59     >>   96 LOAD_FAST                1 (include_extra_attributes)
+          60     >>   96 LOAD_FAST                1 (include_extra_attributes)
                       98 POP_JUMP_FORWARD_IF_TRUE    22 (to 144)
                      100 LOAD_GLOBAL              5 (NULL + isinstance)
                      112 LOAD_FAST                7 (val)
                      114 LOAD_GLOBAL              6 (dict)
                      126 PRECALL                  2
                      130 CALL                     2
                      140 POP_JUMP_FORWARD_IF_TRUE     1 (to 144)
          
-          60         142 JUMP_BACKWARD           34 (to 76)
+          61         142 JUMP_BACKWARD           34 (to 76)
          
-          61     >>  144 LOAD_FAST                6 (key)
+          62     >>  144 LOAD_FAST                6 (key)
                      146 LOAD_FAST                3 (extra_keys)
                      148 CONTAINS_OP              1
-                     150 POP_JUMP_FORWARD_IF_FALSE     6 (to 164)
+                     150 POP_JUMP_FORWARD_IF_FALSE    51 (to 254)
          
-          62         152 LOAD_FAST                7 (val)
-                     154 LOAD_FAST                5 (extra)
-                     156 LOAD_FAST                6 (key)
-                     158 STORE_SUBSCR
-                     162 JUMP_BACKWARD           44 (to 76)
-         
-          64     >>  164 LOAD_FAST                7 (val)
-                     166 LOAD_FAST                4 (events)
-                     168 LOAD_FAST                6 (key)
-                     170 STORE_SUBSCR
-                     174 JUMP_BACKWARD           50 (to 76)
-         
-          65     >>  176 LOAD_FAST                5 (extra)
-                     178 POP_JUMP_FORWARD_IF_FALSE     5 (to 190)
-         
-          66         180 LOAD_FAST                5 (extra)
-                     182 LOAD_FAST                4 (events)
-                     184 LOAD_CONST               4 ('extra')
-                     186 STORE_SUBSCR
+          63         152 LOAD_GLOBAL              5 (NULL + isinstance)
+                     164 LOAD_FAST                7 (val)
+                     166 LOAD_GLOBAL              6 (dict)
+                     178 PRECALL                  2
+                     182 CALL                     2
+                     192 POP_JUMP_FORWARD_IF_FALSE    24 (to 242)
+         
+          64         194 LOAD_GLOBAL              9 (NULL + json)
+                     206 LOAD_ATTR                5 (dumps)
+                     216 LOAD_FAST                7 (val)
+                     218 PRECALL                  1
+                     222 CALL                     1
+                     232 LOAD_FAST                5 (extra)
+                     234 LOAD_FAST                6 (key)
+                     236 STORE_SUBSCR
+                     240 JUMP_BACKWARD           83 (to 76)
+         
+          66     >>  242 LOAD_FAST                7 (val)
+                     244 LOAD_FAST                5 (extra)
+                     246 LOAD_FAST                6 (key)
+                     248 STORE_SUBSCR
+                     252 JUMP_BACKWARD           89 (to 76)
+         
+          68     >>  254 LOAD_FAST                7 (val)
+                     256 LOAD_FAST                4 (events)
+                     258 LOAD_FAST                6 (key)
+                     260 STORE_SUBSCR
+                     264 JUMP_BACKWARD           95 (to 76)
+         
+          69     >>  266 LOAD_FAST                5 (extra)
+                     268 POP_JUMP_FORWARD_IF_FALSE     5 (to 280)
+         
+          70         270 LOAD_FAST                5 (extra)
+                     272 LOAD_FAST                4 (events)
+                     274 LOAD_CONST               4 ('extra')
+                     276 STORE_SUBSCR
          
-          67     >>  190 LOAD_FAST                4 (events)
-                     192 RETURN_VALUE
+          71     >>  280 LOAD_FAST                4 (events)
+                     282 RETURN_VALUE
          consts
             None
             frozenset({'processName', 'threadName', 'exc_text', 'thread', 'pathname', 'exc_info', 'process', 'module', 'msg', 'lineno', 'funcName', 'name', 'msecs', 'levelno', 'message', 'created', 'relativeCreated', 'asctime', 'levelname', 'args'})
             'filename'
             'stack_info'
             'extra'
-         names      ('__dict__', 'items', 'isinstance', 'dict')
+         names      ('__dict__', 'items', 'isinstance', 'dict', 'json', 'dumps')
          varnames   ('record', 'include_extra_attributes', 'default_keys', 'extra_keys', 'events', 'extra', 'key', 'val')
          freevars   ()
          cellvars   ()
          filename   'D:\\constient\\logfire\\logfire-python-source\\logfire\\frame.py'
          name       '_parse_custom_events'
-         firstlineno 44
+         firstlineno 45
          lnotab
-            0x0201080704ff0403040104013c01080102012e01020108010c020c0104
-            010a01
+            0x0201080704ff0403040104013c01080102012e01020108012a0130020c
+            020c0104010a01
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 6
          flags     : 3
          code
             0x97006401640264036404640564069c057c00a000000000000000000000
             0000000000000000000000a6000000ab0000000000000000001900000000
             00000000005300
-          70           0 RESUME                   0
+          74           0 RESUME                   0
          
-          72           2 LOAD_CONST               1 ('debug')
+          76           2 LOAD_CONST               1 ('debug')
          
-          73           4 LOAD_CONST               2 ('info')
+          77           4 LOAD_CONST               2 ('info')
          
-          74           6 LOAD_CONST               3 ('warn')
+          78           6 LOAD_CONST               3 ('warn')
          
-          75           8 LOAD_CONST               4 ('error')
+          79           8 LOAD_CONST               4 ('error')
          
-          76          10 LOAD_CONST               5 ('critical')
+          80          10 LOAD_CONST               5 ('critical')
          
-          71          12 LOAD_CONST               6 (('debug', 'info', 'warning', 'error', 'critical'))
+          75          12 LOAD_CONST               6 (('debug', 'info', 'warning', 'error', 'critical'))
                       14 BUILD_CONST_KEY_MAP      5
          
-          77          16 LOAD_FAST                0 (level)
+          81          16 LOAD_FAST                0 (level)
                       18 LOAD_METHOD              0 (lower)
                       40 PRECALL                  0
                       44 CALL                     0
          
-          71          54 BINARY_SUBSCR
+          75          54 BINARY_SUBSCR
                       64 RETURN_VALUE
          consts
             None
             'debug'
             'info'
             'warn'
             'error'
@@ -455,35 +481,35 @@
             ('debug', 'info', 'warning', 'error', 'critical')
          names      ('lower',)
          varnames   ('level',)
          freevars   ()
          cellvars   ()
          filename   'D:\\constient\\logfire\\logfire-python-source\\logfire\\frame.py'
          name       '_levelname'
-         firstlineno 70
+         firstlineno 74
          lnotab 0x0202020102010201020102fb040626fa
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 4
          flags     : 3
          code
             0x97007401000000000000000000007402000000000000000000006401a6
             020000ab0200000000000000007d017c01720f7405000000000000000000
             007c00a6010000ab0100000000000000006e017c005300
-          80           0 RESUME                   0
+          84           0 RESUME                   0
          
-          81           2 LOAD_GLOBAL              1 (NULL + hasattr)
+          85           2 LOAD_GLOBAL              1 (NULL + hasattr)
                       14 LOAD_GLOBAL              2 (__main__)
                       26 LOAD_CONST               1 ('__file__')
                       28 PRECALL                  2
                       32 CALL                     2
                       42 STORE_FAST               1 (has_main_module)
          
-          82          44 LOAD_FAST                1 (has_main_module)
+          86          44 LOAD_FAST                1 (has_main_module)
                       46 POP_JUMP_FORWARD_IF_FALSE    15 (to 78)
                       48 LOAD_GLOBAL              5 (NULL + _relative_to_main_module)
                       60 LOAD_FAST                0 (pathname)
                       62 PRECALL                  1
                       66 CALL                     1
                       76 JUMP_FORWARD             1 (to 80)
                  >>   78 LOAD_FAST                0 (pathname)
@@ -493,29 +519,29 @@
             '__file__'
          names      ('hasattr', '__main__', '_relative_to_main_module')
          varnames   ('pathname', 'has_main_module')
          freevars   ()
          cellvars   ()
          filename   'D:\\constient\\logfire\\logfire-python-source\\logfire\\frame.py'
          name       '_relative_to_main_module_if_possible'
-         firstlineno 80
+         firstlineno 84
          lnotab 0x02012a01
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 6
          flags     : 3
          code
             0x97007401000000000000000000006a0100000000000000007c00740100
             0000000000000000006a0200000000000000007406000000000000000000
             006a040000000000000000a6010000ab010000000000000000a6020000ab
             0200000000000000005300
-          84           0 RESUME                   0
+          88           0 RESUME                   0
          
-          85           2 LOAD_GLOBAL              1 (NULL + path)
+          89           2 LOAD_GLOBAL              1 (NULL + path)
                       14 LOAD_ATTR                1 (relpath)
                       24 LOAD_FAST                0 (pathname)
                       26 LOAD_GLOBAL              1 (NULL + path)
                       38 LOAD_ATTR                2 (dirname)
                       48 LOAD_GLOBAL              6 (__main__)
                       60 LOAD_ATTR                4 (__file__)
                       70 PRECALL                  1
@@ -527,18 +553,18 @@
             None
          names      ('path', 'relpath', 'dirname', '__main__', '__file__')
          varnames   ('pathname',)
          freevars   ()
          cellvars   ()
          filename   'D:\\constient\\logfire\\logfire-python-source\\logfire\\frame.py'
          name       '_relative_to_main_module'
-         firstlineno 84
+         firstlineno 88
          lnotab 0x0201
       (False,)
-   names      ('__future__', 'print_function', 'unicode_literals', 'datetime', 'os', 'path', '__main__', 'create_frame', '_parse_custom_events', '_levelname', '_relative_to_main_module_if_possible', '_relative_to_main_module')
+   names      ('__future__', 'print_function', 'unicode_literals', 'datetime', 'json', 'os', 'path', '__main__', 'create_frame', '_parse_custom_events', '_levelname', '_relative_to_main_module_if_possible', '_relative_to_main_module')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'D:\\constient\\logfire\\logfire-python-source\\logfire\\frame.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff020210010c020c0108020824061a060a0604
+   lnotab 0x00ff020210010c0108020c0108020824061d060a0604
```

### Comparing `logfire-python-0.0.5/logfire/__pycache__/handler.cpython-311.pyc` & `logfire-python-0.0.6/logfire/__pycache__/handler.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x45869164 (Tue Jun 20 10:58:13 2023 UTC)
+moddate:  0xa9959164 (Tue Jun 20 12:03:53 2023 UTC)
 files sz: 2733
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `logfire-python-0.0.5/logfire/__pycache__/helpers.cpython-311.pyc` & `logfire-python-0.0.6/logfire/__pycache__/helpers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `logfire-python-0.0.5/logfire/__pycache__/uploader.cpython-311.pyc` & `logfire-python-0.0.6/logfire/__pycache__/uploader.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `logfire-python-0.0.5/logfire/flusher.py` & `logfire-python-0.0.6/logfire/flusher.py`

 * *Files identical despite different names*

### Comparing `logfire-python-0.0.5/logfire/formatter.py` & `logfire-python-0.0.6/logfire/formatter.py`

 * *Files identical despite different names*

### Comparing `logfire-python-0.0.5/logfire/frame.py` & `logfire-python-0.0.6/logfire/frame.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # coding: utf-8
 from __future__ import print_function, unicode_literals
 from datetime import datetime
+import json
 
 from os import path
 import __main__
 
 def create_frame(record, message, context, include_extra_attributes=False):
     r = record.__dict__
     frame = {}
@@ -55,15 +56,18 @@
     extra = {}
     for key, val in record.__dict__.items():
         if key in default_keys:
             continue
         if not include_extra_attributes and not isinstance(val, dict):
             continue
         if key not in extra_keys:
-            extra[key] = val
+            if isinstance(val, dict):
+                extra[key] = json.dumps(val)
+            else:
+                extra[key] = val
         else:
             events[key] = val
     if extra :
         events["extra"] = extra
     return events
```

### Comparing `logfire-python-0.0.5/logfire/handler.py` & `logfire-python-0.0.6/logfire/handler.py`

 * *Files identical despite different names*

### Comparing `logfire-python-0.0.5/logfire/helpers.py` & `logfire-python-0.0.6/logfire/helpers.py`

 * *Files identical despite different names*

### Comparing `logfire-python-0.0.5/logfire/uploader.py` & `logfire-python-0.0.6/logfire/uploader.py`

 * *Files identical despite different names*

### Comparing `logfire-python-0.0.5/logfire_python.egg-info/PKG-INFO` & `logfire-python-0.0.6/logfire_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logfire-python
-Version: 0.0.5
+Version: 0.0.6
 Summary: Logfire.sh client library
 Author-email: Logfire <support@logfire.sh>
 Project-URL: Homepage, https://github.com/logfire-sh/logfire-python
 Keywords: api,logfire,logging,client
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Operating System :: OS Independent
```

### Comparing `logfire-python-0.0.5/logfire_python.egg-info/SOURCES.txt` & `logfire-python-0.0.6/logfire_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `logfire-python-0.0.5/pyproject.toml` & `logfire-python-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "logfire-python"
-version = "0.0.5"
+version = "0.0.6"
 description = "Logfire.sh client library"
 readme = "README.md"
 authors = [{ name = "Logfire", email = "support@logfire.sh" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: ISC License (ISCL)",
```

### Comparing `logfire-python-0.0.5/tests/test_flusher.py` & `logfire-python-0.0.6/tests/test_flusher.py`

 * *Files identical despite different names*

### Comparing `logfire-python-0.0.5/tests/test_formatter.py` & `logfire-python-0.0.6/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `logfire-python-0.0.5/tests/test_frame.py` & `logfire-python-0.0.6/tests/test_frame.py`

 * *Files identical despite different names*

### Comparing `logfire-python-0.0.5/tests/test_handler.py` & `logfire-python-0.0.6/tests/test_handler.py`

 * *Files identical despite different names*

### Comparing `logfire-python-0.0.5/tests/test_helpers.py` & `logfire-python-0.0.6/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `logfire-python-0.0.5/tests/test_uploader.py` & `logfire-python-0.0.6/tests/test_uploader.py`

 * *Files identical despite different names*

