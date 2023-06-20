# Comparing `tmp/mellon-1.2.0.tar.gz` & `tmp/mellon-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mellon-1.2.0.tar", last modified: Fri Apr  7 00:19:43 2023, max compression
+gzip compressed data, was "mellon-1.3.0.tar", last modified: Tue Jun 20 18:58:45 2023, max compression
```

## Comparing `mellon-1.2.0.tar` & `mellon-1.3.0.tar`

### file list

```diff
@@ -1,23 +1,37 @@
-drwxrws---   0 dotto    (71780) setty_m_grp (239268)        0 2023-04-07 00:19:43.590659 mellon-1.2.0/
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)    35148 2022-09-23 00:29:04.000000 mellon-1.2.0/LICENSE
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)     1767 2023-04-07 00:19:43.587915 mellon-1.2.0/PKG-INFO
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)     1347 2023-03-28 23:01:29.000000 mellon-1.2.0/README.rst
-drwxrws---   0 dotto    (71780) setty_m_grp (239268)        0 2023-04-07 00:19:43.560958 mellon-1.2.0/mellon/
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)     1051 2023-04-07 00:12:22.000000 mellon-1.2.0/mellon/__init__.py
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)     1897 2023-04-01 02:53:36.000000 mellon-1.2.0/mellon/base_cov.py
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)     7231 2023-03-31 23:12:47.000000 mellon-1.2.0/mellon/conditional.py
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)     2481 2023-03-25 01:09:57.000000 mellon-1.2.0/mellon/cov.py
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)     9200 2023-04-01 02:53:25.000000 mellon-1.2.0/mellon/decomposition.py
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)     2389 2022-12-06 00:00:08.000000 mellon-1.2.0/mellon/derivatives.py
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)    14318 2023-04-03 23:17:39.000000 mellon-1.2.0/mellon/inference.py
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)    57914 2023-04-06 22:16:53.000000 mellon-1.2.0/mellon/model.py
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)     9222 2023-04-03 18:53:33.000000 mellon-1.2.0/mellon/parameters.py
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)     4546 2023-04-02 21:34:32.000000 mellon-1.2.0/mellon/util.py
-drwxrws---   0 dotto    (71780) setty_m_grp (239268)        0 2023-04-07 00:19:43.582831 mellon-1.2.0/mellon.egg-info/
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)     1767 2023-04-07 00:19:43.000000 mellon-1.2.0/mellon.egg-info/PKG-INFO
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)      368 2023-04-07 00:19:43.000000 mellon-1.2.0/mellon.egg-info/SOURCES.txt
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)        1 2023-04-07 00:19:43.000000 mellon-1.2.0/mellon.egg-info/dependency_links.txt
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)       24 2023-04-07 00:19:43.000000 mellon-1.2.0/mellon.egg-info/requires.txt
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)        7 2023-04-07 00:19:43.000000 mellon-1.2.0/mellon.egg-info/top_level.txt
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)       38 2023-04-07 00:19:43.592374 mellon-1.2.0/setup.cfg
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)     1100 2023-03-25 00:23:30.000000 mellon-1.2.0/setup.py
+drwxrws---   0 dotto    (71780) setty_m_grp (239268)        0 2023-06-20 18:58:45.574584 mellon-1.3.0/
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)    35148 2022-09-23 00:29:04.000000 mellon-1.3.0/LICENSE
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)     2586 2023-06-20 18:58:45.573214 mellon-1.3.0/PKG-INFO
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)     2166 2023-05-17 21:27:55.000000 mellon-1.3.0/README.rst
+drwxrws---   0 dotto    (71780) setty_m_grp (239268)        0 2023-06-20 18:58:45.552487 mellon-1.3.0/mellon/
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)      961 2023-06-20 18:33:48.000000 mellon-1.3.0/mellon/__init__.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)      452 2023-06-17 22:03:44.000000 mellon-1.3.0/mellon/_conditional.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)      290 2023-06-17 22:06:30.000000 mellon-1.3.0/mellon/_cov.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)      196 2023-06-17 22:01:57.000000 mellon-1.3.0/mellon/_derivatives.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)      898 2023-06-17 21:58:49.000000 mellon-1.3.0/mellon/_inference.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)      711 2023-06-17 21:44:25.000000 mellon-1.3.0/mellon/_parameters.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)      235 2023-06-17 21:48:14.000000 mellon-1.3.0/mellon/_util.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)     8960 2023-06-17 21:51:01.000000 mellon-1.3.0/mellon/base_cov.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)    12053 2023-06-16 02:26:14.000000 mellon-1.3.0/mellon/base_model.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)    19174 2023-06-17 22:03:30.000000 mellon-1.3.0/mellon/base_predictor.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)     3679 2023-06-16 05:31:47.000000 mellon-1.3.0/mellon/compute_ls_time.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)     7453 2023-06-17 21:51:59.000000 mellon-1.3.0/mellon/conditional.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)     9028 2023-06-17 21:50:46.000000 mellon-1.3.0/mellon/cov.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)     9199 2023-06-16 02:26:11.000000 mellon-1.3.0/mellon/decomposition.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)    17357 2023-06-16 02:26:11.000000 mellon-1.3.0/mellon/density_estimator.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)     4360 2023-06-16 18:57:29.000000 mellon-1.3.0/mellon/derivatives.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)    19510 2023-06-16 02:26:11.000000 mellon-1.3.0/mellon/dimensionality_estimator.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)    13774 2023-06-16 02:26:11.000000 mellon-1.3.0/mellon/function_estimator.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)    19432 2023-06-17 21:52:29.000000 mellon-1.3.0/mellon/inference.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)      368 2023-06-16 02:26:11.000000 mellon-1.3.0/mellon/model.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)    16164 2023-06-17 21:52:14.000000 mellon-1.3.0/mellon/parameters.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)    24211 2023-06-17 07:12:35.000000 mellon-1.3.0/mellon/time_sensitive_density_estimator.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)    12525 2023-06-17 21:52:36.000000 mellon-1.3.0/mellon/util.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)     9661 2023-06-17 22:04:30.000000 mellon-1.3.0/mellon/validation.py
+drwxrws---   0 dotto    (71780) setty_m_grp (239268)        0 2023-06-20 18:58:45.569512 mellon-1.3.0/mellon.egg-info/
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)     2586 2023-06-20 18:58:45.000000 mellon-1.3.0/mellon.egg-info/PKG-INFO
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)      716 2023-06-20 18:58:45.000000 mellon-1.3.0/mellon.egg-info/SOURCES.txt
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)        1 2023-06-20 18:58:45.000000 mellon-1.3.0/mellon.egg-info/dependency_links.txt
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)       24 2023-06-20 18:58:45.000000 mellon-1.3.0/mellon.egg-info/requires.txt
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)        7 2023-06-20 18:58:45.000000 mellon-1.3.0/mellon.egg-info/top_level.txt
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)       38 2023-06-20 18:58:45.575395 mellon-1.3.0/setup.cfg
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)     1100 2023-06-15 06:16:23.000000 mellon-1.3.0/setup.py
```

### Comparing `mellon-1.2.0/LICENSE` & `mellon-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mellon-1.2.0/PKG-INFO` & `mellon-1.3.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,65 @@
 Metadata-Version: 2.1
 Name: mellon
