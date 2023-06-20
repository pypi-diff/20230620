# Comparing `tmp/GabrielGraph-0.0.2.tar.gz` & `tmp/GabrielGraph-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GabrielGraph-0.0.2.tar", last modified: Tue Jun 20 16:57:59 2023, max compression
+gzip compressed data, was "GabrielGraph-0.0.3.tar", last modified: Tue Jun 20 17:14:35 2023, max compression
```

## Comparing `GabrielGraph-0.0.2.tar` & `GabrielGraph-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-06-20 16:57:59.088027 GabrielGraph-0.0.2/
--rw-r--r--   0 leo.guignard   (501) staff       (20)     1081 2023-06-20 16:08:54.000000 GabrielGraph-0.0.2/LICENSE
--rw-r--r--   0 leo.guignard   (501) staff       (20)       96 2023-06-20 16:08:54.000000 GabrielGraph-0.0.2/MANIFEST.in
--rw-r--r--   0 leo.guignard   (501) staff       (20)     3433 2023-06-20 16:57:59.088083 GabrielGraph-0.0.2/PKG-INFO
--rw-r--r--   0 leo.guignard   (501) staff       (20)     2232 2023-06-20 16:08:54.000000 GabrielGraph-0.0.2/README.md
--rw-r--r--   0 leo.guignard   (501) staff       (20)      571 2023-06-20 16:55:49.000000 GabrielGraph-0.0.2/pyproject.toml
--rw-r--r--   0 leo.guignard   (501) staff       (20)     1472 2023-06-20 16:57:59.088366 GabrielGraph-0.0.2/setup.cfg
-drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-06-20 16:57:59.085586 GabrielGraph-0.0.2/src/
-drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-06-20 16:57:59.087021 GabrielGraph-0.0.2/src/GabrielGraph.egg-info/
--rw-r--r--   0 leo.guignard   (501) staff       (20)     3433 2023-06-20 16:57:59.000000 GabrielGraph-0.0.2/src/GabrielGraph.egg-info/PKG-INFO
--rw-r--r--   0 leo.guignard   (501) staff       (20)      391 2023-06-20 16:57:59.000000 GabrielGraph-0.0.2/src/GabrielGraph.egg-info/SOURCES.txt
--rw-r--r--   0 leo.guignard   (501) staff       (20)        1 2023-06-20 16:57:59.000000 GabrielGraph-0.0.2/src/GabrielGraph.egg-info/dependency_links.txt
--rw-r--r--   0 leo.guignard   (501) staff       (20)       53 2023-06-20 16:57:59.000000 GabrielGraph-0.0.2/src/GabrielGraph.egg-info/requires.txt
--rw-r--r--   0 leo.guignard   (501) staff       (20)       13 2023-06-20 16:57:59.000000 GabrielGraph-0.0.2/src/GabrielGraph.egg-info/top_level.txt
-drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-06-20 16:57:59.087384 GabrielGraph-0.0.2/src/gabrielgraph/
--rw-r--r--   0 leo.guignard   (501) staff       (20)       82 2023-06-20 16:55:49.000000 GabrielGraph-0.0.2/src/gabrielgraph/__init__.py
--rw-r--r--   0 leo.guignard   (501) staff       (20)     3351 2023-06-20 16:50:44.000000 GabrielGraph-0.0.2/src/gabrielgraph/_gabrielgraph.py
-drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-06-20 16:57:59.087756 GabrielGraph-0.0.2/src/gabrielgraph/_tests/
--rw-r--r--   0 leo.guignard   (501) staff       (20)        0 2023-06-20 16:08:54.000000 GabrielGraph-0.0.2/src/gabrielgraph/_tests/__init__.py
--rw-r--r--   0 leo.guignard   (501) staff       (20)      513 2023-06-20 16:29:33.000000 GabrielGraph-0.0.2/src/gabrielgraph/_tests/test_module.py
+drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-06-20 17:14:35.169866 GabrielGraph-0.0.3/
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     1081 2023-06-20 16:08:54.000000 GabrielGraph-0.0.3/LICENSE
+-rw-r--r--   0 leo.guignard   (501) staff       (20)       96 2023-06-20 16:08:54.000000 GabrielGraph-0.0.3/MANIFEST.in
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     3433 2023-06-20 17:14:35.169944 GabrielGraph-0.0.3/PKG-INFO
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     2232 2023-06-20 16:08:54.000000 GabrielGraph-0.0.3/README.md
+-rw-r--r--   0 leo.guignard   (501) staff       (20)      571 2023-06-20 17:13:02.000000 GabrielGraph-0.0.3/pyproject.toml
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     1463 2023-06-20 17:14:35.170705 GabrielGraph-0.0.3/setup.cfg
+drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-06-20 17:14:35.167458 GabrielGraph-0.0.3/src/
+drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-06-20 17:14:35.168839 GabrielGraph-0.0.3/src/GabrielGraph.egg-info/
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     3433 2023-06-20 17:14:35.000000 GabrielGraph-0.0.3/src/GabrielGraph.egg-info/PKG-INFO
+-rw-r--r--   0 leo.guignard   (501) staff       (20)      391 2023-06-20 17:14:35.000000 GabrielGraph-0.0.3/src/GabrielGraph.egg-info/SOURCES.txt
+-rw-r--r--   0 leo.guignard   (501) staff       (20)        1 2023-06-20 17:14:35.000000 GabrielGraph-0.0.3/src/GabrielGraph.egg-info/dependency_links.txt
+-rw-r--r--   0 leo.guignard   (501) staff       (20)       45 2023-06-20 17:14:35.000000 GabrielGraph-0.0.3/src/GabrielGraph.egg-info/requires.txt
+-rw-r--r--   0 leo.guignard   (501) staff       (20)       13 2023-06-20 17:14:35.000000 GabrielGraph-0.0.3/src/GabrielGraph.egg-info/top_level.txt
+drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-06-20 17:14:35.169304 GabrielGraph-0.0.3/src/gabrielgraph/
+-rw-r--r--   0 leo.guignard   (501) staff       (20)       81 2023-06-20 17:13:02.000000 GabrielGraph-0.0.3/src/gabrielgraph/__init__.py
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     3376 2023-06-20 17:09:39.000000 GabrielGraph-0.0.3/src/gabrielgraph/_gabrielgraph.py
+drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-06-20 17:14:35.169686 GabrielGraph-0.0.3/src/gabrielgraph/_tests/
+-rw-r--r--   0 leo.guignard   (501) staff       (20)        0 2023-06-20 16:08:54.000000 GabrielGraph-0.0.3/src/gabrielgraph/_tests/__init__.py
+-rw-r--r--   0 leo.guignard   (501) staff       (20)      516 2023-06-20 17:02:29.000000 GabrielGraph-0.0.3/src/gabrielgraph/_tests/test_module.py
```

### Comparing `GabrielGraph-0.0.2/LICENSE` & `GabrielGraph-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `GabrielGraph-0.0.2/PKG-INFO` & `GabrielGraph-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GabrielGraph
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small class to create Gabriel Graphs
 Home-page: https://github.com/GuignardLab/GabrielGraph
 Author: Leo Guignard
 Author-email: leo.guignard@univ-amu.fr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/GuignardLab/GabrielGraph/issues
 Project-URL: Documentation, https://github.com/GuignardLab/GabrielGraph#README.md
```

