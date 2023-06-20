# Comparing `tmp/DeepLogTimedelta-0.2.2.2.tar.gz` & `tmp/DeepLogTimedelta-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DeepLogTimedelta-0.2.2.2.tar", last modified: Tue Jun 20 08:44:31 2023, max compression
+gzip compressed data, was "DeepLogTimedelta-0.3.0.tar", last modified: Tue Jun 20 12:27:13 2023, max compression
```

## Comparing `DeepLogTimedelta-0.2.2.2.tar` & `DeepLogTimedelta-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 08:44:31.164505 DeepLogTimedelta-0.2.2.2/
-drwxrwxrwx   0        0        0        0 2023-06-20 08:44:31.146208 DeepLogTimedelta-0.2.2.2/DeepLogTimedelta/
--rw-rw-rw-   0        0        0     3500 2023-06-20 08:44:23.000000 DeepLogTimedelta-0.2.2.2/DeepLogTimedelta/DeepLogTimedelta.py
--rw-rw-rw-   0        0        0        0 2023-06-19 12:37:56.000000 DeepLogTimedelta-0.2.2.2/DeepLogTimedelta/__init__.py
--rw-rw-rw-   0        0        0       97 2023-06-19 11:56:09.000000 DeepLogTimedelta-0.2.2.2/DeepLogTimedelta/main.py
--rw-rw-rw-   0        0        0     2311 2023-06-19 13:46:57.000000 DeepLogTimedelta-0.2.2.2/DeepLogTimedelta/preproccesing.py
-drwxrwxrwx   0        0        0        0 2023-06-20 08:44:31.161362 DeepLogTimedelta-0.2.2.2/DeepLogTimedelta.egg-info/
--rw-rw-rw-   0        0        0      209 2023-06-20 08:44:30.000000 DeepLogTimedelta-0.2.2.2/DeepLogTimedelta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2023-06-20 08:44:31.000000 DeepLogTimedelta-0.2.2.2/DeepLogTimedelta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 08:44:30.000000 DeepLogTimedelta-0.2.2.2/DeepLogTimedelta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-20 08:44:30.000000 DeepLogTimedelta-0.2.2.2/DeepLogTimedelta.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      209 2023-06-20 08:44:31.163498 DeepLogTimedelta-0.2.2.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-20 08:44:31.164505 DeepLogTimedelta-0.2.2.2/setup.cfg
--rw-rw-rw-   0        0        0      337 2023-06-20 08:44:27.000000 DeepLogTimedelta-0.2.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 12:27:13.732711 DeepLogTimedelta-0.3.0/
+drwxrwxrwx   0        0        0        0 2023-06-20 12:27:13.719564 DeepLogTimedelta-0.3.0/DeepLogTimedelta/
+-rw-rw-rw-   0        0        0     3681 2023-06-20 12:26:05.000000 DeepLogTimedelta-0.3.0/DeepLogTimedelta/DeepLogTimedelta.py
+-rw-rw-rw-   0        0        0        0 2023-06-19 12:37:56.000000 DeepLogTimedelta-0.3.0/DeepLogTimedelta/__init__.py
+-rw-rw-rw-   0        0        0       97 2023-06-19 11:56:09.000000 DeepLogTimedelta-0.3.0/DeepLogTimedelta/main.py
+-rw-rw-rw-   0        0        0     2311 2023-06-19 13:46:57.000000 DeepLogTimedelta-0.3.0/DeepLogTimedelta/preproccesing.py
+drwxrwxrwx   0        0        0        0 2023-06-20 12:27:13.729762 DeepLogTimedelta-0.3.0/DeepLogTimedelta.egg-info/
+-rw-rw-rw-   0        0        0      207 2023-06-20 12:27:13.000000 DeepLogTimedelta-0.3.0/DeepLogTimedelta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2023-06-20 12:27:13.000000 DeepLogTimedelta-0.3.0/DeepLogTimedelta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 12:27:13.000000 DeepLogTimedelta-0.3.0/DeepLogTimedelta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-20 12:27:13.000000 DeepLogTimedelta-0.3.0/DeepLogTimedelta.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      207 2023-06-20 12:27:13.731714 DeepLogTimedelta-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-20 12:27:13.732711 DeepLogTimedelta-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      335 2023-06-20 12:26:09.000000 DeepLogTimedelta-0.3.0/setup.py
```

### Comparing `DeepLogTimedelta-0.2.2.2/DeepLogTimedelta/DeepLogTimedelta.py` & `DeepLogTimedelta-0.3.0/DeepLogTimedelta/DeepLogTimedelta.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import torch.optim as optim
 import numpy as np
 
 
 class DeepLogTimedelta(torchtrain.Module):
     def __init__(self, input_size, hidden_size, output_size, num_layers=2):
         super().__init__()
