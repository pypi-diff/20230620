# Comparing `tmp/Denoising_Diffusion_Probabilistic_Models-0.0.0.6-py3-none-any.whl.zip` & `tmp/Denoising_Diffusion_Probabilistic_Models-0.0.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1873 bytes, number of entries: 6
--rw-r--r--  2.0 unx       44 b- defN 23-Jun-20 09:39 diffusion/Test.py
--rw-r--r--  2.0 unx       62 b- defN 23-Jun-20 09:39 diffusion/__init__.py
--rw-r--r--  2.0 unx      432 b- defN 23-Jun-20 09:39 Denoising_Diffusion_Probabilistic_Models-0.0.0.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-20 09:39 Denoising_Diffusion_Probabilistic_Models-0.0.0.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Jun-20 09:39 Denoising_Diffusion_Probabilistic_Models-0.0.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      585 b- defN 23-Jun-20 09:39 Denoising_Diffusion_Probabilistic_Models-0.0.0.6.dist-info/RECORD
-6 files, 1225 bytes uncompressed, 783 bytes compressed:  36.1%
+Zip file size: 1909 bytes, number of entries: 6
+-rw-r--r--  2.0 unx      137 b- defN 23-Jun-20 11:26 diffusion/Test.py
+-rw-r--r--  2.0 unx       57 b- defN 23-Jun-20 11:26 diffusion/__init__.py
+-rw-r--r--  2.0 unx      432 b- defN 23-Jun-20 11:26 Denoising_Diffusion_Probabilistic_Models-0.0.0.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-20 11:26 Denoising_Diffusion_Probabilistic_Models-0.0.0.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-20 11:26 Denoising_Diffusion_Probabilistic_Models-0.0.0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      586 b- defN 23-Jun-20 11:26 Denoising_Diffusion_Probabilistic_Models-0.0.0.7.dist-info/RECORD
+6 files, 1314 bytes uncompressed, 819 bytes compressed:  37.7%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: diffusion/Test.py
 Comment: 
 
 Filename: diffusion/__init__.py
 Comment: 
 
-Filename: Denoising_Diffusion_Probabilistic_Models-0.0.0.6.dist-info/METADATA
+Filename: Denoising_Diffusion_Probabilistic_Models-0.0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: Denoising_Diffusion_Probabilistic_Models-0.0.0.6.dist-info/WHEEL
+Filename: Denoising_Diffusion_Probabilistic_Models-0.0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: Denoising_Diffusion_Probabilistic_Models-0.0.0.6.dist-info/top_level.txt
+Filename: Denoising_Diffusion_Probabilistic_Models-0.0.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: Denoising_Diffusion_Probabilistic_Models-0.0.0.6.dist-info/RECORD
+Filename: Denoising_Diffusion_Probabilistic_Models-0.0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## diffusion/Test.py

```diff
@@ -1,4 +1,10 @@
 print('Test')
+class Test():
+  def __init__(self):
+    print('Test1')
+
+  def test(self):
+    print('Test2')
 
 def f1():
   print('test f1')
```

## diffusion/__init__.py

```diff
@@ -1,3 +1,3 @@
 import sys
 sys.path.append('../')
-from .diffusion import Test
+from .Test import Test
```