### Comparing `GabrielGraph-0.0.2/README.md` & `GabrielGraph-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `GabrielGraph-0.0.2/pyproject.toml` & `GabrielGraph-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 [tool.isort]
 profile = "black"
 line_length = 79
 
 
 [tool.bumpver]
-current_version = "0.0.2"
+current_version = "0.0.3"
 version_pattern = "MAJOR.MINOR.PATCH[-TAG]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `GabrielGraph-0.0.2/setup.cfg` & `GabrielGraph-0.0.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = GabrielGraph
-version = 0.0.2
+version = 0.0.3
 description = A small class to create Gabriel Graphs
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/GuignardLab/GabrielGraph
 author = Leo Guignard
 author_email = leo.guignard@univ-amu.fr
 license = MIT
@@ -28,15 +28,14 @@
 	User Support = https://github.com/GuignardLab/GabrielGraph/issues
 
 [options]
 packages = find:
 install_requires = 
 	numpy
 	scipy
-	bumpver
 python_requires = >=3.8
 include_package_data = True
 package_dir = 
 	=src
 
 [options.packages.find]
 where = src
```

### Comparing `GabrielGraph-0.0.2/src/GabrielGraph.egg-info/PKG-INFO` & `GabrielGraph-0.0.3/src/GabrielGraph.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GabrielGraph
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small class to create Gabriel Graphs
 Home-page: https://github.com/GuignardLab/GabrielGraph
 Author: Leo Guignard
 Author-email: leo.guignard@univ-amu.fr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/GuignardLab/GabrielGraph/issues
 Project-URL: Documentation, https://github.com/GuignardLab/GabrielGraph#README.md
