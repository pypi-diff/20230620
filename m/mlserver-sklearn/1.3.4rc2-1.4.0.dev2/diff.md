# Comparing `tmp/mlserver-sklearn-1.3.4rc2.tar.gz` & `tmp/mlserver-sklearn-1.4.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlserver-sklearn-1.3.4rc2.tar", last modified: Tue Jun 20 09:09:42 2023, max compression
+gzip compressed data, was "mlserver-sklearn-1.4.0.dev2.tar", last modified: Thu May  4 09:30:47 2023, max compression
```

## Comparing `mlserver-sklearn-1.3.4rc2.tar` & `mlserver-sklearn-1.4.0.dev2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:09:42.594207 mlserver-sklearn-1.3.4rc2/
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-06-20 09:08:54.000000 mlserver-sklearn-1.3.4rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-06-20 09:09:42.594207 mlserver-sklearn-1.3.4rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-20 09:08:54.000000 mlserver-sklearn-1.3.4rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:09:42.590206 mlserver-sklearn-1.3.4rc2/mlserver_sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-20 09:08:54.000000 mlserver-sklearn-1.3.4rc2/mlserver_sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-06-20 09:08:54.000000 mlserver-sklearn-1.3.4rc2/mlserver_sklearn/sklearn.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-20 09:08:54.000000 mlserver-sklearn-1.3.4rc2/mlserver_sklearn/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:09:42.590206 mlserver-sklearn-1.3.4rc2/mlserver_sklearn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-06-20 09:09:42.000000 mlserver-sklearn-1.3.4rc2/mlserver_sklearn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-20 09:09:42.000000 mlserver-sklearn-1.3.4rc2/mlserver_sklearn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 09:09:42.000000 mlserver-sklearn-1.3.4rc2/mlserver_sklearn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-20 09:09:42.000000 mlserver-sklearn-1.3.4rc2/mlserver_sklearn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-20 09:09:42.000000 mlserver-sklearn-1.3.4rc2/mlserver_sklearn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 09:09:42.594207 mlserver-sklearn-1.3.4rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-20 09:08:54.000000 mlserver-sklearn-1.3.4rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:47.090384 mlserver-sklearn-1.4.0.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-05-04 09:30:02.000000 mlserver-sklearn-1.4.0.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-04 09:30:47.090384 mlserver-sklearn-1.4.0.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-04 09:30:02.000000 mlserver-sklearn-1.4.0.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:47.090384 mlserver-sklearn-1.4.0.dev2/mlserver_sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-04 09:30:02.000000 mlserver-sklearn-1.4.0.dev2/mlserver_sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-05-04 09:30:02.000000 mlserver-sklearn-1.4.0.dev2/mlserver_sklearn/sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-04 09:30:02.000000 mlserver-sklearn-1.4.0.dev2/mlserver_sklearn/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:47.090384 mlserver-sklearn-1.4.0.dev2/mlserver_sklearn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-04 09:30:46.000000 mlserver-sklearn-1.4.0.dev2/mlserver_sklearn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-04 09:30:47.000000 mlserver-sklearn-1.4.0.dev2/mlserver_sklearn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 09:30:46.000000 mlserver-sklearn-1.4.0.dev2/mlserver_sklearn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-04 09:30:46.000000 mlserver-sklearn-1.4.0.dev2/mlserver_sklearn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-04 09:30:46.000000 mlserver-sklearn-1.4.0.dev2/mlserver_sklearn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 09:30:47.094384 mlserver-sklearn-1.4.0.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-04 09:30:02.000000 mlserver-sklearn-1.4.0.dev2/setup.py
```

### Comparing `mlserver-sklearn-1.3.4rc2/LICENSE` & `mlserver-sklearn-1.4.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `mlserver-sklearn-1.3.4rc2/mlserver_sklearn/sklearn.py` & `mlserver-sklearn-1.4.0.dev2/mlserver_sklearn/sklearn.py`

 * *Files identical despite different names*

### Comparing `mlserver-sklearn-1.3.4rc2/setup.py` & `mlserver-sklearn-1.4.0.dev2/setup.py`

 * *Files identical despite different names*

