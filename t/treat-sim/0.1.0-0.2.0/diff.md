# Comparing `tmp/treat-sim-0.1.0.tar.gz` & `tmp/treat-sim-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "treat-sim-0.1.0.tar", last modified: Mon Oct 24 17:02:48 2022, max compression
+gzip compressed data, was "treat-sim-0.2.0.tar", last modified: Tue Jun 20 16:03:18 2023, max compression
```

## Comparing `treat-sim-0.1.0.tar` & `treat-sim-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2022-10-24 17:02:48.449374 treat-sim-0.1.0/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1066 2022-10-24 17:02:18.000000 treat-sim-0.1.0/LICENSE
--rw-rw-r--   0 tom       (1000) tom       (1000)       52 2022-10-24 16:53:06.000000 treat-sim-0.1.0/MANIFEST.in
--rw-rw-r--   0 tom       (1000) tom       (1000)     1866 2022-10-24 17:02:48.449374 treat-sim-0.1.0/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)     1266 2022-10-24 16:53:06.000000 treat-sim-0.1.0/README.md
--rw-rw-r--   0 tom       (1000) tom       (1000)       82 2022-10-24 16:53:06.000000 treat-sim-0.1.0/requirements.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       38 2022-10-24 17:02:48.449374 treat-sim-0.1.0/setup.cfg
--rw-rw-r--   0 tom       (1000) tom       (1000)     1817 2022-10-24 16:53:06.000000 treat-sim-0.1.0/setup.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2022-10-24 17:02:48.449374 treat-sim-0.1.0/treat_sim/
--rw-rw-r--   0 tom       (1000) tom       (1000)       45 2022-10-24 16:53:06.000000 treat-sim-0.1.0/treat_sim/__init__.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2022-10-24 17:02:48.449374 treat-sim-0.1.0/treat_sim/data/
--rw-rw-r--   0 tom       (1000) tom       (1000)      381 2022-10-24 16:53:06.000000 treat-sim-0.1.0/treat_sim/data/ed_arrivals.csv
--rw-rw-r--   0 tom       (1000) tom       (1000)     5895 2022-10-24 16:53:06.000000 treat-sim-0.1.0/treat_sim/distributions.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    37160 2022-10-24 16:53:06.000000 treat-sim-0.1.0/treat_sim/model.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2022-10-24 17:02:48.449374 treat-sim-0.1.0/treat_sim.egg-info/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1866 2022-10-24 17:02:48.000000 treat-sim-0.1.0/treat_sim.egg-info/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)      318 2022-10-24 17:02:48.000000 treat-sim-0.1.0/treat_sim.egg-info/SOURCES.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        1 2022-10-24 17:02:48.000000 treat-sim-0.1.0/treat_sim.egg-info/dependency_links.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       72 2022-10-24 17:02:48.000000 treat-sim-0.1.0/treat_sim.egg-info/requires.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       10 2022-10-24 17:02:48.000000 treat-sim-0.1.0/treat_sim.egg-info/top_level.txt
+drwxrwxr-x   0 tom       (1001) tom       (1001)        0 2023-06-20 16:03:18.712889 treat-sim-0.2.0/
+-rw-rw-r--   0 tom       (1001) tom       (1001)       52 2022-10-25 08:21:31.000000 treat-sim-0.2.0/MANIFEST.in
+-rw-rw-r--   0 tom       (1001) tom       (1001)     1824 2023-06-20 16:03:18.712889 treat-sim-0.2.0/PKG-INFO
+-rw-rw-r--   0 tom       (1001) tom       (1001)     1266 2022-10-25 08:21:31.000000 treat-sim-0.2.0/README.md
+-rw-rw-r--   0 tom       (1001) tom       (1001)       82 2023-06-20 16:00:11.000000 treat-sim-0.2.0/requirements.txt
+-rw-rw-r--   0 tom       (1001) tom       (1001)       38 2023-06-20 16:03:18.712889 treat-sim-0.2.0/setup.cfg
+-rw-rw-r--   0 tom       (1001) tom       (1001)     1817 2022-10-25 08:21:31.000000 treat-sim-0.2.0/setup.py
+drwxrwxr-x   0 tom       (1001) tom       (1001)        0 2023-06-20 16:03:18.712889 treat-sim-0.2.0/treat_sim/
+-rw-rw-r--   0 tom       (1001) tom       (1001)       45 2023-06-20 16:00:44.000000 treat-sim-0.2.0/treat_sim/__init__.py
+drwxrwxr-x   0 tom       (1001) tom       (1001)        0 2023-06-20 16:03:18.712889 treat-sim-0.2.0/treat_sim/data/
+-rw-rw-r--   0 tom       (1001) tom       (1001)      381 2022-10-25 08:21:31.000000 treat-sim-0.2.0/treat_sim/data/ed_arrivals.csv
+-rw-rw-r--   0 tom       (1001) tom       (1001)     5895 2022-10-25 08:21:31.000000 treat-sim-0.2.0/treat_sim/distributions.py
+-rw-rw-r--   0 tom       (1001) tom       (1001)    37160 2022-10-25 08:21:31.000000 treat-sim-0.2.0/treat_sim/model.py
+drwxrwxr-x   0 tom       (1001) tom       (1001)        0 2023-06-20 16:03:18.712889 treat-sim-0.2.0/treat_sim.egg-info/
+-rw-rw-r--   0 tom       (1001) tom       (1001)     1824 2023-06-20 16:03:18.000000 treat-sim-0.2.0/treat_sim.egg-info/PKG-INFO
+-rw-rw-r--   0 tom       (1001) tom       (1001)      310 2023-06-20 16:03:18.000000 treat-sim-0.2.0/treat_sim.egg-info/SOURCES.txt
+-rw-rw-r--   0 tom       (1001) tom       (1001)        1 2023-06-20 16:03:18.000000 treat-sim-0.2.0/treat_sim.egg-info/dependency_links.txt
+-rw-rw-r--   0 tom       (1001) tom       (1001)       72 2023-06-20 16:03:18.000000 treat-sim-0.2.0/treat_sim.egg-info/requires.txt
+-rw-rw-r--   0 tom       (1001) tom       (1001)       10 2023-06-20 16:03:18.000000 treat-sim-0.2.0/treat_sim.egg-info/top_level.txt
```

### Comparing `treat-sim-0.1.0/PKG-INFO` & `treat-sim-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: treat-sim
-Version: 0.1.0
+Version: 0.2.0
 Summary: A free and open implementation of the Treatment Centre Model from Nelson (2013)
 Home-page: https://github.com/TomMonks/treatment-centre-sim
 Author: Thomas Monks
 Author-email: forecast-tools@gmail.com
 License: The MIT License (MIT)
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8.12
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/TomMonks/treatment-centre-sim/HEAD)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-360+/)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6497477.svg)](https://doi.org/10.5281/zenodo.6497477)
 [<img src="https://img.shields.io/static/v1?label=dockerhub&message=images&color=important?style=for-the-badge&logo=docker">](https://hub.docker.com/r/tommonks01/treat_sim)
 
@@ -28,9 +26,7 @@
 
 The repo contains an free and open implementation of the Treatment Centre Model from Nelson (2013).  It is published under a permissive MIT license.
 
 ## References
 
 1. *Monks.T, Harper.A, Anagnoustou. A, Allen.M, Taylor.S. (2022) Open Science for Computer Simulation*
 2. *Nelson. B.L. (2013). [Foundations and methods of stochastic simulation](https://www.amazon.co.uk/Foundations-Methods-Stochastic-Simulation-International/dp/1461461596/ref=sr_1_1?dchild=1&keywords=foundations+and+methods+of+stochastic+simulation&qid=1617050801&sr=8-1). Springer.* 
-
-
```

### Comparing `treat-sim-0.1.0/README.md` & `treat-sim-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `treat-sim-0.1.0/setup.py` & `treat-sim-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `treat-sim-0.1.0/treat_sim/distributions.py` & `treat-sim-0.2.0/treat_sim/distributions.py`

 * *Files identical despite different names*

### Comparing `treat-sim-0.1.0/treat_sim/model.py` & `treat-sim-0.2.0/treat_sim/model.py`

 * *Files identical despite different names*

### Comparing `treat-sim-0.1.0/treat_sim.egg-info/PKG-INFO` & `treat-sim-0.2.0/treat_sim.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: treat-sim
-Version: 0.1.0
+Version: 0.2.0
 Summary: A free and open implementation of the Treatment Centre Model from Nelson (2013)
 Home-page: https://github.com/TomMonks/treatment-centre-sim
 Author: Thomas Monks
 Author-email: forecast-tools@gmail.com
 License: The MIT License (MIT)
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8.12
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/TomMonks/treatment-centre-sim/HEAD)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-360+/)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6497477.svg)](https://doi.org/10.5281/zenodo.6497477)
 [<img src="https://img.shields.io/static/v1?label=dockerhub&message=images&color=important?style=for-the-badge&logo=docker">](https://hub.docker.com/r/tommonks01/treat_sim)
 
@@ -28,9 +26,7 @@
 
 The repo contains an free and open implementation of the Treatment Centre Model from Nelson (2013).  It is published under a permissive MIT license.
 
 ## References
 
 1. *Monks.T, Harper.A, Anagnoustou. A, Allen.M, Taylor.S. (2022) Open Science for Computer Simulation*
 2. *Nelson. B.L. (2013). [Foundations and methods of stochastic simulation](https://www.amazon.co.uk/Foundations-Methods-Stochastic-Simulation-International/dp/1461461596/ref=sr_1_1?dchild=1&keywords=foundations+and+methods+of+stochastic+simulation&qid=1617050801&sr=8-1). Springer.* 
-
-
```

