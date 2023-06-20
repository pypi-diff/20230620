# Comparing `tmp/graphflow-0.4.5.tar.gz` & `tmp/graphflow-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/graphflow-0.4.5.tar", last modified: Sat Oct 29 21:20:57 2022, max compression
+gzip compressed data, was "dist/graphflow-0.5.0.tar", last modified: Tue Jun 20 04:13:17 2023, max compression
```

## Comparing `graphflow-0.4.5.tar` & `graphflow-0.5.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-10-29 21:20:57.509150 graphflow-0.4.5/
--rw-r--r--   0 stephenhky   (501) staff       (20)      146 2022-10-04 23:36:26.000000 graphflow-0.4.5/MANIFEST.in
--rw-r--r--   0 stephenhky   (501) staff       (20)      993 2022-10-29 21:20:57.509400 graphflow-0.4.5/PKG-INFO
--rw-r--r--   0 stephenhky   (501) staff       (20)     2213 2022-10-29 21:20:22.000000 graphflow-0.4.5/README.md
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-10-29 21:20:57.480759 graphflow-0.4.5/graphflow/
--rw-r--r--   0 stephenhky   (501) staff       (20)      237 2021-12-15 05:18:21.000000 graphflow-0.4.5/graphflow/__init__.py
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-10-29 21:20:57.490049 graphflow-0.4.5/graphflow/hits/
--rw-r--r--   0 stephenhky   (501) staff       (20)       42 2021-04-10 22:07:35.000000 graphflow-0.4.5/graphflow/hits/__init__.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     1299 2021-04-19 21:42:11.000000 graphflow-0.4.5/graphflow/hits/hitsrank.py
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-10-29 21:20:57.498358 graphflow-0.4.5/graphflow/pagerank/
--rw-r--r--   0 stephenhky   (501) staff       (20)     1987 2021-12-31 23:15:19.000000 graphflow-0.4.5/graphflow/pagerank/GooglePageRank.py
--rw-r--r--   0 stephenhky   (501) staff       (20)        1 2021-12-15 05:18:21.000000 graphflow-0.4.5/graphflow/pagerank/__init__.py
--rw-r--r--   0 stephenhky   (501) staff       (20)   264250 2022-10-04 23:39:01.000000 graphflow-0.4.5/graphflow/pagerank/cpagerank.c
--rw-r--r--   0 stephenhky   (501) staff       (20)      672 2021-04-10 22:07:35.000000 graphflow-0.4.5/graphflow/pagerank/cpagerank.pyx
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-10-29 21:20:57.502843 graphflow-0.4.5/graphflow/simvoltage/
--rw-r--r--   0 stephenhky   (501) staff       (20)     7928 2021-04-19 21:42:11.000000 graphflow-0.4.5/graphflow/simvoltage/SocialNetworkSimVoltage.py
--rw-r--r--   0 stephenhky   (501) staff       (20)      113 2021-04-10 22:07:35.000000 graphflow-0.4.5/graphflow/simvoltage/__init__.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     2743 2021-04-19 21:42:11.000000 graphflow-0.4.5/graphflow/simvoltage/resistancedist.py
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-10-29 21:20:57.487932 graphflow-0.4.5/graphflow.egg-info/
--rw-r--r--   0 stephenhky   (501) staff       (20)      993 2022-10-29 21:20:57.000000 graphflow-0.4.5/graphflow.egg-info/PKG-INFO
--rw-r--r--   0 stephenhky   (501) staff       (20)      692 2022-10-29 21:20:57.000000 graphflow-0.4.5/graphflow.egg-info/SOURCES.txt
--rw-r--r--   0 stephenhky   (501) staff       (20)        1 2022-10-29 21:20:57.000000 graphflow-0.4.5/graphflow.egg-info/dependency_links.txt
--rw-r--r--   0 stephenhky   (501) staff       (20)        1 2022-10-04 23:39:01.000000 graphflow-0.4.5/graphflow.egg-info/not-zip-safe
--rw-r--r--   0 stephenhky   (501) staff       (20)       56 2022-10-29 21:20:57.000000 graphflow-0.4.5/graphflow.egg-info/requires.txt
--rw-r--r--   0 stephenhky   (501) staff       (20)       10 2022-10-29 21:20:57.000000 graphflow-0.4.5/graphflow.egg-info/top_level.txt
--rw-r--r--   0 stephenhky   (501) staff       (20)       83 2022-10-04 23:36:26.000000 graphflow-0.4.5/pyproject.toml
--rw-r--r--   0 stephenhky   (501) staff       (20)       56 2021-12-15 05:18:21.000000 graphflow-0.4.5/requirements.txt
--rw-r--r--   0 stephenhky   (501) staff       (20)       79 2022-10-29 21:20:57.510409 graphflow-0.4.5/setup.cfg
--rw-r--r--   0 stephenhky   (501) staff       (20)     1967 2022-10-29 21:20:22.000000 graphflow-0.4.5/setup.py
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-10-29 21:20:57.508283 graphflow-0.4.5/test/
--rw-r--r--   0 stephenhky   (501) staff       (20)      808 2021-12-15 05:18:21.000000 graphflow-0.4.5/test/test_hits.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     3685 2021-12-31 23:15:19.000000 graphflow-0.4.5/test/test_pagerank.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     1161 2021-04-10 22:07:36.000000 graphflow-0.4.5/test/test_simplecircuits.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     3261 2021-04-10 22:07:36.000000 graphflow-0.4.5/test/test_socialnetworks.py
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2023-06-20 04:13:17.683218 graphflow-0.5.0/
+-rw-r--r--   0 stephenhky   (501) staff       (20)      146 2022-10-04 23:36:26.000000 graphflow-0.5.0/MANIFEST.in
+-rw-r--r--   0 stephenhky   (501) staff       (20)      893 2023-06-20 04:13:17.683435 graphflow-0.5.0/PKG-INFO
+-rw-r--r--   0 stephenhky   (501) staff       (20)     2255 2023-06-20 03:53:57.000000 graphflow-0.5.0/README.md
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2023-06-20 04:13:17.656970 graphflow-0.5.0/graphflow/
+-rw-r--r--   0 stephenhky   (501) staff       (20)      237 2021-12-15 05:18:21.000000 graphflow-0.5.0/graphflow/__init__.py
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2023-06-20 04:13:17.665574 graphflow-0.5.0/graphflow/hits/
+-rw-r--r--   0 stephenhky   (501) staff       (20)       42 2021-04-10 22:07:35.000000 graphflow-0.5.0/graphflow/hits/__init__.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     1305 2023-06-20 03:53:57.000000 graphflow-0.5.0/graphflow/hits/hitsrank.py
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2023-06-20 04:13:17.675141 graphflow-0.5.0/graphflow/pagerank/
+-rw-r--r--   0 stephenhky   (501) staff       (20)     1987 2021-12-31 23:15:19.000000 graphflow-0.5.0/graphflow/pagerank/GooglePageRank.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)        1 2021-12-15 05:18:21.000000 graphflow-0.5.0/graphflow/pagerank/__init__.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)   264250 2022-10-04 23:39:01.000000 graphflow-0.5.0/graphflow/pagerank/cpagerank.c
+-rw-r--r--   0 stephenhky   (501) staff       (20)      672 2021-04-10 22:07:35.000000 graphflow-0.5.0/graphflow/pagerank/cpagerank.pyx
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2023-06-20 04:13:17.678268 graphflow-0.5.0/graphflow/simvoltage/
+-rw-r--r--   0 stephenhky   (501) staff       (20)     7928 2021-04-19 21:42:11.000000 graphflow-0.5.0/graphflow/simvoltage/SocialNetworkSimVoltage.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)      113 2021-04-10 22:07:35.000000 graphflow-0.5.0/graphflow/simvoltage/__init__.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     2746 2023-06-20 03:53:57.000000 graphflow-0.5.0/graphflow/simvoltage/resistancedist.py
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2023-06-20 04:13:17.663407 graphflow-0.5.0/graphflow.egg-info/
+-rw-r--r--   0 stephenhky   (501) staff       (20)      893 2023-06-20 04:13:17.000000 graphflow-0.5.0/graphflow.egg-info/PKG-INFO
+-rw-r--r--   0 stephenhky   (501) staff       (20)      692 2023-06-20 04:13:17.000000 graphflow-0.5.0/graphflow.egg-info/SOURCES.txt
+-rw-r--r--   0 stephenhky   (501) staff       (20)        1 2023-06-20 04:13:17.000000 graphflow-0.5.0/graphflow.egg-info/dependency_links.txt
+-rw-r--r--   0 stephenhky   (501) staff       (20)        1 2022-10-04 23:39:01.000000 graphflow-0.5.0/graphflow.egg-info/not-zip-safe
+-rw-r--r--   0 stephenhky   (501) staff       (20)       56 2023-06-20 04:13:17.000000 graphflow-0.5.0/graphflow.egg-info/requires.txt
+-rw-r--r--   0 stephenhky   (501) staff       (20)       10 2023-06-20 04:13:17.000000 graphflow-0.5.0/graphflow.egg-info/top_level.txt
+-rw-r--r--   0 stephenhky   (501) staff       (20)       83 2022-10-04 23:36:26.000000 graphflow-0.5.0/pyproject.toml
+-rw-r--r--   0 stephenhky   (501) staff       (20)       56 2023-06-20 03:53:57.000000 graphflow-0.5.0/requirements.txt
+-rw-r--r--   0 stephenhky   (501) staff       (20)       79 2023-06-20 04:13:17.684435 graphflow-0.5.0/setup.cfg
+-rw-r--r--   0 stephenhky   (501) staff       (20)     1990 2023-06-20 04:11:30.000000 graphflow-0.5.0/setup.py
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2023-06-20 04:13:17.682548 graphflow-0.5.0/test/
+-rw-r--r--   0 stephenhky   (501) staff       (20)      808 2021-12-15 05:18:21.000000 graphflow-0.5.0/test/test_hits.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     3685 2021-12-31 23:15:19.000000 graphflow-0.5.0/test/test_pagerank.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     1161 2021-04-10 22:07:36.000000 graphflow-0.5.0/test/test_simplecircuits.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     3262 2023-06-20 03:53:57.000000 graphflow-0.5.0/test/test_socialnetworks.py
```

### Comparing `graphflow-0.4.5/PKG-INFO` & `graphflow-0.5.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 1.1
 Name: graphflow
