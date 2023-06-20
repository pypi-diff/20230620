# Comparing `tmp/GabrielGraph-0.0.1.tar.gz` & `tmp/GabrielGraph-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GabrielGraph-0.0.1.tar", last modified: Tue Jun 20 16:17:08 2023, max compression
+gzip compressed data, was "GabrielGraph-0.0.2.tar", last modified: Tue Jun 20 16:57:59 2023, max compression
```

## Comparing `GabrielGraph-0.0.1.tar` & `GabrielGraph-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-06-20 16:17:08.513317 GabrielGraph-0.0.1/
--rw-r--r--   0 leo.guignard   (501) staff       (20)     1081 2023-06-20 16:08:54.000000 GabrielGraph-0.0.1/LICENSE
--rw-r--r--   0 leo.guignard   (501) staff       (20)       96 2023-06-20 16:08:54.000000 GabrielGraph-0.0.1/MANIFEST.in
--rw-r--r--   0 leo.guignard   (501) staff       (20)     3433 2023-06-20 16:17:08.513385 GabrielGraph-0.0.1/PKG-INFO
--rw-r--r--   0 leo.guignard   (501) staff       (20)     2232 2023-06-20 16:08:54.000000 GabrielGraph-0.0.1/README.md
--rw-r--r--   0 leo.guignard   (501) staff       (20)      571 2023-06-20 16:08:54.000000 GabrielGraph-0.0.1/pyproject.toml
--rw-r--r--   0 leo.guignard   (501) staff       (20)     1472 2023-06-20 16:17:08.513705 GabrielGraph-0.0.1/setup.cfg
-drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-06-20 16:17:08.511030 GabrielGraph-0.0.1/src/
-drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-06-20 16:17:08.512285 GabrielGraph-0.0.1/src/GabrielGraph.egg-info/
--rw-r--r--   0 leo.guignard   (501) staff       (20)     3433 2023-06-20 16:17:08.000000 GabrielGraph-0.0.1/src/GabrielGraph.egg-info/PKG-INFO
--rw-r--r--   0 leo.guignard   (501) staff       (20)      391 2023-06-20 16:17:08.000000 GabrielGraph-0.0.1/src/GabrielGraph.egg-info/SOURCES.txt
--rw-r--r--   0 leo.guignard   (501) staff       (20)        1 2023-06-20 16:17:08.000000 GabrielGraph-0.0.1/src/GabrielGraph.egg-info/dependency_links.txt
--rw-r--r--   0 leo.guignard   (501) staff       (20)       53 2023-06-20 16:17:08.000000 GabrielGraph-0.0.1/src/GabrielGraph.egg-info/requires.txt
--rw-r--r--   0 leo.guignard   (501) staff       (20)       13 2023-06-20 16:17:08.000000 GabrielGraph-0.0.1/src/GabrielGraph.egg-info/top_level.txt
-drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-06-20 16:17:08.512692 GabrielGraph-0.0.1/src/gabrielgraph/
--rw-r--r--   0 leo.guignard   (501) staff       (20)       82 2023-06-20 16:12:26.000000 GabrielGraph-0.0.1/src/gabrielgraph/__init__.py
--rw-r--r--   0 leo.guignard   (501) staff       (20)     3320 2023-06-20 16:12:06.000000 GabrielGraph-0.0.1/src/gabrielgraph/_gabrielgraph.py
-drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-06-20 16:17:08.513181 GabrielGraph-0.0.1/src/gabrielgraph/_tests/
--rw-r--r--   0 leo.guignard   (501) staff       (20)        0 2023-06-20 16:08:54.000000 GabrielGraph-0.0.1/src/gabrielgraph/_tests/__init__.py
--rw-r--r--   0 leo.guignard   (501) staff       (20)      157 2023-06-20 16:08:54.000000 GabrielGraph-0.0.1/src/gabrielgraph/_tests/test_module.py
+drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-06-20 16:57:59.088027 GabrielGraph-0.0.2/
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     1081 2023-06-20 16:08:54.000000 GabrielGraph-0.0.2/LICENSE
+-rw-r--r--   0 leo.guignard   (501) staff       (20)       96 2023-06-20 16:08:54.000000 GabrielGraph-0.0.2/MANIFEST.in
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     3433 2023-06-20 16:57:59.088083 GabrielGraph-0.0.2/PKG-INFO
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     2232 2023-06-20 16:08:54.000000 GabrielGraph-0.0.2/README.md
+-rw-r--r--   0 leo.guignard   (501) staff       (20)      571 2023-06-20 16:55:49.000000 GabrielGraph-0.0.2/pyproject.toml
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     1472 2023-06-20 16:57:59.088366 GabrielGraph-0.0.2/setup.cfg
+drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-06-20 16:57:59.085586 GabrielGraph-0.0.2/src/
+drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-06-20 16:57:59.087021 GabrielGraph-0.0.2/src/GabrielGraph.egg-info/
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     3433 2023-06-20 16:57:59.000000 GabrielGraph-0.0.2/src/GabrielGraph.egg-info/PKG-INFO
+-rw-r--r--   0 leo.guignard   (501) staff       (20)      391 2023-06-20 16:57:59.000000 GabrielGraph-0.0.2/src/GabrielGraph.egg-info/SOURCES.txt
+-rw-r--r--   0 leo.guignard   (501) staff       (20)        1 2023-06-20 16:57:59.000000 GabrielGraph-0.0.2/src/GabrielGraph.egg-info/dependency_links.txt
+-rw-r--r--   0 leo.guignard   (501) staff       (20)       53 2023-06-20 16:57:59.000000 GabrielGraph-0.0.2/src/GabrielGraph.egg-info/requires.txt
+-rw-r--r--   0 leo.guignard   (501) staff       (20)       13 2023-06-20 16:57:59.000000 GabrielGraph-0.0.2/src/GabrielGraph.egg-info/top_level.txt
+drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-06-20 16:57:59.087384 GabrielGraph-0.0.2/src/gabrielgraph/
+-rw-r--r--   0 leo.guignard   (501) staff       (20)       82 2023-06-20 16:55:49.000000 GabrielGraph-0.0.2/src/gabrielgraph/__init__.py
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     3351 2023-06-20 16:50:44.000000 GabrielGraph-0.0.2/src/gabrielgraph/_gabrielgraph.py
+drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-06-20 16:57:59.087756 GabrielGraph-0.0.2/src/gabrielgraph/_tests/
+-rw-r--r--   0 leo.guignard   (501) staff       (20)        0 2023-06-20 16:08:54.000000 GabrielGraph-0.0.2/src/gabrielgraph/_tests/__init__.py
+-rw-r--r--   0 leo.guignard   (501) staff       (20)      513 2023-06-20 16:29:33.000000 GabrielGraph-0.0.2/src/gabrielgraph/_tests/test_module.py
```

### Comparing `GabrielGraph-0.0.1/LICENSE` & `GabrielGraph-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `GabrielGraph-0.0.1/PKG-INFO` & `GabrielGraph-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GabrielGraph
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small class to create Gabriel Graphs
 Home-page: https://github.com/GuignardLab/GabrielGraph
 Author: Leo Guignard
 Author-email: leo.guignard@univ-amu.fr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/GuignardLab/GabrielGraph/issues
 Project-URL: Documentation, https://github.com/GuignardLab/GabrielGraph#README.md
```