-Version: 1.2.0
+Version: 1.3.0
 Summary: Non-parametric density estimator.
 Home-page: https://github.com/settylab/mellon
 Author: Setty Lab
 Author-email: msetty@fredhutch.org
 License: GNU General Public License v3.0
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
+Mellon
+======
+
 .. image:: https://zenodo.org/badge/558998366.svg
    :target: https://zenodo.org/badge/latestdoi/558998366
 .. image:: https://codecov.io/github/settylab/Mellon/branch/main/graph/badge.svg?token=TKIKXK4MPG 
     :target: https://app.codecov.io/github/settylab/Mellon
+.. image:: https://www.codefactor.io/repository/github/settylab/mellon/badge/main
+      :target: https://www.codefactor.io/repository/github/settylab/mellon/overview/main
+      :alt: CodeFactor
 .. image:: https://badge.fury.io/py/mellon.svg
        :target: https://badge.fury.io/py/mellon
+.. image:: https://anaconda.org/conda-forge/mellon/badges/version.svg
+       :target: https://anaconda.org/conda-forge/mellon
 .. image:: https://static.pepy.tech/personalized-badge/mellon?period=total&units=international_system&left_color=grey&right_color=lightgrey&left_text=Downloads
     :target: https://pepy.tech/project/mellon
 