-Version: 0.4.5
+Version: 0.5.0
 Summary: Algorithms for Graph Flow Analysis
 Home-page: https://github.com/stephenhky/GraphFlow
 Author: Kwan-Yuet Ho
 Author-email: stephenhky@yahoo.com.hk
 License: MIT
 Description: Numerical routines for analyzing data represented by graphs
 Keywords: Algorithms for Graph Flow Analysis
 Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: C
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `graphflow-0.4.5/README.md` & `graphflow-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 ```
 >>> pip install -U graphflow
 ```
 
 # News
 
+* 06/20/2023: `graphflow` 0.5.0 released.
 * 10/29/2022: `graphflow` 0.4.5 released.
 * 10/04/2022: `graphflow` 0.4.4 released.
 * 12/31/2021: `graphflow` 0.4.3 released.
 * 12/15/2021: `graphflow` 0.4.2 released.
 * 04/19/2021: `graphflow` 0.4.1 released.
 * 04/10/2021: `graphflow` 0.4.0 released.
 * 04/09/2020: `graphflow` 0.3.0 released.
```

### Comparing `graphflow-0.4.5/graphflow/hits/hitsrank.py` & `graphflow-0.5.0/graphflow/hits/hitsrank.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,13 +40,13 @@
     """
 
     :param digraph:
     :param eps:
     :param maxstep:
     :return:
     """
