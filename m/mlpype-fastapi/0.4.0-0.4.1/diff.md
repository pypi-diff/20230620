# Comparing `tmp/mlpype-fastapi-0.4.0.tar.gz` & `tmp/mlpype-fastapi-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpype-fastapi-0.4.0.tar", last modified: Fri May  5 10:36:51 2023, max compression
+gzip compressed data, was "mlpype-fastapi-0.4.1.tar", last modified: Tue Jun 20 16:46:58 2023, max compression
```

## Comparing `mlpype-fastapi-0.4.0.tar` & `mlpype-fastapi-0.4.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 vandejer (1865779777) 296108113        0 2023-05-05 10:36:51.918599 mlpype-fastapi-0.4.0/
--rw-r--r--   0 vandejer (1865779777) 296108113      101 2023-05-05 10:36:51.918339 mlpype-fastapi-0.4.0/PKG-INFO
-drwxr-xr-x   0 vandejer (1865779777) 296108113        0 2023-05-05 10:36:51.917949 mlpype-fastapi-0.4.0/mlpype_fastapi.egg-info/
--rw-r--r--   0 vandejer (1865779777) 296108113      101 2023-05-05 10:36:51.000000 mlpype-fastapi-0.4.0/mlpype_fastapi.egg-info/PKG-INFO
--rw-r--r--   0 vandejer (1865779777) 296108113      197 2023-05-05 10:36:51.000000 mlpype-fastapi-0.4.0/mlpype_fastapi.egg-info/SOURCES.txt
--rw-r--r--   0 vandejer (1865779777) 296108113        1 2023-05-05 10:36:51.000000 mlpype-fastapi-0.4.0/mlpype_fastapi.egg-info/dependency_links.txt
--rw-r--r--   0 vandejer (1865779777) 296108113      138 2023-05-05 10:36:51.000000 mlpype-fastapi-0.4.0/mlpype_fastapi.egg-info/requires.txt
--rw-r--r--   0 vandejer (1865779777) 296108113        1 2023-05-05 10:36:51.000000 mlpype-fastapi-0.4.0/mlpype_fastapi.egg-info/top_level.txt
--rw-r--r--   0 vandejer (1865779777) 296108113       38 2023-05-05 10:36:51.918661 mlpype-fastapi-0.4.0/setup.cfg
--rw-r--r--   0 vandejer (1865779777) 296108113      537 2023-05-05 10:18:55.000000 mlpype-fastapi-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:46:58.477345 mlpype-fastapi-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-20 16:46:58.477345 mlpype-fastapi-0.4.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:46:58.477345 mlpype-fastapi-0.4.1/mlpype_fastapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-20 16:46:58.000000 mlpype-fastapi-0.4.1/mlpype_fastapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-20 16:46:58.000000 mlpype-fastapi-0.4.1/mlpype_fastapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:46:58.000000 mlpype-fastapi-0.4.1/mlpype_fastapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-20 16:46:58.000000 mlpype-fastapi-0.4.1/mlpype_fastapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:46:58.000000 mlpype-fastapi-0.4.1/mlpype_fastapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 16:46:58.477345 mlpype-fastapi-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-20 16:43:35.000000 mlpype-fastapi-0.4.1/setup.py
```

### Comparing `mlpype-fastapi-0.4.0/setup.py` & `mlpype-fastapi-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List
 
 from setuptools import find_namespace_packages, setup
 
 if __name__ == "__main__":
-    version = "0.4.0"
+    version = "0.4.1"
     deps: List[str] = [f"mlpype-base=={version}", "fastapi>=0.79.0"]
     dev_deps = ["uvicorn==0.18.2"]
     strict_deps = [s.replace(">=", "==") for s in deps]
 
     setup(
         name="mlpype-fastapi",
         install_requires=deps,
```