-Mellon is a non-parametric density estimator based on the NearestNeighbors distribution.
+.. image:: https://github.com/settylab/mellon/raw/main/landscape.png?raw=true
+   :target: https://github.com/settylab/Mellon
+
+Mellon is a non-parametric cell-state density estimator based on a
+nearest-neighbors-distance distribution. It uses a sparse gaussian process
+to produce a differntiable density function that can be evaluated out of sample.
 
 Installation
 ============
 
-To install with pip you can run:
+To install Mellon using **pip** you can run:
 
 .. code-block:: bash
 
    pip install mellon
 
+or to install using **conda** you can run:
+
+.. code-block:: bash
+
+   conda install -c conda-forge mellon
+
+or to install using **mamba** you can run:
+
+.. code-block:: bash
+
+   mamba install -c conda-forge mellon
+
 Documentation
 =============
 
 Please read the
 `documentation <https://mellon.readthedocs.io/en/latest/index.html>`_
 or use this
 `basic tutorial notebook <https://github.com/settylab/Mellon/blob/main/notebooks/basic_tutorial.ipynb>`_.
```

### Comparing `mellon-1.2.0/mellon/__init__.py` & `mellon-1.3.0/mellon/_inference.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,35 @@
-from jax.config import config as jaxconfig
-
-jaxconfig.update("jax_enable_x64", True)
-jaxconfig.update("jax_platform_name", "cpu")
-
-__version__ = "1.2.0"
-
-from .base_cov import Covariance
-from .util import stabilize, mle, distance, Log, local_dimensionality
-from .cov import Matern32, Matern52, ExpQuad, Exponential, RatQuad
 from .inference import (
     compute_transform,
     compute_dimensionality_transform,
     compute_loss_func,
     compute_dimensionality_loss_func,
     minimize_adam,
     minimize_lbfgsb,
     compute_log_density_x,
     compute_conditional_mean,
+    compute_conditional_mean_times,
     compute_conditional_mean_explog,
+    generate_gaussian_sample,
+    calculate_gaussian_logpdf,
+    calculate_elbo,
+    calculate_batch_elbo,
+    run_advi,
 )
-from .parameters import (
-    compute_landmarks,
-    k_means,
-    compute_nn_distances,
-    compute_distances,
-    compute_d,
-    compute_mu,
-    compute_ls,
-    compute_cov_func,
-    compute_L,
-    compute_initial_value,
-    compute_initial_dimensionalities,
-)
-from .derivatives import (
-    gradient,
-    hessian,
-    hessian_log_determinant,
-)
-from .model import (
-    DensityEstimator,
-    FunctionEstimator,
-    DimensionalityEstimator,
-)
+
+__all__ = [
+    "compute_transform",
+    "compute_dimensionality_transform",
+    "compute_loss_func",
+    "compute_dimensionality_loss_func",
+    "minimize_adam",
+    "minimize_lbfgsb",
+    "compute_log_density_x",
+    "compute_conditional_mean",
+    "compute_conditional_mean_times",
+    "compute_conditional_mean_explog",
+    "generate_gaussian_sample",
+    "calculate_gaussian_logpdf",
+    "calculate_elbo",
+    "calculate_batch_elbo",
+    "run_advi",
+]
```

### Comparing `mellon-1.2.0/mellon/decomposition.py` & `mellon-1.3.0/mellon/decomposition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from jax.numpy import cumsum, searchsorted, count_nonzero, sqrt, isnan, any
 from jax.numpy.linalg import eigh, cholesky, qr
 from jax.scipy.linalg import solve_triangular
 from .util import stabilize, DEFAULT_JITTER, Log
 
 
