# Comparing `tmp/DeepLogTimedelta-0.2.0.tar.gz` & `tmp/DeepLogTimedelta-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DeepLogTimedelta-0.2.0.tar", last modified: Tue Jun 20 07:07:18 2023, max compression
+gzip compressed data, was "DeepLogTimedelta-0.2.1.tar", last modified: Tue Jun 20 07:17:27 2023, max compression
```

## Comparing `DeepLogTimedelta-0.2.0.tar` & `DeepLogTimedelta-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 07:07:18.509819 DeepLogTimedelta-0.2.0/
-drwxrwxrwx   0        0        0        0 2023-06-20 07:07:18.463077 DeepLogTimedelta-0.2.0/DeepLogTimedelta/
--rw-rw-rw-   0        0        0     3629 2023-06-20 07:06:04.000000 DeepLogTimedelta-0.2.0/DeepLogTimedelta/DeepLogTimedelta.py
--rw-rw-rw-   0        0        0        0 2023-06-19 12:37:56.000000 DeepLogTimedelta-0.2.0/DeepLogTimedelta/__init__.py
--rw-rw-rw-   0        0        0       97 2023-06-19 11:56:09.000000 DeepLogTimedelta-0.2.0/DeepLogTimedelta/main.py
--rw-rw-rw-   0        0        0     2311 2023-06-19 13:46:57.000000 DeepLogTimedelta-0.2.0/DeepLogTimedelta/preproccesing.py
-drwxrwxrwx   0        0        0        0 2023-06-20 07:07:18.501819 DeepLogTimedelta-0.2.0/DeepLogTimedelta.egg-info/
--rw-rw-rw-   0        0        0      207 2023-06-20 07:07:17.000000 DeepLogTimedelta-0.2.0/DeepLogTimedelta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2023-06-20 07:07:18.000000 DeepLogTimedelta-0.2.0/DeepLogTimedelta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 07:07:17.000000 DeepLogTimedelta-0.2.0/DeepLogTimedelta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-20 07:07:17.000000 DeepLogTimedelta-0.2.0/DeepLogTimedelta.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      207 2023-06-20 07:07:18.509819 DeepLogTimedelta-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-20 07:07:18.509819 DeepLogTimedelta-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      335 2023-06-20 07:06:38.000000 DeepLogTimedelta-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 07:17:27.672398 DeepLogTimedelta-0.2.1/
+drwxrwxrwx   0        0        0        0 2023-06-20 07:17:27.604555 DeepLogTimedelta-0.2.1/DeepLogTimedelta/
+-rw-rw-rw-   0        0        0     3466 2023-06-20 07:16:43.000000 DeepLogTimedelta-0.2.1/DeepLogTimedelta/DeepLogTimedelta.py
+-rw-rw-rw-   0        0        0        0 2023-06-19 12:37:56.000000 DeepLogTimedelta-0.2.1/DeepLogTimedelta/__init__.py
+-rw-rw-rw-   0        0        0       97 2023-06-19 11:56:09.000000 DeepLogTimedelta-0.2.1/DeepLogTimedelta/main.py
+-rw-rw-rw-   0        0        0     2311 2023-06-19 13:46:57.000000 DeepLogTimedelta-0.2.1/DeepLogTimedelta/preproccesing.py
+drwxrwxrwx   0        0        0        0 2023-06-20 07:17:27.664398 DeepLogTimedelta-0.2.1/DeepLogTimedelta.egg-info/
+-rw-rw-rw-   0        0        0      207 2023-06-20 07:17:27.000000 DeepLogTimedelta-0.2.1/DeepLogTimedelta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2023-06-20 07:17:27.000000 DeepLogTimedelta-0.2.1/DeepLogTimedelta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 07:17:27.000000 DeepLogTimedelta-0.2.1/DeepLogTimedelta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-20 07:17:27.000000 DeepLogTimedelta-0.2.1/DeepLogTimedelta.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      207 2023-06-20 07:17:27.664398 DeepLogTimedelta-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-20 07:17:27.672398 DeepLogTimedelta-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      335 2023-06-20 07:17:19.000000 DeepLogTimedelta-0.2.1/setup.py
```

### Comparing `DeepLogTimedelta-0.2.0/DeepLogTimedelta/DeepLogTimedelta.py` & `DeepLogTimedelta-0.2.1/DeepLogTimedelta/DeepLogTimedelta.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import torch
 import torchtrain
 from torch import nn
 import torch.nn.functional as F
 import torch.optim as optim
 import numpy as np
 
+
 class DeepLogTimedelta(torchtrain.Module):
     def __init__(self, input_size, hidden_size, output_size, num_layers=2):
         super().__init__()
         self.input_size = input_size
         self.hidden_size = hidden_size
         self.output_size = output_size
         self.num_layers = num_layers
@@ -34,29 +35,25 @@
         return torch.zeros(
             self.num_layers,
             X.size(0),
             self.hidden_size
         ).to(X.device)
 
     def predict(self, X, y,
-                epochs=10,
                 batch_size=32,
-                learning_rate=0.01,
-                criterion=nn.NLLLoss,
-                optimizer=optim.SGD,
                 by_method='abs'):
         methods = ['abs', 'std']
         if by_method not in methods:
             raise ValueError(f'method must be {methods}')
-        result = super().predict(X, y, epochs, batch_size, learning_rate, criterion, optimizer)
+        result = super().predict(X=X, batch_size=batch_size)
 
         if by_method == 'abs':
-            return self.result_abs(y,result)
+            return self.result_abs(y, result)
         elif by_method == 'std':
-            return self.result_std(y,result)
+            return self.result_std(y, result)
 
     def fit_predict(self, X, y,
                     epochs=10,
                     batch_size=32,
                     learning_rate=0.01,
                     criterion=nn.NLLLoss,
                     optimizer=optim.SGD,
@@ -96,16 +93,16 @@
                         epochs,
                         batch_size,
                         learning_rate,
                         criterion,
                         optimizer,
                         ).predict(X, y, epochs, batch_size, learning_rate, criterion, optimizer, by_method='abs')
 
-    def result_abs(self,y_true,y_pred):
+    def result_abs(self, y_true, y_pred):
         result = np.abs(y_true - y_pred)
         return result
 
-    def result_std(self,y_true,y_pred):
-        std_2 = np.std(y_true,axis = 0) * 2
-        vfunc = np.vectorize(lambda x: 1 if x in range(x-std_2,x+std_2+1) else 0)
+    def result_std(self, y_true, y_pred):
+        std_2 = np.std(y_true, axis=0) * 2
+        vfunc = np.vectorize(lambda x: 1 if x in range(x - std_2, x + std_2 + 1) else 0)
         result = vfunc(y_pred)
         return result
```

### Comparing `DeepLogTimedelta-0.2.0/DeepLogTimedelta/preproccesing.py` & `DeepLogTimedelta-0.2.1/DeepLogTimedelta/preproccesing.py`

 * *Files identical despite different names*

