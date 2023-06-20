# Comparing `tmp/mlpype-base-0.4.0.tar.gz` & `tmp/mlpype-base-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpype-base-0.4.0.tar", last modified: Fri May  5 10:36:40 2023, max compression
+gzip compressed data, was "mlpype-base-0.4.1.tar", last modified: Tue Jun 20 16:46:50 2023, max compression
```

## Comparing `mlpype-base-0.4.0.tar` & `mlpype-base-0.4.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 vandejer (1865779777) 296108113        0 2023-05-05 10:36:40.356929 mlpype-base-0.4.0/
--rw-r--r--   0 vandejer (1865779777) 296108113      119 2023-05-05 10:36:40.356628 mlpype-base-0.4.0/PKG-INFO
-drwxr-xr-x   0 vandejer (1865779777) 296108113        0 2023-05-05 10:36:40.356158 mlpype-base-0.4.0/mlpype_base.egg-info/
--rw-r--r--   0 vandejer (1865779777) 296108113      119 2023-05-05 10:36:40.000000 mlpype-base-0.4.0/mlpype_base.egg-info/PKG-INFO
--rw-r--r--   0 vandejer (1865779777) 296108113      182 2023-05-05 10:36:40.000000 mlpype-base-0.4.0/mlpype_base.egg-info/SOURCES.txt
--rw-r--r--   0 vandejer (1865779777) 296108113        1 2023-05-05 10:36:40.000000 mlpype-base-0.4.0/mlpype_base.egg-info/dependency_links.txt
--rw-r--r--   0 vandejer (1865779777) 296108113      453 2023-05-05 10:36:40.000000 mlpype-base-0.4.0/mlpype_base.egg-info/requires.txt
--rw-r--r--   0 vandejer (1865779777) 296108113        1 2023-05-05 10:36:40.000000 mlpype-base-0.4.0/mlpype_base.egg-info/top_level.txt
--rw-r--r--   0 vandejer (1865779777) 296108113       38 2023-05-05 10:36:40.357039 mlpype-base-0.4.0/setup.cfg
--rw-r--r--   0 vandejer (1865779777) 296108113      751 2023-05-05 10:18:55.000000 mlpype-base-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:46:50.220498 mlpype-base-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-20 16:46:50.220498 mlpype-base-0.4.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:46:50.220498 mlpype-base-0.4.1/mlpype_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-20 16:46:50.000000 mlpype-base-0.4.1/mlpype_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-20 16:46:50.000000 mlpype-base-0.4.1/mlpype_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:46:50.000000 mlpype-base-0.4.1/mlpype_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-20 16:46:50.000000 mlpype-base-0.4.1/mlpype_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:46:50.000000 mlpype-base-0.4.1/mlpype_base.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 16:46:50.220498 mlpype-base-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-20 16:43:35.000000 mlpype-base-0.4.1/setup.py
```

### Comparing `mlpype-base-0.4.0/setup.py` & `mlpype-base-0.4.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,22 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == "__main__":
-    version = "0.4.0"
+    version = "0.4.1"
 
     dev_deps = ["pre-commit", "build==0.8.0", "pypiserver==1.5.1", "twine==4.0.1", "pdoc==13.1.0"]
     test_deps = ["pytest", "pytest-cov"]
-    deps = [f"mlpype=={version}", "docstring_parser>=0.14.1", "pydantic>=1.9.1", "joblib>=1.1.0", "PyYAML==6.0"]
+    deps = [
+        f"mlpype=={version}",
+        "docstring_parser>=0.14.1",
+        "pydantic>=1.9.1",
+        "joblib>=1.1.0",
+        "PyYAML==6.0",
+        "jinja2==3.1.2",
+    ]
     strict_deps = [s.replace(">=", "==") for s in deps]
 
     setup(
         name="mlpype-base",
         install_requires=deps,
         extras_require={
             "dev": strict_deps + dev_deps + test_deps,
```

