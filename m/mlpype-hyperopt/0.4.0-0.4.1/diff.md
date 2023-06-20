# Comparing `tmp/mlpype-hyperopt-0.4.0.tar.gz` & `tmp/mlpype-hyperopt-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpype-hyperopt-0.4.0.tar", last modified: Fri May  5 10:37:07 2023, max compression
+gzip compressed data, was "mlpype-hyperopt-0.4.1.tar", last modified: Tue Jun 20 16:47:07 2023, max compression
```

## Comparing `mlpype-hyperopt-0.4.0.tar` & `mlpype-hyperopt-0.4.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 vandejer (1865779777) 296108113        0 2023-05-05 10:37:07.960541 mlpype-hyperopt-0.4.0/
--rw-r--r--   0 vandejer (1865779777) 296108113      102 2023-05-05 10:37:07.957200 mlpype-hyperopt-0.4.0/PKG-INFO
-drwxr-xr-x   0 vandejer (1865779777) 296108113        0 2023-05-05 10:37:07.954461 mlpype-hyperopt-0.4.0/mlpype_hyperopt.egg-info/
--rw-r--r--   0 vandejer (1865779777) 296108113      102 2023-05-05 10:37:07.000000 mlpype-hyperopt-0.4.0/mlpype_hyperopt.egg-info/PKG-INFO
--rw-r--r--   0 vandejer (1865779777) 296108113      202 2023-05-05 10:37:07.000000 mlpype-hyperopt-0.4.0/mlpype_hyperopt.egg-info/SOURCES.txt
--rw-r--r--   0 vandejer (1865779777) 296108113        1 2023-05-05 10:37:07.000000 mlpype-hyperopt-0.4.0/mlpype_hyperopt.egg-info/dependency_links.txt
--rw-r--r--   0 vandejer (1865779777) 296108113      122 2023-05-05 10:37:07.000000 mlpype-hyperopt-0.4.0/mlpype_hyperopt.egg-info/requires.txt
--rw-r--r--   0 vandejer (1865779777) 296108113        1 2023-05-05 10:37:07.000000 mlpype-hyperopt-0.4.0/mlpype_hyperopt.egg-info/top_level.txt
--rw-r--r--   0 vandejer (1865779777) 296108113       38 2023-05-05 10:37:07.960690 mlpype-hyperopt-0.4.0/setup.cfg
--rw-r--r--   0 vandejer (1865779777) 296108113      492 2023-05-05 10:18:55.000000 mlpype-hyperopt-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:47:07.914186 mlpype-hyperopt-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-20 16:47:07.914186 mlpype-hyperopt-0.4.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:47:07.914186 mlpype-hyperopt-0.4.1/mlpype_hyperopt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-20 16:47:07.000000 mlpype-hyperopt-0.4.1/mlpype_hyperopt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-20 16:47:07.000000 mlpype-hyperopt-0.4.1/mlpype_hyperopt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:47:07.000000 mlpype-hyperopt-0.4.1/mlpype_hyperopt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-20 16:47:07.000000 mlpype-hyperopt-0.4.1/mlpype_hyperopt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:47:07.000000 mlpype-hyperopt-0.4.1/mlpype_hyperopt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 16:47:07.914186 mlpype-hyperopt-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-20 16:43:35.000000 mlpype-hyperopt-0.4.1/setup.py
```

