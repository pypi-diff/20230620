# Comparing `tmp/cqt-nsgt-pytorch-0.0.8.tar.gz` & `tmp/cqt-nsgt-pytorch-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cqt-nsgt-pytorch-0.0.8.tar", last modified: Wed Dec 28 15:26:54 2022, max compression
+gzip compressed data, was "cqt-nsgt-pytorch-0.0.9.tar", last modified: Tue Jun 20 17:42:24 2023, max compression
```

## Comparing `cqt-nsgt-pytorch-0.0.8.tar` & `cqt-nsgt-pytorch-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 molinee2 (3243725) domain users (70000)        0 2022-12-28 15:26:54.297296 cqt-nsgt-pytorch-0.0.8/
--rw-r--r--   0 molinee2 (3243725) domain users (70000)      642 2022-12-28 15:26:54.297296 cqt-nsgt-pytorch-0.0.8/PKG-INFO
--rw-r--r--   0 molinee2 (3243725) domain users (70000)     2864 2022-12-02 19:26:42.000000 cqt-nsgt-pytorch-0.0.8/README.md
-drwxr-xr-x   0 molinee2 (3243725) domain users (70000)        0 2022-12-28 15:26:54.297296 cqt-nsgt-pytorch-0.0.8/cqt_nsgt_pytorch/
--rw-r--r--   0 molinee2 (3243725) domain users (70000)    30127 2022-12-28 15:25:02.000000 cqt-nsgt-pytorch-0.0.8/cqt_nsgt_pytorch/CQT_nsgt.py
--rw-r--r--   0 molinee2 (3243725) domain users (70000)       30 2022-11-23 22:06:57.000000 cqt-nsgt-pytorch-0.0.8/cqt_nsgt_pytorch/__init__.py
--rw-r--r--   0 molinee2 (3243725) domain users (70000)     3574 2022-12-16 17:33:53.000000 cqt-nsgt-pytorch-0.0.8/cqt_nsgt_pytorch/fscale.py
--rw-r--r--   0 molinee2 (3243725) domain users (70000)     1398 2022-11-23 19:16:12.000000 cqt-nsgt-pytorch-0.0.8/cqt_nsgt_pytorch/nsdual.py
--rw-rw-r--   0 molinee2 (3243725) domain users (70000)     3401 2022-12-02 18:42:47.000000 cqt-nsgt-pytorch-0.0.8/cqt_nsgt_pytorch/nsgfwin.py
--rw-r--r--   0 molinee2 (3243725) domain users (70000)     2732 2022-12-02 19:23:18.000000 cqt-nsgt-pytorch-0.0.8/cqt_nsgt_pytorch/util.py
-drwxr-xr-x   0 molinee2 (3243725) domain users (70000)        0 2022-12-28 15:26:54.297296 cqt-nsgt-pytorch-0.0.8/cqt_nsgt_pytorch.egg-info/
--rw-r--r--   0 molinee2 (3243725) domain users (70000)      642 2022-12-28 15:26:54.000000 cqt-nsgt-pytorch-0.0.8/cqt_nsgt_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 molinee2 (3243725) domain users (70000)      382 2022-12-28 15:26:54.000000 cqt-nsgt-pytorch-0.0.8/cqt_nsgt_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 molinee2 (3243725) domain users (70000)        1 2022-12-28 15:26:54.000000 cqt-nsgt-pytorch-0.0.8/cqt_nsgt_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 molinee2 (3243725) domain users (70000)       28 2022-12-28 15:26:54.000000 cqt-nsgt-pytorch-0.0.8/cqt_nsgt_pytorch.egg-info/requires.txt
--rw-r--r--   0 molinee2 (3243725) domain users (70000)       17 2022-12-28 15:26:54.000000 cqt-nsgt-pytorch-0.0.8/cqt_nsgt_pytorch.egg-info/top_level.txt
--rw-r--r--   0 molinee2 (3243725) domain users (70000)       38 2022-12-28 15:26:54.297296 cqt-nsgt-pytorch-0.0.8/setup.cfg
--rw-r--r--   0 molinee2 (3243725) domain users (70000)      885 2022-12-28 15:26:18.000000 cqt-nsgt-pytorch-0.0.8/setup.py
+drwxrwsr-x   0 molinee2 (3243725) molinee2 (3243725)        0 2023-06-20 17:42:24.000000 cqt-nsgt-pytorch-0.0.9/
+-rw-rw-r--   0 molinee2 (3243725) molinee2 (3243725)      642 2023-06-20 17:42:24.000000 cqt-nsgt-pytorch-0.0.9/PKG-INFO
+-rw-rw-r--   0 molinee2 (3243725) molinee2 (3243725)     2864 2022-12-02 23:13:48.000000 cqt-nsgt-pytorch-0.0.9/README.md
+drwxrwsr-x   0 molinee2 (3243725) molinee2 (3243725)        0 2023-06-20 17:42:24.000000 cqt-nsgt-pytorch-0.0.9/cqt_nsgt_pytorch/
+-rw-rw-r--   0 molinee2 (3243725) molinee2 (3243725)    30839 2023-06-20 17:29:25.000000 cqt-nsgt-pytorch-0.0.9/cqt_nsgt_pytorch/CQT_nsgt.py
+-rw-rw-r--   0 molinee2 (3243725) molinee2 (3243725)       30 2022-11-24 16:28:43.000000 cqt-nsgt-pytorch-0.0.9/cqt_nsgt_pytorch/__init__.py
+-rw-rw-r--   0 molinee2 (3243725) molinee2 (3243725)     3574 2023-06-20 17:25:48.000000 cqt-nsgt-pytorch-0.0.9/cqt_nsgt_pytorch/fscale.py
+-rw-rw-r--   0 molinee2 (3243725) molinee2 (3243725)     1398 2022-11-24 16:28:43.000000 cqt-nsgt-pytorch-0.0.9/cqt_nsgt_pytorch/nsdual.py
+-rw-rw-r--   0 molinee2 (3243725) molinee2 (3243725)     3401 2022-12-02 23:13:48.000000 cqt-nsgt-pytorch-0.0.9/cqt_nsgt_pytorch/nsgfwin.py
+-rw-rw-r--   0 molinee2 (3243725) molinee2 (3243725)     2732 2022-12-02 23:13:48.000000 cqt-nsgt-pytorch-0.0.9/cqt_nsgt_pytorch/util.py
+drwxrwsr-x   0 molinee2 (3243725) molinee2 (3243725)        0 2023-06-20 17:42:24.000000 cqt-nsgt-pytorch-0.0.9/cqt_nsgt_pytorch.egg-info/
+-rw-rw-r--   0 molinee2 (3243725) molinee2 (3243725)      642 2023-06-20 17:42:24.000000 cqt-nsgt-pytorch-0.0.9/cqt_nsgt_pytorch.egg-info/PKG-INFO
+-rw-rw-r--   0 molinee2 (3243725) molinee2 (3243725)      382 2023-06-20 17:42:24.000000 cqt-nsgt-pytorch-0.0.9/cqt_nsgt_pytorch.egg-info/SOURCES.txt
+-rw-rw-r--   0 molinee2 (3243725) molinee2 (3243725)        1 2023-06-20 17:42:24.000000 cqt-nsgt-pytorch-0.0.9/cqt_nsgt_pytorch.egg-info/dependency_links.txt
+-rw-rw-r--   0 molinee2 (3243725) molinee2 (3243725)       28 2023-06-20 17:42:24.000000 cqt-nsgt-pytorch-0.0.9/cqt_nsgt_pytorch.egg-info/requires.txt
+-rw-rw-r--   0 molinee2 (3243725) molinee2 (3243725)       17 2023-06-20 17:42:24.000000 cqt-nsgt-pytorch-0.0.9/cqt_nsgt_pytorch.egg-info/top_level.txt
+-rw-rw-r--   0 molinee2 (3243725) molinee2 (3243725)       38 2023-06-20 17:42:24.000000 cqt-nsgt-pytorch-0.0.9/setup.cfg
+-rw-rw-r--   0 molinee2 (3243725) molinee2 (3243725)      886 2023-06-20 17:31:48.000000 cqt-nsgt-pytorch-0.0.9/setup.py
```

### Comparing `cqt-nsgt-pytorch-0.0.8/PKG-INFO` & `cqt-nsgt-pytorch-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cqt-nsgt-pytorch
-Version: 0.0.8
+Version: 0.0.9
 Summary: Pytorch implementation of an invertible and differentiable Constant-Q Transform based Non-stationary Gabor Transform (NSGT) for audio processing.
 Home-page: https://github.com/eloimoliner/CQT_pytorch
 Author: Eloi Moliner
 Author-email: eloi.moliner@aalto.fi
 License: MIT
 Keywords: audio processing,constant-q transform,deep learning,pytorch,nsgt
 Classifier: Development Status :: 4 - Beta
