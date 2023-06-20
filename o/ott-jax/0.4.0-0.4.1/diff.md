# Comparing `tmp/ott-jax-0.4.0.tar.gz` & `tmp/ott-jax-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ott-jax-0.4.0.tar", last modified: Mon Feb 13 10:10:50 2023, max compression
+gzip compressed data, was "ott-jax-0.4.1.tar", last modified: Tue Jun 20 14:15:35 2023, max compression
```

## Comparing `ott-jax-0.4.0.tar` & `ott-jax-0.4.1.tar`

### file list

```diff
@@ -1,110 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 10:10:50.135639 ott-jax-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-02-13 10:09:48.000000 ott-jax-0.4.0/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-02-13 10:09:48.000000 ott-jax-0.4.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-02-13 10:09:48.000000 ott-jax-0.4.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-02-13 10:09:48.000000 ott-jax-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-02-13 10:09:48.000000 ott-jax-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-02-13 10:09:48.000000 ott-jax-0.4.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-02-13 10:09:48.000000 ott-jax-0.4.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-02-13 10:09:48.000000 ott-jax-0.4.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-02-13 10:09:48.000000 ott-jax-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-02-13 10:09:48.000000 ott-jax-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    19256 2023-02-13 10:10:50.135639 ott-jax-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-02-13 10:09:48.000000 ott-jax-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-13 10:09:48.000000 ott-jax-0.4.0/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6341 2023-02-13 10:09:48.000000 ott-jax-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-13 10:10:50.135639 ott-jax-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 10:10:50.123639 ott-jax-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 10:10:50.127639 ott-jax-0.4.0/src/ott/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 10:10:50.127639 ott-jax-0.4.0/src/ott/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24760 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/geometry/costs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/geometry/epsilon_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    32985 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/geometry/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    12668 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/geometry/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    15520 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/geometry/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    11933 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/geometry/low_rank.py
--rw-r--r--   0 runner    (1001) docker     (123)    27041 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/geometry/pointcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/geometry/segment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 10:10:50.127639 ott-jax-0.4.0/src/ott/initializers/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/initializers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 10:10:50.127639 ott-jax-0.4.0/src/ott/initializers/linear/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/initializers/linear/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9700 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/initializers/linear/initializers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18488 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/initializers/linear/initializers_lr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 10:10:50.127639 ott-jax-0.4.0/src/ott/initializers/nn/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/initializers/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7842 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/initializers/nn/initializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 10:10:50.127639 ott-jax-0.4.0/src/ott/initializers/quadratic/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/initializers/quadratic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6636 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/initializers/quadratic/initializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 10:10:50.131639 ott-jax-0.4.0/src/ott/math/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/math/decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     8412 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/math/fixed_point_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/math/matrix_square_root.py
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/math/unbalanced_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/math/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 10:10:50.131639 ott-jax-0.4.0/src/ott/problems/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/problems/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 10:10:50.131639 ott-jax-0.4.0/src/ott/problems/linear/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/problems/linear/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/problems/linear/barycenter_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/problems/linear/linear_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)    12706 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/problems/linear/potentials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 10:10:50.131639 ott-jax-0.4.0/src/ott/problems/nn/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/problems/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/problems/nn/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 10:10:50.131639 ott-jax-0.4.0/src/ott/problems/quadratic/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/problems/quadratic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10579 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/problems/quadratic/gw_barycenter.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/problems/quadratic/quadratic_costs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18472 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/problems/quadratic/quadratic_problem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 10:10:50.131639 ott-jax-0.4.0/src/ott/solvers/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/solvers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 10:10:50.131639 ott-jax-0.4.0/src/ott/solvers/linear/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/solvers/linear/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/solvers/linear/acceleration.py
--rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/solvers/linear/continuous_barycenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7672 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/solvers/linear/discrete_barycenter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11966 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/solvers/linear/implicit_differentiation.py
--rw-r--r--   0 runner    (1001) docker     (123)    45996 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/solvers/linear/sinkhorn.py
--rw-r--r--   0 runner    (1001) docker     (123)    22428 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/solvers/linear/sinkhorn_lr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 10:10:50.131639 ott-jax-0.4.0/src/ott/solvers/nn/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/solvers/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/solvers/nn/conjugate_solvers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/solvers/nn/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11887 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/solvers/nn/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    21265 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/solvers/nn/neuraldual.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 10:10:50.131639 ott-jax-0.4.0/src/ott/solvers/quadratic/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/solvers/quadratic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18378 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/solvers/quadratic/gromov_wasserstein.py
--rw-r--r--   0 runner    (1001) docker     (123)    10795 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/solvers/quadratic/gw_barycenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/solvers/was_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 10:10:50.131639 ott-jax-0.4.0/src/ott/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 10:10:50.135639 ott-jax-0.4.0/src/ott/tools/gaussian_mixture/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/tools/gaussian_mixture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9124 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/tools/gaussian_mixture/fit_gmm.py
--rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/tools/gaussian_mixture/fit_gmm_pair.py
--rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/tools/gaussian_mixture/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)    10233 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/tools/gaussian_mixture/gaussian_mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/tools/gaussian_mixture/gaussian_mixture_pair.py
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/tools/gaussian_mixture/linalg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/tools/gaussian_mixture/probabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/tools/gaussian_mixture/scale_tril.py
--rw-r--r--   0 runner    (1001) docker     (123)    13622 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/tools/k_means.py
--rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/tools/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5988 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/tools/segment_sinkhorn.py
--rw-r--r--   0 runner    (1001) docker     (123)    13253 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/tools/sinkhorn_divergence.py
--rw-r--r--   0 runner    (1001) docker     (123)    17573 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/tools/soft_sort.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-02-13 10:09:48.000000 ott-jax-0.4.0/src/ott/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 10:10:50.135639 ott-jax-0.4.0/src/ott_jax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19256 2023-02-13 10:10:49.000000 ott-jax-0.4.0/src/ott_jax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-02-13 10:10:50.000000 ott-jax-0.4.0/src/ott_jax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 10:10:49.000000 ott-jax-0.4.0/src/ott_jax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-02-13 10:10:49.000000 ott-jax-0.4.0/src/ott_jax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-13 10:10:49.000000 ott-jax-0.4.0/src/ott_jax.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:15:35.305106 ott-jax-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-20 14:14:33.000000 ott-jax-0.4.1/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-20 14:14:33.000000 ott-jax-0.4.1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-06-20 14:14:33.000000 ott-jax-0.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-20 14:14:33.000000 ott-jax-0.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-20 14:14:33.000000 ott-jax-0.4.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-20 14:14:33.000000 ott-jax-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-20 14:14:33.000000 ott-jax-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    19488 2023-06-20 14:15:35.305106 ott-jax-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-06-20 14:14:33.000000 ott-jax-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-20 14:14:33.000000 ott-jax-0.4.1/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-06-20 14:14:33.000000 ott-jax-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 14:15:35.305106 ott-jax-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-20 14:14:33.000000 ott-jax-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:15:35.269105 ott-jax-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:15:35.277105 ott-jax-0.4.1/src/ott/
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:15:35.281105 ott-jax-0.4.1/src/ott/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29464 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/geometry/costs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/geometry/epsilon_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32238 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/geometry/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8972 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/geometry/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15339 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/geometry/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12295 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/geometry/low_rank.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/geometry/pointcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/geometry/segment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:15:35.281105 ott-jax-0.4.1/src/ott/initializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/initializers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:15:35.281105 ott-jax-0.4.1/src/ott/initializers/linear/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/initializers/linear/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12862 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/initializers/linear/initializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19405 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/initializers/linear/initializers_lr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:15:35.281105 ott-jax-0.4.1/src/ott/initializers/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/initializers/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8837 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/initializers/nn/initializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:15:35.285106 ott-jax-0.4.1/src/ott/initializers/quadratic/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/initializers/quadratic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/initializers/quadratic/initializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:15:35.285106 ott-jax-0.4.1/src/ott/math/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8334 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/math/fixed_point_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10936 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/math/matrix_square_root.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/math/unbalanced_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/math/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:15:35.285106 ott-jax-0.4.1/src/ott/problems/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/problems/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:15:35.289106 ott-jax-0.4.1/src/ott/problems/linear/
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/problems/linear/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7980 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/problems/linear/barycenter_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/problems/linear/linear_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13549 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/problems/linear/potentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:15:35.289106 ott-jax-0.4.1/src/ott/problems/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/problems/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/problems/nn/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:15:35.289106 ott-jax-0.4.1/src/ott/problems/quadratic/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/problems/quadratic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/problems/quadratic/gw_barycenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/problems/quadratic/quadratic_costs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20108 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/problems/quadratic/quadratic_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:15:35.289106 ott-jax-0.4.1/src/ott/solvers/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/solvers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:15:35.293106 ott-jax-0.4.1/src/ott/solvers/linear/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/solvers/linear/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/solvers/linear/acceleration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7841 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/solvers/linear/continuous_barycenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8466 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/solvers/linear/discrete_barycenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13685 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/solvers/linear/implicit_differentiation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/solvers/linear/lineax_implicit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46962 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/solvers/linear/sinkhorn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27617 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/solvers/linear/sinkhorn_lr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:15:35.293106 ott-jax-0.4.1/src/ott/solvers/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/solvers/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/solvers/nn/conjugate_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/solvers/nn/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11296 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/solvers/nn/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20869 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/solvers/nn/neuraldual.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:15:35.297106 ott-jax-0.4.1/src/ott/solvers/quadratic/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/solvers/quadratic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19738 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/solvers/quadratic/gromov_wasserstein.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11824 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/solvers/quadratic/gw_barycenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/solvers/was_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:15:35.297106 ott-jax-0.4.1/src/ott/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:15:35.301106 ott-jax-0.4.1/src/ott/tools/gaussian_mixture/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/tools/gaussian_mixture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9150 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/tools/gaussian_mixture/fit_gmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12061 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/tools/gaussian_mixture/fit_gmm_pair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/tools/gaussian_mixture/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/tools/gaussian_mixture/gaussian_mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/tools/gaussian_mixture/gaussian_mixture_pair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/tools/gaussian_mixture/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/tools/gaussian_mixture/probabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/tools/gaussian_mixture/scale_tril.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13743 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/tools/k_means.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/tools/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/tools/segment_sinkhorn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13334 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/tools/sinkhorn_divergence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17532 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/tools/soft_sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-06-20 14:14:33.000000 ott-jax-0.4.1/src/ott/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:15:35.301106 ott-jax-0.4.1/src/ott_jax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19488 2023-06-20 14:15:34.000000 ott-jax-0.4.1/src/ott_jax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-06-20 14:15:35.000000 ott-jax-0.4.1/src/ott_jax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 14:15:34.000000 ott-jax-0.4.1/src/ott_jax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-20 14:15:34.000000 ott-jax-0.4.1/src/ott_jax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-20 14:15:34.000000 ott-jax-0.4.1/src/ott_jax.egg-info/top_level.txt
```

### Comparing `ott-jax-0.4.0/.gitignore` & `ott-jax-0.4.1/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -155,13 +155,16 @@
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 .idea/
 
+# vscode
+.vscode/
+
 # generated documentation
 docs/html
 **/_autosummary
 
 # macos
 **/.DS_Store
```

### Comparing `ott-jax-0.4.0/LICENSE` & `ott-jax-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.0/PKG-INFO` & `ott-jax-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ott-jax
-Version: 0.4.0
+Version: 0.4.1
 Summary: Optimal Transport Tools in JAX.
 Author-email: OTT team <optimal.transport.tools@gmail.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -226,15 +226,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
-Provides-Extra: experimental
 Provides-Extra: docs
 License-File: LICENSE
 
 <img src="https://raw.githubusercontent.com/ott-jax/ott/main/docs/_static/images/logoOTT.png" width="10%" alt="logo">
 
 # Optimal Transport Tools (OTT)
 [![Downloads](https://static.pepy.tech/badge/ott-jax)](https://pypi.org/project/ott-jax/)
@@ -242,35 +241,31 @@
 [![Docs](https://img.shields.io/readthedocs/ott-jax/latest)](https://ott-jax.readthedocs.io/en/latest/)
 [![Coverage](https://img.shields.io/codecov/c/github/ott-jax/ott/main)](https://app.codecov.io/gh/ott-jax/ott)
 
 **See the [full documentation](https://ott-jax.readthedocs.io/en/latest/).**
 
 ## What is OTT-JAX?
 A ``JAX`` powered library to compute optimal transport at scale and on accelerators, ``OTT-JAX`` includes the fastest
-implementation of the Sinkhorn algorithm you will find around. We have implemented all tweaks (scheduling,
-acceleration, initializations) and extensions (low-rank), that can be used directly, or within more advanced problems
+implementation of the Sinkhorn algorithm you will find around. We have implemented all tweaks (scheduling, momentum, acceleration, initializations) and extensions (low-rank, entropic maps). They can be used directly between two datasets, or within more advanced problems
 (Gromov-Wasserstein, barycenters). Some of ``JAX`` features, including
 [JIT](https://jax.readthedocs.io/en/latest/notebooks/quickstart.html#Using-jit-to-speed-up-functions),
 [auto-vectorization](https://jax.readthedocs.io/en/latest/notebooks/quickstart.html#Auto-vectorization-with-vmap) and
 [implicit differentiation](https://jax.readthedocs.io/en/latest/notebooks/Custom_derivative_rules_for_Python_code.html)
-work towards the goal of having end-to-end differentiable outputs. OTT-JAX is developed by a team of researchers
-from Apple, Google, Meta and many academic contributors, including TU München, Oxford, ENSAE/IP Paris and the
-Hebrew University.
+work towards the goal of having end-to-end differentiable outputs. OTT-JAX is led by a team of researchers at Apple, with contributions from Google and Meta researchers, as well as many academic partners, including TU München, Oxford, ENSAE/IP Paris, ENS Paris and the Hebrew University.
 
 ## Installation
 Install ``OTT-JAX`` from [PyPI](https://pypi.org/project/ott-jax/) as:
 ```bash
 pip install ott-jax
 ```
 or with ``conda`` via [conda-forge](https://anaconda.org/conda-forge/ott-jax) as:
 ```bash
 conda install -c conda-forge ott-jax
 ```
 
-
 ## What is optimal transport?
 Optimal transport can be loosely described as the branch of mathematics and optimization that studies
 *matching problems*: given two families of points, and a cost function on pairs of points, find a "good" (low cost) way
 to associate bijectively to every point in the first family another in the second.
 
 Such problems appear in all areas of science, are easy to describe, yet hard to solve. Indeed, while matching optimally
 two sets of $n$ points using a pairwise cost can be solved with the
@@ -306,25 +301,27 @@
 prob = linear_problem.LinearProblem(geom, a, b)
 
 solver = sinkhorn.Sinkhorn()
 out = solver(prob)
 ```
 
 The call to `solver(prob)` above works out the optimal transport solution. The `out` object contains a transport matrix
-(here of size $12\times 14$) that quantifies a `link strength` between each point of the first point cloud, to one or
+(here of size $12\times 14$) that quantifies the association strength between each point of the first point cloud, to one or
 more points from the second, as illustrated in the plot below. We provide more flexibility to define custom cost
 functions, objectives, and solvers, as detailed in the [full documentation](https://ott-jax.readthedocs.io/en/latest/).
 
-![obtained coupling](https://raw.githubusercontent.com/ott-jax/ott/main/images/couplings.png)
+![obtained coupling](https://raw.githubusercontent.com/ott-jax/ott/main/docs/_static/images/couplings.png)
 
 ## Citation
 If you have found this work useful, please consider citing this reference:
 
 ```
 @article{cuturi2022optimal,
   title={Optimal Transport Tools (OTT): A JAX Toolbox for all things Wasserstein},
   author={Cuturi, Marco and Meng-Papaxanthos, Laetitia and Tian, Yingtao and Bunne, Charlotte and
           Davis, Geoff and Teboul, Olivier},
   journal={arXiv preprint arXiv:2201.12324},
   year={2022}
 }
 ```
+## See also
+The [moscot](https://moscot.readthedocs.io/en/latest/index.html) package for OT analysis of multi-omics data also uses OTT as a backbone.
```

### Comparing `ott-jax-0.4.0/README.md` & `ott-jax-0.4.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -6,35 +6,31 @@
 [![Docs](https://img.shields.io/readthedocs/ott-jax/latest)](https://ott-jax.readthedocs.io/en/latest/)
 [![Coverage](https://img.shields.io/codecov/c/github/ott-jax/ott/main)](https://app.codecov.io/gh/ott-jax/ott)
 
 **See the [full documentation](https://ott-jax.readthedocs.io/en/latest/).**
 
 ## What is OTT-JAX?
 A ``JAX`` powered library to compute optimal transport at scale and on accelerators, ``OTT-JAX`` includes the fastest
-implementation of the Sinkhorn algorithm you will find around. We have implemented all tweaks (scheduling,
-acceleration, initializations) and extensions (low-rank), that can be used directly, or within more advanced problems
+implementation of the Sinkhorn algorithm you will find around. We have implemented all tweaks (scheduling, momentum, acceleration, initializations) and extensions (low-rank, entropic maps). They can be used directly between two datasets, or within more advanced problems
 (Gromov-Wasserstein, barycenters). Some of ``JAX`` features, including
 [JIT](https://jax.readthedocs.io/en/latest/notebooks/quickstart.html#Using-jit-to-speed-up-functions),
 [auto-vectorization](https://jax.readthedocs.io/en/latest/notebooks/quickstart.html#Auto-vectorization-with-vmap) and
 [implicit differentiation](https://jax.readthedocs.io/en/latest/notebooks/Custom_derivative_rules_for_Python_code.html)
-work towards the goal of having end-to-end differentiable outputs. OTT-JAX is developed by a team of researchers
-from Apple, Google, Meta and many academic contributors, including TU München, Oxford, ENSAE/IP Paris and the
-Hebrew University.
+work towards the goal of having end-to-end differentiable outputs. OTT-JAX is led by a team of researchers at Apple, with contributions from Google and Meta researchers, as well as many academic partners, including TU München, Oxford, ENSAE/IP Paris, ENS Paris and the Hebrew University.
 
 ## Installation
 Install ``OTT-JAX`` from [PyPI](https://pypi.org/project/ott-jax/) as:
 ```bash
 pip install ott-jax
 ```
 or with ``conda`` via [conda-forge](https://anaconda.org/conda-forge/ott-jax) as:
 ```bash
 conda install -c conda-forge ott-jax
 ```
 
-
 ## What is optimal transport?
 Optimal transport can be loosely described as the branch of mathematics and optimization that studies
 *matching problems*: given two families of points, and a cost function on pairs of points, find a "good" (low cost) way
 to associate bijectively to every point in the first family another in the second.
 
 Such problems appear in all areas of science, are easy to describe, yet hard to solve. Indeed, while matching optimally
 two sets of $n$ points using a pairwise cost can be solved with the
@@ -70,25 +66,27 @@
 prob = linear_problem.LinearProblem(geom, a, b)
 
 solver = sinkhorn.Sinkhorn()
 out = solver(prob)
 ```
 
 The call to `solver(prob)` above works out the optimal transport solution. The `out` object contains a transport matrix
-(here of size $12\times 14$) that quantifies a `link strength` between each point of the first point cloud, to one or
+(here of size $12\times 14$) that quantifies the association strength between each point of the first point cloud, to one or
 more points from the second, as illustrated in the plot below. We provide more flexibility to define custom cost
 functions, objectives, and solvers, as detailed in the [full documentation](https://ott-jax.readthedocs.io/en/latest/).
 
-![obtained coupling](https://raw.githubusercontent.com/ott-jax/ott/main/images/couplings.png)
+![obtained coupling](https://raw.githubusercontent.com/ott-jax/ott/main/docs/_static/images/couplings.png)
 
 ## Citation
 If you have found this work useful, please consider citing this reference:
 
 ```
 @article{cuturi2022optimal,
   title={Optimal Transport Tools (OTT): A JAX Toolbox for all things Wasserstein},
   author={Cuturi, Marco and Meng-Papaxanthos, Laetitia and Tian, Yingtao and Bunne, Charlotte and
           Davis, Geoff and Teboul, Olivier},
   journal={arXiv preprint arXiv:2201.12324},
   year={2022}
 }
 ```
+## See also
+The [moscot](https://moscot.readthedocs.io/en/latest/index.html) package for OT analysis of multi-omics data also uses OTT as a backbone.
```

### Comparing `ott-jax-0.4.0/src/ott/__init__.py` & `ott-jax-0.4.1/src/ott/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-# Copyright 2022 Google LLC.
+# Copyright OTT-JAX
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-#     http://www.apache.org/licenses/LICENSE-2.0
+#   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from . import geometry, initializers, math, problems, solvers, tools, utils
```

### Comparing `ott-jax-0.4.0/src/ott/geometry/__init__.py` & `ott-jax-0.4.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,17 @@
-# Copyright 2022 Google LLC.
+# Copyright OTT-JAX
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-#     http://www.apache.org/licenses/LICENSE-2.0
+#   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from . import costs, epsilon_scheduler, geometry, graph, grid, pointcloud, segment
+from setuptools import setup
+
+# for packaging tools not supporting, e.g., PEP 517, PEP 660
+setup()
```

### Comparing `ott-jax-0.4.0/src/ott/geometry/costs.py` & `ott-jax-0.4.1/src/ott/geometry/costs.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,67 +1,90 @@
-# Copyright 2022 Google LLC.
+# Copyright OTT-JAX
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-#     http://www.apache.org/licenses/LICENSE-2.0
+#   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Several cost/norm functions for relevant vector types."""
 import abc
 import functools
 import math
-from typing import Any, Callable, Optional, Tuple, Union
+from typing import Any, Callable, Dict, Optional, Tuple, Union
 
 import jax
 import jax.numpy as jnp
+import numpy as np
 
 from ott.math import fixed_point_loop, matrix_square_root
+from ott.math import utils as mu
 
 __all__ = [
-    "PNormP", "SqPNorm", "Euclidean", "SqEuclidean", "Cosine", "ElasticL1",
-    "ElasticSTVS", "ElasticSqKOverlap", "Bures", "UnbalancedBures"
+    "PNormP",
+    "SqPNorm",
+    "Euclidean",
+    "SqEuclidean",
+    "Cosine",
+    "ElasticL1",
+    "ElasticSTVS",
+    "ElasticSqKOverlap",
+    "Bures",
+    "UnbalancedBures",
+    "SoftDTW",
 ]
 
 
 @jax.tree_util.register_pytree_node_class
 class CostFn(abc.ABC):
   """Base class for all costs.
 
   Cost functions evaluate a function on a pair of inputs. For convenience,
   that function is split into two norms -- evaluated on each input separately --
   followed by a pairwise cost that involves both inputs, as in:
 
-  ``c(x,y) = norm(x) + norm(y) + pairwise(x,y)``
+  .. math::
+
+    c(x,y) = norm(x) + norm(y) + pairwise(x,y)
 
-  If the :attr:`norm` function is not implemented, that value is handled as a 0,
-  and only :func:`pairwise` is used.
+  If the :attr:`norm` function is not implemented, that value is handled as
+  :math:`0`, and only :func:`pairwise` is used.
   """
 
   # no norm function created by default.
   norm: Optional[Callable[[jnp.ndarray], Union[float, jnp.ndarray]]] = None
 
   @abc.abstractmethod
   def pairwise(self, x: jnp.ndarray, y: jnp.ndarray) -> float:
-    pass
+    """Compute cost between :math:`x` and :math:`y`.
 
-  def barycenter(self, weights: jnp.ndarray, xs: jnp.ndarray) -> jnp.ndarray:
+    Args:
+      x: Array.
+      y: Array.
+
+    Returns:
+      The cost.
+    """
+
+  def barycenter(self, weights: jnp.ndarray,
+                 xs: jnp.ndarray) -> Tuple[jnp.ndarray, Any]:
     """Barycentric operator.
 
     Args:
       weights: Convex set of weights.
       xs: Points.
 
     Returns:
-      The barycenter of `xs` using `weights` coefficients.
+      A list, whose first element is the barycenter of `xs` using `weights`
+      coefficients, followed by auxiliary information on the convergence of
+      the algorithm.
     """
     raise NotImplementedError("Barycenter is not implemented.")
 
   @classmethod
   def _padder(cls, dim: int) -> jnp.ndarray:
     """Create a padding vector of adequate dimension, well-suited to a cost.
 
@@ -70,46 +93,59 @@
 
     Returns:
       The padding vector.
     """
     return jnp.zeros((1, dim))
 
   def __call__(self, x: jnp.ndarray, y: jnp.ndarray) -> float:
+    """Compute cost between :math:`x` and :math:`y`.
+
+    Args:
+      x: Array.
+      y: Array.
+
+    Returns:
+      The cost, optionally including the :attr:`norms <norm>` of
+      :math:`x`/:math:`y`.
+    """
     cost = self.pairwise(x, y)
     if self.norm is None:
       return cost
     return cost + self.norm(x) + self.norm(y)
 
+  # TODO(michalk8): unused
   def all_pairs(self, x: jnp.ndarray, y: jnp.ndarray) -> jnp.ndarray:
-    """Compute matrix of all costs (including norms) for vectors in x / y.
+    """Compute matrix of all pairwise costs, including the :attr:`norms <norm>`.
 
     Args:
-      x: [num_a, d] jnp.ndarray
-      y: [num_b, d] jnp.ndarray
+      x: Array of shape ``[n, ...]``.
+      y: Array of shape ``[m, ...]``.
+
     Returns:
-      [num_a, num_b] matrix of cost evaluations.
+      Array of shape ``[n, m]`` of cost evaluations.
     """
     return jax.vmap(lambda x_: jax.vmap(lambda y_: self(x_, y_))(y))(x)
 
   def all_pairs_pairwise(self, x: jnp.ndarray, y: jnp.ndarray) -> jnp.ndarray:
-    """Compute matrix of all pairwise-costs (no norms) for vectors in x / y.
+    """Compute matrix of all pairwise costs, excluding the :attr:`norms <norm>`.
 
     Args:
-      x: [num_a, d] jnp.ndarray
-      y: [num_b, d] jnp.ndarray
+      x: Array of shape ``[n, ...]``.
+      y: Array of shape ``[m, ...]``.
+
     Returns:
-      [num_a, num_b] matrix of pairwise cost evaluations.
+      Array of shape ``[n, m]`` of cost evaluations.
     """
     return jax.vmap(lambda x_: jax.vmap(lambda y_: self.pairwise(x_, y_))(y))(x)
 
-  def tree_flatten(self):
+  def tree_flatten(self):  # noqa: D102
     return (), None
 
   @classmethod
-  def tree_unflatten(cls, aux_data, children):
+  def tree_unflatten(cls, aux_data, children):  # noqa: D102
     del aux_data
     return cls(*children)
 
 
 @jax.tree_util.register_pytree_node_class
 class TICost(CostFn):
   """Base class for translation invariant (TI) costs.
@@ -138,74 +174,72 @@
   def pairwise(self, x: jnp.ndarray, y: jnp.ndarray) -> float:
     """Compute cost as evaluation of :func:`h` on :math:`x-y`."""
     return self.h(x - y)
 
 
 @jax.tree_util.register_pytree_node_class
 class SqPNorm(TICost):
-  """Squared p-norm of the difference of two vectors.
+  r"""Squared p-norm of the difference of two vectors.
 
   Args:
-    p: Power of the p-norm.
+    p: Power of the p-norm, :math:`\ge 1`.
   """
 
   def __init__(self, p: float):
     super().__init__()
-    assert p >= 1.0, "p parameter in sq. p-norm should be >= 1.0"
     self.p = p
-    self.q = 1. / (1. - 1. / self.p) if p > 1.0 else jnp.inf
+    self.q = 1.0 / (1.0 - (1.0 / p)) if p > 1.0 else jnp.inf
 
-  def h(self, z: jnp.ndarray) -> float:
+  def h(self, z: jnp.ndarray) -> float:  # noqa: D102
     return 0.5 * jnp.linalg.norm(z, self.p) ** 2
 
   def h_legendre(self, z: jnp.ndarray) -> float:
     """Legendre transform of :func:`h`.
 
     For details on the derivation, see e.g., :cite:`boyd:04`, p. 93/94.
     """
     return 0.5 * jnp.linalg.norm(z, self.q) ** 2
 
-  def tree_flatten(self):
+  def tree_flatten(self):  # noqa: D102
     return (), (self.p,)
 
   @classmethod
-  def tree_unflatten(cls, aux_data, children):
+  def tree_unflatten(cls, aux_data, children):  # noqa: D102
     del children
-    return cls(aux_data[0])
+    return cls(*aux_data)
 
 
 @jax.tree_util.register_pytree_node_class
 class PNormP(TICost):
-  """p-norm to the power p (and divided by p) of the difference of two vectors.
+  r"""p-norm to the power p (and divided by p) of the difference of two vectors.
 
   Args:
-    p: Power of the p-norm, a finite float larger than 1.0.
+    p: Power of the p-norm in :math:`[1, +\infty)`.
+      Note that :func:`h_legendre` is not defined for ``p = 1``.
   """
 
   def __init__(self, p: float):
     super().__init__()
-    assert p >= 1.0, "p parameter in p-norm should be larger than 1.0"
-    assert p < jnp.inf, "p parameter in p-norm should be finite"
     self.p = p
-    self.q = 1. / (1. - 1. / self.p) if p > 1.0 else jnp.inf
+    self.q = 1.0 / (1.0 - (1.0 / p)) if p > 1.0 else jnp.inf
 
-  def h(self, z: jnp.ndarray) -> float:
+  def h(self, z: jnp.ndarray) -> float:  # noqa: D102
     return jnp.linalg.norm(z, self.p) ** self.p / self.p
 
-  def h_legendre(self, z: jnp.ndarray) -> float:
-    assert self.q < jnp.inf, "Legendre transform not defined for `p=1.0`"
+  def h_legendre(self, z: jnp.ndarray) -> float:  # noqa: D102
+    # not defined for `p=1`
     return jnp.linalg.norm(z, self.q) ** self.q / self.q
 
-  def tree_flatten(self):
+  def tree_flatten(self):  # noqa: D102
     return (), (self.p,)
 
   @classmethod
-  def tree_unflatten(cls, aux_data, children):
+  def tree_unflatten(cls, aux_data, children):  # noqa: D102
     del children
-    return cls(aux_data[0])
+    return cls(*aux_data)
 
 
 @jax.tree_util.register_pytree_node_class
 class Euclidean(CostFn):
   """Euclidean distance.
 
   Note that the Euclidean distance is not cast as a
@@ -227,23 +261,24 @@
     """Compute squared Euclidean norm for vector."""
     return jnp.sum(x ** 2, axis=-1)
 
   def pairwise(self, x: jnp.ndarray, y: jnp.ndarray) -> float:
     """Compute minus twice the dot-product between vectors."""
     return -2. * jnp.vdot(x, y)
 
-  def h(self, z: jnp.ndarray) -> float:
+  def h(self, z: jnp.ndarray) -> float:  # noqa: D102
     return jnp.sum(z ** 2)
 
-  def h_legendre(self, z: jnp.ndarray) -> float:
+  def h_legendre(self, z: jnp.ndarray) -> float:  # noqa: D102
     return 0.25 * jnp.sum(z ** 2)
 
-  def barycenter(self, weights: jnp.ndarray, xs: jnp.ndarray) -> jnp.ndarray:
+  def barycenter(self, weights: jnp.ndarray,
+                 xs: jnp.ndarray) -> Tuple[jnp.ndarray, Any]:
     """Output barycenter of vectors when using squared-Euclidean distance."""
-    return jnp.average(xs, weights=weights, axis=0)
+    return jnp.average(xs, weights=weights, axis=0), None
 
 
 @jax.tree_util.register_pytree_node_class
 class Cosine(CostFn):
   """Cosine distance cost function.
 
   Args:
@@ -283,52 +318,51 @@
   def reg(self, z: jnp.ndarray) -> float:
     """Regularization function."""
 
   def prox_reg(self, z: jnp.ndarray) -> jnp.ndarray:
     """Proximal operator of :func:`reg`."""
     raise NotImplementedError("Proximal operator is not implemented.")
 
-  def h(self, z: jnp.ndarray) -> float:
+  def h(self, z: jnp.ndarray) -> float:  # noqa: D102
     return 0.5 * jnp.linalg.norm(z, ord=2) ** 2 + self.reg(z)
 
-  def h_legendre(self, z: jnp.ndarray) -> float:
+  def h_legendre(self, z: jnp.ndarray) -> float:  # noqa: D102
     q = jax.lax.stop_gradient(self.prox_reg(z))
     return jnp.sum(q * z) - self.h(q)
 
 
 @jax.tree_util.register_pytree_node_class
 class ElasticL1(RegTICost):
   r"""Cost inspired by elastic net :cite:`zou:05` regularization.
 
   .. math::
 
     \frac{1}{2} \|\cdot\|_2^2 + \gamma \|\cdot\|_1
 
   Args:
-    gamma: Strength of the :math:`\|\cdot\|_1` regularization.
+    gamma: Strength of the :math:`\|\cdot\|_1` regularization, :math:`\ge 0`.
   """
 
   def __init__(self, gamma: float = 1.0):
     super().__init__()
-    assert gamma >= 0, "Gamma must be non-negative."
     self.gamma = gamma
 
-  def reg(self, z: jnp.ndarray) -> float:
+  def reg(self, z: jnp.ndarray) -> float:  # noqa: D102
     return self.gamma * jnp.linalg.norm(z, ord=1)
 
-  def prox_reg(self, z: jnp.ndarray) -> float:
+  def prox_reg(self, z: jnp.ndarray) -> float:  # noqa: D102
     return jnp.sign(z) * jax.nn.relu(jnp.abs(z) - self.gamma)
 
-  def tree_flatten(self):
-    return (), (self.gamma,)
+  def tree_flatten(self):  # noqa: D102
+    return (self.gamma,), None
 
   @classmethod
-  def tree_unflatten(cls, aux_data, children):
-    del children
-    return cls(*aux_data)
+  def tree_unflatten(cls, aux_data, children):  # noqa: D102
+    del aux_data
+    return cls(*children)
 
 
 @jax.tree_util.register_pytree_node_class
 class ElasticSTVS(RegTICost):
   r"""Cost with soft thresholding operator with vanishing shrinkage (STVS)
   :cite:`schreck:15` regularization.
 
@@ -336,37 +370,36 @@
 
     \frac{1}{2} \|\cdot\|_2^2 + \gamma^2\mathbf{1}_d^T\left(\sigma(\cdot) -
     \frac{1}{2} \exp\left(-2\sigma(\cdot)\right) + \frac{1}{2}\right)
 
   where :math:`\sigma(\cdot) := \text{asinh}\left(\frac{\cdot}{2\gamma}\right)`
 
   Args:
-    gamma: Strength of the STVS regularization.
+    gamma: Strength of the STVS regularization, :math:`> 0`.
   """  # noqa
 
   def __init__(self, gamma: float = 1.0):
     super().__init__()
-    assert gamma > 0, "Gamma must be positive."
     self.gamma = gamma
 
-  def reg(self, z: jnp.ndarray) -> float:
+  def reg(self, z: jnp.ndarray) -> float:  # noqa: D102
     u = jnp.arcsinh(jnp.abs(z) / (2 * self.gamma))
     out = u - 0.5 * jnp.exp(-2.0 * u)
     return (self.gamma ** 2) * jnp.sum(out + 0.5)  # make positive
 
-  def prox_reg(self, z: jnp.ndarray) -> float:
+  def prox_reg(self, z: jnp.ndarray) -> float:  # noqa: D102
     return jax.nn.relu(1 - (self.gamma / (jnp.abs(z) + 1e-12)) ** 2) * z
 
-  def tree_flatten(self):
-    return (), (self.gamma,)
+  def tree_flatten(self):  # noqa: D102
+    return (self.gamma,), None
 
   @classmethod
-  def tree_unflatten(cls, aux_data, children):
-    del children
-    return cls(*aux_data)
+  def tree_unflatten(cls, aux_data, children):  # noqa: D102
+    del aux_data
+    return cls(*children)
 
 
 @jax.tree_util.register_pytree_node_class
 class ElasticSqKOverlap(RegTICost):
   r"""Cost with squared k-overlap norm regularization :cite:`argyriou:12`.
 
   .. math::
@@ -375,24 +408,23 @@
 
   where :math:`\|\cdot\|_{ovk}^2` is the squared k-overlap norm,
   see def. 2.1 of :cite:`argyriou:12`.
 
   Args:
     k: Number of groups. Must be in ``[0, d)`` where :math:`d` is the
       dimensionality of the data.
-    gamma: Strength of the squared k-overlap norm regularization.
+    gamma: Strength of the squared k-overlap norm regularization, :math:`> 0`.
   """
 
   def __init__(self, k: int, gamma: float = 1.0):
     super().__init__()
-    assert gamma > 0, "Gamma must be positive."
     self.k = k
     self.gamma = gamma
 
-  def reg(self, z: jnp.ndarray) -> float:
+  def reg(self, z: jnp.ndarray) -> float:  # noqa: D102
     # Prop 2.1 in :cite:`argyriou:12`
     k = self.k
     top_w = jax.lax.top_k(jnp.abs(z), k)[0]  # Fetch largest k values
     top_w = jnp.flip(top_w)  # Sort k-largest from smallest to largest
     # sum (dim - k) smallest values
     sum_bottom = jnp.sum(jnp.abs(z)) - jnp.sum(top_w)
     cumsum_top = jnp.cumsum(top_w)
@@ -405,15 +437,15 @@
     upper_bound = jnp.concatenate(((top_w[1:] - cesaro[:-1] > 0),
                                    jnp.array((True,))))
     r = jnp.argmax(lower_bound * upper_bound)
     s = jnp.sum(jnp.where(jnp.arange(k) < k - r - 1, jnp.flip(top_w) ** 2, 0))
 
     return 0.5 * self.gamma * (s + (r + 1) * cesaro[r] ** 2)
 
-  def prox_reg(self, z: jnp.ndarray) -> float:
+  def prox_reg(self, z: jnp.ndarray) -> float:  # noqa: D102
 
     @functools.partial(jax.vmap, in_axes=[0, None, None])
     def find_indices(r: int, l: jnp.ndarray,
                      z: jnp.ndarray) -> Tuple[jnp.ndarray, jnp.ndarray]:
 
       @functools.partial(jax.vmap, in_axes=[None, 0, None])
       def inner(r: int, l: int,
@@ -450,36 +482,36 @@
     q1 = (beta / (beta + 1)) * z_sorted * (ixs < (k - r - 1))
     q2 = (z_sorted - T) * jnp.logical_and((k - r - 1) <= ixs, ixs < (l + k))
     q = q1 + q2
 
     # change sign and reorder
     return sgn * q[jnp.argsort(z_ixs.astype(float))]
 
-  def tree_flatten(self):
-    return (), (self.k, self.gamma)
+  def tree_flatten(self):  # noqa: D102
+    return (self.gamma,), {"k": self.k}
 
   @classmethod
-  def tree_unflatten(cls, aux_data, children):
-    del children
-    return cls(*aux_data)
+  def tree_unflatten(cls, aux_data, children):  # noqa: D102
+    return cls(**aux_data, gamma=children[0])
 
 
 @jax.tree_util.register_pytree_node_class
 class Bures(CostFn):
-  """Bures distance between a pair of (mean, cov matrix) raveled as vectors.
+  """Bures distance between a pair of (mean, covariance matrix).
 
   Args:
     dimension: Dimensionality of the data.
-    kwargs: Keyword arguments for :func:`~ott.math.matrix_square_root.sqrtm`.
+    sqrtm_kw: Dictionary of keyword arguments to control the
+      behavior of inner calls to :func:`~ott.math.matrix_square_root.sqrtm`.
   """
 
-  def __init__(self, dimension: int, **kwargs: Any):
+  def __init__(self, dimension: int, sqrtm_kw: Optional[Dict[str, Any]] = None):
     super().__init__()
     self._dimension = dimension
-    self._sqrtm_kw = kwargs
+    self._sqrtm_kw = {} if sqrtm_kw is None else sqrtm_kw
 
   def norm(self, x: jnp.ndarray) -> jnp.ndarray:
     """Compute norm of Gaussian, sq. 2-norm of mean + trace of covariance."""
     mean, cov = x_to_means_and_covs(x, self._dimension)
     norm = jnp.sum(mean ** 2, axis=-1)
     norm += jnp.trace(cov, axis1=-2, axis2=-1)
     return norm
@@ -497,126 +529,154 @@
     return -2 * (mean_dot_prod + jnp.trace(sq__sq_x_y_sq_x, axis1=-2, axis2=-1))
 
   def covariance_fixpoint_iter(
       self,
       covs: jnp.ndarray,
       weights: jnp.ndarray,
       tolerance: float = 1e-4,
+      sqrtm_kw: Optional[Dict[str, Any]] = None,
       **kwargs: Any
   ) -> jnp.ndarray:
     """Iterate fix-point updates to compute barycenter of Gaussians.
 
     Args:
       covs: [batch, d^2] covariance matrices
-      weights: simplicial weights (nonnegative, sum to 1)
-      tolerance: tolerance of the overall fixed-point procedure
-      kwargs: parameters passed on to the sqrtm (Newton-Schulz)
-        algorithm to compute matrix square roots.
+      weights: simplicial weights (non-negative, sum to 1)
+      tolerance: tolerance of the fixed-point procedure. That tolerance is
+        applied to the Frobenius norm (normalized by total size)
+        of two successive iterations of the algorithm
+      sqrtm_kw: keyword arguments for :func:`~ott.math.matrix_square_root.sqrtm`
+      kwargs: keyword arguments for the outer fixed-point iteration
 
     Returns:
-      a covariance matrix, the weighted Bures average of the covs matrices.
+      List containing Weighted Bures average of the covariance matrices, and
+      vector of (normalized) 2-norms of successive differences between iterates,
+      to monitor convergence.
     """
+    sqrtm_kw = {} if sqrtm_kw is None else sqrtm_kw
+    # Pop values or set defaults for fixed-point loop.
+    min_iterations = kwargs.pop("min_iterations", 1)
+    max_iterations = kwargs.pop("max_iterations", 100)
+    inner_iterations = kwargs.pop("inner_iterations", 5)
+    dtype = covs.dtype
 
     @functools.partial(jax.vmap, in_axes=[None, 0, 0])
     def scale_covariances(
         cov_sqrt: jnp.ndarray, cov: jnp.ndarray, weight: jnp.ndarray
     ) -> jnp.ndarray:
       """Rescale covariance in barycenter step."""
       return weight * matrix_square_root.sqrtm_only((cov_sqrt @ cov) @ cov_sqrt,
-                                                    **kwargs)
+                                                    **sqrtm_kw)
 
     def cond_fn(iteration: int, constants: Tuple[Any, ...], state) -> bool:
-      del iteration, constants
-      _, diff = state
-      return diff > tolerance
+      del constants
+      _, diffs = state
+      return diffs[iteration // inner_iterations] > tolerance
 
     def body_fn(
         iteration: int, constants: Tuple[Any, ...],
         state: Tuple[jnp.ndarray, float], compute_error: bool
     ) -> Tuple[jnp.ndarray, float]:
-      del iteration, constants, compute_error
-      cov, _ = state
-      cov_sqrt, cov_inv_sqrt, _ = matrix_square_root.sqrtm(cov, **kwargs)
+      del constants, compute_error
+      cov, diffs = state
+      cov_sqrt, cov_inv_sqrt, _ = matrix_square_root.sqrtm(cov, **sqrtm_kw)
       scaled_cov = jnp.linalg.matrix_power(
           jnp.sum(scale_covariances(cov_sqrt, covs, weights), axis=0), 2
       )
       next_cov = (cov_inv_sqrt @ scaled_cov) @ cov_inv_sqrt
       diff = jnp.sum((next_cov - cov) ** 2) / jnp.prod(jnp.array(cov.shape))
-      return next_cov, diff
+      diffs = diffs.at[iteration // inner_iterations].set(diff)
+      return next_cov, diffs
 
     def init_state() -> Tuple[jnp.ndarray, float]:
       cov_init = jnp.eye(self._dimension)
-      diff = jnp.inf
-      return cov_init, diff
+      diffs = -jnp.ones(
+          (np.ceil(max_iterations / inner_iterations).astype(int),),
+          dtype=dtype
+      )
+      return cov_init, diffs
 
-    # TODO(marcocuturi): ideally the integer parameters below should be passed
-    # by user, if one wants more fine grained control. This could clash with the
-    # parameters passed on to :func:`ott.math.matrix_square_root.sqrtm` by the
-    # barycenter call. At the moment, only `tolerance` can be used to control
-    # computational effort.
-    cov, _ = fixed_point_loop.fixpoint_iter(
+    cov, diffs = fixed_point_loop.fixpoint_iter(
         cond_fn=cond_fn,
         body_fn=body_fn,
-        min_iterations=1,
-        max_iterations=500,
-        inner_iterations=1,
+        min_iterations=min_iterations,
+        max_iterations=max_iterations,
+        inner_iterations=inner_iterations,
         constants=(),
-        state=init_state()
+        state=init_state(),
     )
-    return cov
+    return cov, diffs
 
   def barycenter(
-      self, weights: jnp.ndarray, xs: jnp.ndarray, **kwargs: Any
-  ) -> jnp.ndarray:
+      self,
+      weights: jnp.ndarray,
+      xs: jnp.ndarray,
+      tolerance: float = 1e-4,
+      sqrtm_kw: Optional[Dict[str, Any]] = None,
+      **kwargs: Any
+  ) -> Tuple[jnp.ndarray, jnp.ndarray]:
     """Compute the Bures barycenter of weighted Gaussian distributions.
 
     Implements the fixed point approach proposed in :cite:`alvarez-esteban:16`
     for the computation of the mean and the covariance of the barycenter of
     weighted Gaussian distributions.
 
     Args:
       weights: The barycentric weights.
       xs: The points to be used in the computation of the barycenter, where
         each point is described by a concatenation of the mean and the
         covariance (raveled).
-      kwargs: Passed on to :meth:`covariance_fixpoint_iter`, and by extension to
-        :func:`ott.math.matrix_square_root.sqrtm`. Note that `tolerance` is used
-        for the fixed-point iteration of the barycenter, whereas `threshold`
-        will apply to the fixed point iteration of Newton-Schulz iterations.
+      tolerance: convergence tolerance to control the termination of the
+        algorithm.
+      sqrtm_kw: Arguments passed on to the
+        :func:`~ott.math.matrix_square_root.sqrtm` function used within
+        :meth:`covariance_fixpoint_iter`. This defines the precision
+        (in terms of convergence threshold, and number of iterations) of the
+        matrix square root calls that are used at each outer iteration of
+        the computation of Gaussian barycenters. These values are, by default,
+        the same as those used to define the Bures cost object itself.
+      kwargs: Passed on to :meth:`covariance_fixpoint_iter`, to specify the
+        number of iterations and tolerance of the fixed-point iteration of the
+        barycenter routine, by parameterizing `tolerance` and other relevant
+        arguments passed on to :func:`~ott.math.fixed_point_loop.fixpoint_iter`,
+        namely `min_iterations`, `max_iterations` and `inner_iterations`.
 
     Returns:
-      A concatenation of the mean and the raveled covariance of the barycenter.
+      A list holding a concatenation of the mean and the raveled covariance
+      of the barycenter as its first element, followed by a vector of
+      norms of successive differences in iterates.
     """
     # Ensure that barycentric weights sum to 1.
     weights = weights / jnp.sum(weights)
     mus, covs = x_to_means_and_covs(xs, self._dimension)
     mu_bary = jnp.sum(weights[:, None] * mus, axis=0)
-    cov_bary = self.covariance_fixpoint_iter(
-        covs=covs, weights=weights, **kwargs
+    cov_bary, diffs = self.covariance_fixpoint_iter(
+        covs=covs,
+        weights=weights,
+        tolerance=tolerance,
+        sqrtm_kw=sqrtm_kw if sqrtm_kw is not None else self._sqrtm_kw,
+        **kwargs
     )
-    barycenter = mean_and_cov_to_x(mu_bary, cov_bary, self._dimension)
-    return barycenter
+    return mean_and_cov_to_x(mu_bary, cov_bary, self._dimension), diffs
 
   @classmethod
   def _padder(cls, dim: int) -> jnp.ndarray:
-    """Pad with concatenated zero means and \
-      raveled identity covariance matrix."""
     dimension = int((-1 + math.sqrt(1 + 4 * dim)) / 2)
     padding = mean_and_cov_to_x(
         jnp.zeros((dimension,)), jnp.eye(dimension), dimension
     )
     return padding[jnp.newaxis, :]
 
-  def tree_flatten(self):
+  def tree_flatten(self):  # noqa: D102
     return (), (self._dimension, self._sqrtm_kw)
 
   @classmethod
-  def tree_unflatten(cls, aux_data, children):
+  def tree_unflatten(cls, aux_data, children):  # noqa: D102
     del children
-    return cls(aux_data[0], **aux_data[1])
+    return cls(*aux_data)
 
 
 @jax.tree_util.register_pytree_node_class
 class UnbalancedBures(CostFn):
   """Unbalanced Bures distance between two triplets of `(mass, mean, cov)`.
 
   This cost uses the notation defined in :cite:`janati:20`, eq. 37, 39, 40.
@@ -714,43 +774,123 @@
     pos_signs = (sldet_c + sldet_c_ab + sldet_t_ab + sldet_t_ab) == 4
 
     return jax.lax.cond(
         pos_signs, lambda: 2 * sig2 * mass_x * mass_y - 2 *
         (sig2 + gam) * jnp.exp(log_m_pi), lambda: jnp.nan
     )
 
-  def tree_flatten(self):
+  def tree_flatten(self):  # noqa: D102
     return (), (self._dimension, self._sigma, self._gamma, self._sqrtm_kw)
 
   @classmethod
-  def tree_unflatten(cls, aux_data, children):
+  def tree_unflatten(cls, aux_data, children):  # noqa: D102
     del children
     dim, sigma, gamma, kwargs = aux_data
     return cls(dim, sigma=sigma, gamma=gamma, **kwargs)
 
 
+@jax.tree_util.register_pytree_node_class
+class SoftDTW(CostFn):
+  """Soft dynamic time warping (DTW) cost :cite:`cuturi:17`.
+
+  Args:
+    gamma: Smoothing parameter :math:`> 0` for the soft-min operator.
+    ground_cost: Ground cost function. If ``None``,
+      use :class:`~ott.geometry.costs.SqEuclidean`.
+    debiased: Whether to compute the debiased soft-DTW :cite:`blondel:21`.
+  """
+
+  def __init__(
+      self,
+      gamma: float,
+      ground_cost: Optional[CostFn] = None,
+      debiased: bool = False
+  ):
+    self.gamma = gamma
+    self.ground_cost = SqEuclidean() if ground_cost is None else ground_cost
+    self.debiased = debiased
+
+  def pairwise(self, x: jnp.ndarray, y: jnp.ndarray) -> float:  # noqa: D102
+    c_xy = self._soft_dtw(x, y)
+    if self.debiased:
+      return c_xy - 0.5 * (self._soft_dtw(x, x) + self._soft_dtw(y, y))
+    return c_xy
+
+  def _soft_dtw(self, t1: jnp.ndarray, t2: jnp.ndarray) -> float:
+
+    def body(
+        carry: Tuple[jnp.ndarray, jnp.ndarray],
+        current_antidiagonal: jnp.ndarray
+    ) -> Tuple[Tuple[jnp.ndarray, jnp.ndarray], jnp.ndarray]:
+      # modified from: https://github.com/khdlr/softdtw_jax
+      two_ago, one_ago = carry
+
+      diagonal, right, down = two_ago[:-1], one_ago[:-1], one_ago[1:]
+      best = mu.softmin(
+          jnp.stack([diagonal, right, down], axis=-1), self.gamma, axis=-1
+      )
+
+      next_row = best + current_antidiagonal
+      next_row = jnp.pad(next_row, (1, 0), constant_values=jnp.inf)
+
+      return (one_ago, next_row), next_row
+
+    t1 = t1[:, None] if t1.ndim == 1 else t1
+    t2 = t2[:, None] if t2.ndim == 1 else t2
+    dist = self.ground_cost.all_pairs(t1, t2)
+
+    n, m = dist.shape
+    if n < m:
+      dist = dist.T
+      n, m = m, n
+
+    model_matrix = jnp.full((n + m - 1, n), fill_value=jnp.inf)
+    mask = np.tri(n + m - 1, n, k=0, dtype=bool)
+    mask = mask & mask[::-1, ::-1]
+    model_matrix = model_matrix.T.at[mask.T].set(dist.ravel()).T
+
+    init = (
+        jnp.pad(model_matrix[0], (1, 0), constant_values=jnp.inf),
+        jnp.pad(
+            model_matrix[1] + model_matrix[0, 0], (1, 0),
+            constant_values=jnp.inf
+        )
+    )
+
+    (_, carry), _ = jax.lax.scan(body, init, model_matrix[2:])
+    return carry[-1]
+
+  def tree_flatten(self):  # noqa: D102
+    return (self.gamma, self.ground_cost), {"debiased": self.debiased}
+
+  @classmethod
+  def tree_unflatten(cls, aux_data, children):  # noqa: D102
+    return cls(*children, **aux_data)
+
+
 def x_to_means_and_covs(x: jnp.ndarray,
                         dimension: int) -> Tuple[jnp.ndarray, jnp.ndarray]:
   """Extract means and covariance matrices of Gaussians from raveled vector.
 
   Args:
     x: [num_gaussians, dimension, (1 + dimension)] array of concatenated means
       and covariances (raveled) dimension: the dimension of the Gaussians.
+    dimension: Dimensionality of the Gaussians.
 
   Returns:
-    means: [num_gaussians, dimension] array that holds the means.
-    covariances: [num_gaussians, dimension] array that holds the covariances.
+    Means and covariances of shape ``[num_gaussian, dimension]``.
   """
   x = jnp.atleast_2d(x)
   means = x[:, :dimension]
   covariances = jnp.reshape(
       x[:, dimension:dimension + dimension ** 2], (-1, dimension, dimension)
   )
   return jnp.squeeze(means), jnp.squeeze(covariances)
 
 
 def mean_and_cov_to_x(
     mean: jnp.ndarray, covariance: jnp.ndarray, dimension: int
 ) -> jnp.ndarray:
   """Ravel a Gaussian's mean and covariance matrix to d(1 + d) vector."""
-  x = jnp.concatenate((mean, jnp.reshape(covariance, (dimension * dimension))))
-  return x
+  return jnp.concatenate(
+      (mean, jnp.reshape(covariance, (dimension * dimension)))
+  )
```

### Comparing `ott-jax-0.4.0/src/ott/geometry/epsilon_scheduler.py` & `ott-jax-0.4.1/src/ott/geometry/epsilon_scheduler.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-# Copyright 2022 Google LLC.
+# Copyright OTT-JAX
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-#     http://www.apache.org/licenses/LICENSE-2.0
+#   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""A class to define a scheduler for the entropic regularization epsilon."""
 from typing import Any, Optional
 
 import jax
 import jax.numpy as jnp
 
 __all__ = ["Epsilon"]
 
@@ -31,65 +30,73 @@
   Concretely, the value returned by such a scheduler will consider first
   the max between ``target`` and ``init * target * decay ** iteration``.
   If the ``scale_epsilon`` parameter is provided, that value is used to
   multiply the max computed previously by ``scale_epsilon``.
 
   Args:
     target: the epsilon regularizer that is targeted.
+      If ``None``, use :math:`0.05`.
     scale_epsilon: if passed, used to multiply the regularizer, to rescale it.
+      If ``None``, use :math:`1`.
     init: initial value when using epsilon scheduling, understood as multiple
       of target value. if passed, ``int * decay ** iteration`` will be used
       to rescale target.
-    decay: geometric decay factor, smaller than 1.
+    decay: geometric decay factor, :math:`<1`.
   """
 
-  # TODO(michalk8): directly use the defaults instead of `None`
   def __init__(
       self,
       target: Optional[float] = None,
       scale_epsilon: Optional[float] = None,
-      init: Optional[float] = None,
-      decay: Optional[float] = None
+      init: float = 1.0,
+      decay: float = 1.0
   ):
-    self._target_init = .01 if target is None else target
-    self._scale_epsilon = 1.0 if scale_epsilon is None else scale_epsilon
-    self._init = 1.0 if init is None else init
-    self._decay = 1.0 if decay is None else decay
+    self._target_init = target
+    self._scale_epsilon = scale_epsilon
+    self._init = init
+    self._decay = decay
 
   @property
   def target(self) -> float:
     """Return the final regularizer value of scheduler."""
-    return self._target_init * self._scale_epsilon
+    target = 5e-2 if self._target_init is None else self._target_init
+    scale = 1.0 if self._scale_epsilon is None else self._scale_epsilon
+    return scale * target
 
   def at(self, iteration: Optional[int] = 1) -> float:
     """Return (intermediate) regularizer value at a given iteration."""
     if iteration is None:
       return self.target
     # check the decay is smaller than 1.0.
-    decay = jnp.where(self._decay < 1.0, self._decay, 1.0)
+    decay = jnp.minimum(self._decay, 1.0)
     # the multiple is either 1.0 or a larger init value that is decayed.
     multiple = jnp.maximum(self._init * (decay ** iteration), 1.0)
     return multiple * self.target
 
   def done(self, eps: float) -> bool:
+    """Return whether the scheduler is done at a given value."""
     return eps == self.target
 
   def done_at(self, iteration: Optional[int]) -> bool:
+    """Return whether the scheduler is done at a given iteration."""
     return self.done(self.at(iteration))
 
-  def tree_flatten(self):
+  def set(self, **kwargs: Any) -> "Epsilon":
+    """Return a copy of self, with potential overwrites."""
+    kwargs = {
+        "target": self._target_init,
+        "scale_epsilon": self._scale_epsilon,
+        "init": self._init,
+        "decay": self._decay,
+        **kwargs
+    }
+    return Epsilon(**kwargs)
+
+  def tree_flatten(self):  # noqa: D102
     return (
         self._target_init, self._scale_epsilon, self._init, self._decay
     ), None
 
   @classmethod
-  def tree_unflatten(cls, aux_data, children):
+  def tree_unflatten(cls, aux_data, children):  # noqa: D102
     del aux_data
     return cls(*children)
-
-  @classmethod
-  def make(cls, *args: Any, **kwargs: Any) -> "Epsilon":
-    """Create or return an Epsilon instance."""
-    if isinstance(args[0], cls):
-      return args[0]
-    else:
-      return cls(*args, **kwargs)
```

### Comparing `ott-jax-0.4.0/src/ott/geometry/geometry.py` & `ott-jax-0.4.1/src/ott/geometry/geometry.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-# Copyright 2022 Google LLC.
+# Copyright OTT-JAX
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-#     http://www.apache.org/licenses/LICENSE-2.0
+#   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""A class describing operations used to instantiate and use a geometry."""
 import functools
 from typing import TYPE_CHECKING, Any, Callable, Literal, Optional, Tuple, Union
 
 if TYPE_CHECKING:
   from ott.geometry import low_rank
 
 import jax
@@ -41,100 +40,70 @@
   or more generally exclusively described through a (dissimilarity) cost matrix,
   or almost equivalently, a (similarity) kernel matrix.
 
   Once that cost or kernel matrix is set, the ``Geometry`` class provides a
   basic operations to be run with the Sinkhorn algorithm.
 
   Args:
-    cost_matrix: jnp.ndarray<float>[num_a, num_b]: a cost matrix storing n x m
-      costs.
-    kernel_matrix: jnp.ndarray<float>[num_a, num_b]: a kernel matrix storing n
-      x m kernel values.
-    epsilon: a regularization parameter.
-      If a :class:`~ott.geometry.epsilon_scheduler.Epsilon` scheduler is passed,
-      other parameters below are ignored in practice. If the
-      parameter is a float, then this is understood to be the regularization
-      that is needed, unless ``relative_epsilon`` below is ``True``, in which
-      case ``epsilon`` is understood as a normalized quantity, to be scaled by
-      the mean value of the :attr:`cost_matrix`.
-    relative_epsilon: whether epsilon is passed relative to scale of problem,
-      here understood as mean value of :attr:`cost_matrix`.
-    scale_epsilon: the scale multiplier for epsilon.
+    cost_matrix: Cost matrix of shape ``[n, m]``.
+    kernel_matrix: Kernel matrix of shape ``[n, m]``.
+    epsilon: Regularization parameter. If ``scale_epsilon = None`` and either
+      ``relative_epsilon = True`` or ``relative_epsilon = None`` and
+      ``epsilon = None`` in :class:`~ott.geometry.epsilon_scheduler.Epsilon`
+      is used, ``scale_epsilon`` the is :attr:`mean_cost_matrix`. If
+      ``epsilon = None``, use :math:`0.05`.
+    relative_epsilon: when `False`, the parameter ``epsilon`` specifies the
+      value of the entropic regularization parameter. When `True`, ``epsilon``
+      refers to a fraction of the :attr:`mean_cost_matrix`, which is computed
+      adaptively from data.
     scale_cost: option to rescale the cost matrix. Implemented scalings are
       'median', 'mean' and 'max_cost'. Alternatively, a float factor can be
       given to rescale the cost such that ``cost_matrix /= scale_cost``.
       If `True`, use 'mean'.
     src_mask: Mask specifying valid rows when computing some statistics of
       :attr:`cost_matrix`, see :attr:`src_mask`.
     tgt_mask: Mask specifying valid columns when computing some statistics of
       :attr:`cost_matrix`, see :attr:`tgt_mask`.
-    kwargs: additional kwargs for epsilon scheduler.
 
   Note:
-    When defining a ``Geometry`` through a ``cost_matrix``, it is important to
-    select an ``epsilon`` regularization parameter that is meaningful. That
-    parameter can be provided by the user, or assigned a default value through
-    a simple rule, using the :attr:`mean_cost_matrix`.
+    When defining a :class:`~ott.geometry.geometry.Geometry` through a
+    ``cost_matrix``, it is important to select an ``epsilon`` regularization
+    parameter that is meaningful. That parameter can be provided by the user,
+    or assigned a default value through a simple rule,
+    using the :attr:`mean_cost_matrix`.
   """
 
   def __init__(
       self,
       cost_matrix: Optional[jnp.ndarray] = None,
       kernel_matrix: Optional[jnp.ndarray] = None,
-      epsilon: Union[epsilon_scheduler.Epsilon, float, None] = None,
+      epsilon: Optional[Union[float, epsilon_scheduler.Epsilon]] = None,
       relative_epsilon: Optional[bool] = None,
-      scale_epsilon: Optional[float] = None,
+      scale_cost: Union[bool, int, float, Literal["mean", "max_cost",
+                                                  "median"]] = 1.0,
       src_mask: Optional[jnp.ndarray] = None,
       tgt_mask: Optional[jnp.ndarray] = None,
-      scale_cost: Union[bool, int, float, Literal['mean', 'max_cost',
-                                                  'median']] = 1.0,
-      **kwargs: Any,
   ):
     self._cost_matrix = cost_matrix
     self._kernel_matrix = kernel_matrix
-    self._epsilon_init = epsilon
+
+    # needed for `copy_epsilon`, because of the `isinstance` check
+    self._epsilon_init = epsilon if isinstance(
+        epsilon, epsilon_scheduler.Epsilon
+    ) else epsilon_scheduler.Epsilon(epsilon)
     self._relative_epsilon = relative_epsilon
-    self._scale_epsilon = scale_epsilon
+
     self._scale_cost = "mean" if scale_cost is True else scale_cost
+
     self._src_mask = src_mask
     self._tgt_mask = tgt_mask
-    # Define default dictionary and update it with user's values.
-    self._kwargs = {**{'init': None, 'decay': None}, **kwargs}
 
   @property
   def cost_rank(self) -> Optional[int]:
     """Output rank of cost matrix, if any was provided."""
-    return None
-
-  @property
-  def scale_epsilon(self) -> float:
-    """Compute the scale of the epsilon, potentially based on data."""
-    if isinstance(self._epsilon_init, epsilon_scheduler.Epsilon):
-      return 1.0
-
-    rel = self._relative_epsilon
-    trigger = ((self._scale_epsilon is None) and
-               ((rel is None and self._epsilon_init is None) or rel))
-
-    if (self._scale_epsilon is None) and (trigger is not None):  # for dry run
-      return jnp.where(
-          trigger, jax.lax.stop_gradient(self.mean_cost_matrix), 1.0
-      )
-    else:
-      return self._scale_epsilon
-
-  @property
-  def _epsilon(self) -> epsilon_scheduler.Epsilon:
-    """Return epsilon scheduler, either passed directly or by building it."""
-    if isinstance(self._epsilon_init, epsilon_scheduler.Epsilon):
-      return self._epsilon_init
-    eps = 5e-2 if self._epsilon_init is None else self._epsilon_init
-    return epsilon_scheduler.Epsilon.make(
-        eps, scale_epsilon=self.scale_epsilon, **self._kwargs
-    )
 
   @property
   def cost_matrix(self) -> jnp.ndarray:
     """Cost matrix, recomputed from kernel if only kernel was specified."""
     if self._cost_matrix is None:
       # If no epsilon was passed on to the geometry, then assume it is one by
       # default.
@@ -154,21 +123,39 @@
   def mean_cost_matrix(self) -> float:
     """Mean of the :attr:`cost_matrix`."""
     tmp = self._masked_geom().apply_cost(self._n_normed_ones).squeeze()
     return jnp.sum(tmp * self._m_normed_ones)
 
   @property
   def kernel_matrix(self) -> jnp.ndarray:
-    """Kernel matrix, either provided by user or recomputed from \
-     :attr:`cost_matrix`."""
+    """Kernel matrix.
+
+    Either provided by user or recomputed from :attr:`cost_matrix`.
+    """
     if self._kernel_matrix is None:
       return jnp.exp(-(self._cost_matrix * self.inv_scale_cost / self.epsilon))
     return self._kernel_matrix ** self.inv_scale_cost
 
   @property
+  def _epsilon(self) -> epsilon_scheduler.Epsilon:
+    (target, scale_eps, _, _), _ = self._epsilon_init.tree_flatten()
+    rel = self._relative_epsilon
+
+    use_mean_scale = rel is True or (rel is None and target is None)
+    if scale_eps is None and use_mean_scale:
+      scale_eps = jax.lax.stop_gradient(self.mean_cost_matrix)
+
+    if isinstance(self._epsilon_init, epsilon_scheduler.Epsilon):
+      return self._epsilon_init.set(scale_epsilon=scale_eps)
+
+    return epsilon_scheduler.Epsilon(
+        target=5e-2 if target is None else target, scale_epsilon=scale_eps
+    )
+
+  @property
   def epsilon(self) -> float:
     """Epsilon regularization value."""
     return self._epsilon.target
 
   @property
   def shape(self) -> Tuple[int, int]:
     """Shape of the geometry."""
@@ -180,21 +167,21 @@
     return 0, 0
 
   @property
   def can_LRC(self) -> bool:
     """Check quickly if casting geometry as LRC makes sense.
 
     This check is only carried out using basic considerations from the geometry,
-    not using a rigorous check involving, e.g., svd.
+    not using a rigorous check involving, e.g., SVD.
     """
     return False
 
   @property
   def is_squared_euclidean(self) -> bool:
-    """Whether cost is computed by taking squared-Eucl. distance of points."""
+    """Whether cost is computed by taking squared Euclidean distance."""
     return False
 
   @property
   def is_online(self) -> bool:
     """Whether geometry cost/kernel should be recomputed on the fly."""
     return False
 
@@ -209,52 +196,62 @@
   @property
   def inv_scale_cost(self) -> float:
     """Compute and return inverse of scaling factor for cost matrix."""
     if isinstance(self._scale_cost,
                   (int, float)) or utils.is_jax_array(self._scale_cost):
       return 1.0 / self._scale_cost
     self = self._masked_geom(mask_value=jnp.nan)
-    if self._scale_cost == 'max_cost':
+    if self._scale_cost == "max_cost":
       return 1.0 / jnp.nanmax(self._cost_matrix)
-    if self._scale_cost == 'mean':
+    if self._scale_cost == "mean":
       return 1.0 / jnp.nanmean(self._cost_matrix)
-    if self._scale_cost == 'median':
+    if self._scale_cost == "median":
       return 1.0 / jnp.nanmedian(self._cost_matrix)
-    raise ValueError(f'Scaling {self._scale_cost} not implemented.')
+    raise ValueError(f"Scaling {self._scale_cost} not implemented.")
 
-  def _set_scale_cost(self, scale_cost: Union[bool, float, str]) -> "Geometry":
+  def set_scale_cost(self, scale_cost: Union[bool, float, str]) -> "Geometry":
+    """Modify how to rescale of the :attr:`cost_matrix`."""
     # case when `geom` doesn't have `scale_cost` or doesn't need to be modified
     # `False` retains the original scale
     if scale_cost is False or scale_cost == self._scale_cost:
       return self
     children, aux_data = self.tree_flatten()
     aux_data["scale_cost"] = scale_cost
     return type(self).tree_unflatten(aux_data, children)
 
-  def copy_epsilon(self, other: 'Geometry') -> "Geometry":
+  def copy_epsilon(self, other: "Geometry") -> "Geometry":
     """Copy the epsilon parameters from another geometry."""
-    scheduler = other._epsilon
-    self._epsilon_init = scheduler._target_init
-    self._relative_epsilon = False
-    self._scale_epsilon = other.scale_epsilon
-    return self
+    other_epsilon = other._epsilon
+    children, aux_data = self.tree_flatten()
+
+    new_children = []
+    for child in children:
+      if isinstance(child, epsilon_scheduler.Epsilon):
+        child = child.set(
+            target=other_epsilon._target_init,
+            scale_epsilon=other_epsilon._scale_epsilon
+        )
+      new_children.append(child)
+
+    aux_data["relative_epsilon"] = False
+    return type(self).tree_unflatten(aux_data, new_children)
 
   # The functions below are at the core of Sinkhorn iterations, they
   # are implemented here in their default form, either in lse (using directly
   # cost matrices in stabilized form) or kernel mode (using kernel matrices).
 
   def apply_lse_kernel(
       self,
       f: jnp.ndarray,
       g: jnp.ndarray,
       eps: float,
       vec: jnp.ndarray = None,
       axis: int = 0
   ) -> jnp.ndarray:
-    r"""Apply :attr:`kernel_matrix` in log domain on a pair of dual potential variables.
+    r"""Apply :attr:`kernel_matrix` in log domain.
 
     This function applies the ground geometry's kernel in log domain, using
     a stabilized formulation. At a high level, this iteration performs either:
 
     - output = eps * log (K (exp(g / eps) * vec))  (1)
     - output = eps * log (K'(exp(f / eps) * vec))  (2)
 
@@ -267,16 +264,16 @@
 
     Args:
       f: jnp.ndarray [num_a,] , potential of size num_rows of cost_matrix
       g: jnp.ndarray [num_b,] , potential of size num_cols of cost_matrix
       eps: float, regularization strength
       vec: jnp.ndarray [num_a or num_b,] , when not None, this has the effect of
         doing log-Kernel computations with an addition elementwise
-        multiplication of exp(g / eps) by a vector. This is carried out by adding
-        weights to the log-sum-exp function, and needs to handle signs
+        multiplication of exp(g / eps) by a vector. This is carried out by
+        adding weights to the log-sum-exp function, and needs to handle signs
         separately.
       axis: summing over axis 0 when doing (2), or over axis 1 when doing (1)
 
     Returns:
       A jnp.ndarray corresponding to output above, depending on axis.
     """
     w_res, w_sgn = self._softmax(f, g, eps, vec, axis)
@@ -287,19 +284,14 @@
       self,
       scaling: jnp.ndarray,
       eps: Optional[float] = None,
       axis: int = 0,
   ) -> jnp.ndarray:
     """Apply :attr:`kernel_matrix` on positive scaling vector.
 
-    This function applies the ground geometry's kernel, to perform either
-    output = K v    (1)
-    output = K'u   (2)
-    where K is [num_a, num_b]
-
     Args:
       scaling: jnp.ndarray [num_a or num_b] , scaling of size num_rows or
         num_cols of kernel_matrix
       eps: passed for consistency, not used yet.
       axis: standard kernel product if axis is 1, transpose if 0.
 
     Returns:
@@ -318,15 +310,15 @@
       f: jnp.ndarray,
       g: jnp.ndarray,
       axis: int = 0,
   ) -> jnp.ndarray:
     """Output marginal of transportation matrix from potentials.
 
     This applies first lse kernel in the standard way, removes the
-    correction used to stabilise computations, and lifts this with an exp to
+    correction used to stabilize computations, and lifts this with an exp to
     recover either of the marginals corresponding to the transport map induced
     by potentials.
 
     Args:
       f: jnp.ndarray [num_a,] , potential of size num_rows of cost_matrix
       g: jnp.ndarray [num_b,] , potential of size num_cols of cost_matrix
       axis: axis along which to integrate, returns marginal on other axis.
@@ -421,19 +413,19 @@
     if vec is not None:
       if axis == 0:
         vec = vec.reshape((-1, 1))
       lse_output = mu.logsumexp(
           self._center(f, g) / eps, b=vec, axis=axis, return_sign=True
       )
       return eps * lse_output[0], lse_output[1]
-    else:
-      lse_output = mu.logsumexp(
-          self._center(f, g) / eps, axis=axis, return_sign=False
-      )
-      return eps * lse_output, jnp.array([1.0])
+
+    lse_output = mu.logsumexp(
+        self._center(f, g) / eps, axis=axis, return_sign=False
+    )
+    return eps * lse_output, jnp.array([1.0])
 
   @functools.partial(jax.vmap, in_axes=[None, None, None, 0, None])
   def _apply_transport_from_potentials(
       self, f: jnp.ndarray, g: jnp.ndarray, vec: jnp.ndarray, axis: int
   ) -> jnp.ndarray:
     """Apply lse_kernel to arbitrary vector while keeping track of signs."""
     lse_res, lse_sgn = self.apply_lse_kernel(
@@ -613,29 +605,29 @@
       *args: Any,
       static_b: bool = False,
       **kwargs: Any
   ) -> Tuple["Geometry", ...]:
     """Instantiate 2 (or 3) geometries to compute a Sinkhorn divergence."""
     size = 2 if static_b else 3
     nones = [None, None, None]
-    cost_matrices = kwargs.pop('cost_matrix', args)
-    kernel_matrices = kwargs.pop('kernel_matrix', nones)
+    cost_matrices = kwargs.pop("cost_matrix", args)
+    kernel_matrices = kwargs.pop("kernel_matrix", nones)
     cost_matrices = cost_matrices if cost_matrices is not None else nones
     return tuple(
         cls(cost_matrix=arg1, kernel_matrix=arg2, **kwargs)
         for arg1, arg2, _ in zip(cost_matrices, kernel_matrices, range(size))
     )
 
   def to_LRCGeometry(
       self,
       rank: int = 0,
       tol: float = 1e-2,
-      seed: int = 0,
+      rng: Optional[jax.random.PRNGKeyArray] = None,
       scale: float = 1.
-  ) -> 'low_rank.LRCGeometry':
+  ) -> "low_rank.LRCGeometry":
     r"""Factorize the cost matrix using either SVD (full) or :cite:`indyk:19`.
 
     When `rank=min(n,m)` or `0` (by default), use :func:`jax.numpy.linalg.svd`.
 
     For other values, use the routine in sublinear time :cite:`indyk:19`.
     Uses the implementation of :cite:`scetbon:21`, algorithm 4.
 
@@ -644,15 +636,15 @@
     where :math:`A` is ``n x m`` cost matrix, :math:`UV` the factorization
     computed in sublinear time and :math:`A_k` the best rank-k approximation.
 
     Args:
       rank: Target rank of the :attr:`cost_matrix`.
       tol: Tolerance of the error. The total number of sampled points is
         :math:`min(n, m,\frac{rank}{tol})`.
-      seed: Random seed.
+      rng: The PRNG key to use for initializing the model.
       scale: Value used to rescale the factors of the low-rank geometry.
         Useful when this geometry is used in the linear term of fused GW.
 
     Returns:
       Low-rank geometry.
     """
     from ott.geometry import low_rank
@@ -666,104 +658,99 @@
           full_matrices=False,
           compute_uv=True,
       )
 
       cost_1 = u
       cost_2 = (s[:, None] * vh).T
     else:
-      rng = jax.random.PRNGKey(seed)
-      key1, key2, key3, key4, key5 = jax.random.split(rng, 5)
+      rng = utils.default_prng_key(rng)
+      rng1, rng2, rng3, rng4, rng5 = jax.random.split(rng, 5)
       n_subset = min(int(rank / tol), n, m)
 
-      i_star = jax.random.randint(key1, shape=(), minval=0, maxval=n)
-      j_star = jax.random.randint(key2, shape=(), minval=0, maxval=m)
+      i_star = jax.random.randint(rng1, shape=(), minval=0, maxval=n)
+      j_star = jax.random.randint(rng2, shape=(), minval=0, maxval=m)
 
-      # force `batch_size=None` since `cost_matrix` would be `None`
-      ci_star = self.subset(
-          i_star, None, batch_size=None
-      ).cost_matrix.ravel() ** 2  # (m,)
-      cj_star = self.subset(
-          None, j_star, batch_size=None
-      ).cost_matrix.ravel() ** 2  # (n,)
+      ci_star = self.subset(i_star, None).cost_matrix.ravel() ** 2  # (m,)
+      cj_star = self.subset(None, j_star).cost_matrix.ravel() ** 2  # (n,)
 
       p_row = cj_star + ci_star[j_star] + jnp.mean(ci_star)  # (n,)
       p_row /= jnp.sum(p_row)
-      row_ixs = jax.random.choice(key3, n, shape=(n_subset,), p=p_row)
+      row_ixs = jax.random.choice(rng3, n, shape=(n_subset,), p=p_row)
       # (n_subset, m)
-      s = self.subset(row_ixs, None, batch_size=None).cost_matrix
+      s = self.subset(row_ixs, None).cost_matrix
       s /= jnp.sqrt(n_subset * p_row[row_ixs][:, None])
 
       p_col = jnp.sum(s ** 2, axis=0)  # (m,)
       p_col /= jnp.sum(p_col)
       # (n_subset,)
-      col_ixs = jax.random.choice(key4, m, shape=(n_subset,), p=p_col)
+      col_ixs = jax.random.choice(rng4, m, shape=(n_subset,), p=p_col)
       # (n_subset, n_subset)
       w = s[:, col_ixs] / jnp.sqrt(n_subset * p_col[col_ixs][None, :])
 
       U, _, V = jsp.linalg.svd(w)
       U = U[:, :rank]  # (n_subset, rank)
       U = (s.T @ U) / jnp.linalg.norm(w.T @ U, axis=0)  # (m, rank)
 
       _, d, v = jnp.linalg.svd(U.T @ U)  # (k,), (k, k)
       v = v.T / jnp.sqrt(d)[None, :]
 
       inv_scale = (1. / jnp.sqrt(n_subset))
-      col_ixs = jax.random.choice(key5, m, shape=(n_subset,))  # (n_subset,)
+      col_ixs = jax.random.choice(rng5, m, shape=(n_subset,))  # (n_subset,)
 
       # (n, n_subset)
-      A_trans = self.subset(
-          None, col_ixs, batch_size=None
-      ).cost_matrix * inv_scale
+      A_trans = self.subset(None, col_ixs).cost_matrix * inv_scale
       B = (U[col_ixs, :] @ v * inv_scale)  # (n_subset, k)
       M = jnp.linalg.inv(B.T @ B)  # (k, k)
       V = jnp.linalg.multi_dot([A_trans, B, M.T, v.T])  # (n, k)
       cost_1 = V
       cost_2 = U
 
     return low_rank.LRCGeometry(
         cost_1=cost_1,
         cost_2=cost_2,
         epsilon=self._epsilon_init,
         relative_epsilon=self._relative_epsilon,
-        scale=self._scale_epsilon,
         scale_cost=self._scale_cost,
         scale_factor=scale,
-        **self._kwargs
     )
 
   def subset(
       self, src_ixs: Optional[jnp.ndarray], tgt_ixs: Optional[jnp.ndarray],
       **kwargs: Any
   ) -> "Geometry":
     """Subset rows or columns of a geometry.
 
     Args:
       src_ixs: Row indices. If ``None``, use all rows.
       tgt_ixs: Column indices. If ``None``, use all columns.
       kwargs: Keyword arguments to override the initialization.
 
     Returns:
-      The subsetted geometry.
+      The modified geometry.
     """
 
     def subset_fn(
         arr: Optional[jnp.ndarray],
         src_ixs: Optional[jnp.ndarray],
         tgt_ixs: Optional[jnp.ndarray],
     ) -> Optional[jnp.ndarray]:
       if arr is None:
         return None
       if src_ixs is not None:
         arr = arr[jnp.atleast_1d(src_ixs)]
       if tgt_ixs is not None:
         arr = arr[:, jnp.atleast_1d(tgt_ixs)]
-      return arr
+      return arr  # noqa: RET504
 
     return self._mask_subset_helper(
-        src_ixs, tgt_ixs, fn=subset_fn, propagate_mask=True, **kwargs
+        src_ixs,
+        tgt_ixs,
+        fn=subset_fn,
+        propagate_mask=True,
+        **kwargs,
     )
 
   def mask(
       self,
       src_mask: Optional[jnp.ndarray],
       tgt_mask: Optional[jnp.ndarray],
       mask_value: float = 0.,
@@ -796,15 +783,15 @@
       if arr is None:
         return arr
       assert arr.ndim == 2, arr.ndim
       if src_mask is not None:
         arr = jnp.where(src_mask[:, None], arr, mask_value)
       if tgt_mask is not None:
         arr = jnp.where(tgt_mask[None, :], arr, mask_value)
-      return arr
+      return arr  # noqa: RET504
 
     src_mask = self._normalize_mask(src_mask, self.shape[0])
     tgt_mask = self._normalize_mask(tgt_mask, self.shape[1])
     return self._mask_subset_helper(
         src_mask, tgt_mask, fn=mask_fn, propagate_mask=False
     )
 
@@ -815,27 +802,26 @@
       *,
       fn: Callable[
           [Optional[jnp.ndarray], Optional[jnp.ndarray], Optional[jnp.ndarray]],
           Optional[jnp.ndarray]],
       propagate_mask: bool,
       **kwargs: Any,
   ) -> "Geometry":
-    (cost, kernel, *children, src_mask, tgt_mask,
-     kws), aux_data = self.tree_flatten()
+    (cost, kernel, eps, src_mask, tgt_mask), aux_data = self.tree_flatten()
     cost = fn(cost, src_ixs, tgt_ixs)
     kernel = fn(kernel, src_ixs, tgt_ixs)
     if propagate_mask:
       src_mask = self._normalize_mask(src_mask, self.shape[0])
       tgt_mask = self._normalize_mask(tgt_mask, self.shape[1])
       src_mask = fn(src_mask, src_ixs, None)
       tgt_mask = fn(tgt_mask, tgt_ixs, None)
 
     aux_data = {**aux_data, **kwargs}
     return type(self).tree_unflatten(
-        aux_data, [cost, kernel] + children + [src_mask, tgt_mask, kws]
+        aux_data, [cost, kernel, eps, src_mask, tgt_mask]
     )
 
   @property
   def src_mask(self) -> Optional[jnp.ndarray]:
     """Mask of shape ``[num_a,]`` to compute :attr:`cost_matrix` statistics.
 
     Specifically, it is used when computing:
@@ -870,24 +856,22 @@
     src_mask, tgt_mask = self.src_mask, self.tgt_mask
     if src_mask is None and tgt_mask is None:
       return self
     return self.mask(src_mask, tgt_mask, mask_value=mask_value)
 
   @property
   def _n_normed_ones(self) -> jnp.ndarray:
-    """Normalized array of shape ``[num_a,]`` \
-    taking into account :attr:`src_mask`."""
+    """Normalized array of shape ``[num_a,]``."""
     mask = self.src_mask
     arr = jnp.ones(self.shape[0]) if mask is None else mask
     return arr / jnp.sum(arr)
 
   @property
   def _m_normed_ones(self) -> jnp.ndarray:
-    """Normalized array of shape ``[num_b,]`` \
-    taking into account :attr:`tgt_mask`."""
+    """Normalized array of shape ``[num_b,]``."""
     mask = self.tgt_mask
     arr = jnp.ones(self.shape[1]) if mask is None else mask
     return arr / jnp.sum(arr)
 
   @staticmethod
   def _normalize_mask(mask: Optional[Union[int, jnp.ndarray]],
                       size: int) -> Optional[jnp.ndarray]:
@@ -896,27 +880,29 @@
       return None
     mask = jnp.atleast_1d(mask)
     if not jnp.issubdtype(mask, (bool, jnp.bool_)):
       mask = jnp.isin(jnp.arange(size), mask)
     assert mask.shape == (size,)
     return mask
 
-  def tree_flatten(self):
+  def tree_flatten(self):  # noqa: D102
     return (
         self._cost_matrix, self._kernel_matrix, self._epsilon_init,
-        self._relative_epsilon, self._scale_epsilon, self._src_mask,
-        self._tgt_mask, self._kwargs
+        self._src_mask, self._tgt_mask
     ), {
-        'scale_cost': self._scale_cost
+        "scale_cost": self._scale_cost,
+        "relative_epsilon": self._relative_epsilon
     }
 
   @classmethod
-  def tree_unflatten(cls, aux_data, children):
-    *args, kwargs = children
-    return cls(*args, **kwargs, **aux_data)
+  def tree_unflatten(cls, aux_data, children):  # noqa: D102
+    cost, kernel, eps, src_mask, tgt_mask = children
+    return cls(
+        cost, kernel, eps, src_mask=src_mask, tgt_mask=tgt_mask, **aux_data
+    )
 
 
 def is_affine(fn) -> bool:
   """Test heuristically if a function is affine."""
   x = jnp.arange(10.0)
   out = jax.vmap(jax.grad(fn))(x)
   return jnp.sum(jnp.diff(jnp.abs(out))) == 0.0
```

### Comparing `ott-jax-0.4.0/src/ott/geometry/grid.py` & `ott-jax-0.4.1/src/ott/geometry/grid.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-# Copyright 2022 Google LLC.
+# Copyright OTT-JAX
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-#     http://www.apache.org/licenses/LICENSE-2.0
+#   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Implements a geometry class for points supported on a cartesian product."""
 import itertools
 from typing import Any, List, NoReturn, Optional, Sequence, Tuple
 
 import jax
 import jax.numpy as jnp
 import numpy as np
 
@@ -26,15 +25,15 @@
 
 
 @jax.tree_util.register_pytree_node_class
 class Grid(geometry.Geometry):
   r"""Class describing the geometry of points taken in a Cartesian product.
 
   This class implements a geometry in which probability measures are supported
-  on a :math:`d`-dimensional cartesian grid, a cartesian product of :math:`d`
+  on a :math:`d`-dimensional Cartesian grid, a Cartesian product of :math:`d`
   lists of values, each list being itself of size :math:`n_i`.
 
   The transportation cost between points in the grid is assumed to be separable,
   namely a sum of coordinate-wise cost functions, as in:
 
   .. math::
 
@@ -56,23 +55,22 @@
       Locations are provided as a list of arrays, that is :math:`d`
       vectors of (possibly varying) size :math:`n_i`. The resulting grid
       is the Cartesian product of these vectors.
     grid_size: tuple of integers describing grid sizes, namely
       :math:`(n_1,...,n_d)`. This will only be used if x is None.
       In that case the grid will be assumed to lie in the hypercube
       :math:`[0,1]^d`, with the :math:`d` dimensions, described as points
-      regularly sampled in [0,1].
-    cost_fns: a sequence of :math:`d` costs.CostFn's, each being a cost taking
+      regularly sampled in :math:`[0,1]`.
+    cost_fns: a sequence of :math:`d` cost functions, each being a cost taking
       two reals as inputs to output a real number.
     num_a: total size of grid. This parameters will be computed from other
-      inputs and used in the flatten/unflatten functions.
+      inputs.
     grid_dimension: dimension of grid. This parameters will be computed from
-      other inputs and used in the flatten/unflatten functions.
-    kwargs: other optional parameters to be passed on to superclass
-      initializer, notably those related to epsilon regularization.
+      other inputs.
+    kwargs: keyword arguments for :class:`~ott.geometry.geometry.Geometry`.
   """
 
   def __init__(
       self,
       x: Optional[Sequence[jnp.ndarray]] = None,
       grid_size: Optional[Sequence[int]] = None,
       cost_fns: Optional[Sequence[costs.CostFn]] = None,
@@ -95,56 +93,58 @@
       self.grid_dimension = len(self.x)
     elif grid_size is not None:
       self.grid_size = tuple(map(int, grid_size))
       self.x = tuple(jnp.linspace(0, 1, n) for n in self.grid_size)
       self.num_a = np.prod(np.array(grid_size))
       self.grid_dimension = len(self.grid_size)
     else:
-      raise ValueError('Input either grid_size t-uple or grid locations x.')
+      raise ValueError("Input either grid_size tuple or grid locations x.")
 
     if cost_fns is None:
       cost_fns = [costs.SqEuclidean()]
     self.cost_fns = cost_fns
     self.kwargs = {
-        'num_a': self.num_a,
-        'grid_size': self.grid_size,
-        'grid_dimension': self.grid_dimension
+        "num_a": self.num_a,
+        "grid_size": self.grid_size,
+        "grid_dimension": self.grid_dimension
     }
 
     super().__init__(**kwargs)
 
   @property
   def geometries(self) -> List[geometry.Geometry]:
     """Cost matrices along each dimension of the grid."""
     geometries = []
     for dimension, cost_fn in itertools.zip_longest(
         range(self.grid_dimension), self.cost_fns, fillvalue=self.cost_fns[-1]
     ):
       x_values = self.x[dimension][:, jnp.newaxis]
       geom = pointcloud.PointCloud(
-          x_values, cost_fn=cost_fn, epsilon=self._epsilon_init
+          x_values,
+          cost_fn=cost_fn,
+          epsilon=self._epsilon_init,
       )
       geometries.append(geom)
     return geometries
 
   @property
   def median_cost_matrix(self) -> NoReturn:
     """Not implemented."""
-    raise NotImplementedError('Median cost not implemented for grids.')
+    raise NotImplementedError("Median cost not implemented for grids.")
 
   @property
-  def can_LRC(self) -> bool:
+  def can_LRC(self) -> bool:  # noqa: D102
     return True
 
   @property
-  def shape(self) -> Tuple[int, int]:
+  def shape(self) -> Tuple[int, int]:  # noqa: D102
     return self.num_a, self.num_a
 
   @property
-  def is_symmetric(self) -> bool:
+  def is_symmetric(self) -> bool:  # noqa: D102
     return True
 
   # Reimplemented functions to be used in regularized OT
   def apply_lse_kernel(
       self,
       f: jnp.ndarray,
       g: jnp.ndarray,
@@ -289,29 +289,29 @@
     return scaling.ravel()
 
   def transport_from_potentials(
       self, f: jnp.ndarray, g: jnp.ndarray, axis: int = 0
   ) -> NoReturn:
     """Not implemented, use :meth:`apply_transport_from_potentials` instead."""
     raise ValueError(
-        'Grid geometry cannot instantiate a transport matrix, use',
-        ' apply_transport_from_potentials(...) if you wish to ',
-        ' apply the transport matrix to a vector, or use a point '
-        ' cloud geometry instead'
+        "Grid geometry cannot instantiate a transport matrix, use",
+        " apply_transport_from_potentials(...) if you wish to ",
+        " apply the transport matrix to a vector, or use a point "
+        " cloud geometry instead"
     )
 
   def transport_from_scalings(
       self, f: jnp.ndarray, g: jnp.ndarray, axis: int = 0
   ) -> NoReturn:
     """Not implemented, use :meth:`apply_transport_from_scalings` instead."""
     raise ValueError(
-        'Grid geometry cannot instantiate a transport matrix, use ',
-        'apply_transport_from_scalings(...) if you wish to ',
-        'apply the transport matrix to a vector, or use a point '
-        'cloud geometry instead.'
+        "Grid geometry cannot instantiate a transport matrix, use ",
+        "apply_transport_from_scalings(...) if you wish to ",
+        "apply the transport matrix to a vector, or use a point "
+        "cloud geometry instead."
     )
 
   def subset(
       self, src_ixs: Optional[jnp.ndarray], tgt_ixs: Optional[jnp.ndarray]
   ) -> NoReturn:
     """Not implemented."""
     raise NotImplementedError("Subsetting is not implemented for grids.")
@@ -329,59 +329,59 @@
   def prepare_divergences(
       cls,
       *args: Any,
       static_b: bool = False,
       **kwargs: Any
   ) -> Tuple["Grid", ...]:
     """Instantiate the geometries used for a divergence computation."""
-    grid_size = kwargs.pop('grid_size', None)
-    x = kwargs.pop('x', args)
+    grid_size = kwargs.pop("grid_size", None)
+    x = kwargs.pop("x", args)
 
     sep_grid = cls(x=x, grid_size=grid_size, **kwargs)
     size = 2 if static_b else 3
     return tuple(sep_grid for _ in range(size))
 
   @property
-  def dtype(self) -> jnp.dtype:
+  def dtype(self) -> jnp.dtype:  # noqa: D102
     return self.x[0].dtype
 
-  def tree_flatten(self):
-    return (self.x, self.cost_fns, self._epsilon), self.kwargs
+  def tree_flatten(self):  # noqa: D102
+    return (self.x, self.cost_fns, self._epsilon_init), self.kwargs
 
   @classmethod
-  def tree_unflatten(cls, aux_data, children):
+  def tree_unflatten(cls, aux_data, children):  # noqa: D102
     return cls(
         x=children[0], cost_fns=children[1], epsilon=children[2], **aux_data
     )
 
   def to_LRCGeometry(
       self,
       scale: float = 1.0,
       **kwargs: Any,
   ) -> low_rank.LRCGeometry:
     """Converts grid to low-rank geometry.
 
     Conversion is carried out by taking advantage of the fact that the true cost
-    matrix of a grid geometry is a sum of kronecker products of local cost
-    matrices (for each dimension) with matrice of 1's (both on left and right
+    matrix of a grid geometry is a sum of Kronecker products of local cost
+    matrices (for each dimension) with matrices of 1's (both on left and right
     sides) of varying dimension. Each of the matrices in that sum can be
     factorized if each of these cost matrices can be factorized, which we do
     by forcing a conversion to a low rank geometry object.
 
     Args:
       scale: Value used to rescale the factors of the low-rank geometry.
         Useful when this geometry is used in the linear term of fused GW.
       kwargs: Keyword arguments, such as ``rank``, to
         :meth:`~ott.geometry.geometry.Geometry.to_LRCGeometry` used when
         geometries on each slice are not low-rank.
+
     Returns:
       :class:`~ott.geometry.low_rank.LRCGeometry` object.
     """
-    cost_1 = []
-    cost_2 = []
+    cost_1, cost_2 = [], []
     for dimension, geom in enumerate(self.geometries):
       # An overall low-rank conversion of the cost matrix on a grid, to an
       # object of :class:`~ott.geometry.low_rank.LRCGeometry`, necesitates an
       # exact low-rank matrix decompisition of the cost matrix of each slice
       # of that grid, even if costs on such slices are not low-rank.
       # The idea here is that even if the cost matrix on slice `i` is full rank
       # `n_i`, we are better off doing 2 redundant `n_i x n_i` matrix products,
@@ -405,13 +405,11 @@
 
     return low_rank.LRCGeometry(
         cost_1=cost_1,
         cost_2=cost_2,
         scale_factor=scale,
         epsilon=self._epsilon_init,
         relative_epsilon=self._relative_epsilon,
-        scale=self._scale_epsilon,
         scale_cost=self._scale_cost,
         src_mask=self.src_mask,
         tgt_mask=self.tgt_mask,
-        **self._kwargs
     )
```

### Comparing `ott-jax-0.4.0/src/ott/geometry/low_rank.py` & `ott-jax-0.4.1/src/ott/geometry/low_rank.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-# Copyright 2022 Google LLC.
+# Copyright OTT-JAX
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-#     http://www.apache.org/licenses/LICENSE-2.0
+#   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""A class describing low-rank geometries."""
 from typing import Any, Callable, Literal, Optional, Tuple, Union
 
 import jax
 import jax.numpy as jnp
 
 from ott import utils
 from ott.geometry import geometry
@@ -44,37 +43,34 @@
       factor can be given to rescale the cost such that
       ``cost_matrix /= scale_cost``. If `True`, use 'mean'.
     batch_size: optional size of the batch to compute online (without
       instantiating the matrix) the scale factor ``scale_cost`` of the
       :attr:`cost_matrix` when ``scale_cost = 'max_cost'``. If `None`, the batch
       size is set to `1024` or to the largest number of samples between
       :attr:`cost_1` and :attr:`cost_2` if smaller than `1024`.
-    kwargs: Additional keyword arguments for
-      :class:`~ott.geometry.geometry.Geometry`.
+    kwargs: keyword arguments for :class:`~ott.geometry.geometry.Geometry`.
   """
 
   def __init__(
       self,
       cost_1: jnp.ndarray,
       cost_2: jnp.ndarray,
-      bias: float = 0.,
-      scale_factor: float = 1.,
-      scale_cost: Union[bool, int, float, Literal['mean', 'max_bound',
-                                                  'max_cost']] = 1.0,
+      bias: float = 0.0,
+      scale_factor: float = 1.0,
+      scale_cost: Union[bool, int, float, Literal["mean", "max_bound",
+                                                  "max_cost"]] = 1.0,
       batch_size: Optional[int] = None,
       **kwargs: Any,
   ):
+    super().__init__(**kwargs)
     self._cost_1 = cost_1
     self._cost_2 = cost_2
     self._bias = bias
     self._scale_factor = scale_factor
-    self._kwargs = kwargs
-
-    super().__init__(**kwargs)
-    self._scale_cost = 'mean' if scale_cost is True else scale_cost
+    self._scale_cost = "mean" if scale_cost is True else scale_cost
     self.batch_size = batch_size
 
   @property
   def cost_1(self) -> jnp.ndarray:
     """First factor of the :attr:`cost_matrix`."""
     scale_factor = jnp.sqrt(self._scale_factor * self.inv_scale_cost)
     return scale_factor * self._cost_1
@@ -87,68 +83,68 @@
 
   @property
   def bias(self) -> float:
     """Constant offset added to the entire :attr:`cost_matrix`."""
     return self._bias * self.inv_scale_cost
 
   @property
-  def cost_rank(self) -> int:
+  def cost_rank(self) -> int:  # noqa: D102
     return self._cost_1.shape[1]
 
   @property
   def cost_matrix(self) -> jnp.ndarray:
     """Materialize the cost matrix."""
     return jnp.matmul(self.cost_1, self.cost_2.T) + self.bias
 
   @property
-  def shape(self) -> Tuple[int, int]:
+  def shape(self) -> Tuple[int, int]:  # noqa: D102
     return self._cost_1.shape[0], self._cost_2.shape[0]
 
   @property
-  def is_symmetric(self) -> bool:
+  def is_symmetric(self) -> bool:  # noqa: D102
     return (
         self._cost_1.shape[0] == self._cost_2.shape[0] and
         jnp.all(self._cost_1 == self._cost_2)
     )
 
   @property
-  def inv_scale_cost(self) -> float:
+  def inv_scale_cost(self) -> float:  # noqa: D102
     if isinstance(self._scale_cost,
                   (int, float)) or utils.is_jax_array(self._scale_cost):
       return 1.0 / self._scale_cost
     self = self._masked_geom()
-    if self._scale_cost == 'max_bound':
+    if self._scale_cost == "max_bound":
       x_norm = self._cost_1[:, 0].max()
       y_norm = self._cost_2[:, 1].max()
       max_bound = x_norm + y_norm + 2 * jnp.sqrt(x_norm * y_norm)
       return 1.0 / (max_bound + self._bias)
-    if self._scale_cost == 'mean':
+    if self._scale_cost == "mean":
       factor1 = jnp.dot(self._n_normed_ones, self._cost_1)
       factor2 = jnp.dot(self._cost_2.T, self._m_normed_ones)
       mean = jnp.dot(factor1, factor2) + self._bias
       return 1.0 / mean
-    if self._scale_cost == 'max_cost':
+    if self._scale_cost == "max_cost":
       return 1.0 / self.compute_max_cost()
-    raise ValueError(f'Scaling {self._scale_cost} not implemented.')
+    raise ValueError(f"Scaling {self._scale_cost} not implemented.")
 
   def apply_square_cost(self, arr: jnp.ndarray, axis: int = 0) -> jnp.ndarray:
     """Apply elementwise-square of cost matrix to array (vector or matrix)."""
     (n, m), r = self.shape, self.cost_rank
     # When applying square of a LRCGeometry, one can either elementwise square
     # the cost matrix, or instantiate an augmented (rank^2) LRCGeometry
     # and apply it. First is O(nm), the other is O((n+m)r^2).
     if n * m < (n + m) * r ** 2:  # better use regular apply
       return super().apply_square_cost(arr, axis)
-    else:
-      new_cost_1 = self.cost_1[:, :, None] * self.cost_1[:, None, :]
-      new_cost_2 = self.cost_2[:, :, None] * self.cost_2[:, None, :]
-      return LRCGeometry(
-          cost_1=new_cost_1.reshape((n, r ** 2)),
-          cost_2=new_cost_2.reshape((m, r ** 2))
-      ).apply_cost(arr, axis)
+
+    new_cost_1 = self.cost_1[:, :, None] * self.cost_1[:, None, :]
+    new_cost_2 = self.cost_2[:, :, None] * self.cost_2[:, None, :]
+    return LRCGeometry(
+        cost_1=new_cost_1.reshape((n, r ** 2)),
+        cost_2=new_cost_2.reshape((m, r ** 2))
+    ).apply_cost(arr, axis)
 
   def _apply_cost_to_vec(
       self,
       vec: jnp.ndarray,
       axis: int = 0,
       fn: Optional[Callable[[jnp.ndarray], jnp.ndarray]] = None,
       is_linear: bool = False,
@@ -220,48 +216,52 @@
           cost2, (slice_idx * batch_size, 0), (batch_size, p)
       )
       out_slice = jnp.max(jnp.dot(cost2_slice, cost1.T))
       return carry, out_slice
 
     def finalize(carry):
       cost1, cost2 = carry
-      out_slice = jnp.dot(cost2[n_batch * batch_size:], cost1.T)
-      return out_slice
+      return jnp.dot(cost2[n_batch * batch_size:], cost1.T)
 
     _, out = jax.lax.scan(body, carry, jnp.arange(n_batch))
     last_slice = finalize(carry)
     max_value = jnp.max(jnp.concatenate((out, last_slice.reshape(-1))))
     return max_value + self._bias
 
   def to_LRCGeometry(
-      self, rank: int = 0, tol: float = 1e-2, seed: int = 0
-  ) -> 'LRCGeometry':
+      self,
+      rank: int = 0,
+      tol: float = 1e-2,
+      rng: Optional[jax.random.PRNGKeyArray] = None,
+      scale: float = 1.0,
+  ) -> "LRCGeometry":
     """Return self."""
+    del rank, tol, rng, scale
     return self
 
   @property
-  def can_LRC(self):
+  def can_LRC(self):  # noqa: D102
     return True
 
-  def subset(
+  def subset(  # noqa: D102
       self, src_ixs: Optional[jnp.ndarray], tgt_ixs: Optional[jnp.ndarray],
       **kwargs: Any
   ) -> "LRCGeometry":
 
     def subset_fn(
         arr: Optional[jnp.ndarray],
         ixs: Optional[jnp.ndarray],
     ) -> jnp.ndarray:
       return arr if arr is None or ixs is None else arr[jnp.atleast_1d(ixs)]
 
     return self._mask_subset_helper(
         src_ixs, tgt_ixs, fn=subset_fn, propagate_mask=True, **kwargs
     )
 
-  def mask(
+  def mask(  # noqa: D102
       self,
       src_mask: Optional[jnp.ndarray],
       tgt_mask: Optional[jnp.ndarray],
       mask_value: float = 0.,
   ) -> "LRCGeometry":
 
     def mask_fn(
@@ -298,35 +298,50 @@
       tgt_mask = fn(tgt_mask, tgt_ixs)
 
     aux_data = {**aux_data, **kwargs}
     return type(self).tree_unflatten(
         aux_data, [c1, c2, src_mask, tgt_mask] + children
     )
 
-  def __add__(self, other: 'LRCGeometry') -> 'LRCGeometry':
-    assert isinstance(other, LRCGeometry), type(other)
-    return type(self)(
+  def __add__(self, other: "LRCGeometry") -> "LRCGeometry":
+    if not isinstance(other, LRCGeometry):
+      return NotImplemented
+    return LRCGeometry(
         cost_1=jnp.concatenate((self.cost_1, other.cost_1), axis=1),
         cost_2=jnp.concatenate((self.cost_2, other.cost_2), axis=1),
-        **self._kwargs
+        bias=self._bias + other._bias,
+        # already included in `cost_{1,2}`
+        scale_factor=1.0,
+        scale_cost=1.0,
     )
 
   @property
-  def dtype(self) -> jnp.dtype:
+  def dtype(self) -> jnp.dtype:  # noqa: D102
     return self._cost_1.dtype
 
-  def tree_flatten(self):
+  def tree_flatten(self):  # noqa: D102
     return (
-        self._cost_1, self._cost_2, self._src_mask, self._tgt_mask, self._kwargs
+        self._cost_1,
+        self._cost_2,
+        self._src_mask,
+        self._tgt_mask,
+        self._epsilon_init,
+        self._bias,
+        self._scale_factor,
     ), {
-        'bias': self._bias,
-        'scale_factor': self._scale_factor,
-        'scale_cost': self._scale_cost,
-        'batch_size': self.batch_size
+        "scale_cost": self._scale_cost,
+        "batch_size": self.batch_size
     }
 
   @classmethod
-  def tree_unflatten(cls, aux_data, children):
-    c1, c2, src_mask, tgt_mask, kwargs = children
+  def tree_unflatten(cls, aux_data, children):  # noqa: D102
+    c1, c2, src_mask, tgt_mask, epsilon, bias, scale_factor = children
     return cls(
-        c1, c2, src_mask=src_mask, tgt_mask=tgt_mask, **kwargs, **aux_data
+        c1,
+        c2,
+        bias=bias,
+        scale_factor=scale_factor,
+        epsilon=epsilon,
+        src_mask=src_mask,
+        tgt_mask=tgt_mask,
+        **aux_data
     )
```

### Comparing `ott-jax-0.4.0/src/ott/geometry/pointcloud.py` & `ott-jax-0.4.1/src/ott/geometry/pointcloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-# Copyright 2022 Google LLC.
+# Copyright OTT-JAX
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-#     http://www.apache.org/licenses/LICENSE-2.0
+#   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""A geometry defined using 2 point clouds and a cost function between them."""
 import math
 from typing import Any, Callable, Literal, Optional, Tuple, Union
 
 import jax
 import jax.numpy as jnp
 
 from ott import utils
@@ -49,36 +48,28 @@
      ``batch_size`` lines at a time, used on a vector and discarded.
      The online computation is particularly useful for big point clouds
      whose cost matrix does not fit in memory.
     scale_cost: option to rescale the cost matrix. Implemented scalings are
       'median', 'mean', 'max_cost', 'max_norm' and 'max_bound'.
       Alternatively, a float factor can be given to rescale the cost such
       that ``cost_matrix /= scale_cost``. If `True`, use 'mean'.
-    kwargs: other optional parameters to be passed on to superclass
-      initializer, notably those related to epsilon regularization.
+    kwargs: keyword arguments for :class:`~ott.geometry.geometry.Geometry`.
   """
 
   def __init__(
       self,
       x: jnp.ndarray,
       y: Optional[jnp.ndarray] = None,
       cost_fn: Optional[costs.CostFn] = None,
       batch_size: Optional[int] = None,
       scale_cost: Union[bool, int, float,
-                        Literal['mean', 'max_norm', 'max_bound', 'max_cost',
-                                'median']] = 1.0,
+                        Literal["mean", "max_norm", "max_bound", "max_cost",
+                                "median"]] = 1.0,
       **kwargs: Any
   ):
-    # For reverse compatibility of deprecated parameter `power`.
-    power = kwargs.pop("power", None)
-    assert power is None or power == 1.0, (
-        "`power` option in `PointCloud` geometries is deprecated."
-        " Specify directly a `CostFn` with that power."
-    )
-
     super().__init__(**kwargs)
     self.x = x
     self.y = self.x if y is None else y
 
     self.cost_fn = costs.SqEuclidean() if cost_fn is None else cost_fn
     self._axis_norm = 0 if callable(self.cost_fn.norm) else None
     if batch_size is not None:
@@ -95,117 +86,116 @@
   @property
   def _norm_y(self) -> Union[float, jnp.ndarray]:
     if self._axis_norm == 0:
       return self.cost_fn.norm(self.y)
     return 0.
 
   @property
-  def can_LRC(self):
+  def can_LRC(self):  # noqa: D102
     return self.is_squared_euclidean and self._check_LRC_dim
 
   @property
   def _check_LRC_dim(self):
     (n, m), d = self.shape, self.x.shape[1]
     return n * m > (n + m) * d
 
   @property
-  def cost_matrix(self) -> Optional[jnp.ndarray]:
+  def cost_matrix(self) -> Optional[jnp.ndarray]:  # noqa: D102
     if self.is_online:
       return None
     cost_matrix = self._compute_cost_matrix()
     return cost_matrix * self.inv_scale_cost
 
   @property
-  def kernel_matrix(self) -> Optional[jnp.ndarray]:
+  def kernel_matrix(self) -> Optional[jnp.ndarray]:  # noqa: D102
     if self.is_online:
       return None
     return jnp.exp(-self.cost_matrix / self.epsilon)
 
   @property
-  def shape(self) -> Tuple[int, int]:
+  def shape(self) -> Tuple[int, int]:  # noqa: D102
     # in the process of flattening/unflattening in vmap, `__init__`
     # can be called with dummy objects
     # we optionally access `shape` in order to get the batch size
     if self.x is None or self.y is None:
       return 0, 0
     return self.x.shape[0], self.y.shape[0]
 
   @property
-  def is_symmetric(self) -> bool:
+  def is_symmetric(self) -> bool:  # noqa: D102
     return self.y is None or (
         jnp.all(self.x.shape == self.y.shape) and jnp.all(self.x == self.y)
     )
 
   @property
-  def is_squared_euclidean(self) -> bool:
+  def is_squared_euclidean(self) -> bool:  # noqa: D102
     return isinstance(self.cost_fn, costs.SqEuclidean)
 
   @property
   def is_online(self) -> bool:
-    """Whether :attr:`cost_matrix` or :attr:`kernel_matrix` \
-      is computed on-the-fly."""
+    """Whether the cost/kernel is computed on-the-fly."""
     return self.batch_size is not None
 
   # TODO(michalk8): when refactoring, consider PC as a subclass of LR?
   @property
-  def cost_rank(self) -> int:
+  def cost_rank(self) -> int:  # noqa: D102
     return self.x.shape[1]
 
   @property
-  def inv_scale_cost(self) -> float:
+  def inv_scale_cost(self) -> float:  # noqa: D102
     if isinstance(self._scale_cost,
                   (int, float)) or utils.is_jax_array(self._scale_cost):
       return 1.0 / self._scale_cost
     self = self._masked_geom()
-    if self._scale_cost == 'max_cost':
+    if self._scale_cost == "max_cost":
       if self.is_online:
         return 1.0 / self._compute_summary_online(self._scale_cost)
       return 1.0 / jnp.max(self._compute_cost_matrix())
-    if self._scale_cost == 'mean':
+    if self._scale_cost == "mean":
       if self.is_online:
         return 1.0 / self._compute_summary_online(self._scale_cost)
       if self.shape[0] > 0:
         geom = self._masked_geom(mask_value=jnp.nan)._compute_cost_matrix()
         return 1.0 / jnp.nanmean(geom)
       return 1.0
-    if self._scale_cost == 'median':
+    if self._scale_cost == "median":
       if not self.is_online:
         geom = self._masked_geom(mask_value=jnp.nan)
         return 1.0 / jnp.nanmedian(geom._compute_cost_matrix())
       raise NotImplementedError(
           "Using the median as scaling factor for "
           "the cost matrix with the online mode is not implemented."
       )
-    if self._scale_cost == 'max_norm':
+    if self._scale_cost == "max_norm":
       if self.cost_fn.norm is not None:
         return 1.0 / jnp.maximum(self._norm_x.max(), self._norm_y.max())
       return 1.0
-    if self._scale_cost == 'max_bound':
+    if self._scale_cost == "max_bound":
       if self.is_squared_euclidean:
         x_argmax = jnp.argmax(self._norm_x)
         y_argmax = jnp.argmax(self._norm_y)
         max_bound = (
             self._norm_x[x_argmax] + self._norm_y[y_argmax] +
             2 * jnp.sqrt(self._norm_x[x_argmax] * self._norm_y[y_argmax])
         )
         return 1.0 / max_bound
       raise NotImplementedError(
           "Using max_bound as scaling factor for "
           "the cost matrix when the cost is not squared euclidean "
           "is not implemented."
       )
-    raise ValueError(f'Scaling {self._scale_cost} not implemented.')
+    raise ValueError(f"Scaling {self._scale_cost} not implemented.")
 
   def _compute_cost_matrix(self) -> jnp.ndarray:
     cost_matrix = self.cost_fn.all_pairs_pairwise(self.x, self.y)
     if self._axis_norm is not None:
       cost_matrix += self._norm_x[:, jnp.newaxis] + self._norm_y[jnp.newaxis, :]
     return cost_matrix
 
-  def apply_lse_kernel(
+  def apply_lse_kernel(  # noqa: D102
       self,
       f: jnp.ndarray,
       g: jnp.ndarray,
       eps: float,
       vec: Optional[jnp.ndarray] = None,
       axis: int = 0
   ) -> jnp.ndarray:
@@ -284,15 +274,15 @@
     h_res, h_sign = jnp.concatenate(h_res), jnp.concatenate(h_sign)
     h_res_rest, h_sign_rest = finalize(n * self.batch_size)
     h_res = jnp.concatenate([h_res, h_res_rest])
     h_sign = jnp.concatenate([h_sign, h_sign_rest])
 
     return eps * h_res - jnp.where(jnp.isfinite(v), v, 0), h_sign
 
-  def apply_kernel(
+  def apply_kernel(  # noqa: D102
       self,
       scaling: jnp.ndarray,
       eps: Optional[float] = None,
       axis: int = 0
   ) -> jnp.ndarray:
     if eps is None:
       eps = self.epsilon
@@ -305,35 +295,34 @@
         in_axes=[None, 0, None, self._axis_norm, None, None, None, None]
     )
     if axis == 0:
       return app(
           self.x, self.y, self._norm_x, self._norm_y, scaling, eps,
           self.cost_fn, self.inv_scale_cost
       )
-    if axis == 1:
-      return app(
-          self.y, self.x, self._norm_y, self._norm_x, scaling, eps,
-          self.cost_fn, self.inv_scale_cost
-      )
+    return app(
+        self.y, self.x, self._norm_y, self._norm_x, scaling, eps, self.cost_fn,
+        self.inv_scale_cost
+    )
 
-  def transport_from_potentials(
+  def transport_from_potentials(  # noqa: D102
       self, f: jnp.ndarray, g: jnp.ndarray
   ) -> jnp.ndarray:
     if not self.is_online:
       return super().transport_from_potentials(f, g)
     transport = jax.vmap(
         _transport_from_potentials_xy,
         in_axes=[None, 0, None, self._axis_norm, None, 0, None, None, None]
     )
     return transport(
         self.y, self.x, self._norm_y, self._norm_x, g, f, self.epsilon,
         self.cost_fn, self.inv_scale_cost
     )
 
-  def transport_from_scalings(
+  def transport_from_scalings(  # noqa: D102
       self, u: jnp.ndarray, v: jnp.ndarray
   ) -> jnp.ndarray:
     if not self.is_online:
       return super().transport_from_scalings(u, v)
     transport = jax.vmap(
         _transport_from_scalings_xy,
         in_axes=[
@@ -388,56 +377,51 @@
 
     return self._apply_cost(arr, axis, fn=fn)
 
   def _apply_cost(
       self, arr: jnp.ndarray, axis: int = 0, fn=None
   ) -> jnp.ndarray:
     """See :meth:`apply_cost`."""
-    if self.is_online:
-      app = jax.vmap(
-          _apply_cost_xy,
-          in_axes=[None, 0, None, self._axis_norm, None, None, None, None]
-      )
-      if arr.ndim == 1:
-        arr = arr.reshape(-1, 1)
-      if axis == 0:
-        return app(
-            self.x, self.y, self._norm_x, self._norm_y, arr, self.cost_fn,
-            self.inv_scale_cost, fn
-        )
-      if axis == 1:
-        return app(
-            self.y, self.x, self._norm_y, self._norm_x, arr, self.cost_fn,
-            self.inv_scale_cost, fn
-        )
-    else:
+    if not self.is_online:
       return super().apply_cost(arr, axis, fn)
 
+    app = jax.vmap(
+        _apply_cost_xy,
+        in_axes=[None, 0, None, self._axis_norm, None, None, None, None]
+    )
+    if arr.ndim == 1:
+      arr = arr.reshape(-1, 1)
+
+    if axis == 0:
+      return app(
+          self.x, self.y, self._norm_x, self._norm_y, arr, self.cost_fn,
+          self.inv_scale_cost, fn
+      )
+    return app(
+        self.y, self.x, self._norm_y, self._norm_x, arr, self.cost_fn,
+        self.inv_scale_cost, fn
+    )
+
   def vec_apply_cost(
       self,
       arr: jnp.ndarray,
       axis: int = 0,
       fn: Optional[Callable[[jnp.ndarray], jnp.ndarray]] = None
   ) -> jnp.ndarray:
-    """Apply the geometry's cost matrix in a vectorised way.
-
-    This performs either:
-    output = C arr (if axis=1)
-    output = C' arr (if axis=0)
-    where C is [num_a, num_b]
+    """Apply the geometry's cost matrix in a vectorized way.
 
     This function can be used when the cost matrix is squared euclidean
-    and fn is a linear map.
+    and ``fn`` is a linear function.
 
     Args:
       arr: jnp.ndarray [num_a or num_b, p], vector that will be multiplied
         by the cost matrix.
-      axis: standard cost matrix if axis=1, transport if 0
+      axis: standard cost matrix if axis=1, transport if 0.
       fn: function optionally applied to cost matrix element-wise, before the
-        apply
+        application.
 
     Returns:
       A jnp.ndarray, [num_b, p] if axis=0 or [num_a, p] if axis=1
     """
     assert self.is_squared_euclidean, "Cost matrix is not a squared Euclidean."
     rank = arr.ndim
     x, y = (self.x, self.y) if axis == 0 else (self.y, self.x)
@@ -454,15 +438,15 @@
 
   def _leading_slice(self, t: jnp.ndarray, i: int) -> jnp.ndarray:
     start_indices = [i * self.batch_size] + (t.ndim - 1) * [0]
     slice_sizes = [self.batch_size] + list(t.shape[1:])
     return jax.lax.dynamic_slice(t, start_indices, slice_sizes)
 
   def _compute_summary_online(
-      self, summary: Literal['mean', 'max_cost']
+      self, summary: Literal["mean", "max_cost"]
   ) -> float:
     """Compute mean or max of cost matrix online, i.e. without instantiating it.
 
     Args:
       summary: can be 'mean' or 'max_cost'.
 
     Returns:
@@ -503,21 +487,21 @@
         )
       norm_x = self._norm_x if self._axis_norm is None else self._norm_x[i:]
       return app(
           self.y, self.x[i:], self._norm_y, norm_x, vec, self.cost_fn,
           scale_cost
       )
 
-    if summary == 'mean':
+    if summary == "mean":
       fn = _apply_cost_xy
-    elif summary == 'max_cost':
+    elif summary == "max_cost":
       fn = _apply_max_xy
     else:
       raise ValueError(
-          f'Scaling method {summary} does not exist for online mode.'
+          f"Scaling method {summary} does not exist for online mode."
       )
     app = jax.vmap(
         fn, in_axes=[None, 0, None, self._axis_norm, None, None, None]
     )
 
     batch_for_y = self.shape[0] < self.shape[1]
     if batch_for_y:
@@ -530,26 +514,26 @@
       vec, other = self._m_normed_ones, self._n_normed_ones
 
     _, val = jax.lax.scan(fun, init=(vec,), xs=jnp.arange(n))
     val = jnp.concatenate(val).squeeze()
     val_rest = finalize(n * self.batch_size)
     val_res = jnp.concatenate([val, val_rest])
 
-    if summary == 'mean':
+    if summary == "mean":
       return jnp.sum(val_res * other)
-    if summary == 'max_cost':
+    if summary == "max_cost":
       # TODO(michalk8): explain why scaling is not needed
       return jnp.max(val_res)
     raise ValueError(
-        f'Scaling method {summary} does not exist for online mode.'
+        f"Scaling method {summary} does not exist for online mode."
     )
 
   def barycenter(self, weights: jnp.ndarray) -> jnp.ndarray:
     """Compute barycenter of points in self.x using weights."""
-    return self.cost_fn.barycenter(self.x, weights)
+    return self.cost_fn.barycenter(self.x, weights)[0]
 
   @classmethod
   def prepare_divergences(
       cls,
       x: jnp.ndarray,
       y: jnp.ndarray,
       static_b: bool = False,
@@ -565,45 +549,55 @@
       masks += [(tgt_mask, tgt_mask)]
 
     return tuple(
         cls(x, y, src_mask=x_mask, tgt_mask=y_mask, **kwargs)
         for ((x, y), (x_mask, y_mask)) in zip(couples, masks)
     )
 
-  def tree_flatten(self):
-    return ([self.x, self.y, self._src_mask, self._tgt_mask, self.cost_fn], {
-        'epsilon': self._epsilon_init,
-        'relative_epsilon': self._relative_epsilon,
-        'scale_epsilon': self._scale_epsilon,
-        'batch_size': self._batch_size,
-        'scale_cost': self._scale_cost
-    })
+  def tree_flatten(self):  # noqa: D102
+    return (
+        self.x,
+        self.y,
+        self._src_mask,
+        self._tgt_mask,
+        self._epsilon_init,
+        self.cost_fn,
+    ), {
+        "batch_size": self._batch_size,
+        "scale_cost": self._scale_cost
+    }
 
   @classmethod
-  def tree_unflatten(cls, aux_data, children):
-    x, y, src_mask, tgt_mask, cost_fn = children
+  def tree_unflatten(cls, aux_data, children):  # noqa: D102
+    x, y, src_mask, tgt_mask, epsilon, cost_fn = children
     return cls(
-        x, y, cost_fn=cost_fn, src_mask=src_mask, tgt_mask=tgt_mask, **aux_data
+        x,
+        y,
+        cost_fn=cost_fn,
+        src_mask=src_mask,
+        tgt_mask=tgt_mask,
+        epsilon=epsilon,
+        **aux_data
     )
 
-  def _cosine_to_sqeucl(self) -> 'PointCloud':
+  def _cosine_to_sqeucl(self) -> "PointCloud":
     assert isinstance(self.cost_fn, costs.Cosine), type(self.cost_fn)
     (x, y, *args, _), aux_data = self.tree_flatten()
     x = x / jnp.linalg.norm(x, axis=-1, keepdims=True)
     y = y / jnp.linalg.norm(y, axis=-1, keepdims=True)
     # TODO(michalk8): find a better way
     aux_data["scale_cost"] = 2. / self.inv_scale_cost
     cost_fn = costs.SqEuclidean()
     return type(self).tree_unflatten(aux_data, [x, y] + args + [cost_fn])
 
   def to_LRCGeometry(
       self,
       scale: float = 1.0,
       **kwargs: Any,
-  ) -> Union[low_rank.LRCGeometry, 'PointCloud']:
+  ) -> Union[low_rank.LRCGeometry, "PointCloud"]:
     r"""Convert point cloud to low-rank geometry.
 
     Args:
       scale: Value used to rescale the factors of the low-rank geometry.
         Useful when this geometry is used in the linear term of fused GW.
       kwargs: Keyword arguments, such as ``rank``, to
         :meth:`~ott.geometry.geometry.Geometry.to_LRCGeometry` used when
@@ -638,37 +632,35 @@
 
     return low_rank.LRCGeometry(
         cost_1=cost_1,
         cost_2=cost_2,
         scale_factor=scale,
         epsilon=self._epsilon_init,
         relative_epsilon=self._relative_epsilon,
-        scale=self._scale_epsilon,
         scale_cost=self._scale_cost,
         src_mask=self.src_mask,
         tgt_mask=self.tgt_mask,
-        **self._kwargs
     )
 
-  def subset(
+  def subset(  # noqa: D102
       self, src_ixs: Optional[jnp.ndarray], tgt_ixs: Optional[jnp.ndarray],
       **kwargs: Any
   ) -> "PointCloud":
 
     def subset_fn(
         arr: Optional[jnp.ndarray],
         ixs: Optional[jnp.ndarray],
     ) -> jnp.ndarray:
       return arr if arr is None or ixs is None else arr[jnp.atleast_1d(ixs)]
 
     return self._mask_subset_helper(
         src_ixs, tgt_ixs, fn=subset_fn, propagate_mask=True, **kwargs
     )
 
-  def mask(
+  def mask(  # noqa: D102
       self,
       src_mask: Optional[jnp.ndarray],
       tgt_mask: Optional[jnp.ndarray],
       mask_value: float = 0.,
   ) -> "PointCloud":
 
     def mask_fn(
@@ -706,15 +698,15 @@
     aux_data = {**aux_data, **kwargs}
 
     return type(self).tree_unflatten(
         aux_data, [x, y, src_mask, tgt_mask] + children
     )
 
   @property
-  def dtype(self) -> jnp.dtype:
+  def dtype(self) -> jnp.dtype:  # noqa: D102
     return self.x.dtype
 
   @property
   def batch_size(self) -> Optional[int]:
     """Batch size for online mode."""
     if self._batch_size is None:
       return None
```

### Comparing `ott-jax-0.4.0/src/ott/geometry/segment.py` & `ott-jax-0.4.1/src/ott/geometry/segment.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 #
+# Copyright OTT-JAX
+#
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-#     http://www.apache.org/licenses/LICENSE-2.0
+#   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Prepare point clouds for parallel computations."""
 from typing import Callable, Optional, Tuple
 
 import jax
 import jax.numpy as jnp
 
 __all__ = ["segment_point_cloud"]
 
@@ -29,48 +30,48 @@
     num_per_segment: Optional[Tuple[int, ...]] = None,
     padding_vector: Optional[jnp.ndarray] = None
 ) -> Tuple[jnp.ndarray, jnp.ndarray]:
   """Segment and pad as needed the entries of a point cloud.
 
   There are two interfaces:
 
-  1. use ``segment_ids``, and optionally ``indices_are_sorted`` to describe
+  #. use ``segment_ids``, and optionally ``indices_are_sorted`` to describe
      for each data point in the matrix to which segment it belongs to.
-  2. use ``num_per_segment`` which describes contiguous segments.
+  #. use ``num_per_segment`` which describes contiguous segments.
 
-  If using the 1st interface, ``num_segments`` is required for JIT compilation.
+  If using the first interface, ``num_segments`` is required for jitting.
   Assumes ``range(0, num_segments)`` are the segment ids.
 
   In both cases, jitting requires defining a ``max_measure_size``, the
   upper bound on the maximal size of measures, which will be used for padding.
 
   Args:
     x: Array of input points, of shape ``[num_x, ndim]``.
       Multiple segments are held in this single array.
     a: Array of shape ``[num_x,]`` containing the weights (within each measure)
       of all the points.
     num_segments: Number of segments. Required for jitting.
-      If `None` and using the 2nd interface, it will be computed as
+      If `None` and using the second interface, it will be computed as
       ``len(num_per_segment)``.
     max_measure_size: Overall size of padding. Required for jitting.
-      If `None` and using the 2nd interface, it will be computed as
+      If `None` and using the second interface, it will be computed as
       ``max(num_per_segment)``.
     segment_ids: **1st interface** The segment ids for which each row of ``x``
       belongs. This is a similar interface to :func:`jax.ops.segment_sum`.
     indices_are_sorted: **1st interface** Whether ``segment_ids`` are sorted.
     num_per_segment: **2nd interface** Number of points in each segment.
       For example, `[100, 20, 30]` would imply that ``x`` is segmented into 3
       arrays of length `[100]`, `[20]`, and `[30]`, respectively.
       Must be a tuple and not a :class:`jax.numpy.ndarray` to allow jitting.
       This means changes in ``num_per_segment`` will re-trigger compilation.
     padding_vector: vector to be used to pad point cloud matrices. Most likely
       to be zero, but can be adjusted to be other values to avoid errors or
       over/underflow in cost matrix that could be problematic (even these values
       are not supposed to be taken given their corresponding masses are 0).
-      See also :func:`ott.geometry.costs.CostFn.padder`.
+      See also :func:`~ott.geometry.costs.CostFn._padder`.
       If ``None``, vector of 0s of shape ``[1, ndim]`` is used.
 
   Returns:
     Segmented ``x`` as an array of shape
     ``[num_measures, max_measure_size, ndim]`` and ``a`` as an array of shape
     ``[num_measures, max_measure_size]``.
   """
```

### Comparing `ott-jax-0.4.0/src/ott/initializers/linear/initializers_lr.py` & `ott-jax-0.4.1/src/ott/initializers/linear/initializers_lr.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+# Copyright OTT-JAX
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#   http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 import abc
 import functools
 from typing import (
     TYPE_CHECKING,
     Any,
     Dict,
     Literal,
@@ -13,14 +26,15 @@
     Union,
 )
 
 import jax
 import jax.numpy as jnp
 import numpy as np
 
+from ott import utils
 from ott.geometry import geometry, low_rank, pointcloud
 from ott.math import fixed_point_loop
 from ott.math import utils as mu
 
 if TYPE_CHECKING:
   from ott.problems.linear import linear_problem
   from ott.problems.quadratic import quadratic_problem
@@ -49,79 +63,79 @@
     self._rank = rank
     self._kwargs = kwargs
 
   @abc.abstractmethod
   def init_q(
       self,
       ot_prob: Problem_t,
-      key: jnp.ndarray,
+      rng: jax.random.PRNGKeyArray,
       *,
       init_g: jnp.ndarray,
       **kwargs: Any,
   ) -> jnp.ndarray:
     """Initialize the low-rank factor :math:`Q`.
 
     Args:
       ot_prob: OT problem.
-      key: Random key for seeding.
+      rng: Random key for seeding.
       init_g: Initial value for :math:`g` factor.
       kwargs: Additional keyword arguments.
 
     Returns:
       Array of shape ``[n, rank]``.
     """
 
   @abc.abstractmethod
   def init_r(
       self,
       ot_prob: Problem_t,
-      key: jnp.ndarray,
+      rng: jax.random.PRNGKeyArray,
       *,
       init_g: jnp.ndarray,
       **kwargs: Any,
   ) -> jnp.ndarray:
     """Initialize the low-rank factor :math:`R`.
 
     Args:
       ot_prob: Linear OT problem.
-      key: Random key for seeding.
+      rng: Random key for seeding.
       init_g: Initial value for :math:`g` factor.
       kwargs: Additional keyword arguments.
 
     Returns:
       Array of shape ``[m, rank]``.
     """
 
   @abc.abstractmethod
   def init_g(
       self,
       ot_prob: Problem_t,
-      key: jnp.ndarray,
+      rng: jax.random.PRNGKeyArray,
       **kwargs: Any,
   ) -> jnp.ndarray:
     """Initialize the low-rank factor :math:`g`.
 
     Args:
       ot_prob: OT problem.
-      key: Random key for seeding.
+      rng: Random key for seeding.
       kwargs: Additional keyword arguments.
 
     Returns:
       Array of shape ``[rank,]``.
     """
 
   @classmethod
   def from_solver(
       cls,
-      solver: Union['sinkhorn_lr.LRSinkhorn',
-                    'gromov_wasserstein.GromovWasserstein'],
+      solver: Union["sinkhorn_lr.LRSinkhorn",
+                    "gromov_wasserstein.GromovWasserstein"],
       *,
       kind: Literal["random", "rank2", "k-means", "generalized-k-means"],
       **kwargs: Any,
-  ) -> 'LRInitializer':
+  ) -> "LRInitializer":
     """Create a low-rank initializer from a linear or quadratic solver.
 
     Args:
       solver: Low-rank linear or quadratic solver.
       kind: Which initializer to instantiate.
       kwargs: Keyword arguments when creating the initializer.
 
@@ -159,109 +173,108 @@
   def __call__(
       self,
       ot_prob: Problem_t,
       q: Optional[jnp.ndarray] = None,
       r: Optional[jnp.ndarray] = None,
       g: Optional[jnp.ndarray] = None,
       *,
-      key: Optional[jnp.ndarray] = None,
+      rng: Optional[jax.random.PRNGKeyArray] = None,
       **kwargs: Any
   ) -> Tuple[jnp.ndarray, jnp.ndarray, jnp.ndarray]:
     """Initialize the factors :math:`Q`, :math:`R` and :math:`g`.
 
     Args:
       ot_prob: OT problem.
       q: Factor of shape ``[n, rank]``. If `None`, it will be initialized
         using :meth:`init_q`.
       r: Factor of shape ``[m, rank]``. If `None`, it will be initialized
         using :meth:`init_r`.
       g: Factor of shape ``[rank,]``. If `None`, it will be initialized
         using :meth:`init_g`.
-      key: Random key for seeding.
+      rng: Random key for seeding.
       kwargs: Additional keyword arguments for :meth:`init_q`, :meth:`init_r`
         and :meth:`init_g`.
 
     Returns:
       The factors :math:`Q`, :math:`R` and :math:`g`, respectively.
     """
-    if key is None:
-      key = jax.random.PRNGKey(0)
-    key1, key2, key3 = jax.random.split(key, 3)
+    rng = utils.default_prng_key(rng)
+    rng1, rng2, rng3 = jax.random.split(rng, 3)
 
     if g is None:
-      g = self.init_g(ot_prob, key1, **kwargs)
+      g = self.init_g(ot_prob, rng1, **kwargs)
     if q is None:
-      q = self.init_q(ot_prob, key2, init_g=g, **kwargs)
+      q = self.init_q(ot_prob, rng2, init_g=g, **kwargs)
     if r is None:
-      r = self.init_r(ot_prob, key3, init_g=g, **kwargs)
+      r = self.init_r(ot_prob, rng3, init_g=g, **kwargs)
 
     assert g.shape == (self.rank,)
     assert q.shape == (ot_prob.a.shape[0], self.rank)
     assert r.shape == (ot_prob.b.shape[0], self.rank)
 
     return q, r, g
 
   @property
   def rank(self) -> int:
     """Rank of the transport matrix factorization."""
     return self._rank
 
-  def tree_flatten(self) -> Tuple[Sequence[Any], Dict[str, Any]]:
+  def tree_flatten(self) -> Tuple[Sequence[Any], Dict[str, Any]]:  # noqa: D102
     return [], {**self._kwargs, "rank": self.rank}
 
   @classmethod
-  def tree_unflatten(
+  def tree_unflatten(  # noqa: D102
       cls, aux_data: Dict[str, Any], children: Sequence[Any]
   ) -> "LRInitializer":
     return cls(*children, **aux_data)
 
 
 @jax.tree_util.register_pytree_node_class
 class RandomInitializer(LRInitializer):
   """Low-rank Sinkhorn factorization using random factors.
 
   Args:
     rank: Rank of the factorization.
     kwargs: Additional keyword arguments.
   """
 
-  def init_q(
+  def init_q(  # noqa: D102
       self,
       ot_prob: Problem_t,
-      key: jnp.ndarray,
+      rng: jax.random.PRNGKeyArray,
       *,
       init_g: jnp.ndarray,
       **kwargs: Any,
   ) -> jnp.ndarray:
     del kwargs, init_g
     a = ot_prob.a
-    init_q = jnp.abs(jax.random.normal(key, (a.shape[0], self.rank)))
+    init_q = jnp.abs(jax.random.normal(rng, (a.shape[0], self.rank)))
     return a[:, None] * (init_q / jnp.sum(init_q, axis=1, keepdims=True))
 
-  def init_r(
+  def init_r(  # noqa: D102
       self,
       ot_prob: Problem_t,
-      key: jnp.ndarray,
+      rng: jax.random.PRNGKeyArray,
       *,
       init_g: jnp.ndarray,
       **kwargs: Any,
   ) -> jnp.ndarray:
     del kwargs, init_g
     b = ot_prob.b
-    init_r = jnp.abs(jax.random.normal(key, (b.shape[0], self.rank)))
+    init_r = jnp.abs(jax.random.normal(rng, (b.shape[0], self.rank)))
     return b[:, None] * (init_r / jnp.sum(init_r, axis=1, keepdims=True))
 
-  def init_g(
+  def init_g(  # noqa: D102
       self,
       ot_prob: Problem_t,
-      key: jnp.ndarray,
+      rng: jax.random.PRNGKeyArray,
       **kwargs: Any,
   ) -> jnp.ndarray:
     del kwargs
-    init_g = jnp.abs(jax.random.uniform(key, (self.rank,))) + 1.
+    init_g = jnp.abs(jax.random.uniform(rng, (self.rank,))) + 1.
     return init_g / jnp.sum(init_g)
 
 
 @jax.tree_util.register_pytree_node_class
 class Rank2Initializer(LRInitializer):
   """Low-rank Sinkhorn factorization using rank-2 factors :cite:`scetbon:21`.
 
@@ -294,43 +307,43 @@
     g2 = (init_g - lambda_1 * g1) / (1. - lambda_1)
     x = 2. * jnp.arange(1, n + 1) / (n ** 2 + n)
     y = (marginal - lambda_1 * x) / (1. - lambda_1)
 
     return ((lambda_1 * x[:, None] @ g1.reshape(1, -1)) +
             ((1 - lambda_1) * y[:, None] @ g2.reshape(1, -1)))
 
-  def init_q(
+  def init_q(  # noqa: D102
       self,
       ot_prob: Problem_t,
-      key: jnp.ndarray,
+      rng: jax.random.PRNGKeyArray,
       *,
       init_g: jnp.ndarray,
       **kwargs: Any,
   ) -> jnp.ndarray:
-    del key, kwargs
+    del rng, kwargs
     return self._compute_factor(ot_prob, init_g, which="q")
 
-  def init_r(
+  def init_r(  # noqa: D102
       self,
       ot_prob: Problem_t,
-      key: jnp.ndarray,
+      rng: jax.random.PRNGKeyArray,
       *,
       init_g: jnp.ndarray,
       **kwargs: Any,
   ) -> jnp.ndarray:
-    del key, kwargs
+    del rng, kwargs
     return self._compute_factor(ot_prob, init_g, which="r")
 
-  def init_g(
+  def init_g(  # noqa: D102
       self,
       ot_prob: Problem_t,
-      key: jnp.ndarray,
+      rng: jax.random.PRNGKeyArray,
       **kwargs: Any,
   ) -> jnp.ndarray:
-    del key, kwargs
+    del rng, kwargs
     return jnp.ones((self.rank,)) / self.rank
 
 
 @jax.tree_util.register_pytree_node_class
 class KMeansInitializer(LRInitializer):
   """K-means initializer for low-rank Sinkhorn :cite:`scetbon:22b`.
 
@@ -370,15 +383,15 @@
     raise TypeError(
         f"k-means initializer not implemented for `{type(geom).__name__}`."
     )
 
   def _compute_factor(
       self,
       ot_prob: Problem_t,
-      key: jnp.ndarray,
+      rng: jax.random.PRNGKeyArray,
       *,
       init_g: jnp.ndarray,
       which: Literal["q", "r"],
       **kwargs: Any,
   ) -> jnp.ndarray:
     from ott.problems.linear import linear_problem
     from ott.problems.quadratic import quadratic_problem
@@ -396,57 +409,57 @@
     if isinstance(ot_prob, quadratic_problem.QuadraticProblem):
       geom = ot_prob.geom_xx if which == "q" else ot_prob.geom_yy
     else:
       geom = ot_prob.geom
     arr = self._extract_array(geom, first=which == "q")
     marginals = ot_prob.a if which == "q" else ot_prob.b
 
-    centroids = fn(arr, self.rank, key=key).centroids
+    centroids = fn(arr, self.rank, rng=rng).centroids
     geom = pointcloud.PointCloud(
         arr, centroids, epsilon=0.1, scale_cost="max_cost"
     )
 
     prob = linear_problem.LinearProblem(geom, marginals, init_g)
     solver = sinkhorn.Sinkhorn(**self._sinkhorn_kwargs)
     return solver(prob).matrix
 
-  def init_q(
+  def init_q(  # noqa: D102
       self,
       ot_prob: Problem_t,
-      key: jnp.ndarray,
+      rng: jax.random.PRNGKeyArray,
       *,
       init_g: jnp.ndarray,
       **kwargs: Any,
   ) -> jnp.ndarray:
     return self._compute_factor(
-        ot_prob, key, init_g=init_g, which="q", **kwargs
+        ot_prob, rng, init_g=init_g, which="q", **kwargs
     )
 
-  def init_r(
+  def init_r(  # noqa: D102
       self,
       ot_prob: Problem_t,
-      key: jnp.ndarray,
+      rng: jax.random.PRNGKeyArray,
       *,
       init_g: jnp.ndarray,
       **kwargs: Any,
   ) -> jnp.ndarray:
     return self._compute_factor(
-        ot_prob, key, init_g=init_g, which="r", **kwargs
+        ot_prob, rng, init_g=init_g, which="r", **kwargs
     )
 
-  def init_g(
+  def init_g(  # noqa: D102
       self,
       ot_prob: Problem_t,
-      key: jnp.ndarray,
+      rng: jax.random.PRNGKeyArray,
       **kwargs: Any,
   ) -> jnp.ndarray:
-    del key, kwargs
+    del rng, kwargs
     return jnp.ones((self.rank,)) / self.rank
 
-  def tree_flatten(self) -> Tuple[Sequence[Any], Dict[str, Any]]:
+  def tree_flatten(self) -> Tuple[Sequence[Any], Dict[str, Any]]:  # noqa: D102
     children, aux_data = super().tree_flatten()
     aux_data["sinkhorn_kwargs"] = self._sinkhorn_kwargs
     aux_data["min_iterations"] = self._min_iter
     aux_data["max_iterations"] = self._max_iter
     return children, aux_data
 
 
@@ -501,27 +514,27 @@
     factor: jnp.ndarray
     criterions: jnp.ndarray
     crossed_threshold: bool
 
   def _compute_factor(
       self,
       ot_prob: Problem_t,
-      key: jnp.ndarray,
+      rng: jax.random.PRNGKeyArray,
       *,
       init_g: jnp.ndarray,
       which: Literal["q", "r"],
       **kwargs: Any,
   ) -> jnp.ndarray:
     from ott.problems.linear import linear_problem
     from ott.problems.quadratic import quadratic_problem
     from ott.solvers.linear import sinkhorn
 
     def init_fn() -> GeneralizedKMeansInitializer.State:
       n = geom.shape[0]
-      factor = jnp.abs(jax.random.normal(key, (n, self.rank))) + 1.  # (n, r)
+      factor = jnp.abs(jax.random.normal(rng, (n, self.rank))) + 1.  # (n, r)
       factor *= consts.marginal[:, None] / jnp.sum(
           factor, axis=1, keepdims=True
       )
 
       return self.State(
           factor,
           criterions=-jnp.ones(outer_iterations),
@@ -626,15 +639,15 @@
     fixpoint_fn = (
         fixed_point_loop.fixpoint_iter
         if force_scan else fixed_point_loop.fixpoint_iter_backprop
     )
 
     consts = self.Constants(
         solver=sinkhorn.Sinkhorn(**self._sinkhorn_kwargs),
-        geom=geom._set_scale_cost("max_cost"),
+        geom=geom.set_scale_cost("max_cost"),
         marginal=ot_prob.a if which == "q" else ot_prob.b,
         g=init_g,
         gamma=self._kwargs["gamma"],
         threshold=self._kwargs["threshold"],
     )
 
     return fixpoint_fn(
```

### Comparing `ott-jax-0.4.0/src/ott/initializers/nn/initializers.py` & `ott-jax-0.4.1/src/ott/initializers/nn/initializers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,31 @@
+# Copyright OTT-JAX
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#   http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 import functools
 from typing import TYPE_CHECKING, Any, Dict, Optional, Sequence, Tuple
 
 import jax
 import jax.numpy as jnp
 import optax
 from flax import linen as nn
+from flax.core import frozen_dict
 from flax.training import train_state
 
+from ott import utils
 from ott.geometry import geometry
 from ott.initializers.linear import initializers
 
 if TYPE_CHECKING:
   from ott.problems.linear import linear_problem
 
 # TODO(michalk8): add initializer for NeuralDual?
@@ -32,15 +47,16 @@
   evaluation. The meta model defaults to the MLP in
   :class:`~ott.initializers.nn.initializers.MetaMLP` and, with batched problem
   instances passed into :meth:`update`.
 
   Args:
     geom: The fixed geometry of the problem instances.
     meta_model: The model to predict the potential :math:`f` from the measures.
-    opt: The optimizer to update the parameters.
+    opt: The optimizer to update the parameters. If ``None``, use
+      :func:`optax.adam` with :math:`0.001` learning rate.
     rng: The PRNG key to use for initializing the model.
     state: The training state of the model to start from.
 
   Examples:
     The following code shows a simple
     example of using ``update`` to train the model, where
     ``a`` and ``b`` are the weights of the measures and
@@ -56,33 +72,35 @@
         )
   """
 
   def __init__(
       self,
       geom: geometry.Geometry,
       meta_model: Optional[nn.Module] = None,
-      opt: optax.GradientTransformation = optax.adam(learning_rate=1e-3),
-      rng: jax.random.PRNGKeyArray = jax.random.PRNGKey(0),
+      opt: Optional[optax.GradientTransformation
+                   ] = optax.adam(learning_rate=1e-3),  # noqa: B008
+      rng: Optional[jax.random.PRNGKeyArray] = None,
       state: Optional[train_state.TrainState] = None
   ):
     self.geom = geom
     self.dtype = geom.x.dtype
     self.opt = opt
-    self.rng = rng
+    self.rng = utils.default_prng_key(rng)
 
     na, nb = geom.shape
     self.meta_model = MetaMLP(
         potential_size=na
     ) if meta_model is None else meta_model
 
     if state is None:
       # Initialize the model's training state.
       a_placeholder = jnp.zeros(na, dtype=self.dtype)
       b_placeholder = jnp.zeros(nb, dtype=self.dtype)
-      params = self.meta_model.init(rng, a_placeholder, b_placeholder)['params']
+      params = self.meta_model.init(self.rng, a_placeholder,
+                                    b_placeholder)["params"]
       self.state = train_state.TrainState.create(
           apply_fn=self.meta_model.apply, params=params, tx=opt
       )
     else:
       self.state = state
 
     self.update_impl = self._get_update_fn()
@@ -98,52 +116,57 @@
     to optimize the dual objective, which :math:`f^\star` also optimizes for.
     The overall learning setup can thus be written as:
 
     .. math::
       \min_\theta\; {\mathbb E}_{(\alpha,\beta)\sim{\mathcal{D}}}\;
         J(\hat f_\theta(a, b); \alpha, \beta),
 
-    where :math:`a,b` are the probabilities of the measures :math:`\alpha,\beta`,
-    :math:`\mathcal{D}` is a meta distribution of optimal transport problems,
+    where :math:`a,b` are the probabilities of the measures :math:`\alpha,\beta`
+    ,:math:`\mathcal{D}` is a meta distribution of optimal transport problems,
 
     .. math::
       -J(f; \alpha, \beta, c) := \langle f, a\rangle + \langle g, b \rangle -
-        \varepsilon\left\langle \exp\{f/\varepsilon\}, K\exp\{g/\varepsilon\}\right\rangle
+      \varepsilon\left\langle \exp\{f/\varepsilon\}, K\exp\{g/\varepsilon\}
+      \right\rangle
 
     is the entropic dual objective,
     and :math:`K_{i,j} := -C_{i,j}/\varepsilon` is the *Gibbs kernel*.
 
     Args:
       state: Optimizer state of the meta model.
-      a: Probabilites of the :math:`\alpha` measure's atoms.
-      b: Probabilites of the :math:`\beta` measure's atoms.
+      a: Probabilities of the :math:`\alpha` measure's atoms.
+      b: Probabilities of the :math:`\beta` measure's atoms.
 
     Returns:
       The training loss, :math:`f`, and updated state.
     """
     return self.update_impl(state, a, b)
 
-  def init_dual_a(
-      self, ot_prob: 'linear_problem.LinearProblem', lse_mode: bool
+  def init_dual_a(  # noqa: D102
+      self,
+      ot_prob: "linear_problem.LinearProblem",
+      lse_mode: bool,
+      rng: Optional[jax.random.PRNGKeyArray] = None,
   ) -> jnp.ndarray:
+    del rng
     # Detect if the problem is batched.
-    assert ot_prob.a.ndim in (1, 2) and ot_prob.b.ndim in (1, 2)
+    assert ot_prob.a.ndim in (1, 2)
+    assert ot_prob.b.ndim in (1, 2)
     vmap_a_val = 0 if ot_prob.a.ndim == 2 else None
     vmap_b_val = 0 if ot_prob.b.ndim == 2 else None
 
     if vmap_a_val is not None or vmap_b_val is not None:
       compute_f_maybe_batch = jax.vmap(
           self._compute_f, in_axes=(vmap_a_val, vmap_b_val, None)
       )
     else:
       compute_f_maybe_batch = self._compute_f
 
     init_f = compute_f_maybe_batch(ot_prob.a, ot_prob.b, self.state.params)
-    f_u = init_f if lse_mode else ot_prob.geom.scaling_from_potential(init_f)
-    return f_u
+    return init_f if lse_mode else ot_prob.geom.scaling_from_potential(init_f)
 
   def _get_update_fn(self):
     """Return the implementation (and jitted) update function."""
     from ott.problems.linear import linear_problem
     from ott.solvers.linear import sinkhorn
 
     def dual_obj_loss_single(params, a, b):
@@ -169,31 +192,34 @@
       b = jnp.atleast_2d(b)
       grad_fn = jax.value_and_grad(loss_batch, has_aux=True)
       (loss, init_f), grads = grad_fn(state.params, a, b)
       return loss, init_f, state.apply_gradients(grads=grads)
 
     return update
 
-  def _compute_f(self, a, b, params):
+  def _compute_f(
+      self, a: jnp.ndarray, b: jnp.ndarray,
+      params: frozen_dict.FrozenDict[str, jnp.ndarray]
+  ) -> jnp.ndarray:
     r"""Predict the optimal :math:`f` potential.
 
     Args:
-      a: Probabilites of the :math:`\alpha` measure's atoms.
-      b: Probabilites of the :math:`\beta` measure's atoms.
+      a: Probabilities of the :math:`\alpha` measure's atoms.
+      b: Probabilities of the :math:`\beta` measure's atoms.
       params: The parameters of the Meta model.
 
     Returns:
       The :math:`f` potential.
     """
-    return self.meta_model.apply({'params': params}, a, b)
+    return self.meta_model.apply({"params": params}, a, b)
 
-  def tree_flatten(self) -> Tuple[Sequence[Any], Dict[str, Any]]:
+  def tree_flatten(self) -> Tuple[Sequence[Any], Dict[str, Any]]:  # noqa: D102
     return [self.geom, self.meta_model, self.opt], {
-        'rng': self.rng,
-        'state': self.state
+        "rng": self.rng,
+        "state": self.state
     }
 
 
 class MetaMLP(nn.Module):
   r"""Potential for :class:`~ott.initializers.nn.initializers.MetaInitializer`.
 
   This provides an MLP :math:`\hat f_\theta(a, b)` that maps from the
@@ -220,9 +246,8 @@
     Returns:
       The :math:`f` potential.
     """
     dtype = a.dtype
     z = jnp.concatenate((a, b))
     for _ in range(self.num_hidden_layers):
       z = nn.relu(nn.Dense(self.num_hidden_units, dtype=dtype)(z))
-    f = nn.Dense(self.potential_size, dtype=dtype)(z)
-    return f
+    return nn.Dense(self.potential_size, dtype=dtype)(z)
```

### Comparing `ott-jax-0.4.0/src/ott/initializers/quadratic/initializers.py` & `ott-jax-0.4.1/src/ott/initializers/quadratic/initializers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+# Copyright OTT-JAX
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#   http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 import abc
 from typing import TYPE_CHECKING, Any, Dict, Sequence, Tuple
 
 import jax
 import jax.numpy as jnp
 
 from ott.geometry import geometry
@@ -22,16 +35,16 @@
     kwargs: Keyword arguments.
   """
 
   def __init__(self, **kwargs: Any):
     self._kwargs = kwargs
 
   def __call__(
-      self, quad_prob: 'quadratic_problem.QuadraticProblem', **kwargs: Any
-  ) -> 'linear_problem.LinearProblem':
+      self, quad_prob: "quadratic_problem.QuadraticProblem", **kwargs: Any
+  ) -> "linear_problem.LinearProblem":
     """Compute the initial linearization of a quadratic problem.
 
     Args:
       quad_prob: Quadratic problem to linearize.
       kwargs: Additional keyword arguments.
 
     Returns:
@@ -49,38 +62,38 @@
         b=quad_prob.b,
         tau_a=quad_prob.tau_a,
         tau_b=quad_prob.tau_b
     )
 
   @abc.abstractmethod
   def _create_geometry(
-      self, quad_prob: 'quadratic_problem.QuadraticProblem', **kwargs: Any
+      self, quad_prob: "quadratic_problem.QuadraticProblem", **kwargs: Any
   ) -> geometry.Geometry:
     """Compute initial geometry for linearization.
 
     Args:
-      quad_problem: Quadratic problem.
+      quad_prob: Quadratic problem.
       kwargs: Additional keyword arguments.
 
     Returns:
       Geometry used to initialize the linearized problem.
     """
 
-  def tree_flatten(self) -> Tuple[Sequence[Any], Dict[str, Any]]:
+  def tree_flatten(self) -> Tuple[Sequence[Any], Dict[str, Any]]:  # noqa: D102
     return [], self._kwargs
 
   @classmethod
-  def tree_unflatten(
+  def tree_unflatten(  # noqa: D102
       cls, aux_data: Dict[str, Any], children: Sequence[Any]
   ) -> "BaseQuadraticInitializer":
     return cls(*children, **aux_data)
 
 
 class QuadraticInitializer(BaseQuadraticInitializer):
-  """Initialize a linear problem locally around a naive initializer ab'.
+  r"""Initialize a linear problem locally around :math:`ab^T` initializer.
 
   If the problem is balanced (``tau_a = 1`` and ``tau_b = 1``),
   the equation of the cost follows eq. 6, p. 1 of :cite:`peyre:16`.
 
   If the problem is unbalanced (``tau_a < 1`` or ``tau_b < 1``), there are two
   possible cases. A first possibility is to introduce a quadratic KL
   divergence on the marginals in the objective as done in :cite:`sejourne:21`
@@ -91,28 +104,28 @@
   local cost unchanged, i.e. follow eq. 6, p. 1 of :cite:`peyre:16`
   (``gw_unbalanced_correction = False``) and include the unbalanced terms
   at the level of the linear problem only.
 
   Let :math:`P` [num_a, num_b] be the transport matrix, `cost_xx` is the
   cost matrix of `geom_xx` and `cost_yy` is the cost matrix of `geom_yy`.
   `left_x` and `right_y` depend on the loss chosen for GW.
-  `gw_unbalanced_correction` is an boolean indicating whether or not the
-  unbalanced correction applies.
-  The equation of the local cost can be written as:
-
-  `cost_matrix` = `marginal_dep_term`
-              + `left_x`(`cost_xx`) :math:`P` `right_y`(`cost_yy`):math:`^T`
-              + `unbalanced_correction` * `gw_unbalanced_correction`
+  `gw_unbalanced_correction` is flag indicating whether the unbalanced
+  correction applies. The equation of the local cost can be written as:
+
+  .. math::
+
+    \text{marginal_dep_term} + \text{left}_x(\text{cost_xx}) P
+     \text{right}_y(\text{cost_yy}) + \text{unbalanced_correction}
 
   When working with the fused problem, a linear term is added to the cost
   matrix: `cost_matrix` += `fused_penalty` * `geom_xy.cost_matrix`
   """
 
   def _create_geometry(
-      self, quad_prob: 'quadratic_problem.QuadraticProblem', *, epsilon: float,
+      self, quad_prob: "quadratic_problem.QuadraticProblem", *, epsilon: float,
       **kwargs: Any
   ) -> geometry.Geometry:
     """Compute initial geometry for linearization.
 
     Args:
       quad_prob: Quadratic OT problem.
       epsilon: Epsilon regularization.
@@ -143,31 +156,31 @@
           epsilon=epsilon, transport_mass=marginal_1.sum()
       )
       unbalanced_correction = quad_prob.cost_unbalanced_correction(
           init_transport, marginal_1, marginal_2, epsilon=epsilon
       )
       cost_matrix = marginal_cost.cost_matrix - tmp + unbalanced_correction
 
-    cost_matrix += quad_prob.fused_penalty * quad_prob._fused_cost_matrix
+    cost_matrix += quad_prob.fused_penalty * quad_prob._fused_cost_matrix()
     return geometry.Geometry(cost_matrix=cost_matrix, epsilon=epsilon)
 
 
 class LRQuadraticInitializer(BaseQuadraticInitializer):
   """Wrapper that wraps low-rank Sinkhorn initializers.
 
   Args:
     lr_linear_initializer: Low-rank linear initializer.
   """
 
-  def __init__(self, lr_linear_initializer: 'initializers_lr.LRInitializer'):
+  def __init__(self, lr_linear_initializer: "initializers_lr.LRInitializer"):
     super().__init__()
     self._linear_lr_initializer = lr_linear_initializer
 
   def _create_geometry(
-      self, quad_prob: 'quadratic_problem.QuadraticProblem', **kwargs: Any
+      self, quad_prob: "quadratic_problem.QuadraticProblem", **kwargs: Any
   ) -> geometry.Geometry:
     """Compute initial geometry for linearization.
 
     Args:
       quad_prob: Quadratic OT problem.
       kwargs: Keyword arguments for
         :meth:`~ott.initializers.linear.initializers_lr.LRInitializer.__call__`.
@@ -185,10 +198,10 @@
     return quad_prob.update_lr_geom(tmp_out)
 
   @property
   def rank(self) -> int:
     """Rank of the transport matrix factorization."""
     return self._linear_lr_initializer.rank
 
-  def tree_flatten(self) -> Tuple[Sequence[Any], Dict[str, Any]]:
+  def tree_flatten(self) -> Tuple[Sequence[Any], Dict[str, Any]]:  # noqa: D102
     children, aux_data = super().tree_flatten()
     return children + [self._linear_lr_initializer], aux_data
```

### Comparing `ott-jax-0.4.0/src/ott/math/fixed_point_loop.py` & `ott-jax-0.4.1/src/ott/math/fixed_point_loop.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-# Copyright 2022 Google LLC.
+# Copyright OTT-JAX
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-#     http://www.apache.org/licenses/LICENSE-2.0
+#   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""jheek@ backprop-friendly implementation of fixed point loop."""
 from typing import Any, Callable
 
 import jax
 import jax.numpy as jnp
 import numpy as np
 
 __all__ = ["fixpoint_iter", "fixpoint_iter_backprop"]
```

### Comparing `ott-jax-0.4.0/src/ott/math/matrix_square_root.py` & `ott-jax-0.4.1/src/ott/math/matrix_square_root.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-# Copyright 2022 Google LLC.
+# Copyright OTT-JAX
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-#     http://www.apache.org/licenses/LICENSE-2.0
+#   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""A Jax backprop friendly version of Matrix square root."""
-
 import functools
 from typing import Tuple
 
 import jax
 import jax.numpy as jnp
 import numpy as np
 
@@ -43,24 +41,25 @@
     threshold: convergence tolerance threshold for Newton-Schulz iterations.
     min_iterations: min number of iterations after which error is computed.
     inner_iterations: error is re-evaluated every inner_iterations iterations.
     max_iterations: max number of iterations.
     regularization: small regularizer added to norm of x, before normalization.
 
   Returns:
-    sqrt matrix of x (or x's if batch), its inverse, errors along iterates.
+    Square root matrix of x (or x's if batch), its inverse,
+    errors along iterates.
   """
   dimension = x.shape[-1]
   norm_x = jnp.linalg.norm(x, axis=(-2, -1)) * (1 + regularization)
 
   if jnp.ndim(x) > 2:
     norm_x = norm_x[..., jnp.newaxis, jnp.newaxis]
 
   def cond_fn(iteration, const, state):
-    """Stopping criterion. Checking decrease of objective is needed here."""  # noqa: D401
+    """Stopping criterion. Checking decrease of objective is needed here."""
     _, threshold = const
     errors, _, _ = state
     err = errors[iteration // inner_iterations - 1]
 
     return jnp.logical_or(
         iteration == 0,
         jnp.logical_and(
@@ -180,15 +179,16 @@
     inner_iterations: int,
     max_iterations: int,
     regularization: float,
     residual: Tuple[jnp.ndarray, jnp.ndarray],
     cotangent: Tuple[jnp.ndarray, jnp.ndarray, jnp.ndarray],
 ) -> Tuple[jnp.ndarray]:
   """Compute the derivative by solving a Sylvester equation."""
-  del threshold, min_iterations, inner_iterations, max_iterations, regularization
+  del threshold, min_iterations, inner_iterations, \
+      max_iterations, regularization
   sqrt_x, inv_sqrt_x = residual
   # ignores cotangent associated with errors
   cot_sqrt, cot_inv_sqrt, _ = cotangent
 
   # Solve for d(X^{1/2}):
   # Start with X^{1/2} X^{1/2} = X
   # Differentiate to obtain
@@ -232,94 +232,97 @@
 sqrtm.defvjp(sqrtm_fwd, sqrtm_bwd)
 
 # Specialized versions of sqrtm that compute only the square root or inverse.
 # These functions have lower complexity gradients than sqrtm.
 
 
 @functools.partial(jax.custom_vjp, nondiff_argnums=(1, 2, 3, 4, 5))
-def sqrtm_only(
+def sqrtm_only(  # noqa: D103
     x: jnp.ndarray,
     threshold: float = 1e-6,
     min_iterations: int = 0,
     inner_iterations: int = 10,
     max_iterations: int = 1000,
     regularization: float = 1e-6
 ) -> jnp.ndarray:
   return sqrtm(
       x, threshold, min_iterations, inner_iterations, max_iterations,
       regularization
   )[0]
 
 
-def sqrtm_only_fwd(
+def sqrtm_only_fwd(  # noqa: D103
     x: jnp.ndarray, threshold: float, min_iterations: int,
     inner_iterations: int, max_iterations: int, regularization: float
 ) -> Tuple[jnp.ndarray, jnp.ndarray]:
   sqrt_x = sqrtm(
       x, threshold, min_iterations, inner_iterations, max_iterations,
       regularization
   )[0]
   return sqrt_x, sqrt_x
 
 
-def sqrtm_only_bwd(
+def sqrtm_only_bwd(  # noqa: D103
     threshold: float, min_iterations: int, inner_iterations: int,
     max_iterations: int, regularization: float, sqrt_x: jnp.ndarray,
     cotangent: jnp.ndarray
 ) -> Tuple[jnp.ndarray]:
-  del threshold, min_iterations, inner_iterations
-  del max_iterations, regularization
+  del threshold, min_iterations, inner_iterations, \
+    max_iterations, regularization
   vjp = jnp.swapaxes(
       solve_sylvester_bartels_stewart(
           a=sqrt_x, b=-sqrt_x, c=jnp.swapaxes(cotangent, axis1=-2, axis2=-1)
       ),
       axis1=-2,
       axis2=-1
   )
   return vjp,
 
 
 sqrtm_only.defvjp(sqrtm_only_fwd, sqrtm_only_bwd)
 
 
 @functools.partial(jax.custom_vjp, nondiff_argnums=(1, 2, 3, 4, 5))
-def inv_sqrtm_only(
+def inv_sqrtm_only(  # noqa: D103
     x: jnp.ndarray,
     threshold: float = 1e-6,
     min_iterations: int = 0,
     inner_iterations: int = 10,
     max_iterations: int = 1000,
     regularization: float = 1e-6
 ) -> jnp.ndarray:
   return sqrtm(
       x, threshold, min_iterations, inner_iterations, max_iterations,
       regularization
   )[1]
 
 
-def inv_sqrtm_only_fwd(
+def inv_sqrtm_only_fwd(  # noqa: D103
     x: jnp.ndarray,
     threshold: float,
     min_iterations: int,
     inner_iterations: int,
     max_iterations: int,
     regularization: float,
 ) -> Tuple[jnp.ndarray, jnp.ndarray]:
   inv_sqrt_x = sqrtm(
       x, threshold, min_iterations, inner_iterations, max_iterations,
       regularization
   )[1]
   return inv_sqrt_x, inv_sqrt_x
 
 
-def inv_sqrtm_only_bwd(
+def inv_sqrtm_only_bwd(  # noqa: D103
     threshold: float, min_iterations: int, inner_iterations: int,
     max_iterations: int, regularization: float, residual: jnp.ndarray,
     cotangent: jnp.ndarray
 ) -> Tuple[jnp.ndarray]:
+  del threshold, min_iterations, inner_iterations, \
+    max_iterations, regularization
+
   inv_sqrt_x = residual
   inv_x = jnp.matmul(inv_sqrt_x, inv_sqrt_x)
   vjp = jnp.swapaxes(
       solve_sylvester_bartels_stewart(
           a=inv_sqrt_x,
           b=-inv_sqrt_x,
           c=-jnp.matmul(
```

### Comparing `ott-jax-0.4.0/src/ott/math/unbalanced_functions.py` & `ott-jax-0.4.1/src/ott/math/unbalanced_functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,33 @@
-# Copyright 2022 Google LLC.
+# Copyright OTT-JAX
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-#     http://www.apache.org/licenses/LICENSE-2.0
+#   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Functions useful to define unbalanced OT problems."""
 from typing import Callable
 
 import jax.numpy as jnp
 
 
 def phi_star(h: jnp.ndarray, rho: float) -> jnp.ndarray:
   """Legendre transform of KL, :cite:`sejourne:19`, p. 9."""
   return rho * (jnp.exp(h / rho) - 1)
 
 
-# TODO(cuturi): use jax.grad directly.
 def derivative_phi_star(f: jnp.ndarray, rho: float) -> jnp.ndarray:
-  """Derivative of Legendre transform of phi_starKL, see phi_star."""  # noqa: D401
+  """Derivative of Legendre transform of phi_starKL, see phi_star."""
+  # TODO(cuturi): use jax.grad directly.
   return jnp.exp(f / rho)
 
 
 def grad_of_marginal_fit(
     c: jnp.ndarray, h: jnp.ndarray, tau: float, epsilon: float
 ) -> jnp.ndarray:
   """Compute grad of terms linked to marginals in objective.
@@ -83,9 +82,9 @@
   return jnp.where(
       c > 0,
       c * second_derivative_phi_star(-h, r) *
       derivative(c * derivative_phi_star(-h, r)), 0.0
   )
 
 
-def rho(epsilon: float, tau: float) -> float:
+def rho(epsilon: float, tau: float) -> float:  # noqa: D103
   return (epsilon * tau) / (1. - tau)
```

### Comparing `ott-jax-0.4.0/src/ott/problems/linear/barycenter_problem.py` & `ott-jax-0.4.1/src/ott/problems/linear/barycenter_problem.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,33 @@
-# Copyright 2022 Apple Inc
+# Copyright OTT-JAX
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-#     http://www.apache.org/licenses/LICENSE-2.0
+#   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Classes defining OT problem(s) (objective function + utilities)."""
 from typing import Any, Dict, Optional, Sequence, Tuple
 
 import jax
 import jax.numpy as jnp
 
-from ott.geometry import costs, segment
+from ott.geometry import costs, geometry, segment
 
-__all__ = ["BarycenterProblem"]
+__all__ = ["FreeBarycenterProblem"]
 
 
 @jax.tree_util.register_pytree_node_class
-class BarycenterProblem:
-  """Wasserstein barycenter problem :cite:`cuturi:14`.
+class FreeBarycenterProblem:
+  """Free Wasserstein barycenter problem :cite:`cuturi:14`.
 
   Args:
     y: Array of shape ``[num_total_points, ndim]`` merging the points of all
       measures. Alternatively, already segmented array of shape
       ``[num_measures, max_measure_size, ndim]`` can be passed.
       See also :func:`~ott.geometry.segment.segment_point_cloud`.
     b: Array of shape ``[num_total_points,]`` containing the weights of all
@@ -41,18 +40,16 @@
     cost_fn: Cost function used. If `None`,
       use the :class:`~ott.geometry.costs.SqEuclidean` cost.
     epsilon: Epsilon regularization used to solve reg-OT problems.
     debiased: **Currently not implemented.**
       Whether the problem is debiased, in the sense that
       the regularized transportation cost of barycenter to itself will
       be considered when computing gradient. Note that if the debiased option
-      is used, the barycenter size in
-      :meth:`~ott.solvers.linear.continuous_barycenter.WassersteinBarycenter.init_state`
-      needs to be smaller than the maximum measure size for parallelization to
-      operate efficiently.
+      is used, the barycenter size needs to be smaller than the maximum measure
+      size for parallelization to operate efficiently.
     kwargs: Keyword arguments :func:`~ott.geometry.segment.segment_point_cloud`.
       Only used when ``y`` is not already segmented. When passing
       ``segment_ids``, 2 arguments must be specified for jitting to work:
 
         - ``num_segments`` - the total number of measures.
         - ``max_measure_size`` -  maximum of support sizes of these measures.
   """
@@ -154,28 +151,79 @@
       weights = jnp.ones((self.num_measures,)) / self.num_measures
     else:
       # Check that the number of measures coincides with the weights' size.
       assert self._weights.shape[0] == self.num_measures
       # By default, we assume that weights sum to 1, and enforce this if needed.
       weights = self._weights / jnp.sum(self._weights)
     if self.debiased:
-      weights = jnp.concatenate((weights, jnp.array([-0.5])))
+      return jnp.concatenate((weights, jnp.array([-0.5])))
     return weights
 
   @property
   def _is_segmented(self) -> bool:
     return self._y.ndim == 3
 
-  def tree_flatten(self) -> Tuple[Sequence[Any], Dict[str, Any]]:
+  def tree_flatten(self) -> Tuple[Sequence[Any], Dict[str, Any]]:  # noqa: D102
     return ([self._y, self._b, self._weights], {
-        'cost_fn': self.cost_fn,
-        'epsilon': self.epsilon,
-        'debiased': self.debiased,
+        "cost_fn": self.cost_fn,
+        "epsilon": self.epsilon,
+        "debiased": self.debiased,
         **self._kwargs,
     })
 
   @classmethod
-  def tree_unflatten(
+  def tree_unflatten(  # noqa: D102
       cls, aux_data: Dict[str, Any], children: Sequence[Any]
-  ) -> "BarycenterProblem":
+  ) -> "FreeBarycenterProblem":
     y, b, weights = children
     return cls(y=y, b=b, weights=weights, **aux_data)
+
+
+@jax.tree_util.register_pytree_node_class
+class FixedBarycenterProblem:
+  """Fixed-support Wasserstein barycenter problem.
+
+  Args:
+    geom: Geometry object.
+    a: batch of histograms of shape ``[batch, num_a]`` where ``num_a`` matches
+      the first value of the :attr:`~ott.geometry.Geometry.shape` attribute of
+      ``geom``.
+    weights: ``[batch,]`` positive weights summing to :math`1`. Uniform by
+      default.
+  """
+
+  def __init__(
+      self,
+      geom: geometry.Geometry,
+      a: jnp.ndarray,
+      weights: Optional[jnp.ndarray] = None,
+  ):
+    self.geom = geom
+    self.a = a
+    self._weights = weights
+
+  @property
+  def num_measures(self) -> int:
+    """Number of measures."""
+    return self.a.shape[0]
+
+  @property
+  def weights(self) -> jnp.ndarray:
+    """Barycenter weights of shape ``[num_measures,]`` that sum to :math`1`."""
+    if self._weights is None:
+      return jnp.ones((self.num_measures,)) / self.num_measures
+
+    # check that the number of measures coincides with the weights' size
+    assert self._weights.shape[0] == self.num_measures
+    # by default, we assume that weights sum to 1, and enforce this if needed
+    return self._weights / jnp.sum(self._weights)
+
+  def tree_flatten(self):  # noqa: D102
+    return [self.geom, self.a, self._weights], None
+
+  @classmethod
+  def tree_unflatten(  # noqa: D102
+      cls, aux_data: Dict[str, Any], children: Sequence[Any]
+  ) -> "FixedBarycenterProblem":
+    del aux_data
+    geom, a, weights = children
+    return cls(geom=geom, a=a, weights=weights)
```

### Comparing `ott-jax-0.4.0/src/ott/problems/linear/linear_problem.py` & `ott-jax-0.4.1/src/ott/problems/linear/linear_problem.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-# Copyright 2022 Google LLC.
+# Copyright OTT-JAX
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-#     http://www.apache.org/licenses/LICENSE-2.0
+#   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Classes defining OT problem(s) (objective function + utilities)."""
-
 from typing import Any, Callable, Dict, Optional, Sequence, Tuple
 
 import jax
 import jax.numpy as jnp
 
 from ott.geometry import geometry
 
@@ -37,19 +35,19 @@
   clouds or the support of measures, followed by probability masses ``a`` and
   ``b``. Unbalancedness of the problem is also kept track of, through two
   coefficients ``tau_a`` and ``tau_b``, which are both kept between 0 and 1
   (1 corresponding to a balanced OT problem).
 
   Args:
     geom: The ground geometry cost of the linear problem.
-    a: The first marginal. If `None`, it will be uniform.
-    b: The second marginal. If `None`, it will be uniform.
-    tau_a: If `< 1`, defines how much unbalanced the problem is
+    a: The first marginal. If ``None``, it will be uniform.
+    b: The second marginal. If ``None``, it will be uniform.
+    tau_a: If :math:`<1`, defines how much unbalanced the problem is
       on the first marginal.
-    tau_b: If `< 1`, defines how much unbalanced the problem is
+    tau_b: If :math:`< 1`, defines how much unbalanced the problem is
       on the second marginal.
   """
 
   def __init__(
       self,
       geom: geometry.Geometry,
       a: Optional[jnp.ndarray] = None,
@@ -103,18 +101,18 @@
       )
       app_transport = lambda f, g, z, axis: geom.apply_transport_from_scalings(
           geom.scaling_from_potential(f), geom.scaling_from_potential(g), z,
           axis
       )
     return marginal_a, marginal_b, app_transport
 
-  def tree_flatten(self) -> Tuple[Sequence[Any], Dict[str, Any]]:
+  def tree_flatten(self) -> Tuple[Sequence[Any], Dict[str, Any]]:  # noqa: D102
     return ([self.geom, self._a, self._b], {
-        'tau_a': self.tau_a,
-        'tau_b': self.tau_b
+        "tau_a": self.tau_a,
+        "tau_b": self.tau_b
     })
 
   @classmethod
-  def tree_unflatten(
+  def tree_unflatten(  # noqa: D102
       cls, aux_data: Dict[str, Any], children: Sequence[Any]
   ) -> "LinearProblem":
     return cls(*children, **aux_data)
```

### Comparing `ott-jax-0.4.0/src/ott/problems/linear/potentials.py` & `ott-jax-0.4.1/src/ott/problems/linear/potentials.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+# Copyright OTT-JAX
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#   http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     Literal,
     Optional,
@@ -11,22 +24,25 @@
 
 import jax
 import jax.numpy as jnp
 import jax.scipy as jsp
 import jax.tree_util as jtu
 import numpy as np
 
-import matplotlib
-import matplotlib.pyplot as plt
-
 from ott.problems.linear import linear_problem
 
 if TYPE_CHECKING:
   from ott.geometry import costs
 
+try:
+  import matplotlib as mpl
+  import matplotlib.pyplot as plt
+except ImportError:
+  mpl = plt = None
+
 __all__ = ["DualPotentials", "EntropicPotentials"]
 Potential_t = Callable[[jnp.ndarray], float]
 
 
 @jtu.register_pytree_node_class
 class DualPotentials:
   r"""The Kantorovich dual potential functions :math:`f` and :math:`g`.
@@ -44,32 +60,33 @@
   """
 
   def __init__(
       self,
       f: Potential_t,
       g: Potential_t,
       *,
-      cost_fn: 'costs.CostFn',
+      cost_fn: "costs.CostFn",
       corr: bool = False
   ):
     self._f = f
     self._g = g
     self.cost_fn = cost_fn
     self._corr = corr
 
   def transport(self, vec: jnp.ndarray, forward: bool = True) -> jnp.ndarray:
     r"""Transport ``vec`` according to Brenier formula :cite:`brenier:91`.
 
     Uses Theorem 1.17 from :cite:`santambrogio:15` to compute an OT map when
     given the Legendre transform of the dual potentials.
 
-    That OT map can be recovered as :math:`x- (\nabla h)^{-1}\circ \nabla f(x)`
-    For the case :math:`h(\cdot) = \|\cdot\|^2, \nabla h(\cdot) = 2 \cdot\,`,
-    and as a consequence :math:`h^*(\cdot) = \|.\|^2 / 4`, while one has that
-    :math:`\nabla h^*(\cdot) = (\nabla h)^{-1}(\cdot) = 0.5 \cdot\,`.
+    That OT map can be recovered as :math:`x- (\nabla h^*)\circ \nabla f(x)`,
+    where :math:`h^*` is the Legendre transform of :math:`h`. For instance,
+    in the case :math:`h(\cdot) = \|\cdot\|^2, \nabla h(\cdot) = 2 \cdot\,`,
+    one has :math:`h^*(\cdot) = \|.\|^2 / 4`, and therefore
+    :math:`\nabla h^*(\cdot) = 0.5 \cdot\,`.
 
     When the dual potentials are solved in correlation form (only in the Sq.
     Euclidean distance case), the maps are :math:`\nabla g` for forward,
     :math:`\nabla f` for backward.
 
     Args:
       vec: Points to transport, array of shape ``[n, d]``.
@@ -82,16 +99,15 @@
     from ott.geometry import costs
 
     vec = jnp.atleast_2d(vec)
     if self._corr and isinstance(self.cost_fn, costs.SqEuclidean):
       return self._grad_f(vec) if forward else self._grad_g(vec)
     if forward:
       return vec - self._grad_h_inv(self._grad_f(vec))
-    else:
-      return vec - self._grad_h_inv(self._grad_g(vec))
+    return vec - self._grad_h_inv(self._grad_g(vec))
 
   def distance(self, src: jnp.ndarray, tgt: jnp.ndarray) -> float:
     """Evaluate 2-Wasserstein distance between samples using dual potentials.
 
     Uses Eq. 5 from :cite:`makkuva:20` when given in `corr` form, direct
     estimation by integrating dual function against points when using dual form.
 
@@ -143,59 +159,64 @@
 
     assert isinstance(self.cost_fn, costs.TICost), (
         "Cost must be a `TICost` and "
         "provide access to Legendre transform of `h`."
     )
     return jax.vmap(jax.grad(self.cost_fn.h_legendre))
 
-  def tree_flatten(self) -> Tuple[Sequence[Any], Dict[str, Any]]:
+  def tree_flatten(self) -> Tuple[Sequence[Any], Dict[str, Any]]:  # noqa: D102
     return [], {
         "f": self._f,
         "g": self._g,
         "cost_fn": self.cost_fn,
         "corr": self._corr
     }
 
   @classmethod
-  def tree_unflatten(
+  def tree_unflatten(  # noqa: D102
       cls, aux_data: Dict[str, Any], children: Sequence[Any]
   ) -> "DualPotentials":
     return cls(*children, **aux_data)
 
   def plot_ot_map(
       self,
       source: jnp.ndarray,
       target: jnp.ndarray,
       forward: bool = True,
-      ax: Optional[matplotlib.axes.Axes] = None,
+      ax: Optional["plt.Axes"] = None,
       legend_kwargs: Optional[Dict[str, Any]] = None,
       scatter_kwargs: Optional[Dict[str, Any]] = None,
-  ) -> Tuple[matplotlib.figure.Figure, matplotlib.axes.Axes]:
+  ) -> Tuple["plt.Figure", "plt.Axes"]:
     """Plot data and learned optimal transport map.
 
     Args:
       source: samples from the source measure
       target: samples from the target measure
       forward: use the forward map from the potentials
         if ``True``, otherwise use the inverse map
       ax: axis to add the plot to
-      scatter_kwargs: additional kwargs passed into :meth:`~matplotlib.axes.Axes.scatter`
-      legend_kwargs: additional kwargs passed into :meth:`~matplotlib.axes.Axes.legend`
+      scatter_kwargs: additional kwargs passed into
+        :meth:`~matplotlib.axes.Axes.scatter`
+      legend_kwargs: additional kwargs passed into
+        :meth:`~matplotlib.axes.Axes.legend`
 
     Returns:
-      matplotlib figure and axis with the plots
+      a `matplotlib` figure and axis with the plots
     """
+    if mpl is None:
+      raise RuntimeError("Please install `matplotlib` first.")
+
     if scatter_kwargs is None:
-      scatter_kwargs = {'alpha': 0.5}
+      scatter_kwargs = {"alpha": 0.5}
     if legend_kwargs is None:
       legend_kwargs = {
-          'ncol': 3,
-          'loc': 'upper center',
-          'bbox_to_anchor': (0.5, -0.05),
-          'edgecolor': 'k'
+          "ncol": 3,
+          "loc": "upper center",
+          "bbox_to_anchor": (0.5, -0.05),
+          "edgecolor": "k"
       }
 
     if ax is None:
       fig = plt.figure(facecolor="white")
       ax = fig.add_subplot(111)
     else:
       fig = ax.get_figure()
@@ -208,22 +229,22 @@
       label_transport = r"$\nabla g(target)$"
       source_color, target_color = "#A7BED3", "#1A254B"
 
     ax.scatter(
         source[:, 0],
         source[:, 1],
         color=source_color,
-        label='source',
+        label="source",
         **scatter_kwargs,
     )
     ax.scatter(
         target[:, 0],
         target[:, 1],
         color=target_color,
-        label='target',
+        label="target",
         **scatter_kwargs,
     )
 
     # plot the transported samples
     base_samples = source if forward else target
     transported_samples = self.transport(base_samples, forward=forward)
     ax.scatter(
@@ -247,36 +268,38 @@
     ax.legend(**legend_kwargs)
     return fig, ax
 
   def plot_potential(
       self,
       forward: bool = True,
       quantile: float = 0.05,
-      ax: Optional[matplotlib.axes.Axes] = None,
+      ax: Optional["mpl.axes.Axes"] = None,
       x_bounds: Tuple[float, float] = (-6, 6),
       y_bounds: Tuple[float, float] = (-6, 6),
       num_grid: int = 50,
       contourf_kwargs: Optional[Dict[str, Any]] = None,
-  ) -> Tuple[matplotlib.figure.Figure, matplotlib.axes.Axes]:
-    """Plot the potential.
+  ) -> Tuple["mpl.figure.Figure", "mpl.axes.Axes"]:
+    r"""Plot the potential.
 
     Args:
       forward: use the forward map from the potentials
         if ``True``, otherwise use the inverse map
       quantile: quantile to filter the potentials with
       ax: axis to add the plot to
-      x_bounds: x-axis bounds of the plot (xmin, xmax)
-      y_bounds: y-axis bounds of the plot (ymin, ymax)
+      x_bounds: x-axis bounds of the plot
+        :math:`(x_{\text{min}}, x_{\text{max}})`
+      y_bounds: y-axis bounds of the plot
+        :math:`(y_{\text{min}}, y_{\text{max}})`
       num_grid: number of points to discretize the domain into a grid
         along each dimension
       contourf_kwargs: additional kwargs passed into
         :meth:`~matplotlib.axes.Axes.contourf`
 
     Returns:
-      matplotlib figure and axis with the plots.
+      a `matplotlib` figure with axis, with the plots.
     """
     if contourf_kwargs is None:
       contourf_kwargs = {}
 
     ax_specified = ax is not None
     if not ax_specified:
       fig, ax = plt.subplots(figsize=(6, 6), facecolor="white")
@@ -330,19 +353,19 @@
     # since only the properties need to be callable
     super().__init__(f_xy, g_xy, cost_fn=prob.geom.cost_fn, corr=False)
     self._prob = prob
     self._f_xx = f_xx
     self._g_yy = g_yy
 
   @property
-  def f(self) -> Potential_t:
+  def f(self) -> Potential_t:  # noqa: D102
     return self._potential_fn(kind="f")
 
   @property
-  def g(self) -> Potential_t:
+  def g(self) -> Potential_t:  # noqa: D102
     return self._potential_fn(kind="g")
 
   def _potential_fn(self, *, kind: Literal["f", "g"]) -> Potential_t:
     from ott.geometry import pointcloud
 
     def callback(
         x: jnp.ndarray,
@@ -397,9 +420,9 @@
     return self._f_xx is not None and self._g_yy is not None
 
   @property
   def epsilon(self) -> float:
     """Entropy regularizer."""
     return self._prob.geom.epsilon
 
-  def tree_flatten(self) -> Tuple[Sequence[Any], Dict[str, Any]]:
+  def tree_flatten(self) -> Tuple[Sequence[Any], Dict[str, Any]]:  # noqa: D102
     return [self._f, self._g, self._prob, self._f_xx, self._g_yy], {}
```

### Comparing `ott-jax-0.4.0/src/ott/problems/nn/dataset.py` & `ott-jax-0.4.1/src/ott/problems/nn/dataset.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,146 +1,154 @@
+# Copyright OTT-JAX
+#
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Toy datasets for neural OT."""
-
 import dataclasses
-from typing import Iterable, Iterator, Literal, NamedTuple, Tuple
+from typing import Iterator, Literal, NamedTuple, Optional, Tuple
 
 import jax
 import jax.numpy as jnp
 import numpy as np
 
-__all__ = ['create_gaussian_mixture_samplers', 'Dataset', 'GaussianMixture']
+__all__ = ["create_gaussian_mixture_samplers", "Dataset", "GaussianMixture"]
 
-Name_t = Literal['simple', 'circle', 'square_five', 'square_four']
+from ott import utils
+
+Name_t = Literal["simple", "circle", "square_five", "square_four"]
 
 
 class Dataset(NamedTuple):
   r"""Samplers from source and target measures.
 
   Args:
     source_iter: loader for the source measure
     target_iter: loader for the target measure
   """
-  source_iter: Iterable[jnp.ndarray]
-  target_iter: Iterable[jnp.ndarray]
+  source_iter: Iterator[jnp.ndarray]
+  target_iter: Iterator[jnp.ndarray]
 
 
 @dataclasses.dataclass
 class GaussianMixture:
   """A mixture of Gaussians.
 
   Args:
     name: the name specifying the centers of the mixture components:
 
-        - ``simple`` (data clustered in one center),
-        - ``circle`` (two-dimensional Gaussians arranged on a circle),
-        - ``square_five`` (two-dimensional Gaussians on a square with
-          one Gaussian in the center), and
-        - ``square_four`` (two-dimensional Gaussians in the corners of a rectangle)
+      - ``simple`` - data clustered in one center,
+      - ``circle`` - two-dimensional Gaussians arranged on a circle,
+      - ``square_five`` - two-dimensional Gaussians on a square with
+        one Gaussian in the center, and
+      - ``square_four`` - two-dimensional Gaussians in the corners of a
+        rectangle
 
     batch_size: batch size of the samples
-    init_key: initial PRNG key
+    init_rng: initial PRNG key
     scale: scale of the individual Gaussian samples
     variance: the variance of the individual Gaussian samples
   """
   name: Name_t
   batch_size: int
-  init_key: jax.random.PRNGKey
+  init_rng: jax.random.PRNGKeyArray
   scale: float = 5.0
   variance: float = 0.5
 
   def __post_init__(self):
     gaussian_centers = {
-        'simple':
+        "simple":
             np.array([[0, 0]]),
-        'circle':
+        "circle":
             np.array([
                 (1, 0),
                 (-1, 0),
                 (0, 1),
                 (0, -1),
                 (1.0 / np.sqrt(2), 1.0 / np.sqrt(2)),
                 (1.0 / np.sqrt(2), -1.0 / np.sqrt(2)),
                 (-1.0 / np.sqrt(2), 1.0 / np.sqrt(2)),
                 (-1.0 / np.sqrt(2), -1.0 / np.sqrt(2)),
             ]),
-        'square_five':
+        "square_five":
             np.array([[0, 0], [1, 1], [-1, 1], [-1, -1], [1, -1]]),
-        'square_four':
+        "square_four":
             np.array([[1, 0], [0, 1], [-1, 0], [0, -1]]),
     }
     if self.name not in gaussian_centers:
       raise ValueError(
-          f'{self.name} is not a valid dataset for GaussianMixture'
+          f"{self.name} is not a valid dataset for GaussianMixture"
       )
     self.centers = gaussian_centers[self.name]
 
   def __iter__(self) -> Iterator[jnp.array]:
-    return self.create_sample_generators()
+    """Random sample generator from Gaussian mixture.
+
+    Returns:
+      A generator of samples from the Gaussian mixture.
+    """
+    return self._create_sample_generators()
 
-  def create_sample_generators(self) -> Iterator[jnp.array]:
-    # create generator which randomly picks center and adds noise
-    key = self.init_key
+  def _create_sample_generators(self) -> Iterator[jnp.array]:
+    rng = self.init_rng
     while True:
-      k1, k2, key = jax.random.split(key, 3)
-      means = jax.random.choice(k1, self.centers, [self.batch_size])
-      normal_samples = jax.random.normal(k2, [self.batch_size, 2])
+      rng1, rng2, rng = jax.random.split(rng, 3)
+      means = jax.random.choice(rng1, self.centers, [self.batch_size])
+      normal_samples = jax.random.normal(rng2, [self.batch_size, 2])
       samples = self.scale * means + self.variance ** 2 * normal_samples
       yield samples
 
 
 def create_gaussian_mixture_samplers(
     name_source: Name_t,
     name_target: Name_t,
     train_batch_size: int = 2048,
     valid_batch_size: int = 2048,
-    key: jax.random.PRNGKey = jax.random.PRNGKey(0),
+    rng: Optional[jax.random.PRNGKeyArray] = None,
 ) -> Tuple[Dataset, Dataset, int]:
-  """Creates Gaussian samplers for :class:`~ott.solvers.nn.neuraldual.W2NeuralDual`.
+  """Gaussian samplers for :class:`~ott.solvers.nn.neuraldual.W2NeuralDual`.
 
   Args:
     name_source: name of the source sampler
     name_target: name of the target sampler
     train_batch_size: the training batch size
     valid_batch_size: the validation batch size
-    key: initial PRNG key
+    rng: initial PRNG key
 
   Returns:
     The dataset and dimension of the data.
   """
-  k1, k2, k3, k4 = jax.random.split(key, 4)
+  rng = utils.default_prng_key(rng)
+  rng1, rng2, rng3, rng4 = jax.random.split(rng, 4)
   train_dataset = Dataset(
       source_iter=iter(
           GaussianMixture(
-              name_source, batch_size=train_batch_size, init_key=k1
+              name_source, batch_size=train_batch_size, init_rng=rng1
           )
       ),
       target_iter=iter(
           GaussianMixture(
-              name_target, batch_size=train_batch_size, init_key=k2
+              name_target, batch_size=train_batch_size, init_rng=rng2
           )
       )
   )
   valid_dataset = Dataset(
       source_iter=iter(
           GaussianMixture(
-              name_source, batch_size=valid_batch_size, init_key=k3
+              name_source, batch_size=valid_batch_size, init_rng=rng3
           )
       ),
       target_iter=iter(
           GaussianMixture(
-              name_target, batch_size=valid_batch_size, init_key=k4
+              name_target, batch_size=valid_batch_size, init_rng=rng4
           )
       )
   )
   dim_data = 2
   return train_dataset, valid_dataset, dim_data
```

### Comparing `ott-jax-0.4.0/src/ott/problems/quadratic/gw_barycenter.py` & `ott-jax-0.4.1/src/ott/problems/quadratic/gw_barycenter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+# Copyright OTT-JAX
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#   http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 import functools
 from typing import Any, Dict, Literal, Optional, Sequence, Tuple, Union
 
 import jax
 import jax.numpy as jnp
 
 from ott.geometry import costs, geometry, pointcloud, segment
@@ -10,15 +23,15 @@
 from ott.problems.quadratic import quadratic_costs, quadratic_problem
 
 __all__ = ["GWBarycenterProblem"]
 
 
 # TODO(michalk8): better abstraction (common superclass for Wasserstein bary)
 @jax.tree_util.register_pytree_node_class
-class GWBarycenterProblem(barycenter_problem.BarycenterProblem):
+class GWBarycenterProblem(barycenter_problem.FreeBarycenterProblem):
   """(Fused) Gromov-Wasserstein barycenter problem :cite:`peyre:16,vayer:19`.
 
   Args:
     y: Array of shape ``[num_total_points, ndim]`` merging the points of all
       measures. Alternatively, already segmented array of shape
       ``[num_measures, max_measure_size, ndim]`` can be passed.
       See also :func:`~ott.geometry.segment.segment_point_cloud`.
@@ -49,15 +62,15 @@
       self,
       y: Optional[jnp.ndarray] = None,
       b: Optional[jnp.ndarray] = None,
       weights: Optional[jnp.ndarray] = None,
       costs: Optional[jnp.ndarray] = None,
       y_fused: Optional[jnp.ndarray] = None,
       fused_penalty: float = 1.0,
-      gw_loss: Literal['sqeucl', 'kl'] = 'sqeucl',
+      gw_loss: Literal["sqeucl", "kl"] = "sqeucl",
       scale_cost: Union[int, float, Literal["mean", "max_cost"]] = 1.0,
       **kwargs: Any,
   ):
     assert y is None or costs is None, "Cannot specify both `y` and `costs`."
     y = y if costs is None else costs
 
     super().__init__(y=y, b=b, weights=weights, **kwargs)
@@ -115,26 +128,26 @@
           transport.T,
           axis=0,
           fn=fn,
           is_linear=lin,
       )
       return transport @ tmp
 
-    fn = None if self._loss_name == 'sqeucl' else self.gw_loss.h2
+    fn = None if self._loss_name == "sqeucl" else self.gw_loss.h2
     y, b = self.segmented_y_b
     weights = self.weights[:, None, None]
 
     barycenter = jnp.sum(weights * project(y, b, transports, fn), axis=0)
     inv_a = jnp.where(a > 0, 1.0 / a, 1.0)
     barycenter = (barycenter * inv_a[None, :]) * inv_a[:, None]
 
     # TODO(michalk8): in future, use `isinstanceof(self.gw_loss, ...)`
     # once refactoring has been done
-    if self._loss_name == 'kl':
-      barycenter = jnp.exp(barycenter)
+    if self._loss_name == "kl":
+      return jnp.exp(barycenter)
     return barycenter
 
   def update_features(self, transports: jnp.ndarray,
                       a: jnp.ndarray) -> Optional[jnp.ndarray]:
     """Update the barycenter features in the fused case :cite:`vayer:19`.
 
     Uses :cite:`cuturi:14` eq. 8, and is implemented only
@@ -217,15 +230,15 @@
         scale_cost=self.scale_cost,
         src_mask=src_mask,
         tgt_mask=tgt_mask
     )
 
   def _create_problem(
       self,
-      state: 'GWBarycenterState',  # noqa: F821
+      state: "GWBarycenterState",  # noqa: F821
       y: jnp.ndarray,
       b: jnp.ndarray,
       f: Optional[jnp.ndarray] = None
   ) -> quadratic_problem.QuadraticProblem:
     # TODO(michalk8): in future, mask in the problem for convenience?
     bary_mask = state.a > 0.
     y_mask = b > 0.
@@ -253,61 +266,60 @@
   @property
   def is_fused(self) -> bool:
     """Whether the problem is fused."""
     return self._y_fused is not None
 
   @property
   def segmented_y_fused(self) -> Optional[jnp.ndarray]:
-    """Feature array of shape ``[num_measures, max_measure_size, ndim_fused]`` \
-    used in the fused case."""
+    """Feature array of shape used in the fused case."""
     if not self.is_fused or self._y_fused.ndim == 3:
       return self._y_fused
     y_fused, _ = segment.segment_point_cloud(
         x=self._y_fused,
         padding_vector=self.cost_fn._padder(self.ndim_fused),
         **self._kwargs
     )
     return y_fused
 
   @property
-  def ndim(self) -> Optional[int]:
+  def ndim(self) -> Optional[int]:  # noqa: D102
     return None if self._y_as_costs else self._y.shape[-1]
 
   @property
   def ndim_fused(self) -> Optional[int]:
     """Number of dimensions of the fused term."""
     return self._y_fused.shape[-1] if self.is_fused else None
 
   @property
   def gw_loss(self) -> quadratic_costs.GWLoss:
     """Gromov-Wasserstein loss."""
     # TODO(michalk8): custom losses would require inverting some fns;
     # `https://jax.readthedocs.io/en/latest/notebooks/ some fns;
     # Writing_custom_interpreters_in_Jax.html#your-first-interpreter-invert`
     # might be useful
-    if self._loss_name == 'sqeucl':
+    if self._loss_name == "sqeucl":
       return quadratic_costs.make_square_loss()
-    if self._loss_name == 'kl':
+    if self._loss_name == "kl":
       return quadratic_costs.make_kl_loss()
     raise NotImplementedError(
         f"Loss `{self._loss_name}` is not yet implemented."
     )
 
-  def tree_flatten(self) -> Tuple[Sequence[Any], Dict[str, Any]]:
+  def tree_flatten(self) -> Tuple[Sequence[Any], Dict[str, Any]]:  # noqa: D102
     (y, b, weights), aux = super().tree_flatten()
     if self._y_as_costs:
       children = [None, b, weights, y]
     else:
       children = [y, b, weights, None]
-    aux['fused_penalty'] = self.fused_penalty
-    aux['gw_loss'] = self._loss_name
-    aux['scale_cost'] = self.scale_cost
+    aux["fused_penalty"] = self.fused_penalty
+    aux["gw_loss"] = self._loss_name
+    aux["scale_cost"] = self.scale_cost
     return children + [self._y_fused], aux
 
   @classmethod
-  def tree_unflatten(
+  def tree_unflatten(  # noqa: D102
       cls, aux_data: Dict[str, Any], children: Sequence[Any]
   ) -> "GWBarycenterProblem":
     y, b, weights, costs, y_fused = children
     return cls(
         y=y, b=b, weights=weights, costs=costs, y_fused=y_fused, **aux_data
     )
```

### Comparing `ott-jax-0.4.0/src/ott/problems/quadratic/quadratic_costs.py` & `ott-jax-0.4.1/src/ott/problems/quadratic/quadratic_costs.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,47 @@
+# Copyright OTT-JAX
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#   http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 from typing import Callable, NamedTuple
 
 import jax
 import jax.numpy as jnp
 
 __all__ = ["make_square_loss", "make_kl_loss"]
 
 
-class Loss(NamedTuple):
+class Loss(NamedTuple):  # noqa: D101
   func: Callable[[jnp.ndarray], jnp.ndarray]
   is_linear: bool
 
 
-class GWLoss(NamedTuple):
+class GWLoss(NamedTuple):  # noqa: D101
   f1: Loss
   f2: Loss
   h1: Loss
   h2: Loss
 
 
-def make_square_loss() -> GWLoss:
+def make_square_loss() -> GWLoss:  # noqa: D103
   f1 = Loss(lambda x: x ** 2, is_linear=False)
   f2 = Loss(lambda y: y ** 2, is_linear=False)
   h1 = Loss(lambda x: x, is_linear=True)
   h2 = Loss(lambda y: 2.0 * y, is_linear=True)
   return GWLoss(f1, f2, h1, h2)
 
 
-def make_kl_loss(clipping_value: float = 1e-8) -> GWLoss:
+def make_kl_loss(clipping_value: float = 1e-8) -> GWLoss:  # noqa: D103
   f1 = Loss(lambda x: -jax.scipy.special.entr(x) - x, is_linear=False)
   f2 = Loss(lambda y: y, is_linear=True)
   h1 = Loss(lambda x: x, is_linear=True)
   h2 = Loss(lambda y: jnp.log(jnp.clip(y, clipping_value)), is_linear=False)
   return GWLoss(f1, f2, h1, h2)
```

### Comparing `ott-jax-0.4.0/src/ott/problems/quadratic/quadratic_problem.py` & `ott-jax-0.4.1/src/ott/problems/quadratic/quadratic_problem.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,27 @@
-# Copyright 2022 Google LLC.
+# Copyright OTT-JAX
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-#     http://www.apache.org/licenses/LICENSE-2.0
+#   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Classes defining OT problem(s) (objective function + utilities)."""
-
 from typing import TYPE_CHECKING, Literal, Optional, Tuple, Union
 
 import jax
 import jax.numpy as jnp
 import jax.scipy as jsp
 
+from ott import utils
 from ott.geometry import epsilon_scheduler, geometry, low_rank, pointcloud
 from ott.problems.linear import linear_problem
 from ott.problems.quadratic import quadratic_costs
 from ott.types import Transport
 
 if TYPE_CHECKING:
   from ott.solvers.linear import sinkhorn_lr
@@ -74,16 +73,16 @@
       computations. Alternatively, KL loss can be specified in no less optimized
       way.
     tau_a: if `< 1.0`, defines how much unbalanced the problem is on
       the first marginal.
     tau_b: if `< 1.0`, defines how much unbalanced the problem is on
       the second marginal.
     gw_unbalanced_correction: Whether the unbalanced version of
-      :cite:`sejourne:21` is used. Otherwise, ``tau_a`` and ``tau_b`` only affect
-      the inner Sinkhorn loop.
+      :cite:`sejourne:21` is used. Otherwise, ``tau_a`` and ``tau_b``
+      only affect the inner Sinkhorn loop.
     ranks: Ranks of the cost matrices, see
       :meth:`~ott.geometry.geometry.Geometry.to_LRCGeometry`. Used when
       geometries are *not* :class:`~ott.geometry.pointcloud.PointCloud` with
       `'sqeucl'` cost function. If `-1`, the geometries will not be converted
       to low-rank. If :class:`tuple`, it specifies the ranks of ``geom_xx``,
       ``geom_yy`` and ``geom_xy``, respectively. If :class:`int`, rank is shared
       across all geometries.
@@ -97,76 +96,92 @@
       geom_xx: geometry.Geometry,
       geom_yy: geometry.Geometry,
       geom_xy: Optional[geometry.Geometry] = None,
       fused_penalty: float = 1.0,
       scale_cost: Optional[Union[bool, float, str]] = False,
       a: Optional[jnp.ndarray] = None,
       b: Optional[jnp.ndarray] = None,
-      loss: Union[Literal['sqeucl', 'kl'], quadratic_costs.GWLoss] = 'sqeucl',
+      loss: Union[Literal["sqeucl", "kl"], quadratic_costs.GWLoss] = "sqeucl",
       tau_a: Optional[float] = 1.0,
       tau_b: Optional[float] = 1.0,
       gw_unbalanced_correction: bool = True,
       ranks: Union[int, Tuple[int, ...]] = -1,
       tolerances: Union[float, Tuple[float, ...]] = 1e-2,
   ):
-    self._geom_xx = geom_xx._set_scale_cost(scale_cost)
-    self._geom_yy = geom_yy._set_scale_cost(scale_cost)
+    self._geom_xx = geom_xx.set_scale_cost(scale_cost)
+    self._geom_yy = geom_yy.set_scale_cost(scale_cost)
     self._geom_xy = (
-        None if geom_xy is None else geom_xy._set_scale_cost(scale_cost)
+        None if geom_xy is None else geom_xy.set_scale_cost(scale_cost)
     )
     self.fused_penalty = fused_penalty
     self.scale_cost = scale_cost
     self._a = a
     self._b = b
     self.tau_a = tau_a
     self.tau_b = tau_b
     self.gw_unbalanced_correction = gw_unbalanced_correction
     self.ranks = ranks
     self.tolerances = tolerances
 
     self._loss_name = loss
-    if self._loss_name == 'sqeucl':
+    if self._loss_name == "sqeucl":
       self.loss = quadratic_costs.make_square_loss()
-    elif loss == 'kl':
+    elif loss == "kl":
       self.loss = quadratic_costs.make_kl_loss()
     else:
       self.loss = loss
 
   def marginal_dependent_cost(
-      self, marginal_1: jnp.ndarray, marginal_2: jnp.ndarray
+      self,
+      marginal_1: jnp.ndarray,
+      marginal_2: jnp.ndarray,
+      *,
+      remove_scale: bool = False,
   ) -> low_rank.LRCGeometry:
-    r"""Initialise cost term that depends on the marginals of the transport.
+    r"""Initialize cost term that depends on the marginals of the transport.
 
     Uses the first term in eq. 6, p. 1 of :cite:`peyre:16`.
 
-    Let :math:`p` [num_a,] be the marginal of the transport matrix for samples
-    from `geom_xx` and :math:`q` [num_b,] be the marginal of the transport
-    matrix for samples from `geom_yy`. `cost_xx` (resp. `cost_yy`) is the
-    cost matrix of `geom_xx` (resp. `geom_yy`). The cost term that
-    depends on these marginals can be written as:
+    Let :math:`p` be the `[n,]` marginal of the transport matrix for samples
+    from :attr:`geom_xx` and :math:`q` the `[m,]` marginal of the
+    transport matrix for samples from :attr:`geom_yy`.
+
+    When ``cost_xx`` (resp. ``cost_yy``) is the cost matrix of :attr:`geom_xx`
+    (resp. :attr:`geom_yy`), the cost term that depends on these marginals can
+    be written as:
 
-    `marginal_dep_term` = `lin1`(`cost_xx`) :math:`p \mathbb{1}_{num_b}^T`
-                      + (`lin2`(`cost_yy`) :math:`q \mathbb{1}_{num_a}^T)^T`
+    .. math::
+
+      \text{marginal_dep_term} = \text{lin1}(\text{cost_xx}) p \mathbb{1}_{m}^T
+                      +  \mathbb{1}_{n}(\text{lin2}(\text{cost_yy}) q)^T
+
+    This helper function instantiates these two low-rank matrices and groups
+    them into a single low-rank cost geometry object.
 
     Args:
-      marginal_1: jnp.ndarray<float>[num_a,], marginal of the transport matrix
-       for samples from geom_xx
-      marginal_2: jnp.ndarray<float>[num_b,], marginal of the transport matrix
-       for samples from geom_yy
+      marginal_1: [n,], first marginal of transport matrix.
+      marginal_2: [m,], second marginal of transport matrix.
+      remove_scale: Whether to remove any scaling from the cost matrices before
+        computing the linearization.
 
     Returns:
-      Low-rank geometry.
+      Low-rank geometry of rank 2, storing normalization constants.
     """
-    if self._loss_name == 'sqeucl':  # quadratic apply, efficient for LR
-      tmp1 = self.geom_xx.apply_square_cost(marginal_1, axis=1)
-      tmp2 = self.geom_yy.apply_square_cost(marginal_2, axis=1)
+    geom_xx, geom_yy = self.geom_xx, self.geom_yy
+    if remove_scale:
+      geom_xx = geom_xx.set_scale_cost(1.0)
+      geom_yy = geom_yy.set_scale_cost(1.0)
+
+    if self._loss_name == "sqeucl":  # quadratic apply, efficient for LR
+      tmp1 = geom_xx.apply_square_cost(marginal_1, axis=1)
+      tmp2 = geom_yy.apply_square_cost(marginal_2, axis=1)
     else:
       f1, f2 = self.linear_loss
-      tmp1 = apply_cost(self.geom_xx, marginal_1, axis=1, fn=f1)
-      tmp2 = apply_cost(self.geom_yy, marginal_2, axis=1, fn=f2)
+      tmp1 = apply_cost(geom_xx, marginal_1, axis=1, fn=f1)
+      tmp2 = apply_cost(geom_yy, marginal_2, axis=1, fn=f2)
     x_term = jnp.concatenate((tmp1, jnp.ones_like(tmp1)), axis=1)
     y_term = jnp.concatenate((jnp.ones_like(tmp2), tmp2), axis=1)
     return low_rank.LRCGeometry(cost_1=x_term, cost_2=y_term)
 
   def cost_unbalanced_correction(
       self,
       transport_matrix: jnp.ndarray,
@@ -194,15 +209,15 @@
 
     Args:
       transport_matrix: jnp.ndarray<float>[num_a, num_b], transport matrix.
       marginal_1: jnp.ndarray<float>[num_a,], marginal of the transport matrix
         for samples from :attr:`geom_xx`.
       marginal_2: jnp.ndarray<float>[num_b,], marginal of the transport matrix
         for samples from :attr:`geom_yy`.
-      epsilon: regulariser.
+      epsilon: entropy regularizer.
 
     Returns:
       The cost term.
     """
 
     def regularizer(tau: float) -> float:
       return eps * tau / (1.0 - tau)
@@ -220,55 +235,65 @@
       cost += regularizer(
           self.tau_b
       ) * (-jsp.special.entr(marginal_2).sum() - marginal_2logb)
     return cost
 
   # TODO(michalk8): highly coupled to the pre-defined initializer, refactor
   def init_transport_mass(self) -> float:
-    """Initialise the transport mass.
+    """Initialize the transport mass.
 
     Returns:
-      The sum of the elements of the normalised transport matrix.
+      The sum of the elements of the normalized transport matrix.
     """
     a = jax.lax.stop_gradient(self.a)
     b = jax.lax.stop_gradient(self.b)
     return a.sum() * b.sum()
 
   def update_lr_geom(
-      self, lr_sink: 'sinkhorn_lr.LRSinkhornOutput'
+      self,
+      lr_sink: "sinkhorn_lr.LRSinkhornOutput",
+      remove_scale: bool = False,
   ) -> geometry.Geometry:
     """Recompute (possibly LRC) linearization using LR Sinkhorn output."""
     marginal_1 = lr_sink.marginal(1)
     marginal_2 = lr_sink.marginal(0)
-    marginal_cost = self.marginal_dependent_cost(marginal_1, marginal_2)
+    marginal_cost = self.marginal_dependent_cost(
+        marginal_1, marginal_2, remove_scale=remove_scale
+    )
 
     # Extract factors from LR Sinkhorn output
     q, r, inv_sqg = lr_sink.q, lr_sink.r, 1.0 / jnp.sqrt(lr_sink.g)
     # Distribute middle marginal evenly across both factors.
     q, r = q * inv_sqg[None, :], r * inv_sqg[None, :]
 
     # Handle LRC Geometry case.
     h1, h2 = self.quad_loss
-    tmp1 = apply_cost(self.geom_xx, q, axis=1, fn=h1)
-    tmp2 = apply_cost(self.geom_yy, r, axis=1, fn=h2)
+    geom_xx, geom_yy, geom_xy = self.geom_xx, self.geom_yy, self.geom_xy
+    if remove_scale:
+      geom_xx = geom_xx.set_scale_cost(1.0)
+      geom_yy = geom_yy.set_scale_cost(1.0)
+      geom_xy = geom_xy.set_scale_cost(1.0) if self.is_fused else None
+    tmp1 = apply_cost(geom_xx, q, axis=1, fn=h1)
+    tmp2 = apply_cost(geom_yy, r, axis=1, fn=h2)
     if self.is_low_rank:
       geom = low_rank.LRCGeometry(cost_1=tmp1, cost_2=-tmp2) + marginal_cost
       if self.is_fused:
-        geom = geom + self.geom_xy
+        geom = geom + geom_xy
     else:
       cost_matrix = marginal_cost.cost_matrix - jnp.dot(tmp1, tmp2.T)
-      cost_matrix += self.fused_penalty * self._fused_cost_matrix
+      cost_matrix += self.fused_penalty * self._fused_cost_matrix(remove_scale)
       geom = geometry.Geometry(cost_matrix=cost_matrix)
-    return geom
+    return geom  # noqa: RET504
 
   def update_linearization(
       self,
       transport: Transport,
       epsilon: Optional[Union[epsilon_scheduler.Epsilon, float]] = None,
-      old_transport_mass: float = 1.0
+      old_transport_mass: float = 1.0,
+      remove_scale: bool = False,
   ) -> linear_problem.LinearProblem:
     """Update linearization of GW problem by updating cost matrix.
 
     If the problem is balanced (``tau_a = 1.0 and tau_b = 1.0``), the equation
     follows eq. 6, p. 1 of :cite:`peyre:16`.
 
     If the problem is unbalanced (``tau_a < 1.0 or tau_b < 1.0``), two cases are
@@ -278,73 +303,92 @@
     :meth:`init_linearization`.
 
     Args:
       transport: Solution of the linearization of the quadratic problem.
       epsilon: An epsilon scheduler or a float passed on to the linearization.
       old_transport_mass: Sum of the elements of the transport matrix at the
         previous iteration.
+      remove_scale: Whether to remove any scaling from the cost matrices when
+        computing the linearization of the quadratic cost. At the moment, this
+        is only used when doing this update at the last outer iteration of the
+        :class:`~ott.solvers.quadratic.gromov_wasserstein.GromovWasserstein`
+        solver.
 
     Returns:
       Updated linear OT problem, a new local linearization of GW problem.
     """
     rescale_factor = 1.0
     unbalanced_correction = 0.0
 
     if not self.is_balanced:
       marginal_1 = transport.marginal(axis=1)
       transport_mass = jax.lax.stop_gradient(marginal_1.sum())
       rescale_factor = jnp.sqrt(old_transport_mass / transport_mass)
 
     marginal_1 = transport.marginal(axis=1) * rescale_factor
     marginal_2 = transport.marginal(axis=0) * rescale_factor
-    marginal_cost = self.marginal_dependent_cost(marginal_1, marginal_2)
+    marginal_cost = self.marginal_dependent_cost(
+        marginal_1, marginal_2, remove_scale=remove_scale
+    )
 
     transport_matrix = transport.matrix * rescale_factor
 
     if not self.is_balanced:
       # Rescales transport for Unbalanced GW according to Sejourne et al. (2021)
       transport_mass = jax.lax.stop_gradient(marginal_1.sum())
       epsilon = update_epsilon_unbalanced(epsilon, transport_mass)
       unbalanced_correction = self.cost_unbalanced_correction(
           transport_matrix, marginal_1, marginal_2, epsilon
       )
 
     h1, h2 = self.quad_loss
-    tmp = apply_cost(self.geom_xx, transport_matrix, axis=1, fn=h1)
-    tmp = apply_cost(self.geom_yy, tmp.T, axis=1, fn=h2).T
+    geom_xx, geom_yy = self.geom_xx, self.geom_yy
+    if remove_scale:
+      geom_xx = geom_xx.set_scale_cost(1.0)
+      geom_yy = geom_yy.set_scale_cost(1.0)
+
+    tmp = apply_cost(geom_xx, transport_matrix, axis=1, fn=h1)
+    tmp = apply_cost(geom_yy, tmp.T, axis=1, fn=h2).T
 
     cost_matrix = marginal_cost.cost_matrix - tmp + unbalanced_correction
-    cost_matrix += self.fused_penalty * self._fused_cost_matrix * rescale_factor
+    cost_matrix += self.fused_penalty * rescale_factor * \
+                   self._fused_cost_matrix(remove_scale)
 
     geom = geometry.Geometry(cost_matrix=cost_matrix, epsilon=epsilon)
+
     return linear_problem.LinearProblem(
         geom, self.a, self.b, tau_a=self.tau_a, tau_b=self.tau_b
     )
 
   def update_lr_linearization(
-      self, lr_sink: 'sinkhorn_lr.LRSinkhornOutput'
+      self,
+      lr_sink: "sinkhorn_lr.LRSinkhornOutput",
+      *,
+      remove_scale: bool = False,
   ) -> linear_problem.LinearProblem:
     """Update a Quad problem linearization using a LR Sinkhorn."""
     return linear_problem.LinearProblem(
-        self.update_lr_geom(lr_sink),
+        self.update_lr_geom(lr_sink, remove_scale=remove_scale),
         self.a,
         self.b,
         tau_a=self.tau_a,
         tau_b=self.tau_b
     )
 
-  @property
-  def _fused_cost_matrix(self) -> Union[float, jnp.ndarray]:
+  def _fused_cost_matrix(self,
+                         unscale: bool = False) -> Union[float, jnp.ndarray]:
     if not self.is_fused:
-      return 0.
-    if isinstance(
-        self.geom_xy, pointcloud.PointCloud
-    ) and self.geom_xy.is_online:
-      return self.geom_xy._compute_cost_matrix() * self.geom_xy.inv_scale_cost
-    return self.geom_xy.cost_matrix
+      return 0.0
+    geom_xy = self.geom_xy
+    if unscale:
+      geom_xy = geom_xy.set_scale_cost(1.0)
+
+    if isinstance(geom_xy, pointcloud.PointCloud) and geom_xy.is_online:
+      return geom_xy._compute_cost_matrix() * geom_xy.inv_scale_cost
+    return geom_xy.cost_matrix
 
   @property
   def _is_low_rank_convertible(self) -> bool:
 
     def convertible(geom: geometry.Geometry) -> bool:
       return isinstance(geom, low_rank.LRCGeometry) or (
           isinstance(geom, pointcloud.PointCloud) and geom.is_squared_euclidean
@@ -356,19 +400,22 @@
     geom_xx, geom_yy, geom_xy = self.geom_xx, self.geom_yy, self.geom_xy
     # either explicitly via cost factorization or implicitly (e.g., a PC)
     return self.ranks != -1 or (
         convertible(geom_xx) and convertible(geom_yy) and
         (geom_xy is None or convertible(geom_xy))
     )
 
-  def to_low_rank(self, seed: int = 0) -> "QuadraticProblem":
+  def to_low_rank(
+      self,
+      rng: Optional[jax.random.PRNGKeyArray] = None,
+  ) -> "QuadraticProblem":
     """Convert geometries to low-rank.
 
     Args:
-      seed: Random seed.
+      rng: Random key for seeding.
 
     Returns:
       Quadratic problem with low-rank geometries.
     """
 
     def convert(
         vals: Union[int, float, Tuple[Union[int, float], ...]]
@@ -378,28 +425,29 @@
         return (vals,) * 3
       assert len(vals) == size, vals
       return vals + (None,) * (3 - size)
 
     if self.is_low_rank:
       return self
 
+    rng = utils.default_prng_key(rng)
+    rng1, rng2, rng3 = jax.random.split(rng, 3)
     (geom_xx, geom_yy, geom_xy, *children), aux_data = self.tree_flatten()
-    (s1, s2, s3) = jax.random.split(jax.random.PRNGKey(seed), 3)[:, 0]
     (r1, r2, r3), (t1, t2, t3) = convert(self.ranks), convert(self.tolerances)
 
-    geom_xx = geom_xx.to_LRCGeometry(rank=r1, tol=t1, seed=s1)
-    geom_yy = geom_yy.to_LRCGeometry(rank=r2, tol=t2, seed=s2)
+    geom_xx = geom_xx.to_LRCGeometry(rank=r1, tol=t1, rng=rng1)
+    geom_yy = geom_yy.to_LRCGeometry(rank=r2, tol=t2, rng=rng2)
     if self.is_fused:
       if isinstance(
           geom_xy, pointcloud.PointCloud
       ) and geom_xy.is_squared_euclidean:
         geom_xy = geom_xy.to_LRCGeometry(scale=self.fused_penalty)
       else:
         geom_xy = geom_xy.to_LRCGeometry(
-            rank=r3, tol=t3, seed=s3, scale=self.fused_penalty
+            rank=r3, tol=t3, rng=rng3, scale=self.fused_penalty
         )
 
     return type(self).tree_unflatten(
         aux_data, [geom_xx, geom_yy, geom_xy] + children
     )
 
   @property
@@ -455,40 +503,38 @@
 
   @property
   def is_balanced(self) -> bool:
     """Whether the problem is balanced."""
     return ((not self.gw_unbalanced_correction) or
             (self.tau_a == 1.0 and self.tau_b == 1.0))
 
-  def tree_flatten(self):
+  def tree_flatten(self):  # noqa: D102
     return ([self.geom_xx, self.geom_yy, self.geom_xy, self._a, self._b], {
-        'tau_a': self.tau_a,
-        'tau_b': self.tau_b,
-        'loss': self._loss_name,
-        'fused_penalty': self.fused_penalty,
-        'scale_cost': self.scale_cost,
-        'gw_unbalanced_correction': self.gw_unbalanced_correction,
-        'ranks': self.ranks,
-        'tolerances': self.tolerances
+        "tau_a": self.tau_a,
+        "tau_b": self.tau_b,
+        "loss": self._loss_name,
+        "fused_penalty": self.fused_penalty,
+        "scale_cost": self.scale_cost,
+        "gw_unbalanced_correction": self.gw_unbalanced_correction,
+        "ranks": self.ranks,
+        "tolerances": self.tolerances
     })
 
   @classmethod
-  def tree_unflatten(cls, aux_data, children):
+  def tree_unflatten(cls, aux_data, children):  # noqa: D102
     geoms, (a, b) = children[:3], children[3:]
     return cls(*geoms, a=a, b=b, **aux_data)
 
 
-def update_epsilon_unbalanced(
+def update_epsilon_unbalanced(  # noqa: D103
     epsilon: Union[float, epsilon_scheduler.Epsilon], transport_mass: float
 ) -> epsilon_scheduler.Epsilon:
-  updated_epsilon = epsilon_scheduler.Epsilon.make(epsilon)
-  updated_epsilon._scale_epsilon = (
-      updated_epsilon._scale_epsilon * transport_mass
-  )
-  return updated_epsilon
+  if not isinstance(epsilon, epsilon_scheduler.Epsilon):
+    epsilon = epsilon_scheduler.Epsilon(epsilon, scale_epsilon=1.0)
+  return epsilon.set(scale_epsilon=epsilon._scale_epsilon * transport_mass)
 
 
-def apply_cost(
+def apply_cost(  # noqa: D103
     geom: geometry.Geometry, arr: jnp.ndarray, *, axis: int,
     fn: quadratic_costs.Loss
 ) -> jnp.ndarray:
   return geom.apply_cost(arr, axis=axis, fn=fn.func, is_linear=fn.is_linear)
```

### Comparing `ott-jax-0.4.0/src/ott/solvers/linear/acceleration.py` & `ott-jax-0.4.1/src/ott/solvers/linear/acceleration.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,29 @@
+# Copyright OTT-JAX
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#   http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 from typing import TYPE_CHECKING
 
 import jax
 import jax.numpy as jnp
 
 from ott import utils
 
 if TYPE_CHECKING:
+  from ott.problems.linear import linear_problem
   from ott.solvers.linear import sinkhorn
 
 __all__ = ["AndersonAcceleration", "Momentum"]
 
 
 @utils.register_pytree_node
 class AndersonAcceleration:
@@ -40,36 +54,37 @@
     # Recover linear combination and return it with NaN (caused
     # by 0 weights leading to -jnp.inf potentials, mixed with weights
     # coefficients of different signs), disambiguated to -inf.
     combination = jnp.sum(fxs * weights[None, :], axis=1)
     return jnp.where(jnp.isfinite(combination), combination, -jnp.inf)
 
   def update(
-      self, state: 'sinkhorn.SinkhornState', iteration: int, pb, lse_mode: bool
-  ) -> 'sinkhorn.SinkhornState':
+      self, state: "sinkhorn.SinkhornState", iteration: int,
+      prob: "linear_problem.LinearProblem", lse_mode: bool
+  ) -> "sinkhorn.SinkhornState":
     """Anderson acceleration update.
 
     When using Anderson acceleration, first update the dual variable f_u with
     previous updates (if iteration count sufficiently large), then record
     new iterations in array.
 
     Anderson acceleration always happens in potentials (not scalings) space,
     regardless of the lse_mode setting. If the iteration count is large
     enough the update below will output a potential variable.
 
     Args:
-      state: A sinkhorn.SinkhornState
-      iteration: int, the current iteration.
-      pb: a problem.LinearProblem defining the OT problem.
+      state: Sinkhorn state.
+      iteration: the current iteration.
+      prob: linear OT problem.
       lse_mode: whether to compute in log-sum-exp or in scalings.
 
     Returns:
       A potential variable.
     """
-    geom = pb.geom
+    geom = prob.geom
     trigger_update = jnp.logical_and(
         iteration > self.memory, iteration % self.refresh_every == 0
     )
     fu = jnp.where(
         trigger_update, self.extrapolation(state.old_fus, state.old_mapped_fus),
         state.fu
     )
@@ -90,67 +105,68 @@
     # from the extrapolation was outputted in potential form.
     fu = jnp.where(
         trigger_update, fu if lse_mode else geom.scaling_from_potential(fu), fu
     )
     return state.set(fu=fu, old_fus=old_fus)
 
   def init_maps(
-      self, pb, state: 'sinkhorn.SinkhornState'
-  ) -> 'sinkhorn.SinkhornState':
-    """Initialize log matrix used in Anderson acceleration with nan values."""
+      self, pb, state: "sinkhorn.SinkhornState"
+  ) -> "sinkhorn.SinkhornState":
+    """Initialize log matrix used in Anderson acceleration with *NaN* values."""
     fus = jnp.ones((pb.geom.shape[0], self.memory)) * jnp.nan
     return state.set(old_fus=fus, old_mapped_fus=fus)
 
   def update_history(
-      self, state: 'sinkhorn.SinkhornState', pb, lse_mode: bool
-  ) -> 'sinkhorn.SinkhornState':
+      self, state: "sinkhorn.SinkhornState", pb, lse_mode: bool
+  ) -> "sinkhorn.SinkhornState":
+    """Update history of mapped dual variables."""
     f = state.fu if lse_mode else pb.geom.potential_from_scaling(state.fu)
     mapped = jnp.concatenate((state.old_mapped_fus[:, 1:], f[:, None]), axis=1)
     return state.set(old_mapped_fus=mapped)
 
 
 @utils.register_pytree_node
 class Momentum:
-  """Momentum for Sinkhorn updates, either constant :cite:`thibault:21` or \
-  adaptive :cite:`lehmann:21`."""
+  """Momentum for Sinkhorn updates.
+
+  Can be either constant :cite:`thibault:21` or adaptive :cite:`lehmann:21`.
+  """
 
   start: int = 0
   error_threshold: float = jnp.inf
   value: float = 1.0
   inner_iterations: int = 1
 
-  def weight(self, state: 'sinkhorn.SinkhornState', iteration: int) -> float:
+  def weight(self, state: "sinkhorn.SinkhornState", iteration: int) -> float:
     """Compute momentum term if needed, using previously seen errors."""
     if self.start == 0:
       return self.value
     idx = self.start // self.inner_iterations
 
-    weight = jax.lax.cond(
+    return jax.lax.cond(
         jnp.logical_and(
             iteration >= self.start,
             state.errors[idx - 1, -1] < self.error_threshold
         ), lambda state: self.lehmann(state), lambda state: self.value, state
     )
-    return weight
 
-  def lehmann(self, state: 'sinkhorn.SinkhornState') -> float:
+  def lehmann(self, state: "sinkhorn.SinkhornState") -> float:
     """Momentum formula :cite:`lehmann:21`, eq. 5."""
     idx = self.start // self.inner_iterations
     error_ratio = jnp.minimum(
         state.errors[idx - 1, -1] / state.errors[idx - 2, -1], 0.99
     )
     power = 1.0 / self.inner_iterations
     return 2.0 / (1.0 + jnp.sqrt(1.0 - error_ratio ** power))
 
-  def __call__(
+  def __call__(  # noqa: D102
       self,
       weight: float,
       value: jnp.ndarray,
       new_value: jnp.ndarray,
       lse_mode: bool = True
   ) -> jnp.ndarray:
     if lse_mode:
       value = jnp.where(jnp.isfinite(value), value, 0.0)
       return (1.0 - weight) * value + weight * new_value
-    else:
-      value = jnp.where(value > 0.0, value, 1.0)
-      return value ** (1.0 - weight) * new_value ** weight
+    value = jnp.where(value > 0.0, value, 1.0)
+    return value ** (1.0 - weight) * new_value ** weight
```

### Comparing `ott-jax-0.4.0/src/ott/solvers/linear/continuous_barycenter.py` & `ott-jax-0.4.1/src/ott/solvers/linear/continuous_barycenter.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-# Copyright 2022 Apple.
+# Copyright OTT-JAX
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-#     http://www.apache.org/licenses/LICENSE-2.0
+#   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""A Jax version of the W barycenter algorithm (Cuturi Doucet 2014)."""
 import functools
 from typing import Any, NamedTuple, Optional, Tuple
 
 import jax
 import jax.numpy as jnp
 
+from ott import utils
 from ott.geometry import pointcloud
 from ott.math import fixed_point_loop
 from ott.math import utils as mu
 from ott.problems.linear import barycenter_problem, linear_problem
 from ott.solvers import was_solver
 
-__all__ = ["BarycenterState", "WassersteinBarycenter"]
+__all__ = ["FreeBarycenterState", "FreeWassersteinBarycenter"]
 
 
-class BarycenterState(NamedTuple):
+class FreeBarycenterState(NamedTuple):
   """Holds the state of the Wasserstein barycenter solver.
 
   Args:
     costs: Holds the sequence of regularized GW costs seen through the outer
       loop of the solver.
     linear_convergence: Holds the sequence of bool convergence flags of the
       inner Sinkhorn iterations.
@@ -43,22 +43,33 @@
 
   costs: Optional[jnp.ndarray] = None
   linear_convergence: Optional[jnp.ndarray] = None
   errors: Optional[jnp.ndarray] = None
   x: Optional[jnp.ndarray] = None
   a: Optional[jnp.ndarray] = None
 
-  def set(self, **kwargs: Any) -> 'BarycenterState':
+  def set(self, **kwargs: Any) -> "FreeBarycenterState":
     """Return a copy of self, possibly with overwrites."""
     return self._replace(**kwargs)
 
   def update(
-      self, iteration: int, bar_prob: barycenter_problem.BarycenterProblem,
+      self, iteration: int, bar_prob: barycenter_problem.FreeBarycenterProblem,
       linear_ot_solver: Any, store_errors: bool
-  ) -> 'BarycenterState':
+  ) -> "FreeBarycenterState":
+    """Update the state of the solver.
+
+    Args:
+      iteration: the current iteration of the outer loop.
+      bar_prob: the barycenter problem.
+      linear_ot_solver: the linear OT solver to use.
+      store_errors: whether to store the errors of the inner loop.
+
+    Returns:
+      The updated state.
+    """
     seg_y, seg_b = bar_prob.segmented_y_b
 
     @functools.partial(jax.vmap, in_axes=[None, None, 0, 0])
     def solve_linear_ot(
         a: Optional[jnp.ndarray], x: jnp.ndarray, b: jnp.ndarray, y: jnp.ndarray
     ):
       out = linear_ot_solver(
@@ -101,69 +112,69 @@
     # Approximation of barycenter as barycenter of barycenters per measure.
 
     barycenters_per_measure = mu.barycentric_projection(
         matrices, seg_y, bar_prob.cost_fn
     )
 
     x_new = jax.vmap(
-        bar_prob.cost_fn.barycenter, in_axes=[None, 1]
+        lambda w, y: bar_prob.cost_fn.barycenter(w, y)[0], in_axes=[None, 1]
     )(bar_prob.weights, barycenters_per_measure)
 
     return self.set(
         costs=updated_costs,
         linear_convergence=linear_convergence,
         errors=errors,
         x=x_new
     )
 
 
 @jax.tree_util.register_pytree_node_class
-class WassersteinBarycenter(was_solver.WassersteinSolver):
-  """A Continuous Wasserstein barycenter solver, built on generic template."""
+class FreeWassersteinBarycenter(was_solver.WassersteinSolver):
+  """Continuous Wasserstein barycenter solver :cite:`cuturi:14`."""
 
-  def __call__(
+  def __call__(  # noqa: D102
       self,
-      bar_prob: barycenter_problem.BarycenterProblem,
+      bar_prob: barycenter_problem.FreeBarycenterProblem,
       bar_size: int = 100,
       x_init: Optional[jnp.ndarray] = None,
-      rng: int = 0
-  ) -> BarycenterState:
+      rng: Optional[jax.random.PRNGKeyArray] = None,
+  ) -> FreeBarycenterState:
     # TODO(michalk8): no reason for iterations to be outside this class
-    run_fn = jax.jit(iterations, static_argnums=1) if self.jit else iterations
-    return run_fn(self, bar_size, bar_prob, x_init, rng)
+    rng = utils.default_prng_key(rng)
+    return iterations(self, bar_size, bar_prob, x_init, rng)
 
   def init_state(
       self,
-      bar_prob: barycenter_problem.BarycenterProblem,
+      bar_prob: barycenter_problem.FreeBarycenterProblem,
       bar_size: int,
       x_init: Optional[jnp.ndarray] = None,
-      # TODO(michalk8): change the API to pass the PRNG key directly
-      rng: int = 0,
-  ) -> BarycenterState:
+      rng: Optional[jax.random.PRNGKeyArray] = None,
+  ) -> FreeBarycenterState:
     """Initialize the state of the Wasserstein barycenter iterations.
 
     Args:
       bar_prob: The barycenter problem.
       bar_size: Size of the barycenter.
       x_init: Initial barycenter estimate of shape ``[bar_size, ndim]``.
         If `None`, ``bar_size`` points will be sampled from the input
         measures according to their weights
-        :attr:`~ott.problems.linear.barycenter_problem.BarycenterProblem.flattened_y`.
-      rng: Seed for :func:`jax.random.PRNGKey`.
+        :attr:`~ott.problems.linear.barycenter_problem.FreeBarycenterProblem.flattened_y`.
+      rng: Random key for seeding.
 
     Returns:
       The initial barycenter state.
     """
     if x_init is not None:
       assert bar_size == x_init.shape[0]
       x = x_init
     else:
       # sample randomly points in the support of the y measures
+      rng = utils.default_prng_key(rng)
       indices_subset = jax.random.choice(
-          jax.random.PRNGKey(rng),
+          rng,
           a=bar_prob.flattened_y.shape[0],
           shape=(bar_size,),
           replace=False,
           p=bar_prob.flattened_b
       )
       x = bar_prob.flattened_y[indices_subset, :]
 
@@ -173,43 +184,46 @@
     if self.store_inner_errors:
       errors = -jnp.ones((
           num_iter, bar_prob.num_measures,
           self.linear_ot_solver.outer_iterations
       ))
     else:
       errors = None
-    return BarycenterState(
+    return FreeBarycenterState(
         -jnp.ones((num_iter,)), -jnp.ones((num_iter,)), errors, x, a
     )
 
-  def output_from_state(self, state: BarycenterState) -> BarycenterState:
+  def output_from_state(  # noqa: D102
+      self, state: FreeBarycenterState
+  ) -> FreeBarycenterState:
     # TODO(michalk8): create an output variable to match rest of the framework
     return state
 
 
 def iterations(
-    solver: WassersteinBarycenter, bar_size: int,
-    bar_prob: barycenter_problem.BarycenterProblem, x_init: jnp.ndarray,
-    rng: int
-) -> BarycenterState:
+    solver: FreeWassersteinBarycenter, bar_size: int,
+    bar_prob: barycenter_problem.FreeBarycenterProblem, x_init: jnp.ndarray,
+    rng: jax.random.PRNGKeyArray
+) -> FreeBarycenterState:
   """Jittable Wasserstein barycenter outer loop."""
 
   def cond_fn(
-      iteration: int, constants: Tuple[WassersteinBarycenter,
-                                       barycenter_problem.BarycenterProblem],
-      state: BarycenterState
+      iteration: int,
+      constants: Tuple[FreeWassersteinBarycenter,
+                       barycenter_problem.FreeBarycenterProblem],
+      state: FreeBarycenterState
   ) -> bool:
     solver, _ = constants
     return solver._continue(state, iteration)
 
   def body_fn(
-      iteration, constants: Tuple[WassersteinBarycenter,
-                                  barycenter_problem.BarycenterProblem],
-      state: BarycenterState, compute_error: bool
-  ) -> BarycenterState:
+      iteration, constants: Tuple[FreeWassersteinBarycenter,
+                                  barycenter_problem.FreeBarycenterProblem],
+      state: FreeBarycenterState, compute_error: bool
+  ) -> FreeBarycenterState:
     del compute_error  # Always assumed True
     solver, bar_prob = constants
     return state.update(
         iteration, bar_prob, solver.linear_ot_solver, solver.store_inner_errors
     )
 
   state = fixed_point_loop.fixpoint_iter(
```

### Comparing `ott-jax-0.4.0/src/ott/solvers/linear/implicit_differentiation.py` & `ott-jax-0.4.1/src/ott/solvers/linear/implicit_differentiation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,65 +1,88 @@
-# Copyright 2022 Google LLC.
+# Copyright OTT-JAX
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-#     http://www.apache.org/licenses/LICENSE-2.0
+#   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Functions entering the implicit differentiation of Sinkhorn."""
-
-from typing import TYPE_CHECKING, Callable, Optional, Tuple
+import dataclasses
+from typing import TYPE_CHECKING, Any, Callable, Dict, Optional, Tuple
 
 import jax
 import jax.numpy as jnp
 
 from ott import utils
 from ott.math import unbalanced_functions as uf
 
 if TYPE_CHECKING:
   from ott.problems.linear import linear_problem
 
+LinOp_t = Callable[[jnp.ndarray], jnp.ndarray]
+Solver_t = Callable[[LinOp_t, jnp.ndarray, Optional[LinOp_t], bool],
+                    jnp.ndarray]
+
 __all__ = ["ImplicitDiff"]
 
 
 @utils.register_pytree_node
 class ImplicitDiff:
   """Implicit differentiation of Sinkhorn algorithm.
 
   Args:
-    solver_fun: Callable, should return (solution, ...)
-    ridge_kernel: promotes zero-sum solutions. only used if tau_a = tau_b = 1.0
-    ridge_identity: handles rank deficient transport matrices (this happens
-      typically when rows/cols in cost/kernel matrices are collinear, or,
-      equivalently when two points from either measure are close).
+    solver: Callable to compute the solution to a linear problem. The callable
+      expects a linear function, a vector, optionally another linear function
+      that implements the transpose of that function, and a boolean flag to
+      specify symmetry. This solver is by default one of :class:`lineax.CG` or
+      :class:`lineax.NormalCG` solvers, if the package can be imported, as
+      described in :func:`~ott.solvers.linear.lineax_implicit.solve_lineax`.
+      The :mod:`jax` alternative is described in
+      :func:`~ott.solvers.linear.implicit_differentiation.solve_jax_cg`.
+      Note that `lineax` solvers handle better poorly conditioned problems,
+      which arise typically when differentiating the solutions of balanced OT
+      problems (when ``tau_a==tau_b==1.0``). Relying on
+      :func:`~ott.solvers.linear.implicit_differentiation.solve_jax_cg`
+      for such cases might require hand-tuning ridge parameters,
+      in particular ``ridge_kernel`` and ``ridge_identity`` as described in its
+      doc. These parameters can be passed using ``solver_kwargs`` below.
+    solver_kwargs: keyword arguments passed on to the solver.
     symmetric: flag used to figure out whether the linear system solved in the
-      implicit function theorem is symmetric or not. This happens when either
-      ``a == b`` or the precondition_fun is the identity. False by default, and,
-      at the moment, needs to be set manually by the user in the more favorable
-      case where the system is guaranteed to be symmetric.
-    precondition_fun: TODO(marcocuturi)
+      implicit function theorem is symmetric or not. This happens when
+      ``tau_a==tau_b``, and when ``a == b``, or the precondition_fun
+      is the identity. The flag is False by default, and is also tested against
+      ``tau_a==tau_b``. It needs to be set manually by the user in the more
+      favorable case where the system is guaranteed to be symmetric.
+    precondition_fun: Function used to precondition, on both sides, the linear
+      system derived from first-order conditions of the regularized OT problem.
+      That linear system typically involves an equality between marginals (or
+      simple transform of these marginals when the problem is unbalanced) and
+      another function of the potentials. When that function is specified, that
+      function is applied on both sides of the equality, before being further
+      differentiated to provide the Jacobians needed for implicit function
+      theorem differentiation.
   """
 
-  solver_fun: Callable[[jnp.ndarray, jnp.ndarray],
-                       Tuple[jnp.ndarray, ...]] = jax.scipy.sparse.linalg.cg
-  ridge_kernel: float = 0.0
-  ridge_identity: float = 0.0
+  solver: Optional[Solver_t] = None
+  solver_kwargs: Optional[Dict[str, Any]] = None
   symmetric: bool = False
   precondition_fun: Optional[Callable[[jnp.ndarray], jnp.ndarray]] = None
 
   def solve(
-      self, gr: Tuple[jnp.ndarray,
-                      jnp.ndarray], ot_prob: "linear_problem.LinearProblem",
-      f: jnp.ndarray, g: jnp.ndarray, lse_mode: bool
+      self,
+      gr: Tuple[jnp.ndarray, jnp.ndarray],
+      ot_prob: "linear_problem.LinearProblem",
+      f: jnp.ndarray,
+      g: jnp.ndarray,
+      lse_mode: bool,
   ) -> jnp.ndarray:
     r"""Apply minus inverse of [hessian ``reg_ot_cost`` w.r.t. ``f``, ``g``].
 
     This function is used to carry out implicit differentiation of ``sinkhorn``
     outputs, notably optimal potentials ``f`` and ``g``. That differentiation
     requires solving a linear system, using (and inverting) the Jacobian of
     (preconditioned) first-order conditions w.r.t. the reg-OT problem.
@@ -107,62 +130,53 @@
     depending on ``lse_mode``)
 
     The Jacobian's diagonal + off-diagonal blocks structure allows to exploit
     Schur complements. Depending on the sizes involved, it is better to
     instantiate the Schur complement of the first or of the second diagonal
     block.
 
-    In either case, the Schur complement is rank deficient, with a 0 eigenvalue
-    for the vector of ones in the balanced case, which is why we add a ridge on
-    that subspace to enforce solutions have zero sum.
-
-    The Schur complement can also be rank deficient if two lines or columns of T
-    are collinear. This will typically happen it two rows or columns of the cost
-    or kernel matrix are numerically close. To avoid this, we add a more global
-    ``ridge_identity * z`` regularizer to achieve better conditioning.
-
-    These linear systems are solved using the user defined ``solver_fun``,
-    which is set by default to ``cg``. When the system is symmetric (as detected
-    by the corresponding flag ``symmetric``), ``cg`` is applied directly. When
-    it is not, normal equations are used (i.e. the Schur complement is
-    multiplied by its transpose before solving the system).
+    These linear systems are solved using the user-defined ``solver``, using
+    by default :mod:`lineax` solvers when available, or falling back on
+    :mod:`jax` when not.
 
     Args:
       gr: 2-tuple, (vector of size ``n``, vector of size ``m``).
       ot_prob: the instantiation of the regularized transport problem.
       f: potential, w.r.t marginal a.
       g: potential, w.r.t marginal b.
       lse_mode: bool, log-sum-exp mode if True, kernel else.
 
     Returns:
       A tuple of two vectors, of the same size as ``gr``.
     """
+    solver = _get_solver() if self.solver is None else self.solver
+    solver_kwargs = {} if self.solver_kwargs is None else self.solver_kwargs
     geom = ot_prob.geom
     marginal_a, marginal_b, app_transport = (
         ot_prob.get_transport_functions(lse_mode)
     )
-
-    # elementwise vmap apply of derivative of precondition_fun. No vmapping
-    # can be problematic here.
     if self.precondition_fun is None:
       precond_fun = lambda x: geom.epsilon * jnp.log(x)
+      symmetric = False
     else:
       precond_fun = self.precondition_fun
+      symmetric = self.symmetric
+
     derivative = jax.vmap(jax.grad(precond_fun))
 
     n, m = geom.shape
     # pylint: disable=g-long-lambda
     vjp_fg = lambda z: app_transport(
         f, g, z * derivative(marginal_b(f, g)), axis=1
     ) / geom.epsilon
     vjp_gf = lambda z: app_transport(
         f, g, z * derivative(marginal_a(f, g)), axis=0
     ) / geom.epsilon
 
-    if not self.symmetric:
+    if not symmetric:
       vjp_fgt = lambda z: app_transport(
           f, g, z, axis=0
       ) * derivative(marginal_b(f, g)) / geom.epsilon
       vjp_gft = lambda z: app_transport(
           f, g, z, axis=1
       ) * derivative(marginal_a(f, g)) / geom.epsilon
 
@@ -174,60 +188,40 @@
     )
     diag_hess_b = (
         marginal_b(f, g) * derivative(marginal_b(f, g)) / geom.epsilon +
         uf.diag_jacobian_of_marginal_fit(
             ot_prob.b, g, ot_prob.tau_b, geom.epsilon, derivative
         )
     )
-
     n, m = geom.shape
-    # Remove ridge on kernel space if problem is balanced.
-    ridge_kernel = jnp.where(ot_prob.is_balanced, self.ridge_kernel, 0.0)
-
+    # TODO(cuturi) consider materializing linear operator schur if size allows.
     # Forks on using Schur complement of either A or D, depending on size.
     if n > m:  #  if n is bigger, run m x m linear system.
       inv_vjp_ff = lambda z: z / diag_hess_a
       vjp_gg = lambda z: z * diag_hess_b
-      schur_ = lambda z: vjp_gg(z) - vjp_gf(inv_vjp_ff(vjp_fg(z)))
-      res = gr[1] - vjp_gf(inv_vjp_ff(gr[0]))
-
-      if self.symmetric:
-        schur = lambda z: (
-            schur_(z) + ridge_kernel * jnp.sum(z) + self.ridge_identity * z
-        )
-      else:
+      schur = lambda z: vjp_gg(z) - vjp_gf(inv_vjp_ff(vjp_fg(z)))
+      if not symmetric:
         schur_t = lambda z: vjp_gg(z) - vjp_fgt(inv_vjp_ff(vjp_gft(z)))
-        res = schur_t(res)
-        schur = lambda z: (
-            schur_t(schur_(z)) + ridge_kernel * jnp.sum(z) + self.ridge_identity
-            * z
-        )
-
-      sch = self.solver_fun(schur, res)[0]
+      else:
+        schur_t = None
+      res = gr[1] - vjp_gf(inv_vjp_ff(gr[0]))
+      sch = solver(schur, res, schur_t, symmetric, **solver_kwargs)
       vjp_gr_f = inv_vjp_ff(gr[0] - vjp_fg(sch))
       vjp_gr_g = sch
     else:
       vjp_ff = lambda z: z * diag_hess_a
       inv_vjp_gg = lambda z: z / diag_hess_b
-      schur_ = lambda z: vjp_ff(z) - vjp_fg(inv_vjp_gg(vjp_gf(z)))
-      res = gr[0] - vjp_fg(inv_vjp_gg(gr[1]))
+      schur = lambda z: vjp_ff(z) - vjp_fg(inv_vjp_gg(vjp_gf(z)))
 
-      if self.symmetric:
-        schur = lambda z: (
-            schur_(z) + ridge_kernel * jnp.sum(z) + self.ridge_identity * z
-        )
-      else:
+      if not symmetric:
         schur_t = lambda z: vjp_ff(z) - vjp_gft(inv_vjp_gg(vjp_fgt(z)))
-        res = schur_t(res)
-        schur = lambda z: (
-            schur_t(schur_(z)) + ridge_kernel * jnp.sum(z) + self.ridge_identity
-            * z
-        )
-
-      sch = self.solver_fun(schur, res)[0]
+      else:
+        schur_t = None
+      res = gr[0] - vjp_fg(inv_vjp_gg(gr[1]))
+      sch = solver(schur, res, schur_t, symmetric, **solver_kwargs)
       vjp_gr_g = inv_vjp_gg(gr[1] - vjp_gf(sch))
       vjp_gr_f = sch
 
     return jnp.concatenate((-vjp_gr_f, -vjp_gr_g))
 
   def first_order_conditions(
       self, prob, f: jnp.ndarray, g: jnp.ndarray, lse_mode: bool
@@ -271,18 +265,60 @@
     )
     return jnp.concatenate((result_a, result_b))
 
   def gradient(
       self, prob: "linear_problem.LinearProblem", f: jnp.ndarray,
       g: jnp.ndarray, lse_mode: bool, gr: Tuple[jnp.ndarray, jnp.ndarray]
   ) -> "linear_problem.LinearProblem":
-    """Apply vjp to recover gradient in reverse mode differentiation."""
+    """Apply VJP to recover gradient in reverse mode differentiation."""
     # Applies first part of vjp to gr: inverse part of implicit function theorem
     vjp_gr = self.solve(gr, prob, f, g, lse_mode)
 
     # Instantiates vjp of first order conditions of the objective, as a
     # function of geom, a and b parameters (against which we differentiate)
     foc_prob = lambda prob: self.first_order_conditions(prob, f, g, lse_mode)
 
     # Carries pullback onto original inputs, here geom, a and b.
     _, pull_prob = jax.vjp(foc_prob, prob)
     return pull_prob(vjp_gr)
+
+  def replace(self, **kwargs: Any) -> "ImplicitDiff":  # noqa: D102
+    return dataclasses.replace(self, **kwargs)
+
+
+def solve_jax_cg(
+    lin: LinOp_t,
+    b: jnp.ndarray,
+    lin_t: Optional[LinOp_t] = None,
+    symmetric: bool = False,
+    ridge_identity: float = 0.0,
+    ridge_kernel: float = 0.0,
+    **kwargs: Any
+) -> jnp.ndarray:
+  """Wrapper around JAX native linear solvers.
+
+  Args:
+    lin: Linear operator
+    b: vector. Returned `x` is such that `lin(x)=b`
+    lin_t: Linear operator, corresponding to transpose of `lin`.
+    symmetric: whether `lin` is symmetric.
+    ridge_kernel: promotes zero-sum solutions. Only use if `tau_a = tau_b = 1.0`
+    ridge_identity: handles rank deficient transport matrices (this happens
+      typically when rows/cols in cost/kernel matrices are collinear, or,
+      equivalently when two points from either measure are close).
+    kwargs: arguments passed to :func:`~jax.scipy.sparse.linalg.cg`
+  """
+  op = lin if symmetric else lambda x: lin_t(lin(x))
+  if ridge_kernel > 0.0 or ridge_identity > 0.0:
+    lin_reg = lambda x: op(x) + ridge_kernel * jnp.sum(x) + ridge_identity * x
+  else:
+    lin_reg = op
+  return jax.scipy.sparse.linalg.cg(lin_reg, b, **kwargs)[0]
+
+
+def _get_solver() -> Solver_t:
+  """Get lineax solver when possible, default to jax.scipy else."""
+  try:
+    from ott.solvers.linear import lineax_implicit
+    return lineax_implicit.solve_lineax
+  except ImportError:
+    return solve_jax_cg
```

### Comparing `ott-jax-0.4.0/src/ott/solvers/linear/sinkhorn.py` & `ott-jax-0.4.1/src/ott/solvers/linear/sinkhorn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,62 +1,67 @@
-# Copyright 2022 Google LLC.
+# Copyright OTT-JAX
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-#     http://www.apache.org/licenses/LICENSE-2.0
+#   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""A Jax implementation of the Sinkhorn algorithm."""
 from typing import (
     TYPE_CHECKING,
     Any,
+    Callable,
     Literal,
     Mapping,
     NamedTuple,
     Optional,
     Sequence,
     Tuple,
     Union,
 )
 
 import jax
 import jax.numpy as jnp
 import numpy as np
+from jax.experimental import host_callback
 
+from ott import utils
 from ott.geometry import geometry
 from ott.initializers.linear import initializers as init_lib
 from ott.math import fixed_point_loop
 from ott.math import unbalanced_functions as uf
 from ott.math import utils as mu
 from ott.problems.linear import linear_problem, potentials
 from ott.solvers.linear import acceleration
 from ott.solvers.linear import implicit_differentiation as implicit_lib
 
 if TYPE_CHECKING:
   from ott.solvers.linear.sinkhorn_lr import LRSinkhorn, LRSinkhornOutput
 
 __all__ = ["Sinkhorn", "SinkhornOutput", "solve"]
 
+ProgressCallbackFn_t = Callable[
+    [Tuple[np.ndarray, np.ndarray, np.ndarray, "SinkhornState"]], None]
+
 
 class SinkhornState(NamedTuple):
   """Holds the state variables used to solve OT with Sinkhorn."""
 
   errors: Optional[jnp.ndarray] = None
   fu: Optional[jnp.ndarray] = None
   gv: Optional[jnp.ndarray] = None
   old_fus: Optional[jnp.ndarray] = None
   old_mapped_fus: Optional[jnp.ndarray] = None
 
-  def set(self, **kwargs: Any) -> 'SinkhornState':
+  def set(self, **kwargs: Any) -> "SinkhornState":
     """Return a copy of self, with potential overwrites."""
     return self._replace(**kwargs)
 
   def solution_error(
       self,
       ot_prob: linear_problem.LinearProblem,
       norm_error: Sequence[int],
@@ -75,30 +80,30 @@
         gv,
         ot_prob,
         norm_error=norm_error,
         lse_mode=lse_mode,
         parallel_dual_updates=parallel_dual_updates
     )
 
-  def ent_reg_cost(
+  def ent_reg_cost(  # noqa: D102
       self, ot_prob: linear_problem.LinearProblem, lse_mode: bool
   ) -> float:
     return ent_reg_cost(self.fu, self.gv, ot_prob, lse_mode)
 
   def recenter(
       self,
       f: jnp.ndarray,
       g: jnp.ndarray,
       ot_prob: linear_problem.LinearProblem,
   ) -> Tuple[jnp.ndarray, jnp.ndarray]:
     """Re-center dual potentials.
 
     If the ``ot_prob`` is balanced, the ``f`` potential is zero-centered.
-    Otherwise, use prop. 2 of :cite:`sejourne:22` re-center the potentials only
-    iff ``tau_a < 1`` and ``tau_b < 1``.
+    Otherwise, use prop. 2 of :cite:`sejourne:22` re-center the potentials iff
+    ``tau_a < 1`` and ``tau_b < 1``.
 
     Args:
       f: The first dual potential.
       g: The second dual potential.
       ot_prob: Linear OT problem.
 
     Returns:
@@ -213,18 +218,17 @@
     Array of floats, quantifying difference between target / marginal.
   """
   if lse_mode:
     marginal = geom.marginal_from_potentials(f_u, g_v, axis=axis)
   else:
     marginal = geom.marginal_from_scalings(f_u, g_v, axis=axis)
   norm_error = jnp.asarray(norm_error)
-  error = jnp.sum(
+  return jnp.sum(
       jnp.abs(marginal - target) ** norm_error[:, jnp.newaxis], axis=1
   ) ** (1.0 / norm_error)
-  return error
 
 
 def ent_reg_cost(
     f: jnp.ndarray, g: jnp.ndarray, ot_prob: linear_problem.LinearProblem,
     lse_mode: bool
 ) -> float:
   r"""Compute objective of Sinkhorn for OT problem given dual solutions.
@@ -283,36 +287,36 @@
 
   f: Optional[jnp.ndarray] = None
   g: Optional[jnp.ndarray] = None
   errors: Optional[jnp.ndarray] = None
   reg_ot_cost: Optional[float] = None
   ot_prob: Optional[linear_problem.LinearProblem] = None
 
-  def set(self, **kwargs: Any) -> 'SinkhornOutput':
+  def set(self, **kwargs: Any) -> "SinkhornOutput":
     """Return a copy of self, with potential overwrites."""
     return self._replace(**kwargs)
 
-  def set_cost(
+  def set_cost(  # noqa: D102
       self, ot_prob: linear_problem.LinearProblem, lse_mode: bool,
       use_danskin: bool
-  ) -> 'SinkhornOutput':
+  ) -> "SinkhornOutput":
     f = jax.lax.stop_gradient(self.f) if use_danskin else self.f
     g = jax.lax.stop_gradient(self.g) if use_danskin else self.g
     return self.set(reg_ot_cost=ent_reg_cost(f, g, ot_prob, lse_mode))
 
   @property
   def dual_cost(self) -> jnp.ndarray:
     """Return transport cost in dual form of current solution."""
     a, b = self.ot_prob.a, self.ot_prob.b
     dual_cost = jnp.sum(jnp.where(a > 0.0, a * self.f, 0))
     dual_cost += jnp.sum(jnp.where(b > 0.0, b * self.g, 0))
     return dual_cost
 
   @property
-  def primal_cost(self) -> jnp.ndarray:
+  def primal_cost(self) -> float:
     """Return transport cost of current solution at geometry."""
     return self.transport_cost_at_geom(other_geom=self.geom)
 
   def transport_cost_at_geom(
       self, other_geom: geometry.Geometry
   ) -> jnp.ndarray:
     r"""Return bare transport cost of current solution at any geometry.
@@ -333,50 +337,50 @@
     # TODO(michalk8): handle SqEucl point cloud is not converted to LRCGeom
     if other_geom.can_LRC:
       geom = other_geom.to_LRCGeometry()
       return jnp.sum(self.apply(geom.cost_1.T) * geom.cost_2.T)
     return jnp.sum(self.matrix * other_geom.cost_matrix)
 
   @property
-  def linear(self) -> bool:
+  def linear(self) -> bool:  # noqa: D102
     return isinstance(self.ot_prob, linear_problem.LinearProblem)
 
   @property
-  def geom(self) -> geometry.Geometry:
+  def geom(self) -> geometry.Geometry:  # noqa: D102
     return self.ot_prob.geom
 
   @property
-  def a(self) -> jnp.ndarray:
+  def a(self) -> jnp.ndarray:  # noqa: D102
     return self.ot_prob.a
 
   @property
-  def b(self) -> jnp.ndarray:
+  def b(self) -> jnp.ndarray:  # noqa: D102
     return self.ot_prob.b
 
   @property
-  def linear_output(self) -> bool:
+  def linear_output(self) -> bool:  # noqa: D102
     return True
 
   @property
-  def converged(self) -> bool:
+  def converged(self) -> bool:  # noqa: D102
     if self.errors is None:
       return False
     return jnp.logical_and(
         jnp.any(self.errors == -1), jnp.all(jnp.isfinite(self.errors))
     )
 
   # TODO(michalk8): this should be always present
   @property
-  def n_iters(self) -> int:
+  def n_iters(self) -> int:  # noqa: D102
     if self.errors is None:
       return -1
     return jnp.sum(self.errors > -1)
 
   @property
-  def scalings(self) -> Tuple[jnp.ndarray, jnp.ndarray]:
+  def scalings(self) -> Tuple[jnp.ndarray, jnp.ndarray]:  # noqa: D102
     u = self.ot_prob.geom.scaling_from_potential(self.f)
     v = self.ot_prob.geom.scaling_from_potential(self.g)
     return u, v
 
   @property
   def matrix(self) -> jnp.ndarray:
     """Transport matrix if it can be instantiated."""
@@ -392,15 +396,15 @@
 
   def apply(self, inputs: jnp.ndarray, axis: int = 0) -> jnp.ndarray:
     """Apply the transport to a ndarray; axis=1 for its transpose."""
     return self.ot_prob.geom.apply_transport_from_potentials(
         self.f, self.g, inputs, axis=axis
     )
 
-  def marginal(self, axis: int) -> jnp.ndarray:
+  def marginal(self, axis: int) -> jnp.ndarray:  # noqa: D102
     return self.ot_prob.geom.marginal_from_potentials(self.f, self.g, axis=axis)
 
   def cost_at_geom(self, other_geom: geometry.Geometry) -> float:
     """Return reg-OT cost for matrix, evaluated at other cost matrix."""
     return (
         jnp.sum(self.matrix * other_geom.cost_matrix) -
         self.geom.epsilon * jnp.sum(jax.scipy.special.entr(self.matrix))
@@ -414,15 +418,15 @@
 @jax.tree_util.register_pytree_node_class
 class Sinkhorn:
   r"""Sinkhorn solver.
 
   The Sinkhorn algorithm is a fixed point iteration that solves a regularized
   optimal transport (reg-OT) problem between two measures.
   The optimization variables are a pair of vectors (called potentials, or
-  scalings when parameterized as exponentials of the former). Calling this
+  scalings when parameterized as exponential of the former). Calling this
   function returns therefore a pair of optimal vectors. In addition to these,
   it also returns the objective value achieved by these optimal vectors;
   a vector of size ``max_iterations/inner_iterations`` that records the vector
   of values recorded to monitor convergence, throughout the execution of the
   algorithm (padded with `-1` if convergence happens before), as well as a
   boolean to signify whether the algorithm has converged within the number of
   iterations specified by the user.
@@ -432,15 +436,15 @@
   only seen through a triplet (``geom``, ``a``, ``b``), where ``geom`` is a
   ``Geometry`` object, and ``a`` and ``b`` are weight vectors of respective
   sizes ``n`` and ``m``. Starting from two initial values for those potentials
   or scalings (both can be defined by the user by passing value in
   ``init_dual_a`` or ``init_dual_b``), the Sinkhorn algorithm will use
   elementary operations that are carried out by the ``geom`` object.
 
-  Some maths:
+  Math:
     Given a geometry ``geom``, which provides a cost matrix :math:`C` with its
     regularization parameter :math:`\varepsilon`, (or a kernel matrix :math:`K`)
     the reg-OT problem consists in finding two vectors `f`, `g` of size ``n``,
     ``m`` that maximize the following criterion.
 
     .. math::
 
@@ -496,15 +500,15 @@
     To handle the case :math:`\rho_a, \rho_b \rightarrow \infty`, the
     ``sinkhorn`` function uses parameters :math:`tau\_a := \rho_a /
     (\varepsilon + \rho_a)` and :math:`tau\_b := \rho_b / (\varepsilon +
     \rho_b)` instead. Setting either of these parameters to 1 corresponds to
     setting the corresponding :math:`\rho_a, \rho_b` to :math:`\infty`.
 
     The Sinkhorn algorithm solves the reg-OT problem by seeking optimal `f`, `g`
-    potentials (or alternatively their parametrization as positive scalings
+    potentials (or alternatively their parameterization as positive scalings
     `u`, `v`), rather than solving the primal problem in :math:`P`.
     This is mostly for efficiency (potentials and scalings have a ``n + m``
     memory footprint, rather than ``n m`` required to store `P`). This is also
     because both problems are, in fact, equivalent, since the optimal transport
     math:`P^*` can be recovered from optimal potentials :math:`f^*`, :math:`g^*`
     or scalings :math:`u^*`, :math:`v^*`, using the geometry's cost or kernel
     matrix respectively:
@@ -570,16 +574,16 @@
     using some form of averaging (e.g. ``momentum=0.5``). Without this, and on
     its own ``parallel_dual_updates`` won't work.
 
   Differentiation:
     The optimal solutions ``f`` and ``g`` and the optimal objective
     (``reg_ot_cost``) outputted by the Sinkhorn algorithm can be differentiated
     w.r.t. relevant inputs ``geom``, ``a`` and ``b`` using, by default, implicit
-    differentiation of the optimality conditions (``implicit_differentiation``
-    set to ``True``). This choice has two consequences.
+    differentiation of the optimality conditions (``implicit_diff``
+    not equal to ``None``). This choice has two consequences.
 
     - The termination criterion used to stop Sinkhorn (cancellation of
       gradient of objective w.r.t. ``f_u`` and ``g_v``) is used to differentiate
       ``f`` and ``g``, given a change in the inputs. These changes are computed
       by solving a linear system. The arguments starting with
       ``implicit_solver_*`` allow to define the linear solver that is used, and
       to control for two types or regularization (we have observed that,
@@ -603,15 +607,15 @@
 
     An alternative yet more costly way to differentiate the outputs of the
     Sinkhorn iterations is to use unrolling, i.e. reverse mode differentiation
     of the Sinkhorn loop. This is possible because Sinkhorn iterations are
     wrapped in a custom fixed point iteration loop, defined in
     ``fixed_point_loop``, rather than a standard while loop. This is to ensure
     the end result of this fixed point loop can also be differentiated, if
-    needed, using standard JAX operations. To ensure backprop differentiability,
+    needed, using standard JAX operations. To ensure differentiability,
     the ``fixed_point_loop.fixpoint_iter_backprop`` loop does checkpointing of
     state variables (here ``f_u`` and ``g_v``) every ``inner_iterations``, and
     backpropagates automatically, block by block, through blocks of
     ``inner_iterations`` at a time.
 
   Note:
     * The Sinkhorn algorithm may not converge within the maximum number of
@@ -655,15 +659,15 @@
       successive solutions in the unbalanced case.
     norm_error: power used to define p-norm of error for marginal/target.
     inner_iterations: the Sinkhorn error is not recomputed at each
       iteration but every inner_num_iter instead.
     min_iterations: the minimum number of Sinkhorn iterations carried
       out before the error is computed and monitored.
     max_iterations: the maximum number of Sinkhorn iterations. If
-      ``max_iterations`` is equal to ``min_iterations``, sinkhorn iterations are
+      ``max_iterations`` is equal to ``min_iterations``, Sinkhorn iterations are
       run by default using a :func:`jax.lax.scan` loop rather than a custom,
       unroll-able :func:`jax.lax.while_loop` that monitors convergence.
       In that case the error is not monitored and the ``converged``
       flag will return ``False`` as a consequence.
     momentum: Momentum instance.
     anderson: AndersonAcceleration instance.
     implicit_diff: instance used to solve implicit differentiation. Unrolls
@@ -676,16 +680,19 @@
       to achieve faster convergence. Only used when ``lse_mode = True`` and
       ``tau_a < 1`` and ``tau_b < 1``.
     use_danskin: when ``True``, it is assumed the entropy regularized cost
       is evaluated using optimal potentials that are frozen, i.e. whose
       gradients have been stopped. This is useful when carrying out first order
       differentiation, and is only valid (as with ``implicit_differentiation``)
       when the algorithm has converged with a low tolerance.
-    jit: Whether to jit the iteration loop.
     initializer: how to compute the initial potentials/scalings.
+    progress_fn: callback function which gets called during the Sinkhorn
+      iterations, so the user can display the error at each iteration,
+      e.g., using a progress bar. See :func:`~ott.utils.default_progress_fn`
+      for a basic implementation.
     kwargs_init: keyword arguments when creating the initializer.
   """
 
   def __init__(
       self,
       lse_mode: bool = True,
       threshold: float = 1e-3,
@@ -694,30 +701,29 @@
       min_iterations: int = 0,
       max_iterations: int = 2000,
       momentum: Optional[acceleration.Momentum] = None,
       anderson: Optional[acceleration.AndersonAcceleration] = None,
       parallel_dual_updates: bool = False,
       recenter_potentials: bool = False,
       use_danskin: Optional[bool] = None,
-      jit: bool = True,
       implicit_diff: Optional[implicit_lib.ImplicitDiff
-                             ] = implicit_lib.ImplicitDiff(),  # noqa: E124
-      initializer: Union[Literal["default", "gaussian", "sorting"],
+                             ] = implicit_lib.ImplicitDiff(),  # noqa: B008
+      initializer: Union[Literal["default", "gaussian", "sorting", "subsample"],
                          init_lib.SinkhornInitializer] = "default",
+      progress_fn: Optional[ProgressCallbackFn_t] = None,
       kwargs_init: Optional[Mapping[str, Any]] = None,
   ):
     self.lse_mode = lse_mode
     self.threshold = threshold
     self.inner_iterations = inner_iterations
     self.min_iterations = min_iterations
     self.max_iterations = max_iterations
     self._norm_error = norm_error
     self.anderson = anderson
     self.implicit_diff = implicit_diff
-    self.jit = jit
 
     if momentum is not None:
       self.momentum = acceleration.Momentum(
           momentum.start, momentum.error_threshold, momentum.value,
           self.inner_iterations
       )
     else:
@@ -729,14 +735,15 @@
       else:
         # no momentum
         self.momentum = acceleration.Momentum()
 
     self.parallel_dual_updates = parallel_dual_updates
     self.recenter_potentials = recenter_potentials
     self.initializer = initializer
+    self.progress_fn = progress_fn
     self.kwargs_init = {} if kwargs_init is None else kwargs_init
 
     # Force implicit_differentiation to True when using Anderson acceleration,
     # Reset all momentum parameters to default (i.e. no momentum)
     if anderson:
       self.implicit_diff = (
           implicit_lib.ImplicitDiff()
@@ -751,31 +758,33 @@
     self.use_danskin = ((self.implicit_diff is not None)
                         if use_danskin is None else use_danskin)
 
   def __call__(
       self,
       ot_prob: linear_problem.LinearProblem,
       init: Tuple[Optional[jnp.ndarray], Optional[jnp.ndarray]] = (None, None),
+      rng: Optional[jax.random.PRNGKeyArray] = None,
   ) -> SinkhornOutput:
     """Run Sinkhorn algorithm.
 
     Args:
       ot_prob: Linear OT problem.
       init: Initial dual potentials/scalings f_u and g_v, respectively.
         Any `None` values will be initialized using the initializer.
+      rng: Random number generator key for stochastic initialization.
 
     Returns:
       The Sinkhorn output.
     """
+    rng = utils.default_prng_key(rng)
     initializer = self.create_initializer()
     init_dual_a, init_dual_b = initializer(
-        ot_prob, *init, lse_mode=self.lse_mode
+        ot_prob, *init, lse_mode=self.lse_mode, rng=rng
     )
-    run_fn = jax.jit(run) if self.jit else run
-    return run_fn(ot_prob, self, (init_dual_a, init_dual_b))
+    return run(ot_prob, self, (init_dual_a, init_dual_b))
 
   def lse_step(
       self, ot_prob: linear_problem.LinearProblem, state: SinkhornState,
       iteration: int
   ) -> SinkhornState:
     """Sinkhorn LSE update."""
 
@@ -849,15 +858,15 @@
     fu = self.momentum(w, state.fu, new_fu, self.lse_mode)
     return state.set(fu=fu, gv=gv)
 
   def one_iteration(
       self, ot_prob: linear_problem.LinearProblem, state: SinkhornState,
       iteration: int, compute_error: bool
   ) -> SinkhornState:
-    """Carries out sinkhorn iteration.
+    """Carries out one Sinkhorn iteration.
 
     Depending on lse_mode, these iterations can be either in:
 
       - log-space for numerical stability.
       - scaling space, using standard kernel-vector multiply operations.
 
     Args:
@@ -894,15 +903,22 @@
             recenter=self.recenter_potentials
         )[0],
         lambda *_: jnp.inf,
         state,
         ot_prob,
     )
     errors = state.errors.at[iteration // self.inner_iterations, :].set(err)
-    return state.set(errors=errors)
+    state = state.set(errors=errors)
+
+    if self.progress_fn is not None:
+      host_callback.id_tap(
+          self.progress_fn,
+          (iteration, self.inner_iterations, self.max_iterations, state)
+      )
+    return state
 
   def _converged(self, state: SinkhornState, iteration: int) -> bool:
     err = state.errors[iteration // self.inner_iterations - 1, 0]
     return jnp.logical_and(iteration > 0, err < self.threshold)
 
   def _diverged(self, state: SinkhornState, iteration: int) -> bool:
     err = state.errors[iteration // self.inner_iterations - 1, 0]
@@ -981,35 +997,37 @@
     # In that case, we add this exponent to the list of errors to compute,
     # notably if that was not the error requested by the user.
     if self.momentum and self.momentum.start > 0 and self._norm_error != 1:
       return self._norm_error, 1
     return self._norm_error,
 
   # TODO(michalk8): in the future, enforce this (+ in GW) via abstract method
-  def create_initializer(self) -> init_lib.SinkhornInitializer:
+  def create_initializer(self) -> init_lib.SinkhornInitializer:  # noqa: D102
     if isinstance(self.initializer, init_lib.SinkhornInitializer):
       return self.initializer
     if self.initializer == "default":
       return init_lib.DefaultInitializer()
     if self.initializer == "gaussian":
       return init_lib.GaussianInitializer()
     if self.initializer == "sorting":
       return init_lib.SortingInitializer(**self.kwargs_init)
+    if self.initializer == "subsample":
+      return init_lib.SubsampleInitializer(**self.kwargs_init)
     raise NotImplementedError(
         f"Initializer `{self.initializer}` is not yet implemented."
     )
 
-  def tree_flatten(self):
+  def tree_flatten(self):  # noqa: D102
     aux = vars(self).copy()
-    aux['norm_error'] = aux.pop('_norm_error')
-    aux.pop('threshold')
+    aux["norm_error"] = aux.pop("_norm_error")
+    aux.pop("threshold")
     return [self.threshold], aux
 
   @classmethod
-  def tree_unflatten(cls, aux_data, children):
+  def tree_unflatten(cls, aux_data, children):  # noqa: D102
     return cls(**aux_data, threshold=children[0])
 
 
 def run(
     ot_prob: linear_problem.LinearProblem, solver: Sinkhorn,
     init: Tuple[jnp.ndarray, ...]
 ) -> SinkhornOutput:
@@ -1101,15 +1119,15 @@
     geom: geometry.Geometry,
     a: Optional[jnp.ndarray] = None,
     b: Optional[jnp.ndarray] = None,
     tau_a: float = 1.0,
     tau_b: float = 1.0,
     rank: int = -1,
     **kwargs: Any
-) -> Union[SinkhornOutput, 'LRSinkhornOutput']:
+) -> Union[SinkhornOutput, "LRSinkhornOutput"]:
   """Solve linear regularized OT problem using Sinkhorn iterations.
 
   Args:
     geom: The ground geometry cost of the linear problem.
     a: The first marginal. If `None`, it will be uniform.
     b: The second marginal. If `None`, it will be uniform.
     tau_a: If `< 1`, defines how much unbalanced the problem is
@@ -1118,15 +1136,15 @@
       on the second marginal.
     rank:
       Rank constraint on the coupling to minimize the linear OT problem
       :cite:`scetbon:21`. If `-1`, no rank constraint is used.
     kwargs: Keyword arguments for
       :class:`~ott.solvers.linear.sinkhorn.Sinkhorn` or
       :class:`~ott.solvers.linear.sinkhorn_lr.LRSinkhorn`,
-      depending ``rank``.
+      depending on ``rank``.
 
   Returns:
     The Sinkhorn output.
   """
   prob = linear_problem.LinearProblem(geom, a=a, b=b, tau_a=tau_a, tau_b=tau_b)
   solver = LRSinkhorn(rank=rank, **kwargs) if rank > 0 else Sinkhorn(**kwargs)
   return solver(prob)
```

### Comparing `ott-jax-0.4.0/src/ott/solvers/linear/sinkhorn_lr.py` & `ott-jax-0.4.1/src/ott/solvers/linear/sinkhorn_lr.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,105 +1,131 @@
-# Copyright 2022 Google LLC.
+# Copyright OTT-JAX
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-#     http://www.apache.org/licenses/LICENSE-2.0
+#   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """A Jax implementation of the Low-Rank Sinkhorn algorithm."""
-from typing import Any, Literal, Mapping, NamedTuple, NoReturn, Optional, Tuple, Union
+from typing import (
+    Any,
+    Callable,
+    Literal,
+    Mapping,
+    NamedTuple,
+    Optional,
+    Tuple,
+    Union,
+)
 
 import jax
 import jax.numpy as jnp
 import jax.scipy as jsp
+import numpy as np
+from jax.experimental import host_callback
 
 from ott.geometry import geometry, low_rank, pointcloud
 from ott.initializers.linear import initializers_lr as init_lib
 from ott.math import fixed_point_loop
 from ott.math import utils as mu
 from ott.problems.linear import linear_problem
 from ott.solvers.linear import sinkhorn
 
 __all__ = ["LRSinkhorn", "LRSinkhornOutput"]
 
+ProgressCallbackFn_t = Callable[
+    [Tuple[np.ndarray, np.ndarray, np.ndarray, "LRSinkhornState"]], None]
+
 
 class LRSinkhornState(NamedTuple):
   """State of the Low Rank Sinkhorn algorithm."""
 
   q: jnp.ndarray
   r: jnp.ndarray
   g: jnp.ndarray
   gamma: float
   costs: jnp.ndarray
   errors: jnp.ndarray
   crossed_threshold: bool
 
-  def compute_error(self, previous_state: "LRSinkhornState") -> float:
+  def compute_error(  # noqa: D102
+      self, previous_state: "LRSinkhornState"
+  ) -> float:
     err_1 = mu.js(self.q, previous_state.q, c=1.)
     err_2 = mu.js(self.r, previous_state.r, c=1.)
     err_3 = mu.js(self.g, previous_state.g, c=1.)
 
     return ((1. / self.gamma) ** 2) * (err_1 + err_2 + err_3)
 
-  def reg_ot_cost(
+  def reg_ot_cost(  # noqa: D102
       self,
       ot_prob: linear_problem.LinearProblem,
       use_danskin: bool = False
   ) -> float:
     return compute_reg_ot_cost(self.q, self.r, self.g, ot_prob, use_danskin)
 
-  def solution_error(
-      self, ot_prob: linear_problem.LinearProblem, norm_error: Tuple[int, ...],
-      lse_mode: bool
+  def solution_error(  # noqa: D102
+      self, ot_prob: linear_problem.LinearProblem, norm_error: Tuple[int, ...]
   ) -> jnp.ndarray:
-    return solution_error(self.q, self.r, ot_prob, norm_error, lse_mode)
+    return solution_error(self.q, self.r, ot_prob, norm_error)
 
-  def set(self, **kwargs: Any) -> 'LRSinkhornState':
+  def set(self, **kwargs: Any) -> "LRSinkhornState":
     """Return a copy of self, with potential overwrites."""
     return self._replace(**kwargs)
 
 
 def compute_reg_ot_cost(
     q: jnp.ndarray,
     r: jnp.ndarray,
     g: jnp.ndarray,
     ot_prob: linear_problem.LinearProblem,
     use_danskin: bool = False
 ) -> float:
+  """Compute the regularized OT cost.
+
+  Args:
+    q: first factor of solution
+    r: second factor of solution
+    g: weights of solution
+    ot_prob: linear problem
+    use_danskin: if True, use Danskin's theorem :cite:`danskin:67,bertsekas:71`
+      to avoid computing the gradient of the cost function.
+
+  Returns:
+    regularized OT cost
+  """
   q = jax.lax.stop_gradient(q) if use_danskin else q
   r = jax.lax.stop_gradient(r) if use_danskin else r
   g = jax.lax.stop_gradient(g) if use_danskin else g
   return jnp.sum(ot_prob.geom.apply_cost(r, axis=1) * q * (1. / g)[None, :])
 
 
 def solution_error(
     q: jnp.ndarray, r: jnp.ndarray, ot_prob: linear_problem.LinearProblem,
-    norm_error: Tuple[int, ...], lse_mode: bool
+    norm_error: Tuple[int, ...]
 ) -> jnp.ndarray:
   """Compute solution error.
 
   Since only balanced case is available for LR, this is marginal deviation.
 
   Args:
-    q: first factor of solution
-    r: second factor of solution
-    ot_prob: linear problem
+    q: first factor of solution.
+    r: second factor of solution.
+    ot_prob: linear problem.
     norm_error: int, p-norm used to compute error.
-    lse_mode: True if log-sum-exp operations, False if kernel vector products.
 
   Returns:
     one or possibly many numbers quantifying deviation to true marginals.
   """
-  del lse_mode
   norm_error = jnp.array(norm_error)
   # Update the error
   err = jnp.sum(
       jnp.abs(jnp.sum(q, axis=1) - ot_prob.a) ** norm_error[:, None], axis=1
   ) ** (1.0 / norm_error)
   err += jnp.sum(
       jnp.abs(jnp.sum(r, axis=1) - ot_prob.b) ** norm_error[:, None], axis=1
@@ -122,56 +148,56 @@
   # TODO(michalk8): must be called `errors`, because of `store_inner_errors`
   # in future, enforce via class hierarchy
   errors: jnp.ndarray
   ot_prob: linear_problem.LinearProblem
   # TODO(michalk8): Optional is an artifact of the current impl., refactor
   reg_ot_cost: Optional[float] = None
 
-  def set(self, **kwargs: Any) -> 'LRSinkhornOutput':
+  def set(self, **kwargs: Any) -> "LRSinkhornOutput":
     """Return a copy of self, with potential overwrites."""
     return self._replace(**kwargs)
 
-  def set_cost(
+  def set_cost(  # noqa: D102
       self,
       ot_prob: linear_problem.LinearProblem,
       lse_mode: bool,
       use_danskin: bool = False
-  ) -> 'LRSinkhornOutput':
+  ) -> "LRSinkhornOutput":
     del lse_mode
     return self.set(reg_ot_cost=self.compute_reg_ot_cost(ot_prob, use_danskin))
 
-  def compute_reg_ot_cost(
+  def compute_reg_ot_cost(  # noqa: D102
       self,
       ot_prob: linear_problem.LinearProblem,
       use_danskin: bool = False,
   ) -> float:
     return compute_reg_ot_cost(self.q, self.r, self.g, ot_prob, use_danskin)
 
   @property
-  def linear(self) -> bool:
+  def linear(self) -> bool:  # noqa: D102
     return isinstance(self.ot_prob, linear_problem.LinearProblem)
 
   @property
-  def geom(self) -> geometry.Geometry:
+  def geom(self) -> geometry.Geometry:  # noqa: D102
     return self.ot_prob.geom
 
   @property
-  def a(self) -> jnp.ndarray:
+  def a(self) -> jnp.ndarray:  # noqa: D102
     return self.ot_prob.a
 
   @property
-  def b(self) -> jnp.ndarray:
+  def b(self) -> jnp.ndarray:  # noqa: D102
     return self.ot_prob.b
 
   @property
-  def linear_output(self) -> bool:
+  def linear_output(self) -> bool:  # noqa: D102
     return True
 
   @property
-  def converged(self) -> bool:
+  def converged(self) -> bool:  # noqa: D102
     return jnp.logical_and(
         jnp.any(self.costs == -1), jnp.all(jnp.isfinite(self.costs))
     )
 
   @property
   def matrix(self) -> jnp.ndarray:
     """Transport matrix if it can be instantiated."""
@@ -179,28 +205,28 @@
 
   def apply(self, inputs: jnp.ndarray, axis: int = 0) -> jnp.ndarray:
     """Apply the transport to a array; axis=1 for its transpose."""
     q, r = (self.q, self.r) if axis == 1 else (self.r, self.q)
     # for `axis=0`: (batch, m), (m, r), (r,), (r, n)
     return ((inputs @ r) * self._inv_g) @ q.T
 
-  def marginal(self, axis: int) -> jnp.ndarray:
+  def marginal(self, axis: int) -> jnp.ndarray:  # noqa: D102
     length = self.q.shape[0] if axis == 0 else self.r.shape[0]
     return self.apply(jnp.ones(length,), axis=axis)
 
   def cost_at_geom(self, other_geom: geometry.Geometry) -> float:
     """Return OT cost for current solution, evaluated at any cost matrix."""
     return jnp.sum(self.q * other_geom.apply_cost(self.r, axis=1) * self._inv_g)
 
   def transport_cost_at_geom(self, other_geom: geometry.Geometry) -> float:
     """Return (by recomputing it) bare transport cost of current solution."""
     return self.cost_at_geom(other_geom)
 
   @property
-  def primal_cost(self) -> jnp.ndarray:
+  def primal_cost(self) -> float:
     """Return (by recomputing it) transport cost of current solution."""
     return self.transport_cost_at_geom(other_geom=self.geom)
 
   @property
   def transport_mass(self) -> float:
     """Sum of transport matrix."""
     return self.marginal(0).sum()
@@ -225,35 +251,34 @@
   Args:
     rank: Rank constraint on the coupling to minimize the linear OT problem
     gamma: The (inverse of) gradient step size used by mirror descent.
     gamma_rescale: Whether to rescale :math:`\gamma` every iteration as
       described in :cite:`scetbon:22b`.
     epsilon: Entropic regularization added on top of low-rank problem.
     initializer: How to initialize the :math:`Q`, :math:`R` and :math:`g`
-      factors. Valid options are:
-
-        - `'random'` - :class:`~ott.initializers.linear.initializers_lr.RandomInitializer`.
-        - `'rank2'` - :class:`~ott.initializers.linear.initializers_lr.Rank2Initializer`.
-        - `'k-means'` - :class:`~ott.initializers.linear.initializers_lr.KMeansInitializer`.
-        - `'generalized-k-means'` - :class:`~ott.initializers.linear.initializers_lr.GeneralizedKMeansInitializer`.
-
-      If `None`, :class:`~ott.initializers.linear.initializers_lr.KMeansInitializer`
+      factors. Valid options are `'random'`, `'rank2'`, `'k-means'`, and
+      `'generalized-k-means`. If `None`,
+      :class:`~ott.initializers.linear.initializers_lr.KMeansInitializer`
       is used when the linear problem's geometry is
       :class:`~ott.geometry.pointcloud.PointCloud` or
-      :class:`~ott.geometry.low_rank.LRCGeometry`.
-      Otherwise, use :class:`~ott.initializers.linear.initializers_lr.RandomInitializer`.
+      :class:`~ott.geometry.low_rank.LRCGeometry`. Otherwise, use
+      :class:`~ott.initializers.linear.initializers_lr.RandomInitializer`.
 
     lse_mode: Whether to run computations in lse or kernel mode. At the moment,
       only ``lse_mode = True`` is implemented.
     inner_iterations: Number of inner iterations used by the algorithm before
       re-evaluating progress.
     use_danskin: Use Danskin theorem to evaluate gradient of objective w.r.t.
       input parameters. Only `True` handled at this moment.
     implicit_diff: Whether to use implicit differentiation. Currently, only
       ``implicit_diff = False`` is implemented.
+    progress_fn: callback function which gets called during the Sinkhorn
+      iterations, so the user can display the error at each iteration,
+      e.g., using a progress bar. See :func:`~ott.utils.default_progress_fn`
+      for a basic implementation.
     kwargs_dys: Keyword arguments passed to :meth:`dykstra_update`.
     kwargs_init: Keyword arguments for
       :class:`~ott.initializers.linear.initializers_lr.LRInitializer`.
     kwargs: Keyword arguments for
       :class:`~ott.solvers.linear.sinkhorn.Sinkhorn`.
   """
 
@@ -268,64 +293,64 @@
                                   init_lib.LRInitializer]] = "random",
       lse_mode: bool = True,
       inner_iterations: int = 10,
       use_danskin: bool = True,
       implicit_diff: bool = False,
       kwargs_dys: Optional[Mapping[str, Any]] = None,
       kwargs_init: Optional[Mapping[str, Any]] = None,
+      progress_fn: Optional[ProgressCallbackFn_t] = None,
       **kwargs: Any,
   ):
-    assert lse_mode, "Kernel mode not yet implemented."
     assert not implicit_diff, "Implicit diff. not yet implemented."
     super().__init__(
         lse_mode=lse_mode,
         inner_iterations=inner_iterations,
         use_danskin=use_danskin,
         implicit_diff=implicit_diff,
         **kwargs
     )
     self.rank = rank
     self.gamma = gamma
     self.gamma_rescale = gamma_rescale
     self.epsilon = epsilon
     self.initializer = initializer
+    self.progress_fn = progress_fn
     # can be `None`
     self.kwargs_dys = {} if kwargs_dys is None else kwargs_dys
     self.kwargs_init = {} if kwargs_init is None else kwargs_init
 
   def __call__(
       self,
       ot_prob: linear_problem.LinearProblem,
       init: Tuple[Optional[jnp.ndarray], Optional[jnp.ndarray],
                   Optional[jnp.ndarray]] = (None, None, None),
-      key: Optional[jnp.ndarray] = None,
+      rng: Optional[jax.random.PRNGKeyArray] = None,
       **kwargs: Any,
   ) -> LRSinkhornOutput:
     """Run low-rank Sinkhorn.
 
     Args:
       ot_prob: Linear OT problem.
       init: Initial values for the low-rank factors:
 
         - :attr:`~ott.solvers.linear.sinkhorn_lr.LRSinkhornOutput.q`.
         - :attr:`~ott.solvers.linear.sinkhorn_lr.LRSinkhornOutput.r`.
         - :attr:`~ott.solvers.linear.sinkhorn_lr.LRSinkhornOutput.g`.
 
         Any `None` values will be initialized using the initializer.
-      key: Random key for seeding.
+      rng: Random key for seeding.
       kwargs: Additional arguments when calling the initializer.
 
     Returns:
       The low-rank Sinkhorn output.
     """
     assert ot_prob.is_balanced, "Unbalanced case is not implemented."
     initializer = self.create_initializer(ot_prob)
-    init = initializer(ot_prob, *init, key=key, **kwargs)
-    run_fn = jax.jit(run) if self.jit else run
-    return run_fn(ot_prob, self, init)
+    init = initializer(ot_prob, *init, rng=rng, **kwargs)
+    return run(ot_prob, self, init)
 
   def _lr_costs(
       self,
       ot_prob: linear_problem.LinearProblem,
       state: LRSinkhornState,
   ) -> Tuple[jnp.ndarray, jnp.ndarray, jnp.ndarray, float]:
     log_q, log_r, log_g = (
@@ -352,27 +377,61 @@
       gamma = self.gamma
 
     c_q = grad_q - (1. / gamma) * log_q
     c_r = grad_r - (1. / gamma) * log_r
     h = -grad_g + (1. / gamma) * log_g
     return c_q, c_r, h, gamma
 
-  def dykstra_update(
+  def _lr_kernels(
+      self,
+      ot_prob: linear_problem.LinearProblem,
+      state: LRSinkhornState,
+  ) -> Tuple[jnp.ndarray, jnp.ndarray, jnp.ndarray, float]:
+    log_q, log_r, log_g = (
+        mu.safe_log(state.q), mu.safe_log(state.r), mu.safe_log(state.g)
+    )
+
+    grad_q = ot_prob.geom.apply_cost(state.r, axis=1) / state.g[None, :]
+    grad_r = ot_prob.geom.apply_cost(state.q) / state.g[None, :]
+    diag_qcr = jnp.sum(
+        state.q * ot_prob.geom.apply_cost(state.r, axis=1), axis=0
+    )
+    grad_g = -diag_qcr / (state.g ** 2)
+    if self.is_entropic:
+      grad_q += self.epsilon * log_q
+      grad_r += self.epsilon * log_r
+      grad_g += self.epsilon * log_g
+
+    if self.gamma_rescale:
+      norm_q = jnp.max(jnp.abs(grad_q)) ** 2
+      norm_r = jnp.max(jnp.abs(grad_r)) ** 2
+      norm_g = jnp.max(jnp.abs(grad_g)) ** 2
+      gamma = self.gamma / jnp.max(jnp.array([norm_q, norm_r, norm_g]))
+    else:
+      gamma = self.gamma
+
+    k_q = jnp.exp((-gamma) * (grad_q - (1. / gamma) * log_q))
+    k_r = jnp.exp((-gamma) * (grad_r - (1. / gamma) * log_r))
+    k_g = jnp.exp((-gamma) * (grad_g - (1. / gamma) * log_g))
+    return k_q, k_r, k_g, gamma
+
+  def dykstra_update_lse(
       self,
       c_q: jnp.ndarray,
       c_r: jnp.ndarray,
       h: jnp.ndarray,
       gamma: float,
       ot_prob: linear_problem.LinearProblem,
       min_entry_value: float = 1e-6,
       tolerance: float = 1e-3,
       min_iter: int = 0,
       inner_iter: int = 10,
       max_iter: int = 10000
   ) -> Tuple[jnp.ndarray, jnp.ndarray, jnp.ndarray]:
+    """Run Dykstra's algorithm."""
     # shortcuts for problem's definition.
     r = self.rank
     n, m = ot_prob.geom.shape
     loga, logb = jnp.log(ot_prob.a), jnp.log(ot_prob.b)
 
     h_old = h
     g1_old, g2_old = jnp.zeros(r), jnp.zeros(r)
@@ -441,16 +500,15 @@
 
       g1_old = g1
       g2_old = g2
       h_old = h
 
       err = jax.lax.cond(
           jnp.logical_and(compute_error, iteration >= min_iter),
-          lambda: solution_error(q, r, ot_prob, self.norm_error, self.lse_mode)[
-              0], lambda: err
+          lambda: solution_error(q, r, ot_prob, self.norm_error)[0], lambda: err
       )
 
       return f1, f2, g1_old, g2_old, h_old, w_gi, w_gp, w_q, w_r, err
 
     def recompute_couplings(
         f1: jnp.ndarray,
         g1: jnp.ndarray,
@@ -469,38 +527,138 @@
     state_inner = fixed_point_loop.fixpoint_iter_backprop(
         cond_fn, body_fn, min_iter, max_iter, inner_iter, constants, state_inner
     )
 
     f1, f2, g1_old, g2_old, h_old, _, _, _, _, _ = state_inner
     return recompute_couplings(f1, g1_old, c_q, f2, g2_old, c_r, h_old, gamma)
 
+  def dykstra_update_kernel(
+      self,
+      k_q: jnp.ndarray,
+      k_r: jnp.ndarray,
+      k_g: jnp.ndarray,
+      gamma: float,
+      ot_prob: linear_problem.LinearProblem,
+      min_entry_value: float = 1e-6,
+      tolerance: float = 1e-3,
+      min_iter: int = 0,
+      inner_iter: int = 10,
+      max_iter: int = 10000
+  ) -> Tuple[jnp.ndarray, jnp.ndarray, jnp.ndarray]:
+    """Run Dykstra's algorithm."""
+    # shortcuts for problem's definition.
+    rank = self.rank
+    n, m = ot_prob.geom.shape
+    a, b = ot_prob.a, ot_prob.b
+    supp_a, supp_b = a > 0, b > 0
+
+    g_old = k_g
+    v1_old, v2_old = jnp.ones(rank), jnp.ones(rank)
+    u1, u2 = jnp.ones(n), jnp.ones(m)
+
+    q_gi, q_gp = jnp.ones(rank), jnp.ones(rank)
+    q_q, q_r = jnp.ones(rank), jnp.ones(rank)
+    err = jnp.inf
+    state_inner = u1, u2, v1_old, v2_old, g_old, q_gi, q_gp, q_q, q_r, err
+    constants = k_q, k_r, k_g, a, b
+
+    def cond_fn(
+        iteration: int, constants: Tuple[jnp.ndarray, ...],
+        state_inner: Tuple[jnp.ndarray, ...]
+    ) -> bool:
+      del iteration, constants
+      *_, err = state_inner
+      return err > tolerance
+
+    def body_fn(
+        iteration: int, constants: Tuple[jnp.ndarray, ...],
+        state_inner: Tuple[jnp.ndarray, ...], compute_error: bool
+    ) -> Tuple[jnp.ndarray, ...]:
+      # TODO(michalk8): in the future, use `NamedTuple`
+      u1, u2, v1_old, v2_old, g_old, q_gi, q_gp, q_q, q_r, err = state_inner
+      k_q, k_r, k_g, a, b = constants
+
+      # First Projection
+      u1 = jnp.where(supp_a, a / jnp.dot(k_q, v1_old), 0.0)
+      u2 = jnp.where(supp_b, b / jnp.dot(k_r, v2_old), 0.0)
+      g = jnp.maximum(min_entry_value, g_old * q_gi)
+      q_gi = (g_old * q_gi) / g
+      g_old = g
+
+      # Second Projection
+      v1_trans = jnp.dot(k_q.T, u1)
+      v2_trans = jnp.dot(k_r.T, u2)
+      g = (g_old * q_gp * v1_old * q_q * v1_trans * v2_old * q_r *
+           v2_trans) ** (1 / 3)
+      v1 = g / v1_trans
+      v2 = g / v2_trans
+      q_gp = (g_old * q_gp) / g
+      q_q = (q_q * v1_old) / v1
+      q_r = (q_r * v2_old) / v2
+      v1_old = v1
+      v2_old = v2
+      g_old = g
+
+      # Compute Couplings
+      q, r, _ = recompute_couplings(u1, v1, k_q, u2, v2, k_r, g)
+
+      err = jax.lax.cond(
+          jnp.logical_and(compute_error, iteration >= min_iter),
+          lambda: solution_error(q, r, ot_prob, self.norm_error)[0], lambda: err
+      )
+
+      return u1, u2, v1_old, v2_old, g_old, q_gi, q_gp, q_q, q_r, err
+
+    def recompute_couplings(
+        u1: jnp.ndarray,
+        v1: jnp.ndarray,
+        k_q: jnp.ndarray,
+        u2: jnp.ndarray,
+        v2: jnp.ndarray,
+        k_r: jnp.ndarray,
+        g: jnp.ndarray,
+    ) -> Tuple[jnp.ndarray, jnp.ndarray, jnp.ndarray]:
+      q = u1.reshape((-1, 1)) * k_q * v1.reshape((1, -1))
+      r = u2.reshape((-1, 1)) * k_r * v2.reshape((1, -1))
+      return q, r, g
+
+    state_inner = fixed_point_loop.fixpoint_iter_backprop(
+        cond_fn, body_fn, min_iter, max_iter, inner_iter, constants, state_inner
+    )
+
+    u1, u2, v1_old, v2_old, g_old, _, _, _, _, _ = state_inner
+    return recompute_couplings(u1, v1_old, k_q, u2, v2_old, k_r, g_old)
+
   def lse_step(
       self, ot_prob: linear_problem.LinearProblem, state: LRSinkhornState,
       iteration: int
   ) -> LRSinkhornState:
     """LR Sinkhorn LSE update."""
     c_q, c_r, h, gamma = self._lr_costs(ot_prob, state)
-    q, r, g = self.dykstra_update(
+    q, r, g = self.dykstra_update_lse(
         c_q, c_r, h, gamma, ot_prob, **self.kwargs_dys
     )
     return state.set(q=q, g=g, r=r, gamma=gamma)
 
   def kernel_step(
       self, ot_prob: linear_problem.LinearProblem, state: LRSinkhornState,
       iteration: int
-  ) -> NoReturn:
-    """Not implemented."""
-    # TODO(cuturi): kernel step not implemented.
-    raise NotImplementedError("Not implemented.")
+  ) -> LRSinkhornState:
+    """LR Sinkhorn Kernel update."""
+    k_q, k_r, k_g, gamma = self._lr_kernels(ot_prob, state)
+    q, r, g = self.dykstra_update_kernel(
+        k_q, k_r, k_g, gamma, ot_prob, **self.kwargs_dys
+    )
+    return state.set(q=q, g=g, r=r, gamma=gamma)
 
   def one_iteration(
       self, ot_prob: linear_problem.LinearProblem, state: LRSinkhornState,
       iteration: int, compute_error: bool
   ) -> LRSinkhornState:
-    """Carries out one LR sinkhorn iteration.
+    """Carries out one low-rank Sinkhorn iteration.
 
     Depending on lse_mode, these iterations can be either in:
 
       - log-space for numerical stability.
       - scaling space, using standard kernel-vector multiply operations.
 
     Args:
@@ -528,22 +686,30 @@
     crossed_threshold = jnp.logical_or(
         state.crossed_threshold,
         jnp.logical_and(
             state.errors[it - 1] >= self.threshold, error < self.threshold
         )
     )
 
-    return state.set(
+    state = state.set(
         costs=state.costs.at[it].set(cost),
         errors=state.errors.at[it].set(error),
         crossed_threshold=crossed_threshold,
     )
 
+    if self.progress_fn is not None:
+      host_callback.id_tap(
+          self.progress_fn,
+          (iteration, self.inner_iterations, self.max_iterations, state)
+      )
+
+    return state
+
   @property
-  def norm_error(self) -> Tuple[int]:
+  def norm_error(self) -> Tuple[int]:  # noqa: D102
     return self._norm_error,
 
   @property
   def is_entropic(self) -> bool:
     """Whether entropy regularization is used."""
     return self.epsilon > 0.
```

### Comparing `ott-jax-0.4.0/src/ott/solvers/nn/conjugate_solvers.py` & `ott-jax-0.4.1/src/ott/solvers/nn/conjugate_solvers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,25 @@
+# Copyright OTT-JAX
+#
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Implementation of :cite:`amos:17` input convex neural networks (ICNN)."""
-
 import abc
 from typing import Callable, Literal, NamedTuple, Optional
 
-from jaxopt import LBFGS
-
 import jax.numpy as jnp
+from jaxopt import LBFGS
 
 from ott import utils
 
 __all__ = [
     "ConjugateResults",
     "FenchelConjugateSolver",
     "FenchelConjugateLBFGS",
@@ -32,15 +31,14 @@
   r"""Holds the results of numerically conjugating a function.
 
   Args:
     val: the conjugate value, i.e., :math:`f^\star(y)`
     grad: the gradient, i.e., :math:`\nabla f^\star(y)`
     num_iter: the number of iterations taken by the solver
   """
-
   val: float
   grad: jnp.ndarray
   num_iter: int
 
 
 class FenchelConjugateSolver(abc.ABC):
   r"""Abstract conjugate solver class.
@@ -71,34 +69,34 @@
 @utils.register_pytree_node
 class FenchelConjugateLBFGS(FenchelConjugateSolver):
   """Solve for the conjugate using :class:`jaxopt.LBFGS`.
 
   Args:
     gtol: gradient tolerance
     max_iter: maximum number of iterations
-    max_linesearch_iter: maximum number of linesearch iterations
-    linesearch_type: type of linesearch
+    max_linesearch_iter: maximum number of line search iterations
+    linesearch_type: type of line search
     decrease_factor: decrease factor for a backtracking line search
     ls_method: the line search method
   """
 
   gtol: float = 1e-3
   max_iter: int = 10
   max_linesearch_iter: int = 10
-  linesearch_type: Literal['zoom', 'backtracking'] = 'backtracking'
+  linesearch_type: Literal["zoom", "backtracking"] = "backtracking"
   decrease_factor: float = 0.66
-  ls_method: Literal['wolf', 'strong-wolfe'] = 'strong-wolfe'
+  ls_method: Literal["wolf", "strong-wolfe"] = "strong-wolfe"
 
-  def solve(
+  def solve(  # noqa: D102
       self,
       f: Callable[[jnp.ndarray], jnp.ndarray],
       y: jnp.ndarray,
       x_init: Optional[jnp.array] = None
   ) -> ConjugateResults:
-    assert y.ndim == 1
+    assert y.ndim == 1, y.ndim
 
     solver = LBFGS(
         fun=lambda x: f(x) - x.dot(y),
         tol=self.gtol,
         maxiter=self.max_iter,
         decrease_factor=self.decrease_factor,
         linesearch=self.linesearch_type,
@@ -113,9 +111,9 @@
     )
 
 
 DEFAULT_CONJUGATE_SOLVER = FenchelConjugateLBFGS(
     gtol=1e-5,
     max_iter=20,
     max_linesearch_iter=20,
-    linesearch_type='backtracking',
+    linesearch_type="backtracking",
 )
```

### Comparing `ott-jax-0.4.0/src/ott/solvers/nn/layers.py` & `ott-jax-0.4.1/src/ott/solvers/nn/layers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
+# Copyright OTT-JAX
+#
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-#     http://www.apache.org/licenses/LICENSE-2.0
+#   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Layers used in input convex neural networks :cite:`amos:17,bunne:22`."""
-
 from typing import Any, Callable, Tuple
 
 import flax.linen as nn
 import jax
 import jax.numpy as jnp
 
 __all__ = ["PositiveDense", "PosDefPotentials"]
@@ -52,31 +52,33 @@
 
   @nn.compact
   def __call__(self, inputs: jnp.ndarray) -> jnp.ndarray:
     """Applies a linear transformation to inputs along the last dimension.
 
     Args:
       inputs: Array to be transformed.
+
     Returns:
       The transformed input.
     """
     inputs = jnp.asarray(inputs, self.dtype)
     kernel = self.param(
-        'kernel', self.kernel_init, (inputs.shape[-1], self.dim_hidden)
+        "kernel", self.kernel_init, (inputs.shape[-1], self.dim_hidden)
     )
     kernel = self.rectifier_fn(kernel)
+    kernel = jnp.asarray(kernel, self.dtype)
     y = jax.lax.dot_general(
         inputs,
         kernel, (((inputs.ndim - 1,), (0,)), ((), ())),
         precision=self.precision
     )
     if self.use_bias:
-      bias = self.param('bias', self.bias_init, (self.dim_hidden,))
+      bias = self.param("bias", self.bias_init, (self.dim_hidden,))
       bias = jnp.asarray(bias, self.dtype)
-      y = y + bias
+      return y + bias
     return y
 
 
 class PosDefPotentials(nn.Module):
   """A layer to output  (0.5 [A_i A_i^T] (x - b_i)_i potentials.
 
   Args:
@@ -127,9 +129,8 @@
       y = jax.lax.dot_general(
           inputs,
           kernel, (((inputs.ndim - 1,), (0,)), ((), ())),
           precision=self.precision
       )
 
     y = 0.5 * y * y
-    out = jnp.sum(y.reshape((-1, self.num_potentials, self.dim_data)), axis=2)
-    return out
+    return jnp.sum(y.reshape((-1, self.num_potentials, self.dim_data)), axis=2)
```

### Comparing `ott-jax-0.4.0/src/ott/solvers/nn/models.py` & `ott-jax-0.4.1/src/ott/solvers/nn/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
+# Copyright OTT-JAX
+#
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Neural potential models."""
-
 import abc
-from typing import Callable, Optional, Sequence, Tuple, Union
+from typing import Any, Callable, Optional, Sequence, Tuple, Union
 
 import flax.linen as nn
 import jax
 import jax.numpy as jnp
 import optax
 from flax import struct
 from flax.core import frozen_dict
@@ -31,15 +31,15 @@
 PotentialValueFn_t = Callable[[jnp.ndarray], jnp.ndarray]
 PotentialGradientFn_t = Callable[[jnp.ndarray], jnp.ndarray]
 
 
 class NeuralTrainState(train_state.TrainState):
   """Adds information about the model's value and gradient to the state.
 
-  This extends :class:`flax.training.train_state.TrainState` to include
+  This extends :class:`~flax.training.train_state.TrainState` to include
   the potential methods from :class:`~ott.solvers.nn.models.ModelBase`
   used during training.
 
   Args:
     potential_value_fn: the potential's value function
     potential_gradient_fn: the potential's gradient function
   """
@@ -72,45 +72,46 @@
   ) -> PotentialValueFn_t:
     r"""Return a function giving the value of the potential.
 
     Applies the module if :attr:`is_potential` is ``True``, otherwise
     constructs the value of the potential from the gradient with
 
     .. math::
+
       g(y) = -f(\nabla_y g(y)) + y^T \nabla_y g(y)
 
     where :math:`\nabla_y g(y)` is detached for the envelope theorem
     :cite:`danskin:67,bertsekas:71`
     to give the appropriate first derivatives of this construction.
 
     Args:
       params: parameters of the module
-      x: point to evaluate the value at
-      other_potential_value: function giving the value of the other potential.
-        Only needed when :attr:`is_potential` is ``False``.
+      other_potential_value_fn: function giving the value of the other
+        potential. Only needed when :attr:`is_potential` is ``False``.
 
     Returns:
       A function that can be evaluated to obtain the potential's value
     """
     if self.is_potential:
       return lambda x: self.apply({"params": params}, x)
-    else:
-      assert other_potential_value_fn is not None, \
-          "The value of the gradient-based potential depends on the value of the other potential"
 
-      def value_fn(x: jnp.ndarray) -> jnp.ndarray:
-        squeeze = x.ndim == 1
-        if squeeze:
-          x = jnp.expand_dims(x, 0)
-        grad_g_x = jax.lax.stop_gradient(self.apply({"params": params}, x))
-        value = -other_potential_value_fn(grad_g_x) + \
-            jax.vmap(jnp.dot)(grad_g_x, x)
-        return value.squeeze(0) if squeeze else value
+    assert other_potential_value_fn is not None, \
+        "The value of the gradient-based potential depends " \
+        "on the value of the other potential."
+
+    def value_fn(x: jnp.ndarray) -> jnp.ndarray:
+      squeeze = x.ndim == 1
+      if squeeze:
+        x = jnp.expand_dims(x, 0)
+      grad_g_x = jax.lax.stop_gradient(self.apply({"params": params}, x))
+      value = -other_potential_value_fn(grad_g_x) + \
+          jax.vmap(jnp.dot)(grad_g_x, x)
+      return value.squeeze(0) if squeeze else value
 
-      return value_fn
+    return value_fn
 
   def potential_gradient_fn(
       self,
       params: frozen_dict.FrozenDict[str, jnp.ndarray],
   ) -> PotentialGradientFn_t:
     """Return a function giving the gradient of the potential.
 
@@ -118,16 +119,34 @@
       params: parameters of the module
 
     Returns:
       A function that can be evaluated to obtain the potential's gradient
     """
     if self.is_potential:
       return jax.vmap(jax.grad(self.potential_value_fn(params)))
-    else:
-      return lambda x: self.apply({'params': params}, x)
+    return lambda x: self.apply({"params": params}, x)
+
+  def create_train_state(
+      self,
+      rng: jax.random.PRNGKeyArray,
+      optimizer: optax.OptState,
+      input: Union[int, Tuple[int, ...]],
+      **kwargs: Any,
+  ) -> NeuralTrainState:
+    """Create initial training state."""
+    params = self.init(rng, jnp.ones(input))["params"]
+
+    return NeuralTrainState.create(
+        apply_fn=self.apply,
+        params=params,
+        tx=optimizer,
+        potential_value_fn=self.potential_value_fn,
+        potential_gradient_fn=self.potential_gradient_fn,
+        **kwargs,
+    )
 
 
 class ICNN(ModelBase):
   """Input convex neural network (ICNN) architecture with initialization.
 
   Implementation of input convex neural networks as introduced in
   :cite:`amos:17` with initialization schemes proposed by :cite:`bunne:22`.
@@ -144,28 +163,27 @@
     pos_weights: Enforce positive weights with a projection.
       If ``False``, the positive weights should be enforced with clipping
       or regularization in the loss.
     gaussian_map: data inputs of source and target measures for
       initialization scheme based on Gaussian approximation of input and
       target measure (if ``None``, identity initialization is used).
   """
-
   dim_data: int
   dim_hidden: Sequence[int]
   init_std: float = 1e-2
   init_fn: Callable = jax.nn.initializers.normal
-  act_fn: Callable = nn.relu
+  act_fn: Callable[[jnp.ndarray], jnp.ndarray] = nn.relu
   pos_weights: bool = True
-  gaussian_map: Tuple[jnp.ndarray, jnp.ndarray] = None
+  gaussian_map: Optional[Tuple[jnp.ndarray, jnp.ndarray]] = None
 
   @property
-  def is_potential(self) -> bool:
+  def is_potential(self) -> bool:  # noqa: D102
     return True
 
-  def setup(self) -> None:
+  def setup(self) -> None:  # noqa: D102
     self.num_hidden = len(self.dim_hidden)
 
     if self.pos_weights:
       hid_dense = layers.PositiveDense
       # this function needs to be the inverse map of function
       # used in PositiveDense layers
       rescale = hid_dense.inv_rectifier_fn
@@ -207,15 +225,15 @@
         self.dim_data,
         num_potentials=1,
         kernel_init=lambda *_: factor,
         bias_init=lambda *_: mean,
         use_bias=True,
     )
 
-    # subsequent layers reinjected into convex functions
+    # subsequent layers re-injected into convex functions
     w_xs = []
     for i in range(self.num_hidden):
       w_xs.append(
           nn.Dense(
               self.dim_hidden[i],
               kernel_init=self.init_fn(self.init_std),
               bias_init=initializers.constant(0.),
@@ -249,63 +267,43 @@
       sigma = jnp.sum(sigma, axis=0) / (shape[0] - 1)
       # regularize
       sigma = sigma + reg * jnp.eye(shape[1])
 
       if sqrt_inv:
         sigma_sqrt, sigma_inv_sqrt, _ = matrix_square_root.sqrtm(sigma)
         return sigma, sigma_sqrt, sigma_inv_sqrt, mu
-      else:
-        return sigma, mu
+      return sigma, mu
 
     source, target = inputs
     _, covs_sqrt, covs_inv_sqrt, mus = compute_moments(source, sqrt_inv=True)
     covt, mut = compute_moments(target, sqrt_inv=False)
 
     mo = matrix_square_root.sqrtm_only(
         jnp.dot(jnp.dot(covs_sqrt, covt), covs_sqrt)
     )
     A = jnp.dot(jnp.dot(covs_inv_sqrt, mo), covs_inv_sqrt)
     b = jnp.squeeze(mus) - jnp.linalg.solve(A, jnp.squeeze(mut))
     A = matrix_square_root.sqrtm_only(A)
-
     return jnp.expand_dims(A, 0), jnp.expand_dims(b, 0)
 
   @staticmethod
   def _compute_identity_map(input_dim: int) -> Tuple[jnp.ndarray, jnp.ndarray]:
     A = jnp.eye(input_dim).reshape((1, input_dim, input_dim))
     b = jnp.zeros((1, input_dim))
-
     return A, b
 
   @nn.compact
-  def __call__(self, x: jnp.ndarray) -> float:
+  def __call__(self, x: jnp.ndarray) -> float:  # noqa: D102
     z = self.act_fn(self.w_xs[0](x))
     for i in range(self.num_hidden):
       z = jnp.add(self.w_zs[i](z), self.w_xs[i + 1](x))
       z = self.act_fn(z)
     z += self.pos_def_potential(x)
     return z.squeeze()
 
-  def create_train_state(
-      self,
-      rng: jnp.ndarray,
-      optimizer: optax.OptState,
-      input: Union[int, Tuple[int, ...]],
-      params: Optional[frozen_dict.FrozenDict[str, jnp.ndarray]] = None,
-  ) -> NeuralTrainState:
-    """Create initial `TrainState`."""
-    params = self.init(rng, jnp.ones(input))["params"]
-    return NeuralTrainState.create(
-        apply_fn=self.apply,
-        params=params,
-        tx=optimizer,
-        potential_value_fn=self.potential_value_fn,
-        potential_gradient_fn=self.potential_gradient_fn,
-    )
-
 
 class MLP(ModelBase):
   """A non-convex MLP.
 
   Args:
     dim_hidden: sequence specifying size of hidden dimensions. The output
       dimension of the last layer is automatically set to 1 if
@@ -316,15 +314,15 @@
   """
 
   dim_hidden: Sequence[int]
   is_potential: bool = True
   act_fn: Callable[[jnp.ndarray], jnp.ndarray] = nn.leaky_relu
 
   @nn.compact
-  def __call__(self, x: jnp.ndarray) -> jnp.ndarray:
+  def __call__(self, x: jnp.ndarray) -> jnp.ndarray:  # noqa: D102
     squeeze = x.ndim == 1
     if squeeze:
       x = jnp.expand_dims(x, 0)
     assert x.ndim == 2, x.ndim
     n_input = x.shape[-1]
 
     z = x
@@ -339,25 +337,7 @@
       quad_term = 0.5 * jax.vmap(jnp.dot)(x, x)
       z += quad_term
     else:
       Wx = nn.Dense(n_input, use_bias=True)
       z = x + Wx(z)
 
     return z.squeeze(0) if squeeze else z
-
-  def create_train_state(
-      self,
-      rng: jnp.ndarray,
-      optimizer: optax.OptState,
-      input: Union[int, Tuple[int, ...]],
-      params: Optional[frozen_dict.FrozenDict[str, jnp.ndarray]] = None,
-  ) -> NeuralTrainState:
-    """Create initial `TrainState`."""
-    if params is None:
-      params = self.init(rng, jnp.ones(input))["params"]
-    return NeuralTrainState.create(
-        apply_fn=self.apply,
-        params=params,
-        tx=optimizer,
-        potential_value_fn=self.potential_value_fn,
-        potential_gradient_fn=self.potential_gradient_fn,
-    )
```

### Comparing `ott-jax-0.4.0/src/ott/solvers/nn/neuraldual.py` & `ott-jax-0.4.1/src/ott/solvers/nn/neuraldual.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,38 @@
+# Copyright OTT-JAX
+#
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""A Jax implementation of the neural-based Kantorovich dual."""
-
 import warnings
-from typing import Callable, Dict, Iterable, List, Literal, Optional, Tuple, Union
+from typing import (
+    Callable,
+    Dict,
+    Iterator,
+    List,
+    Literal,
+    Optional,
+    Tuple,
+    Union,
+)
 
 import jax
 import jax.numpy as jnp
 import optax
 from flax import core
-from flax.core import frozen_dict
 
+from ott import utils
 from ott.geometry import costs
 from ott.problems.linear import potentials
 from ott.solvers.nn import conjugate_solvers, models
 
 __all__ = ["W2NeuralDual"]
 
 Train_t = Dict[Literal["train_logs", "valid_logs"], Dict[str, List[float]]]
@@ -31,34 +40,29 @@
 Conj_t = Optional[conjugate_solvers.FenchelConjugateSolver]
 
 
 class W2NeuralDual:
   r"""Solver for the Wasserstein-2 Kantorovich dual between Euclidean spaces.
 
   Learn the Wasserstein-2 optimal transport between two measures
-  :math:`\alpha` and :math:`\beta` in
-  :math:`n`-dimensional Euclidean space,
-  denoted source and target, respectively.
-  This is achieved by parameterizing a Kantorovich potential
-  :math:`f_\theta: \mathbb{R}^n\rightarrow\mathbb{R}`
-  associated with the :math:`\alpha` measure with
-  an :class:`~ott.solvers.nn.models.ICNN`,
-  :class:`~ott.solvers.nn.models.MLP`, or other
-  :class:`~ott.solvers.nn.models.ModelBase`, where
-  :math:`\nabla f` transports source to target cells.
-  This potential is learned by optimizing the dual
-  form associated with the negative inner product cost
+  :math:`\alpha` and :math:`\beta` in :math:`n`-dimensional Euclidean space,
+  denoted source and target, respectively. This is achieved by parameterizing
+  a Kantorovich potential :math:`f_\theta: \mathbb{R}^n\rightarrow\mathbb{R}`
+  associated with the :math:`\alpha` measure with an
+  :class:`~ott.solvers.nn.models.ICNN`, :class:`~ott.solvers.nn.models.MLP`,
+  or other :class:`~ott.solvers.nn.models.ModelBase`, where :math:`\nabla f`
+  transports source to target cells. This potential is learned by optimizing
+  the dual form associated with the negative inner product cost
 
   .. math::
 
     \text{argsup}_{\theta}\; -\mathbb{E}_{x\sim\alpha}[f_\theta(x)] -
       \mathbb{E}_{y\sim\beta}[f^\star_\theta(y)],
 
-  where
-  :math:`f^\star(y) := -\inf_{x\in\mathbb{R}^n} f(x)-\langle x, y\rangle`
+  where :math:`f^\star(y) := -\inf_{x\in\mathbb{R}^n} f(x)-\langle x, y\rangle`
   is the convex conjugate.
   :math:`\nabla f^\star` transports from the target
   to source cells and provides the inverse optimal
   transport map from :math:`\beta` to :math:`\alpha`.
   This solver estimates the conjugate :math:`f^\star`
   with a neural approximation :math:`g` that is fine-tuned
   with :class:`~ott.solvers.nn.conjugate_solvers.FenchelConjugateSolver`,
@@ -74,33 +78,34 @@
 
   The potential's value or gradient mapping is specified via
   :attr:`~ott.solvers.nn.models.ModelBase.is_potential`.
 
   Args:
     dim_data: input dimensionality of data required for network init
     neural_f: network architecture for potential :math:`f`.
-    neural_g: network architecture for the conjugate potential :math:`g\approx f^\star`
+    neural_g: network architecture for the conjugate potential
+      :math:`g\approx f^\star`
     optimizer_f: optimizer function for potential :math:`f`
     optimizer_g: optimizer function for the conjugate potential :math:`g`
     num_train_iters: number of total training iterations
-    num_inner_iters: number of training iterations of :math:`g` per iteration of :math:`f`
-    back_and_forth: alternate between updating the forward and backward directions.
-      Inspired from :cite:`jacobs:20`
+    num_inner_iters: number of training iterations of :math:`g` per iteration
+      of :math:`f`
+    back_and_forth: alternate between updating the forward and backward
+      directions. Inspired from :cite:`jacobs:20`
     valid_freq: frequency with which model is validated
     log_freq: frequency with training and validation are logged
     logging: option to return logs
-    seed: random seed for network initializations
+    rng: random key used for seeding for network initializations
     pos_weights: option to train networks with positive weights or regularizer
     beta: regularization parameter when not training with positive weights
     conjugate_solver: numerical solver for the Fenchel conjugate.
-    amortization_loss: amortization loss for the conjugate :math:`g\approx f^\star`.
-      Options are 'objective' :cite:`makkuva:20` or 'regression' :cite:`amos:23`.
+    amortization_loss: amortization loss for the conjugate
+      :math:`g\approx f^\star`. Options are `'objective'` :cite:`makkuva:20` or
+      `'regression'` :cite:`amos:23`.
     parallel_updates: Update :math:`f` and :math:`g` at the same time
-    init_f_params: initial parameters for :math:`f`
-    init_g_params: initial parameters for :math:`g`
   """
 
   def __init__(
       self,
       dim_data: int,
       neural_f: Optional[models.ModelBase] = None,
       neural_g: Optional[models.ModelBase] = None,
@@ -108,38 +113,33 @@
       optimizer_g: Optional[optax.OptState] = None,
       num_train_iters: int = 20000,
       num_inner_iters: int = 1,
       back_and_forth: Optional[bool] = None,
       valid_freq: int = 1000,
       log_freq: int = 1000,
       logging: bool = False,
-      seed: int = 0,
+      rng: Optional[jax.random.PRNGKeyArray] = None,
       pos_weights: bool = True,
       beta: float = 1.0,
       conjugate_solver: Conj_t = conjugate_solvers.DEFAULT_CONJUGATE_SOLVER,
-      amortization_loss: Literal['objective', 'regression'] = 'regression',
+      amortization_loss: Literal["objective", "regression"] = "regression",
       parallel_updates: bool = True,
-      init_f_params: Optional[frozen_dict.FrozenDict[str, jnp.ndarray]] = None,
-      init_g_params: Optional[frozen_dict.FrozenDict[str, jnp.ndarray]] = None,
   ):
     self.num_train_iters = num_train_iters
     self.num_inner_iters = num_inner_iters
     self.back_and_forth = back_and_forth
     self.valid_freq = valid_freq
     self.log_freq = log_freq
     self.logging = logging
     self.pos_weights = pos_weights
     self.beta = beta
     self.parallel_updates = parallel_updates
     self.conjugate_solver = conjugate_solver
     self.amortization_loss = amortization_loss
 
-    # set random key
-    rng = jax.random.PRNGKey(seed)
-
     # set default optimizers
     if optimizer_f is None:
       optimizer_f = optax.adam(learning_rate=0.0001, b1=0.5, b2=0.9, eps=1e-8)
     if optimizer_g is None:
       optimizer_g = optax.adam(learning_rate=0.0001, b1=0.5, b2=0.9, eps=1e-8)
 
     # set default neural architectures
@@ -148,51 +148,61 @@
     if neural_g is None:
       neural_g = models.ICNN(dim_data=dim_data, dim_hidden=[64, 64, 64, 64])
     self.neural_f = neural_f
     self.neural_g = neural_g
 
     # set optimizer and networks
     self.setup(
-        rng, neural_f, neural_g, dim_data, optimizer_f, optimizer_g,
-        init_f_params, init_g_params
+        utils.default_prng_key(rng),
+        neural_f,
+        neural_g,
+        dim_data,
+        optimizer_f,
+        optimizer_g,
     )
 
   def setup(
-      self, rng: jnp.ndarray, neural_f: models.ModelBase,
-      neural_g: models.ModelBase, dim_data: int, optimizer_f: optax.OptState,
+      self,
+      rng: jax.random.PRNGKeyArray,
+      neural_f: models.ModelBase,
+      neural_g: models.ModelBase,
+      dim_data: int,
+      optimizer_f: optax.OptState,
       optimizer_g: optax.OptState,
-      init_f_params: Optional[frozen_dict.FrozenDict[str, jnp.ndarray]],
-      init_g_params: Optional[frozen_dict.FrozenDict[str, jnp.ndarray]]
   ) -> None:
     """Setup all components required to train the network."""
-    # split random key
+    # split random number generator
     rng, rng_f, rng_g = jax.random.split(rng, 3)
 
     # check setting of network architectures
     warn_str = f"Setting of ICNN and the positive weights setting of the " \
         f"`W2NeuralDual` are not consistent. Proceeding with " \
         f"the `W2NeuralDual` setting, with positive weights " \
         f"being {self.pos_weights}."
     if isinstance(
         neural_f, models.ICNN
     ) and neural_f.pos_weights is not self.pos_weights:
-      warnings.warn(warn_str)
+      warnings.warn(warn_str, stacklevel=2)
       neural_f.pos_weights = self.pos_weights
 
     if isinstance(
         neural_g, models.ICNN
     ) and neural_g.pos_weights is not self.pos_weights:
-      warnings.warn(warn_str)
+      warnings.warn(warn_str, stacklevel=2)
       neural_g.pos_weights = self.pos_weights
 
     self.state_f = neural_f.create_train_state(
-        rng_f, optimizer_f, dim_data, init_f_params
+        rng_f,
+        optimizer_f,
+        dim_data,
     )
     self.state_g = neural_g.create_train_state(
-        rng_g, optimizer_g, dim_data, init_g_params
+        rng_g,
+        optimizer_g,
+        dim_data,
     )
 
     # default to using back_and_forth with the non-convex models
     if self.back_and_forth is None:
       self.back_and_forth = isinstance(neural_f, models.MLP)
 
     if self.num_inner_iters == 1 and self.parallel_updates:
@@ -202,32 +212,34 @@
       self.valid_step_parallel = self.get_step_fn(
           train=False, to_optimize="both"
       )
       self.train_fn = self.train_neuraldual_parallel
     else:
       if self.parallel_updates:
         warnings.warn(
-            'parallel_updates set to True but disabling it because num_inner_iters>1'
+            "parallel_updates set to True but disabling it "
+            "because num_inner_iters>1",
+            stacklevel=2
         )
       if self.back_and_forth:
         raise NotImplementedError(
             "back_and_forth not implemented without parallel updates"
         )
       self.train_step_f = self.get_step_fn(train=True, to_optimize="f")
       self.valid_step_f = self.get_step_fn(train=False, to_optimize="f")
       self.train_step_g = self.get_step_fn(train=True, to_optimize="g")
       self.valid_step_g = self.get_step_fn(train=False, to_optimize="g")
       self.train_fn = self.train_neuraldual_alternating
 
-  def __call__(
+  def __call__(  # noqa: D102
       self,
-      trainloader_source: Iterable[jnp.ndarray],
-      trainloader_target: Iterable[jnp.ndarray],
-      validloader_source: Iterable[jnp.ndarray],
-      validloader_target: Iterable[jnp.ndarray],
+      trainloader_source: Iterator[jnp.ndarray],
+      trainloader_target: Iterator[jnp.ndarray],
+      validloader_source: Iterator[jnp.ndarray],
+      validloader_target: Iterator[jnp.ndarray],
       callback: Optional[Callback_t] = None,
   ) -> Union[potentials.DualPotentials, Tuple[potentials.DualPotentials,
                                               Train_t]]:
     logs = self.train_fn(
         trainloader_source,
         trainloader_target,
         validloader_source,
@@ -236,56 +248,57 @@
     )
     res = self.to_dual_potentials()
 
     return (res, logs) if self.logging else res
 
   def train_neuraldual_parallel(
       self,
-      trainloader_source: Iterable[jnp.ndarray],
-      trainloader_target: Iterable[jnp.ndarray],
-      validloader_source: Iterable[jnp.ndarray],
-      validloader_target: Iterable[jnp.ndarray],
+      trainloader_source: Iterator[jnp.ndarray],
+      trainloader_target: Iterator[jnp.ndarray],
+      validloader_source: Iterator[jnp.ndarray],
+      validloader_target: Iterator[jnp.ndarray],
       callback: Optional[Callback_t] = None,
   ) -> Train_t:
-    """Implementation of the training and validation with parallel updates."""  # noqa: D401
+    """Training and validation with parallel updates."""
     try:
       from tqdm.auto import tqdm
     except ImportError:
       tqdm = lambda _: _
     # define dict to contain source and target batch
-    train_batch = {}
-    valid_batch = {}
+    train_batch, valid_batch = {}, {}
 
     # set logging dictionaries
     train_logs = {"loss_f": [], "loss_g": [], "w_dist": [], "directions": []}
     valid_logs = {"loss_f": [], "loss_g": [], "w_dist": []}
 
     for step in tqdm(range(self.num_train_iters)):
       update_forward = not self.back_and_forth or step % 2 == 0
       if update_forward:
         train_batch["source"] = jnp.asarray(next(trainloader_source))
         train_batch["target"] = jnp.asarray(next(trainloader_target))
-        self.state_f, self.state_g, loss, loss_f, loss_g, w_dist = self.train_step_parallel(
-            self.state_f,
-            self.state_g,
-            train_batch,
-        )
+        (self.state_f, self.state_g, loss, loss_f, loss_g,
+         w_dist) = self.train_step_parallel(
+             self.state_f,
+             self.state_g,
+             train_batch,
+         )
       else:
         train_batch["target"] = jnp.asarray(next(trainloader_source))
         train_batch["source"] = jnp.asarray(next(trainloader_target))
-        self.state_g, self.state_f, loss, loss_f, loss_g, w_dist = self.train_step_parallel(
-            self.state_g,
-            self.state_f,
-            train_batch,
-        )
+        (self.state_g, self.state_f, loss, loss_f, loss_g,
+         w_dist) = self.train_step_parallel(
+             self.state_g,
+             self.state_f,
+             train_batch,
+         )
 
       if self.logging and step % self.log_freq == 0:
         self._update_logs(train_logs, loss_f, loss_g, w_dist)
         train_logs["directions"].append(
-            'forward' if update_forward else 'backward'
+            "forward" if update_forward else "backward"
         )
 
       if callback is not None:
         _ = callback(step, self.to_dual_potentials())
 
       if not self.pos_weights:
         # Only clip the weights of the f network
@@ -310,29 +323,27 @@
               valid_logs, valid_loss_f, valid_loss_g, valid_w_dist
           )
 
     return {"train_logs": train_logs, "valid_logs": valid_logs}
 
   def train_neuraldual_alternating(
       self,
-      trainloader_source: Iterable[jnp.ndarray],
-      trainloader_target: Iterable[jnp.ndarray],
-      validloader_source: Iterable[jnp.ndarray],
-      validloader_target: Iterable[jnp.ndarray],
+      trainloader_source: Iterator[jnp.ndarray],
+      trainloader_target: Iterator[jnp.ndarray],
+      validloader_source: Iterator[jnp.ndarray],
+      validloader_target: Iterator[jnp.ndarray],
       callback: Optional[Callback_t] = None,
   ) -> Train_t:
-    """Implementation of the training and validation with alternating updates."""  # noqa: D401
+    """Training and validation with alternating updates."""
     try:
       from tqdm.auto import tqdm
     except ImportError:
       tqdm = lambda _: _
     # define dict to contain source and target batch
-    batch_g = {}
-    batch_f = {}
-    valid_batch = {}
+    batch_g, batch_f, valid_batch = {}, {}, {}
 
     # set logging dictionaries
     train_logs = {"loss_f": [], "loss_g": [], "w_dist": []}
     valid_logs = {"loss_f": [], "loss_g": [], "w_dist": []}
 
     for step in tqdm(range(self.num_train_iters)):
       # execute training steps
@@ -360,15 +371,15 @@
 
       if callback is not None:
         callback(step, self.to_dual_potentials())
 
       if self.logging and step % self.log_freq == 0:
         self._update_logs(train_logs, loss_f, loss_g, w_dist)
 
-      # report the loss on an validuation dataset periodically
+      # report the loss on validation dataset periodically
       if step != 0 and step % self.valid_freq == 0:
         # get batch
         valid_batch["source"] = jnp.asarray(next(validloader_source))
         valid_batch["target"] = jnp.asarray(next(validloader_target))
 
         valid_loss_f, _ = self.valid_step_f(
             self.state_f, self.state_g, valid_batch
@@ -381,15 +392,15 @@
           self._update_logs(
               valid_logs, valid_loss_f, valid_loss_g, valid_w_dist
           )
 
     return {"train_logs": train_logs, "valid_logs": valid_logs}
 
   def get_step_fn(
-      self, train: bool, to_optimize: Literal["f", "g", "parallel"]
+      self, train: bool, to_optimize: Literal["f", "g", "parallel", "both"]
   ):
     """Create a parallel training and evaluation function."""
 
     def loss_fn(params_f, params_g, f_value, g_value, g_gradient, batch):
       """Loss function for both potentials."""
       # get two distributions
       source, target = batch["source"], batch["target"]
@@ -417,19 +428,19 @@
       f_source = f_value_partial(source)
       f_star_target = batch_dot(source_hat_detach,
                                 target) - f_value_partial(source_hat_detach)
       dual_source = f_source.mean()
       dual_target = f_star_target.mean()
       dual_loss = dual_source + dual_target
 
-      if self.amortization_loss == 'regression':
+      if self.amortization_loss == "regression":
         amor_loss = ((init_source_hat - source_hat_detach) ** 2).mean()
-      elif self.amortization_loss == 'objective':
-        f_value_parameters_detached = lambda x: f_value(
-            jax.lax.stop_gradient(params_f), x
+      elif self.amortization_loss == "objective":
+        f_value_parameters_detached = f_value(
+            jax.lax.stop_gradient(params_f), g_value_partial
         )
         amor_loss = (
             f_value_parameters_detached(init_source_hat) -
             batch_dot(init_source_hat, target)
         ).mean()
       else:
         raise ValueError("Amortization loss has been misspecified.")
@@ -470,87 +481,83 @@
             state_f.params,
             state_g.params,
             state_f.potential_value_fn,
             state_g.potential_value_fn,
             state_g.potential_gradient_fn,
             batch,
         )
-
         # update state
         if to_optimize == "both":
-          return state_f.apply_gradients(grads=grads_f), \
-              state_g.apply_gradients(grads=grads_g), \
-              loss, loss_f, loss_g, W2_dist
-        elif to_optimize == "f":
-          return state_f.apply_gradients(grads=grads_f), \
-              loss_f, W2_dist
-        elif to_optimize == "g":
-          return state_g.apply_gradients(grads=grads_g), \
-              loss_g, W2_dist
-        else:
-          raise ValueError("Optimization target has been misspecified.")
-
-      else:
-        # compute loss and gradients
-        (loss, (loss_f, loss_g, W2_dist)), (grads_f, grads_g) = grad_fn(
-            state_f.params,
-            state_g.params,
-            state_f.potential_value_fn,
-            state_g.potential_value_fn,
-            state_g.potential_gradient_fn,
-            batch,
-        )
+          return (
+              state_f.apply_gradients(grads=grads_f),
+              state_g.apply_gradients(grads=grads_g), loss, loss_f, loss_g,
+              W2_dist
+          )
+        if to_optimize == "f":
+          return state_f.apply_gradients(grads=grads_f), loss_f, W2_dist
+        if to_optimize == "g":
+          return state_g.apply_gradients(grads=grads_g), loss_g, W2_dist
+        raise ValueError("Optimization target has been misspecified.")
+
+      # compute loss and gradients
+      (loss, (loss_f, loss_g, W2_dist)), _ = grad_fn(
+          state_f.params,
+          state_g.params,
+          state_f.potential_value_fn,
+          state_g.potential_value_fn,
+          state_g.potential_gradient_fn,
+          batch,
+      )
 
-        # do not update state
-        if to_optimize == "both":
-          return loss_f, loss_g, W2_dist
-        elif to_optimize == "f":
-          return loss_f, W2_dist
-        elif to_optimize == "g":
-          return loss_g, W2_dist
-        else:
-          raise ValueError("Optimization target has been misspecified.")
+      # do not update state
+      if to_optimize == "both":
+        return loss_f, loss_g, W2_dist
+      if to_optimize == "f":
+        return loss_f, W2_dist
+      if to_optimize == "g":
+        return loss_g, W2_dist
+      raise ValueError("Optimization target has been misspecified.")
 
     return step_fn
 
   def to_dual_potentials(
       self, finetune_g: bool = True
   ) -> potentials.DualPotentials:
     r"""Return the Kantorovich dual potentials from the trained potentials.
 
     Args:
-      finetune_g: Run the conjugate solver to finetune the prediction.
+      finetune_g: Run the conjugate solver to fine-tune the prediction.
 
     Returns:
       A dual potential object
     """
     f_value = self.state_f.potential_value_fn(self.state_f.params)
     g_value_prediction = self.state_g.potential_value_fn(
         self.state_g.params, f_value
     )
 
     def g_value_finetuned(y: jnp.ndarray) -> jnp.ndarray:
       x_hat = jax.grad(g_value_prediction)(y)
       grad_g_y = jax.lax.stop_gradient(
           self.conjugate_solver.solve(f_value, y, x_init=x_hat).grad
       )
-      g_y = -f_value(grad_g_y) + jnp.dot(grad_g_y, y)
-      return g_y
+      return -f_value(grad_g_y) + jnp.dot(grad_g_y, y)
 
     return potentials.DualPotentials(
         f=f_value,
-        g=g_value_prediction if not finetune_g else g_value_finetuned,
+        g=g_value_prediction if not finetune_g or self.conjugate_solver is None
+        else g_value_finetuned,
         cost_fn=costs.SqEuclidean(),
         corr=True
     )
 
   @staticmethod
   def _clip_weights_icnn(params):
     params = params.unfreeze()
-    for k in params.keys():
+    for k in params:
       if k.startswith("w_z"):
         params[k]["kernel"] = jnp.clip(params[k]["kernel"], a_min=0)
 
     return core.freeze(params)
 
   @staticmethod
   def _penalize_weights_icnn(params: Dict[str, jnp.ndarray]) -> float:
@@ -558,15 +565,15 @@
     for k, param in params.items():
       if k.startswith("w_z"):
         penalty += jnp.linalg.norm(jax.nn.relu(-param["kernel"]))
     return penalty
 
   @staticmethod
   def _update_logs(
-      logs: Dict[str, Union[float, str]],
+      logs: Dict[str, List[Union[float, str]]],
       loss_f: jnp.ndarray,
       loss_g: jnp.ndarray,
       w_dist: jnp.ndarray,
   ) -> None:
     logs["loss_f"].append(float(loss_f))
     logs["loss_g"].append(float(loss_g))
     logs["w_dist"].append(float(w_dist))
```

### Comparing `ott-jax-0.4.0/src/ott/solvers/quadratic/gromov_wasserstein.py` & `ott-jax-0.4.1/src/ott/solvers/quadratic/gromov_wasserstein.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,59 +1,65 @@
-# Copyright 2022 Google LLC.
+# Copyright OTT-JAX
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-#     http://www.apache.org/licenses/LICENSE-2.0
+#   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""A Jax version of the regularised GW Solver (Peyre et al. 2016)."""
 from typing import (
     Any,
+    Callable,
     Dict,
     Literal,
     Mapping,
     NamedTuple,
     Optional,
     Sequence,
     Tuple,
     Union,
 )
 
 import jax
 import jax.numpy as jnp
+import numpy as np
+from jax.experimental import host_callback
 
+from ott import utils
 from ott.geometry import geometry, low_rank, pointcloud
 from ott.initializers.linear import initializers_lr
 from ott.initializers.quadratic import initializers as quad_initializers
 from ott.math import fixed_point_loop
 from ott.problems.linear import linear_problem
 from ott.problems.quadratic import quadratic_costs, quadratic_problem
 from ott.solvers import was_solver
 from ott.solvers.linear import sinkhorn, sinkhorn_lr
 
 __all__ = ["GWOutput", "GromovWasserstein", "solve"]
 
 LinearOutput = Union[sinkhorn.SinkhornOutput, sinkhorn_lr.LRSinkhornOutput]
 
+ProgressCallbackFn_t = Callable[
+    [Tuple[np.ndarray, np.ndarray, np.ndarray, "GWState"]], None]
+
 
 class GWOutput(NamedTuple):
   """Holds the output of the Gromov-Wasserstein solver.
 
   Args:
     costs: Holds the sequence of regularized GW costs seen through the outer
       loop of the solver.
     linear_convergence: Holds the sequence of bool convergence flags of the
       inner Sinkhorn iterations.
-    converged: Bool convergence flag for the outer GW iterations.
+    converged: Convergence flag for the outer GW iterations.
     errors: Holds sequence of vectors of errors of the Sinkhorn algorithm
       at each iteration.
     linear_state: State used to solve and store solutions to the local
       linearization of GW.
     geom: The geometry underlying the local linearization.
     old_transport_mass: Holds total mass of transport at previous iteration.
   """
@@ -63,15 +69,15 @@
   converged: bool = False
   errors: Optional[jnp.ndarray] = None
   linear_state: Optional[LinearOutput] = None
   geom: Optional[geometry.Geometry] = None
   # Intermediate values.
   old_transport_mass: float = 1.0
 
-  def set(self, **kwargs: Any) -> 'GWOutput':
+  def set(self, **kwargs: Any) -> "GWOutput":
     """Return a copy of self, possibly with overwrites."""
     return self._replace(**kwargs)
 
   @property
   def matrix(self) -> jnp.ndarray:
     """Transport matrix."""
     return self._rescale_factor * self.linear_state.matrix
@@ -85,50 +91,55 @@
     """Regularized optimal transport cost of the linearization."""
     return self.linear_state.reg_ot_cost
 
   @property
   def _rescale_factor(self) -> float:
     return jnp.sqrt(self.old_transport_mass / self.linear_state.transport_mass)
 
+  @property
+  def primal_cost(self) -> float:
+    """Return transport cost of current linear OT solution at geometry."""
+    return self.linear_state.transport_cost_at_geom(other_geom=self.geom)
+
 
 class GWState(NamedTuple):
-  """Holds the state of the Gromov-Wasserstein solver.
+  """State of the Gromov-Wasserstein solver.
 
   Attributes:
     costs: Holds the sequence of regularized GW costs seen through the outer
       loop of the solver.
     linear_convergence: Holds the sequence of bool convergence flags of the
       inner Sinkhorn iterations.
     linear_state: State used to solve and store solutions to the local
       linearization of GW.
     linear_pb: Local linearization of the quadratic GW problem.
     old_transport_mass: Intermediary value of the mass of the transport matrix.
-    keys: Random keys passed to low-rank initializers at every GW iteration
+    rngs: Random keys passed to low-rank initializers at every GW iteration
       when not using warm start.
     errors: Holds sequence of vectors of errors of the Sinkhorn algorithm
       at each iteration.
   """
 
   costs: jnp.ndarray
   linear_convergence: jnp.ndarray
   linear_state: LinearOutput
   linear_pb: linear_problem.LinearProblem
   old_transport_mass: float
-  keys: Optional[jnp.ndarray] = None
+  rngs: Optional[jax.random.PRNGKeyArray] = None
   errors: Optional[jnp.ndarray] = None
 
-  def set(self, **kwargs: Any) -> 'GWState':
+  def set(self, **kwargs: Any) -> "GWState":
     """Return a copy of self, possibly with overwrites."""
     return self._replace(**kwargs)
 
-  def update(
+  def update(  # noqa: D102
       self, iteration: int, linear_sol: LinearOutput,
       linear_pb: linear_problem.LinearProblem, store_errors: bool,
       old_transport_mass: float
-  ) -> 'GWState':
+  ) -> "GWState":
     costs = self.costs.at[iteration].set(linear_sol.reg_ot_cost)
     errors = None
     if store_errors and self.errors is not None:
       errors = self.errors.at[iteration, :].set(linear_sol.errors)
     linear_convergence = self.linear_convergence.at[iteration].set(
         linear_sol.converged
     )
@@ -141,122 +152,132 @@
         errors=errors,
         old_transport_mass=old_transport_mass
     )
 
 
 @jax.tree_util.register_pytree_node_class
 class GromovWasserstein(was_solver.WassersteinSolver):
-  """Gromov-Wasserstein solver.
+  """Gromov-Wasserstein solver :cite:`peyre:16`.
 
   Args:
     args: Positional arguments for
       :class:`~ott.solvers.was_solver.WassersteinSolver`.
     warm_start: Whether to initialize (low-rank) Sinkhorn calls using values
       from the previous iteration. If `None`, warm starts are not used for
       standard Sinkhorn, but used for low-rank Sinkhorn.
+    unscale_last_linearization: Whether to remove any scaling from the
+      cost matrices of the last linearization stored in
+      :attr:`~ott.solvers.quadratic.gromov_wasserstein.GWOutput.geom`.
+      This has the practical benefit that, while the OT coupling matrices
+      obtained with GW might have been computed by re-scaling cost matrices for
+      numerical stability, the last linearization stored in the geometry will be
+      unscaled and recomputed with the original cost values.
     quad_initializer: Quadratic initializer. If the solver is entropic,
       :class:`~ott.initializers.quadratic.initializers.QuadraticInitializer`
       is always used. Otherwise, the quadratic initializer wraps the low-rank
-      Sinkhorn initializers:
-
-        - `'random'` - :class:`~ott.initializers.linear.initializers_lr.RandomInitializer`.
-        - `'rank2'` - :class:`~ott.initializers.linear.initializers_lr.Rank2Initializer`.
-        - `'k-means'` - :class:`~ott.initializers.linear.initializers_lr.KMeansInitializer`.
-        - `'generalized-k-means'` - :class:`~ott.initializers.linear.initializers_lr.GeneralizedKMeansInitializer`.
-
-      If `None`, the low-rank initializer will be selected in a problem-specific
-      manner:
-
-        - if both :attr:`~ott.problems.quadratic.quadratic_problem.QuadraticProblem.geom_xx`
-          and :attr:`~ott.problems.quadratic.quadratic_problem.QuadraticProblem.geom_yy`
-          are :class:`~ott.geometry.pointcloud.PointCloud` or :class:`~ott.geometry.low_rank.LRCGeometry`,
-          :class:`~ott.initializers.linear.initializers_lr.KMeansInitializer`
-          is used.
-        - otherwise, use :class:`~ott.initializers.linear.initializers_lr.RandomInitializer`.
-
+      Sinkhorn initializers. If `None`, the low-rank initializer will be
+      selected in a problem-specific manner. If both ``geom_xx`` and ``geom_yy``
+      are :class:`~ott.geometry.pointcloud.PointCloud` or
+      :class:`~ott.geometry.low_rank.LRCGeometry`, use
+      :class:`~ott.initializers.linear.initializers_lr.KMeansInitializer`.
+      Otherwise, use
+      :class:`~ott.initializers.linear.initializers_lr.RandomInitializer`.
+    progress_fn: callback function which gets called during the
+      Gromov-Wasserstein iterations, so the user can display the error at each
+      iteration, e.g., using a progress bar.
+      See :func:`~ott.utils.default_progress_fn` for a basic implementation.
     kwargs_init: Keyword arguments when creating the initializer.
     kwargs: Keyword arguments for
       :class:`~ott.solvers.was_solver.WassersteinSolver`.
   """
 
   def __init__(
       self,
       *args: Any,
       warm_start: Optional[bool] = None,
+      unscale_last_linearization: bool = False,
       quad_initializer: Optional[
           Union[Literal["random", "rank2", "k-means", "generalized-k-means"],
                 quad_initializers.BaseQuadraticInitializer]] = None,
+      progress_fn: Optional[ProgressCallbackFn_t] = None,
       kwargs_init: Optional[Mapping[str, Any]] = None,
       **kwargs: Any
   ):
     super().__init__(*args, **kwargs)
     self._warm_start = warm_start
+    self.unscale_last_linearization = unscale_last_linearization
     self.quad_initializer = quad_initializer
+    self.progress_fn = progress_fn
     self.kwargs_init = {} if kwargs_init is None else kwargs_init
 
   def __call__(
       self,
       prob: quadratic_problem.QuadraticProblem,
       init: Optional[linear_problem.LinearProblem] = None,
-      key: Optional[jnp.ndarray] = None,
+      rng: Optional[jax.random.PRNGKeyArray] = None,
       **kwargs: Any,
   ) -> GWOutput:
     """Run the Gromov-Wasserstein solver.
 
     Args:
       prob: Quadratic OT problem.
       init: Initial linearization of the quadratic problem. If `None`, it will
         be computed using the initializer.
+      rng: Random number key.
       kwargs: Keyword arguments used when calling the initializer.
 
     Returns:
       The Gromov-Wasserstein output.
     """
-    if key is None:
-      key = jax.random.PRNGKey(0)
-    key1, key2 = jax.random.split(key, 2)
+    rng = utils.default_prng_key(rng)
+    rng1, rng2 = jax.random.split(rng, 2)
 
     if prob._is_low_rank_convertible:
       prob = prob.to_low_rank()
 
     if init is None:
       initializer = self.create_initializer(prob)
-      init = initializer(prob, epsilon=self.epsilon, key=key1, **kwargs)
+      init = initializer(prob, epsilon=self.epsilon, rng=rng1, **kwargs)
 
-    run_fn = jax.jit(iterations) if self.jit else iterations
-    out = run_fn(self, prob, init, key2)
-    # TODO(lpapaxanthos): remove stop_gradient when using backprop
+    out = iterations(self, prob, init, rng2)
+    # TODO(lpapaxanthoos): remove stop_gradient when using backprop
     if self.is_low_rank:
       linearization = prob.update_lr_linearization(
-          jax.lax.stop_gradient(out.linear_state)
+          jax.lax.stop_gradient(out.linear_state),
+          remove_scale=self.unscale_last_linearization
       )
     else:
       linearization = prob.update_linearization(
-          jax.lax.stop_gradient(out.linear_state), self.epsilon,
-          jax.lax.stop_gradient(out.old_transport_mass)
+          jax.lax.stop_gradient(out.linear_state),
+          epsilon=self.epsilon,
+          old_transport_mass=jax.lax.stop_gradient(out.old_transport_mass),
+          remove_scale=self.unscale_last_linearization,
       )
+
     linear_state = out.linear_state.set_cost(linearization, True, True)
     iteration = jnp.sum(out.costs != -1)
     converged = jnp.logical_and(
         iteration < self.max_iterations, jnp.all(out.linear_convergence)
     )
-    return out.set(linear_state=linear_state, converged=converged)
+    return out.set(
+        linear_state=linear_state, geom=linearization.geom, converged=converged
+    )
 
   def init_state(
       self,
       prob: quadratic_problem.QuadraticProblem,
       init: linear_problem.LinearProblem,
-      key: jnp.ndarray,
+      rng: jax.random.PRNGKeyArray,
   ) -> GWState:
     """Initialize the state of the Gromov-Wasserstein iterations.
 
     Args:
       prob: Quadratic OT problem.
       init: Initial linearization of the quadratic problem.
-      key: Random key for low-rank initializers. Only used when
+      rng: Random key for low-rank initializers. Only used when
         :attr:`warm_start` is `False`.
 
     Returns:
       The initial Gromov-Wasserstein state.
     """
     linear_state = self.linear_ot_solver(init)
     num_iter = self.max_iterations
@@ -268,19 +289,22 @@
 
     return GWState(
         costs=-jnp.ones((num_iter,)),
         linear_convergence=-jnp.ones((num_iter,)),
         linear_state=linear_state,
         linear_pb=init,
         old_transport_mass=transport_mass,
-        keys=jax.random.split(key, num_iter),
+        rngs=jax.random.split(rng, num_iter),
         errors=errors,
     )
 
-  def output_from_state(self, state: GWState) -> GWOutput:
+  def output_from_state(
+      self,
+      state: GWState,
+  ) -> GWOutput:
     """Create an output from a loop state.
 
     Arguments:
       state: A GWState.
 
     Returns:
       A GWOutput.
@@ -334,27 +358,29 @@
     return quad_initializers.QuadraticInitializer(**self.kwargs_init)
 
   @property
   def warm_start(self) -> bool:
     """Whether to initialize (low-rank) Sinkhorn using previous solutions."""
     return self.is_low_rank if self._warm_start is None else self._warm_start
 
-  def tree_flatten(self) -> Tuple[Sequence[Any], Dict[str, Any]]:
+  def tree_flatten(self) -> Tuple[Sequence[Any], Dict[str, Any]]:  # noqa: D102
     children, aux_data = super().tree_flatten()
     aux_data["warm_start"] = self._warm_start
+    aux_data["progress_fn"] = self.progress_fn
+    aux_data["unscale_last_linearization"] = self.unscale_last_linearization
     aux_data["quad_initializer"] = self.quad_initializer
     aux_data["kwargs_init"] = self.kwargs_init
     return children, aux_data
 
 
 def iterations(
     solver: GromovWasserstein,
     prob: quadratic_problem.QuadraticProblem,
     init: linear_problem.LinearProblem,
-    key: jnp.ndarray,
+    rng: jax.random.PRNGKeyArray,
 ) -> GWOutput:
   """Jittable Gromov-Wasserstein outer loop."""
 
   def cond_fn(
       iteration: int, solver: GromovWasserstein, state: GWState
   ) -> bool:
     return solver._continue(state, iteration)
@@ -363,55 +389,65 @@
       iteration: int, solver: GromovWasserstein, state: GWState,
       compute_error: bool
   ) -> GWState:
     del compute_error  # always assumed true for the outer loop of GW
 
     lin_state = state.linear_state
     if solver.is_low_rank:
-      key = state.keys[iteration]
+      rng = state.rngs[iteration]
       init = (lin_state.q, lin_state.r,
               lin_state.g) if solver.warm_start else (None, None, None)
       linear_pb = prob.update_lr_linearization(state.linear_state)
-      out = solver.linear_ot_solver(linear_pb, init=init, key=key)
+      out = solver.linear_ot_solver(linear_pb, init=init, rng=rng)
     else:
       init = (lin_state.f, lin_state.g) if solver.warm_start else (None, None)
       linear_pb = prob.update_linearization(
           lin_state, solver.epsilon, state.old_transport_mass
       )
       out = solver.linear_ot_solver(linear_pb, init=init)
 
     old_transport_mass = jax.lax.stop_gradient(
         state.linear_state.transport_mass
     )
-    return state.update(
+    new_state = state.update(
         iteration, out, linear_pb, solver.store_inner_errors, old_transport_mass
     )
 
+    # Inner iterations is currently fixed to 1.
+    inner_iterations = 1
+    if solver.progress_fn is not None:
+      host_callback.id_tap(
+          solver.progress_fn,
+          (iteration, inner_iterations, solver.max_iterations, state)
+      )
+
+    return new_state
+
   state = fixed_point_loop.fixpoint_iter(
       cond_fn=cond_fn,
       body_fn=body_fn,
       min_iterations=solver.min_iterations,
       max_iterations=solver.max_iterations,
       inner_iterations=1,
       constants=solver,
-      state=solver.init_state(prob, init, key=key)
+      state=solver.init_state(prob, init, rng=rng)
   )
 
   return solver.output_from_state(state)
 
 
 def solve(
     geom_xx: geometry.Geometry,
     geom_yy: geometry.Geometry,
     geom_xy: Optional[geometry.Geometry] = None,
     fused_penalty: float = 1.0,
     scale_cost: Optional[Union[bool, float, str]] = False,
     a: Optional[jnp.ndarray] = None,
     b: Optional[jnp.ndarray] = None,
-    loss: Union[Literal['sqeucl', 'kl'], quadratic_costs.GWLoss] = 'sqeucl',
+    loss: Union[Literal["sqeucl", "kl"], quadratic_costs.GWLoss] = "sqeucl",
     tau_a: Optional[float] = 1.0,
     tau_b: Optional[float] = 1.0,
     gw_unbalanced_correction: bool = True,
     ranks: Union[int, Tuple[int, ...]] = -1,
     tolerances: Union[float, Tuple[float, ...]] = 1e-2,
     **kwargs: Any,
 ) -> GWOutput:
@@ -457,16 +493,16 @@
       computations. Alternatively, KL loss can be specified in no less optimized
       way.
     tau_a: if `< 1.0`, defines how much unbalanced the problem is on
       the first marginal.
     tau_b: if `< 1.0`, defines how much unbalanced the problem is on
       the second marginal.
     gw_unbalanced_correction: Whether the unbalanced version of
-      :cite:`sejourne:21` is used. Otherwise, ``tau_a`` and ``tau_b`` only affect
-      the inner Sinkhorn loop.
+      :cite:`sejourne:21` is used. Otherwise, ``tau_a`` and ``tau_b`` only
+      affect the inner Sinkhorn loop.
     ranks: Ranks of the cost matrices, see
       :meth:`~ott.geometry.geometry.Geometry.to_LRCGeometry`. Used when
       geometries are *not* :class:`~ott.geometry.pointcloud.PointCloud` with
       `'sqeucl'` cost function. If `-1`, the geometries will not be converted
       to low-rank. If :class:`tuple`, it specifies the ranks of ``geom_xx``,
       ``geom_yy`` and ``geom_xy``, respectively. If :class:`int`, rank is shared
       across all geometries.
```

### Comparing `ott-jax-0.4.0/src/ott/solvers/quadratic/gw_barycenter.py` & `ott-jax-0.4.1/src/ott/solvers/quadratic/gw_barycenter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,92 +1,111 @@
+# Copyright OTT-JAX
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#   http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 from functools import partial
 from typing import Any, Dict, NamedTuple, Optional, Sequence, Tuple, Union
 
 import jax
 import jax.numpy as jnp
 
+from ott import utils
 from ott.geometry import pointcloud
 from ott.math import fixed_point_loop
 from ott.problems.linear import linear_problem
 from ott.problems.quadratic import gw_barycenter
 from ott.solvers import was_solver
 from ott.solvers.quadratic import gromov_wasserstein
 
 __all__ = ["GWBarycenterState", "GromovWassersteinBarycenter"]
 
 
 class GWBarycenterState(NamedTuple):
-  """Holds the state of the \
-  :class:`~ott.problems.quadratic.gw_barycenter.GWBarycenterProblem`.
+  """State of the GW barycenter problem.
 
   Args:
-    c: Barycenter cost matrix of shape ``[bar_size, bar_size]``.
+    cost: Barycenter cost matrix of shape ``[bar_size, bar_size]``.
     x: Barycenter features of shape ``[bar_size, ndim_fused]``.
       Only used in the fused case.
     a: Weights of the barycenter of shape ``[bar_size,]``.
     errors: Array of shape
       ``[max_iter, num_measures, quad_max_iter, lin_outer_iter]`` containing
       the GW errors at each iteration.
     costs: Array of shape ``[max_iter,]`` containing the cost at each iteration.
+    costs_bary: Array of shape ``[max_iter, num_measures]`` containing the
+      cost between the individual measures and the barycenter at each iteration.
     gw_convergence: Array of shape ``[max_iter,]`` containing the convergence
       of all GW problems at each iteration.
   """
   cost: Optional[jnp.ndarray] = None
   x: Optional[jnp.ndarray] = None
   a: Optional[jnp.ndarray] = None
   errors: Optional[jnp.ndarray] = None
   costs: Optional[jnp.ndarray] = None
+  costs_bary: Optional[jnp.ndarray] = None
   gw_convergence: Optional[jnp.ndarray] = None
 
-  def set(self, **kwargs: Any) -> 'GWBarycenterState':
+  def set(self, **kwargs: Any) -> "GWBarycenterState":
     """Return a copy of self, possibly with overwrites."""
     return self._replace(**kwargs)
 
+  @property
+  def n_iters(self) -> int:
+    """Number of iterations."""
+    if self.gw_convergence is None:
+      return -1
+    return jnp.sum(self.gw_convergence > -1)
+
 
 @jax.tree_util.register_pytree_node_class
 class GromovWassersteinBarycenter(was_solver.WassersteinSolver):
-  """Gromov-Wasserstein barycenter solver of the \
-  :class:`~ott.problems.quadratic.gw_barycenter.GWBarycenterProblem`.
+  """Gromov-Wasserstein barycenter solver.
 
   Args:
-    epsilon: Entropy regulariser.
+    epsilon: Entropy regularizer.
     min_iterations: Minimum number of iterations.
     max_iterations: Maximum number of outermost iterations.
     threshold: Convergence threshold.
-    jit: Whether to jit the iteration loop.
     store_inner_errors: Whether to store the errors of the GW solver, as well
       as its linear solver, at each iteration for each measure.
     quad_solver: The GW solver.
     kwargs: Keyword argument for
       :class:`~ott.solvers.quadratic.gromov_wasserstein.GromovWasserstein`.
       Only used when ``quad_solver = None``.
   """
 
   def __init__(
       self,
       epsilon: Optional[float] = None,
       min_iterations: int = 5,
       max_iterations: int = 50,
       threshold: float = 1e-3,
-      jit: bool = True,
       store_inner_errors: bool = False,
       quad_solver: Optional[gromov_wasserstein.GromovWasserstein] = None,
       # TODO(michalk8): maintain the API compatibility with `was_solver`
       # but makes passing kwargs with the same name to `quad_solver` impossible
       # will be fixed when refactoring the solvers
       # note that `was_solver` also suffers from this
       **kwargs: Any,
   ):
     super().__init__(
         epsilon=epsilon,
         min_iterations=min_iterations,
         max_iterations=max_iterations,
         threshold=threshold,
         store_inner_errors=store_inner_errors,
-        jit=jit,
     )
     if quad_solver is None:
       kwargs["epsilon"] = epsilon
       # TODO(michalk8): store only GW errors?
       kwargs["store_inner_errors"] = store_inner_errors
       self._quad_solver = gromov_wasserstein.GromovWasserstein(**kwargs)
     else:
@@ -103,61 +122,60 @@
       bar_size: Size of the barycenter.
       kwargs: Keyword arguments for :meth:`init_state`.
 
     Returns:
       The solution.
     """
     state = self.init_state(problem, bar_size, **kwargs)
-    run_fn = jax.jit(iterations) if self.jit else iterations
-    state = run_fn(self, problem, state)
+    state = iterations(self, problem, state)
     return self.output_from_state(state)
 
   def init_state(
       self,
       problem: gw_barycenter.GWBarycenterProblem,
       bar_size: int,
       bar_init: Optional[Union[jnp.ndarray, Tuple[jnp.ndarray,
                                                   jnp.ndarray]]] = None,
       a: Optional[jnp.ndarray] = None,
-      seed: int = 0,
+      rng: Optional[jax.random.PRNGKeyArray] = None,
   ) -> GWBarycenterState:
     """Initialize the (fused) Gromov-Wasserstein barycenter state.
 
     Args:
       problem: The barycenter problem.
       bar_size: Size of the barycenter.
       bar_init: Initial barycenter value. Can be one of the following:
 
         - ``None`` - randomly initialize the barycenter.
         - :class:`jax.numpy.ndarray` - barycenter cost matrix of shape
           ``[bar_size, bar_size]``.
           Only used in the non-fused case.
-        - :class:`tuple` of :class:`jax.numpy.ndarray` - the 1st array
+        - :class:`tuple` of :class:`jax.numpy.ndarray` - the first array
           corresponds to a cost matrix of shape ``[bar_size, bar_size]``,
-          the 2nd array is a ``[bar_size, ndim_fused]`` feature matrix used in
-          the fused case.
+          the second array is a ``[bar_size, ndim_fused]`` feature matrix used
+          in the fused case.
 
       a: An array of shape ``[bar_size,]`` containing the barycenter weights.
-      seed: Random seed used when ``bar_init = None``.
+      rng: Random key for seeding used when ``bar_init = None``.
 
     Returns:
       The initial barycenter state.
     """
     if a is None:
       a = jnp.ones((bar_size,)) / bar_size
     else:
       assert a.shape == (bar_size,)
 
     if bar_init is None:
+      rng = utils.default_prng_key(rng)
       _, b = problem.segmented_y_b
-      rng = jax.random.PRNGKey(seed)
-      keys = jax.random.split(rng, problem.num_measures)
+      rngs = jax.random.split(rng, problem.num_measures)
       linear_solver = self._quad_solver.linear_ot_solver
 
-      transports = init_transports(linear_solver, keys, a, b, problem.epsilon)
+      transports = init_transports(linear_solver, rngs, a, b, problem.epsilon)
       x = problem.update_features(transports, a) if problem.is_fused else None
       cost = problem.update_barycenter(transports, a)
     else:
       cost, x = bar_init if isinstance(bar_init, tuple) else (bar_init, None)
       assert cost.shape == (bar_size, bar_size)
       if problem.is_fused:
         assert x is not None, "Barycenter features are not initialized."
@@ -170,31 +188,34 @@
           num_iter, problem.num_measures, self._quad_solver.max_iterations,
           self._quad_solver.linear_ot_solver.outer_iterations
       ))
     else:
       errors = None
 
     costs = -jnp.ones((num_iter,))
+    costs_bary = -jnp.ones((num_iter, problem.num_measures))
     gw_convergence = -jnp.ones((num_iter,))
     return GWBarycenterState(
         cost=cost,
         x=x,
         a=a,
         errors=errors,
         costs=costs,
+        costs_bary=costs_bary,
         gw_convergence=gw_convergence
     )
 
   def update_state(
       self,
       state: GWBarycenterState,
       iteration: int,
       problem: gw_barycenter.GWBarycenterProblem,
       store_errors: bool = True,
   ) -> Tuple[float, bool, jnp.ndarray, Optional[jnp.ndarray]]:
+    """Solve the (fused) Gromov-Wasserstein barycenter problem."""
 
     def solve_gw(
         state: GWBarycenterState, b: jnp.ndarray, y: jnp.ndarray,
         f: Optional[jnp.ndarray]
     ) -> Tuple[float, bool, jnp.ndarray, Optional[jnp.ndarray]]:
       quad_problem = problem._create_problem(state, y=y, b=b, f=f)
       out = self._quad_solver(quad_problem)
@@ -208,15 +229,17 @@
     solve_fn = jax.vmap(solve_gw, in_axes=in_axes)
 
     y, b = problem.segmented_y_b
     y_f = problem.segmented_y_fused
     costs, convergeds, transports, errors = solve_fn(state, b, y, y_f)
 
     cost = jnp.sum(costs * problem.weights)
+    costs_bary = state.costs_bary.at[iteration].set(costs)
     costs = state.costs.at[iteration].set(cost)
+
     converged = jnp.all(convergeds)
     gw_convergence = state.gw_convergence.at[iteration].set(converged)
 
     if self.store_inner_errors:
       errors = state.errors.at[iteration, ...].set(errors)
     else:
       errors = None
@@ -225,69 +248,70 @@
         transports, state.a
     ) if problem.is_fused else state.x
     cost = problem.update_barycenter(transports, state.a)
     return state.set(
         cost=cost,
         x=x,
         costs=costs,
+        costs_bary=costs_bary,
         errors=errors,
         gw_convergence=gw_convergence
     )
 
   def output_from_state(self, state: GWBarycenterState) -> GWBarycenterState:
     """No-op."""
     # TODO(michalk8): just for consistency with continuous barycenter
     # will be refactored in the future to create an output
     return state
 
-  def tree_flatten(self) -> Tuple[Sequence[Any], Dict[str, Any]]:
+  def tree_flatten(self) -> Tuple[Sequence[Any], Dict[str, Any]]:  # noqa: D102
     children, aux = super().tree_flatten()
     return children + [self._quad_solver], aux
 
   @classmethod
-  def tree_unflatten(
+  def tree_unflatten(  # noqa: D102
       cls, aux_data: Dict[str, Any], children: Sequence[Any]
   ) -> "GromovWassersteinBarycenter":
     epsilon, _, threshold, quad_solver = children
     return cls(
         epsilon=epsilon,
         threshold=threshold,
         quad_solver=quad_solver,
         **aux_data,
     )
 
 
 @partial(jax.vmap, in_axes=[None, 0, None, 0, None])
 def init_transports(
-    solver, key: jnp.ndarray, a: jnp.ndarray, b: jnp.ndarray,
+    solver, rng: jax.random.PRNGKeyArray, a: jnp.ndarray, b: jnp.ndarray,
     epsilon: Optional[float]
 ) -> jnp.ndarray:
   """Initialize random 2D point cloud and solve the linear OT problem.
 
   Args:
     solver: Linear OT solver.
-    key: Random key.
+    rng: Random key for seeding.
     a: Source marginals (e.g., for barycenter) of shape ``[bar_size,]``.
     b: Target marginals of shape ``[max_measure_size,]``.
     epsilon: Entropy regularization.
 
   Returns:
     Transport map of shape ``[bar_size, max_measure_size]``.
   """
-  key1, key2 = jax.random.split(key, 2)
-  x = jax.random.normal(key1, shape=(len(a), 2))
-  y = jax.random.normal(key2, shape=(len(b), 2))
+  rng1, rng2 = jax.random.split(rng, 2)
+  x = jax.random.normal(rng1, shape=(len(a), 2))
+  y = jax.random.normal(rng2, shape=(len(b), 2))
   geom = pointcloud.PointCloud(
       x, y, epsilon=epsilon, src_mask=a > 0, tgt_mask=b > 0
   )
   problem = linear_problem.LinearProblem(geom, a=a, b=b)
   return solver(problem).matrix
 
 
-def iterations(
+def iterations(  # noqa: D103
     solver: GromovWassersteinBarycenter,
     problem: gw_barycenter.GWBarycenterProblem, init_state: GWBarycenterState
 ) -> GWBarycenterState:
 
   def cond_fn(
       iteration: int, constants: GromovWassersteinBarycenter,
       state: GWBarycenterState
@@ -300,17 +324,16 @@
                                   gw_barycenter.GWBarycenterProblem],
       state: GWBarycenterState, compute_error: bool
   ) -> GWBarycenterState:
     del compute_error  # always assumed true
     solver, problem = constants
     return solver.update_state(state, iteration, problem)
 
-  state = fixed_point_loop.fixpoint_iter(
+  return fixed_point_loop.fixpoint_iter(
       cond_fn=cond_fn,
       body_fn=body_fn,
       min_iterations=solver.min_iterations,
       max_iterations=solver.max_iterations,
       inner_iterations=1,
       constants=(solver, problem),
       state=init_state,
   )
-  return state
```

### Comparing `ott-jax-0.4.0/src/ott/solvers/was_solver.py` & `ott-jax-0.4.1/src/ott/solvers/was_solver.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,50 +1,48 @@
-# Copyright 2022 Apple Inc.
+# Copyright OTT-JAX
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-#     http://www.apache.org/licenses/LICENSE-2.0
+#   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""A Jax version of the regularised GW Solver (Peyre et al. 2016)."""
 from typing import TYPE_CHECKING, Any, Dict, Optional, Sequence, Tuple, Union
 
 import jax
 import jax.numpy as jnp
 
 if TYPE_CHECKING:
   from ott.solvers.linear import continuous_barycenter, sinkhorn, sinkhorn_lr
 
 __all__ = ["WassersteinSolver"]
 
 State = Union["sinkhorn.SinkhornState", "sinkhorn_lr.LRSinkhornState",
-              "continuous_barycenter.BarycenterState"]
+              "continuous_barycenter.FreeBarycenterState"]
 
 
 # TODO(michalk8): refactor to have generic nested solver API
 @jax.tree_util.register_pytree_node_class
 class WassersteinSolver:
-  """A generic solver for problems that use a linear reg-OT pb in inner loop."""
+  """A generic solver for problems that use a linear problem in inner loop."""
 
   def __init__(
       self,
       epsilon: Optional[float] = None,
       rank: int = -1,
       linear_ot_solver: Optional[Union["sinkhorn.Sinkhorn",
                                        "sinkhorn_lr.LRSinkhorn"]] = None,
       min_iterations: int = 5,
       max_iterations: int = 50,
       threshold: float = 1e-3,
-      jit: bool = True,
       store_inner_errors: bool = False,
       **kwargs: Any,
   ):
     from ott.solvers.linear import sinkhorn, sinkhorn_lr
     default_epsilon = 1.0
     # Set epsilon value to default if needed, but keep track of whether None was
     # passed to handle the case where a linear_ot_solver is passed or not.
@@ -70,35 +68,33 @@
         # but rather added back to the Geometry object re-instantiated
         # when linearizing the problem. Therefore, no need to pass it to solver.
         self.linear_ot_solver = sinkhorn.Sinkhorn(**kwargs)
 
     self.min_iterations = min_iterations
     self.max_iterations = max_iterations
     self.threshold = threshold
-    self.jit = jit
     self.store_inner_errors = store_inner_errors
     self._kwargs = kwargs
 
   @property
   def is_low_rank(self) -> bool:
     """Whether the solver is low-rank."""
     return self.rank > 0
 
-  def tree_flatten(self) -> Tuple[Sequence[Any], Dict[str, Any]]:
+  def tree_flatten(self) -> Tuple[Sequence[Any], Dict[str, Any]]:  # noqa: D102
     return ([self.epsilon, self.linear_ot_solver, self.threshold], {
         "min_iterations": self.min_iterations,
         "max_iterations": self.max_iterations,
         "rank": self.rank,
-        "jit": self.jit,
         "store_inner_errors": self.store_inner_errors,
         **self._kwargs
     })
 
   @classmethod
-  def tree_unflatten(
+  def tree_unflatten(  # noqa: D102
       cls, aux_data: Dict[str, Any], children: Sequence[Any]
   ) -> "WassersteinSolver":
     epsilon, linear_ot_solver, threshold = children
     return cls(
         epsilon=epsilon,
         linear_ot_solver=linear_ot_solver,
         threshold=threshold,
```

### Comparing `ott-jax-0.4.0/src/ott/tools/__init__.py` & `ott-jax-0.4.1/src/ott/problems/nn/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-# Copyright 2022 Google LLC.
+# Copyright OTT-JAX
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-#     http://www.apache.org/licenses/LICENSE-2.0
+#   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from . import gaussian_mixture, k_means, plot, sinkhorn_divergence, soft_sort
+from . import dataset
```

### Comparing `ott-jax-0.4.0/src/ott/tools/gaussian_mixture/__init__.py` & `ott-jax-0.4.1/src/ott/tools/gaussian_mixture/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-# Copyright 2022 Google LLC.
+# Copyright OTT-JAX
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-#     http://www.apache.org/licenses/LICENSE-2.0
+#   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from . import fit_gmm_pair, gaussian, gaussian_mixture, gaussian_mixture_pair
```

### Comparing `ott-jax-0.4.0/src/ott/tools/gaussian_mixture/fit_gmm.py` & `ott-jax-0.4.1/src/ott/tools/gaussian_mixture/fit_gmm.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-# Copyright 2022 Google LLC.
+# Copyright OTT-JAX
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-#     http://www.apache.org/licenses/LICENSE-2.0
+#   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 r"""Fit a Gaussian mixture model.
 
 Sample usage:
 
 # initialize GMM with K-means++
 gmm_init = fit_gmm.initialize(
-  key=key,
+  rng=rng,
   points=my_points,
   point_weights=None,
   n_components=COMPONENTS)
 
 # refine GMM parameters using EM
 gmm = fit_gmm.fit_model_em(
   gmm=gmm_init,
@@ -162,24 +162,24 @@
     e_step_fn = jax.jit(e_step_fn)
     m_step_fn = jax.jit(m_step_fn)
 
   for i in range(steps):
     assignment_probs = e_step_fn(gmm, points)
     gmm_new = m_step_fn(points, point_weights, assignment_probs)
     if gmm_new.has_nans():
-      raise ValueError('NaNs in fit.')
+      raise ValueError("NaNs in fit.")
     if verbose:
       loss = loss_fn(gmm_new, points, point_weights)
       q = get_q_fn(
           gmm=gmm_new,
           assignment_probs=assignment_probs,
           points=points,
           point_weights=point_weights
       )
-      print(f'{i}  q={q}  -log prob={loss}', flush=True)
+      print(f"{i}  q={q}  -log prob={loss}")  # noqa: T201
     gmm = gmm_new
   return gmm
 
 
 # KMeans++ for initialization
 # See https://en.wikipedia.org/wiki/K-means%2B%2B for details
 
@@ -191,69 +191,69 @@
     return jnp.sum((points - loc[None]) ** 2., axis=-1)
 
   dist_sq_fn = jax.vmap(_dist_sq_one_loc, in_axes=(None, 0), out_axes=1)
   return dist_sq_fn(points, loc)
 
 
 def _get_locs(
-    key: jnp.ndarray, points: jnp.ndarray, n_components: int
+    rng: jax.random.PRNGKeyArray, points: jnp.ndarray, n_components: int
 ) -> jnp.ndarray:
   """Get the initial component means.
 
   Args:
-    key: jax.random seed
+    rng: jax.random key
     points: (n, n_dimensions) array of observations
     n_components: desired number of components
 
   Returns:
     (n_components, n_dimensions) array of means.
   """
   points = points.copy()
   n_points = points.shape[0]
   weights = jnp.ones(n_points) / n_points
-  key, subkey = jax.random.split(key)
-  index = jax.random.choice(key=subkey, a=points.shape[0], p=weights)
+  rng, subrng = jax.random.split(rng)
+  index = jax.random.choice(key=subrng, a=points.shape[0], p=weights)
   loc = points[index]
   points = jnp.concatenate([points[:index], points[index + 1:]], axis=0)
 
   locs = loc[None]
   for _ in range(n_components - 1):
     dist_sq = _get_dist_sq(points, locs)
     min_dist_sq = jnp.min(dist_sq, axis=-1)
     weights = min_dist_sq / jnp.sum(min_dist_sq)
-    key, subkey = jax.random.split(key)
-    index = jax.random.choice(key=subkey, a=points.shape[0], p=weights)
+    rng, subrng = jax.random.split(rng)
+    index = jax.random.choice(key=subrng, a=points.shape[0], p=weights)
     loc = points[index]
     points = jnp.concatenate([points[:index], points[index + 1:]], axis=0)
     locs = jnp.concatenate([locs, loc[None]], axis=0)
   return locs
 
 
 def from_kmeans_plusplus(
-    key: jnp.ndarray,
+    rng: jax.random.PRNGKeyArray,
     points: jnp.ndarray,
     point_weights: Optional[jnp.ndarray],
     n_components: int,
 ) -> gaussian_mixture.GaussianMixture:
   """Initialize a GMM via a single pass of K-means++.
 
   Args:
-    key: jax.random seed
+    rng: jax.random key
     points: (n, n_dimensions) array of observations
     point_weights: (n,) array of weights for points
     n_components: desired number of components
 
   Returns:
     An initial Gaussian mixture model.
 
   Raises:
     ValueError if any fitted parameters are non-finite.
   """
-  key, subkey = jax.random.split(key)
-  locs = _get_locs(key=subkey, points=points, n_components=n_components)
+  rng, subrng = jax.random.split(rng)
+  locs = _get_locs(rng=subrng, points=points, n_components=n_components)
   dist_sq = _get_dist_sq(points, locs)
   assignment_prob = (dist_sq == jnp.min(dist_sq,
                                         axis=-1)[:, None]).astype(points.dtype)
   del dist_sq
 
   if point_weights is None:
     point_weights = jnp.ones_like(points[..., 0])
@@ -261,43 +261,43 @@
       points=points,
       point_weights=point_weights,
       assignment_probs=assignment_prob
   )
 
 
 def initialize(
-    key: jnp.ndarray,
+    rng: jax.random.PRNGKeyArray,
     points: jnp.ndarray,
     point_weights: Optional[jnp.ndarray],
     n_components: int,
     n_attempts: int = 50,
     verbose: bool = False
 ) -> gaussian_mixture.GaussianMixture:
   """Initialize a GMM via K-means++ with retries on failure.
 
   Args:
-    key: jax.random seed
+    rng: jax.random key
     points: (n, n_dimensions) array of observations
     point_weights: (n,) array of weights for points
     n_components: desired number of components
     n_attempts: number of attempts to initialize before failing
     verbose: if True, print status information
 
   Returns:
     An initial Gaussian mixture model.
 
   Raises:
     ValueError if initialization was unsuccessful after n_attempts attempts.
   """
   for attempt in range(n_attempts):
-    key, subkey = jax.random.split(key)
+    rng, subrng = jax.random.split(rng)
     try:
       return from_kmeans_plusplus(
-          key=subkey,
+          rng=subrng,
           points=points,
           point_weights=point_weights,
           n_components=n_components
       )
     except ValueError:
       if verbose:
-        print(f'Failed to initialize, attempt {attempt}.', flush=True)
-  raise ValueError('Failed to initialize.')
+        print(f"Failed to initialize, attempt {attempt}.")  # noqa: T201
+  raise ValueError("Failed to initialize.")
```

### Comparing `ott-jax-0.4.0/src/ott/tools/gaussian_mixture/fit_gmm_pair.py` & `ott-jax-0.4.1/src/ott/tools/gaussian_mixture/fit_gmm_pair.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-# Copyright 2022 Google LLC.
+# Copyright OTT-JAX
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-#     http://www.apache.org/licenses/LICENSE-2.0
+#   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 r"""Fit 2 GMMs to 2 point clouds using likelihood and (approx) W2 distance.
@@ -81,15 +81,19 @@
 import math
 from typing import Callable, NamedTuple, Optional, Tuple
 
 import jax
 import jax.numpy as jnp
 import optax
 
-from ott.tools.gaussian_mixture import fit_gmm, gaussian_mixture, gaussian_mixture_pair
+from ott.tools.gaussian_mixture import (
+    fit_gmm,
+    gaussian_mixture,
+    gaussian_mixture_pair,
+)
 
 __all__ = ["get_fit_model_em_fn"]
 
 LOG2 = math.log(2)
 
 
 class Observations(NamedTuple):
@@ -186,26 +190,25 @@
   q0 = get_q(gmm=pair.gmm0, obs=obs0)
   q1 = get_q(gmm=pair.gmm1, obs=obs1)
   cost_matrix = pair.get_cost_matrix()
   sinkhorn_output = pair.get_sinkhorn(cost_matrix=cost_matrix)
   transport_penalty = sinkhorn_output.reg_ot_cost
   objective = q0 + q1 - weight_transport * transport_penalty
 
-  print((
-      f'{iteration:3d} {q0:.3f} {q1:.3f} '
-      f'transport:{transport_penalty:.3f} '
-      f'objective:{objective:.3f}'
-  ),
-        flush=True)
+  print(  # noqa: T201
+      f"{iteration:3d} {q0:.3f} {q1:.3f} "
+      f"transport:{transport_penalty:.3f} "
+      f"objective:{objective:.3f}"
+  )
 
 
 # The E-step for a single GMM
 
 
-def do_e_step(
+def do_e_step(  # noqa: D103
     e_step_fn: Callable[[gaussian_mixture.GaussianMixture, jnp.ndarray],
                         jnp.ndarray],
     gmm: gaussian_mixture.GaussianMixture,
     points: jnp.ndarray,
     point_weights: jnp.ndarray,
 ) -> Observations:
   assignment_probs = e_step_fn(gmm, points)
@@ -228,25 +231,14 @@
     learning_rate: learning rate to use for the Adam optimizer
     objective_fn: the objective function to maximize
     jit: if True, precompile key methods
 
   Returns:
     A function that performs the M-step of EM.
   """
-  grad_objective_fn = jax.grad(objective_fn, argnums=(0,))
-  gmm_m_step_fn = gaussian_mixture.GaussianMixture.from_points_and_assignment_probs
-  if jit:
-    grad_objective_fn = jax.jit(grad_objective_fn)
-    gmm_m_step_fn = jax.jit(gmm_m_step_fn)
-
-  opt_init, opt_update = optax.chain(
-      # Set the parameters of Adam. Note the learning_rate is not here.
-      optax.scale_by_adam(b1=0.9, b2=0.999, eps=1e-8),
-      optax.scale(learning_rate)
-  )
 
   def _m_step_fn(
       pair: gaussian_mixture_pair.GaussianMixturePair,
       obs0: Observations,
       obs1: Observations,
       steps: int,
   ) -> gaussian_mixture_pair.GaussianMixturePair:
@@ -265,17 +257,27 @@
 
     for _ in range(steps):
       grad_objective = grad_objective_fn(pair, obs0, obs1)
       updates, state = opt_update(grad_objective, state, (pair,))
       (pair,) = optax.apply_updates((pair,), updates)
       for j, gmm in enumerate((pair.gmm0, pair.gmm1)):
         if gmm.has_nans():
-          raise ValueError(f'NaN in gmm{j}')
+          raise ValueError(f"NaN in gmm{j}")
     return pair
 
+  grad_objective_fn = jax.grad(objective_fn, argnums=(0,))
+  if jit:
+    grad_objective_fn = jax.jit(grad_objective_fn)
+
+  opt_init, opt_update = optax.chain(
+      # Set the parameters of Adam. Note the learning_rate is not here.
+      optax.scale_by_adam(b1=0.9, b2=0.999, eps=1e-8),
+      optax.scale(learning_rate)
+  )
+
   return _m_step_fn
 
 
 def get_fit_model_em_fn(
     weight_transport: float,
     learning_rate: float = 0.001,
     jit: bool = True,
```

### Comparing `ott-jax-0.4.0/src/ott/tools/gaussian_mixture/gaussian.py` & `ott-jax-0.4.1/src/ott/tools/gaussian_mixture/gaussian.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-# Copyright 2022 Google LLC.
+# Copyright OTT-JAX
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-#     http://www.apache.org/licenses/LICENSE-2.0
+#   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Pytree for a normal distribution."""
-
 import math
 from typing import Optional, Union
 
 import jax
 import jax.numpy as jnp
 
 from ott.tools.gaussian_mixture import scale_tril
@@ -24,30 +22,30 @@
 __all__ = ["Gaussian"]
 
 LOG2PI = math.log(2. * math.pi)
 
 
 @jax.tree_util.register_pytree_node_class
 class Gaussian:
-  """PyTree for a normal distribution."""
+  """Normal distribution."""
 
   def __init__(self, loc: jnp.ndarray, scale: scale_tril.ScaleTriL):
     self._loc = loc
     self._scale = scale
 
   @classmethod
   def from_samples(
       cls,
       points: jnp.ndarray,
       weights: Optional[jnp.ndarray] = None
-  ) -> 'Gaussian':
+  ) -> "Gaussian":
     """Construct a Gaussian from weighted samples.
 
-    Unbiased, weighted covariance formula from https://en.wikipedia.org/wiki/Sample_mean_and_covariance#Weighted_samples
-    and https://www.gnu.org/software/gsl/doc/html/statistics.html?highlight=weighted#weighted-samples
+    Unbiased, weighted covariance formula from `GSL
+    <https://www.gnu.org/software/gsl/doc/html/statistics.html#weighted-samples>`_.
 
     Args:
       points: [n x d] array of samples
       weights: [n] array of weights
 
     Returns:
       Gaussian.
@@ -61,109 +59,119 @@
     scaled_centered_x = centered_x * weights.reshape(-1, 1)
     cov = scaled_centered_x.T.dot(centered_x) / (1 - weights.dot(weights))
     return cls.from_mean_and_cov(mean=mean, cov=cov)
 
   @classmethod
   def from_random(
       cls,
-      key: jnp.ndarray,
+      rng: jax.random.PRNGKeyArray,
       n_dimensions: int,
       stdev_mean: float = 0.1,
       stdev_cov: float = 0.1,
-      ridge: Union[float, jnp.array] = 0,
+      ridge: Union[float, jnp.ndarray] = 0,
       dtype: Optional[jnp.dtype] = None
-  ) -> 'Gaussian':
+  ) -> "Gaussian":
     """Construct a random Gaussian.
 
     Args:
-      key: jax.random seed
+      rng: jax.random key
       n_dimensions: desired covariance dimensions
-      stdev: standard deviation of loc and log eigenvalues
+      stdev_mean: standard deviation of location and log eigenvalues
         (means for both are 0)
+      stdev_cov: standard deviated of the covariance
+      ridge: Offset for means.
       dtype: data type
 
     Returns:
       A random Gaussian.
     """
-    key, subkey0, subkey1 = jax.random.split(key, num=3)
+    rng, subrng0, subrng1 = jax.random.split(rng, num=3)
     loc = jax.random.normal(
-        key=subkey0, shape=(n_dimensions,), dtype=dtype
+        key=subrng0, shape=(n_dimensions,), dtype=dtype
     ) * stdev_mean + ridge
     scale = scale_tril.ScaleTriL.from_random(
-        key=subkey1, n_dimensions=n_dimensions, stdev=stdev_cov, dtype=dtype
+        rng=subrng1, n_dimensions=n_dimensions, stdev=stdev_cov, dtype=dtype
     )
     return cls(loc=loc, scale=scale)
 
   @classmethod
-  def from_mean_and_cov(cls, mean: jnp.ndarray, cov: jnp.ndarray) -> 'Gaussian':
+  def from_mean_and_cov(cls, mean: jnp.ndarray, cov: jnp.ndarray) -> "Gaussian":
     """Construct a Gaussian from a mean and covariance."""
     scale = scale_tril.ScaleTriL.from_covariance(cov)
     return cls(loc=mean, scale=scale)
 
   @property
   def loc(self) -> jnp.ndarray:
+    """Mean of the Gaussian."""
     return self._loc
 
   @property
   def scale(self) -> scale_tril.ScaleTriL:
+    """Scale of the Gaussian."""
     return self._scale
 
   @property
   def n_dimensions(self) -> int:
+    """Dimensionality of the Gaussian."""
     return self.loc.shape[-1]
 
   def covariance(self) -> jnp.ndarray:
+    """Covariance of the Gaussian."""
     return self.scale.covariance()
 
   def to_z(self, x: jnp.ndarray) -> jnp.ndarray:
+    r"""Transform :math:`x` to :math:`z = \frac{x - loc}{scale}`."""
     return self.scale.centered_to_z(x_centered=x - self.loc)
 
   def from_z(self, z: jnp.ndarray) -> jnp.ndarray:
+    r"""Transform :math:`z` to :math:`x = loc + scale \cdot z`."""
     return self.scale.z_to_centered(z=z) + self.loc
 
   def log_prob(
       self,
       x: jnp.ndarray,  # (?, d)
   ) -> jnp.ndarray:  # (?, d)
-    """Log probability for a gaussian with a diagonal covariance."""
+    """Log probability for a Gaussian with a diagonal covariance."""
     d = x.shape[-1]
     z = self.to_z(x)
     log_det = self.scale.log_det_covariance()
     return (
         -0.5 * (d * LOG2PI + log_det[None] + jnp.sum(z ** 2., axis=-1))
     )  # (?, k)
 
-  def sample(self, key: jnp.ndarray, size: int) -> jnp.ndarray:
+  def sample(self, rng: jax.random.PRNGKeyArray, size: int) -> jnp.ndarray:
     """Generate samples from the distribution."""
-    std_samples_t = jax.random.normal(key=key, shape=(self.n_dimensions, size))
+    std_samples_t = jax.random.normal(key=rng, shape=(self.n_dimensions, size))
     return self.loc[None] + (
         jnp.swapaxes(
             jnp.matmul(self.scale.cholesky(), std_samples_t),
             axis1=-2,
             axis2=-1
         )
     )
 
-  def w2_dist(self, other: 'Gaussian') -> jnp.ndarray:
-    r"""Wasserstein distance W_2^2 to another Gaussian.
+  def w2_dist(self, other: "Gaussian") -> jnp.ndarray:
+    r"""Wasserstein distance :math:`W_2^2` to another Gaussian.
+
+    .. math::
 
-    W_2^2 = ||\mu_0-\mu_1||^2 +
-       \text{trace} ( (\Lambda_0^\frac{1}{2} - \Lambda_1^\frac{1}{2})^2 )
+      W_2^2 = ||\mu_0-\mu_1||^2 +
+         \text{trace} ( (\Lambda_0^\frac{1}{2} - \Lambda_1^\frac{1}{2})^2 )
 
     Args:
       other: other Gaussian
 
     Returns:
-      The W_2^2 distance between self and other
+      The :math:`W_2^2` distance between self and other
     """
     delta_mean = jnp.sum((self.loc - other.loc) ** 2., axis=-1)
     delta_sigma = self.scale.w2_dist(other.scale)
     return delta_mean + delta_sigma
 
-  def f_potential(self, dest: 'Gaussian', points: jnp.ndarray) -> jnp.ndarray:
+  def f_potential(self, dest: "Gaussian", points: jnp.ndarray) -> jnp.ndarray:
     """Optimal potential for W2 distance between Gaussians. Evaluated on points.
 
     Args:
       dest: Gaussian object
       points: samples
 
     Returns:
@@ -179,35 +187,35 @@
 
     return (
         0.5 * batch_inner_product(points, points) -
         0.5 * batch_inner_product(centered_x, scaled_x.T) -
         points.dot(dest.loc)
     )
 
-  def transport(self, dest: 'Gaussian', points: jnp.ndarray) -> jnp.ndarray:
+  def transport(self, dest: "Gaussian", points: jnp.ndarray) -> jnp.ndarray:
     """Transport points according to map between two Gaussian measures.
 
     Args:
       dest: Gaussian object
       points: samples
 
     Returns:
       Transported samples
     """
     return self.scale.transport(
         dest_scale=dest.scale, points=points - self.loc[None]
     ) + dest.loc[None]
 
-  def tree_flatten(self):
+  def tree_flatten(self):  # noqa: D102
     children = (self.loc, self.scale)
     aux_data = {}
     return children, aux_data
 
   @classmethod
-  def tree_unflatten(cls, aux_data, children):
+  def tree_unflatten(cls, aux_data, children):  # noqa: D102
     return cls(*children, **aux_data)
 
   def __hash__(self):
     return jax.tree_util.tree_flatten(self).__hash__()
 
   def __eq__(self, other):
     return jax.tree_util.tree_flatten(self) == jax.tree_util.tree_flatten(other)
```

### Comparing `ott-jax-0.4.0/src/ott/tools/gaussian_mixture/gaussian_mixture.py` & `ott-jax-0.4.1/src/ott/tools/gaussian_mixture/gaussian_mixture.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,31 @@
-# Copyright 2022 Google LLC.
+# Copyright OTT-JAX
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-#     http://www.apache.org/licenses/LICENSE-2.0
+#   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Pytree for a Gaussian mixture model."""
-
 from typing import List, Optional, Tuple, Union
 
 import jax
 import jax.numpy as jnp
 
-from ott.tools.gaussian_mixture import gaussian, linalg, probabilities, scale_tril
+from ott.tools.gaussian_mixture import (
+    gaussian,
+    linalg,
+    probabilities,
+    scale_tril,
+)
 
 __all__ = ["GaussianMixture"]
 
 
 def get_summary_stats_from_points_and_assignment_probs(
     points: jnp.ndarray, point_weights: jnp.ndarray,
     assignment_probs: jnp.ndarray
@@ -58,55 +61,55 @@
   )
 
   return components_from_points_fn(points, point_weights, assignment_probs)
 
 
 @jax.tree_util.register_pytree_node_class
 class GaussianMixture:
-  """Pytree for a Gaussian Mixture model."""
+  """Gaussian Mixture model."""
 
   def __init__(
       self, loc: jnp.ndarray, scale_params: jnp.ndarray,
       component_weight_ob: probabilities.Probabilities
   ):
     self._loc = loc
     self._scale_params = scale_params
     self._component_weight_ob = component_weight_ob
 
   @classmethod
   def from_random(
       cls,
-      key: jnp.ndarray,
+      rng: jax.random.PRNGKeyArray,
       n_components: int,
       n_dimensions: int,
       stdev_mean: float = 0.1,
       stdev_cov: float = 0.1,
       stdev_weights: float = 0.1,
       ridge: Union[float, jnp.array] = 0,
       dtype: Optional[jnp.dtype] = None
-  ) -> 'GaussianMixture':
+  ) -> "GaussianMixture":
     """Construct a random GMM."""
     loc = []
     scale_params = []
     for _ in range(n_components):
-      key, subkey = jax.random.split(key)
+      rng, subrng = jax.random.split(rng)
       component = gaussian.Gaussian.from_random(
-          key=subkey,
+          rng=subrng,
           n_dimensions=n_dimensions,
           stdev_mean=stdev_mean,
           stdev_cov=stdev_cov,
           ridge=ridge,
           dtype=dtype
       )
       loc.append(component.loc)
       scale_params.append(component.scale.params)
     loc = jnp.stack(loc, axis=0)
     scale_params = jnp.stack(scale_params, axis=0)
     weight_ob = probabilities.Probabilities.from_random(
-        key=subkey, n_dimensions=n_components, stdev=stdev_weights, dtype=dtype
+        rng=subrng, n_dimensions=n_components, stdev=stdev_weights, dtype=dtype
     )
     return cls(
         loc=loc, scale_params=scale_params, component_weight_ob=weight_ob
     )
 
   @classmethod
   def from_mean_cov_component_weights(
@@ -124,98 +127,108 @@
 
   @classmethod
   def from_points_and_assignment_probs(
       cls,
       points: jnp.ndarray,
       point_weights: jnp.ndarray,
       assignment_probs: jnp.ndarray,
-  ) -> 'GaussianMixture':
+  ) -> "GaussianMixture":
     """Estimate a GMM from points and a set of component probabilities."""
     mean, cov, wts = get_summary_stats_from_points_and_assignment_probs(
         points=points,
         point_weights=point_weights,
         assignment_probs=assignment_probs
     )
     return cls.from_mean_cov_component_weights(
         mean=mean, cov=cov, component_weights=wts
     )
 
   @property
   def dtype(self):
+    """Dtype of the GMM parameters."""
     return self.loc.dtype
 
   @property
   def n_dimensions(self):
+    """Number of dimensions of the GMM parameters."""
     return self._loc.shape[-1]
 
   @property
   def n_components(self):
+    """Number of components of the GMM parameters."""
     return self._loc.shape[-2]
 
   @property
   def loc(self) -> jnp.ndarray:
+    """Location parameters of the GMM."""
     return self._loc
 
   @property
   def scale_params(self) -> jnp.ndarray:
+    """Scale parameters of the GMM."""
     return self._scale_params
 
   @property
   def cholesky(self) -> jnp.ndarray:
+    """Cholesky decomposition of the GMM covariance matrices."""
     size = self.n_dimensions
 
     def _get_cholesky(scale_params):
       return scale_tril.ScaleTriL(params=scale_params, size=size).cholesky()
 
     return jax.vmap(_get_cholesky, in_axes=0, out_axes=0)(self.scale_params)
 
   @property
   def covariance(self) -> jnp.ndarray:
+    """Covariance matrices of the GMM."""
     size = self.n_dimensions
 
     def _get_covariance(scale_params):
       return scale_tril.ScaleTriL(params=scale_params, size=size).covariance()
 
     return jax.vmap(_get_covariance, in_axes=0, out_axes=0)(self.scale_params)
 
   @property
   def component_weight_ob(self) -> probabilities.Probabilities:
+    """Component weight object."""
     return self._component_weight_ob
 
   @property
   def component_weights(self) -> jnp.ndarray:
+    """Component weights probabilities."""
     return self._component_weight_ob.probs()
 
   def log_component_weights(self) -> jnp.ndarray:
+    """Log component weights probabilities."""
     return self._component_weight_ob.log_probs()
 
   def _get_normal(
       self, loc: jnp.ndarray, scale_params: jnp.ndarray
   ) -> gaussian.Gaussian:
     size = loc.shape[-1]
     return gaussian.Gaussian(
         loc=loc, scale=scale_tril.ScaleTriL(params=scale_params, size=size)
     )
 
   def get_component(self, index: int) -> gaussian.Gaussian:
-    """Get the specified GMM component."""
+    """Specified GMM component."""
     return self._get_normal(
         loc=self.loc[index], scale_params=self.scale_params[index]
     )
 
   def components(self) -> List[gaussian.Gaussian]:
-    """Get a list of all GMM components."""
+    """List of all GMM components."""
     return [self.get_component(i) for i in range(self.n_components)]
 
-  def sample(self, key: jnp.ndarray, size: int) -> jnp.ndarray:
+  def sample(self, rng: jax.random.PRNGKeyArray, size: int) -> jnp.ndarray:
     """Generate samples from the distribution."""
-    subkey0, subkey1 = jax.random.split(key)
-    component = self.component_weight_ob.sample(key=subkey0, size=size)
+    subrng0, subrng1 = jax.random.split(rng)
+    component = self.component_weight_ob.sample(rng=subrng0, size=size)
     std_samples = jax.random.normal(
-        key=subkey1, shape=(size, self.n_dimensions)
+        key=subrng1, shape=(size, self.n_dimensions)
     )
 
     def _transform_single_component(k, scale, loc):
 
       def _transform_single_value(single_component, single_x):
         return jax.lax.cond(
             single_component == k,
@@ -284,35 +297,35 @@
     log_prob_conditional = self.conditional_log_prob(x)
     log_component_weight = self.log_component_weights()
     log_prob_unnorm = log_prob_conditional + log_component_weight[None, :]
     return log_prob_unnorm - jax.scipy.special.logsumexp(
         log_prob_unnorm, axis=-1, keepdims=True
     )
 
-  def has_nans(self) -> bool:
+  def has_nans(self) -> bool:  # noqa: D102
     for leaf in jax.tree_util.tree_leaves(self):
       if jnp.any(~jnp.isfinite(leaf)):
         return True
     return False
 
-  def tree_flatten(self):
+  def tree_flatten(self):  # noqa: D102
     children = (self.loc, self.scale_params, self.component_weight_ob)
     aux_data = {}
     return children, aux_data
 
   @classmethod
-  def tree_unflatten(cls, aux_data, children):
+  def tree_unflatten(cls, aux_data, children):  # noqa: D102
     return cls(*children, **aux_data)
 
   def __repr__(self):
     class_name = type(self).__name__
     children, aux = self.tree_flatten()
-    return '{}({})'.format(
-        class_name, ', '.join([repr(c) for c in children] +
-                              [f'{k}: {repr(v)}' for k, v in aux.items()])
+    return "{}({})".format(
+        class_name, ", ".join([repr(c) for c in children] +
+                              [f"{k}: {repr(v)}" for k, v in aux.items()])
     )
 
   def __hash__(self):
     return jax.tree_util.tree_flatten(self).__hash__()
 
   def __eq__(self, other):
     return jax.tree_util.tree_flatten(self) == jax.tree_util.tree_flatten(other)
```

### Comparing `ott-jax-0.4.0/src/ott/tools/gaussian_mixture/gaussian_mixture_pair.py` & `ott-jax-0.4.1/src/ott/tools/gaussian_mixture/gaussian_mixture_pair.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-# Copyright 2022 Google LLC.
+# Copyright OTT-JAX
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-#     http://www.apache.org/licenses/LICENSE-2.0
+#   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Pytree containing parameters for a pair of coupled Gaussian mixture models.
-"""  # noqa: D200
 from typing import Any
 
 import jax
 import jax.numpy as jnp
 
 from ott.geometry import costs, geometry, pointcloud
 from ott.problems.linear import linear_problem
@@ -24,31 +22,31 @@
 from ott.tools.gaussian_mixture import gaussian_mixture
 
 __all__ = ["GaussianMixturePair"]
 
 
 @jax.tree_util.register_pytree_node_class
 class GaussianMixturePair:
-  """Pytree for a coupled pair of Gaussian mixture models.
+  """Coupled pair of Gaussian mixture models.
 
   Includes methods used in estimating an optimal pairing between GMM components
   using the Wasserstein-like method described in :cite:`delon:20`,
-  as well as generalization that allows for the re-weighting of components.
+  as well as generalization that allows for the reweighting of components.
 
-  The Delon & Desolneux paper above proposes fitting a pair of GMMs to a pair
+  :cite:`delon:20` propose fitting a pair of GMMs to a pair
   of point clouds in such a way that the sum of the log likelihood of the
   points minus a weighted penalty involving a Wasserstein-like distance between
   the GMMs. Their proposed algorithm involves using EM in which a balanced
   Sinkhorn algorithm is used to estimate a coupling between the GMMs at each
   step of EM.
 
   Our generalization of this algorithm allows for a mismatch between the
   marginals of the coupling and the GMM component weights. This mismatch can be
-  interpreted as components being re-weighted rather than being transported.
-  We penalize re-weighting with a generalized KL-divergence penalty, and we give
+  interpreted as components being reweighted rather than being transported.
+  We penalize reweighting with a generalized KL-divergence penalty, and we give
   the option to use the unbalanced Sinkhorn algorithm rather than the balanced
   to compute the divergence between GMMs.
   """
 
   def __init__(
       self,
       gmm0: gaussian_mixture.GaussianMixture,
@@ -81,39 +79,39 @@
     self._gmm0 = gmm0
     self._gmm1 = gmm1
     self._epsilon = epsilon
     self._tau = tau
     self._lock_gmm1 = lock_gmm1
 
   @property
-  def dtype(self):
+  def dtype(self):  # noqa: D102
     return self.gmm0.dtype
 
   @property
-  def gmm0(self):
+  def gmm0(self):  # noqa: D102
     return self._gmm0
 
   @property
-  def gmm1(self):
+  def gmm1(self):  # noqa: D102
     return self._gmm1
 
   @property
-  def epsilon(self):
+  def epsilon(self):  # noqa: D102
     return self._epsilon
 
   @property
-  def tau(self):
+  def tau(self):  # noqa: D102
     return self._tau
 
   @property
-  def rho(self):
+  def rho(self):  # noqa: D102
     return self.epsilon * self.tau / (1. - self.tau)
 
   @property
-  def lock_gmm1(self):
+  def lock_gmm1(self):  # noqa: D102
     return self._lock_gmm1
 
   def get_bures_geometry(self) -> pointcloud.PointCloud:
     """Get a Bures Geometry for the two GMMs."""
     mean0 = self.gmm0.loc
     dimension = mean0.shape[-1]
     cov0 = self.gmm0.covariance
@@ -127,15 +125,15 @@
         x=x,
         y=y,
         cost_fn=costs.Bures(dimension=dimension),
         epsilon=self.epsilon
     )
 
   def get_cost_matrix(self) -> jnp.ndarray:
-    """Get matrix of W2^2 costs between all pairs of (gmm0, gmm1) components."""
+    """Get matrix of :math:`W_2^2` costs between all pairs of components."""
     return self.get_bures_geometry().cost_matrix
 
   def get_sinkhorn(
       self, cost_matrix: jnp.ndarray, **kwargs: Any
   ) -> sinkhorn.SinkhornOutput:
     """Get the output of Sinkhorn's method for a given cost matrix."""
     # We use a Geometry here rather than the PointCloud created in
@@ -154,19 +152,20 @@
   def get_normalized_sinkhorn_coupling(
       self,
       sinkhorn_output: sinkhorn.SinkhornOutput,
   ) -> jnp.ndarray:
     """Get the normalized coupling matrix for the specified Sinkhorn output.
 
     Args:
-      sinkhorn_output: Sinkhorn algorithm output as returned by get_sinkhorn()
+      sinkhorn_output: Sinkhorn algorithm output as returned by
+        :meth:`get_sinkhorn`.
 
     Returns:
       A coupling matrix that tells how much of the mass of each component of
-      gmm0 is mapped to each component of gmm1.
+      :attr:`gmm0` is mapped to each component of :attr:`gmm1`.
     """
     return sinkhorn_output.matrix / jnp.sum(sinkhorn_output.matrix)
 
   def tree_flatten(self):
     """Method used by jax.tree_util to flatten a GaussianMixturePair.
 
     We control the subset of parameters that we will optimize in fit_gmm_pair
@@ -174,20 +173,20 @@
     or aux_data (the parameters to leave alone).
 
     Returns:
       A tuple of child pytrees and a dict of auxiliary data.
     """  # noqa: D401
     children = [self.gmm0]
     aux_data = {
-        'epsilon': self.epsilon,
-        'tau': self.tau,
-        'lock_gmm1': self.lock_gmm1
+        "epsilon": self.epsilon,
+        "tau": self.tau,
+        "lock_gmm1": self.lock_gmm1
     }
     if self.lock_gmm1:
-      aux_data['gmm1'] = self.gmm1
+      aux_data["gmm1"] = self.gmm1
     else:
       children.append(self.gmm1)
     return tuple(children), aux_data
 
   @classmethod
   def tree_unflatten(cls, aux_data, children):
     """Method used by jax.tree_util to unflatten a GaussianMixturePair.
@@ -199,25 +198,25 @@
       aux_data: auxiliary data that is passed to the constructor as kwargs
       children: child pytrees passed to the constructor as args
 
     Returns:
       A GaussianMixturePair.
     """  # noqa: D401
     children = list(children)
-    if 'gmm1' in aux_data:
-      gmm1 = aux_data.pop('gmm1')
+    if "gmm1" in aux_data:
+      gmm1 = aux_data.pop("gmm1")
       children.insert(1, gmm1)
     return cls(*children, **aux_data)
 
   def __repr__(self):
     class_name = type(self).__name__
     children, aux = self.tree_flatten()
-    return '{}({})'.format(
-        class_name, ', '.join([repr(c) for c in children] +
-                              [f'{k}: {repr(v)}' for k, v in aux.items()])
+    return "{}({})".format(
+        class_name, ", ".join([repr(c) for c in children] +
+                              [f"{k}: {repr(v)}" for k, v in aux.items()])
     )
 
   def __hash__(self):
     return jax.tree_util.tree_flatten(self).__hash__()
 
   def __eq__(self, other):
     return jax.tree_util.tree_flatten(self) == jax.tree_util.tree_flatten(other)
```

### Comparing `ott-jax-0.4.0/src/ott/tools/gaussian_mixture/linalg.py` & `ott-jax-0.4.1/src/ott/tools/gaussian_mixture/linalg.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-# Copyright 2022 Google LLC.
+# Copyright OTT-JAX
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-#     http://www.apache.org/licenses/LICENSE-2.0
+#   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Linear algebra utility methods for optimal transport of Gaussian mixtures."""
-
 from typing import Callable, Iterable, List, Optional, Tuple
 
 import jax
 import jax.numpy as jnp
 
 
 def get_mean_and_var(
@@ -130,15 +128,15 @@
   """
   return jnp.transpose(
       jax.scipy.linalg.solve_triangular(m, jnp.transpose(x), lower=lower)
   )
 
 
 def get_random_orthogonal(
-    key: jnp.ndarray,
+    rng: jax.random.PRNGKeyArray,
     dim: int,
     dtype: Optional[jnp.dtype] = None
 ) -> jnp.ndarray:
   """Get a random orthogonal matrix with the specified dimension."""
-  m = jax.random.normal(key=key, shape=[dim, dim], dtype=dtype)
+  m = jax.random.normal(key=rng, shape=[dim, dim], dtype=dtype)
   q, _ = jnp.linalg.qr(m)
   return q
```

### Comparing `ott-jax-0.4.0/src/ott/tools/gaussian_mixture/probabilities.py` & `ott-jax-0.4.1/src/ott/tools/gaussian_mixture/probabilities.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-# Copyright 2022 Google LLC.
+# Copyright OTT-JAX
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-#     http://www.apache.org/licenses/LICENSE-2.0
+#   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Pytree for a vector of probabilities."""
-
 from typing import Optional
 
 import jax
 import jax.numpy as jnp
 
 __all__ = ["Probabilities"]
 
@@ -33,72 +31,76 @@
 
   def __init__(self, params):
     self._params = params
 
   @classmethod
   def from_random(
       cls,
-      key: jnp.ndarray,
+      rng: jax.random.PRNGKeyArray,
       n_dimensions: int,
       stdev: Optional[float] = 0.1,
       dtype: Optional[jnp.dtype] = None
-  ) -> 'Probabilities':
+  ) -> "Probabilities":
     """Construct a random Probabilities."""
     return cls(
         params=jax.random
-        .normal(key=key, shape=(n_dimensions - 1,), dtype=dtype) * stdev
+        .normal(key=rng, shape=(n_dimensions - 1,), dtype=dtype) * stdev
     )
 
   @classmethod
-  def from_probs(cls, probs: jnp.ndarray) -> 'Probabilities':
+  def from_probs(cls, probs: jnp.ndarray) -> "Probabilities":
     """Construct Probabilities from a vector of probabilities."""
     log_probs = jnp.log(probs)
     log_probs_normalized, norm = log_probs[:-1], log_probs[-1]
     log_probs_normalized -= norm
     return cls(params=log_probs_normalized)
 
   @property
-  def params(self):
+  def params(self):  # noqa: D102
     return self._params
 
   @property
-  def dtype(self):
+  def dtype(self):  # noqa: D102
     return self._params.dtype
 
   def unnormalized_log_probs(self) -> jnp.ndarray:
+    """Get the unnormalized log probabilities."""
     return jnp.concatenate([self._params,
                             jnp.zeros((1,), dtype=self.dtype)],
                            axis=-1)
 
   def log_probs(self) -> jnp.ndarray:
+    """Get the log probabilities."""
     return jax.nn.log_softmax(self.unnormalized_log_probs())
 
   def probs(self) -> jnp.ndarray:
+    """Get the probabilities."""
     return jax.nn.softmax(self.unnormalized_log_probs())
 
-  def sample(self, key: jnp.ndarray, size: int) -> jnp.ndarray:
+  def sample(self, rng: jax.random.PRNGKeyArray, size: int) -> jnp.ndarray:
+    """Sample from the distribution."""
     return jax.random.categorical(
-        key=key, logits=self.unnormalized_log_probs(), shape=(size,)
+        key=rng, logits=self.unnormalized_log_probs(), shape=(size,)
     )
 
-  def tree_flatten(self):
+  def tree_flatten(self):  # noqa: D102
     children = (self.params,)
     aux_data = {}
     return children, aux_data
 
   @classmethod
-  def tree_unflatten(cls, aux_data, children):
+  def tree_unflatten(cls, aux_data, children):  # noqa: D102
     return cls(*children, **aux_data)
 
   def __repr__(self):
     class_name = type(self).__name__
     children, aux = self.tree_flatten()
-    return '{}({})'.format(
-        class_name, ', '.join([repr(c) for c in children] +
-                              [f'{k}: {repr(v)}' for k, v in aux.items()])
+    return "{}({})".format(
+        class_name, ", ".join([repr(c) for c in children] +
+                              [f"{k}: {repr(v)}" for k, v in aux.items()])
     )
 
   def __hash__(self):
     return jax.tree_util.tree_flatten(self).__hash__()
 
   def __eq__(self, other):
     return jax.tree_util.tree_flatten(self) == jax.tree_util.tree_flatten(other)
```

### Comparing `ott-jax-0.4.0/src/ott/tools/gaussian_mixture/scale_tril.py` & `ott-jax-0.4.1/src/ott/tools/gaussian_mixture/scale_tril.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-# Copyright 2022 Google LLC.
+# Copyright OTT-JAX
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-#     http://www.apache.org/licenses/LICENSE-2.0
+#   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Pytree for a lower triangular Cholesky factored covariance matrix."""
-
 from typing import Optional, Tuple
 
 import jax
 import jax.numpy as jnp
 
 from ott.geometry import costs
 from ott.math import matrix_square_root
@@ -34,69 +32,69 @@
     self._size = size
 
   @classmethod
   def from_points_and_weights(
       cls,
       points: jnp.ndarray,
       weights: jnp.ndarray,
-  ) -> Tuple[jnp.ndarray, 'ScaleTriL']:
+  ) -> Tuple[jnp.ndarray, "ScaleTriL"]:
     """Get a mean and a ScaleTriL from a set of points and weights."""
     mean, cov = linalg.get_mean_and_cov(points=points, weights=weights)
     return mean, cls.from_covariance(cov)
 
   @classmethod
   def from_random(
       cls,
-      key: jnp.ndarray,
+      rng: jax.random.PRNGKeyArray,
       n_dimensions: int,
       stdev: Optional[float] = 0.1,
       dtype: jnp.dtype = jnp.float32,
-  ) -> 'ScaleTriL':
+  ) -> "ScaleTriL":
     """Construct a random ScaleTriL.
 
     Args:
-      key: pseudo-random number generator key
+      rng: pseudo-random number generator key
       n_dimensions: number of dimensions
       stdev: desired standard deviation (around 0) for the log eigenvalues
       dtype: data type for the covariance matrix
 
     Returns:
       A ScaleTriL.
     """
     # generate a random orthogonal matrix
-    key, subkey = jax.random.split(key)
-    q = linalg.get_random_orthogonal(key=subkey, dim=n_dimensions, dtype=dtype)
+    rng, subrng = jax.random.split(rng)
+    q = linalg.get_random_orthogonal(rng=subrng, dim=n_dimensions, dtype=dtype)
 
     # generate random eigenvalues
     eigs = stdev * jnp.exp(
-        jax.random.normal(key=key, shape=(n_dimensions,), dtype=dtype)
+        jax.random.normal(key=rng, shape=(n_dimensions,), dtype=dtype)
     )
 
     # random positive definite matrix
     sigma = q * jnp.expand_dims(eigs, -2) @ q.T
 
     # cholesky factorization
     chol = jnp.linalg.cholesky(sigma)
     # flatten
     m = linalg.apply_to_diag(chol, jnp.log)
     flat = linalg.tril_to_flat(m)
     return cls(params=flat, size=n_dimensions)
 
   @classmethod
-  def from_cholesky(cls, cholesky: jnp.ndarray) -> 'ScaleTriL':
+  def from_cholesky(cls, cholesky: jnp.ndarray) -> "ScaleTriL":
     """Construct ScaleTriL from a Cholesky factor of a covariance matrix."""
     m = linalg.apply_to_diag(cholesky, jnp.log)
     flat = linalg.tril_to_flat(m)
     return cls(params=flat, size=cholesky.shape[-1])
 
   @classmethod
   def from_covariance(
       cls,
       covariance: jnp.ndarray,
-  ) -> 'ScaleTriL':
+  ) -> "ScaleTriL":
     """Construct ScaleTriL from a covariance matrix."""
     cholesky = jnp.linalg.cholesky(covariance)
     return cls.from_cholesky(cholesky)
 
   @property
   def params(self) -> jnp.ndarray:
     """Internal representation."""
@@ -135,15 +133,15 @@
     """Map centered points to standardized centered points (i.e. cov(z) = I)."""
     return linalg.invmatvectril(m=self.cholesky(), x=x_centered, lower=True)
 
   def z_to_centered(self, z: jnp.ndarray) -> jnp.ndarray:
     """Scale standardized points to points with the specified covariance."""
     return (self.cholesky() @ z.T).T
 
-  def w2_dist(self, other: 'ScaleTriL') -> jnp.ndarray:
+  def w2_dist(self, other: "ScaleTriL") -> jnp.ndarray:
     r"""Wasserstein distance W_2^2 to another Gaussian with same mean.
 
     Args:
       other: Scale for the other Gaussian
 
     Returns:
       The W_2^2 distance
@@ -156,15 +154,15 @@
 
     x0 = _flatten_cov(self.covariance())
     x1 = _flatten_cov(other.covariance())
     cost_fn = costs.Bures(dimension=dimension)
     return (cost_fn.norm(x0) + cost_fn.norm(x1) +
             cost_fn.pairwise(x0, x1))[...,]
 
-  def gaussian_map(self, dest_scale: 'ScaleTriL') -> jnp.ndarray:
+  def gaussian_map(self, dest_scale: "ScaleTriL") -> jnp.ndarray:
     """Scaling matrix used in transport between 0-mean Gaussians.
 
     Sigma_mu^{-1/2} @
       [Sigma_mu ^{1/2} Sigma_nu Sigma_mu ^{1/2}]^{1/2}
     @ Sigma_mu ^{-1/2}
 
     Args:
@@ -174,47 +172,46 @@
       Gaussian scaling matrix, same dimension as self.covaraince
     """
     sqrt0, sqrt0_inv = linalg.matrix_powers(self.covariance(), (0.5, -0.5))
     sigma1 = dest_scale.covariance()
     m = matrix_square_root.sqrtm_only(
         jnp.matmul(sqrt0, jnp.matmul(sigma1, sqrt0))
     )
-    m = jnp.matmul(sqrt0_inv, jnp.matmul(m, sqrt0_inv))
-    return m
+    return jnp.matmul(sqrt0_inv, jnp.matmul(m, sqrt0_inv))
 
   def transport(
-      self, dest_scale: 'ScaleTriL', points: jnp.ndarray
+      self, dest_scale: "ScaleTriL", points: jnp.ndarray
   ) -> jnp.ndarray:
     """Apply Monge map, computed between two 0-mean Gaussians, to points.
 
     Args:
       dest_scale: destination Scale
       points: points to transport
 
     Returns:
       Points transported to a Gaussian with the new scale.
     """
     m = self.gaussian_map(dest_scale)
     return (m @ points.T).T
 
-  def tree_flatten(self):
+  def tree_flatten(self):  # noqa: D102
     children = (self.params,)
-    aux_data = {'size': self.size}
+    aux_data = {"size": self.size}
     return children, aux_data
 
   @classmethod
-  def tree_unflatten(cls, aux_data, children):
+  def tree_unflatten(cls, aux_data, children):  # noqa: D102
     return cls(*children, **aux_data)
 
   def __repr__(self):
     class_name = type(self).__name__
     children, aux = self.tree_flatten()
-    return '{}({})'.format(
-        class_name, ', '.join([repr(c) for c in children] +
-                              [f'{k}: {repr(v)}' for k, v in aux.items()])
+    return "{}({})".format(
+        class_name, ", ".join([repr(c) for c in children] +
+                              [f"{k}: {repr(v)}" for k, v in aux.items()])
     )
 
   def __hash__(self):
     return jax.tree_util.tree_flatten(self).__hash__()
 
   def __eq__(self, other):
     return jax.tree_util.tree_flatten(self) == jax.tree_util.tree_flatten(other)
```

### Comparing `ott-jax-0.4.0/src/ott/tools/k_means.py` & `ott-jax-0.4.1/src/ott/tools/k_means.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,51 +1,52 @@
-# Copyright 2022 The OTT Authors
+# Copyright OTT-JAX
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-#     http://www.apache.org/licenses/LICENSE-2.0
+#   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import functools
 import math
 from typing import Callable, Literal, NamedTuple, Optional, Tuple, Union
 
 import jax
 import jax.numpy as jnp
 
+from ott import utils
 from ott.geometry import costs, pointcloud
 from ott.math import fixed_point_loop
 
 __all__ = ["k_means", "KMeansOutput"]
 
 Init_t = Union[Literal["k-means++", "random"],
                Callable[[pointcloud.PointCloud, int, jnp.ndarray], jnp.ndarray]]
 
 
-class KPPState(NamedTuple):
-  key: jnp.ndarray
+class KPPState(NamedTuple):  # noqa: D101
+  rng: jax.random.PRNGKeyArray
   centroids: jnp.ndarray
   centroid_dists: jnp.ndarray
 
 
-class KMeansState(NamedTuple):
+class KMeansState(NamedTuple):  # noqa: D101
   centroids: jnp.ndarray
   prev_assignment: jnp.ndarray
   assignment: jnp.ndarray
   errors: jnp.ndarray
   center_shift: float
 
 
-class KMeansConst(NamedTuple):
+class KMeansConst(NamedTuple):  # noqa: D101
   geom: pointcloud.PointCloud
   x_weights: jnp.ndarray
 
   @property
   def x(self) -> jnp.ndarray:
     """Array of shape ``[n, ndim]`` containing the unweighted point cloud."""
     return self.geom.x
@@ -104,65 +105,67 @@
         iteration=jnp.sum(~mask),
         error=error,
         inner_errors=errs if store_inner_errors else None,
     )
 
 
 def _random_init(
-    geom: pointcloud.PointCloud, k: int, key: jnp.ndarray
+    geom: pointcloud.PointCloud, k: int, rng: jax.random.PRNGKeyArray
 ) -> jnp.ndarray:
   ixs = jnp.arange(geom.shape[0])
-  ixs = jax.random.choice(key, ixs, shape=(k,), replace=False)
+  ixs = jax.random.choice(rng, ixs, shape=(k,), replace=False)
   return geom.subset(ixs, None).x
 
 
 def _k_means_plus_plus(
     geom: pointcloud.PointCloud,
     k: int,
-    key: jnp.ndarray,
+    rng: jax.random.PRNGKeyArray,
     n_local_trials: Optional[int] = None,
 ) -> jnp.ndarray:
 
-  def init_fn(geom: pointcloud.PointCloud, key: jnp.ndarray) -> KPPState:
-    key, next_key = jax.random.split(key, 2)
-    ix = jax.random.choice(key, jnp.arange(geom.shape[0]), shape=())
+  def init_fn(
+      geom: pointcloud.PointCloud, rng: jax.random.PRNGKeyArray
+  ) -> KPPState:
+    rng, next_rng = jax.random.split(rng, 2)
+    ix = jax.random.choice(rng, jnp.arange(geom.shape[0]), shape=())
     centroids = jnp.full((k, geom.cost_rank), jnp.inf).at[0].set(geom.x[ix])
     dists = geom.subset(ix, None).cost_matrix[0]
-    return KPPState(key=next_key, centroids=centroids, centroid_dists=dists)
+    return KPPState(rng=next_rng, centroids=centroids, centroid_dists=dists)
 
   def body_fn(
       iteration: int, const: Tuple[pointcloud.PointCloud, jnp.ndarray],
       state: KPPState, compute_error: bool
   ) -> KPPState:
     del compute_error
-    key, next_key = jax.random.split(state.key, 2)
+    rng, next_rng = jax.random.split(state.rng, 2)
     geom, ixs = const
 
     # no need to normalize when `replace=True`
     probs = state.centroid_dists
     ixs = jax.random.choice(
-        key, ixs, shape=(n_local_trials,), p=probs, replace=True
+        rng, ixs, shape=(n_local_trials,), p=probs, replace=True
     )
     geom = geom.subset(ixs, None)
 
     candidate_dists = jnp.minimum(geom.cost_matrix, state.centroid_dists)
     best_ix = jnp.argmin(candidate_dists.sum(1))
 
     centroids = state.centroids.at[iteration + 1].set(geom.x[best_ix])
     centroid_dists = candidate_dists[best_ix]
 
     return KPPState(
-        key=next_key, centroids=centroids, centroid_dists=centroid_dists
+        rng=next_rng, centroids=centroids, centroid_dists=centroid_dists
     )
 
   if n_local_trials is None:
     n_local_trials = 2 + int(math.log(k))
   assert n_local_trials > 0, n_local_trials
 
-  state = init_fn(geom, key)
+  state = init_fn(geom, rng)
   constants = (geom, jnp.arange(geom.shape[0]))
   state = fixed_point_loop.fixpoint_iter(
       lambda *_, **__: True,
       body_fn,
       min_iterations=k - 1,
       max_iterations=k - 1,
       inner_iterations=1,
@@ -219,15 +222,15 @@
   ws -= to_remove[:, -1:]
 
   return centroids * jnp.where(ws > 0., 1. / ws, 1.)
 
 
 @functools.partial(jax.vmap, in_axes=[0] + [None] * 9)
 def _k_means(
-    key: jnp.ndarray,
+    rng: jax.random.PRNGKeyArray,
     geom: pointcloud.PointCloud,
     k: int,
     weights: Optional[jnp.ndarray] = None,
     init: Init_t = "k-means++",
     n_local_trials: Optional[int] = None,
     tol: float = 1e-4,
     min_iterations: int = 0,
@@ -244,15 +247,15 @@
       init = _random_init
     if not callable(init):
       raise TypeError(
           f"Expected `init` to be 'k-means++', 'random' "
           f"or a callable, found `{init_fn!r}`."
       )
 
-    centroids = init(geom, k, key)
+    centroids = init(geom, k, rng)
     if centroids.shape != (k, geom.cost_rank):
       raise ValueError(
           f"Expected initial centroids to have shape "
           f"`{k, geom.cost_rank}`, found `{centroids.shape}`."
       )
     n = geom.shape[0]
     # TODO(michalk8): find a better solution for the below error
@@ -347,15 +350,15 @@
     init: Init_t = "k-means++",
     n_init: int = 10,
     n_local_trials: Optional[int] = None,
     tol: float = 1e-4,
     min_iterations: int = 0,
     max_iterations: int = 300,
     store_inner_errors: bool = False,
-    key: Optional[jnp.ndarray] = None,
+    rng: Optional[jax.random.PRNGKeyArray] = None,
 ) -> KMeansOutput:
   r"""K-means clustering using Lloyd's algorithm :cite:`lloyd:82`.
 
   Args:
     geom: Point cloud of shape ``[n, ndim]`` to cluster. If passed as an array,
       :class:`~ott.geometry.costs.SqEuclidean` cost is assumed.
     k: The number of clusters.
@@ -374,39 +377,38 @@
     n_local_trials: Number of local trials when ``init = 'k-means++'``.
       If ``None``, :math:`2 + \lfloor log(k) \rfloor` is used.
     tol: Relative tolerance with respect to the Frobenius norm of the centroids'
       shift between two consecutive iterations.
     min_iterations: Minimum number of iterations.
     max_iterations: Maximum number of iterations.
     store_inner_errors: Whether to store the errors (inertia) at each iteration.
-    key: Random key to seed the initializations.
+    rng: Random key for seeding the initializations.
 
   Returns:
     The k-means clustering.
   """
   assert geom.shape[
       0] >= k, f"Cannot cluster `{geom.shape[0]}` points into `{k}` clusters."
   if isinstance(geom, jnp.ndarray):
     geom = pointcloud.PointCloud(geom)
   if isinstance(geom.cost_fn, costs.Cosine):
     geom = geom._cosine_to_sqeucl()
   assert geom.is_squared_euclidean
+  rng = utils.default_prng_key(rng)
 
   if geom.is_online:
     # to allow materializing the cost matrix
     children, aux_data = geom.tree_flatten()
     aux_data["batch_size"] = None
     geom = type(geom).tree_unflatten(aux_data, children)
 
   if weights is None:
     weights = jnp.ones(geom.shape[0])
   assert weights.shape == (geom.shape[0],)
 
-  if key is None:
-    key = jax.random.PRNGKey(0)
-  keys = jax.random.split(key, n_init)
+  rngs = jax.random.split(rng, n_init)
   out = _k_means(
-      keys, geom, k, weights, init, n_local_trials, tol, min_iterations,
+      rngs, geom, k, weights, init, n_local_trials, tol, min_iterations,
       max_iterations, store_inner_errors
   )
   best_ix = jnp.argmin(out.error)
   return jax.tree_util.tree_map(lambda arr: arr[best_ix], out)
```

### Comparing `ott-jax-0.4.0/src/ott/tools/plot.py` & `ott-jax-0.4.1/src/ott/tools/plot.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,73 +1,81 @@
-# Copyright 2022 Google LLC.
+# Copyright OTT-JAX
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-#     http://www.apache.org/licenses/LICENSE-2.0
+#   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Plotting utils."""
-
 from typing import List, Optional, Sequence, Tuple, Union
 
 import jax.numpy as jnp
 import numpy as np
 import scipy
 
-import matplotlib.pyplot as plt
-from matplotlib import animation
-
 from ott import utils
 from ott.geometry import pointcloud
 from ott.solvers.linear import sinkhorn, sinkhorn_lr
 from ott.solvers.quadratic import gromov_wasserstein
 
+try:
+  import matplotlib.pyplot as plt
+  from matplotlib import animation
+except ImportError:
+  plt = animation = None
+
 # TODO(michalk8): make sure all outputs conform to a unified transport interface
 Transport = Union[sinkhorn.SinkhornOutput, sinkhorn_lr.LRSinkhornOutput,
                   gromov_wasserstein.GWOutput]
 
 
 def bidimensional(x: jnp.ndarray,
                   y: jnp.ndarray) -> Tuple[jnp.ndarray, jnp.ndarray]:
-  """Apply PCA to reduce to bimensional data."""
+  """Apply PCA to reduce to bi-dimensional data."""
   if x.shape[1] < 3:
     return x, y
 
   u, s, _ = scipy.sparse.linalg.svds(jnp.concatenate([x, y], axis=0), k=2)
   proj = u * s
   k = x.shape[0]
   return proj[:k], proj[k:]
 
 
 class Plot:
   """Plot an optimal transport map between two point clouds.
 
   It enables to either plot or update a plot in a single object, offering the
-  possibilities to create animations as matplotlib.animation.FuncAnimation,
-  which can in turned be saved to disk at will. There are two design principles
-  here: 1) we do not rely on saving to/loading from disk to create animations
-  2) we try as much as possible to disentangle the transport problem(s) from
-  its visualization(s).
+  possibilities to create animations as a
+  :class:`~matplotlib.animation.FuncAnimation`, which can in turned be saved to
+  disk at will. There are two design principles here:
+
+  #. we do not rely on saving to/loading from disk to create animations
+  #. we try as much as possible to disentangle the transport problem from
+     its visualization.
   """
 
   def __init__(
       self,
-      fig: Optional[plt.Figure] = None,
-      ax: Optional[plt.Axes] = None,
+      fig: Optional["plt.Figure"] = None,
+      ax: Optional["plt.Axes"] = None,
       cost_threshold: float = -1.0,  # should be negative for animations.
       scale: int = 200,
       show_lines: bool = True,
-      cmap: str = 'cool'
+      cmap: str = "cool",
+      scale_alpha_by_coupling: bool = False,
+      alpha: float = 0.7,
   ):
+    if plt is None:
+      raise RuntimeError("Please install `matplotlib` first.")
+
     if ax is None and fig is None:
       fig, ax = plt.subplots()
     elif fig is None:
       fig = plt.gcf()
     elif ax is None:
       ax = plt.gca()
     self.fig = fig
@@ -75,148 +83,174 @@
     self._show_lines = show_lines
     self._lines = []
     self._points_x = None
     self._points_y = None
     self._threshold = cost_threshold
     self._scale = scale
     self._cmap = cmap
+    self._scale_alpha_by_coupling = scale_alpha_by_coupling
+    self._alpha = alpha
 
   def _scatter(self, ot: Transport):
     """Compute the position and scales of the points on a 2D plot."""
     if not isinstance(ot.geom, pointcloud.PointCloud):
-      raise ValueError('So far we only plot PointCloud geometry.')
+      raise ValueError("So far we only plot PointCloud geometry.")
 
     x, y = ot.geom.x, ot.geom.y
     a, b = ot.a, ot.b
     x, y = bidimensional(x, y)
     scales_x = a * self._scale * a.shape[0]
     scales_y = b * self._scale * b.shape[0]
     return x, y, scales_x, scales_y
 
   def _mapping(self, x: jnp.ndarray, y: jnp.ndarray, matrix: jnp.ndarray):
     """Compute the lines representing the mapping between the 2 point clouds."""
+    # Only plot the lines with a cost above the threshold.
     u, v = jnp.where(matrix > self._threshold)
     c = matrix[jnp.where(matrix > self._threshold)]
     xy = jnp.concatenate([x[u], y[v]], axis=-1)
+
+    # Check if we want to adjust transparency.
+    scale_alpha_by_coupling = self._scale_alpha_by_coupling
+
+    # We can only adjust transparency if max(c) != min(c).
+    if scale_alpha_by_coupling:
+      min_matrix, max_matrix = jnp.min(c), jnp.max(c)
+      scale_alpha_by_coupling = max_matrix != min_matrix
+
     result = []
     for i in range(xy.shape[0]):
       strength = jnp.max(jnp.array(matrix.shape)) * c[i]
-      result.append((xy[i, [0, 2]], xy[i, [1, 3]], strength))
+      if scale_alpha_by_coupling:
+        normalized_strength = (c[i] - min_matrix) / (max_matrix - min_matrix)
+        alpha = self._alpha * float(normalized_strength)
+      else:
+        alpha = self._alpha
+
+      # Matplotlib's transparency is sensitive to numerical errors.
+      alpha = np.clip(alpha, 0.0, 1.0)
+
+      start, end = xy[i, [0, 2]], xy[i, [1, 3]]
+      result.append((start, end, strength, alpha))
+
     return result
 
-  def __call__(self, ot: Transport) -> List[plt.Artist]:
+  def __call__(self, ot: Transport) -> List["plt.Artist"]:
     """Plot 2-D couplings. Projects via PCA if data is higher dimensional."""
     x, y, sx, sy = self._scatter(ot)
     self._points_x = self.ax.scatter(
-        *x.T, s=sx, edgecolors='k', marker='o', label='x'
+        *x.T, s=sx, edgecolors="k", marker="o", label="x"
     )
     self._points_y = self.ax.scatter(
-        *y.T, s=sy, edgecolors='k', marker='X', label='y'
+        *y.T, s=sy, edgecolors="k", marker="X", label="y"
     )
     self.ax.legend(fontsize=15)
     if not self._show_lines:
       return []
 
     lines = self._mapping(x, y, ot.matrix)
     cmap = plt.get_cmap(self._cmap)
     self._lines = []
-    for start, end, strength in lines:
+    for start, end, strength, alpha in lines:
       line, = self.ax.plot(
           start,
           end,
           linewidth=0.5 + 4 * strength,
           color=cmap(strength),
           zorder=0,
-          alpha=0.7
+          alpha=alpha
       )
       self._lines.append(line)
     return [self._points_x, self._points_y] + self._lines
 
-  def update(self, ot: Transport) -> List[plt.Artist]:
+  def update(self, ot: Transport) -> List["plt.Artist"]:
     """Update a plot with a transport instance."""
     x, y, _, _ = self._scatter(ot)
     self._points_x.set_offsets(x)
     self._points_y.set_offsets(y)
     if not self._show_lines:
       return []
 
     new_lines = self._mapping(x, y, ot.matrix)
     cmap = plt.get_cmap(self._cmap)
     for line, new_line in zip(self._lines, new_lines):
-      start, end, strength = new_line
+      start, end, strength, alpha = new_line
+
       line.set_data(start, end)
       line.set_linewidth(0.5 + 4 * strength)
       line.set_color(cmap(strength))
+      line.set_alpha(alpha)
 
     # Maybe add new lines to the plot.
     num_lines = len(self._lines)
     num_to_plot = len(new_lines) if self._show_lines else 0
     for i in range(num_lines, num_to_plot):
-      start, end, strength = new_lines[i]
+      start, end, strength, alpha = new_lines[i]
+
       line, = self.ax.plot(
           start,
           end,
           linewidth=0.5 + 4 * strength,
           color=cmap(strength),
           zorder=0,
-          alpha=0.7
+          alpha=alpha
       )
       self._lines.append(line)
 
     self._lines = self._lines[:num_to_plot]  # Maybe remove some
     return [self._points_x, self._points_y] + self._lines
 
   def animate(
       self,
       transports: Sequence[Transport],
       frame_rate: float = 10.0
-  ) -> animation.FuncAnimation:
+  ) -> "animation.FuncAnimation":
     """Make an animation from several transports."""
     _ = self(transports[0])
     return animation.FuncAnimation(
         self.fig,
         lambda i: self.update(transports[i]),
         np.arange(0, len(transports)),
         init_func=lambda: self.update(transports[0]),
         interval=1000 / frame_rate,
         blit=True
     )
 
 
 def _barycenters(
-    ax: plt.Axes,
+    ax: "plt.Axes",
     y: jnp.ndarray,
     a: jnp.ndarray,
     b: jnp.ndarray,
     matrix: jnp.ndarray,
     scale: int = 200
-):
+) -> None:
   """Plot 2-D sinkhorn barycenters."""
   sa, sb = jnp.min(a) / scale, jnp.min(b) / scale
-  ax.scatter(*y.T, s=b / sb, edgecolors='k', marker='X', label='y')
+  ax.scatter(*y.T, s=b / sb, edgecolors="k", marker="X", label="y")
   tx = 1 / a[:, None] * jnp.matmul(matrix, y)
-  ax.scatter(*tx.T, s=a / sa, edgecolors='k', marker='X', label='T(x)')
+  ax.scatter(*tx.T, s=a / sa, edgecolors="k", marker="X", label="T(x)")
   ax.legend(fontsize=15)
 
 
 def barycentric_projections(
     arg: Union[Transport, jnp.ndarray],
     a: jnp.ndarray = None,
     b: jnp.ndarray = None,
     matrix: jnp.ndarray = None,
-    ax: Optional[plt.Axes] = None,
+    ax: Optional["plt.Axes"] = None,
     **kwargs
 ):
   """Plot the barycenters, from the Transport object or from arguments."""
   if ax is None:
     _, ax = plt.subplots(1, 1, figsize=(8, 5))
 
   if utils.is_jax_array(arg):
     if matrix is None:
-      raise ValueError('The `matrix` argument cannot be None.')
+      raise ValueError("The `matrix` argument cannot be None.")
 
     a = jnp.ones(matrix.shape[0]) / matrix.shape[0] if a is None else a
     b = jnp.ones(matrix.shape[1]) / matrix.shape[1] if b is None else b
     return _barycenters(ax, arg, a, b, matrix, **kwargs)
 
   if isinstance(arg, gromov_wasserstein.GWOutput):
     geom = arg.linear_state.geom
```

### Comparing `ott-jax-0.4.0/src/ott/tools/segment_sinkhorn.py` & `ott-jax-0.4.1/src/ott/tools/segment_sinkhorn.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-# Copyright 2022 The OTT Authors.
+# Copyright OTT-JAX
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-#     http://www.apache.org/licenses/LICENSE-2.0
+#   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Segmented sinkhorn utility."""
 from types import MappingProxyType
 from typing import Any, Mapping, Optional, Tuple
 
 import jax.numpy as jnp
 
 from ott.geometry import costs, pointcloud, segment
 from ott.problems.linear import linear_problem
@@ -34,30 +33,30 @@
     num_per_segment_x: Optional[Tuple[int, ...]] = None,
     num_per_segment_y: Optional[Tuple[int, ...]] = None,
     weights_x: Optional[jnp.ndarray] = None,
     weights_y: Optional[jnp.ndarray] = None,
     sinkhorn_kwargs: Mapping[str, Any] = MappingProxyType({}),
     **kwargs: Any
 ) -> jnp.ndarray:
-  """Compute `reg_ot_cost` between subsets of vectors described in `x` & `y`.
+  """Compute regularized OT cost between subsets of vectors in `x` and `y`.
 
   Helper function designed to compute Sinkhorn regularized OT cost between
   several point clouds of varying size, in parallel, using padding.
   In practice, The inputs `x` and `y` (and their weight vectors `weights_x` and
   `weights_y`) are assumed to be large weighted point clouds, that describe
   points taken from multiple measures. To extract several subsets of points, we
   provide two interfaces. The first interface assumes that a vector of id's is
   passed, describing for each point of `x` (resp. `y`) to which measure the
   point belongs to. The second interface assumes that `x` and `y` were simply
   formed by concatenating several measures contiguously, and that only indices
   that segment these groups are needed to recover them.
 
   For both interfaces, both `x` and `y` should contain the same total number of
   segments. Each segment will be padded as necessary, all segments rearranged as
-  a tensor, and :func:`jax.vmap` used to evaluate sinkhorn divergences in
+  a tensor, and :func:`jax.vmap` used to evaluate Sinkhorn divergences in
   parallel.
 
   Args:
     x: Array of input points, of shape `[num_x, feature]`.
       Multiple segments are held in this single array.
     y: Array of target points, of shape `[num_y, feature]`.
     num_segments: Number of segments contained in `x` and `y`.
@@ -80,25 +79,25 @@
     num_per_segment_y: **2nd interface** Number of points in each segment in
       `y`.
     weights_x: Weights of each input points, arranged in the same segmented
       order as `x`.
     weights_y: Weights of each input points, arranged in the same segmented
       order as `y`.
     sinkhorn_kwargs: Optionally a dict containing the keywords arguments for
-      calls to the `sinkhorn` function, called three times to evaluate for each
-      segment the sinkhorn regularized OT cost between `x`/`y`, `x`/`x`, and
-      `y`/`y` (except when `static_b` is `True`, in which case `y`/`y` is not
-      evaluated).
+      calls for the :class:`~ott.solvers.linear.sinkhorn.Sinkhorn` solver,
+      called three times to evaluate for each segment the Sinkhorn regularized
+      OT cost between `x`/`y`, `x`/`x`, and `y`/`y` (except when `static_b` is
+      `True`, in which case `y`/`y` is not evaluated).
     kwargs: keywords arguments passed to form
       :class:`~ott.geometry.pointcloud.PointCloud` geometry objects from the
       subsets of points and masses selected in `x` and `y`, possibly a
       :class:`~ott.geometry.costs.CostFn` or an entropy regularizer.
 
   Returns:
-    An array of sinkhorn reg_ot_cost for each segment.
+    An array of Sinkhorn regularized OT costs for each segment.
   """
   # instantiate padding vector
   dim = x.shape[1]
   if cost_fn is None:
     # default padder
     padding_vector = costs.CostFn._padder(dim=dim)
   else:
```

### Comparing `ott-jax-0.4.0/src/ott/tools/sinkhorn_divergence.py` & `ott-jax-0.4.1/src/ott/tools/sinkhorn_divergence.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-# Copyright 2022 Google LLC.
+# Copyright OTT-JAX
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-#     http://www.apache.org/licenses/LICENSE-2.0
+#   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Implements the sinkhorn divergence."""
 from types import MappingProxyType
 from typing import Any, List, Mapping, NamedTuple, Optional, Tuple, Type
 
 import jax.numpy as jnp
 
 from ott.geometry import costs, geometry, pointcloud, segment
 from ott.problems.linear import linear_problem, potentials
@@ -23,15 +22,15 @@
 
 __all__ = [
     "sinkhorn_divergence", "segment_sinkhorn_divergence",
     "SinkhornDivergenceOutput"
 ]
 
 
-class SinkhornDivergenceOutput(NamedTuple):
+class SinkhornDivergenceOutput(NamedTuple):  # noqa: D101
   divergence: float
   potentials: Tuple[List[jnp.ndarray], List[jnp.ndarray], List[jnp.ndarray]]
   geoms: Tuple[geometry.Geometry, geometry.Geometry, geometry.Geometry]
   errors: Tuple[Optional[jnp.ndarray], Optional[jnp.ndarray],
                 Optional[jnp.ndarray]]
   converged: Tuple[bool, bool, bool]
   a: jnp.ndarray
@@ -66,15 +65,15 @@
       :meth:`~ott.geometry.geometry.Geometry.prepare_divergences` that are
       specific to each geometry.
     a: the weight of each input point. The sum of all elements of `a` must
       match that of `b` to converge.
     b: the weight of each target point. The sum of all elements of `b` must
       match that of `a` to converge.
     sinkhorn_kwargs: keywords arguments for
-      :func:`~ott.solvers.linear.sinkhorn.sinkhorn` that is called twice
+      :class:`~ott.solvers.linear.sinkhorn.Sinkhorn` that is called twice
       if ``static_b = True`` else 3 times.
     static_b: if True, divergence of measure `b` against itself is **not**
       computed.
     share_epsilon: if True, enforces that the same epsilon regularizer is shared
       for all 2 or 3 terms of the Sinkhorn divergence. In that case, the epsilon
       will be by default that used when comparing x to y (contained in the first
       geometry). This flag is set to True by default, because in the default
@@ -116,15 +115,15 @@
     geometry_xx: geometry.Geometry,
     geometry_yy: Optional[geometry.Geometry],
     a: jnp.ndarray,
     b: jnp.ndarray,
     symmetric_sinkhorn: bool,
     **kwargs: Any,
 ) -> SinkhornDivergenceOutput:
-  """Compute the (unbalanced) sinkhorn divergence for the wrapper function.
+  """Compute the (unbalanced) Sinkhorn divergence for the wrapper function.
 
     This definition includes a correction depending on the total masses of each
     measure, as defined in :sejourne:19:, eq. 15.
 
   Args:
     geometry_xy: a Cost object able to apply kernels with a certain epsilon,
     between the views X and Y.
@@ -155,16 +154,18 @@
   # the symmetric parts should be marked as symmetric.
   kwargs_symmetric = kwargs.copy()
   if symmetric_sinkhorn:
     kwargs_symmetric.update(
         parallel_dual_updates=True,
         momentum=acceleration.Momentum(start=0, value=0.5),
         anderson=None,
-        # TODO(michalk8): implicit_diff
     )
+    implicit_diff = kwargs.get("implicit_diff", None)
+    if implicit_diff is not None:
+      kwargs_symmetric["implicit_diff"] = implicit_diff.replace(symmetric=True)
 
   out_xy = sinkhorn.solve(geometry_xy, a, b, **kwargs)
   out_xx = sinkhorn.solve(geometry_xx, a, a, **kwargs_symmetric)
   if geometry_yy is None:
     out_yy = sinkhorn.SinkhornOutput(errors=jnp.array([]), reg_ot_cost=0.0)
   else:
     out_yy = sinkhorn.solve(geometry_yy, b, b, **kwargs_symmetric)
@@ -196,30 +197,30 @@
     weights_y: Optional[jnp.ndarray] = None,
     sinkhorn_kwargs: Mapping[str, Any] = MappingProxyType({}),
     static_b: bool = False,
     share_epsilon: bool = True,
     symmetric_sinkhorn: bool = False,
     **kwargs: Any
 ) -> jnp.ndarray:
-  """Compute sinkhorn divergence between subsets of vectors given in `x` & `y`.
+  """Compute Sinkhorn divergence between subsets of vectors in `x` and `y`.
 
   Helper function designed to compute Sinkhorn divergences between several point
   clouds of varying size, in parallel, using padding for efficiency.
   In practice, The inputs `x` and `y` (and their weight vectors `weights_x` and
   `weights_y`) are assumed to be large weighted point clouds, that describe
   points taken from multiple measures. To extract several subsets of points, we
   provide two interfaces. The first interface assumes that a vector of id's is
   passed, describing for each point of `x` (resp. `y`) to which measure the
   point belongs to. The second interface assumes that `x` and `y` were simply
   formed by concatenating several measures contiguously, and that only indices
   that segment these groups are needed to recover them.
 
   For both interfaces, both `x` and `y` should contain the same total number of
   segments. Each segment will be padded as necessary, all segments rearranged as
-  a tensor, and `vmap` used to evaluate sinkhorn divergences in parallel.
+  a tensor, and `vmap` used to evaluate Sinkhorn divergences in parallel.
 
   Args:
     x: Array of input points, of shape `[num_x, feature]`.
       Multiple segments are held in this single array.
     y: Array of target points, of shape `[num_y, feature]`.
     num_segments: Number of segments contained in `x` and `y`.
       Providing this is required for JIT compilation to work,
@@ -243,15 +244,15 @@
       `y`.
     weights_x: Weights of each input points, arranged in the same segmented
       order as `x`.
     weights_y: Weights of each input points, arranged in the same segmented
       order as `y`.
     sinkhorn_kwargs: Optionally a dict containing the keywords arguments for
       calls to the `sinkhorn` function, called three times to evaluate for each
-      segment the sinkhorn regularized OT cost between `x`/`y`, `x`/`x`, and
+      segment the Sinkhorn regularized OT cost between `x`/`y`, `x`/`x`, and
       `y`/`y` (except when `static_b` is `True`, in which case `y`/`y` is not
       evaluated)
     static_b: if True, divergence of measure b against itself is NOT computed
     share_epsilon: if True, enforces that the same epsilon regularizer is shared
       for all 2 or 3 terms of the Sinkhorn divergence. In that case, the epsilon
       will be by default that used when comparing x to y (contained in the first
       geometry). This flag is set to True by default, because in the default
@@ -259,16 +260,17 @@
       matrix.
     symmetric_sinkhorn: Use Sinkhorn updates in Eq. 25 of :cite:`feydy:19` for
       symmetric terms comparing x/x and y/y.
     kwargs: keywords arguments passed to form
       :class:`~ott.geometry.pointcloud.PointCloud` geometry objects from the
       subsets of points and masses selected in `x` and `y`, this could be for
       instance entropy regularization float, scheduler or normalization.
+
   Returns:
-    An array of sinkhorn divergence values for each segment.
+    An array of Sinkhorn divergences for each segment.
   """
   # instantiate padding vector
   dim = x.shape[1]
   if cost_fn is None:
     # default padder
     padding_vector = costs.CostFn._padder(dim=dim)
   else:
```

### Comparing `ott-jax-0.4.0/src/ott/tools/soft_sort.py` & `ott-jax-0.4.1/src/ott/tools/soft_sort.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-# Copyright 2022 Google LLC.
+# Copyright OTT-JAX
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-#     http://www.apache.org/licenses/LICENSE-2.0
+#   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Soft sort operators."""
-
 import functools
 from typing import Any, Callable, Optional
 
 import jax
 import jax.numpy as jnp
 import numpy as np
 
@@ -52,15 +50,15 @@
   Returns:
     A jnp.ndarray<float> num_points x num_target transport matrix, from all
     inputs onto the sorted target.
   """
   shape = inputs.shape
   if len(shape) > 2 or (len(shape) == 2 and shape[1] != 1):
     raise ValueError(
-        f'Shape ({shape}) not supported. The input should be one-dimensional.'
+        f"Shape ({shape}) not supported. The input should be one-dimensional."
     )
 
   x = jnp.expand_dims(jnp.squeeze(inputs), axis=1)
   if squashing_fun is None:
     squashing_fun = lambda z: jax.nn.sigmoid((z - jnp.mean(z)) /
                                              (jnp.std(z) + 1e-10))
   x = squashing_fun(x)
@@ -106,16 +104,15 @@
   shrink = len(axis)
   result = jnp.reshape(result, inputs.shape[:-shrink] + result.shape[-1:])
 
   permutation = tuple(range(len(result.shape)))
   rank = len(result.shape) - 1
   axis = min(axis)
   permutation = permutation[:axis] + (rank,) + permutation[axis:-1]
-  result = jnp.transpose(result, permutation)
-  return result
+  return jnp.transpose(result, permutation)
 
 
 def _sort(
     inputs: jnp.ndarray, topk: int, num_targets: Optional[int], **kwargs: Any
 ) -> jnp.ndarray:
   """Apply the soft sort operator on a one dimensional array."""
   num_points = inputs.shape[0]
@@ -144,16 +141,16 @@
 ) -> jnp.ndarray:
   r"""Apply the soft sort operator on a given axis of the input.
 
   Args:
     inputs: jnp.ndarray<float> of any shape.
     axis: the axis on which to apply the operator.
     topk: if set to a positive value, the returned vector will only contain
-      the topk values. This also reduces the complexity of soft sorting.
-    num_targets: if topk is not specified, num_targets defines the number of
+      the top-k values. This also reduces the complexity of soft sorting.
+    num_targets: if top-k is not specified, num_targets defines the number of
       (composite) sorted values computed from the inputs (each value is a convex
       combination of values recorded in the inputs, provided in increasing
       order). If not specified, ``num_targets`` is set by default to be the size
       of the slices of the input that are sorted, i.e. the number of composite
       sorted values is equal to that of the inputs that are sorted.
     kwargs: keyword arguments passed on to lower level functions. Of interest
       to the user are ``squashing_fun``, which will redistribute the values in
@@ -184,15 +181,15 @@
 
 def ranks(
     inputs: jnp.ndarray,
     axis: int = -1,
     num_targets: Optional[int] = None,
     **kwargs: Any,
 ) -> jnp.ndarray:
-  r"""Apply the soft trank operator on input tensor.
+  r"""Apply the soft rank operator on input tensor.
 
   Args:
     inputs: a jnp.ndarray<float> of any shape.
     axis: the axis on which to apply the soft ranks operator.
     num_targets: num_targets defines the number of targets used to compute a
       composite ranks for each value in ``inputs``: that soft rank will be a
       convex combination of values in [0,...,``(num_targets-2)/num_targets``,1]
@@ -222,32 +219,33 @@
     **kwargs: Any,
 ) -> jnp.ndarray:
   r"""Apply the soft quantile operator on the input tensor.
 
   For instance:
 
   x = jax.random.uniform(rng, (1000,))
-  q = quantile(x, 0.5, 0.01)
+  q = quantile(x, level=0.5, weight=0.01)
 
   Then q will be computed as a mean over the 10 median points of x.
-  Therefore, there is a tradeoff between accuracy and gradient.
+  Therefore, there is a trade-off between accuracy and gradient.
 
   Args:
    inputs: a jnp.ndarray<float> of any shape.
    axis: the axis on which to apply the operator.
    level: the value of the quantile level to be computed. 0.5 for median.
    weight: the weight of the quantile in the transport problem.
    kwargs: keyword arguments passed on to lower level functions. Of interest
       to the user are ``squashing_fun``, which will redistribute the values in
       ``inputs`` to lie in [0,1] (sigmoid of whitened values by default) to
       solve the optimal transport problem; ``cost_fn``, used in ``PointCloud``,
       that defines the ground cost function to transport from ``inputs`` to the
       ``num_targets`` target values (squared Euclidean distance by default, see
       ``pointcloud.py`` for more details); ``epsilon`` values as well as other
       parameters to shape the ``sinkhorn`` algorithm.
+
   Returns:
     A jnp.ndarray, which has the same shape as the input, except on the give
     axis on which the dimension is 1.
   """
 
   def _quantile(
       inputs: jnp.ndarray, level: float, weight: float, **kwargs
@@ -296,26 +294,27 @@
       to the user are ``squashing_fun``, which will redistribute the values in
       ``inputs`` to lie in [0,1] (sigmoid of whitened values by default) to
       solve the optimal transport problem; ``cost_fn``, used in ``PointCloud``,
       that defines the ground cost function to transport from ``inputs`` to the
       ``num_targets`` target values (squared Euclidean distance by default, see
       ``pointcloud.py`` for more details); ``epsilon`` values as well as other
       parameters to shape the ``sinkhorn`` algorithm.
+
   Returns:
     A jnp.ndarray, which has the same shape as the input, except on the give
     axis on which the dimension is 1.
 
   Raises:
     A ValueError in case the weights and the targets are both set and not of
     compatible shapes.
   """
   if weights is not None and weights.shape != targets.shape:
     raise ValueError(
-        'The target weights and targets values should have the '
-        f'same shape: {targets.shape} != {weights.shape}'
+        "The target weights and targets values should have the "
+        f"same shape: {targets.shape} != {weights.shape}"
     )
   if weights is None:
     num_targets = targets.shape[0]
     weights = jnp.ones((num_targets,)) / num_targets
 
   op = _quantile_normalization
   return apply_on_axis(op, inputs, axis, targets, weights, **kwargs)
@@ -399,15 +398,15 @@
   does so by carrying out a `soft` concentration that is differentiable. The
   ``inputs`` values are first soft-sorted, resulting in ``num_levels`` values.
   In a second step, the ``inputs`` values are then provided again a composite
   value that is equal (for each) to a convex combination of those soft-sorted
   values using the transportation matrix. As the regularization parameter
   ``epsilon`` of regularized optimal transport goes to 0, this operator recovers
   the expected behavior of quantization, namely each value in ``inputs`` is
-  assigned a single level. When using ``epsilon>0`` the bheaviour is similar but
+  assigned a single level. When using ``epsilon>0`` the behavior is similar but
   differentiable.
 
   Args:
     inputs: the inputs as a jnp.ndarray[batch, dim].
     num_levels: number of levels available to quantize the signal.
     axis: axis along which quantization is carried out.
     kwargs: keyword arguments passed on to lower level functions. Of interest
```

### Comparing `ott-jax-0.4.0/src/ott_jax.egg-info/PKG-INFO` & `ott-jax-0.4.1/src/ott_jax.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ott-jax
-Version: 0.4.0
+Version: 0.4.1
 Summary: Optimal Transport Tools in JAX.
 Author-email: OTT team <optimal.transport.tools@gmail.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -226,15 +226,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
-Provides-Extra: experimental
 Provides-Extra: docs
 License-File: LICENSE
 
 <img src="https://raw.githubusercontent.com/ott-jax/ott/main/docs/_static/images/logoOTT.png" width="10%" alt="logo">
 
 # Optimal Transport Tools (OTT)
 [![Downloads](https://static.pepy.tech/badge/ott-jax)](https://pypi.org/project/ott-jax/)
@@ -242,35 +241,31 @@
 [![Docs](https://img.shields.io/readthedocs/ott-jax/latest)](https://ott-jax.readthedocs.io/en/latest/)
 [![Coverage](https://img.shields.io/codecov/c/github/ott-jax/ott/main)](https://app.codecov.io/gh/ott-jax/ott)
 
 **See the [full documentation](https://ott-jax.readthedocs.io/en/latest/).**
 
 ## What is OTT-JAX?
 A ``JAX`` powered library to compute optimal transport at scale and on accelerators, ``OTT-JAX`` includes the fastest
-implementation of the Sinkhorn algorithm you will find around. We have implemented all tweaks (scheduling,
-acceleration, initializations) and extensions (low-rank), that can be used directly, or within more advanced problems
+implementation of the Sinkhorn algorithm you will find around. We have implemented all tweaks (scheduling, momentum, acceleration, initializations) and extensions (low-rank, entropic maps). They can be used directly between two datasets, or within more advanced problems
 (Gromov-Wasserstein, barycenters). Some of ``JAX`` features, including
 [JIT](https://jax.readthedocs.io/en/latest/notebooks/quickstart.html#Using-jit-to-speed-up-functions),
 [auto-vectorization](https://jax.readthedocs.io/en/latest/notebooks/quickstart.html#Auto-vectorization-with-vmap) and
 [implicit differentiation](https://jax.readthedocs.io/en/latest/notebooks/Custom_derivative_rules_for_Python_code.html)
-work towards the goal of having end-to-end differentiable outputs. OTT-JAX is developed by a team of researchers
-from Apple, Google, Meta and many academic contributors, including TU München, Oxford, ENSAE/IP Paris and the
-Hebrew University.
+work towards the goal of having end-to-end differentiable outputs. OTT-JAX is led by a team of researchers at Apple, with contributions from Google and Meta researchers, as well as many academic partners, including TU München, Oxford, ENSAE/IP Paris, ENS Paris and the Hebrew University.
 
 ## Installation
 Install ``OTT-JAX`` from [PyPI](https://pypi.org/project/ott-jax/) as:
 ```bash
 pip install ott-jax
 ```
 or with ``conda`` via [conda-forge](https://anaconda.org/conda-forge/ott-jax) as:
 ```bash
 conda install -c conda-forge ott-jax
 ```
 
-
 ## What is optimal transport?
 Optimal transport can be loosely described as the branch of mathematics and optimization that studies
 *matching problems*: given two families of points, and a cost function on pairs of points, find a "good" (low cost) way
 to associate bijectively to every point in the first family another in the second.
 
 Such problems appear in all areas of science, are easy to describe, yet hard to solve. Indeed, while matching optimally
 two sets of $n$ points using a pairwise cost can be solved with the
@@ -306,25 +301,27 @@
 prob = linear_problem.LinearProblem(geom, a, b)
 
 solver = sinkhorn.Sinkhorn()
 out = solver(prob)
 ```
 
 The call to `solver(prob)` above works out the optimal transport solution. The `out` object contains a transport matrix
-(here of size $12\times 14$) that quantifies a `link strength` between each point of the first point cloud, to one or
+(here of size $12\times 14$) that quantifies the association strength between each point of the first point cloud, to one or
 more points from the second, as illustrated in the plot below. We provide more flexibility to define custom cost
 functions, objectives, and solvers, as detailed in the [full documentation](https://ott-jax.readthedocs.io/en/latest/).
 
-![obtained coupling](https://raw.githubusercontent.com/ott-jax/ott/main/images/couplings.png)
+![obtained coupling](https://raw.githubusercontent.com/ott-jax/ott/main/docs/_static/images/couplings.png)
 
 ## Citation
 If you have found this work useful, please consider citing this reference:
 
 ```
 @article{cuturi2022optimal,
   title={Optimal Transport Tools (OTT): A JAX Toolbox for all things Wasserstein},
   author={Cuturi, Marco and Meng-Papaxanthos, Laetitia and Tian, Yingtao and Bunne, Charlotte and
           Davis, Geoff and Teboul, Olivier},
   journal={arXiv preprint arXiv:2201.12324},
   year={2022}
 }
 ```
+## See also
+The [moscot](https://moscot.readthedocs.io/en/latest/index.html) package for OT analysis of multi-omics data also uses OTT as a backbone.
```

### Comparing `ott-jax-0.4.0/src/ott_jax.egg-info/SOURCES.txt` & `ott-jax-0.4.1/src/ott_jax.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 .codecov.yml
 .editorconfig
-.flake8
 .gitignore
 .pre-commit-config.yaml
 .readthedocs.yaml
-CODE_OF_CONDUCT.md
-CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
 environment.yml
 pyproject.toml
+setup.py
 src/ott/__init__.py
 src/ott/_version.py
+src/ott/py.typed
 src/ott/types.py
 src/ott/utils.py
 src/ott/geometry/__init__.py
 src/ott/geometry/costs.py
 src/ott/geometry/epsilon_scheduler.py
 src/ott/geometry/geometry.py
 src/ott/geometry/graph.py
@@ -29,15 +28,14 @@
 src/ott/initializers/linear/initializers.py
 src/ott/initializers/linear/initializers_lr.py
 src/ott/initializers/nn/__init__.py
 src/ott/initializers/nn/initializers.py
 src/ott/initializers/quadratic/__init__.py
 src/ott/initializers/quadratic/initializers.py
 src/ott/math/__init__.py
-src/ott/math/decomposition.py
 src/ott/math/fixed_point_loop.py
 src/ott/math/matrix_square_root.py
 src/ott/math/unbalanced_functions.py
 src/ott/math/utils.py
 src/ott/problems/__init__.py
 src/ott/problems/linear/__init__.py
 src/ott/problems/linear/barycenter_problem.py
@@ -52,14 +50,15 @@
 src/ott/solvers/__init__.py
 src/ott/solvers/was_solver.py
 src/ott/solvers/linear/__init__.py
 src/ott/solvers/linear/acceleration.py
 src/ott/solvers/linear/continuous_barycenter.py
 src/ott/solvers/linear/discrete_barycenter.py
 src/ott/solvers/linear/implicit_differentiation.py
+src/ott/solvers/linear/lineax_implicit.py
 src/ott/solvers/linear/sinkhorn.py
 src/ott/solvers/linear/sinkhorn_lr.py
 src/ott/solvers/nn/__init__.py
 src/ott/solvers/nn/conjugate_solvers.py
 src/ott/solvers/nn/layers.py
 src/ott/solvers/nn/models.py
 src/ott/solvers/nn/neuraldual.py
```

