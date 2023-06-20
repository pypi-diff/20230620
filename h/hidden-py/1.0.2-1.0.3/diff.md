# Comparing `tmp/hidden-py-1.0.2.tar.gz` & `tmp/hidden-py-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hidden-py-1.0.2.tar", last modified: Tue Jun 20 19:10:06 2023, max compression
+gzip compressed data, was "hidden-py-1.0.3.tar", last modified: Tue Jun 20 19:18:42 2023, max compression
```

## Comparing `hidden-py-1.0.2.tar` & `hidden-py-1.0.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 19:10:06.898041 hidden-py-1.0.2/
--rw-rw-rw-   0        0        0     1088 2023-04-19 15:14:57.000000 hidden-py-1.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0    11150 2023-06-20 19:10:06.898041 hidden-py-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    10445 2023-06-20 19:09:10.000000 hidden-py-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 19:10:06.870072 hidden-py-1.0.2/hidden_py/
--rw-rw-rw-   0        0        0        0 2023-06-20 18:29:03.000000 hidden-py-1.0.2/hidden_py/__init__.py
--rw-rw-rw-   0        0        0     5692 2023-06-20 18:29:03.000000 hidden-py-1.0.2/hidden_py/dynamics.py
-drwxrwxrwx   0        0        0        0 2023-06-20 19:10:06.879042 hidden-py-1.0.2/hidden_py/filters/
--rw-rw-rw-   0        0        0        0 2023-06-20 18:29:03.000000 hidden-py-1.0.2/hidden_py/filters/__init__.py
--rw-rw-rw-   0        0        0     9542 2023-06-20 18:29:03.000000 hidden-py-1.0.2/hidden_py/filters/bayesian.py
--rw-rw-rw-   0        0        0    11766 2023-06-20 18:29:03.000000 hidden-py-1.0.2/hidden_py/infer.py
-drwxrwxrwx   0        0        0        0 2023-06-20 19:10:06.890042 hidden-py-1.0.2/hidden_py/optimize/
--rw-rw-rw-   0        0        0        0 2023-06-20 18:29:03.000000 hidden-py-1.0.2/hidden_py/optimize/__init__.py
--rw-rw-rw-   0        0        0    11671 2023-06-20 18:29:03.000000 hidden-py-1.0.2/hidden_py/optimize/base.py
--rw-rw-rw-   0        0        0      183 2023-06-20 18:29:03.000000 hidden-py-1.0.2/hidden_py/optimize/config.py
--rw-rw-rw-   0        0        0    19953 2023-06-20 18:29:03.000000 hidden-py-1.0.2/hidden_py/optimize/optimization.py
--rw-rw-rw-   0        0        0      289 2023-06-20 18:29:03.000000 hidden-py-1.0.2/hidden_py/optimize/registry.py
--rw-rw-rw-   0        0        0     2395 2023-06-20 18:29:03.000000 hidden-py-1.0.2/hidden_py/optimize/results.py
--rw-rw-rw-   0        0        0        0 2023-06-20 18:29:03.000000 hidden-py-1.0.2/hidden_py/optimize/types.py
-drwxrwxrwx   0        0        0        0 2023-06-20 19:10:06.877040 hidden-py-1.0.2/hidden_py.egg-info/
--rw-rw-rw-   0        0        0    11150 2023-06-20 19:10:06.000000 hidden-py-1.0.2/hidden_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      623 2023-06-20 19:10:06.000000 hidden-py-1.0.2/hidden_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 19:10:06.000000 hidden-py-1.0.2/hidden_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-20 19:10:06.000000 hidden-py-1.0.2/hidden_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-20 19:10:06.000000 hidden-py-1.0.2/hidden_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-20 19:10:06.898041 hidden-py-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1162 2023-06-20 19:09:37.000000 hidden-py-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-20 19:10:06.895041 hidden-py-1.0.2/tests/
--rw-rw-rw-   0        0        0     3808 2023-06-20 18:29:03.000000 hidden-py-1.0.2/tests/test_dynamics.py
--rw-rw-rw-   0        0        0    11048 2023-06-20 18:29:03.000000 hidden-py-1.0.2/tests/test_filters.py
--rw-rw-rw-   0        0        0     5943 2023-06-20 18:29:03.000000 hidden-py-1.0.2/tests/test_inferrence.py
--rw-rw-rw-   0        0        0     7823 2023-06-20 18:29:03.000000 hidden-py-1.0.2/tests/test_optimizers.py
+drwxrwxrwx   0        0        0        0 2023-06-20 19:18:42.231190 hidden-py-1.0.3/
+-rw-rw-rw-   0        0        0     1088 2023-04-19 15:14:57.000000 hidden-py-1.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0    11168 2023-06-20 19:18:42.230191 hidden-py-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0    10463 2023-06-20 19:14:58.000000 hidden-py-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 19:18:42.203190 hidden-py-1.0.3/hidden_py/
+-rw-rw-rw-   0        0        0        0 2023-06-20 18:29:03.000000 hidden-py-1.0.3/hidden_py/__init__.py
+-rw-rw-rw-   0        0        0     5692 2023-06-20 18:29:03.000000 hidden-py-1.0.3/hidden_py/dynamics.py
+drwxrwxrwx   0        0        0        0 2023-06-20 19:18:42.212190 hidden-py-1.0.3/hidden_py/filters/
+-rw-rw-rw-   0        0        0        0 2023-06-20 18:29:03.000000 hidden-py-1.0.3/hidden_py/filters/__init__.py
+-rw-rw-rw-   0        0        0     9542 2023-06-20 18:29:03.000000 hidden-py-1.0.3/hidden_py/filters/bayesian.py
+-rw-rw-rw-   0        0        0    11766 2023-06-20 18:29:03.000000 hidden-py-1.0.3/hidden_py/infer.py
+drwxrwxrwx   0        0        0        0 2023-06-20 19:18:42.223191 hidden-py-1.0.3/hidden_py/optimize/
+-rw-rw-rw-   0        0        0        0 2023-06-20 18:29:03.000000 hidden-py-1.0.3/hidden_py/optimize/__init__.py
+-rw-rw-rw-   0        0        0    11671 2023-06-20 18:29:03.000000 hidden-py-1.0.3/hidden_py/optimize/base.py
+-rw-rw-rw-   0        0        0      183 2023-06-20 18:29:03.000000 hidden-py-1.0.3/hidden_py/optimize/config.py
+-rw-rw-rw-   0        0        0    19953 2023-06-20 18:29:03.000000 hidden-py-1.0.3/hidden_py/optimize/optimization.py
+-rw-rw-rw-   0        0        0      289 2023-06-20 18:29:03.000000 hidden-py-1.0.3/hidden_py/optimize/registry.py
+-rw-rw-rw-   0        0        0     2395 2023-06-20 18:29:03.000000 hidden-py-1.0.3/hidden_py/optimize/results.py
+-rw-rw-rw-   0        0        0        0 2023-06-20 18:29:03.000000 hidden-py-1.0.3/hidden_py/optimize/types.py
+drwxrwxrwx   0        0        0        0 2023-06-20 19:18:42.210191 hidden-py-1.0.3/hidden_py.egg-info/
+-rw-rw-rw-   0        0        0    11168 2023-06-20 19:18:42.000000 hidden-py-1.0.3/hidden_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      623 2023-06-20 19:18:42.000000 hidden-py-1.0.3/hidden_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 19:18:42.000000 hidden-py-1.0.3/hidden_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-20 19:18:42.000000 hidden-py-1.0.3/hidden_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-20 19:18:42.000000 hidden-py-1.0.3/hidden_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 19:18:42.231190 hidden-py-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1162 2023-06-20 19:18:00.000000 hidden-py-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 19:18:42.228192 hidden-py-1.0.3/tests/
+-rw-rw-rw-   0        0        0     3808 2023-06-20 18:29:03.000000 hidden-py-1.0.3/tests/test_dynamics.py
+-rw-rw-rw-   0        0        0    11048 2023-06-20 18:29:03.000000 hidden-py-1.0.3/tests/test_filters.py
+-rw-rw-rw-   0        0        0     5943 2023-06-20 18:29:03.000000 hidden-py-1.0.3/tests/test_inferrence.py
+-rw-rw-rw-   0        0        0     7823 2023-06-20 18:29:03.000000 hidden-py-1.0.3/tests/test_optimizers.py
```

### Comparing `hidden-py-1.0.2/LICENSE.txt` & `hidden-py-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hidden-py-1.0.2/PKG-INFO` & `hidden-py-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hidden-py
-Version: 1.0.2
+Version: 1.0.3
 Summary: A python package for discrete-output hidden Markov models
 Author: Steven Large
 Author-email: stevelarge7@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/StevenJLarge/hmm
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -46,24 +46,24 @@
 
 ## Hidden Markov Models
 
 Markov Models are a class of stochastic models for characterizing the behaviour of systems that transition between states randomly, with a probability that depends only on the current state of the system (_i.e._ they are memoryless). Because if this simplification, the dynamics on a set of discrete states can be captured entirely by a single matrix, known as the _transition matrix_, $A$, with elements $A_{ij} = p(x_t=i | x_{t-1} = j)$ quantifying the probability that during timestep $t-1 \to t$, the system will transition from state $j\to i$. Because of the normalization of probability, the columns of $A$ are constrained to be equal to unity.
 
 Without any ambiguity in the observed value (_i.e._ the underlying Markov model is directly observed) the system is just a Markov model. The causal diagram of a Markov model is shown in the figure below.
 