-DEFAULT_RANK = 0.99
+DEFAULT_RANK = 1.0
 DEFAULT_METHOD = "auto"
 
 logger = Log()
 
 
 def _check_method(rank, full, method):
     R"""
```

### Comparing `mellon-1.2.0/mellon/inference.py` & `mellon-1.3.0/mellon/inference.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 from collections import namedtuple
-from jax.numpy import log, pi, exp, stack, arange, median, sort, max
+from functools import partial
+from jax import random, vmap
+from jax.numpy import log, pi, exp, stack, arange, sort, mean, zeros_like
 from jax.numpy import sum as arraysum
 from jax.scipy.special import gammaln
+import jax.scipy.stats.norm as norm
 import jax
 from jax.example_libraries.optimizers import adam
 from jaxopt import ScipyMinimize
 from .conditional import (
-    _full_conditional_mean,
-    _full_conditional_mean_y,
-    _landmarks_conditional_mean,
-    _landmarks_conditional_mean_y,
+    FullConditionalMean,
+    FullConditionalMeanTime,
+    LandmarksConditionalMean,
+    LandmarksConditionalMeanTime,
+    LandmarksConditionalMeanCholesky,
+    LandmarksConditionalMeanCholeskyTime,
 )
-from .util import DEFAULT_JITTER
+from .util import ensure_2d, Exp, DEFAULT_JITTER
 
 
 DEFAULT_N_ITER = 100
-DEFAULT_INIT_LEARN_RATE = 1
+DEFAULT_INIT_LEARN_RATE = 1e-1
+DEFAULT_NUM_SAMPLES = 40
 DEFAULT_OPTIMIZER = "L-BFGS-B"
 DEFAULT_JIT = False
 
 
 def _normal(k):
     R"""
     Builds the log pdf of :math:`z \sim \text{Normal}(0, I)`.
@@ -34,22 +40,22 @@
         return -(1 / 2) * arraysum(z**2) - (k / 2) * log(2 * pi)
 
     return logpdf
 
 
 def _multivariate(mu, L):
     R"""
-    Builds the transformation function from :math:`z \sim \text{Normal}(0, I)
-    \rightarrow f \sim \text{Normal}(mu, K')`, where :math:`I` is the identity matrix
+    Builds the transformation function from
+    :math:`z \sim \text{Normal}(0, I) \rightarrow f \sim \text{Normal}(\mu, K')`,
+    where :math:`I` is the identity matrix
     and :math:`K \approx K' = L L^\top`.
 
-    :param mu: The Gaussian process mean.
+    :param mu: The Gaussian process mean :math:`\mu`.
     :type mu: float
-    :param L: A matrix such that :math:`L L^\top
-    \approx K`.
+    :param L: A matrix such that :math:`L L^\top \approx K`.
     :type L: array-like
     :return: A function :math:`z \rightarrow f`.
     :rtype: function
     """
 
     def transform(z):
         return L.dot(z) + mu
@@ -109,36 +115,36 @@
 
     return logpdf
 
 
 def compute_transform(mu, L):
     R"""
     Computes a function transform that maps :math:`z \sim
-    \text{Normal}(0, I) \rightarrow f \sim \text{Normal}(mu, K')`,
+    \text{Normal}(0, I) \rightarrow f \sim \text{Normal}(\mu, K')`,
     where :math:`I` is the identity matrix and :math:`K \approx K' = L L^\top`,
     where :math:`K` is the covariance matrix.
 
-    :param mu: The Gaussian process mean.
+    :param mu: The Gaussian process mean:math:`\mu`.
     :type mu: float
     :param L: A matrix such that :math:`L L^\top \approx K`, where :math:`K` is the
         covariance matrix.
     :type L: array-like
     :return: transform - The transform function :math:`z \rightarrow f`.
     """
     return _multivariate(mu, L)
 
 
 def compute_dimensionality_transform(mu_dim, mu_dens, L):
     R"""
     Computes a function transform that maps :math:`z \sim
-    \text{Normal}(0, I) \rightarrow \log(f) \sim \text{Normal}(mu, K')`,
+    \text{Normal}(0, I) \rightarrow \log(f) \sim \text{Normal}(\mu, K')`,
     where :math:`I` is the identity matrix and :math:`K \approx K' = L L^\top`,
     where :math:`K` is the covariance matrix.
 
-    :param mu: The Gaussian process mean.
+    :param mu: The Gaussian process mean :math:`\mu`.
     :type mu: float
     :param L: A matrix such that :math:`L L^\top \approx K`, where :math:`K` is the
         covariance matrix.
     :type L: array-like
     :return: transform - The transform function :math:`z \rightarrow f`.
     """
 
@@ -158,15 +164,15 @@
     likelihood(transform(:math:`z`))).
 
     :param nn_distances: The observed nearest neighbor distances.
     :type nn_distances: array-like
     :param d: The dimensionality of the data.
     :type d: int
     :param transform:
-        Maps :math:`z \sim \text{Normal}(0, I) \rightarrow f \sim \text{Normal}(mu, K')`,
+        Maps :math:`z \sim \text{Normal}(0, I) \rightarrow f \sim \text{Normal}(\mu, K')`,
         where :math:`I` is the identity matrix and :math:`K \approx K' = L L^\top`,
         where :math:`K` is the covariance matrix.
     :type transform: function
     :param k: dimension of transform input
     :type k: int
     :return: loss_func - The Bayesian loss function
     :rtype: function, function
