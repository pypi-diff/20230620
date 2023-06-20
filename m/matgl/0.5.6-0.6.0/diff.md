# Comparing `tmp/matgl-0.5.6.tar.gz` & `tmp/matgl-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matgl-0.5.6.tar", last modified: Thu Jun 15 04:34:46 2023, max compression
+gzip compressed data, was "matgl-0.6.0.tar", last modified: Tue Jun 20 17:13:23 2023, max compression
```

## Comparing `matgl-0.5.6.tar` & `matgl-0.6.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-15 04:34:46.364474 matgl-0.5.6/
--rw-r--r--   0 shyue      (501) staff       (20)     1529 2023-06-13 15:50:33.000000 matgl-0.5.6/LICENSE
--rw-r--r--   0 shyue      (501) staff       (20)    12119 2023-06-15 04:34:46.364309 matgl-0.5.6/PKG-INFO
--rw-r--r--   0 shyue      (501) staff       (20)    10950 2023-06-15 04:33:22.000000 matgl-0.5.6/README.md
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-15 04:34:46.359264 matgl-0.5.6/matgl/
--rw-r--r--   0 shyue      (501) staff       (20)      394 2023-06-13 19:01:28.000000 matgl-0.5.6/matgl/__init__.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-15 04:34:46.360303 matgl-0.5.6/matgl/apps/
--rw-r--r--   0 shyue      (501) staff       (20)      180 2023-06-13 19:01:28.000000 matgl-0.5.6/matgl/apps/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     4169 2023-06-13 19:16:50.000000 matgl-0.5.6/matgl/apps/pes.py
--rw-r--r--   0 shyue      (501) staff       (20)     1996 2023-06-14 22:12:57.000000 matgl-0.5.6/matgl/config.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-15 04:34:46.360553 matgl-0.5.6/matgl/data/
--rw-r--r--   0 shyue      (501) staff       (20)       55 2023-06-13 19:01:28.000000 matgl-0.5.6/matgl/data/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     2503 2023-06-13 19:04:59.000000 matgl-0.5.6/matgl/data/transformer.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-15 04:34:46.360888 matgl-0.5.6/matgl/ext/
--rw-r--r--   0 shyue      (501) staff       (20)      118 2023-06-13 19:01:28.000000 matgl-0.5.6/matgl/ext/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)    15898 2023-06-14 19:28:56.000000 matgl-0.5.6/matgl/ext/ase.py
--rw-r--r--   0 shyue      (501) staff       (20)     5268 2023-06-13 19:01:28.000000 matgl-0.5.6/matgl/ext/pymatgen.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-15 04:34:46.361328 matgl-0.5.6/matgl/graph/
--rw-r--r--   0 shyue      (501) staff       (20)       52 2023-06-13 19:01:28.000000 matgl-0.5.6/matgl/graph/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     5101 2023-06-13 19:01:28.000000 matgl-0.5.6/matgl/graph/compute.py
--rw-r--r--   0 shyue      (501) staff       (20)      513 2023-06-13 19:01:28.000000 matgl-0.5.6/matgl/graph/converters.py
--rw-r--r--   0 shyue      (501) staff       (20)    11483 2023-06-13 19:01:28.000000 matgl-0.5.6/matgl/graph/data.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-15 04:34:46.362559 matgl-0.5.6/matgl/layers/
--rw-r--r--   0 shyue      (501) staff       (20)      676 2023-06-15 04:03:30.000000 matgl-0.5.6/matgl/layers/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     2030 2023-06-14 19:29:50.000000 matgl-0.5.6/matgl/layers/_activations.py
--rw-r--r--   0 shyue      (501) staff       (20)     3541 2023-06-13 19:01:28.000000 matgl-0.5.6/matgl/layers/_atom_ref.py
--rw-r--r--   0 shyue      (501) staff       (20)     9428 2023-06-15 04:30:45.000000 matgl-0.5.6/matgl/layers/_basis.py
--rw-r--r--   0 shyue      (501) staff       (20)     2186 2023-06-15 03:59:01.000000 matgl-0.5.6/matgl/layers/_bond.py
--rw-r--r--   0 shyue      (501) staff       (20)     6029 2023-06-13 19:01:28.000000 matgl-0.5.6/matgl/layers/_core.py
--rw-r--r--   0 shyue      (501) staff       (20)     3509 2023-06-13 19:01:28.000000 matgl-0.5.6/matgl/layers/_embedding.py
--rw-r--r--   0 shyue      (501) staff       (20)    16554 2023-06-14 19:31:44.000000 matgl-0.5.6/matgl/layers/_graph_convolution.py
--rw-r--r--   0 shyue      (501) staff       (20)     3872 2023-06-13 19:01:28.000000 matgl-0.5.6/matgl/layers/_readout.py
--rw-r--r--   0 shyue      (501) staff       (20)     3912 2023-06-15 04:31:02.000000 matgl-0.5.6/matgl/layers/_three_body.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-15 04:34:46.362992 matgl-0.5.6/matgl/models/
--rw-r--r--   0 shyue      (501) staff       (20)      187 2023-06-13 19:01:28.000000 matgl-0.5.6/matgl/models/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)    11480 2023-06-14 15:48:06.000000 matgl-0.5.6/matgl/models/_m3gnet.py
--rw-r--r--   0 shyue      (501) staff       (20)     9539 2023-06-14 15:46:44.000000 matgl-0.5.6/matgl/models/_megnet.py
--rw-r--r--   0 shyue      (501) staff       (20)     2147 2023-06-15 04:29:37.000000 matgl-0.5.6/matgl/models/_wrappers.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-15 04:34:46.363726 matgl-0.5.6/matgl/utils/
--rw-r--r--   0 shyue      (501) staff       (20)       61 2023-06-13 19:01:28.000000 matgl-0.5.6/matgl/utils/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)      799 2023-06-13 19:01:28.000000 matgl-0.5.6/matgl/utils/cutoff.py
--rw-r--r--   0 shyue      (501) staff       (20)    10527 2023-06-14 19:27:59.000000 matgl-0.5.6/matgl/utils/io.py
--rw-r--r--   0 shyue      (501) staff       (20)     7147 2023-06-15 04:31:50.000000 matgl-0.5.6/matgl/utils/maths.py
--rw-r--r--   0 shyue      (501) staff       (20)   131200 2023-03-22 18:49:07.000000 matgl-0.5.6/matgl/utils/sb_roots.npy
--rw-r--r--   0 shyue      (501) staff       (20)    12839 2023-06-14 19:36:00.000000 matgl-0.5.6/matgl/utils/training.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-15 04:34:46.359866 matgl-0.5.6/matgl.egg-info/
--rw-r--r--   0 shyue      (501) staff       (20)    12119 2023-06-15 04:34:46.000000 matgl-0.5.6/matgl.egg-info/PKG-INFO
--rw-r--r--   0 shyue      (501) staff       (20)      979 2023-06-15 04:34:46.000000 matgl-0.5.6/matgl.egg-info/SOURCES.txt
--rw-r--r--   0 shyue      (501) staff       (20)        1 2023-06-15 04:34:46.000000 matgl-0.5.6/matgl.egg-info/dependency_links.txt
--rw-r--r--   0 shyue      (501) staff       (20)       41 2023-06-15 04:34:46.000000 matgl-0.5.6/matgl.egg-info/requires.txt
--rw-r--r--   0 shyue      (501) staff       (20)        6 2023-06-15 04:34:46.000000 matgl-0.5.6/matgl.egg-info/top_level.txt
--rw-r--r--   0 shyue      (501) staff       (20)     2427 2023-06-14 21:01:08.000000 matgl-0.5.6/pyproject.toml
--rw-r--r--   0 shyue      (501) staff       (20)       38 2023-06-15 04:34:46.364520 matgl-0.5.6/setup.cfg
--rw-r--r--   0 shyue      (501) staff       (20)     1913 2023-06-15 04:17:12.000000 matgl-0.5.6/setup.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-15 04:34:46.363836 matgl-0.5.6/tests/
--rw-r--r--   0 shyue      (501) staff       (20)      160 2023-06-14 22:12:57.000000 matgl-0.5.6/tests/test_config.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-20 17:13:23.376536 matgl-0.6.0/
+-rw-r--r--   0 shyue      (501) staff       (20)     1529 2023-06-13 15:50:33.000000 matgl-0.6.0/LICENSE
+-rw-r--r--   0 shyue      (501) staff       (20)    12710 2023-06-20 17:13:23.376361 matgl-0.6.0/PKG-INFO
+-rw-r--r--   0 shyue      (501) staff       (20)    11541 2023-06-18 20:24:30.000000 matgl-0.6.0/README.md
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-20 17:13:23.371466 matgl-0.6.0/matgl/
+-rw-r--r--   0 shyue      (501) staff       (20)      394 2023-06-13 19:01:28.000000 matgl-0.6.0/matgl/__init__.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-20 17:13:23.372420 matgl-0.6.0/matgl/apps/
+-rw-r--r--   0 shyue      (501) staff       (20)      180 2023-06-13 19:01:28.000000 matgl-0.6.0/matgl/apps/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     4160 2023-06-20 15:49:52.000000 matgl-0.6.0/matgl/apps/pes.py
+-rw-r--r--   0 shyue      (501) staff       (20)     1996 2023-06-14 22:12:57.000000 matgl-0.6.0/matgl/config.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-20 17:13:23.372659 matgl-0.6.0/matgl/data/
+-rw-r--r--   0 shyue      (501) staff       (20)       55 2023-06-13 19:01:28.000000 matgl-0.6.0/matgl/data/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2503 2023-06-13 19:04:59.000000 matgl-0.6.0/matgl/data/transformer.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-20 17:13:23.372995 matgl-0.6.0/matgl/ext/
+-rw-r--r--   0 shyue      (501) staff       (20)      118 2023-06-13 19:01:28.000000 matgl-0.6.0/matgl/ext/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)    15898 2023-06-20 15:38:59.000000 matgl-0.6.0/matgl/ext/ase.py
+-rw-r--r--   0 shyue      (501) staff       (20)     5278 2023-06-20 15:33:59.000000 matgl-0.6.0/matgl/ext/pymatgen.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-20 17:13:23.373457 matgl-0.6.0/matgl/graph/
+-rw-r--r--   0 shyue      (501) staff       (20)       52 2023-06-13 19:01:28.000000 matgl-0.6.0/matgl/graph/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     5133 2023-06-20 15:44:52.000000 matgl-0.6.0/matgl/graph/compute.py
+-rw-r--r--   0 shyue      (501) staff       (20)      513 2023-06-13 19:01:28.000000 matgl-0.6.0/matgl/graph/converters.py
+-rw-r--r--   0 shyue      (501) staff       (20)    11614 2023-06-20 15:52:57.000000 matgl-0.6.0/matgl/graph/data.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-20 17:13:23.374611 matgl-0.6.0/matgl/layers/
+-rw-r--r--   0 shyue      (501) staff       (20)      676 2023-06-15 04:03:30.000000 matgl-0.6.0/matgl/layers/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2030 2023-06-20 15:42:17.000000 matgl-0.6.0/matgl/layers/_activations.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2983 2023-06-20 15:39:42.000000 matgl-0.6.0/matgl/layers/_atom_ref.py
+-rw-r--r--   0 shyue      (501) staff       (20)     9428 2023-06-20 15:39:42.000000 matgl-0.6.0/matgl/layers/_basis.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2186 2023-06-20 15:39:42.000000 matgl-0.6.0/matgl/layers/_bond.py
+-rw-r--r--   0 shyue      (501) staff       (20)     6029 2023-06-20 15:39:42.000000 matgl-0.6.0/matgl/layers/_core.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3509 2023-06-13 19:01:28.000000 matgl-0.6.0/matgl/layers/_embedding.py
+-rw-r--r--   0 shyue      (501) staff       (20)    16602 2023-06-20 15:47:00.000000 matgl-0.6.0/matgl/layers/_graph_convolution.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3872 2023-06-20 15:39:42.000000 matgl-0.6.0/matgl/layers/_readout.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3944 2023-06-20 15:46:20.000000 matgl-0.6.0/matgl/layers/_three_body.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-20 17:13:23.375054 matgl-0.6.0/matgl/models/
+-rw-r--r--   0 shyue      (501) staff       (20)      187 2023-06-13 19:01:28.000000 matgl-0.6.0/matgl/models/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)    11558 2023-06-20 15:53:17.000000 matgl-0.6.0/matgl/models/_m3gnet.py
+-rw-r--r--   0 shyue      (501) staff       (20)     9539 2023-06-20 15:39:42.000000 matgl-0.6.0/matgl/models/_megnet.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2147 2023-06-15 04:29:37.000000 matgl-0.6.0/matgl/models/_wrappers.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-20 17:13:23.375801 matgl-0.6.0/matgl/utils/
+-rw-r--r--   0 shyue      (501) staff       (20)       61 2023-06-13 19:01:28.000000 matgl-0.6.0/matgl/utils/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)      799 2023-06-13 19:01:28.000000 matgl-0.6.0/matgl/utils/cutoff.py
+-rw-r--r--   0 shyue      (501) staff       (20)    10520 2023-06-17 15:05:12.000000 matgl-0.6.0/matgl/utils/io.py
+-rw-r--r--   0 shyue      (501) staff       (20)     7129 2023-06-20 15:43:24.000000 matgl-0.6.0/matgl/utils/maths.py
+-rw-r--r--   0 shyue      (501) staff       (20)   131200 2023-03-22 18:49:07.000000 matgl-0.6.0/matgl/utils/sb_roots.npy
+-rw-r--r--   0 shyue      (501) staff       (20)    13317 2023-06-20 16:49:51.000000 matgl-0.6.0/matgl/utils/training.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-20 17:13:23.372173 matgl-0.6.0/matgl.egg-info/
+-rw-r--r--   0 shyue      (501) staff       (20)    12710 2023-06-20 17:13:23.000000 matgl-0.6.0/matgl.egg-info/PKG-INFO
+-rw-r--r--   0 shyue      (501) staff       (20)      979 2023-06-20 17:13:23.000000 matgl-0.6.0/matgl.egg-info/SOURCES.txt
+-rw-r--r--   0 shyue      (501) staff       (20)        1 2023-06-20 17:13:23.000000 matgl-0.6.0/matgl.egg-info/dependency_links.txt
+-rw-r--r--   0 shyue      (501) staff       (20)       41 2023-06-20 17:13:23.000000 matgl-0.6.0/matgl.egg-info/requires.txt
+-rw-r--r--   0 shyue      (501) staff       (20)        6 2023-06-20 17:13:23.000000 matgl-0.6.0/matgl.egg-info/top_level.txt
+-rw-r--r--   0 shyue      (501) staff       (20)     2427 2023-06-14 21:01:08.000000 matgl-0.6.0/pyproject.toml
+-rw-r--r--   0 shyue      (501) staff       (20)       38 2023-06-20 17:13:23.376589 matgl-0.6.0/setup.cfg
+-rw-r--r--   0 shyue      (501) staff       (20)     2018 2023-06-20 17:12:29.000000 matgl-0.6.0/setup.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-20 17:13:23.375913 matgl-0.6.0/tests/
+-rw-r--r--   0 shyue      (501) staff       (20)      194 2023-06-15 14:49:26.000000 matgl-0.6.0/tests/test_config.py
```

### Comparing `matgl-0.5.6/LICENSE` & `matgl-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `matgl-0.5.6/PKG-INFO` & `matgl-0.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matgl
-Version: 0.5.6
+Version: 0.6.0
 Summary: MatGL (Materials Graph Library) is a framework for graph deep learning for materials science.
 Author: Tsz Wai Ko, Marcel Nassar, Ji Qi, Santiago Miret, Eliott Liu, Shyue Ping Ong
 Author-email: t1ko@ucsd.edu, ongsp@ucsd.edu
 Maintainer: Shyue Ping Ong
 Maintainer-email: ongsp@ucsd.edu
 Keywords: materials,interatomic potential,force field,science,property prediction,AI,machine learning,graph,deep learning
 Classifier: Development Status :: 4 - Beta
@@ -20,23 +20,23 @@
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![GitHub license](https://img.shields.io/github/license/materialsvirtuallab/matgl)](https://github.com/materialsvirtuallab/matgl/blob/main/LICENSE)
 [![Linting](https://github.com/materialsvirtuallab/matgl/workflows/Linting/badge.svg)](https://github.com/materialsvirtuallab/matgl/workflows/Linting/badge.svg)
-[![Testing](https://github.com/materialsvirtuallab/matgl/workflows/Testing%20-%20main/badge.svg)](https://github.com/materialsvirtuallab/matgl/workflows/Testing/badge.svg)
+[![Testing](https://github.com/materialsvirtuallab/matgl/workflows/Testing/badge.svg)](https://github.com/materialsvirtuallab/matgl/workflows/Testing/badge.svg)
 [![Downloads](https://pepy.tech/badge/matgl)](https://pepy.tech/project/matgl)
 [![Coverage Status](https://coveralls.io/repos/github/materialsvirtuallab/matgl/badge.svg?branch=main)](https://coveralls.io/github/materialsvirtuallab/matgl?branch=main)
 
 <img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/MatGL.png?raw=true" alt="matgl" width="30%" style="float: right">
 
 # Materials Graph Library
 
-Official Documentation: [link][doc]
+### Official Documentation: [:books:][doc]
 
 ## Introduction
 
 MatGL (Materials Graph Library) is a graph deep learning library for materials science. Mathematical graphs are a
 natural representation for a collection of atoms (e.g., molecules or crystals). Graph deep learning models have been
 shown to consistently deliver exceptional performance as surrogate models for the prediction of materials properties.
 
@@ -99,15 +99,15 @@
 ```bash
 pip install matgl
 ```
 
 For the latest dev version, please clone this repo and install using:
 
 ```bash
