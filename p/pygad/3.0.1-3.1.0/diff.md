# Comparing `tmp/pygad-3.0.1.tar.gz` & `tmp/pygad-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygad-3.0.1.tar", last modified: Thu Apr 20 13:31:16 2023, max compression
+gzip compressed data, was "pygad-3.1.0.tar", last modified: Tue Jun 20 19:10:29 2023, max compression
```

## Comparing `pygad-3.0.1.tar` & `pygad-3.1.0.tar`

### file list

```diff
@@ -1,43 +1,45 @@
-drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-04-20 13:31:16.074518 pygad-3.0.1/
--rw-rw-r--   0 ahmedgad  (1000) ahmedgad  (1000)    18208 2023-04-20 13:31:16.074518 pygad-3.0.1/PKG-INFO
--rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)    17829 2023-04-08 18:12:48.000000 pygad-3.0.1/README.md
-drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-04-20 13:31:16.018519 pygad-3.0.1/pygad/
--rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)       63 2023-04-20 13:25:25.000000 pygad-3.0.1/pygad/__init__.py
-drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-04-20 13:31:16.022519 pygad-3.0.1/pygad/cnn/
--rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)       43 2023-02-23 13:33:40.000000 pygad-3.0.1/pygad/cnn/__init__.py
--rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)    37968 2023-02-23 13:33:40.000000 pygad-3.0.1/pygad/cnn/cnn.py
-drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-04-20 13:31:16.022519 pygad-3.0.1/pygad/gacnn/
--rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)       45 2023-02-23 13:33:40.000000 pygad-3.0.1/pygad/gacnn/__init__.py
--rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)     5166 2023-02-23 13:33:40.000000 pygad-3.0.1/pygad/gacnn/gacnn.py
-drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-04-20 13:31:16.026519 pygad-3.0.1/pygad/gann/
--rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)       44 2023-02-23 13:33:40.000000 pygad-3.0.1/pygad/gann/__init__.py
--rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)    21058 2023-02-23 13:33:40.000000 pygad-3.0.1/pygad/gann/gann.py
-drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-04-20 13:31:16.026519 pygad-3.0.1/pygad/helper/
--rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)       54 2023-04-03 22:17:26.000000 pygad-3.0.1/pygad/helper/__init__.py
--rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)    47690 2023-02-28 16:43:38.000000 pygad-3.0.1/pygad/helper/unique.py
-drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-04-20 13:31:16.030519 pygad-3.0.1/pygad/kerasga/
--rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)       46 2023-04-03 22:17:19.000000 pygad-3.0.1/pygad/kerasga/__init__.py
--rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)     3243 2023-03-01 16:53:25.000000 pygad-3.0.1/pygad/kerasga/kerasga.py
-drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-04-20 13:31:16.038519 pygad-3.0.1/pygad/nn/
--rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)       42 2023-02-23 13:33:40.000000 pygad-3.0.1/pygad/nn/__init__.py
--rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)    19363 2023-02-23 13:33:40.000000 pygad-3.0.1/pygad/nn/nn.py
--rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)   217095 2023-04-20 13:24:25.000000 pygad-3.0.1/pygad/pygad.py
-drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-04-20 13:31:16.050518 pygad-3.0.1/pygad/torchga/
--rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)       46 2023-04-03 22:17:09.000000 pygad-3.0.1/pygad/torchga/__init__.py
--rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)     3362 2023-03-01 17:53:14.000000 pygad-3.0.1/pygad/torchga/torchga.py
-drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-04-20 13:31:16.058518 pygad-3.0.1/pygad/utils/
--rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)      130 2023-04-03 22:16:41.000000 pygad-3.0.1/pygad/utils/__init__.py
--rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)    13968 2023-03-02 02:30:43.000000 pygad-3.0.1/pygad/utils/crossover.py
--rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)    53487 2023-03-02 02:41:53.000000 pygad-3.0.1/pygad/utils/mutation.py
--rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)    10106 2023-04-03 22:10:06.000000 pygad-3.0.1/pygad/utils/parent_selection.py
-drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-04-20 13:31:16.062518 pygad-3.0.1/pygad/visualize/
--rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)       55 2023-04-03 22:16:52.000000 pygad-3.0.1/pygad/visualize/__init__.py
--rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)    18572 2023-02-28 16:43:27.000000 pygad-3.0.1/pygad/visualize/plot.py
-drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-04-20 13:31:16.022519 pygad-3.0.1/pygad.egg-info/
--rw-rw-r--   0 ahmedgad  (1000) ahmedgad  (1000)    18208 2023-04-20 13:31:15.000000 pygad-3.0.1/pygad.egg-info/PKG-INFO
--rw-rw-r--   0 ahmedgad  (1000) ahmedgad  (1000)      664 2023-04-20 13:31:15.000000 pygad-3.0.1/pygad.egg-info/SOURCES.txt
--rw-rw-r--   0 ahmedgad  (1000) ahmedgad  (1000)        1 2023-04-20 13:31:15.000000 pygad-3.0.1/pygad.egg-info/dependency_links.txt
--rw-rw-r--   0 ahmedgad  (1000) ahmedgad  (1000)       29 2023-04-20 13:31:15.000000 pygad-3.0.1/pygad.egg-info/requires.txt
--rw-rw-r--   0 ahmedgad  (1000) ahmedgad  (1000)        6 2023-04-20 13:31:15.000000 pygad-3.0.1/pygad.egg-info/top_level.txt
--rw-rw-r--   0 ahmedgad  (1000) ahmedgad  (1000)       38 2023-04-20 13:31:16.074518 pygad-3.0.1/setup.cfg
--rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)      637 2023-04-20 13:29:39.000000 pygad-3.0.1/setup.py
+drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-06-20 19:10:29.769369 pygad-3.1.0/
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)     1494 2023-06-20 19:02:41.000000 pygad-3.1.0/LICENSE
+-rw-rw-r--   0 ahmedgad  (1000) ahmedgad  (1000)    18004 2023-06-20 19:10:29.769369 pygad-3.1.0/PKG-INFO
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)    17936 2023-06-20 19:02:41.000000 pygad-3.1.0/README.md
+drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-06-20 19:10:29.761366 pygad-3.1.0/pygad/
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)       66 2023-06-20 19:02:42.000000 pygad-3.1.0/pygad/__init__.py
+drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-06-20 19:10:29.761366 pygad-3.1.0/pygad/cnn/
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)       47 2023-06-20 19:02:42.000000 pygad-3.1.0/pygad/cnn/__init__.py
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)    43732 2023-06-20 19:02:42.000000 pygad-3.1.0/pygad/cnn/cnn.py
+drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-06-20 19:10:29.769369 pygad-3.1.0/pygad/gacnn/
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)       49 2023-06-20 19:02:42.000000 pygad-3.1.0/pygad/gacnn/__init__.py
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)     5166 2023-06-20 19:02:42.000000 pygad-3.1.0/pygad/gacnn/gacnn.py
+drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-06-20 19:10:29.769369 pygad-3.1.0/pygad/gann/
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)       48 2023-06-20 19:02:42.000000 pygad-3.1.0/pygad/gann/__init__.py
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)    20882 2023-06-20 19:02:42.000000 pygad-3.1.0/pygad/gann/gann.py
+drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-06-20 19:10:29.769369 pygad-3.1.0/pygad/helper/
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)       56 2023-06-20 19:02:42.000000 pygad-3.1.0/pygad/helper/__init__.py
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)    53096 2023-06-20 19:02:42.000000 pygad-3.1.0/pygad/helper/unique.py
+drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-06-20 19:10:29.769369 pygad-3.1.0/pygad/kerasga/
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)       49 2023-06-20 19:02:42.000000 pygad-3.1.0/pygad/kerasga/__init__.py
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)     4972 2023-06-20 19:02:42.000000 pygad-3.1.0/pygad/kerasga/kerasga.py
+drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-06-20 19:10:29.769369 pygad-3.1.0/pygad/nn/
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)       46 2023-06-20 19:02:42.000000 pygad-3.1.0/pygad/nn/__init__.py
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)    18932 2023-06-20 19:02:42.000000 pygad-3.1.0/pygad/nn/nn.py
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)   190568 2023-06-20 19:02:42.000000 pygad-3.1.0/pygad/pygad.py
+drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-06-20 19:10:29.769369 pygad-3.1.0/pygad/torchga/
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)       49 2023-06-20 19:02:42.000000 pygad-3.1.0/pygad/torchga/__init__.py
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)     3362 2023-06-20 19:02:42.000000 pygad-3.1.0/pygad/torchga/torchga.py
+drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-06-20 19:10:29.769369 pygad-3.1.0/pygad/utils/
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)      134 2023-06-20 19:02:42.000000 pygad-3.1.0/pygad/utils/__init__.py
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)    13974 2023-06-20 19:02:42.000000 pygad-3.1.0/pygad/utils/crossover.py
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)    59935 2023-06-20 19:02:42.000000 pygad-3.1.0/pygad/utils/mutation.py
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)    11148 2023-06-20 19:02:42.000000 pygad-3.1.0/pygad/utils/parent_selection.py
+drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-06-20 19:10:29.769369 pygad-3.1.0/pygad/visualize/
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)       57 2023-06-20 19:02:42.000000 pygad-3.1.0/pygad/visualize/__init__.py
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)    18552 2023-06-20 19:02:42.000000 pygad-3.1.0/pygad/visualize/plot.py
+drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-06-20 19:10:29.761366 pygad-3.1.0/pygad.egg-info/
+-rw-rw-r--   0 ahmedgad  (1000) ahmedgad  (1000)    18004 2023-06-20 19:10:29.000000 pygad-3.1.0/pygad.egg-info/PKG-INFO
+-rw-rw-r--   0 ahmedgad  (1000) ahmedgad  (1000)      687 2023-06-20 19:10:29.000000 pygad-3.1.0/pygad.egg-info/SOURCES.txt
+-rw-rw-r--   0 ahmedgad  (1000) ahmedgad  (1000)        1 2023-06-20 19:10:29.000000 pygad-3.1.0/pygad.egg-info/dependency_links.txt
+-rw-rw-r--   0 ahmedgad  (1000) ahmedgad  (1000)       29 2023-06-20 19:10:29.000000 pygad-3.1.0/pygad.egg-info/requires.txt
+-rw-rw-r--   0 ahmedgad  (1000) ahmedgad  (1000)        6 2023-06-20 19:10:29.000000 pygad-3.1.0/pygad.egg-info/top_level.txt
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)     2394 2023-06-20 19:02:42.000000 pygad-3.1.0/pyproject.toml
+-rw-rw-r--   0 ahmedgad  (1000) ahmedgad  (1000)       38 2023-06-20 19:10:29.769369 pygad-3.1.0/setup.cfg
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)      636 2023-06-20 19:02:42.000000 pygad-3.1.0/setup.py
```

### Comparing `pygad-3.0.1/PKG-INFO` & `pygad-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: pygad
-Version: 3.0.1
-Summary: PyGAD: A Python 3 Library for Building the Genetic Algorithm and Training Machine Learning Algoithms (Keras & PyTorch).
+Version: 3.1.0
+Summary: PyGAD: A Python Library for Building the Genetic Algorithm and Training Machine Learning Algoithms (Keras & PyTorch).
 Home-page: https://github.com/ahmedfgad/GeneticAlgorithmPython
 Author: Ahmed Fawzy Gad
 Author-email: ahmed.f.gad@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # PyGAD:  Genetic Algorithm in Python
 
 [PyGAD](https://pypi.org/project/pygad) is an open-source easy-to-use Python 3 library for building the genetic algorithm and optimizing machine learning algorithms. It supports Keras and PyTorch.
 
 Check documentation of the [PyGAD](https://pygad.readthedocs.io/en/latest).
 
@@ -21,31 +22,29 @@
 
 [PyGAD](https://pypi.org/project/pygad) supports different types of crossover, mutation, and parent selection. [PyGAD](https://pypi.org/project/pygad) allows different types of problems to be optimized using the genetic algorithm by customizing the fitness function. 
 
 The library is under active development and more features are added regularly. If you want a feature to be supported, please check the **Contact Us** section to send a request.
 
 # Donation
 
-- [Credit/Debit Card](https://donate.stripe.com/eVa5kO866elKgM0144): https://donate.stripe.com/eVa5kO866elKgM0144
-- [Open Collective](https://opencollective.com/pygad): [opencollective.com/pygad](https://opencollective.com/pygad)
-- PayPal: Use either this link: [paypal.me/ahmedfgad](https://paypal.me/ahmedfgad) or the e-mail address ahmed.f.gad@gmail.com
-- Interac e-Transfer: Use e-mail address ahmed.f.gad@gmail.com
+* [Credit/Debit Card](https://donate.stripe.com/eVa5kO866elKgM0144): https://donate.stripe.com/eVa5kO866elKgM0144
+* [Open Collective](https://opencollective.com/pygad): [opencollective.com/pygad](https://opencollective.com/pygad)
+* PayPal: Use either this link: [paypal.me/ahmedfgad](https://paypal.me/ahmedfgad) or the e-mail address ahmed.f.gad@gmail.com
+* Interac e-Transfer: Use e-mail address ahmed.f.gad@gmail.com
 
 # Installation
 
-To install [PyGAD](https://pypi.org/project/pygad), simply use pip to download and install the library from [PyPI](https://pypi.org/project/pygad) (Python Package Index). The library lives a PyPI at this page https://pypi.org/project/pygad.
+To install [PyGAD](https://pypi.org/project/pygad), simply use pip to download and install the library from [PyPI](https://pypi.org/project/pygad) (Python Package Index). The library is at PyPI at this page https://pypi.org/project/pygad.
 
 Install PyGAD with the following command:
 
 ```python
 pip install pygad
 ```
 
-PyGAD is developed in Python 3.7.3 and depends on NumPy for creating and manipulating arrays and Matplotlib for creating figures. The exact NumPy version used in developing PyGAD is 1.16.4. For Matplotlib, the version is 3.1.0.
-
 To get started with PyGAD, please read the documentation at [Read The Docs](https://pygad.readthedocs.io/) https://pygad.readthedocs.io.
 
 # PyGAD Source Code
 
 The source code of the PyGAD' modules is found in the following GitHub projects:
 
 - [pygad](https://github.com/ahmedfgad/GeneticAlgorithmPython): (https://github.com/ahmedfgad/GeneticAlgorithmPython)
@@ -83,15 +82,15 @@
 ```python
 import pygad
 import numpy
 
 function_inputs = [4,-2,3.5,5,-11,-4.7]
 desired_output = 44
 
-def fitness_func(solution, solution_idx):
+def fitness_func(ga_instance, solution, solution_idx):
     output = numpy.sum(solution*function_inputs)
     fitness = 1.0 / (numpy.abs(output - desired_output) + 0.000001)
     return fitness
 
 fitness_function = fitness_func
 
 def on_start(ga_instance):
@@ -155,15 +154,15 @@
 on_generation()
 
 on_stop()
 ```
 
 # Example
 
-Check the [PyGAD's documentation](https://pygad.readthedocs.io/en/latest/README_pygad_ReadTheDocs.html) for information about the implementation of this example.
+Check the [PyGAD's documentation](https://pygad.readthedocs.io/en/latest/pygad.html) for information about the implementation of this example.
 
 ```python
 import pygad
 import numpy
 
 """
 Given the following function:
@@ -171,15 +170,15 @@
     where (x1,x2,x3,x4,x5,x6)=(4,-2,3.5,5,-11,-4.7) and y=44
 What are the best values for the 6 weights (w1 to w6)? We are going to use the genetic algorithm to optimize this function.
 """
 
 function_inputs = [4,-2,3.5,5,-11,-4.7] # Function inputs.
 desired_output = 44 # Function output.
 
-def fitness_func(solution, solution_idx):
+def fitness_func(ga_instance, solution, solution_idx):
     # Calculating the fitness value of each solution in the current population.
     # The fitness function calulates the sum of products between each input and its corresponding weight.
     output = numpy.sum(solution*function_inputs)
     fitness = 1.0 / numpy.abs(output - desired_output)
     return fitness
 
 fitness_function = fitness_func
```

### Comparing `pygad-3.0.1/README.md` & `pygad-3.1.0/pygad.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: pygad
+Version: 3.1.0
+Summary: PyGAD: A Python Library for Building the Genetic Algorithm and Training Machine Learning Algoithms (Keras & PyTorch).
+Home-page: https://github.com/ahmedfgad/GeneticAlgorithmPython
+Author: Ahmed Fawzy Gad
+Author-email: ahmed.f.gad@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # PyGAD:  Genetic Algorithm in Python
 
 [PyGAD](https://pypi.org/project/pygad) is an open-source easy-to-use Python 3 library for building the genetic algorithm and optimizing machine learning algorithms. It supports Keras and PyTorch.
 
 Check documentation of the [PyGAD](https://pygad.readthedocs.io/en/latest).
 
 [![Downloads](https://pepy.tech/badge/pygad)](https://pepy.tech/project/pygad) ![Docs](https://readthedocs.org/projects/pygad/badge)
@@ -10,31 +22,29 @@
 
 [PyGAD](https://pypi.org/project/pygad) supports different types of crossover, mutation, and parent selection. [PyGAD](https://pypi.org/project/pygad) allows different types of problems to be optimized using the genetic algorithm by customizing the fitness function. 
 
 The library is under active development and more features are added regularly. If you want a feature to be supported, please check the **Contact Us** section to send a request.
 
 # Donation
 
-- [Credit/Debit Card](https://donate.stripe.com/eVa5kO866elKgM0144): https://donate.stripe.com/eVa5kO866elKgM0144
-- [Open Collective](https://opencollective.com/pygad): [opencollective.com/pygad](https://opencollective.com/pygad)
-- PayPal: Use either this link: [paypal.me/ahmedfgad](https://paypal.me/ahmedfgad) or the e-mail address ahmed.f.gad@gmail.com
-- Interac e-Transfer: Use e-mail address ahmed.f.gad@gmail.com
+* [Credit/Debit Card](https://donate.stripe.com/eVa5kO866elKgM0144): https://donate.stripe.com/eVa5kO866elKgM0144
+* [Open Collective](https://opencollective.com/pygad): [opencollective.com/pygad](https://opencollective.com/pygad)
+* PayPal: Use either this link: [paypal.me/ahmedfgad](https://paypal.me/ahmedfgad) or the e-mail address ahmed.f.gad@gmail.com
+* Interac e-Transfer: Use e-mail address ahmed.f.gad@gmail.com
 
 # Installation
 
-To install [PyGAD](https://pypi.org/project/pygad), simply use pip to download and install the library from [PyPI](https://pypi.org/project/pygad) (Python Package Index). The library lives a PyPI at this page https://pypi.org/project/pygad.
+To install [PyGAD](https://pypi.org/project/pygad), simply use pip to download and install the library from [PyPI](https://pypi.org/project/pygad) (Python Package Index). The library is at PyPI at this page https://pypi.org/project/pygad.
 
 Install PyGAD with the following command:
 
 ```python
 pip install pygad
 ```
 
-PyGAD is developed in Python 3.7.3 and depends on NumPy for creating and manipulating arrays and Matplotlib for creating figures. The exact NumPy version used in developing PyGAD is 1.16.4. For Matplotlib, the version is 3.1.0.
-
 To get started with PyGAD, please read the documentation at [Read The Docs](https://pygad.readthedocs.io/) https://pygad.readthedocs.io.
 
 # PyGAD Source Code
 
 The source code of the PyGAD' modules is found in the following GitHub projects:
 
 - [pygad](https://github.com/ahmedfgad/GeneticAlgorithmPython): (https://github.com/ahmedfgad/GeneticAlgorithmPython)
@@ -72,15 +82,15 @@
 ```python
 import pygad
 import numpy
 
 function_inputs = [4,-2,3.5,5,-11,-4.7]
 desired_output = 44
 
-def fitness_func(solution, solution_idx):
+def fitness_func(ga_instance, solution, solution_idx):
     output = numpy.sum(solution*function_inputs)
     fitness = 1.0 / (numpy.abs(output - desired_output) + 0.000001)
     return fitness
 
 fitness_function = fitness_func
 
 def on_start(ga_instance):
@@ -144,15 +154,15 @@
 on_generation()
 
 on_stop()
 ```
 
 # Example
 
-Check the [PyGAD's documentation](https://pygad.readthedocs.io/en/latest/README_pygad_ReadTheDocs.html) for information about the implementation of this example.
+Check the [PyGAD's documentation](https://pygad.readthedocs.io/en/latest/pygad.html) for information about the implementation of this example.
 
 ```python
 import pygad
 import numpy
 
 """
 Given the following function:
@@ -160,15 +170,15 @@
     where (x1,x2,x3,x4,x5,x6)=(4,-2,3.5,5,-11,-4.7) and y=44
 What are the best values for the 6 weights (w1 to w6)? We are going to use the genetic algorithm to optimize this function.
 """
 
 function_inputs = [4,-2,3.5,5,-11,-4.7] # Function inputs.
 desired_output = 44 # Function output.
 
-def fitness_func(solution, solution_idx):
+def fitness_func(ga_instance, solution, solution_idx):
     # Calculating the fitness value of each solution in the current population.
     # The fitness function calulates the sum of products between each input and its corresponding weight.
     output = numpy.sum(solution*function_inputs)
     fitness = 1.0 / numpy.abs(output - desired_output)
     return fitness
 
 fitness_function = fitness_func
@@ -327,7 +337,9 @@
 
 * E-mail: ahmed.f.gad@gmail.com
 * [LinkedIn](https://www.linkedin.com/in/ahmedfgad)
 * [Paperspace](https://blog.paperspace.com/author/ahmed)
 * [KDnuggets](https://kdnuggets.com/author/ahmed-gad)
 * [TowardsDataScience](https://towardsdatascience.com/@ahmedfgad)
 * [GitHub](https://github.com/ahmedfgad)
+
+
```

### Comparing `pygad-3.0.1/pygad/cnn/cnn.py` & `pygad-3.1.0/pygad/cnn/cnn.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy
 import functools
+import logging
 
 """
 Convolutional neural network implementation using NumPy
 A tutorial that helps to get started (Building Convolutional Neural Network using NumPy from Scratch) available in these links: 
     https://www.linkedin.com/pulse/building-convolutional-neural-network-using-numpy-from-ahmed-gad
     https://towardsdatascience.com/building-convolutional-neural-network-using-numpy-from-scratch-b30aac50e50a
     https://www.kdnuggets.com/2018/04/building-convolutional-neural-network-numpy-scratch.html
@@ -80,22 +81,26 @@
         if type(layer) in [Conv2D, Dense]:
             # If the 'initial' parameter is True, append the initial weights. Otherwise, append the trained weights.
             if initial == True:
                 network_weights.append(layer.initial_weights)
             elif initial == False:
                 network_weights.append(layer.trained_weights)
             else:
-                raise ValueError("Unexpected value to the 'initial' parameter: {initial}.".format(initial=initial))
+                msg = f"Unexpected value to the 'initial' parameter: {initial}."
+                model.logger.error(msg)
+                raise ValueError(msg)
 
         # Go to the previous layer.
         layer = layer.previous_layer
 
     # If the first layer in the network is not an input layer (i.e. an instance of the Input2D class), raise an error.
     if not (type(layer) is Input2D):
-        raise TypeError("The first layer in the network architecture must be an input layer.")
+        msg = "The first layer in the network architecture must be an input layer."
+        model.logger.error(msg)
+        raise TypeError(msg)
 
     # Currently, the weights of the layers are in the reverse order. In other words, the weights of the first layer are at the last index of the 'network_weights' list while the weights of the last layer are at the first index.
     # Reversing the 'network_weights' list to order the layers' weights according to their location in the network architecture (i.e. the weights of the first layer appears at index 0 of the list).
     network_weights.reverse()
     return numpy.array(network_weights)
 
 def layers_weights_as_matrix(model, vector_weights):
@@ -127,15 +132,17 @@
             start = start + layer_weights_size
     
         # Go to the previous layer.
         layer = layer.previous_layer
 
     # If the first layer in the network is not an input layer (i.e. an instance of the Input2D class), raise an error.
     if not (type(layer) is Input2D):
-        raise TypeError("The first layer in the network architecture must be an input layer.")
+        msg = "The first layer in the network architecture must be an input layer."
+        model.logger.error(msg)
+        raise TypeError(msg)
 
     # Currently, the weights of the layers are in the reverse order. In other words, the weights of the first layer are at the last index of the 'network_weights' list while the weights of the last layer are at the first index.
     # Reversing the 'network_weights' list to order the layers' weights according to their location in the network architecture (i.e. the weights of the first layer appears at index 0 of the list).
     network_weights.reverse()
     return numpy.array(network_weights)
 
 def layers_weights_as_vector(model, initial=True):
@@ -160,22 +167,26 @@
     #            vector = pygad.nn.DenseLayer.to_vector(matrix=layer.initial_weights)
                 network_weights.extend(vector)
             elif initial == False:
                 vector = numpy.reshape(layer.trained_weights, newshape=(layer.trained_weights.size))
     #            vector = pygad.nn.DenseLayer.to_vector(array=layer.trained_weights)
                 network_weights.extend(vector)
             else:
-                raise ValueError("Unexpected value to the 'initial' parameter: {initial}.".format(initial=initial))
+                msg = f"Unexpected value to the 'initial' parameter: {initial}."
+                model.logger.error(msg)
+                raise ValueError(msg)
 
         # Go to the previous layer.
         layer = layer.previous_layer
 
     # If the first layer in the network is not an input layer (i.e. an instance of the Input2D class), raise an error.
     if not (type(layer) is Input2D):
-        raise TypeError("The first layer in the network architecture must be an input layer.")
+        msg = "The first layer in the network architecture must be an input layer."
+        model.logger.error(msg)
+        raise TypeError(msg)
 
     # Currently, the weights of the layers are in the reverse order. In other words, the weights of the first layer are at the last index of the 'network_weights' list while the weights of the last layer are at the first index.
     # Reversing the 'network_weights' list to order the layers' weights according to their location in the network architecture (i.e. the weights of the first layer appears at index 0 of the list).
     network_weights.reverse()
     return numpy.array(network_weights)
 
 def update_layers_trained_weights(model, final_weights):
@@ -195,83 +206,152 @@
             layer.trained_weights = final_weights[layer_idx]
     
             layer_idx = layer_idx - 1
 
         # Go to the previous layer.
         layer = layer.previous_layer
 
-class Input2D:
+
+class CustomLogger:
+
+    def __init__(self):
+        # Create a logger named with the module name.
+        logger = logging.getLogger(__name__)
+        # Set the logger log level to 'DEBUG' to log all kinds of messages.
+        logger.setLevel(logging.DEBUG)
+
+        # Clear any attached handlers to the logger from the previous runs.
+        # If the handlers are not cleared, then the new handler will be appended to the list of handlers.
+        # This makes the single log message be repeated according to the length of the list of handlers.
+        logger.handlers.clear()
+
+        # Create the handlers.
+        stream_handler = logging.StreamHandler()
+        # Set the handler log level to 'DEBUG' to log all kinds of messages received from the logger.
+        stream_handler.setLevel(logging.DEBUG)
+
+        # Create the formatter that just includes the log message.
+        formatter = logging.Formatter('%(message)s')
+
+        # Add the formatter to the handler.
+        stream_handler.setFormatter(formatter)
+
+        # Add the handler to the logger.
+        logger.addHandler(stream_handler)
+
+        # Create the 'self.logger' attribute to hold the logger.
+        # Instead of using 'print()', use 'self.logger.info()'
+        self.logger = logger
+
+class Input2D(CustomLogger):
 
     """
     Implementing the input layer of a CNN.
     The CNN architecture must start with an input layer.
     """
 
-    def __init__(self, input_shape):
+    def __init__(self, 
+                 input_shape,
+                 logger=None):
 
         """
         input_shape: Shape of the input sample to the CNN.
         """
 
+        super().__init__()
+
+        # If logger is None, then the CustomLogger.logger is created.
+        if logger is None:
+            pass
+        else:
+            self.logger = logger
+
         # If the input sample has less than 2 dimensions, then an exception is raised.
         if len(input_shape) < 2:
-            raise ValueError("The Input2D class creates an input layer for data inputs with at least 2 dimensions but ({num_dim}) dimensions found.".format(num_dim=len(input_shape)))
+            msg = f"The Input2D class creates an input layer for data inputs with at least 2 dimensions but ({len(input_shape)}) dimensions found."
+            self.logger.error(msg)
+            raise ValueError(msg)
         # If the input sample has exactly 2 dimensions, the third dimension is set to 1.
         elif len(input_shape) == 2:
             input_shape = (input_shape[0], input_shape[1], 1)
 
         for dim_idx, dim in enumerate(input_shape):
             if dim <= 0:
-                raise ValueError("The dimension size of the inputs cannot be <= 0. Please pass a valid value to the 'input_size' parameter.")
+                msg = "The dimension size of the inputs cannot be <= 0. Please pass a valid value to the 'input_size' parameter."
+                self.logger.error(msg)
+                raise ValueError(msg)
 
         self.input_shape = input_shape # Shape of the input sample.
         self.layer_output_size = input_shape # Shape of the output from the current layer. For an input layer, it is the same as the shape of the input sample.
 
-class Conv2D:
+class Conv2D(CustomLogger):
 
     """
     Implementing the convolution layer.
     """
 
-    def __init__(self, num_filters, kernel_size, previous_layer, activation_function=None):
+    def __init__(self, 
+                 num_filters, 
+                 kernel_size, 
+                 previous_layer, 
+                 activation_function=None,
+                 logger=None):
 
         """
         num_filters: Number of filters in the convolution layer.
         kernel_size: Kernel size of the filter.
         previous_layer: A reference to the previous layer.
         activation_function=None: The name of the activation function to be used in the conv layer. If None, then no activation function is applied besides the convolution operation. The activation function can be applied by a separate layer.
         """
 
+        super().__init__()
+
+        # If logger is None, then the CustomLogger.logger is created.
+        if logger is None:
+            pass
+        else:
+            self.logger = logger
+
         if num_filters <= 0:
-            raise ValueError("Number of filters cannot be <= 0. Please pass a valid value to the 'num_filters' parameter.")
+            msg = "Number of filters cannot be <= 0. Please pass a valid value to the 'num_filters' parameter."
+            self.logger.error(msg)
+            raise ValueError(msg)
         # Number of filters in the conv layer.
         self.num_filters = num_filters
 
         if kernel_size <= 0:
-            raise ValueError("The kernel size cannot be <= 0. Please pass a valid value to the 'kernel_size' parameter.")
+            msg = "The kernel size cannot be <= 0. Please pass a valid value to the 'kernel_size' parameter."
+            self.logger.error(msg)
+            raise ValueError(msg)
         # Kernel size of each filter.
         self.kernel_size = kernel_size
 
         # Validating the activation function
         if (activation_function is None):
             self.activation = None
         elif (activation_function == "relu"):
             self.activation = relu
         elif (activation_function == "sigmoid"):
             self.activation = sigmoid
         elif (activation_function == "softmax"):
-            raise ValueError("The softmax activation function cannot be used in a conv layer.")
+            msg = "The softmax activation function cannot be used in a conv layer."
+            self.logger.error(msg)
+            raise ValueError(msg)
         else:
-            raise ValueError("The specified activation function '{activation_function}' is not among the supported activation functions {supported_activation_functions}. Please use one of the supported functions.".format(activation_function=activation_function, supported_activation_functions=supported_activation_functions))
+            msg = f"The specified activation function '{activation_function}' is not among the supported activation functions {supported_activation_functions}. Please use one of the supported functions."
+            self.logger.error(msg)
+            raise ValueError(msg)
 
         # The activation function used in the current layer.
         self.activation_function = activation_function
 
         if previous_layer is None:
-            raise TypeError("The previous layer cannot be of Type 'None'. Please pass a valid layer to the 'previous_layer' parameter.")
+            msg = "The previous layer cannot be of Type 'None'. Please pass a valid layer to the 'previous_layer' parameter."
+            self.logger.error(msg)
+            raise TypeError(msg)
         # A reference to the layer that preceeds the current layer in the network architecture.
         self.previous_layer = previous_layer
         
         # A reference to the bank of filters.
         self.filter_bank_size = (self.num_filters,
                                  self.kernel_size, 
                                  self.kernel_size, 
@@ -349,52 +429,80 @@
         
         input2D: The input to be convolved by the filter bank.
 
         The conv() method saves the result of convolving the input by the filter bank in the layer_output attribute.
         """
 
         if len(input2D.shape) != len(self.initial_weights.shape) - 1: # Check if there is a match in the number of dimensions between the image and the filters.
-            raise ValueError("Number of dimensions in the conv filter and the input do not match.")  
+            msg = "Number of dimensions in the conv filter and the input do not match."
+            self.logger.error(msg)
+            raise ValueError(msg)
         if len(input2D.shape) > 2 or len(self.initial_weights.shape) > 3: # Check if number of image channels matches the filter depth.
             if input2D.shape[-1] != self.initial_weights.shape[-1]:
-                raise ValueError("Number of channels in both the input and the filter must match.")
+                msg = "Number of channels in both the input and the filter must match."
+                self.logger.error(msg)
+                raise ValueError(msg)
         if self.initial_weights.shape[1] != self.initial_weights.shape[2]: # Check if filter dimensions are equal.
-            raise ValueError('A filter must be a square matrix. I.e. number of rows and columns must match.')
+            msg = 'A filter must be a square matrix. I.e. number of rows and columns must match.'
+            self.logger.error(msg)
+            raise ValueError(msg)
         if self.initial_weights.shape[1]%2==0: # Check if filter diemnsions are odd.
-            raise ValueError('A filter must have an odd size. I.e. number of rows and columns must be odd.')
+            msg = 'A filter must have an odd size. I.e. number of rows and columns must be odd.'
+            self.logger.error(msg)
+            raise ValueError(msg)
 
         self.layer_output = self.conv_(input2D, self.trained_weights)
 
-class AveragePooling2D:
+class AveragePooling2D(CustomLogger):
 
     """
     Implementing the average pooling layer.
     """
 
-    def __init__(self, pool_size, previous_layer, stride=2):
+    def __init__(self, 
+                 pool_size, 
+                 previous_layer, 
+                 stride=2,
+                 logger=None):
 
         """
         pool_size: Pool size.
         previous_layer: Reference to the previous layer in the CNN architecture.
         stride=2: Stride
         """
 
+        super().__init__()
+
+        # If logger is None, then the CustomLogger.logger is created.
+        if logger is None:
+            pass
+        else:
+            self.logger = logger
+
         if not (type(pool_size) is int):
-            raise ValueError("The expected type of the pool_size is int but {pool_size_type} found.".format(pool_size_type=type(pool_size)))
+            msg = "The expected type of the pool_size is int but {pool_size_type} found.".format(pool_size_type=type(pool_size))
+            self.logger.error(msg)
+            raise ValueError(msg)
 
         if pool_size <= 0:
-            raise ValueError("The passed value to the pool_size parameter cannot be <= 0.")
+            msg = "The passed value to the pool_size parameter cannot be <= 0."
+            self.logger.error(msg)
+            raise ValueError(msg)
         self.pool_size = pool_size
 
         if stride <= 0:
-            raise ValueError("The passed value to the stride parameter cannot be <= 0.")
+            msg = "The passed value to the stride parameter cannot be <= 0."
+            self.logger.error(msg)
+            raise ValueError(msg)
         self.stride = stride
 
         if previous_layer is None:
-            raise TypeError("The previous layer cannot be of Type 'None'. Please pass a valid layer to the 'previous_layer' parameter.")
+            msg = "The previous layer cannot be of Type 'None'. Please pass a valid layer to the 'previous_layer' parameter."
+            self.logger.error(msg)
+            raise TypeError(msg)
         # A reference to the layer that preceeds the current layer in the network architecture.
         self.previous_layer = previous_layer
 
         # Size of the input to the layer.
         self.layer_input_size = self.previous_layer.layer_output_size
 
         # Size of the output from the layer.
@@ -426,41 +534,61 @@
                 for c in numpy.arange(0, input2D.shape[1]-self.pool_size+1, self.stride):
                     pool_out[r2, c2, map_num] = numpy.mean([input2D[r:r+self.pool_size,  c:c+self.pool_size, map_num]])
                     c2 = c2 + 1
                 r2 = r2 +1
 
         self.layer_output = pool_out
 
-class MaxPooling2D:
+class MaxPooling2D(CustomLogger):
 
     """
     Similar to the AveragePooling2D class except that it implements max pooling.
     """
 
-    def __init__(self, pool_size, previous_layer, stride=2):
+    def __init__(self, 
+                 pool_size, 
+                 previous_layer, 
+                 stride=2,
+                 logger=None):
         
         """
         pool_size: Pool size.
         previous_layer: Reference to the previous layer in the CNN architecture.
         stride=2: Stride
         """
-        
+
+        super().__init__()
+
+        # If logger is None, then the CustomLogger.logger is created.
+        if logger is None:
+            pass
+        else:
+            self.logger = logger
+
         if not (type(pool_size) is int):
-            raise ValueError("The expected type of the pool_size is int but {pool_size_type} found.".format(pool_size_type=type(pool_size)))
+            msg = f"The expected type of the pool_size is int but {type(pool_size)} found."
+            self.logger.error(msg)
+            raise ValueError(msg)
 
         if pool_size <= 0:
-            raise ValueError("The passed value to the pool_size parameter cannot be <= 0.")
+            msg = "The passed value to the pool_size parameter cannot be <= 0."
+            self.logger.error(msg)
+            raise ValueError(msg)
         self.pool_size = pool_size
 
         if stride <= 0:
-            raise ValueError("The passed value to the stride parameter cannot be <= 0.")
+            msg = "The passed value to the stride parameter cannot be <= 0."
+            self.logger.error(msg)
+            raise ValueError(msg)
         self.stride = stride
 
         if previous_layer is None:
-            raise TypeError("The previous layer cannot be of Type 'None'. Please pass a valid layer to the 'previous_layer' parameter.")
+            msg = "The previous layer cannot be of Type 'None'. Please pass a valid layer to the 'previous_layer' parameter."
+            self.logger.error(msg)
+            raise TypeError(msg)
         # A reference to the layer that preceeds the current layer in the network architecture.
         self.previous_layer = previous_layer
 
         # Size of the input to the layer.
         self.layer_input_size = self.previous_layer.layer_output_size
 
         # Size of the output from the layer.
@@ -492,28 +620,40 @@
                 for c in numpy.arange(0, input2D.shape[1]-self.pool_size+1, self.stride):
                     pool_out[r2, c2, map_num] = numpy.max([input2D[r:r+self.pool_size,  c:c+self.pool_size, map_num]])
                     c2 = c2 + 1
                 r2 = r2 +1
 
         self.layer_output = pool_out
 
-class ReLU:
+class ReLU(CustomLogger):
 
     """
     Implementing the ReLU layer.
     """
 
-    def __init__(self, previous_layer):
+    def __init__(self, 
+                 previous_layer,
+                 logger=None):
 
         """
         previous_layer: Reference to the previous layer.
         """
 
+        super().__init__()
+
+        # If logger is None, then the CustomLogger.logger is created.
+        if logger is None:
+            pass
+        else:
+            self.logger = logger
+
         if previous_layer is None:
-            raise TypeError("The previous layer cannot be of Type 'None'. Please pass a valid layer to the 'previous_layer' parameter.")
+            msg = "The previous layer cannot be of Type 'None'. Please pass a valid layer to the 'previous_layer' parameter."
+            self.logger.error(msg)
+            raise TypeError(msg)
 
         # A reference to the layer that preceeds the current layer in the network architecture.
         self.previous_layer = previous_layer
 
         # Size of the input to the layer.
         self.layer_input_size = self.previous_layer.layer_output_size
 
@@ -532,28 +672,40 @@
 
         The relu_layer() method saves its result in the layer_output attribute.
         """
 
         self.layer_output_size = layer_input.size
         self.layer_output = relu(layer_input)
 
-class Sigmoid:
+class Sigmoid(CustomLogger):
 
     """
     Implementing the sigmoid layer.
     """
 
-    def __init__(self, previous_layer):
+    def __init__(self, 
+                 previous_layer,
+                 logger=None):
 
         """
         previous_layer: Reference to the previous layer.
         """
 
+        super().__init__()
+
+        # If logger is None, then the CustomLogger.logger is created.
+        if logger is None:
+            pass
+        else:
+            self.logger = logger
+
         if previous_layer is None:
-            raise TypeError("The previous layer cannot be of Type 'None'. Please pass a valid layer to the 'previous_layer' parameter.")
+            msg = "The previous layer cannot be of Type 'None'. Please pass a valid layer to the 'previous_layer' parameter."
+            self.logger.error(msg)
+            raise TypeError(msg)
         # A reference to the layer that preceeds the current layer in the network architecture.
         self.previous_layer = previous_layer
 
         # Size of the input to the layer.
         self.layer_input_size = self.previous_layer.layer_output_size
 
         # Size of the output from the layer.
@@ -571,28 +723,40 @@
 
         The sigmoid_layer() method saves its result in the layer_output attribute.
         """
 
         self.layer_output_size = layer_input.size
         self.layer_output = sigmoid(layer_input)
 
-class Flatten:
+class Flatten(CustomLogger):
 
     """
     Implementing the flatten layer.
     """
 
-    def __init__(self, previous_layer):
+    def __init__(self, 
+                 previous_layer,
+                 logger=None):
         
         """
         previous_layer: Reference to the previous layer.
         """
 
+        super().__init__()
+
+        # If logger is None, then the CustomLogger.logger is created.
+        if logger is None:
+            pass
+        else:
+            self.logger = logger
+
         if previous_layer is None:
-            raise TypeError("The previous layer cannot be of Type 'None'. Please pass a valid layer to the 'previous_layer' parameter.")
+            msg = "The previous layer cannot be of Type 'None'. Please pass a valid layer to the 'previous_layer' parameter."
+            self.logger.error(msg)
+            raise TypeError(msg)
         # A reference to the layer that preceeds the current layer in the network architecture.
         self.previous_layer = previous_layer
 
         # Size of the input to the layer.
         self.layer_input_size = self.previous_layer.layer_output_size
 
         # Size of the output from the layer.
@@ -610,53 +774,74 @@
 
         The flatten() method saves its result in the layer_output attribute.
         """
 
         self.layer_output_size = input2D.size
         self.layer_output = numpy.ravel(input2D)
 
-class Dense:
+class Dense(CustomLogger):
 
     """
     Implementing the input dense (fully connected) layer of a CNN.
     """
 
-    def __init__(self, num_neurons, previous_layer, activation_function="relu"):
+    def __init__(self, 
+                 num_neurons, 
+                 previous_layer, 
+                 activation_function="relu",
+                 logger=None):
 
         """
         num_neurons: Number of neurons in the dense layer.
         previous_layer: Reference to the previous layer.
         activation_function: Name of the activation function to be used in the current layer.
+        logger=None: Reference to the instance of the logging.Logger class.
         """
 
+        super().__init__()
+
+        # If logger is None, then the CustomLogger.logger is created.
+        if logger is None:
+            pass
+        else:
+            self.logger = logger
+
         if num_neurons <= 0:
-            raise ValueError("Number of neurons cannot be <= 0. Please pass a valid value to the 'num_neurons' parameter.")
+            msg = "Number of neurons cannot be <= 0. Please pass a valid value to the 'num_neurons' parameter."
+            self.logger.error(msg)
+            raise ValueError(msg)
 
         # Number of neurons in the dense layer.
         self.num_neurons = num_neurons
 
         # Validating the activation function
         if (activation_function == "relu"):
             self.activation = relu
         elif (activation_function == "sigmoid"):
             self.activation = sigmoid
         elif (activation_function == "softmax"):
             self.activation = softmax
         else:
-            raise ValueError("The specified activation function '{activation_function}' is not among the supported activation functions {supported_activation_functions}. Please use one of the supported functions.".format(activation_function=activation_function, supported_activation_functions=supported_activation_functions))
+            msg = f"The specified activation function '{activation_function}' is not among the supported activation functions {supported_activation_functions}. Please use one of the supported functions."
+            self.logger.error(msg)
+            raise ValueError(msg)
 
         self.activation_function = activation_function
 
         if previous_layer is None:
-            raise TypeError("The previous layer cannot be of Type 'None'. Please pass a valid layer to the 'previous_layer' parameter.")
+            msg = "The previous layer cannot be of Type 'None'. Please pass a valid layer to the 'previous_layer' parameter."
+            self.logger.error(msg)
+            raise TypeError(msg)
         # A reference to the layer that preceeds the current layer in the network architecture.
         self.previous_layer = previous_layer
-        
+
         if type(self.previous_layer.layer_output_size) in [list, tuple, numpy.ndarray] and len(self.previous_layer.layer_output_size) > 1:
-            raise ValueError("The input to the dense layer must be of type int but {sh} found.".format(sh=type(self.previous_layer.layer_output_size)))
+            msg = f"The input to the dense layer must be of type int but {type(self.previous_layer.layer_output_size)} found."
+            self.logger.error(msg)
+            raise ValueError(msg)
         # Initializing the weights of the layer.
         self.initial_weights = numpy.random.uniform(low=-0.1,
                                                     high=0.1,
                                                     size=(self.previous_layer.layer_output_size, self.num_neurons))
 
         # The trained weights of the layer. Only assigned a value after the network is trained (i.e. the train_network() function completes).
         # Just initialized to be equal to the initial weights
@@ -678,34 +863,49 @@
         
         layer_input: The input to the dense layer
 
         The dense_layer() method saves its result in the layer_output attribute.
         """
 
         if self.trained_weights is None:
-            raise TypeError("The weights of the dense layer cannot be of Type 'None'.")
+            msg = "The weights of the dense layer cannot be of Type 'None'."
+            self.logger.error(msg)
+            raise TypeError(msg)
 
         sop = numpy.matmul(layer_input, self.trained_weights)
 
         self.layer_output = self.activation(sop)
 
-class Model:
+class Model(CustomLogger):
 
     """
     Creating a CNN model.
     """
 
-    def __init__(self, last_layer, epochs=10, learning_rate=0.01):
+    def __init__(self, 
+                 last_layer, 
+                 epochs=10, 
+                 learning_rate=0.01,
+                 logger=None):
         
         """
         last_layer: A reference to the last layer in the CNN architecture.
         epochs=10: Number of epochs.
         learning_rate=0.01: Learning rate.
+        logger=None: Reference to the instance of the logging.Logger class.
         """
 
+        super().__init__()
+
+        # If logger is None, then the CustomLogger.logger is created.
+        if logger is None:
+            pass
+        else:
+            self.logger = logger
+
         self.last_layer = last_layer
         self.epochs = epochs
         self.learning_rate = learning_rate
 
         # The network_layers attribute is a list holding references to all CNN layers.
         self.network_layers = self.get_layers()
 
@@ -724,43 +924,49 @@
         while "previous_layer" in layer.__init__.__code__.co_varnames:
             network_layers.insert(0, layer)
             layer = layer.previous_layer
 
         return network_layers
 
     def train(self, train_inputs, train_outputs):
-        
+
         """
         Trains the CNN model.
         It is important to note that no learning algorithm is used for training the CNN. Just the learning rate is used for making some changes which is better than leaving the weights unchanged.
         
         train_inputs: Training data inputs.
         train_outputs: Training data outputs. 
         """
         
         if (train_inputs.ndim != 4):
-            raise ValueError("The training data input has {num_dims} but it must have 4 dimensions. The first dimension is the number of training samples, the second & third dimensions represent the width and height of the sample, and the fourth dimension represents the number of channels in the sample.".format(num_dims=train_inputs.ndim))    
+            msg = f"The training data input has {train_inputs.ndim} but it must have 4 dimensions. The first dimension is the number of training samples, the second & third dimensions represent the width and height of the sample, and the fourth dimension represents the number of channels in the sample."
+            self.logger.error(msg)
+            raise ValueError(msg)
 
         if (train_inputs.shape[0] != len(train_outputs)):
-            raise ValueError("Mismatch between the number of input samples and number of labels: {num_samples_inputs} != {num_samples_outputs}.".format(num_samples_inputs=train_inputs.shape[0], num_samples_outputs=len(train_outputs)))
+            msg = f"Mismatch between the number of input samples and number of labels: {train_inputs.shape[0]} != {len(train_outputs)}."
+            self.logger.error(msg)
+            raise ValueError(msg)
 
         network_predictions = []
         network_error = 0
     
         for epoch in range(self.epochs):
-            print("Epoch {epoch}".format(epoch=epoch))
+            self.logger.info(f"Epoch {epoch}")
             for sample_idx in range(train_inputs.shape[0]):
                 # print("Sample {sample_idx}".format(sample_idx=sample_idx))
                 self.feed_sample(train_inputs[sample_idx, :])
     
                 try:
                     predicted_label = numpy.where(numpy.max(self.last_layer.layer_output) == self.last_layer.layer_output)[0][0]
                 except IndexError:
-                    print(self.last_layer.layer_output)
-                    raise IndexError("Index out of range")
+                    self.logger.info(self.last_layer.layer_output)
+                    msg = "Index out of range"
+                    self.logger.error(msg)
+                    raise IndexError(msg)
                 network_predictions.append(predicted_label)
     
                 network_error = network_error + abs(predicted_label - train_outputs[sample_idx])
 
             self.update_weights(network_error)
 
     def feed_sample(self, sample):
@@ -792,16 +998,18 @@
             elif type(layer) is Sigmoid:
                 layer.sigmoid_layer(layer_input=last_layer_outputs)
             elif type(layer) is Flatten:
                 layer.flatten(input2D=last_layer_outputs)
             elif type(layer) is Input2D:
                 pass
             else:
-                print("Other")
-                raise TypeError("The layer of type {layer_type} is not supported yet.".format(layer_type=type(layer)))
+                # self.logger.info("Other")
+                msg = "The layer of type {type(layer)} is not supported."
+                self.logger.error(msg)
+                raise TypeError(msg)
 
             last_layer_outputs = layer.layer_output
         return self.network_layers[-1].layer_output
 
     def update_weights(self, network_error):
         
         """
@@ -824,26 +1032,28 @@
         
         data_inputs: The inputs to predict their label.
 
         Returns a list holding the samples predictions.
         """
 
         if (data_inputs.ndim != 4):
-            raise ValueError("The data input has {num_dims} but it must have 4 dimensions. The first dimension is the number of training samples, the second & third dimensions represent the width and height of the sample, and the fourth dimension represents the number of channels in the sample.".format(num_dims=data_inputs.ndim))
+            msg = "The data input has {data_inputs.ndim} but it must have 4 dimensions. The first dimension is the number of training samples, the second & third dimensions represent the width and height of the sample, and the fourth dimension represents the number of channels in the sample."
+            self.logger.error(msg)
+            raise ValueError(msg)
 
         predictions = []
         for sample in data_inputs:
             probs = self.feed_sample(sample=sample)
             predicted_label = numpy.where(numpy.max(probs) == probs)[0][0]
             predictions.append(predicted_label)
         return predictions
 
     def summary(self):
 
         """
         Prints a summary of the CNN architecture.
         """
 
-        print("\n----------Network Architecture----------")
+        self.logger.info("\n----------Network Architecture----------")
         for layer in self.network_layers:
-            print(type(layer))
-        print("----------------------------------------\n")
+            self.logger.info(type(layer))
+        self.logger.info("----------------------------------------\n")
```

### Comparing `pygad-3.0.1/pygad/gacnn/gacnn.py` & `pygad-3.1.0/pygad/gacnn/gacnn.py`

 * *Files identical despite different names*

### Comparing `pygad-3.0.1/pygad/gann/gann.py` & `pygad-3.1.0/pygad/gann/gann.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from ..nn import nn
+import warnings
 
 def validate_network_parameters(num_neurons_input, 
                                 num_neurons_output, 
                                 num_neurons_hidden_layers, 
                                 output_activation, 
                                 hidden_activations, 
                                 num_solutions=None):
@@ -22,40 +23,40 @@
     
     Returns a list holding the name(s) of the activation function(s) for the hidden layer(s). 
     """
 
     # Validating the number of solutions within the population.
     if not (num_solutions is None):
         if num_solutions < 2:
-            raise ValueError("num_solutions: The number of solutions within the population must be at least 2. The current value is {num_solutions}.".format(num_solutions=num_solutions))
-        
+            raise ValueError(f"num_solutions: The number of solutions within the population must be at least 2. The current value is {num_solutions}.")
+
     # Validating the number of neurons in the input layer.
     if num_neurons_input is int and num_neurons_input <= 0:
         raise ValueError("num_neurons_input: The number of neurons in the input layer must be > 0.")
     
     # Validating the number of neurons in the output layer.
     if num_neurons_output is int and num_neurons_output <= 0:
         raise ValueError("num_neurons_output: The number of neurons in the output layer must be > 0.")
-    
+
     # Validating the type of the 'num_neurons_hidden_layers' parameter which is expected to be list or tuple.
     if not (type(num_neurons_hidden_layers) in [list, tuple]):
-        raise TypeError("num_neurons_hidden_layers: A list or a tuple is expected but {hidden_layers_neurons_type} found.".format(hidden_layers_neurons_type=type(num_neurons_hidden_layers)))
-    
+        raise TypeError(f"num_neurons_hidden_layers: A list or a tuple is expected but {type(num_neurons_hidden_layers)} found.")
+
     # Frequently used error messages.
-    unexpected_output_activation_value = "Output activation function: The activation function of the output layer is passed as a string not {activation_type}."
+    unexpected_output_activation_value = f"Output activation function: The activation function of the output layer is passed as a string not {type(output_activation)}."
     unexpected_activation_value = "Activation function: The supported values for the activation function are {supported_activations} but an unexpected value is found:\n{activations}"
     unexpected_activation_type = "Activation Function: A list, tuple, or a string is expected but {activations_type} found."
     length_mismatch = "Hidden activation functions: When passing the activation function(s) as a list or a tuple, its length must match the length of the 'num_neurons_hidden_layers' parameter but a mismatch is found:\n{mismatched_lengths}"
 
     # A list of the names of the supported activation functions.
     supported_activations = ["sigmoid", "relu", "softmax", "None"]
 
     # Validating the output layer activation function.
     if not (type(output_activation) is str):
-        raise ValueError(unexpected_output_activation_value.format(activation_type=type(output_activation)))
+        raise ValueError(unexpected_output_activation_value)
     if not (output_activation in supported_activations): #activation_type
         raise ValueError(unexpected_activation_value.format(activations=output_activation, supported_activations=supported_activations))
     
     # Number of hidden layers.
     num_hidden_layers = len(num_neurons_hidden_layers)
     if num_hidden_layers > 1: # In case there are more than 1 hidden layer.
         if type(hidden_activations) in [list, tuple]:
@@ -77,17 +78,17 @@
             if not (hidden_activations in supported_activations):
                 raise ValueError(unexpected_activation_value.format(supported_activations=supported_activations, activations=hidden_activations))
             else:
                 hidden_activations = [hidden_activations]
         else:
             raise TypeError(unexpected_activation_type.format(activations_type=type(hidden_activations)))
     else: # In case there are no hidden layers (num_hidden_layers == 0)
-        print("WARNING: There are no hidden layers however a value is assigned to the parameter 'hidden_activations'. It will be reset to [].".format(hidden_activations=hidden_activations))
+        warnings.warn("WARNING: There are no hidden layers however a value is assigned to the parameter 'hidden_activations'. It will be reset to [].")
         hidden_activations = []
-    
+
     # If the value passed to the 'hidden_activations' parameter is actually a list, then its elements are checked to make sure the listed name(s) of the activation function(s) are supported.
     for act in hidden_activations:
         if not (act in supported_activations):
             raise ValueError(unexpected_activation_value.format(supported_activations=supported_activations, activations=act))
 
     return hidden_activations
```

### Comparing `pygad-3.0.1/pygad/helper/unique.py` & `pygad-3.1.0/pygad/helper/unique.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,638 +1,815 @@
-"""
-The pygad.helper.unique module has helper methods to solve duplicate genes and make sure every gene is unique.
-"""
-    
-import numpy
-import warnings
-import random
-import pygad
-
-class Unique:
-    def solve_duplicate_genes_randomly(self, 
-                                       solution, 
-                                       min_val, 
-                                       max_val, 
-                                       mutation_by_replacement, 
-                                       gene_type, 
-                                       num_trials=10):
-    
-            """
-            Solves the duplicates in a solution by randomly selecting new values for the duplicating genes.
-            
-            solution: A solution with duplicate values.
-            min_val: Minimum value of the range to sample a number randomly.
-            max_val: Maximum value of the range to sample a number randomly.
-            mutation_by_replacement: Identical to the self.mutation_by_replacement attribute.
-            gene_type: Exactly the same as the self.gene_type attribute.
-            num_trials: Maximum number of trials to change the gene value to solve the duplicates.
-    
-            Returns:
-                new_solution: Solution after trying to solve its duplicates. If no duplicates solved, then it is identical to the passed solution parameter.
-                not_unique_indices: Indices of the genes with duplicate values.
-                num_unsolved_duplicates: Number of unsolved duplicates.
-            """
-    
-            new_solution = solution.copy()
-    
-            _, unique_gene_indices = numpy.unique(solution, return_index=True)
-            not_unique_indices = set(range(len(solution))) - set(unique_gene_indices)
-    
-            num_unsolved_duplicates = 0
-            if len(not_unique_indices) > 0:
-                for duplicate_index in not_unique_indices:
-                    for trial_index in range(num_trials):
-                        if self.gene_type_single == True:
-                            if gene_type[0] in pygad.GA.supported_int_types:
-                                temp_val = self.unique_int_gene_from_range(solution=new_solution, 
-                                                                           gene_index=duplicate_index, 
-                                                                           min_val=min_val, 
-                                                                           max_val=max_val, 
-                                                                           mutation_by_replacement=mutation_by_replacement, 
-                                                                           gene_type=gene_type)
-                            else:
-                                temp_val = numpy.random.uniform(low=min_val,
-                                                                high=max_val,
-                                                                size=1)
-                                if mutation_by_replacement:
-                                    pass
-                                else:
-                                    temp_val = new_solution[duplicate_index] + temp_val
-                        else:
-                            if gene_type[duplicate_index] in pygad.GA.supported_int_types:
-                                temp_val = self.unique_int_gene_from_range(solution=new_solution, 
-                                                                           gene_index=duplicate_index, 
-                                                                           min_val=min_val, 
-                                                                           max_val=max_val, 
-                                                                           mutation_by_replacement=mutation_by_replacement, 
-                                                                           gene_type=gene_type)
-                            else:
-                                temp_val = numpy.random.uniform(low=min_val,
-                                                                high=max_val,
-                                                                size=1)
-                                if mutation_by_replacement:
-                                    pass
-                                else:
-                                    temp_val = new_solution[duplicate_index] + temp_val
-    
-                        if self.gene_type_single == True:
-                            if not gene_type[1] is None:
-                                temp_val = numpy.round(gene_type[0](temp_val),
-                                                       gene_type[1])
-                            else:
-                                temp_val = gene_type[0](temp_val)
-                        else:
-                            if not gene_type[duplicate_index][1] is None:
-                                temp_val = numpy.round(gene_type[duplicate_index][0](temp_val),
-                                                       gene_type[duplicate_index][1])
-                            else:
-                                temp_val = gene_type[duplicate_index][0](temp_val)
-    
-                        if temp_val in new_solution and trial_index == (num_trials - 1):
-                            num_unsolved_duplicates = num_unsolved_duplicates + 1
-                            if not self.suppress_warnings: warnings.warn("Failed to find a unique value for gene with index {gene_idx} whose value is {gene_value}. Consider adding more values in the gene space or use a wider range for initial population or random mutation.".format(gene_idx=duplicate_index, gene_value=solution[duplicate_index]))
-                        elif temp_val in new_solution:
-                            continue
-                        else:
-                            new_solution[duplicate_index] = temp_val
-                            break
-    
-                    # Update the list of duplicate indices after each iteration.
-                    _, unique_gene_indices = numpy.unique(new_solution, return_index=True)
-                    not_unique_indices = set(range(len(solution))) - set(unique_gene_indices)
-                    # self.logger.info("not_unique_indices INSIDE", not_unique_indices)
-    
-            return new_solution, not_unique_indices, num_unsolved_duplicates
-    
-    def solve_duplicate_genes_by_space(self, 
-                                       solution, 
-                                       gene_type, 
-                                       num_trials=10, 
-                                       build_initial_pop=False):
-    
-            """
-            Solves the duplicates in a solution by selecting values for the duplicating genes from the gene space.
-    
-            solution: A solution with duplicate values.
-            gene_type: Exactly the same as the self.gene_type attribute.
-            num_trials: Maximum number of trials to change the gene value to solve the duplicates.
-    
-            Returns:
-                new_solution: Solution after trying to solve its duplicates. If no duplicates solved, then it is identical to the passed solution parameter.
-                not_unique_indices: Indices of the genes with duplicate values.
-                num_unsolved_duplicates: Number of unsolved duplicates.
-            """
-            
-            new_solution = solution.copy()
-    
-            _, unique_gene_indices = numpy.unique(solution, return_index=True)
-            not_unique_indices = set(range(len(solution))) - set(unique_gene_indices)
-            # self.logger.info("not_unique_indices OUTSIDE", not_unique_indices)
-    
-            # First try to solve the duplicates.
-            # For a solution like [3 2 0 0], the indices of the 2 duplicating genes are 2 and 3.
-            # The next call to the find_unique_value() method tries to change the value of the gene with index 3 to solve the duplicate.
-            if len(not_unique_indices) > 0:
-                new_solution, not_unique_indices, num_unsolved_duplicates = self.unique_genes_by_space(new_solution=new_solution, 
-                                                                                                       gene_type=gene_type, 
-                                                                                                       not_unique_indices=not_unique_indices, 
-                                                                                                       num_trials=10,
-                                                                                                       build_initial_pop=build_initial_pop)
-            else:
-                return new_solution, not_unique_indices, len(not_unique_indices)
-    
-            # Do another try if there exist duplicate genes.
-            # If there are no possible values for the gene 3 with index 3 to solve the duplicate, try to change the value of the other gene with index 2.
-            if len(not_unique_indices) > 0:
-                not_unique_indices = set(numpy.where(new_solution == new_solution[list(not_unique_indices)[0]])[0]) - set([list(not_unique_indices)[0]])
-                new_solution, not_unique_indices, num_unsolved_duplicates = self.unique_genes_by_space(new_solution=new_solution, 
-                                                                                                       gene_type=gene_type, 
-                                                                                                       not_unique_indices=not_unique_indices, 
-                                                                                                       num_trials=10,
-                                                                                                       build_initial_pop=build_initial_pop)
-            else:
-                # If there exist duplicate genes, then changing either of the 2 duplicating genes (with indices 2 and 3) will not solve the problem.
-                # This problem can be solved by randomly changing one of the non-duplicating genes that may make a room for a unique value in one the 2 duplicating genes.
-                # For example, if gene_space=[[3, 0, 1], [4, 1, 2], [0, 2], [3, 2, 0]] and the solution is [3 2 0 0], then the values of the last 2 genes duplicate.
-                # There are no possible changes in the last 2 genes to solve the problem. But it could be solved by changing the second gene from 2 to 4.
-                # As a result, any of the last 2 genes can take the value 2 and solve the duplicates.
-                return new_solution, not_unique_indices, len(not_unique_indices)
-    
-            return new_solution, not_unique_indices, num_unsolved_duplicates
-    
-    def unique_int_gene_from_range(self, 
-                                   solution, 
-                                   gene_index, 
-                                   min_val, 
-                                   max_val, 
-                                   mutation_by_replacement, 
-                                   gene_type, 
-                                   step=None):
-    
-            """
-            Finds a unique integer value for the gene.
-    
-            solution: A solution with duplicate values.
-            gene_index: Index of the gene to find a unique value.
-            min_val: Minimum value of the range to sample a number randomly.
-            max_val: Maximum value of the range to sample a number randomly.
-            mutation_by_replacement: Identical to the self.mutation_by_replacement attribute.
-            gene_type: Exactly the same as the self.gene_type attribute.
-    
-            Returns:
-                selected_value: The new value of the gene. It may be identical to the original gene value in case there are no possible unique values for the gene.
-            """
-    
-            if self.gene_type_single == True:
-                if step is None:
-                    all_gene_values = numpy.arange(min_val, max_val, dtype=gene_type[0])
-                else:
-                    # For non-integer steps, the numpy.arange() function returns zeros id the dtype parameter is set to an integer data type. So, this returns zeros if step is non-integer and dtype is set to an int data type: numpy.arange(min_val, max_val, step, dtype=gene_type[0])
-                    # To solve this issue, the data type casting will not be handled inside numpy.arange(). The range is generated by numpy.arange() and then the data type is converted using the numpy.asarray() function.
-                    all_gene_values = numpy.asarray(numpy.arange(min_val, max_val, step), dtype=gene_type[0])
-            else:
-                if step is None:
-                    all_gene_values = numpy.arange(min_val, max_val, dtype=gene_type[gene_index][0])
-                else:
-                    all_gene_values = numpy.asarray(numpy.arange(min_val, max_val, step), dtype=gene_type[gene_index][0])
-    
-            if mutation_by_replacement:
-                pass
-            else:
-                all_gene_values = all_gene_values + solution[gene_index]
-    
-            if self.gene_type_single == True:
-                if not gene_type[1] is None:
-                    all_gene_values = numpy.round(gene_type[0](all_gene_values),
-                                                  gene_type[1])
-                else:
-                    if type(all_gene_values) is numpy.ndarray:
-                        all_gene_values = numpy.asarray(all_gene_values, dtype=gene_type[0])
-                    else:
-                        all_gene_values = gene_type[0](all_gene_values)
-            else:
-                if not gene_type[gene_index][1] is None:
-                    all_gene_values = numpy.round(gene_type[gene_index][0](all_gene_values),
-                                                  gene_type[gene_index][1])
-                else:
-                    all_gene_values = gene_type[gene_index][0](all_gene_values)
-    
-            values_to_select_from = list(set(all_gene_values) - set(solution))
-    
-            if len(values_to_select_from) == 0:
-                if not self.suppress_warnings: warnings.warn("You set 'allow_duplicate_genes=False' but there is no enough values to prevent duplicates.")
-                selected_value = solution[gene_index]
-            else:
-                selected_value = random.choice(values_to_select_from)
-    
-            #if self.gene_type_single == True:
-            #    selected_value = gene_type[0](selected_value)
-            #else:
-            #    selected_value = gene_type[gene_index][0](selected_value)
-    
-            return selected_value
-    
-    def unique_genes_by_space(self, 
-                              new_solution, 
-                              gene_type, 
-                              not_unique_indices, 
-                              num_trials=10, 
-                              build_initial_pop=False):
-    
-            """
-            Loops through all the duplicating genes to find unique values that from their gene spaces to solve the duplicates.
-            For each duplicating gene, a call to the unique_gene_by_space() function is made.
-    
-            new_solution: A solution with duplicate values.
-            gene_type: Exactly the same as the self.gene_type attribute.
-            not_unique_indices: Indices with duplicating values.
-            num_trials: Maximum number of trials to change the gene value to solve the duplicates.
-    
-            Returns:
-                new_solution: Solution after trying to solve all of its duplicates. If no duplicates solved, then it is identical to the passed solution parameter.
-                not_unique_indices: Indices of the genes with duplicate values.
-                num_unsolved_duplicates: Number of unsolved duplicates.
-            """
-    
-            num_unsolved_duplicates = 0
-            for duplicate_index in not_unique_indices:
-                for trial_index in range(num_trials):
-                    temp_val = self.unique_gene_by_space(solution=new_solution, 
-                                                         gene_idx=duplicate_index, 
-                                                         gene_type=gene_type,
-                                                         build_initial_pop=build_initial_pop)
-
-                    if temp_val in new_solution and trial_index == (num_trials - 1):
-                        # self.logger.info("temp_val, duplicate_index", temp_val, duplicate_index, new_solution)
-                        num_unsolved_duplicates = num_unsolved_duplicates + 1
-                        if not self.suppress_warnings: warnings.warn("Failed to find a unique value for gene with index {gene_idx} whose value is {gene_value}. Consider adding more values in the gene space or use a wider range for initial population or random mutation.".format(gene_idx=duplicate_index, gene_value=new_solution[duplicate_index]))
-                    elif temp_val in new_solution:
-                        continue
-                    else:
-                        new_solution[duplicate_index] = temp_val
-                        # self.logger.info("SOLVED", duplicate_index)
-                        break
-    
-            # Update the list of duplicate indices after each iteration.
-            _, unique_gene_indices = numpy.unique(new_solution, return_index=True)
-            not_unique_indices = set(range(len(new_solution))) - set(unique_gene_indices)
-            # self.logger.info("not_unique_indices INSIDE", not_unique_indices)        
-    
-            return new_solution, not_unique_indices, num_unsolved_duplicates
-    
-    def unique_gene_by_space(self, 
-                             solution, 
-                             gene_idx, 
-                             gene_type, 
-                             build_initial_pop=False):
-    
-            """
-            Returns a unique gene value for a single gene based on its value space to solve the duplicates.
-    
-            solution: A solution with duplicate values.
-            gene_idx: The index of the gene that duplicates its value with another gene.
-            gene_type: Exactly the same as the self.gene_type attribute.
-    
-            Returns:
-                A unique value, if exists, for the gene.
-            """
-    
-            if self.gene_space_nested:
-                # Returning the current gene space from the 'gene_space' attribute.
-                if type(self.gene_space[gene_idx]) in [numpy.ndarray, list]:
-                    curr_gene_space = self.gene_space[gene_idx].copy()
-                else:
-                    curr_gene_space = self.gene_space[gene_idx]
-    
-                # If the gene space has only a single value, use it as the new gene value.
-                if type(curr_gene_space) in pygad.GA.supported_int_float_types:
-                    value_from_space = curr_gene_space
-                    # If the gene space is None, apply mutation by adding a random value between the range defined by the 2 parameters 'random_mutation_min_val' and 'random_mutation_max_val'.
-                elif curr_gene_space is None:
-                    if self.gene_type_single == True:
-                        if gene_type[0] in pygad.GA.supported_int_types:
-                            if build_initial_pop == True:
-                                value_from_space = self.unique_int_gene_from_range(solution=solution,
-                                                                                   gene_index=gene_idx,
-                                                                                   # min_val=self.random_mutation_min_val,
-                                                                                   # max_val=self.random_mutation_max_val,
-                                                                                   min_val=self.init_range_low,
-                                                                                   max_val=self.init_range_high,
-                                                                                   mutation_by_replacement=True, 
-                                                                                   gene_type=gene_type)
-                            else:
-                                value_from_space = self.unique_int_gene_from_range(solution=solution, 
-                                                                                   gene_index=gene_idx, 
-                                                                                   min_val=self.random_mutation_min_val, 
-                                                                                   max_val=self.random_mutation_max_val, 
-                                                                                   mutation_by_replacement=True,
-                                                                                   gene_type=gene_type)
-                        else:
-                            if build_initial_pop == True:
-                                value_from_space = numpy.random.uniform(# low=self.random_mutation_min_val,
-                                                                        # high=self.random_mutation_max_val,
-                                                                        low=self.init_range_low,
-                                                                        high=self.init_range_high,
-                                                                        size=1)
-                            else:
-                                value_from_space = numpy.random.uniform(low=self.random_mutation_min_val,
-                                                                        high=self.random_mutation_max_val,
-                                                                        size=1)
-                            if self.mutation_by_replacement:
-                                pass
-                            else:
-                                value_from_space = solution[gene_idx] + value_from_space
-                    else:
-                        if gene_type[gene_idx] in pygad.GA.supported_int_types:
-                            if build_initial_pop == True:
-                                value_from_space = self.unique_int_gene_from_range(solution=solution, 
-                                                                                   gene_index=gene_idx, 
-                                                                                   # min_val=self.random_mutation_min_val, 
-                                                                                   # max_val=self.random_mutation_max_val, 
-                                                                                   min_val=self.init_range_low,
-                                                                                   max_val=self.init_range_high,
-                                                                                   mutation_by_replacement=True, 
-                                                                                   gene_type=gene_type)
-                            else:
-                                value_from_space = self.unique_int_gene_from_range(solution=solution, 
-                                                                                   gene_index=gene_idx, 
-                                                                                   min_val=self.random_mutation_min_val, 
-                                                                                   max_val=self.random_mutation_max_val, 
-                                                                                   mutation_by_replacement=True,
-                                                                                   gene_type=gene_type)
-                        else:
-                            if build_initial_pop == True:
-                                value_from_space = numpy.random.uniform(# low=self.random_mutation_min_val,
-                                                                        # high=self.random_mutation_max_val,
-                                                                        low=self.init_range_low,
-                                                                        high=self.init_range_high,
-                                                                        size=1)
-                            else:
-                                value_from_space = numpy.random.uniform(low=self.random_mutation_min_val,
-                                                                        high=self.random_mutation_max_val,
-                                                                        size=1)
-                            if self.mutation_by_replacement:
-                                pass
-                            else:
-                                value_from_space = solution[gene_idx] + value_from_space
-    
-                elif type(curr_gene_space) is dict:
-                    if self.gene_type_single == True:
-                        if gene_type[0] in pygad.GA.supported_int_types:
-                            if build_initial_pop == True:
-                                if 'step' in curr_gene_space.keys():
-                                    value_from_space = self.unique_int_gene_from_range(solution=solution, 
-                                                                                       gene_index=gene_idx, 
-                                                                                       min_val=curr_gene_space['low'], 
-                                                                                       max_val=curr_gene_space['high'], 
-                                                                                       step=curr_gene_space['step'],
-                                                                                       mutation_by_replacement=True, 
-                                                                                       gene_type=gene_type)
-                                else:
-                                    value_from_space = self.unique_int_gene_from_range(solution=solution, 
-                                                                                       gene_index=gene_idx, 
-                                                                                       min_val=curr_gene_space['low'], 
-                                                                                       max_val=curr_gene_space['high'], 
-                                                                                       step=None,
-                                                                                       mutation_by_replacement=True, 
-                                                                                       gene_type=gene_type)
-                            else:
-                                if 'step' in curr_gene_space.keys():
-                                    value_from_space = self.unique_int_gene_from_range(solution=solution, 
-                                                                                       gene_index=gene_idx, 
-                                                                                       min_val=curr_gene_space['low'], 
-                                                                                       max_val=curr_gene_space['high'], 
-                                                                                       step=curr_gene_space['step'],
-                                                                                       mutation_by_replacement=True, 
-                                                                                       gene_type=gene_type)
-                                else:
-                                    value_from_space = self.unique_int_gene_from_range(solution=solution, 
-                                                                                       gene_index=gene_idx, 
-                                                                                       min_val=curr_gene_space['low'], 
-                                                                                       max_val=curr_gene_space['high'], 
-                                                                                       step=None,
-                                                                                       mutation_by_replacement=True, 
-                                                                                       gene_type=gene_type)
-                        else:
-                            if 'step' in curr_gene_space.keys():
-                                value_from_space = numpy.random.choice(numpy.arange(start=curr_gene_space['low'],
-                                                                                    stop=curr_gene_space['high'],
-                                                                                    step=curr_gene_space['step']),
-                                                                       size=1)
-                            else:
-                                value_from_space = numpy.random.uniform(low=curr_gene_space['low'],
-                                                                        high=curr_gene_space['high'],
-                                                                        size=1)
-                            if self.mutation_by_replacement:
-                                pass
-                            else:
-                                value_from_space = solution[gene_idx] + value_from_space
-                    else:
-                        if gene_type[gene_idx] in pygad.GA.supported_int_types:
-                            if build_initial_pop == True:
-                                if 'step' in curr_gene_space.keys():
-                                    value_from_space = self.unique_int_gene_from_range(solution=solution, 
-                                                                                       gene_index=gene_idx, 
-                                                                                       min_val=curr_gene_space['low'], 
-                                                                                       max_val=curr_gene_space['high'], 
-                                                                                       step=curr_gene_space['step'],
-                                                                                       mutation_by_replacement=True, 
-                                                                                       gene_type=gene_type)
-                                else:
-                                    value_from_space = self.unique_int_gene_from_range(solution=solution, 
-                                                                                       gene_index=gene_idx, 
-                                                                                       min_val=curr_gene_space['low'], 
-                                                                                       max_val=curr_gene_space['high'], 
-                                                                                       step=None,
-                                                                                       mutation_by_replacement=True, 
-                                                                                       gene_type=gene_type)
-                            else:
-                                if 'step' in curr_gene_space.keys():
-                                    value_from_space = self.unique_int_gene_from_range(solution=solution, 
-                                                                                       gene_index=gene_idx, 
-                                                                                       min_val=curr_gene_space['low'], 
-                                                                                       max_val=curr_gene_space['high'], 
-                                                                                       step=curr_gene_space['step'],
-                                                                                       mutation_by_replacement=True, 
-                                                                                       gene_type=gene_type)
-                                else:
-                                    value_from_space = self.unique_int_gene_from_range(solution=solution, 
-                                                                                      gene_index=gene_idx, 
-                                                                                      min_val=curr_gene_space['low'], 
-                                                                                      max_val=curr_gene_space['high'], 
-                                                                                      step=None,
-                                                                                      mutation_by_replacement=True, 
-                                                                                      gene_type=gene_type)
-                        else:
-                            if 'step' in curr_gene_space.keys():
-                                value_from_space = numpy.random.choice(numpy.arange(start=curr_gene_space['low'],
-                                                                                    stop=curr_gene_space['high'],
-                                                                                    step=curr_gene_space['step']),
-                                                                       size=1)
-                            else:
-                                value_from_space = numpy.random.uniform(low=curr_gene_space['low'],
-                                                                        high=curr_gene_space['high'],
-                                                                        size=1)
-                            if self.mutation_by_replacement:
-                                pass
-                            else:
-                                value_from_space = solution[gene_idx] + value_from_space
-    
-                else:
-                    # Selecting a value randomly based on the current gene's space in the 'gene_space' attribute.
-                    # If the gene space has only 1 value, then select it. The old and new values of the gene are identical.
-                    if len(curr_gene_space) == 1:
-                        value_from_space = curr_gene_space[0]
-                        if not self.suppress_warnings: warnings.warn("You set 'allow_duplicate_genes=False' but the space of the gene with index {gene_idx} has only a single value. Thus, duplicates are possible.".format(gene_idx=gene_idx))
-                    # If the gene space has more than 1 value, then select a new one that is different from the current value.
-                    else:
-                        values_to_select_from = list(set(curr_gene_space) - set(solution))
-    
-                        if len(values_to_select_from) == 0:
-                            if not self.suppress_warnings: warnings.warn("You set 'allow_duplicate_genes=False' but the gene space does not have enough values to prevent duplicates.")
-                            value_from_space = solution[gene_idx]
-                        else:
-                            value_from_space = random.choice(values_to_select_from)
-            else:
-                # Selecting a value randomly from the global gene space in the 'gene_space' attribute.
-                if type(self.gene_space) is dict:
-                    if self.gene_type_single == True:
-                        if gene_type[0] in pygad.GA.supported_int_types:
-                            if build_initial_pop == True:
-                                if 'step' in self.gene_space.keys():
-                                    value_from_space = self.unique_int_gene_from_range(solution=solution, 
-                                                                                       gene_index=gene_idx, 
-                                                                                       min_val=self.gene_space['low'], 
-                                                                                       max_val=self.gene_space['high'], 
-                                                                                       step=self.gene_space['step'],
-                                                                                       mutation_by_replacement=True, 
-                                                                                       gene_type=gene_type)
-                                else:
-                                    value_from_space = self.unique_int_gene_from_range(solution=solution, 
-                                                                                       gene_index=gene_idx, 
-                                                                                       min_val=self.gene_space['low'], 
-                                                                                       max_val=self.gene_space['high'], 
-                                                                                       step=None,
-                                                                                       mutation_by_replacement=True, 
-                                                                                       gene_type=gene_type)
-                            else:
-                                if 'step' in self.gene_space.keys():
-                                    value_from_space = self.unique_int_gene_from_range(solution=solution, 
-                                                                                       gene_index=gene_idx, 
-                                                                                       min_val=self.gene_space['low'], 
-                                                                                       max_val=self.gene_space['high'], 
-                                                                                       step=self.gene_space['step'],
-                                                                                       mutation_by_replacement=True, 
-                                                                                       gene_type=gene_type)
-                                else:
-                                    value_from_space = self.unique_int_gene_from_range(solution=solution, 
-                                                                                       gene_index=gene_idx, 
-                                                                                       min_val=self.gene_space['low'], 
-                                                                                       max_val=self.gene_space['high'], 
-                                                                                       step=None,
-                                                                                       mutation_by_replacement=True, 
-                                                                                       gene_type=gene_type)
-                        else:
-                            # When the gene_space is assigned a dict object, then it specifies the lower and upper limits of all genes in the space.
-                            if 'step' in self.gene_space.keys():
-                                value_from_space = numpy.random.choice(numpy.arange(start=self.gene_space['low'],
-                                                                                    stop=self.gene_space['high'],
-                                                                                    step=self.gene_space['step']),
-                                                                       size=1)
-                            else:
-                                value_from_space = numpy.random.uniform(low=self.gene_space['low'],
-                                                                        high=self.gene_space['high'],
-                                                                        size=1)
-                            if self.mutation_by_replacement:
-                                pass
-                            else:
-                                value_from_space = solution[gene_idx] + value_from_space
-                    else:
-                        if gene_type[gene_idx] in pygad.GA.supported_int_types:
-                            if build_initial_pop == True:
-                                if 'step' in self.gene_space.keys():
-                                    value_from_space = self.unique_int_gene_from_range(solution=solution, 
-                                                                                       gene_index=gene_idx, 
-                                                                                       min_val=self.gene_space['low'], 
-                                                                                       max_val=self.gene_space['high'], 
-                                                                                       step=self.gene_space['step'],
-                                                                                       mutation_by_replacement=True, 
-                                                                                       gene_type=gene_type)
-                                else:
-                                    value_from_space = self.unique_int_gene_from_range(solution=solution, 
-                                                                                       gene_index=gene_idx, 
-                                                                                       min_val=self.gene_space['low'], 
-                                                                                       max_val=self.gene_space['high'], 
-                                                                                       step=None,
-                                                                                       mutation_by_replacement=True, 
-                                                                                       gene_type=gene_type)
-                            else:
-                                if 'step' in self.gene_space.keys():
-                                    value_from_space = self.unique_int_gene_from_range(solution=solution, 
-                                                                                       gene_index=gene_idx, 
-                                                                                       min_val=self.gene_space['low'], 
-                                                                                       max_val=self.gene_space['high'], 
-                                                                                       step=self.gene_space['step'],
-                                                                                       mutation_by_replacement=True, 
-                                                                                       gene_type=gene_type)
-                                else:
-                                    value_from_space = self.unique_int_gene_from_range(solution=solution, 
-                                                                                       gene_index=gene_idx, 
-                                                                                       min_val=self.gene_space['low'], 
-                                                                                       max_val=self.gene_space['high'], 
-                                                                                       step=None,
-                                                                                       mutation_by_replacement=True, 
-                                                                                       gene_type=gene_type)
-                        else:
-                            # When the gene_space is assigned a dict object, then it specifies the lower and upper limits of all genes in the space.
-                            if 'step' in self.gene_space.keys():
-                                value_from_space = numpy.random.choice(numpy.arange(start=self.gene_space['low'],
-                                                                                    stop=self.gene_space['high'],
-                                                                                    step=self.gene_space['step']),
-                                                                       size=1)
-                            else:
-                                value_from_space = numpy.random.uniform(low=self.gene_space['low'],
-                                                                        high=self.gene_space['high'],
-                                                                        size=1)
-                            if self.mutation_by_replacement:
-                                pass
-                            else:
-                                value_from_space = solution[gene_idx] + value_from_space
-    
-                else:
-                    # If the space type is not of type dict, then a value is randomly selected from the gene_space attribute.
-                    # Remove all the genes in the current solution from the gene_space.
-                    # This only leaves the unique values that could be selected for the gene.
-                    values_to_select_from = list(set(self.gene_space) - set(solution))
-    
-                    if len(values_to_select_from) == 0:
-                        if not self.suppress_warnings: warnings.warn("You set 'allow_duplicate_genes=False' but the gene space does not have enough values to prevent duplicates.")
-                        value_from_space = solution[gene_idx]
-                    else:
-                        value_from_space = random.choice(values_to_select_from)
-    
-            if value_from_space is None:
-                if build_initial_pop == True:
-                    value_from_space = numpy.random.uniform(# low=self.random_mutation_min_val,
-                                                            # high=self.random_mutation_max_val,
-                                                            low=self.init_range_low,
-                                                            high=self.init_range_high,
-                                                            size=1)
-                else:
-                    value_from_space = numpy.random.uniform(low=self.random_mutation_min_val,
-                                                            high=self.random_mutation_max_val,
-                                                            size=1)
-    
-            if self.gene_type_single == True:
-                if not gene_type[1] is None:
-                    value_from_space = numpy.round(gene_type[0](value_from_space),
-                                                   gene_type[1])
-                else:
-                    value_from_space = gene_type[0](value_from_space)
-            else:
-                if not gene_type[gene_idx][1] is None:
-                    value_from_space = numpy.round(gene_type[gene_idx][0](value_from_space),
-                                                  gene_type[gene_idx][1])
-                else:
-                    value_from_space = gene_type[gene_idx][0](value_from_space)
-    
-            return value_from_space
+"""
+The pygad.helper.unique module has helper methods to solve duplicate genes and make sure every gene is unique.
+"""
+
+import numpy
+import warnings
+import random
+import pygad
+
+class Unique:
+
+    def solve_duplicate_genes_randomly(self, 
+                                       solution, 
+                                       min_val, 
+                                       max_val, 
+                                       mutation_by_replacement, 
+                                       gene_type, 
+                                       num_trials=10):
+    
+            """
+            Solves the duplicates in a solution by randomly selecting new values for the duplicating genes.
+
+            solution: A solution with duplicate values.
+            min_val: Minimum value of the range to sample a number randomly.
+            max_val: Maximum value of the range to sample a number randomly.
+            mutation_by_replacement: Identical to the self.mutation_by_replacement attribute.
+            gene_type: Exactly the same as the self.gene_type attribute.
+            num_trials: Maximum number of trials to change the gene value to solve the duplicates.
+
+            Returns:
+                new_solution: Solution after trying to solve its duplicates. If no duplicates solved, then it is identical to the passed solution parameter.
+                not_unique_indices: Indices of the genes with duplicate values.
+                num_unsolved_duplicates: Number of unsolved duplicates.
+            """
+    
+            new_solution = solution.copy()
+    
+            _, unique_gene_indices = numpy.unique(solution, return_index=True)
+            not_unique_indices = set(range(len(solution))) - set(unique_gene_indices)
+    
+            num_unsolved_duplicates = 0
+            if len(not_unique_indices) > 0:
+                for duplicate_index in not_unique_indices:
+                    for trial_index in range(num_trials):
+                        if self.gene_type_single == True:
+                            if gene_type[0] in pygad.GA.supported_int_types:
+                                temp_val = self.unique_int_gene_from_range(solution=new_solution, 
+                                                                           gene_index=duplicate_index, 
+                                                                           min_val=min_val, 
+                                                                           max_val=max_val, 
+                                                                           mutation_by_replacement=mutation_by_replacement, 
+                                                                           gene_type=gene_type)
+                            else:
+                                temp_val = numpy.random.uniform(low=min_val,
+                                                                high=max_val,
+                                                                size=1)[0]
+                                if mutation_by_replacement:
+                                    pass
+                                else:
+                                    temp_val = new_solution[duplicate_index] + temp_val
+                        else:
+                            if gene_type[duplicate_index][0] in pygad.GA.supported_int_types:
+                                temp_val = self.unique_int_gene_from_range(solution=new_solution, 
+                                                                           gene_index=duplicate_index, 
+                                                                           min_val=min_val, 
+                                                                           max_val=max_val, 
+                                                                           mutation_by_replacement=mutation_by_replacement, 
+                                                                           gene_type=gene_type)
+                            else:
+                                temp_val = numpy.random.uniform(low=min_val,
+                                                                high=max_val,
+                                                                size=1)[0]
+                                if mutation_by_replacement:
+                                    pass
+                                else:
+                                    temp_val = new_solution[duplicate_index] + temp_val
+
+                        # Similar to the round_genes() method in the pygad module,
+                        # Create a round_gene() method to round a single gene.
+                        if self.gene_type_single == True:
+                            if not gene_type[1] is None:
+                                temp_val = numpy.round(gene_type[0](temp_val),
+                                                       gene_type[1])
+                            else:
+                                temp_val = gene_type[0](temp_val)
+                        else:
+                            if not gene_type[duplicate_index][1] is None:
+                                temp_val = numpy.round(gene_type[duplicate_index][0](temp_val),
+                                                       gene_type[duplicate_index][1])
+                            else:
+                                temp_val = gene_type[duplicate_index][0](temp_val)
+    
+                        if temp_val in new_solution and trial_index == (num_trials - 1):
+                            num_unsolved_duplicates = num_unsolved_duplicates + 1
+                            if not self.suppress_warnings: warnings.warn(f"Failed to find a unique value for gene with index {duplicate_index} whose value is {solution[duplicate_index]}. Consider adding more values in the gene space or use a wider range for initial population or random mutation.")
+                        elif temp_val in new_solution:
+                            continue
+                        else:
+                            new_solution[duplicate_index] = temp_val
+                            break
+    
+                    # Update the list of duplicate indices after each iteration.
+                    _, unique_gene_indices = numpy.unique(new_solution, return_index=True)
+                    not_unique_indices = set(range(len(solution))) - set(unique_gene_indices)
+                    # self.logger.info("not_unique_indices INSIDE", not_unique_indices)
+    
+            return new_solution, not_unique_indices, num_unsolved_duplicates
+
+    def solve_duplicate_genes_by_space(self, 
+                                       solution, 
+                                       gene_type, 
+                                       num_trials=10, 
+                                       build_initial_pop=False):
+    
+            """
+            Solves the duplicates in a solution by selecting values for the duplicating genes from the gene space.
+    
+            solution: A solution with duplicate values.
+            gene_type: Exactly the same as the self.gene_type attribute.
+            num_trials: Maximum number of trials to change the gene value to solve the duplicates.
+    
+            Returns:
+                new_solution: Solution after trying to solve its duplicates. If no duplicates solved, then it is identical to the passed solution parameter.
+                not_unique_indices: Indices of the genes with duplicate values.
+                num_unsolved_duplicates: Number of unsolved duplicates.
+            """
+            new_solution = solution.copy()
+
+            _, unique_gene_indices = numpy.unique(solution, return_index=True)
+            not_unique_indices = set(range(len(solution))) - set(unique_gene_indices)
+            # self.logger.info("not_unique_indices OUTSIDE", not_unique_indices)
+
+            # First try to solve the duplicates.
+            # For a solution like [3 2 0 0], the indices of the 2 duplicating genes are 2 and 3.
+            # The next call to the find_unique_value() method tries to change the value of the gene with index 3 to solve the duplicate.
+            if len(not_unique_indices) > 0:
+                new_solution, not_unique_indices, num_unsolved_duplicates = self.unique_genes_by_space(new_solution=new_solution, 
+                                                                                                       gene_type=gene_type, 
+                                                                                                       not_unique_indices=not_unique_indices, 
+                                                                                                       num_trials=10,
+                                                                                                       build_initial_pop=build_initial_pop)
+            else:
+                return new_solution, not_unique_indices, len(not_unique_indices)
+    
+            # Do another try if there exist duplicate genes.
+            # If there are no possible values for the gene 3 with index 3 to solve the duplicate, try to change the value of the other gene with index 2.
+            if len(not_unique_indices) > 0:
+                not_unique_indices = set(numpy.where(new_solution == new_solution[list(not_unique_indices)[0]])[0]) - set([list(not_unique_indices)[0]])
+                new_solution, not_unique_indices, num_unsolved_duplicates = self.unique_genes_by_space(new_solution=new_solution, 
+                                                                                                       gene_type=gene_type, 
+                                                                                                       not_unique_indices=not_unique_indices, 
+                                                                                                       num_trials=10,
+                                                                                                       build_initial_pop=build_initial_pop)
+            else:
+                # DEEP-DUPLICATE-REMOVAL-NEEDED
+                # Search by this phrase to find where deep duplicates removal should be applied.
+
+                # If there exist duplicate genes, then changing either of the 2 duplicating genes (with indices 2 and 3) will not solve the problem.
+                # This problem can be solved by randomly changing one of the non-duplicating genes that may make a room for a unique value in one the 2 duplicating genes.
+                # For example, if gene_space=[[3, 0, 1], [4, 1, 2], [0, 2], [3, 2, 0]] and the solution is [3 2 0 0], then the values of the last 2 genes duplicate.
+                # There are no possible changes in the last 2 genes to solve the problem. But it could be solved by changing the second gene from 2 to 4.
+                # As a result, any of the last 2 genes can take the value 2 and solve the duplicates.
+                return new_solution, not_unique_indices, len(not_unique_indices)
+
+            return new_solution, not_unique_indices, num_unsolved_duplicates
+    
+    def unique_int_gene_from_range(self, 
+                                   solution, 
+                                   gene_index, 
+                                   min_val, 
+                                   max_val, 
+                                   mutation_by_replacement, 
+                                   gene_type, 
+                                   step=None):
+
+            """
+            Finds a unique integer value for the gene.
+    
+            solution: A solution with duplicate values.
+            gene_index: Index of the gene to find a unique value.
+            min_val: Minimum value of the range to sample a number randomly.
+            max_val: Maximum value of the range to sample a number randomly.
+            mutation_by_replacement: Identical to the self.mutation_by_replacement attribute.
+            gene_type: Exactly the same as the self.gene_type attribute.
+    
+            Returns:
+                selected_value: The new value of the gene. It may be identical to the original gene value in case there are no possible unique values for the gene.
+            """
+
+            if self.gene_type_single == True:
+                if step is None:
+                    # all_gene_values = numpy.arange(min_val, 
+                    #                                max_val, 
+                    #                                dtype=gene_type[0])
+                    all_gene_values = numpy.asarray(numpy.arange(min_val, max_val), 
+                                                    dtype=gene_type[0])
+                else:
+                    # For non-integer steps, the numpy.arange() function returns zeros if the dtype parameter is set to an integer data type. So, this returns zeros if step is non-integer and dtype is set to an int data type: numpy.arange(min_val, max_val, step, dtype=gene_type[0])
+                    # To solve this issue, the data type casting will not be handled inside numpy.arange(). The range is generated by numpy.arange() and then the data type is converted using the numpy.asarray() function.
+                    all_gene_values = numpy.asarray(numpy.arange(min_val, 
+                                                                 max_val, 
+                                                                 step), 
+                                                    dtype=gene_type[0])
+            else:
+                if step is None:
+                    # all_gene_values = numpy.arange(min_val, 
+                    #                                max_val, 
+                    #                                dtype=gene_type[gene_index][0])
+                    all_gene_values = numpy.asarray(numpy.arange(min_val, 
+                                                                 max_val), 
+                                                    dtype=gene_type[gene_index][0])
+                else:
+                    all_gene_values = numpy.asarray(numpy.arange(min_val, 
+                                                                 max_val, 
+                                                                 step), 
+                                                    dtype=gene_type[gene_index][0])
+    
+            if mutation_by_replacement:
+                pass
+            else:
+                all_gene_values = all_gene_values + solution[gene_index]
+
+            # TODO: The gene data type is converted twine. One above and one here.
+            if self.gene_type_single == True:
+                # Note that we already know that the data type is integer.
+                all_gene_values = numpy.asarray(all_gene_values, 
+                                                dtype=gene_type[0])
+            else:
+                # Note that we already know that the data type is integer.
+                all_gene_values = numpy.asarray(all_gene_values, 
+                                                gene_type[gene_index][0])
+
+            values_to_select_from = list(set(list(all_gene_values)) - set(solution))
+    
+            if len(values_to_select_from) == 0:
+                # If there is no values, then keep the current gene value.
+                if not self.suppress_warnings: warnings.warn("You set 'allow_duplicate_genes=False' but there is no enough values to prevent duplicates.")
+                selected_value = solution[gene_index]
+            else:
+                selected_value = random.choice(values_to_select_from)
+    
+            return selected_value
+
+    def unique_genes_by_space(self, 
+                              new_solution, 
+                              gene_type, 
+                              not_unique_indices, 
+                              num_trials=10, 
+                              build_initial_pop=False):
+
+        """
+        Loops through all the duplicating genes to find unique values that from their gene spaces to solve the duplicates.
+        For each duplicating gene, a call to the unique_gene_by_space() function is made.
+    
+        new_solution: A solution with duplicate values.
+        gene_type: Exactly the same as the self.gene_type attribute.
+        not_unique_indices: Indices with duplicating values.
+        num_trials: Maximum number of trials to change the gene value to solve the duplicates.
+    
+        Returns:
+            new_solution: Solution after trying to solve all of its duplicates. If no duplicates solved, then it is identical to the passed solution parameter.
+            not_unique_indices: Indices of the genes with duplicate values.
+            num_unsolved_duplicates: Number of unsolved duplicates.
+        """
+
+        num_unsolved_duplicates = 0
+        for duplicate_index in not_unique_indices:
+            for trial_index in range(num_trials):
+                temp_val = self.unique_gene_by_space(solution=new_solution, 
+                                                     gene_idx=duplicate_index, 
+                                                     gene_type=gene_type,
+                                                     build_initial_pop=build_initial_pop)
+
+                if temp_val in new_solution and trial_index == (num_trials - 1):
+                    # self.logger.info("temp_val, duplicate_index", temp_val, duplicate_index, new_solution)
+                    num_unsolved_duplicates = num_unsolved_duplicates + 1
+                    if not self.suppress_warnings: warnings.warn(f"Failed to find a unique value for gene with index {duplicate_index} whose value is {new_solution[duplicate_index]}. Consider adding more values in the gene space or use a wider range for initial population or random mutation.")
+                elif temp_val in new_solution:
+                    continue
+                else:
+                    new_solution[duplicate_index] = temp_val
+                    # self.logger.info("SOLVED", duplicate_index)
+                    break
+    
+        # Update the list of duplicate indices after each iteration.
+        _, unique_gene_indices = numpy.unique(new_solution, return_index=True)
+        not_unique_indices = set(range(len(new_solution))) - set(unique_gene_indices)
+        # self.logger.info("not_unique_indices INSIDE", not_unique_indices)        
+
+        return new_solution, not_unique_indices, num_unsolved_duplicates
+
+    def unique_gene_by_space(self, 
+                             solution, 
+                             gene_idx, 
+                             gene_type, 
+                             build_initial_pop=False):
+    
+            """
+            Returns a unique gene value for a single gene based on its value space to solve the duplicates.
+    
+            solution: A solution with duplicate values.
+            gene_idx: The index of the gene that duplicates its value with another gene.
+            gene_type: Exactly the same as the self.gene_type attribute.
+    
+            Returns:
+                A unique value, if exists, for the gene.
+            """
+
+            if self.gene_space_nested:
+                if type(self.gene_space[gene_idx]) in [numpy.ndarray, list, tuple]:
+                    # Return the current gene space from the 'gene_space' attribute.
+                    curr_gene_space = list(self.gene_space[gene_idx]).copy()
+                else:
+                    # Return the entire gene space from the 'gene_space' attribute.
+                    # curr_gene_space = list(self.gene_space[gene_idx]).copy()
+                    curr_gene_space = self.gene_space[gene_idx]
+
+                # If the gene space has only a single value, use it as the new gene value.
+                if type(curr_gene_space) in pygad.GA.supported_int_float_types:
+                    value_from_space = curr_gene_space
+                    # If the gene space is None, apply mutation by adding a random value between the range defined by the 2 parameters 'random_mutation_min_val' and 'random_mutation_max_val'.
+                elif curr_gene_space is None:
+                    if self.gene_type_single == True:
+                        if gene_type[0] in pygad.GA.supported_int_types:
+                            if build_initial_pop == True:
+                                # If we are building the initial population, then use the range of the initial population.
+                                min_val = self.init_range_low
+                                max_val = self.init_range_high
+                            else:
+                                # If we are NOT building the initial population, then use the range of the random mutation.
+                                min_val = self.random_mutation_min_val
+                                max_val = self.random_mutation_max_val
+
+                            value_from_space = self.unique_int_gene_from_range(solution=solution, 
+                                                                               gene_index=gene_idx, 
+                                                                               min_val=min_val, 
+                                                                               max_val=max_val, 
+                                                                               mutation_by_replacement=True,
+                                                                               gene_type=gene_type)
+                        else:
+                            if build_initial_pop == True:
+                                low = self.init_range_low
+                                high = self.init_range_high
+                            else:
+                                low = self.random_mutation_min_val
+                                high = self.random_mutation_max_val
+
+                            value_from_space = numpy.random.uniform(low=low,
+                                                                    high=high,
+                                                                    size=1)[0]
+                            # TODO: Remove check for mutation_by_replacement when solving duplicates. Just replace the gene by the selected value from space.
+                            # if self.mutation_by_replacement:
+                            #     pass
+                            # else:
+                            #     value_from_space = solution[gene_idx] + value_from_space
+                    else:
+                        if gene_type[gene_idx][0] in pygad.GA.supported_int_types:
+                            if build_initial_pop == True:
+                                min_val = self.init_range_low
+                                max_val = self.init_range_high
+                            else:
+                                min_val = self.random_mutation_min_val
+                                max_val = self.random_mutation_max_val
+
+                            value_from_space = self.unique_int_gene_from_range(solution=solution, 
+                                                                               gene_index=gene_idx, 
+                                                                               min_val=min_val, 
+                                                                               max_val=max_val, 
+                                                                               mutation_by_replacement=True,
+                                                                               gene_type=gene_type)
+                        else:
+                            if build_initial_pop == True:
+                                low = self.init_range_low
+                                high = self.init_range_high
+                            else:
+                                low = self.random_mutation_min_val
+                                high = self.random_mutation_max_val
+
+                            value_from_space = numpy.random.uniform(low=low,
+                                                                    high=high,
+                                                                    size=1)[0]
+                            # TODO: Remove check for mutation_by_replacement when solving duplicates. Just replace the gene by the selected value from space.
+                            # if self.mutation_by_replacement:
+                            #     pass
+                            # else:
+                            #     value_from_space = solution[gene_idx] + value_from_space
+    
+                elif type(curr_gene_space) is dict:
+                    if self.gene_type_single == True:
+                        if gene_type[0] in pygad.GA.supported_int_types:
+                            if 'step' in curr_gene_space.keys():
+                                step = curr_gene_space['step']
+                            else:
+                                step = None
+
+                            value_from_space = self.unique_int_gene_from_range(solution=solution, 
+                                                                               gene_index=gene_idx, 
+                                                                               min_val=curr_gene_space['low'], 
+                                                                               max_val=curr_gene_space['high'], 
+                                                                               step=step,
+                                                                               mutation_by_replacement=True, 
+                                                                               gene_type=gene_type)
+                        else:
+                            if 'step' in curr_gene_space.keys():
+                                value_from_space = numpy.random.choice(numpy.arange(start=curr_gene_space['low'],
+                                                                                    stop=curr_gene_space['high'],
+                                                                                    step=curr_gene_space['step']),
+                                                                       size=1)
+                            else:
+                                value_from_space = numpy.random.uniform(low=curr_gene_space['low'],
+                                                                        high=curr_gene_space['high'],
+                                                                        size=1)[0]
+                            # TODO: Remove check for mutation_by_replacement when solving duplicates. Just replace the gene by the selected value from space.
+                            # if self.mutation_by_replacement:
+                            #     pass
+                            # else:
+                            #     value_from_space = solution[gene_idx] + value_from_space
+                    else:
+                        # Use index 0 to return the type from the list (e.g. [int, None] or [float, 2]).
+                        if gene_type[gene_idx][0] in pygad.GA.supported_int_types:
+                            if 'step' in curr_gene_space.keys():
+                                step = curr_gene_space['step']
+                            else:
+                                step = None
+
+                            value_from_space = self.unique_int_gene_from_range(solution=solution, 
+                                                                               gene_index=gene_idx, 
+                                                                               min_val=curr_gene_space['low'], 
+                                                                               max_val=curr_gene_space['high'], 
+                                                                               step=step,
+                                                                               mutation_by_replacement=True, 
+                                                                               gene_type=gene_type)
+                        else:
+                            if 'step' in curr_gene_space.keys():
+                                value_from_space = numpy.random.choice(numpy.arange(start=curr_gene_space['low'],
+                                                                                    stop=curr_gene_space['high'],
+                                                                                    step=curr_gene_space['step']),
+                                                                       size=1)
+                            else:
+                                value_from_space = numpy.random.uniform(low=curr_gene_space['low'],
+                                                                        high=curr_gene_space['high'],
+                                                                        size=1)[0]
+                            # TODO: Remove check for mutation_by_replacement when solving duplicates. Just replace the gene by the selected value from space.
+                            # if self.mutation_by_replacement:
+                            #     pass
+                            # else:
+                            #     value_from_space = solution[gene_idx] + value_from_space
+
+                else:
+                    # Selecting a value randomly based on the current gene's space in the 'gene_space' attribute.
+                    # If the gene space has only 1 value, then select it. The old and new values of the gene are identical.
+                    if len(curr_gene_space) == 1:
+                        value_from_space = curr_gene_space[0]
+                        if not self.suppress_warnings: warnings.warn(f"You set 'allow_duplicate_genes=False' but the space of the gene with index {gene_idx} has only a single value. Thus, duplicates are possible.")
+                    # If the gene space has more than 1 value, then select a new one that is different from the current value.
+                    else:
+                        values_to_select_from = list(set(curr_gene_space) - set(solution))
+    
+                        if len(values_to_select_from) == 0:
+                            # DEEP-DUPLICATE-REMOVAL-NEEDED
+                            # Search by this phrase to find where deep duplicates removal should be applied.
+
+                            # Reaching this block means there is no value in the gene space of this gene to solve the duplicates.
+                            # To solve the duplicate between the 2 genes, the solution is to change the value of a third gene that makes a room to solve the duplicate.
+
+                            if not self.suppress_warnings: warnings.warn("You set 'allow_duplicate_genes=False' but the gene space does not have enough values to prevent duplicates.")
+
+                            solution2 = self.solve_duplicates_deeply(solution)
+                            if solution2 is None:
+                                # Cannot solve duplicates. At the moment, we are changing the value of a third gene to solve the duplicates between 2 genes.
+                                # Maybe a 4th, 5th, 6th, or even more genes need to be changed to solve the duplicates.
+                                pass
+                            else:
+                                solution = solution2
+                            value_from_space = solution[gene_idx]
+
+                        else:
+                            value_from_space = random.choice(values_to_select_from)
+            else:
+                # Selecting a value randomly from the global gene space in the 'gene_space' attribute.
+                if type(self.gene_space) is dict:
+                    if self.gene_type_single == True:
+                        if gene_type[0] in pygad.GA.supported_int_types:
+                            if 'step' in self.gene_space.keys():
+                                step = self.gene_space['step']
+                            else:
+                                step = None
+
+                            value_from_space = self.unique_int_gene_from_range(solution=solution, 
+                                                                               gene_index=gene_idx, 
+                                                                               min_val=self.gene_space['low'], 
+                                                                               max_val=self.gene_space['high'], 
+                                                                               step=step,
+                                                                               mutation_by_replacement=True, 
+                                                                               gene_type=gene_type)
+                        else:
+                            # When the gene_space is assigned a dict object, then it specifies the lower and upper limits of all genes in the space.
+                            if 'step' in self.gene_space.keys():
+                                value_from_space = numpy.random.choice(numpy.arange(start=self.gene_space['low'],
+                                                                                    stop=self.gene_space['high'],
+                                                                                    step=self.gene_space['step']),
+                                                                       size=1)
+                            else:
+                                value_from_space = numpy.random.uniform(low=self.gene_space['low'],
+                                                                        high=self.gene_space['high'],
+                                                                        size=1)[0]
+                            # TODO: Remove check for mutation_by_replacement when solving duplicates. Just replace the gene by the selected value from space.
+                            # if self.mutation_by_replacement:
+                            #     pass
+                            # else:
+                            #     value_from_space = solution[gene_idx] + value_from_space
+                    else:
+                        if gene_type[gene_idx][0] in pygad.GA.supported_int_types:
+                            if 'step' in self.gene_space.keys():
+                                step = self.gene_space['step']
+                            else:
+                                step = None
+
+                            value_from_space = self.unique_int_gene_from_range(solution=solution, 
+                                                                               gene_index=gene_idx, 
+                                                                               min_val=self.gene_space['low'], 
+                                                                               max_val=self.gene_space['high'], 
+                                                                               step=step,
+                                                                               mutation_by_replacement=True, 
+                                                                               gene_type=gene_type)
+                        else:
+                            # When the gene_space is assigned a dict object, then it specifies the lower and upper limits of all genes in the space.
+                            if 'step' in self.gene_space.keys():
+                                value_from_space = numpy.random.choice(numpy.arange(start=self.gene_space['low'],
+                                                                                    stop=self.gene_space['high'],
+                                                                                    step=self.gene_space['step']),
+                                                                       size=1)
+                            else:
+                                value_from_space = numpy.random.uniform(low=self.gene_space['low'],
+                                                                        high=self.gene_space['high'],
+                                                                        size=1)[0]
+                            # TODO: Remove check for mutation_by_replacement when solving duplicates. Just replace the gene by the selected value from space.
+                            # if self.mutation_by_replacement:
+                            #     pass
+                            # else:
+                            #     value_from_space = solution[gene_idx] + value_from_space
+    
+                else:
+                    # If the space type is not of type dict, then a value is randomly selected from the gene_space attribute.
+                    # Remove all the genes in the current solution from the gene_space.
+                    # This only leaves the unique values that could be selected for the gene.
+                    values_to_select_from = list(set(self.gene_space) - set(solution))
+    
+                    if len(values_to_select_from) == 0:
+                        if not self.suppress_warnings: warnings.warn("You set 'allow_duplicate_genes=False' but the gene space does not have enough values to prevent duplicates.")
+                        value_from_space = solution[gene_idx]
+                    else:
+                        value_from_space = random.choice(values_to_select_from)
+
+            if value_from_space is None:
+                if build_initial_pop == True:
+                    low = self.init_range_low
+                    high = self.init_range_high
+                else:
+                    low = self.random_mutation_min_val
+                    high = self.random_mutation_max_val
+
+                value_from_space = numpy.random.uniform(low=low,
+                                                        high=high,
+                                                        size=1)[0]
+
+            # Similar to the round_genes() method in the pygad module,
+            # Create a round_gene() method to round a single gene.
+            if self.gene_type_single == True:
+                if not gene_type[1] is None:
+                    value_from_space = numpy.round(gene_type[0](value_from_space),
+                                                   gene_type[1])
+                else:
+                    value_from_space = gene_type[0](value_from_space)
+            else:
+                if not gene_type[gene_idx][1] is None:
+                    value_from_space = numpy.round(gene_type[gene_idx][0](value_from_space),
+                                                  gene_type[gene_idx][1])
+                else:
+                    value_from_space = gene_type[gene_idx][0](value_from_space)
+
+            return value_from_space
+
+    def find_two_duplicates(self, 
+                            solution,
+                            gene_space_unpacked):
+        """
+        Returns the first occurrence of duplicate genes.
+        It returns:
+            The index of a gene with a duplicate value.
+            The value of the gene.
+        """
+        for gene in set(solution):
+            gene_indices = numpy.where(numpy.array(solution) == gene)[0]
+            if len(gene_indices) == 1:
+                continue
+            for gene_idx in gene_indices:
+                number_alternate_values = len(set(gene_space_unpacked[gene_idx]))
+                if number_alternate_values > 1:
+                    return gene_idx, gene
+        # This means there is no way to solve the duplicates between the genes.
+        # Because the space of the duplicates genes only has a single value and there is no alternatives.
+        return None, gene
+    
+    def unpack_gene_space(self, 
+                          range_min,
+                          range_max,
+                          num_values_from_inf_range=100):
+        """
+        Unpack the gene_space for the purpose of selecting a value that solves the duplicates.
+        This is by replacing each range by a list of values.
+        It accepts:
+            range_min: The range minimum value.
+            range_min: The range maximum value.
+            num_values_from_inf_range: For infinite range of float values, a fixed number of values equal to num_values_from_inf_range is selected using the numpy.linspace() function.
+        It returns the unpacked gene space.
+        """
+
+        # Copy the gene_space to keep it isolated form the changes.
+        if self.gene_space is None:
+            return None
+
+        if self.gene_space_nested == False:
+            if type(self.gene_space) is range:
+                gene_space_unpacked = list(self.gene_space)
+            elif type(self.gene_space) in [numpy.ndarray, list]:
+                gene_space_unpacked = self.gene_space.copy()
+            elif type(self.gene_space) is dict:
+                if 'step' in self.gene_space.keys():
+                    gene_space_unpacked = numpy.arange(start=self.gene_space['low'],
+                                                       stop=self.gene_space['high'],
+                                                       step=self.gene_space['step'])
+                else:
+                    gene_space_unpacked = numpy.linspace(start=self.gene_space['low'],
+                                                         stop=self.gene_space['high'],
+                                                         num=num_values_from_inf_range,
+                                                         endpoint=False)
+
+            if self.gene_type_single == True:
+                # Change the data type.
+                gene_space_unpacked = numpy.array(gene_space_unpacked,
+                                                  dtype=self.gene_type[0])
+                if not self.gene_type[1] is None:
+                    # Round the values for float (non-int) data types.
+                    gene_space_unpacked = numpy.round(gene_space_unpacked,
+                                                      self.gene_type[1])
+            else:
+                temp_gene_space_unpacked = gene_space_unpacked.copy()
+                gene_space_unpacked = []
+                # Get the number of genes from the length of gene_type.
+                # The num_genes attribute is not set yet when this method (unpack_gene_space) is called for the first time.
+                for gene_idx in range(len(self.gene_type)):
+                    # Change the data type.
+                    gene_space_item_unpacked = numpy.array(temp_gene_space_unpacked,
+                                                           self.gene_type[gene_idx][0])
+                    if not self.gene_type[gene_idx][1] is None:
+                        # Round the values for float (non-int) data types.
+                        gene_space_item_unpacked = numpy.round(temp_gene_space_unpacked,
+                                                               self.gene_type[gene_idx][1])
+                    gene_space_unpacked.append(gene_space_item_unpacked)
+
+        elif self.gene_space_nested == True:
+            gene_space_unpacked = self.gene_space.copy()
+            for space_idx, space in enumerate(gene_space_unpacked):
+                if type(space) in pygad.GA.supported_int_float_types:
+                    gene_space_unpacked[space_idx] = [space]
+                elif space is None:
+                    # Randomly generate the value using the mutation range.
+                    gene_space_unpacked[space_idx] = numpy.arange(start=range_min,
+                                                                  stop=range_max)
+                elif type(space) is range:
+                    # Convert the range to a list.
+                    gene_space_unpacked[space_idx] = list(space)
+                elif type(space) is dict:
+                    # Create a list of values using the dict range.
+                    # Use numpy.linspace()
+                    if self.gene_type_single == True: # self.gene_type_single
+                        if self.gene_type[0] in pygad.GA.supported_int_types:
+                            if 'step' in space.keys():
+                                step = space['step']
+                            else:
+                                step = 1
+    
+                            gene_space_unpacked[space_idx] = numpy.arange(start=space['low'],
+                                                                          stop=space['high'],
+                                                                          step=step)
+                        else:
+                            if 'step' in space.keys():
+                                gene_space_unpacked[space_idx] = numpy.arange(start=space['low'],
+                                                                              stop=space['high'],
+                                                                              step=space['step'])
+                            else:
+                                gene_space_unpacked[space_idx] = numpy.linspace(start=space['low'],
+                                                                                stop=space['high'],
+                                                                                num=num_values_from_inf_range,
+                                                                                endpoint=False)
+                    else:
+                        if self.gene_type[space_idx][0] in pygad.GA.supported_int_types:
+                            if 'step' in space.keys():
+                                step = space['step']
+                            else:
+                                step = 1
+    
+                            gene_space_unpacked[space_idx] = numpy.arange(start=space['low'],
+                                                                          stop=space['high'],
+                                                                          step=step)
+                        else:
+                            if 'step' in space.keys():
+                                gene_space_unpacked[space_idx] = numpy.arange(start=space['low'],
+                                                                              stop=space['high'],
+                                                                              step=space['step'])
+                            else:
+                                gene_space_unpacked[space_idx] = numpy.linspace(start=space['low'],
+                                                                                stop=space['high'],
+                                                                                num=num_values_from_inf_range,
+                                                                                endpoint=False)
+    
+                elif type(space) in [numpy.ndarray, list, tuple]:
+                    # list/tuple/numpy.ndarray
+                    # Convert all to list
+                    gene_space_unpacked[space_idx] = list(space)
+    
+                    # Check if there is an item with the value None. If so, replace it with a random value using the mutation range.
+                    none_indices = numpy.where(numpy.array(gene_space_unpacked[space_idx]) == None)[0]
+                    if len(none_indices) > 0:
+                        for idx in none_indices:
+                            random_value = numpy.random.uniform(low=range_min,
+                                                                high=range_max,
+                                                                size=1)[0]
+                            gene_space_unpacked[space_idx][idx] = random_value
+    
+                if self.gene_type_single == True: # self.gene_type_single
+                    # Change the data type.
+                    gene_space_unpacked[space_idx] = numpy.array(gene_space_unpacked[space_idx],
+                                                                 dtype=self.gene_type[0])
+                    if not self.gene_type[1] is None:
+                        # Round the values for float (non-int) data types.
+                        gene_space_unpacked[space_idx] = numpy.round(gene_space_unpacked[space_idx],
+                                                                     self.gene_type[1])
+                else:
+                    # Change the data type.
+                    gene_space_unpacked[space_idx] = numpy.array(gene_space_unpacked[space_idx],
+                                                                 self.gene_type[space_idx][0])
+                    if not self.gene_type[space_idx][1] is None:
+                        # Round the values for float (non-int) data types.
+                        gene_space_unpacked[space_idx] = numpy.round(gene_space_unpacked[space_idx],
+                                                                     self.gene_type[space_idx][1])
+
+        return gene_space_unpacked
+
+    def solve_duplicates_deeply(self,
+                                solution):
+        """
+        Sometimes it is impossible to solve the duplicate genes by simply selecting another value for either genes.
+        This function solve the duplicates between 2 genes by searching for a third gene that can make assist in the solution.
+        It returns:
+            The solution after solving the duplicates or the None if duplicates cannot be solved.
+        """
+
+        # gene_space_unpacked = self.unpack_gene_space()
+        # Create a copy of the gene_space_unpacked attribute because it will be changed later.
+        gene_space_unpacked = self.gene_space_unpacked.copy()
+
+        duplicate_index, duplicate_value = self.find_two_duplicates(solution, 
+                                                                    gene_space_unpacked)
+    
+        if duplicate_index is None:
+            # Impossible to solve the duplicates for the genes with value duplicate_value.
+            return None
+    
+    
+        # Without copy(), the gene will be removed from the gene_space.
+        # Convert the space to list because tuples do not have copy()
+        gene_other_values = list(gene_space_unpacked[duplicate_index]).copy()
+
+        # This removes all the occurrences of this value.
+        gene_other_values = [v for v in gene_other_values if v != duplicate_value]
+
+        # The remove() function only removes the first occurrence of the value.
+        # Do not use it.
+        # gene_other_values.remove(duplicate_value)
+    
+        # Two conditions to solve the duplicates of the value D:
+            # 1. From gene_other_values, select a value V such that it is available in the gene space of another gene X.
+            # 2. Find an alternate value for the gene X that will not cause any duplicates.
+            #    2.1 If the gene X does not have alternatives, then go back to step 1 to find another gene.
+            #    2.2 Set the gene X to the value D.
+            #    2.3 Set the target gene to the value V.
+        # Set the space of the duplicate gene to empty list []. Do not remove it to not alter the indices of the gene spaces.
+        gene_space_unpacked[duplicate_index] = []
+
+        for other_value in gene_other_values:
+            for space_idx, space in enumerate(gene_space_unpacked):
+                if other_value in space:
+                    if other_value in solution and list(solution).index(other_value) != space_idx:
+                        continue
+                    else:
+                        # Find an alternate value for the third gene.
+                        # Copy the space so that the original space is not changed after removing the value.
+                        space_other_values = space.copy()
+                        # This removes all the occurrences of this value. It is not enough to use the remove() function because it only removes the first occurrence.
+                        space_other_values = [v for v in space_other_values if v != other_value]
+
+                        for val in space_other_values:
+                            if val in solution:
+                                # If the value exists in another gene of the solution, then we cannot use this value as it will cause another duplicate.
+                                # End the current iteration and go check another value.
+                                continue
+                            else:
+                                solution[space_idx] = val
+                                solution[duplicate_index] = other_value
+                                return solution
+
+        # Reaching here means we cannot solve the duplicate genes.
+        return None
```

### Comparing `pygad-3.0.1/pygad/nn/nn.py` & `pygad-3.1.0/pygad/nn/nn.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     while "previous_layer" in layer.__init__.__code__.co_varnames:
         # If the 'initial' parameter is True, append the initial weights. Otherwise, append the trained weights.
         if initial == True:
             network_weights.append(layer.initial_weights)
         elif initial == False:
             network_weights.append(layer.trained_weights)
         else:
-            raise ValueError("Unexpected value to the 'initial' parameter: {initial}.".format(initial=initial))
+            raise ValueError(f"Unexpected value to the 'initial' parameter: {initial}.")
 
         # Go to the previous layer.
         layer = layer.previous_layer
 
     # If the first layer in the network is not an input layer (i.e. an instance of the InputLayer class), raise an error.
     if not (type(layer) is InputLayer):
         raise TypeError("The first layer in the network architecture must be an input layer.")
@@ -60,15 +60,15 @@
 #            vector = DenseLayer.to_vector(matrix=layer.initial_weights)
             network_weights.extend(vector)
         elif initial == False:
             vector = numpy.reshape(layer.trained_weights, newshape=(layer.trained_weights.size))
 #            vector = DenseLayer.to_vector(array=layer.trained_weights)
             network_weights.extend(vector)
         else:
-            raise ValueError("Unexpected value to the 'initial' parameter: {initial}.".format(initial=initial))
+            raise ValueError(f"Unexpected value to the 'initial' parameter: {initial}.")
 
         # Go to the previous layer.
         layer = layer.previous_layer
 
     # If the first layer in the network is not an input layer (i.e. an instance of the InputLayer class), raise an error.
     if not (type(layer) is InputLayer):
         raise TypeError("The first layer in the network architecture must be an input layer.")
@@ -203,16 +203,16 @@
     data_inputs: Data features.
     data_outputs: Data outputs.
     problem_type: Can be either classification or regression to define the problem type.
     learning_rate: Learning rate which defaults to 0.01.
     """
     
     if not (problem_type in ["classification", "regression"]):
-        raise ValueError("The value of the problem_type parameter can be either classification or regression but {problem_type_val} found.".format(problem_type_val=problem_type))
-    
+        raise ValueError(f"The value of the problem_type parameter can be either classification or regression but {problem_type} found.")
+
     # To fetch the initial weights of the layer, the 'initial' argument is set to True.
     weights = layers_weights(last_layer, initial=True)
     activations = layers_activations(last_layer)
     
     network_error = 0
     for epoch in range(num_epochs):
         print("Epoch ", epoch)
@@ -290,22 +290,22 @@
     last_layer: A reference to the last (output) layer in the network architecture.
     data_inputs: Data features.
     problem_type: Can be either classification or regression to define the problem type.
 
     Returns the predictions of all samples.
     """
     if not (problem_type in ["classification", "regression"]):
-        raise ValueError("The value of the problem_type parameter can be either classification or regression but {problem_type_val} found.".format(problem_type_val=problem_type))
-    
+        raise ValueError(f"The value of the problem_type parameter can be either classification or regression but {problem_type} found.")
+
     # To fetch the trained weights of the layer, the 'initial' argument is set to False.
     weights = layers_weights(last_layer, initial=False)
     activations = layers_activations(last_layer)
 
     if len(weights) != len(activations):
-        raise TypeError("The length of layers {num_layers} is not equal to the number of activations functions {num_activations} and they must be equal.".format(num_layers=len(weights), num_activations=len(activations)))
+        raise TypeError(f"The length of layers {len(weights)} is not equal to the number of activations functions {len(activations)} and they must be equal.")
 
     predictions = []
     for sample_idx in range(data_inputs.shape[0]):
         r1 = data_inputs[sample_idx, :]
         for curr_weights, activation in zip(weights, activations):
             r1 = numpy.matmul(r1, curr_weights)
             if activation == "relu":
@@ -333,34 +333,34 @@
     array: The NumPy array to be converted into a 1D vector.
 
     Returns the array after being reshaped into a NumPy 1D vector.
 
     Example: weights_vector = nn.DenseLayer.to_vector(array=array)
     """
     if not (type(array) is numpy.ndarray):
-        raise TypeError("An input of type numpy.ndarray is expected but an input of type {in_type} found.".format(in_type=type(array)))
+        raise TypeError(f"An input of type numpy.ndarray is expected but an input of type {type(array)} found.")
     return numpy.reshape(array, newshape=(array.size))
 
 def to_array(vector, shape):
     """
     Converts a passed vector to its `vector`  parameter into a NumPy array and returns the array.
 
     vector: The 1D vector to be converted into an array.
     shape: The target shape of the array.
 
     Returns the NumPy 1D vector after being reshaped into an array.
 
     Example: weights_matrix = nn.DenseLayer.to_array(vector=vector, shape=shape)
     """
     if not (type(vector) is numpy.ndarray):
-        raise TypeError("An input of type numpy.ndarray is expected but an input of type {in_type} found.".format(in_type=type(vector)))
+        raise TypeError(f"An input of type numpy.ndarray is expected but an input of type {type(vector)} found.")
     if vector.ndim > 1:
-        raise ValueError("A 1D NumPy array is expected but an array of {ndim} dimensions found.".format(ndim=vector.ndim))
+        raise ValueError(f"A 1D NumPy array is expected but an array of {vector.ndim} dimensions found.")
     if vector.size != functools.reduce(lambda x,y:x*y, shape, 1): # (operator.mul == lambda x,y:x*y
-        raise ValueError("Mismatch between the vector length and the array shape. A vector of length {vector_length} cannot be converted into a array of shape ({array_shape}).".format(vector_length=vector.size, array_shape=shape))
+        raise ValueError(f"Mismatch between the vector length and the array shape. A vector of length {vector.size} cannot be converted into a array of shape ({shape}).")
     return numpy.reshape(vector, newshape=shape)
 
 class InputLayer:
     """
     Implementing the input layer of a neural network.
     """
     def __init__(self, num_inputs):
@@ -377,15 +377,15 @@
         if num_neurons <= 0:
             raise ValueError("Number of neurons cannot be <= 0. Please pass a valid value to the 'num_neurons' parameter.")
         # Number of neurons in the dense layer.
         self.num_neurons = num_neurons
 
         supported_activation_functions = ("sigmoid", "relu", "softmax", "None")
         if not (activation_function in supported_activation_functions):
-            raise ValueError("The specified activation function '{activation_function}' is not among the supported activation functions {supported_activation_functions}. Please use one of the supported functions.".format(activation_function=activation_function, supported_activation_functions=supported_activation_functions))
+            raise ValueError(f"The specified activation function '{activation_function}' is not among the supported activation functions {supported_activation_functions}. Please use one of the supported functions.")
         self.activation_function = activation_function
 
         if previous_layer is None:
             raise TypeError("The previous layer cannot be of Type 'None'. Please pass a valid layer to the 'previous_layer' parameter.")
         # A reference to the layer that preceeds the current layer in the network architecture.
         self.previous_layer = previous_layer
```

### Comparing `pygad-3.0.1/pygad/pygad.py` & `pygad-3.1.0/pygad/pygad.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,32 +5,35 @@
 import warnings
 import concurrent.futures
 import inspect
 import logging
 from pygad import utils
 from pygad import helper
 from pygad import visualize
+import sys
 
-class GA(utils.parent_selection.ParentSelection, 
-         utils.crossover.Crossover, 
-         utils.mutation.Mutation, 
+class GA(utils.parent_selection.ParentSelection,
+         utils.crossover.Crossover,
+         utils.mutation.Mutation,
          helper.unique.Unique,
          visualize.plot.Plot):
 
-    supported_int_types = [int, numpy.int8, numpy.int16, numpy.int32, numpy.int64, numpy.uint, numpy.uint8, numpy.uint16, numpy.uint32, numpy.uint64]
-    supported_float_types = [float, numpy.float16, numpy.float32, numpy.float64]
+    supported_int_types = [int, numpy.int8, numpy.int16, numpy.int32, numpy.int64,
+                           numpy.uint, numpy.uint8, numpy.uint16, numpy.uint32, numpy.uint64]
+    supported_float_types = [
+        float, numpy.float16, numpy.float32, numpy.float64]
     supported_int_float_types = supported_int_types + supported_float_types
 
-    def __init__(self, 
-                 num_generations, 
-                 num_parents_mating, 
+    def __init__(self,
+                 num_generations,
+                 num_parents_mating,
                  fitness_func,
                  fitness_batch_size=None,
                  initial_population=None,
-                 sol_per_pop=None, 
+                 sol_per_pop=None,
                  num_genes=None,
                  init_range_low=-4,
                  init_range_high=4,
                  gene_type=float,
                  parent_selection_type="sss",
                  keep_parents=-1,
                  keep_elitism=1,
@@ -57,15 +60,14 @@
                  save_best_solutions=False,
                  save_solutions=False,
                  suppress_warnings=False,
                  stop_criteria=None,
                  parallel_processing=None,
                  random_seed=None,
                  logger=None):
-
         """
         The constructor of the GA class accepts all parameters required to create an instance of the GA class. It validates such parameters.
 
         num_generations: Number of generations.
         num_parents_mating: Number of solutions to be selected as parents in the mating pool.
 
         fitness_func: Accepts a function/method and returns the fitness value of the solution. In PyGAD 2.20.0, a third parameter is passed referring to the 'pygad.GA' instance. If method, then it must accept 4 parameters where the fourth one refers to the method's object.
@@ -123,1353 +125,1478 @@
 
         parallel_processing: Added in PyGAD 2.17.0. Defaults to `None` which means no parallel processing is used. If a positive integer is assigned, it specifies the number of threads to be used. If a list or a tuple of exactly 2 elements is assigned, then: 1) The first element can be either "process" or "thread" to specify whether processes or threads are used, respectively. 2) The second element can be: 1) A positive integer to select the maximum number of processes or threads to be used. 2) 0 to indicate that parallel processing is not used. This is identical to setting 'parallel_processing=None'. 3) None to use the default value as calculated by the concurrent.futures module.
 
         random_seed: Added in PyGAD 2.18.0. It defines the random seed to be used by the random function generators (we use random functions in the NumPy and random modules). This helps to reproduce the same results by setting the same random seed.
 
         logger: Added in PyGAD 2.20.0. It accepts a logger object of the 'logging.Logger' class to log the messages. If no logger is passed, then a default logger is created to log/print the messages to the console exactly like using the 'print()' function.
         """
+        try:
+            # If no logger is passed, then create a logger that logs only the messages to the console.
+            if logger is None:
+                # Create a logger named with the module name.
+                logger = logging.getLogger(__name__)
+                # Set the logger log level to 'DEBUG' to log all kinds of messages.
+                logger.setLevel(logging.DEBUG)
+
+                # Clear any attached handlers to the logger from the previous runs.
+                # If the handlers are not cleared, then the new handler will be appended to the list of handlers.
+                # This makes the single log message be repeated according to the length of the list of handlers.
+                logger.handlers.clear()
+
+                # Create the handlers.
+                stream_handler = logging.StreamHandler()
+                # Set the handler log level to 'DEBUG' to log all kinds of messages received from the logger.
+                stream_handler.setLevel(logging.DEBUG)
+
+                # Create the formatter that just includes the log message.
+                formatter = logging.Formatter('%(message)s')
 
-        # If no logger is passed, then create a logger that logs only the messages to the console.
-        if logger is None:
-            # Create a logger named with the module name.
-            logger = logging.getLogger(__name__)
-            # Set the logger log level to 'DEBUG' to log all kinds of messages.
-            logger.setLevel(logging.DEBUG)
-
-            # Clear any attached handlers to the logger from the previous runs.
-            # If the handlers are not cleared, then the new handler will be appended to the list of handlers.
-            # This makes the single log message be repeated according to the length of the list of handlers.
-            logger.handlers.clear()
-
-            # Create the handlers.
-            stream_handler = logging.StreamHandler()
-            # Set the handler log level to 'DEBUG' to log all kinds of messages received from the logger.
-            stream_handler.setLevel(logging.DEBUG)
+                # Add the formatter to the handler.
+                stream_handler.setFormatter(formatter)
 
-            # Create the formatter that just includes the log message.
-            formatter = logging.Formatter('%(message)s')
+                # Add the handler to the logger.
+                logger.addHandler(stream_handler)
+            else:
+                # Validate that the passed logger is of type 'logging.Logger'.
+                if isinstance(logger, logging.Logger):
+                    pass
+                else:
+                    raise TypeError(f"The expected type of the 'logger' parameter is 'logging.Logger' but {type(logger)} found.")
 
-            # Add the formatter to the handler.
-            stream_handler.setFormatter(formatter)
+            # Create the 'self.logger' attribute to hold the logger.
+            # Instead of using 'print()', use 'self.logger.info()'
+            self.logger = logger
 
-            # Add the handler to the logger.
-            logger.addHandler(stream_handler)
-        else:
-            # Validate that the passed logger is of type 'logging.Logger'.
-            if isinstance(logger, logging.Logger):
+            self.random_seed = random_seed
+            if random_seed is None:
                 pass
             else:
-                raise TypeError("The expected type of the 'logger' parameter is 'logging.Logger' but {logger_type} found.".format(logger_type=type(logger)))
+                numpy.random.seed(self.random_seed)
+                random.seed(self.random_seed)
 
-        # Create the 'self.logger' attribute to hold the logger.
-        # Instead of using 'print()', use 'self.logger.info()'
-        self.logger = logger
-
-        self.random_seed = random_seed
-        if random_seed is None:
-            pass
-        else:
-            numpy.random.seed(self.random_seed)
-            random.seed(self.random_seed)
+            # If suppress_warnings is bool and its valud is False, then print warning messages.
+            if type(suppress_warnings) is bool:
+                self.suppress_warnings = suppress_warnings
+            else:
+                self.valid_parameters = False
+                raise TypeError(f"The expected type of the 'suppress_warnings' parameter is bool but {type(suppress_warnings)} found.")
 
-        # If suppress_warnings is bool and its valud is False, then print warning messages.
-        if type(suppress_warnings) is bool:
-            self.suppress_warnings = suppress_warnings
-        else:
-            self.valid_parameters = False
-            self.logger.error("The expected type of the 'suppress_warnings' parameter is bool but {suppress_warnings_type} found.".format(suppress_warnings_type=type(suppress_warnings)))
-            raise TypeError("The expected type of the 'suppress_warnings' parameter is bool but {suppress_warnings_type} found.".format(suppress_warnings_type=type(suppress_warnings)))
-
-        # Validating mutation_by_replacement
-        if not (type(mutation_by_replacement) is bool):
-            self.valid_parameters = False
-            self.logger.error("The expected type of the 'mutation_by_replacement' parameter is bool but {mutation_by_replacement_type} found.".format(mutation_by_replacement_type=type(mutation_by_replacement)))
-            raise TypeError("The expected type of the 'mutation_by_replacement' parameter is bool but {mutation_by_replacement_type} found.".format(mutation_by_replacement_type=type(mutation_by_replacement)))
-
-        self.mutation_by_replacement = mutation_by_replacement
-
-        # Validate gene_space
-        self.gene_space_nested = False
-        if type(gene_space) is type(None):
-            pass
-        elif type(gene_space) in [list, tuple, range, numpy.ndarray]:
-            if len(gene_space) == 0:
-                self.valid_parameters = False
-                self.logger.error("'gene_space' cannot be empty (i.e. its length must be >= 0).")
-                raise ValueError("'gene_space' cannot be empty (i.e. its length must be >= 0).")
-            else:
-                for index, el in enumerate(gene_space):
-                    if type(el) in [list, tuple, range, numpy.ndarray]:
-                        if len(el) == 0:
-                            self.valid_parameters = False
-                            self.logger.error("The element indexed {index} of 'gene_space' with type {el_type} cannot be empty (i.e. its length must be >= 0).".format(index=index, el_type=type(el)))
-                            raise ValueError("The element indexed {index} of 'gene_space' with type {el_type} cannot be empty (i.e. its length must be >= 0).".format(index=index, el_type=type(el)))
-                        else:
-                            for val in el:
-                                if not (type(val) in [type(None)] + GA.supported_int_float_types):
-                                    self.logger.error("All values in the sublists inside the 'gene_space' attribute must be numeric of type int/float/None but ({val}) of type {typ} found.".format(val=val, typ=type(val)))
-                                    raise TypeError("All values in the sublists inside the 'gene_space' attribute must be numeric of type int/float/None but ({val}) of type {typ} found.".format(val=val, typ=type(val)))
-                        self.gene_space_nested = True
-                    elif type(el) == type(None):
-                        pass
-                        # self.gene_space_nested = True
-                    elif type(el) is dict:
-                        if len(el.items()) == 2:
-                            if ('low' in el.keys()) and ('high' in el.keys()):
-                                pass
-                            else:
+            # Validating mutation_by_replacement
+            if not (type(mutation_by_replacement) is bool):
+                self.valid_parameters = False
+                raise TypeError(f"The expected type of the 'mutation_by_replacement' parameter is bool but {type(mutation_by_replacement)} found.")
+
+            self.mutation_by_replacement = mutation_by_replacement
+
+            # Validate allow_duplicate_genes
+            if not (type(allow_duplicate_genes) is bool):
+                self.valid_parameters = False
+                raise TypeError(f"The expected type of the 'allow_duplicate_genes' parameter is bool but {type(allow_duplicate_genes)} found.")
+
+            self.allow_duplicate_genes = allow_duplicate_genes
+
+            # Validate gene_space
+            self.gene_space_nested = False
+            if type(gene_space) is type(None):
+                pass
+            elif type(gene_space) is range:
+                if len(gene_space) == 0:
+                    self.valid_parameters = False
+                    raise ValueError("'gene_space' cannot be empty (i.e. its length must be >= 0).")
+            elif type(gene_space) in [list, numpy.ndarray]:
+                if len(gene_space) == 0:
+                    self.valid_parameters = False
+                    raise ValueError("'gene_space' cannot be empty (i.e. its length must be >= 0).")
+                else:
+                    for index, el in enumerate(gene_space):
+                        if type(el) in [numpy.ndarray, list, tuple, range]:
+                            if len(el) == 0:
                                 self.valid_parameters = False
-                                self.logger.error("When an element in the 'gene_space' parameter is of type dict, then it can have the keys 'low', 'high', and 'step' (optional) but the following keys found: {gene_space_dict_keys}".format(gene_space_dict_keys=el.keys()))
-                                raise ValueError("When an element in the 'gene_space' parameter is of type dict, then it can have the keys 'low', 'high', and 'step' (optional) but the following keys found: {gene_space_dict_keys}".format(gene_space_dict_keys=el.keys()))
-                        elif len(el.items()) == 3:
-                            if ('low' in el.keys()) and ('high' in el.keys()) and ('step' in el.keys()):
-                                pass
+                                raise ValueError(f"The element indexed {index} of 'gene_space' with type {type(el)} cannot be empty (i.e. its length must be >= 0).")
+                            else:
+                                for val in el:
+                                    if not (type(val) in [type(None)] + GA.supported_int_float_types):
+                                        raise TypeError(f"All values in the sublists inside the 'gene_space' attribute must be numeric of type int/float/None but ({val}) of type {type(val)} found.")
+                            self.gene_space_nested = True
+                        elif type(el) == type(None):
+                            pass
+                            # self.gene_space_nested = True
+                        elif type(el) is dict:
+                            if len(el.items()) == 2:
+                                if ('low' in el.keys()) and ('high' in el.keys()):
+                                    pass
+                                else:
+                                    self.valid_parameters = False
+                                    raise ValueError(f"When an element in the 'gene_space' parameter is of type dict, then it can have the keys 'low', 'high', and 'step' (optional) but the following keys found: {el.keys()}")
+                            elif len(el.items()) == 3:
+                                if ('low' in el.keys()) and ('high' in el.keys()) and ('step' in el.keys()):
+                                    pass
+                                else:
+                                    self.valid_parameters = False
+                                    raise ValueError(f"When an element in the 'gene_space' parameter is of type dict, then it can have the keys 'low', 'high', and 'step' (optional) but the following keys found: {el.keys()}")
                             else:
                                 self.valid_parameters = False
-                                self.logger.error("When an element in the 'gene_space' parameter is of type dict, then it can have the keys 'low', 'high', and 'step' (optional) but the following keys found: {gene_space_dict_keys}".format(gene_space_dict_keys=el.keys()))
-                                raise ValueError("When an element in the 'gene_space' parameter is of type dict, then it can have the keys 'low', 'high', and 'step' (optional) but the following keys found: {gene_space_dict_keys}".format(gene_space_dict_keys=el.keys()))
-                        else:
+                                raise ValueError(f"When an element in the 'gene_space' parameter is of type dict, then it must have only 2 items but ({len(el.items())}) items found.")
+                            self.gene_space_nested = True
+                        elif not (type(el) in GA.supported_int_float_types):
                             self.valid_parameters = False
-                            self.logger.error("When an element in the 'gene_space' parameter is of type dict, then it must have only 2 items but ({num_items}) items found.".format(num_items=len(el.items())))
-                            raise ValueError("When an element in the 'gene_space' parameter is of type dict, then it must have only 2 items but ({num_items}) items found.".format(num_items=len(el.items())))
-                        self.gene_space_nested = True
-                    elif not (type(el) in GA.supported_int_float_types):
-                        self.valid_parameters = False
-                        self.logger.error("Unexpected type {el_type} for the element indexed {index} of 'gene_space'. The accepted types are list/tuple/range/numpy.ndarray of numbers, a single number (int/float), or None.".format(index=index, el_type=type(el)))
-                        raise TypeError("Unexpected type {el_type} for the element indexed {index} of 'gene_space'. The accepted types are list/tuple/range/numpy.ndarray of numbers, a single number (int/float), or None.".format(index=index, el_type=type(el)))
-
-        elif type(gene_space) is dict:
-            if len(gene_space.items()) == 2:
-                if ('low' in gene_space.keys()) and ('high' in gene_space.keys()):
-                    pass
-                else:
-                    self.valid_parameters = False
-                    self.logger.error("When the 'gene_space' parameter is of type dict, then it can have only the keys 'low', 'high', and 'step' (optional) but the following keys found: {gene_space_dict_keys}".format(gene_space_dict_keys=gene_space.keys()))
-                    raise ValueError("When the 'gene_space' parameter is of type dict, then it can have only the keys 'low', 'high', and 'step' (optional) but the following keys found: {gene_space_dict_keys}".format(gene_space_dict_keys=gene_space.keys()))
-            elif len(gene_space.items()) == 3:
-                if ('low' in gene_space.keys()) and ('high' in gene_space.keys()) and  ('step' in gene_space.keys()):
-                    pass
+                            raise TypeError(f"Unexpected type {type(el)} for the element indexed {index} of 'gene_space'. The accepted types are list/tuple/range/numpy.ndarray of numbers, a single number (int/float), or None.")
+
+            elif type(gene_space) is dict:
+                if len(gene_space.items()) == 2:
+                    if ('low' in gene_space.keys()) and ('high' in gene_space.keys()):
+                        pass
+                    else:
+                        self.valid_parameters = False
+                        raise ValueError(f"When the 'gene_space' parameter is of type dict, then it can have only the keys 'low', 'high', and 'step' (optional) but the following keys found: {gene_space.keys()}")
+                elif len(gene_space.items()) == 3:
+                    if ('low' in gene_space.keys()) and ('high' in gene_space.keys()) and ('step' in gene_space.keys()):
+                        pass
+                    else:
+                        self.valid_parameters = False
+                        raise ValueError(f"When the 'gene_space' parameter is of type dict, then it can have only the keys 'low', 'high', and 'step' (optional) but the following keys found: {gene_space.keys()}")
                 else:
                     self.valid_parameters = False
-                    self.logger.error("When the 'gene_space' parameter is of type dict, then it can have only the keys 'low', 'high', and 'step' (optional) but the following keys found: {gene_space_dict_keys}".format(gene_space_dict_keys=gene_space.keys()))
-                    raise ValueError("When the 'gene_space' parameter is of type dict, then it can have only the keys 'low', 'high', and 'step' (optional) but the following keys found: {gene_space_dict_keys}".format(gene_space_dict_keys=gene_space.keys()))
+                    raise ValueError(f"When the 'gene_space' parameter is of type dict, then it must have only 2 items but ({len(gene_space.items())}) items found.")
+
             else:
                 self.valid_parameters = False
-                self.logger.error("When the 'gene_space' parameter is of type dict, then it must have only 2 items but ({num_items}) items found.".format(num_items=len(gene_space.items())))
-                raise ValueError("When the 'gene_space' parameter is of type dict, then it must have only 2 items but ({num_items}) items found.".format(num_items=len(gene_space.items())))
+                raise TypeError(f"The expected type of 'gene_space' is list, range, or numpy.ndarray but {type(gene_space)} found.")
 
-        else:
-            self.valid_parameters = False
-            self.logger.error("The expected type of 'gene_space' is list, tuple, range, or numpy.ndarray but {gene_space_type} found.".format(gene_space_type=type(gene_space)))
-            raise TypeError("The expected type of 'gene_space' is list, tuple, range, or numpy.ndarray but {gene_space_type} found.".format(gene_space_type=type(gene_space)))
+            self.gene_space = gene_space
 
-        self.gene_space = gene_space
+            # Validate init_range_low and init_range_high
+            # if type(init_range_low) in GA.supported_int_float_types:
+            #     if type(init_range_high) in GA.supported_int_float_types:
+            #         self.init_range_low = init_range_low
+            #         self.init_range_high = init_range_high
+            #     else:
+            #         self.valid_parameters = False
+            #         raise ValueError(f"The value passed to the 'init_range_high' parameter must be either integer or floating-point number but the value ({init_range_high}) of type {type(init_range_high)} found.")
+            # else:
+            #     self.valid_parameters = False
+            #     raise ValueError(f"The value passed to the 'init_range_low' parameter must be either integer or floating-point number but the value ({init_range_low}) of type {type(init_range_low)} found.")
 
-        # Validate init_range_low and init_range_high
-        if type(init_range_low) in GA.supported_int_float_types:
-            if type(init_range_high) in GA.supported_int_float_types:
-                self.init_range_low = init_range_low
-                self.init_range_high = init_range_high
-            else:
-                self.valid_parameters = False
-                self.logger.error("The value passed to the 'init_range_high' parameter must be either integer or floating-point number but the value ({init_range_high_value}) of type {init_range_high_type} found.".format(init_range_high_value=init_range_high, init_range_high_type=type(init_range_high)))
-                raise ValueError("The value passed to the 'init_range_high' parameter must be either integer or floating-point number but the value ({init_range_high_value}) of type {init_range_high_type} found.".format(init_range_high_value=init_range_high, init_range_high_type=type(init_range_high)))
-        else:
-            self.valid_parameters = False
-            self.logger.error("The value passed to the 'init_range_low' parameter must be either integer or floating-point number but the value ({init_range_low_value}) of type {init_range_low_type} found.".format(init_range_low_value=init_range_low, init_range_low_type=type(init_range_low)))
-            raise ValueError("The value passed to the 'init_range_low' parameter must be either integer or floating-point number but the value ({init_range_low_value}) of type {init_range_low_type} found.".format(init_range_low_value=init_range_low, init_range_low_type=type(init_range_low)))
-
-        # Validate random_mutation_min_val and random_mutation_max_val
-        if type(random_mutation_min_val) in GA.supported_int_float_types:
-            if type(random_mutation_max_val) in GA.supported_int_float_types:
-                if random_mutation_min_val == random_mutation_max_val:
-                    if not self.suppress_warnings: warnings.warn("The values of the 2 parameters 'random_mutation_min_val' and 'random_mutation_max_val' are equal and this causes a fixed change to all genes.")
+            # Validate init_range_low and init_range_high
+            if type(init_range_low) in GA.supported_int_float_types:
+                if type(init_range_high) in GA.supported_int_float_types:
+                    if init_range_low == init_range_high:
+                        if not self.suppress_warnings:
+                            warnings.warn("The values of the 2 parameters 'init_range_low' and 'init_range_high' are equal and this might return the same value for some genes in the initial population.")
+                else:
+                    self.valid_parameters = False
+                    raise TypeError(f"Type mismatch between the 2 parameters 'init_range_low' {type(init_range_low)} and 'init_range_high' {type(init_range_high)}.")
+            elif type(init_range_low) in [list, tuple, numpy.ndarray]:
+                # The self.num_genes attribute is not created yet.
+                # if len(init_range_low) == self.num_genes:
+                #     pass
+                # else:
+                #     self.valid_parameters = False
+                #     raise ValueError(f"The length of the 'init_range_low' parameter is {len(init_range_low)} which is different from the number of genes {self.num_genes}.")
+
+                # Get the number of genes before validating the num_genes parameter.
+                if num_genes is None:
+                    if initial_population is None:
+                        self.valid_parameters = False
+                        raise TypeError("When the parameter 'initial_population' is None, then the 2 parameters 'sol_per_pop' and 'num_genes' cannot be None too.")
+                    elif not len(init_range_low) == len(initial_population[0]):
+                        self.valid_parameters = False
+                        raise ValueError(f"The length of the 'init_range_low' parameter is {len(init_range_low)} which is different from the number of genes {len(initial_population[0])}.")
+                elif not len(init_range_low) == num_genes:
+                    self.valid_parameters = False
+                    raise ValueError(f"The length of the 'init_range_low' parameter is {len(init_range_low)} which is different from the number of genes {num_genes}.")
+
+                if type(init_range_high) in [list, tuple, numpy.ndarray]:
+                    if len(init_range_low) == len(init_range_high):
+                        pass
+                    else:
+                        self.valid_parameters = False
+                        raise ValueError(f"Size mismatch between the 2 parameters 'init_range_low' {len(init_range_low)} and 'init_range_high' {len(init_range_high)}.")
+
+                    # Validate the values in init_range_low
+                    for val in init_range_low:
+                        if type(val) in GA.supported_int_float_types:
+                            pass
+                        else:
+                            self.valid_parameters = False
+                            raise TypeError(f"When an iterable (list/tuple/numpy.ndarray) is assigned to the 'init_range_low' parameter, its elements must be numeric but the value {val} of type {type(val)} found.")
+
+                    # Validate the values in init_range_high
+                    for val in init_range_high:
+                        if type(val) in GA.supported_int_float_types:
+                            pass
+                        else:
+                            self.valid_parameters = False
+                            raise TypeError(f"When an iterable (list/tuple/numpy.ndarray) is assigned to the 'init_range_high' parameter, its elements must be numeric but the value {val} of type {type(val)} found.")
+                else:
+                    self.valid_parameters = False
+                    raise TypeError(f"Type mismatch between the 2 parameters 'init_range_low' {type(init_range_low)} and 'init_range_high' {type(init_range_high)}. Both of them can be either numeric or iterable (list/tuple/numpy.ndarray).")
             else:
                 self.valid_parameters = False
-                self.logger.error("The expected type of the 'random_mutation_max_val' parameter is numeric but {random_mutation_max_val_type} found.".format(random_mutation_max_val_type=type(random_mutation_max_val)))
-                raise TypeError("The expected type of the 'random_mutation_max_val' parameter is numeric but {random_mutation_max_val_type} found.".format(random_mutation_max_val_type=type(random_mutation_max_val)))
-        else:
-            self.valid_parameters = False
-            self.logger.error("The expected type of the 'random_mutation_min_val' parameter is numeric but {random_mutation_min_val_type} found.".format(random_mutation_min_val_type=type(random_mutation_min_val)))
-            raise TypeError("The expected type of the 'random_mutation_min_val' parameter is numeric but {random_mutation_min_val_type} found.".format(random_mutation_min_val_type=type(random_mutation_min_val)))
-        self.random_mutation_min_val = random_mutation_min_val
-        self.random_mutation_max_val = random_mutation_max_val
-
-        # Validate gene_type
-        if gene_type in GA.supported_int_float_types:
-            self.gene_type = [gene_type, None]
-            self.gene_type_single = True
-        # A single data type of float with precision.
-        elif len(gene_type) == 2 and gene_type[0] in GA.supported_float_types and (type(gene_type[1]) in GA.supported_int_types or gene_type[1] is None):
-            self.gene_type = gene_type
-            self.gene_type_single = True
-        elif type(gene_type) in [list, tuple, numpy.ndarray]:
-            if num_genes is None:
-                if initial_population is None:
-                    self.valid_parameters = False
-                    self.logger.error("When the parameter 'initial_population' is None, then the 2 parameters 'sol_per_pop' and 'num_genes' cannot be None too.")
-                    raise TypeError("When the parameter 'initial_population' is None, then the 2 parameters 'sol_per_pop' and 'num_genes' cannot be None too.")
-                elif not len(gene_type) == len(initial_population[0]):
-                    self.valid_parameters = False
-                    self.logger.error("When the parameter 'gene_type' is nested, then it can be either [float, int<precision>] or with length equal to the number of genes parameter. Instead, value {gene_type_val} with len(gene_type) ({len_gene_type}) != number of genes ({num_genes}) found.".format(gene_type_val=gene_type, len_gene_type=len(gene_type), num_genes=len(initial_population[0])))
-                    raise ValueError("When the parameter 'gene_type' is nested, then it can be either [float, int<precision>] or with length equal to the number of genes parameter. Instead, value {gene_type_val} with len(gene_type) ({len_gene_type}) != number of genes ({num_genes}) found.".format(gene_type_val=gene_type, len_gene_type=len(gene_type), num_genes=len(initial_population[0])))
-            elif not len(gene_type) == num_genes:
-                self.valid_parameters = False
-                self.logger.error("When the parameter 'gene_type' is nested, then it can be either [float, int<precision>] or with length equal to the value passed to the 'num_genes' parameter. Instead, value {gene_type_val} with len(gene_type) ({len_gene_type}) != len(num_genes) ({num_genes}) found.".format(gene_type_val=gene_type, len_gene_type=len(gene_type), num_genes=num_genes))
-                raise ValueError("When the parameter 'gene_type' is nested, then it can be either [float, int<precision>] or with length equal to the value passed to the 'num_genes' parameter. Instead, value {gene_type_val} with len(gene_type) ({len_gene_type}) != len(num_genes) ({num_genes}) found.".format(gene_type_val=gene_type, len_gene_type=len(gene_type), num_genes=num_genes))
-            for gene_type_idx, gene_type_val in enumerate(gene_type):
-                if gene_type_val in GA.supported_float_types:
-                    # If the gene type is float and no precision is passed, set it to None.
-                    gene_type[gene_type_idx] = [gene_type_val, None]
-                elif gene_type_val in GA.supported_int_types:
-                    gene_type[gene_type_idx] = [gene_type_val, None]
-                elif type(gene_type_val) in [list, tuple, numpy.ndarray]:
-                    # A float type is expected in a list/tuple/numpy.ndarray of length 2.
-                    if len(gene_type_val) == 2:
-                        if gene_type_val[0] in GA.supported_float_types:
-                            if type(gene_type_val[1]) in GA.supported_int_types:
-                                pass
+                raise TypeError(f"The expected type of the 'init_range_low' parameter is numeric or list/tuple/numpy.ndarray but {type(init_range_low)} found.")
+
+            self.init_range_low = init_range_low
+            self.init_range_high = init_range_high
+
+            # Validate gene_type
+            if gene_type in GA.supported_int_float_types:
+                self.gene_type = [gene_type, None]
+                self.gene_type_single = True
+            # A single data type of float with precision.
+            elif len(gene_type) == 2 and gene_type[0] in GA.supported_float_types and (type(gene_type[1]) in GA.supported_int_types or gene_type[1] is None):
+                self.gene_type = gene_type
+                self.gene_type_single = True
+            # A single data type of int with precision.
+            elif len(gene_type) == 2 and gene_type[0] in GA.supported_int_types and (type(gene_type[1]) in GA.supported_int_types or gene_type[1] is None):
+                self.gene_type_single = False
+                raise ValueError(f"Integers cannot have precision. Please use the integer data type directly instead of {gene_type}.")
+            elif type(gene_type) in [list, tuple, numpy.ndarray]:
+                # Get the number of genes before validating the num_genes parameter.
+                if num_genes is None:
+                    if initial_population is None:
+                        self.valid_parameters = False
+                        raise TypeError("When the parameter 'initial_population' is None, then the 2 parameters 'sol_per_pop' and 'num_genes' cannot be None too.")
+                    elif not len(gene_type) == len(initial_population[0]):
+                        self.valid_parameters = False
+                        raise ValueError(f"When the parameter 'gene_type' is nested, then it can be either [float, int<precision>] or with length equal to the number of genes parameter. Instead, value {gene_type} with len(gene_type) ({len(gene_type)}) != number of genes ({len(initial_population[0])}) found.")
+                elif not len(gene_type) == num_genes:
+                    self.valid_parameters = False
+                    raise ValueError(f"When the parameter 'gene_type' is nested, then it can be either [float, int<precision>] or with length equal to the value passed to the 'num_genes' parameter. Instead, value {gene_type} with len(gene_type) ({len(gene_type)}) != len(num_genes) ({num_genes}) found.")
+                for gene_type_idx, gene_type_val in enumerate(gene_type):
+                    if gene_type_val in GA.supported_float_types:
+                        # If the gene type is float and no precision is passed, set it to None.
+                        gene_type[gene_type_idx] = [gene_type_val, None]
+                    elif gene_type_val in GA.supported_int_types:
+                        gene_type[gene_type_idx] = [gene_type_val, None]
+                    elif type(gene_type_val) in [list, tuple, numpy.ndarray]:
+                        # A float type is expected in a list/tuple/numpy.ndarray of length 2.
+                        if len(gene_type_val) == 2:
+                            if gene_type_val[0] in GA.supported_float_types:
+                                if type(gene_type_val[1]) in GA.supported_int_types:
+                                    pass
+                                else:
+                                    self.valid_parameters = False
+                                    raise TypeError(f"In the 'gene_type' parameter, the precision for float gene data types must be an integer but the element {gene_type_val} at index {gene_type_idx} has a precision of {gene_type_val[1]} with type {gene_type_val[0]}.")
                             else:
                                 self.valid_parameters = False
-                                self.logger.error("In the 'gene_type' parameter, the precision for float gene data types must be an integer but the element {gene_type_val} at index {gene_type_idx} has a precision of {gene_type_precision_val} with type {gene_type_type}.".format(gene_type_val=gene_type_val, gene_type_precision_val=gene_type_val[1], gene_type_type=gene_type_val[0], gene_type_idx=gene_type_idx))
-                                raise TypeError("In the 'gene_type' parameter, the precision for float gene data types must be an integer but the element {gene_type_val} at index {gene_type_idx} has a precision of {gene_type_precision_val} with type {gene_type_type}.".format(gene_type_val=gene_type_val, gene_type_precision_val=gene_type_val[1], gene_type_type=gene_type_val[0], gene_type_idx=gene_type_idx))
+                                raise TypeError(
+                                    f"In the 'gene_type' parameter, a precision is expected only for float gene data types but the element {gene_type_val} found at index {gene_type_idx}.\nNote that the data type must be at index 0 of the item followed by precision at index 1.")
                         else:
                             self.valid_parameters = False
-                            self.logger.error("In the 'gene_type' parameter, a precision is expected only for float gene data types but the element {gene_type} found at index {gene_type_idx}.\nNote that the data type must be at index 0 followed by precision at index 1.".format(gene_type=gene_type_val, gene_type_idx=gene_type_idx))
-                            raise TypeError("In the 'gene_type' parameter, a precision is expected only for float gene data types but the element {gene_type} found at index {gene_type_idx}.\nNote that the data type must be at index 0 followed by precision at index 1.".format(gene_type=gene_type_val, gene_type_idx=gene_type_idx))
+                            raise ValueError(f"In the 'gene_type' parameter, a precision is specified in a list/tuple/numpy.ndarray of length 2 but value ({gene_type_val}) of type {type(gene_type_val)} with length {len(gene_type_val)} found at index {gene_type_idx}.")
                     else:
                         self.valid_parameters = False
-                        self.logger.error("In the 'gene_type' parameter, a precision is specified in a list/tuple/numpy.ndarray of length 2 but value ({gene_type_val}) of type {gene_type_type} with length {gene_type_length} found at index {gene_type_idx}.".format(gene_type_val=gene_type_val, gene_type_type=type(gene_type_val), gene_type_idx=gene_type_idx, gene_type_length=len(gene_type_val)))
-                        raise ValueError("In the 'gene_type' parameter, a precision is specified in a list/tuple/numpy.ndarray of length 2 but value ({gene_type_val}) of type {gene_type_type} with length {gene_type_length} found at index {gene_type_idx}.".format(gene_type_val=gene_type_val, gene_type_type=type(gene_type_val), gene_type_idx=gene_type_idx, gene_type_length=len(gene_type_val)))
+                        raise ValueError(f"When a list/tuple/numpy.ndarray is assigned to the 'gene_type' parameter, then its elements must be of integer, floating-point, list, tuple, or numpy.ndarray data types but the value ({gene_type_val}) of type {type(gene_type_val)} found at index {gene_type_idx}.")
+                self.gene_type = gene_type
+                self.gene_type_single = False
+            else:
+                self.valid_parameters = False
+                raise ValueError(f"The value passed to the 'gene_type' parameter must be either a single integer, floating-point, list, tuple, or numpy.ndarray but ({gene_type}) of type {type(gene_type)} found.")
+
+            # Call the unpack_gene_space() method in the pygad.helper.unique.Unique class.
+            self.gene_space_unpacked = self.unpack_gene_space(range_min=self.init_range_low,
+                                                              range_max=self.init_range_high)
+
+            # Build the initial population
+            if initial_population is None:
+                if (sol_per_pop is None) or (num_genes is None):
+                    self.valid_parameters = False
+                    raise TypeError("Error creating the initial population:\n\nWhen the parameter 'initial_population' is None, then the 2 parameters 'sol_per_pop' and 'num_genes' cannot be None too.\nThere are 2 options to prepare the initial population:\n1) Assinging the initial population to the 'initial_population' parameter. In this case, the values of the 2 parameters sol_per_pop and num_genes will be deduced.\n2) Assign integer values to the 'sol_per_pop' and 'num_genes' parameters so that PyGAD can create the initial population automatically.")
+                elif (type(sol_per_pop) is int) and (type(num_genes) is int):
+                    # Validating the number of solutions in the population (sol_per_pop)
+                    if sol_per_pop <= 0:
+                        self.valid_parameters = False
+                        raise ValueError(f"The number of solutions in the population (sol_per_pop) must be > 0 but ({sol_per_pop}) found. \nThe following parameters must be > 0: \n1) Population size (i.e. number of solutions per population) (sol_per_pop).\n2) Number of selected parents in the mating pool (num_parents_mating).\n")
+                    # Validating the number of gene.
+                    if (num_genes <= 0):
+                        self.valid_parameters = False
+                        raise ValueError(f"The number of genes cannot be <= 0 but ({num_genes}) found.\n")
+                    # When initial_population=None and the 2 parameters sol_per_pop and num_genes have valid integer values, then the initial population is created.
+                    # Inside the initialize_population() method, the initial_population attribute is assigned to keep the initial population accessible.
+                    self.num_genes = num_genes  # Number of genes in the solution.
+
+                    # In case the 'gene_space' parameter is nested, then make sure the number of its elements equals to the number of genes.
+                    if self.gene_space_nested:
+                        if len(gene_space) != self.num_genes:
+                            self.valid_parameters = False
+                            raise ValueError(f"When the parameter 'gene_space' is nested, then its length must be equal to the value passed to the 'num_genes' parameter. Instead, length of gene_space ({len(gene_space)}) != num_genes ({self.num_genes})")
+
+                    # Number of solutions in the population.
+                    self.sol_per_pop = sol_per_pop
+                    self.initialize_population(low=self.init_range_low,
+                                               high=self.init_range_high,
+                                               allow_duplicate_genes=allow_duplicate_genes,
+                                               mutation_by_replacement=True,
+                                               gene_type=self.gene_type)
                 else:
                     self.valid_parameters = False
-                    self.logger.error("When a list/tuple/numpy.ndarray is assigned to the 'gene_type' parameter, then its elements must be of integer, floating-point, list, tuple, or numpy.ndarray data types but the value ({gene_type_val}) of type {gene_type_type} found at index {gene_type_idx}.".format(gene_type_val=gene_type_val, gene_type_type=type(gene_type_val), gene_type_idx=gene_type_idx))
-                    raise ValueError("When a list/tuple/numpy.ndarray is assigned to the 'gene_type' parameter, then its elements must be of integer, floating-point, list, tuple, or numpy.ndarray data types but the value ({gene_type_val}) of type {gene_type_type} found at index {gene_type_idx}.".format(gene_type_val=gene_type_val, gene_type_type=type(gene_type_val), gene_type_idx=gene_type_idx))
-            self.gene_type = gene_type
-            self.gene_type_single = False
-        else:
-            self.valid_parameters = False
-            self.logger.error("The value passed to the 'gene_type' parameter must be either a single integer, floating-point, list, tuple, or numpy.ndarray but ({gene_type_val}) of type {gene_type_type} found.".format(gene_type_val=gene_type, gene_type_type=type(gene_type)))
-            raise ValueError("The value passed to the 'gene_type' parameter must be either a single integer, floating-point, list, tuple, or numpy.ndarray but ({gene_type_val}) of type {gene_type_type} found.".format(gene_type_val=gene_type, gene_type_type=type(gene_type)))
-
-        # Build the initial population
-        if initial_population is None:
-            if (sol_per_pop is None) or (num_genes is None):
-                self.valid_parameters = False
-                self.logger.error("Error creating the initial population:\n\nWhen the parameter 'initial_population' is None, then the 2 parameters 'sol_per_pop' and 'num_genes' cannot be None too.\nThere are 2 options to prepare the initial population:\n1) Assinging the initial population to the 'initial_population' parameter. In this case, the values of the 2 parameters sol_per_pop and num_genes will be deduced.\n2) Assign integer values to the 'sol_per_pop' and 'num_genes' parameters so that PyGAD can create the initial population automatically.")
-                raise TypeError("Error creating the initial population:\n\nWhen the parameter 'initial_population' is None, then the 2 parameters 'sol_per_pop' and 'num_genes' cannot be None too.\nThere are 2 options to prepare the initial population:\n1) Assinging the initial population to the 'initial_population' parameter. In this case, the values of the 2 parameters sol_per_pop and num_genes will be deduced.\n2) Assign integer values to the 'sol_per_pop' and 'num_genes' parameters so that PyGAD can create the initial population automatically.")
-            elif (type(sol_per_pop) is int) and (type(num_genes) is int):
-                # Validating the number of solutions in the population (sol_per_pop)
-                if sol_per_pop <= 0:
-                    self.valid_parameters = False
-                    self.logger.error("The number of solutions in the population (sol_per_pop) must be > 0 but ({sol_per_pop}) found. \nThe following parameters must be > 0: \n1) Population size (i.e. number of solutions per population) (sol_per_pop).\n2) Number of selected parents in the mating pool (num_parents_mating).\n".format(sol_per_pop=sol_per_pop))
-                    raise ValueError("The number of solutions in the population (sol_per_pop) must be > 0 but ({sol_per_pop}) found. \nThe following parameters must be > 0: \n1) Population size (i.e. number of solutions per population) (sol_per_pop).\n2) Number of selected parents in the mating pool (num_parents_mating).\n".format(sol_per_pop=sol_per_pop))
-                # Validating the number of gene.
-                if (num_genes <= 0):
-                    self.valid_parameters = False
-                    self.logger.error("The number of genes cannot be <= 0 but ({num_genes}) found.\n".format(num_genes=num_genes))
-                    raise ValueError("The number of genes cannot be <= 0 but ({num_genes}) found.\n".format(num_genes=num_genes))
-                # When initial_population=None and the 2 parameters sol_per_pop and num_genes have valid integer values, then the initial population is created.
-                # Inside the initialize_population() method, the initial_population attribute is assigned to keep the initial population accessible.
-                self.num_genes = num_genes # Number of genes in the solution.
-
-                # In case the 'gene_space' parameter is nested, then make sure the number of its elements equals to the number of genes.
-                if self.gene_space_nested:
-                    if len(gene_space) != self.num_genes:
-                        self.valid_parameters = False
-                        self.logger.error("When the parameter 'gene_space' is nested, then its length must be equal to the value passed to the 'num_genes' parameter. Instead, length of gene_space ({len_gene_space}) != num_genes ({num_genes})".format(len_gene_space=len(gene_space), num_genes=self.num_genes))
-                        raise ValueError("When the parameter 'gene_space' is nested, then its length must be equal to the value passed to the 'num_genes' parameter. Instead, length of gene_space ({len_gene_space}) != num_genes ({num_genes})".format(len_gene_space=len(gene_space), num_genes=self.num_genes))
-
-                self.sol_per_pop = sol_per_pop # Number of solutions in the population.
-                self.initialize_population(self.init_range_low, 
-                                           self.init_range_high, 
-                                           allow_duplicate_genes, 
-                                           True, 
-                                           self.gene_type)
-            else:
-                self.valid_parameters = False
-                self.logger.error("The expected type of both the sol_per_pop and num_genes parameters is int but {sol_per_pop_type} and {num_genes_type} found.".format(sol_per_pop_type=type(sol_per_pop), num_genes_type=type(num_genes)))
-                raise TypeError("The expected type of both the sol_per_pop and num_genes parameters is int but {sol_per_pop_type} and {num_genes_type} found.".format(sol_per_pop_type=type(sol_per_pop), num_genes_type=type(num_genes)))
-        elif not type(initial_population) in [list, tuple, numpy.ndarray]:
-            self.valid_parameters = False
-            self.logger.error("The value assigned to the 'initial_population' parameter is expected to by of type list, tuple, or ndarray but {initial_population_type} found.".format(initial_population_type=type(initial_population)))
-            raise TypeError("The value assigned to the 'initial_population' parameter is expected to by of type list, tuple, or ndarray but {initial_population_type} found.".format(initial_population_type=type(initial_population)))
-        elif numpy.array(initial_population).ndim != 2:
-            self.valid_parameters = False
-            self.logger.error("A 2D list is expected to the initail_population parameter but a ({initial_population_ndim}-D) list found.".format(initial_population_ndim=numpy.array(initial_population).ndim))
-            raise ValueError("A 2D list is expected to the initail_population parameter but a ({initial_population_ndim}-D) list found.".format(initial_population_ndim=numpy.array(initial_population).ndim))
-        else:
-            # Validate the type of each value in the 'initial_population' parameter.
-            for row_idx in range(len(initial_population)):
-                for col_idx in range(len(initial_population[0])):
-                    if type(initial_population[row_idx][col_idx]) in GA.supported_int_float_types:
+                    raise TypeError(f"The expected type of both the sol_per_pop and num_genes parameters is int but {type(sol_per_pop)} and {type(num_genes)} found.")
+            elif not type(initial_population) in [list, tuple, numpy.ndarray]:
+                self.valid_parameters = False
+                raise TypeError(f"The value assigned to the 'initial_population' parameter is expected to by of type list, tuple, or ndarray but {type(initial_population)} found.")
+            elif numpy.array(initial_population).ndim != 2:
+                self.valid_parameters = False
+                raise ValueError(f"A 2D list is expected to the initail_population parameter but a ({numpy.array(initial_population).ndim}-D) list found.")
+            else:
+                # Validate the type of each value in the 'initial_population' parameter.
+                for row_idx in range(len(initial_population)):
+                    for col_idx in range(len(initial_population[0])):
+                        if type(initial_population[row_idx][col_idx]) in GA.supported_int_float_types:
+                            pass
+                        else:
+                            self.valid_parameters = False
+                            raise TypeError(f"The values in the initial population can be integers or floats but the value ({initial_population[row_idx][col_idx]}) of type {type(initial_population[row_idx][col_idx])} found.")
+
+                # Forcing the initial_population array to have the data type assigned to the gene_type parameter.
+                if self.gene_type_single == True:
+                    if self.gene_type[1] == None:
+                        self.initial_population = numpy.array(initial_population,
+                                                            dtype=self.gene_type[0])
+                    else:
+                        # This block is reached only for non-integer data types (i.e. float).
+                        self.initial_population = numpy.round(numpy.array(initial_population,
+                                                                        dtype=self.gene_type[0]),
+                                                            self.gene_type[1])
+                else:
+                    initial_population = numpy.array(initial_population)
+                    self.initial_population = numpy.zeros(shape=(initial_population.shape[0],
+                                                                initial_population.shape[1]),
+                                                        dtype=object)
+                    for gene_idx in range(initial_population.shape[1]):
+                        if self.gene_type[gene_idx][1] is None:
+                            self.initial_population[:, gene_idx] = numpy.asarray(initial_population[:, gene_idx],
+                                                                                dtype=self.gene_type[gene_idx][0])
+                        else:
+                            # This block is reached only for non-integer data types (i.e. float).
+                            self.initial_population[:, gene_idx] = numpy.round(numpy.asarray(initial_population[:, gene_idx],
+                                                                                            dtype=self.gene_type[gene_idx][0]),
+                                                                            self.gene_type[gene_idx][1])
+
+                # Check if duplicates are allowed. If not, then solve any exisiting duplicates in the passed initial population.
+                if self.allow_duplicate_genes == False:
+                    for initial_solution_idx, initial_solution in enumerate(self.initial_population):
+                        if self.gene_space is None:
+                            self.initial_population[initial_solution_idx], _, _ = self.solve_duplicate_genes_randomly(solution=initial_solution,
+                                                                                                                    min_val=self.init_range_low,
+                                                                                                                    max_val=self.init_range_high,
+                                                                                                                    mutation_by_replacement=self.mutation_by_replacement,
+                                                                                                                    gene_type=self.gene_type,
+                                                                                                                    num_trials=10)
+                        else:
+                            self.initial_population[initial_solution_idx], _, _ = self.solve_duplicate_genes_by_space(solution=initial_solution,
+                                                                                                                    gene_type=self.gene_type,
+                                                                                                                    num_trials=10)
+
+                # A NumPy array holding the initial population.
+                self.population = self.initial_population.copy()
+                # Number of genes in the solution.
+                self.num_genes = self.initial_population.shape[1]
+                # Number of solutions in the population.
+                self.sol_per_pop = self.initial_population.shape[0]
+                # The population size.
+                self.pop_size = (self.sol_per_pop, self.num_genes)
+
+            # Round initial_population and population
+            self.initial_population = self.round_genes(self.initial_population)
+            self.population = self.round_genes(self.population)
+
+            # In case the 'gene_space' parameter is nested, then make sure the number of its elements equals to the number of genes.
+            if self.gene_space_nested:
+                if len(gene_space) != self.num_genes:
+                    self.valid_parameters = False
+                    raise ValueError(f"When the parameter 'gene_space' is nested, then its length must be equal to the value passed to the 'num_genes' parameter. Instead, length of gene_space ({len(gene_space)}) != num_genes ({self.num_genes})")
+
+            # Validate random_mutation_min_val and random_mutation_max_val
+            if type(random_mutation_min_val) in GA.supported_int_float_types:
+                if type(random_mutation_max_val) in GA.supported_int_float_types:
+                    if random_mutation_min_val == random_mutation_max_val:
+                        if not self.suppress_warnings:
+                            warnings.warn("The values of the 2 parameters 'random_mutation_min_val' and 'random_mutation_max_val' are equal and this might cause a fixed mutation to some genes.")
+                else:
+                    self.valid_parameters = False
+                    raise TypeError(f"Type mismatch between the 2 parameters 'random_mutation_min_val' {type(random_mutation_min_val)} and 'random_mutation_max_val' {type(random_mutation_max_val)}.")
+            elif type(random_mutation_min_val) in [list, tuple, numpy.ndarray]:
+                if len(random_mutation_min_val) == self.num_genes:
+                    pass
+                else:
+                    self.valid_parameters = False
+                    raise ValueError(f"The length of the 'random_mutation_min_val' parameter is {len(random_mutation_min_val)} which is different from the number of genes {self.num_genes}.")
+                if type(random_mutation_max_val) in [list, tuple, numpy.ndarray]:
+                    if len(random_mutation_min_val) == len(random_mutation_max_val):
                         pass
                     else:
                         self.valid_parameters = False
-                        self.logger.error("The values in the initial population can be integers or floats but the value ({value}) of type {value_type} found.".format(value=initial_population[row_idx][col_idx], value_type=type(initial_population[row_idx][col_idx])))
-                        raise TypeError("The values in the initial population can be integers or floats but the value ({value}) of type {value_type} found.".format(value=initial_population[row_idx][col_idx], value_type=type(initial_population[row_idx][col_idx])))
+                        raise ValueError(f"Size mismatch between the 2 parameters 'random_mutation_min_val' {len(random_mutation_min_val)} and 'random_mutation_max_val' {len(random_mutation_max_val)}.")
 
-            # Forcing the initial_population array to have the data type assigned to the gene_type parameter.
-            if self.gene_type_single == True:
-                if self.gene_type[1] == None:
-                    self.initial_population = numpy.array(initial_population, dtype=self.gene_type[0])
+                    # Validate the values in random_mutation_min_val
+                    for val in random_mutation_min_val:
+                        if type(val) in GA.supported_int_float_types:
+                            pass
+                        else:
+                            self.valid_parameters = False
+                            raise TypeError(f"When an iterable (list/tuple/numpy.ndarray) is assigned to the 'random_mutation_min_val' parameter, its elements must be numeric but the value {val} of type {type(val)} found.")
+
+                    # Validate the values in random_mutation_max_val
+                    for val in random_mutation_max_val:
+                        if type(val) in GA.supported_int_float_types:
+                            pass
+                        else:
+                            self.valid_parameters = False
+                            raise TypeError(f"When an iterable (list/tuple/numpy.ndarray) is assigned to the 'random_mutation_max_val' parameter, its elements must be numeric but the value {val} of type {type(val)} found.")
                 else:
-                    self.initial_population = numpy.round(numpy.array(initial_population, dtype=self.gene_type[0]), self.gene_type[1])
+                    self.valid_parameters = False
+                    raise TypeError(f"Type mismatch between the 2 parameters 'random_mutation_min_val' {type(random_mutation_min_val)} and 'random_mutation_max_val' {type(random_mutation_max_val)}.")
             else:
-                initial_population = numpy.array(initial_population)
-                self.initial_population = numpy.zeros(shape=(initial_population.shape[0], initial_population.shape[1]), dtype=object)
-                for gene_idx in range(initial_population.shape[1]):
-                    if self.gene_type[gene_idx][1] is None:
-                        self.initial_population[:, gene_idx] = numpy.asarray(initial_population[:, gene_idx], 
-                                                                             dtype=self.gene_type[gene_idx][0])
-                    else:
-                        self.initial_population[:, gene_idx] = numpy.round(numpy.asarray(initial_population[:, gene_idx], 
-                                                                                         dtype=self.gene_type[gene_idx][0]), 
-                                                                           self.gene_type[gene_idx][1])
-
-            self.population = self.initial_population.copy() # A NumPy array holding the initial population.
-            self.num_genes = self.initial_population.shape[1] # Number of genes in the solution.
-            self.sol_per_pop = self.initial_population.shape[0]  # Number of solutions in the population.
-            self.pop_size = (self.sol_per_pop,self.num_genes) # The population size.
-
-        # Round initial_population and population
-        self.initial_population = self.round_genes(self.initial_population)
-        self.population = self.round_genes(self.population)
-
-        # In case the 'gene_space' parameter is nested, then make sure the number of its elements equals to the number of genes.
-        if self.gene_space_nested:
-            if len(gene_space) != self.num_genes:
-                self.valid_parameters = False
-                self.logger.error("When the parameter 'gene_space' is nested, then its length must be equal to the value passed to the 'num_genes' parameter. Instead, length of gene_space ({len_gene_space}) != num_genes ({len_num_genes})".format(len_gene_space=len(gene_space), len_num_genes=self.num_genes))
-                raise ValueError("When the parameter 'gene_space' is nested, then its length must be equal to the value passed to the 'num_genes' parameter. Instead, length of gene_space ({len_gene_space}) != num_genes ({len_num_genes})".format(len_gene_space=len(gene_space), len_num_genes=self.num_genes))
-
-        # Validating the number of parents to be selected for mating (num_parents_mating)
-        if num_parents_mating <= 0:
-            self.valid_parameters = False
-            self.logger.error("The number of parents mating (num_parents_mating) parameter must be > 0 but ({num_parents_mating}) found. \nThe following parameters must be > 0: \n1) Population size (i.e. number of solutions per population) (sol_per_pop).\n2) Number of selected parents in the mating pool (num_parents_mating).\n".format(num_parents_mating=num_parents_mating))
-            raise ValueError("The number of parents mating (num_parents_mating) parameter must be > 0 but ({num_parents_mating}) found. \nThe following parameters must be > 0: \n1) Population size (i.e. number of solutions per population) (sol_per_pop).\n2) Number of selected parents in the mating pool (num_parents_mating).\n".format(num_parents_mating=num_parents_mating))
-
-        # Validating the number of parents to be selected for mating: num_parents_mating
-        if (num_parents_mating > self.sol_per_pop):
-            self.valid_parameters = False
-            self.logger.error("The number of parents to select for mating ({num_parents_mating}) cannot be greater than the number of solutions in the population ({sol_per_pop}) (i.e., num_parents_mating must always be <= sol_per_pop).\n".format(num_parents_mating=num_parents_mating, sol_per_pop=self.sol_per_pop))
-            raise ValueError("The number of parents to select for mating ({num_parents_mating}) cannot be greater than the number of solutions in the population ({sol_per_pop}) (i.e., num_parents_mating must always be <= sol_per_pop).\n".format(num_parents_mating=num_parents_mating, sol_per_pop=self.sol_per_pop))
-
-        self.num_parents_mating = num_parents_mating
-
-        # crossover: Refers to the method that applies the crossover operator based on the selected type of crossover in the crossover_type property.
-        # Validating the crossover type: crossover_type
-        if (crossover_type is None):
-            self.crossover = None
-        elif inspect.ismethod(crossover_type):
-            # Check if the crossover_type is a method that accepts 4 paramaters.
-            if (crossover_type.__code__.co_argcount == 4):
-                # The crossover method assigned to the crossover_type parameter is validated.
-                self.crossover = crossover_type
-            else:
-                self.valid_parameters = False
-                self.logger.error("When 'crossover_type' is assigned to a method, then this crossover method must accept 4 parameters:\n1) Expected to be the 'self' object.\n2) The selected parents.\n3) The size of the offspring to be produced.\n4) The instance from the pygad.GA class.\n\nThe passed crossover method named '{funcname}' accepts {argcount} parameter(s).".format(funcname=crossover_type.__code__.co_name, argcount=crossover_type.__code__.co_argcount))
-                raise ValueError("When 'crossover_type' is assigned to a method, then this crossover method must accept 4 parameters:\n1) Expected to be the 'self' object.\n2) The selected parents.\n3) The size of the offspring to be produced.\n4) The instance from the pygad.GA class.\n\nThe passed crossover method named '{funcname}' accepts {argcount} parameter(s).".format(funcname=crossover_type.__code__.co_name, argcount=crossover_type.__code__.co_argcount))
-        elif callable(crossover_type):
-            # Check if the crossover_type is a function that accepts 2 paramaters.
-            if (crossover_type.__code__.co_argcount == 3):
-                # The crossover function assigned to the crossover_type parameter is validated.
-                self.crossover = crossover_type
-            else:
-                self.valid_parameters = False
-                self.logger.error("When 'crossover_type' is assigned to a function, then this crossover function must accept 3 parameters:\n1) The selected parents.\n2) The size of the offspring to be produced.3) The instance from the pygad.GA class to retrieve any property like population, gene data type, gene space, etc.\n\nThe passed crossover function named '{funcname}' accepts {argcount} parameter(s).".format(funcname=crossover_type.__code__.co_name, argcount=crossover_type.__code__.co_argcount))
-                raise ValueError("When 'crossover_type' is assigned to a function, then this crossover function must accept 3 parameters:\n1) The selected parents.\n2) The size of the offspring to be produced.3) The instance from the pygad.GA class to retrieve any property like population, gene data type, gene space, etc.\n\nThe passed crossover function named '{funcname}' accepts {argcount} parameter(s).".format(funcname=crossover_type.__code__.co_name, argcount=crossover_type.__code__.co_argcount))
-        elif not (type(crossover_type) is str):
-            self.valid_parameters = False
-            self.logger.error("The expected type of the 'crossover_type' parameter is either callable or str but {crossover_type} found.".format(crossover_type=type(crossover_type)))
-            raise TypeError("The expected type of the 'crossover_type' parameter is either callable or str but {crossover_type} found.".format(crossover_type=type(crossover_type)))
-        else: # type crossover_type is str
-            crossover_type = crossover_type.lower()
-            if (crossover_type == "single_point"):
-                self.crossover = self.single_point_crossover
-            elif (crossover_type == "two_points"):
-                self.crossover = self.two_points_crossover
-            elif (crossover_type == "uniform"):
-                self.crossover = self.uniform_crossover
-            elif (crossover_type == "scattered"):
-                self.crossover = self.scattered_crossover
-            else:
-                self.valid_parameters = False
-                self.logger.error("Undefined crossover type. \nThe assigned value to the crossover_type ({crossover_type}) parameter does not refer to one of the supported crossover types which are: \n-single_point (for single point crossover)\n-two_points (for two points crossover)\n-uniform (for uniform crossover)\n-scattered (for scattered crossover).\n".format(crossover_type=crossover_type))
-                raise TypeError("Undefined crossover type. \nThe assigned value to the crossover_type ({crossover_type}) parameter does not refer to one of the supported crossover types which are: \n-single_point (for single point crossover)\n-two_points (for two points crossover)\n-uniform (for uniform crossover)\n-scattered (for scattered crossover).\n".format(crossover_type=crossover_type))
-
-        self.crossover_type = crossover_type
-
-        # Calculate the value of crossover_probability
-        if crossover_probability is None:
-            self.crossover_probability = None
-        elif type(crossover_probability) in GA.supported_int_float_types:
-            if crossover_probability >= 0 and crossover_probability <= 1:
-                self.crossover_probability = crossover_probability
+                self.valid_parameters = False
+                raise TypeError(f"The expected type of the 'random_mutation_min_val' parameter is numeric or list/tuple/numpy.ndarray but {type(random_mutation_min_val)} found.")
+
+            self.random_mutation_min_val = random_mutation_min_val
+            self.random_mutation_max_val = random_mutation_max_val
+
+            # Validating the number of parents to be selected for mating (num_parents_mating)
+            if num_parents_mating <= 0:
+                self.valid_parameters = False
+                raise ValueError(f"The number of parents mating (num_parents_mating) parameter must be > 0 but ({num_parents_mating}) found. \nThe following parameters must be > 0: \n1) Population size (i.e. number of solutions per population) (sol_per_pop).\n2) Number of selected parents in the mating pool (num_parents_mating).\n")
+
+            # Validating the number of parents to be selected for mating: num_parents_mating
+            if (num_parents_mating > self.sol_per_pop):
+                self.valid_parameters = False
+                raise ValueError(f"The number of parents to select for mating ({num_parents_mating}) cannot be greater than the number of solutions in the population ({self.sol_per_pop}) (i.e., num_parents_mating must always be <= sol_per_pop).\n")
+
+            self.num_parents_mating = num_parents_mating
+
+            # crossover: Refers to the method that applies the crossover operator based on the selected type of crossover in the crossover_type property.
+            # Validating the crossover type: crossover_type
+            if (crossover_type is None):
+                self.crossover = None
+            elif inspect.ismethod(crossover_type):
+                # Check if the crossover_type is a method that accepts 4 paramaters.
+                if (crossover_type.__code__.co_argcount == 4):
+                    # The crossover method assigned to the crossover_type parameter is validated.
+                    self.crossover = crossover_type
+                else:
+                    self.valid_parameters = False
+                    raise ValueError(f"When 'crossover_type' is assigned to a method, then this crossover method must accept 4 parameters:\n1) Expected to be the 'self' object.\n2) The selected parents.\n3) The size of the offspring to be produced.\n4) The instance from the pygad.GA class.\n\nThe passed crossover method named '{crossover_type.__code__.co_name}' accepts {crossover_type.__code__.co_argcount} parameter(s).")
+            elif callable(crossover_type):
+                # Check if the crossover_type is a function that accepts 2 paramaters.
+                if (crossover_type.__code__.co_argcount == 3):
+                    # The crossover function assigned to the crossover_type parameter is validated.
+                    self.crossover = crossover_type
+                else:
+                    self.valid_parameters = False
+                    raise ValueError(f"When 'crossover_type' is assigned to a function, then this crossover function must accept 3 parameters:\n1) The selected parents.\n2) The size of the offspring to be produced.3) The instance from the pygad.GA class to retrieve any property like population, gene data type, gene space, etc.\n\nThe passed crossover function named '{crossover_type.__code__.co_name}' accepts {crossover_type.__code__.co_argcount} parameter(s).")
+            elif not (type(crossover_type) is str):
+                self.valid_parameters = False
+                raise TypeError(f"The expected type of the 'crossover_type' parameter is either callable or str but {type(crossover_type)} found.")
+            else:  # type crossover_type is str
+                crossover_type = crossover_type.lower()
+                if (crossover_type == "single_point"):
+                    self.crossover = self.single_point_crossover
+                elif (crossover_type == "two_points"):
+                    self.crossover = self.two_points_crossover
+                elif (crossover_type == "uniform"):
+                    self.crossover = self.uniform_crossover
+                elif (crossover_type == "scattered"):
+                    self.crossover = self.scattered_crossover
+                else:
+                    self.valid_parameters = False
+                    raise TypeError(f"Undefined crossover type. \nThe assigned value to the crossover_type ({crossover_type}) parameter does not refer to one of the supported crossover types which are: \n-single_point (for single point crossover)\n-two_points (for two points crossover)\n-uniform (for uniform crossover)\n-scattered (for scattered crossover).\n")
+
+            self.crossover_type = crossover_type
+
+            # Calculate the value of crossover_probability
+            if crossover_probability is None:
+                self.crossover_probability = None
+            elif type(crossover_probability) in GA.supported_int_float_types:
+                if crossover_probability >= 0 and crossover_probability <= 1:
+                    self.crossover_probability = crossover_probability
+                else:
+                    self.valid_parameters = False
+                    raise ValueError(f"The value assigned to the 'crossover_probability' parameter must be between 0 and 1 inclusive but ({crossover_probability}) found.")
             else:
                 self.valid_parameters = False
-                self.logger.error("The value assigned to the 'crossover_probability' parameter must be between 0 and 1 inclusive but ({crossover_probability_value}) found.".format(crossover_probability_value=crossover_probability))
-                raise ValueError("The value assigned to the 'crossover_probability' parameter must be between 0 and 1 inclusive but ({crossover_probability_value}) found.".format(crossover_probability_value=crossover_probability))
-        else:
-            self.valid_parameters = False
-            self.logger.error("Unexpected type for the 'crossover_probability' parameter. Float is expected but ({crossover_probability_value}) of type {crossover_probability_type} found.".format(crossover_probability_value=crossover_probability, crossover_probability_type=type(crossover_probability)))
-            raise TypeError("Unexpected type for the 'crossover_probability' parameter. Float is expected but ({crossover_probability_value}) of type {crossover_probability_type} found.".format(crossover_probability_value=crossover_probability, crossover_probability_type=type(crossover_probability)))
-
-        # mutation: Refers to the method that applies the mutation operator based on the selected type of mutation in the mutation_type property.
-        # Validating the mutation type: mutation_type
-        # "adaptive" mutation is supported starting from PyGAD 2.10.0
-        if mutation_type is None:
-            self.mutation = None
-        elif inspect.ismethod(mutation_type):
-            # Check if the mutation_type is a method that accepts 3 paramater.
-            if (mutation_type.__code__.co_argcount == 3):
-                # The mutation method assigned to the mutation_type parameter is validated.
-                self.mutation = mutation_type
-            else:
-                self.valid_parameters = False
-                self.logger.error("When 'mutation_type' is assigned to a method, then it must accept 3 parameters:\n1) Expected to be the 'self' object.\n2) The offspring to be mutated.\n3) The instance from the pygad.GA class.\n\nThe passed mutation method named '{funcname}' accepts {argcount} parameter(s).".format(funcname=mutation_type.__code__.co_name, argcount=mutation_type.__code__.co_argcount))
-                raise ValueError("When 'mutation_type' is assigned to a method, then it must accept 3 parameters:\n1) Expected to be the 'self' object.\n2) The offspring to be mutated.\n3) The instance from the pygad.GA class.\n\nThe passed mutation method named '{funcname}' accepts {argcount} parameter(s).".format(funcname=mutation_type.__code__.co_name, argcount=mutation_type.__code__.co_argcount))
-        elif callable(mutation_type):
-            # Check if the mutation_type is a function that accepts 2 paramater.
-            if (mutation_type.__code__.co_argcount == 2):
-                # The mutation function assigned to the mutation_type parameter is validated.
-                self.mutation = mutation_type
-            else:
-                self.valid_parameters = False
-                self.logger.error("When 'mutation_type' is assigned to a function, then this mutation function must accept 2 parameters:\n1) The offspring to be mutated.\n2) The instance from the pygad.GA class to retrieve any property like population, gene data type, gene space, etc.\n\nThe passed mutation function named '{funcname}' accepts {argcount} parameter(s).".format(funcname=mutation_type.__code__.co_name, argcount=mutation_type.__code__.co_argcount))
-                raise ValueError("When 'mutation_type' is assigned to a function, then this mutation function must accept 2 parameters:\n1) The offspring to be mutated.\n2) The instance from the pygad.GA class to retrieve any property like population, gene data type, gene space, etc.\n\nThe passed mutation function named '{funcname}' accepts {argcount} parameter(s).".format(funcname=mutation_type.__code__.co_name, argcount=mutation_type.__code__.co_argcount))
-        elif not (type(mutation_type) is str):
-            self.valid_parameters = False
-            self.logger.error("The expected type of the 'mutation_type' parameter is either callable or str but {mutation_type} found.".format(mutation_type=type(mutation_type)))
-            raise TypeError("The expected type of the 'mutation_type' parameter is either callable or str but {mutation_type} found.".format(mutation_type=type(mutation_type)))
-        else: # type mutation_type is str
-            mutation_type = mutation_type.lower()
-            if (mutation_type == "random"):
-                self.mutation = self.random_mutation
-            elif (mutation_type == "swap"):
-                self.mutation = self.swap_mutation
-            elif (mutation_type == "scramble"):
-                self.mutation = self.scramble_mutation
-            elif (mutation_type == "inversion"):
-                self.mutation = self.inversion_mutation
-            elif (mutation_type == "adaptive"):
-                self.mutation = self.adaptive_mutation
-            else:
-                self.valid_parameters = False
-                self.logger.error("Undefined mutation type. \nThe assigned string value to the 'mutation_type' parameter ({mutation_type}) does not refer to one of the supported mutation types which are: \n-random (for random mutation)\n-swap (for swap mutation)\n-inversion (for inversion mutation)\n-scramble (for scramble mutation)\n-adaptive (for adaptive mutation).\n".format(mutation_type=mutation_type))
-                raise TypeError("Undefined mutation type. \nThe assigned string value to the 'mutation_type' parameter ({mutation_type}) does not refer to one of the supported mutation types which are: \n-random (for random mutation)\n-swap (for swap mutation)\n-inversion (for inversion mutation)\n-scramble (for scramble mutation)\n-adaptive (for adaptive mutation).\n".format(mutation_type=mutation_type))
-
-        self.mutation_type = mutation_type
-
-        # Calculate the value of mutation_probability
-        if not (self.mutation_type is None):
-            if mutation_probability is None:
-                self.mutation_probability = None
-            elif (mutation_type != "adaptive"):
-                # Mutation probability is fixed not adaptive.
-                if type(mutation_probability) in GA.supported_int_float_types:
-                    if mutation_probability >= 0 and mutation_probability <= 1:
-                        self.mutation_probability = mutation_probability
-                    else:
-                        self.valid_parameters = False
-                        self.logger.error("The value assigned to the 'mutation_probability' parameter must be between 0 and 1 inclusive but ({mutation_probability_value}) found.".format(mutation_probability_value=mutation_probability))
-                        raise ValueError("The value assigned to the 'mutation_probability' parameter must be between 0 and 1 inclusive but ({mutation_probability_value}) found.".format(mutation_probability_value=mutation_probability))
-                else:
-                    self.valid_parameters = False
-                    self.logger.error("Unexpected type for the 'mutation_probability' parameter. A numeric value is expected but ({mutation_probability_value}) of type {mutation_probability_type} found.".format(mutation_probability_value=mutation_probability, mutation_probability_type=type(mutation_probability)))
-                    raise TypeError("Unexpected type for the 'mutation_probability' parameter. A numeric value is expected but ({mutation_probability_value}) of type {mutation_probability_type} found.".format(mutation_probability_value=mutation_probability, mutation_probability_type=type(mutation_probability)))
-            else:
-                # Mutation probability is adaptive not fixed.
-                if type(mutation_probability) in [list, tuple, numpy.ndarray]:
-                    if len(mutation_probability) == 2:
-                        for el in mutation_probability:
-                            if type(el) in GA.supported_int_float_types:
-                                if el >= 0 and el <= 1:
-                                    pass
-                                else:
-                                    self.valid_parameters = False
-                                    self.logger.error("The values assigned to the 'mutation_probability' parameter must be between 0 and 1 inclusive but ({mutation_probability_value}) found.".format(mutation_probability_value=el))
-                                    raise ValueError("The values assigned to the 'mutation_probability' parameter must be between 0 and 1 inclusive but ({mutation_probability_value}) found.".format(mutation_probability_value=el))
-                            else:
-                                self.valid_parameters = False
-                                self.logger.error("Unexpected type for a value assigned to the 'mutation_probability' parameter. A numeric value is expected but ({mutation_probability_value}) of type {mutation_probability_type} found.".format(mutation_probability_value=el, mutation_probability_type=type(el)))
-                                raise TypeError("Unexpected type for a value assigned to the 'mutation_probability' parameter. A numeric value is expected but ({mutation_probability_value}) of type {mutation_probability_type} found.".format(mutation_probability_value=el, mutation_probability_type=type(el)))
-                        if mutation_probability[0] < mutation_probability[1]:
-                            if not self.suppress_warnings: warnings.warn("The first element in the 'mutation_probability' parameter is {first_el} which is smaller than the second element {second_el}. This means the mutation rate for the high-quality solutions is higher than the mutation rate of the low-quality ones. This causes high disruption in the high qualitiy solutions while making little changes in the low quality solutions. Please make the first element higher than the second element.".format(first_el=mutation_probability[0], second_el=mutation_probability[1]))
-                        self.mutation_probability = mutation_probability
-                    else:
-                        self.valid_parameters = False
-                        self.logger.error("When mutation_type='adaptive', then the 'mutation_probability' parameter must have only 2 elements but ({mutation_probability_length}) element(s) found.".format(mutation_probability_length=len(mutation_probability)))
-                        raise ValueError("When mutation_type='adaptive', then the 'mutation_probability' parameter must have only 2 elements but ({mutation_probability_length}) element(s) found.".format(mutation_probability_length=len(mutation_probability)))
+                raise TypeError(f"Unexpected type for the 'crossover_probability' parameter. Float is expected but ({crossover_probability}) of type {type(crossover_probability)} found.")
+
+            # mutation: Refers to the method that applies the mutation operator based on the selected type of mutation in the mutation_type property.
+            # Validating the mutation type: mutation_type
+            # "adaptive" mutation is supported starting from PyGAD 2.10.0
+            if mutation_type is None:
+                self.mutation = None
+            elif inspect.ismethod(mutation_type):
+                # Check if the mutation_type is a method that accepts 3 paramater.
+                if (mutation_type.__code__.co_argcount == 3):
+                    # The mutation method assigned to the mutation_type parameter is validated.
+                    self.mutation = mutation_type
                 else:
                     self.valid_parameters = False
-                    self.logger.error("Unexpected type for the 'mutation_probability' parameter. When mutation_type='adaptive', then list/tuple/numpy.ndarray is expected but ({mutation_probability_value}) of type {mutation_probability_type} found.".format(mutation_probability_value=mutation_probability, mutation_probability_type=type(mutation_probability)))
-                    raise TypeError("Unexpected type for the 'mutation_probability' parameter. When mutation_type='adaptive', then list/tuple/numpy.ndarray is expected but ({mutation_probability_value}) of type {mutation_probability_type} found.".format(mutation_probability_value=mutation_probability, mutation_probability_type=type(mutation_probability)))
-        else:
-            pass
+                    raise ValueError(f"When 'mutation_type' is assigned to a method, then it must accept 3 parameters:\n1) Expected to be the 'self' object.\n2) The offspring to be mutated.\n3) The instance from the pygad.GA class.\n\nThe passed mutation method named '{mutation_type.__code__.co_name}' accepts {mutation_type.__code__.co_argcount} parameter(s).")
+            elif callable(mutation_type):
+                # Check if the mutation_type is a function that accepts 2 paramater.
+                if (mutation_type.__code__.co_argcount == 2):
+                    # The mutation function assigned to the mutation_type parameter is validated.
+                    self.mutation = mutation_type
+                else:
+                    self.valid_parameters = False
+                    raise ValueError(f"When 'mutation_type' is assigned to a function, then this mutation function must accept 2 parameters:\n1) The offspring to be mutated.\n2) The instance from the pygad.GA class to retrieve any property like population, gene data type, gene space, etc.\n\nThe passed mutation function named '{mutation_type.__code__.co_name}' accepts {mutation_type.__code__.co_argcount} parameter(s).")
+            elif not (type(mutation_type) is str):
+                self.valid_parameters = False
+                raise TypeError(f"The expected type of the 'mutation_type' parameter is either callable or str but {type(mutation_type)} found.")
+            else:  # type mutation_type is str
+                mutation_type = mutation_type.lower()
+                if (mutation_type == "random"):
+                    self.mutation = self.random_mutation
+                elif (mutation_type == "swap"):
+                    self.mutation = self.swap_mutation
+                elif (mutation_type == "scramble"):
+                    self.mutation = self.scramble_mutation
+                elif (mutation_type == "inversion"):
+                    self.mutation = self.inversion_mutation
+                elif (mutation_type == "adaptive"):
+                    self.mutation = self.adaptive_mutation
+                else:
+                    self.valid_parameters = False
+                    raise TypeError(f"Undefined mutation type. \nThe assigned string value to the 'mutation_type' parameter ({mutation_type}) does not refer to one of the supported mutation types which are: \n-random (for random mutation)\n-swap (for swap mutation)\n-inversion (for inversion mutation)\n-scramble (for scramble mutation)\n-adaptive (for adaptive mutation).\n")
 
-        # Calculate the value of mutation_num_genes
-        if not (self.mutation_type is None):
-            if mutation_num_genes is None:
-                # The mutation_num_genes parameter does not exist. Checking whether adaptive mutation is used.
-                if (mutation_type != "adaptive"):
-                    # The percent of genes to mutate is fixed not adaptive.
-                    if mutation_percent_genes == 'default'.lower():
-                        mutation_percent_genes = 10
-                        # Based on the mutation percentage in the 'mutation_percent_genes' parameter, the number of genes to mutate is calculated.
-                        mutation_num_genes = numpy.uint32((mutation_percent_genes*self.num_genes)/100)
-                        # Based on the mutation percentage of genes, if the number of selected genes for mutation is less than the least possible value which is 1, then the number will be set to 1.
-                        if mutation_num_genes == 0:
-                            if self.mutation_probability is None:
-                                if not self.suppress_warnings: warnings.warn("The percentage of genes to mutate (mutation_percent_genes={mutation_percent}) resutled in selecting ({mutation_num}) genes. The number of genes to mutate is set to 1 (mutation_num_genes=1).\nIf you do not want to mutate any gene, please set mutation_type=None.".format(mutation_percent=mutation_percent_genes, mutation_num=mutation_num_genes))
-                            mutation_num_genes = 1
+            self.mutation_type = mutation_type
 
-                    elif type(mutation_percent_genes) in GA.supported_int_float_types:
-                        if (mutation_percent_genes <= 0 or mutation_percent_genes > 100):
+            # Calculate the value of mutation_probability
+            if not (self.mutation_type is None):
+                if mutation_probability is None:
+                    self.mutation_probability = None
+                elif (mutation_type != "adaptive"):
+                    # Mutation probability is fixed not adaptive.
+                    if type(mutation_probability) in GA.supported_int_float_types:
+                        if mutation_probability >= 0 and mutation_probability <= 1:
+                            self.mutation_probability = mutation_probability
+                        else:
                             self.valid_parameters = False
-                            self.logger.error("The percentage of selected genes for mutation (mutation_percent_genes) must be > 0 and <= 100 but ({mutation_percent_genes}) found.\n".format(mutation_percent_genes=mutation_percent_genes))
-                            raise ValueError("The percentage of selected genes for mutation (mutation_percent_genes) must be > 0 and <= 100 but ({mutation_percent_genes}) found.\n".format(mutation_percent_genes=mutation_percent_genes))
+                            raise ValueError(f"The value assigned to the 'mutation_probability' parameter must be between 0 and 1 inclusive but ({mutation_probability}) found.")
+                    else:
+                        self.valid_parameters = False
+                        raise TypeError(f"Unexpected type for the 'mutation_probability' parameter. A numeric value is expected but ({mutation_probability}) of type {type(mutation_probability)} found.")
+                else:
+                    # Mutation probability is adaptive not fixed.
+                    if type(mutation_probability) in [list, tuple, numpy.ndarray]:
+                        if len(mutation_probability) == 2:
+                            for el in mutation_probability:
+                                if type(el) in GA.supported_int_float_types:
+                                    if el >= 0 and el <= 1:
+                                        pass
+                                    else:
+                                        self.valid_parameters = False
+                                        raise ValueError(f"The values assigned to the 'mutation_probability' parameter must be between 0 and 1 inclusive but ({el}) found.")
+                                else:
+                                    self.valid_parameters = False
+                                    raise TypeError(f"Unexpected type for a value assigned to the 'mutation_probability' parameter. A numeric value is expected but ({el}) of type {type(el)} found.")
+                            if mutation_probability[0] < mutation_probability[1]:
+                                if not self.suppress_warnings:
+                                    warnings.warn(f"The first element in the 'mutation_probability' parameter is {mutation_probability[0]} which is smaller than the second element {mutation_probability[1]}. This means the mutation rate for the high-quality solutions is higher than the mutation rate of the low-quality ones. This causes high disruption in the high qualitiy solutions while making little changes in the low quality solutions. Please make the first element higher than the second element.")
+                            self.mutation_probability = mutation_probability
                         else:
-                            # If mutation_percent_genes equals the string "default", then it is replaced by the numeric value 10.
-                            if mutation_percent_genes == 'default'.lower():
-                                mutation_percent_genes = 10
+                            self.valid_parameters = False
+                            raise ValueError(f"When mutation_type='adaptive', then the 'mutation_probability' parameter must have only 2 elements but ({len(mutation_probability)}) element(s) found.")
+                    else:
+                        self.valid_parameters = False
+                        raise TypeError(f"Unexpected type for the 'mutation_probability' parameter. When mutation_type='adaptive', then list/tuple/numpy.ndarray is expected but ({mutation_probability}) of type {type(mutation_probability)} found.")
+            else:
+                pass
 
+            # Calculate the value of mutation_num_genes
+            if not (self.mutation_type is None):
+                if mutation_num_genes is None:
+                    # The mutation_num_genes parameter does not exist. Checking whether adaptive mutation is used.
+                    if (mutation_type != "adaptive"):
+                        # The percent of genes to mutate is fixed not adaptive.
+                        if mutation_percent_genes == 'default'.lower():
+                            mutation_percent_genes = 10
                             # Based on the mutation percentage in the 'mutation_percent_genes' parameter, the number of genes to mutate is calculated.
-                            mutation_num_genes = numpy.uint32((mutation_percent_genes*self.num_genes)/100)
+                            mutation_num_genes = numpy.uint32(
+                                (mutation_percent_genes*self.num_genes)/100)
                             # Based on the mutation percentage of genes, if the number of selected genes for mutation is less than the least possible value which is 1, then the number will be set to 1.
                             if mutation_num_genes == 0:
                                 if self.mutation_probability is None:
-                                    if not self.suppress_warnings: warnings.warn("The percentage of genes to mutate (mutation_percent_genes={mutation_percent}) resutled in selecting ({mutation_num}) genes. The number of genes to mutate is set to 1 (mutation_num_genes=1).\nIf you do not want to mutate any gene, please set mutation_type=None.".format(mutation_percent=mutation_percent_genes, mutation_num=mutation_num_genes))
+                                    if not self.suppress_warnings:
+                                        warnings.warn(
+                                            f"The percentage of genes to mutate (mutation_percent_genes={mutation_percent_genes}) resutled in selecting ({mutation_num_genes}) genes. The number of genes to mutate is set to 1 (mutation_num_genes=1).\nIf you do not want to mutate any gene, please set mutation_type=None.")
                                 mutation_num_genes = 1
+
+                        elif type(mutation_percent_genes) in GA.supported_int_float_types:
+                            if (mutation_percent_genes <= 0 or mutation_percent_genes > 100):
+                                self.valid_parameters = False
+                                raise ValueError(f"The percentage of selected genes for mutation (mutation_percent_genes) must be > 0 and <= 100 but ({mutation_percent_genes}) found.\n")
+                            else:
+                                # If mutation_percent_genes equals the string "default", then it is replaced by the numeric value 10.
+                                if mutation_percent_genes == 'default'.lower():
+                                    mutation_percent_genes = 10
+
+                                # Based on the mutation percentage in the 'mutation_percent_genes' parameter, the number of genes to mutate is calculated.
+                                mutation_num_genes = numpy.uint32(
+                                    (mutation_percent_genes*self.num_genes)/100)
+                                # Based on the mutation percentage of genes, if the number of selected genes for mutation is less than the least possible value which is 1, then the number will be set to 1.
+                                if mutation_num_genes == 0:
+                                    if self.mutation_probability is None:
+                                        if not self.suppress_warnings:
+                                            warnings.warn(f"The percentage of genes to mutate (mutation_percent_genes={mutation_percent_genes}) resutled in selecting ({mutation_num_genes}) genes. The number of genes to mutate is set to 1 (mutation_num_genes=1).\nIf you do not want to mutate any gene, please set mutation_type=None.")
+                                    mutation_num_genes = 1
+                        else:
+                            self.valid_parameters = False
+                            raise TypeError(f"Unexpected value or type of the 'mutation_percent_genes' parameter. It only accepts the string 'default' or a numeric value but ({mutation_percent_genes}) of type {type(mutation_percent_genes)} found.")
+                    else:
+                        # The percent of genes to mutate is adaptive not fixed.
+                        if type(mutation_percent_genes) in [list, tuple, numpy.ndarray]:
+                            if len(mutation_percent_genes) == 2:
+                                mutation_num_genes = numpy.zeros_like(
+                                    mutation_percent_genes, dtype=numpy.uint32)
+                                for idx, el in enumerate(mutation_percent_genes):
+                                    if type(el) in GA.supported_int_float_types:
+                                        if (el <= 0 or el > 100):
+                                            self.valid_parameters = False
+                                            raise ValueError(f"The values assigned to the 'mutation_percent_genes' must be > 0 and <= 100 but ({mutation_percent_genes}) found.\n")
+                                    else:
+                                        self.valid_parameters = False
+                                        raise TypeError(f"Unexpected type for a value assigned to the 'mutation_percent_genes' parameter. An integer value is expected but ({el}) of type {type(el)} found.")
+                                    # At this point of the loop, the current value assigned to the parameter 'mutation_percent_genes' is validated.
+                                    # Based on the mutation percentage in the 'mutation_percent_genes' parameter, the number of genes to mutate is calculated.
+                                    mutation_num_genes[idx] = numpy.uint32(
+                                        (mutation_percent_genes[idx]*self.num_genes)/100)
+                                    # Based on the mutation percentage of genes, if the number of selected genes for mutation is less than the least possible value which is 1, then the number will be set to 1.
+                                    if mutation_num_genes[idx] == 0:
+                                        if not self.suppress_warnings:
+                                            warnings.warn(f"The percentage of genes to mutate ({mutation_percent_genes[idx]}) resutled in selecting ({mutation_num_genes[idx]}) genes. The number of genes to mutate is set to 1 (mutation_num_genes=1).\nIf you do not want to mutate any gene, please set mutation_type=None.")
+                                        mutation_num_genes[idx] = 1
+                                if mutation_percent_genes[0] < mutation_percent_genes[1]:
+                                    if not self.suppress_warnings:
+                                        warnings.warn(f"The first element in the 'mutation_percent_genes' parameter is ({mutation_percent_genes[0]}) which is smaller than the second element ({mutation_percent_genes[1]}).\nThis means the mutation rate for the high-quality solutions is higher than the mutation rate of the low-quality ones. This causes high disruption in the high qualitiy solutions while making little changes in the low quality solutions.\nPlease make the first element higher than the second element.")
+                                # At this point outside the loop, all values of the parameter 'mutation_percent_genes' are validated. Eveyrthing is OK.
+                            else:
+                                self.valid_parameters = False
+                                raise ValueError(f"When mutation_type='adaptive', then the 'mutation_percent_genes' parameter must have only 2 elements but ({len(mutation_percent_genes)}) element(s) found.")
+                        else:
+                            if self.mutation_probability is None:
+                                self.valid_parameters = False
+                                raise TypeError(f"Unexpected type of the 'mutation_percent_genes' parameter. When mutation_type='adaptive', then the 'mutation_percent_genes' parameter should exist and assigned a list/tuple/numpy.ndarray with 2 values but ({mutation_percent_genes}) found.")
+                # The mutation_num_genes parameter exists. Checking whether adaptive mutation is used.
+                elif (mutation_type != "adaptive"):
+                    # Number of genes to mutate is fixed not adaptive.
+                    if type(mutation_num_genes) in GA.supported_int_types:
+                        if (mutation_num_genes <= 0):
+                            self.valid_parameters = False
+                            raise ValueError(f"The number of selected genes for mutation (mutation_num_genes) cannot be <= 0 but ({mutation_num_genes}) found. If you do not want to use mutation, please set mutation_type=None\n")
+                        elif (mutation_num_genes > self.num_genes):
+                            self.valid_parameters = False
+                            raise ValueError(f"The number of selected genes for mutation (mutation_num_genes), which is ({mutation_num_genes}), cannot be greater than the number of genes ({self.num_genes}).\n")
                     else:
                         self.valid_parameters = False
-                        self.logger.error("Unexpected value or type of the 'mutation_percent_genes' parameter. It only accepts the string 'default' or a numeric value but ({mutation_percent_genes_value}) of type {mutation_percent_genes_type} found.".format(mutation_percent_genes_value=mutation_percent_genes, mutation_percent_genes_type=type(mutation_percent_genes)))
-                        raise TypeError("Unexpected value or type of the 'mutation_percent_genes' parameter. It only accepts the string 'default' or a numeric value but ({mutation_percent_genes_value}) of type {mutation_percent_genes_type} found.".format(mutation_percent_genes_value=mutation_percent_genes, mutation_percent_genes_type=type(mutation_percent_genes)))
+                        raise TypeError(f"The 'mutation_num_genes' parameter is expected to be a positive integer but the value ({mutation_num_genes}) of type {type(mutation_num_genes)} found.\n")
                 else:
-                    # The percent of genes to mutate is adaptive not fixed.
-                    if type(mutation_percent_genes) in [list, tuple, numpy.ndarray]:
-                        if len(mutation_percent_genes) == 2:
-                            mutation_num_genes = numpy.zeros_like(mutation_percent_genes, dtype=numpy.uint32)
-                            for idx, el in enumerate(mutation_percent_genes):
-                                if type(el) in GA.supported_int_float_types:
-                                    if (el <= 0 or el > 100):
+                    # Number of genes to mutate is adaptive not fixed.
+                    if type(mutation_num_genes) in [list, tuple, numpy.ndarray]:
+                        if len(mutation_num_genes) == 2:
+                            for el in mutation_num_genes:
+                                if type(el) in GA.supported_int_types:
+                                    if (el <= 0):
                                         self.valid_parameters = False
-                                        self.logger.error("The values assigned to the 'mutation_percent_genes' must be > 0 and <= 100 but ({mutation_percent_genes}) found.\n".format(mutation_percent_genes=mutation_percent_genes))
-                                        raise ValueError("The values assigned to the 'mutation_percent_genes' must be > 0 and <= 100 but ({mutation_percent_genes}) found.\n".format(mutation_percent_genes=mutation_percent_genes))
+                                        raise ValueError(f"The values assigned to the 'mutation_num_genes' cannot be <= 0 but ({el}) found. If you do not want to use mutation, please set mutation_type=None\n")
+                                    elif (el > self.num_genes):
+                                        self.valid_parameters = False
+                                        raise ValueError(f"The values assigned to the 'mutation_num_genes' cannot be greater than the number of genes ({self.num_genes}) but ({el}) found.\n")
                                 else:
                                     self.valid_parameters = False
-                                    self.logger.error("Unexpected type for a value assigned to the 'mutation_percent_genes' parameter. An integer value is expected but ({mutation_percent_genes_value}) of type {mutation_percent_genes_type} found.".format(mutation_percent_genes_value=el, mutation_percent_genes_type=type(el)))
-                                    raise TypeError("Unexpected type for a value assigned to the 'mutation_percent_genes' parameter. An integer value is expected but ({mutation_percent_genes_value}) of type {mutation_percent_genes_type} found.".format(mutation_percent_genes_value=el, mutation_percent_genes_type=type(el)))
-                                # At this point of the loop, the current value assigned to the parameter 'mutation_percent_genes' is validated.
-                                # Based on the mutation percentage in the 'mutation_percent_genes' parameter, the number of genes to mutate is calculated.
-                                mutation_num_genes[idx] = numpy.uint32((mutation_percent_genes[idx]*self.num_genes)/100)
-                                # Based on the mutation percentage of genes, if the number of selected genes for mutation is less than the least possible value which is 1, then the number will be set to 1.
-                                if mutation_num_genes[idx] == 0:
-                                    if not self.suppress_warnings: warnings.warn("The percentage of genes to mutate ({mutation_percent}) resutled in selecting ({mutation_num}) genes. The number of genes to mutate is set to 1 (mutation_num_genes=1).\nIf you do not want to mutate any gene, please set mutation_type=None.".format(mutation_percent=mutation_percent_genes[idx], mutation_num=mutation_num_genes[idx]))
-                                    mutation_num_genes[idx] = 1
-                            if mutation_percent_genes[0] < mutation_percent_genes[1]:
-                                if not self.suppress_warnings: warnings.warn("The first element in the 'mutation_percent_genes' parameter is ({first_el}) which is smaller than the second element ({second_el}).\nThis means the mutation rate for the high-quality solutions is higher than the mutation rate of the low-quality ones. This causes high disruption in the high qualitiy solutions while making little changes in the low quality solutions.\nPlease make the first element higher than the second element.".format(first_el=mutation_percent_genes[0], second_el=mutation_percent_genes[1]))
-                            # At this point outside the loop, all values of the parameter 'mutation_percent_genes' are validated. Eveyrthing is OK.
+                                    raise TypeError(f"Unexpected type for a value assigned to the 'mutation_num_genes' parameter. An integer value is expected but ({el}) of type {type(el)} found.")
+                                # At this point of the loop, the current value assigned to the parameter 'mutation_num_genes' is validated.
+                            if mutation_num_genes[0] < mutation_num_genes[1]:
+                                if not self.suppress_warnings:
+                                    warnings.warn(f"The first element in the 'mutation_num_genes' parameter is {mutation_num_genes[0]} which is smaller than the second element {mutation_num_genes[1]}. This means the mutation rate for the high-quality solutions is higher than the mutation rate of the low-quality ones. This causes high disruption in the high qualitiy solutions while making little changes in the low quality solutions. Please make the first element higher than the second element.")
+                            # At this point outside the loop, all values of the parameter 'mutation_num_genes' are validated. Eveyrthing is OK.
                         else:
                             self.valid_parameters = False
-                            self.logger.error("When mutation_type='adaptive', then the 'mutation_percent_genes' parameter must have only 2 elements but ({mutation_percent_genes_length}) element(s) found.".format(mutation_percent_genes_length=len(mutation_percent_genes)))
-                            raise ValueError("When mutation_type='adaptive', then the 'mutation_percent_genes' parameter must have only 2 elements but ({mutation_percent_genes_length}) element(s) found.".format(mutation_percent_genes_length=len(mutation_percent_genes)))
-                    else:
-                        if self.mutation_probability is None:
-                            self.valid_parameters = False
-                            self.logger.error("Unexpected type of the 'mutation_percent_genes' parameter. When mutation_type='adaptive', then the 'mutation_percent_genes' parameter should exist and assigned a list/tuple/numpy.ndarray with 2 values but ({mutation_percent_genes_value}) found.".format(mutation_percent_genes_value=mutation_percent_genes))
-                            raise TypeError("Unexpected type of the 'mutation_percent_genes' parameter. When mutation_type='adaptive', then the 'mutation_percent_genes' parameter should exist and assigned a list/tuple/numpy.ndarray with 2 values but ({mutation_percent_genes_value}) found.".format(mutation_percent_genes_value=mutation_percent_genes))
-            # The mutation_num_genes parameter exists. Checking whether adaptive mutation is used.
-            elif (mutation_type != "adaptive"):
-                # Number of genes to mutate is fixed not adaptive.
-                if type(mutation_num_genes) in GA.supported_int_types:
-                    if (mutation_num_genes <= 0):
-                        self.valid_parameters = False
-                        self.logger.error("The number of selected genes for mutation (mutation_num_genes) cannot be <= 0 but ({mutation_num_genes}) found. If you do not want to use mutation, please set mutation_type=None\n".format(mutation_num_genes=mutation_num_genes))
-                        raise ValueError("The number of selected genes for mutation (mutation_num_genes) cannot be <= 0 but ({mutation_num_genes}) found. If you do not want to use mutation, please set mutation_type=None\n".format(mutation_num_genes=mutation_num_genes))
-                    elif (mutation_num_genes > self.num_genes):
-                        self.valid_parameters = False
-                        self.logger.error("The number of selected genes for mutation (mutation_num_genes), which is ({mutation_num_genes}), cannot be greater than the number of genes ({num_genes}).\n".format(mutation_num_genes=mutation_num_genes, num_genes=self.num_genes))
-                        raise ValueError("The number of selected genes for mutation (mutation_num_genes), which is ({mutation_num_genes}), cannot be greater than the number of genes ({num_genes}).\n".format(mutation_num_genes=mutation_num_genes, num_genes=self.num_genes))
-                else:
-                    self.valid_parameters = False
-                    self.logger.error("The 'mutation_num_genes' parameter is expected to be a positive integer but the value ({mutation_num_genes_value}) of type {mutation_num_genes_type} found.\n".format(mutation_num_genes_value=mutation_num_genes, mutation_num_genes_type=type(mutation_num_genes)))
-                    raise TypeError("The 'mutation_num_genes' parameter is expected to be a positive integer but the value ({mutation_num_genes_value}) of type {mutation_num_genes_type} found.\n".format(mutation_num_genes_value=mutation_num_genes, mutation_num_genes_type=type(mutation_num_genes)))
-            else:
-                # Number of genes to mutate is adaptive not fixed.
-                if type(mutation_num_genes) in [list, tuple, numpy.ndarray]:
-                    if len(mutation_num_genes) == 2:
-                        for el in mutation_num_genes:
-                            if type(el) in GA.supported_int_types:
-                                if (el <= 0):
-                                    self.valid_parameters = False
-                                    self.logger.error("The values assigned to the 'mutation_num_genes' cannot be <= 0 but ({mutation_num_genes_value}) found. If you do not want to use mutation, please set mutation_type=None\n".format(mutation_num_genes_value=el))
-                                    raise ValueError("The values assigned to the 'mutation_num_genes' cannot be <= 0 but ({mutation_num_genes_value}) found. If you do not want to use mutation, please set mutation_type=None\n".format(mutation_num_genes_value=el))
-                                elif (el > self.num_genes):
-                                    self.valid_parameters = False
-                                    self.logger.error("The values assigned to the 'mutation_num_genes' cannot be greater than the number of genes ({num_genes}) but ({mutation_num_genes_value}) found.\n".format(mutation_num_genes_value=el, num_genes=self.num_genes))
-                                    raise ValueError("The values assigned to the 'mutation_num_genes' cannot be greater than the number of genes ({num_genes}) but ({mutation_num_genes_value}) found.\n".format(mutation_num_genes_value=el, num_genes=self.num_genes))
-                            else:
-                                self.valid_parameters = False
-                                self.logger.error("Unexpected type for a value assigned to the 'mutation_num_genes' parameter. An integer value is expected but ({mutation_num_genes_value}) of type {mutation_num_genes_type} found.".format(mutation_num_genes_value=el, mutation_num_genes_type=type(el)))
-                                raise TypeError("Unexpected type for a value assigned to the 'mutation_num_genes' parameter. An integer value is expected but ({mutation_num_genes_value}) of type {mutation_num_genes_type} found.".format(mutation_num_genes_value=el, mutation_num_genes_type=type(el)))
-                            # At this point of the loop, the current value assigned to the parameter 'mutation_num_genes' is validated.
-                        if mutation_num_genes[0] < mutation_num_genes[1]:
-                            if not self.suppress_warnings: warnings.warn("The first element in the 'mutation_num_genes' parameter is {first_el} which is smaller than the second element {second_el}. This means the mutation rate for the high-quality solutions is higher than the mutation rate of the low-quality ones. This causes high disruption in the high qualitiy solutions while making little changes in the low quality solutions. Please make the first element higher than the second element.".format(first_el=mutation_num_genes[0], second_el=mutation_num_genes[1]))
-                        # At this point outside the loop, all values of the parameter 'mutation_num_genes' are validated. Eveyrthing is OK.
+                            raise ValueError(f"When mutation_type='adaptive', then the 'mutation_num_genes' parameter must have only 2 elements but ({len(mutation_num_genes)}) element(s) found.")
                     else:
                         self.valid_parameters = False
-                        self.logger.error("When mutation_type='adaptive', then the 'mutation_num_genes' parameter must have only 2 elements but ({mutation_num_genes_length}) element(s) found.".format(mutation_num_genes_length=len(mutation_num_genes)))
-                        raise ValueError("When mutation_type='adaptive', then the 'mutation_num_genes' parameter must have only 2 elements but ({mutation_num_genes_length}) element(s) found.".format(mutation_num_genes_length=len(mutation_num_genes)))
+                        raise TypeError(f"Unexpected type for the 'mutation_num_genes' parameter. When mutation_type='adaptive', then list/tuple/numpy.ndarray is expected but ({mutation_num_genes}) of type {type(mutation_num_genes)} found.")
+            else:
+                pass
+
+            # Validating mutation_by_replacement and mutation_type
+            if self.mutation_type != "random" and self.mutation_by_replacement:
+                if not self.suppress_warnings:
+                    warnings.warn(f"The mutation_by_replacement parameter is set to True while the mutation_type parameter is not set to random but ({mutation_type}). Note that the mutation_by_replacement parameter has an effect only when mutation_type='random'.")
+
+            # Check if crossover and mutation are both disabled.
+            if (self.mutation_type is None) and (self.crossover_type is None):
+                if not self.suppress_warnings:
+                    warnings.warn("The 2 parameters mutation_type and crossover_type are None. This disables any type of evolution the genetic algorithm can make. As a result, the genetic algorithm cannot find a better solution that the best solution in the initial population.")
+
+            # select_parents: Refers to a method that selects the parents based on the parent selection type specified in the parent_selection_type attribute.
+            # Validating the selected type of parent selection: parent_selection_type
+            if inspect.ismethod(parent_selection_type):
+                # Check if the parent_selection_type is a method that accepts 4 paramaters.
+                if (parent_selection_type.__code__.co_argcount == 4):
+                    # population: Added in PyGAD 2.16.0. It should used only to support custom parent selection functions. Otherwise, it should be left to None to retirve the population by self.population.
+                    # The parent selection method assigned to the parent_selection_type parameter is validated.
+                    self.select_parents = parent_selection_type
+                else:
+                    self.valid_parameters = False
+                    raise ValueError(f"When 'parent_selection_type' is assigned to a method, then it must accept 4 parameters:\n1) Expected to be the 'self' object.\n2) The fitness values of the current population.\n3) The number of parents needed.\n4) The instance from the pygad.GA class.\n\nThe passed parent selection method named '{parent_selection_type.__code__.co_name}' accepts {parent_selection_type.__code__.co_argcount} parameter(s).")
+            elif callable(parent_selection_type):
+                # Check if the parent_selection_type is a function that accepts 3 paramaters.
+                if (parent_selection_type.__code__.co_argcount == 3):
+                    # population: Added in PyGAD 2.16.0. It should used only to support custom parent selection functions. Otherwise, it should be left to None to retirve the population by self.population.
+                    # The parent selection function assigned to the parent_selection_type parameter is validated.
+                    self.select_parents = parent_selection_type
                 else:
                     self.valid_parameters = False
-                    self.logger.error("Unexpected type for the 'mutation_num_genes' parameter. When mutation_type='adaptive', then list/tuple/numpy.ndarray is expected but ({mutation_num_genes_value}) of type {mutation_num_genes_type} found.".format(mutation_num_genes_value=mutation_num_genes, mutation_num_genes_type=type(mutation_num_genes)))
-                    raise TypeError("Unexpected type for the 'mutation_num_genes' parameter. When mutation_type='adaptive', then list/tuple/numpy.ndarray is expected but ({mutation_num_genes_value}) of type {mutation_num_genes_type} found.".format(mutation_num_genes_value=mutation_num_genes, mutation_num_genes_type=type(mutation_num_genes)))
-        else:
-            pass
-        
-        # Validating mutation_by_replacement and mutation_type
-        if self.mutation_type != "random" and self.mutation_by_replacement:
-            if not self.suppress_warnings: warnings.warn("The mutation_by_replacement parameter is set to True while the mutation_type parameter is not set to random but ({mut_type}). Note that the mutation_by_replacement parameter has an effect only when mutation_type='random'.".format(mut_type=mutation_type))
-
-        # Check if crossover and mutation are both disabled.
-        if (self.mutation_type is None) and (self.crossover_type is None):
-            if not self.suppress_warnings: warnings.warn("The 2 parameters mutation_type and crossover_type are None. This disables any type of evolution the genetic algorithm can make. As a result, the genetic algorithm cannot find a better solution that the best solution in the initial population.")
-
-        # select_parents: Refers to a method that selects the parents based on the parent selection type specified in the parent_selection_type attribute.
-        # Validating the selected type of parent selection: parent_selection_type
-        if inspect.ismethod(parent_selection_type):
-            # Check if the parent_selection_type is a method that accepts 4 paramaters.
-            if (parent_selection_type.__code__.co_argcount == 4):
-                # population: Added in PyGAD 2.16.0. It should used only to support custom parent selection functions. Otherwise, it should be left to None to retirve the population by self.population.
-                # The parent selection method assigned to the parent_selection_type parameter is validated.
-                self.select_parents = parent_selection_type
-            else:
-                self.valid_parameters = False
-                self.logger.error("When 'parent_selection_type' is assigned to a method, then it must accept 4 parameters:\n1) Expected to be the 'self' object.\n2) The fitness values of the current population.\n3) The number of parents needed.\n4) The instance from the pygad.GA class.\n\nThe passed parent selection method named '{funcname}' accepts {argcount} parameter(s).".format(funcname=parent_selection_type.__code__.co_name, argcount=parent_selection_type.__code__.co_argcount))
-                raise ValueError("When 'parent_selection_type' is assigned to a method, then it must accept 4 parameters:\n1) Expected to be the 'self' object.\n2) The fitness values of the current population.\n3) The number of parents needed.\n4) The instance from the pygad.GA class.\n\nThe passed parent selection method named '{funcname}' accepts {argcount} parameter(s).".format(funcname=parent_selection_type.__code__.co_name, argcount=parent_selection_type.__code__.co_argcount))
-        elif callable(parent_selection_type):
-            # Check if the parent_selection_type is a function that accepts 3 paramaters.
-            if (parent_selection_type.__code__.co_argcount == 3):
-                # population: Added in PyGAD 2.16.0. It should used only to support custom parent selection functions. Otherwise, it should be left to None to retirve the population by self.population.
-                # The parent selection function assigned to the parent_selection_type parameter is validated.
-                self.select_parents = parent_selection_type
-            else:
-                self.valid_parameters = False
-                self.logger.error("When 'parent_selection_type' is assigned to a user-defined function, then this parent selection function must accept 3 parameters:\n1) The fitness values of the current population.\n2) The number of parents needed.\n3) The instance from the pygad.GA class to retrieve any property like population, gene data type, gene space, etc.\n\nThe passed parent selection function named '{funcname}' accepts {argcount} parameter(s).".format(funcname=parent_selection_type.__code__.co_name, argcount=parent_selection_type.__code__.co_argcount))
-                raise ValueError("When 'parent_selection_type' is assigned to a user-defined function, then this parent selection function must accept 3 parameters:\n1) The fitness values of the current population.\n2) The number of parents needed.\n3) The instance from the pygad.GA class to retrieve any property like population, gene data type, gene space, etc.\n\nThe passed parent selection function named '{funcname}' accepts {argcount} parameter(s).".format(funcname=parent_selection_type.__code__.co_name, argcount=parent_selection_type.__code__.co_argcount))
-        elif not (type(parent_selection_type) is str):
-            self.valid_parameters = False
-            self.logger.error("The expected type of the 'parent_selection_type' parameter is either callable or str but {parent_selection_type} found.".format(parent_selection_type=type(parent_selection_type)))
-            raise TypeError("The expected type of the 'parent_selection_type' parameter is either callable or str but {parent_selection_type} found.".format(parent_selection_type=type(parent_selection_type)))
-        else:
-            parent_selection_type = parent_selection_type.lower()
-            if (parent_selection_type == "sss"):
-                self.select_parents = self.steady_state_selection
-            elif (parent_selection_type == "rws"):
-                self.select_parents = self.roulette_wheel_selection
-            elif (parent_selection_type == "sus"):
-                self.select_parents = self.stochastic_universal_selection
-            elif (parent_selection_type == "random"):
-                self.select_parents = self.random_selection
-            elif (parent_selection_type == "tournament"):
-                self.select_parents = self.tournament_selection
-            elif (parent_selection_type == "rank"):
-                self.select_parents = self.rank_selection
-            else:
-                self.valid_parameters = False
-                self.logger.error("Undefined parent selection type: {parent_selection_type}. \nThe assigned value to the 'parent_selection_type' parameter does not refer to one of the supported parent selection techniques which are: \n-sss (for steady state selection)\n-rws (for roulette wheel selection)\n-sus (for stochastic universal selection)\n-rank (for rank selection)\n-random (for random selection)\n-tournament (for tournament selection).\n".format(parent_selection_type=parent_selection_type))
-                raise TypeError("Undefined parent selection type: {parent_selection_type}. \nThe assigned value to the 'parent_selection_type' parameter does not refer to one of the supported parent selection techniques which are: \n-sss (for steady state selection)\n-rws (for roulette wheel selection)\n-sus (for stochastic universal selection)\n-rank (for rank selection)\n-random (for random selection)\n-tournament (for tournament selection).\n".format(parent_selection_type=parent_selection_type))
-
-        # For tournament selection, validate the K value.
-        if(parent_selection_type == "tournament"):
-            if (K_tournament > self.sol_per_pop):
-                K_tournament = self.sol_per_pop
-                if not self.suppress_warnings: warnings.warn("K of the tournament selection ({K_tournament}) should not be greater than the number of solutions within the population ({sol_per_pop}).\nK will be clipped to be equal to the number of solutions in the population (sol_per_pop).\n".format(K_tournament=K_tournament, sol_per_pop=self.sol_per_pop))
-            elif (K_tournament <= 0):
-                self.valid_parameters = False
-                self.logger.error("K of the tournament selection cannot be <=0 but ({K_tournament}) found.\n".format(K_tournament=K_tournament))
-                raise ValueError("K of the tournament selection cannot be <=0 but ({K_tournament}) found.\n".format(K_tournament=K_tournament))
-
-        self.K_tournament = K_tournament
-
-        # Validating the number of parents to keep in the next population: keep_parents
-        if not (type(keep_parents) in GA.supported_int_types):
-            self.valid_parameters = False
-            self.logger.error("Incorrect type of the value assigned to the keep_parents parameter. The value ({keep_parents}) of type {keep_parents_type} found but an integer is expected.".format(keep_parents=keep_parents, keep_parents_type=type(keep_parents)))
-            raise TypeError("Incorrect type of the value assigned to the keep_parents parameter. The value ({keep_parents}) of type {keep_parents_type} found but an integer is expected.".format(keep_parents=keep_parents, keep_parents_type=type(keep_parents)))
-        elif (keep_parents > self.sol_per_pop or keep_parents > self.num_parents_mating or keep_parents < -1):
-            self.valid_parameters = False
-            self.logger.error("Incorrect value to the keep_parents parameter: {keep_parents}. \nThe assigned value to the keep_parent parameter must satisfy the following conditions: \n1) Less than or equal to sol_per_pop\n2) Less than or equal to num_parents_mating\n3) Greater than or equal to -1.".format(keep_parents=keep_parents))
-            raise ValueError("Incorrect value to the keep_parents parameter: {keep_parents}. \nThe assigned value to the keep_parent parameter must satisfy the following conditions: \n1) Less than or equal to sol_per_pop\n2) Less than or equal to num_parents_mating\n3) Greater than or equal to -1.".format(keep_parents=keep_parents))
-
-        self.keep_parents = keep_parents
-
-        if parent_selection_type == "sss" and self.keep_parents == 0:
-            if not self.suppress_warnings: warnings.warn("The steady-state parent (sss) selection operator is used despite that no parents are kept in the next generation.")
-
-        # Validating the number of elitism to keep in the next population: keep_elitism
-        if not (type(keep_elitism) in GA.supported_int_types):
-            self.valid_parameters = False
-            self.logger.error("Incorrect type of the value assigned to the keep_elitism parameter. The value ({keep_elitism}) of type {keep_elitism_type} found but an integer is expected.".format(keep_elitism=keep_elitism, keep_elitism_type=type(keep_elitism)))
-            raise TypeError("Incorrect type of the value assigned to the keep_elitism parameter. The value ({keep_elitism}) of type {keep_elitism_type} found but an integer is expected.".format(keep_elitism=keep_elitism, keep_elitism_type=type(keep_elitism)))
-        elif (keep_elitism > self.sol_per_pop or keep_elitism < 0):
-            self.valid_parameters = False
-            self.logger.error("Incorrect value to the keep_elitism parameter: {keep_elitism}. \nThe assigned value to the keep_elitism parameter must satisfy the following conditions: \n1) Less than or equal to sol_per_pop\n2) Greater than or equal to 0.".format(keep_elitism=keep_elitism))
-            raise ValueError("Incorrect value to the keep_elitism parameter: {keep_elitism}. \nThe assigned value to the keep_elitism parameter must satisfy the following conditions: \n1) Less than or equal to sol_per_pop\n2) Greater than or equal to 0.".format(keep_elitism=keep_elitism))
-
-        self.keep_elitism = keep_elitism
-
-        # Validate keep_parents.
-        if self.keep_elitism == 0:
-            if (self.keep_parents == -1): # Keep all parents in the next population.
-                self.num_offspring = self.sol_per_pop - self.num_parents_mating
-            elif (self.keep_parents == 0): # Keep no parents in the next population.
-                self.num_offspring = self.sol_per_pop
-            elif (self.keep_parents > 0): # Keep the specified number of parents in the next population.
-                self.num_offspring = self.sol_per_pop - self.keep_parents
-        else:
-            self.num_offspring = self.sol_per_pop - self.keep_elitism
-
-        # Check if the fitness_func is a method.
-        # In PyGAD 2.19.0, a method can be passed to the fitness function. If function is passed, then it accepts 2 parameters. If method, then it accepts 3 parameters.
-        # In PyGAD 2.20.0, a new parameter is passed referring to the instance of the `pygad.GA` class. So, the function accepts 3 parameters and the method accepts 4 parameters.
-        if inspect.ismethod(fitness_func):
-            # If the fitness is calculated through a method, not a function, then there is a fourth 'self` paramaters.
-            if (fitness_func.__code__.co_argcount == 4):
-                self.fitness_func = fitness_func
-            else:
-                self.valid_parameters = False
-                self.logger.error("In PyGAD 2.20.0, if a method is used to calculate the fitness value, then it must accept 4 parameters\n1) Expected to be the 'self' object.\n2) The instance of the 'pygad.GA' class.\n3) A solution to calculate its fitness value.\n4) The solution's index within the population.\n\nThe passed fitness method named '{funcname}' accepts {argcount} parameter(s).".format(funcname=fitness_func.__code__.co_name, argcount=fitness_func.__code__.co_argcount))
-                raise ValueError("In PyGAD 2.20.0, if a method is used to calculate the fitness value, then it must accept 4 parameters\n1) Expected to be the 'self' object.\n2) The instance of the 'pygad.GA' class.\n3) A solution to calculate its fitness value.\n4) The solution's index within the population.\n\nThe passed fitness method named '{funcname}' accepts {argcount} parameter(s).".format(funcname=fitness_func.__code__.co_name, argcount=fitness_func.__code__.co_argcount))
-        elif callable(fitness_func):
-            # Check if the fitness function accepts 2 paramaters.
-            if (fitness_func.__code__.co_argcount == 3):
-                self.fitness_func = fitness_func
-            else:
+                    raise ValueError(f"When 'parent_selection_type' is assigned to a user-defined function, then this parent selection function must accept 3 parameters:\n1) The fitness values of the current population.\n2) The number of parents needed.\n3) The instance from the pygad.GA class to retrieve any property like population, gene data type, gene space, etc.\n\nThe passed parent selection function named '{parent_selection_type.__code__.co_name}' accepts {parent_selection_type.__code__.co_argcount} parameter(s).")
+            elif not (type(parent_selection_type) is str):
                 self.valid_parameters = False
-                self.logger.error("In PyGAD 2.20.0, the fitness function must accept 3 parameters:\n1) The instance of the 'pygad.GA' class.\n2) A solution to calculate its fitness value.\n3) The solution's index within the population.\n\nThe passed fitness function named '{funcname}' accepts {argcount} parameter(s).".format(funcname=fitness_func.__code__.co_name, argcount=fitness_func.__code__.co_argcount))
-                raise ValueError("In PyGAD 2.20.0, the fitness function must accept 3 parameters:\n1) The instance of the 'pygad.GA' class.\n2) A solution to calculate its fitness value.\n3) The solution's index within the population.\n\nThe passed fitness function named '{funcname}' accepts {argcount} parameter(s).".format(funcname=fitness_func.__code__.co_name, argcount=fitness_func.__code__.co_argcount))
-        else:
-            self.valid_parameters = False
-            self.logger.error("The value assigned to the fitness_func parameter is expected to be of type function but {fitness_func_type} found.".format(fitness_func_type=type(fitness_func)))
-            raise TypeError("The value assigned to the fitness_func parameter is expected to be of type function but {fitness_func_type} found.".format(fitness_func_type=type(fitness_func)))
-        
-        if fitness_batch_size is None:
-            pass
-        elif not (type(fitness_batch_size) in GA.supported_int_types):
-            self.valid_parameters = False
-            self.logger.error("The value assigned to the fitness_batch_size parameter is expected to be integer but the value ({fitness_batch_size}) of type {fitness_batch_size_type} found.".format(fitness_batch_size=fitness_batch_size, fitness_batch_size_type=type(fitness_batch_size)))
-            raise TypeError("The value assigned to the fitness_batch_size parameter is expected to be integer but the value ({fitness_batch_size}) of type {fitness_batch_size_type} found.".format(fitness_batch_size=fitness_batch_size, fitness_batch_size_type=type(fitness_batch_size)))
-        elif fitness_batch_size <= 0 or fitness_batch_size > self.sol_per_pop:
-            self.valid_parameters = False
-            self.logger.error("The value assigned to the fitness_batch_size parameter must be:\n1) Greater than 0.\n2) Less than or equal to sol_per_pop ({sol_per_pop}).\nBut the value ({fitness_batch_size}) found.".format(fitness_batch_size=fitness_batch_size, sol_per_pop=self.sol_per_pop))
-            raise ValueError("The value assigned to the fitness_batch_size parameter must be:\n1) Greater than 0.\n2) Less than or equal to sol_per_pop ({sol_per_pop}).\nBut the value ({fitness_batch_size}) found.".format(fitness_batch_size=fitness_batch_size, sol_per_pop=self.sol_per_pop))
-
-        self.fitness_batch_size = fitness_batch_size
-
-        # Check if the on_start exists.
-        if not (on_start is None):
-            if inspect.ismethod(on_start):
-                # Check if the on_start method accepts 2 paramaters.
-                if (on_start.__code__.co_argcount == 2):
-                    self.on_start = on_start
-                else:
-                    self.valid_parameters = False
-                    self.logger.error("The method assigned to the on_start parameter must accept only 2 parameters:\n1) Expected to be the 'self' object.\n2) The instance of the genetic algorithm.\nThe passed method named '{funcname}' accepts {argcount} parameter(s).".format(funcname=on_start.__code__.co_name, argcount=on_start.__code__.co_argcount))
-                    raise ValueError("The method assigned to the on_start parameter must accept only 2 parameters:\n1) Expected to be the 'self' object.\n2) The instance of the genetic algorithm.\nThe passed method named '{funcname}' accepts {argcount} parameter(s).".format(funcname=on_start.__code__.co_name, argcount=on_start.__code__.co_argcount))
-            # Check if the on_start is a function.
-            elif callable(on_start):
-                # Check if the on_start function accepts only a single paramater.
-                if (on_start.__code__.co_argcount == 1):
-                    self.on_start = on_start
+                
+                raise TypeError(f"The expected type of the 'parent_selection_type' parameter is either callable or str but {type(parent_selection_type)} found.")
+            else:
+                parent_selection_type = parent_selection_type.lower()
+                if (parent_selection_type == "sss"):
+                    self.select_parents = self.steady_state_selection
+                elif (parent_selection_type == "rws"):
+                    self.select_parents = self.roulette_wheel_selection
+                elif (parent_selection_type == "sus"):
+                    self.select_parents = self.stochastic_universal_selection
+                elif (parent_selection_type == "random"):
+                    self.select_parents = self.random_selection
+                elif (parent_selection_type == "tournament"):
+                    self.select_parents = self.tournament_selection
+                elif (parent_selection_type == "rank"):
+                    self.select_parents = self.rank_selection
                 else:
                     self.valid_parameters = False
-                    self.logger.error("The function assigned to the on_start parameter must accept only 1 parameter representing the instance of the genetic algorithm.\nThe passed function named '{funcname}' accepts {argcount} parameter(s).".format(funcname=on_start.__code__.co_name, argcount=on_start.__code__.co_argcount))
-                    raise ValueError("The function assigned to the on_start parameter must accept only 1 parameter representing the instance of the genetic algorithm.\nThe passed function named '{funcname}' accepts {argcount} parameter(s).".format(funcname=on_start.__code__.co_name, argcount=on_start.__code__.co_argcount))
-            else:
+                    raise TypeError(f"Undefined parent selection type: {parent_selection_type}. \nThe assigned value to the 'parent_selection_type' parameter does not refer to one of the supported parent selection techniques which are: \n-sss (for steady state selection)\n-rws (for roulette wheel selection)\n-sus (for stochastic universal selection)\n-rank (for rank selection)\n-random (for random selection)\n-tournament (for tournament selection).\n")
+
+            # For tournament selection, validate the K value.
+            if (parent_selection_type == "tournament"):
+                if (K_tournament > self.sol_per_pop):
+                    K_tournament = self.sol_per_pop
+                    if not self.suppress_warnings:
+                        warnings.warn(f"K of the tournament selection ({K_tournament}) should not be greater than the number of solutions within the population ({self.sol_per_pop}).\nK will be clipped to be equal to the number of solutions in the population (sol_per_pop).\n")
+                elif (K_tournament <= 0):
+                    self.valid_parameters = False
+                    raise ValueError(f"K of the tournament selection cannot be <=0 but ({K_tournament}) found.\n")
+
+            self.K_tournament = K_tournament
+
+            # Validating the number of parents to keep in the next population: keep_parents
+            if not (type(keep_parents) in GA.supported_int_types):
                 self.valid_parameters = False
-                self.logger.error("The value assigned to the on_start parameter is expected to be of type function but {on_start_type} found.".format(on_start_type=type(on_start)))
-                raise TypeError("The value assigned to the on_start parameter is expected to be of type function but {on_start_type} found.".format(on_start_type=type(on_start)))
-        else:
-            self.on_start = None
+                raise TypeError(f"Incorrect type of the value assigned to the keep_parents parameter. The value ({keep_parents}) of type {type(keep_parents)} found but an integer is expected.")
+            elif (keep_parents > self.sol_per_pop or keep_parents > self.num_parents_mating or keep_parents < -1):
+                self.valid_parameters = False
+                raise ValueError(f"Incorrect value to the keep_parents parameter: {keep_parents}. \nThe assigned value to the keep_parent parameter must satisfy the following conditions: \n1) Less than or equal to sol_per_pop\n2) Less than or equal to num_parents_mating\n3) Greater than or equal to -1.")
 
-        # Check if the on_fitness exists.
-        if not (on_fitness is None):
-            # Check if the on_fitness is a method.
-            if inspect.ismethod(on_fitness):
-                # Check if the on_fitness method accepts 3 paramaters.
-                if (on_fitness.__code__.co_argcount == 3):
-                    self.on_fitness = on_fitness
+            self.keep_parents = keep_parents
+
+            if parent_selection_type == "sss" and self.keep_parents == 0:
+                if not self.suppress_warnings:
+                    warnings.warn("The steady-state parent (sss) selection operator is used despite that no parents are kept in the next generation.")
+
+            # Validating the number of elitism to keep in the next population: keep_elitism
+            if not (type(keep_elitism) in GA.supported_int_types):
+                self.valid_parameters = False
+                raise TypeError(f"Incorrect type of the value assigned to the keep_elitism parameter. The value ({keep_elitism}) of type {type(keep_elitism)} found but an integer is expected.")
+            elif (keep_elitism > self.sol_per_pop or keep_elitism < 0):
+                self.valid_parameters = False
+                raise ValueError(f"Incorrect value to the keep_elitism parameter: {keep_elitism}. \nThe assigned value to the keep_elitism parameter must satisfy the following conditions: \n1) Less than or equal to sol_per_pop\n2) Greater than or equal to 0.")
+
+            self.keep_elitism = keep_elitism
+
+            # Validate keep_parents.
+            if self.keep_elitism == 0:
+                # Keep all parents in the next population.
+                if (self.keep_parents == -1):
+                    self.num_offspring = self.sol_per_pop - self.num_parents_mating
+                # Keep no parents in the next population.
+                elif (self.keep_parents == 0):
+                    self.num_offspring = self.sol_per_pop
+                # Keep the specified number of parents in the next population.
+                elif (self.keep_parents > 0):
+                    self.num_offspring = self.sol_per_pop - self.keep_parents
+            else:
+                self.num_offspring = self.sol_per_pop - self.keep_elitism
+
+            # Check if the fitness_func is a method.
+            # In PyGAD 2.19.0, a method can be passed to the fitness function. If function is passed, then it accepts 2 parameters. If method, then it accepts 3 parameters.
+            # In PyGAD 2.20.0, a new parameter is passed referring to the instance of the `pygad.GA` class. So, the function accepts 3 parameters and the method accepts 4 parameters.
+            if inspect.ismethod(fitness_func):
+                # If the fitness is calculated through a method, not a function, then there is a fourth 'self` paramaters.
+                if (fitness_func.__code__.co_argcount == 4):
+                    self.fitness_func = fitness_func
                 else:
                     self.valid_parameters = False
-                    self.logger.error("The method assigned to the on_fitness parameter must accept 3 parameters:\n1) Expected to be the 'self' object.\n2) The instance of the genetic algorithm.3) The fitness values of all solutions.\nThe passed method named '{funcname}' accepts {argcount} parameter(s).".format(funcname=on_fitness.__code__.co_name, argcount=on_fitness.__code__.co_argcount))
-                    raise ValueError("The method assigned to the on_fitness parameter must accept 3 parameters:\n1) Expected to be the 'self' object.\n2) The instance of the genetic algorithm.3) The fitness values of all solutions.\nThe passed method named '{funcname}' accepts {argcount} parameter(s).".format(funcname=on_fitness.__code__.co_name, argcount=on_fitness.__code__.co_argcount))
-            # Check if the on_fitness is a function.
-            elif callable(on_fitness):
-                # Check if the on_fitness function accepts 2 paramaters.
-                if (on_fitness.__code__.co_argcount == 2):
-                    self.on_fitness = on_fitness
+                    raise ValueError(f"In PyGAD 2.20.0, if a method is used to calculate the fitness value, then it must accept 4 parameters\n1) Expected to be the 'self' object.\n2) The instance of the 'pygad.GA' class.\n3) A solution to calculate its fitness value.\n4) The solution's index within the population.\n\nThe passed fitness method named '{fitness_func.__code__.co_name}' accepts {fitness_func.__code__.co_argcount} parameter(s).")
+            elif callable(fitness_func):
+                # Check if the fitness function accepts 2 paramaters.
+                if (fitness_func.__code__.co_argcount == 3):
+                    self.fitness_func = fitness_func
                 else:
                     self.valid_parameters = False
-                    self.logger.error("The function assigned to the on_fitness parameter must accept 2 parameters representing the instance of the genetic algorithm and the fitness values of all solutions.\nThe passed function named '{funcname}' accepts {argcount} parameter(s).".format(funcname=on_fitness.__code__.co_name, argcount=on_fitness.__code__.co_argcount))
-                    raise ValueError("The function assigned to the on_fitness parameter must accept 2 parameters representing the instance of the genetic algorithm and the fitness values of all solutions.\nThe passed function named '{funcname}' accepts {argcount} parameter(s).".format(funcname=on_fitness.__code__.co_name, argcount=on_fitness.__code__.co_argcount))
+                    raise ValueError(f"In PyGAD 2.20.0, the fitness function must accept 3 parameters:\n1) The instance of the 'pygad.GA' class.\n2) A solution to calculate its fitness value.\n3) The solution's index within the population.\n\nThe passed fitness function named '{fitness_func.__code__.co_name}' accepts {fitness_func.__code__.co_argcount} parameter(s).")
             else:
                 self.valid_parameters = False
-                self.logger.error("The value assigned to the on_fitness parameter is expected to be of type function but {on_fitness_type} found.".format(on_fitness_type=type(on_fitness)))
-                raise TypeError("The value assigned to the on_fitness parameter is expected to be of type function but {on_fitness_type} found.".format(on_fitness_type=type(on_fitness)))
-        else:
-            self.on_fitness = None
+                
+                raise TypeError(f"The value assigned to the fitness_func parameter is expected to be of type function but {type(fitness_func)} found.")
+
+            if fitness_batch_size is None:
+                pass
+            elif not (type(fitness_batch_size) in GA.supported_int_types):
+                self.valid_parameters = False
+                raise TypeError(f"The value assigned to the fitness_batch_size parameter is expected to be integer but the value ({fitness_batch_size}) of type {type(fitness_batch_size)} found.")
+            elif fitness_batch_size <= 0 or fitness_batch_size > self.sol_per_pop:
+                self.valid_parameters = False
+                raise ValueError(f"The value assigned to the fitness_batch_size parameter must be:\n1) Greater than 0.\n2) Less than or equal to sol_per_pop ({self.sol_per_pop}).\nBut the value ({fitness_batch_size}) found.")
 
-        # Check if the on_parents exists.
-        if not (on_parents is None):
-            # Check if the on_parents is a method.
-            if inspect.ismethod(on_parents):
-                # Check if the on_parents method accepts 3 paramaters.
-                if (on_parents.__code__.co_argcount == 3):
-                    self.on_parents = on_parents
+            self.fitness_batch_size = fitness_batch_size
+
+            # Check if the on_start exists.
+            if not (on_start is None):
+                if inspect.ismethod(on_start):
+                    # Check if the on_start method accepts 2 paramaters.
+                    if (on_start.__code__.co_argcount == 2):
+                        self.on_start = on_start
+                    else:
+                        self.valid_parameters = False
+                        raise ValueError(f"The method assigned to the on_start parameter must accept only 2 parameters:\n1) Expected to be the 'self' object.\n2) The instance of the genetic algorithm.\nThe passed method named '{on_start.__code__.co_name}' accepts {on_start.__code__.co_argcount} parameter(s).")
+                # Check if the on_start is a function.
+                elif callable(on_start):
+                    # Check if the on_start function accepts only a single paramater.
+                    if (on_start.__code__.co_argcount == 1):
+                        self.on_start = on_start
+                    else:
+                        self.valid_parameters = False
+                        raise ValueError(f"The function assigned to the on_start parameter must accept only 1 parameter representing the instance of the genetic algorithm.\nThe passed function named '{on_start.__code__.co_name}' accepts {on_start.__code__.co_argcount} parameter(s).")
                 else:
                     self.valid_parameters = False
-                    self.logger.error("The method assigned to the on_parents parameter must accept 3 parameters:\n1) Expected to be the 'self' object.\n2) The instance of the genetic algorithm.\n3) The fitness values of all solutions.\nThe passed method named '{funcname}' accepts {argcount} parameter(s).".format(funcname=on_parents.__code__.co_name, argcount=on_parents.__code__.co_argcount))
-                    raise ValueError("The method assigned to the on_parents parameter must accept 3 parameters:\n1) Expected to be the 'self' object.\n2) The instance of the genetic algorithm.\n3) The fitness values of all solutions.\nThe passed method named '{funcname}' accepts {argcount} parameter(s).".format(funcname=on_parents.__code__.co_name, argcount=on_parents.__code__.co_argcount))
-            # Check if the on_parents is a function.
-            elif callable(on_parents):
-                # Check if the on_parents function accepts 2 paramaters.
-                if (on_parents.__code__.co_argcount == 2):
-                    self.on_parents = on_parents
+                    
+                    raise TypeError(f"The value assigned to the on_start parameter is expected to be of type function but {type(on_start)} found.")
+            else:
+                self.on_start = None
+
+            # Check if the on_fitness exists.
+            if not (on_fitness is None):
+                # Check if the on_fitness is a method.
+                if inspect.ismethod(on_fitness):
+                    # Check if the on_fitness method accepts 3 paramaters.
+                    if (on_fitness.__code__.co_argcount == 3):
+                        self.on_fitness = on_fitness
+                    else:
+                        self.valid_parameters = False
+                        raise ValueError(f"The method assigned to the on_fitness parameter must accept 3 parameters:\n1) Expected to be the 'self' object.\n2) The instance of the genetic algorithm.3) The fitness values of all solutions.\nThe passed method named '{on_fitness.__code__.co_name}' accepts {on_fitness.__code__.co_argcount} parameter(s).")
+                # Check if the on_fitness is a function.
+                elif callable(on_fitness):
+                    # Check if the on_fitness function accepts 2 paramaters.
+                    if (on_fitness.__code__.co_argcount == 2):
+                        self.on_fitness = on_fitness
+                    else:
+                        self.valid_parameters = False
+                        raise ValueError(f"The function assigned to the on_fitness parameter must accept 2 parameters representing the instance of the genetic algorithm and the fitness values of all solutions.\nThe passed function named '{on_fitness.__code__.co_name}' accepts {on_fitness.__code__.co_argcount} parameter(s).")
                 else:
                     self.valid_parameters = False
-                    self.logger.error("The function assigned to the on_parents parameter must accept 2 parameters representing the instance of the genetic algorithm and the fitness values of all solutions.\nThe passed function named '{funcname}' accepts {argcount} parameter(s).".format(funcname=on_parents.__code__.co_name, argcount=on_parents.__code__.co_argcount))
-                    raise ValueError("The function assigned to the on_parents parameter must accept 2 parameters representing the instance of the genetic algorithm and the fitness values of all solutions.\nThe passed function named '{funcname}' accepts {argcount} parameter(s).".format(funcname=on_parents.__code__.co_name, argcount=on_parents.__code__.co_argcount))
+                    raise TypeError(f"The value assigned to the on_fitness parameter is expected to be of type function but {type(on_fitness)} found.")
             else:
-                self.valid_parameters = False
-                self.logger.error("The value assigned to the on_parents parameter is expected to be of type function but {on_parents_type} found.".format(on_parents_type=type(on_parents)))
-                raise TypeError("The value assigned to the on_parents parameter is expected to be of type function but {on_parents_type} found.".format(on_parents_type=type(on_parents)))
-        else:
-            self.on_parents = None
+                self.on_fitness = None
 
-        # Check if the on_crossover exists.
-        if not (on_crossover is None):
-            # Check if the on_crossover is a method.
-            if inspect.ismethod(on_crossover):
-                # Check if the on_crossover method accepts 3 paramaters.
-                if (on_crossover.__code__.co_argcount == 3):
-                    self.on_crossover = on_crossover
+            # Check if the on_parents exists.
+            if not (on_parents is None):
+                # Check if the on_parents is a method.
+                if inspect.ismethod(on_parents):
+                    # Check if the on_parents method accepts 3 paramaters.
+                    if (on_parents.__code__.co_argcount == 3):
+                        self.on_parents = on_parents
+                    else:
+                        self.valid_parameters = False
+                        raise ValueError(f"The method assigned to the on_parents parameter must accept 3 parameters:\n1) Expected to be the 'self' object.\n2) The instance of the genetic algorithm.\n3) The fitness values of all solutions.\nThe passed method named '{on_parents.__code__.co_name}' accepts {on_parents.__code__.co_argcount} parameter(s).")
+                # Check if the on_parents is a function.
+                elif callable(on_parents):
+                    # Check if the on_parents function accepts 2 paramaters.
+                    if (on_parents.__code__.co_argcount == 2):
+                        self.on_parents = on_parents
+                    else:
+                        self.valid_parameters = False
+                        raise ValueError(f"The function assigned to the on_parents parameter must accept 2 parameters representing the instance of the genetic algorithm and the fitness values of all solutions.\nThe passed function named '{on_parents.__code__.co_name}' accepts {on_parents.__code__.co_argcount} parameter(s).")
                 else:
                     self.valid_parameters = False
-                    self.logger.error("The method assigned to the on_crossover parameter must accept 3 parameters:\n1) Expected to be the 'self' object.\n2) The instance of the genetic algorithm.\n2) The offspring generated using crossover.\nThe passed method named '{funcname}' accepts {argcount} parameter(s).".format(funcname=on_crossover.__code__.co_name, argcount=on_crossover.__code__.co_argcount))
-                    raise ValueError("The method assigned to the on_crossover parameter must accept 3 parameters:\n1) Expected to be the 'self' object.\n2) The instance of the genetic algorithm.\n2) The offspring generated using crossover.\nThe passed method named '{funcname}' accepts {argcount} parameter(s).".format(funcname=on_crossover.__code__.co_name, argcount=on_crossover.__code__.co_argcount))
-            # Check if the on_crossover is a function.
-            elif callable(on_crossover):
-                # Check if the on_crossover function accepts 2 paramaters.
-                if (on_crossover.__code__.co_argcount == 2):
-                    self.on_crossover = on_crossover
+                    raise TypeError(f"The value assigned to the on_parents parameter is expected to be of type function but {type(on_parents)} found.")
+            else:
+                self.on_parents = None
+
+            # Check if the on_crossover exists.
+            if not (on_crossover is None):
+                # Check if the on_crossover is a method.
+                if inspect.ismethod(on_crossover):
+                    # Check if the on_crossover method accepts 3 paramaters.
+                    if (on_crossover.__code__.co_argcount == 3):
+                        self.on_crossover = on_crossover
+                    else:
+                        self.valid_parameters = False
+                        raise ValueError(f"The method assigned to the on_crossover parameter must accept 3 parameters:\n1) Expected to be the 'self' object.\n2) The instance of the genetic algorithm.\n2) The offspring generated using crossover.\nThe passed method named '{on_crossover.__code__.co_name}' accepts {on_crossover.__code__.co_argcount} parameter(s).")
+                # Check if the on_crossover is a function.
+                elif callable(on_crossover):
+                    # Check if the on_crossover function accepts 2 paramaters.
+                    if (on_crossover.__code__.co_argcount == 2):
+                        self.on_crossover = on_crossover
+                    else:
+                        self.valid_parameters = False
+                        raise ValueError(f"The function assigned to the on_crossover parameter must accept 2 parameters representing the instance of the genetic algorithm and the offspring generated using crossover.\nThe passed function named '{on_crossover.__code__.co_name}' accepts {on_crossover.__code__.co_argcount} parameter(s).")
                 else:
                     self.valid_parameters = False
-                    self.logger.error("The function assigned to the on_crossover parameter must accept 2 parameters representing the instance of the genetic algorithm and the offspring generated using crossover.\nThe passed function named '{funcname}' accepts {argcount} parameter(s).".format(funcname=on_crossover.__code__.co_name, argcount=on_crossover.__code__.co_argcount))
-                    raise ValueError("The function assigned to the on_crossover parameter must accept 2 parameters representing the instance of the genetic algorithm and the offspring generated using crossover.\nThe passed function named '{funcname}' accepts {argcount} parameter(s).".format(funcname=on_crossover.__code__.co_name, argcount=on_crossover.__code__.co_argcount))
+                    raise TypeError(f"The value assigned to the on_crossover parameter is expected to be of type function but {type(on_crossover)} found.")
             else:
-                self.valid_parameters = False
-                self.logger.error("The value assigned to the on_crossover parameter is expected to be of type function but {on_crossover_type} found.".format(on_crossover_type=type(on_crossover)))
-                raise TypeError("The value assigned to the on_crossover parameter is expected to be of type function but {on_crossover_type} found.".format(on_crossover_type=type(on_crossover)))
-        else:
-            self.on_crossover = None
+                self.on_crossover = None
 
-        # Check if the on_mutation exists.
-        if not (on_mutation is None):
-            # Check if the on_mutation is a method.
-            if inspect.ismethod(on_mutation):
-                # Check if the on_mutation method accepts 3 paramaters.
-                if (on_mutation.__code__.co_argcount == 3):
-                    self.on_mutation = on_mutation
+            # Check if the on_mutation exists.
+            if not (on_mutation is None):
+                # Check if the on_mutation is a method.
+                if inspect.ismethod(on_mutation):
+                    # Check if the on_mutation method accepts 3 paramaters.
+                    if (on_mutation.__code__.co_argcount == 3):
+                        self.on_mutation = on_mutation
+                    else:
+                        self.valid_parameters = False
+                        raise ValueError(f"The method assigned to the on_mutation parameter must accept 3 parameters:\n1) Expected to be the 'self' object.\n2) The instance of the genetic algorithm.\n2) The offspring after applying the mutation operation.\nThe passed method named '{on_mutation.__code__.co_name}' accepts {on_mutation.__code__.co_argcount} parameter(s).")
+                # Check if the on_mutation is a function.
+                elif callable(on_mutation):
+                    # Check if the on_mutation function accepts 2 paramaters.
+                    if (on_mutation.__code__.co_argcount == 2):
+                        self.on_mutation = on_mutation
+                    else:
+                        self.valid_parameters = False
+                        raise ValueError(f"The function assigned to the on_mutation parameter must accept 2 parameters representing the instance of the genetic algorithm and the offspring after applying the mutation operation.\nThe passed function named '{on_mutation.__code__.co_name}' accepts {on_mutation.__code__.co_argcount} parameter(s).")
                 else:
                     self.valid_parameters = False
-                    self.logger.error("The method assigned to the on_mutation parameter must accept 3 parameters:\n1) Expected to be the 'self' object.\n2) The instance of the genetic algorithm.\n2) The offspring after applying the mutation operation.\nThe passed method named '{funcname}' accepts {argcount} parameter(s).".format(funcname=on_mutation.__code__.co_name, argcount=on_mutation.__code__.co_argcount))
-                    raise ValueError("The method assigned to the on_mutation parameter must accept 3 parameters:\n1) Expected to be the 'self' object.\n2) The instance of the genetic algorithm.\n2) The offspring after applying the mutation operation.\nThe passed method named '{funcname}' accepts {argcount} parameter(s).".format(funcname=on_mutation.__code__.co_name, argcount=on_mutation.__code__.co_argcount))
-            # Check if the on_mutation is a function.
-            elif callable(on_mutation):
-                # Check if the on_mutation function accepts 2 paramaters.
-                if (on_mutation.__code__.co_argcount == 2):
-                    self.on_mutation = on_mutation
+                    raise TypeError(f"The value assigned to the on_mutation parameter is expected to be of type function but {type(on_mutation)} found.")
+            else:
+                self.on_mutation = None
+
+            # Check if the on_generation exists.
+            if not (on_generation is None):
+                # Check if the on_generation is a method.
+                if inspect.ismethod(on_generation):
+                    # Check if the on_generation method accepts 2 paramaters.
+                    if (on_generation.__code__.co_argcount == 2):
+                        self.on_generation = on_generation
+                    else:
+                        self.valid_parameters = False
+                        raise ValueError(f"The method assigned to the on_generation parameter must accept 2 parameters:\n1) Expected to be the 'self' object.\n2) The instance of the genetic algorithm.\nThe passed method named '{on_generation.__code__.co_name}' accepts {on_generation.__code__.co_argcount} parameter(s).")
+                # Check if the on_generation is a function.
+                elif callable(on_generation):
+                    # Check if the on_generation function accepts only a single paramater.
+                    if (on_generation.__code__.co_argcount == 1):
+                        self.on_generation = on_generation
+                    else:
+                        self.valid_parameters = False
+                        raise ValueError(f"The function assigned to the on_generation parameter must accept only 1 parameter representing the instance of the genetic algorithm.\nThe passed function named '{on_generation.__code__.co_name}' accepts {on_generation.__code__.co_argcount} parameter(s).")
                 else:
                     self.valid_parameters = False
-                    self.logger.error("The function assigned to the on_mutation parameter must accept 2 parameters representing the instance of the genetic algorithm and the offspring after applying the mutation operation.\nThe passed function named '{funcname}' accepts {argcount} parameter(s).".format(funcname=on_mutation.__code__.co_name, argcount=on_mutation.__code__.co_argcount))
-                    raise ValueError("The function assigned to the on_mutation parameter must accept 2 parameters representing the instance of the genetic algorithm and the offspring after applying the mutation operation.\nThe passed function named '{funcname}' accepts {argcount} parameter(s).".format(funcname=on_mutation.__code__.co_name, argcount=on_mutation.__code__.co_argcount))
+                    raise TypeError(f"The value assigned to the on_generation parameter is expected to be of type function but {type(on_generation)} found.")
             else:
-                self.valid_parameters = False
-                self.logger.error("The value assigned to the on_mutation parameter is expected to be of type function but {on_mutation_type} found.".format(on_mutation_type=type(on_mutation)))
-                raise TypeError("The value assigned to the on_mutation parameter is expected to be of type function but {on_mutation_type} found.".format(on_mutation_type=type(on_mutation)))
-        else:
-            self.on_mutation = None
+                self.on_generation = None
 
-        # Check if the on_generation exists.
-        if not (on_generation is None):
-            # Check if the on_generation is a method.
-            if inspect.ismethod(on_generation):
-                # Check if the on_generation method accepts 2 paramaters.
-                if (on_generation.__code__.co_argcount == 2):
-                    self.on_generation = on_generation
+            # Check if the on_stop exists.
+            if not (on_stop is None):
+                # Check if the on_stop is a method.
+                if inspect.ismethod(on_stop):
+                    # Check if the on_stop method accepts 3 paramaters.
+                    if (on_stop.__code__.co_argcount == 3):
+                        self.on_stop = on_stop
+                    else:
+                        self.valid_parameters = False
+                        raise ValueError(f"The method assigned to the on_stop parameter must accept 3 parameters:\n1) Expected to be the 'self' object.\n2) The instance of the genetic algorithm.\n2) A list of the fitness values of the solutions in the last population.\nThe passed method named '{on_stop.__code__.co_name}' accepts {on_stop.__code__.co_argcount} parameter(s).")
+                # Check if the on_stop is a function.
+                elif callable(on_stop):
+                    # Check if the on_stop function accepts 2 paramaters.
+                    if (on_stop.__code__.co_argcount == 2):
+                        self.on_stop = on_stop
+                    else:
+                        self.valid_parameters = False
+                        raise ValueError(f"The function assigned to the on_stop parameter must accept 2 parameters representing the instance of the genetic algorithm and a list of the fitness values of the solutions in the last population.\nThe passed function named '{on_stop.__code__.co_name}' accepts {on_stop.__code__.co_argcount} parameter(s).")
                 else:
                     self.valid_parameters = False
-                    self.logger.error("The method assigned to the on_generation parameter must accept 2 parameters:\n1) Expected to be the 'self' object.\n2) The instance of the genetic algorithm.\nThe passed method named '{funcname}' accepts {argcount} parameter(s).".format(funcname=on_generation.__code__.co_name, argcount=on_generation.__code__.co_argcount))
-                    raise ValueError("The method assigned to the on_generation parameter must accept 2 parameters:\n1) Expected to be the 'self' object.\n2) The instance of the genetic algorithm.\nThe passed method named '{funcname}' accepts {argcount} parameter(s).".format(funcname=on_generation.__code__.co_name, argcount=on_generation.__code__.co_argcount))
-            # Check if the on_generation is a function.
-            elif callable(on_generation):
-                # Check if the on_generation function accepts only a single paramater.
-                if (on_generation.__code__.co_argcount == 1):
-                    self.on_generation = on_generation
+                    raise TypeError(f"The value assigned to the 'on_stop' parameter is expected to be of type function but {type(on_stop)} found.")
+            else:
+                self.on_stop = None
+
+            # Validate delay_after_gen
+            if type(delay_after_gen) in GA.supported_int_float_types:
+                if delay_after_gen >= 0.0:
+                    self.delay_after_gen = delay_after_gen
                 else:
                     self.valid_parameters = False
-                    self.logger.error("The function assigned to the on_generation parameter must accept only 1 parameter representing the instance of the genetic algorithm.\nThe passed function named '{funcname}' accepts {argcount} parameter(s).".format(funcname=on_generation.__code__.co_name, argcount=on_generation.__code__.co_argcount))
-                    raise ValueError("The function assigned to the on_generation parameter must accept only 1 parameter representing the instance of the genetic algorithm.\nThe passed function named '{funcname}' accepts {argcount} parameter(s).".format(funcname=on_generation.__code__.co_name, argcount=on_generation.__code__.co_argcount))
+                    raise ValueError(f"The value passed to the 'delay_after_gen' parameter must be a non-negative number. The value passed is ({delay_after_gen}) of type {type(delay_after_gen)}.")
             else:
                 self.valid_parameters = False
-                self.logger.error("The value assigned to the on_generation parameter is expected to be of type function but {on_generation_type} found.".format(on_generation_type=type(on_generation)))
-                raise TypeError("The value assigned to the on_generation parameter is expected to be of type function but {on_generation_type} found.".format(on_generation_type=type(on_generation)))
-        else:
-            self.on_generation = None
+                raise TypeError(f"The value passed to the 'delay_after_gen' parameter must be of type int or float but {type(delay_after_gen)} found.")
 
-        # Check if the on_stop exists.
-        if not (on_stop is None):
-            # Check if the on_stop is a method.
-            if inspect.ismethod(on_stop):
-                # Check if the on_stop method accepts 3 paramaters.
-                if (on_stop.__code__.co_argcount == 3):
-                    self.on_stop = on_stop
-                else:
-                    self.valid_parameters = False
-                    self.logger.error("The method assigned to the on_stop parameter must accept 3 parameters:\n1) Expected to be the 'self' object.\n2) The instance of the genetic algorithm.\n2) A list of the fitness values of the solutions in the last population.\nThe passed method named '{funcname}' accepts {argcount} parameter(s).".format(funcname=on_stop.__code__.co_name, argcount=on_stop.__code__.co_argcount))
-                    raise ValueError("The method assigned to the on_stop parameter must accept 3 parameters:\n1) Expected to be the 'self' object.\n2) The instance of the genetic algorithm.\n2) A list of the fitness values of the solutions in the last population.\nThe passed method named '{funcname}' accepts {argcount} parameter(s).".format(funcname=on_stop.__code__.co_name, argcount=on_stop.__code__.co_argcount))
-            # Check if the on_stop is a function.
-            elif callable(on_stop):
-                # Check if the on_stop function accepts 2 paramaters.
-                if (on_stop.__code__.co_argcount == 2):
-                    self.on_stop = on_stop
-                else:
-                    self.valid_parameters = False
-                    self.logger.error("The function assigned to the on_stop parameter must accept 2 parameters representing the instance of the genetic algorithm and a list of the fitness values of the solutions in the last population.\nThe passed function named '{funcname}' accepts {argcount} parameter(s).".format(funcname=on_stop.__code__.co_name, argcount=on_stop.__code__.co_argcount))
-                    raise ValueError("The function assigned to the on_stop parameter must accept 2 parameters representing the instance of the genetic algorithm and a list of the fitness values of the solutions in the last population.\nThe passed function named '{funcname}' accepts {argcount} parameter(s).".format(funcname=on_stop.__code__.co_name, argcount=on_stop.__code__.co_argcount))
+            # Validate save_best_solutions
+            if type(save_best_solutions) is bool:
+                if save_best_solutions == True:
+                    if not self.suppress_warnings:
+                        warnings.warn("Use the 'save_best_solutions' parameter with caution as it may cause memory overflow when either the number of generations or number of genes is large.")
             else:
                 self.valid_parameters = False
-                self.logger.error("The value assigned to the 'on_stop' parameter is expected to be of type function but {on_stop_type} found.".format(on_stop_type=type(on_stop)))
-                raise TypeError("The value assigned to the 'on_stop' parameter is expected to be of type function but {on_stop_type} found.".format(on_stop_type=type(on_stop)))
-        else:
-            self.on_stop = None
+                raise TypeError(f"The value passed to the 'save_best_solutions' parameter must be of type bool but {type(save_best_solutions)} found.")
 
-        # Validate delay_after_gen
-        if type(delay_after_gen) in GA.supported_int_float_types:
-            if delay_after_gen >= 0.0:
-                self.delay_after_gen = delay_after_gen
+            # Validate save_solutions
+            if type(save_solutions) is bool:
+                if save_solutions == True:
+                    if not self.suppress_warnings:
+                        warnings.warn("Use the 'save_solutions' parameter with caution as it may cause memory overflow when either the number of generations, number of genes, or number of solutions in population is large.")
             else:
                 self.valid_parameters = False
-                self.logger.error("The value passed to the 'delay_after_gen' parameter must be a non-negative number. The value passed is ({delay_after_gen}) of type {delay_after_gen_type}.".format(delay_after_gen=delay_after_gen, delay_after_gen_type=type(delay_after_gen)))
-                raise ValueError("The value passed to the 'delay_after_gen' parameter must be a non-negative number. The value passed is ({delay_after_gen}) of type {delay_after_gen_type}.".format(delay_after_gen=delay_after_gen, delay_after_gen_type=type(delay_after_gen)))
-        else:
-            self.valid_parameters = False
-            self.logger.error("The value passed to the 'delay_after_gen' parameter must be of type int or float but {delay_after_gen_type} found.".format(delay_after_gen_type=type(delay_after_gen)))
-            raise TypeError("The value passed to the 'delay_after_gen' parameter must be of type int or float but {delay_after_gen_type} found.".format(delay_after_gen_type=type(delay_after_gen)))
-
-        # Validate save_best_solutions
-        if type(save_best_solutions) is bool:
-            if save_best_solutions == True:
-                if not self.suppress_warnings: warnings.warn("Use the 'save_best_solutions' parameter with caution as it may cause memory overflow when either the number of generations or number of genes is large.")
-        else:
-            self.valid_parameters = False
-            self.logger.error("The value passed to the 'save_best_solutions' parameter must be of type bool but {save_best_solutions_type} found.".format(save_best_solutions_type=type(save_best_solutions)))
-            raise TypeError("The value passed to the 'save_best_solutions' parameter must be of type bool but {save_best_solutions_type} found.".format(save_best_solutions_type=type(save_best_solutions)))
-
-        # Validate save_solutions
-        if type(save_solutions) is bool:
-            if save_solutions == True:
-                if not self.suppress_warnings: warnings.warn("Use the 'save_solutions' parameter with caution as it may cause memory overflow when either the number of generations, number of genes, or number of solutions in population is large.")
-        else:
-            self.valid_parameters = False
-            self.logger.error("The value passed to the 'save_solutions' parameter must be of type bool but {save_solutions_type} found.".format(save_solutions_type=type(save_solutions)))
-            raise TypeError("The value passed to the 'save_solutions' parameter must be of type bool but {save_solutions_type} found.".format(save_solutions_type=type(save_solutions)))
-
-        # Validate allow_duplicate_genes
-        if not (type(allow_duplicate_genes) is bool):
-            self.valid_parameters = False
-            self.logger.error("The expected type of the 'allow_duplicate_genes' parameter is bool but {allow_duplicate_genes_type} found.".format(allow_duplicate_genes_type=type(allow_duplicate_genes)))
-            raise TypeError("The expected type of the 'allow_duplicate_genes' parameter is bool but {allow_duplicate_genes_type} found.".format(allow_duplicate_genes_type=type(allow_duplicate_genes)))
-
-        self.allow_duplicate_genes = allow_duplicate_genes
-
-        self.stop_criteria = []
-        self.supported_stop_words = ["reach", "saturate"]
-        if stop_criteria is None:
-            # None: Stop after passing through all generations.
-            self.stop_criteria = None
-        elif type(stop_criteria) is str:
-            # reach_{target_fitness}: Stop if the target fitness value is reached.
-            # saturate_{num_generations}: Stop if the fitness value does not change (saturates) for the given number of generations.
-            criterion = stop_criteria.split("_")
-            if len(criterion) == 2:
-                stop_word = criterion[0]
-                number = criterion[1]
+                raise TypeError(f"The value passed to the 'save_solutions' parameter must be of type bool but {type(save_solutions)} found.")
 
-                if stop_word in self.supported_stop_words:
-                    pass
-                else:
-                    self.valid_parameters = False
-                    self.logger.error("In the 'stop_criteria' parameter, the supported stop words are '{supported_stop_words}' but '{stop_word}' found.".format(supported_stop_words=self.supported_stop_words, stop_word=stop_word))
-                    raise ValueError("In the 'stop_criteria' parameter, the supported stop words are '{supported_stop_words}' but '{stop_word}' found.".format(supported_stop_words=self.supported_stop_words, stop_word=stop_word))
+            self.stop_criteria = []
+            self.supported_stop_words = ["reach", "saturate"]
+            if stop_criteria is None:
+                # None: Stop after passing through all generations.
+                self.stop_criteria = None
+            elif type(stop_criteria) is str:
+                # reach_{target_fitness}: Stop if the target fitness value is reached.
+                # saturate_{num_generations}: Stop if the fitness value does not change (saturates) for the given number of generations.
+                criterion = stop_criteria.split("_")
+                if len(criterion) == 2:
+                    stop_word = criterion[0]
+                    number = criterion[1]
+
+                    if stop_word in self.supported_stop_words:
+                        pass
+                    else:
+                        self.valid_parameters = False
+                        raise ValueError(f"In the 'stop_criteria' parameter, the supported stop words are '{self.supported_stop_words}' but '{stop_word}' found.")
+
+                    if number.replace(".", "").isnumeric():
+                        number = float(number)
+                    else:
+                        self.valid_parameters = False
+                        raise ValueError(f"The value following the stop word in the 'stop_criteria' parameter must be a number but the value ({number}) of type {type(number)} found.")
+
+                    self.stop_criteria.append([stop_word, number])
 
-                if number.replace(".", "").isnumeric():
-                    number = float(number)
                 else:
                     self.valid_parameters = False
-                    self.logger.error("The value following the stop word in the 'stop_criteria' parameter must be a number but the value ({stop_val}) of type {stop_val_type} found.".format(stop_val=number, stop_val_type=type(number)))
-                    raise ValueError("The value following the stop word in the 'stop_criteria' parameter must be a number but the value ({stop_val}) of type {stop_val_type} found.".format(stop_val=number, stop_val_type=type(number)))
-                
-                self.stop_criteria.append([stop_word, number])
+                    raise ValueError(f"For format of a single criterion in the 'stop_criteria' parameter is 'word_number' but '{stop_criteria}' found.")
 
-            else:
-                self.valid_parameters = False
-                self.logger.error("For format of a single criterion in the 'stop_criteria' parameter is 'word_number' but '{stop_criteria}' found.".format(stop_criteria=stop_criteria))
-                raise ValueError("For format of a single criterion in the 'stop_criteria' parameter is 'word_number' but '{stop_criteria}' found.".format(stop_criteria=stop_criteria))
+            elif type(stop_criteria) in [list, tuple, numpy.ndarray]:
+                # Remove duplicate criterira by converting the list to a set then back to a list.
+                stop_criteria = list(set(stop_criteria))
+                for idx, val in enumerate(stop_criteria):
+                    if type(val) is str:
+                        criterion = val.split("_")
+                        if len(criterion) == 2:
+                            stop_word = criterion[0]
+                            number = criterion[1]
 
-        elif type(stop_criteria) in [list, tuple, numpy.ndarray]:
-            # Remove duplicate criterira by converting the list to a set then back to a list.
-            stop_criteria = list(set(stop_criteria))
-            for idx, val in enumerate(stop_criteria):
-                if type(val) is str:
-                    criterion = val.split("_")
-                    if len(criterion) == 2:
-                        stop_word = criterion[0]
-                        number = criterion[1]
+                            if stop_word in self.supported_stop_words:
+                                pass
+                            else:
+                                self.valid_parameters = False
+                                raise ValueError(f"In the 'stop_criteria' parameter, the supported stop words are {self.supported_stop_words} but '{stop_word}' found.")
 
-                        if stop_word in self.supported_stop_words:
-                            pass
-                        else:
-                            self.valid_parameters = False
-                            self.logger.error("In the 'stop_criteria' parameter, the supported stop words are {supported_stop_words} but '{stop_word}' found.".format(supported_stop_words=self.supported_stop_words, stop_word=stop_word))
-                            raise ValueError("In the 'stop_criteria' parameter, the supported stop words are {supported_stop_words} but '{stop_word}' found.".format(supported_stop_words=self.supported_stop_words, stop_word=stop_word))
+                            if number.replace(".", "").isnumeric():
+                                number = float(number)
+                            else:
+                                self.valid_parameters = False
+                                raise ValueError(f"The value following the stop word in the 'stop_criteria' parameter must be a number but the value ({number}) of type {type(number)} found.")
+
+                            self.stop_criteria.append([stop_word, number])
 
-                        if number.replace(".", "").isnumeric():
-                            number = float(number)
                         else:
                             self.valid_parameters = False
-                            self.logger.error("The value following the stop word in the 'stop_criteria' parameter must be a number but the value ({stop_val}) of type {stop_val_type} found.".format(stop_val=number, stop_val_type=type(number)))
-                            raise ValueError("The value following the stop word in the 'stop_criteria' parameter must be a number but the value ({stop_val}) of type {stop_val_type} found.".format(stop_val=number, stop_val_type=type(number)))
-
-                        self.stop_criteria.append([stop_word, number])
-
+                            raise ValueError(f"The format of a single criterion in the 'stop_criteria' parameter is 'word_number' but {criterion} found.")
                     else:
                         self.valid_parameters = False
-                        self.logger.error("The format of a single criterion in the 'stop_criteria' parameter is 'word_number' but {stop_criteria} found.".format(stop_criteria=criterion))
-                        raise ValueError("The format of a single criterion in the 'stop_criteria' parameter is 'word_number' but {stop_criteria} found.".format(stop_criteria=criterion))
-                else:
-                    self.valid_parameters = False
-                    self.logger.error("When the 'stop_criteria' parameter is assigned a tuple/list/numpy.ndarray, then its elements must be strings but the value ({stop_criteria_val}) of type {stop_criteria_val_type} found at index {stop_criteria_val_idx}.".format(stop_criteria_val=val, stop_criteria_val_type=type(val), stop_criteria_val_idx=idx))
-                    raise TypeError("When the 'stop_criteria' parameter is assigned a tuple/list/numpy.ndarray, then its elements must be strings but the value ({stop_criteria_val}) of type {stop_criteria_val_type} found at index {stop_criteria_val_idx}.".format(stop_criteria_val=val, stop_criteria_val_type=type(val), stop_criteria_val_idx=idx))
-        else:
-            self.valid_parameters = False
-            self.logger.error("The expected value of the 'stop_criteria' is a single string or a list/tuple/numpy.ndarray of strings but the value ({stop_criteria_val}) of type {stop_criteria_type} found.".format(stop_criteria_val=stop_criteria, stop_criteria_type=type(stop_criteria)))
-            raise TypeError("The expected value of the 'stop_criteria' is a single string or a list/tuple/numpy.ndarray of strings but the value ({stop_criteria_val}) of type {stop_criteria_type} found.".format(stop_criteria_val=stop_criteria, stop_criteria_type=type(stop_criteria)))
-
-        if parallel_processing is None:
-            self.parallel_processing = None
-        elif type(parallel_processing) in GA.supported_int_types:
-            if parallel_processing > 0:
-                self.parallel_processing = ["thread", parallel_processing]
-            else:
-                self.valid_parameters = False
-                self.logger.error("When the 'parallel_processing' parameter is assigned an integer, then the integer must be positive but the value ({parallel_processing_value}) found.".format(parallel_processing_value=parallel_processing))
-                raise ValueError("When the 'parallel_processing' parameter is assigned an integer, then the integer must be positive but the value ({parallel_processing_value}) found.".format(parallel_processing_value=parallel_processing))
-        elif type(parallel_processing) in [list, tuple]:
-            if len(parallel_processing) == 2:
-                if type(parallel_processing[0]) is str:
-                    if parallel_processing[0] in ["process", "thread"]:
-                        if (type(parallel_processing[1]) in GA.supported_int_types and parallel_processing[1] > 0) or (parallel_processing[1] == 0) or (parallel_processing[1] is None):
-                            if parallel_processing[1] == 0:
-                                # If the number of processes/threads is 0, this means no parallel processing is used. It is equivelant to setting parallel_processing=None.
-                                self.parallel_processing = None
+                        raise TypeError(f"When the 'stop_criteria' parameter is assigned a tuple/list/numpy.ndarray, then its elements must be strings but the value ({val}) of type {type(val)} found at index {idx}.")
+            else:
+                self.valid_parameters = False
+                raise TypeError(f"The expected value of the 'stop_criteria' is a single string or a list/tuple/numpy.ndarray of strings but the value ({stop_criteria}) of type {type(stop_criteria)} found.")
+
+            if parallel_processing is None:
+                self.parallel_processing = None
+            elif type(parallel_processing) in GA.supported_int_types:
+                if parallel_processing > 0:
+                    self.parallel_processing = ["thread", parallel_processing]
+                else:
+                    self.valid_parameters = False
+                    raise ValueError(f"When the 'parallel_processing' parameter is assigned an integer, then the integer must be positive but the value ({parallel_processing}) found.")
+            elif type(parallel_processing) in [list, tuple]:
+                if len(parallel_processing) == 2:
+                    if type(parallel_processing[0]) is str:
+                        if parallel_processing[0] in ["process", "thread"]:
+                            if (type(parallel_processing[1]) in GA.supported_int_types and parallel_processing[1] > 0) or (parallel_processing[1] == 0) or (parallel_processing[1] is None):
+                                if parallel_processing[1] == 0:
+                                    # If the number of processes/threads is 0, this means no parallel processing is used. It is equivelant to setting parallel_processing=None.
+                                    self.parallel_processing = None
+                                else:
+                                    # Whether the second value is None or a positive integer.
+                                    self.parallel_processing = parallel_processing
                             else:
-                                # Whether the second value is None or a positive integer.
-                                self.parallel_processing = parallel_processing
+                                self.valid_parameters = False
+                                raise TypeError(f"When a list or tuple is assigned to the 'parallel_processing' parameter, then the second element must be an integer but the value ({parallel_processing[1]}) of type {type(parallel_processing[1])} found.")
                         else:
                             self.valid_parameters = False
-                            self.logger.error("When a list or tuple is assigned to the 'parallel_processing' parameter, then the second element must be an integer but the value ({second_value}) of type {second_value_type} found.".format(second_value=parallel_processing[1], second_value_type=type(parallel_processing[1])))
-                            raise TypeError("When a list or tuple is assigned to the 'parallel_processing' parameter, then the second element must be an integer but the value ({second_value}) of type {second_value_type} found.".format(second_value=parallel_processing[1], second_value_type=type(parallel_processing[1])))
+                            raise ValueError(f"When a list or tuple is assigned to the 'parallel_processing' parameter, then the value of the first element must be either 'process' or 'thread' but the value ({parallel_processing[0]}) found.")
                     else:
                         self.valid_parameters = False
-                        self.logger.error("When a list or tuple is assigned to the 'parallel_processing' parameter, then the value of the first element must be either 'process' or 'thread' but the value ({first_value}) found.".format(first_value=parallel_processing[0]))
-                        raise ValueError("When a list or tuple is assigned to the 'parallel_processing' parameter, then the value of the first element must be either 'process' or 'thread' but the value ({first_value}) found.".format(first_value=parallel_processing[0]))
+                        raise TypeError(f"When a list or tuple is assigned to the 'parallel_processing' parameter, then the first element must be of type 'str' but the value ({parallel_processing[0]}) of type {type(parallel_processing[0])} found.")
                 else:
                     self.valid_parameters = False
-                    self.logger.error("When a list or tuple is assigned to the 'parallel_processing' parameter, then the first element must be of type 'str' but the value ({first_value}) of type {first_value_type} found.".format(first_value=parallel_processing[0], first_value_type=type(parallel_processing[0])))
-                    raise TypeError("When a list or tuple is assigned to the 'parallel_processing' parameter, then the first element must be of type 'str' but the value ({first_value}) of type {first_value_type} found.".format(first_value=parallel_processing[0], first_value_type=type(parallel_processing[0])))
+                    raise ValueError(f"When a list or tuple is assigned to the 'parallel_processing' parameter, then it must have 2 elements but ({len(parallel_processing)}) found.")
             else:
                 self.valid_parameters = False
-                self.logger.error("When a list or tuple is assigned to the 'parallel_processing' parameter, then it must have 2 elements but ({num_elements}) found.".format(num_elements=len(parallel_processing)))
-                raise ValueError("When a list or tuple is assigned to the 'parallel_processing' parameter, then it must have 2 elements but ({num_elements}) found.".format(num_elements=len(parallel_processing)))
-        else:
-            self.valid_parameters = False
-            self.logger.error("Unexpected value ({parallel_processing_value}) of type ({parallel_processing_type}) assigned to the 'parallel_processing' parameter. The accepted values for this parameter are:\n1) None: (Default) It means no parallel processing is used.\n2) A positive integer referring to the number of threads to be used (i.e. threads, not processes, are used.\n3) list/tuple: If a list or a tuple of exactly 2 elements is assigned, then:\n\t*1) The first element can be either 'process' or 'thread' to specify whether processes or threads are used, respectively.\n\t*2) The second element can be:\n\t\t**1) A positive integer to select the maximum number of processes or threads to be used.\n\t\t**2) 0 to indicate that parallel processing is not used. This is identical to setting 'parallel_processing=None'.\n\t\t**3) None to use the default value as calculated by the concurrent.futures module.".format(parallel_processing_value=parallel_processing, parallel_processing_type=type(parallel_processing)))
-            raise ValueError("Unexpected value ({parallel_processing_value}) of type ({parallel_processing_type}) assigned to the 'parallel_processing' parameter. The accepted values for this parameter are:\n1) None: (Default) It means no parallel processing is used.\n2) A positive integer referring to the number of threads to be used (i.e. threads, not processes, are used.\n3) list/tuple: If a list or a tuple of exactly 2 elements is assigned, then:\n\t*1) The first element can be either 'process' or 'thread' to specify whether processes or threads are used, respectively.\n\t*2) The second element can be:\n\t\t**1) A positive integer to select the maximum number of processes or threads to be used.\n\t\t**2) 0 to indicate that parallel processing is not used. This is identical to setting 'parallel_processing=None'.\n\t\t**3) None to use the default value as calculated by the concurrent.futures module.".format(parallel_processing_value=parallel_processing, parallel_processing_type=type(parallel_processing)))
-
-        # Set the `run_completed` property to False. It is set to `True` only after the `run()` method is complete.
-        self.run_completed = False
-
-        # The number of completed generations.
-        self.generations_completed = 0
-
-        # At this point, all necessary parameters validation is done successfully and we are sure that the parameters are valid.
-        self.valid_parameters = True # Set to True when all the parameters passed in the GA class constructor are valid.
-
-        # Parameters of the genetic algorithm.
-        self.num_generations = abs(num_generations)
-        self.parent_selection_type = parent_selection_type
-
-        # Parameters of the mutation operation.
-        self.mutation_percent_genes = mutation_percent_genes
-        self.mutation_num_genes = mutation_num_genes
-
-        # Even such this parameter is declared in the class header, it is assigned to the object here to access it after saving the object.
-        self.best_solutions_fitness = [] # A list holding the fitness value of the best solution for each generation.
-
-        self.best_solution_generation = -1 # The generation number at which the best fitness value is reached. It is only assigned the generation number after the `run()` method completes. Otherwise, its value is -1.
-
-        self.save_best_solutions = save_best_solutions
-        self.best_solutions = [] # Holds the best solution in each generation.
-
-        self.save_solutions = save_solutions
-        self.solutions = [] # Holds the solutions in each generation.
-        self.solutions_fitness = [] # Holds the fitness of the solutions in each generation.
-
-        self.last_generation_fitness = None # A list holding the fitness values of all solutions in the last generation.
-        self.last_generation_parents = None # A list holding the parents of the last generation.
-        self.last_generation_offspring_crossover = None # A list holding the offspring after applying crossover in the last generation.
-        self.last_generation_offspring_mutation = None # A list holding the offspring after applying mutation in the last generation.
-        self.previous_generation_fitness = None # Holds the fitness values of one generation before the fitness values saved in the last_generation_fitness attribute. Added in PyGAD 2.16.2.
-        self.last_generation_elitism = None # Added in PyGAD 2.18.0. A NumPy array holding the elitism of the current generation according to the value passed in the 'keep_elitism' parameter. It works only if the 'keep_elitism' parameter has a non-zero value. 
-        self.last_generation_elitism_indices = None # Added in PyGAD 2.19.0. A NumPy array holding the indices of the elitism of the current generation. It works only if the 'keep_elitism' parameter has a non-zero value. 
+                raise ValueError(f"Unexpected value ({parallel_processing}) of type ({type(parallel_processing)}) assigned to the 'parallel_processing' parameter. The accepted values for this parameter are:\n1) None: (Default) It means no parallel processing is used.\n2) A positive integer referring to the number of threads to be used (i.e. threads, not processes, are used.\n3) list/tuple: If a list or a tuple of exactly 2 elements is assigned, then:\n\t*1) The first element can be either 'process' or 'thread' to specify whether processes or threads are used, respectively.\n\t*2) The second element can be:\n\t\t**1) A positive integer to select the maximum number of processes or threads to be used.\n\t\t**2) 0 to indicate that parallel processing is not used. This is identical to setting 'parallel_processing=None'.\n\t\t**3) None to use the default value as calculated by the concurrent.futures module.")
+
+            # Set the `run_completed` property to False. It is set to `True` only after the `run()` method is complete.
+            self.run_completed = False
+
+            # The number of completed generations.
+            self.generations_completed = 0
+
+            # At this point, all necessary parameters validation is done successfully and we are sure that the parameters are valid.
+            # Set to True when all the parameters passed in the GA class constructor are valid.
+            self.valid_parameters = True
+
+            # Parameters of the genetic algorithm.
+            self.num_generations = abs(num_generations)
+            self.parent_selection_type = parent_selection_type
+
+            # Parameters of the mutation operation.
+            self.mutation_percent_genes = mutation_percent_genes
+            self.mutation_num_genes = mutation_num_genes
+
+            # Even such this parameter is declared in the class header, it is assigned to the object here to access it after saving the object.
+            # A list holding the fitness value of the best solution for each generation.
+            self.best_solutions_fitness = []
+
+            # The generation number at which the best fitness value is reached. It is only assigned the generation number after the `run()` method completes. Otherwise, its value is -1.
+            self.best_solution_generation = -1
+
+            self.save_best_solutions = save_best_solutions
+            self.best_solutions = []  # Holds the best solution in each generation.
+
+            self.save_solutions = save_solutions
+            self.solutions = []  # Holds the solutions in each generation.
+            # Holds the fitness of the solutions in each generation.
+            self.solutions_fitness = []
+
+            # A list holding the fitness values of all solutions in the last generation.
+            self.last_generation_fitness = None
+            # A list holding the parents of the last generation.
+            self.last_generation_parents = None
+            # A list holding the offspring after applying crossover in the last generation.
+            self.last_generation_offspring_crossover = None
+            # A list holding the offspring after applying mutation in the last generation.
+            self.last_generation_offspring_mutation = None
+            # Holds the fitness values of one generation before the fitness values saved in the last_generation_fitness attribute. Added in PyGAD 2.16.2.
+            self.previous_generation_fitness = None
+            # Added in PyGAD 2.18.0. A NumPy array holding the elitism of the current generation according to the value passed in the 'keep_elitism' parameter. It works only if the 'keep_elitism' parameter has a non-zero value.
+            self.last_generation_elitism = None
+            # Added in PyGAD 2.19.0. A NumPy array holding the indices of the elitism of the current generation. It works only if the 'keep_elitism' parameter has a non-zero value.
+            self.last_generation_elitism_indices = None
+        except Exception as e:
+            self.logger.exception(e)
+            sys.exit(-1)
 
     def round_genes(self, solutions):
         for gene_idx in range(self.num_genes):
             if self.gene_type_single:
                 if not self.gene_type[1] is None:
-                    solutions[:, gene_idx] = numpy.round(solutions[:, gene_idx], self.gene_type[1])
+                    solutions[:, gene_idx] = numpy.round(solutions[:, gene_idx],
+                                                         self.gene_type[1])
             else:
                 if not self.gene_type[gene_idx][1] is None:
-                    solutions[:, gene_idx] = numpy.round(numpy.asarray(solutions[:, gene_idx], 
-                                                                       dtype=self.gene_type[gene_idx][0]), 
+                    solutions[:, gene_idx] = numpy.round(numpy.asarray(solutions[:, gene_idx],
+                                                                       dtype=self.gene_type[gene_idx][0]),
                                                          self.gene_type[gene_idx][1])
         return solutions
 
-    def initialize_population(self, 
-                              low, 
-                              high, 
-                              allow_duplicate_genes, 
-                              mutation_by_replacement, 
+    def initialize_population(self,
+                              low,
+                              high,
+                              allow_duplicate_genes,
+                              mutation_by_replacement,
                               gene_type):
-
         """
         Creates an initial population randomly as a NumPy array. The array is saved in the instance attribute named 'population'.
 
         low: The lower value of the random range from which the gene values in the initial population are selected. It defaults to -4. Available in PyGAD 1.0.20 and higher.
         high: The upper value of the random range from which the gene values in the initial population are selected. It defaults to -4. Available in PyGAD 1.0.20.
 
         This method assigns the values of the following 3 instance attributes:
             1. pop_size: Size of the population.
             2. population: Initially, holds the initial population and later updated after each generation.
             3. init_population: Keeping the initial population.
         """
 
         # Population size = (number of chromosomes, number of genes per chromosome)
-        self.pop_size = (self.sol_per_pop,self.num_genes) # The population will have sol_per_pop chromosome where each chromosome has num_genes genes.
+        # The population will have sol_per_pop chromosome where each chromosome has num_genes genes.
+        self.pop_size = (self.sol_per_pop, self.num_genes)
 
         if self.gene_space is None:
             # Creating the initial population randomly.
             if self.gene_type_single == True:
-                self.population = numpy.asarray(numpy.random.uniform(low=low, 
-                                                                     high=high, 
-                                                                     size=self.pop_size), 
-                                                dtype=self.gene_type[0]) # A NumPy array holding the initial population.
+                self.population = numpy.asarray(numpy.random.uniform(low=low,
+                                                                     high=high,
+                                                                     size=self.pop_size),
+                                                dtype=self.gene_type[0])  # A NumPy array holding the initial population.
             else:
                 # Create an empty population of dtype=object to support storing mixed data types within the same array.
-                self.population = numpy.zeros(shape=self.pop_size, dtype=object)
+                self.population = numpy.zeros(
+                    shape=self.pop_size, dtype=object)
                 # Loop through the genes, randomly generate the values of a single gene across the entire population, and add the values of each gene to the population.
                 for gene_idx in range(self.num_genes):
+
+                    if type(self.init_range_low) in self.supported_int_float_types:
+                        range_min = self.init_range_low
+                        range_max = self.init_range_high
+                    else:
+                        range_min = self.init_range_low[gene_idx]
+                        range_max = self.init_range_high[gene_idx]
+
                     # A vector of all values of this single gene across all solutions in the population.
-                    gene_values = numpy.asarray(numpy.random.uniform(low=low, 
-                                                                     high=high, 
-                                                                     size=self.pop_size[0]), 
+                    gene_values = numpy.asarray(numpy.random.uniform(low=range_min,
+                                                                     high=range_max,
+                                                                     size=self.pop_size[0]),
                                                 dtype=self.gene_type[gene_idx][0])
                     # Adding the current gene values to the population.
                     self.population[:, gene_idx] = gene_values
 
             if allow_duplicate_genes == False:
                 for solution_idx in range(self.population.shape[0]):
                     # self.logger.info("Before", self.population[solution_idx])
                     self.population[solution_idx], _, _ = self.solve_duplicate_genes_randomly(solution=self.population[solution_idx],
-                                                                                              min_val=low, 
+                                                                                              min_val=low,
                                                                                               max_val=high,
                                                                                               mutation_by_replacement=True,
                                                                                               gene_type=gene_type,
                                                                                               num_trials=10)
                     # self.logger.info("After", self.population[solution_idx])
 
         elif self.gene_space_nested:
             if self.gene_type_single == True:
-                self.population = numpy.zeros(shape=self.pop_size, dtype=self.gene_type[0])
+                # Reaching this block means:
+                # 1) gene_space is nested (gene_space_nested is True).
+                # 2) gene_type is not nested (gene_type_single is True).
+                self.population = numpy.zeros(shape=self.pop_size,
+                                              dtype=self.gene_type[0])
                 for sol_idx in range(self.sol_per_pop):
                     for gene_idx in range(self.num_genes):
-                        if type(self.gene_space[gene_idx]) in [list, tuple, range]:
+
+                        if type(self.init_range_low) in self.supported_int_float_types:
+                            range_min = self.init_range_low
+                            range_max = self.init_range_high
+                        else:
+                            range_min = self.init_range_low[gene_idx]
+                            range_max = self.init_range_high[gene_idx]
+
+                        if self.gene_space[gene_idx] is None:
+
+                            # The following commented code replace the None value with a single number that will not change again.
+                            # This means the gene value will be the same across all solutions.
+                            # self.gene_space[gene_idx] = numpy.asarray(numpy.random.uniform(low=low,
+                            #                high=high,
+                            #                size=1), dtype=self.gene_type[0])[0]
+                            # self.population[sol_idx, gene_idx] = list(self.gene_space[gene_idx]).copy()
+
+                            # The above problem is solved by keeping the None value in the gene_space parameter. This forces PyGAD to generate this value for each solution.
+                            self.population[sol_idx, gene_idx] = numpy.asarray(numpy.random.uniform(low=range_min,
+                                                                                                    high=range_max,
+                                                                                                    size=1),
+                                                                               dtype=self.gene_type[0])[0]
+                        elif type(self.gene_space[gene_idx]) in [numpy.ndarray, list, tuple, range]:
                             # Check if the gene space has None values. If any, then replace it with randomly generated values according to the 3 attributes init_range_low, init_range_high, and gene_type.
                             if type(self.gene_space[gene_idx]) is range:
-                                temp = self.gene_space[gene_idx]
+                                temp_gene_space = self.gene_space[gene_idx]
                             else:
-                                temp = self.gene_space[gene_idx].copy()
+                                # Convert to list because tuple and range do not have copy().
+                                # We copy the gene_space to a temp variable to keep its original value.
+                                # In the next for loop, the gene_space is changed.
+                                # Later, the gene_space is restored to its original value using the temp variable.
+                                temp_gene_space = list(
+                                    self.gene_space[gene_idx]).copy()
+
                             for idx, val in enumerate(self.gene_space[gene_idx]):
                                 if val is None:
-                                    self.gene_space[gene_idx][idx] = numpy.asarray(numpy.random.uniform(low=low, 
-                                                                                                        high=high, 
-                                                                                                        size=1), 
+                                    self.gene_space[gene_idx][idx] = numpy.asarray(numpy.random.uniform(low=range_min,
+                                                                                                        high=range_max,
+                                                                                                        size=1),
                                                                                    dtype=self.gene_type[0])[0]
-                            self.population[sol_idx, gene_idx] = random.choice(self.gene_space[gene_idx])
-                            self.population[sol_idx, gene_idx] = self.gene_type[0](self.population[sol_idx, gene_idx])
-                            self.gene_space[gene_idx] = temp
+                            # Find the difference between the current gene space and the current values in the solution.
+                            unique_gene_values = list(set(self.gene_space[gene_idx]).difference(
+                                set(self.population[sol_idx, :gene_idx])))
+                            if len(unique_gene_values) > 0:
+                                self.population[sol_idx, gene_idx] = random.choice(unique_gene_values)
+                            else:
+                                # If there is no unique values, then we have to select a duplicate value.
+                                self.population[sol_idx, gene_idx] = random.choice(
+                                    self.gene_space[gene_idx])
+
+                            self.population[sol_idx, gene_idx] = self.gene_type[0](
+                                self.population[sol_idx, gene_idx])
+                            # Restore the gene_space from the temp_gene_space variable.
+                            self.gene_space[gene_idx] = list(
+                                temp_gene_space).copy()
                         elif type(self.gene_space[gene_idx]) is dict:
                             if 'step' in self.gene_space[gene_idx].keys():
                                 self.population[sol_idx, gene_idx] = numpy.asarray(numpy.random.choice(numpy.arange(start=self.gene_space[gene_idx]['low'],
                                                                                                                     stop=self.gene_space[gene_idx]['high'],
                                                                                                                     step=self.gene_space[gene_idx]['step']),
                                                                                                        size=1),
                                                                                    dtype=self.gene_type[0])[0]
                             else:
                                 self.population[sol_idx, gene_idx] = numpy.asarray(numpy.random.uniform(low=self.gene_space[gene_idx]['low'],
                                                                                                         high=self.gene_space[gene_idx]['high'],
                                                                                                         size=1),
                                                                                    dtype=self.gene_type[0])[0]
-                        elif type(self.gene_space[gene_idx]) == type(None):
-
-                            # The following commented code replace the None value with a single number that will not change again. 
-                            # This means the gene value will be the same across all solutions.
-                            # self.gene_space[gene_idx] = numpy.asarray(numpy.random.uniform(low=low,
-                            #                high=high, 
-                            #                size=1), dtype=self.gene_type[0])[0]
-                            # self.population[sol_idx, gene_idx] = self.gene_space[gene_idx].copy()
-                            
-                            # The above problem is solved by keeping the None value in the gene_space parameter. This forces PyGAD to generate this value for each solution.
-                            self.population[sol_idx, gene_idx] = numpy.asarray(numpy.random.uniform(low=low,
-                                                                                                    high=high, 
-                                                                                                    size=1), 
-                                                                               dtype=self.gene_type[0])[0]
                         elif type(self.gene_space[gene_idx]) in GA.supported_int_float_types:
                             self.population[sol_idx, gene_idx] = self.gene_space[gene_idx]
+                        else:
+                            # There is no more options.
+                            pass
             else:
-                self.population = numpy.zeros(shape=self.pop_size, dtype=object)
+                # Reaching this block means:
+                # 1) gene_space is nested (gene_space_nested is True).
+                # 2) gene_type is nested (gene_type_single is False).
+                self.population = numpy.zeros(shape=self.pop_size,
+                                              dtype=object)
                 for sol_idx in range(self.sol_per_pop):
                     for gene_idx in range(self.num_genes):
-                        if type(self.gene_space[gene_idx]) in [list, tuple, range]:
+
+                        if type(self.init_range_low) in self.supported_int_float_types:
+                            range_min = self.init_range_low
+                            range_max = self.init_range_high
+                        else:
+                            range_min = self.init_range_low[gene_idx]
+                            range_max = self.init_range_high[gene_idx]
+
+                        if type(self.gene_space[gene_idx]) in [numpy.ndarray, list, tuple, range]:
+                            # Convert to list because tuple and range do not have copy().
+                            # We copy the gene_space to a temp variable to keep its original value.
+                            # In the next for loop, the gene_space is changed.
+                            # Later, the gene_space is restored to its original value using the temp variable.
+                            temp_gene_space = list(self.gene_space[gene_idx]).copy()
+
                             # Check if the gene space has None values. If any, then replace it with randomly generated values according to the 3 attributes init_range_low, init_range_high, and gene_type.
-                            temp = self.gene_space[gene_idx].copy()
                             for idx, val in enumerate(self.gene_space[gene_idx]):
                                 if val is None:
-                                    self.gene_space[gene_idx][idx] = numpy.asarray(numpy.random.uniform(low=low, 
-                                                                                                        high=high, 
-                                                                                                        size=1), 
+                                    self.gene_space[gene_idx][idx] = numpy.asarray(numpy.random.uniform(low=range_min,
+                                                                                                        high=range_max,
+                                                                                                        size=1),
                                                                                    dtype=self.gene_type[gene_idx][0])[0]
+
                             self.population[sol_idx, gene_idx] = random.choice(self.gene_space[gene_idx])
                             self.population[sol_idx, gene_idx] = self.gene_type[gene_idx][0](self.population[sol_idx, gene_idx])
-                            self.gene_space[gene_idx] = temp.copy()
+                            # Restore the gene_space from the temp_gene_space variable.
+                            self.gene_space[gene_idx] = temp_gene_space.copy()
                         elif type(self.gene_space[gene_idx]) is dict:
                             if 'step' in self.gene_space[gene_idx].keys():
                                 self.population[sol_idx, gene_idx] = numpy.asarray(numpy.random.choice(numpy.arange(start=self.gene_space[gene_idx]['low'],
                                                                                                                     stop=self.gene_space[gene_idx]['high'],
                                                                                                                     step=self.gene_space[gene_idx]['step']),
                                                                                                        size=1),
                                                                                    dtype=self.gene_type[gene_idx][0])[0]
                             else:
                                 self.population[sol_idx, gene_idx] = numpy.asarray(numpy.random.uniform(low=self.gene_space[gene_idx]['low'],
                                                                                                         high=self.gene_space[gene_idx]['high'],
-                                                                                                        size=1), 
+                                                                                                        size=1),
                                                                                    dtype=self.gene_type[gene_idx][0])[0]
                         elif type(self.gene_space[gene_idx]) == type(None):
-                            # self.gene_space[gene_idx] = numpy.asarray(numpy.random.uniform(low=low,
-                            #                                                                high=high, 
-                            #                                                                size=1), 
-                            #                                           dtype=self.gene_type[gene_idx][0])[0]
-
-                            # self.population[sol_idx, gene_idx] = self.gene_space[gene_idx].copy()
-
-                            temp = numpy.asarray(numpy.random.uniform(low=low,
-                                                                      high=high, 
-                                                                      size=1), 
-                                                 dtype=self.gene_type[gene_idx][0])[0]
-                            self.population[sol_idx, gene_idx] = temp
+                            temp_gene_value = numpy.asarray(numpy.random.uniform(low=range_min,
+                                                                                 high=range_max,
+                                                                                 size=1),
+                                                            dtype=self.gene_type[gene_idx][0])[0]
+
+                            self.population[sol_idx, gene_idx] = temp_gene_value.copy()
                         elif type(self.gene_space[gene_idx]) in GA.supported_int_float_types:
                             self.population[sol_idx, gene_idx] = self.gene_space[gene_idx]
+                        else:
+                            # There is no more options.
+                            pass
         else:
+            # Handle the non-nested gene_space. It can be assigned a numeric value, list, numpy.ndarray, or a dict.
             if self.gene_type_single == True:
+                # Reaching this block means:
+                # 1) gene_space is not nested (gene_space_nested is False).
+                # 2) gene_type is not nested (gene_type_single is True).
+
                 # Replace all the None values with random values using the init_range_low, init_range_high, and gene_type attributes.
-                for idx, curr_gene_space in enumerate(self.gene_space):
+                for gene_idx, curr_gene_space in enumerate(self.gene_space):
+
+                    if type(self.init_range_low) in self.supported_int_float_types:
+                        range_min = self.init_range_low
+                        range_max = self.init_range_high
+                    else:
+                        range_min = self.init_range_low[gene_idx]
+                        range_max = self.init_range_high[gene_idx]
+
                     if curr_gene_space is None:
-                        self.gene_space[idx] = numpy.asarray(numpy.random.uniform(low=low, 
-                                                                                  high=high, 
-                                                                                  size=1), 
-                                                             dtype=self.gene_type[0])[0]
-    
+                        self.gene_space[gene_idx] = numpy.asarray(numpy.random.uniform(low=range_min,
+                                                                                       high=range_max,
+                                                                                       size=1),
+                                                                  dtype=self.gene_type[0])[0]
+
                 # Creating the initial population by randomly selecting the genes' values from the values inside the 'gene_space' parameter.
                 if type(self.gene_space) is dict:
                     if 'step' in self.gene_space.keys():
                         self.population = numpy.asarray(numpy.random.choice(numpy.arange(start=self.gene_space['low'],
                                                                                          stop=self.gene_space['high'],
                                                                                          step=self.gene_space['step']),
                                                                             size=self.pop_size),
                                                         dtype=self.gene_type[0])
                     else:
                         self.population = numpy.asarray(numpy.random.uniform(low=self.gene_space['low'],
                                                                              high=self.gene_space['high'],
                                                                              size=self.pop_size),
-                                                        dtype=self.gene_type[0]) # A NumPy array holding the initial population.
+                                                        dtype=self.gene_type[0])  # A NumPy array holding the initial population.
                 else:
                     self.population = numpy.asarray(numpy.random.choice(self.gene_space,
                                                                         size=self.pop_size),
-                                                    dtype=self.gene_type[0]) # A NumPy array holding the initial population.
+                                                    dtype=self.gene_type[0])  # A NumPy array holding the initial population.
             else:
-                # Replace all the None values with random values using the init_range_low, init_range_high, and gene_type attributes.
-                for gene_idx, curr_gene_space in enumerate(self.gene_space):
-                    if curr_gene_space is None:
-                        self.gene_space[gene_idx] = numpy.asarray(numpy.random.uniform(low=low, 
-                                                                                  high=high, 
-                                                                                  size=1), 
-                                                             dtype=self.gene_type[gene_idx][0])[0]
-    
+                # Reaching this block means:
+                # 1) gene_space is not nested (gene_space_nested is False).
+                # 2) gene_type is nested (gene_type_single is False).
+
                 # Creating the initial population by randomly selecting the genes' values from the values inside the 'gene_space' parameter.
                 if type(self.gene_space) is dict:
                     # Create an empty population of dtype=object to support storing mixed data types within the same array.
-                    self.population = numpy.zeros(shape=self.pop_size, dtype=object)
+                    self.population = numpy.zeros(shape=self.pop_size,
+                                                  dtype=object)
                     # Loop through the genes, randomly generate the values of a single gene across the entire population, and add the values of each gene to the population.
                     for gene_idx in range(self.num_genes):
+                        # Generate the values of the current gene across all solutions.
                         # A vector of all values of this single gene across all solutions in the population.
-                        if 'step' in self.gene_space[gene_idx].keys():
-                            gene_values = numpy.asarray(numpy.random.choice(numpy.arange(start=self.gene_space[gene_idx]['low'],
-                                                                                         stop=self.gene_space[gene_idx]['high'],
-                                                                                         step=self.gene_space[gene_idx]['step']),
+                        if 'step' in self.gene_space.keys():
+                            gene_values = numpy.asarray(numpy.random.choice(numpy.arange(start=self.gene_space['low'],
+                                                                                         stop=self.gene_space['high'],
+                                                                                         step=self.gene_space['step']),
                                                                             size=self.pop_size[0]),
                                                         dtype=self.gene_type[gene_idx][0])
                         else:
-                            gene_values = numpy.asarray(numpy.random.uniform(low=self.gene_space['low'], 
-                                                                             high=self.gene_space['high'], 
-                                                                             size=self.pop_size[0]), 
+                            gene_values = numpy.asarray(numpy.random.uniform(low=self.gene_space['low'],
+                                                                             high=self.gene_space['high'],
+                                                                             size=self.pop_size[0]),
                                                         dtype=self.gene_type[gene_idx][0])
                         # Adding the current gene values to the population.
                         self.population[:, gene_idx] = gene_values
-        
+
                 else:
+                    # Reaching this block means that the gene_space is not None or dict.
+                    # It can be either range, numpy.ndarray, or list.
+
                     # Create an empty population of dtype=object to support storing mixed data types within the same array.
                     self.population = numpy.zeros(shape=self.pop_size, dtype=object)
                     # Loop through the genes, randomly generate the values of a single gene across the entire population, and add the values of each gene to the population.
                     for gene_idx in range(self.num_genes):
                         # A vector of all values of this single gene across all solutions in the population.
-                        gene_values = numpy.asarray(numpy.random.choice(self.gene_space, 
-                                                                        size=self.pop_size[0]), 
+                        gene_values = numpy.asarray(numpy.random.choice(self.gene_space,
+                                                                        size=self.pop_size[0]),
                                                     dtype=self.gene_type[gene_idx][0])
                         # Adding the current gene values to the population.
                         self.population[:, gene_idx] = gene_values
 
         if not (self.gene_space is None):
             if allow_duplicate_genes == False:
                 for sol_idx in range(self.population.shape[0]):
@@ -1478,517 +1605,597 @@
                                                                                          num_trials=10,
                                                                                          build_initial_pop=True)
 
         # Keeping the initial population in the initial_population attribute.
         self.initial_population = self.population.copy()
 
     def cal_pop_fitness(self):
-
         """
         Calculating the fitness values of batches of solutions in the current population. 
         It returns:
             -fitness: An array of the calculated fitness values.
         """
-
-        if self.valid_parameters == False:
-            self.logger.error("ERROR calling the cal_pop_fitness() method: \nPlease check the parameters passed while creating an instance of the GA class.\n")
-            raise Exception("ERROR calling the cal_pop_fitness() method: \nPlease check the parameters passed while creating an instance of the GA class.\n")
-
-        # 'last_generation_parents_as_list' is the list version of 'self.last_generation_parents'
-        # It is used to return the parent index using the 'in' membership operator of Python lists. This is much faster than using 'numpy.where()'.
-        if self.last_generation_parents is not None:
-            last_generation_parents_as_list = [list(gen_parent) for gen_parent in self.last_generation_parents]
-
-        # 'last_generation_elitism_as_list' is the list version of 'self.last_generation_elitism'
-        # It is used to return the elitism index using the 'in' membership operator of Python lists. This is much faster than using 'numpy.where()'.
-        if self.last_generation_elitism is not None:
-            last_generation_elitism_as_list = [list(gen_elitism) for gen_elitism in self.last_generation_elitism]
-
-        pop_fitness = ["undefined"] * len(self.population)
-        if self.parallel_processing is None:
-            # Calculating the fitness value of each solution in the current population.
-            for sol_idx, sol in enumerate(self.population):
-                # Check if the `save_solutions` parameter is `True` and whether the solution already exists in the `solutions` list. If so, use its fitness rather than calculating it again.
-                # The functions numpy.any()/numpy.all()/numpy.where()/numpy.equal() are very slow.
-                # So, list membership operator 'in' is used to check if the solution exists in the 'self.solutions' list.
-                # Make sure that both the solution and 'self.solutions' are of type 'list' not 'numpy.ndarray'.
-                # if (self.save_solutions) and (len(self.solutions) > 0) and (numpy.any(numpy.all(self.solutions == numpy.array(sol), axis=1))):
-                # if (self.save_solutions) and (len(self.solutions) > 0) and (numpy.any(numpy.all(numpy.equal(self.solutions, numpy.array(sol)), axis=1))):
-                if (self.save_solutions) and (len(self.solutions) > 0) and (list(sol) in self.solutions):
-                    solution_idx = self.solutions.index(list(sol))
-                    fitness = self.solutions_fitness[solution_idx]
-                elif (self.keep_elitism > 0) and (self.last_generation_elitism is not None) and (len(self.last_generation_elitism) > 0) and (list(sol) in last_generation_elitism_as_list):
-                    # Return the index of the elitism from the elitism array 'self.last_generation_elitism'.
-                    # This is not its index within the population. It is just its index in the 'self.last_generation_elitism' array.
-                    elitism_idx = last_generation_elitism_as_list.index(list(sol))
-                    # Use the returned elitism index to return its index in the last population.
-                    elitism_idx = self.last_generation_elitism_indices[elitism_idx]
-                    # Use the elitism's index to return its pre-calculated fitness value.
-                    fitness = self.previous_generation_fitness[elitism_idx]
-                # If the solutions are not saved (i.e. `save_solutions=False`), check if this solution is a parent from the previous generation and its fitness value is already calculated. If so, use the fitness value instead of calling the fitness function.
-                # We cannot use the `numpy.where()` function directly because it does not support the `axis` parameter. This is why the `numpy.all()` function is used to match the solutions on axis=1.
-                # elif (self.last_generation_parents is not None) and len(numpy.where(numpy.all(self.last_generation_parents == sol, axis=1))[0] > 0):
-                elif ((self.keep_parents == -1) or (self.keep_parents > 0)) and (self.last_generation_parents is not None) and (len(self.last_generation_parents) > 0) and (list(sol) in last_generation_parents_as_list):
-                    # Index of the parent in the 'self.last_generation_parents' array. 
-                    # This is not its index within the population. It is just its index in the 'self.last_generation_parents' array.
-                    # parent_idx = numpy.where(numpy.all(self.last_generation_parents == sol, axis=1))[0][0]
-                    parent_idx = last_generation_parents_as_list.index(list(sol))
-                    # Use the returned parent index to return its index in the last population.
-                    parent_idx = self.last_generation_parents_indices[parent_idx]
-                    # Use the parent's index to return its pre-calculated fitness value.
-                    fitness = self.previous_generation_fitness[parent_idx]
-                else:
-                    # Check if batch processing is used. If not, then calculate this missing fitness value.
-                    if self.fitness_batch_size in [1, None]:
-                        fitness = self.fitness_func(self, sol, sol_idx)
-                        if type(fitness) in GA.supported_int_float_types:
-                            pass
-                        else:
-                            self.logger.error("The fitness function should return a number but the value {fit_val} of type {fit_type} found.".format(fit_val=fitness, fit_type=type(fitness)))
-                            raise ValueError("The fitness function should return a number but the value {fit_val} of type {fit_type} found.".format(fit_val=fitness, fit_type=type(fitness)))
+        try:
+            if self.valid_parameters == False:
+                raise Exception("ERROR calling the cal_pop_fitness() method: \nPlease check the parameters passed while creating an instance of the GA class.\n")
+
+            # 'last_generation_parents_as_list' is the list version of 'self.last_generation_parents'
+            # It is used to return the parent index using the 'in' membership operator of Python lists. This is much faster than using 'numpy.where()'.
+            if self.last_generation_parents is not None:
+                last_generation_parents_as_list = [
+                    list(gen_parent) for gen_parent in self.last_generation_parents]
+
+            # 'last_generation_elitism_as_list' is the list version of 'self.last_generation_elitism'
+            # It is used to return the elitism index using the 'in' membership operator of Python lists. This is much faster than using 'numpy.where()'.
+            if self.last_generation_elitism is not None:
+                last_generation_elitism_as_list = [
+                    list(gen_elitism) for gen_elitism in self.last_generation_elitism]
+
+            pop_fitness = ["undefined"] * len(self.population)
+            if self.parallel_processing is None:
+                # Calculating the fitness value of each solution in the current population.
+                for sol_idx, sol in enumerate(self.population):
+                    # Check if the `save_solutions` parameter is `True` and whether the solution already exists in the `solutions` list. If so, use its fitness rather than calculating it again.
+                    # The functions numpy.any()/numpy.all()/numpy.where()/numpy.equal() are very slow.
+                    # So, list membership operator 'in' is used to check if the solution exists in the 'self.solutions' list.
+                    # Make sure that both the solution and 'self.solutions' are of type 'list' not 'numpy.ndarray'.
+                    # if (self.save_solutions) and (len(self.solutions) > 0) and (numpy.any(numpy.all(self.solutions == numpy.array(sol), axis=1))):
+                    # if (self.save_solutions) and (len(self.solutions) > 0) and (numpy.any(numpy.all(numpy.equal(self.solutions, numpy.array(sol)), axis=1))):
+                    if (self.save_solutions) and (len(self.solutions) > 0) and (list(sol) in self.solutions):
+                        solution_idx = self.solutions.index(list(sol))
+                        fitness = self.solutions_fitness[solution_idx]
+                    elif (self.keep_elitism > 0) and (self.last_generation_elitism is not None) and (len(self.last_generation_elitism) > 0) and (list(sol) in last_generation_elitism_as_list):
+                        # Return the index of the elitism from the elitism array 'self.last_generation_elitism'.
+                        # This is not its index within the population. It is just its index in the 'self.last_generation_elitism' array.
+                        elitism_idx = last_generation_elitism_as_list.index(list(sol))
+                        # Use the returned elitism index to return its index in the last population.
+                        elitism_idx = self.last_generation_elitism_indices[elitism_idx]
+                        # Use the elitism's index to return its pre-calculated fitness value.
+                        fitness = self.previous_generation_fitness[elitism_idx]
+                    # If the solutions are not saved (i.e. `save_solutions=False`), check if this solution is a parent from the previous generation and its fitness value is already calculated. If so, use the fitness value instead of calling the fitness function.
+                    # We cannot use the `numpy.where()` function directly because it does not support the `axis` parameter. This is why the `numpy.all()` function is used to match the solutions on axis=1.
+                    # elif (self.last_generation_parents is not None) and len(numpy.where(numpy.all(self.last_generation_parents == sol, axis=1))[0] > 0):
+                    elif ((self.keep_parents == -1) or (self.keep_parents > 0)) and (self.last_generation_parents is not None) and (len(self.last_generation_parents) > 0) and (list(sol) in last_generation_parents_as_list):
+                        # Index of the parent in the 'self.last_generation_parents' array.
+                        # This is not its index within the population. It is just its index in the 'self.last_generation_parents' array.
+                        # parent_idx = numpy.where(numpy.all(self.last_generation_parents == sol, axis=1))[0][0]
+                        parent_idx = last_generation_parents_as_list.index(list(sol))
+                        # Use the returned parent index to return its index in the last population.
+                        parent_idx = self.last_generation_parents_indices[parent_idx]
+                        # Use the parent's index to return its pre-calculated fitness value.
+                        fitness = self.previous_generation_fitness[parent_idx]
                     else:
-                        # Reaching this point means that batch processing is in effect to calculate the fitness values.
-                        # Do not continue the loop as no fitness is calculated. The fitness will be calculated later in batch mode.
-                        continue
-
-                # This is only executed if the fitness value was already calculated.
-                pop_fitness[sol_idx] = fitness
-
-            if self.fitness_batch_size not in [1, None]:
-                # Reaching this block means that batch fitness calculation is used.
-
-                # Indices of the solutions to calculate their fitness.
-                solutions_indices = numpy.where(numpy.array(pop_fitness) == "undefined")[0]
-                # Number of batches.
-                num_batches = int(numpy.ceil(len(solutions_indices) / self.fitness_batch_size))
-                # For each batch, get its indices and call the fitness function.
-                for batch_idx in range(num_batches):
-                    batch_first_index = batch_idx * self.fitness_batch_size
-                    batch_last_index = (batch_idx + 1) * self.fitness_batch_size
-                    batch_indices = solutions_indices[batch_first_index:batch_last_index]
-                    batch_solutions = self.population[batch_indices, :]
-
-                    batch_fitness = self.fitness_func(self, batch_solutions, batch_indices)
-                    if type(batch_fitness) not in [list, tuple, numpy.ndarray]:
-                        self.logger.error("Expected to receive a list, tuple, or numpy.ndarray from the fitness function but the value ({batch_fitness}) of type {batch_fitness_type}.".format(batch_fitness=batch_fitness, batch_fitness_type=type(batch_fitness)))
-                        raise TypeError("Expected to receive a list, tuple, or numpy.ndarray from the fitness function but the value ({batch_fitness}) of type {batch_fitness_type}.".format(batch_fitness=batch_fitness, batch_fitness_type=type(batch_fitness)))
-                    elif len(numpy.array(batch_fitness)) != len(batch_indices):
-                        self.logger.error("There is a mismatch between the number of solutions passed to the fitness function ({batch_indices_len}) and the number of fitness values returned ({batch_fitness_len}). They must match.".format(batch_fitness_len=len(batch_fitness), batch_indices_len=len(batch_indices)))
-                        raise ValueError("There is a mismatch between the number of solutions passed to the fitness function ({batch_indices_len}) and the number of fitness values returned ({batch_fitness_len}). They must match.".format(batch_fitness_len=len(batch_fitness), batch_indices_len=len(batch_indices)))
-
-                    for index, fitness in zip(batch_indices, batch_fitness):
-                        if type(fitness) in GA.supported_int_float_types:
-                            pop_fitness[index] = fitness
+                        # Check if batch processing is used. If not, then calculate this missing fitness value.
+                        if self.fitness_batch_size in [1, None]:
+                            fitness = self.fitness_func(self, sol, sol_idx)
+                            if type(fitness) in GA.supported_int_float_types:
+                                pass
+                            else:
+                                raise ValueError(f"The fitness function should return a number but the value {fitness} of type {type(fitness)} found.")
                         else:
-                            self.logger.error("The fitness function should return a number but the value {fit_val} of type {fit_type} found.".format(fit_val=fitness, fit_type=type(fitness)))
-                            raise ValueError("The fitness function should return a number but the value {fit_val} of type {fit_type} found.".format(fit_val=fitness, fit_type=type(fitness)))
-        else:
-            # Calculating the fitness value of each solution in the current population.
-            for sol_idx, sol in enumerate(self.population):
-                # Check if the `save_solutions` parameter is `True` and whether the solution already exists in the `solutions` list. If so, use its fitness rather than calculating it again.
-                # The functions numpy.any()/numpy.all()/numpy.where()/numpy.equal() are very slow.
-                # So, list membership operator 'in' is used to check if the solution exists in the 'self.solutions' list.
-                # Make sure that both the solution and 'self.solutions' are of type 'list' not 'numpy.ndarray'.
-                if (self.save_solutions) and (len(self.solutions) > 0) and (list(sol) in self.solutions):
-                    solution_idx = self.solutions.index(list(sol))
-                    fitness = self.solutions_fitness[solution_idx]
-                    pop_fitness[sol_idx] = fitness
-                elif (self.keep_elitism > 0) and (self.last_generation_elitism is not None) and (len(self.last_generation_elitism) > 0) and (list(sol) in last_generation_elitism_as_list):
-                    # Return the index of the elitism from the elitism array 'self.last_generation_elitism'.
-                    # This is not its index within the population. It is just its index in the 'self.last_generation_elitism' array.
-                    elitism_idx = last_generation_elitism_as_list.index(list(sol))
-                    # Use the returned elitism index to return its index in the last population.
-                    elitism_idx = self.last_generation_elitism_indices[elitism_idx]
-                    # Use the elitism's index to return its pre-calculated fitness value.
-                    fitness = self.previous_generation_fitness[elitism_idx]
+                            # Reaching this point means that batch processing is in effect to calculate the fitness values.
+                            # Do not continue the loop as no fitness is calculated. The fitness will be calculated later in batch mode.
+                            continue
 
+                    # This is only executed if the fitness value was already calculated.
                     pop_fitness[sol_idx] = fitness
-                # If the solutions are not saved (i.e. `save_solutions=False`), check if this solution is a parent from the previous generation and its fitness value is already calculated. If so, use the fitness value instead of calling the fitness function.
-                # We cannot use the `numpy.where()` function directly because it does not support the `axis` parameter. This is why the `numpy.all()` function is used to match the solutions on axis=1.
-                # elif (self.last_generation_parents is not None) and len(numpy.where(numpy.all(self.last_generation_parents == sol, axis=1))[0] > 0):
-                elif ((self.keep_parents == -1) or (self.keep_parents > 0)) and (self.last_generation_parents is not None) and (len(self.last_generation_parents) > 0) and (list(sol) in last_generation_parents_as_list):
-                    # Index of the parent in the 'self.last_generation_parents' array. 
-                    # This is not its index within the population. It is just its index in the 'self.last_generation_parents' array.
-                    # parent_idx = numpy.where(numpy.all(self.last_generation_parents == sol, axis=1))[0][0]
-                    parent_idx = last_generation_parents_as_list.index(list(sol))
-                    # Use the returned parent index to return its index in the last population.
-                    parent_idx = self.last_generation_parents_indices[parent_idx]
-                    # Use the parent's index to return its pre-calculated fitness value.
-                    fitness = self.previous_generation_fitness[parent_idx]
 
-                    pop_fitness[sol_idx] = fitness
-
-            # Decide which class to use based on whether the user selected "process" or "thread"
-            if self.parallel_processing[0] == "process":
-                ExecutorClass = concurrent.futures.ProcessPoolExecutor
-            else:
-                ExecutorClass = concurrent.futures.ThreadPoolExecutor
-
-            # We can use a with statement to ensure threads are cleaned up promptly (https://docs.python.org/3/library/concurrent.futures.html#threadpoolexecutor-example)
-            with ExecutorClass(max_workers=self.parallel_processing[1]) as executor:
-                solutions_to_submit_indices = []
-                solutions_to_submit = []
-                for sol_idx, sol in enumerate(self.population):
-                    # The "undefined" value means that the fitness of this solution must be calculated.
-                    if pop_fitness[sol_idx] == "undefined":
-                        solutions_to_submit.append(sol.copy())
-                        solutions_to_submit_indices.append(sol_idx)
-
-                # Check if batch processing is used. If not, then calculate the fitness value for individual solutions.
-                if self.fitness_batch_size in [1, None]:
-                    for index, fitness in zip(solutions_to_submit_indices, executor.map(self.fitness_func, [self]*len(solutions_to_submit_indices), solutions_to_submit, solutions_to_submit_indices)):
-                        if type(fitness) in GA.supported_int_float_types:
-                            pop_fitness[index] = fitness
-                        else:
-                            self.logger.error("The fitness function should return a number but the value {fit_val} of type {fit_type} found.".format(fit_val=fitness, fit_type=type(fitness)))
-                            raise ValueError("The fitness function should return a number but the value {fit_val} of type {fit_type} found.".format(fit_val=fitness, fit_type=type(fitness)))
-                else:
-                    # Reaching this block means that batch processing is used. The fitness values are calculated in batches.
+                if self.fitness_batch_size not in [1, None]:
+                    # Reaching this block means that batch fitness calculation is used.
 
+                    # Indices of the solutions to calculate their fitness.
+                    solutions_indices = numpy.where(
+                        numpy.array(pop_fitness) == "undefined")[0]
                     # Number of batches.
-                    num_batches = int(numpy.ceil(len(solutions_to_submit_indices) / self.fitness_batch_size))
-                    # Each element of the `batches_solutions` list represents the solutions in one batch.
-                    batches_solutions = []
-                    # Each element of the `batches_indices` list represents the solutions' indices in one batch.
-                    batches_indices = []
+                    num_batches = int(numpy.ceil(len(solutions_indices) / self.fitness_batch_size))
                     # For each batch, get its indices and call the fitness function.
                     for batch_idx in range(num_batches):
                         batch_first_index = batch_idx * self.fitness_batch_size
                         batch_last_index = (batch_idx + 1) * self.fitness_batch_size
-                        batch_indices = solutions_to_submit_indices[batch_first_index:batch_last_index]
+                        batch_indices = solutions_indices[batch_first_index:batch_last_index]
                         batch_solutions = self.population[batch_indices, :]
 
-                        batches_solutions.append(batch_solutions)
-                        batches_indices.append(batch_indices)
-
-                    for batch_indices, batch_fitness in zip(batches_indices, executor.map(self.fitness_func, [self]*len(solutions_to_submit_indices), batches_solutions, batches_indices)):
+                        batch_fitness = self.fitness_func(
+                            self, batch_solutions, batch_indices)
                         if type(batch_fitness) not in [list, tuple, numpy.ndarray]:
-                            self.logger.error("Expected to receive a list, tuple, or numpy.ndarray from the fitness function but the value ({batch_fitness}) of type {batch_fitness_type}.".format(batch_fitness=batch_fitness, batch_fitness_type=type(batch_fitness)))
-                            raise TypeError("Expected to receive a list, tuple, or numpy.ndarray from the fitness function but the value ({batch_fitness}) of type {batch_fitness_type}.".format(batch_fitness=batch_fitness, batch_fitness_type=type(batch_fitness)))
+                            raise TypeError(f"Expected to receive a list, tuple, or numpy.ndarray from the fitness function but the value ({batch_fitness}) of type {type(batch_fitness)}.")
                         elif len(numpy.array(batch_fitness)) != len(batch_indices):
-                            self.logger.error("There is a mismatch between the number of solutions passed to the fitness function ({batch_indices_len}) and the number of fitness values returned ({batch_fitness_len}). They must match.".format(batch_fitness_len=len(batch_fitness), batch_indices_len=len(batch_indices)))
-                            raise ValueError("There is a mismatch between the number of solutions passed to the fitness function ({batch_indices_len}) and the number of fitness values returned ({batch_fitness_len}). They must match.".format(batch_fitness_len=len(batch_fitness), batch_indices_len=len(batch_indices)))
+                            raise ValueError(f"There is a mismatch between the number of solutions passed to the fitness function ({len(batch_indices)}) and the number of fitness values returned ({len(batch_fitness)}). They must match.")
 
                         for index, fitness in zip(batch_indices, batch_fitness):
                             if type(fitness) in GA.supported_int_float_types:
                                 pop_fitness[index] = fitness
                             else:
-                                self.logger.error("The fitness function should return a number but the value ({fit_val}) of type {fit_type} found.".format(fit_val=fitness, fit_type=type(fitness)))
-                                raise ValueError("The fitness function should return a number but the value ({fit_val}) of type {fit_type} found.".format(fit_val=fitness, fit_type=type(fitness)))
+                                raise ValueError(f"The fitness function should return a number but the value {fitness} of type {type(fitness)} found.")
+            else:
+                # Calculating the fitness value of each solution in the current population.
+                for sol_idx, sol in enumerate(self.population):
+                    # Check if the `save_solutions` parameter is `True` and whether the solution already exists in the `solutions` list. If so, use its fitness rather than calculating it again.
+                    # The functions numpy.any()/numpy.all()/numpy.where()/numpy.equal() are very slow.
+                    # So, list membership operator 'in' is used to check if the solution exists in the 'self.solutions' list.
+                    # Make sure that both the solution and 'self.solutions' are of type 'list' not 'numpy.ndarray'.
+                    if (self.save_solutions) and (len(self.solutions) > 0) and (list(sol) in self.solutions):
+                        solution_idx = self.solutions.index(list(sol))
+                        fitness = self.solutions_fitness[solution_idx]
+                        pop_fitness[sol_idx] = fitness
+                    elif (self.keep_elitism > 0) and (self.last_generation_elitism is not None) and (len(self.last_generation_elitism) > 0) and (list(sol) in last_generation_elitism_as_list):
+                        # Return the index of the elitism from the elitism array 'self.last_generation_elitism'.
+                        # This is not its index within the population. It is just its index in the 'self.last_generation_elitism' array.
+                        elitism_idx = last_generation_elitism_as_list.index(
+                            list(sol))
+                        # Use the returned elitism index to return its index in the last population.
+                        elitism_idx = self.last_generation_elitism_indices[elitism_idx]
+                        # Use the elitism's index to return its pre-calculated fitness value.
+                        fitness = self.previous_generation_fitness[elitism_idx]
+
+                        pop_fitness[sol_idx] = fitness
+                    # If the solutions are not saved (i.e. `save_solutions=False`), check if this solution is a parent from the previous generation and its fitness value is already calculated. If so, use the fitness value instead of calling the fitness function.
+                    # We cannot use the `numpy.where()` function directly because it does not support the `axis` parameter. This is why the `numpy.all()` function is used to match the solutions on axis=1.
+                    # elif (self.last_generation_parents is not None) and len(numpy.where(numpy.all(self.last_generation_parents == sol, axis=1))[0] > 0):
+                    elif ((self.keep_parents == -1) or (self.keep_parents > 0)) and (self.last_generation_parents is not None) and (len(self.last_generation_parents) > 0) and (list(sol) in last_generation_parents_as_list):
+                        # Index of the parent in the 'self.last_generation_parents' array.
+                        # This is not its index within the population. It is just its index in the 'self.last_generation_parents' array.
+                        # parent_idx = numpy.where(numpy.all(self.last_generation_parents == sol, axis=1))[0][0]
+                        parent_idx = last_generation_parents_as_list.index(
+                            list(sol))
+                        # Use the returned parent index to return its index in the last population.
+                        parent_idx = self.last_generation_parents_indices[parent_idx]
+                        # Use the parent's index to return its pre-calculated fitness value.
+                        fitness = self.previous_generation_fitness[parent_idx]
+
+                        pop_fitness[sol_idx] = fitness
+
+                # Decide which class to use based on whether the user selected "process" or "thread"
+                if self.parallel_processing[0] == "process":
+                    ExecutorClass = concurrent.futures.ProcessPoolExecutor
+                else:
+                    ExecutorClass = concurrent.futures.ThreadPoolExecutor
+
+                # We can use a with statement to ensure threads are cleaned up promptly (https://docs.python.org/3/library/concurrent.futures.html#threadpoolexecutor-example)
+                with ExecutorClass(max_workers=self.parallel_processing[1]) as executor:
+                    solutions_to_submit_indices = []
+                    solutions_to_submit = []
+                    for sol_idx, sol in enumerate(self.population):
+                        # The "undefined" value means that the fitness of this solution must be calculated.
+                        if pop_fitness[sol_idx] == "undefined":
+                            solutions_to_submit.append(sol.copy())
+                            solutions_to_submit_indices.append(sol_idx)
 
-        pop_fitness = numpy.array(pop_fitness)
+                    # Check if batch processing is used. If not, then calculate the fitness value for individual solutions.
+                    if self.fitness_batch_size in [1, None]:
+                        for index, fitness in zip(solutions_to_submit_indices, executor.map(self.fitness_func, [self]*len(solutions_to_submit_indices), solutions_to_submit, solutions_to_submit_indices)):
+                            if type(fitness) in GA.supported_int_float_types:
+                                pop_fitness[index] = fitness
+                            else:
+                                raise ValueError(f"The fitness function should return a number but the value {fitness} of type {type(fitness)} found.")
+                    else:
+                        # Reaching this block means that batch processing is used. The fitness values are calculated in batches.
+
+                        # Number of batches.
+                        num_batches = int(numpy.ceil(len(solutions_to_submit_indices) / self.fitness_batch_size))
+                        # Each element of the `batches_solutions` list represents the solutions in one batch.
+                        batches_solutions = []
+                        # Each element of the `batches_indices` list represents the solutions' indices in one batch.
+                        batches_indices = []
+                        # For each batch, get its indices and call the fitness function.
+                        for batch_idx in range(num_batches):
+                            batch_first_index = batch_idx * self.fitness_batch_size
+                            batch_last_index = (batch_idx + 1) * self.fitness_batch_size
+                            batch_indices = solutions_to_submit_indices[batch_first_index:batch_last_index]
+                            batch_solutions = self.population[batch_indices, :]
+
+                            batches_solutions.append(batch_solutions)
+                            batches_indices.append(batch_indices)
+
+                        for batch_indices, batch_fitness in zip(batches_indices, executor.map(self.fitness_func, [self]*len(solutions_to_submit_indices), batches_solutions, batches_indices)):
+                            if type(batch_fitness) not in [list, tuple, numpy.ndarray]:
+                                raise TypeError(f"Expected to receive a list, tuple, or numpy.ndarray from the fitness function but the value ({batch_fitness}) of type {type(batch_fitness)}.")
+                            elif len(numpy.array(batch_fitness)) != len(batch_indices):
+                                
+                                raise ValueError(f"There is a mismatch between the number of solutions passed to the fitness function ({len(batch_indices)}) and the number of fitness values returned ({len(batch_fitness)}). They must match.")
+
+                            for index, fitness in zip(batch_indices, batch_fitness):
+                                if type(fitness) in GA.supported_int_float_types:
+                                    pop_fitness[index] = fitness
+                                else:
+                                    raise ValueError(f"The fitness function should return a number but the value ({fitness}) of type {type(fitness)} found.")
 
+            pop_fitness = numpy.array(pop_fitness)
+        except Exception as ex:
+            self.logger.exception(ex)
+            sys.exit(-1)
         return pop_fitness
 
     def run(self):
-
         """
         Runs the genetic algorithm. This is the main method in which the genetic algorithm is evolved through a number of generations.
         """
+        try:
+            if self.valid_parameters == False:
+                raise Exception("Error calling the run() method: \nThe run() method cannot be executed with invalid parameters. Please check the parameters passed while creating an instance of the GA class.\n")
+
+            # Starting from PyGAD 2.18.0, the 4 properties (best_solutions, best_solutions_fitness, solutions, and solutions_fitness) are no longer reset with each call to the run() method. Instead, they are extended.
+            # For example, if there are 50 generations and the user set save_best_solutions=True, then the length of the 2 properties best_solutions and best_solutions_fitness will be 50 after the first call to the run() method, then 100 after the second call, 150 after the third, and so on.
+
+            # self.best_solutions: Holds the best solution in each generation.
+            if type(self.best_solutions) is numpy.ndarray:
+                self.best_solutions = list(self.best_solutions)
+            # self.best_solutions_fitness: A list holding the fitness value of the best solution for each generation.
+            if type(self.best_solutions_fitness) is numpy.ndarray:
+                self.best_solutions_fitness = list(self.best_solutions_fitness)
+            # self.solutions: Holds the solutions in each generation.
+            if type(self.solutions) is numpy.ndarray:
+                self.solutions = list(self.solutions)
+            # self.solutions_fitness: Holds the fitness of the solutions in each generation.
+            if type(self.solutions_fitness) is numpy.ndarray:
+                self.solutions_fitness = list(self.solutions_fitness)
+
+            if not (self.on_start is None):
+                self.on_start(self)
+
+            stop_run = False
+
+            # To continue from where we stopped, the first generation index should start from the value of the 'self.generations_completed' parameter.
+            if self.generations_completed != 0 and type(self.generations_completed) in GA.supported_int_types:
+                # If the 'self.generations_completed' parameter is not '0', then this means we continue execution.
+                generation_first_idx = self.generations_completed
+                generation_last_idx = self.num_generations + self.generations_completed
+            else:
+                # If the 'self.generations_completed' parameter is '0', then stat from scratch.
+                generation_first_idx = 0
+                generation_last_idx = self.num_generations
 
-        if self.valid_parameters == False:
-            self.logger.error("Error calling the run() method: \nThe run() method cannot be executed with invalid parameters. Please check the parameters passed while creating an instance of the GA class.\n")
-            raise Exception("Error calling the run() method: \nThe run() method cannot be executed with invalid parameters. Please check the parameters passed while creating an instance of the GA class.\n")
-
-        # Starting from PyGAD 2.18.0, the 4 properties (best_solutions, best_solutions_fitness, solutions, and solutions_fitness) are no longer reset with each call to the run() method. Instead, they are extended. 
-        # For example, if there are 50 generations and the user set save_best_solutions=True, then the length of the 2 properties best_solutions and best_solutions_fitness will be 50 after the first call to the run() method, then 100 after the second call, 150 after the third, and so on.
-
-        # self.best_solutions: Holds the best solution in each generation.
-        if type(self.best_solutions) is numpy.ndarray:
-            self.best_solutions = list(self.best_solutions)
-        # self.best_solutions_fitness: A list holding the fitness value of the best solution for each generation.
-        if type(self.best_solutions_fitness) is numpy.ndarray:
-            self.best_solutions_fitness = list(self.best_solutions_fitness)
-        # self.solutions: Holds the solutions in each generation.
-        if type(self.solutions) is numpy.ndarray:
-            self.solutions = list(self.solutions)
-        # self.solutions_fitness: Holds the fitness of the solutions in each generation.
-        if type(self.solutions_fitness) is numpy.ndarray:
-            self.solutions_fitness = list(self.solutions_fitness)
-
-        if not (self.on_start is None):
-            self.on_start(self)
-
-        stop_run = False
-
-        # To continue from where we stopped, the first generation index should start from the value of the 'self.generations_completed' parameter.
-        if self.generations_completed != 0 and type(self.generations_completed) in GA.supported_int_types:
-            # If the 'self.generations_completed' parameter is not '0', then this means we continue execution.
-            generation_first_idx = self.generations_completed
-            generation_last_idx = self.num_generations + self.generations_completed
-        else:
-            # If the 'self.generations_completed' parameter is '0', then stat from scratch.
-            generation_first_idx = 0
-            generation_last_idx = self.num_generations
-
-        # Measuring the fitness of each chromosome in the population. Save the fitness in the last_generation_fitness attribute.
-        self.last_generation_fitness = self.cal_pop_fitness()
-
-        best_solution, best_solution_fitness, best_match_idx = self.best_solution(pop_fitness=self.last_generation_fitness)
+            # Measuring the fitness of each chromosome in the population. Save the fitness in the last_generation_fitness attribute.
+            self.last_generation_fitness = self.cal_pop_fitness()
 
-        # Appending the best solution in the initial population to the best_solutions list.
-        if self.save_best_solutions:
-            self.best_solutions.append(best_solution)
+            best_solution, best_solution_fitness, best_match_idx = self.best_solution(pop_fitness=self.last_generation_fitness)
 
-        for generation in range(generation_first_idx, generation_last_idx):
-            if not (self.on_fitness is None):
-                self.on_fitness(self, self.last_generation_fitness)
+            # Appending the best solution in the initial population to the best_solutions list.
+            if self.save_best_solutions:
+                self.best_solutions.append(best_solution)
 
-            # Appending the fitness value of the best solution in the current generation to the best_solutions_fitness attribute.
-            self.best_solutions_fitness.append(best_solution_fitness)
-            
-            # Appending the solutions in the current generation to the solutions list.
-            if self.save_solutions:
-                # self.solutions.extend(self.population.copy())
-                population_as_list = self.population.copy()
-                population_as_list = [list(item) for item in population_as_list]
-                self.solutions.extend(population_as_list)
+            for generation in range(generation_first_idx, generation_last_idx):
+                if not (self.on_fitness is None):
+                    on_fitness_output = self.on_fitness(self, 
+                                                        self.last_generation_fitness)
 
-                self.solutions_fitness.extend(self.last_generation_fitness)
+                    if on_fitness_output is None:
+                        pass
+                    else:
+                        if type(on_fitness_output) in [tuple, list, numpy.ndarray, range]:
+                            on_fitness_output = numpy.array(on_fitness_output)
+                            if on_fitness_output.shape == self.last_generation_fitness.shape:
+                                self.last_generation_fitness = on_fitness_output
+                            else:
+                                raise ValueError(f"Size mismatch between the output of on_fitness() {on_fitness_output.shape} and the expected fitness output {self.last_generation_fitness.shape}.")
+                        else:
+                            raise ValueError(f"The output of on_fitness() is expected to be tuple/list/range/numpy.ndarray but {type(on_fitness_output)} found.")
 
-            # Selecting the best parents in the population for mating.
-            if callable(self.parent_selection_type):
-                self.last_generation_parents, self.last_generation_parents_indices = self.select_parents(self.last_generation_fitness, 
-                                                                                                         self.num_parents_mating, 
-                                                                                                         self)
-                if not type(self.last_generation_parents) is numpy.ndarray:
-                    self.logger.error("The type of the iterable holding the selected parents is expected to be (numpy.ndarray) but {last_generation_parents_type} found.".format(last_generation_parents_type=type(self.last_generation_parents)))
-                    raise TypeError("The type of the iterable holding the selected parents is expected to be (numpy.ndarray) but {last_generation_parents_type} found.".format(last_generation_parents_type=type(self.last_generation_parents)))
-                if not type(self.last_generation_parents_indices) is numpy.ndarray:
-                    self.logger.error("The type of the iterable holding the selected parents' indices is expected to be (numpy.ndarray) but {last_generation_parents_indices_type} found.".format(last_generation_parents_indices_type=type(self.last_generation_parents_indices)))
-                    raise TypeError("The type of the iterable holding the selected parents' indices is expected to be (numpy.ndarray) but {last_generation_parents_indices_type} found.".format(last_generation_parents_indices_type=type(self.last_generation_parents_indices)))
-            else:
-                self.last_generation_parents, self.last_generation_parents_indices = self.select_parents(self.last_generation_fitness, 
-                                                                                                         num_parents=self.num_parents_mating)
-
-            # Validate the output of the parent selection step: self.select_parents()
-            if self.last_generation_parents.shape != (self.num_parents_mating, self.num_genes):
-                if self.last_generation_parents.shape[0] != self.num_parents_mating:
-                    self.logger.error("Size mismatch between the size of the selected parents {parents_size_actual} and the expected size {parents_size_expected}. It is expected to select ({num_parents_mating}) parents but ({num_parents_mating_selected}) selected.".format(parents_size_actual=self.last_generation_parents.shape, parents_size_expected=(self.num_parents_mating, self.num_genes), num_parents_mating=self.num_parents_mating, num_parents_mating_selected=self.last_generation_parents.shape[0]))
-                    raise ValueError("Size mismatch between the size of the selected parents {parents_size_actual} and the expected size {parents_size_expected}. It is expected to select ({num_parents_mating}) parents but ({num_parents_mating_selected}) selected.".format(parents_size_actual=self.last_generation_parents.shape, parents_size_expected=(self.num_parents_mating, self.num_genes), num_parents_mating=self.num_parents_mating, num_parents_mating_selected=self.last_generation_parents.shape[0]))
-                elif self.last_generation_parents.shape[1] != self.num_genes:
-                    self.logger.error("Size mismatch between the size of the selected parents {parents_size_actual} and the expected size {parents_size_expected}. Parents are expected to have ({num_genes}) genes but ({num_genes_selected}) produced.".format(parents_size_actual=self.last_generation_parents.shape, parents_size_expected=(self.num_parents_mating, self.num_genes), num_genes=self.num_genes, num_genes_selected=self.last_generation_parents.shape[1]))
-                    raise ValueError("Size mismatch between the size of the selected parents {parents_size_actual} and the expected size {parents_size_expected}. Parents are expected to have ({num_genes}) genes but ({num_genes_selected}) produced.".format(parents_size_actual=self.last_generation_parents.shape, parents_size_expected=(self.num_parents_mating, self.num_genes), num_genes=self.num_genes, num_genes_selected=self.last_generation_parents.shape[1]))
-
-            if self.last_generation_parents_indices.ndim != 1:
-                self.logger.error("The iterable holding the selected parents indices is expected to have 1 dimension but ({parents_indices_ndim}) found.".format(parents_indices_ndim=len(self.last_generation_parents_indices)))
-                raise ValueError("The iterable holding the selected parents indices is expected to have 1 dimension but ({parents_indices_ndim}) found.".format(parents_indices_ndim=len(self.last_generation_parents_indices)))
-            elif len(self.last_generation_parents_indices) != self.num_parents_mating:
-                self.logger.error("The iterable holding the selected parents indices is expected to have ({num_parents_mating}) values but ({num_parents_mating_selected}) found.".format(num_parents_mating=self.num_parents_mating, num_parents_mating_selected=len(self.last_generation_parents_indices)))
-                raise ValueError("The iterable holding the selected parents indices is expected to have ({num_parents_mating}) values but ({num_parents_mating_selected}) found.".format(num_parents_mating=self.num_parents_mating, num_parents_mating_selected=len(self.last_generation_parents_indices)))
+                # Appending the fitness value of the best solution in the current generation to the best_solutions_fitness attribute.
+                self.best_solutions_fitness.append(best_solution_fitness)
 
-            if not (self.on_parents is None):
-                self.on_parents(self, self.last_generation_parents)
+                # Appending the solutions in the current generation to the solutions list.
+                if self.save_solutions:
+                    # self.solutions.extend(self.population.copy())
+                    population_as_list = self.population.copy()
+                    population_as_list = [list(item)
+                                        for item in population_as_list]
+                    self.solutions.extend(population_as_list)
+
+                    self.solutions_fitness.extend(self.last_generation_fitness)
+
+                # Selecting the best parents in the population for mating.
+                if callable(self.parent_selection_type):
+                    self.last_generation_parents, self.last_generation_parents_indices = self.select_parents(self.last_generation_fitness,
+                                                                                                            self.num_parents_mating,
+                                                                                                            self)
+                    if not type(self.last_generation_parents) is numpy.ndarray:
+                        raise TypeError(f"The type of the iterable holding the selected parents is expected to be (numpy.ndarray) but {type(self.last_generation_parents)} found.")
+                    if not type(self.last_generation_parents_indices) is numpy.ndarray:
+                        raise TypeError(f"The type of the iterable holding the selected parents' indices is expected to be (numpy.ndarray) but {type(self.last_generation_parents_indices)} found.")
+                else:
+                    self.last_generation_parents, self.last_generation_parents_indices = self.select_parents(self.last_generation_fitness,
+                                                                                                            num_parents=self.num_parents_mating)
+
+                # Validate the output of the parent selection step: self.select_parents()
+                if self.last_generation_parents.shape != (self.num_parents_mating, self.num_genes):
+                    if self.last_generation_parents.shape[0] != self.num_parents_mating:
+                        raise ValueError(f"Size mismatch between the size of the selected parents {self.last_generation_parents.shape} and the expected size {(self.num_parents_mating, self.num_genes)}. It is expected to select ({self.num_parents_mating}) parents but ({self.last_generation_parents.shape[0]}) selected.")
+                    elif self.last_generation_parents.shape[1] != self.num_genes:
+                        raise ValueError(f"Size mismatch between the size of the selected parents {self.last_generation_parents.shape} and the expected size {(self.num_parents_mating, self.num_genes)}. Parents are expected to have ({self.num_genes}) genes but ({self.last_generation_parents.shape[1]}) produced.")
+
+                if self.last_generation_parents_indices.ndim != 1:
+                    raise ValueError(f"The iterable holding the selected parents indices is expected to have 1 dimension but ({len(self.last_generation_parents_indices)}) found.")
+                elif len(self.last_generation_parents_indices) != self.num_parents_mating:
+                    raise ValueError(f"The iterable holding the selected parents indices is expected to have ({self.num_parents_mating}) values but ({len(self.last_generation_parents_indices)}) found.")
+
+                if not (self.on_parents is None):
+                    on_parents_output = self.on_parents(self, 
+                                                        self.last_generation_parents)
+                    
+                    if on_parents_output is None:
+                        pass
+                    elif type(on_parents_output) in [list, tuple, numpy.ndarray]:
+                        if len(on_parents_output) == 2:
+                            on_parents_selected_parents, on_parents_selected_parents_indices = on_parents_output
+                        else:
+                            raise ValueError(f"The output of on_parents() is expected to be tuple/list/numpy.ndarray of length 2 but {type(on_parents_output)} of length {len(on_parents_output)} found.")
 
-            # If self.crossover_type=None, then no crossover is applied and thus no offspring will be created in the next generations. The next generation will use the solutions in the current population.
-            if self.crossover_type is None:
-                if self.keep_elitism == 0:
-                    num_parents_to_keep = self.num_parents_mating if self.keep_parents == -1 else self.keep_parents
-                    if self.num_offspring <= num_parents_to_keep:
-                        self.last_generation_offspring_crossover = self.last_generation_parents[0:self.num_offspring]
-                    else:
-                        self.last_generation_offspring_crossover = numpy.concatenate((self.last_generation_parents, self.population[0:(self.num_offspring - self.last_generation_parents.shape[0])]))
-                else:
-                    # The steady_state_selection() function is called to select the best solutions (i.e. elitism). The keep_elitism parameter defines the number of these solutions.
-                    # The steady_state_selection() function is still called here even if its output may not be used given that the condition of the next if statement is True. The reason is that it will be used later.
-                    self.last_generation_elitism, _ = self.steady_state_selection(self.last_generation_fitness, 
-                                                                                  num_parents=self.keep_elitism)
-                    if self.num_offspring <= self.keep_elitism:
-                        self.last_generation_offspring_crossover = self.last_generation_parents[0:self.num_offspring]
-                    else:
-                        self.last_generation_offspring_crossover = numpy.concatenate((self.last_generation_elitism, self.population[0:(self.num_offspring - self.last_generation_elitism.shape[0])]))
-            else:
-                # Generating offspring using crossover.
-                if callable(self.crossover_type):
-                    self.last_generation_offspring_crossover = self.crossover(self.last_generation_parents,
-                                                                              (self.num_offspring, self.num_genes),
-                                                                              self)
-                    if not type(self.last_generation_offspring_crossover) is numpy.ndarray:
-                        self.logger.error("The output of the crossover step is expected to be of type (numpy.ndarray) but {last_generation_offspring_crossover_type} found.".format(last_generation_offspring_crossover_type=type(self.last_generation_offspring_crossover)))
-                        raise TypeError("The output of the crossover step is expected to be of type (numpy.ndarray) but {last_generation_offspring_crossover_type} found.".format(last_generation_offspring_crossover_type=type(self.last_generation_offspring_crossover)))
-                else:
-                    self.last_generation_offspring_crossover = self.crossover(self.last_generation_parents,
-                                                                              offspring_size=(self.num_offspring, self.num_genes))
-                if self.last_generation_offspring_crossover.shape != (self.num_offspring, self.num_genes):
-                    if self.last_generation_offspring_crossover.shape[0] != self.num_offspring:
-                        self.logger.error("Size mismatch between the crossover output {crossover_actual_size} and the expected crossover output {crossover_expected_size}. It is expected to produce ({num_offspring}) offspring but ({num_offspring_produced}) produced.".format(crossover_actual_size=self.last_generation_offspring_crossover.shape, crossover_expected_size=(self.num_offspring, self.num_genes), num_offspring=self.num_offspring, num_offspring_produced=self.last_generation_offspring_crossover.shape[0]))
-                        raise ValueError("Size mismatch between the crossover output {crossover_actual_size} and the expected crossover output {crossover_expected_size}. It is expected to produce ({num_offspring}) offspring but ({num_offspring_produced}) produced.".format(crossover_actual_size=self.last_generation_offspring_crossover.shape, crossover_expected_size=(self.num_offspring, self.num_genes), num_offspring=self.num_offspring, num_offspring_produced=self.last_generation_offspring_crossover.shape[0]))
-                    elif self.last_generation_offspring_crossover.shape[1] != self.num_genes:
-                        self.logger.error("Size mismatch between the crossover output {crossover_actual_size} and the expected crossover output {crossover_expected_size}. It is expected that the offspring has ({num_genes}) genes but ({num_genes_produced}) produced.".format(crossover_actual_size=self.last_generation_offspring_crossover.shape, crossover_expected_size=(self.num_offspring, self.num_genes), num_genes=self.num_genes, num_genes_produced=self.last_generation_offspring_crossover.shape[1]))
-                        raise ValueError("Size mismatch between the crossover output {crossover_actual_size} and the expected crossover output {crossover_expected_size}. It is expected that the offspring has ({num_genes}) genes but ({num_genes_produced}) produced.".format(crossover_actual_size=self.last_generation_offspring_crossover.shape, crossover_expected_size=(self.num_offspring, self.num_genes), num_genes=self.num_genes, num_genes_produced=self.last_generation_offspring_crossover.shape[1]))
-
-            # PyGAD 2.18.2 // The on_crossover() callback function is called even if crossover_type is None.
-            if not (self.on_crossover is None):
-                self.on_crossover(self, self.last_generation_offspring_crossover)
-
-            # If self.mutation_type=None, then no mutation is applied and thus no changes are applied to the offspring created using the crossover operation. The offspring will be used unchanged in the next generation.
-            if self.mutation_type is None:
-                self.last_generation_offspring_mutation = self.last_generation_offspring_crossover
-            else:
-                # Adding some variations to the offspring using mutation.
-                if callable(self.mutation_type):
-                    self.last_generation_offspring_mutation = self.mutation(self.last_generation_offspring_crossover, 
-                                                                            self)
-                    if not type(self.last_generation_offspring_mutation) is numpy.ndarray:
-                        self.logger.error("The output of the mutation step is expected to be of type (numpy.ndarray) but {last_generation_offspring_mutation_type} found.".format(last_generation_offspring_mutation_type=type(self.last_generation_offspring_mutation)))
-                        raise TypeError("The output of the mutation step is expected to be of type (numpy.ndarray) but {last_generation_offspring_mutation_type} found.".format(last_generation_offspring_mutation_type=type(self.last_generation_offspring_mutation)))
-                else:
-                    self.last_generation_offspring_mutation = self.mutation(self.last_generation_offspring_crossover)
-
-                if self.last_generation_offspring_mutation.shape != (self.num_offspring, self.num_genes):
-                    if self.last_generation_offspring_mutation.shape[0] != self.num_offspring:
-                        self.logger.error("Size mismatch between the mutation output {mutation_actual_size} and the expected mutation output {mutation_expected_size}. It is expected to produce ({num_offspring}) offspring but ({num_offspring_produced}) produced.".format(mutation_actual_size=self.last_generation_offspring_mutation.shape, mutation_expected_size=(self.num_offspring, self.num_genes), num_offspring=self.num_offspring, num_offspring_produced=self.last_generation_offspring_mutation.shape[0]))
-                        raise ValueError("Size mismatch between the mutation output {mutation_actual_size} and the expected mutation output {mutation_expected_size}. It is expected to produce ({num_offspring}) offspring but ({num_offspring_produced}) produced.".format(mutation_actual_size=self.last_generation_offspring_mutation.shape, mutation_expected_size=(self.num_offspring, self.num_genes), num_offspring=self.num_offspring, num_offspring_produced=self.last_generation_offspring_mutation.shape[0]))
-                    elif self.last_generation_offspring_mutation.shape[1] != self.num_genes:
-                        self.logger.error("Size mismatch between the mutation output {mutation_actual_size} and the expected mutation output {mutation_expected_size}. It is expected that the offspring has ({num_genes}) genes but ({num_genes_produced}) produced.".format(mutation_actual_size=self.last_generation_offspring_mutation.shape, mutation_expected_size=(self.num_offspring, self.num_genes), num_genes=self.num_genes, num_genes_produced=self.last_generation_offspring_mutation.shape[1]))
-                        raise ValueError("Size mismatch between the mutation output {mutation_actual_size} and the expected mutation output {mutation_expected_size}. It is expected that the offspring has ({num_genes}) genes but ({num_genes_produced}) produced.".format(mutation_actual_size=self.last_generation_offspring_mutation.shape, mutation_expected_size=(self.num_offspring, self.num_genes), num_genes=self.num_genes, num_genes_produced=self.last_generation_offspring_mutation.shape[1]))
-
-            # PyGAD 2.18.2 // The on_mutation() callback function is called even if mutation_type is None.
-            if not (self.on_mutation is None):
-                self.on_mutation(self, self.last_generation_offspring_mutation)
+                        # Validate the parents.
+                        if on_parents_selected_parents is None:
+                            raise ValueError("The returned outputs of on_parents() cannot be None but the first output is None.")
+                        else:
+                            if type(on_parents_selected_parents) in [tuple, list, numpy.ndarray]:
+                                on_parents_selected_parents = numpy.array(on_parents_selected_parents)
+                                if on_parents_selected_parents.shape == self.last_generation_parents.shape:
+                                    self.last_generation_parents = on_parents_selected_parents
+                                else:
+                                    raise ValueError(f"Size mismatch between the parents retrned by on_parents() {on_parents_selected_parents.shape} and the expected parents shape {self.last_generation_parents.shape}.")
+                            else:
+                                raise ValueError(f"The output of on_parents() is expected to be tuple/list/numpy.ndarray but the first output type is {type(on_parents_selected_parents)}.")
 
-            # Update the population attribute according to the offspring generated.
-            if self.keep_elitism == 0:
-                # If the keep_elitism parameter is 0, then the keep_parents parameter will be used to decide if the parents are kept in the next generation.
-                if (self.keep_parents == 0):
-                    self.population = self.last_generation_offspring_mutation
-                elif (self.keep_parents == -1):
-                    # Creating the new population based on the parents and offspring.
-                    self.population[0:self.last_generation_parents.shape[0], :] = self.last_generation_parents
-                    self.population[self.last_generation_parents.shape[0]:, :] = self.last_generation_offspring_mutation
-                elif (self.keep_parents > 0):
-                    parents_to_keep, _ = self.steady_state_selection(self.last_generation_fitness, 
-                                                                     num_parents=self.keep_parents)
-                    self.population[0:parents_to_keep.shape[0], :] = parents_to_keep
-                    self.population[parents_to_keep.shape[0]:, :] = self.last_generation_offspring_mutation
-            else:
-                self.last_generation_elitism, self.last_generation_elitism_indices = self.steady_state_selection(self.last_generation_fitness, 
-                                                                                                                 num_parents=self.keep_elitism)
-                self.population[0:self.last_generation_elitism.shape[0], :] = self.last_generation_elitism
-                self.population[self.last_generation_elitism.shape[0]:, :] = self.last_generation_offspring_mutation
+                        # Validate the parents indices.
+                        if on_parents_selected_parents_indices is None:
+                            raise ValueError("The returned outputs of on_parents() cannot be None but the second output is None.")
+                        else:
+                            if type(on_parents_selected_parents_indices) in [tuple, list, numpy.ndarray, range]:
+                                on_parents_selected_parents_indices = numpy.array(on_parents_selected_parents_indices)
+                                if on_parents_selected_parents_indices.shape == self.last_generation_parents_indices.shape:
+                                    self.last_generation_parents_indices = on_parents_selected_parents_indices
+                                else:
+                                    raise ValueError(f"Size mismatch between the parents indices returned by on_parents() {on_parents_selected_parents_indices.shape} and the expected crossover output {self.last_generation_parents_indices.shape}.")
+                            else:
+                                raise ValueError(f"The output of on_parents() is expected to be tuple/list/range/numpy.ndarray but the second output type is {type(on_parents_selected_parents_indices)}.")
 
-            self.generations_completed = generation + 1 # The generations_completed attribute holds the number of the last completed generation.
+                    else:
+                        raise TypeError(f"The output of on_parents() is expected to be tuple/list/numpy.ndarray but {type(on_parents_output)} found.")
 
-            self.previous_generation_fitness = self.last_generation_fitness.copy()
-            # Measuring the fitness of each chromosome in the population. Save the fitness in the last_generation_fitness attribute.
-            self.last_generation_fitness = self.cal_pop_fitness()
+                # If self.crossover_type=None, then no crossover is applied and thus no offspring will be created in the next generations. The next generation will use the solutions in the current population.
+                if self.crossover_type is None:
+                    if self.keep_elitism == 0:
+                        num_parents_to_keep = self.num_parents_mating if self.keep_parents == - \
+                            1 else self.keep_parents
+                        if self.num_offspring <= num_parents_to_keep:
+                            self.last_generation_offspring_crossover = self.last_generation_parents[
+                                0:self.num_offspring]
+                        else:
+                            self.last_generation_offspring_crossover = numpy.concatenate(
+                                (self.last_generation_parents, self.population[0:(self.num_offspring - self.last_generation_parents.shape[0])]))
+                    else:
+                        # The steady_state_selection() function is called to select the best solutions (i.e. elitism). The keep_elitism parameter defines the number of these solutions.
+                        # The steady_state_selection() function is still called here even if its output may not be used given that the condition of the next if statement is True. The reason is that it will be used later.
+                        self.last_generation_elitism, _ = self.steady_state_selection(self.last_generation_fitness,
+                                                                                    num_parents=self.keep_elitism)
+                        if self.num_offspring <= self.keep_elitism:
+                            self.last_generation_offspring_crossover = self.last_generation_parents[
+                                0:self.num_offspring]
+                        else:
+                            self.last_generation_offspring_crossover = numpy.concatenate(
+                                (self.last_generation_elitism, self.population[0:(self.num_offspring - self.last_generation_elitism.shape[0])]))
+                else:
+                    # Generating offspring using crossover.
+                    if callable(self.crossover_type):
+                        self.last_generation_offspring_crossover = self.crossover(self.last_generation_parents,
+                                                                                (self.num_offspring,
+                                                                                self.num_genes),
+                                                                                self)
+                        if not type(self.last_generation_offspring_crossover) is numpy.ndarray:
+                            raise TypeError(f"The output of the crossover step is expected to be of type (numpy.ndarray) but {type(self.last_generation_offspring_crossover)} found.")
+                    else:
+                        self.last_generation_offspring_crossover = self.crossover(self.last_generation_parents,
+                                                                                offspring_size=(self.num_offspring, self.num_genes))
+                    if self.last_generation_offspring_crossover.shape != (self.num_offspring, self.num_genes):
+                        if self.last_generation_offspring_crossover.shape[0] != self.num_offspring:
+                            raise ValueError(f"Size mismatch between the crossover output {self.last_generation_offspring_crossover.shape} and the expected crossover output {(self.num_offspring, self.num_genes)}. It is expected to produce ({self.num_offspring}) offspring but ({self.last_generation_offspring_crossover.shape[0]}) produced.")
+                        elif self.last_generation_offspring_crossover.shape[1] != self.num_genes:
+                            raise ValueError(f"Size mismatch between the crossover output {self.last_generation_offspring_crossover.shape} and the expected crossover output {(self.num_offspring, self.num_genes)}. It is expected that the offspring has ({self.num_genes}) genes but ({self.last_generation_offspring_crossover.shape[1]}) produced.")
+
+                # PyGAD 2.18.2 // The on_crossover() callback function is called even if crossover_type is None.
+                if not (self.on_crossover is None):
+                    on_crossover_output = self.on_crossover(self, 
+                                                            self.last_generation_offspring_crossover)
+                    if on_crossover_output is None:
+                        pass
+                    else:
+                        if type(on_crossover_output) in [tuple, list, numpy.ndarray]:
+                            on_crossover_output = numpy.array(on_crossover_output)
+                            if on_crossover_output.shape == self.last_generation_offspring_crossover.shape:
+                                self.last_generation_offspring_crossover = on_crossover_output
+                            else:
+                                raise ValueError(f"Size mismatch between the output of on_crossover() {on_crossover_output.shape} and the expected crossover output {self.last_generation_offspring_crossover.shape}.")
+                        else:
+                            raise ValueError(f"The output of on_crossover() is expected to be tuple/list/numpy.ndarray but {type(on_crossover_output)} found.")
 
-            best_solution, best_solution_fitness, best_match_idx = self.best_solution(pop_fitness=self.last_generation_fitness)
+                # If self.mutation_type=None, then no mutation is applied and thus no changes are applied to the offspring created using the crossover operation. The offspring will be used unchanged in the next generation.
+                if self.mutation_type is None:
+                    self.last_generation_offspring_mutation = self.last_generation_offspring_crossover
+                else:
+                    # Adding some variations to the offspring using mutation.
+                    if callable(self.mutation_type):
+                        self.last_generation_offspring_mutation = self.mutation(self.last_generation_offspring_crossover,
+                                                                                self)
+                        if not type(self.last_generation_offspring_mutation) is numpy.ndarray:
+                            raise TypeError(f"The output of the mutation step is expected to be of type (numpy.ndarray) but {type(self.last_generation_offspring_mutation)} found.")
+                    else:
+                        self.last_generation_offspring_mutation = self.mutation(self.last_generation_offspring_crossover)
 
-            # Appending the best solution in the current generation to the best_solutions list.
-            if self.save_best_solutions:
-                self.best_solutions.append(best_solution)
+                    if self.last_generation_offspring_mutation.shape != (self.num_offspring, self.num_genes):
+                        if self.last_generation_offspring_mutation.shape[0] != self.num_offspring:
+                            raise ValueError(f"Size mismatch between the mutation output {self.last_generation_offspring_mutation.shape} and the expected mutation output {(self.num_offspring, self.num_genes)}. It is expected to produce ({self.num_offspring}) offspring but ({self.last_generation_offspring_mutation.shape[0]}) produced.")
+                        elif self.last_generation_offspring_mutation.shape[1] != self.num_genes:
+                            raise ValueError(f"Size mismatch between the mutation output {self.last_generation_offspring_mutation.shape} and the expected mutation output {(self.num_offspring, self.num_genes)}. It is expected that the offspring has ({self.num_genes}) genes but ({self.last_generation_offspring_mutation.shape[1]}) produced.")
+
+                # PyGAD 2.18.2 // The on_mutation() callback function is called even if mutation_type is None.
+                if not (self.on_mutation is None):
+                    on_mutation_output = self.on_mutation(self, 
+                                                          self.last_generation_offspring_mutation)
 
-            # If the on_generation attribute is not None, then cal the callback function after the generation.
-            if not (self.on_generation is None):
-                r = self.on_generation(self)
-                if type(r) is str and r.lower() == "stop":
-                    # Before aborting the loop, save the fitness value of the best solution.
-                    # _, best_solution_fitness, _ = self.best_solution()
-                    self.best_solutions_fitness.append(best_solution_fitness)
-                    break
+                    if on_mutation_output is None:
+                        pass
+                    else:
+                        if type(on_mutation_output) in [tuple, list, numpy.ndarray]:
+                            on_mutation_output = numpy.array(on_mutation_output)
+                            if on_mutation_output.shape == self.last_generation_offspring_mutation.shape:
+                                self.last_generation_offspring_mutation = on_mutation_output
+                            else:
+                                raise ValueError(f"Size mismatch between the output of on_mutation() {on_mutation_output.shape} and the expected mutation output {self.last_generation_offspring_mutation.shape}.")
+                        else:
+                            raise ValueError(f"The output of on_mutation() is expected to be tuple/list/numpy.ndarray but {type(on_mutation_output)} found.")
 
-            if not self.stop_criteria is None:
-                for criterion in self.stop_criteria:
-                    if criterion[0] == "reach":
-                        if max(self.last_generation_fitness) >= criterion[1]:
-                            stop_run = True
-                            break
-                    elif criterion[0] == "saturate":
-                        criterion[1] = int(criterion[1])
-                        if (self.generations_completed >= criterion[1]):
-                            if (self.best_solutions_fitness[self.generations_completed - criterion[1]] - self.best_solutions_fitness[self.generations_completed - 1]) == 0:
+                # Update the population attribute according to the offspring generated.
+                if self.keep_elitism == 0:
+                    # If the keep_elitism parameter is 0, then the keep_parents parameter will be used to decide if the parents are kept in the next generation.
+                    if (self.keep_parents == 0):
+                        self.population = self.last_generation_offspring_mutation
+                    elif (self.keep_parents == -1):
+                        # Creating the new population based on the parents and offspring.
+                        self.population[0:self.last_generation_parents.shape[0],
+                                        :] = self.last_generation_parents
+                        self.population[self.last_generation_parents.shape[0]:, :] = self.last_generation_offspring_mutation
+                    elif (self.keep_parents > 0):
+                        parents_to_keep, _ = self.steady_state_selection(self.last_generation_fitness,
+                                                                        num_parents=self.keep_parents)
+                        self.population[0:parents_to_keep.shape[0],
+                                        :] = parents_to_keep
+                        self.population[parents_to_keep.shape[0]:,
+                                        :] = self.last_generation_offspring_mutation
+                else:
+                    self.last_generation_elitism, self.last_generation_elitism_indices = self.steady_state_selection(self.last_generation_fitness,
+                                                                                                                    num_parents=self.keep_elitism)
+                    self.population[0:self.last_generation_elitism.shape[0],
+                                    :] = self.last_generation_elitism
+                    self.population[self.last_generation_elitism.shape[0]:, :] = self.last_generation_offspring_mutation
+
+                # The generations_completed attribute holds the number of the last completed generation.
+                self.generations_completed = generation + 1
+
+                self.previous_generation_fitness = self.last_generation_fitness.copy()
+                # Measuring the fitness of each chromosome in the population. Save the fitness in the last_generation_fitness attribute.
+                self.last_generation_fitness = self.cal_pop_fitness()
+
+                best_solution, best_solution_fitness, best_match_idx = self.best_solution(
+                    pop_fitness=self.last_generation_fitness)
+
+                # Appending the best solution in the current generation to the best_solutions list.
+                if self.save_best_solutions:
+                    self.best_solutions.append(best_solution)
+
+                # If the on_generation attribute is not None, then cal the callback function after the generation.
+                if not (self.on_generation is None):
+                    r = self.on_generation(self)
+                    if type(r) is str and r.lower() == "stop":
+                        # Before aborting the loop, save the fitness value of the best solution.
+                        # _, best_solution_fitness, _ = self.best_solution()
+                        self.best_solutions_fitness.append(best_solution_fitness)
+                        break
+
+                if not self.stop_criteria is None:
+                    for criterion in self.stop_criteria:
+                        if criterion[0] == "reach":
+                            if max(self.last_generation_fitness) >= criterion[1]:
                                 stop_run = True
                                 break
+                        elif criterion[0] == "saturate":
+                            criterion[1] = int(criterion[1])
+                            if (self.generations_completed >= criterion[1]):
+                                if (self.best_solutions_fitness[self.generations_completed - criterion[1]] - self.best_solutions_fitness[self.generations_completed - 1]) == 0:
+                                    stop_run = True
+                                    break
 
-            if stop_run:
-                break
-
-            time.sleep(self.delay_after_gen)
-
-        # Save the fitness of the last generation.
-        if self.save_solutions:
-            # self.solutions.extend(self.population.copy())
-            population_as_list = self.population.copy()
-            population_as_list = [list(item) for item in population_as_list]
-            self.solutions.extend(population_as_list)
-
-            self.solutions_fitness.extend(self.last_generation_fitness)
+                if stop_run:
+                    break
 
-        # Save the fitness value of the best solution.
-        _, best_solution_fitness, _ = self.best_solution(pop_fitness=self.last_generation_fitness)
-        self.best_solutions_fitness.append(best_solution_fitness)
+                time.sleep(self.delay_after_gen)
 
-        self.best_solution_generation = numpy.where(numpy.array(self.best_solutions_fitness) == numpy.max(numpy.array(self.best_solutions_fitness)))[0][0]
-        # After the run() method completes, the run_completed flag is changed from False to True.
-        self.run_completed = True # Set to True only after the run() method completes gracefully.
+            # Save the fitness of the last generation.
+            if self.save_solutions:
+                # self.solutions.extend(self.population.copy())
+                population_as_list = self.population.copy()
+                population_as_list = [list(item) for item in population_as_list]
+                self.solutions.extend(population_as_list)
 
-        if not (self.on_stop is None):
-            self.on_stop(self, self.last_generation_fitness)
+                self.solutions_fitness.extend(self.last_generation_fitness)
 
-        # Converting the 'best_solutions' list into a NumPy array.
-        self.best_solutions = numpy.array(self.best_solutions)
+            # Save the fitness value of the best solution.
+            _, best_solution_fitness, _ = self.best_solution(
+                pop_fitness=self.last_generation_fitness)
+            self.best_solutions_fitness.append(best_solution_fitness)
 
-        # Converting the 'solutions' list into a NumPy array.
-        # self.solutions = numpy.array(self.solutions)
+            self.best_solution_generation = numpy.where(numpy.array(
+                self.best_solutions_fitness) == numpy.max(numpy.array(self.best_solutions_fitness)))[0][0]
+            # After the run() method completes, the run_completed flag is changed from False to True.
+            # Set to True only after the run() method completes gracefully.
+            self.run_completed = True
+
+            if not (self.on_stop is None):
+                self.on_stop(self, self.last_generation_fitness)
+
+            # Converting the 'best_solutions' list into a NumPy array.
+            self.best_solutions = numpy.array(self.best_solutions)
+
+            # Converting the 'solutions' list into a NumPy array.
+            # self.solutions = numpy.array(self.solutions)
+        except Exception as ex:
+            self.logger.exception(ex)
+            sys.exit(-1)
 
     def best_solution(self, pop_fitness=None):
-
         """
         Returns information about the best solution found by the genetic algorithm.
         Accepts the following parameters:
             pop_fitness: An optional parameter holding the fitness values of the solutions in the latest population. If passed, then it save time calculating the fitness. If None, then the 'cal_pop_fitness()' method is called to calculate the fitness of the latest population.
         The following are returned:
             -best_solution: Best solution in the current population.
             -best_solution_fitness: Fitness value of the best solution.
             -best_match_idx: Index of the best solution in the current population.
         """
-
-        if pop_fitness is None:
-            # If the 'pop_fitness' parameter is not passed, then we have to call the 'cal_pop_fitness()' method to calculate the fitness of all solutions in the lastest population.
-            pop_fitness = self.cal_pop_fitness()
-        # Verify the type of the 'pop_fitness' parameter.
-        elif type(pop_fitness) in [tuple, list, numpy.ndarray]:
-            # Verify that the length of the passed population fitness matches the length of the 'self.population' attribute.
-            if len(pop_fitness) == len(self.population):
-                # This successfully verifies the 'pop_fitness' parameter.
-                pass
+        try:
+            if pop_fitness is None:
+                # If the 'pop_fitness' parameter is not passed, then we have to call the 'cal_pop_fitness()' method to calculate the fitness of all solutions in the lastest population.
+                pop_fitness = self.cal_pop_fitness()
+            # Verify the type of the 'pop_fitness' parameter.
+            elif type(pop_fitness) in [tuple, list, numpy.ndarray]:
+                # Verify that the length of the passed population fitness matches the length of the 'self.population' attribute.
+                if len(pop_fitness) == len(self.population):
+                    # This successfully verifies the 'pop_fitness' parameter.
+                    pass
+                else:
+                    raise ValueError(f"The length of the list/tuple/numpy.ndarray passed to the 'pop_fitness' parameter ({len(pop_fitness)}) must match the length of the 'self.population' attribute ({len(self.population)}).")
             else:
-                self.logger.error("The length of the list/tuple/numpy.ndarray passed to the 'pop_fitness' parameter ({pop_fitness_length}) must match the length of the 'self.population' attribute ({population_length}).".format(pop_fitness_length=len(pop_fitness), population_length=len(self.population)))
-                raise ValueError("The length of the list/tuple/numpy.ndarray passed to the 'pop_fitness' parameter ({pop_fitness_length}) must match the length of the 'self.population' attribute ({population_length}).".format(pop_fitness_length=len(pop_fitness), population_length=len(self.population)))
-        else:
-            self.logger.error("The type of the 'pop_fitness' parameter is expected to be list, tuple, or numpy.ndarray but ({pop_fitness_type}) found.".format(pop_fitness_type=type(pop_fitness)))
-            raise ValueError("The type of the 'pop_fitness' parameter is expected to be list, tuple, or numpy.ndarray but ({pop_fitness_type}) found.".format(pop_fitness_type=type(pop_fitness)))
+                raise ValueError(f"The type of the 'pop_fitness' parameter is expected to be list, tuple, or numpy.ndarray but ({type(pop_fitness)}) found.")
 
-        # Return the index of the best solution that has the best fitness value.
-        best_match_idx = numpy.where(pop_fitness == numpy.max(pop_fitness))[0][0]
-
-        best_solution = self.population[best_match_idx, :].copy()
-        best_solution_fitness = pop_fitness[best_match_idx]
+            # Return the index of the best solution that has the best fitness value.
+            best_match_idx = numpy.where(
+                pop_fitness == numpy.max(pop_fitness))[0][0]
+
+            best_solution = self.population[best_match_idx, :].copy()
+            best_solution_fitness = pop_fitness[best_match_idx]
+        except Exception as ex:
+            self.logger.exception(ex)
+            sys.exit(-1)
 
         return best_solution, best_solution_fitness, best_match_idx
 
     def save(self, filename):
-
         """
         Saves the genetic algorithm instance:
             -filename: Name of the file to save the instance. No extension is needed.
         """
 
         cloudpickle_serialized_object = cloudpickle.dumps(self)
         with open(filename + ".pkl", 'wb') as file:
             file.write(cloudpickle_serialized_object)
             cloudpickle.dump(self, file)
 
-    def summary(self, 
-                line_length=70, 
-                fill_character=" ", 
-                line_character="-", 
-                line_character2="=", 
-                columns_equal_len=False, 
+    def summary(self,
+                line_length=70,
+                fill_character=" ",
+                line_character="-",
+                line_character2="=",
+                columns_equal_len=False,
                 print_step_parameters=True,
                 print_parameters_summary=True):
         """
         The summary() method prints a summary of the PyGAD lifecycle in a Keras style.
         The parameters are:
             line_length: An integer representing the length of the single line in characters.
             fill_character: A character to fill the lines.
@@ -2000,190 +2207,204 @@
         """
 
         summary_output = ""
 
         def fill_message(msg, line_length=line_length, fill_character=fill_character):
             num_spaces = int((line_length - len(msg))/2)
             num_spaces = int(num_spaces / len(fill_character))
-            msg = "{spaces}{msg}{spaces}".format(msg=msg, spaces=fill_character * num_spaces)
+            msg = "{spaces}{msg}{spaces}".format(
+                msg=msg, spaces=fill_character * num_spaces)
             return msg
 
         def line_separator(line_length=line_length, line_character=line_character):
             num_characters = int(line_length / len(line_character))
             return line_character * num_characters
 
         def create_row(columns, line_length=line_length, fill_character=fill_character, split_percentages=None):
             filled_columns = []
             if split_percentages == None:
                 split_percentages = [int(100/len(columns))] * 3
-            columns_lengths = [int((split_percentages[idx] * line_length) / 100) for idx in range(len(split_percentages))]
+            columns_lengths = [int((split_percentages[idx] * line_length) / 100)
+                               for idx in range(len(split_percentages))]
             for column_idx, column in enumerate(columns):
                 current_column_length = len(column)
-                extra_characters = columns_lengths[column_idx] - current_column_length
+                extra_characters = columns_lengths[column_idx] - \
+                    current_column_length
                 filled_column = column + fill_character * extra_characters
                 filled_column = column + fill_character * extra_characters
                 filled_columns.append(filled_column)
 
             return "".join(filled_columns)
 
         def print_parent_selection_params():
             nonlocal summary_output
-            m = "Number of Parents: {num_parents_mating}".format(num_parents_mating=self.num_parents_mating)
+            m = f"Number of Parents: {self.num_parents_mating}"
             self.logger.info(m)
             summary_output = summary_output + m + "\n"
             if self.parent_selection_type == "tournament":
-                m = "K Tournament: {K_tournament}".format(K_tournament=self.K_tournament)
+                m = f"K Tournament: {self.K_tournament}"
                 self.logger.info(m)
                 summary_output = summary_output + m + "\n"
 
         def print_fitness_params():
             nonlocal summary_output
             if not self.fitness_batch_size is None:
-                m = "Fitness batch size: {fitness_batch_size}".format(fitness_batch_size=self.fitness_batch_size)
+                m = f"Fitness batch size: {self.fitness_batch_size}"
                 self.logger.info(m)
                 summary_output = summary_output + m + "\n"
 
         def print_crossover_params():
             nonlocal summary_output
             if not self.crossover_probability is None:
-                m = "Crossover probability: {crossover_probability}".format(crossover_probability=self.crossover_probability)
+                m = f"Crossover probability: {self.crossover_probability}"
                 self.logger.info(m)
                 summary_output = summary_output + m + "\n"
 
         def print_mutation_params():
             nonlocal summary_output
             if not self.mutation_probability is None:
-                m = "Mutation Probability: {mutation_probability}".format(mutation_probability=self.mutation_probability)
+                m = f"Mutation Probability: {self.mutation_probability}"
                 self.logger.info(m)
                 summary_output = summary_output + m + "\n"
             if self.mutation_percent_genes == "default":
-                m = "Mutation Percentage: {mutation_percent_genes}".format(mutation_percent_genes=self.mutation_percent_genes)
+                m = f"Mutation Percentage: {self.mutation_percent_genes}"
                 self.logger.info(m)
                 summary_output = summary_output + m + "\n"
             # Number of mutation genes is already showed above.
-            m = "Mutation Genes: {mutation_num_genes}".format(mutation_num_genes=self.mutation_num_genes)
+            m = f"Mutation Genes: {self.mutation_num_genes}"
             self.logger.info(m)
             summary_output = summary_output + m + "\n"
-            m = "Random Mutation Range: ({random_mutation_min_val}, {random_mutation_max_val})".format(random_mutation_min_val=self.random_mutation_min_val, random_mutation_max_val=self.random_mutation_max_val)
+            m = f"Random Mutation Range: ({self.random_mutation_min_val}, {self.random_mutation_max_val})"
             self.logger.info(m)
             summary_output = summary_output + m + "\n"
             if not self.gene_space is None:
-                m = "Gene Space: {gene_space}".format(gene_space=self.gene_space)
+                m = f"Gene Space: {self.gene_space}"
                 self.logger.info(m)
                 summary_output = summary_output + m + "\n"
-            m = "Mutation by Replacement: {mutation_by_replacement}".format(mutation_by_replacement=self.mutation_by_replacement)
+            m = f"Mutation by Replacement: {self.mutation_by_replacement}"
             self.logger.info(m)
             summary_output = summary_output + m + "\n"
-            m = "Allow Duplicated Genes: {allow_duplicate_genes}".format(allow_duplicate_genes=self.allow_duplicate_genes)
+            m = f"Allow Duplicated Genes: {self.allow_duplicate_genes}"
             self.logger.info(m)
             summary_output = summary_output + m + "\n"
 
         def print_on_generation_params():
             nonlocal summary_output
             if not self.stop_criteria is None:
-                m = "Stop Criteria: {stop_criteria}".format(stop_criteria=self.stop_criteria)
+                m = f"Stop Criteria: {self.stop_criteria}"
                 self.logger.info(m)
                 summary_output = summary_output + m + "\n"
 
         def print_params_summary():
             nonlocal summary_output
-            m = "Population Size: ({sol_per_pop}, {num_genes})".format(sol_per_pop=self.sol_per_pop, num_genes=self.num_genes)
+            m = f"Population Size: ({self.sol_per_pop}, {self.num_genes})"
             self.logger.info(m)
             summary_output = summary_output + m + "\n"
-            m = "Number of Generations: {num_generations}".format(num_generations=self.num_generations)
+            m = f"Number of Generations: {self.num_generations}"
             self.logger.info(m)
             summary_output = summary_output + m + "\n"
-            m = "Initial Population Range: ({init_range_low}, {init_range_high})".format(init_range_low=self.init_range_low, init_range_high=self.init_range_high)
+            m = f"Initial Population Range: ({self.init_range_low}, {self.init_range_high})"
             self.logger.info(m)
             summary_output = summary_output + m + "\n"
 
             if not print_step_parameters:
                 print_fitness_params()
 
             if not print_step_parameters:
                 print_parent_selection_params()
 
             if self.keep_elitism != 0:
-                m = "Keep Elitism: {keep_elitism}".format(keep_elitism=self.keep_elitism)
+                m = f"Keep Elitism: {self.keep_elitism}"
                 self.logger.info(m)
                 summary_output = summary_output + m + "\n"
             else:
-                m = "Keep Parents: {keep_parents}".format(keep_parents=self.keep_parents)
+                m = f"Keep Parents: {self.keep_parents}"
                 self.logger.info(m)
                 summary_output = summary_output + m + "\n"
-            m = "Gene DType: {gene_type}".format(gene_type=self.gene_type)
+            m = f"Gene DType: {self.gene_type}"
             self.logger.info(m)
             summary_output = summary_output + m + "\n"
 
             if not print_step_parameters:
                 print_crossover_params()
 
             if not print_step_parameters:
                 print_mutation_params()
 
             if self.delay_after_gen != 0:
-                m = "Post-Generation Delay: {delay_after_gen}".format(delay_after_gen=self.delay_after_gen)
+                m = f"Post-Generation Delay: {self.delay_after_gen}"
                 self.logger.info(m)
                 summary_output = summary_output + m + "\n"
 
             if not print_step_parameters:
                 print_on_generation_params()
 
             if not self.parallel_processing is None:
-                m = "Parallel Processing: {parallel_processing}".format(parallel_processing=self.parallel_processing)
+                m = f"Parallel Processing: {self.parallel_processing}"
                 self.logger.info(m)
                 summary_output = summary_output + m + "\n"
             if not self.random_seed is None:
-                m = "Random Seed: {random_seed}".format(random_seed=self.random_seed)
+                m = f"Random Seed: {self.random_seed}"
                 self.logger.info(m)
                 summary_output = summary_output + m + "\n"
-            m = "Save Best Solutions: {save_best_solutions}".format(save_best_solutions=self.save_best_solutions)
+            m = f"Save Best Solutions: {self.save_best_solutions}"
             self.logger.info(m)
             summary_output = summary_output + m + "\n"
-            m = "Save Solutions: {save_solutions}".format(save_solutions=self.save_solutions)
+            m = f"Save Solutions: {self.save_solutions}"
             self.logger.info(m)
             summary_output = summary_output + m + "\n"
 
         m = line_separator(line_character=line_character)
         self.logger.info(m)
         summary_output = summary_output + m + "\n"
         m = fill_message("PyGAD Lifecycle")
         self.logger.info(m)
         summary_output = summary_output + m + "\n"
         m = line_separator(line_character=line_character2)
         self.logger.info(m)
         summary_output = summary_output + m + "\n"
 
-        lifecycle_steps = ["on_start()", "Fitness Function", "On Fitness", "Parent Selection", "On Parents", "Crossover", "On Crossover", "Mutation", "On Mutation", "On Generation", "On Stop"]
-        lifecycle_functions = [self.on_start, self.fitness_func, self.on_fitness, self.select_parents, self.on_parents, self.crossover, self.on_crossover, self.mutation, self.on_mutation, self.on_generation, self.on_stop]
-        lifecycle_functions = [getattr(lifecycle_func, '__name__', "None") for lifecycle_func in lifecycle_functions]
-        lifecycle_functions = [lifecycle_func + "()" if lifecycle_func != "None" else "None" for lifecycle_func in lifecycle_functions]
-        lifecycle_output = ["None", "(1)", "None", "({num_parents_mating}, {num_genes})".format(num_parents_mating=self.num_parents_mating, num_genes=self.num_genes), "None", "({num_parents_mating}, {num_genes})".format(num_parents_mating=self.num_parents_mating, num_genes=self.num_genes), "None", "({num_parents_mating}, {num_genes})".format(num_parents_mating=self.num_parents_mating, num_genes=self.num_genes), "None", "None", "None"]
-        lifecycle_step_parameters = [None, print_fitness_params, None, print_parent_selection_params, None, print_crossover_params, None, print_mutation_params, None, print_on_generation_params, None]
+        lifecycle_steps = ["on_start()", "Fitness Function", "On Fitness", "Parent Selection", "On Parents",
+                           "Crossover", "On Crossover", "Mutation", "On Mutation", "On Generation", "On Stop"]
+        lifecycle_functions = [self.on_start, self.fitness_func, self.on_fitness, self.select_parents, self.on_parents,
+                               self.crossover, self.on_crossover, self.mutation, self.on_mutation, self.on_generation, self.on_stop]
+        lifecycle_functions = [getattr(
+            lifecycle_func, '__name__', "None") for lifecycle_func in lifecycle_functions]
+        lifecycle_functions = [lifecycle_func + "()" if lifecycle_func !=
+                               "None" else "None" for lifecycle_func in lifecycle_functions]
+        lifecycle_output = ["None", "(1)", "None", f"({self.num_parents_mating}, {self.num_genes})", "None",
+                            f"({self.num_parents_mating}, {self.num_genes})", "None", f"({self.num_parents_mating}, {self.num_genes})", "None", "None", "None"]
+        lifecycle_step_parameters = [None, print_fitness_params, None, print_parent_selection_params, None,
+                                     print_crossover_params, None, print_mutation_params, None, print_on_generation_params, None]
 
         if not columns_equal_len:
-            max_lengthes = [max(list(map(len, lifecycle_steps))), max(list(map(len, lifecycle_functions))), max(list(map(len, lifecycle_output)))]
-            split_percentages = [int((column_len / sum(max_lengthes)) * 100) for column_len in max_lengthes]
+            max_lengthes = [max(list(map(len, lifecycle_steps))), max(
+                list(map(len, lifecycle_functions))), max(list(map(len, lifecycle_output)))]
+            split_percentages = [
+                int((column_len / sum(max_lengthes)) * 100) for column_len in max_lengthes]
         else:
             split_percentages = None
 
         header_columns = ["Step", "Handler", "Output Shape"]
-        header_row = create_row(header_columns, split_percentages=split_percentages)
+        header_row = create_row(
+            header_columns, split_percentages=split_percentages)
         m = header_row
         self.logger.info(m)
         summary_output = summary_output + m + "\n"
         m = line_separator(line_character=line_character2)
         self.logger.info(m)
         summary_output = summary_output + m + "\n"
 
         for lifecycle_idx in range(len(lifecycle_steps)):
-            lifecycle_column = [lifecycle_steps[lifecycle_idx], lifecycle_functions[lifecycle_idx], lifecycle_output[lifecycle_idx]]
+            lifecycle_column = [lifecycle_steps[lifecycle_idx],
+                                lifecycle_functions[lifecycle_idx], lifecycle_output[lifecycle_idx]]
             if lifecycle_column[1] == "None":
                 continue
-            lifecycle_row = create_row(lifecycle_column, split_percentages=split_percentages)
+            lifecycle_row = create_row(
+                lifecycle_column, split_percentages=split_percentages)
             m = lifecycle_row
             self.logger.info(m)
             summary_output = summary_output + m + "\n"
             if print_step_parameters:
                 if not lifecycle_step_parameters[lifecycle_idx] is None:
                     lifecycle_step_parameters[lifecycle_idx]()
             m = line_separator(line_character=line_character)
@@ -2197,23 +2418,22 @@
             print_params_summary()
             m = line_separator(line_character=line_character2)
             self.logger.info(m)
             summary_output = summary_output + m + "\n"
         return summary_output
 
 def load(filename):
-
     """
     Reads a saved instance of the genetic algorithm:
         -filename: Name of the file to read the instance. No extension is needed.
     Returns the genetic algorithm instance.
     """
 
     try:
         with open(filename + ".pkl", 'rb') as file:
             ga_in = cloudpickle.load(file)
     except FileNotFoundError:
-        raise FileNotFoundError("Error reading the file {filename}. Please check your inputs.".format(filename=filename))
+        raise FileNotFoundError(f"Error reading the file {filename}. Please check your inputs.")
     except:
         # raise BaseException("Error loading the file. If the file already exists, please reload all the functions previously used (e.g. fitness function).")
         raise BaseException("Error loading the file.")
-    return ga_in
+    return ga_in
```

### Comparing `pygad-3.0.1/pygad/torchga/torchga.py` & `pygad-3.1.0/pygad/torchga/torchga.py`

 * *Files identical despite different names*

### Comparing `pygad-3.0.1/pygad/utils/mutation.py` & `pygad-3.1.0/pygad/utils/mutation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,822 +1,928 @@
-"""
-The pygad.utils.mutation module has all the built-in mutation operators.
-"""
-
-import numpy
-import random
-
-import pygad
-
-class Mutation:
-    def random_mutation(self, offspring):
-
-        """
-        Applies the random mutation which changes the values of a number of genes randomly.
-        The random value is selected either using the 'gene_space' parameter or the 2 parameters 'random_mutation_min_val' and 'random_mutation_max_val'.
-        It accepts a single parameter:
-            -offspring: The offspring to mutate.
-        It returns an array of the mutated offspring.
-        """
-
-        # If the mutation values are selected from the mutation space, the attribute 'gene_space' is not None. Otherwise, it is None.
-        # When the 'mutation_probability' parameter exists (i.e. not None), then it is used in the mutation. Otherwise, the 'mutation_num_genes' parameter is used.
-
-        if self.mutation_probability is None:
-            # When the 'mutation_probability' parameter does not exist (i.e. None), then the parameter 'mutation_num_genes' is used in the mutation.
-            if not (self.gene_space is None):
-                # When the attribute 'gene_space' exists (i.e. not None), the mutation values are selected randomly from the space of values of each gene.
-                offspring = self.mutation_by_space(offspring)
-            else:
-                offspring = self.mutation_randomly(offspring)
-        else:
-            # When the 'mutation_probability' parameter exists (i.e. not None), then it is used in the mutation.
-            if not (self.gene_space is None):
-                # When the attribute 'gene_space' does not exist (i.e. None), the mutation values are selected randomly based on the continuous range specified by the 2 attributes 'random_mutation_min_val' and 'random_mutation_max_val'.
-                offspring = self.mutation_probs_by_space(offspring)
-            else:
-                offspring = self.mutation_probs_randomly(offspring)
-
-        return offspring
-
-    def mutation_by_space(self, offspring):
-
-        """
-        Applies the random mutation using the mutation values' space.
-        It accepts a single parameter:
-            -offspring: The offspring to mutate.
-        It returns an array of the mutated offspring using the mutation space.
-        """
-
-        # For each offspring, a value from the gene space is selected randomly and assigned to the selected mutated gene.
-        for offspring_idx in range(offspring.shape[0]):
-            mutation_indices = numpy.array(random.sample(range(0, self.num_genes), self.mutation_num_genes))
-            for gene_idx in mutation_indices:
-
-                if self.gene_space_nested:
-                    # Returning the current gene space from the 'gene_space' attribute.
-                    if type(self.gene_space[gene_idx]) in [numpy.ndarray, list]:
-                        curr_gene_space = self.gene_space[gene_idx].copy()
-                    else:
-                        curr_gene_space = self.gene_space[gene_idx]
-
-                    # If the gene space has only a single value, use it as the new gene value.
-                    if type(curr_gene_space) in pygad.GA.supported_int_float_types:
-                        value_from_space = curr_gene_space
-                    # If the gene space is None, apply mutation by adding a random value between the range defined by the 2 parameters 'random_mutation_min_val' and 'random_mutation_max_val'.
-                    elif curr_gene_space is None:
-                        rand_val = numpy.random.uniform(low=self.random_mutation_min_val,
-                                                        high=self.random_mutation_max_val,
-                                                        size=1)
-                        if self.mutation_by_replacement:
-                            value_from_space = rand_val
-                        else:
-                            value_from_space = offspring[offspring_idx, gene_idx] + rand_val
-                    elif type(curr_gene_space) is dict:
-                        # The gene's space of type dict specifies the lower and upper limits of a gene.
-                        if 'step' in curr_gene_space.keys():
-                            value_from_space = numpy.random.choice(numpy.arange(start=curr_gene_space['low'],
-                                                                                stop=curr_gene_space['high'],
-                                                                                step=curr_gene_space['step']),
-                                                                   size=1)
-                        else:
-                            value_from_space = numpy.random.uniform(low=curr_gene_space['low'],
-                                                                    high=curr_gene_space['high'],
-                                                                    size=1)
-                    else:
-                        # Selecting a value randomly based on the current gene's space in the 'gene_space' attribute.
-                        # If the gene space has only 1 value, then select it. The old and new values of the gene are identical.
-                        if len(curr_gene_space) == 1:
-                            value_from_space = curr_gene_space[0]
-                        # If the gene space has more than 1 value, then select a new one that is different from the current value.
-                        else:
-                            values_to_select_from = list(set(curr_gene_space) - set([offspring[offspring_idx, gene_idx]]))
-
-                            if len(values_to_select_from) == 0:
-                                value_from_space = offspring[offspring_idx, gene_idx]
-                            else:
-                                value_from_space = random.choice(values_to_select_from)
-                else:
-                    # Selecting a value randomly from the global gene space in the 'gene_space' attribute.
-                    if type(self.gene_space) is dict:
-                        # When the gene_space is assigned a dict object, then it specifies the lower and upper limits of all genes in the space.
-                        if 'step' in self.gene_space.keys():
-                            value_from_space = numpy.random.choice(numpy.arange(start=self.gene_space['low'],
-                                                                                stop=self.gene_space['high'],
-                                                                                step=self.gene_space['step']),
-                                                                   size=1)
-                        else:
-                            value_from_space = numpy.random.uniform(low=self.gene_space['low'],
-                                                                    high=self.gene_space['high'],
-                                                                    size=1)
-                    else:
-                        # If the space type is not of type dict, then a value is randomly selected from the gene_space attribute.
-                        values_to_select_from = list(set(self.gene_space) - set([offspring[offspring_idx, gene_idx]]))
-
-                        if len(values_to_select_from) == 0:
-                            value_from_space = offspring[offspring_idx, gene_idx]
-                        else:
-                            value_from_space = random.choice(values_to_select_from)
-                    # value_from_space = random.choice(self.gene_space)
-
-                if value_from_space is None:
-                    value_from_space = numpy.random.uniform(low=self.random_mutation_min_val, 
-                                                            high=self.random_mutation_max_val, 
-                                                            size=1)
-
-                # Assinging the selected value from the space to the gene.
-                if self.gene_type_single == True:
-                    if not self.gene_type[1] is None:
-                        offspring[offspring_idx, gene_idx] = numpy.round(self.gene_type[0](value_from_space),
-                                                                         self.gene_type[1])
-                    else:
-                        offspring[offspring_idx, gene_idx] = self.gene_type[0](value_from_space)
-                else:
-                    if not self.gene_type[gene_idx][1] is None:
-                        offspring[offspring_idx, gene_idx] = numpy.round(self.gene_type[gene_idx][0](value_from_space),
-                                                                         self.gene_type[gene_idx][1])
-                    else:
-                        offspring[offspring_idx, gene_idx] = self.gene_type[gene_idx][0](value_from_space)
-
-                if self.allow_duplicate_genes == False:
-                    offspring[offspring_idx], _, _ = self.solve_duplicate_genes_by_space(solution=offspring[offspring_idx],
-                                                                                         gene_type=self.gene_type,
-                                                                                         num_trials=10)
-        return offspring
-
-    def mutation_probs_by_space(self, offspring):
-
-        """
-        Applies the random mutation using the mutation values' space and the mutation probability. For each gene, if its probability is <= that mutation probability, then it will be mutated based on the mutation space.
-        It accepts a single parameter:
-            -offspring: The offspring to mutate.
-        It returns an array of the mutated offspring using the mutation space.
-        """
-
-        # For each offspring, a value from the gene space is selected randomly and assigned to the selected mutated gene.
-        for offspring_idx in range(offspring.shape[0]):
-            probs = numpy.random.random(size=offspring.shape[1])
-            for gene_idx in range(offspring.shape[1]):
-                if probs[gene_idx] <= self.mutation_probability:
-                    if self.gene_space_nested:
-                        # Returning the current gene space from the 'gene_space' attribute.
-                        if type(self.gene_space[gene_idx]) in [numpy.ndarray, list]:
-                            curr_gene_space = self.gene_space[gene_idx].copy()
-                        else:
-                            curr_gene_space = self.gene_space[gene_idx]
-        
-                        # If the gene space has only a single value, use it as the new gene value.
-                        if type(curr_gene_space) in pygad.GA.supported_int_float_types:
-                            value_from_space = curr_gene_space
-                        # If the gene space is None, apply mutation by adding a random value between the range defined by the 2 parameters 'random_mutation_min_val' and 'random_mutation_max_val'.
-                        elif curr_gene_space is None:
-                            rand_val = numpy.random.uniform(low=self.random_mutation_min_val,
-                                                            high=self.random_mutation_max_val,
-                                                            size=1)
-                            if self.mutation_by_replacement:
-                                value_from_space = rand_val
-                            else:
-                                value_from_space = offspring[offspring_idx, gene_idx] + rand_val
-                        elif type(curr_gene_space) is dict:
-                            # Selecting a value randomly from the current gene's space in the 'gene_space' attribute.
-                            if 'step' in curr_gene_space.keys():
-                                value_from_space = numpy.random.choice(numpy.arange(start=curr_gene_space['low'],
-                                                                                    stop=curr_gene_space['high'],
-                                                                                    step=curr_gene_space['step']),
-                                                                       size=1)
-                            else:
-                                value_from_space = numpy.random.uniform(low=curr_gene_space['low'],
-                                                                        high=curr_gene_space['high'],
-                                                                        size=1)
-                        else:
-                            # Selecting a value randomly from the current gene's space in the 'gene_space' attribute.
-                            # If the gene space has only 1 value, then select it. The old and new values of the gene are identical.
-                            if len(curr_gene_space) == 1:
-                                value_from_space = curr_gene_space[0]
-                            # If the gene space has more than 1 value, then select a new one that is different from the current value.
-                            else:
-                                values_to_select_from = list(set(curr_gene_space) - set([offspring[offspring_idx, gene_idx]]))
-
-                                if len(values_to_select_from) == 0:
-                                    value_from_space = offspring[offspring_idx, gene_idx]
-                                else:
-                                    value_from_space = random.choice(values_to_select_from)
-                    else:
-                        # Selecting a value randomly from the global gene space in the 'gene_space' attribute.
-                        if type(self.gene_space) is dict:
-                            if 'step' in self.gene_space.keys():
-                                value_from_space = numpy.random.choice(numpy.arange(start=self.gene_space['low'],
-                                                                                    stop=self.gene_space['high'],
-                                                                                    step=self.gene_space['step']),
-                                                                       size=1)
-                            else:
-                                value_from_space = numpy.random.uniform(low=self.gene_space['low'],
-                                                                        high=self.gene_space['high'],
-                                                                        size=1)
-                        else:
-                            values_to_select_from = list(set(self.gene_space) - set([offspring[offspring_idx, gene_idx]]))
-
-                            if len(values_to_select_from) == 0:
-                                value_from_space = offspring[offspring_idx, gene_idx]
-                            else:
-                                value_from_space = random.choice(values_to_select_from)
-
-                    # Assigning the selected value from the space to the gene.
-                    if self.gene_type_single == True:
-                        if not self.gene_type[1] is None:
-                            offspring[offspring_idx, gene_idx] = numpy.round(self.gene_type[0](value_from_space),
-                                                                             self.gene_type[1])
-                        else:
-                            offspring[offspring_idx, gene_idx] = self.gene_type[0](value_from_space)
-                    else:
-                        if not self.gene_type[gene_idx][1] is None:
-                            offspring[offspring_idx, gene_idx] = numpy.round(self.gene_type[gene_idx][0](value_from_space),
-                                                                             self.gene_type[gene_idx][1])
-                        else:
-                            offspring[offspring_idx, gene_idx] = self.gene_type[gene_idx][0](value_from_space)
-
-                    if self.allow_duplicate_genes == False:
-                        offspring[offspring_idx], _, _ = self.solve_duplicate_genes_by_space(solution=offspring[offspring_idx],
-                                                                                             gene_type=self.gene_type,
-                                                                                             num_trials=10)
-        return offspring
-
-    def mutation_randomly(self, offspring):
-
-        """
-        Applies the random mutation the mutation probability. For each gene, if its probability is <= that mutation probability, then it will be mutated randomly.
-        It accepts a single parameter:
-            -offspring: The offspring to mutate.
-        It returns an array of the mutated offspring.
-        """
-
-        # Random mutation changes one or more genes in each offspring randomly.
-        for offspring_idx in range(offspring.shape[0]):
-            mutation_indices = numpy.array(random.sample(range(0, self.num_genes), self.mutation_num_genes))
-            for gene_idx in mutation_indices:
-                # Generating a random value.
-                random_value = numpy.random.uniform(low=self.random_mutation_min_val, 
-                                                    high=self.random_mutation_max_val, 
-                                                    size=1)
-                # If the mutation_by_replacement attribute is True, then the random value replaces the current gene value.
-                if self.mutation_by_replacement:
-                    if self.gene_type_single == True:
-                        random_value = self.gene_type[0](random_value)
-                    else:
-                        random_value = self.gene_type[gene_idx][0](random_value)
-                        if type(random_value) is numpy.ndarray:
-                            random_value = random_value[0]
-               # If the mutation_by_replacement attribute is False, then the random value is added to the gene value.
-                else:
-                    if self.gene_type_single == True:
-                        random_value = self.gene_type[0](offspring[offspring_idx, gene_idx] + random_value)
-                    else:
-                        random_value = self.gene_type[gene_idx][0](offspring[offspring_idx, gene_idx] + random_value)
-                        if type(random_value) is numpy.ndarray:
-                            random_value = random_value[0]
-
-                # Round the gene
-                if self.gene_type_single == True:
-                    if not self.gene_type[1] is None:
-                        random_value = numpy.round(random_value, self.gene_type[1])
-                else:
-                    if not self.gene_type[gene_idx][1] is None:
-                        random_value = numpy.round(random_value, self.gene_type[gene_idx][1])
-
-                offspring[offspring_idx, gene_idx] = random_value
-
-                if self.allow_duplicate_genes == False:
-                    offspring[offspring_idx], _, _ = self.solve_duplicate_genes_randomly(solution=offspring[offspring_idx],
-                                                                                         min_val=self.random_mutation_min_val,
-                                                                                         max_val=self.random_mutation_max_val,
-                                                                                         mutation_by_replacement=self.mutation_by_replacement,
-                                                                                         gene_type=self.gene_type,
-                                                                                         num_trials=10)
-
-        return offspring
-
-    def mutation_probs_randomly(self, offspring):
-
-        """
-        Applies the random mutation using the mutation probability. For each gene, if its probability is <= that mutation probability, then it will be mutated randomly.
-        It accepts a single parameter:
-            -offspring: The offspring to mutate.
-        It returns an array of the mutated offspring.
-        """
-
-        # Random mutation changes one or more gene in each offspring randomly.
-        for offspring_idx in range(offspring.shape[0]):
-            probs = numpy.random.random(size=offspring.shape[1])
-            for gene_idx in range(offspring.shape[1]):
-                if probs[gene_idx] <= self.mutation_probability:
-                    # Generating a random value.
-                    random_value = numpy.random.uniform(low=self.random_mutation_min_val, 
-                                                        high=self.random_mutation_max_val, 
-                                                        size=1)
-                    # If the mutation_by_replacement attribute is True, then the random value replaces the current gene value.
-                    if self.mutation_by_replacement:
-                        if self.gene_type_single == True:
-                            random_value = self.gene_type[0](random_value)
-                        else:
-                            random_value = self.gene_type[gene_idx][0](random_value)
-                            if type(random_value) is numpy.ndarray:
-                                random_value = random_value[0]
-                    # If the mutation_by_replacement attribute is False, then the random value is added to the gene value.
-                    else:
-                        if self.gene_type_single == True:
-                            random_value = self.gene_type[0](offspring[offspring_idx, gene_idx] + random_value)
-                        else:
-                            random_value = self.gene_type[gene_idx][0](offspring[offspring_idx, gene_idx] + random_value)
-                            if type(random_value) is numpy.ndarray:
-                                random_value = random_value[0]
-
-                    # Round the gene
-                    if self.gene_type_single == True:
-                        if not self.gene_type[1] is None:
-                            random_value = numpy.round(random_value, self.gene_type[1])
-                    else:
-                        if not self.gene_type[gene_idx][1] is None:
-                            random_value = numpy.round(random_value, self.gene_type[gene_idx][1])
-
-                    offspring[offspring_idx, gene_idx] = random_value
-
-                    if self.allow_duplicate_genes == False:
-                        offspring[offspring_idx], _, _ = self.solve_duplicate_genes_randomly(solution=offspring[offspring_idx],
-                                                                                             min_val=self.random_mutation_min_val,
-                                                                                             max_val=self.random_mutation_max_val,
-                                                                                             mutation_by_replacement=self.mutation_by_replacement,
-                                                                                             gene_type=self.gene_type,
-                                                                                             num_trials=10)
-        return offspring
-
-    def swap_mutation(self, offspring):
-
-        """
-        Applies the swap mutation which interchanges the values of 2 randomly selected genes.
-        It accepts a single parameter:
-            -offspring: The offspring to mutate.
-        It returns an array of the mutated offspring.
-        """
-
-        for idx in range(offspring.shape[0]):
-            mutation_gene1 = numpy.random.randint(low=0, high=offspring.shape[1]/2, size=1)[0]
-            mutation_gene2 = mutation_gene1 + int(offspring.shape[1]/2)
-
-            temp = offspring[idx, mutation_gene1]
-            offspring[idx, mutation_gene1] = offspring[idx, mutation_gene2]
-            offspring[idx, mutation_gene2] = temp
-        return offspring
-
-    def inversion_mutation(self, offspring):
-
-        """
-        Applies the inversion mutation which selects a subset of genes and inverts them (in order).
-        It accepts a single parameter:
-            -offspring: The offspring to mutate.
-        It returns an array of the mutated offspring.
-        """
-
-        for idx in range(offspring.shape[0]):
-            mutation_gene1 = numpy.random.randint(low=0, high=numpy.ceil(offspring.shape[1]/2 + 1), size=1)[0]
-            mutation_gene2 = mutation_gene1 + int(offspring.shape[1]/2)
-
-            genes_to_scramble = numpy.flip(offspring[idx, mutation_gene1:mutation_gene2])
-            offspring[idx, mutation_gene1:mutation_gene2] = genes_to_scramble
-        return offspring
-
-    def scramble_mutation(self, offspring):
-
-        """
-        Applies the scramble mutation which selects a subset of genes and shuffles their order randomly.
-        It accepts a single parameter:
-            -offspring: The offspring to mutate.
-        It returns an array of the mutated offspring.
-        """
-
-        for idx in range(offspring.shape[0]):
-            mutation_gene1 = numpy.random.randint(low=0, high=numpy.ceil(offspring.shape[1]/2 + 1), size=1)[0]
-            mutation_gene2 = mutation_gene1 + int(offspring.shape[1]/2)
-            genes_range = numpy.arange(start=mutation_gene1, stop=mutation_gene2)
-            numpy.random.shuffle(genes_range)
-            
-            genes_to_scramble = numpy.flip(offspring[idx, genes_range])
-            offspring[idx, genes_range] = genes_to_scramble
-        return offspring
-
-    def adaptive_mutation_population_fitness(self, offspring):
-
-        """
-        A helper method to calculate the average fitness of the solutions before applying the adaptive mutation.
-        It accepts a single parameter:
-            -offspring: The offspring to mutate.
-        It returns the average fitness to be used in adaptive mutation.
-        """        
-
-        fitness = self.last_generation_fitness.copy()
-        temp_population = numpy.zeros_like(self.population)
-
-        if (self.keep_elitism == 0):
-            if (self.keep_parents == 0):
-                parents_to_keep = []
-            elif (self.keep_parents == -1):
-                parents_to_keep = self.last_generation_parents.copy()
-                temp_population[0:len(parents_to_keep), :] = parents_to_keep
-            elif (self.keep_parents > 0):
-                parents_to_keep, _ = self.steady_state_selection(self.last_generation_fitness, num_parents=self.keep_parents)
-                temp_population[0:len(parents_to_keep), :] = parents_to_keep
-        else:
-            parents_to_keep, _ = self.steady_state_selection(self.last_generation_fitness, num_parents=self.keep_elitism)
-            temp_population[0:len(parents_to_keep), :] = parents_to_keep
-
-        temp_population[len(parents_to_keep):, :] = offspring
-
-        fitness[:self.last_generation_parents.shape[0]] = self.last_generation_fitness[self.last_generation_parents_indices]
-
-        for idx in range(len(parents_to_keep), fitness.shape[0]):
-            fitness[idx] = self.fitness_func(self, temp_population[idx], None)
-        average_fitness = numpy.mean(fitness)
-
-        return average_fitness, fitness[len(parents_to_keep):]
-
-    def adaptive_mutation(self, offspring):
-
-        """
-        Applies the adaptive mutation which changes the values of a number of genes randomly. In adaptive mutation, the number of genes to mutate differs based on the fitness value of the solution.
-        The random value is selected either using the 'gene_space' parameter or the 2 parameters 'random_mutation_min_val' and 'random_mutation_max_val'.
-        It accepts a single parameter:
-            -offspring: The offspring to mutate.
-        It returns an array of the mutated offspring.
-        """
-
-        # If the attribute 'gene_space' exists (i.e. not None), then the mutation values are selected from the 'gene_space' parameter according to the space of values of each gene. Otherwise, it is selected randomly based on the 2 parameters 'random_mutation_min_val' and 'random_mutation_max_val'.
-        # When the 'mutation_probability' parameter exists (i.e. not None), then it is used in the mutation. Otherwise, the 'mutation_num_genes' parameter is used.
-
-        if self.mutation_probability is None:
-            # When the 'mutation_probability' parameter does not exist (i.e. None), then the parameter 'mutation_num_genes' is used in the mutation.
-            if not (self.gene_space is None):
-                # When the attribute 'gene_space' exists (i.e. not None), the mutation values are selected randomly from the space of values of each gene.
-                offspring = self.adaptive_mutation_by_space(offspring)
-            else:
-                # When the attribute 'gene_space' does not exist (i.e. None), the mutation values are selected randomly based on the continuous range specified by the 2 attributes 'random_mutation_min_val' and 'random_mutation_max_val'.
-                offspring = self.adaptive_mutation_randomly(offspring)
-        else:
-            # When the 'mutation_probability' parameter exists (i.e. not None), then it is used in the mutation.
-            if not (self.gene_space is None):
-                # When the attribute 'gene_space' exists (i.e. not None), the mutation values are selected randomly from the space of values of each gene.
-                offspring = self.adaptive_mutation_probs_by_space(offspring)
-            else:
-                # When the attribute 'gene_space' does not exist (i.e. None), the mutation values are selected randomly based on the continuous range specified by the 2 attributes 'random_mutation_min_val' and 'random_mutation_max_val'.
-                offspring = self.adaptive_mutation_probs_randomly(offspring)
-
-        return offspring
-
-    def adaptive_mutation_by_space(self, offspring):
-
-        """
-        Applies the adaptive mutation based on the 2 parameters 'mutation_num_genes' and 'gene_space'. 
-        A number of genes equal are selected randomly for mutation. This number depends on the fitness of the solution.
-        The random values are selected from the 'gene_space' parameter.
-        It accepts a single parameter:
-            -offspring: The offspring to mutate.
-        It returns an array of the mutated offspring.
-        """
-        
-        # For each offspring, a value from the gene space is selected randomly and assigned to the selected gene for mutation.
-
-        average_fitness, offspring_fitness = self.adaptive_mutation_population_fitness(offspring)
-
-        # Adaptive mutation changes one or more genes in each offspring randomly.
-        # The number of genes to mutate depends on the solution's fitness value.
-        for offspring_idx in range(offspring.shape[0]):
-            if offspring_fitness[offspring_idx] < average_fitness:
-                adaptive_mutation_num_genes = self.mutation_num_genes[0]
-            else:
-                adaptive_mutation_num_genes = self.mutation_num_genes[1]
-            mutation_indices = numpy.array(random.sample(range(0, self.num_genes), adaptive_mutation_num_genes))
-            for gene_idx in mutation_indices:
-
-                if self.gene_space_nested:
-                    # Returning the current gene space from the 'gene_space' attribute.
-                    if type(self.gene_space[gene_idx]) in [numpy.ndarray, list]:
-                        curr_gene_space = self.gene_space[gene_idx].copy()
-                    else:
-                        curr_gene_space = self.gene_space[gene_idx]
-
-                    # If the gene space has only a single value, use it as the new gene value.
-                    if type(curr_gene_space) in pygad.GA.supported_int_float_types:
-                        value_from_space = curr_gene_space
-                    # If the gene space is None, apply mutation by adding a random value between the range defined by the 2 parameters 'random_mutation_min_val' and 'random_mutation_max_val'.
-                    elif curr_gene_space is None:
-                        rand_val = numpy.random.uniform(low=self.random_mutation_min_val,
-                                                        high=self.random_mutation_max_val,
-                                                        size=1)
-                        if self.mutation_by_replacement:
-                            value_from_space = rand_val
-                        else:
-                            value_from_space = offspring[offspring_idx, gene_idx] + rand_val
-                    elif type(curr_gene_space) is dict:
-                            # Selecting a value randomly from the current gene's space in the 'gene_space' attribute.
-                            if 'step' in curr_gene_space.keys():
-                                value_from_space = numpy.random.choice(numpy.arange(start=curr_gene_space['low'],
-                                                                                    stop=curr_gene_space['high'],
-                                                                                    step=curr_gene_space['step']),
-                                                                       size=1)
-                            else:
-                                value_from_space = numpy.random.uniform(low=curr_gene_space['low'],
-                                                                        high=curr_gene_space['high'],
-                                                                        size=1)
-                    else:
-                        # Selecting a value randomly from the current gene's space in the 'gene_space' attribute.
-                        # If the gene space has only 1 value, then select it. The old and new values of the gene are identical.
-                        if len(curr_gene_space) == 1:
-                            value_from_space = curr_gene_space[0]
-                        # If the gene space has more than 1 value, then select a new one that is different from the current value.
-                        else:
-                            values_to_select_from = list(set(curr_gene_space) - set([offspring[offspring_idx, gene_idx]]))
-
-                            if len(values_to_select_from) == 0:
-                                value_from_space = offspring[offspring_idx, gene_idx]
-                            else:
-                                value_from_space = random.choice(values_to_select_from)
-                else:
-                    # Selecting a value randomly from the global gene space in the 'gene_space' attribute.
-                    if type(self.gene_space) is dict:
-                        if 'step' in self.gene_space.keys():
-                            value_from_space = numpy.random.choice(numpy.arange(start=self.gene_space['low'],
-                                                                                stop=self.gene_space['high'],
-                                                                                step=self.gene_space['step']),
-                                                                   size=1)
-                        else:
-                            value_from_space = numpy.random.uniform(low=self.gene_space['low'],
-                                                                    high=self.gene_space['high'],
-                                                                    size=1)
-                    else:
-                        values_to_select_from = list(set(self.gene_space) - set([offspring[offspring_idx, gene_idx]]))
-
-                        if len(values_to_select_from) == 0:
-                            value_from_space = offspring[offspring_idx, gene_idx]
-                        else:
-                            value_from_space = random.choice(values_to_select_from)
-
-
-                if value_from_space is None:
-                    value_from_space = numpy.random.uniform(low=self.random_mutation_min_val, 
-                                                            high=self.random_mutation_max_val, 
-                                                            size=1)
-
-                # Assinging the selected value from the space to the gene.
-                if self.gene_type_single == True:
-                    if not self.gene_type[1] is None:
-                        offspring[offspring_idx, gene_idx] = numpy.round(self.gene_type[0](value_from_space),
-                                                                         self.gene_type[1])
-                    else:
-                        offspring[offspring_idx, gene_idx] = self.gene_type[0](value_from_space)
-                else:
-                    if not self.gene_type[gene_idx][1] is None:
-                        offspring[offspring_idx, gene_idx] = numpy.round(self.gene_type[gene_idx][0](value_from_space),
-                                                                         self.gene_type[gene_idx][1])
-                    else:
-                        offspring[offspring_idx, gene_idx] = self.gene_type[gene_idx][0](value_from_space)
-
-                if self.allow_duplicate_genes == False:
-                    offspring[offspring_idx], _, _ = self.solve_duplicate_genes_by_space(solution=offspring[offspring_idx],
-                                                                                         gene_type=self.gene_type,
-                                                                                         num_trials=10)
-        return offspring
-        
-    def adaptive_mutation_randomly(self, offspring):
-
-        """
-        Applies the adaptive mutation based on the 'mutation_num_genes' parameter. 
-        A number of genes equal are selected randomly for mutation. This number depends on the fitness of the solution.
-        The random values are selected based on the 2 parameters 'random_mutation_min_val' and 'random_mutation_max_val'.
-        It accepts a single parameter:
-            -offspring: The offspring to mutate.
-        It returns an array of the mutated offspring.
-        """
-
-        average_fitness, offspring_fitness = self.adaptive_mutation_population_fitness(offspring)
-
-        # Adaptive random mutation changes one or more genes in each offspring randomly.
-        # The number of genes to mutate depends on the solution's fitness value.
-        for offspring_idx in range(offspring.shape[0]):
-            if offspring_fitness[offspring_idx] < average_fitness:
-                adaptive_mutation_num_genes = self.mutation_num_genes[0]
-            else:
-                adaptive_mutation_num_genes = self.mutation_num_genes[1]
-            mutation_indices = numpy.array(random.sample(range(0, self.num_genes), adaptive_mutation_num_genes))
-            for gene_idx in mutation_indices:
-                # Generating a random value.
-                random_value = numpy.random.uniform(low=self.random_mutation_min_val, 
-                                                    high=self.random_mutation_max_val, 
-                                                    size=1)
-                # If the mutation_by_replacement attribute is True, then the random value replaces the current gene value.
-                if self.mutation_by_replacement:
-                    if self.gene_type_single == True:
-                        random_value = self.gene_type[0](random_value)
-                    else:
-                        random_value = self.gene_type[gene_idx][0](random_value)
-                        if type(random_value) is numpy.ndarray:
-                            random_value = random_value[0]
-                # If the mutation_by_replacement attribute is False, then the random value is added to the gene value.
-                else:
-                    if self.gene_type_single == True:
-                        random_value = self.gene_type[0](offspring[offspring_idx, gene_idx] + random_value)
-                    else:
-                        random_value = self.gene_type[gene_idx][0](offspring[offspring_idx, gene_idx] + random_value)
-                        if type(random_value) is numpy.ndarray:
-                            random_value = random_value[0]
-
-                if self.gene_type_single == True:
-                    if not self.gene_type[1] is None:
-                        random_value = numpy.round(random_value, self.gene_type[1])
-                else:
-                    if not self.gene_type[gene_idx][1] is None:
-                        random_value = numpy.round(random_value, self.gene_type[gene_idx][1])
-
-                offspring[offspring_idx, gene_idx] = random_value
-
-                if self.allow_duplicate_genes == False:
-                    offspring[offspring_idx], _, _ = self.solve_duplicate_genes_randomly(solution=offspring[offspring_idx],
-                                                                                         min_val=self.random_mutation_min_val,
-                                                                                         max_val=self.random_mutation_max_val,
-                                                                                         mutation_by_replacement=self.mutation_by_replacement,
-                                                                                         gene_type=self.gene_type,
-                                                                                         num_trials=10)
-        return offspring
-
-    def adaptive_mutation_probs_by_space(self, offspring):
-
-        """
-        Applies the adaptive mutation based on the 2 parameters 'mutation_probability' and 'gene_space'.
-        Based on whether the solution fitness is above or below a threshold, the mutation is applied diffrently by mutating high or low number of genes.
-        The random values are selected based on space of values for each gene.
-        It accepts a single parameter:
-            -offspring: The offspring to mutate.
-        It returns an array of the mutated offspring.
-        """
-
-        # For each offspring, a value from the gene space is selected randomly and assigned to the selected gene for mutation.
-
-        average_fitness, offspring_fitness = self.adaptive_mutation_population_fitness(offspring)
-
-        # Adaptive random mutation changes one or more genes in each offspring randomly.
-        # The probability of mutating a gene depends on the solution's fitness value.
-        for offspring_idx in range(offspring.shape[0]):
-            if offspring_fitness[offspring_idx] < average_fitness:
-                adaptive_mutation_probability = self.mutation_probability[0]
-            else:
-                adaptive_mutation_probability = self.mutation_probability[1]
-
-            probs = numpy.random.random(size=offspring.shape[1])
-            for gene_idx in range(offspring.shape[1]):
-                if probs[gene_idx] <= adaptive_mutation_probability:
-                    if self.gene_space_nested:
-                        # Returning the current gene space from the 'gene_space' attribute.
-                        if type(self.gene_space[gene_idx]) in [numpy.ndarray, list]:
-                            curr_gene_space = self.gene_space[gene_idx].copy()
-                        else:
-                            curr_gene_space = self.gene_space[gene_idx]
-        
-                        # If the gene space has only a single value, use it as the new gene value.
-                        if type(curr_gene_space) in pygad.GA.supported_int_float_types:
-                            value_from_space = curr_gene_space
-                        # If the gene space is None, apply mutation by adding a random value between the range defined by the 2 parameters 'random_mutation_min_val' and 'random_mutation_max_val'.
-                        elif curr_gene_space is None:
-                            rand_val = numpy.random.uniform(low=self.random_mutation_min_val,
-                                                            high=self.random_mutation_max_val,
-                                                            size=1)
-                            if self.mutation_by_replacement:
-                                value_from_space = rand_val
-                            else:
-                                value_from_space = offspring[offspring_idx, gene_idx] + rand_val
-                        elif type(curr_gene_space) is dict:
-                            # Selecting a value randomly from the current gene's space in the 'gene_space' attribute.
-                            if 'step' in curr_gene_space.keys():
-                                value_from_space = numpy.random.choice(numpy.arange(start=curr_gene_space['low'],
-                                                                                    stop=curr_gene_space['high'],
-                                                                                    step=curr_gene_space['step']),
-                                                                       size=1)
-                            else:
-                                value_from_space = numpy.random.uniform(low=curr_gene_space['low'],
-                                                                        high=curr_gene_space['high'],
-                                                                        size=1)
-                        else:
-                            # Selecting a value randomly from the current gene's space in the 'gene_space' attribute.
-                            # If the gene space has only 1 value, then select it. The old and new values of the gene are identical.
-                            if len(curr_gene_space) == 1:
-                                value_from_space = curr_gene_space[0]
-                            # If the gene space has more than 1 value, then select a new one that is different from the current value.
-                            else:
-                                values_to_select_from = list(set(curr_gene_space) - set([offspring[offspring_idx, gene_idx]]))
-
-                                if len(values_to_select_from) == 0:
-                                    value_from_space = offspring[offspring_idx, gene_idx]
-                                else:
-                                    value_from_space = random.choice(values_to_select_from)
-                    else:
-                        # Selecting a value randomly from the global gene space in the 'gene_space' attribute.
-                        if type(self.gene_space) is dict:
-                            if 'step' in self.gene_space.keys():
-                                value_from_space = numpy.random.choice(numpy.arange(start=self.gene_space['low'],
-                                                                                    stop=self.gene_space['high'],
-                                                                                    step=self.gene_space['step']),
-                                                                       size=1)
-                            else:
-                                value_from_space = numpy.random.uniform(low=self.gene_space['low'],
-                                                                        high=self.gene_space['high'],
-                                                                        size=1)
-                        else:
-                            values_to_select_from = list(set(self.gene_space) - set([offspring[offspring_idx, gene_idx]]))
-
-                            if len(values_to_select_from) == 0:
-                                value_from_space = offspring[offspring_idx, gene_idx]
-                            else:
-                                value_from_space = random.choice(values_to_select_from)
-
-                    if value_from_space is None:
-                        value_from_space = numpy.random.uniform(low=self.random_mutation_min_val, 
-                                                                high=self.random_mutation_max_val, 
-                                                                size=1)
-
-                    # Assinging the selected value from the space to the gene.
-                    if self.gene_type_single == True:
-                        if not self.gene_type[1] is None:
-                            offspring[offspring_idx, gene_idx] = numpy.round(self.gene_type[0](value_from_space),
-                                                                             self.gene_type[1])
-                        else:
-                            offspring[offspring_idx, gene_idx] = self.gene_type[0](value_from_space)
-                    else:
-                        if not self.gene_type[gene_idx][1] is None:
-                            offspring[offspring_idx, gene_idx] = numpy.round(self.gene_type[gene_idx][0](value_from_space),
-                                                                             self.gene_type[gene_idx][1])
-                        else:
-                            offspring[offspring_idx, gene_idx] = self.gene_type[gene_idx][0](value_from_space)
-
-                    if self.allow_duplicate_genes == False:
-                        offspring[offspring_idx], _, _ = self.solve_duplicate_genes_by_space(solution=offspring[offspring_idx],
-                                                                                             gene_type=self.gene_type,
-                                                                                             num_trials=10)
-        return offspring
-
-    def adaptive_mutation_probs_randomly(self, offspring):
-
-        """
-        Applies the adaptive mutation based on the 'mutation_probability' parameter. 
-        Based on whether the solution fitness is above or below a threshold, the mutation is applied diffrently by mutating high or low number of genes.
-        The random values are selected based on the 2 parameters 'random_mutation_min_val' and 'random_mutation_max_val'.
-        It accepts a single parameter:
-            -offspring: The offspring to mutate.
-        It returns an array of the mutated offspring.
-        """
-
-        average_fitness, offspring_fitness = self.adaptive_mutation_population_fitness(offspring)
-
-        # Adaptive random mutation changes one or more genes in each offspring randomly.
-        # The probability of mutating a gene depends on the solution's fitness value.
-        for offspring_idx in range(offspring.shape[0]):
-            if offspring_fitness[offspring_idx] < average_fitness:
-                adaptive_mutation_probability = self.mutation_probability[0]
-            else:
-                adaptive_mutation_probability = self.mutation_probability[1]
-
-            probs = numpy.random.random(size=offspring.shape[1])
-            for gene_idx in range(offspring.shape[1]):
-                if probs[gene_idx] <= adaptive_mutation_probability:
-                    # Generating a random value.
-                    random_value = numpy.random.uniform(low=self.random_mutation_min_val, 
-                                                        high=self.random_mutation_max_val, 
-                                                        size=1)
-                    # If the mutation_by_replacement attribute is True, then the random value replaces the current gene value.
-                    if self.mutation_by_replacement:
-                        if self.gene_type_single == True:
-                            random_value = self.gene_type[0](random_value)
-                        else:
-                            random_value = self.gene_type[gene_idx][0](random_value)
-                            if type(random_value) is numpy.ndarray:
-                                random_value = random_value[0]
-                    # If the mutation_by_replacement attribute is False, then the random value is added to the gene value.
-                    else:
-                        if self.gene_type_single == True:
-                            random_value = self.gene_type[0](offspring[offspring_idx, gene_idx] + random_value)
-                        else:
-                            random_value = self.gene_type[gene_idx][0](offspring[offspring_idx, gene_idx] + random_value)
-                            if type(random_value) is numpy.ndarray:
-                                random_value = random_value[0]
-
-                    if self.gene_type_single == True:
-                        if not self.gene_type[1] is None:
-                            random_value = numpy.round(random_value, self.gene_type[1])
-                    else:
-                        if not self.gene_type[gene_idx][1] is None:
-                            random_value = numpy.round(random_value, self.gene_type[gene_idx][1])
-
-                    offspring[offspring_idx, gene_idx] = random_value
-
-                    if self.allow_duplicate_genes == False:
-                        offspring[offspring_idx], _, _ = self.solve_duplicate_genes_randomly(solution=offspring[offspring_idx],
-                                                                                             min_val=self.random_mutation_min_val,
-                                                                                             max_val=self.random_mutation_max_val,
-                                                                                             mutation_by_replacement=self.mutation_by_replacement,
-                                                                                             gene_type=self.gene_type,
-                                                                                             num_trials=10)
-        return offspring
+"""
+The pygad.utils.mutation module has all the built-in mutation operators.
+"""
+
+import numpy
+import random
+
+import pygad
+
+class Mutation:
+
+    def random_mutation(self, offspring):
+
+        """
+        Applies the random mutation which changes the values of a number of genes randomly.
+        The random value is selected either using the 'gene_space' parameter or the 2 parameters 'random_mutation_min_val' and 'random_mutation_max_val'.
+        It accepts a single parameter:
+            -offspring: The offspring to mutate.
+        It returns an array of the mutated offspring.
+        """
+
+        # If the mutation values are selected from the mutation space, the attribute 'gene_space' is not None. Otherwise, it is None.
+        # When the 'mutation_probability' parameter exists (i.e. not None), then it is used in the mutation. Otherwise, the 'mutation_num_genes' parameter is used.
+
+        if self.mutation_probability is None:
+            # When the 'mutation_probability' parameter does not exist (i.e. None), then the parameter 'mutation_num_genes' is used in the mutation.
+            if not (self.gene_space is None):
+                # When the attribute 'gene_space' exists (i.e. not None), the mutation values are selected randomly from the space of values of each gene.
+                offspring = self.mutation_by_space(offspring)
+            else:
+                offspring = self.mutation_randomly(offspring)
+        else:
+            # When the 'mutation_probability' parameter exists (i.e. not None), then it is used in the mutation.
+            if not (self.gene_space is None):
+                # When the attribute 'gene_space' does not exist (i.e. None), the mutation values are selected randomly based on the continuous range specified by the 2 attributes 'random_mutation_min_val' and 'random_mutation_max_val'.
+                offspring = self.mutation_probs_by_space(offspring)
+            else:
+                offspring = self.mutation_probs_randomly(offspring)
+
+        return offspring
+
+    def mutation_by_space(self, offspring):
+
+        """
+        Applies the random mutation using the mutation values' space.
+        It accepts a single parameter:
+            -offspring: The offspring to mutate.
+        It returns an array of the mutated offspring using the mutation space.
+        """
+
+        # For each offspring, a value from the gene space is selected randomly and assigned to the selected mutated gene.
+        for offspring_idx in range(offspring.shape[0]):
+            mutation_indices = numpy.array(random.sample(range(0, self.num_genes), self.mutation_num_genes))
+            for gene_idx in mutation_indices:
+
+                if type(self.random_mutation_min_val) in self.supported_int_float_types:
+                    range_min = self.random_mutation_min_val
+                    range_max = self.random_mutation_max_val
+                else:
+                    range_min = self.random_mutation_min_val[gene_idx]
+                    range_max = self.random_mutation_max_val[gene_idx]
+
+                if self.gene_space_nested:
+                    # Returning the current gene space from the 'gene_space' attribute.
+                    if type(self.gene_space[gene_idx]) in [numpy.ndarray, list]:
+                        curr_gene_space = self.gene_space[gene_idx].copy()
+                    else:
+                        curr_gene_space = self.gene_space[gene_idx]
+
+                    # If the gene space has only a single value, use it as the new gene value.
+                    if type(curr_gene_space) in pygad.GA.supported_int_float_types:
+                        value_from_space = curr_gene_space
+                    # If the gene space is None, apply mutation by adding a random value between the range defined by the 2 parameters 'random_mutation_min_val' and 'random_mutation_max_val'.
+                    elif curr_gene_space is None:
+                        rand_val = numpy.random.uniform(low=range_min,
+                                                        high=range_max,
+                                                        size=1)[0]
+                        if self.mutation_by_replacement:
+                            value_from_space = rand_val
+                        else:
+                            value_from_space = offspring[offspring_idx, gene_idx] + rand_val
+                    elif type(curr_gene_space) is dict:
+                        # The gene's space of type dict specifies the lower and upper limits of a gene.
+                        if 'step' in curr_gene_space.keys():
+                            # The numpy.random.choice() and numpy.random.uniform() functions return a NumPy array as the output even if the array has a single value.
+                            # We have to return the output at index 0 to force a numeric value to be returned not an object of type numpy.ndarray. 
+                            # If numpy.ndarray is returned, then it will cause an issue later while using the set() function.
+                            value_from_space = numpy.random.choice(numpy.arange(start=curr_gene_space['low'],
+                                                                                stop=curr_gene_space['high'],
+                                                                                step=curr_gene_space['step']),
+                                                                   size=1)[0]
+                        else:
+                            value_from_space = numpy.random.uniform(low=curr_gene_space['low'],
+                                                                    high=curr_gene_space['high'],
+                                                                    size=1)[0]
+                    else:
+                        # Selecting a value randomly based on the current gene's space in the 'gene_space' attribute.
+                        # If the gene space has only 1 value, then select it. The old and new values of the gene are identical.
+                        if len(curr_gene_space) == 1:
+                            value_from_space = curr_gene_space[0]
+                        # If the gene space has more than 1 value, then select a new one that is different from the current value.
+                        else:
+                            values_to_select_from = list(set(curr_gene_space) - set([offspring[offspring_idx, gene_idx]]))
+
+                            if len(values_to_select_from) == 0:
+                                value_from_space = offspring[offspring_idx, gene_idx]
+                            else:
+                                value_from_space = random.choice(values_to_select_from)
+                else:
+                    # Selecting a value randomly from the global gene space in the 'gene_space' attribute.
+                    if type(self.gene_space) is dict:
+                        # When the gene_space is assigned a dict object, then it specifies the lower and upper limits of all genes in the space.
+                        if 'step' in self.gene_space.keys():
+                            value_from_space = numpy.random.choice(numpy.arange(start=self.gene_space['low'],
+                                                                                stop=self.gene_space['high'],
+                                                                                step=self.gene_space['step']),
+                                                                   size=1)[0]
+                        else:
+                            value_from_space = numpy.random.uniform(low=self.gene_space['low'],
+                                                                    high=self.gene_space['high'],
+                                                                    size=1)[0]
+                    else:
+                        # If the space type is not of type dict, then a value is randomly selected from the gene_space attribute.
+                        values_to_select_from = list(set(self.gene_space) - set([offspring[offspring_idx, gene_idx]]))
+
+                        if len(values_to_select_from) == 0:
+                            value_from_space = offspring[offspring_idx, gene_idx]
+                        else:
+                            value_from_space = random.choice(values_to_select_from)
+                    # value_from_space = random.choice(self.gene_space)
+
+                if value_from_space is None:
+                    # TODO: Return index 0.
+                    # TODO: Check if this if statement is necessary.
+                    value_from_space = numpy.random.uniform(low=range_min, 
+                                                            high=range_max, 
+                                                            size=1)[0]
+
+                # Assinging the selected value from the space to the gene.
+                if self.gene_type_single == True:
+                    if not self.gene_type[1] is None:
+                        offspring[offspring_idx, gene_idx] = numpy.round(self.gene_type[0](value_from_space),
+                                                                         self.gene_type[1])
+                    else:
+                        offspring[offspring_idx, gene_idx] = self.gene_type[0](value_from_space)
+                else:
+                    if not self.gene_type[gene_idx][1] is None:
+                        offspring[offspring_idx, gene_idx] = numpy.round(self.gene_type[gene_idx][0](value_from_space),
+                                                                         self.gene_type[gene_idx][1])
+
+                    else:
+                        offspring[offspring_idx, gene_idx] = self.gene_type[gene_idx][0](value_from_space)
+
+                if self.allow_duplicate_genes == False:
+                    offspring[offspring_idx], _, _ = self.solve_duplicate_genes_by_space(solution=offspring[offspring_idx],
+                                                                                         gene_type=self.gene_type,
+                                                                                         num_trials=10)
+        return offspring
+
+    def mutation_probs_by_space(self, offspring):
+
+        """
+        Applies the random mutation using the mutation values' space and the mutation probability. For each gene, if its probability is <= that mutation probability, then it will be mutated based on the mutation space.
+        It accepts a single parameter:
+            -offspring: The offspring to mutate.
+        It returns an array of the mutated offspring using the mutation space.
+        """
+
+        # For each offspring, a value from the gene space is selected randomly and assigned to the selected mutated gene.
+        for offspring_idx in range(offspring.shape[0]):
+            probs = numpy.random.random(size=offspring.shape[1])
+            for gene_idx in range(offspring.shape[1]):
+
+                if type(self.random_mutation_min_val) in self.supported_int_float_types:
+                    range_min = self.random_mutation_min_val
+                    range_max = self.random_mutation_max_val
+                else:
+                    range_min = self.random_mutation_min_val[gene_idx]
+                    range_max = self.random_mutation_max_val[gene_idx]
+
+                if probs[gene_idx] <= self.mutation_probability:
+                    if self.gene_space_nested:
+                        # Returning the current gene space from the 'gene_space' attribute.
+                        if type(self.gene_space[gene_idx]) in [numpy.ndarray, list]:
+                            curr_gene_space = self.gene_space[gene_idx].copy()
+                        else:
+                            curr_gene_space = self.gene_space[gene_idx]
+        
+                        # If the gene space has only a single value, use it as the new gene value.
+                        if type(curr_gene_space) in pygad.GA.supported_int_float_types:
+                            value_from_space = curr_gene_space
+                        # If the gene space is None, apply mutation by adding a random value between the range defined by the 2 parameters 'random_mutation_min_val' and 'random_mutation_max_val'.
+                        elif curr_gene_space is None:
+                            rand_val = numpy.random.uniform(low=range_min,
+                                                            high=range_max,
+                                                            size=1)[0]
+                            if self.mutation_by_replacement:
+                                value_from_space = rand_val
+                            else:
+                                value_from_space = offspring[offspring_idx, gene_idx] + rand_val
+                        elif type(curr_gene_space) is dict:
+                            # Selecting a value randomly from the current gene's space in the 'gene_space' attribute.
+                            if 'step' in curr_gene_space.keys():
+                                value_from_space = numpy.random.choice(numpy.arange(start=curr_gene_space['low'],
+                                                                                    stop=curr_gene_space['high'],
+                                                                                    step=curr_gene_space['step']),
+                                                                       size=1)[0]
+                            else:
+                                value_from_space = numpy.random.uniform(low=curr_gene_space['low'],
+                                                                        high=curr_gene_space['high'],
+                                                                        size=1)[0]
+                        else:
+                            # Selecting a value randomly from the current gene's space in the 'gene_space' attribute.
+                            # If the gene space has only 1 value, then select it. The old and new values of the gene are identical.
+                            if len(curr_gene_space) == 1:
+                                value_from_space = curr_gene_space[0]
+                            # If the gene space has more than 1 value, then select a new one that is different from the current value.
+                            else:
+                                values_to_select_from = list(set(curr_gene_space) - set([offspring[offspring_idx, gene_idx]]))
+
+                                if len(values_to_select_from) == 0:
+                                    value_from_space = offspring[offspring_idx, gene_idx]
+                                else:
+                                    value_from_space = random.choice(values_to_select_from)
+                    else:
+                        # Selecting a value randomly from the global gene space in the 'gene_space' attribute.
+                        if type(self.gene_space) is dict:
+                            if 'step' in self.gene_space.keys():
+                                value_from_space = numpy.random.choice(numpy.arange(start=self.gene_space['low'],
+                                                                                    stop=self.gene_space['high'],
+                                                                                    step=self.gene_space['step']),
+                                                                       size=1)[0]
+                            else:
+                                value_from_space = numpy.random.uniform(low=self.gene_space['low'],
+                                                                        high=self.gene_space['high'],
+                                                                        size=1)[0]
+                        else:
+                            values_to_select_from = list(set(self.gene_space) - set([offspring[offspring_idx, gene_idx]]))
+
+                            if len(values_to_select_from) == 0:
+                                value_from_space = offspring[offspring_idx, gene_idx]
+                            else:
+                                value_from_space = random.choice(values_to_select_from)
+
+                    # Assigning the selected value from the space to the gene.
+                    if self.gene_type_single == True:
+                        if not self.gene_type[1] is None:
+                            offspring[offspring_idx, gene_idx] = numpy.round(self.gene_type[0](value_from_space),
+                                                                             self.gene_type[1])
+                        else:
+                            offspring[offspring_idx, gene_idx] = self.gene_type[0](value_from_space)
+                    else:
+                        if not self.gene_type[gene_idx][1] is None:
+                            offspring[offspring_idx, gene_idx] = numpy.round(self.gene_type[gene_idx][0](value_from_space),
+                                                                             self.gene_type[gene_idx][1])
+                        else:
+                            offspring[offspring_idx, gene_idx] = self.gene_type[gene_idx][0](value_from_space)
+
+                    if self.allow_duplicate_genes == False:
+                        offspring[offspring_idx], _, _ = self.solve_duplicate_genes_by_space(solution=offspring[offspring_idx],
+                                                                                             gene_type=self.gene_type,
+                                                                                             num_trials=10)
+        return offspring
+
+    def mutation_randomly(self, offspring):
+
+        """
+        Applies the random mutation the mutation probability. For each gene, if its probability is <= that mutation probability, then it will be mutated randomly.
+        It accepts a single parameter:
+            -offspring: The offspring to mutate.
+        It returns an array of the mutated offspring.
+        """
+
+        # Random mutation changes one or more genes in each offspring randomly.
+        for offspring_idx in range(offspring.shape[0]):
+            mutation_indices = numpy.array(random.sample(range(0, self.num_genes), self.mutation_num_genes))
+            for gene_idx in mutation_indices:
+
+                if type(self.random_mutation_min_val) in self.supported_int_float_types:
+                    range_min = self.random_mutation_min_val
+                    range_max = self.random_mutation_max_val
+                else:
+                    range_min = self.random_mutation_min_val[gene_idx]
+                    range_max = self.random_mutation_max_val[gene_idx]
+
+                # Generating a random value.
+                random_value = numpy.random.uniform(low=range_min, 
+                                                    high=range_max, 
+                                                    size=1)[0]
+                # If the mutation_by_replacement attribute is True, then the random value replaces the current gene value.
+                if self.mutation_by_replacement:
+                    if self.gene_type_single == True:
+                        random_value = self.gene_type[0](random_value)
+                    else:
+                        random_value = self.gene_type[gene_idx][0](random_value)
+                        if type(random_value) is numpy.ndarray:
+                            random_value = random_value[0]
+               # If the mutation_by_replacement attribute is False, then the random value is added to the gene value.
+                else:
+                    if self.gene_type_single == True:
+                        random_value = self.gene_type[0](offspring[offspring_idx, gene_idx] + random_value)
+                    else:
+                        random_value = self.gene_type[gene_idx][0](offspring[offspring_idx, gene_idx] + random_value)
+                        if type(random_value) is numpy.ndarray:
+                            random_value = random_value[0]
+
+                # Round the gene
+                if self.gene_type_single == True:
+                    if not self.gene_type[1] is None:
+                        random_value = numpy.round(random_value, self.gene_type[1])
+                else:
+                    if not self.gene_type[gene_idx][1] is None:
+                        random_value = numpy.round(random_value, self.gene_type[gene_idx][1])
+
+                offspring[offspring_idx, gene_idx] = random_value
+
+                if self.allow_duplicate_genes == False:
+                    offspring[offspring_idx], _, _ = self.solve_duplicate_genes_randomly(solution=offspring[offspring_idx],
+                                                                                         min_val=range_min,
+                                                                                         max_val=range_max,
+                                                                                         mutation_by_replacement=self.mutation_by_replacement,
+                                                                                         gene_type=self.gene_type,
+                                                                                         num_trials=10)
+
+        return offspring
+
+    def mutation_probs_randomly(self, offspring):
+
+        """
+        Applies the random mutation using the mutation probability. For each gene, if its probability is <= that mutation probability, then it will be mutated randomly.
+        It accepts a single parameter:
+            -offspring: The offspring to mutate.
+        It returns an array of the mutated offspring.
+        """
+
+        # Random mutation changes one or more gene in each offspring randomly.
+        for offspring_idx in range(offspring.shape[0]):
+            probs = numpy.random.random(size=offspring.shape[1])
+            for gene_idx in range(offspring.shape[1]):
+
+                if type(self.random_mutation_min_val) in self.supported_int_float_types:
+                    range_min = self.random_mutation_min_val
+                    range_max = self.random_mutation_max_val
+                else:
+                    range_min = self.random_mutation_min_val[gene_idx]
+                    range_max = self.random_mutation_max_val[gene_idx]
+
+                if probs[gene_idx] <= self.mutation_probability:
+                    # Generating a random value.
+                    random_value = numpy.random.uniform(low=range_min, 
+                                                        high=range_max, 
+                                                        size=1)[0]
+                    # If the mutation_by_replacement attribute is True, then the random value replaces the current gene value.
+                    if self.mutation_by_replacement:
+                        if self.gene_type_single == True:
+                            random_value = self.gene_type[0](random_value)
+                        else:
+                            random_value = self.gene_type[gene_idx][0](random_value)
+                            if type(random_value) is numpy.ndarray:
+                                random_value = random_value[0]
+                    # If the mutation_by_replacement attribute is False, then the random value is added to the gene value.
+                    else:
+                        if self.gene_type_single == True:
+                            random_value = self.gene_type[0](offspring[offspring_idx, gene_idx] + random_value)
+                        else:
+                            random_value = self.gene_type[gene_idx][0](offspring[offspring_idx, gene_idx] + random_value)
+                            if type(random_value) is numpy.ndarray:
+                                random_value = random_value[0]
+
+                    # Round the gene
+                    if self.gene_type_single == True:
+                        if not self.gene_type[1] is None:
+                            random_value = numpy.round(random_value, self.gene_type[1])
+                    else:
+                        if not self.gene_type[gene_idx][1] is None:
+                            random_value = numpy.round(random_value, self.gene_type[gene_idx][1])
+
+                    offspring[offspring_idx, gene_idx] = random_value
+
+                    if self.allow_duplicate_genes == False:
+                        offspring[offspring_idx], _, _ = self.solve_duplicate_genes_randomly(solution=offspring[offspring_idx],
+                                                                                             min_val=range_min,
+                                                                                             max_val=range_max,
+                                                                                             mutation_by_replacement=self.mutation_by_replacement,
+                                                                                             gene_type=self.gene_type,
+                                                                                             num_trials=10)
+        return offspring
+
+    def swap_mutation(self, offspring):
+
+        """
+        Applies the swap mutation which interchanges the values of 2 randomly selected genes.
+        It accepts a single parameter:
+            -offspring: The offspring to mutate.
+        It returns an array of the mutated offspring.
+        """
+
+        for idx in range(offspring.shape[0]):
+            mutation_gene1 = numpy.random.randint(low=0, high=offspring.shape[1]/2, size=1)[0]
+            mutation_gene2 = mutation_gene1 + int(offspring.shape[1]/2)
+
+            temp = offspring[idx, mutation_gene1]
+            offspring[idx, mutation_gene1] = offspring[idx, mutation_gene2]
+            offspring[idx, mutation_gene2] = temp
+        return offspring
+
+    def inversion_mutation(self, offspring):
+
+        """
+        Applies the inversion mutation which selects a subset of genes and inverts them (in order).
+        It accepts a single parameter:
+            -offspring: The offspring to mutate.
+        It returns an array of the mutated offspring.
+        """
+
+        for idx in range(offspring.shape[0]):
+            mutation_gene1 = numpy.random.randint(low=0, high=numpy.ceil(offspring.shape[1]/2 + 1), size=1)[0]
+            mutation_gene2 = mutation_gene1 + int(offspring.shape[1]/2)
+
+            genes_to_scramble = numpy.flip(offspring[idx, mutation_gene1:mutation_gene2])
+            offspring[idx, mutation_gene1:mutation_gene2] = genes_to_scramble
+        return offspring
+
+    def scramble_mutation(self, offspring):
+
+        """
+        Applies the scramble mutation which selects a subset of genes and shuffles their order randomly.
+        It accepts a single parameter:
+            -offspring: The offspring to mutate.
+        It returns an array of the mutated offspring.
+        """
+
+        for idx in range(offspring.shape[0]):
+            mutation_gene1 = numpy.random.randint(low=0, high=numpy.ceil(offspring.shape[1]/2 + 1), size=1)[0]
+            mutation_gene2 = mutation_gene1 + int(offspring.shape[1]/2)
+            genes_range = numpy.arange(start=mutation_gene1, stop=mutation_gene2)
+            numpy.random.shuffle(genes_range)
+            
+            genes_to_scramble = numpy.flip(offspring[idx, genes_range])
+            offspring[idx, genes_range] = genes_to_scramble
+        return offspring
+
+    def adaptive_mutation_population_fitness(self, offspring):
+
+        """
+        A helper method to calculate the average fitness of the solutions before applying the adaptive mutation.
+        It accepts a single parameter:
+            -offspring: The offspring to mutate.
+        It returns the average fitness to be used in adaptive mutation.
+        """        
+
+        fitness = self.last_generation_fitness.copy()
+        temp_population = numpy.zeros_like(self.population)
+
+        if (self.keep_elitism == 0):
+            if (self.keep_parents == 0):
+                parents_to_keep = []
+            elif (self.keep_parents == -1):
+                parents_to_keep = self.last_generation_parents.copy()
+                temp_population[0:len(parents_to_keep), :] = parents_to_keep
+            elif (self.keep_parents > 0):
+                parents_to_keep, _ = self.steady_state_selection(self.last_generation_fitness, num_parents=self.keep_parents)
+                temp_population[0:len(parents_to_keep), :] = parents_to_keep
+        else:
+            parents_to_keep, _ = self.steady_state_selection(self.last_generation_fitness, num_parents=self.keep_elitism)
+            temp_population[0:len(parents_to_keep), :] = parents_to_keep
+
+        temp_population[len(parents_to_keep):, :] = offspring
+
+        fitness[:self.last_generation_parents.shape[0]] = self.last_generation_fitness[self.last_generation_parents_indices]
+
+        first_idx = len(parents_to_keep)
+        last_idx = fitness.shape[0]
+        fitness[first_idx:last_idx] = [0]*(last_idx - first_idx)
+
+        if self.fitness_batch_size in [1, None]:
+            # Calculate the fitness for each individual solution.
+            for idx in range(first_idx, last_idx):
+                fitness[idx] = self.fitness_func(self, 
+                                                 temp_population[idx], 
+                                                 None)
+        else:
+            # Calculate the fitness for batch of solutions.
+
+            # Number of batches.
+            num_batches = int(numpy.ceil((last_idx - first_idx) / self.fitness_batch_size))
+
+            for batch_idx in range(num_batches):
+                # The index of the first solution in the current batch.
+                batch_first_index = first_idx + batch_idx * self.fitness_batch_size
+                # The index of the last solution in the current batch.
+                if batch_idx == (num_batches - 1):
+                    batch_last_index = last_idx
+                else:
+                    batch_last_index = first_idx + (batch_idx + 1) * self.fitness_batch_size
+
+                # Calculate the fitness values for the batch.
+                fitness_temp = self.fitness_func(self, 
+                                                 temp_population[batch_first_index:batch_last_index], 
+                                                 None) 
+                # Insert the fitness of each solution at the proper index.
+                for idx in range(batch_first_index, batch_last_index):
+                    fitness[idx] = fitness_temp[idx - batch_first_index]
+
+        average_fitness = numpy.mean(fitness)
+
+        return average_fitness, fitness[len(parents_to_keep):]
+
+    def adaptive_mutation(self, offspring):
+
+        """
+        Applies the adaptive mutation which changes the values of a number of genes randomly. In adaptive mutation, the number of genes to mutate differs based on the fitness value of the solution.
+        The random value is selected either using the 'gene_space' parameter or the 2 parameters 'random_mutation_min_val' and 'random_mutation_max_val'.
+        It accepts a single parameter:
+            -offspring: The offspring to mutate.
+        It returns an array of the mutated offspring.
+        """
+
+        # If the attribute 'gene_space' exists (i.e. not None), then the mutation values are selected from the 'gene_space' parameter according to the space of values of each gene. Otherwise, it is selected randomly based on the 2 parameters 'random_mutation_min_val' and 'random_mutation_max_val'.
+        # When the 'mutation_probability' parameter exists (i.e. not None), then it is used in the mutation. Otherwise, the 'mutation_num_genes' parameter is used.
+
+        if self.mutation_probability is None:
+            # When the 'mutation_probability' parameter does not exist (i.e. None), then the parameter 'mutation_num_genes' is used in the mutation.
+            if not (self.gene_space is None):
+                # When the attribute 'gene_space' exists (i.e. not None), the mutation values are selected randomly from the space of values of each gene.
+                offspring = self.adaptive_mutation_by_space(offspring)
+            else:
+                # When the attribute 'gene_space' does not exist (i.e. None), the mutation values are selected randomly based on the continuous range specified by the 2 attributes 'random_mutation_min_val' and 'random_mutation_max_val'.
+                offspring = self.adaptive_mutation_randomly(offspring)
+        else:
+            # When the 'mutation_probability' parameter exists (i.e. not None), then it is used in the mutation.
+            if not (self.gene_space is None):
+                # When the attribute 'gene_space' exists (i.e. not None), the mutation values are selected randomly from the space of values of each gene.
+                offspring = self.adaptive_mutation_probs_by_space(offspring)
+            else:
+                # When the attribute 'gene_space' does not exist (i.e. None), the mutation values are selected randomly based on the continuous range specified by the 2 attributes 'random_mutation_min_val' and 'random_mutation_max_val'.
+                offspring = self.adaptive_mutation_probs_randomly(offspring)
+
+        return offspring
+
+    def adaptive_mutation_by_space(self, offspring):
+
+        """
+        Applies the adaptive mutation based on the 2 parameters 'mutation_num_genes' and 'gene_space'. 
+        A number of genes equal are selected randomly for mutation. This number depends on the fitness of the solution.
+        The random values are selected from the 'gene_space' parameter.
+        It accepts a single parameter:
+            -offspring: The offspring to mutate.
+        It returns an array of the mutated offspring.
+        """
+        
+        # For each offspring, a value from the gene space is selected randomly and assigned to the selected gene for mutation.
+
+        average_fitness, offspring_fitness = self.adaptive_mutation_population_fitness(offspring)
+
+        # Adaptive mutation changes one or more genes in each offspring randomly.
+        # The number of genes to mutate depends on the solution's fitness value.
+        for offspring_idx in range(offspring.shape[0]):
+            if offspring_fitness[offspring_idx] < average_fitness:
+                adaptive_mutation_num_genes = self.mutation_num_genes[0]
+            else:
+                adaptive_mutation_num_genes = self.mutation_num_genes[1]
+            mutation_indices = numpy.array(random.sample(range(0, self.num_genes), adaptive_mutation_num_genes))
+            for gene_idx in mutation_indices:
+
+                if type(self.random_mutation_min_val) in self.supported_int_float_types:
+                    range_min = self.random_mutation_min_val
+                    range_max = self.random_mutation_max_val
+                else:
+                    range_min = self.random_mutation_min_val[gene_idx]
+                    range_max = self.random_mutation_max_val[gene_idx]
+
+                if self.gene_space_nested:
+                    # Returning the current gene space from the 'gene_space' attribute.
+                    if type(self.gene_space[gene_idx]) in [numpy.ndarray, list]:
+                        curr_gene_space = self.gene_space[gene_idx].copy()
+                    else:
+                        curr_gene_space = self.gene_space[gene_idx]
+
+                    # If the gene space has only a single value, use it as the new gene value.
+                    if type(curr_gene_space) in pygad.GA.supported_int_float_types:
+                        value_from_space = curr_gene_space
+                    # If the gene space is None, apply mutation by adding a random value between the range defined by the 2 parameters 'random_mutation_min_val' and 'random_mutation_max_val'.
+                    elif curr_gene_space is None:
+                        rand_val = numpy.random.uniform(low=range_min,
+                                                        high=range_max,
+                                                        size=1)[0]
+                        if self.mutation_by_replacement:
+                            value_from_space = rand_val
+                        else:
+                            value_from_space = offspring[offspring_idx, gene_idx] + rand_val
+                    elif type(curr_gene_space) is dict:
+                            # Selecting a value randomly from the current gene's space in the 'gene_space' attribute.
+                            if 'step' in curr_gene_space.keys():
+                                # The numpy.random.choice() and numpy.random.uniform() functions return a NumPy array as the output even if the array has a single value.
+                                # We have to return the output at index 0 to force a numeric value to be returned not an object of type numpy.ndarray. 
+                                # If numpy.ndarray is returned, then it will cause an issue later while using the set() function.
+                                value_from_space = numpy.random.choice(numpy.arange(start=curr_gene_space['low'],
+                                                                                    stop=curr_gene_space['high'],
+                                                                                    step=curr_gene_space['step']),
+                                                                       size=1)[0]
+                            else:
+                                value_from_space = numpy.random.uniform(low=curr_gene_space['low'],
+                                                                        high=curr_gene_space['high'],
+                                                                        size=1)[0]
+                    else:
+                        # Selecting a value randomly from the current gene's space in the 'gene_space' attribute.
+                        # If the gene space has only 1 value, then select it. The old and new values of the gene are identical.
+                        if len(curr_gene_space) == 1:
+                            value_from_space = curr_gene_space[0]
+                        # If the gene space has more than 1 value, then select a new one that is different from the current value.
+                        else:
+                            values_to_select_from = list(set(curr_gene_space) - set([offspring[offspring_idx, gene_idx]]))
+
+                            if len(values_to_select_from) == 0:
+                                value_from_space = offspring[offspring_idx, gene_idx]
+                            else:
+                                value_from_space = random.choice(values_to_select_from)
+                else:
+                    # Selecting a value randomly from the global gene space in the 'gene_space' attribute.
+                    if type(self.gene_space) is dict:
+                        if 'step' in self.gene_space.keys():
+                            value_from_space = numpy.random.choice(numpy.arange(start=self.gene_space['low'],
+                                                                                stop=self.gene_space['high'],
+                                                                                step=self.gene_space['step']),
+                                                                   size=1)[0]
+                        else:
+                            value_from_space = numpy.random.uniform(low=self.gene_space['low'],
+                                                                    high=self.gene_space['high'],
+                                                                    size=1)[0]
+                    else:
+                        values_to_select_from = list(set(self.gene_space) - set([offspring[offspring_idx, gene_idx]]))
+
+                        if len(values_to_select_from) == 0:
+                            value_from_space = offspring[offspring_idx, gene_idx]
+                        else:
+                            value_from_space = random.choice(values_to_select_from)
+
+
+                if value_from_space is None:
+                    value_from_space = numpy.random.uniform(low=range_min, 
+                                                            high=range_max, 
+                                                            size=1)[0]
+
+                # Assinging the selected value from the space to the gene.
+                if self.gene_type_single == True:
+                    if not self.gene_type[1] is None:
+                        offspring[offspring_idx, gene_idx] = numpy.round(self.gene_type[0](value_from_space),
+                                                                         self.gene_type[1])
+                    else:
+                        offspring[offspring_idx, gene_idx] = self.gene_type[0](value_from_space)
+                else:
+                    if not self.gene_type[gene_idx][1] is None:
+                        offspring[offspring_idx, gene_idx] = numpy.round(self.gene_type[gene_idx][0](value_from_space),
+                                                                         self.gene_type[gene_idx][1])
+                    else:
+                        offspring[offspring_idx, gene_idx] = self.gene_type[gene_idx][0](value_from_space)
+
+                if self.allow_duplicate_genes == False:
+                    offspring[offspring_idx], _, _ = self.solve_duplicate_genes_by_space(solution=offspring[offspring_idx],
+                                                                                         gene_type=self.gene_type,
+                                                                                         num_trials=10)
+        return offspring
+        
+    def adaptive_mutation_randomly(self, offspring):
+
+        """
+        Applies the adaptive mutation based on the 'mutation_num_genes' parameter. 
+        A number of genes equal are selected randomly for mutation. This number depends on the fitness of the solution.
+        The random values are selected based on the 2 parameters 'random_mutation_min_val' and 'random_mutation_max_val'.
+        It accepts a single parameter:
+            -offspring: The offspring to mutate.
+        It returns an array of the mutated offspring.
+        """
+
+        average_fitness, offspring_fitness = self.adaptive_mutation_population_fitness(offspring)
+
+        # Adaptive random mutation changes one or more genes in each offspring randomly.
+        # The number of genes to mutate depends on the solution's fitness value.
+        for offspring_idx in range(offspring.shape[0]):
+            if offspring_fitness[offspring_idx] < average_fitness:
+                adaptive_mutation_num_genes = self.mutation_num_genes[0]
+            else:
+                adaptive_mutation_num_genes = self.mutation_num_genes[1]
+            mutation_indices = numpy.array(random.sample(range(0, self.num_genes), adaptive_mutation_num_genes))
+            for gene_idx in mutation_indices:
+
+                if type(self.random_mutation_min_val) in self.supported_int_float_types:
+                    range_min = self.random_mutation_min_val
+                    range_max = self.random_mutation_max_val
+                else:
+                    range_min = self.random_mutation_min_val[gene_idx]
+                    range_max = self.random_mutation_max_val[gene_idx]
+
+                # Generating a random value.
+                random_value = numpy.random.uniform(low=range_min, 
+                                                    high=range_max, 
+                                                    size=1)[0]
+                # If the mutation_by_replacement attribute is True, then the random value replaces the current gene value.
+                if self.mutation_by_replacement:
+                    if self.gene_type_single == True:
+                        random_value = self.gene_type[0](random_value)
+                    else:
+                        random_value = self.gene_type[gene_idx][0](random_value)
+                        if type(random_value) is numpy.ndarray:
+                            random_value = random_value[0]
+                # If the mutation_by_replacement attribute is False, then the random value is added to the gene value.
+                else:
+                    if self.gene_type_single == True:
+                        random_value = self.gene_type[0](offspring[offspring_idx, gene_idx] + random_value)
+                    else:
+                        random_value = self.gene_type[gene_idx][0](offspring[offspring_idx, gene_idx] + random_value)
+                        if type(random_value) is numpy.ndarray:
+                            random_value = random_value[0]
+
+                if self.gene_type_single == True:
+                    if not self.gene_type[1] is None:
+                        random_value = numpy.round(random_value, self.gene_type[1])
+                else:
+                    if not self.gene_type[gene_idx][1] is None:
+                        random_value = numpy.round(random_value, self.gene_type[gene_idx][1])
+
+                offspring[offspring_idx, gene_idx] = random_value
+
+                if self.allow_duplicate_genes == False:
+                    offspring[offspring_idx], _, _ = self.solve_duplicate_genes_randomly(solution=offspring[offspring_idx],
+                                                                                         min_val=range_min,
+                                                                                         max_val=range_max,
+                                                                                         mutation_by_replacement=self.mutation_by_replacement,
+                                                                                         gene_type=self.gene_type,
+                                                                                         num_trials=10)
+        return offspring
+
+    def adaptive_mutation_probs_by_space(self, offspring):
+
+        """
+        Applies the adaptive mutation based on the 2 parameters 'mutation_probability' and 'gene_space'.
+        Based on whether the solution fitness is above or below a threshold, the mutation is applied diffrently by mutating high or low number of genes.
+        The random values are selected based on space of values for each gene.
+        It accepts a single parameter:
+            -offspring: The offspring to mutate.
+        It returns an array of the mutated offspring.
+        """
+
+        # For each offspring, a value from the gene space is selected randomly and assigned to the selected gene for mutation.
+
+        average_fitness, offspring_fitness = self.adaptive_mutation_population_fitness(offspring)
+
+        # Adaptive random mutation changes one or more genes in each offspring randomly.
+        # The probability of mutating a gene depends on the solution's fitness value.
+        for offspring_idx in range(offspring.shape[0]):
+            if offspring_fitness[offspring_idx] < average_fitness:
+                adaptive_mutation_probability = self.mutation_probability[0]
+            else:
+                adaptive_mutation_probability = self.mutation_probability[1]
+
+            probs = numpy.random.random(size=offspring.shape[1])
+            for gene_idx in range(offspring.shape[1]):
+
+                if type(self.random_mutation_min_val) in self.supported_int_float_types:
+                    range_min = self.random_mutation_min_val
+                    range_max = self.random_mutation_max_val
+                else:
+                    range_min = self.random_mutation_min_val[gene_idx]
+                    range_max = self.random_mutation_max_val[gene_idx]
+
+                if probs[gene_idx] <= adaptive_mutation_probability:
+                    if self.gene_space_nested:
+                        # Returning the current gene space from the 'gene_space' attribute.
+                        if type(self.gene_space[gene_idx]) in [numpy.ndarray, list]:
+                            curr_gene_space = self.gene_space[gene_idx].copy()
+                        else:
+                            curr_gene_space = self.gene_space[gene_idx]
+        
+                        # If the gene space has only a single value, use it as the new gene value.
+                        if type(curr_gene_space) in pygad.GA.supported_int_float_types:
+                            value_from_space = curr_gene_space
+                        # If the gene space is None, apply mutation by adding a random value between the range defined by the 2 parameters 'random_mutation_min_val' and 'random_mutation_max_val'.
+                        elif curr_gene_space is None:
+                            rand_val = numpy.random.uniform(low=range_min,
+                                                            high=range_max,
+                                                            size=1)[0]
+                            if self.mutation_by_replacement:
+                                value_from_space = rand_val
+                            else:
+                                value_from_space = offspring[offspring_idx, gene_idx] + rand_val
+                        elif type(curr_gene_space) is dict:
+                            # Selecting a value randomly from the current gene's space in the 'gene_space' attribute.
+                            if 'step' in curr_gene_space.keys():
+                                value_from_space = numpy.random.choice(numpy.arange(start=curr_gene_space['low'],
+                                                                                    stop=curr_gene_space['high'],
+                                                                                    step=curr_gene_space['step']),
+                                                                       size=1)[0]
+                            else:
+                                value_from_space = numpy.random.uniform(low=curr_gene_space['low'],
+                                                                        high=curr_gene_space['high'],
+                                                                        size=1)[0]
+                        else:
+                            # Selecting a value randomly from the current gene's space in the 'gene_space' attribute.
+                            # If the gene space has only 1 value, then select it. The old and new values of the gene are identical.
+                            if len(curr_gene_space) == 1:
+                                value_from_space = curr_gene_space[0]
+                            # If the gene space has more than 1 value, then select a new one that is different from the current value.
+                            else:
+                                values_to_select_from = list(set(curr_gene_space) - set([offspring[offspring_idx, gene_idx]]))
+
+                                if len(values_to_select_from) == 0:
+                                    value_from_space = offspring[offspring_idx, gene_idx]
+                                else:
+                                    value_from_space = random.choice(values_to_select_from)
+                    else:
+                        # Selecting a value randomly from the global gene space in the 'gene_space' attribute.
+                        if type(self.gene_space) is dict:
+                            if 'step' in self.gene_space.keys():
+                                # The numpy.random.choice() and numpy.random.uniform() functions return a NumPy array as the output even if the array has a single value.
+                                # We have to return the output at index 0 to force a numeric value to be returned not an object of type numpy.ndarray. 
+                                # If numpy.ndarray is returned, then it will cause an issue later while using the set() function.
+                                value_from_space = numpy.random.choice(numpy.arange(start=self.gene_space['low'],
+                                                                                    stop=self.gene_space['high'],
+                                                                                    step=self.gene_space['step']),
+                                                                       size=1)[0]
+                            else:
+                                value_from_space = numpy.random.uniform(low=self.gene_space['low'],
+                                                                        high=self.gene_space['high'],
+                                                                        size=1)[0]
+                        else:
+                            values_to_select_from = list(set(self.gene_space) - set([offspring[offspring_idx, gene_idx]]))
+
+                            if len(values_to_select_from) == 0:
+                                value_from_space = offspring[offspring_idx, gene_idx]
+                            else:
+                                value_from_space = random.choice(values_to_select_from)
+
+                    if value_from_space is None:
+                        value_from_space = numpy.random.uniform(low=range_min, 
+                                                                high=range_max, 
+                                                                size=1)[0]
+
+                    # Assinging the selected value from the space to the gene.
+                    if self.gene_type_single == True:
+                        if not self.gene_type[1] is None:
+                            offspring[offspring_idx, gene_idx] = numpy.round(self.gene_type[0](value_from_space),
+                                                                             self.gene_type[1])
+                        else:
+                            offspring[offspring_idx, gene_idx] = self.gene_type[0](value_from_space)
+                    else:
+                        if not self.gene_type[gene_idx][1] is None:
+                            offspring[offspring_idx, gene_idx] = numpy.round(self.gene_type[gene_idx][0](value_from_space),
+                                                                             self.gene_type[gene_idx][1])
+                        else:
+                            offspring[offspring_idx, gene_idx] = self.gene_type[gene_idx][0](value_from_space)
+
+                    if self.allow_duplicate_genes == False:
+                        offspring[offspring_idx], _, _ = self.solve_duplicate_genes_by_space(solution=offspring[offspring_idx],
+                                                                                             gene_type=self.gene_type,
+                                                                                             num_trials=10)
+        return offspring
+
+    def adaptive_mutation_probs_randomly(self, offspring):
+
+        """
+        Applies the adaptive mutation based on the 'mutation_probability' parameter. 
+        Based on whether the solution fitness is above or below a threshold, the mutation is applied diffrently by mutating high or low number of genes.
+        The random values are selected based on the 2 parameters 'random_mutation_min_val' and 'random_mutation_max_val'.
+        It accepts a single parameter:
+            -offspring: The offspring to mutate.
+        It returns an array of the mutated offspring.
+        """
+
+        average_fitness, offspring_fitness = self.adaptive_mutation_population_fitness(offspring)
+
+        # Adaptive random mutation changes one or more genes in each offspring randomly.
+        # The probability of mutating a gene depends on the solution's fitness value.
+        for offspring_idx in range(offspring.shape[0]):
+            if offspring_fitness[offspring_idx] < average_fitness:
+                adaptive_mutation_probability = self.mutation_probability[0]
+            else:
+                adaptive_mutation_probability = self.mutation_probability[1]
+
+            probs = numpy.random.random(size=offspring.shape[1])
+            for gene_idx in range(offspring.shape[1]):
+
+                if type(self.random_mutation_min_val) in self.supported_int_float_types:
+                    range_min = self.random_mutation_min_val
+                    range_max = self.random_mutation_max_val
+                else:
+                    range_min = self.random_mutation_min_val[gene_idx]
+                    range_max = self.random_mutation_max_val[gene_idx]
+
+                if probs[gene_idx] <= adaptive_mutation_probability:
+                    # Generating a random value.
+                    random_value = numpy.random.uniform(low=range_min, 
+                                                        high=range_max, 
+                                                        size=1)[0]
+                    # If the mutation_by_replacement attribute is True, then the random value replaces the current gene value.
+                    if self.mutation_by_replacement:
+                        if self.gene_type_single == True:
+                            random_value = self.gene_type[0](random_value)
+                        else:
+                            random_value = self.gene_type[gene_idx][0](random_value)
+                            if type(random_value) is numpy.ndarray:
+                                random_value = random_value[0]
+                    # If the mutation_by_replacement attribute is False, then the random value is added to the gene value.
+                    else:
+                        if self.gene_type_single == True:
+                            random_value = self.gene_type[0](offspring[offspring_idx, gene_idx] + random_value)
+                        else:
+                            random_value = self.gene_type[gene_idx][0](offspring[offspring_idx, gene_idx] + random_value)
+                            if type(random_value) is numpy.ndarray:
+                                random_value = random_value[0]
+
+                    if self.gene_type_single == True:
+                        if not self.gene_type[1] is None:
+                            random_value = numpy.round(random_value, self.gene_type[1])
+                    else:
+                        if not self.gene_type[gene_idx][1] is None:
+                            random_value = numpy.round(random_value, self.gene_type[gene_idx][1])
+
+                    offspring[offspring_idx, gene_idx] = random_value
+
+                    if self.allow_duplicate_genes == False:
+                        offspring[offspring_idx], _, _ = self.solve_duplicate_genes_randomly(solution=offspring[offspring_idx],
+                                                                                             min_val=range_min,
+                                                                                             max_val=range_max,
+                                                                                             mutation_by_replacement=self.mutation_by_replacement,
+                                                                                             gene_type=self.gene_type,
+                                                                                             num_trials=10)
+        return offspring
```

### Comparing `pygad-3.0.1/pygad/utils/parent_selection.py` & `pygad-3.1.0/pygad/utils/parent_selection.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,191 +1,231 @@
-"""
-The pygad.utils.parent_selection module has all the built-in parent selection operators.
-"""
-
-import numpy
-
-class ParentSelection:
-    def steady_state_selection(self, fitness, num_parents):
-    
-            """
-            Selects the parents using the steady-state selection technique. Later, these parents will mate to produce the offspring.
-            It accepts 2 parameters:
-                -fitness: The fitness values of the solutions in the current population.
-                -num_parents: The number of parents to be selected.
-            It returns an array of the selected parents.
-            """
-    
-            fitness_sorted = sorted(range(len(fitness)), key=lambda k: fitness[k])
-            fitness_sorted.reverse()
-            # Selecting the best individuals in the current generation as parents for producing the offspring of the next generation.
-            if self.gene_type_single == True:
-                parents = numpy.empty((num_parents, self.population.shape[1]), dtype=self.gene_type[0])
-            else:
-                parents = numpy.empty((num_parents, self.population.shape[1]), dtype=object)
-            for parent_num in range(num_parents):
-                parents[parent_num, :] = self.population[fitness_sorted[parent_num], :].copy()
-    
-            return parents, numpy.array(fitness_sorted[:num_parents])
-    
-    def rank_selection(self, fitness, num_parents):
-    
-            """
-            Selects the parents using the rank selection technique. Later, these parents will mate to produce the offspring.
-            It accepts 2 parameters:
-                -fitness: The fitness values of the solutions in the current population.
-                -num_parents: The number of parents to be selected.
-            It returns an array of the selected parents.
-            """
-    
-            fitness_sorted = sorted(range(len(fitness)), key=lambda k: fitness[k])
-            fitness_sorted.reverse()
-            # Selecting the best individuals in the current generation as parents for producing the offspring of the next generation.
-            if self.gene_type_single == True:
-                parents = numpy.empty((num_parents, self.population.shape[1]), dtype=self.gene_type[0])
-            else:
-                parents = numpy.empty((num_parents, self.population.shape[1]), dtype=object)
-            for parent_num in range(num_parents):
-                parents[parent_num, :] = self.population[fitness_sorted[parent_num], :].copy()
-    
-            return parents, numpy.array(fitness_sorted[:num_parents])
-    
-    def random_selection(self, fitness, num_parents):
-    
-            """
-            Selects the parents randomly. Later, these parents will mate to produce the offspring.
-            It accepts 2 parameters:
-                -fitness: The fitness values of the solutions in the current population.
-                -num_parents: The number of parents to be selected.
-            It returns an array of the selected parents.
-            """
-    
-            if self.gene_type_single == True:
-                parents = numpy.empty((num_parents, self.population.shape[1]), dtype=self.gene_type[0])
-            else:
-                parents = numpy.empty((num_parents, self.population.shape[1]), dtype=object)
-    
-            rand_indices = numpy.random.randint(low=0.0, high=fitness.shape[0], size=num_parents)
-    
-            for parent_num in range(num_parents):
-                parents[parent_num, :] = self.population[rand_indices[parent_num], :].copy()
-    
-            return parents, rand_indices
-    
-    def tournament_selection(self, fitness, num_parents):
-    
-            """
-            Selects the parents using the tournament selection technique. Later, these parents will mate to produce the offspring.
-            It accepts 2 parameters:
-                -fitness: The fitness values of the solutions in the current population.
-                -num_parents: The number of parents to be selected.
-            It returns an array of the selected parents.
-            """
-    
-            if self.gene_type_single == True:
-                parents = numpy.empty((num_parents, self.population.shape[1]), dtype=self.gene_type[0])
-            else:
-                parents = numpy.empty((num_parents, self.population.shape[1]), dtype=object)
-    
-            parents_indices = []
-    
-            for parent_num in range(num_parents):
-                rand_indices = numpy.random.randint(low=0.0, high=len(fitness), size=self.K_tournament)
-                K_fitnesses = fitness[rand_indices]
-                selected_parent_idx = numpy.where(K_fitnesses == numpy.max(K_fitnesses))[0][0]
-                parents_indices.append(rand_indices[selected_parent_idx])
-                parents[parent_num, :] = self.population[rand_indices[selected_parent_idx], :].copy()
-    
-            return parents, numpy.array(parents_indices)
-    
-    def roulette_wheel_selection(self, fitness, num_parents):
-    
-            """
-            Selects the parents using the roulette wheel selection technique. Later, these parents will mate to produce the offspring.
-            It accepts 2 parameters:
-                -fitness: The fitness values of the solutions in the current population.
-                -num_parents: The number of parents to be selected.
-            It returns an array of the selected parents.
-            """
-    
-            fitness_sum = numpy.sum(fitness)
-            if fitness_sum == 0:
-                self.logger.error("Cannot proceed because the sum of fitness values is zero. Cannot divide by zero.")
-                raise ZeroDivisionError("Cannot proceed because the sum of fitness values is zero. Cannot divide by zero.")
-            probs = fitness / fitness_sum
-            probs_start = numpy.zeros(probs.shape, dtype=float) # An array holding the start values of the ranges of probabilities.
-            probs_end = numpy.zeros(probs.shape, dtype=float) # An array holding the end values of the ranges of probabilities.
-    
-            curr = 0.0
-    
-            # Calculating the probabilities of the solutions to form a roulette wheel.
-            for _ in range(probs.shape[0]):
-                min_probs_idx = numpy.where(probs == numpy.min(probs))[0][0]
-                probs_start[min_probs_idx] = curr
-                curr = curr + probs[min_probs_idx]
-                probs_end[min_probs_idx] = curr
-                probs[min_probs_idx] = 99999999999
-    
-            # Selecting the best individuals in the current generation as parents for producing the offspring of the next generation.
-            if self.gene_type_single == True:
-                parents = numpy.empty((num_parents, self.population.shape[1]), dtype=self.gene_type[0])
-            else:
-                parents = numpy.empty((num_parents, self.population.shape[1]), dtype=object)
-            
-            parents_indices = []
-    
-            for parent_num in range(num_parents):
-                rand_prob = numpy.random.rand()
-                for idx in range(probs.shape[0]):
-                    if (rand_prob >= probs_start[idx] and rand_prob < probs_end[idx]):
-                        parents[parent_num, :] = self.population[idx, :].copy()
-                        parents_indices.append(idx)
-                        break
-            return parents, numpy.array(parents_indices)
-    
-    def stochastic_universal_selection(self, fitness, num_parents):
-    
-            """
-            Selects the parents using the stochastic universal selection technique. Later, these parents will mate to produce the offspring.
-            It accepts 2 parameters:
-                -fitness: The fitness values of the solutions in the current population.
-                -num_parents: The number of parents to be selected.
-            It returns an array of the selected parents.
-            """
-    
-            fitness_sum = numpy.sum(fitness)
-            if fitness_sum == 0:
-                self.logger.error("Cannot proceed because the sum of fitness values is zero. Cannot divide by zero.")
-                raise ZeroDivisionError("Cannot proceed because the sum of fitness values is zero. Cannot divide by zero.")
-            probs = fitness / fitness_sum
-            probs_start = numpy.zeros(probs.shape, dtype=float) # An array holding the start values of the ranges of probabilities.
-            probs_end = numpy.zeros(probs.shape, dtype=float) # An array holding the end values of the ranges of probabilities.
-    
-            curr = 0.0
-    
-            # Calculating the probabilities of the solutions to form a roulette wheel.
-            for _ in range(probs.shape[0]):
-                min_probs_idx = numpy.where(probs == numpy.min(probs))[0][0]
-                probs_start[min_probs_idx] = curr
-                curr = curr + probs[min_probs_idx]
-                probs_end[min_probs_idx] = curr
-                probs[min_probs_idx] = 99999999999
-    
-            pointers_distance = 1.0 / self.num_parents_mating # Distance between different pointers.
-            first_pointer = numpy.random.uniform(low=0.0, high=pointers_distance, size=1) # Location of the first pointer.
-    
-            # Selecting the best individuals in the current generation as parents for producing the offspring of the next generation.
-            if self.gene_type_single == True:
-                parents = numpy.empty((num_parents, self.population.shape[1]), dtype=self.gene_type[0])
-            else:
-                parents = numpy.empty((num_parents, self.population.shape[1]), dtype=object)
-            
-            parents_indices = []
-    
-            for parent_num in range(num_parents):
-                rand_pointer = first_pointer + parent_num*pointers_distance
-                for idx in range(probs.shape[0]):
-                    if (rand_pointer >= probs_start[idx] and rand_pointer < probs_end[idx]):
-                        parents[parent_num, :] = self.population[idx, :].copy()
-                        parents_indices.append(idx)
-                        break
-            return parents, numpy.array(parents_indices)
+"""
+The pygad.utils.parent_selection module has all the built-in parent selection operators.
+"""
+
+import numpy
+
+class ParentSelection:
+    def steady_state_selection(self, fitness, num_parents):
+    
+        """
+        Selects the parents using the steady-state selection technique. Later, these parents will mate to produce the offspring.
+        It accepts 2 parameters:
+            -fitness: The fitness values of the solutions in the current population.
+            -num_parents: The number of parents to be selected.
+        It returns an array of the selected parents.
+        """
+
+        fitness_sorted = sorted(range(len(fitness)), key=lambda k: fitness[k])
+        fitness_sorted.reverse()
+
+        # Selecting the best individuals in the current generation as parents for producing the offspring of the next generation.
+        if self.gene_type_single == True:
+            parents = numpy.empty((num_parents, self.population.shape[1]), dtype=self.gene_type[0])
+        else:
+            parents = numpy.empty((num_parents, self.population.shape[1]), dtype=object)
+
+        for parent_num in range(num_parents):
+            parents[parent_num, :] = self.population[fitness_sorted[parent_num], :].copy()
+
+        return parents, numpy.array(fitness_sorted[:num_parents])
+
+    def rank_selection(self, fitness, num_parents):
+
+        """
+        Selects the parents using the rank selection technique. Later, these parents will mate to produce the offspring.
+        Rank selection gives a rank from 1 to N (number of solutions) to each solution based on its fitness.
+        It accepts 2 parameters:
+            -fitness: The fitness values of the solutions in the current population.
+            -num_parents: The number of parents to be selected.
+        It returns an array of the selected parents.
+        """
+
+        # This has the index of each solution in the population.
+        fitness_sorted = sorted(range(len(fitness)), key=lambda k: fitness[k])
+
+        # Rank the solutions based on their fitness. The worst is gives the rank 1. The best has the rank N.
+        rank = numpy.arange(1, self.sol_per_pop+1)
+
+        probs = rank / numpy.sum(rank)
+
+        probs_start, probs_end, parents = self.wheel_cumulative_probs(probs=probs.copy(), 
+                                                                      num_parents=num_parents)
+
+        parents_indices = []
+
+        for parent_num in range(num_parents):
+            rand_prob = numpy.random.rand()
+            for idx in range(probs.shape[0]):
+                if (rand_prob >= probs_start[idx] and rand_prob < probs_end[idx]):
+                    # The variable idx has the rank of solution but not its index in the population.
+                    # Return the correct index of the solution.
+                    mapped_idx = fitness_sorted[idx]
+                    parents[parent_num, :] = self.population[mapped_idx, :].copy()
+                    parents_indices.append(mapped_idx)
+                    break
+
+        return parents, numpy.array(parents_indices)
+
+    def random_selection(self, fitness, num_parents):
+    
+        """
+        Selects the parents randomly. Later, these parents will mate to produce the offspring.
+        It accepts 2 parameters:
+            -fitness: The fitness values of the solutions in the current population.
+            -num_parents: The number of parents to be selected.
+        It returns an array of the selected parents.
+        """
+
+        if self.gene_type_single == True:
+            parents = numpy.empty((num_parents, self.population.shape[1]), dtype=self.gene_type[0])
+        else:
+            parents = numpy.empty((num_parents, self.population.shape[1]), dtype=object)
+
+        rand_indices = numpy.random.randint(low=0.0, high=fitness.shape[0], size=num_parents)
+
+        for parent_num in range(num_parents):
+            parents[parent_num, :] = self.population[rand_indices[parent_num], :].copy()
+
+        return parents, rand_indices
+
+    def tournament_selection(self, fitness, num_parents):
+
+        """
+        Selects the parents using the tournament selection technique. Later, these parents will mate to produce the offspring.
+        It accepts 2 parameters:
+            -fitness: The fitness values of the solutions in the current population.
+            -num_parents: The number of parents to be selected.
+        It returns an array of the selected parents.
+        """
+    
+        if self.gene_type_single == True:
+            parents = numpy.empty((num_parents, self.population.shape[1]), dtype=self.gene_type[0])
+        else:
+            parents = numpy.empty((num_parents, self.population.shape[1]), dtype=object)
+    
+        parents_indices = []
+    
+        for parent_num in range(num_parents):
+            rand_indices = numpy.random.randint(low=0.0, high=len(fitness), size=self.K_tournament)
+            K_fitnesses = fitness[rand_indices]
+            selected_parent_idx = numpy.where(K_fitnesses == numpy.max(K_fitnesses))[0][0]
+            parents_indices.append(rand_indices[selected_parent_idx])
+            parents[parent_num, :] = self.population[rand_indices[selected_parent_idx], :].copy()
+    
+        return parents, numpy.array(parents_indices)
+    
+    def roulette_wheel_selection(self, fitness, num_parents):
+    
+        """
+        Selects the parents using the roulette wheel selection technique. Later, these parents will mate to produce the offspring.
+        It accepts 2 parameters:
+            -fitness: The fitness values of the solutions in the current population.
+            -num_parents: The number of parents to be selected.
+        It returns an array of the selected parents.
+        """
+    
+        fitness_sum = numpy.sum(fitness)
+        if fitness_sum == 0:
+            self.logger.error("Cannot proceed because the sum of fitness values is zero. Cannot divide by zero.")
+            raise ZeroDivisionError("Cannot proceed because the sum of fitness values is zero. Cannot divide by zero.")
+
+        probs = fitness / fitness_sum
+
+        probs_start, probs_end, parents = self.wheel_cumulative_probs(probs=probs.copy(), 
+                                                                      num_parents=num_parents)
+
+        parents_indices = []
+
+        for parent_num in range(num_parents):
+            rand_prob = numpy.random.rand()
+            for idx in range(probs.shape[0]):
+                if (rand_prob >= probs_start[idx] and rand_prob < probs_end[idx]):
+                    parents[parent_num, :] = self.population[idx, :].copy()
+                    parents_indices.append(idx)
+                    break
+
+        return parents, numpy.array(parents_indices)
+
+    def wheel_cumulative_probs(self, probs, num_parents):
+        """
+        A helper function to calculate the wheel probabilities for these 2 methods:
+            1) roulette_wheel_selection
+            2) rank_selection
+        It accepts a single 1D array representing the probabilities of selecting each solution.
+        It returns 2 1D arrays:
+            1) probs_start has the start of each range.
+            2) probs_start has the end of each range.
+        It also returns an empty array for the parents.
+        """
+
+        probs_start = numpy.zeros(probs.shape, dtype=float) # An array holding the start values of the ranges of probabilities.
+        probs_end = numpy.zeros(probs.shape, dtype=float) # An array holding the end values of the ranges of probabilities.
+
+        curr = 0.0
+
+        # Calculating the probabilities of the solutions to form a roulette wheel.
+        for _ in range(probs.shape[0]):
+            min_probs_idx = numpy.where(probs == numpy.min(probs))[0][0]
+            probs_start[min_probs_idx] = curr
+            curr = curr + probs[min_probs_idx]
+            probs_end[min_probs_idx] = curr
+            probs[min_probs_idx] = 99999999999
+
+        # Selecting the best individuals in the current generation as parents for producing the offspring of the next generation.
+        if self.gene_type_single == True:
+            parents = numpy.empty((num_parents, self.population.shape[1]), dtype=self.gene_type[0])
+        else:
+            parents = numpy.empty((num_parents, self.population.shape[1]), dtype=object)
+
+        return probs_start, probs_end, parents
+
+    def stochastic_universal_selection(self, fitness, num_parents):
+
+        """
+        Selects the parents using the stochastic universal selection technique. Later, these parents will mate to produce the offspring.
+        It accepts 2 parameters:
+            -fitness: The fitness values of the solutions in the current population.
+            -num_parents: The number of parents to be selected.
+        It returns an array of the selected parents.
+        """
+
+        fitness_sum = numpy.sum(fitness)
+        if fitness_sum == 0:
+            self.logger.error("Cannot proceed because the sum of fitness values is zero. Cannot divide by zero.")
+            raise ZeroDivisionError("Cannot proceed because the sum of fitness values is zero. Cannot divide by zero.")
+        probs = fitness / fitness_sum
+        probs_start = numpy.zeros(probs.shape, dtype=float) # An array holding the start values of the ranges of probabilities.
+        probs_end = numpy.zeros(probs.shape, dtype=float) # An array holding the end values of the ranges of probabilities.
+
+        curr = 0.0
+
+        # Calculating the probabilities of the solutions to form a roulette wheel.
+        for _ in range(probs.shape[0]):
+            min_probs_idx = numpy.where(probs == numpy.min(probs))[0][0]
+            probs_start[min_probs_idx] = curr
+            curr = curr + probs[min_probs_idx]
+            probs_end[min_probs_idx] = curr
+            probs[min_probs_idx] = 99999999999
+
+        pointers_distance = 1.0 / self.num_parents_mating # Distance between different pointers.
+        first_pointer = numpy.random.uniform(low=0.0, 
+                                             high=pointers_distance, 
+                                             size=1)[0] # Location of the first pointer.
+
+        # Selecting the best individuals in the current generation as parents for producing the offspring of the next generation.
+        if self.gene_type_single == True:
+            parents = numpy.empty((num_parents, self.population.shape[1]), dtype=self.gene_type[0])
+        else:
+            parents = numpy.empty((num_parents, self.population.shape[1]), dtype=object)
+
+        parents_indices = []
+
+        for parent_num in range(num_parents):
+            rand_pointer = first_pointer + parent_num*pointers_distance
+            for idx in range(probs.shape[0]):
+                if (rand_pointer >= probs_start[idx] and rand_pointer < probs_end[idx]):
+                    parents[parent_num, :] = self.population[idx, :].copy()
+                    parents_indices.append(idx)
+                    break
+
+        return parents, numpy.array(parents_indices)
```

### Comparing `pygad-3.0.1/pygad/visualize/plot.py` & `pygad-3.1.0/pygad/visualize/plot.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,348 +1,348 @@
-"""
-The pygad.visualize.plot module has methods to create plots.
-"""
-
-import numpy
-import warnings
-import matplotlib.pyplot
-
-class Plot:
-    def plot_result(self, 
-                    title="PyGAD - Generation vs. Fitness", 
-                    xlabel="Generation", 
-                    ylabel="Fitness", 
-                    linewidth=3, 
-                    font_size=14, 
-                    plot_type="plot",
-                    color="#3870FF",
-                    save_dir=None):
-
-        if not self.suppress_warnings: 
-            warnings.warn("Please use the plot_fitness() method instead of plot_result(). The plot_result() method will be removed in the future.")
-
-        return self.plot_fitness(title=title, 
-                                 xlabel=xlabel, 
-                                 ylabel=ylabel, 
-                                 linewidth=linewidth, 
-                                 font_size=font_size, 
-                                 plot_type=plot_type,
-                                 color=color,
-                                 save_dir=save_dir)
-
-    def plot_fitness(self, 
-                    title="PyGAD - Generation vs. Fitness", 
-                    xlabel="Generation", 
-                    ylabel="Fitness", 
-                    linewidth=3, 
-                    font_size=14, 
-                    plot_type="plot",
-                    color="#3870FF",
-                    save_dir=None):
-
-        """
-        Creates, shows, and returns a figure that summarizes how the fitness value evolved by generation. Can only be called after completing at least 1 generation. If no generation is completed, an exception is raised.
-
-        Accepts the following:
-            title: Figure title.
-            xlabel: Label on the X-axis.
-            ylabel: Label on the Y-axis.
-            linewidth: Line width of the plot. Defaults to 3.
-            font_size: Font size for the labels and title. Defaults to 14.
-            plot_type: Type of the plot which can be either "plot" (default), "scatter", or "bar".
-            color: Color of the plot which defaults to "#3870FF".
-            save_dir: Directory to save the figure.
-
-        Returns the figure.
-        """
-
-        if self.generations_completed < 1:
-            self.logger.error("The plot_fitness() (i.e. plot_result()) method can only be called after completing at least 1 generation but ({generations_completed}) is completed.".format(generations_completed=self.generations_completed))
-            raise RuntimeError("The plot_fitness() (i.e. plot_result()) method can only be called after completing at least 1 generation but ({generations_completed}) is completed.".format(generations_completed=self.generations_completed))
-
-        fig = matplotlib.pyplot.figure()
-        if plot_type == "plot":
-            matplotlib.pyplot.plot(self.best_solutions_fitness, linewidth=linewidth, color=color)
-        elif plot_type == "scatter":
-            matplotlib.pyplot.scatter(range(len(self.best_solutions_fitness)), self.best_solutions_fitness, linewidth=linewidth, color=color)
-        elif plot_type == "bar":
-            matplotlib.pyplot.bar(range(len(self.best_solutions_fitness)), self.best_solutions_fitness, linewidth=linewidth, color=color)
-        matplotlib.pyplot.title(title, fontsize=font_size)
-        matplotlib.pyplot.xlabel(xlabel, fontsize=font_size)
-        matplotlib.pyplot.ylabel(ylabel, fontsize=font_size)
-
-        if not save_dir is None:
-            matplotlib.pyplot.savefig(fname=save_dir, 
-                                      bbox_inches='tight')
-        matplotlib.pyplot.show()
-
-        return fig
-
-    def plot_new_solution_rate(self,
-                               title="PyGAD - Generation vs. New Solution Rate", 
-                               xlabel="Generation", 
-                               ylabel="New Solution Rate", 
-                               linewidth=3, 
-                               font_size=14, 
-                               plot_type="plot",
-                               color="#3870FF",
-                               save_dir=None):
-
-        """
-        Creates, shows, and returns a figure that summarizes the rate of exploring new solutions. This method works only when save_solutions=True in the constructor of the pygad.GA class.
-
-        Accepts the following:
-            title: Figure title.
-            xlabel: Label on the X-axis.
-            ylabel: Label on the Y-axis.
-            linewidth: Line width of the plot. Defaults to 3.
-            font_size: Font size for the labels and title. Defaults to 14.
-            plot_type: Type of the plot which can be either "plot" (default), "scatter", or "bar".
-            color: Color of the plot which defaults to "#3870FF".
-            save_dir: Directory to save the figure.
-
-        Returns the figure.
-        """
-
-        if self.generations_completed < 1:
-            self.logger.error("The plot_new_solution_rate() method can only be called after completing at least 1 generation but ({generations_completed}) is completed.".format(generations_completed=self.generations_completed))
-            raise RuntimeError("The plot_new_solution_rate() method can only be called after completing at least 1 generation but ({generations_completed}) is completed.".format(generations_completed=self.generations_completed))
-
-        if self.save_solutions == False:
-            self.logger.error("The plot_new_solution_rate() method works only when save_solutions=True in the constructor of the pygad.GA class.")
-            raise RuntimeError("The plot_new_solution_rate() method works only when save_solutions=True in the constructor of the pygad.GA class.")
-
-        unique_solutions = set()
-        num_unique_solutions_per_generation = []
-        for generation_idx in range(self.generations_completed):
-            
-            len_before = len(unique_solutions)
-
-            start = generation_idx * self.sol_per_pop
-            end = start + self.sol_per_pop
-        
-            for sol in self.solutions[start:end]:
-                unique_solutions.add(tuple(sol))
-        
-            len_after = len(unique_solutions)
-        
-            generation_num_unique_solutions = len_after - len_before
-            num_unique_solutions_per_generation.append(generation_num_unique_solutions)
-
-        fig = matplotlib.pyplot.figure()
-        if plot_type == "plot":
-            matplotlib.pyplot.plot(num_unique_solutions_per_generation, linewidth=linewidth, color=color)
-        elif plot_type == "scatter":
-            matplotlib.pyplot.scatter(range(self.generations_completed), num_unique_solutions_per_generation, linewidth=linewidth, color=color)
-        elif plot_type == "bar":
-            matplotlib.pyplot.bar(range(self.generations_completed), num_unique_solutions_per_generation, linewidth=linewidth, color=color)
-        matplotlib.pyplot.title(title, fontsize=font_size)
-        matplotlib.pyplot.xlabel(xlabel, fontsize=font_size)
-        matplotlib.pyplot.ylabel(ylabel, fontsize=font_size)
-
-        if not save_dir is None:
-            matplotlib.pyplot.savefig(fname=save_dir, 
-                                      bbox_inches='tight')
-        matplotlib.pyplot.show()
-
-        return fig
-
-    def plot_genes(self, 
-                   title="PyGAD - Gene", 
-                   xlabel="Gene", 
-                   ylabel="Value", 
-                   linewidth=3, 
-                   font_size=14,
-                   plot_type="plot",
-                   graph_type="plot",
-                   fill_color="#3870FF",
-                   color="black",
-                   solutions="all",
-                   save_dir=None):
-
-        """
-        Creates, shows, and returns a figure with number of subplots equal to the number of genes. Each subplot shows the gene value for each generation. 
-        This method works only when save_solutions=True in the constructor of the pygad.GA class. 
-        It also works only after completing at least 1 generation. If no generation is completed, an exception is raised.
-
-        Accepts the following:
-            title: Figure title.
-            xlabel: Label on the X-axis.
-            ylabel: Label on the Y-axis.
-            linewidth: Line width of the plot. Defaults to 3.
-            font_size: Font size for the labels and title. Defaults to 14.
-            plot_type: Type of the plot which can be either "plot" (default), "scatter", or "bar".
-            graph_type: Type of the graph which can be either "plot" (default), "boxplot", or "histogram".
-            fill_color: Fill color of the graph which defaults to "#3870FF". This has no effect if graph_type="plot".
-            color: Color of the plot which defaults to "black".
-            solutions: Defaults to "all" which means use all solutions. If "best" then only the best solutions are used.
-            save_dir: Directory to save the figure.
-
-        Returns the figure.
-        """
-
-        if self.generations_completed < 1:
-            self.logger.error("The plot_genes() method can only be called after completing at least 1 generation but ({generations_completed}) is completed.".format(generations_completed=self.generations_completed))
-            raise RuntimeError("The plot_genes() method can only be called after completing at least 1 generation but ({generations_completed}) is completed.".format(generations_completed=self.generations_completed))
-
-        if type(solutions) is str:
-            if solutions == 'all':
-                if self.save_solutions:
-                    solutions_to_plot = numpy.array(self.solutions)
-                else:
-                    self.logger.error("The plot_genes() method with solutions='all' can only be called if 'save_solutions=True' in the pygad.GA class constructor.")
-                    raise RuntimeError("The plot_genes() method with solutions='all' can only be called if 'save_solutions=True' in the pygad.GA class constructor.")
-            elif solutions == 'best':
-                if self.save_best_solutions:
-                    solutions_to_plot = self.best_solutions
-                else:
-                    self.logger.error("The plot_genes() method with solutions='best' can only be called if 'save_best_solutions=True' in the pygad.GA class constructor.")
-                    raise RuntimeError("The plot_genes() method with solutions='best' can only be called if 'save_best_solutions=True' in the pygad.GA class constructor.")
-            else:
-                self.logger.error("The solutions parameter can be either 'all' or 'best' but {solutions} found.".format(solutions=solutions))
-                raise RuntimeError("The solutions parameter can be either 'all' or 'best' but {solutions} found.".format(solutions=solutions))
-        else:
-            self.logger.error("The solutions parameter must be a string but {solutions_type} found.".format(solutions_type=type(solutions)))
-            raise RuntimeError("The solutions parameter must be a string but {solutions_type} found.".format(solutions_type=type(solutions)))
-
-        if graph_type == "plot":
-            # num_rows will be always be >= 1
-            # num_cols can only be 0 if num_genes=1
-            num_rows = int(numpy.ceil(self.num_genes/5.0))
-            num_cols = int(numpy.ceil(self.num_genes/num_rows))
-    
-            if num_cols == 0:
-                figsize = (10, 8)
-                # There is only a single gene
-                fig, ax = matplotlib.pyplot.subplots(num_rows, figsize=figsize)
-                if plot_type == "plot":
-                    ax.plot(solutions_to_plot[:, 0], linewidth=linewidth, color=fill_color)
-                elif plot_type == "scatter":
-                    ax.scatter(range(self.generations_completed + 1), solutions_to_plot[:, 0], linewidth=linewidth, color=fill_color)
-                elif plot_type == "bar":
-                    ax.bar(range(self.generations_completed + 1), solutions_to_plot[:, 0], linewidth=linewidth, color=fill_color)
-                ax.set_xlabel(0, fontsize=font_size)
-            else:
-                fig, axs = matplotlib.pyplot.subplots(num_rows, num_cols)
-    
-                if num_cols == 1 and num_rows == 1:
-                    fig.set_figwidth(5 * num_cols)
-                    fig.set_figheight(4)
-                    axs.plot(solutions_to_plot[:, 0], linewidth=linewidth, color=fill_color)
-                    axs.set_xlabel("Gene " + str(0), fontsize=font_size)
-                elif num_cols == 1 or num_rows == 1:
-                    fig.set_figwidth(5 * num_cols)
-                    fig.set_figheight(4)
-                    for gene_idx in range(len(axs)):
-                        if plot_type == "plot":
-                            axs[gene_idx].plot(solutions_to_plot[:, gene_idx], linewidth=linewidth, color=fill_color)
-                        elif plot_type == "scatter":
-                            axs[gene_idx].scatter(range(solutions_to_plot.shape[0]), solutions_to_plot[:, gene_idx], linewidth=linewidth, color=fill_color)
-                        elif plot_type == "bar":
-                            axs[gene_idx].bar(range(solutions_to_plot.shape[0]), solutions_to_plot[:, gene_idx], linewidth=linewidth, color=fill_color)
-                        axs[gene_idx].set_xlabel("Gene " + str(gene_idx), fontsize=font_size)
-                else:
-                    gene_idx = 0
-                    fig.set_figwidth(25)
-                    fig.set_figheight(4*num_rows)
-                    for row_idx in range(num_rows):
-                        for col_idx in range(num_cols):
-                            if gene_idx >= self.num_genes:
-                                # axs[row_idx, col_idx].remove()
-                                break
-                            if plot_type == "plot":
-                                axs[row_idx, col_idx].plot(solutions_to_plot[:, gene_idx], linewidth=linewidth, color=fill_color)
-                            elif plot_type == "scatter":
-                                axs[row_idx, col_idx].scatter(range(solutions_to_plot.shape[0]), solutions_to_plot[:, gene_idx], linewidth=linewidth, color=fill_color)
-                            elif plot_type == "bar":
-                                axs[row_idx, col_idx].bar(range(solutions_to_plot.shape[0]), solutions_to_plot[:, gene_idx], linewidth=linewidth, color=fill_color)
-                            axs[row_idx, col_idx].set_xlabel("Gene " + str(gene_idx), fontsize=font_size)
-                            gene_idx += 1
-    
-            fig.suptitle(title, fontsize=font_size, y=1.001)
-            matplotlib.pyplot.tight_layout()
-
-        elif graph_type == "boxplot":
-            fig = matplotlib.pyplot.figure(1, figsize=(0.7*self.num_genes, 6))
-
-            # Create an axes instance
-            ax = fig.add_subplot(111)
-            boxeplots = ax.boxplot(solutions_to_plot, 
-                                   labels=range(self.num_genes),
-                                   patch_artist=True)
-            # adding horizontal grid lines
-            ax.yaxis.grid(True)
-    
-            for box in boxeplots['boxes']:
-                # change outline color
-                box.set(color='black', linewidth=linewidth)
-                # change fill color https://color.adobe.com/create/color-wheel
-                box.set_facecolor(fill_color)
-
-            for whisker in boxeplots['whiskers']:
-                whisker.set(color=color, linewidth=linewidth)
-            for median in boxeplots['medians']:
-                median.set(color=color, linewidth=linewidth)
-            for cap in boxeplots['caps']:
-                cap.set(color=color, linewidth=linewidth)
-    
-            matplotlib.pyplot.title(title, fontsize=font_size)
-            matplotlib.pyplot.xlabel(xlabel, fontsize=font_size)
-            matplotlib.pyplot.ylabel(ylabel, fontsize=font_size)
-            matplotlib.pyplot.tight_layout()
-
-        elif graph_type == "histogram":
-            # num_rows will always be >= 1
-            # num_cols can only be 0 if num_genes=1
-            num_rows = int(numpy.ceil(self.num_genes/5.0))
-            num_cols = int(numpy.ceil(self.num_genes/num_rows))
-    
-            if num_cols == 0:
-                figsize = (10, 8)
-                # There is only a single gene
-                fig, ax = matplotlib.pyplot.subplots(num_rows, 
-                                                     figsize=figsize)
-                ax.hist(solutions_to_plot[:, 0], color=fill_color)
-                ax.set_xlabel(0, fontsize=font_size)
-            else:
-                fig, axs = matplotlib.pyplot.subplots(num_rows, num_cols)
-    
-                if num_cols == 1 and num_rows == 1:
-                    fig.set_figwidth(4 * num_cols)
-                    fig.set_figheight(3)
-                    axs.hist(solutions_to_plot[:, 0], 
-                             color=fill_color,
-                             rwidth=0.95)
-                    axs.set_xlabel("Gene " + str(0), fontsize=font_size)
-                elif num_cols == 1 or num_rows == 1:
-                    fig.set_figwidth(4 * num_cols)
-                    fig.set_figheight(3)
-                    for gene_idx in range(len(axs)):
-                        axs[gene_idx].hist(solutions_to_plot[:, gene_idx], 
-                                           color=fill_color,
-                                           rwidth=0.95)
-                        axs[gene_idx].set_xlabel("Gene " + str(gene_idx), fontsize=font_size)
-                else:
-                    gene_idx = 0
-                    fig.set_figwidth(20)
-                    fig.set_figheight(3*num_rows)
-                    for row_idx in range(num_rows):
-                        for col_idx in range(num_cols):
-                            if gene_idx >= self.num_genes:
-                                # axs[row_idx, col_idx].remove()
-                                break
-                            axs[row_idx, col_idx].hist(solutions_to_plot[:, gene_idx], 
-                                                       color=fill_color,
-                                                       rwidth=0.95)
-                            axs[row_idx, col_idx].set_xlabel("Gene " + str(gene_idx), fontsize=font_size)
-                            gene_idx += 1
-    
-            fig.suptitle(title, fontsize=font_size, y=1.001)
-            matplotlib.pyplot.tight_layout()
-
-        if not save_dir is None:
-            matplotlib.pyplot.savefig(fname=save_dir, 
-                                      bbox_inches='tight')
-
-        matplotlib.pyplot.show()
-
-        return fig
+"""
+The pygad.visualize.plot module has methods to create plots.
+"""
+
+import numpy
+import warnings
+import matplotlib.pyplot
+
+class Plot:
+    def plot_result(self, 
+                    title="PyGAD - Generation vs. Fitness", 
+                    xlabel="Generation", 
+                    ylabel="Fitness", 
+                    linewidth=3, 
+                    font_size=14, 
+                    plot_type="plot",
+                    color="#3870FF",
+                    save_dir=None):
+
+        if not self.suppress_warnings: 
+            warnings.warn("Please use the plot_fitness() method instead of plot_result(). The plot_result() method will be removed in the future.")
+
+        return self.plot_fitness(title=title, 
+                                 xlabel=xlabel, 
+                                 ylabel=ylabel, 
+                                 linewidth=linewidth, 
+                                 font_size=font_size, 
+                                 plot_type=plot_type,
+                                 color=color,
+                                 save_dir=save_dir)
+
+    def plot_fitness(self, 
+                    title="PyGAD - Generation vs. Fitness", 
+                    xlabel="Generation", 
+                    ylabel="Fitness", 
+                    linewidth=3, 
+                    font_size=14, 
+                    plot_type="plot",
+                    color="#3870FF",
+                    save_dir=None):
+
+        """
+        Creates, shows, and returns a figure that summarizes how the fitness value evolved by generation. Can only be called after completing at least 1 generation. If no generation is completed, an exception is raised.
+
+        Accepts the following:
+            title: Figure title.
+            xlabel: Label on the X-axis.
+            ylabel: Label on the Y-axis.
+            linewidth: Line width of the plot. Defaults to 3.
+            font_size: Font size for the labels and title. Defaults to 14.
+            plot_type: Type of the plot which can be either "plot" (default), "scatter", or "bar".
+            color: Color of the plot which defaults to "#3870FF".
+            save_dir: Directory to save the figure.
+
+        Returns the figure.
+        """
+
+        if self.generations_completed < 1:
+            self.logger.error("The plot_fitness() (i.e. plot_result()) method can only be called after completing at least 1 generation but ({self.generations_completed}) is completed.")
+            raise RuntimeError("The plot_fitness() (i.e. plot_result()) method can only be called after completing at least 1 generation but ({self.generations_completed}) is completed.")
+
+        fig = matplotlib.pyplot.figure()
+        if plot_type == "plot":
+            matplotlib.pyplot.plot(self.best_solutions_fitness, linewidth=linewidth, color=color)
+        elif plot_type == "scatter":
+            matplotlib.pyplot.scatter(range(len(self.best_solutions_fitness)), self.best_solutions_fitness, linewidth=linewidth, color=color)
+        elif plot_type == "bar":
+            matplotlib.pyplot.bar(range(len(self.best_solutions_fitness)), self.best_solutions_fitness, linewidth=linewidth, color=color)
+        matplotlib.pyplot.title(title, fontsize=font_size)
+        matplotlib.pyplot.xlabel(xlabel, fontsize=font_size)
+        matplotlib.pyplot.ylabel(ylabel, fontsize=font_size)
+
+        if not save_dir is None:
+            matplotlib.pyplot.savefig(fname=save_dir, 
+                                      bbox_inches='tight')
+        matplotlib.pyplot.show()
+
+        return fig
+
+    def plot_new_solution_rate(self,
+                               title="PyGAD - Generation vs. New Solution Rate", 
+                               xlabel="Generation", 
+                               ylabel="New Solution Rate", 
+                               linewidth=3, 
+                               font_size=14, 
+                               plot_type="plot",
+                               color="#3870FF",
+                               save_dir=None):
+
+        """
+        Creates, shows, and returns a figure that summarizes the rate of exploring new solutions. This method works only when save_solutions=True in the constructor of the pygad.GA class.
+
+        Accepts the following:
+            title: Figure title.
+            xlabel: Label on the X-axis.
+            ylabel: Label on the Y-axis.
+            linewidth: Line width of the plot. Defaults to 3.
+            font_size: Font size for the labels and title. Defaults to 14.
+            plot_type: Type of the plot which can be either "plot" (default), "scatter", or "bar".
+            color: Color of the plot which defaults to "#3870FF".
+            save_dir: Directory to save the figure.
+
+        Returns the figure.
+        """
+
+        if self.generations_completed < 1:
+            self.logger.error("The plot_new_solution_rate() method can only be called after completing at least 1 generation but ({self.generations_completed}) is completed.")
+            raise RuntimeError("The plot_new_solution_rate() method can only be called after completing at least 1 generation but ({self.generations_completed}) is completed.")
+
+        if self.save_solutions == False:
+            self.logger.error("The plot_new_solution_rate() method works only when save_solutions=True in the constructor of the pygad.GA class.")
+            raise RuntimeError("The plot_new_solution_rate() method works only when save_solutions=True in the constructor of the pygad.GA class.")
+
+        unique_solutions = set()
+        num_unique_solutions_per_generation = []
+        for generation_idx in range(self.generations_completed):
+            
+            len_before = len(unique_solutions)
+
+            start = generation_idx * self.sol_per_pop
+            end = start + self.sol_per_pop
+        
+            for sol in self.solutions[start:end]:
+                unique_solutions.add(tuple(sol))
+        
+            len_after = len(unique_solutions)
+        
+            generation_num_unique_solutions = len_after - len_before
+            num_unique_solutions_per_generation.append(generation_num_unique_solutions)
+
+        fig = matplotlib.pyplot.figure()
+        if plot_type == "plot":
+            matplotlib.pyplot.plot(num_unique_solutions_per_generation, linewidth=linewidth, color=color)
+        elif plot_type == "scatter":
+            matplotlib.pyplot.scatter(range(self.generations_completed), num_unique_solutions_per_generation, linewidth=linewidth, color=color)
+        elif plot_type == "bar":
+            matplotlib.pyplot.bar(range(self.generations_completed), num_unique_solutions_per_generation, linewidth=linewidth, color=color)
+        matplotlib.pyplot.title(title, fontsize=font_size)
+        matplotlib.pyplot.xlabel(xlabel, fontsize=font_size)
+        matplotlib.pyplot.ylabel(ylabel, fontsize=font_size)
+
+        if not save_dir is None:
+            matplotlib.pyplot.savefig(fname=save_dir, 
+                                      bbox_inches='tight')
+        matplotlib.pyplot.show()
+
+        return fig
+
+    def plot_genes(self, 
+                   title="PyGAD - Gene", 
+                   xlabel="Gene", 
+                   ylabel="Value", 
+                   linewidth=3, 
+                   font_size=14,
+                   plot_type="plot",
+                   graph_type="plot",
+                   fill_color="#3870FF",
+                   color="black",
+                   solutions="all",
+                   save_dir=None):
+
+        """
+        Creates, shows, and returns a figure with number of subplots equal to the number of genes. Each subplot shows the gene value for each generation. 
+        This method works only when save_solutions=True in the constructor of the pygad.GA class. 
+        It also works only after completing at least 1 generation. If no generation is completed, an exception is raised.
+
+        Accepts the following:
+            title: Figure title.
+            xlabel: Label on the X-axis.
+            ylabel: Label on the Y-axis.
+            linewidth: Line width of the plot. Defaults to 3.
+            font_size: Font size for the labels and title. Defaults to 14.
+            plot_type: Type of the plot which can be either "plot" (default), "scatter", or "bar".
+            graph_type: Type of the graph which can be either "plot" (default), "boxplot", or "histogram".
+            fill_color: Fill color of the graph which defaults to "#3870FF". This has no effect if graph_type="plot".
+            color: Color of the plot which defaults to "black".
+            solutions: Defaults to "all" which means use all solutions. If "best" then only the best solutions are used.
+            save_dir: Directory to save the figure.
+
+        Returns the figure.
+        """
+
+        if self.generations_completed < 1:
+            self.logger.error("The plot_genes() method can only be called after completing at least 1 generation but ({self.generations_completed}) is completed.")
+            raise RuntimeError("The plot_genes() method can only be called after completing at least 1 generation but ({self.generations_completed}) is completed.")
+
+        if type(solutions) is str:
+            if solutions == 'all':
+                if self.save_solutions:
+                    solutions_to_plot = numpy.array(self.solutions)
+                else:
+                    self.logger.error("The plot_genes() method with solutions='all' can only be called if 'save_solutions=True' in the pygad.GA class constructor.")
+                    raise RuntimeError("The plot_genes() method with solutions='all' can only be called if 'save_solutions=True' in the pygad.GA class constructor.")
+            elif solutions == 'best':
+                if self.save_best_solutions:
+                    solutions_to_plot = self.best_solutions
+                else:
+                    self.logger.error("The plot_genes() method with solutions='best' can only be called if 'save_best_solutions=True' in the pygad.GA class constructor.")
+                    raise RuntimeError("The plot_genes() method with solutions='best' can only be called if 'save_best_solutions=True' in the pygad.GA class constructor.")
+            else:
+                self.logger.error("The solutions parameter can be either 'all' or 'best' but {solutions} found.")
+                raise RuntimeError("The solutions parameter can be either 'all' or 'best' but {solutions} found.")
+        else:
+            self.logger.error("The solutions parameter must be a string but {solutions_type} found.".format(solutions_type=type(solutions)))
+            raise RuntimeError("The solutions parameter must be a string but {solutions_type} found.".format(solutions_type=type(solutions)))
+
+        if graph_type == "plot":
+            # num_rows will be always be >= 1
+            # num_cols can only be 0 if num_genes=1
+            num_rows = int(numpy.ceil(self.num_genes/5.0))
+            num_cols = int(numpy.ceil(self.num_genes/num_rows))
+    
+            if num_cols == 0:
+                figsize = (10, 8)
+                # There is only a single gene
+                fig, ax = matplotlib.pyplot.subplots(num_rows, figsize=figsize)
+                if plot_type == "plot":
+                    ax.plot(solutions_to_plot[:, 0], linewidth=linewidth, color=fill_color)
+                elif plot_type == "scatter":
+                    ax.scatter(range(self.generations_completed + 1), solutions_to_plot[:, 0], linewidth=linewidth, color=fill_color)
+                elif plot_type == "bar":
+                    ax.bar(range(self.generations_completed + 1), solutions_to_plot[:, 0], linewidth=linewidth, color=fill_color)
+                ax.set_xlabel(0, fontsize=font_size)
+            else:
+                fig, axs = matplotlib.pyplot.subplots(num_rows, num_cols)
+    
+                if num_cols == 1 and num_rows == 1:
+                    fig.set_figwidth(5 * num_cols)
+                    fig.set_figheight(4)
+                    axs.plot(solutions_to_plot[:, 0], linewidth=linewidth, color=fill_color)
+                    axs.set_xlabel("Gene " + str(0), fontsize=font_size)
+                elif num_cols == 1 or num_rows == 1:
+                    fig.set_figwidth(5 * num_cols)
+                    fig.set_figheight(4)
+                    for gene_idx in range(len(axs)):
+                        if plot_type == "plot":
+                            axs[gene_idx].plot(solutions_to_plot[:, gene_idx], linewidth=linewidth, color=fill_color)
+                        elif plot_type == "scatter":
+                            axs[gene_idx].scatter(range(solutions_to_plot.shape[0]), solutions_to_plot[:, gene_idx], linewidth=linewidth, color=fill_color)
+                        elif plot_type == "bar":
+                            axs[gene_idx].bar(range(solutions_to_plot.shape[0]), solutions_to_plot[:, gene_idx], linewidth=linewidth, color=fill_color)
+                        axs[gene_idx].set_xlabel("Gene " + str(gene_idx), fontsize=font_size)
+                else:
+                    gene_idx = 0
+                    fig.set_figwidth(25)
+                    fig.set_figheight(4*num_rows)
+                    for row_idx in range(num_rows):
+                        for col_idx in range(num_cols):
+                            if gene_idx >= self.num_genes:
+                                # axs[row_idx, col_idx].remove()
+                                break
+                            if plot_type == "plot":
+                                axs[row_idx, col_idx].plot(solutions_to_plot[:, gene_idx], linewidth=linewidth, color=fill_color)
+                            elif plot_type == "scatter":
+                                axs[row_idx, col_idx].scatter(range(solutions_to_plot.shape[0]), solutions_to_plot[:, gene_idx], linewidth=linewidth, color=fill_color)
+                            elif plot_type == "bar":
+                                axs[row_idx, col_idx].bar(range(solutions_to_plot.shape[0]), solutions_to_plot[:, gene_idx], linewidth=linewidth, color=fill_color)
+                            axs[row_idx, col_idx].set_xlabel("Gene " + str(gene_idx), fontsize=font_size)
+                            gene_idx += 1
+    
+            fig.suptitle(title, fontsize=font_size, y=1.001)
+            matplotlib.pyplot.tight_layout()
+
+        elif graph_type == "boxplot":
+            fig = matplotlib.pyplot.figure(1, figsize=(0.7*self.num_genes, 6))
+
+            # Create an axes instance
+            ax = fig.add_subplot(111)
+            boxeplots = ax.boxplot(solutions_to_plot, 
+                                   labels=range(self.num_genes),
+                                   patch_artist=True)
+            # adding horizontal grid lines
+            ax.yaxis.grid(True)
+    
+            for box in boxeplots['boxes']:
+                # change outline color
+                box.set(color='black', linewidth=linewidth)
+                # change fill color https://color.adobe.com/create/color-wheel
+                box.set_facecolor(fill_color)
+
+            for whisker in boxeplots['whiskers']:
+                whisker.set(color=color, linewidth=linewidth)
+            for median in boxeplots['medians']:
+                median.set(color=color, linewidth=linewidth)
+            for cap in boxeplots['caps']:
+                cap.set(color=color, linewidth=linewidth)
+    
+            matplotlib.pyplot.title(title, fontsize=font_size)
+            matplotlib.pyplot.xlabel(xlabel, fontsize=font_size)
+            matplotlib.pyplot.ylabel(ylabel, fontsize=font_size)
+            matplotlib.pyplot.tight_layout()
+
+        elif graph_type == "histogram":
+            # num_rows will always be >= 1
+            # num_cols can only be 0 if num_genes=1
+            num_rows = int(numpy.ceil(self.num_genes/5.0))
+            num_cols = int(numpy.ceil(self.num_genes/num_rows))
+    
+            if num_cols == 0:
+                figsize = (10, 8)
+                # There is only a single gene
+                fig, ax = matplotlib.pyplot.subplots(num_rows, 
+                                                     figsize=figsize)
+                ax.hist(solutions_to_plot[:, 0], color=fill_color)
+                ax.set_xlabel(0, fontsize=font_size)
+            else:
+                fig, axs = matplotlib.pyplot.subplots(num_rows, num_cols)
+    
+                if num_cols == 1 and num_rows == 1:
+                    fig.set_figwidth(4 * num_cols)
+                    fig.set_figheight(3)
+                    axs.hist(solutions_to_plot[:, 0], 
+                             color=fill_color,
+                             rwidth=0.95)
+                    axs.set_xlabel("Gene " + str(0), fontsize=font_size)
+                elif num_cols == 1 or num_rows == 1:
+                    fig.set_figwidth(4 * num_cols)
+                    fig.set_figheight(3)
+                    for gene_idx in range(len(axs)):
+                        axs[gene_idx].hist(solutions_to_plot[:, gene_idx], 
+                                           color=fill_color,
+                                           rwidth=0.95)
+                        axs[gene_idx].set_xlabel("Gene " + str(gene_idx), fontsize=font_size)
+                else:
+                    gene_idx = 0
+                    fig.set_figwidth(20)
+                    fig.set_figheight(3*num_rows)
+                    for row_idx in range(num_rows):
+                        for col_idx in range(num_cols):
+                            if gene_idx >= self.num_genes:
+                                # axs[row_idx, col_idx].remove()
+                                break
+                            axs[row_idx, col_idx].hist(solutions_to_plot[:, gene_idx], 
+                                                       color=fill_color,
+                                                       rwidth=0.95)
+                            axs[row_idx, col_idx].set_xlabel("Gene " + str(gene_idx), fontsize=font_size)
+                            gene_idx += 1
+    
+            fig.suptitle(title, fontsize=font_size, y=1.001)
+            matplotlib.pyplot.tight_layout()
+
+        if not save_dir is None:
+            matplotlib.pyplot.savefig(fname=save_dir, 
+                                      bbox_inches='tight')
+
+        matplotlib.pyplot.show()
+
+        return fig
```

### Comparing `pygad-3.0.1/pygad.egg-info/PKG-INFO` & `pygad-3.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,346 +1,331 @@
-Metadata-Version: 2.1
-Name: pygad
-Version: 3.0.1
-Summary: PyGAD: A Python 3 Library for Building the Genetic Algorithm and Training Machine Learning Algoithms (Keras & PyTorch).
-Home-page: https://github.com/ahmedfgad/GeneticAlgorithmPython
-Author: Ahmed Fawzy Gad
-Author-email: ahmed.f.gad@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-
-# PyGAD:  Genetic Algorithm in Python
-
-[PyGAD](https://pypi.org/project/pygad) is an open-source easy-to-use Python 3 library for building the genetic algorithm and optimizing machine learning algorithms. It supports Keras and PyTorch.
-
-Check documentation of the [PyGAD](https://pygad.readthedocs.io/en/latest).
-
-[![Downloads](https://pepy.tech/badge/pygad)](https://pepy.tech/project/pygad) ![Docs](https://readthedocs.org/projects/pygad/badge)
-
-![PYGAD-LOGO](https://user-images.githubusercontent.com/16560492/101267295-c74c0180-375f-11eb-9ad0-f8e37bd796ce.png)
-
-[PyGAD](https://pypi.org/project/pygad) supports different types of crossover, mutation, and parent selection. [PyGAD](https://pypi.org/project/pygad) allows different types of problems to be optimized using the genetic algorithm by customizing the fitness function. 
-
-The library is under active development and more features are added regularly. If you want a feature to be supported, please check the **Contact Us** section to send a request.
-
-# Donation
-
-- [Credit/Debit Card](https://donate.stripe.com/eVa5kO866elKgM0144): https://donate.stripe.com/eVa5kO866elKgM0144
-- [Open Collective](https://opencollective.com/pygad): [opencollective.com/pygad](https://opencollective.com/pygad)
-- PayPal: Use either this link: [paypal.me/ahmedfgad](https://paypal.me/ahmedfgad) or the e-mail address ahmed.f.gad@gmail.com
-- Interac e-Transfer: Use e-mail address ahmed.f.gad@gmail.com
-
-# Installation
-
-To install [PyGAD](https://pypi.org/project/pygad), simply use pip to download and install the library from [PyPI](https://pypi.org/project/pygad) (Python Package Index). The library lives a PyPI at this page https://pypi.org/project/pygad.
-
-Install PyGAD with the following command:
-
-```python
-pip install pygad
-```
-
-PyGAD is developed in Python 3.7.3 and depends on NumPy for creating and manipulating arrays and Matplotlib for creating figures. The exact NumPy version used in developing PyGAD is 1.16.4. For Matplotlib, the version is 3.1.0.
-
-To get started with PyGAD, please read the documentation at [Read The Docs](https://pygad.readthedocs.io/) https://pygad.readthedocs.io.
-
-# PyGAD Source Code
-
-The source code of the PyGAD' modules is found in the following GitHub projects:
-
-- [pygad](https://github.com/ahmedfgad/GeneticAlgorithmPython): (https://github.com/ahmedfgad/GeneticAlgorithmPython)
-- [pygad.nn](https://github.com/ahmedfgad/NumPyANN): https://github.com/ahmedfgad/NumPyANN
-- [pygad.gann](https://github.com/ahmedfgad/NeuralGenetic): https://github.com/ahmedfgad/NeuralGenetic
-- [pygad.cnn](https://github.com/ahmedfgad/NumPyCNN): https://github.com/ahmedfgad/NumPyCNN
-- [pygad.gacnn](https://github.com/ahmedfgad/CNNGenetic): https://github.com/ahmedfgad/CNNGenetic
-- [pygad.kerasga](https://github.com/ahmedfgad/KerasGA): https://github.com/ahmedfgad/KerasGA
-- [pygad.torchga](https://github.com/ahmedfgad/TorchGA): https://github.com/ahmedfgad/TorchGA
-
-The documentation of PyGAD is available at [Read The Docs](https://pygad.readthedocs.io/) https://pygad.readthedocs.io.
-
-# PyGAD Documentation
-
-The documentation of the PyGAD library is available at [Read The Docs](https://pygad.readthedocs.io) at this link: https://pygad.readthedocs.io. It discusses the modules supported by PyGAD, all its classes, methods, attribute, and functions. For each module, a number of examples are given.
-
-If there is an issue using PyGAD, feel free to post at issue in this [GitHub repository](https://github.com/ahmedfgad/GeneticAlgorithmPython) https://github.com/ahmedfgad/GeneticAlgorithmPython or by sending an e-mail to ahmed.f.gad@gmail.com. 
-
-If you built a project that uses PyGAD, then please drop an e-mail to ahmed.f.gad@gmail.com with the following information so that your project is included in the documentation.
-
-- Project title
-- Brief description
-- Preferably, a link that directs the readers to your project
-
-Please check the **Contact Us** section for more contact details.
-
-# Life Cycle of PyGAD
-
-The next figure lists the different stages in the lifecycle of an instance of the `pygad.GA` class. Note that PyGAD stops when either all generations are completed or when the function passed to the `on_generation` parameter returns the string `stop`.
-
-![PyGAD Lifecycle](https://user-images.githubusercontent.com/16560492/220486073-c5b6089d-81e4-44d9-a53c-385f479a7273.jpg)
-
-The next code implements all the callback functions to trace the execution of the genetic algorithm. Each callback function prints its name.
-
-```python
-import pygad
-import numpy
-
-function_inputs = [4,-2,3.5,5,-11,-4.7]
-desired_output = 44
-
-def fitness_func(solution, solution_idx):
-    output = numpy.sum(solution*function_inputs)
-    fitness = 1.0 / (numpy.abs(output - desired_output) + 0.000001)
-    return fitness
-
-fitness_function = fitness_func
-
-def on_start(ga_instance):
-    print("on_start()")
-
-def on_fitness(ga_instance, population_fitness):
-    print("on_fitness()")
-
-def on_parents(ga_instance, selected_parents):
-    print("on_parents()")
-
-def on_crossover(ga_instance, offspring_crossover):
-    print("on_crossover()")
-
-def on_mutation(ga_instance, offspring_mutation):
-    print("on_mutation()")
-
-def on_generation(ga_instance):
-    print("on_generation()")
-
-def on_stop(ga_instance, last_population_fitness):
-    print("on_stop()")
-
-ga_instance = pygad.GA(num_generations=3,
-                       num_parents_mating=5,
-                       fitness_func=fitness_function,
-                       sol_per_pop=10,
-                       num_genes=len(function_inputs),
-                       on_start=on_start,
-                       on_fitness=on_fitness,
-                       on_parents=on_parents,
-                       on_crossover=on_crossover,
-                       on_mutation=on_mutation,
-                       on_generation=on_generation,
-                       on_stop=on_stop)
-
-ga_instance.run()
-```
-
-Based on the used 3 generations as assigned to the `num_generations` argument, here is the output.
-
-```
-on_start()
-
-on_fitness()
-on_parents()
-on_crossover()
-on_mutation()
-on_generation()
-
-on_fitness()
-on_parents()
-on_crossover()
-on_mutation()
-on_generation()
-
-on_fitness()
-on_parents()
-on_crossover()
-on_mutation()
-on_generation()
-
-on_stop()
-```
-
-# Example
-
-Check the [PyGAD's documentation](https://pygad.readthedocs.io/en/latest/README_pygad_ReadTheDocs.html) for information about the implementation of this example.
-
-```python
-import pygad
-import numpy
-
-"""
-Given the following function:
-    y = f(w1:w6) = w1x1 + w2x2 + w3x3 + w4x4 + w5x5 + 6wx6
-    where (x1,x2,x3,x4,x5,x6)=(4,-2,3.5,5,-11,-4.7) and y=44
-What are the best values for the 6 weights (w1 to w6)? We are going to use the genetic algorithm to optimize this function.
-"""
-
-function_inputs = [4,-2,3.5,5,-11,-4.7] # Function inputs.
-desired_output = 44 # Function output.
-
-def fitness_func(solution, solution_idx):
-    # Calculating the fitness value of each solution in the current population.
-    # The fitness function calulates the sum of products between each input and its corresponding weight.
-    output = numpy.sum(solution*function_inputs)
-    fitness = 1.0 / numpy.abs(output - desired_output)
-    return fitness
-
-fitness_function = fitness_func
-
-num_generations = 100 # Number of generations.
-num_parents_mating = 7 # Number of solutions to be selected as parents in the mating pool.
-
-# To prepare the initial population, there are 2 ways:
-# 1) Prepare it yourself and pass it to the initial_population parameter. This way is useful when the user wants to start the genetic algorithm with a custom initial population.
-# 2) Assign valid integer values to the sol_per_pop and num_genes parameters. If the initial_population parameter exists, then the sol_per_pop and num_genes parameters are useless.
-sol_per_pop = 50 # Number of solutions in the population.
-num_genes = len(function_inputs)
-
-last_fitness = 0
-def callback_generation(ga_instance):
-    global last_fitness
-    print("Generation = {generation}".format(generation=ga_instance.generations_completed))
-    print("Fitness    = {fitness}".format(fitness=ga_instance.best_solution()[1]))
-    print("Change     = {change}".format(change=ga_instance.best_solution()[1] - last_fitness))
-    last_fitness = ga_instance.best_solution()[1]
-
-# Creating an instance of the GA class inside the ga module. Some parameters are initialized within the constructor.
-ga_instance = pygad.GA(num_generations=num_generations,
-                       num_parents_mating=num_parents_mating, 
-                       fitness_func=fitness_function,
-                       sol_per_pop=sol_per_pop, 
-                       num_genes=num_genes,
-                       on_generation=callback_generation)
-
-# Running the GA to optimize the parameters of the function.
-ga_instance.run()
-
-# After the generations complete, some plots are showed that summarize the how the outputs/fitenss values evolve over generations.
-ga_instance.plot_fitness()
-
-# Returning the details of the best solution.
-solution, solution_fitness, solution_idx = ga_instance.best_solution()
-print("Parameters of the best solution : {solution}".format(solution=solution))
-print("Fitness value of the best solution = {solution_fitness}".format(solution_fitness=solution_fitness))
-print("Index of the best solution : {solution_idx}".format(solution_idx=solution_idx))
-
-prediction = numpy.sum(numpy.array(function_inputs)*solution)
-print("Predicted output based on the best solution : {prediction}".format(prediction=prediction))
-
-if ga_instance.best_solution_generation != -1:
-    print("Best fitness value reached after {best_solution_generation} generations.".format(best_solution_generation=ga_instance.best_solution_generation))
-
-# Saving the GA instance.
-filename = 'genetic' # The filename to which the instance is saved. The name is without extension.
-ga_instance.save(filename=filename)
-
-# Loading the saved GA instance.
-loaded_ga_instance = pygad.load(filename=filename)
-loaded_ga_instance.plot_fitness()
-```
-
-# For More Information
-
-There are different resources that can be used to get started with the genetic algorithm and building it in Python. 
-
-## Tutorial: Implementing Genetic Algorithm in Python
-
-To start with coding the genetic algorithm, you can check the tutorial titled [**Genetic Algorithm Implementation in Python**](https://www.linkedin.com/pulse/genetic-algorithm-implementation-python-ahmed-gad) available at these links:
-
-- [LinkedIn](https://www.linkedin.com/pulse/genetic-algorithm-implementation-python-ahmed-gad)
-- [Towards Data Science](https://towardsdatascience.com/genetic-algorithm-implementation-in-python-5ab67bb124a6)
-- [KDnuggets](https://www.kdnuggets.com/2018/07/genetic-algorithm-implementation-python.html)
-
-[This tutorial](https://www.linkedin.com/pulse/genetic-algorithm-implementation-python-ahmed-gad) is prepared based on a previous version of the project but it still a good resource to start with coding the genetic algorithm.
-
-[![Genetic Algorithm Implementation in Python](https://user-images.githubusercontent.com/16560492/78830052-a3c19300-79e7-11ea-8b9b-4b343ea4049c.png)](https://www.linkedin.com/pulse/genetic-algorithm-implementation-python-ahmed-gad)
-
-## Tutorial: Introduction to Genetic Algorithm
-
-Get started with the genetic algorithm by reading the tutorial titled [**Introduction to Optimization with Genetic Algorithm**](https://www.linkedin.com/pulse/introduction-optimization-genetic-algorithm-ahmed-gad) which is available at these links:
-
-* [LinkedIn](https://www.linkedin.com/pulse/introduction-optimization-genetic-algorithm-ahmed-gad)
-* [Towards Data Science](https://towardsdatascience.com/introduction-to-optimization-with-genetic-algorithm-2f5001d9964b)
-* [KDnuggets](https://www.kdnuggets.com/2018/03/introduction-optimization-with-genetic-algorithm.html)
-
-[![Introduction to Genetic Algorithm](https://user-images.githubusercontent.com/16560492/82078259-26252d00-96e1-11ea-9a02-52a99e1054b9.jpg)](https://www.linkedin.com/pulse/introduction-optimization-genetic-algorithm-ahmed-gad)
-
-## Tutorial: Build Neural Networks in Python
-
-Read about building neural networks in Python through the tutorial titled [**Artificial Neural Network Implementation using NumPy and Classification of the Fruits360 Image Dataset**](https://www.linkedin.com/pulse/artificial-neural-network-implementation-using-numpy-fruits360-gad) available at these links:
-
-* [LinkedIn](https://www.linkedin.com/pulse/artificial-neural-network-implementation-using-numpy-fruits360-gad)
-* [Towards Data Science](https://towardsdatascience.com/artificial-neural-network-implementation-using-numpy-and-classification-of-the-fruits360-image-3c56affa4491)
-* [KDnuggets](https://www.kdnuggets.com/2019/02/artificial-neural-network-implementation-using-numpy-and-image-classification.html)
-
-[![Building Neural Networks Python](https://user-images.githubusercontent.com/16560492/82078281-30472b80-96e1-11ea-8017-6a1f4383d602.jpg)](https://www.linkedin.com/pulse/artificial-neural-network-implementation-using-numpy-fruits360-gad)
-
-## Tutorial: Optimize Neural Networks with Genetic Algorithm
-
-Read about training neural networks using the genetic algorithm through the tutorial titled [**Artificial Neural Networks Optimization using Genetic Algorithm with Python**](https://www.linkedin.com/pulse/artificial-neural-networks-optimization-using-genetic-ahmed-gad) available at these links:
-
-- [LinkedIn](https://www.linkedin.com/pulse/artificial-neural-networks-optimization-using-genetic-ahmed-gad)
-- [Towards Data Science](https://towardsdatascience.com/artificial-neural-networks-optimization-using-genetic-algorithm-with-python-1fe8ed17733e)
-- [KDnuggets](https://www.kdnuggets.com/2019/03/artificial-neural-networks-optimization-genetic-algorithm-python.html)
-
-[![Training Neural Networks using Genetic Algorithm Python](https://user-images.githubusercontent.com/16560492/82078300-376e3980-96e1-11ea-821c-aa6b8ceb44d4.jpg)](https://www.linkedin.com/pulse/artificial-neural-networks-optimization-using-genetic-ahmed-gad)
-
-## Tutorial: Building CNN in Python
-
-To start with coding the genetic algorithm, you can check the tutorial titled [**Building Convolutional Neural Network using NumPy from Scratch**](https://www.linkedin.com/pulse/building-convolutional-neural-network-using-numpy-from-ahmed-gad) available at these links:
-
-- [LinkedIn](https://www.linkedin.com/pulse/building-convolutional-neural-network-using-numpy-from-ahmed-gad)
-- [Towards Data Science](https://towardsdatascience.com/building-convolutional-neural-network-using-numpy-from-scratch-b30aac50e50a)
-- [KDnuggets](https://www.kdnuggets.com/2018/04/building-convolutional-neural-network-numpy-scratch.html)
-- [Chinese Translation](http://m.aliyun.com/yunqi/articles/585741)
-
-[This tutorial](https://www.linkedin.com/pulse/building-convolutional-neural-network-using-numpy-from-ahmed-gad)) is prepared based on a previous version of the project but it still a good resource to start with coding CNNs.
-
-[![Building CNN in Python](https://user-images.githubusercontent.com/16560492/82431022-6c3a1200-9a8e-11ea-8f1b-b055196d76e3.png)](https://www.linkedin.com/pulse/building-convolutional-neural-network-using-numpy-from-ahmed-gad)
-
-## Tutorial: Derivation of CNN from FCNN
-
-Get started with the genetic algorithm by reading the tutorial titled [**Derivation of Convolutional Neural Network from Fully Connected Network Step-By-Step**](https://www.linkedin.com/pulse/derivation-convolutional-neural-network-from-fully-connected-gad) which is available at these links:
-
-* [LinkedIn](https://www.linkedin.com/pulse/derivation-convolutional-neural-network-from-fully-connected-gad)
-* [Towards Data Science](https://towardsdatascience.com/derivation-of-convolutional-neural-network-from-fully-connected-network-step-by-step-b42ebafa5275)
-* [KDnuggets](https://www.kdnuggets.com/2018/04/derivation-convolutional-neural-network-fully-connected-step-by-step.html)
-
-[![Derivation of CNN from FCNN](https://user-images.githubusercontent.com/16560492/82431369-db176b00-9a8e-11ea-99bd-e845192873fc.png)](https://www.linkedin.com/pulse/derivation-convolutional-neural-network-from-fully-connected-gad)
-
-## Book: Practical Computer Vision Applications Using Deep Learning with CNNs
-
-You can also check my book cited as [**Ahmed Fawzy Gad 'Practical Computer Vision Applications Using Deep Learning with CNNs'. Dec. 2018, Apress, 978-1-4842-4167-7**](https://www.amazon.com/Practical-Computer-Vision-Applications-Learning/dp/1484241665) which discusses neural networks, convolutional neural networks, deep learning, genetic algorithm, and more.
-
-Find the book at these links:
-
-- [Amazon](https://www.amazon.com/Practical-Computer-Vision-Applications-Learning/dp/1484241665)
-- [Springer](https://link.springer.com/book/10.1007/978-1-4842-4167-7)
-- [Apress](https://www.apress.com/gp/book/9781484241660)
-- [O'Reilly](https://www.oreilly.com/library/view/practical-computer-vision/9781484241677)
-- [Google Books](https://books.google.com.eg/books?id=xLd9DwAAQBAJ)
-
-![Fig04](https://user-images.githubusercontent.com/16560492/78830077-ae7c2800-79e7-11ea-980b-53b6bd879eeb.jpg)
-
-# Citing PyGAD - Bibtex Formatted Citation
-
-If you used PyGAD, please consider adding a citation to the following paper about PyGAD:
-
-```
-@misc{gad2021pygad,
-      title={PyGAD: An Intuitive Genetic Algorithm Python Library}, 
-      author={Ahmed Fawzy Gad},
-      year={2021},
-      eprint={2106.06158},
-      archivePrefix={arXiv},
-      primaryClass={cs.NE}
-}
-```
-
-# Contact Us
-
-* E-mail: ahmed.f.gad@gmail.com
-* [LinkedIn](https://www.linkedin.com/in/ahmedfgad)
-* [Paperspace](https://blog.paperspace.com/author/ahmed)
-* [KDnuggets](https://kdnuggets.com/author/ahmed-gad)
-* [TowardsDataScience](https://towardsdatascience.com/@ahmedfgad)
-* [GitHub](https://github.com/ahmedfgad)
-
-
+# PyGAD:  Genetic Algorithm in Python
+
+[PyGAD](https://pypi.org/project/pygad) is an open-source easy-to-use Python 3 library for building the genetic algorithm and optimizing machine learning algorithms. It supports Keras and PyTorch.
+
+Check documentation of the [PyGAD](https://pygad.readthedocs.io/en/latest).
+
+[![Downloads](https://pepy.tech/badge/pygad)](https://pepy.tech/project/pygad) ![Docs](https://readthedocs.org/projects/pygad/badge)
+
+![PYGAD-LOGO](https://user-images.githubusercontent.com/16560492/101267295-c74c0180-375f-11eb-9ad0-f8e37bd796ce.png)
+
+[PyGAD](https://pypi.org/project/pygad) supports different types of crossover, mutation, and parent selection. [PyGAD](https://pypi.org/project/pygad) allows different types of problems to be optimized using the genetic algorithm by customizing the fitness function. 
+
+The library is under active development and more features are added regularly. If you want a feature to be supported, please check the **Contact Us** section to send a request.
+
+# Donation
+
+* [Credit/Debit Card](https://donate.stripe.com/eVa5kO866elKgM0144): https://donate.stripe.com/eVa5kO866elKgM0144
+* [Open Collective](https://opencollective.com/pygad): [opencollective.com/pygad](https://opencollective.com/pygad)
+* PayPal: Use either this link: [paypal.me/ahmedfgad](https://paypal.me/ahmedfgad) or the e-mail address ahmed.f.gad@gmail.com
+* Interac e-Transfer: Use e-mail address ahmed.f.gad@gmail.com
+
+# Installation
+
+To install [PyGAD](https://pypi.org/project/pygad), simply use pip to download and install the library from [PyPI](https://pypi.org/project/pygad) (Python Package Index). The library is at PyPI at this page https://pypi.org/project/pygad.
+
+Install PyGAD with the following command:
+
+```python
+pip install pygad
+```
+
+To get started with PyGAD, please read the documentation at [Read The Docs](https://pygad.readthedocs.io/) https://pygad.readthedocs.io.
+
+# PyGAD Source Code
+
+The source code of the PyGAD' modules is found in the following GitHub projects:
+
+- [pygad](https://github.com/ahmedfgad/GeneticAlgorithmPython): (https://github.com/ahmedfgad/GeneticAlgorithmPython)
+- [pygad.nn](https://github.com/ahmedfgad/NumPyANN): https://github.com/ahmedfgad/NumPyANN
+- [pygad.gann](https://github.com/ahmedfgad/NeuralGenetic): https://github.com/ahmedfgad/NeuralGenetic
+- [pygad.cnn](https://github.com/ahmedfgad/NumPyCNN): https://github.com/ahmedfgad/NumPyCNN
+- [pygad.gacnn](https://github.com/ahmedfgad/CNNGenetic): https://github.com/ahmedfgad/CNNGenetic
+- [pygad.kerasga](https://github.com/ahmedfgad/KerasGA): https://github.com/ahmedfgad/KerasGA
+- [pygad.torchga](https://github.com/ahmedfgad/TorchGA): https://github.com/ahmedfgad/TorchGA
+
+The documentation of PyGAD is available at [Read The Docs](https://pygad.readthedocs.io/) https://pygad.readthedocs.io.
+
+# PyGAD Documentation
+
+The documentation of the PyGAD library is available at [Read The Docs](https://pygad.readthedocs.io) at this link: https://pygad.readthedocs.io. It discusses the modules supported by PyGAD, all its classes, methods, attribute, and functions. For each module, a number of examples are given.
+
+If there is an issue using PyGAD, feel free to post at issue in this [GitHub repository](https://github.com/ahmedfgad/GeneticAlgorithmPython) https://github.com/ahmedfgad/GeneticAlgorithmPython or by sending an e-mail to ahmed.f.gad@gmail.com. 
+
+If you built a project that uses PyGAD, then please drop an e-mail to ahmed.f.gad@gmail.com with the following information so that your project is included in the documentation.
+
+- Project title
+- Brief description
+- Preferably, a link that directs the readers to your project
+
+Please check the **Contact Us** section for more contact details.
+
+# Life Cycle of PyGAD
+
+The next figure lists the different stages in the lifecycle of an instance of the `pygad.GA` class. Note that PyGAD stops when either all generations are completed or when the function passed to the `on_generation` parameter returns the string `stop`.
+
+![PyGAD Lifecycle](https://user-images.githubusercontent.com/16560492/220486073-c5b6089d-81e4-44d9-a53c-385f479a7273.jpg)
+
+The next code implements all the callback functions to trace the execution of the genetic algorithm. Each callback function prints its name.
+
+```python
+import pygad
+import numpy
+
+function_inputs = [4,-2,3.5,5,-11,-4.7]
+desired_output = 44
+
+def fitness_func(ga_instance, solution, solution_idx):
+    output = numpy.sum(solution*function_inputs)
+    fitness = 1.0 / (numpy.abs(output - desired_output) + 0.000001)
+    return fitness
+
+fitness_function = fitness_func
+
+def on_start(ga_instance):
+    print("on_start()")
+
+def on_fitness(ga_instance, population_fitness):
+    print("on_fitness()")
+
+def on_parents(ga_instance, selected_parents):
+    print("on_parents()")
+
+def on_crossover(ga_instance, offspring_crossover):
+    print("on_crossover()")
+
+def on_mutation(ga_instance, offspring_mutation):
+    print("on_mutation()")
+
+def on_generation(ga_instance):
+    print("on_generation()")
+
+def on_stop(ga_instance, last_population_fitness):
+    print("on_stop()")
+
+ga_instance = pygad.GA(num_generations=3,
+                       num_parents_mating=5,
+                       fitness_func=fitness_function,
+                       sol_per_pop=10,
+                       num_genes=len(function_inputs),
+                       on_start=on_start,
+                       on_fitness=on_fitness,
+                       on_parents=on_parents,
+                       on_crossover=on_crossover,
+                       on_mutation=on_mutation,
+                       on_generation=on_generation,
+                       on_stop=on_stop)
+
+ga_instance.run()
+```
+
+Based on the used 3 generations as assigned to the `num_generations` argument, here is the output.
+
+```
+on_start()
+
+on_fitness()
+on_parents()
+on_crossover()
+on_mutation()
+on_generation()
+
+on_fitness()
+on_parents()
+on_crossover()
+on_mutation()
+on_generation()
+
+on_fitness()
+on_parents()
+on_crossover()
+on_mutation()
+on_generation()
+
+on_stop()
+```
+
+# Example
+
+Check the [PyGAD's documentation](https://pygad.readthedocs.io/en/latest/pygad.html) for information about the implementation of this example.
+
+```python
+import pygad
+import numpy
+
+"""
+Given the following function:
+    y = f(w1:w6) = w1x1 + w2x2 + w3x3 + w4x4 + w5x5 + 6wx6
+    where (x1,x2,x3,x4,x5,x6)=(4,-2,3.5,5,-11,-4.7) and y=44
+What are the best values for the 6 weights (w1 to w6)? We are going to use the genetic algorithm to optimize this function.
+"""
+
+function_inputs = [4,-2,3.5,5,-11,-4.7] # Function inputs.
+desired_output = 44 # Function output.
+
+def fitness_func(ga_instance, solution, solution_idx):
+    # Calculating the fitness value of each solution in the current population.
+    # The fitness function calulates the sum of products between each input and its corresponding weight.
+    output = numpy.sum(solution*function_inputs)
+    fitness = 1.0 / numpy.abs(output - desired_output)
+    return fitness
+
+fitness_function = fitness_func
+
+num_generations = 100 # Number of generations.
+num_parents_mating = 7 # Number of solutions to be selected as parents in the mating pool.
+
+# To prepare the initial population, there are 2 ways:
+# 1) Prepare it yourself and pass it to the initial_population parameter. This way is useful when the user wants to start the genetic algorithm with a custom initial population.
+# 2) Assign valid integer values to the sol_per_pop and num_genes parameters. If the initial_population parameter exists, then the sol_per_pop and num_genes parameters are useless.
+sol_per_pop = 50 # Number of solutions in the population.
+num_genes = len(function_inputs)
+
+last_fitness = 0
+def callback_generation(ga_instance):
+    global last_fitness
+    print("Generation = {generation}".format(generation=ga_instance.generations_completed))
+    print("Fitness    = {fitness}".format(fitness=ga_instance.best_solution()[1]))
+    print("Change     = {change}".format(change=ga_instance.best_solution()[1] - last_fitness))
+    last_fitness = ga_instance.best_solution()[1]
+
+# Creating an instance of the GA class inside the ga module. Some parameters are initialized within the constructor.
+ga_instance = pygad.GA(num_generations=num_generations,
+                       num_parents_mating=num_parents_mating, 
+                       fitness_func=fitness_function,
+                       sol_per_pop=sol_per_pop, 
+                       num_genes=num_genes,
+                       on_generation=callback_generation)
+
+# Running the GA to optimize the parameters of the function.
+ga_instance.run()
+
+# After the generations complete, some plots are showed that summarize the how the outputs/fitenss values evolve over generations.
+ga_instance.plot_fitness()
+
+# Returning the details of the best solution.
+solution, solution_fitness, solution_idx = ga_instance.best_solution()
+print("Parameters of the best solution : {solution}".format(solution=solution))
+print("Fitness value of the best solution = {solution_fitness}".format(solution_fitness=solution_fitness))
+print("Index of the best solution : {solution_idx}".format(solution_idx=solution_idx))
+
+prediction = numpy.sum(numpy.array(function_inputs)*solution)
+print("Predicted output based on the best solution : {prediction}".format(prediction=prediction))
+
+if ga_instance.best_solution_generation != -1:
+    print("Best fitness value reached after {best_solution_generation} generations.".format(best_solution_generation=ga_instance.best_solution_generation))
+
+# Saving the GA instance.
+filename = 'genetic' # The filename to which the instance is saved. The name is without extension.
+ga_instance.save(filename=filename)
+
+# Loading the saved GA instance.
+loaded_ga_instance = pygad.load(filename=filename)
+loaded_ga_instance.plot_fitness()
+```
+
+# For More Information
+
+There are different resources that can be used to get started with the genetic algorithm and building it in Python. 
+
+## Tutorial: Implementing Genetic Algorithm in Python
+
+To start with coding the genetic algorithm, you can check the tutorial titled [**Genetic Algorithm Implementation in Python**](https://www.linkedin.com/pulse/genetic-algorithm-implementation-python-ahmed-gad) available at these links:
+
+- [LinkedIn](https://www.linkedin.com/pulse/genetic-algorithm-implementation-python-ahmed-gad)
+- [Towards Data Science](https://towardsdatascience.com/genetic-algorithm-implementation-in-python-5ab67bb124a6)
+- [KDnuggets](https://www.kdnuggets.com/2018/07/genetic-algorithm-implementation-python.html)
+
+[This tutorial](https://www.linkedin.com/pulse/genetic-algorithm-implementation-python-ahmed-gad) is prepared based on a previous version of the project but it still a good resource to start with coding the genetic algorithm.
+
+[![Genetic Algorithm Implementation in Python](https://user-images.githubusercontent.com/16560492/78830052-a3c19300-79e7-11ea-8b9b-4b343ea4049c.png)](https://www.linkedin.com/pulse/genetic-algorithm-implementation-python-ahmed-gad)
+
+## Tutorial: Introduction to Genetic Algorithm
+
+Get started with the genetic algorithm by reading the tutorial titled [**Introduction to Optimization with Genetic Algorithm**](https://www.linkedin.com/pulse/introduction-optimization-genetic-algorithm-ahmed-gad) which is available at these links:
+
+* [LinkedIn](https://www.linkedin.com/pulse/introduction-optimization-genetic-algorithm-ahmed-gad)
+* [Towards Data Science](https://towardsdatascience.com/introduction-to-optimization-with-genetic-algorithm-2f5001d9964b)
+* [KDnuggets](https://www.kdnuggets.com/2018/03/introduction-optimization-with-genetic-algorithm.html)
+
+[![Introduction to Genetic Algorithm](https://user-images.githubusercontent.com/16560492/82078259-26252d00-96e1-11ea-9a02-52a99e1054b9.jpg)](https://www.linkedin.com/pulse/introduction-optimization-genetic-algorithm-ahmed-gad)
+
+## Tutorial: Build Neural Networks in Python
+
+Read about building neural networks in Python through the tutorial titled [**Artificial Neural Network Implementation using NumPy and Classification of the Fruits360 Image Dataset**](https://www.linkedin.com/pulse/artificial-neural-network-implementation-using-numpy-fruits360-gad) available at these links:
+
+* [LinkedIn](https://www.linkedin.com/pulse/artificial-neural-network-implementation-using-numpy-fruits360-gad)
+* [Towards Data Science](https://towardsdatascience.com/artificial-neural-network-implementation-using-numpy-and-classification-of-the-fruits360-image-3c56affa4491)
+* [KDnuggets](https://www.kdnuggets.com/2019/02/artificial-neural-network-implementation-using-numpy-and-image-classification.html)
+
+[![Building Neural Networks Python](https://user-images.githubusercontent.com/16560492/82078281-30472b80-96e1-11ea-8017-6a1f4383d602.jpg)](https://www.linkedin.com/pulse/artificial-neural-network-implementation-using-numpy-fruits360-gad)
+
+## Tutorial: Optimize Neural Networks with Genetic Algorithm
+
+Read about training neural networks using the genetic algorithm through the tutorial titled [**Artificial Neural Networks Optimization using Genetic Algorithm with Python**](https://www.linkedin.com/pulse/artificial-neural-networks-optimization-using-genetic-ahmed-gad) available at these links:
+
+- [LinkedIn](https://www.linkedin.com/pulse/artificial-neural-networks-optimization-using-genetic-ahmed-gad)
+- [Towards Data Science](https://towardsdatascience.com/artificial-neural-networks-optimization-using-genetic-algorithm-with-python-1fe8ed17733e)
+- [KDnuggets](https://www.kdnuggets.com/2019/03/artificial-neural-networks-optimization-genetic-algorithm-python.html)
+
+[![Training Neural Networks using Genetic Algorithm Python](https://user-images.githubusercontent.com/16560492/82078300-376e3980-96e1-11ea-821c-aa6b8ceb44d4.jpg)](https://www.linkedin.com/pulse/artificial-neural-networks-optimization-using-genetic-ahmed-gad)
+
+## Tutorial: Building CNN in Python
+
+To start with coding the genetic algorithm, you can check the tutorial titled [**Building Convolutional Neural Network using NumPy from Scratch**](https://www.linkedin.com/pulse/building-convolutional-neural-network-using-numpy-from-ahmed-gad) available at these links:
+
+- [LinkedIn](https://www.linkedin.com/pulse/building-convolutional-neural-network-using-numpy-from-ahmed-gad)
+- [Towards Data Science](https://towardsdatascience.com/building-convolutional-neural-network-using-numpy-from-scratch-b30aac50e50a)
+- [KDnuggets](https://www.kdnuggets.com/2018/04/building-convolutional-neural-network-numpy-scratch.html)
+- [Chinese Translation](http://m.aliyun.com/yunqi/articles/585741)
+
+[This tutorial](https://www.linkedin.com/pulse/building-convolutional-neural-network-using-numpy-from-ahmed-gad)) is prepared based on a previous version of the project but it still a good resource to start with coding CNNs.
+
+[![Building CNN in Python](https://user-images.githubusercontent.com/16560492/82431022-6c3a1200-9a8e-11ea-8f1b-b055196d76e3.png)](https://www.linkedin.com/pulse/building-convolutional-neural-network-using-numpy-from-ahmed-gad)
+
+## Tutorial: Derivation of CNN from FCNN
+
+Get started with the genetic algorithm by reading the tutorial titled [**Derivation of Convolutional Neural Network from Fully Connected Network Step-By-Step**](https://www.linkedin.com/pulse/derivation-convolutional-neural-network-from-fully-connected-gad) which is available at these links:
+
+* [LinkedIn](https://www.linkedin.com/pulse/derivation-convolutional-neural-network-from-fully-connected-gad)
+* [Towards Data Science](https://towardsdatascience.com/derivation-of-convolutional-neural-network-from-fully-connected-network-step-by-step-b42ebafa5275)
+* [KDnuggets](https://www.kdnuggets.com/2018/04/derivation-convolutional-neural-network-fully-connected-step-by-step.html)
+
+[![Derivation of CNN from FCNN](https://user-images.githubusercontent.com/16560492/82431369-db176b00-9a8e-11ea-99bd-e845192873fc.png)](https://www.linkedin.com/pulse/derivation-convolutional-neural-network-from-fully-connected-gad)
+
+## Book: Practical Computer Vision Applications Using Deep Learning with CNNs
+
+You can also check my book cited as [**Ahmed Fawzy Gad 'Practical Computer Vision Applications Using Deep Learning with CNNs'. Dec. 2018, Apress, 978-1-4842-4167-7**](https://www.amazon.com/Practical-Computer-Vision-Applications-Learning/dp/1484241665) which discusses neural networks, convolutional neural networks, deep learning, genetic algorithm, and more.
+
+Find the book at these links:
+
+- [Amazon](https://www.amazon.com/Practical-Computer-Vision-Applications-Learning/dp/1484241665)
+- [Springer](https://link.springer.com/book/10.1007/978-1-4842-4167-7)
+- [Apress](https://www.apress.com/gp/book/9781484241660)
+- [O'Reilly](https://www.oreilly.com/library/view/practical-computer-vision/9781484241677)
+- [Google Books](https://books.google.com.eg/books?id=xLd9DwAAQBAJ)
+
+![Fig04](https://user-images.githubusercontent.com/16560492/78830077-ae7c2800-79e7-11ea-980b-53b6bd879eeb.jpg)
+
+# Citing PyGAD - Bibtex Formatted Citation
+
+If you used PyGAD, please consider adding a citation to the following paper about PyGAD:
+
+```
+@misc{gad2021pygad,
+      title={PyGAD: An Intuitive Genetic Algorithm Python Library}, 
+      author={Ahmed Fawzy Gad},
+      year={2021},
+      eprint={2106.06158},
+      archivePrefix={arXiv},
+      primaryClass={cs.NE}
+}
+```
+
+# Contact Us
+
+* E-mail: ahmed.f.gad@gmail.com
+* [LinkedIn](https://www.linkedin.com/in/ahmedfgad)
+* [Paperspace](https://blog.paperspace.com/author/ahmed)
+* [KDnuggets](https://kdnuggets.com/author/ahmed-gad)
+* [TowardsDataScience](https://towardsdatascience.com/@ahmedfgad)
+* [GitHub](https://github.com/ahmedfgad)
```

### Comparing `pygad-3.0.1/setup.py` & `pygad-3.1.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import setuptools  
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(  
     name="pygad",  
-    version="3.0.1",  
+    version="3.1.0",  
     author="Ahmed Fawzy Gad",
-    install_requires=["numpy", "matplotlib","cloudpickle",],
+    install_requires=["numpy", "matplotlib", "cloudpickle",],
     author_email="ahmed.f.gad@gmail.com",  
-    description="PyGAD: A Python 3 Library for Building the Genetic Algorithm and Training Machine Learning Algoithms (Keras & PyTorch).",
+    description="PyGAD: A Python Library for Building the Genetic Algorithm and Training Machine Learning Algoithms (Keras & PyTorch).",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ahmedfgad/GeneticAlgorithmPython",
     packages=setuptools.find_packages())
```

