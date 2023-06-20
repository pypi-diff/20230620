# Comparing `tmp/stabletrees-0.1.0.tar.gz` & `tmp/stabletrees-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stabletrees-0.1.0.tar", last modified: Thu Dec 22 11:45:29 2022, max compression
+gzip compressed data, was "stabletrees-0.1.1.tar", last modified: Tue Jun 20 10:00:38 2023, max compression
```

## Comparing `stabletrees-0.1.0.tar` & `stabletrees-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxrwxrwx   0        0        0        0 2022-12-22 11:45:29.086342 stabletrees-0.1.0/
--rw-rw-rw-   0        0        0      246 2022-12-22 11:45:29.085333 stabletrees-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      232 2022-12-22 11:36:49.000000 stabletrees-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-12-22 11:45:29.086342 stabletrees-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1471 2022-12-22 11:39:47.000000 stabletrees-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-12-22 11:45:29.063934 stabletrees-0.1.0/src/
--rw-rw-rw-   0        0        0     4020 2022-12-19 11:00:55.000000 stabletrees-0.1.0/src/pybind.cpp
-drwxrwxrwx   0        0        0        0 2022-12-22 11:45:29.065441 stabletrees-0.1.0/src/stabletrees/
--rw-rw-rw-   0        0        0      175 2022-12-19 08:54:19.000000 stabletrees-0.1.0/src/stabletrees/__init__.py
--rw-rw-rw-   0        0        0     7515 2022-12-22 10:54:08.000000 stabletrees-0.1.0/src/stabletrees/tree.py
-drwxrwxrwx   0        0        0        0 2022-12-22 11:45:29.083827 stabletrees-0.1.0/src/stabletrees.egg-info/
--rw-rw-rw-   0        0        0      246 2022-12-22 11:45:28.000000 stabletrees-0.1.0/src/stabletrees.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2022-12-22 11:45:28.000000 stabletrees-0.1.0/src/stabletrees.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-22 11:45:28.000000 stabletrees-0.1.0/src/stabletrees.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2022-12-22 11:45:28.000000 stabletrees-0.1.0/src/stabletrees.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2022-12-22 11:45:28.000000 stabletrees-0.1.0/src/stabletrees.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 10:00:38.116552 stabletrees-0.1.1/
+-rw-rw-rw-   0        0        0      246 2023-06-20 10:00:38.115554 stabletrees-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2023-03-27 10:13:54.000000 stabletrees-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-20 10:00:38.116552 stabletrees-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1926 2023-06-20 10:00:30.000000 stabletrees-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 10:00:38.100021 stabletrees-0.1.1/src/
+-rw-rw-rw-   0        0        0    14086 2023-06-20 06:56:40.000000 stabletrees-0.1.1/src/pybind.cpp
+drwxrwxrwx   0        0        0        0 2023-06-20 10:00:38.107031 stabletrees-0.1.1/src/stabletrees/
+-rw-rw-rw-   0        0        0     6685 2023-06-20 06:56:40.000000 stabletrees-0.1.1/src/stabletrees/AGTBoost.py
+-rw-rw-rw-   0        0        0    13082 2023-06-20 06:56:40.000000 stabletrees-0.1.1/src/stabletrees/PoissonTree.py
+-rw-rw-rw-   0        0        0      914 2023-06-20 06:56:40.000000 stabletrees-0.1.1/src/stabletrees/__init__.py
+-rw-rw-rw-   0        0        0     4850 2023-06-20 06:56:40.000000 stabletrees-0.1.1/src/stabletrees/gradient_tree_boosting.py
+-rw-rw-rw-   0        0        0    25318 2023-06-20 06:56:40.000000 stabletrees-0.1.1/src/stabletrees/random_forest.py
+-rw-rw-rw-   0        0        0    25739 2023-06-20 06:56:40.000000 stabletrees-0.1.1/src/stabletrees/tree.py
+drwxrwxrwx   0        0        0        0 2023-06-20 10:00:38.114555 stabletrees-0.1.1/src/stabletrees.egg-info/
+-rw-rw-rw-   0        0        0      246 2023-06-20 10:00:37.000000 stabletrees-0.1.1/src/stabletrees.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      418 2023-06-20 10:00:38.000000 stabletrees-0.1.1/src/stabletrees.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 10:00:37.000000 stabletrees-0.1.1/src/stabletrees.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-06-20 10:00:37.000000 stabletrees-0.1.1/src/stabletrees.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-06-20 10:00:37.000000 stabletrees-0.1.1/src/stabletrees.egg-info/top_level.txt
```

### Comparing `stabletrees-0.1.0/setup.py` & `stabletrees-0.1.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,44 +2,53 @@
 import os
 from glob import glob
 from setuptools import find_packages, setup
 import pybind11; print(pybind11.__file__)
 from pybind11.setup_helpers import Pybind11Extension
 
 
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 
 ext_modules = [
     Pybind11Extension(
         "_stabletrees",
         sorted(glob("src/*.cpp")),
         cxx_std=14,
         include_dirs=[
             os.path.join(os.path.dirname(__file__), "../include/stabletrees"),
             os.path.join(os.path.dirname(__file__), "../include/stabletrees/trees"),
             os.path.join(os.path.dirname(__file__), "../include/stabletrees/splitters"),
             os.path.join(os.path.dirname(__file__), "../include/stabletrees/criterions"),
+            os.path.join(os.path.dirname(__file__), "../include/stabletrees/optimism"),
             os.path.join(os.path.dirname(__file__), "../include/thirdparty/eigen"),
             "/usr/include/eigen3",
             "/usr/local/include/eigen3",
             "/usr/local/include/thirdparty/eigen",
             "../eigen",
         ],
         define_macros=[("VERSION_INFO", __version__)],
     ),
 ]
+from setuptools.command.build_ext import build_ext
+class BuildExt(build_ext):
+    def build_extensions(self):
+        for ext in self.extensions:
+            # add /openmp and /openmp:llvm to extra_compile_args
+            ext.extra_compile_args += ['/openmp', '/openmp:llvm']
+        build_ext.build_extensions(self)
 
 setup(
     name='stabletrees',
-    version='0.1.0',    
+    version='0.1.1',    
     description='Regression tree with stable update',
     author='Morten Blørstad',
     author_email='mblorstad@email.com',
     url="https://github.com/MortenBlorstad/StableTrees",
     package_dir={"": "src"},
     packages=find_packages(where="src"),
     ext_modules=ext_modules,
+    cmdclass = {'build_ext': BuildExt},
     install_requires=['numpy', "scikit-learn", "matplotlib"],
     python_requires=">=3.6",
 
     
 )
```

