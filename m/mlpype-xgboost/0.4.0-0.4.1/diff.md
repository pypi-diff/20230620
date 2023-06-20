# Comparing `tmp/mlpype-xgboost-0.4.0.tar.gz` & `tmp/mlpype-xgboost-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpype-xgboost-0.4.0.tar", last modified: Fri May  5 10:38:15 2023, max compression
+gzip compressed data, was "mlpype-xgboost-0.4.1.tar", last modified: Tue Jun 20 16:47:49 2023, max compression
```

## Comparing `mlpype-xgboost-0.4.0.tar` & `mlpype-xgboost-0.4.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 vandejer (1865779777) 296108113        0 2023-05-05 10:38:15.859125 mlpype-xgboost-0.4.0/
--rw-r--r--   0 vandejer (1865779777) 296108113      101 2023-05-05 10:38:15.858856 mlpype-xgboost-0.4.0/PKG-INFO
-drwxr-xr-x   0 vandejer (1865779777) 296108113        0 2023-05-05 10:38:15.857689 mlpype-xgboost-0.4.0/mlpype_xgboost.egg-info/
--rw-r--r--   0 vandejer (1865779777) 296108113      101 2023-05-05 10:38:15.000000 mlpype-xgboost-0.4.0/mlpype_xgboost.egg-info/PKG-INFO
--rw-r--r--   0 vandejer (1865779777) 296108113      197 2023-05-05 10:38:15.000000 mlpype-xgboost-0.4.0/mlpype_xgboost.egg-info/SOURCES.txt
--rw-r--r--   0 vandejer (1865779777) 296108113        1 2023-05-05 10:38:15.000000 mlpype-xgboost-0.4.0/mlpype_xgboost.egg-info/dependency_links.txt
--rw-r--r--   0 vandejer (1865779777) 296108113      164 2023-05-05 10:38:15.000000 mlpype-xgboost-0.4.0/mlpype_xgboost.egg-info/requires.txt
--rw-r--r--   0 vandejer (1865779777) 296108113        1 2023-05-05 10:38:15.000000 mlpype-xgboost-0.4.0/mlpype_xgboost.egg-info/top_level.txt
--rw-r--r--   0 vandejer (1865779777) 296108113       38 2023-05-05 10:38:15.859179 mlpype-xgboost-0.4.0/setup.cfg
--rw-r--r--   0 vandejer (1865779777) 296108113      504 2023-05-05 10:18:55.000000 mlpype-xgboost-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:47:49.038107 mlpype-xgboost-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-20 16:47:49.038107 mlpype-xgboost-0.4.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:47:49.038107 mlpype-xgboost-0.4.1/mlpype_xgboost.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-20 16:47:49.000000 mlpype-xgboost-0.4.1/mlpype_xgboost.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-20 16:47:49.000000 mlpype-xgboost-0.4.1/mlpype_xgboost.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:47:49.000000 mlpype-xgboost-0.4.1/mlpype_xgboost.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-20 16:47:49.000000 mlpype-xgboost-0.4.1/mlpype_xgboost.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:47:49.000000 mlpype-xgboost-0.4.1/mlpype_xgboost.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 16:47:49.038107 mlpype-xgboost-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-20 16:43:35.000000 mlpype-xgboost-0.4.1/setup.py
```

