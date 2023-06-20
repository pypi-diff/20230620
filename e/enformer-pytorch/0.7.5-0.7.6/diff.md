# Comparing `tmp/enformer-pytorch-0.7.5.tar.gz` & `tmp/enformer-pytorch-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enformer-pytorch-0.7.5.tar", last modified: Mon May 29 17:29:49 2023, max compression
+gzip compressed data, was "enformer-pytorch-0.7.6.tar", last modified: Tue Jun 20 15:11:04 2023, max compression
```

## Comparing `enformer-pytorch-0.7.5.tar` & `enformer-pytorch-0.7.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:29:49.622995 enformer-pytorch-0.7.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-29 17:29:38.000000 enformer-pytorch-0.7.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-29 17:29:38.000000 enformer-pytorch-0.7.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-29 17:29:49.622995 enformer-pytorch-0.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12222 2023-05-29 17:29:38.000000 enformer-pytorch-0.7.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:29:49.622995 enformer-pytorch-0.7.5/enformer_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-29 17:29:38.000000 enformer-pytorch-0.7.5/enformer_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-29 17:29:38.000000 enformer-pytorch-0.7.5/enformer_pytorch/config_enformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-05-29 17:29:38.000000 enformer-pytorch-0.7.5/enformer_pytorch/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    12764 2023-05-29 17:29:38.000000 enformer-pytorch-0.7.5/enformer_pytorch/finetune.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-29 17:29:38.000000 enformer-pytorch-0.7.5/enformer_pytorch/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    13835 2023-05-29 17:29:38.000000 enformer-pytorch-0.7.5/enformer_pytorch/modeling_enformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:29:49.622995 enformer-pytorch-0.7.5/enformer_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-29 17:29:49.000000 enformer-pytorch-0.7.5/enformer_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-29 17:29:49.000000 enformer-pytorch-0.7.5/enformer_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 17:29:49.000000 enformer-pytorch-0.7.5/enformer_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-29 17:29:49.000000 enformer-pytorch-0.7.5/enformer_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-29 17:29:49.000000 enformer-pytorch-0.7.5/enformer_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 17:29:49.622995 enformer-pytorch-0.7.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-29 17:29:38.000000 enformer-pytorch-0.7.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:04.344051 enformer-pytorch-0.7.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-20 15:10:54.000000 enformer-pytorch-0.7.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-20 15:10:54.000000 enformer-pytorch-0.7.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-20 15:11:04.344051 enformer-pytorch-0.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12222 2023-06-20 15:10:54.000000 enformer-pytorch-0.7.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:04.340052 enformer-pytorch-0.7.6/enformer_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-20 15:10:54.000000 enformer-pytorch-0.7.6/enformer_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-20 15:10:54.000000 enformer-pytorch-0.7.6/enformer_pytorch/config_enformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-06-20 15:10:54.000000 enformer-pytorch-0.7.6/enformer_pytorch/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12764 2023-06-20 15:10:54.000000 enformer-pytorch-0.7.6/enformer_pytorch/finetune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-06-20 15:10:54.000000 enformer-pytorch-0.7.6/enformer_pytorch/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13835 2023-06-20 15:10:54.000000 enformer-pytorch-0.7.6/enformer_pytorch/modeling_enformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:04.344051 enformer-pytorch-0.7.6/enformer_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-20 15:11:04.000000 enformer-pytorch-0.7.6/enformer_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-20 15:11:04.000000 enformer-pytorch-0.7.6/enformer_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:11:04.000000 enformer-pytorch-0.7.6/enformer_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-20 15:11:04.000000 enformer-pytorch-0.7.6/enformer_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-20 15:11:04.000000 enformer-pytorch-0.7.6/enformer_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 15:11:04.344051 enformer-pytorch-0.7.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-20 15:10:54.000000 enformer-pytorch-0.7.6/setup.py
```

### Comparing `enformer-pytorch-0.7.5/LICENSE` & `enformer-pytorch-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `enformer-pytorch-0.7.5/PKG-INFO` & `enformer-pytorch-0.7.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enformer-pytorch
-Version: 0.7.5
+Version: 0.7.6
 Summary: Enformer - Pytorch
 Home-page: https://github.com/lucidrains/enformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,transformer,gene-expression
 Classifier: Development Status :: 4 - Beta
```

### Comparing `enformer-pytorch-0.7.5/README.md` & `enformer-pytorch-0.7.6/README.md`

 * *Files identical despite different names*

### Comparing `enformer-pytorch-0.7.5/enformer_pytorch/config_enformer.py` & `enformer-pytorch-0.7.6/enformer_pytorch/config_enformer.py`

 * *Files identical despite different names*

### Comparing `enformer-pytorch-0.7.5/enformer_pytorch/data.py` & `enformer-pytorch-0.7.6/enformer_pytorch/data.py`

 * *Files identical despite different names*

### Comparing `enformer-pytorch-0.7.5/enformer_pytorch/finetune.py` & `enformer-pytorch-0.7.6/enformer_pytorch/finetune.py`

 * *Files identical despite different names*

### Comparing `enformer-pytorch-0.7.5/enformer_pytorch/metrics.py` & `enformer-pytorch-0.7.6/enformer_pytorch/metrics.py`

 * *Files identical despite different names*

### Comparing `enformer-pytorch-0.7.5/enformer_pytorch/modeling_enformer.py` & `enformer-pytorch-0.7.6/enformer_pytorch/modeling_enformer.py`

 * *Files identical despite different names*

### Comparing `enformer-pytorch-0.7.5/enformer_pytorch.egg-info/PKG-INFO` & `enformer-pytorch-0.7.6/enformer_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enformer-pytorch
-Version: 0.7.5
+Version: 0.7.6
 Summary: Enformer - Pytorch
 Home-page: https://github.com/lucidrains/enformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,transformer,gene-expression
 Classifier: Development Status :: 4 - Beta
```

### Comparing `enformer-pytorch-0.7.5/setup.py` & `enformer-pytorch-0.7.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'enformer-pytorch',
   packages = find_packages(exclude=[]),
   include_package_data = True,
-  version = '0.7.5',
+  version = '0.7.6',
   license='MIT',
   description = 'Enformer - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/enformer-pytorch',
   keywords = [
     'artificial intelligence',
     'transformer',
     'gene-expression'
   ],
   install_requires=[
-    'discrete-key-value-bottleneck-pytorch',
+    'discrete-key-value-bottleneck-pytorch>=0.0.8',
     'einops>=0.3',
     'numpy',
     'torch>=1.6',
     'torchmetrics',
     'polars',
     'pyfaidx',
     'pyyaml',
```