-    A = nx.adj_matrix(digraph).toarray()
+    A = nx.adjacency_matrix(digraph).toarray()
     nodes = list(digraph.nodes())
     hubvec, authvec = hits(A, eps=eps, maxstep=maxstep)
     hubdict = {nodes[i]: hubvec[i] for i in range(len(hubvec))}
     authdict = {nodes[i]: authvec[i] for i in range(len(authvec))}
     return hubdict, authdict
```

### Comparing `graphflow-0.4.5/graphflow/pagerank/GooglePageRank.py` & `graphflow-0.5.0/graphflow/pagerank/GooglePageRank.py`

 * *Files identical despite different names*

### Comparing `graphflow-0.4.5/graphflow/pagerank/cpagerank.c` & `graphflow-0.5.0/graphflow/pagerank/cpagerank.c`

 * *Files identical despite different names*

### Comparing `graphflow-0.4.5/graphflow/pagerank/cpagerank.pyx` & `graphflow-0.5.0/graphflow/pagerank/cpagerank.pyx`

 * *Files identical despite different names*

### Comparing `graphflow-0.4.5/graphflow/simvoltage/SocialNetworkSimVoltage.py` & `graphflow-0.5.0/graphflow/simvoltage/SocialNetworkSimVoltage.py`

 * *Files identical despite different names*

### Comparing `graphflow-0.4.5/graphflow/simvoltage/resistancedist.py` & `graphflow-0.5.0/graphflow/simvoltage/resistancedist.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,27 +54,27 @@
         self.nodesIdx = {self.nodes[idx]: idx for idx in range(len(self.nodes))}
 
     def calculateDegreeMatrix(self):
         """
 
         :return:
         """
-        Dmatrix = dok_matrix((len(self.nodes), len(self.nodes)), dtype=np.float)
+        Dmatrix = dok_matrix((len(self.nodes), len(self.nodes)), dtype=np.float_)
         for edge in self.edges:
             for node in edge:
                 idx = self.nodesIdx[node]
                 Dmatrix[idx, idx] += 1
         return Dmatrix
         
     def calculateAdjacencyMatrix(self):
         """
 
         :return:
         """
