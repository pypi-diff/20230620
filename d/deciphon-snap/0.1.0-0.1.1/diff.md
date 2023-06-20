# Comparing `tmp/deciphon_snap-0.1.0.tar.gz` & `tmp/deciphon_snap-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deciphon_snap-0.1.0.tar", max compression
+gzip compressed data, was "deciphon_snap-0.1.1.tar", max compression
```

## Comparing `deciphon_snap-0.1.0.tar` & `deciphon_snap-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1063 2023-06-19 20:36:33.678696 deciphon_snap-0.1.0/LICENSE
--rw-r--r--   0        0        0     2453 2023-06-19 20:36:33.678696 deciphon_snap-0.1.0/README.md
--rw-r--r--   0        0        0      275 2023-06-19 20:36:33.678696 deciphon_snap-0.1.0/deciphon_snap/hit.py
--rw-r--r--   0        0        0      607 2023-06-19 20:36:33.678696 deciphon_snap-0.1.0/deciphon_snap/match.py
--rw-r--r--   0        0        0      563 2023-06-19 20:36:33.678696 deciphon_snap-0.1.0/deciphon_snap/match_list.py
--rw-r--r--   0        0        0       72 2023-06-19 20:36:33.678696 deciphon_snap-0.1.0/deciphon_snap/path_like.py
--rw-r--r--   0        0        0      245 2023-06-19 20:36:33.678696 deciphon_snap-0.1.0/deciphon_snap/prod.py
--rw-r--r--   0        0        0      352 2023-06-19 20:36:33.678696 deciphon_snap-0.1.0/deciphon_snap/prod_list.py
--rw-r--r--   0        0        0      251 2023-06-19 20:36:33.678696 deciphon_snap-0.1.0/deciphon_snap/read_snap.py
--rw-r--r--   0        0        0      343 2023-06-19 20:36:33.678696 deciphon_snap-0.1.0/deciphon_snap/shorten.py
--rw-r--r--   0        0        0     1962 2023-06-19 20:36:33.678696 deciphon_snap-0.1.0/deciphon_snap/snap_file.py
--rw-r--r--   0        0        0      157 2023-06-19 20:36:33.678696 deciphon_snap-0.1.0/deciphon_snap/stringify.py
--rw-r--r--   0        0        0      521 2023-06-19 20:36:33.678696 deciphon_snap-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3055 1970-01-01 00:00:00.000000 deciphon_snap-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-20 10:58:55.718808 deciphon_snap-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2453 2023-06-20 10:58:55.718808 deciphon_snap-0.1.1/README.md
+-rw-r--r--   0        0        0      275 2023-06-20 10:58:55.718808 deciphon_snap-0.1.1/deciphon_snap/hit.py
+-rw-r--r--   0        0        0      607 2023-06-20 10:58:55.718808 deciphon_snap-0.1.1/deciphon_snap/match.py
+-rw-r--r--   0        0        0      563 2023-06-20 10:58:55.718808 deciphon_snap-0.1.1/deciphon_snap/match_list.py
+-rw-r--r--   0        0        0       72 2023-06-20 10:58:55.718808 deciphon_snap-0.1.1/deciphon_snap/path_like.py
+-rw-r--r--   0        0        0      257 2023-06-20 10:58:55.718808 deciphon_snap-0.1.1/deciphon_snap/prod.py
+-rw-r--r--   0        0        0      360 2023-06-20 10:58:55.718808 deciphon_snap-0.1.1/deciphon_snap/prod_list.py
+-rw-r--r--   0        0        0      251 2023-06-20 10:58:55.718808 deciphon_snap-0.1.1/deciphon_snap/read_snap.py
+-rw-r--r--   0        0        0      343 2023-06-20 10:58:55.718808 deciphon_snap-0.1.1/deciphon_snap/shorten.py
+-rw-r--r--   0        0        0     2010 2023-06-20 10:58:55.718808 deciphon_snap-0.1.1/deciphon_snap/snap_file.py
+-rw-r--r--   0        0        0      157 2023-06-20 10:58:55.718808 deciphon_snap-0.1.1/deciphon_snap/stringify.py
+-rw-r--r--   0        0        0      521 2023-06-20 10:58:55.718808 deciphon_snap-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3055 1970-01-01 00:00:00.000000 deciphon_snap-0.1.1/PKG-INFO
```

### Comparing `deciphon_snap-0.1.0/LICENSE` & `deciphon_snap-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.1.0/README.md` & `deciphon_snap-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.1.0/deciphon_snap/match.py` & `deciphon_snap-0.1.1/deciphon_snap/match.py`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.1.0/deciphon_snap/match_list.py` & `deciphon_snap-0.1.1/deciphon_snap/match_list.py`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.1.0/deciphon_snap/snap_file.py` & `deciphon_snap-0.1.1/deciphon_snap/snap_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-import csv
+from csv import DictReader
 from typing import List
 
 import prettytable as pt
 
 from deciphon_snap.match_list import MatchList
 from deciphon_snap.prod import Prod
 from deciphon_snap.prod_list import ProdList
@@ -50,17 +50,18 @@
 
         header = f"shape: ({num_products}, {num_fields})"
         return header + "\n" + x.get_string()
 
 
 def read_products(file):
     prods: List[Prod] = []
-    for row in csv.DictReader((stringify(i) for i in file), delimiter="\t"):
+    for i, row in enumerate(DictReader((stringify(i) for i in file), delimiter="\t")):
         prods.append(
             Prod(
+                id=i,
                 seq_id=int(row["seq_id"]),
                 profile=str(row["profile"]),
                 abc=str(row["abc"]),
                 alt=float(row["alt"]),
                 null=float(row["null"]),
                 evalue=float(row["evalue"]),
                 match_list=MatchList.from_string(str(row["match"])),
```

### Comparing `deciphon_snap-0.1.0/pyproject.toml` & `deciphon_snap-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deciphon-snap"
-version = "0.1.0"
+version = "0.1.1"
 description = "Reader for Deciphon snap files."
 authors = ["Danilo Horta <horta@ebi.ac.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "deciphon_snap" }]
 
 [tool.poetry.dependencies]
```

### Comparing `deciphon_snap-0.1.0/PKG-INFO` & `deciphon_snap-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deciphon-snap
-Version: 0.1.0
+Version: 0.1.1
 Summary: Reader for Deciphon snap files.
 License: MIT
 Author: Danilo Horta
 Author-email: horta@ebi.ac.uk
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