+
         self.input_size = input_size
         self.hidden_size = hidden_size
         self.output_size = output_size
         self.num_layers = num_layers
 
         self.lstm = nn.LSTM(input_size, hidden_size, num_layers, batch_first=True)
         self.out = nn.Linear(hidden_size, output_size)
@@ -34,27 +35,14 @@
         """Return a given hidden state for X."""
         return torch.zeros(
             self.num_layers,
             X.size(0),
             self.hidden_size
         ).to(X.device)
 
-    def predict(self, X, y,
-                batch_size=32,
-                by_method='abs'):
-        methods = ['abs', 'std']
-        if by_method not in methods:
-            raise ValueError(f'method must be {methods}')
-        result = super().predict(X=X, batch_size=batch_size)
-
-        if by_method == 'abs':
-            return self.result_abs(y, result)
-        elif by_method == 'std':
-            return self.result_std(y, result)
-
     def fit_predict(self, X, y,
                     epochs=10,
                     batch_size=32,
                     learning_rate=0.01,
                     criterion=nn.NLLLoss,
                     optimizer=optim.SGD,
                     by_method='abs'):
@@ -85,25 +73,43 @@
 
             by_method: str, method use for implement result
             Returns
             -------
             result : torch.Tensor
                 Resulting prediction
             """
-        return self.fit(X, y,
-                        epochs,
+        return self.fit(X,
                         batch_size,
-                        learning_rate,
-                        criterion,
-                        optimizer,
-                        ).predict(X, y, epochs, batch_size, learning_rate, criterion, optimizer, by_method='abs')
+                        ).predict(X=X, batch_size=batch_size)
 
     def result_abs(self, y_true, y_pred):
         result = np.abs(y_true - y_pred)
         return result
 
-    def result_std(self, y_true, y_pred):
+    def result_std(self, y_true, y_pred, koef=2):
         flatten_y = y_true.flatten()
-        std_2 = torch.std(flatten_y).item() * 2
-        vfunc = np.vectorize(lambda x: 1 if x - std_2 <= x <= x + std_2 else 0)
-        result = vfunc(y_pred)
+        std_2 = torch.std(flatten_y).item() * koef
+        result = []
+        y_pred = y_pred.flatten()
+        for i in range(len(y_pred)):
+            if y_true[i] - std_2 <= y_pred[i] <= y_true[i] + std_2:
+                result.append(1)
+            else:
+                result.append(0)
         return result
+
+    def result_std_mean(self, y_true, koef=2, window=20):
+        y_true = y_true.flatten()
+        result = [0 for i in range(window)]
+        for i in range(window, len(y_true) - window):
+            temp_values = y_true[i - window:i + window + 1]
+            temp_std = torch.std(temp_values).item()
+            temp_mean = torch.mean(temp_values).item()
+            if y_true[i] > temp_mean + temp_std * koef:
+                result.append(1)
+            else:
+                result.append(0)
+        for i in range(window):
+            result.append(0)
+        return result
+
+    # mean , get point by window, find mean and std, get koef and x20>mean+std*koef
```

### Comparing `DeepLogTimedelta-0.2.2.2/DeepLogTimedelta/preproccesing.py` & `DeepLogTimedelta-0.3.0/DeepLogTimedelta/preproccesing.py`

 * *Files identical despite different names*

