# Comparing `tmp/xrd-xy-parser-0.0.3.tar.gz` & `tmp/xrd-xy-parser-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xrd-xy-parser-0.0.3.tar", last modified: Fri Sep 30 11:51:43 2022, max compression
+gzip compressed data, was "xrd-xy-parser-0.0.4.tar", last modified: Tue Jun 20 14:33:46 2023, max compression
```

## Comparing `xrd-xy-parser-0.0.3.tar` & `xrd-xy-parser-0.0.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 masaki    (1000) masaki    (1000)        0 2022-09-30 11:51:43.170058 xrd-xy-parser-0.0.3/
--rw-rw-r--   0 masaki    (1000) masaki    (1000)       38 2022-09-30 07:06:10.000000 xrd-xy-parser-0.0.3/.gitignore
--rw-rw-r--   0 masaki    (1000) masaki    (1000)     1064 2022-09-30 07:09:10.000000 xrd-xy-parser-0.0.3/LICENSE
--rw-rw-r--   0 masaki    (1000) masaki    (1000)     1334 2022-09-30 11:51:43.170058 xrd-xy-parser-0.0.3/PKG-INFO
--rw-rw-r--   0 masaki    (1000) masaki    (1000)      928 2022-09-30 11:16:08.000000 xrd-xy-parser-0.0.3/README.md
-drwxrwxr-x   0 masaki    (1000) masaki    (1000)        0 2022-09-30 11:51:43.170058 xrd-xy-parser-0.0.3/examples/
--rw-rw-r--   0 masaki    (1000) masaki    (1000)      265 2022-09-30 07:06:10.000000 xrd-xy-parser-0.0.3/examples/example.py
--rw-rw-r--   0 masaki    (1000) masaki    (1000)    23824 2022-09-30 07:06:10.000000 xrd-xy-parser-0.0.3/examples/example.xy
--rw-rw-r--   0 masaki    (1000) masaki    (1000)      592 2022-09-30 11:07:08.000000 xrd-xy-parser-0.0.3/pyproject.toml
--rw-rw-r--   0 masaki    (1000) masaki    (1000)       38 2022-09-30 11:51:43.170058 xrd-xy-parser-0.0.3/setup.cfg
-drwxrwxr-x   0 masaki    (1000) masaki    (1000)        0 2022-09-30 11:51:43.170058 xrd-xy-parser-0.0.3/tests/
-drwxrwxr-x   0 masaki    (1000) masaki    (1000)        0 2022-09-30 11:51:43.170058 xrd-xy-parser-0.0.3/tests/fail/
--rw-rw-r--   0 masaki    (1000) masaki    (1000)       30 2022-09-30 07:06:10.000000 xrd-xy-parser-0.0.3/tests/fail/1.xy
--rw-rw-r--   0 masaki    (1000) masaki    (1000)       39 2022-09-30 07:06:10.000000 xrd-xy-parser-0.0.3/tests/fail/2.xy
--rw-rw-r--   0 masaki    (1000) masaki    (1000)       46 2022-09-30 07:06:10.000000 xrd-xy-parser-0.0.3/tests/fail/3.xy
--rw-rw-r--   0 masaki    (1000) masaki    (1000)     2483 2022-09-30 07:06:10.000000 xrd-xy-parser-0.0.3/tests/success_cases.py
--rw-rw-r--   0 masaki    (1000) masaki    (1000)     1366 2022-09-30 07:06:10.000000 xrd-xy-parser-0.0.3/tests/test1.py
-drwxrwxr-x   0 masaki    (1000) masaki    (1000)        0 2022-09-30 11:51:43.170058 xrd-xy-parser-0.0.3/xrd_xy_parser/
--rw-rw-r--   0 masaki    (1000) masaki    (1000)       42 2022-09-30 07:06:10.000000 xrd-xy-parser-0.0.3/xrd_xy_parser/__init__.py
--rw-rw-r--   0 masaki    (1000) masaki    (1000)     3157 2022-09-30 07:06:10.000000 xrd-xy-parser-0.0.3/xrd_xy_parser/xy.py
-drwxrwxr-x   0 masaki    (1000) masaki    (1000)        0 2022-09-30 11:51:43.170058 xrd-xy-parser-0.0.3/xrd_xy_parser.egg-info/
--rw-rw-r--   0 masaki    (1000) masaki    (1000)     1334 2022-09-30 11:51:43.000000 xrd-xy-parser-0.0.3/xrd_xy_parser.egg-info/PKG-INFO
--rw-rw-r--   0 masaki    (1000) masaki    (1000)      399 2022-09-30 11:51:43.000000 xrd-xy-parser-0.0.3/xrd_xy_parser.egg-info/SOURCES.txt
--rw-rw-r--   0 masaki    (1000) masaki    (1000)        1 2022-09-30 11:51:43.000000 xrd-xy-parser-0.0.3/xrd_xy_parser.egg-info/dependency_links.txt
--rw-rw-r--   0 masaki    (1000) masaki    (1000)        6 2022-09-30 11:51:43.000000 xrd-xy-parser-0.0.3/xrd_xy_parser.egg-info/requires.txt
--rw-rw-r--   0 masaki    (1000) masaki    (1000)       14 2022-09-30 11:51:43.000000 xrd-xy-parser-0.0.3/xrd_xy_parser.egg-info/top_level.txt
+drwxrwxr-x   0 masaki    (1000) masaki    (1000)        0 2023-06-20 14:33:46.071723 xrd-xy-parser-0.0.4/
+-rw-rw-r--   0 masaki    (1000) masaki    (1000)       47 2023-06-20 14:03:58.000000 xrd-xy-parser-0.0.4/.gitignore
+-rw-rw-r--   0 masaki    (1000) masaki    (1000)     1064 2023-06-20 13:30:01.000000 xrd-xy-parser-0.0.4/LICENSE
+-rw-rw-r--   0 masaki    (1000) masaki    (1000)     2506 2023-06-20 14:33:46.071723 xrd-xy-parser-0.0.4/PKG-INFO
+-rw-rw-r--   0 masaki    (1000) masaki    (1000)     2101 2023-06-20 14:23:18.000000 xrd-xy-parser-0.0.4/README.md
+drwxrwxr-x   0 masaki    (1000) masaki    (1000)        0 2023-06-20 14:33:46.067723 xrd-xy-parser-0.0.4/examples/
+-rw-rw-r--   0 masaki    (1000) masaki    (1000)      265 2022-09-30 07:06:10.000000 xrd-xy-parser-0.0.4/examples/example.py
+-rw-rw-r--   0 masaki    (1000) masaki    (1000)    23824 2022-09-30 07:06:10.000000 xrd-xy-parser-0.0.4/examples/example.xy
+-rw-rw-r--   0 masaki    (1000) masaki    (1000)      592 2023-06-20 13:30:01.000000 xrd-xy-parser-0.0.4/pyproject.toml
+-rw-rw-r--   0 masaki    (1000) masaki    (1000)       38 2023-06-20 14:33:46.071723 xrd-xy-parser-0.0.4/setup.cfg
+drwxrwxr-x   0 masaki    (1000) masaki    (1000)        0 2023-06-20 14:33:46.067723 xrd-xy-parser-0.0.4/tests/
+drwxrwxr-x   0 masaki    (1000) masaki    (1000)        0 2023-06-20 14:33:46.067723 xrd-xy-parser-0.0.4/tests/fail/
+-rw-rw-r--   0 masaki    (1000) masaki    (1000)       30 2022-09-30 07:06:10.000000 xrd-xy-parser-0.0.4/tests/fail/1.xy
+-rw-rw-r--   0 masaki    (1000) masaki    (1000)       39 2022-09-30 07:06:10.000000 xrd-xy-parser-0.0.4/tests/fail/2.xy
+-rw-rw-r--   0 masaki    (1000) masaki    (1000)       46 2022-09-30 07:06:10.000000 xrd-xy-parser-0.0.4/tests/fail/3.xy
+-rw-rw-r--   0 masaki    (1000) masaki    (1000)     2483 2022-09-30 07:06:10.000000 xrd-xy-parser-0.0.4/tests/success_cases.py
+-rw-rw-r--   0 masaki    (1000) masaki    (1000)     1802 2023-06-20 14:03:58.000000 xrd-xy-parser-0.0.4/tests/test1.py
+drwxrwxr-x   0 masaki    (1000) masaki    (1000)        0 2023-06-20 14:33:46.071723 xrd-xy-parser-0.0.4/xrd_xy_parser/
+-rw-rw-r--   0 masaki    (1000) masaki    (1000)       42 2022-09-30 07:06:10.000000 xrd-xy-parser-0.0.4/xrd_xy_parser/__init__.py
+-rw-rw-r--   0 masaki    (1000) masaki    (1000)     4668 2023-06-20 14:03:58.000000 xrd-xy-parser-0.0.4/xrd_xy_parser/xy.py
+drwxrwxr-x   0 masaki    (1000) masaki    (1000)        0 2023-06-20 14:33:46.071723 xrd-xy-parser-0.0.4/xrd_xy_parser.egg-info/
+-rw-rw-r--   0 masaki    (1000) masaki    (1000)     2506 2023-06-20 14:33:46.000000 xrd-xy-parser-0.0.4/xrd_xy_parser.egg-info/PKG-INFO
+-rw-rw-r--   0 masaki    (1000) masaki    (1000)      399 2023-06-20 14:33:46.000000 xrd-xy-parser-0.0.4/xrd_xy_parser.egg-info/SOURCES.txt
+-rw-rw-r--   0 masaki    (1000) masaki    (1000)        1 2023-06-20 14:33:46.000000 xrd-xy-parser-0.0.4/xrd_xy_parser.egg-info/dependency_links.txt
+-rw-rw-r--   0 masaki    (1000) masaki    (1000)        6 2023-06-20 14:33:46.000000 xrd-xy-parser-0.0.4/xrd_xy_parser.egg-info/requires.txt
+-rw-rw-r--   0 masaki    (1000) masaki    (1000)       14 2023-06-20 14:33:46.000000 xrd-xy-parser-0.0.4/xrd_xy_parser.egg-info/top_level.txt
```

### Comparing `xrd-xy-parser-0.0.3/LICENSE` & `xrd-xy-parser-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xrd-xy-parser-0.0.3/examples/example.xy` & `xrd-xy-parser-0.0.4/examples/example.xy`

 * *Files identical despite different names*

### Comparing `xrd-xy-parser-0.0.3/pyproject.toml` & `xrd-xy-parser-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xrd-xy-parser-0.0.3/tests/success_cases.py` & `xrd-xy-parser-0.0.4/tests/success_cases.py`

 * *Files identical despite different names*

### Comparing `xrd-xy-parser-0.0.3/tests/test1.py` & `xrd-xy-parser-0.0.4/tests/test1.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,7 +37,21 @@
     def test_fail(self):
         cnt = 0
 
         for f in Path(failpath).glob("*"):
             cnt += 1
             self.assertRaises(xy.ParseError, xy.read, f.resolve())
         self.assertTrue(cnt > 0, "fail file not found")
