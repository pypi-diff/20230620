# Comparing `tmp/dynamax-0.1.0.tar.gz` & `tmp/dynamax-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dynamax-0.1.0.tar", last modified: Mon Nov 14 16:58:37 2022, max compression
+gzip compressed data, was "dist/dynamax-0.1.1.tar", last modified: Tue Jun 20 16:52:04 2023, max compression
```

## Comparing `dynamax-0.1.0.tar` & `dynamax-0.1.1.tar`

### file list

```diff
@@ -1,79 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:58:37.000000 dynamax-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-11-14 16:58:25.000000 dynamax-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     8730 2022-11-14 16:58:37.000000 dynamax-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6828 2022-11-14 16:58:25.000000 dynamax-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:58:37.000000 dynamax-0.1.0/dynamax/
--rw-r--r--   0 runner    (1001) docker     (121)      265 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-11-14 16:58:37.000000 dynamax-0.1.0/dynamax/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:58:37.000000 dynamax-0.1.0/dynamax/generalized_gaussian_ssm/
--rw-r--r--   0 runner    (1001) docker     (121)      570 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/generalized_gaussian_ssm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15349 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/generalized_gaussian_ssm/inference.py
--rw-r--r--   0 runner    (1001) docker     (121)     3189 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/generalized_gaussian_ssm/inference_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     4937 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/generalized_gaussian_ssm/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     4487 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/generalized_gaussian_ssm/models_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:58:37.000000 dynamax-0.1.0/dynamax/hidden_markov_model/
--rw-r--r--   0 runner    (1001) docker     (121)     1918 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/hidden_markov_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    25898 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/hidden_markov_model/inference.py
--rw-r--r--   0 runner    (1001) docker     (121)    11956 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/hidden_markov_model/inference_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:58:37.000000 dynamax-0.1.0/dynamax/hidden_markov_model/models/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/hidden_markov_model/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    29011 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/hidden_markov_model/models/abstractions.py
--rw-r--r--   0 runner    (1001) docker     (121)    12216 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/hidden_markov_model/models/arhmm.py
--rw-r--r--   0 runner    (1001) docker     (121)     8510 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/hidden_markov_model/models/bernoulli_hmm.py
--rw-r--r--   0 runner    (1001) docker     (121)     8696 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/hidden_markov_model/models/categorical_glm_hmm.py
--rw-r--r--   0 runner    (1001) docker     (121)     9222 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/hidden_markov_model/models/categorical_hmm.py
--rw-r--r--   0 runner    (1001) docker     (121)    54269 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/hidden_markov_model/models/gaussian_hmm.py
--rw-r--r--   0 runner    (1001) docker     (121)    27438 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/hidden_markov_model/models/gmm_hmm.py
--rw-r--r--   0 runner    (1001) docker     (121)     2803 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/hidden_markov_model/models/initial.py
--rw-r--r--   0 runner    (1001) docker     (121)    10997 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/hidden_markov_model/models/linreg_hmm.py
--rw-r--r--   0 runner    (1001) docker     (121)     8756 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/hidden_markov_model/models/logreg_hmm.py
--rw-r--r--   0 runner    (1001) docker     (121)     8223 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/hidden_markov_model/models/multinomial_hmm.py
--rw-r--r--   0 runner    (1001) docker     (121)     8254 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/hidden_markov_model/models/poisson_hmm.py
--rw-r--r--   0 runner    (1001) docker     (121)     8521 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/hidden_markov_model/models/test_models.py
--rw-r--r--   0 runner    (1001) docker     (121)     3291 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/hidden_markov_model/models/transitions.py
--rw-r--r--   0 runner    (1001) docker     (121)     4312 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/hidden_markov_model/parallel_inference.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:58:37.000000 dynamax-0.1.0/dynamax/linear_gaussian_ssm/
--rw-r--r--   0 runner    (1001) docker     (121)     1292 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/linear_gaussian_ssm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:58:37.000000 dynamax-0.1.0/dynamax/linear_gaussian_ssm/demos/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/linear_gaussian_ssm/demos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16006 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/linear_gaussian_ssm/inference.py
--rw-r--r--   0 runner    (1001) docker     (121)     4755 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/linear_gaussian_ssm/inference_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    16703 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/linear_gaussian_ssm/info_inference.py
--rw-r--r--   0 runner    (1001) docker     (121)     6313 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/linear_gaussian_ssm/info_inference_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    25526 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/linear_gaussian_ssm/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     1061 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/linear_gaussian_ssm/models_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     6457 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/linear_gaussian_ssm/parallel_inference.py
--rw-r--r--   0 runner    (1001) docker     (121)     2511 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/linear_gaussian_ssm/parallel_inference_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:58:37.000000 dynamax-0.1.0/dynamax/nonlinear_gaussian_ssm/
--rw-r--r--   0 runner    (1001) docker     (121)      662 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/nonlinear_gaussian_ssm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9222 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/nonlinear_gaussian_ssm/inference_ekf.py
--rw-r--r--   0 runner    (1001) docker     (121)     2699 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/nonlinear_gaussian_ssm/inference_ekf_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     7426 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/nonlinear_gaussian_ssm/inference_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    10136 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/nonlinear_gaussian_ssm/inference_ukf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1253 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/nonlinear_gaussian_ssm/inference_ukf_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     3989 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/nonlinear_gaussian_ssm/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     7209 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/nonlinear_gaussian_ssm/sarkka_lib.py
--rw-r--r--   0 runner    (1001) docker     (121)     4897 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/parameters.py
--rw-r--r--   0 runner    (1001) docker     (121)     5304 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/parameters_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    18620 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/ssm.py
--rw-r--r--   0 runner    (1001) docker     (121)      266 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/types.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:58:37.000000 dynamax-0.1.0/dynamax/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1111 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/utils/bijectors.py
--rw-r--r--   0 runner    (1001) docker     (121)    15052 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/utils/distributions.py
--rw-r--r--   0 runner    (1001) docker     (121)     6865 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/utils/distributions_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     4119 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/utils/optimize.py
--rw-r--r--   0 runner    (1001) docker     (121)     3084 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/utils/plotting.py
--rw-r--r--   0 runner    (1001) docker     (121)     6178 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1507 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/utils/utils_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      621 2022-11-14 16:58:25.000000 dynamax-0.1.0/dynamax/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:58:37.000000 dynamax-0.1.0/dynamax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8730 2022-11-14 16:58:37.000000 dynamax-0.1.0/dynamax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2590 2022-11-14 16:58:37.000000 dynamax-0.1.0/dynamax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-14 16:58:37.000000 dynamax-0.1.0/dynamax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      567 2022-11-14 16:58:37.000000 dynamax-0.1.0/dynamax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-11-14 16:58:37.000000 dynamax-0.1.0/dynamax.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-11-14 16:58:25.000000 dynamax-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1021 2022-11-14 16:58:37.000000 dynamax-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      585 2022-11-14 16:58:25.000000 dynamax-0.1.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    83607 2022-11-14 16:58:25.000000 dynamax-0.1.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:52:04.000000 dynamax-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-20 16:51:55.000000 dynamax-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8730 2023-06-20 16:52:04.000000 dynamax-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-06-20 16:51:55.000000 dynamax-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:52:04.000000 dynamax-0.1.1/dynamax/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-20 16:52:04.000000 dynamax-0.1.1/dynamax/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:52:04.000000 dynamax-0.1.1/dynamax/generalized_gaussian_ssm/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/generalized_gaussian_ssm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:52:04.000000 dynamax-0.1.1/dynamax/generalized_gaussian_ssm/demos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/generalized_gaussian_ssm/demos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/generalized_gaussian_ssm/demos/cmgf_logreg_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15349 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/generalized_gaussian_ssm/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/generalized_gaussian_ssm/inference_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/generalized_gaussian_ssm/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/generalized_gaussian_ssm/models_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:52:04.000000 dynamax-0.1.1/dynamax/hidden_markov_model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/hidden_markov_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26282 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/hidden_markov_model/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11956 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/hidden_markov_model/inference_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:52:04.000000 dynamax-0.1.1/dynamax/hidden_markov_model/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/hidden_markov_model/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29011 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/hidden_markov_model/models/abstractions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12216 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/hidden_markov_model/models/arhmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8510 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/hidden_markov_model/models/bernoulli_hmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8696 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/hidden_markov_model/models/categorical_glm_hmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9222 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/hidden_markov_model/models/categorical_hmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7085 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/hidden_markov_model/models/gamma_hmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54269 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/hidden_markov_model/models/gaussian_hmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27438 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/hidden_markov_model/models/gmm_hmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/hidden_markov_model/models/initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/hidden_markov_model/models/linreg_hmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8756 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/hidden_markov_model/models/logreg_hmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/hidden_markov_model/models/multinomial_hmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8254 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/hidden_markov_model/models/poisson_hmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/hidden_markov_model/models/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/hidden_markov_model/models/transitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/hidden_markov_model/parallel_inference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:52:04.000000 dynamax-0.1.1/dynamax/linear_gaussian_ssm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/linear_gaussian_ssm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:52:04.000000 dynamax-0.1.1/dynamax/linear_gaussian_ssm/demos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/linear_gaussian_ssm/demos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10260 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/linear_gaussian_ssm/demos/kf_linreg_jax_vs_pt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21300 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/linear_gaussian_ssm/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/linear_gaussian_ssm/inference_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16703 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/linear_gaussian_ssm/info_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6313 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/linear_gaussian_ssm/info_inference_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25526 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/linear_gaussian_ssm/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/linear_gaussian_ssm/models_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/linear_gaussian_ssm/parallel_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/linear_gaussian_ssm/parallel_inference_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:52:04.000000 dynamax-0.1.1/dynamax/nonlinear_gaussian_ssm/
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/nonlinear_gaussian_ssm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12245 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/nonlinear_gaussian_ssm/inference_ekf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/nonlinear_gaussian_ssm/inference_ekf_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/nonlinear_gaussian_ssm/inference_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10757 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/nonlinear_gaussian_ssm/inference_ukf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/nonlinear_gaussian_ssm/inference_ukf_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/nonlinear_gaussian_ssm/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7209 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/nonlinear_gaussian_ssm/sarkka_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4897 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/parameters_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18620 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/ssm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:52:04.000000 dynamax-0.1.1/dynamax/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/utils/bijectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15052 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/utils/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6865 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/utils/distributions_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/utils/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/utils/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/utils/utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-20 16:51:55.000000 dynamax-0.1.1/dynamax/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:52:04.000000 dynamax-0.1.1/dynamax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8730 2023-06-20 16:52:04.000000 dynamax-0.1.1/dynamax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-06-20 16:52:04.000000 dynamax-0.1.1/dynamax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:52:04.000000 dynamax-0.1.1/dynamax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-20 16:52:04.000000 dynamax-0.1.1/dynamax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-20 16:52:04.000000 dynamax-0.1.1/dynamax.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-20 16:51:55.000000 dynamax-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-20 16:52:04.000000 dynamax-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-20 16:51:55.000000 dynamax-0.1.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-06-20 16:51:55.000000 dynamax-0.1.1/versioneer.py
```

### Comparing `dynamax-0.1.0/PKG-INFO` & `dynamax-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamax
-Version: 0.1.0
+Version: 0.1.1
 Summary: Dynamic State Space Models in JAX.
 Home-page: https://github.com/probml/dynamax
 Author: Peter Chang, Giles Harper-Donnelly, Aleyna Kara, Xinglong Li, Scott Linderman, Kevin Murphy
 License: MIT
 Description: # Welcome to DYNAMAX!
         
         ![Logo](https://raw.githubusercontent.com/probml/dynamax/main/logo/logo.gif)
```

### Comparing `dynamax-0.1.0/README.md` & `dynamax-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `dynamax-0.1.0/dynamax/generalized_gaussian_ssm/__init__.py` & `dynamax-0.1.1/dynamax/generalized_gaussian_ssm/__init__.py`

 * *Files identical despite different names*

### Comparing `dynamax-0.1.0/dynamax/generalized_gaussian_ssm/inference.py` & `dynamax-0.1.1/dynamax/generalized_gaussian_ssm/inference.py`

 * *Files identical despite different names*

### Comparing `dynamax-0.1.0/dynamax/generalized_gaussian_ssm/inference_test.py` & `dynamax-0.1.1/dynamax/generalized_gaussian_ssm/inference_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 import jax.numpy as jnp
+import jax.random as jr
 
 from dynamax.generalized_gaussian_ssm.models import ParamsGGSSM
 from dynamax.generalized_gaussian_ssm.inference import conditional_moments_gaussian_smoother, EKFIntegrals, UKFIntegrals
 from dynamax.nonlinear_gaussian_ssm.inference_ekf import extended_kalman_smoother
 from dynamax.nonlinear_gaussian_ssm.inference_ukf import unscented_kalman_smoother, UKFHyperParams
 from dynamax.nonlinear_gaussian_ssm.inference_test_utils import random_nlgssm_args
 from dynamax.utils.utils import has_tpu
 
+
 if has_tpu():
     def allclose(x, y):
-        print(jnp.max(abs(x - y)))
-        return True # hack!
+        print(jnp.max(x-y))
+        #return jnp.allclose(x, y, atol=1e-1)
+        return True # hack !!!
 else:
     def allclose(x,y):
-        print(jnp.max(abs(x-y)))
-        return jnp.allclose(x, y, atol=1e-1)
+        m = jnp.max(x-y)
+        if jnp.abs(m) > 1e-1:
+            print(m)
+            return False
+        else:
+            return True
 
 
-def test_ekf(key=0, num_timesteps=15):
+def ekf(key=0, num_timesteps=15):
     nlgssm_args, _, emissions = random_nlgssm_args(key=key, num_timesteps=num_timesteps)
 
     # Run EKF from dynamax.ekf
     ekf_post = extended_kalman_smoother(nlgssm_args, emissions)
     # Run EKF as a GGF
     ekf_params = ParamsGGSSM(
         initial_mean=nlgssm_args.initial_mean,
@@ -36,14 +43,20 @@
     # Compare filter and smoother results
     assert allclose(ekf_post.marginal_loglik, ggf_post.marginal_loglik)
     assert allclose(ekf_post.filtered_means, ggf_post.filtered_means)
     assert allclose(ekf_post.filtered_covariances, ggf_post.filtered_covariances)
     assert allclose(ekf_post.smoothed_means, ggf_post.smoothed_means)
     assert allclose(ekf_post.smoothed_covariances, ggf_post.smoothed_covariances)
 
+def skip_test_ekf():
+    key = jr.PRNGKey(0)
+    keys = jr.split(key, 5)
+    for key in keys:
+        ekf(key, num_timesteps=15)
+
 
 def test_ukf(key=1, num_timesteps=15):
     nlgssm_args, _, emissions = random_nlgssm_args(key=key, num_timesteps=num_timesteps)
     hyperparams = UKFHyperParams()
 
     # Run UKF from dynamax.ukf
     ukf_post = unscented_kalman_smoother(nlgssm_args, emissions, hyperparams)
```

### Comparing `dynamax-0.1.0/dynamax/generalized_gaussian_ssm/models.py` & `dynamax-0.1.1/dynamax/generalized_gaussian_ssm/models.py`

 * *Files identical despite different names*

### Comparing `dynamax-0.1.0/dynamax/generalized_gaussian_ssm/models_test.py` & `dynamax-0.1.1/dynamax/generalized_gaussian_ssm/models_test.py`

 * *Files identical despite different names*

### Comparing `dynamax-0.1.0/dynamax/hidden_markov_model/__init__.py` & `dynamax-0.1.1/dynamax/hidden_markov_model/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from dynamax.hidden_markov_model.models.abstractions import HMM, HMMEmissions, HMMInitialState, HMMTransitions, HMMParameterSet, HMMPropertySet
 from dynamax.hidden_markov_model.models.arhmm import LinearAutoregressiveHMM
 from dynamax.hidden_markov_model.models.bernoulli_hmm import BernoulliHMM
 from dynamax.hidden_markov_model.models.categorical_glm_hmm import CategoricalRegressionHMM
 from dynamax.hidden_markov_model.models.categorical_hmm import CategoricalHMM
+from dynamax.hidden_markov_model.models.gamma_hmm import GammaHMM
 from dynamax.hidden_markov_model.models.gaussian_hmm import GaussianHMM, DiagonalGaussianHMM, SphericalGaussianHMM, SharedCovarianceGaussianHMM, LowRankGaussianHMM
 from dynamax.hidden_markov_model.models.gmm_hmm import GaussianMixtureHMM, DiagonalGaussianMixtureHMM
 from dynamax.hidden_markov_model.models.linreg_hmm import LinearRegressionHMM
 from dynamax.hidden_markov_model.models.logreg_hmm import LogisticRegressionHMM
 from dynamax.hidden_markov_model.models.multinomial_hmm import MultinomialHMM
 from dynamax.hidden_markov_model.models.poisson_hmm import PoissonHMM
```

### Comparing `dynamax-0.1.0/dynamax/hidden_markov_model/inference.py` & `dynamax-0.1.1/dynamax/hidden_markov_model/inference.py`

 * *Files 2% similar despite different names*

```diff
@@ -285,15 +285,17 @@
         # Unpack the inputs
         smoothed_probs_next = carry
         t, filtered_probs, predicted_probs_next = args
 
         A = get_trans_mat(transition_matrix, transition_fn, t)
 
         # Fold in the next state (Eq. 8.2 of Saarka, 2013)
-        relative_probs_next = smoothed_probs_next / predicted_probs_next
+        # If hard 0. in predicted_probs_next, set relative_probs_next as 0. to avoid NaN values
+        relative_probs_next = jnp.where(jnp.isclose(predicted_probs_next, 0.0), 0.0,
+                                        smoothed_probs_next / predicted_probs_next)
         smoothed_probs = filtered_probs * (A @ relative_probs_next)
         smoothed_probs /= smoothed_probs.sum()
 
         return smoothed_probs, smoothed_probs
 
     # Run the HMM smoother
     carry = filtered_probs[-1]
@@ -547,15 +549,17 @@
     def _step(carry, args):
         filtered_probs, smoothed_probs_next, predicted_probs_next, t = args
 
         # Get parameters for time t
         A = _get_params(transition_matrix, 2, t)
 
         # Compute smoothed transition probabilities (Eq. 8.4 of Saarka, 2013)
-        relative_probs_next = smoothed_probs_next / predicted_probs_next
+        # If hard 0. in predicted_probs_next, set relative_probs_next as 0. to avoid NaN values
+        relative_probs_next = jnp.where(jnp.isclose(predicted_probs_next, 0.0), 0.0,
+                                        smoothed_probs_next / predicted_probs_next)
         smoothed_trans_probs = filtered_probs[:, None] * A * relative_probs_next[None, :]
         smoothed_trans_probs /= smoothed_trans_probs.sum()
         return carry + smoothed_trans_probs, None
 
     # Initialize the recursion
     num_states = transition_matrix.shape[-1]
     num_timesteps = len(hmm_posterior.filtered_probs)
```

### Comparing `dynamax-0.1.0/dynamax/hidden_markov_model/inference_test.py` & `dynamax-0.1.1/dynamax/hidden_markov_model/inference_test.py`

 * *Files identical despite different names*

### Comparing `dynamax-0.1.0/dynamax/hidden_markov_model/models/abstractions.py` & `dynamax-0.1.1/dynamax/hidden_markov_model/models/abstractions.py`

 * *Files identical despite different names*

### Comparing `dynamax-0.1.0/dynamax/hidden_markov_model/models/arhmm.py` & `dynamax-0.1.1/dynamax/hidden_markov_model/models/arhmm.py`

 * *Files identical despite different names*

### Comparing `dynamax-0.1.0/dynamax/hidden_markov_model/models/bernoulli_hmm.py` & `dynamax-0.1.1/dynamax/hidden_markov_model/models/bernoulli_hmm.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
             elif method.lower() == "kmeans":
                 raise NotImplementedError("kmeans initialization is not yet implemented!")
             else:
                 raise Exception("invalid initialization method: {}".format(method))
         else:
             assert emission_probs.shape == (self.num_states, self.emission_dim)
             assert jnp.all(emission_probs >= 0)
-            assert jnp.all(emission_probs <= 0)
+            assert jnp.all(emission_probs <= 1)
 
         # Add parameters to the dictionary
         params = ParamsBernoulliHMMEmissions(probs=emission_probs)
         props = ParamsBernoulliHMMEmissions(probs=ParameterProperties(constrainer=tfb.Sigmoid()))
         return params, props
 
     def collect_suff_stats(self, params, posterior, emissions, inputs=None):
```

### Comparing `dynamax-0.1.0/dynamax/hidden_markov_model/models/categorical_glm_hmm.py` & `dynamax-0.1.1/dynamax/hidden_markov_model/models/categorical_glm_hmm.py`

 * *Files identical despite different names*

### Comparing `dynamax-0.1.0/dynamax/hidden_markov_model/models/categorical_hmm.py` & `dynamax-0.1.1/dynamax/hidden_markov_model/models/categorical_hmm.py`

 * *Files identical despite different names*

### Comparing `dynamax-0.1.0/dynamax/hidden_markov_model/models/gaussian_hmm.py` & `dynamax-0.1.1/dynamax/hidden_markov_model/models/gaussian_hmm.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,15 +170,15 @@
             km = KMeans(self.num_states).fit(emissions.reshape(-1, self.emission_dim))
             _emission_means = jnp.array(km.cluster_centers_)
             _emission_scale_diags = jnp.ones((self.num_states, self.emission_dim))
 
         elif method.lower() == "prior":
             this_key, key = jr.split(key)
             prior = NormalInverseGamma(self.emission_prior_mean, self.emission_prior_mean_conc,
-                                       self.emission_prior_scale, self.emission_prior_conc)
+                                       self.emission_prior_conc, self.emission_prior_scale)
             (_emission_vars, _emission_means) = prior.sample(seed=this_key, sample_shape=(self.num_states,))
             _emission_scale_diags = jnp.sqrt(_emission_vars)
 
         else:
             raise Exception("Invalid initialization method: {}".format(method))
 
         # Only use the values above if the user hasn't specified their own
```

### Comparing `dynamax-0.1.0/dynamax/hidden_markov_model/models/gmm_hmm.py` & `dynamax-0.1.1/dynamax/hidden_markov_model/models/gmm_hmm.py`

 * *Files identical despite different names*

### Comparing `dynamax-0.1.0/dynamax/hidden_markov_model/models/initial.py` & `dynamax-0.1.1/dynamax/hidden_markov_model/models/initial.py`

 * *Files identical despite different names*

### Comparing `dynamax-0.1.0/dynamax/hidden_markov_model/models/linreg_hmm.py` & `dynamax-0.1.1/dynamax/hidden_markov_model/models/linreg_hmm.py`

 * *Files identical despite different names*

### Comparing `dynamax-0.1.0/dynamax/hidden_markov_model/models/logreg_hmm.py` & `dynamax-0.1.1/dynamax/hidden_markov_model/models/logreg_hmm.py`

 * *Files identical despite different names*

### Comparing `dynamax-0.1.0/dynamax/hidden_markov_model/models/multinomial_hmm.py` & `dynamax-0.1.1/dynamax/hidden_markov_model/models/multinomial_hmm.py`

 * *Files identical despite different names*

### Comparing `dynamax-0.1.0/dynamax/hidden_markov_model/models/poisson_hmm.py` & `dynamax-0.1.1/dynamax/hidden_markov_model/models/poisson_hmm.py`

 * *Files identical despite different names*

### Comparing `dynamax-0.1.0/dynamax/hidden_markov_model/models/test_models.py` & `dynamax-0.1.1/dynamax/hidden_markov_model/models/test_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 NUM_TIMESTEPS = 50
 
 CONFIGS = [
     (models.BernoulliHMM, dict(num_states=4, emission_dim=3), None),
     (models.CategoricalHMM, dict(num_states=4, emission_dim=3, num_classes=5), None),
     (models.CategoricalRegressionHMM, dict(num_states=4, num_classes=3, input_dim=5), jnp.ones((NUM_TIMESTEPS, 5))),
+    (models.GammaHMM, dict(num_states=4), None),
     (models.GaussianHMM, dict(num_states=4, emission_dim=3, emission_prior_concentration=1.0, emission_prior_scale=1.0), None),
     (models.DiagonalGaussianHMM, dict(num_states=4, emission_dim=3), None),
     (models.SphericalGaussianHMM, dict(num_states=4, emission_dim=3), None),
     (models.SharedCovarianceGaussianHMM, dict(num_states=4, emission_dim=3), None),
     (models.LowRankGaussianHMM, dict(num_states=4, emission_dim=3, emission_rank=1), None),
     (models.GaussianMixtureHMM, dict(num_states=4, num_components=2, emission_dim=3, emission_prior_mean_concentration=1.0), None),
     (models.DiagonalGaussianMixtureHMM, dict(num_states=4, num_components=2, emission_dim=3, emission_prior_mean_concentration=1.0), None),
```

### Comparing `dynamax-0.1.0/dynamax/hidden_markov_model/models/transitions.py` & `dynamax-0.1.1/dynamax/hidden_markov_model/models/transitions.py`

 * *Files identical despite different names*

### Comparing `dynamax-0.1.0/dynamax/hidden_markov_model/parallel_inference.py` & `dynamax-0.1.1/dynamax/hidden_markov_model/parallel_inference.py`

 * *Files identical despite different names*

### Comparing `dynamax-0.1.0/dynamax/linear_gaussian_ssm/__init__.py` & `dynamax-0.1.1/dynamax/linear_gaussian_ssm/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,18 +3,20 @@
 from dynamax.linear_gaussian_ssm.inference import ParamsLGSSMDynamics
 from dynamax.linear_gaussian_ssm.inference import ParamsLGSSMEmissions
 from dynamax.linear_gaussian_ssm.inference import PosteriorGSSMFiltered
 from dynamax.linear_gaussian_ssm.inference import PosteriorGSSMSmoothed
 from dynamax.linear_gaussian_ssm.inference import lgssm_filter
 from dynamax.linear_gaussian_ssm.inference import lgssm_smoother
 from dynamax.linear_gaussian_ssm.inference import lgssm_posterior_sample
+from dynamax.linear_gaussian_ssm.inference import lgssm_joint_sample
 
 from dynamax.linear_gaussian_ssm.info_inference import ParamsLGSSMInfo
 from dynamax.linear_gaussian_ssm.info_inference import PosteriorGSSMInfoFiltered
 from dynamax.linear_gaussian_ssm.info_inference import PosteriorGSSMInfoSmoothed
 from dynamax.linear_gaussian_ssm.info_inference import lgssm_info_filter
 from dynamax.linear_gaussian_ssm.info_inference import lgssm_info_smoother
 
 from dynamax.linear_gaussian_ssm.parallel_inference import lgssm_filter as parallel_lgssm_filter
 from dynamax.linear_gaussian_ssm.parallel_inference import lgssm_smoother as parallel_lgssm_smoother
+from dynamax.linear_gaussian_ssm.parallel_inference import lgssm_posterior_sample as parallel_lgssm_posterior_sample
 
 from dynamax.linear_gaussian_ssm.models import LinearGaussianConjugateSSM, LinearGaussianSSM
```

### Comparing `dynamax-0.1.0/dynamax/linear_gaussian_ssm/inference.py` & `dynamax-0.1.1/dynamax/nonlinear_gaussian_ssm/inference_ekf.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,400 +1,306 @@
 import jax.numpy as jnp
 import jax.random as jr
 from jax import lax
+from jax import jacfwd
 from tensorflow_probability.substrates.jax.distributions import MultivariateNormalFullCovariance as MVN
-from functools import wraps
-import inspect
-
 from jaxtyping import Array, Float
-from typing import NamedTuple, Optional, Union
-
-from dynamax.utils.utils import psd_solve
-from dynamax.parameters import ParameterProperties
-from dynamax.types import PRNGKey, Scalar
-
-class ParamsLGSSMInitial(NamedTuple):
-    r"""Parameters of the initial distribution
-
-    $$p(x_1) = \mathcal{N}(x_1 \mid \mu_1, Q_1)$$
-
-    The tuple doubles as a container for the ParameterProperties.
-
-    :param mean: $\mu_1$
-    :param cov: $Q_1$
-
-    """
-    mean: Union[Float[Array, "state_dim"], ParameterProperties]
-    # unconstrained parameters are stored as a vector.
-    cov: Union[Float[Array, "state_dim state_dim"], Float[Array, "state_dim_triu"], ParameterProperties]
-
-
-class ParamsLGSSMDynamics(NamedTuple):
-    r"""Parameters of the emission distribution
-
-    $$p(x_{t+1} \mid x_t, u_t) = \mathcal{N}(x_{t+1} \mid F x_t + B u_t + b, Q)$$
-
-    The tuple doubles as a container for the ParameterProperties.
-
-    :param weights: dynamics weights $F$
-    :param bias: dynamics bias $b$
-    :param input_weights: dynamics input weights $B$
-    :param cov: dynamics covariance $Q$
-
-    """
-    weights: Union[Float[Array, "state_dim state_dim"], Float[Array, "ntime state_dim state_dim"], ParameterProperties]
-    bias: Union[Float[Array, "state_dim"], Float[Array, "ntime state_dim"], ParameterProperties]
-    input_weights: Union[Float[Array, "state_dim input_dim"], Float[Array, "ntime state_dim input_dim"], ParameterProperties]
-    cov: Union[Float[Array, "state_dim state_dim"], Float[Array, "ntime state_dim state_dim"], Float[Array, "state_dim_triu"], ParameterProperties]
-
-
-class ParamsLGSSMEmissions(NamedTuple):
-    r"""Parameters of the emission distribution
-
-    $$p(y_t \mid x_t, u_t) = \mathcal{N}(y_t \mid H x_t + D u_t + d, R)$$
-
-    The tuple doubles as a container for the ParameterProperties.
-
-    :param weights: emission weights $H$
-    :param bias: emission bias $d$
-    :param input_weights: emission input weights $D$
-    :param cov: emission covariance $R$
-
-    """
-    weights: Union[Float[Array, "emission_dim state_dim"], Float[Array, "ntime emission_dim state_dim"], ParameterProperties]
-    bias: Union[Float[Array, "emission_dim"], Float[Array, "ntime emission_dim"], ParameterProperties]
-    input_weights: Union[Float[Array, "emission_dim input_dim"], Float[Array, "ntime emission_dim input_dim"], ParameterProperties]
-    cov: Union[Float[Array, "emission_dim emission_dim"], Float[Array, "ntime emission_dim emission_dim"], Float[Array, "emission_dim_triu"], ParameterProperties]
-
-
-
-class ParamsLGSSM(NamedTuple):
-    r"""Parameters of a linear Gaussian SSM.
-
-    :param initial: initial distribution parameters
-    :param dynamics: dynamics distribution parameters
-    :param emissions: emission distribution parameters
-
-    """
-    initial: ParamsLGSSMInitial
-    dynamics: ParamsLGSSMDynamics
-    emissions: ParamsLGSSMEmissions
-
-
-class PosteriorGSSMFiltered(NamedTuple):
-    r"""Marginals of the Gaussian filtering posterior.
-
-    :param marginal_loglik: marginal log likelihood, $p(y_{1:T} \mid u_{1:T})$
-    :param filtered_means: array of filtered means $\mathbb{E}[x_t \mid y_{1:t}, u_{1:t}]$
-    :param filtered_covariances: array of filtered covariances $\mathrm{Cov}[x_t \mid y_{1:t}, u_{1:t}]$
-
-    """
-    marginal_loglik: Scalar
-    filtered_means: Float[Array, "ntime state_dim"]
-    filtered_covariances: Float[Array, "ntime state_dim state_dim"]
-
-
-class PosteriorGSSMSmoothed(NamedTuple):
-    r"""Marginals of the Gaussian filtering and smoothing posterior.
-
-    :param marginal_loglik: marginal log likelihood, $p(y_{1:T} \mid u_{1:T})$
-    :param filtered_means: array of filtered means $\mathbb{E}[x_t \mid y_{1:t}, u_{1:t}]$
-    :param filtered_covariances: array of filtered covariances $\mathrm{Cov}[x_t \mid y_{1:t}, u_{1:t}]$
-    :param smoothed_means: array of smoothed means $\mathbb{E}[x_t \mid y_{1:T}, u_{1:T}]$
-    :param smoothed_covariances: array of smoothed marginal covariances, $\mathrm{Cov}[x_t \mid y_{1:T}, u_{1:T}]$
-    :param smoothed_cross_covariances: array of smoothed cross products, $\mathbb{E}[x_t x_{t+1}^T \mid y_{1:T}, u_{1:T}]$
-
-    """
-    marginal_loglik: Scalar
-    filtered_means: Float[Array, "ntime state_dim"]
-    filtered_covariances: Float[Array, "ntime state_dim state_dim"]
-    smoothed_means: Float[Array, "ntime state_dim"]
-    smoothed_covariances: Float[Array, "ntime state_dim state_dim"]
-    smoothed_cross_covariances: Optional[Float[Array, "ntime_minus1 state_dim state_dim"]] = None
+from typing import List, Optional
 
+from dynamax.utils.utils import psd_solve, symmetrize
+from dynamax.nonlinear_gaussian_ssm.models import ParamsNLGSSM
+from dynamax.linear_gaussian_ssm.inference import PosteriorGSSMFiltered, PosteriorGSSMSmoothed
+from dynamax.types import PRNGKey
 
 # Helper functions
 _get_params = lambda x, dim, t: x[t] if x.ndim == dim + 1 else x
-_zeros_if_none = lambda x, shape: x if x is not None else jnp.zeros(shape)
+_process_fn = lambda f, u: (lambda x, y: f(x)) if u is None else f
+_process_input = lambda x, y: jnp.zeros((y,1)) if x is None else x
+
 
-def _predict(m, S, F, B, b, Q, u):
-    r"""Predict next mean and covariance under a linear Gaussian model.
+def _predict(m, P, f, F, Q, u):
+    r"""Predict next mean and covariance using first-order additive EKF
 
-        p(x_{t+1}) = int N(x_t \mid m, S) N(x_{t+1} \mid Fx_t + Bu + b, Q)
-                    = N(x_{t+1} \mid Fm + Bu, F S F^T + Q)
+        p(z_{t+1}) = \int N(z_t | m, S) N(z_{t+1} | f(z_t, u), Q)
+                    = N(z_{t+1} | f(m, u), F(m, u) S F(m, u)^T + Q)
 
     Args:
         m (D_hid,): prior mean.
-        S (D_hid,D_hid): prior covariance.
-        F (D_hid,D_hid): dynamics matrix.
-        B (D_hid,D_in): dynamics input matrix.
-        u (D_in,): inputs.
+        P (D_hid,D_hid): prior covariance.
+        f (Callable): dynamics function.
+        F (Callable): Jacobian of dynamics function.
         Q (D_hid,D_hid): dynamics covariance matrix.
-        b (D_hid,): dynamics bias.
+        u (D_in,): inputs.
 
     Returns:
         mu_pred (D_hid,): predicted mean.
         Sigma_pred (D_hid,D_hid): predicted covariance.
     """
-    mu_pred = F @ m + B @ u + b
-    Sigma_pred = F @ S @ F.T + Q
+    F_x = F(m, u)
+    mu_pred = f(m, u)
+    Sigma_pred = F_x @ P @ F_x.T + Q
     return mu_pred, Sigma_pred
 
 
-def _condition_on(m, P, H, D, d, R, u, y):
-    r"""Condition a Gaussian potential on a new linear Gaussian observation
-       p(x_t \mid y_t, u_t, y_{1:t-1}, u_{1:t-1})
-         propto p(x_t \mid y_{1:t-1}, u_{1:t-1}) p(y_t \mid x_t, u_t)
-         = N(x_t \mid m, P) N(y_t \mid H_t x_t + D_t u_t + d_t, R_t)
-         = N(x_t \mid mm, PP)
+def _condition_on(m, P, h, H, R, u, y, num_iter):
+    r"""Condition a Gaussian potential on a new observation.
+
+       p(z_t | y_t, u_t, y_{1:t-1}, u_{1:t-1})
+         propto p(z_t | y_{1:t-1}, u_{1:t-1}) p(y_t | z_t, u_t)
+         = N(z_t | m, S) N(y_t | h_t(z_t, u_t), R_t)
+         = N(z_t | mm, SS)
      where
          mm = m + K*(y - yhat) = mu_cond
-         yhat = H*m + D*u + d
-         S = (R + H * P * H')
-         K = P * H' * S^{-1}
-         PP = P - K S K' = Sigma_cond
+         yhat = h(m, u)
+         S = R + H(m,u) * P * H(m,u)'
+         K = P * H(m, u)' * S^{-1}
+         SS = P - K * S * K' = Sigma_cond
      **Note! This can be done more efficiently when R is diagonal.**
 
     Args:
          m (D_hid,): prior mean.
          P (D_hid,D_hid): prior covariance.
-         H (D_obs,D_hid): emission matrix.
-         D (D_obs,D_in): emission input weights.
-         u (D_in,): inputs.
-         d (D_obs,): emission bias.
+         h (Callable): emission function.
+         H (Callable): Jacobian of emission function.
          R (D_obs,D_obs): emission covariance matrix.
+         u (D_in,): inputs.
          y (D_obs,): observation.
+         num_iter (int): number of re-linearizations around posterior for update step.
 
      Returns:
-         mu_pred (D_hid,): predicted mean.
-         Sigma_pred (D_hid,D_hid): predicted covariance.
+         mu_cond (D_hid,): filtered mean.
+         Sigma_cond (D_hid,D_hid): filtered covariance.
     """
-    # Compute the Kalman gain
-    S = R + H @ P @ H.T
-    K = psd_solve(S, H @ P).T
-    Sigma_cond = P - K @ S @ K.T
-    mu_cond = m + K @ (y - D @ u - d - H @ m)
-    return mu_cond, Sigma_cond
-
-
-def preprocess_args(f):
-    """Preprocess the parameters and inputs in case some are set to None."""
-    sig = inspect.signature(f)
-
-    @wraps(f)
-    def wrapper(*args, **kwargs):
-        # Extract the arguments by name
-        bound_args = sig.bind(*args, **kwargs)
-        bound_args.apply_defaults()
-        params = bound_args.arguments['params']
-        emissions = bound_args.arguments['emissions']
-        inputs = bound_args.arguments['inputs']
-
-        # Make sure all the required parameters are there
-        assert params.initial.mean is not None
-        assert params.initial.cov is not None
-        assert params.dynamics.weights is not None
-        assert params.dynamics.cov is not None
-        assert params.emissions.weights is not None
-        assert params.emissions.cov is not None
-
-        # Get shapes
-        emission_dim, state_dim = params.emissions.weights.shape[-2:]
-        num_timesteps = len(emissions)
-
-        # Default the inputs to zero
-        inputs = _zeros_if_none(inputs, (num_timesteps, 0))
-        input_dim = inputs.shape[-1]
-
-        # Default other parameters to zero
-        dynamics_input_weights = _zeros_if_none(params.dynamics.input_weights, (state_dim, input_dim))
-        dynamics_bias = _zeros_if_none(params.dynamics.bias, (state_dim,))
-        emissions_input_weights = _zeros_if_none(params.emissions.input_weights, (emission_dim, input_dim))
-        emissions_bias = _zeros_if_none(params.emissions.bias, (emission_dim,))
-
-        full_params = ParamsLGSSM(
-            initial=ParamsLGSSMInitial(
-                mean=params.initial.mean,
-                cov=params.initial.cov),
-            dynamics=ParamsLGSSMDynamics(
-                weights=params.dynamics.weights,
-                bias=dynamics_bias,
-                input_weights=dynamics_input_weights,
-                cov=params.dynamics.cov),
-            emissions=ParamsLGSSMEmissions(
-                weights=params.emissions.weights,
-                bias=emissions_bias,
-                input_weights=emissions_input_weights,
-                cov=params.emissions.cov)
-            )
-        return f(full_params, emissions, inputs=inputs)
-    return wrapper
-
-
-@preprocess_args
-def lgssm_filter(
-    params: ParamsLGSSM,
-    emissions:  Float[Array, "ntime emission_dim"],
-    inputs: Optional[Float[Array, "ntime input_dim"]]=None
+    def _step(carry, _):
+        prior_mean, prior_cov = carry
+        H_x = H(prior_mean, u)
+        S = R + H_x @ prior_cov @ H_x.T
+        K = psd_solve(S, H_x @ prior_cov).T
+        posterior_cov = prior_cov - K @ S @ K.T
+        posterior_mean = prior_mean + K @ (y - h(prior_mean, u))
+        return (posterior_mean, posterior_cov), None
+
+    # Iterate re-linearization over posterior mean and covariance
+    carry = (m, P)
+    (mu_cond, Sigma_cond), _ = lax.scan(_step, carry, jnp.arange(num_iter))
+    return mu_cond, symmetrize(Sigma_cond)
+
+
+def extended_kalman_filter(
+    params: ParamsNLGSSM,
+    emissions: Float[Array, "ntime emission_dim"],
+    num_iter: int = 1,
+    inputs: Optional[Float[Array, "ntime input_dim"]] = None,
+    output_fields: Optional[List[str]]=["filtered_means", "filtered_covariances", "predicted_means", "predicted_covariances"],
 ) -> PosteriorGSSMFiltered:
-    r"""Run a Kalman filter to produce the marginal likelihood and filtered state estimates.
+    r"""Run an (iterated) extended Kalman filter to produce the
+    marginal likelihood and filtered state estimates.
 
     Args:
-        params: model parameters
-        emissions: array of observations.
+        params: model parameters.
+        emissions: observation sequence.
+        num_iter: number of linearizations around posterior for update step (default 1).
         inputs: optional array of inputs.
+        output_fields: list of fields to return in posterior object.
+            These can take the values "filtered_means", "filtered_covariances",
+            "predicted_means", "predicted_covariances", and "marginal_loglik".
 
     Returns:
-        PosteriorGSSMFiltered: filtered posterior object
+        post: posterior object.
 
     """
     num_timesteps = len(emissions)
-    inputs = jnp.zeros((num_timesteps, 0)) if inputs is None else inputs
+
+    # Dynamics and emission functions and their Jacobians
+    f, h = params.dynamics_function, params.emission_function
+    F, H = jacfwd(f), jacfwd(h)
+    f, h, F, H = (_process_fn(fn, inputs) for fn in (f, h, F, H))
+    inputs = _process_input(inputs, num_timesteps)
 
     def _step(carry, t):
         ll, pred_mean, pred_cov = carry
 
-        # Shorthand: get parameters and inputs for time index t
-        F = _get_params(params.dynamics.weights, 2, t)
-        B = _get_params(params.dynamics.input_weights, 2, t)
-        b = _get_params(params.dynamics.bias, 1, t)
-        Q = _get_params(params.dynamics.cov, 2, t)
-        H = _get_params(params.emissions.weights, 2, t)
-        D = _get_params(params.emissions.input_weights, 2, t)
-        d = _get_params(params.emissions.bias, 1, t)
-        R = _get_params(params.emissions.cov, 2, t)
+        # Get parameters and inputs for time index t
+        Q = _get_params(params.dynamics_covariance, 2, t)
+        R = _get_params(params.emission_covariance, 2, t)
         u = inputs[t]
         y = emissions[t]
 
         # Update the log likelihood
-        ll += MVN(H @ pred_mean + D @ u + d, H @ pred_cov @ H.T + R).log_prob(y)
+        H_x = H(pred_mean, u)
+        ll += MVN(h(pred_mean, u), H_x @ pred_cov @ H_x.T + R).log_prob(jnp.atleast_1d(y))
 
         # Condition on this emission
-        filtered_mean, filtered_cov = _condition_on(pred_mean, pred_cov, H, D, d, R, u, y)
+        filtered_mean, filtered_cov = _condition_on(pred_mean, pred_cov, h, H, R, u, y, num_iter)
 
         # Predict the next state
-        pred_mean, pred_cov = _predict(filtered_mean, filtered_cov, F, B, b, Q, u)
+        pred_mean, pred_cov = _predict(filtered_mean, filtered_cov, f, F, Q, u)
+
+        # Build carry and output states
+        carry = (ll, pred_mean, pred_cov)
+        outputs = {
+            "filtered_means": filtered_mean,
+            "filtered_covariances": filtered_cov,
+            "predicted_means": pred_mean,
+            "predicted_covariances": pred_cov,
+            "marginal_loglik": ll,
+        }
+        outputs = {key: val for key, val in outputs.items() if key in output_fields}
+
+        return carry, outputs
+
+    # Run the extended Kalman filter
+    carry = (0.0, params.initial_mean, params.initial_covariance)
+    (ll, *_), outputs = lax.scan(_step, carry, jnp.arange(num_timesteps))
+    outputs = {"marginal_loglik": ll, **outputs}
+    posterior_filtered = PosteriorGSSMFiltered(
+        **outputs,
+    )
+    return posterior_filtered
+
 
-        return (ll, pred_mean, pred_cov), (filtered_mean, filtered_cov)
+def iterated_extended_kalman_filter(
+    params: ParamsNLGSSM,
+    emissions:  Float[Array, "ntime emission_dim"],
+    num_iter: int = 2,
+    inputs: Optional[Float[Array, "ntime input_dim"]] = None
+) -> PosteriorGSSMFiltered:
+    r"""Run an iterated extended Kalman filter to produce the
+    marginal likelihood and filtered state estimates.
+
+    Args:
+        params: model parameters.
+        emissions: observation sequence.
+        num_iter: number of linearizations around posterior for update step (default 2).
+        inputs: optional array of inputs.
 
-    # Run the Kalman filter
-    carry = (0.0, params.initial.mean, params.initial.cov)
-    (ll, _, _), (filtered_means, filtered_covs) = lax.scan(_step, carry, jnp.arange(num_timesteps))
-    return PosteriorGSSMFiltered(marginal_loglik=ll, filtered_means=filtered_means, filtered_covariances=filtered_covs)
+    Returns:
+        post: posterior object.
 
+    """
+    filtered_posterior = extended_kalman_filter(params, emissions, num_iter, inputs)
+    return filtered_posterior
 
-@preprocess_args
-def lgssm_smoother(
-    params: ParamsLGSSM,
-    emissions: Float[Array, "ntime emission_dim"],
-    inputs: Optional[Float[Array, "ntime input_dim"]]=None
+
+def extended_kalman_smoother(
+    params: ParamsNLGSSM,
+    emissions:  Float[Array, "ntime emission_dim"],
+    filtered_posterior: Optional[PosteriorGSSMFiltered] = None,
+    inputs: Optional[Float[Array, "ntime input_dim"]] = None
 ) -> PosteriorGSSMSmoothed:
-    r"""Run forward-filtering, backward-smoother to compute expectations
-    under the posterior distribution on latent states. Technically, this
-    implements the Rauch-Tung-Striebel (RTS) smoother.
+    r"""Run an extended Kalman (RTS) smoother.
 
     Args:
-        params: an LGSSMParams instance (or object with the same fields)
-        emissions: array of observations.
-        inputs: array of inputs.
+        params: model parameters.
+        emissions: observation sequence.
+        filtered_posterior: optional output from filtering step.
+        inputs: optional array of inputs.
 
     Returns:
-        PosteriorGSSMSmoothed: smoothed posterior object.
+        post: posterior object.
 
     """
     num_timesteps = len(emissions)
-    inputs = jnp.zeros((num_timesteps, 0)) if inputs is None else inputs
 
-    # Run the Kalman filter
-    filtered_posterior = lgssm_filter(params, emissions, inputs)
-    ll, filtered_means, filtered_covs, *_ = filtered_posterior
+    # Get filtered posterior
+    if filtered_posterior is None:
+        filtered_posterior = extended_kalman_filter(params, emissions, inputs=inputs)
+    ll = filtered_posterior.marginal_loglik
+    filtered_means = filtered_posterior.filtered_means
+    filtered_covs = filtered_posterior.filtered_covariances
+
+    # Dynamics and emission functions and their Jacobians
+    f = params.dynamics_function
+    F = jacfwd(f)
+    f, F = (_process_fn(fn, inputs) for fn in (f, F))
+    inputs = _process_input(inputs, num_timesteps)
 
-    # Run the smoother backward in time
     def _step(carry, args):
         # Unpack the inputs
         smoothed_mean_next, smoothed_cov_next = carry
         t, filtered_mean, filtered_cov = args
 
-        # Shorthand: get parameters and inputs for time index t
-        F = _get_params(params.dynamics.weights, 2, t)
-        B = _get_params(params.dynamics.input_weights, 2, t)
-        b = _get_params(params.dynamics.bias, 1, t)
-        Q = _get_params(params.dynamics.cov, 2, t)
+        # Get parameters and inputs for time index t
+        Q = _get_params(params.dynamics_covariance, 2, t)
+        R = _get_params(params.emission_covariance, 2, t)
         u = inputs[t]
+        F_x = F(filtered_mean, u)
 
-        # This is like the Kalman gain but in reverse
-        # See Eq 8.11 of Saarka's "Bayesian Filtering and Smoothing"
-        G = psd_solve(Q + F @ filtered_cov @ F.T, F @ filtered_cov).T
-
-        # Compute the smoothed mean and covariance
-        smoothed_mean = filtered_mean + G @ (smoothed_mean_next - F @ filtered_mean - B @ u - b)
-        smoothed_cov = filtered_cov + G @ (smoothed_cov_next - F @ filtered_cov @ F.T - Q) @ G.T
+        # Prediction step
+        m_pred = f(filtered_mean, u)
+        S_pred = Q + F_x @ filtered_cov @ F_x.T
+        G = psd_solve(S_pred, F_x @ filtered_cov).T
 
-        # Compute the smoothed expectation of x_t x_{t+1}^T
-        smoothed_cross = G @ smoothed_cov_next + jnp.outer(smoothed_mean, smoothed_mean_next)
+        # Compute smoothed mean and covariance
+        smoothed_mean = filtered_mean + G @ (smoothed_mean_next - m_pred)
+        smoothed_cov = filtered_cov + G @ (smoothed_cov_next - S_pred) @ G.T
 
-        return (smoothed_mean, smoothed_cov), (smoothed_mean, smoothed_cov, smoothed_cross)
+        return (smoothed_mean, smoothed_cov), (smoothed_mean, smoothed_cov)
 
-    # Run the Kalman smoother
+    # Run the extended Kalman smoother
     init_carry = (filtered_means[-1], filtered_covs[-1])
     args = (jnp.arange(num_timesteps - 2, -1, -1), filtered_means[:-1][::-1], filtered_covs[:-1][::-1])
-    _, (smoothed_means, smoothed_covs, smoothed_cross) = lax.scan(_step, init_carry, args)
+    _, (smoothed_means, smoothed_covs) = lax.scan(_step, init_carry, args)
 
     # Reverse the arrays and return
     smoothed_means = jnp.row_stack((smoothed_means[::-1], filtered_means[-1][None, ...]))
     smoothed_covs = jnp.row_stack((smoothed_covs[::-1], filtered_covs[-1][None, ...]))
-    smoothed_cross = smoothed_cross[::-1]
     return PosteriorGSSMSmoothed(
         marginal_loglik=ll,
         filtered_means=filtered_means,
         filtered_covariances=filtered_covs,
         smoothed_means=smoothed_means,
         smoothed_covariances=smoothed_covs,
-        smoothed_cross_covariances=smoothed_cross,
     )
 
 
-def lgssm_posterior_sample(
+
+
+def extended_kalman_posterior_sample(
     key: PRNGKey,
-    params: ParamsLGSSM,
+    params: ParamsNLGSSM,
     emissions:  Float[Array, "ntime emission_dim"],
-    inputs: Optional[Float[Array, "ntime input_dim"]]=None
+    inputs: Optional[Float[Array, "ntime input_dim"]] = None
 ) -> Float[Array, "ntime state_dim"]:
-    r"""Run forward-filtering, backward-sampling to draw samples from $p(x_{1:T} \mid y_{1:T}, u_{1:T})$.
+    r"""Run forward-filtering, backward-sampling to draw samples.
 
     Args:
         key: random number key.
-        params: parameters.
-        emissions: sequence of observations.
-        inputs: optional sequence of inptus.
+        params: model parameters.
+        emissions: observation sequence.
+        inputs: optional array of inputs.
 
     Returns:
-        Float[Array, "ntime state_dim"]: one sample of $x_{1:T}$ from the posterior distribution on latent states.
+        Float[Array, "ntime state_dim"]: one sample of $z_{1:T}$ from the posterior distribution on latent states.
     """
     num_timesteps = len(emissions)
-    inputs = jnp.zeros((num_timesteps, 0)) if inputs is None else inputs
 
-    # Run the Kalman filter
-    filtered_posterior = lgssm_filter(params, emissions, inputs)
-    ll, filtered_means, filtered_covs, *_ = filtered_posterior
+    # Get filtered posterior
+    filtered_posterior = extended_kalman_filter(params, emissions, inputs=inputs)
+    ll = filtered_posterior.marginal_loglik
+    filtered_means = filtered_posterior.filtered_means
+    filtered_covs = filtered_posterior.filtered_covariances
+
+    # Dynamics and emission functions and their Jacobians
+    f = params.dynamics_function
+    F = jacfwd(f)
+    f, F = (_process_fn(fn, inputs) for fn in (f, F))
+    inputs = _process_input(inputs, num_timesteps)
 
-    # Sample backward in time
     def _step(carry, args):
+        # Unpack the inputs
         next_state = carry
         key, filtered_mean, filtered_cov, t = args
 
-        # Shorthand: get parameters and inputs for time index t
-        F = _get_params(params.dynamics.weights, 2, t)
-        B = _get_params(params.dynamics.input_weights, 2, t)
-        b = _get_params(params.dynamics.bias, 1, t)
-        Q = _get_params(params.dynamics.cov, 2, t)
+        # Get parameters and inputs for time index t
+        Q = _get_params(params.dynamics_covariance, 2, t)
         u = inputs[t]
 
         # Condition on next state
-        smoothed_mean, smoothed_cov = _condition_on(filtered_mean, filtered_cov, F, B, b, Q, u, next_state)
+        smoothed_mean, smoothed_cov = _condition_on(filtered_mean, filtered_cov, f, F, Q, u, next_state, 1)
         state = MVN(smoothed_mean, smoothed_cov).sample(seed=key)
         return state, state
 
     # Initialize the last state
     key, this_key = jr.split(key, 2)
     last_state = MVN(filtered_means[-1], filtered_covs[-1]).sample(seed=this_key)
 
@@ -403,7 +309,37 @@
         filtered_means[:-1][::-1],
         filtered_covs[:-1][::-1],
         jnp.arange(num_timesteps - 2, -1, -1),
     )
     _, reversed_states = lax.scan(_step, last_state, args)
     states = jnp.row_stack([reversed_states[::-1], last_state])
     return states
+
+
+
+def iterated_extended_kalman_smoother(
+    params: ParamsNLGSSM,
+    emissions:  Float[Array, "ntime emission_dim"],
+    num_iter: int = 2,
+    inputs: Optional[Float[Array, "ntime input_dim"]] = None
+) -> PosteriorGSSMSmoothed:
+    r"""Run an iterated extended Kalman smoother (IEKS).
+
+    Args:
+        params: model parameters.
+        emissions: observation sequence.
+        num_iter: number of linearizations around posterior for update step (default 2).
+        inputs: optional array of inputs.
+
+    Returns:
+        post: posterior object.
+
+    """
+
+    def _step(carry, _):
+        # Relinearize around smoothed posterior from previous iteration
+        smoothed_prior = carry
+        smoothed_posterior = extended_kalman_smoother(params, emissions, smoothed_prior, inputs)
+        return smoothed_posterior, None
+
+    smoothed_posterior, _ = lax.scan(_step, None, jnp.arange(num_iter))
+    return smoothed_posterior
```

### Comparing `dynamax-0.1.0/dynamax/linear_gaussian_ssm/info_inference.py` & `dynamax-0.1.1/dynamax/linear_gaussian_ssm/info_inference.py`

 * *Files identical despite different names*

### Comparing `dynamax-0.1.0/dynamax/linear_gaussian_ssm/info_inference_test.py` & `dynamax-0.1.1/dynamax/linear_gaussian_ssm/info_inference_test.py`

 * *Files identical despite different names*

### Comparing `dynamax-0.1.0/dynamax/linear_gaussian_ssm/models.py` & `dynamax-0.1.1/dynamax/linear_gaussian_ssm/models.py`

 * *Files identical despite different names*

### Comparing `dynamax-0.1.0/dynamax/linear_gaussian_ssm/models_test.py` & `dynamax-0.1.1/dynamax/linear_gaussian_ssm/models_test.py`

 * *Files identical despite different names*

### Comparing `dynamax-0.1.0/dynamax/nonlinear_gaussian_ssm/__init__.py` & `dynamax-0.1.1/dynamax/nonlinear_gaussian_ssm/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from dynamax.nonlinear_gaussian_ssm.models import ParamsNLGSSM, NonlinearGaussianSSM
 from dynamax.nonlinear_gaussian_ssm.inference_ekf import extended_kalman_filter
 from dynamax.nonlinear_gaussian_ssm.inference_ekf import iterated_extended_kalman_filter
 from dynamax.nonlinear_gaussian_ssm.inference_ekf import extended_kalman_smoother
 from dynamax.nonlinear_gaussian_ssm.inference_ekf import iterated_extended_kalman_smoother
+from dynamax.nonlinear_gaussian_ssm.inference_ekf import extended_kalman_posterior_sample
 from dynamax.nonlinear_gaussian_ssm.inference_ukf import unscented_kalman_filter
 from dynamax.nonlinear_gaussian_ssm.inference_ukf import unscented_kalman_smoother
 from dynamax.nonlinear_gaussian_ssm.inference_ukf import UKFHyperParams
```

### Comparing `dynamax-0.1.0/dynamax/nonlinear_gaussian_ssm/inference_test_utils.py` & `dynamax-0.1.1/dynamax/nonlinear_gaussian_ssm/inference_test_utils.py`

 * *Files identical despite different names*

### Comparing `dynamax-0.1.0/dynamax/nonlinear_gaussian_ssm/inference_ukf.py` & `dynamax-0.1.1/dynamax/nonlinear_gaussian_ssm/inference_ukf.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import jax.numpy as jnp
 from jax import lax
 from jax import vmap
 from tensorflow_probability.substrates.jax.distributions import MultivariateNormalFullCovariance as MVN
 from jaxtyping import Array, Float
-from typing import NamedTuple, Optional
+from typing import NamedTuple, Optional, List
 
 from dynamax.utils.utils import psd_solve
 from dynamax.nonlinear_gaussian_ssm.models import  ParamsNLGSSM
 from dynamax.linear_gaussian_ssm.models import PosteriorGSSMFiltered, PosteriorGSSMSmoothed
 
 class UKFHyperParams(NamedTuple):
     """Lightweight container for UKF hyperparameters.
@@ -136,15 +136,16 @@
     return ll, m_cond, P_cond
 
 
 def unscented_kalman_filter(
     params: ParamsNLGSSM,
     emissions: Float[Array, "ntime emission_dim"],
     hyperparams: UKFHyperParams,
-    inputs: Optional[Float[Array, "ntime input_dim"]]=None
+    inputs: Optional[Float[Array, "ntime input_dim"]]=None,
+    output_fields: Optional[List[str]]=["filtered_means", "filtered_covariances", "predicted_means", "predicted_covariances"],
 ) -> PosteriorGSSMFiltered:
     """Run a unscented Kalman filter to produce the marginal likelihood and
     filtered state estimates.
 
     Args:
         params: model parameters.
         emissions: array of observations.
@@ -184,20 +185,35 @@
 
         # Update the log likelihood
         ll += log_likelihood
 
         # Predict the next state
         pred_mean, pred_cov, _ = _predict(filtered_mean, filtered_cov, f, Q, lamb, w_mean, w_cov, u)
 
-        return (ll, pred_mean, pred_cov), (filtered_mean, filtered_cov)
+        # Build carry and output states
+        carry = (ll, pred_mean, pred_cov)
+        outputs = {
+            "filtered_means": filtered_mean,
+            "filtered_covariances": filtered_cov,
+            "predicted_means": pred_mean,
+            "predicted_covariances": pred_cov,
+            "marginal_loglik": ll,
+        }
+        outputs = {key: val for key, val in outputs.items() if key in output_fields}
+        return carry, outputs
+
 
-    # Run the UKF
+    # Run the Unscented Kalman Filter
     carry = (0.0, params.initial_mean, params.initial_covariance)
-    (ll, _, _), (filtered_means, filtered_covs) = lax.scan(_step, carry, jnp.arange(num_timesteps))
-    return PosteriorGSSMFiltered(marginal_loglik=ll, filtered_means=filtered_means, filtered_covariances=filtered_covs)
+    (ll, *_), outputs = lax.scan(_step, carry, jnp.arange(num_timesteps))
+    outputs = {"marginal_loglik": ll, **outputs}
+    posterior_filtered = PosteriorGSSMFiltered(
+        **outputs,
+    )
+    return posterior_filtered
 
 
 def unscented_kalman_smoother(
     params: ParamsNLGSSM,
     emissions: Float[Array, "ntime emission_dim"],
     hyperparams: UKFHyperParams,
     inputs: Optional[Float[Array, "ntime input_dim"]]=None
@@ -215,15 +231,17 @@
 
     """
     num_timesteps = len(emissions)
     state_dim = params.dynamics_covariance.shape[0]
 
     # Run the unscented Kalman filter
     ukf_posterior = unscented_kalman_filter(params, emissions, hyperparams, inputs)
-    ll, filtered_means, filtered_covs, *_ = ukf_posterior
+    ll = ukf_posterior.marginal_loglik
+    filtered_means = ukf_posterior.filtered_means
+    filtered_covs = ukf_posterior.filtered_covariances
 
     # Compute lambda and weights from from hyperparameters
     alpha, beta, kappa = hyperparams.alpha, hyperparams.beta, hyperparams.kappa
     lamb = _compute_lambda(alpha, kappa, state_dim)
     w_mean, w_cov = _compute_weights(state_dim, alpha, beta, lamb)
 
     # Dynamics and emission functions
```

### Comparing `dynamax-0.1.0/dynamax/nonlinear_gaussian_ssm/inference_ukf_test.py` & `dynamax-0.1.1/dynamax/nonlinear_gaussian_ssm/inference_ukf_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import jax.numpy as jnp
+import jax.random as jr
 
 from dynamax.nonlinear_gaussian_ssm.inference_ukf import unscented_kalman_smoother, UKFHyperParams
 from dynamax.nonlinear_gaussian_ssm.sarkka_lib import ukf, uks
 from dynamax.nonlinear_gaussian_ssm.inference_test_utils import random_nlgssm_args
 from dynamax.utils.utils import has_tpu
 
 if has_tpu():
     def allclose(x, y):
         print(jnp.max(x-y))
         return jnp.allclose(x, y, atol=1e-1)
 else:
     def allclose(x,y):
+        print(jnp.max(x-y))
         return jnp.allclose(x, y, atol=1e-1)
 
 def test_ukf_nonlinear(key=0, num_timesteps=15):
     nlgssm_args, _, emissions = random_nlgssm_args(key=key, num_timesteps=num_timesteps)
     hyperparams = UKFHyperParams()
 
     # Run UKF from sarkka-jax library
```

### Comparing `dynamax-0.1.0/dynamax/nonlinear_gaussian_ssm/models.py` & `dynamax-0.1.1/dynamax/nonlinear_gaussian_ssm/models.py`

 * *Files identical despite different names*

### Comparing `dynamax-0.1.0/dynamax/nonlinear_gaussian_ssm/sarkka_lib.py` & `dynamax-0.1.1/dynamax/nonlinear_gaussian_ssm/sarkka_lib.py`

 * *Files identical despite different names*

### Comparing `dynamax-0.1.0/dynamax/parameters.py` & `dynamax-0.1.1/dynamax/parameters.py`

 * *Files identical despite different names*

### Comparing `dynamax-0.1.0/dynamax/parameters_test.py` & `dynamax-0.1.1/dynamax/parameters_test.py`

 * *Files identical despite different names*

### Comparing `dynamax-0.1.0/dynamax/ssm.py` & `dynamax-0.1.1/dynamax/ssm.py`

 * *Files identical despite different names*

### Comparing `dynamax-0.1.0/dynamax/utils/bijectors.py` & `dynamax-0.1.1/dynamax/utils/bijectors.py`

 * *Files identical despite different names*

### Comparing `dynamax-0.1.0/dynamax/utils/distributions.py` & `dynamax-0.1.1/dynamax/utils/distributions.py`

 * *Files identical despite different names*

### Comparing `dynamax-0.1.0/dynamax/utils/distributions_test.py` & `dynamax-0.1.1/dynamax/utils/distributions_test.py`

 * *Files identical despite different names*

### Comparing `dynamax-0.1.0/dynamax/utils/optimize.py` & `dynamax-0.1.1/dynamax/utils/optimize.py`

 * *Files identical despite different names*

### Comparing `dynamax-0.1.0/dynamax/utils/utils.py` & `dynamax-0.1.1/dynamax/utils/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -196,8 +196,13 @@
     overlap = compute_state_overlap(z1, z2)
     _, perm = linear_sum_assignment(-overlap)
     return perm
 
 
 def psd_solve(A,b):
     """A wrapper for coordinating the linalg solvers used in the library for psd matrices."""
-    return jnp.linalg.solve(A,b)
+    A = A + 1e-6
+    return jnp.linalg.solve(A,b)
+
+def symmetrize(A):
+    """Symmetrize one or more matrices."""
+    return 0.5 * (A + jnp.swapaxes(A, -1, -2))
```

### Comparing `dynamax-0.1.0/dynamax/utils/utils_test.py` & `dynamax-0.1.1/dynamax/utils/utils_test.py`

 * *Files identical despite different names*

### Comparing `dynamax-0.1.0/dynamax/warnings.py` & `dynamax-0.1.1/dynamax/warnings.py`

 * *Files identical despite different names*

### Comparing `dynamax-0.1.0/dynamax.egg-info/PKG-INFO` & `dynamax-0.1.1/dynamax.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamax
-Version: 0.1.0
+Version: 0.1.1
 Summary: Dynamic State Space Models in JAX.
 Home-page: https://github.com/probml/dynamax
 Author: Peter Chang, Giles Harper-Donnelly, Aleyna Kara, Xinglong Li, Scott Linderman, Kevin Murphy
 License: MIT
 Description: # Welcome to DYNAMAX!
         
         ![Logo](https://raw.githubusercontent.com/probml/dynamax/main/logo/logo.gif)
```

### Comparing `dynamax-0.1.0/dynamax.egg-info/SOURCES.txt` & `dynamax-0.1.1/dynamax.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -17,24 +17,27 @@
 dynamax.egg-info/requires.txt
 dynamax.egg-info/top_level.txt
 dynamax/generalized_gaussian_ssm/__init__.py
 dynamax/generalized_gaussian_ssm/inference.py
 dynamax/generalized_gaussian_ssm/inference_test.py
 dynamax/generalized_gaussian_ssm/models.py
 dynamax/generalized_gaussian_ssm/models_test.py
+dynamax/generalized_gaussian_ssm/demos/__init__.py
+dynamax/generalized_gaussian_ssm/demos/cmgf_logreg_estimator.py
 dynamax/hidden_markov_model/__init__.py
 dynamax/hidden_markov_model/inference.py
 dynamax/hidden_markov_model/inference_test.py
 dynamax/hidden_markov_model/parallel_inference.py
 dynamax/hidden_markov_model/models/__init__.py
 dynamax/hidden_markov_model/models/abstractions.py
 dynamax/hidden_markov_model/models/arhmm.py
 dynamax/hidden_markov_model/models/bernoulli_hmm.py
 dynamax/hidden_markov_model/models/categorical_glm_hmm.py
 dynamax/hidden_markov_model/models/categorical_hmm.py
+dynamax/hidden_markov_model/models/gamma_hmm.py
 dynamax/hidden_markov_model/models/gaussian_hmm.py
 dynamax/hidden_markov_model/models/gmm_hmm.py
 dynamax/hidden_markov_model/models/initial.py
 dynamax/hidden_markov_model/models/linreg_hmm.py
 dynamax/hidden_markov_model/models/logreg_hmm.py
 dynamax/hidden_markov_model/models/multinomial_hmm.py
 dynamax/hidden_markov_model/models/poisson_hmm.py
@@ -46,14 +49,15 @@
 dynamax/linear_gaussian_ssm/info_inference.py
 dynamax/linear_gaussian_ssm/info_inference_test.py
 dynamax/linear_gaussian_ssm/models.py
 dynamax/linear_gaussian_ssm/models_test.py
 dynamax/linear_gaussian_ssm/parallel_inference.py
 dynamax/linear_gaussian_ssm/parallel_inference_test.py
 dynamax/linear_gaussian_ssm/demos/__init__.py
+dynamax/linear_gaussian_ssm/demos/kf_linreg_jax_vs_pt.py
 dynamax/nonlinear_gaussian_ssm/__init__.py
 dynamax/nonlinear_gaussian_ssm/inference_ekf.py
 dynamax/nonlinear_gaussian_ssm/inference_ekf_test.py
 dynamax/nonlinear_gaussian_ssm/inference_test_utils.py
 dynamax/nonlinear_gaussian_ssm/inference_ukf.py
 dynamax/nonlinear_gaussian_ssm/inference_ukf_test.py
 dynamax/nonlinear_gaussian_ssm/models.py
```

### Comparing `dynamax-0.1.0/dynamax.egg-info/requires.txt` & `dynamax-0.1.1/dynamax.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dynamax-0.1.0/setup.cfg` & `dynamax-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `dynamax-0.1.0/setup.py` & `dynamax-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `dynamax-0.1.0/versioneer.py` & `dynamax-0.1.1/versioneer.py`

 * *Files identical despite different names*

