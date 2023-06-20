# Comparing `tmp/pybefit-0.1.22.tar.gz` & `tmp/pybefit-0.1.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybefit-0.1.22.tar", last modified: Mon Jun 19 15:32:05 2023, max compression
+gzip compressed data, was "pybefit-0.1.23.tar", last modified: Tue Jun 20 08:46:02 2023, max compression
```

## Comparing `pybefit-0.1.22.tar` & `pybefit-0.1.23.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-06-19 15:32:05.661570 pybefit-0.1.22/
--rw-r--r--   0 dima      (1000) dima      (1000)     1114 2023-01-22 14:03:59.000000 pybefit-0.1.22/LICENSE.md
--rw-r--r--   0 dima      (1000) dima      (1000)      461 2023-06-19 15:32:05.661570 pybefit-0.1.22/PKG-INFO
--rw-r--r--   0 dima      (1000) dima      (1000)     2996 2023-01-22 14:03:59.000000 pybefit-0.1.22/README.md
--rw-r--r--   0 dima      (1000) dima      (1000)       79 2023-06-19 15:32:05.664903 pybefit-0.1.22/setup.cfg
--rw-r--r--   0 dima      (1000) dima      (1000)     1433 2023-06-19 15:30:30.000000 pybefit-0.1.22/setup.py
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-06-19 15:32:05.658237 pybefit-0.1.22/src/
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-06-19 15:32:05.658237 pybefit-0.1.22/src/pybefit/
--rw-r--r--   0 dima      (1000) dima      (1000)        0 2023-04-21 16:18:55.000000 pybefit-0.1.22/src/pybefit/__init__.py
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-06-19 15:32:05.661570 pybefit-0.1.22/src/pybefit/agents/
--rwxr-xr-x   0 dima      (1000) dima      (1000)       40 2023-06-13 14:22:04.000000 pybefit-0.1.22/src/pybefit/agents/__init__.py
--rwxr-xr-x   0 dima      (1000) dima      (1000)     1901 2023-06-19 15:19:44.000000 pybefit-0.1.22/src/pybefit/agents/base.py
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-06-19 15:32:05.661570 pybefit-0.1.22/src/pybefit/agents/jax/
--rw-r--r--   0 dima      (1000) dima      (1000)        0 2023-04-21 16:18:01.000000 pybefit-0.1.22/src/pybefit/agents/jax/__init__.py
--rw-r--r--   0 dima      (1000) dima      (1000)     6438 2023-01-22 14:03:59.000000 pybefit-0.1.22/src/pybefit/agents/jax/hsmm_ai.py
--rw-r--r--   0 dima      (1000) dima      (1000)      337 2023-01-22 14:03:59.000000 pybefit-0.1.22/src/pybefit/agents/jax/utils.py
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-06-19 15:32:05.661570 pybefit-0.1.22/src/pybefit/agents/torch/
--rw-r--r--   0 dima      (1000) dima      (1000)      130 2023-04-21 16:18:01.000000 pybefit-0.1.22/src/pybefit/agents/torch/__init__.py
--rwxr-xr-x   0 dima      (1000) dima      (1000)    13071 2023-04-21 16:18:01.000000 pybefit-0.1.22/src/pybefit/agents/torch/active_inference.py
--rwxr-xr-x   0 dima      (1000) dima      (1000)    21780 2023-04-21 16:18:01.000000 pybefit-0.1.22/src/pybefit/agents/torch/bayesian.py
--rw-r--r--   0 dima      (1000) dima      (1000)    22613 2023-04-21 16:18:01.000000 pybefit-0.1.22/src/pybefit/agents/torch/dynamic_programming.py
--rw-r--r--   0 dima      (1000) dima      (1000)     1190 2023-04-21 16:18:01.000000 pybefit-0.1.22/src/pybefit/agents/torch/random.py
--rwxr-xr-x   0 dima      (1000) dima      (1000)     5247 2023-04-21 16:18:01.000000 pybefit-0.1.22/src/pybefit/agents/torch/rl.py
--rw-r--r--   0 dima      (1000) dima      (1000)      484 2023-06-14 07:55:30.000000 pybefit-0.1.22/src/pybefit/agents/utils.py
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-06-19 15:32:05.661570 pybefit-0.1.22/src/pybefit/inference/
--rwxr-xr-x   0 dima      (1000) dima      (1000)       92 2023-04-21 16:18:01.000000 pybefit-0.1.22/src/pybefit/inference/__init__.py
--rwxr-xr-x   0 dima      (1000) dima      (1000)    10166 2023-06-19 11:01:13.000000 pybefit-0.1.22/src/pybefit/inference/methods.py
--rw-r--r--   0 dima      (1000) dima      (1000)     1610 2023-04-21 16:18:01.000000 pybefit-0.1.22/src/pybefit/inference/models.py
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-06-19 15:32:05.661570 pybefit-0.1.22/src/pybefit/inference/numpyro/
--rw-r--r--   0 dima      (1000) dima      (1000)        0 2023-04-21 16:18:01.000000 pybefit-0.1.22/src/pybefit/inference/numpyro/__init__.py
--rw-r--r--   0 dima      (1000) dima      (1000)     4114 2023-06-19 14:30:28.000000 pybefit-0.1.22/src/pybefit/inference/numpyro/likelihoods.py
--rw-r--r--   0 dima      (1000) dima      (1000)     6507 2023-04-21 16:18:01.000000 pybefit-0.1.22/src/pybefit/inference/numpyro/regression.py
--rw-r--r--   0 dima      (1000) dima      (1000)     5489 2023-06-19 10:51:25.000000 pybefit-0.1.22/src/pybefit/inference/posteriors.py
--rw-r--r--   0 dima      (1000) dima      (1000)     5906 2023-06-19 10:40:53.000000 pybefit-0.1.22/src/pybefit/inference/priors.py
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-06-19 15:32:05.661570 pybefit-0.1.22/src/pybefit/inference/pyro/
--rw-r--r--   0 dima      (1000) dima      (1000)       20 2023-04-21 16:18:01.000000 pybefit-0.1.22/src/pybefit/inference/pyro/__init__.py
--rwxr-xr-x   0 dima      (1000) dima      (1000)     4860 2023-04-21 16:18:01.000000 pybefit-0.1.22/src/pybefit/inference/pyro/flat.py
--rwxr-xr-x   0 dima      (1000) dima      (1000)    10394 2023-04-21 16:18:01.000000 pybefit-0.1.22/src/pybefit/inference/pyro/hierarchical.py
--rwxr-xr-x   0 dima      (1000) dima      (1000)     8701 2023-04-21 16:18:01.000000 pybefit-0.1.22/src/pybefit/inference/pyro/infer.py
--rw-r--r--   0 dima      (1000) dima      (1000)     2580 2023-06-19 14:30:19.000000 pybefit-0.1.22/src/pybefit/inference/pyro/likelihoods.py
--rw-r--r--   0 dima      (1000) dima      (1000)     6139 2023-04-21 16:18:01.000000 pybefit-0.1.22/src/pybefit/inference/pyro/mixed.py
--rwxr-xr-x   0 dima      (1000) dima      (1000)     8109 2023-04-21 16:18:01.000000 pybefit-0.1.22/src/pybefit/inference/pyro/nonparametric.py
--rw-r--r--   0 dima      (1000) dima      (1000)     6575 2023-04-21 16:18:01.000000 pybefit-0.1.22/src/pybefit/inference/regression.py
--rwxr--r--   0 dima      (1000) dima      (1000)     2916 2023-01-22 14:03:59.000000 pybefit-0.1.22/src/pybefit/simulate.py
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-06-19 15:32:05.661570 pybefit-0.1.22/src/pybefit/tasks/
--rwxr--r--   0 dima      (1000) dima      (1000)       78 2023-06-13 14:32:29.000000 pybefit-0.1.22/src/pybefit/tasks/__init__.py
--rwxr--r--   0 dima      (1000) dima      (1000)     4230 2023-06-13 14:55:44.000000 pybefit-0.1.22/src/pybefit/tasks/bandits.py
--rw-r--r--   0 dima      (1000) dima      (1000)      798 2023-06-13 16:41:50.000000 pybefit-0.1.22/src/pybefit/tasks/base.py
--rwxr--r--   0 dima      (1000) dima      (1000)     2594 2023-06-13 15:22:54.000000 pybefit-0.1.22/src/pybefit/tasks/rev_learning.py
--rw-r--r--   0 dima      (1000) dima      (1000)     3722 2023-06-13 15:04:34.000000 pybefit-0.1.22/src/pybefit/tasks/sat.py
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-06-19 15:32:05.661570 pybefit-0.1.22/src/pybefit.egg-info/
--rw-r--r--   0 dima      (1000) dima      (1000)      461 2023-06-19 15:32:05.000000 pybefit-0.1.22/src/pybefit.egg-info/PKG-INFO
--rw-r--r--   0 dima      (1000) dima      (1000)     1434 2023-06-19 15:32:05.000000 pybefit-0.1.22/src/pybefit.egg-info/SOURCES.txt
--rw-r--r--   0 dima      (1000) dima      (1000)        1 2023-06-19 15:32:05.000000 pybefit-0.1.22/src/pybefit.egg-info/dependency_links.txt
--rw-r--r--   0 dima      (1000) dima      (1000)      104 2023-06-19 15:32:05.000000 pybefit-0.1.22/src/pybefit.egg-info/requires.txt
--rw-r--r--   0 dima      (1000) dima      (1000)        8 2023-06-19 15:32:05.000000 pybefit-0.1.22/src/pybefit.egg-info/top_level.txt
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-06-20 08:46:02.292999 pybefit-0.1.23/
+-rw-r--r--   0 dima      (1000) dima      (1000)     1114 2023-01-22 14:03:59.000000 pybefit-0.1.23/LICENSE.md
+-rw-r--r--   0 dima      (1000) dima      (1000)      461 2023-06-20 08:46:02.292999 pybefit-0.1.23/PKG-INFO
+-rw-r--r--   0 dima      (1000) dima      (1000)     3019 2023-06-20 07:44:34.000000 pybefit-0.1.23/README.md
+-rw-r--r--   0 dima      (1000) dima      (1000)       79 2023-06-20 08:46:02.292999 pybefit-0.1.23/setup.cfg
+-rw-r--r--   0 dima      (1000) dima      (1000)     1419 2023-06-20 07:43:41.000000 pybefit-0.1.23/setup.py
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-06-20 08:46:02.286330 pybefit-0.1.23/src/
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-06-20 08:46:02.289664 pybefit-0.1.23/src/pybefit/
+-rw-r--r--   0 dima      (1000) dima      (1000)        0 2023-04-21 16:18:55.000000 pybefit-0.1.23/src/pybefit/__init__.py
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-06-20 08:46:02.289664 pybefit-0.1.23/src/pybefit/agents/
+-rwxr--r--   0 dima      (1000) dima      (1000)       40 2023-06-13 14:22:04.000000 pybefit-0.1.23/src/pybefit/agents/__init__.py
+-rwxr--r--   0 dima      (1000) dima      (1000)     1901 2023-06-19 15:19:44.000000 pybefit-0.1.23/src/pybefit/agents/base.py
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-06-20 08:46:02.289664 pybefit-0.1.23/src/pybefit/agents/jax/
+-rw-r--r--   0 dima      (1000) dima      (1000)        0 2023-04-21 16:18:01.000000 pybefit-0.1.23/src/pybefit/agents/jax/__init__.py
+-rw-r--r--   0 dima      (1000) dima      (1000)     6438 2023-01-22 14:03:59.000000 pybefit-0.1.23/src/pybefit/agents/jax/hsmm_ai.py
+-rw-r--r--   0 dima      (1000) dima      (1000)      337 2023-01-22 14:03:59.000000 pybefit-0.1.23/src/pybefit/agents/jax/utils.py
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-06-20 08:46:02.289664 pybefit-0.1.23/src/pybefit/agents/torch/
+-rw-r--r--   0 dima      (1000) dima      (1000)      130 2023-04-21 16:18:01.000000 pybefit-0.1.23/src/pybefit/agents/torch/__init__.py
+-rwxr--r--   0 dima      (1000) dima      (1000)    13071 2023-04-21 16:18:01.000000 pybefit-0.1.23/src/pybefit/agents/torch/active_inference.py
+-rwxr--r--   0 dima      (1000) dima      (1000)    21780 2023-04-21 16:18:01.000000 pybefit-0.1.23/src/pybefit/agents/torch/bayesian.py
+-rw-r--r--   0 dima      (1000) dima      (1000)    22613 2023-04-21 16:18:01.000000 pybefit-0.1.23/src/pybefit/agents/torch/dynamic_programming.py
+-rw-r--r--   0 dima      (1000) dima      (1000)     1190 2023-04-21 16:18:01.000000 pybefit-0.1.23/src/pybefit/agents/torch/random.py
+-rwxr--r--   0 dima      (1000) dima      (1000)     5247 2023-04-21 16:18:01.000000 pybefit-0.1.23/src/pybefit/agents/torch/rl.py
+-rw-r--r--   0 dima      (1000) dima      (1000)      484 2023-06-13 15:23:11.000000 pybefit-0.1.23/src/pybefit/agents/utils.py
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-06-20 08:46:02.289664 pybefit-0.1.23/src/pybefit/inference/
+-rwxr--r--   0 dima      (1000) dima      (1000)       92 2023-04-21 16:18:01.000000 pybefit-0.1.23/src/pybefit/inference/__init__.py
+-rwxr--r--   0 dima      (1000) dima      (1000)    10166 2023-06-19 11:01:13.000000 pybefit-0.1.23/src/pybefit/inference/methods.py
+-rw-r--r--   0 dima      (1000) dima      (1000)     1610 2023-04-21 16:18:01.000000 pybefit-0.1.23/src/pybefit/inference/models.py
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-06-20 08:46:02.289664 pybefit-0.1.23/src/pybefit/inference/numpyro/
+-rw-r--r--   0 dima      (1000) dima      (1000)        0 2023-04-21 16:18:01.000000 pybefit-0.1.23/src/pybefit/inference/numpyro/__init__.py
+-rw-r--r--   0 dima      (1000) dima      (1000)     4114 2023-06-19 14:30:28.000000 pybefit-0.1.23/src/pybefit/inference/numpyro/likelihoods.py
+-rw-r--r--   0 dima      (1000) dima      (1000)     6507 2023-04-21 16:18:01.000000 pybefit-0.1.23/src/pybefit/inference/numpyro/regression.py
+-rw-r--r--   0 dima      (1000) dima      (1000)     5489 2023-06-19 10:51:25.000000 pybefit-0.1.23/src/pybefit/inference/posteriors.py
+-rw-r--r--   0 dima      (1000) dima      (1000)     6013 2023-06-19 15:49:33.000000 pybefit-0.1.23/src/pybefit/inference/priors.py
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-06-20 08:46:02.292999 pybefit-0.1.23/src/pybefit/inference/pyro/
+-rw-r--r--   0 dima      (1000) dima      (1000)       20 2023-04-21 16:18:01.000000 pybefit-0.1.23/src/pybefit/inference/pyro/__init__.py
+-rwxr-xr-x   0 dima      (1000) dima      (1000)     4860 2023-04-21 16:18:01.000000 pybefit-0.1.23/src/pybefit/inference/pyro/flat.py
+-rwxr-xr-x   0 dima      (1000) dima      (1000)    10394 2023-04-21 16:18:01.000000 pybefit-0.1.23/src/pybefit/inference/pyro/hierarchical.py
+-rwxr-xr-x   0 dima      (1000) dima      (1000)     8701 2023-04-21 16:18:01.000000 pybefit-0.1.23/src/pybefit/inference/pyro/infer.py
+-rw-r--r--   0 dima      (1000) dima      (1000)     2580 2023-06-19 14:30:19.000000 pybefit-0.1.23/src/pybefit/inference/pyro/likelihoods.py
+-rw-r--r--   0 dima      (1000) dima      (1000)     6139 2023-04-21 16:18:01.000000 pybefit-0.1.23/src/pybefit/inference/pyro/mixed.py
+-rwxr-xr-x   0 dima      (1000) dima      (1000)     8109 2023-04-21 16:18:01.000000 pybefit-0.1.23/src/pybefit/inference/pyro/nonparametric.py
+-rw-r--r--   0 dima      (1000) dima      (1000)     6575 2023-04-21 16:18:01.000000 pybefit-0.1.23/src/pybefit/inference/regression.py
+-rwxr-xr-x   0 dima      (1000) dima      (1000)     2916 2023-01-22 14:03:59.000000 pybefit-0.1.23/src/pybefit/simulate.py
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-06-20 08:46:02.292999 pybefit-0.1.23/src/pybefit/tasks/
+-rwxr--r--   0 dima      (1000) dima      (1000)       78 2023-06-13 14:32:29.000000 pybefit-0.1.23/src/pybefit/tasks/__init__.py
+-rwxr--r--   0 dima      (1000) dima      (1000)     4230 2023-06-13 14:52:56.000000 pybefit-0.1.23/src/pybefit/tasks/bandits.py
+-rw-r--r--   0 dima      (1000) dima      (1000)      798 2023-06-13 16:41:28.000000 pybefit-0.1.23/src/pybefit/tasks/base.py
+-rwxr--r--   0 dima      (1000) dima      (1000)     2594 2023-06-13 15:22:54.000000 pybefit-0.1.23/src/pybefit/tasks/rev_learning.py
+-rw-r--r--   0 dima      (1000) dima      (1000)     3722 2023-06-13 15:04:28.000000 pybefit-0.1.23/src/pybefit/tasks/sat.py
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-06-20 08:46:02.289664 pybefit-0.1.23/src/pybefit.egg-info/
+-rw-r--r--   0 dima      (1000) dima      (1000)      461 2023-06-20 08:46:02.000000 pybefit-0.1.23/src/pybefit.egg-info/PKG-INFO
+-rw-r--r--   0 dima      (1000) dima      (1000)     1434 2023-06-20 08:46:02.000000 pybefit-0.1.23/src/pybefit.egg-info/SOURCES.txt
+-rw-r--r--   0 dima      (1000) dima      (1000)        1 2023-06-20 08:46:02.000000 pybefit-0.1.23/src/pybefit.egg-info/dependency_links.txt
+-rw-r--r--   0 dima      (1000) dima      (1000)       98 2023-06-20 08:46:02.000000 pybefit-0.1.23/src/pybefit.egg-info/requires.txt
+-rw-r--r--   0 dima      (1000) dima      (1000)        8 2023-06-20 08:46:02.000000 pybefit-0.1.23/src/pybefit.egg-info/top_level.txt
```

### Comparing `pybefit-0.1.22/LICENSE.md` & `pybefit-0.1.23/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.22/README.md` & `pybefit-0.1.23/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 # Probabilistic inference for models of behaviour
 =================================================
 
 PyBefit is a Python library for Bayesian analysis of behavioral data. It is based on [Pyro/Numpyro](pyro.ai) a probabilistic programing language, [PyTorch](https://pytorch.org/), and [Jax](https://github.com/google/jax) machine learning libraries.
 
 Requirements
 ------------
-    numpy
-    pandas
-    matplotlib
-    seaborn
     pyro
     pytorch
     numpyro
     jax
-    jaxlib
-
+    [Optional]
+     - matplolib
+     - seaborn
+     - arviz
+     - jupyterlab
+    
 Installation
 ------------
 To install PyBefit with CPU-only versions of JAX and PyTorch you can run
 ```sh
 pip install pip --upgrade
 pip install pybefit --upgrade
 ```
 ### Conda installation
 To install either JAX or Pytorch with Nvidia GPU support we recomment using [anaconda](https://conda.io/miniconda.html) package manager. First create pybefit environment and activate it
 ```sh
-conda create -n befit python=3.10
+conda create -n befit python=3.11
 conda activate befit
 ```
 Then follow instructions for installing [JAX](https://github.com/google/jax#installation) or [Pytorch](https://pytorch.org/) with GPU support.
 
 Finally install pybefit via pip within the conda environment
 ```sh
 pip install pip --upgrade
```

### Comparing `pybefit-0.1.22/setup.py` & `pybefit-0.1.23/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,25 +14,23 @@
  'pybefit.inference.numpyro',
  'pybefit.tasks']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['jax',
- 'numpy',
- 'numpyro',
+['numpyro',
  'optax',
  'torch',
  'pyro-ppl',
- 'pandas',
  'pycm',
  'seaborn',
  'matplotlib',
  'arviz',
+ 'jupyterlab',
  'jupyterthemes',
  'jupyter-black']
 
 classifiers = \
 [
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
@@ -40,15 +38,15 @@
     'Topic :: Scientific/Engineering',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3.10'
 ]
 
 setup_kwargs = {
     'name': 'pybefit',
-    'version': '0.1.22',
+    'version': '0.1.23',
     'description': 'Probabilistic inference for models of behaviour',
     'long_description': 'PyBefit is a Python library for Bayesian analysis of behavioral data. It is based on Pyro/Numpyro a probabilistic programing language, PyTorch, and Jax machine learning libraries.',
     'author': 'Dimitrije Marković',
     'author_email': 'dimitrije.markovic@tu-dresden.de',
     'url': 'https://github.com/dimarkov/pybefit',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `pybefit-0.1.22/src/pybefit/agents/base.py` & `pybefit-0.1.23/src/pybefit/agents/base.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.22/src/pybefit/agents/jax/hsmm_ai.py` & `pybefit-0.1.23/src/pybefit/agents/jax/hsmm_ai.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.22/src/pybefit/agents/torch/active_inference.py` & `pybefit-0.1.23/src/pybefit/agents/torch/active_inference.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.22/src/pybefit/agents/torch/bayesian.py` & `pybefit-0.1.23/src/pybefit/agents/torch/bayesian.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.22/src/pybefit/agents/torch/dynamic_programming.py` & `pybefit-0.1.23/src/pybefit/agents/torch/dynamic_programming.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.22/src/pybefit/agents/torch/random.py` & `pybefit-0.1.23/src/pybefit/agents/torch/random.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.22/src/pybefit/agents/torch/rl.py` & `pybefit-0.1.23/src/pybefit/agents/torch/rl.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.22/src/pybefit/inference/methods.py` & `pybefit-0.1.23/src/pybefit/inference/methods.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.22/src/pybefit/inference/models.py` & `pybefit-0.1.23/src/pybefit/inference/models.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.22/src/pybefit/inference/numpyro/likelihoods.py` & `pybefit-0.1.23/src/pybefit/inference/numpyro/likelihoods.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.22/src/pybefit/inference/numpyro/regression.py` & `pybefit-0.1.23/src/pybefit/inference/numpyro/regression.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.22/src/pybefit/inference/posteriors.py` & `pybefit-0.1.23/src/pybefit/inference/posteriors.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.22/src/pybefit/inference/priors.py` & `pybefit-0.1.23/src/pybefit/inference/priors.py`

 * *Files 6% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 
         return z
 
 
 class NormalGamma(ModelBase):
     """NormalGamma over free model parameters.
     """
-    def __init__(self, num_params, num_agents, init_scale=1., backend=BACKEND):
+    def __init__(self, num_params, num_agents, init_scale=.5, backend=BACKEND):
         super().__init__(num_params=num_params, num_agents=num_agents, backend=backend)
         self.init_scale = init_scale
 
     def __call__(self, *args, **kwargs):
         na = self.num_agents
         np = self.num_params
 
@@ -128,23 +128,27 @@
         return z
 
 
 class RegularisedHorseshoe(ModelBase):
     """Regularised horseshoe prior over free model parameters. For details see: Piironen, Juho, and Aki Vehtari. "Sparsity information and regularization in the horseshoe and other shrinkage priors." (2017): 5018-5051.
     """
 
-    def __init__(self, num_params, num_agents, backend=BACKEND):
+    def __init__(self, num_params, num_agents, init_scale=1., backend=BACKEND):
         super().__init__(num_params=num_params, num_agents=num_agents, backend=backend)
+        self.init_scale = init_scale
 
     def __call__(self, *args, **kwargs):
         na = self.num_agents
         np = self.num_params
+        iscl = self.init_scale
 
         # each model parameter has a hyperparameter defining a group level mean
-        mu = self.sample('mu', self.dist.Normal(self.tensor.zeros(np), 10 * self.tensor.ones(np)).to_event(1))
+        mu = self.sample(
+            'mu', self.dist.Normal(self.tensor.zeros(np), iscl * self.tensor.ones(np)).to_event(1)
+        )
 
         # define prior uncertanty over model parameters
         c_sqr_inv = self.sample('c^{-2}', self.dist.Gamma(2 * self.tensor.ones(1), 2 * self.tensor.ones(1)).to_event(1))
 
         u = self.sample('u', self.dist.Gamma(self.tensor.ones(np + 1)/2, self.tensor.ones(np + 1)).to_event(1))
         v = self.sample('v', self.dist.Gamma(self.tensor.ones(np + 1)/2, self.tensor.ones(np + 1)).to_event(1))
```

### Comparing `pybefit-0.1.22/src/pybefit/inference/pyro/flat.py` & `pybefit-0.1.23/src/pybefit/inference/pyro/flat.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.22/src/pybefit/inference/pyro/hierarchical.py` & `pybefit-0.1.23/src/pybefit/inference/pyro/hierarchical.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.22/src/pybefit/inference/pyro/infer.py` & `pybefit-0.1.23/src/pybefit/inference/pyro/infer.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.22/src/pybefit/inference/pyro/likelihoods.py` & `pybefit-0.1.23/src/pybefit/inference/pyro/likelihoods.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.22/src/pybefit/inference/pyro/mixed.py` & `pybefit-0.1.23/src/pybefit/inference/pyro/mixed.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.22/src/pybefit/inference/pyro/nonparametric.py` & `pybefit-0.1.23/src/pybefit/inference/pyro/nonparametric.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.22/src/pybefit/inference/regression.py` & `pybefit-0.1.23/src/pybefit/inference/regression.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.22/src/pybefit/simulate.py` & `pybefit-0.1.23/src/pybefit/simulate.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.22/src/pybefit/tasks/bandits.py` & `pybefit-0.1.23/src/pybefit/tasks/bandits.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.22/src/pybefit/tasks/base.py` & `pybefit-0.1.23/src/pybefit/tasks/base.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.22/src/pybefit/tasks/rev_learning.py` & `pybefit-0.1.23/src/pybefit/tasks/rev_learning.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.22/src/pybefit/tasks/sat.py` & `pybefit-0.1.23/src/pybefit/tasks/sat.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.22/src/pybefit.egg-info/SOURCES.txt` & `pybefit-0.1.23/src/pybefit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

