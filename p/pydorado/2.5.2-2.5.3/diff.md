# Comparing `tmp/pydorado-2.5.2.tar.gz` & `tmp/pydorado-2.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydorado-2.5.2.tar", last modified: Tue Dec  6 03:13:31 2022, max compression
+gzip compressed data, was "pydorado-2.5.3.tar", last modified: Tue Jun 20 20:55:55 2023, max compression
```

## Comparing `pydorado-2.5.2.tar` & `pydorado-2.5.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:13:31.743794 pydorado-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (122)     1074 2022-12-06 03:13:03.000000 pydorado-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      573 2022-12-06 03:13:31.743794 pydorado-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2828 2022-12-06 03:13:03.000000 pydorado-2.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:13:31.743794 pydorado-2.5.2/dorado/
--rw-r--r--   0 runner    (1001) docker     (122)      138 2022-12-06 03:13:03.000000 pydorado-2.5.2/dorado/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:13:31.743794 pydorado-2.5.2/dorado/example_data/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-06 03:13:03.000000 pydorado-2.5.2/dorado/example_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1645 2022-12-06 03:13:03.000000 pydorado-2.5.2/dorado/example_data/define_params.py
--rw-r--r--   0 runner    (1001) docker     (122)   240676 2022-12-06 03:13:03.000000 pydorado-2.5.2/dorado/example_data/ex_anuga_data.npz
--rw-r--r--   0 runner    (1001) docker     (122)   230866 2022-12-06 03:13:03.000000 pydorado-2.5.2/dorado/example_data/ex_deltarcm_data.npz
--rw-r--r--   0 runner    (1001) docker     (122)    17072 2022-12-06 03:13:03.000000 pydorado-2.5.2/dorado/lagrangian_walker.py
--rw-r--r--   0 runner    (1001) docker     (122)     4836 2022-12-06 03:13:03.000000 pydorado-2.5.2/dorado/parallel_routing.py
--rw-r--r--   0 runner    (1001) docker     (122)    51147 2022-12-06 03:13:03.000000 pydorado-2.5.2/dorado/particle_track.py
--rw-r--r--   0 runner    (1001) docker     (122)    46140 2022-12-06 03:13:03.000000 pydorado-2.5.2/dorado/routines.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:13:31.743794 pydorado-2.5.2/pydorado.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      573 2022-12-06 03:13:31.000000 pydorado-2.5.2/pydorado.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      451 2022-12-06 03:13:31.000000 pydorado-2.5.2/pydorado.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-06 03:13:31.000000 pydorado-2.5.2/pydorado.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       35 2022-12-06 03:13:31.000000 pydorado-2.5.2/pydorado.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2022-12-06 03:13:31.000000 pydorado-2.5.2/pydorado.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-06 03:13:31.743794 pydorado-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      892 2022-12-06 03:13:03.000000 pydorado-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:55:55.292387 pydorado-2.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-20 20:55:23.000000 pydorado-2.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-20 20:55:55.292387 pydorado-2.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-06-20 20:55:23.000000 pydorado-2.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:55:55.292387 pydorado-2.5.3/dorado/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-20 20:55:23.000000 pydorado-2.5.3/dorado/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:55:55.292387 pydorado-2.5.3/dorado/example_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 20:55:23.000000 pydorado-2.5.3/dorado/example_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-20 20:55:23.000000 pydorado-2.5.3/dorado/example_data/define_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)   240676 2023-06-20 20:55:23.000000 pydorado-2.5.3/dorado/example_data/ex_anuga_data.npz
+-rw-r--r--   0 runner    (1001) docker     (123)   230866 2023-06-20 20:55:23.000000 pydorado-2.5.3/dorado/example_data/ex_deltarcm_data.npz
+-rw-r--r--   0 runner    (1001) docker     (123)    17072 2023-06-20 20:55:23.000000 pydorado-2.5.3/dorado/lagrangian_walker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-06-20 20:55:23.000000 pydorado-2.5.3/dorado/parallel_routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51147 2023-06-20 20:55:23.000000 pydorado-2.5.3/dorado/particle_track.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46140 2023-06-20 20:55:23.000000 pydorado-2.5.3/dorado/routines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:55:55.292387 pydorado-2.5.3/pydorado.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-20 20:55:55.000000 pydorado-2.5.3/pydorado.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-20 20:55:55.000000 pydorado-2.5.3/pydorado.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 20:55:55.000000 pydorado-2.5.3/pydorado.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-20 20:55:55.000000 pydorado-2.5.3/pydorado.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 20:55:55.000000 pydorado-2.5.3/pydorado.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 20:55:55.292387 pydorado-2.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-20 20:55:23.000000 pydorado-2.5.3/setup.py
```

### Comparing `pydorado-2.5.2/LICENSE` & `pydorado-2.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pydorado-2.5.2/PKG-INFO` & `pydorado-2.5.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: pydorado
-Version: 2.5.2
+Version: 2.5.3
 Summary: dorado - Lagrangian particle routing routine via weighted random walks
 Home-page: https://github.com/passaH2O/dorado
 Author: J. Hariharan, K. Wright, P. Passalacqua
 Author-email: jayaram.hariharan@utexas.edu
 License: MIT
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
 
 See project webpage for details: https://github.com/passaH2O/dorado