```

### Comparing `cqt-nsgt-pytorch-0.0.8/README.md` & `cqt-nsgt-pytorch-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cqt-nsgt-pytorch-0.0.8/cqt_nsgt_pytorch/CQT_nsgt.py` & `cqt-nsgt-pytorch-0.0.9/cqt_nsgt_pytorch/CQT_nsgt.py`

 * *Files 3% similar despite different names*

```diff
@@ -343,22 +343,42 @@
             Lg = len(gdii)
             wr1 = win_range[:(Lg)//2]
             wr2 = win_range[-((Lg+1)//2):]
             p = (wr1,wr2,Lg)
             self.loopparams_dec.append(p)
 
     def apply_hpf_DC(self, x):
+        Lin=x.shape[-1]
+        if Lin<self.Ls:
+            #pad zeros
+            x=torch.nn.functional.pad(x, (0, self.Ls-Lin))
+        elif Lin> self.Ls:
+            raise ValueError("Input signal is longer than the maximum length. I could have patched it, but I didn't. sorry :(")
+
         X=torch.fft.fft(x)
         X=X*torch.conj(self.Hhpf)
-        return torch.fft.ifft(X).real
+        out= torch.fft.ifft(X).real
+        if Lin<self.Ls:
+            out=out[:, :Lin]
+        return out
+
 
     def apply_lpf_DC(self, x):
+        Lin=x.shape[-1]
+        if Lin<self.Ls:
+            #pad zeros
+            x=torch.nn.functional.pad(x, (0, self.Ls-Lin))
+        elif Lin> self.Ls:
+            raise ValueError("Input signal is longer than the maximum length. I could have patched it, but I didn't. sorry :(")
         X=torch.fft.fft(x)
         X=X*torch.conj(self.Hlpf)
-        return torch.fft.ifft(X).real
+        out= torch.fft.ifft(X).real
+        if Lin<self.Ls:
+            out=out[:, :Lin]
+        return out
 
 
     def nsgtf(self,f):
         """
             forward transform
             args:
                 t: Tensor shape(B, C, T) time-domain waveform
```

### Comparing `cqt-nsgt-pytorch-0.0.8/cqt_nsgt_pytorch/fscale.py` & `cqt-nsgt-pytorch-0.0.9/cqt_nsgt_pytorch/fscale.py`

 * *Files identical despite different names*

### Comparing `cqt-nsgt-pytorch-0.0.8/cqt_nsgt_pytorch/nsdual.py` & `cqt-nsgt-pytorch-0.0.9/cqt_nsgt_pytorch/nsdual.py`

 * *Files identical despite different names*

### Comparing `cqt-nsgt-pytorch-0.0.8/cqt_nsgt_pytorch/nsgfwin.py` & `cqt-nsgt-pytorch-0.0.9/cqt_nsgt_pytorch/nsgfwin.py`

 * *Files identical despite different names*

### Comparing `cqt-nsgt-pytorch-0.0.8/cqt_nsgt_pytorch/util.py` & `cqt-nsgt-pytorch-0.0.9/cqt_nsgt_pytorch/util.py`

 * *Files identical despite different names*

### Comparing `cqt-nsgt-pytorch-0.0.8/cqt_nsgt_pytorch.egg-info/PKG-INFO` & `cqt-nsgt-pytorch-0.0.9/cqt_nsgt_pytorch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cqt-nsgt-pytorch
-Version: 0.0.8
+Version: 0.0.9
 Summary: Pytorch implementation of an invertible and differentiable Constant-Q Transform based Non-stationary Gabor Transform (NSGT) for audio processing.
 Home-page: https://github.com/eloimoliner/CQT_pytorch
 Author: Eloi Moliner
 Author-email: eloi.moliner@aalto.fi
 License: MIT
 Keywords: audio processing,constant-q transform,deep learning,pytorch,nsgt
 Classifier: Development Status :: 4 - Beta
```

### Comparing `cqt-nsgt-pytorch-0.0.8/setup.py` & `cqt-nsgt-pytorch-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages, setup
 
 setup(
     name="cqt-nsgt-pytorch",
     packages=find_packages(exclude=[]),
-    version="0.0.8",
+    version="0.0.9",
     license="MIT",
     description="Pytorch implementation of an invertible and differentiable Constant-Q Transform based Non-stationary Gabor Transform (NSGT) for audio processing.",
     long_description_content_type="text/markdown",
     author="Eloi Moliner",
     author_email="eloi.moliner@aalto.fi",
     url="https://github.com/eloimoliner/CQT_pytorch",
     keywords=["audio processing", "constant-q transform", "deep learning", "pytorch", "nsgt"],
@@ -17,8 +17,8 @@
     ],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.6",
     ],
-)
+)
```