-python setup.py -e .
+pip install -e .
 ```
 
 ## Usage
 
 Pre-trained M3GNet universal potential and MEGNet models for the Materials Project formation energy and
 multi-fidelity band gap are now available. Users who just want to use the models out of the box should use the newly
 implemented `matgl.load_model` convenience method. The following is an example of a prediction of the formation
@@ -160,53 +160,59 @@
 > Chen, C., Ong, S.P. _A universal graph deep learning interatomic potential for the periodic table._ Nature
 > Computational Science, 2023, 2, 718–728. DOI: [10.1038/s43588-022-00349-3][m3gnet].
 
 ## FAQs
 
 1. **The `M3GNet-MP-2021.2.8-PES` differs from the original tensorflow (TF) implementation!**
 
-   Answer: `M3GNet-MP-2021.2.8-PES` is a refitted model with some data improvements and minor architectural changes.
+   _Answer:_ `M3GNet-MP-2021.2.8-PES` is a refitted model with some data improvements and minor architectural changes.
    Porting over the weights from the TF version to DGL/PyTorch is non-trivial. We have performed reasonable benchmarking
    to ensure that the new implementation reproduces the broad error characteristics of the original TF implementation
    (see [examples][jupyternb]). However, it is not expected to reproduce the TF version exactly. This refitted model
    serves as a baseline for future model improvements. We do not believe there is value in expending the resources
    to reproduce the TF version exactly.
 
 2. **I am getting errors with `matgl.load_model()`!**
 
-   Answer: The most likely reason is that you have a cached older version of the model. We often refactor models to
+   _Answer:_ The most likely reason is that you have a cached older version of the model. We often refactor models to
    ensure the best implementation. This can usually be solved by updating your matgl to the latest version
    and clearing your cache using:
 
    ```bash
    pip install matgl --upgrade
    python -c "import matgl; matgl.clear_cache()"
    ```
 
    On the next run, the latest model will be downloaded. With effect from v0.5.2, we have implemented a model
    versioning scheme that will detect code vs model version conflicts and alert the user of such problems.
 
 3. **What pre-trained models should I be using?**
 
-   Answer: There is no one definitive answer. In general, the newer the architecture and dataset, the more likely
+   _Answer:_ There is no one definitive answer. In general, the newer the architecture and dataset, the more likely
    the model performs better. However, it should also be noted that a model operating on a more diverse dataset may
    compromise on  performance on a specific system. The best way is to look at the READMEs included with each model
    and do some tests on the systems you are interested in.
 
 4. **How do I contribute to matgl?**
 
-   Answer: For code contributions, please fork and submit pull requests. You should read the [developer guide]
-   (developer) to understand the general design guidelines.
-
-   We welcome pre-trained model contributions as well, which should also be submitted via PRs. Please follow the
-   folder structure of the pretrained models. In particular, we expect all models to come with a README and notebook
+   _Answer:_ For code contributions, please fork and submit pull requests. You should read the
+   [developer guide](developer.md) to understand the general design guidelines. We welcome pre-trained model
+   contributions as well, which should also be submitted via PRs. Please follow the folder structure of the
+   pretrained models. In particular, we expect all models to come with a README and notebook
    documenting its use and its key performance metrics. Also, we expect contributions to be on new properties
    or systems or to significantly outperform the existing models. We will develop an alternative means for model
    sharing in the future.
 
+5. **None of your models do what I need. Where can I get help?**
+
+   _Answer:_ Please contact [Prof Ong][ongemail] with a brief description of your needs. For simple problems, we are
+   glad to advise and point you in the right direction. For more complicated problems, we are always open to
+   academic collaborations or projects. We also offer [consulting services][mqm] for companies with unique needs,
+   including but not limited to custom data generation, model development and materials design.
+
 ## Acknowledgments
 
 This work was primarily supported by the [Materials Project][mp], funded by the U.S. Department of Energy, Office of
 Science, Office of Basic Energy Sciences, Materials Sciences and Engineering Division under contract no.
 DE-AC02-05-CH11231: Materials Project program KC23MP. This work used the Expanse supercomputing cluster at the Extreme
 Science and Engineering Discovery Environment (XSEDE), which is supported by National Science Foundation grant number
 ACI-1548562.
@@ -221,7 +227,9 @@
 [mfimegnet]: https://www.nature.com/articles/s43588-020-00002-x "mfi MEGNet paper"
 [m3gnet]: https://www.nature.com/articles/s43588-022-00349-3 "M3GNet paper"
 [mp]: http://materialsproject.org "Materials Project"
 [apidocs]: https://matgl.ai/matgl.html "MatGL API docs"
 [doc]: https://matgl.ai "MatGL Documentation"
 [colab]: http://colab.google.com "Google Colab"
 [jupyternb]: https://github.com/materialsvirtuallab/matgl/tree/main/examples
+[ongemail]: mailto:ongsp@ucsd.edu "Email"
+[mqm]: https://materialsqm.com "MaterialsQM"
```