```

### Comparing `pydorado-2.5.2/README.md` & `pydorado-2.5.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,18 @@
 
 ## Installation:
 dorado supports Python 2.7 as well as Python 3.5+. For the full distribution including examples, clone this repository using `git clone` and run `python setup.py install` from the cloned directory. To test this "full" installation, you must first install `pytest` via `pip install pytest`. Then from the cloned directory the command `pytest` can be run to ensure that your installed distribution passes all of the unit tests.
 
 For a lightweight distribution including just the core functionality, use `pip` to install via PyPI:
 
     pip install pydorado
+    
+Installation using `conda` via `conda-forge` is also supported:
+
+    conda install -c conda-forge pydorado
 
 For additional installation options and instructions, refer to the [documentation](https://passah2o.github.io/dorado/install/index.html).
 
 ## Contributing
 We welcome contributions to the dorado project. Please open an issue or a pull request if there is functionality you would like to see or propose. Refer to our [contributing guide](https://passah2o.github.io/dorado/misc/contributing.html) for more information.
 
 ## Citing
```

### Comparing `pydorado-2.5.2/dorado/example_data/define_params.py` & `pydorado-2.5.3/dorado/example_data/define_params.py`

 * *Files identical despite different names*

### Comparing `pydorado-2.5.2/dorado/example_data/ex_anuga_data.npz` & `pydorado-2.5.3/dorado/example_data/ex_anuga_data.npz`

 * *Files identical despite different names*

### Comparing `pydorado-2.5.2/dorado/example_data/ex_deltarcm_data.npz` & `pydorado-2.5.3/dorado/example_data/ex_deltarcm_data.npz`

 * *Files identical despite different names*

### Comparing `pydorado-2.5.2/dorado/lagrangian_walker.py` & `pydorado-2.5.3/dorado/lagrangian_walker.py`

 * *Files identical despite different names*

### Comparing `pydorado-2.5.2/dorado/parallel_routing.py` & `pydorado-2.5.3/dorado/parallel_routing.py`

 * *Files identical despite different names*

### Comparing `pydorado-2.5.2/dorado/particle_track.py` & `pydorado-2.5.3/dorado/particle_track.py`

 * *Files identical despite different names*

### Comparing `pydorado-2.5.2/dorado/routines.py` & `pydorado-2.5.3/dorado/routines.py`

 * *Files identical despite different names*

### Comparing `pydorado-2.5.2/pydorado.egg-info/PKG-INFO` & `pydorado-2.5.3/pydorado.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: pydorado
-Version: 2.5.2
+Version: 2.5.3
 Summary: dorado - Lagrangian particle routing routine via weighted random walks
 Home-page: https://github.com/passaH2O/dorado
 Author: J. Hariharan, K. Wright, P. Passalacqua
 Author-email: jayaram.hariharan@utexas.edu
 License: MIT
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
 
 See project webpage for details: https://github.com/passaH2O/dorado
```