-        Amatrix = dok_matrix((len(self.nodes), len(self.nodes)), dtype=np.float)
+        Amatrix = dok_matrix((len(self.nodes), len(self.nodes)), dtype=np.float_)
         for edge in self.edges:
             idx0 = self.nodesIdx[edge[0]]
             idx1 = self.nodesIdx[edge[1]]
             Amatrix[idx0, idx1] = 1
             Amatrix[idx1, idx0] = 1
         return Amatrix
         
@@ -83,12 +83,12 @@
 
         :return:
         """
         Dmatrix = self.calculateDegreeMatrix()
         Amatrix = self.calculateAdjacencyMatrix()
         Lmatrix = Dmatrix.toarray() - Amatrix.toarray()
         Lambda = np.linalg.pinv(Lmatrix)
-        Omega = dok_matrix((len(self.nodes), len(self.nodes)), dtype=np.float)
+        Omega = dok_matrix((len(self.nodes), len(self.nodes)), dtype=np.float_)
         for i in range(len(self.nodes)):
             for j in range(len(self.nodes)):
                 Omega[i, j] = Lambda[i, i] + Lambda[j, j] - 2 * Lambda[i, j]
         return Omega
```

### Comparing `graphflow-0.4.5/graphflow.egg-info/PKG-INFO` & `graphflow-0.5.0/graphflow.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 1.1
 Name: graphflow
-Version: 0.4.5
+Version: 0.5.0
 Summary: Algorithms for Graph Flow Analysis
 Home-page: https://github.com/stephenhky/GraphFlow
 Author: Kwan-Yuet Ho
 Author-email: stephenhky@yahoo.com.hk
 License: MIT
 Description: Numerical routines for analyzing data represented by graphs
 Keywords: Algorithms for Graph Flow Analysis
 Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: C
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `graphflow-0.4.5/graphflow.egg-info/SOURCES.txt` & `graphflow-0.5.0/graphflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graphflow-0.4.5/setup.py` & `graphflow-0.5.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 
-from setuptools import setup
+from setuptools import setup, Extension
 import numpy as np
 from Cython.Build import cythonize
 
 dynprog_ext_modules = cythonize(['graphflow/pagerank/cpagerank.pyx'])
+# dynprog_ext_modules = [
+#     Extension('graphflow.pagerank.cpagerank', ['graphflow/pagerank/cpagerank.c'])
+# ]
 
 
 def readme():
     with open('README.md') as f:
         return f.read()
 
 
 def install_requirements():
     return [package_string.strip() for package_string in open('requirements.txt', 'r')]
 
 
 setup(name='graphflow',
-      version="0.4.5",
+      version="0.5.0",
       description="Algorithms for Graph Flow Analysis",
       long_description="Numerical routines for analyzing data represented by graphs",
       classifiers=[
           "Topic :: Scientific/Engineering :: Artificial Intelligence",
           "Topic :: Scientific/Engineering :: Mathematics",
           "Topic :: Software Development :: Libraries :: Python Modules",
-          "Programming Language :: Python :: 3.6",
-          "Programming Language :: Python :: 3.7",
           "Programming Language :: Python :: 3.8",
           "Programming Language :: Python :: 3.9",
           "Programming Language :: Python :: 3.10",
           "Programming Language :: Python :: 3.11",
           "Programming Language :: Cython",
           "Programming Language :: C",
           "License :: OSI Approved :: MIT License",
```

### Comparing `graphflow-0.4.5/test/test_hits.py` & `graphflow-0.5.0/test/test_hits.py`

 * *Files identical despite different names*

### Comparing `graphflow-0.4.5/test/test_pagerank.py` & `graphflow-0.5.0/test/test_pagerank.py`

 * *Files identical despite different names*

### Comparing `graphflow-0.4.5/test/test_simplecircuits.py` & `graphflow-0.5.0/test/test_simplecircuits.py`

 * *Files identical despite different names*

### Comparing `graphflow-0.4.5/test/test_socialnetworks.py` & `graphflow-0.5.0/test/test_socialnetworks.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,15 +58,15 @@
                  ('Zoe', 'Wallace', 1)]
         wn1 = SocialNetworkSimVoltage(nodes=nodes, edges=edges, precalculated_distance=True)
 
         THIS_DIR = os.path.dirname(os.path.abspath(__file__))
         testresults = pd.read_csv(os.path.join(THIS_DIR, 'socialnetworkranks.csv'),
                                   header=None,
                                   names=['name1', 'name2', 'resistance'],
-                                  dtype={'name1': str, 'name2': str, 'resistance': np.float})
+                                  dtype={'name1': str, 'name2': str, 'resistance': np.float_})
 
         for _, row in testresults.iterrows():
             name1 = row['name1']
             name2 = row['name2']
             resistance = row['resistance']
             self.assertAlmostEqual(wn1.getResistance(name1, name2), resistance, places=3)
             print('%s\t%s : %.4f passed.' % (name1, name2, resistance))
```