@@ -184,15 +190,15 @@
     R"""
     Computes the Bayesian loss function -(prior(:math:`z`) +
     likelihood(transform(:math:`z`))) for dimensionality inference.
 
     :param distances: The observed k nearest neighbor distances.
     :type distances: array-like
     :param transform:
-        Maps :math:`z \sim \text{Normal}(0, I) \rightarrow \log(f) \sim \text{Normal}(mu, K')`,
+        Maps :math:`z \sim \text{Normal}(0, I) \rightarrow \log(f) \sim \text{Normal}(\mu, K')`,
         where :math:`I` is the identity matrix and :math:`K \approx K' = L L^\top`,
         where :math:`K` is the covariance matrix.
     :type transform: function
     :param k: dimension of transform input
     :type k: int
     :return: loss_func - The Bayesian loss function
     :rtype: function, function
@@ -279,67 +285,165 @@
 def compute_log_density_x(pre_transformation, transform):
     R"""
     Computes the log density at the training points.
 
     :param pre_transformation: :math:`z \sim \text{Normal}(0, I)`
     :type pre_transformation: array-like
     :param transform: A function
-        :math:`z \sim \text{Normal}(0, I) \rightarrow f \sim \text{Normal}(mu, K')`,
+        :math:`z \sim \text{Normal}(0, I) \rightarrow f \sim \text{Normal}(\mu, K')`,
         where :math:`I` is the identity matrix and :math:`K \approx K' = L L^\top`,
         where :math:`K` is the covariance matrix.
     :type transform: function
     :return: log_density_x - The log density at the training points.
     """
     return transform(pre_transformation)
 
 
 def compute_conditional_mean(
     x,
     landmarks,
+    pre_transformation,
     y,
     mu,
     cov_func,
     sigma=0,
     jitter=DEFAULT_JITTER,
 ):
     R"""
     Builds the mean function of the Gaussian process, conditioned on the
-    function values (e.g., log-density) on x.
-    Returns a function that is defined on the whole domain of x.
+    function values (e.g., log-density) on x. Returns an instance of
+    mellon.Predictor that acts as a function, defined on the whole domain of x.
 
-    :param x: The training instances.
-    :type x: array-like
-    :param landmarks: The landmark points for fast sparse computation.
+    Parameters
+    ----------
+    x : array-like
+        The training instances.
+    landmarks : array-like or None
+        The landmark points for fast sparse computation.
         Landmarks can be None if not using landmark points.