+
+    def test_read2xy_success(self):
+        for case in inouts:
+
+            mock = mock_open(read_data=case.in_)
+            with patch("pathlib.Path.open", mock):
+
+                got = xy.read2xy("")
+
+                dummydata = np.array(case.out_[1])
+                xs = dummydata[:, 0]
+                ys = dummydata[:, 1]
+                self.assertTrue((got.x == xs).all())
+                self.assertTrue((got.y == ys).all())
```

### Comparing `xrd-xy-parser-0.0.3/xrd_xy_parser/xy.py` & `xrd-xy-parser-0.0.4/xrd_xy_parser/xy.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+from functools import singledispatch
+
 from enum import Enum
-from io import TextIOWrapper
+from io import TextIOWrapper, TextIOBase
 import pathlib
 import re
 import numpy as np
 
+from typing import NamedTuple
 
 number_patt = r"[0-9]+(?:\.[0-9]+)?"
 """
 match integer or numbers like 12.33,0.1
 """
 delimiter_patt = r"(?:\s|\t)"
 
@@ -55,42 +58,79 @@
         if self.current is self.state.HEAD:
             self.head(line)
         elif self.current is self.state.BODY:
             self.body(line)
         elif self.current is self.state.FOOT:
             self.foot(line)
 
-    def error(self, file: TextIOWrapper) -> None:
+    def error(self, file: TextIOBase) -> None:
         """if cannot parse file,raise Error"""
 
         if self.current is not self.state.HEAD and self.foot_ == "":
             return None
 
         raise ParseError(file, self.head_, self.foot_)
 
 
 class ParseError(Exception):
     """cannot parse xy file."""
 
