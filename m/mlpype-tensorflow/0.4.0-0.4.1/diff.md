# Comparing `tmp/mlpype-tensorflow-0.4.0.tar.gz` & `tmp/mlpype-tensorflow-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpype-tensorflow-0.4.0.tar", last modified: Fri May  5 10:38:04 2023, max compression
+gzip compressed data, was "mlpype-tensorflow-0.4.1.tar", last modified: Tue Jun 20 16:47:40 2023, max compression
```

## Comparing `mlpype-tensorflow-0.4.0.tar` & `mlpype-tensorflow-0.4.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 vandejer (1865779777) 296108113        0 2023-05-05 10:38:04.566667 mlpype-tensorflow-0.4.0/
--rw-r--r--   0 vandejer (1865779777) 296108113      104 2023-05-05 10:38:04.566403 mlpype-tensorflow-0.4.0/PKG-INFO
-drwxr-xr-x   0 vandejer (1865779777) 296108113        0 2023-05-05 10:38:04.565878 mlpype-tensorflow-0.4.0/mlpype_tensorflow.egg-info/
--rw-r--r--   0 vandejer (1865779777) 296108113      104 2023-05-05 10:38:04.000000 mlpype-tensorflow-0.4.0/mlpype_tensorflow.egg-info/PKG-INFO
--rw-r--r--   0 vandejer (1865779777) 296108113      212 2023-05-05 10:38:04.000000 mlpype-tensorflow-0.4.0/mlpype_tensorflow.egg-info/SOURCES.txt
--rw-r--r--   0 vandejer (1865779777) 296108113        1 2023-05-05 10:38:04.000000 mlpype-tensorflow-0.4.0/mlpype_tensorflow.egg-info/dependency_links.txt
--rw-r--r--   0 vandejer (1865779777) 296108113      218 2023-05-05 10:38:04.000000 mlpype-tensorflow-0.4.0/mlpype_tensorflow.egg-info/requires.txt
--rw-r--r--   0 vandejer (1865779777) 296108113        1 2023-05-05 10:38:04.000000 mlpype-tensorflow-0.4.0/mlpype_tensorflow.egg-info/top_level.txt
--rw-r--r--   0 vandejer (1865779777) 296108113       38 2023-05-05 10:38:04.566717 mlpype-tensorflow-0.4.0/setup.cfg
--rw-r--r--   0 vandejer (1865779777) 296108113      623 2023-05-05 10:18:55.000000 mlpype-tensorflow-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:47:40.857306 mlpype-tensorflow-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-20 16:47:40.857306 mlpype-tensorflow-0.4.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:47:40.853305 mlpype-tensorflow-0.4.1/mlpype_tensorflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-20 16:47:40.000000 mlpype-tensorflow-0.4.1/mlpype_tensorflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-20 16:47:40.000000 mlpype-tensorflow-0.4.1/mlpype_tensorflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:47:40.000000 mlpype-tensorflow-0.4.1/mlpype_tensorflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-20 16:47:40.000000 mlpype-tensorflow-0.4.1/mlpype_tensorflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:47:40.000000 mlpype-tensorflow-0.4.1/mlpype_tensorflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 16:47:40.857306 mlpype-tensorflow-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-20 16:43:35.000000 mlpype-tensorflow-0.4.1/setup.py
```

### Comparing `mlpype-tensorflow-0.4.0/setup.py` & `mlpype-tensorflow-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == "__main__":
-    version = "0.4.0"
+    version = "0.4.1"
 
     deps = [
         f"mlpype-base=={version}",
         # on mac, it is recommended to use conda/mamba or source to install tensorflow
         "tensorflow>=2.12",
         "numpy>=1.23.0",
         "protobuf>=3.20.3",
```