-    :type landmarks: array-like
-    :param y: The function values at each point in x.
-    :type y: array-like
-    :param mu: The original Gaussian process mean.
-    :type mu: float
-    :param cov_func: The Gaussian process covariance function.
-    :type cov_func: function
-    :param sigma: White moise veriance. Defaults to 0.
-    :type sigma: float
-    :param jitter: A small amount to add to the diagonal for stability. Defaults to 1e-6.
-    :type jitter: float
-    :return: conditional_mean - The conditioned Gaussian process mean function.
-    :rtype: function
+    pre_transformation : array-like or None
+        The pre-transformed latent function representation.
+    y : array-like
+        The function values at each point in x.
+    mu : float
+        The original Gaussian process mean :math:`\mu`.
+    cov_func : function
+        The Gaussian process covariance function.
+    sigma : float, optional
+        White noise variance, by default 0.
+    jitter : float, optional
+        A small amount to add to the diagonal for stability, by default 1e-6.
+
+    Returns
+    -------
+    mellon.Predictor
+        The conditioned Gaussian process mean function.
     """
+
     if landmarks is None:
-        return _full_conditional_mean(
+        return FullConditionalMean(
             x,
             y,
             mu,
             cov_func,
             jitter=jitter,
         )
+    elif (
+        pre_transformation is not None
+        and pre_transformation.shape[0] == landmarks.shape[0]
+    ):
+        landmarks = ensure_2d(landmarks)
+        return LandmarksConditionalMeanCholesky(
+            landmarks,
+            pre_transformation,
+            mu,
+            cov_func,
+            sigma=sigma,
+            jitter=jitter,
+        )
     else:
-        if len(landmarks.shape) < 2:
-            landmarks = landmarks[:, None]
-        return _landmarks_conditional_mean(
+        landmarks = ensure_2d(landmarks)
+        return LandmarksConditionalMean(
+            x,
+            landmarks,
+            y,
+            mu,
+            cov_func,
+            sigma=sigma,
+            jitter=jitter,
+        )
+
+
+def compute_conditional_mean_times(
+    x,
+    landmarks,
+    pre_transformation,
+    y,
+    mu,
+    cov_func,
+    sigma=0,
+    jitter=DEFAULT_JITTER,
+):
+    R"""
+    Builds the mean function of the Gaussian process, conditioned on the
+    function values (e.g., log-density) on x, taking into account the associated
+    times of each sample. Returns an instance of mellon.Predictor that acts as a
+    function, defined on the whole domain of x, and can be evaluated at any given time.
+
+    Parameters
+    ----------
+    x : array-like
+        The training instances.
+    landmarks : array-like or None
+        The landmark points for fast sparse computation.
+        Landmarks can be None if not using landmark points.
+    pre_transformation : array-like or None
+        The pre-transformed latent function representation.
+    y : array-like
+        The function values at each point in x.
+    mu : float
+        The original Gaussian process mean :math:`\mu`.
+    cov_func : function
+        The Gaussian process covariance function.
+    sigma : float, optional
+        White noise variance, by default 0.
+    jitter : float, optional
+        A small amount to add to the diagonal for stability, by default 1e-6.
+
+    Returns
+    -------
+    mellon.Predictor
+        The conditioned Gaussian process mean function that also accepts a 'times'
+        argument to account for time-sensitive inferences.
+    """
+
+    if landmarks is None:
+        return FullConditionalMeanTime(
+            x,
+            y,
+            mu,
+            cov_func,
+            jitter=jitter,
+        )
+    elif (
+        pre_transformation is not None
+        and pre_transformation.shape[0] == landmarks.shape[0]
+    ):
+        landmarks = ensure_2d(landmarks)
+        return LandmarksConditionalMeanCholeskyTime(
+            landmarks,
+            pre_transformation,
+            mu,
+            cov_func,
+            sigma=sigma,
+            jitter=jitter,
+        )
+    else:
+        landmarks = ensure_2d(landmarks)
+        return LandmarksConditionalMeanTime(
             x,
             landmarks,
             y,
             mu,
             cov_func,
             sigma=sigma,
             jitter=jitter,
@@ -363,107 +467,151 @@
     :param x: The training instances.
     :type x: array-like
     :param landmarks: The landmark points for fast sparse computation.
         Landmarks can be None if not using landmark points.
     :type landmarks: array-like
     :param y: The function values at each point in x.
     :type y: array-like
-    :param mu: The original Gaussian process mean.
+    :param mu: The original Gaussian process mean :math:`\mu`.
     :type mu: float
     :param cov_func: The Gaussian process covariance function.
     :type cov_func: function
     :param sigma: White moise veriance. Defaults to 0.
     :type sigma: float
     :param jitter: A small amount to add to the diagonal for stability. Defaults to 1e-6.
     :type jitter: float
     :return: conditional_mean - The conditioned Gaussian process mean function.
     :rtype: function
     """
     if landmarks is None:
         return Exp(
-            _full_conditional_mean(
+            FullConditionalMean(
                 x,
                 log(y),
                 mu,
                 cov_func,
                 jitter=jitter,
             )
         )
     else:
-        if len(landmarks.shape) < 2:
-            landmarks = landmarks[:, None]
+        landmarks = ensure_2d(landmarks)
         return Exp(
-            _landmarks_conditional_mean(
+            LandmarksConditionalMean(
                 x,
                 landmarks,
                 log(y),
                 mu,
                 cov_func,
                 sigma=sigma,
                 jitter=jitter,
             )
         )
 
 
-def compute_conditional_mean_y(
-    x,
-    landmarks,
-    Xnew,
-    mu,
-    cov_func,
-    sigma=0,
-    jitter=DEFAULT_JITTER,
-):
-    R"""
-    Builds the mean function of the Gaussian process, conditioned on the
-    function values (e.g., log-density) on x, and for fixed
-    output locations Xnew and therefor flexible output values y.
+def generate_gaussian_sample(rng, mean, log_std):
+    """
+    Generates a single sample from a multivariate Gaussian with diagonal covariance.
 
-    :param x: The training instances.
-    :type x: array-like
-    :param landmarks: The landmark points for fast sparse computation.
-        Landmarks can be None if not using landmark points.
-    :type landmarks: array-like
-    :param Xnew: The output locations.
-    :type Xnew: array-like
-    :param mu: The original Gaussian process mean.
-    :type mu: float
-    :param cov_func: The Gaussian process covariance function.
-    :type cov_func: function
-    :param sigma: White moise veriance. Defaults to 0.
-    :type sigma: float
-    :param jitter: A small amount to add to the diagonal for stability. Defaults to 1e-6.
-    :type jitter: float
-    :return: conditional_mean - The conditioned Gaussian process mean function.
-    :rtype: function
+    :param rng: random number generator
+    :param mean: mean of the Gaussian distribution
+    :param log_std: logarithm of standard deviation of the Gaussian distribution
+    :return: sample from the Gaussian distribution
     """
-    if landmarks is None:
-        return _full_conditional_mean_y(
-            x,
-            Xnew,
-            mu,
-            cov_func,
-            jitter=jitter,
-        )
-    else:
-        if len(landmarks.shape) < 2:
-            landmarks = landmarks[:, None]
-        return _landmarks_conditional_mean_y(
-            x,
-            landmarks,
-            Xnew,
-            mu,
-            cov_func,
-            sigma=sigma,
-            jitter=jitter,
-        )
+    return mean + exp(log_std) * random.normal(rng, mean.shape)
+
+
+def calculate_gaussian_logpdf(x, mean, log_std):
+    """
+    Calculates the log probability density function of a multivariate Gaussian with diagonal covariance.
+
+    :param x: value to evaluate the Gaussian on
+    :param mean: mean of the Gaussian distribution
+    :param log_std: logarithm of standard deviation of the Gaussian distribution
+    :return: log pdf of the Gaussian distribution
+    """
+    return arraysum(vmap(norm.logpdf)(x, mean, exp(log_std)))
 
 
-def Exp(func):
+def calculate_elbo(logprob, rng, mean, log_std):
+    """
+    Calculates the single-sample Monte Carlo estimate of the variational lower bound (ELBO).
+
+    :param logprob: log probability of the sample
+    :param rng: random number generator
+    :param mean: mean of the Gaussian distribution
+    :param log_std: logarithm of standard deviation of the Gaussian distribution
+    :return: ELBO estimate
     """
-    Function wrapper, making a function that returns the exponent of the wrapped function.
+    sample = generate_gaussian_sample(rng, mean, log_std)
+    return logprob(sample) - calculate_gaussian_logpdf(sample, mean, log_std)
+
+
+def calculate_batch_elbo(logprob, rng, params, num_samples):
+    """
+    Calculates the average ELBO over a batch of random samples.
+
+    :param logprob: log probability of the sample
+    :param rng: random number generator key
+    :param params: parameters of the Gaussian distribution
+    :param num_samples: number of samples in the batch
+    :return: batch ELBO
+    """
+    rngs = random.split(rng, num_samples)
+    vectorized_elbo = vmap(partial(calculate_elbo, logprob), in_axes=(0, None, None))
+    return mean(vectorized_elbo(rngs, *params))
+
+
+def run_advi(
+    loss_func,
+    initial_parameters,
+    n_iter=DEFAULT_N_ITER,
+    init_learn_rate=DEFAULT_INIT_LEARN_RATE,
+    nsamples=DEFAULT_NUM_SAMPLES,
+    jit=DEFAULT_JIT,
+):
     """
+    Performs automatic differentiation variational inference (ADVI) to fit a
+    Gaussian approximation to an intractable, unnormalized density.
+
+    :param loss_func: function to calculate the loss
+    :param initial_parameters: initial parameters for the optimization
+    :param n_iter: number of iterations for the optimization (default: DEFAULT_N_ITER)
+    :param init_learn_rate: The initial learn rate. Defaults to 1.
+    :type init_learn_rate: float
+    :return: parameters, standard deviations, and loss after the optimization
+    :return: Results - A named tuple containing pre_transformation,
+        pre_transform_std, losses: The optimized parameters, the optimized
+        standard deviations, and a history of ELBO values.
+    :rtype: array-like, array-like, Object
+    """
+
+    def negative_logprob(x):
+        return -loss_func(x)
+
+    def objective(params, t):
+        rng = random.PRNGKey(t)
+        return -calculate_batch_elbo(negative_logprob, rng, params, nsamples)
+
+    def learn_schedule(i):
+        return exp(-1e-2 * i) * init_learn_rate
+
+    init_mean, init_std = initial_parameters, -10 * zeros_like(initial_parameters)
+    opt_init, opt_update, get_params = adam(learn_schedule)
+    opt_state = opt_init((init_mean, init_std))
+
+    def update(i, opt_state):
+        params = get_params(opt_state)
+        elbo, gradient = jax.value_and_grad(objective)(params, i)
+        return opt_update(i, gradient, opt_state), elbo
+
+    if jit:
+        update = jax.jit(update)
+
+    elbos = list()
+    for t in range(n_iter):
+        opt_state, elbo = update(t, opt_state)
+        elbos.append(elbo.item())
 
-    def new_func(x):
-        return exp(func(x))
+    params, stds = get_params(opt_state)
 
-    return new_func
+    Results = namedtuple("Results", "pre_transformation pre_transformation_std losses")
+    return Results(params, stds, elbos)
```

### Comparing `mellon-1.2.0/mellon.egg-info/PKG-INFO` & `mellon-1.3.0/mellon.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,65 @@
 Metadata-Version: 2.1
 Name: mellon
-Version: 1.2.0
+Version: 1.3.0
 Summary: Non-parametric density estimator.
 Home-page: https://github.com/settylab/mellon
 Author: Setty Lab
 Author-email: msetty@fredhutch.org
 License: GNU General Public License v3.0
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
+Mellon
+======
+
 .. image:: https://zenodo.org/badge/558998366.svg
    :target: https://zenodo.org/badge/latestdoi/558998366
 .. image:: https://codecov.io/github/settylab/Mellon/branch/main/graph/badge.svg?token=TKIKXK4MPG 
     :target: https://app.codecov.io/github/settylab/Mellon
+.. image:: https://www.codefactor.io/repository/github/settylab/mellon/badge/main
+      :target: https://www.codefactor.io/repository/github/settylab/mellon/overview/main
+      :alt: CodeFactor
 .. image:: https://badge.fury.io/py/mellon.svg
        :target: https://badge.fury.io/py/mellon
+.. image:: https://anaconda.org/conda-forge/mellon/badges/version.svg
+       :target: https://anaconda.org/conda-forge/mellon
 .. image:: https://static.pepy.tech/personalized-badge/mellon?period=total&units=international_system&left_color=grey&right_color=lightgrey&left_text=Downloads
     :target: https://pepy.tech/project/mellon
 
-Mellon is a non-parametric density estimator based on the NearestNeighbors distribution.
+.. image:: https://github.com/settylab/mellon/raw/main/landscape.png?raw=true
+   :target: https://github.com/settylab/Mellon
+
+Mellon is a non-parametric cell-state density estimator based on a
+nearest-neighbors-distance distribution. It uses a sparse gaussian process
+to produce a differntiable density function that can be evaluated out of sample.
 
 Installation
 ============
 
-To install with pip you can run:
+To install Mellon using **pip** you can run:
 
 .. code-block:: bash
 
    pip install mellon
 
+or to install using **conda** you can run:
+
+.. code-block:: bash
+
+   conda install -c conda-forge mellon
+
+or to install using **mamba** you can run:
+
+.. code-block:: bash
+
+   mamba install -c conda-forge mellon
+
 Documentation
 =============
 
 Please read the
 `documentation <https://mellon.readthedocs.io/en/latest/index.html>`_
 or use this
 `basic tutorial notebook <https://github.com/settylab/Mellon/blob/main/notebooks/basic_tutorial.ipynb>`_.
```

### Comparing `mellon-1.2.0/setup.py` & `mellon-1.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 
 
 def get_version(rel_path):
     for line in (this_directory / rel_path).read_text().splitlines():
-        if line.startswith('__version__'):
+        if line.startswith("__version__"):
             delim = '"' if '"' in line else "'"
             return line.split(delim)[1]
     else:
         raise RuntimeError("Unable to find version string.")
 
 
 setup(
     name="mellon",
-    version=get_version('mellon/__init__.py'),
+    version=get_version("mellon/__init__.py"),
     description="Non-parametric density estimator.",
     url="https://github.com/settylab/mellon",
     author="Setty Lab",
     author_email="msetty@fredhutch.org",
     license="GNU General Public License v3.0",
     packages=["mellon"],
     install_requires=[
```

