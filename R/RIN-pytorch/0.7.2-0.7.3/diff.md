# Comparing `tmp/RIN-pytorch-0.7.2.tar.gz` & `tmp/RIN-pytorch-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RIN-pytorch-0.7.2.tar", last modified: Wed Mar 22 21:08:42 2023, max compression
+gzip compressed data, was "RIN-pytorch-0.7.3.tar", last modified: Tue Jun 20 19:50:50 2023, max compression
```

## Comparing `RIN-pytorch-0.7.2.tar` & `RIN-pytorch-0.7.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 21:08:42.407834 RIN-pytorch-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-03-22 21:08:31.000000 RIN-pytorch-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-03-22 21:08:42.407834 RIN-pytorch-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-03-22 21:08:31.000000 RIN-pytorch-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 21:08:42.407834 RIN-pytorch-0.7.2/RIN_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-03-22 21:08:42.000000 RIN-pytorch-0.7.2/RIN_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-03-22 21:08:42.000000 RIN-pytorch-0.7.2/RIN_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 21:08:42.000000 RIN-pytorch-0.7.2/RIN_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-22 21:08:42.000000 RIN-pytorch-0.7.2/RIN_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-22 21:08:42.000000 RIN-pytorch-0.7.2/RIN_pytorch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 21:08:42.407834 RIN-pytorch-0.7.2/rin_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-22 21:08:31.000000 RIN-pytorch-0.7.2/rin_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32635 2023-03-22 21:08:31.000000 RIN-pytorch-0.7.2/rin_pytorch/rin_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-22 21:08:42.407834 RIN-pytorch-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-03-22 21:08:31.000000 RIN-pytorch-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:50:50.545798 RIN-pytorch-0.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-20 19:50:26.000000 RIN-pytorch-0.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-20 19:50:50.541798 RIN-pytorch-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-06-20 19:50:26.000000 RIN-pytorch-0.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:50:50.541798 RIN-pytorch-0.7.3/RIN_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-20 19:50:50.000000 RIN-pytorch-0.7.3/RIN_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-20 19:50:50.000000 RIN-pytorch-0.7.3/RIN_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 19:50:50.000000 RIN-pytorch-0.7.3/RIN_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-20 19:50:50.000000 RIN-pytorch-0.7.3/RIN_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-20 19:50:50.000000 RIN-pytorch-0.7.3/RIN_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:50:50.541798 RIN-pytorch-0.7.3/rin_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-20 19:50:26.000000 RIN-pytorch-0.7.3/rin_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32662 2023-06-20 19:50:26.000000 RIN-pytorch-0.7.3/rin_pytorch/rin_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 19:50:50.545798 RIN-pytorch-0.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-20 19:50:26.000000 RIN-pytorch-0.7.3/setup.py
```

### Comparing `RIN-pytorch-0.7.2/LICENSE` & `RIN-pytorch-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `RIN-pytorch-0.7.2/PKG-INFO` & `RIN-pytorch-0.7.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RIN-pytorch
-Version: 0.7.2
+Version: 0.7.3
 Summary: RIN - Recurrent Interface Network - Pytorch
 Home-page: https://github.com/lucidrains/RIN-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,attention mechanism,denoising diffusion,image and video generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `RIN-pytorch-0.7.2/README.md` & `RIN-pytorch-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `RIN-pytorch-0.7.2/RIN_pytorch.egg-info/PKG-INFO` & `RIN-pytorch-0.7.3/RIN_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RIN-pytorch
-Version: 0.7.2
+Version: 0.7.3
 Summary: RIN - Recurrent Interface Network - Pytorch
 Home-page: https://github.com/lucidrains/RIN-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,attention mechanism,denoising diffusion,image and video generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `RIN-pytorch-0.7.2/rin_pytorch/rin_pytorch.py` & `RIN-pytorch-0.7.3/rin_pytorch/rin_pytorch.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,16 @@
 
 def cycle(dl):
     while True:
         for data in dl:
             yield data
 
 def has_int_squareroot(num):
-    return (math.sqrt(num) ** 2) == num
+    num_sqrt = math.sqrt(num)
+    return int(num_sqrt) == num_sqrt
 
 def num_to_groups(num, divisor):
     groups = num // divisor
     remainder = num % divisor
     arr = [divisor] * groups
     if remainder > 0:
         arr.append(remainder)
```

### Comparing `RIN-pytorch-0.7.2/setup.py` & `RIN-pytorch-0.7.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'RIN-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.7.2',
+  version = '0.7.3',
   license='MIT',
   description = 'RIN - Recurrent Interface Network - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/RIN-pytorch',
   keywords = [
```