-    def __init__(self, file: TextIOWrapper, head: str, foot: str) -> None:
+    def __init__(self, file: TextIOBase, head: str, foot: str) -> None:
         # super.__init__(filename, foot)
         self.file = file
         self.head = head
         self.foot = foot
 
     def __str__(self) -> str:
-        return """Cannot parse ,wrong with something in '{}',
+        fmt = """Cannot parse ,wrong with something in '{}',
         header is {},
         footer is '{}'
-        """.format(
-            self.file.name, self.head, self.foot
-        )
+        """
+        if isinstance(self.file, TextIOWrapper):
+            return fmt.format(self.file.name, self.head, self.foot)
+        else:
+            return fmt.format("NOT text file", self.head, self.foot)
+
 
+@singledispatch
+def read(filelike: TextIOBase) -> tuple[str, np.ndarray, str]:
+    """
+    Parses the filelike xy data and returns a tuple consisting of error, header, body, and footer.
+    ファイルライクなxyデータをパースし、エラー、ヘッダ、ボディ、フットからなるタプルを返す.
 
-def read(path: pathlib.Path) -> tuple[str, np.ndarray, str]:
+    Parametors
+    ---
+        `filelike`: TextIOBase
+           filelike xydata
+
+    Returns
+    ---
+        `header`:str
+            path's file header
+
+        `body`:numpy.ndarray
+            path's file data
+
+        `footer`:str
+            path's file header
+
+    Raises:
+        ParseError:
+            raise on fail parsing
+    """
+    parser = xy_parser()
+    for line in filelike:
+        parser.transit(line)
+
+    parser.error(filelike)
+    return parser.head_, parser.body_, parser.foot_
+
+
+@read.register
+def _(path: pathlib.Path) -> tuple[str, np.ndarray, str]:
     """
     Parses the xy file specified by path and returns a tuple consisting of error, header, body, and footer.
     パスで指定されたxyファイルをパースし、エラー、ヘッダ、ボディ、フットからなるタプルを返す.
 
     Parametors
     ---
         `path`:pathlib.Path
@@ -107,20 +147,47 @@
         `footer`:str
             path's file header
 
     Raises:
         ParseError:
             raise on fail parsing
     """
-
-    parser: xy_parser = xy_parser()
     with path.open() as xyfile:
+        return read(xyfile)
 
-        for line in xyfile:
-            parser.transit(line)
 
-    parser.error(xyfile)
-    return parser.head_, parser.body_, parser.foot_
+@read.register
+def _(path: str) -> tuple[str, np.ndarray, str]:
+    return read(pathlib.Path(path))
 
 
 def readstr(path: str) -> tuple[str, np.ndarray, str]:
     return read(pathlib.Path(path))
+
+
+class xrdXY(NamedTuple):
+    x: np.ndarray
+    y: np.ndarray
+
+
+@singledispatch
+def read2xy(filelike: TextIOBase) -> xrdXY:
+    """
+    Return
+    ---
+    (x,y):xrdXY
+        x:ndarray[30.0,30.1,...]
+        y:ndarray[10,13,...]
+    """
+    _, body, _ = read(filelike)
+    return xrdXY(body[:, 0], body[:, 1])
+
+
+@read2xy.register
+def _(path: pathlib.Path) -> xrdXY:
+    with path.open() as xyfile:
+        return read2xy(xyfile)
+
+
+@read2xy.register
+def _(path: str) -> xrdXY:
+    return read2xy(pathlib.Path(path))
```