```

### Comparing `GabrielGraph-0.0.2/src/gabrielgraph/_gabrielgraph.py` & `GabrielGraph-0.0.3/src/gabrielgraph/_gabrielgraph.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 """
 You should write your module/set of function/class(es) here
 """
 import numpy as np
 from scipy.spatial import Delaunay
 from itertools import combinations
 import scipy as sp
+from typing import Union
 
-def build_gabriel_graph(node_ids, pos, data_struct="adj-dict", dist=False):
+
+def build_gabriel_graph(
+    node_ids: np.ndarray,
+    pos: np.ndarray,
+    data_struct: str = "adj-dict",
+    dist: bool = False,
+) -> Union[dict, np.ndarray]:
     """
     Build the gabriel graph of a set of nodes with
     associtated positions.
 
     Args:
         node_ids ([int, ] (size n)): list of node ids
         pos (n x m ndarray): ndarray of the positions where n is
@@ -19,24 +26,22 @@
             the graph be saved, currently either 'adj-dict' and
             'adj-mat' are supported.
             'adj-dict': Adjacency dictionary
             'adj-mat' : Adjacency matrix
         dist (bool): in the case of adjacency matrix, put the L2 norm
             between the points if they are connected rather than True.
             /!\ Note that if the distance is asked, for pratical reason
-            (because of sparse matrices), no connection is coded as 0. /!\
+            (because of sparse matrices), no connection is coded as 0. /!\\
     Returns:
         final_GG (dict id: set([ids, ])): the gabriel graph as
             an adjacency list, a dictionary that maps node ids
             to the list of neighboring node ids
     """
     if not data_struct in ["adj-dict", "adj-mat"]:
-        raise ValueError(
-            "Data structure for the Gabriel graph not understood"
-        )
+        raise ValueError("Data structure for the Gabriel graph not understood")
     tmp = Delaunay(pos)
     delaunay_graph = {}
 
     for N in tmp.simplices:
         for e1, e2 in combinations(np.sort(N), 2):
             delaunay_graph.setdefault(e1, set()).add(e2)
             delaunay_graph.setdefault(e2, set()).add(e1)
@@ -51,27 +56,23 @@
                     for i in neighbs.intersection(delaunay_graph[ni])
                 ):
                     Gabriel_graph.setdefault(e1, set()).add(ni)
                     Gabriel_graph.setdefault(ni, set()).add(e1)
 
         final_GG = {}
         for e1, neighbs in Gabriel_graph.items():
-            final_GG[node_ids[e1]] = {
-                node_ids[ni]
-                for ni in neighbs
-            }
+            final_GG[node_ids[e1]] = {node_ids[ni] for ni in neighbs}
 
     elif data_struct.lower() == "adj-mat":
         X, Y, val = [], [], []
         for e1, neighbs in delaunay_graph.items():
             for ni in [n for n in neighbs if e1 < n]:
                 D = np.linalg.norm(pos[e1] - pos[ni])
                 if not any(
-                    np.linalg.norm((pos[ni] + pos[e1]) / 2 - pos[i])
-                    < D / 2
+                    np.linalg.norm((pos[ni] + pos[e1]) / 2 - pos[i]) < D / 2
                     for i in neighbs.intersection(delaunay_graph[ni])
                 ):
                     X.append(node_ids[e1])
                     Y.append(node_ids[ni])
                     X.append(node_ids[ni])
                     Y.append(node_ids[e1])
                     if dist:
@@ -80,8 +81,8 @@
                     else:
                         val.append(True)
                         val.append(True)
         final_GG = sp.sparse.coo_array(
             (val, (X, Y)), shape=(max(node_ids) + 1, max(node_ids) + 1)
         )
 
-    return final_GG
+    return final_GG
```

### Comparing `GabrielGraph-0.0.2/src/gabrielgraph/_tests/test_module.py` & `GabrielGraph-0.0.3/src/gabrielgraph/_tests/test_module.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from gabrielgraph import build_gabriel_graph
 import numpy as np
 
+
 def test_module():
     """You should write tests here!"""
     np.random.seed(0)
     ids = np.arange(10)
     pos = np.random.rand(20).reshape(-1, 2)
     test_obj = build_gabriel_graph(ids, pos)
     assert test_obj == {
@@ -13,9 +14,9 @@
         1: {0, 2, 5},
         3: {0, 2, 6, 8},
         7: {2, 8},
         8: {2, 3, 7},
         5: {1, 4, 9},
         4: {5},
         9: {0, 5, 6},
-        6: {0, 3, 9}
-    }
+        6: {0, 3, 9},
+    }
```