### Comparing `matgl-0.5.6/README.md` & `matgl-0.6.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [![GitHub license](https://img.shields.io/github/license/materialsvirtuallab/matgl)](https://github.com/materialsvirtuallab/matgl/blob/main/LICENSE)
 [![Linting](https://github.com/materialsvirtuallab/matgl/workflows/Linting/badge.svg)](https://github.com/materialsvirtuallab/matgl/workflows/Linting/badge.svg)
-[![Testing](https://github.com/materialsvirtuallab/matgl/workflows/Testing%20-%20main/badge.svg)](https://github.com/materialsvirtuallab/matgl/workflows/Testing/badge.svg)
+[![Testing](https://github.com/materialsvirtuallab/matgl/workflows/Testing/badge.svg)](https://github.com/materialsvirtuallab/matgl/workflows/Testing/badge.svg)
 [![Downloads](https://pepy.tech/badge/matgl)](https://pepy.tech/project/matgl)
 [![Coverage Status](https://coveralls.io/repos/github/materialsvirtuallab/matgl/badge.svg?branch=main)](https://coveralls.io/github/materialsvirtuallab/matgl?branch=main)
 
 <img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/MatGL.png?raw=true" alt="matgl" width="30%" style="float: right">
 
 # Materials Graph Library
 
-Official Documentation: [link][doc]
+### Official Documentation: [:books:][doc]
 
 ## Introduction
 
 MatGL (Materials Graph Library) is a graph deep learning library for materials science. Mathematical graphs are a
 natural representation for a collection of atoms (e.g., molecules or crystals). Graph deep learning models have been
 shown to consistently deliver exceptional performance as surrogate models for the prediction of materials properties.
 
@@ -75,15 +75,15 @@
 ```bash
 pip install matgl
 ```
 
 For the latest dev version, please clone this repo and install using:
 
 ```bash
-python setup.py -e .
+pip install -e .
 ```
 
 ## Usage
 
 Pre-trained M3GNet universal potential and MEGNet models for the Materials Project formation energy and
 multi-fidelity band gap are now available. Users who just want to use the models out of the box should use the newly
 implemented `matgl.load_model` convenience method. The following is an example of a prediction of the formation
@@ -136,53 +136,59 @@
 > Chen, C., Ong, S.P. _A universal graph deep learning interatomic potential for the periodic table._ Nature
 > Computational Science, 2023, 2, 718–728. DOI: [10.1038/s43588-022-00349-3][m3gnet].
 
 ## FAQs
 
 1. **The `M3GNet-MP-2021.2.8-PES` differs from the original tensorflow (TF) implementation!**
 
-   Answer: `M3GNet-MP-2021.2.8-PES` is a refitted model with some data improvements and minor architectural changes.
+   _Answer:_ `M3GNet-MP-2021.2.8-PES` is a refitted model with some data improvements and minor architectural changes.
    Porting over the weights from the TF version to DGL/PyTorch is non-trivial. We have performed reasonable benchmarking
    to ensure that the new implementation reproduces the broad error characteristics of the original TF implementation
    (see [examples][jupyternb]). However, it is not expected to reproduce the TF version exactly. This refitted model
    serves as a baseline for future model improvements. We do not believe there is value in expending the resources
    to reproduce the TF version exactly.
 
 2. **I am getting errors with `matgl.load_model()`!**
 
-   Answer: The most likely reason is that you have a cached older version of the model. We often refactor models to
+   _Answer:_ The most likely reason is that you have a cached older version of the model. We often refactor models to
    ensure the best implementation. This can usually be solved by updating your matgl to the latest version
    and clearing your cache using:
 
    ```bash
    pip install matgl --upgrade
    python -c "import matgl; matgl.clear_cache()"
    ```
 
    On the next run, the latest model will be downloaded. With effect from v0.5.2, we have implemented a model
    versioning scheme that will detect code vs model version conflicts and alert the user of such problems.
 
 3. **What pre-trained models should I be using?**
 
-   Answer: There is no one definitive answer. In general, the newer the architecture and dataset, the more likely
+   _Answer:_ There is no one definitive answer. In general, the newer the architecture and dataset, the more likely
    the model performs better. However, it should also be noted that a model operating on a more diverse dataset may
    compromise on  performance on a specific system. The best way is to look at the READMEs included with each model
    and do some tests on the systems you are interested in.
 
 4. **How do I contribute to matgl?**
 
-   Answer: For code contributions, please fork and submit pull requests. You should read the [developer guide]
-   (developer) to understand the general design guidelines.
-
-   We welcome pre-trained model contributions as well, which should also be submitted via PRs. Please follow the
-   folder structure of the pretrained models. In particular, we expect all models to come with a README and notebook
+   _Answer:_ For code contributions, please fork and submit pull requests. You should read the
+   [developer guide](developer.md) to understand the general design guidelines. We welcome pre-trained model
+   contributions as well, which should also be submitted via PRs. Please follow the folder structure of the
+   pretrained models. In particular, we expect all models to come with a README and notebook
    documenting its use and its key performance metrics. Also, we expect contributions to be on new properties
    or systems or to significantly outperform the existing models. We will develop an alternative means for model
    sharing in the future.
 
+5. **None of your models do what I need. Where can I get help?**
+
+   _Answer:_ Please contact [Prof Ong][ongemail] with a brief description of your needs. For simple problems, we are
+   glad to advise and point you in the right direction. For more complicated problems, we are always open to
+   academic collaborations or projects. We also offer [consulting services][mqm] for companies with unique needs,
+   including but not limited to custom data generation, model development and materials design.
+
 ## Acknowledgments
 
 This work was primarily supported by the [Materials Project][mp], funded by the U.S. Department of Energy, Office of
 Science, Office of Basic Energy Sciences, Materials Sciences and Engineering Division under contract no.
 DE-AC02-05-CH11231: Materials Project program KC23MP. This work used the Expanse supercomputing cluster at the Extreme
 Science and Engineering Discovery Environment (XSEDE), which is supported by National Science Foundation grant number
 ACI-1548562.
@@ -197,7 +203,9 @@
 [mfimegnet]: https://www.nature.com/articles/s43588-020-00002-x "mfi MEGNet paper"
 [m3gnet]: https://www.nature.com/articles/s43588-022-00349-3 "M3GNet paper"
 [mp]: http://materialsproject.org "Materials Project"
 [apidocs]: https://matgl.ai/matgl.html "MatGL API docs"
 [doc]: https://matgl.ai "MatGL Documentation"
 [colab]: http://colab.google.com "Google Colab"
 [jupyternb]: https://github.com/materialsvirtuallab/matgl/tree/main/examples
+[ongemail]: mailto:ongsp@ucsd.edu "Email"
+[mqm]: https://materialsqm.com "MaterialsQM"
```

### Comparing `matgl-0.5.6/matgl/apps/pes.py` & `matgl-0.6.0/matgl/apps/pes.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,16 +15,16 @@
     """A class representing an interatomic potential."""
 
     __version__ = 1
 
     def __init__(
         self,
         model: nn.Module,
-        data_mean: torch.tensor | None = None,
-        data_std: torch.tensor | None = None,
+        data_mean: torch.Tensor | None = None,
+        data_std: torch.Tensor | None = None,
         element_refs: np.ndarray | None = None,
         calc_forces: bool = True,
         calc_stresses: bool = True,
         calc_hessian: bool = False,
     ):
         """Initialize Potential from a model and elemental references.
 
@@ -49,23 +49,23 @@
         else:
             self.element_refs = None
 
         self.data_mean = data_mean if data_mean is not None else torch.zeros(1)
         self.data_std = data_std if data_std is not None else torch.ones(1)
 
     def forward(
-        self, g: dgl.DGLGraph, state_attr: torch.tensor | None = None, l_g: dgl.DGLGraph | None = None
+        self, g: dgl.DGLGraph, state_attr: torch.Tensor | None = None, l_g: dgl.DGLGraph | None = None
     ) -> tuple:
         """Args:
             g: DGL graph
             state_attr: State attrs
             l_g: Line graph.
 
         Returns:
-            energies, forces, stresses, hessian: torch.tensor
+            energies, forces, stresses, hessian: torch.Tensor
         """
         forces = torch.zeros(1)
         stresses = torch.zeros(1)
         hessian = torch.zeros(1)
         if self.calc_forces:
             g.ndata["pos"].requires_grad_(True)
         total_energies = self.data_std * self.model(g=g, state_attr=state_attr, l_g=l_g) + self.data_mean
@@ -89,30 +89,30 @@
                 hessian = total_energies.new_zeros((s, s))
                 for iatom in range(s):
                     tmp = grad([r[iatom]], g.ndata["pos"], retain_graph=iatom < s)[0]
                     if tmp is not None:
                         hessian[iatom] = tmp.view(-1)
         if self.calc_stresses:
             f_ij = -grads[1]
-            stresses = []
+            sts: list = []
             count_edge = 0
             count_node = 0
             for graph_id in range(g.batch_size):
                 num_edges = g.batch_num_edges()[graph_id]
                 num_nodes = 0
-                stresses.append(
+                sts.append(
                     -1
                     * (
                         160.21766208
                         * torch.matmul(
                             g.edata["bond_vec"][count_edge : count_edge + num_edges].T,
                             f_ij[count_edge : count_edge + num_edges],
                         )
                         / g.ndata["volume"][count_node + num_nodes]
                     )
                 )
                 count_edge = count_edge + num_edges
                 num_nodes = g.batch_num_nodes()[graph_id]
                 count_node = count_node + num_nodes
-            stresses = torch.cat(stresses)
+            stresses = torch.cat(sts)
 
         return total_energies, forces, stresses, hessian
```

### Comparing `matgl-0.5.6/matgl/config.py` & `matgl-0.6.0/matgl/config.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.6/matgl/data/transformer.py` & `matgl-0.6.0/matgl/data/transformer.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.6/matgl/ext/ase.py` & `matgl-0.6.0/matgl/ext/ase.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
     """M3GNet calculator for ASE."""
 
     implemented_properties = ["energy", "free_energy", "forces", "stress", "hessian"]
 
     def __init__(
         self,
         potential: Potential,
-        state_attr: torch.tensor = None,
+        state_attr: torch.Tensor = None,
         stress_weight: float = 1.0,
         **kwargs,
     ):
         """
         Init M3GNetCalculator with a Potential.
 
         Args:
@@ -175,24 +175,24 @@
 
 class Relaxer:
     """Relaxer is a class for structural relaxation."""
 
     def __init__(
         self,
         potential: Potential = None,
-        state_attr: torch.tensor = None,
+        state_attr: torch.Tensor = None,
         optimizer: Optimizer | str = "FIRE",
         relax_cell: bool = True,
         stress_weight: float = 0.01,
     ):
         """
         Args:
             potential (Potential): a M3GNet potential, a str path to a saved model or a short name for saved model
             that comes with M3GNet distribution
-            state_attr (torch.tensor): State attr.
+            state_attr (torch.Tensor): State attr.
             optimizer (str or ase Optimizer): the optimization algorithm.
             Defaults to "FIRE"
             relax_cell (bool): whether to relax the lattice cell
             stress_weight (float): the stress weight for relaxation.
         """
         if isinstance(optimizer, str):
             optimizer_obj = OPTIMIZERS.get(optimizer, None)
@@ -308,15 +308,15 @@
 class MolecularDynamics:
     """Molecular dynamics class."""
 
     def __init__(
         self,
         atoms: Atoms,
         potential: Potential,
-        state_attr: torch.tensor = None,
+        state_attr: torch.Tensor = None,
         ensemble: str = "nvt",
         temperature: int = 300,
         timestep: float = 1.0,
         pressure: float = 1.01325 * units.bar,
         taut: float | None = None,
         taup: float | None = None,
         compressibility_au: float | None = None,
@@ -328,15 +328,15 @@
         """
         Init the MD simulation.
 
         Args:
             atoms (Atoms): atoms to run the MD
             potential (Potential): potential for calculating the energy, force,
             stress of the atoms
-            state_attr (torch.tensor): State attr.
+            state_attr (torch.Tensor): State attr.
             ensemble (str): choose from 'nvt' or 'npt'. NPT is not tested,
             use with extra caution
             temperature (float): temperature for MD simulation, in K
             timestep (float): time step in fs
             pressure (float): pressure in eV/A^3
             taut (float): time constant for Berendsen temperature coupling
             taup (float): time constant for pressure coupling
```

### Comparing `matgl-0.5.6/matgl/ext/pymatgen.py` & `matgl-0.6.0/matgl/ext/pymatgen.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     Args:
         train_structures: pymatgen Molecule/Structure object
 
     Returns:
         Tuple of elements covered in training set
     """
-    elements = set()
+    elements: set[str] = set()
     for s in train_structures:
         elements.update(s.composition.get_el_amt_dict().keys())
     return tuple(sorted(elements, key=lambda el: Element(el).Z))  # type: ignore
 
 
 class Molecule2Graph(GraphConverter):
     """Construct a DGL graph from Pymatgen Molecules."""
```

### Comparing `matgl-0.5.6/matgl/graph/compute.py` & `matgl-0.6.0/matgl/graph/compute.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     n_atoms_total = np.sum(g.num_nodes())
     first_col = g.edges()[0].reshape(-1, 1)
     all_indices = torch.arange(n_atoms_total).reshape(1, -1)
     n_bond_per_atom = torch.count_nonzero(first_col == all_indices, dim=0)
     n_triple_i = n_bond_per_atom * (n_bond_per_atom - 1)
     n_triple = torch.sum(n_triple_i)
     n_triple_ij = (n_bond_per_atom - 1).repeat_interleave(n_bond_per_atom)
-    triple_bond_indices = torch.empty((n_triple, 2), dtype=torch.int64)
+    triple_bond_indices = torch.empty((n_triple, 2), dtype=torch.int64)  # type: ignore
 
     start = 0
     cs = 0
     for n in n_bond_per_atom:
         if n > 0:
             """
             triple_bond_indices is generated from all pair permutations of atom indices. The
@@ -60,15 +60,15 @@
 
     src_id, dst_id = (triple_bond_indices[:, 0], triple_bond_indices[:, 1])
     l_g = dgl.graph((src_id, dst_id))
     l_g.ndata["bond_dist"] = g.edata["bond_dist"]
     l_g.ndata["bond_vec"] = g.edata["bond_vec"]
     l_g.ndata["pbc_offset"] = g.edata["pbc_offset"]
     l_g.ndata["n_triple_ij"] = n_triple_ij
-    n_triple_s = torch.tensor(n_triple_s, dtype=torch.int64)
+    n_triple_s = torch.tensor(n_triple_s, dtype=torch.int64)  # type: ignore
     return l_g, triple_bond_indices, n_triple_ij, n_triple_i, n_triple_s
 
 
 def compute_pair_vector_and_distance(g: dgl.DGLGraph):
     """Calculate bond vectors and distances using dgl graphs.
 
     Args:
@@ -93,16 +93,16 @@
 def compute_theta_and_phi(edges: dgl.udf.EdgeBatch):
     """Calculate bond angle Theta and Phi using dgl graphs.
 
     Args:
     edges: DGL graph edges
 
     Returns:
-    cos_theta: torch.tensor
-    phi: torch.tensor
+    cos_theta: torch.Tensor
+    phi: torch.Tensor
     triple_bond_lengths (torch.tensor):
     """
     vec1 = edges.src["bond_vec"]
     vec2 = edges.dst["bond_vec"]
     cosine_theta = torch.sum(vec1 * vec2, dim=1) / (torch.norm(vec1, dim=1) * torch.norm(vec2, dim=1))
     return {
         "cos_theta": cosine_theta,
```

### Comparing `matgl-0.5.6/matgl/graph/converters.py` & `matgl-0.6.0/matgl/graph/converters.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.6/matgl/graph/data.py` & `matgl-0.6.0/matgl/graph/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -290,35 +290,38 @@
 
     def load(
         self,
         filename: str = "dgl_graph.bin",
         filename_line_graph: str = "dgl_line_graph.bin",
         filename_state_attr: str = "state_attr.pt",
     ):
-        """Load dgl graphs
+        """
+        Load dgl graphs from files.
+
         Args:
-        :filename: Name of file storing dgl graphs
-        :filename: Name of file storing state attrs.
+            filename: Name of file storing dgl graphs
+            filename_line_graph: Name of file storing dgl line graphs
+            filename_state_attr: Name of file storing state attrs.
         """
         self.graphs = load_graphs(filename)
         self.line_graphs = load_graphs(filename_line_graph)
         with open("labels.json") as file:
-            labels = json.load(file)
+            labels: dict = json.load(file)
         self.energies = labels["energies"]
         self.forces = labels["forces"]
         self.stresses = labels["stresses"]
         self.state_attr = torch.load("state_attr.pt")
 
     def __getitem__(self, idx: int):
         """Get graph and label with idx."""
         return (
             self.graphs[idx],
             self.line_graphs[idx],
             self.state_attr[idx],
             self.energies[idx],
             torch.tensor(self.forces[idx]),
-            torch.tensor(self.stresses[idx]),
+            torch.tensor(self.stresses[idx]),  # type: ignore
         )
 
     def __len__(self):
         """Get size of dataset."""
         return len(self.graphs)
```

### Comparing `matgl-0.5.6/matgl/layers/__init__.py` & `matgl-0.6.0/matgl/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.6/matgl/layers/_activations.py` & `matgl-0.6.0/matgl/layers/_activations.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     """
 
     def __init__(self) -> None:
         """Initializes the SoftPlus2 class."""
         super().__init__()
         self.ssp = nn.Softplus()
 
-    def forward(self, x: torch.tensor) -> torch.tensor:
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
         """Evaluate activation function given the input tensor x.
 
         Args:
             x (torch.tensor): Input tensor
 
         Returns:
             out (torch.tensor): Output tensor
@@ -52,15 +52,15 @@
         if alpha is None:
             self.alpha = nn.Parameter(torch.tensor(0.0))
         else:
             self.alpha = nn.Parameter(torch.tensor(alpha))
 
         self.alpha.requires_grad_(True)
 
-    def forward(self, x: torch.tensor) -> torch.tensor:
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
         """Evaluate activation function given the input tensor x.
 
         Args:
             x (torch.tensor): Input tensor
 
         Returns:
             out (torch.tensor): Output tensor
```

### Comparing `matgl-0.5.6/matgl/layers/_atom_ref.py` & `matgl-0.6.0/matgl/layers/_atom_ref.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,74 +1,67 @@
 """Atomic energy offset. Used for predicting extensive properties."""
 from __future__ import annotations
 
 import dgl
 import numpy as np
 import torch
-from pymatgen.core import Molecule, Structure
 from torch import nn
 
 
 class AtomRef(nn.Module):
     """Get total property offset for a system."""
 
     def __init__(
         self,
         property_offset: np.array,  # type: ignore
     ) -> None:
         """Args:
-        -----------
         property_offset (np.array): a array of elemental property offset.
         """
         super().__init__()
         self.property_offset = torch.tensor(property_offset)
         self.max_z = self.property_offset.size(dim=0)
 
-    def get_feature_matrix(self, structs_or_graphs: list, element_list: tuple[str]) -> np.typing.NDArray:
+    def get_feature_matrix(self, graphs: list) -> np.typing.NDArray:
         """Get the number of atoms for different elements in the structure.
 
         Args:
-            structs_or_graphs (list): a list of pymatgen Structure or dgl graph
-            element_list: a dictionary containing element types in the training set
+            graphs (list): a list of dgl graph
 
         Returns:
             features (np.array): a matrix (num_structures, num_elements)
         """
-        n = len(structs_or_graphs)
+        n = len(graphs)
         features = np.zeros(shape=(n, self.max_z))
-        for i, s in enumerate(structs_or_graphs):
-            if isinstance(s, (Structure, Molecule)):
-                atomic_numbers = [element_list.index(site.specie.symbol) for site in s.sites]
-            else:
-                one_hot_vecs = s.ndata["attr"]
-                atomic_numbers = ((one_hot_vecs == 1).nonzero(as_tuple=True)[0]).tolist()
+        for i, s in enumerate(graphs):
+            one_hot_vecs = s.ndata["attr"]
+            atomic_numbers = ((one_hot_vecs == 1).nonzero(as_tuple=True)[0]).tolist()
             features[i] = np.bincount(atomic_numbers, minlength=self.max_z)
         return features
 
-    def fit(self, structs_or_graphs: list, element_list: tuple[str], properties: np.typing.NDArray) -> None:
+    def fit(self, graphs: list, properties: np.typing.NDArray) -> None:
         """Fit the elemental reference values for the properties.
 
         Args:
-            structs_or_graphs: pymatgen Structures or dgl graphs
-            element_list (tuple): a list of element types
+            graphs: dgl graphs
             properties (np.ndarray): array of extensive properties
         """
-        features = self.get_feature_matrix(structs_or_graphs, element_list)
+        features = self.get_feature_matrix(graphs)
         self.property_offset = np.linalg.pinv(features.T.dot(features)).dot(features.T.dot(properties))
         self.property_offset = torch.tensor(self.property_offset)
 
-    def forward(self, g: dgl.DGLGraph, state_attr: torch.tensor | None = None):
+    def forward(self, g: dgl.DGLGraph, state_attr: torch.Tensor | None = None):
         """Get the total property offset for a system.
 
         Args:
-        g: a batch of dgl graphs
-        state_attr: state attributes
+            g: a batch of dgl graphs
+            state_attr: state attributes
 
         Returns:
-        offset_per_graph:
+            offset_per_graph
         """
         if self.property_offset.ndim > 1:
             offset_batched_with_state = []
             for i in range(0, self.property_offset.size(dim=0)):
                 property_offset_batched = self.property_offset[i].repeat(g.num_nodes(), 1)
                 offset = property_offset_batched * g.ndata["attr"]
                 g.ndata["atomic_offset"] = torch.sum(offset, 1)
```

### Comparing `matgl-0.5.6/matgl/layers/_basis.py` & `matgl-0.6.0/matgl/layers/_basis.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 
     @lru_cache(maxsize=128)
     def _calculate_smooth_symbolic_funcs(self) -> list:
         return _get_lambda_func(max_n=self.max_n, cutoff=self.cutoff)
 
     def __call__(self, r):
         """Args:
-            r: torch.tensor, distance tensor, 1D.
+            r: torch.Tensor, distance tensor, 1D.
 
 
         Returns: [n, max_n * max_l] spherical Bessel function results
 
         """
         if self.smooth:
             return self._call_smooth_sbf(r)
@@ -124,15 +124,15 @@
 
     @staticmethod
     def rbf_j0(r, cutoff: float = 5.0, max_n: int = 3):
         """Spherical Bessel function of order 0, ensuring the function value
         vanishes at cutoff.
 
         Args:
-            r: torch.tensor pytorch tensors
+            r: torch.Tensor pytorch tensors
             cutoff: float, the cutoff radius
             max_n: int max number of basis
         Returns: basis function expansion using first spherical Bessel function
         """
         n = (torch.arange(1, max_n + 1)).type(dtype=torch.float32)[None, :]
         r = r[:, None]
         return sqrt(2.0 / cutoff) * torch.sin(n * pi / cutoff * r) / r
@@ -162,15 +162,15 @@
         self.orig_funcs = [sympy.simplify(i).evalf() for i in funcs]
         self.funcs = [sympy.lambdify([costheta, phi], i, [{"conjugate": _conjugate}, torch]) for i in self.orig_funcs]
         self.funcs[0] = _y00
 
     def __call__(self, costheta, phi=None):
         """Args:
             costheta: Cosine of the azimuthal angle
-            phi: torch.tensor, the polar angle.
+            phi: torch.Tensor, the polar angle.
 
         Returns: [n, m] spherical harmonic results, where n is the number
             of angles. The column is arranged following
             `[Y_0^0, Y_1^{-1}, Y_1^{0}, Y_1^1, Y_2^{-2}, ...]`
         """
         # costheta = torch.tensor(costheta, dtype=torch.complex64)
         # phi = torch.tensor(phi, dtype=torch.complex64)
@@ -182,16 +182,16 @@
 def _y00(theta, phi):
     r"""Spherical Harmonics with `l=m=0`.
 
     ..math::
         Y_0^0 = \frac{1}{2} \sqrt{\frac{1}{\pi}}
 
     Args:
-        theta: torch.tensor, the azimuthal angle
-        phi: torch.tensor, the polar angle
+        theta: torch.Tensor, the azimuthal angle
+        phi: torch.Tensor, the polar angle
 
     Returns: `Y_0^0` results
 
     """
     return 0.5 * torch.ones_like(theta) * sqrt(1.0 / pi)
 
 
@@ -205,15 +205,15 @@
     equals to zero. The function was derived from the order 0 spherical Bessel
     function, and was expanded by the different zero roots.
 
     Ref:
         https://arxiv.org/pdf/1907.02374.pdf
 
     Args:
-        r: torch.tensor distance tensor
+        r: torch.Tensor distance tensor
         cutoff: float, cutoff radius
         max_n: int, max number of basis, expanded by the zero roots
 
     Returns: expanded spherical harmonics with derivatives smooth at boundary
 
     """
     n = torch.arange(max_n).type(dtype=torch.float32)[None, :]
```

### Comparing `matgl-0.5.6/matgl/layers/_bond.py` & `matgl-0.6.0/matgl/layers/_bond.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         if rbf_type == "SphericalBessel":
             self.rbf = SphericalBesselFunction(max_l, max_n, cutoff, smooth)  # type: ignore
         elif rbf_type == "Gaussian":
             self.rbf = GaussianExpansion(initial, final, num_centers, width)  # type: ignore
         else:
             raise Exception("undefined rbf_type, please use SphericalBessel or Gaussian instead.")
 
-    def forward(self, bond_dist: torch.tensor):
+    def forward(self, bond_dist: torch.Tensor):
         """Forward.
 
         Args:
         bond_dist: Bond distance
 
         Return:
         bond_basis: Radial basis functions
```

### Comparing `matgl-0.5.6/matgl/layers/_core.py` & `matgl-0.6.0/matgl/layers/_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,15 @@
             else:
                 self.layers.append(nn.Linear(in_dim, out_dim, bias=use_bias))
                 if self.activate_last:
                     self.layers.append(nn.SiLU())
                 self.gates.append(nn.Linear(in_dim, out_dim, bias=use_bias))
                 self.gates.append(nn.Sigmoid())
 
-    def forward(self, inputs: torch.tensor):
+    def forward(self, inputs: torch.Tensor):
         return self.layers(inputs) * self.gates(inputs)
 
 
 class EdgeSet2Set(Module):
     """Implementation of Set2Set."""
 
     def __init__(self, input_dim: int, n_iters: int, n_layers: int) -> None:
@@ -140,15 +140,15 @@
         self.lstm = LSTM(self.output_dim, self.input_dim, n_layers)
         self.reset_parameters()
 
     def reset_parameters(self):
         """Reinitialize learnable parameters."""
         self.lstm.reset_parameters()
 
-    def forward(self, g: DGLGraph, feat: torch.tensor):
+    def forward(self, g: DGLGraph, feat: torch.Tensor):
         """Defines the computation performed at every call.
 
         :param g: Input graph
         :param feat: Input features.
         :return: One hot vector
         """
         with g.local_scope():
```

### Comparing `matgl-0.5.6/matgl/layers/_embedding.py` & `matgl-0.6.0/matgl/layers/_embedding.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.6/matgl/layers/_graph_convolution.py` & `matgl-0.6.0/matgl/layers/_graph_convolution.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,17 +154,17 @@
 
         mlp_kwargs = {
             "dims": dims,
             "activation": self.activation,
             "activate_last": True,
             "bias_last": True,
         }
-        self.edge_func = MLP(**mlp_kwargs) if self.has_dense else Identity()
-        self.node_func = MLP(**mlp_kwargs) if self.has_dense else Identity()
-        self.state_func = MLP(**mlp_kwargs) if self.has_dense else Identity()
+        self.edge_func = MLP(**mlp_kwargs) if self.has_dense else Identity()  # type: ignore
+        self.node_func = MLP(**mlp_kwargs) if self.has_dense else Identity()  # type: ignore
+        self.state_func = MLP(**mlp_kwargs) if self.has_dense else Identity()  # type: ignore
 
         # compute input sizes
         edge_in = 2 * conv_dim + conv_dim + conv_dim  # 2*NDIM+EDIM+GDIM
         node_in = out_dim + conv_dim + conv_dim  # EDIM+NDIM+GDIM
         attr_in = out_dim + out_dim + conv_dim  # EDIM+NDIM+GDIM
         self.conv = MEGNetGraphConv.from_dims(
             edge_dims=[edge_in, *conv_hiddens],
```

### Comparing `matgl-0.5.6/matgl/layers/_readout.py` & `matgl-0.6.0/matgl/layers/_readout.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         self.dims = [in_feats, *dims, num_targets]
         self.gated = GatedMLP(in_feats=in_feats, dims=self.dims, activate_last=False)
 
     def forward(self, g: dgl.DGLGraph):
         """Args:
             g: DGL graph
         Returns:
-            atomic_properties: torch.tensor.
+            atomic_properties: torch.Tensor.
         """
         atomic_properties = self.gated(g.ndata["node_feat"])
         return atomic_properties
 
 
 class WeightedReadOutPair(nn.Module):
     """Feed the average of atomic features i and j into weighted readout layer."""
```

### Comparing `matgl-0.5.6/matgl/layers/_three_body.py` & `matgl-0.6.0/matgl/layers/_three_body.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,18 +29,18 @@
         self.update_network_atom = update_network_atom
         self.update_network_bond = update_network_bond
 
     def forward(
         self,
         graph: dgl.DGLGraph,
         line_graph: dgl.DGLGraph,
-        three_basis: torch.tensor,
+        three_basis: torch.Tensor,
         three_cutoff: float,
-        node_feat: torch.tensor,
-        edge_feat: torch.tensor,
+        node_feat: torch.Tensor,
+        edge_feat: torch.Tensor,
     ):
         """
         Forward function for ThreeBodyInteractions.
 
         Args:
             graph: dgl graph
             line_graph: line graph.
@@ -50,19 +50,19 @@
             edge_feat: edge features.
         """
         end_atom_index = torch.gather(graph.edges()[1], 0, line_graph.edges()[1].to(torch.int64))
         atoms = self.update_network_atom(node_feat)
         end_atom_index = torch.unsqueeze(end_atom_index, 1)
         atoms = torch.squeeze(atoms[end_atom_index])
         basis = three_basis * atoms
-        three_cutoff = torch.unsqueeze(three_cutoff, dim=1)
+        three_cutoff = torch.unsqueeze(three_cutoff, dim=1)  # type: ignore
         weights = torch.reshape(
             three_cutoff[torch.stack(list(line_graph.edges()), dim=1).to(torch.int64)], (-1, 2)  # type: ignore
         )
-        weights = torch.prod(weights, axis=-1)
+        weights = torch.prod(weights, axis=-1)  # type: ignore
         basis = basis * weights[:, None]
         new_bonds = scatter_sum(
             basis.to(torch.float32),
             segment_ids=get_segment_indices_from_n(line_graph.ndata["n_triple_ij"]),
             num_segments=graph.num_edges(),
             dim=0,
         )
@@ -79,16 +79,16 @@
     For the spherical Harmonics function, the column is ordered by
         [m=[0], m=[-1, 0, 1], m=[-2, -1, 0, 1, 2], ...] max_l blocks, and each
         block has 2*l + 1
         if use_phi is False, then the columns become
         [m=[0], m=[0], ...] max_l columns
 
     Args:
-        sbf: torch.tensor spherical bessel function results
-        shf: torch.tensor spherical harmonics function results
+        sbf: torch.Tensor spherical bessel function results
+        shf: torch.Tensor spherical harmonics function results
         max_n: int, max number of n
         max_l: int, max number of l
         use_phi: whether to use phi
     Returns:
     """
     if sbf.size()[0] == 0:
         return sbf
```

### Comparing `matgl-0.5.6/matgl/models/_m3gnet.py` & `matgl-0.6.0/matgl/models/_m3gnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,38 +176,40 @@
         )
         if is_intensive:
             input_feats = dim_node_embedding if field == "node_feat" else dim_edge_embedding
             if readout_type == "set2set":
                 self.readout = Set2SetReadOut(num_steps=niters_set2set, num_layers=nlayers_set2set, field=field)
                 readout_feats = 2 * input_feats + dim_state_feats if include_state else 2 * input_feats  # type: ignore
             else:
-                self.readout = ReduceReadOut("mean", field=field)
+                self.readout = ReduceReadOut("mean", field=field)  # type: ignore
                 readout_feats = input_feats + dim_state_feats if include_state else input_feats  # type: ignore
 
             dims_final_layer = [readout_feats, units, units, ntargets]
             self.final_layer = MLP(dims_final_layer, activation, activate_last=False)
             if task_type == "classification":
                 self.sigmoid = nn.Sigmoid()
 
         else:
             if task_type == "classification":
                 raise ValueError("Classification task cannot be extensive")
-            self.final_layer = WeightedReadOut(in_feats=dim_node_embedding, dims=[units, units], num_targets=ntargets)
+            self.final_layer = WeightedReadOut(
+                in_feats=dim_node_embedding, dims=[units, units], num_targets=ntargets  # type: ignore
+            )
 
         self.max_n = max_n
         self.max_l = max_l
         self.n_blocks = nblocks
         self.units = units
         self.cutoff = cutoff
         self.threebody_cutoff = threebody_cutoff
         self.include_states = include_state
         self.task_type = task_type
         self.is_intensive = is_intensive
 
-    def forward(self, g: dgl.DGLGraph, state_attr: torch.tensor | None = None, l_g: dgl.DGLGraph | None = None):
+    def forward(self, g: dgl.DGLGraph, state_attr: torch.Tensor | None = None, l_g: dgl.DGLGraph | None = None):
         """Performs message passing and updates node representations.
 
         Args:
             g : DGLGraph for a batch of graphs.
             state_attr: State attrs for a batch of graphs.
             l_g : DGLGraph for a batch of line graphs.
 
@@ -239,25 +241,25 @@
             num_edge_feats, num_node_feats, num_state_feats = self.graph_layers[i](
                 g, num_edge_feats, num_node_feats, num_state_feats
             )
         g.ndata["node_feat"] = num_node_feats
         g.edata["edge_feat"] = num_edge_feats
         if self.is_intensive:
             node_vec = self.readout(g)
-            vec = torch.hstack([node_vec, state_attr]) if self.include_states else node_vec
+            vec = torch.hstack([node_vec, state_attr]) if self.include_states else node_vec  # type: ignore
             output = self.final_layer(vec)
             if self.task_type == "classification":
                 output = self.sigmoid(output)
         else:
             g.ndata["atomic_properties"] = self.final_layer(g)
             output = dgl.readout_nodes(g, "atomic_properties", op="sum")
         return torch.squeeze(output)
 
     def predict_structure(
-        self, structure, state_feats: torch.tensor | None = None, graph_converter: GraphConverter | None = None
+        self, structure, state_feats: torch.Tensor | None = None, graph_converter: GraphConverter | None = None
     ):
         """Convenience method to directly predict property from structure.
 
         Args:
             structure: An input crystal/molecule.
             state_feats (torch.tensor): Graph attributes
             graph_converter: Object that implements a get_graph_from_structure.
```

### Comparing `matgl-0.5.6/matgl/models/_megnet.py` & `matgl-0.6.0/matgl/models/_megnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,15 +199,15 @@
             output = torch.sigmoid(output)
 
         return output
 
     def predict_structure(
         self,
         structure,
-        state_feats: torch.tensor | None = None,
+        state_feats: torch.Tensor | None = None,
         graph_converter: GraphConverter | None = None,
     ):
         """Convenience method to directly predict property from structure.
 
         Args:
             structure: An input crystal/molecule.
             state_feats (torch.tensor): Graph attributes
```

### Comparing `matgl-0.5.6/matgl/models/_wrappers.py` & `matgl-0.6.0/matgl/models/_wrappers.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.6/matgl/utils/cutoff.py` & `matgl-0.6.0/matgl/utils/cutoff.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.6/matgl/utils/io.py` & `matgl-0.6.0/matgl/utils/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -256,15 +256,15 @@
     """
     if getattr(cls_, "__version__", 0) > d.get("@model_version", 0):
         warnings.warn(
             "Incompatible model version detected! The code will continue to load the model but it is "
             "recommended that you provide a path to an updated model, increment your @model_version in model.json "
             "if you are confident that the changes are not problematic, or clear your ~/.matgl cache using "
             '`python -c "import matgl; matgl.clear_cache()"`',
-            DeprecationWarning,
+            UserWarning,
             stacklevel=2,
         )
 
 
 def get_available_pretrained_models() -> list[str]:
     """Checks Github for available pretrained_models for download. These can be used with load_model.
```

### Comparing `matgl-0.5.6/matgl/utils/maths.py` & `matgl-0.6.0/matgl/utils/maths.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,30 +94,30 @@
 
 
 def get_segment_indices_from_n(ns):
     """Get segment indices from number array. For example if
     ns = [2, 3], then the function will return [0, 0, 1, 1, 1].
 
     Args:
-        ns: torch.tensor, the number of atoms/bonds array
+        ns: torch.Tensor, the number of atoms/bonds array
 
     Returns:
         object:
 
     Returns: segment indices tensor
     """
     a = torch.arange(ns.size(dim=0))
     return a.repeat_interleave(ns, dim=0)
 
 
 def get_range_indices_from_n(ns):
     """Give ns = [2, 3], return [0, 1, 0, 1, 2].
 
     Args:
-        ns: torch.tensor, the number of atoms/bonds array
+        ns: torch.Tensor, the number of atoms/bonds array
 
     Returns: range indices
     """
     max_n = torch.max(ns)
     n = ns.size(dim=0)
     n_range = torch.arange(max_n)
     matrix = n_range.tile(
@@ -165,15 +165,15 @@
 
     Returns: broadcasted state attributes
 
     """
     return state_feat.repeat((g.num_nodes(), 1))
 
 
-def scatter_sum(input_tensor: torch.tensor, segment_ids: torch.tensor, num_segments: int, dim: int) -> torch.tensor:
+def scatter_sum(input_tensor: torch.Tensor, segment_ids: torch.Tensor, num_segments: int, dim: int) -> torch.Tensor:
     """Scatter sum operation along the specified dimension. Modified from the
     torch_scatter library (https://github.com/rusty1s/pytorch_scatter).
 
     Args:
         input_tensor (torch.Tensor): The input tensor to be scattered.
         segment_ids (torch.Tensor): Segment ID for each element in the input tensor.
         num_segments (int): The number of segments.
@@ -188,29 +188,29 @@
         size[dim] = 0
     else:
         size[dim] = num_segments
     output = torch.zeros(size, dtype=input_tensor.dtype)
     return output.scatter_add_(dim, segment_ids, input_tensor)
 
 
-def unsorted_segment_fraction(data: torch.tensor, segment_ids: torch.tensor, num_segments: torch.tensor):
+def unsorted_segment_fraction(data: torch.Tensor, segment_ids: torch.Tensor, num_segments: int):
     """Segment fraction
     Args:
         data (torch.tensor): original data
         segment_ids (torch.tensor): segment ids
-        num_segments (torch.tensor): number of segments
+        num_segments (int): number of segments
     Returns:
         data (torch.tensor): data after fraction.
     """
     segment_sum = scatter_sum(input_tensor=data, segment_ids=segment_ids, dim=0, num_segments=num_segments)
     sums = torch.gather(segment_sum, 0, segment_ids)
     return torch.div(data, sums)
 
 
-def broadcast(input_tensor: torch.tensor, target_tensor: torch.tensor, dim: int):
+def broadcast(input_tensor: torch.Tensor, target_tensor: torch.Tensor, dim: int):
     """Broadcast input tensor along a given dimension to match the shape of the target tensor.
     Modified from torch_scatter library (https://github.com/rusty1s/pytorch_scatter).
 
     Args:
         input_tensor: The tensor to broadcast.
         target_tensor: The tensor whose shape to match.
         dim: The dimension along which to broadcast.
```

### Comparing `matgl-0.5.6/matgl/utils/sb_roots.npy` & `matgl-0.6.0/matgl/utils/sb_roots.npy`

 * *Files identical despite different names*

### Comparing `matgl-0.5.6/matgl/utils/training.py` & `matgl-0.6.0/matgl/utils/training.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 import dgl
 import numpy as np
 import pytorch_lightning as pl
 import torch
 import torch.nn.functional as F
 import torchmetrics
 from torch import nn
-from torch.optim import Optimizer, lr_scheduler
+from torch.optim import Optimizer
 
 from matgl.apps.pes import Potential
 from matgl.models import M3GNet
 
 
-class TrainerMixin:
+class MatglLightningModuleMixin:
     """Mix-in class implementing common functions for training."""
 
     def training_step(self, batch: tuple, batch_idx: int):
         """Training step.
 
         Args:
             batch: Data batch.
@@ -125,41 +125,46 @@
         Returns:
             Prediction
         """
         torch.set_grad_enabled(True)
         return self(batch)
 
 
-class ModelTrainer(TrainerMixin, pl.LightningModule):
-    """Trainer for MEGNet and M3GNet models."""
+class ModelLightningModule(MatglLightningModuleMixin, pl.LightningModule):
+    """A PyTorch.LightningModule for training MEGNet and M3GNet models."""
 
     def __init__(
         self,
         model,
         data_mean=None,
         data_std=None,
         loss: str = "mse_loss",
         optimizer: Optimizer | None = None,
-        scheduler: lr_scheduler | None = None,
+        scheduler=None,
         lr: float = 0.001,
         decay_steps: int = 1000,
         decay_alpha: float = 0.01,
+        **kwargs,
     ):
-        """Args:
-        model: Which type of the model for training
-        data_mean: average of training data
-        data_std: standard deviation of training data
-        loss: loss function used for training
-        optimizer: optimizer for training
-        scheduler: scheduler for training
-        lr: learning rate for training
-        decay_steps: number of steps for decaying learning rate
-        decay_alpha: parameter determines the minimum learning rate.
         """
-        super().__init__()
+        Init ModelLightningModule with key parameters.
+
+        Args:
+            model: Which type of the model for training
+            data_mean: average of training data
+            data_std: standard deviation of training data
+            loss: loss function used for training
+            optimizer: optimizer for training
+            scheduler: scheduler for training
+            lr: learning rate for training
+            decay_steps: number of steps for decaying learning rate
+            decay_alpha: parameter determines the minimum learning rate.
+            **kwargs: Passthrough to parent init.
+        """
+        super().__init__(**kwargs)
 
         self.model = model
 
         self.mae = torchmetrics.MeanAbsoluteError()
         self.rmse = torchmetrics.MeanSquaredError(squared=False)
         if data_mean is None:
             data_mean = torch.zeros(1)
@@ -174,15 +179,15 @@
             self.loss = F.mse_loss
         else:
             self.loss = F.l1_loss
         self.optimizer = optimizer
         self.scheduler = scheduler
         self.save_hyperparameters()
 
-    def forward(self, g: dgl.DGLGraph, l_g: dgl.DGLGraph | None = None, state_attr: torch.tensor | None = None):
+    def forward(self, g: dgl.DGLGraph, l_g: dgl.DGLGraph | None = None, state_attr: torch.Tensor | None = None):
         """Args:
             g: dgl Graph
             l_g: Line graph
             state_attr: State attribute.
 
         Returns:
             Model prediction.
@@ -199,15 +204,15 @@
             batch: Batch of training data.
 
         Returns:
             results, batch_size
         """
         g, labels, state_attr = batch
         preds = self(g=g, state_attr=state_attr)
-        results = self.loss_fn(loss=self.loss, preds=preds, labels=labels)
+        results = self.loss_fn(loss=self.loss, preds=preds, labels=labels)  # type: ignore
         batch_size = preds.numel()
         return results, batch_size
 
     def loss_fn(self, loss: nn.Module, labels: tuple, preds: tuple):
         """Args:
             loss: Loss function.
             labels: Labels to compute the loss.
@@ -218,36 +223,41 @@
         """
         total_loss = loss(labels, torch.squeeze(preds * self.data_std + self.data_mean))
         mae = self.mae(labels, torch.squeeze(preds * self.data_std + self.data_mean))
         rmse = self.rmse(labels, torch.squeeze(preds * self.data_std + self.data_mean))
         return {"Total_Loss": total_loss, "MAE": mae, "RMSE": rmse}
 
 
-class PotentialTrainer(TrainerMixin, pl.LightningModule):
-    """Trainer for MatGL potentials."""
+class PotentialLightningModule(MatglLightningModuleMixin, pl.LightningModule):
+    """A PyTorch.LightningModule for training MatGL potentials.
+
+    This is slightly different from the ModelLightningModel due to the need to account for energy, forces and stress
+    losses.
+    """
 
     def __init__(
         self,
         model,
-        element_refs: np.darray | None = None,
+        element_refs: np.ndarray | None = None,
         energy_weight: float = 1.0,
         force_weight: float = 1.0,
         stress_weight: float | None = None,
         data_mean=None,
         data_std=None,
         calc_stress: bool = False,
         loss: str = "mse_loss",
         optimizer: Optimizer | None = None,
-        scheduler: lr_scheduler | None = None,
+        scheduler=None,
         lr: float = 0.001,
         decay_steps: int = 1000,
         decay_alpha: float = 0.01,
+        **kwargs,
     ):
         """
-        Init PotentialTrainer with key parameters.
+        Init PotentialLightningModule with key parameters.
 
         Args:
             model: Which type of the model for training
             element_refs: element offset for PES
             energy_weight: relative importance of energy
             force_weight: relative importance of force
             stress_weight: relative importance of stress
@@ -256,16 +266,17 @@
             calc_stress: whether stress calculation is required
             loss: loss function used for training
             optimizer: optimizer for training
             scheduler: scheduler for training
             lr: learning rate for training
             decay_steps: number of steps for decaying learning rate
             decay_alpha: parameter determines the minimum learning rate.
+            **kwargs: Passthrough to parent init.
         """
-        super().__init__()
+        super().__init__(**kwargs)
 
         self.model = Potential(model=model, element_refs=element_refs, calc_stresses=calc_stress)
 
         self.mae = torchmetrics.MeanAbsoluteError()
         self.rmse = torchmetrics.MeanSquaredError(squared=False)
         if data_mean is None:
             data_mean = torch.zeros(1)
@@ -283,15 +294,15 @@
             self.loss = F.mse_loss
         else:
             self.loss = F.l1_loss
         self.optimizer = optimizer
         self.scheduler = scheduler
         self.save_hyperparameters()
 
-    def forward(self, g: dgl.DGLGraph, l_g: dgl.DGLGraph | None = None, state_attr: torch.tensor | None = None):
+    def forward(self, g: dgl.DGLGraph, l_g: dgl.DGLGraph | None = None, state_attr: torch.Tensor | None = None):
         """Args:
             g: dgl Graph
             l_g: Line graph
             state_attr: State attr.
 
         Returns:
             energy, force, stress, h
@@ -310,15 +321,15 @@
         g, l_g, state_attr, energies, forces, stresses = batch
         e, f, s, _ = self(g=g, state_attr=state_attr, l_g=l_g)
         f = f.to(torch.float)
         preds: tuple = (e, f, s)
         labels: tuple = (energies, forces, stresses)
         num_atoms = g.batch_num_nodes()
         results = self.loss_fn(
-            loss=self.loss,
+            loss=self.loss,  # type: ignore
             preds=preds,
             labels=labels,
             energy_weight=self.energy_weight,
             force_weight=self.force_weight,
             stress_weight=self.stress_weight,
             num_atoms=num_atoms,
         )
```

### Comparing `matgl-0.5.6/matgl.egg-info/PKG-INFO` & `matgl-0.6.0/matgl.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matgl
-Version: 0.5.6
+Version: 0.6.0
 Summary: MatGL (Materials Graph Library) is a framework for graph deep learning for materials science.
 Author: Tsz Wai Ko, Marcel Nassar, Ji Qi, Santiago Miret, Eliott Liu, Shyue Ping Ong
 Author-email: t1ko@ucsd.edu, ongsp@ucsd.edu
 Maintainer: Shyue Ping Ong
 Maintainer-email: ongsp@ucsd.edu
 Keywords: materials,interatomic potential,force field,science,property prediction,AI,machine learning,graph,deep learning
 Classifier: Development Status :: 4 - Beta
@@ -20,23 +20,23 @@
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![GitHub license](https://img.shields.io/github/license/materialsvirtuallab/matgl)](https://github.com/materialsvirtuallab/matgl/blob/main/LICENSE)
 [![Linting](https://github.com/materialsvirtuallab/matgl/workflows/Linting/badge.svg)](https://github.com/materialsvirtuallab/matgl/workflows/Linting/badge.svg)
-[![Testing](https://github.com/materialsvirtuallab/matgl/workflows/Testing%20-%20main/badge.svg)](https://github.com/materialsvirtuallab/matgl/workflows/Testing/badge.svg)
+[![Testing](https://github.com/materialsvirtuallab/matgl/workflows/Testing/badge.svg)](https://github.com/materialsvirtuallab/matgl/workflows/Testing/badge.svg)
 [![Downloads](https://pepy.tech/badge/matgl)](https://pepy.tech/project/matgl)
 [![Coverage Status](https://coveralls.io/repos/github/materialsvirtuallab/matgl/badge.svg?branch=main)](https://coveralls.io/github/materialsvirtuallab/matgl?branch=main)
 
 <img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/MatGL.png?raw=true" alt="matgl" width="30%" style="float: right">
 
 # Materials Graph Library
 
-Official Documentation: [link][doc]
+### Official Documentation: [:books:][doc]
 
 ## Introduction
 
 MatGL (Materials Graph Library) is a graph deep learning library for materials science. Mathematical graphs are a
 natural representation for a collection of atoms (e.g., molecules or crystals). Graph deep learning models have been
 shown to consistently deliver exceptional performance as surrogate models for the prediction of materials properties.
 
@@ -99,15 +99,15 @@
 ```bash
 pip install matgl
 ```
 
 For the latest dev version, please clone this repo and install using:
 
 ```bash
-python setup.py -e .
+pip install -e .
 ```
 
 ## Usage
 
 Pre-trained M3GNet universal potential and MEGNet models for the Materials Project formation energy and
 multi-fidelity band gap are now available. Users who just want to use the models out of the box should use the newly
 implemented `matgl.load_model` convenience method. The following is an example of a prediction of the formation
@@ -160,53 +160,59 @@
 > Chen, C., Ong, S.P. _A universal graph deep learning interatomic potential for the periodic table._ Nature
 > Computational Science, 2023, 2, 718–728. DOI: [10.1038/s43588-022-00349-3][m3gnet].
 
 ## FAQs
 
 1. **The `M3GNet-MP-2021.2.8-PES` differs from the original tensorflow (TF) implementation!**
 
-   Answer: `M3GNet-MP-2021.2.8-PES` is a refitted model with some data improvements and minor architectural changes.
+   _Answer:_ `M3GNet-MP-2021.2.8-PES` is a refitted model with some data improvements and minor architectural changes.
    Porting over the weights from the TF version to DGL/PyTorch is non-trivial. We have performed reasonable benchmarking
    to ensure that the new implementation reproduces the broad error characteristics of the original TF implementation
    (see [examples][jupyternb]). However, it is not expected to reproduce the TF version exactly. This refitted model
    serves as a baseline for future model improvements. We do not believe there is value in expending the resources
    to reproduce the TF version exactly.
 
 2. **I am getting errors with `matgl.load_model()`!**
 
-   Answer: The most likely reason is that you have a cached older version of the model. We often refactor models to
+   _Answer:_ The most likely reason is that you have a cached older version of the model. We often refactor models to
    ensure the best implementation. This can usually be solved by updating your matgl to the latest version
    and clearing your cache using:
 
    ```bash
    pip install matgl --upgrade
    python -c "import matgl; matgl.clear_cache()"
    ```
 
    On the next run, the latest model will be downloaded. With effect from v0.5.2, we have implemented a model
    versioning scheme that will detect code vs model version conflicts and alert the user of such problems.
 
 3. **What pre-trained models should I be using?**
 
-   Answer: There is no one definitive answer. In general, the newer the architecture and dataset, the more likely
+   _Answer:_ There is no one definitive answer. In general, the newer the architecture and dataset, the more likely
    the model performs better. However, it should also be noted that a model operating on a more diverse dataset may
    compromise on  performance on a specific system. The best way is to look at the READMEs included with each model
    and do some tests on the systems you are interested in.
 
 4. **How do I contribute to matgl?**
 
-   Answer: For code contributions, please fork and submit pull requests. You should read the [developer guide]
-   (developer) to understand the general design guidelines.
-
-   We welcome pre-trained model contributions as well, which should also be submitted via PRs. Please follow the
-   folder structure of the pretrained models. In particular, we expect all models to come with a README and notebook
+   _Answer:_ For code contributions, please fork and submit pull requests. You should read the
+   [developer guide](developer.md) to understand the general design guidelines. We welcome pre-trained model
+   contributions as well, which should also be submitted via PRs. Please follow the folder structure of the
+   pretrained models. In particular, we expect all models to come with a README and notebook
    documenting its use and its key performance metrics. Also, we expect contributions to be on new properties
    or systems or to significantly outperform the existing models. We will develop an alternative means for model
    sharing in the future.
 
+5. **None of your models do what I need. Where can I get help?**
+
+   _Answer:_ Please contact [Prof Ong][ongemail] with a brief description of your needs. For simple problems, we are
+   glad to advise and point you in the right direction. For more complicated problems, we are always open to
+   academic collaborations or projects. We also offer [consulting services][mqm] for companies with unique needs,
+   including but not limited to custom data generation, model development and materials design.
+
 ## Acknowledgments
 
 This work was primarily supported by the [Materials Project][mp], funded by the U.S. Department of Energy, Office of
 Science, Office of Basic Energy Sciences, Materials Sciences and Engineering Division under contract no.
 DE-AC02-05-CH11231: Materials Project program KC23MP. This work used the Expanse supercomputing cluster at the Extreme
 Science and Engineering Discovery Environment (XSEDE), which is supported by National Science Foundation grant number
 ACI-1548562.
@@ -221,7 +227,9 @@
 [mfimegnet]: https://www.nature.com/articles/s43588-020-00002-x "mfi MEGNet paper"
 [m3gnet]: https://www.nature.com/articles/s43588-022-00349-3 "M3GNet paper"
 [mp]: http://materialsproject.org "Materials Project"
 [apidocs]: https://matgl.ai/matgl.html "MatGL API docs"
 [doc]: https://matgl.ai "MatGL Documentation"
 [colab]: http://colab.google.com "Google Colab"
 [jupyternb]: https://github.com/materialsvirtuallab/matgl/tree/main/examples
+[ongemail]: mailto:ongsp@ucsd.edu "Email"
+[mqm]: https://materialsqm.com "MaterialsQM"
```

### Comparing `matgl-0.5.6/matgl.egg-info/SOURCES.txt` & `matgl-0.6.0/matgl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `matgl-0.5.6/pyproject.toml` & `matgl-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `matgl-0.5.6/setup.py` & `matgl-0.6.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 this_dir = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(this_dir, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="matgl",
-    version="0.5.6",
+    version="0.6.0",
     author="Tsz Wai Ko, Marcel Nassar, Ji Qi, Santiago Miret, Eliott Liu, Shyue Ping Ong",
     author_email="t1ko@ucsd.edu, ongsp@ucsd.edu",
     maintainer="Shyue Ping Ong",
     maintainer_email="ongsp@ucsd.edu",
     description="MatGL (Materials Graph Library) is a framework for graph deep learning for materials science.",
     long_description=long_description,
     long_description_content_type="text/markdown",
@@ -39,14 +39,18 @@
     install_requires=(
         "ase",
         "dgl",
         "pymatgen",
         "pytorch_lightning",
         "torch",
     ),
+    extra_requires={
+        "ase": ["ase>=3.22.1"],
+        "pymatgen": ["pymatgen>=2023.5.31"],
+    },
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