### Comparing `GabrielGraph-0.0.1/README.md` & `GabrielGraph-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `GabrielGraph-0.0.1/pyproject.toml` & `GabrielGraph-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 [tool.isort]
 profile = "black"
 line_length = 79
 
 
 [tool.bumpver]
-current_version = "0.0.1"
+current_version = "0.0.2"
 version_pattern = "MAJOR.MINOR.PATCH[-TAG]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `GabrielGraph-0.0.1/setup.cfg` & `GabrielGraph-0.0.2/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = GabrielGraph
-version = 0.0.1
+version = 0.0.2
 description = A small class to create Gabriel Graphs
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/GuignardLab/GabrielGraph
 author = Leo Guignard
 author_email = leo.guignard@univ-amu.fr
 license = MIT
```

### Comparing `GabrielGraph-0.0.1/src/GabrielGraph.egg-info/PKG-INFO` & `GabrielGraph-0.0.2/src/GabrielGraph.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GabrielGraph
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small class to create Gabriel Graphs
 Home-page: https://github.com/GuignardLab/GabrielGraph
 Author: Leo Guignard
 Author-email: leo.guignard@univ-amu.fr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/GuignardLab/GabrielGraph/issues
 Project-URL: Documentation, https://github.com/GuignardLab/GabrielGraph#README.md
```

### Comparing `GabrielGraph-0.0.1/src/gabrielgraph/_gabrielgraph.py` & `GabrielGraph-0.0.2/src/gabrielgraph/_gabrielgraph.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,18 @@
         pos (n x m ndarray): ndarray of the positions where n is
             the number of nodes and m is the spatial dimension
         data_struct (str): in which type of data structure will
             the graph be saved, currently either 'adj-dict' and
             'adj-mat' are supported.
             'adj-dict': Adjacency dictionary
             'adj-mat' : Adjacency matrix
-        dist (bool)
+        dist (bool): in the case of adjacency matrix, put the L2 norm
+            between the points if they are connected rather than True.
+            /!\ Note that if the distance is asked, for pratical reason
+            (because of sparse matrices), no connection is coded as 0. /!\
     Returns:
         final_GG (dict id: set([ids, ])): the gabriel graph as
             an adjacency list, a dictionary that maps node ids
             to the list of neighboring node ids
     """
     if not data_struct in ["adj-dict", "adj-mat"]:
         raise ValueError(
@@ -48,21 +51,17 @@
                     for i in neighbs.intersection(delaunay_graph[ni])
                 ):
                     Gabriel_graph.setdefault(e1, set()).add(ni)
                     Gabriel_graph.setdefault(ni, set()).add(e1)
 
         final_GG = {}
         for e1, neighbs in Gabriel_graph.items():
-            neighbs = np.array(list(neighbs))
-            distances = np.linalg.norm(
-                pos[e1] - [pos[ni] for ni in neighbs], axis=1
-            )
             final_GG[node_ids[e1]] = {
                 node_ids[ni]
-                for ni in neighbs[distances <= 5 * np.median(distances)]
+                for ni in neighbs
             }
 
     elif data_struct.lower() == "adj-mat":
         X, Y, val = [], [], []
         for e1, neighbs in delaunay_graph.items():
             for ni in [n for n in neighbs if e1 < n]:
                 D = np.linalg.norm(pos[e1] - pos[ni])
@@ -80,10 +79,9 @@
                         val.append(D)
                     else:
                         val.append(True)
                         val.append(True)
         final_GG = sp.sparse.coo_array(
             (val, (X, Y)), shape=(max(node_ids) + 1, max(node_ids) + 1)
         )
-        final_GG = final_GG.tocsr()
 
     return final_GG
```

