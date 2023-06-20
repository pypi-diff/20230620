# Comparing `tmp/mlpype-mlflow-0.4.0.tar.gz` & `tmp/mlpype-mlflow-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpype-mlflow-0.4.0.tar", last modified: Fri May  5 10:37:23 2023, max compression
+gzip compressed data, was "mlpype-mlflow-0.4.1.tar", last modified: Tue Jun 20 16:47:16 2023, max compression
```

## Comparing `mlpype-mlflow-0.4.0.tar` & `mlpype-mlflow-0.4.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 vandejer (1865779777) 296108113        0 2023-05-05 10:37:23.466396 mlpype-mlflow-0.4.0/
--rw-r--r--   0 vandejer (1865779777) 296108113      100 2023-05-05 10:37:23.465711 mlpype-mlflow-0.4.0/PKG-INFO
-drwxr-xr-x   0 vandejer (1865779777) 296108113        0 2023-05-05 10:37:23.464978 mlpype-mlflow-0.4.0/mlpype_mlflow.egg-info/
--rw-r--r--   0 vandejer (1865779777) 296108113      100 2023-05-05 10:37:23.000000 mlpype-mlflow-0.4.0/mlpype_mlflow.egg-info/PKG-INFO
--rw-r--r--   0 vandejer (1865779777) 296108113      192 2023-05-05 10:37:23.000000 mlpype-mlflow-0.4.0/mlpype_mlflow.egg-info/SOURCES.txt
--rw-r--r--   0 vandejer (1865779777) 296108113        1 2023-05-05 10:37:23.000000 mlpype-mlflow-0.4.0/mlpype_mlflow.egg-info/dependency_links.txt
--rw-r--r--   0 vandejer (1865779777) 296108113      188 2023-05-05 10:37:23.000000 mlpype-mlflow-0.4.0/mlpype_mlflow.egg-info/requires.txt
--rw-r--r--   0 vandejer (1865779777) 296108113        1 2023-05-05 10:37:23.000000 mlpype-mlflow-0.4.0/mlpype_mlflow.egg-info/top_level.txt
--rw-r--r--   0 vandejer (1865779777) 296108113       38 2023-05-05 10:37:23.466520 mlpype-mlflow-0.4.0/setup.cfg
--rw-r--r--   0 vandejer (1865779777) 296108113      512 2023-05-05 10:18:55.000000 mlpype-mlflow-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:47:16.162923 mlpype-mlflow-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-20 16:47:16.162923 mlpype-mlflow-0.4.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:47:16.162923 mlpype-mlflow-0.4.1/mlpype_mlflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-20 16:47:16.000000 mlpype-mlflow-0.4.1/mlpype_mlflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-20 16:47:16.000000 mlpype-mlflow-0.4.1/mlpype_mlflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:47:16.000000 mlpype-mlflow-0.4.1/mlpype_mlflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-20 16:47:16.000000 mlpype-mlflow-0.4.1/mlpype_mlflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:47:16.000000 mlpype-mlflow-0.4.1/mlpype_mlflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 16:47:16.162923 mlpype-mlflow-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-20 16:43:35.000000 mlpype-mlflow-0.4.1/setup.py
```

### Comparing `mlpype-mlflow-0.4.0/setup.py` & `mlpype-mlflow-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == "__main__":
-    version = "0.4.0"
+    version = "0.4.1"
 
     deps = [
         f"mlpype-base=={version}",
         "mlflow>=1.28.0, <2.0",
         "GitPython>=3.1.27",
     ]
     strict_deps = [s.replace(">=", "==") for s in deps]
```