-![markov_model](https://github.com/StevenJLarge/hmm/blob/master/public/resources/markov_schematic.png)
+![markov_model](https://github.com/StevenJLarge/hmm/blob/master/public/resources/markov_schematic.png?raw=true)
 
 Here, the state $x_t$ at time $t$ only depends on the state at the previous time $t-1$. As a result the ecolution of a probability distribution over states can be modelled by simply multiplying an initial distribution by the transition matrix, and repeating the process for each time step.  For example, given an initial distribution over states at time 0 and a transition matrix $A$, the probability distribution at time $T$ is
 
 $$ p_{T} = A^T \cdot p_0 $$
 
 
 A hidden Markov model (HMM), on the other hand, is a probabilistic function of a Markov model. This means that the output of an HMM (th0e observation $y$) is correlated with the underlying (hidden/unobserved) state of the Markov model, but only probabilitsically so. For a set of discrete possible observations (as we capture in this package), the observation process can also be modelled by a matrix (the _observation matrix_) $B$ with elemetnts $B_{ij} = p(y_t = i | x_{t} = j)$ quantifying the probability that our measurement/observation $y_t$ at time $t$ is equal to $i$ given the hidden system is in state $j$. Here, the diagonal elements represent our probability of observing the _correct_ state, while off-diagonals represent the probability of error. In comparison to the figure used in the Markov system, the below diagram shows how causality works in a hidden Markov model.
 
-![midden_markov_model](https://github.com/StevenJLarge/hmm/blob/master/public/resources/hidden_markov_schematic.png)
+![hidden_markov_model](https://github.com/StevenJLarge/hmm/blob/master/public/resources/hidden_markov_schematic.png?raw=true)
 
 Here, the observations ($y_t$) are stochastic (random) functions of the underlying state, but not necessarily equal to it. However (importantly) the observation at time $t$ only depends explicitly on the hiddenstate at time $t$.
 
 --- 
 
 As for the components of the package, the goal of the simulation functionality is simply to generate trajectories of both the hidden state and observation time-series that are conistent with these probabilities. The goal for system identification/parameter fitting is to fit the most likely parameters (elements of the $A$ and $B$) matrices, given only a time series of observations. Finally, the goal if signal processing is to make use of the observation sequence to infer what the hidden state is at a particular point in time.
```

### Comparing `hidden-py-1.0.2/README.md` & `hidden-py-1.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -28,24 +28,24 @@
 
 ## Hidden Markov Models
 
 Markov Models are a class of stochastic models for characterizing the behaviour of systems that transition between states randomly, with a probability that depends only on the current state of the system (_i.e._ they are memoryless). Because if this simplification, the dynamics on a set of discrete states can be captured entirely by a single matrix, known as the _transition matrix_, $A$, with elements $A_{ij} = p(x_t=i | x_{t-1} = j)$ quantifying the probability that during timestep $t-1 \to t$, the system will transition from state $j\to i$. Because of the normalization of probability, the columns of $A$ are constrained to be equal to unity.
 
 Without any ambiguity in the observed value (_i.e._ the underlying Markov model is directly observed) the system is just a Markov model. The causal diagram of a Markov model is shown in the figure below.
 
-![markov_model](https://github.com/StevenJLarge/hmm/blob/master/public/resources/markov_schematic.png)
+![markov_model](https://github.com/StevenJLarge/hmm/blob/master/public/resources/markov_schematic.png?raw=true)
 
 Here, the state $x_t$ at time $t$ only depends on the state at the previous time $t-1$. As a result the ecolution of a probability distribution over states can be modelled by simply multiplying an initial distribution by the transition matrix, and repeating the process for each time step.  For example, given an initial distribution over states at time 0 and a transition matrix $A$, the probability distribution at time $T$ is
 
 $$ p_{T} = A^T \cdot p_0 $$
 
 
 A hidden Markov model (HMM), on the other hand, is a probabilistic function of a Markov model. This means that the output of an HMM (th0e observation $y$) is correlated with the underlying (hidden/unobserved) state of the Markov model, but only probabilitsically so. For a set of discrete possible observations (as we capture in this package), the observation process can also be modelled by a matrix (the _observation matrix_) $B$ with elemetnts $B_{ij} = p(y_t = i | x_{t} = j)$ quantifying the probability that our measurement/observation $y_t$ at time $t$ is equal to $i$ given the hidden system is in state $j$. Here, the diagonal elements represent our probability of observing the _correct_ state, while off-diagonals represent the probability of error. In comparison to the figure used in the Markov system, the below diagram shows how causality works in a hidden Markov model.
 
-![midden_markov_model](https://github.com/StevenJLarge/hmm/blob/master/public/resources/hidden_markov_schematic.png)
+![hidden_markov_model](https://github.com/StevenJLarge/hmm/blob/master/public/resources/hidden_markov_schematic.png?raw=true)
 
 Here, the observations ($y_t$) are stochastic (random) functions of the underlying state, but not necessarily equal to it. However (importantly) the observation at time $t$ only depends explicitly on the hiddenstate at time $t$.
 
 --- 
 
 As for the components of the package, the goal of the simulation functionality is simply to generate trajectories of both the hidden state and observation time-series that are conistent with these probabilities. The goal for system identification/parameter fitting is to fit the most likely parameters (elements of the $A$ and $B$) matrices, given only a time series of observations. Finally, the goal if signal processing is to make use of the observation sequence to infer what the hidden state is at a particular point in time.
```

### Comparing `hidden-py-1.0.2/hidden_py/dynamics.py` & `hidden-py-1.0.3/hidden_py/dynamics.py`

 * *Files identical despite different names*

### Comparing `hidden-py-1.0.2/hidden_py/filters/bayesian.py` & `hidden-py-1.0.3/hidden_py/filters/bayesian.py`

 * *Files identical despite different names*

### Comparing `hidden-py-1.0.2/hidden_py/infer.py` & `hidden-py-1.0.3/hidden_py/infer.py`

 * *Files identical despite different names*

### Comparing `hidden-py-1.0.2/hidden_py/optimize/base.py` & `hidden-py-1.0.3/hidden_py/optimize/base.py`

 * *Files identical despite different names*

### Comparing `hidden-py-1.0.2/hidden_py/optimize/optimization.py` & `hidden-py-1.0.3/hidden_py/optimize/optimization.py`

 * *Files identical despite different names*

### Comparing `hidden-py-1.0.2/hidden_py/optimize/results.py` & `hidden-py-1.0.3/hidden_py/optimize/results.py`

 * *Files identical despite different names*

### Comparing `hidden-py-1.0.2/hidden_py.egg-info/PKG-INFO` & `hidden-py-1.0.3/hidden_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hidden-py
-Version: 1.0.2
+Version: 1.0.3
 Summary: A python package for discrete-output hidden Markov models
 Author: Steven Large
 Author-email: stevelarge7@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/StevenJLarge/hmm
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -46,24 +46,24 @@
 
 ## Hidden Markov Models
 
 Markov Models are a class of stochastic models for characterizing the behaviour of systems that transition between states randomly, with a probability that depends only on the current state of the system (_i.e._ they are memoryless). Because if this simplification, the dynamics on a set of discrete states can be captured entirely by a single matrix, known as the _transition matrix_, $A$, with elements $A_{ij} = p(x_t=i | x_{t-1} = j)$ quantifying the probability that during timestep $t-1 \to t$, the system will transition from state $j\to i$. Because of the normalization of probability, the columns of $A$ are constrained to be equal to unity.
 
 Without any ambiguity in the observed value (_i.e._ the underlying Markov model is directly observed) the system is just a Markov model. The causal diagram of a Markov model is shown in the figure below.
 
-![markov_model](https://github.com/StevenJLarge/hmm/blob/master/public/resources/markov_schematic.png)
+![markov_model](https://github.com/StevenJLarge/hmm/blob/master/public/resources/markov_schematic.png?raw=true)
 
 Here, the state $x_t$ at time $t$ only depends on the state at the previous time $t-1$. As a result the ecolution of a probability distribution over states can be modelled by simply multiplying an initial distribution by the transition matrix, and repeating the process for each time step.  For example, given an initial distribution over states at time 0 and a transition matrix $A$, the probability distribution at time $T$ is
 
 $$ p_{T} = A^T \cdot p_0 $$
 
 
 A hidden Markov model (HMM), on the other hand, is a probabilistic function of a Markov model. This means that the output of an HMM (th0e observation $y$) is correlated with the underlying (hidden/unobserved) state of the Markov model, but only probabilitsically so. For a set of discrete possible observations (as we capture in this package), the observation process can also be modelled by a matrix (the _observation matrix_) $B$ with elemetnts $B_{ij} = p(y_t = i | x_{t} = j)$ quantifying the probability that our measurement/observation $y_t$ at time $t$ is equal to $i$ given the hidden system is in state $j$. Here, the diagonal elements represent our probability of observing the _correct_ state, while off-diagonals represent the probability of error. In comparison to the figure used in the Markov system, the below diagram shows how causality works in a hidden Markov model.
 
-![midden_markov_model](https://github.com/StevenJLarge/hmm/blob/master/public/resources/hidden_markov_schematic.png)
+![hidden_markov_model](https://github.com/StevenJLarge/hmm/blob/master/public/resources/hidden_markov_schematic.png?raw=true)
 
 Here, the observations ($y_t$) are stochastic (random) functions of the underlying state, but not necessarily equal to it. However (importantly) the observation at time $t$ only depends explicitly on the hiddenstate at time $t$.
 
 --- 
 
 As for the components of the package, the goal of the simulation functionality is simply to generate trajectories of both the hidden state and observation time-series that are conistent with these probabilities. The goal for system identification/parameter fitting is to fit the most likely parameters (elements of the $A$ and $B$) matrices, given only a time series of observations. Finally, the goal if signal processing is to make use of the observation sequence to infer what the hidden state is at a particular point in time.
```

### Comparing `hidden-py-1.0.2/hidden_py.egg-info/SOURCES.txt` & `hidden-py-1.0.3/hidden_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hidden-py-1.0.2/setup.py` & `hidden-py-1.0.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # README contents
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='hidden-py',
     packages=find_packages(),
-    version="1.0.2",
+    version="1.0.3",
     long_description=long_description,
     long_description_content_type='text/markdown',
     description='''
         A python package for discrete-output hidden Markov models
     ''',
     author='Steven Large',
     author_email='stevelarge7@gmail.com',
```

### Comparing `hidden-py-1.0.2/tests/test_dynamics.py` & `hidden-py-1.0.3/tests/test_dynamics.py`

 * *Files identical despite different names*

### Comparing `hidden-py-1.0.2/tests/test_filters.py` & `hidden-py-1.0.3/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `hidden-py-1.0.2/tests/test_inferrence.py` & `hidden-py-1.0.3/tests/test_inferrence.py`

 * *Files identical despite different names*

### Comparing `hidden-py-1.0.2/tests/test_optimizers.py` & `hidden-py-1.0.3/tests/test_optimizers.py`

 * *Files identical despite different names*

