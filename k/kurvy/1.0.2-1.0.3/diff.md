# Comparing `tmp/kurvy-1.0.2.tar.gz` & `tmp/kurvy-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kurvy-1.0.2.tar", last modified: Tue Jun 20 08:50:57 2023, max compression
+gzip compressed data, was "kurvy-1.0.3.tar", last modified: Tue Jun 20 14:53:15 2023, max compression
```

## Comparing `kurvy-1.0.2.tar` & `kurvy-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 lucbatty   (501) staff       (20)        0 2023-06-20 08:50:57.336665 kurvy-1.0.2/
--rw-r--r--   0 lucbatty   (501) staff       (20)     1069 2023-05-19 09:22:17.000000 kurvy-1.0.2/LICENSE
--rw-r--r--   0 lucbatty   (501) staff       (20)      831 2023-06-20 08:50:57.336287 kurvy-1.0.2/PKG-INFO
--rw-r--r--   0 lucbatty   (501) staff       (20)      338 2023-06-20 08:31:42.000000 kurvy-1.0.2/README.md
-drwxr-xr-x   0 lucbatty   (501) staff       (20)        0 2023-06-20 08:50:57.332279 kurvy-1.0.2/kurvy/
--rw-r--r--   0 lucbatty   (501) staff       (20)       71 2023-05-19 09:51:28.000000 kurvy-1.0.2/kurvy/__init__.py
--rw-r--r--   0 lucbatty   (501) staff       (20)    12401 2023-05-23 12:33:36.000000 kurvy-1.0.2/kurvy/plots.py
--rw-r--r--   0 lucbatty   (501) staff       (20)    17670 2023-05-23 12:33:36.000000 kurvy-1.0.2/kurvy/trig.py
--rw-r--r--   0 lucbatty   (501) staff       (20)     4475 2023-05-23 12:32:06.000000 kurvy-1.0.2/kurvy/utils.py
-drwxr-xr-x   0 lucbatty   (501) staff       (20)        0 2023-06-20 08:50:57.335725 kurvy-1.0.2/kurvy.egg-info/
--rw-r--r--   0 lucbatty   (501) staff       (20)      831 2023-06-20 08:50:57.000000 kurvy-1.0.2/kurvy.egg-info/PKG-INFO
--rw-r--r--   0 lucbatty   (501) staff       (20)      219 2023-06-20 08:50:57.000000 kurvy-1.0.2/kurvy.egg-info/SOURCES.txt
--rw-r--r--   0 lucbatty   (501) staff       (20)        1 2023-06-20 08:50:57.000000 kurvy-1.0.2/kurvy.egg-info/dependency_links.txt
--rw-r--r--   0 lucbatty   (501) staff       (20)        6 2023-06-20 08:50:57.000000 kurvy-1.0.2/kurvy.egg-info/top_level.txt
--rw-r--r--   0 lucbatty   (501) staff       (20)      231 2023-06-20 08:47:52.000000 kurvy-1.0.2/pyproject.toml
--rw-r--r--   0 lucbatty   (501) staff       (20)       38 2023-06-20 08:50:57.336833 kurvy-1.0.2/setup.cfg
--rw-r--r--   0 lucbatty   (501) staff       (20)      702 2023-06-20 08:50:22.000000 kurvy-1.0.2/setup.py
+drwxr-xr-x   0 lucbatty   (501) staff       (20)        0 2023-06-20 14:53:15.720199 kurvy-1.0.3/
+-rw-r--r--   0 lucbatty   (501) staff       (20)     1069 2023-05-19 09:22:17.000000 kurvy-1.0.3/LICENSE
+-rw-r--r--   0 lucbatty   (501) staff       (20)     1956 2023-06-20 14:53:15.719536 kurvy-1.0.3/PKG-INFO
+-rw-r--r--   0 lucbatty   (501) staff       (20)     1463 2023-06-20 14:50:34.000000 kurvy-1.0.3/README.md
+drwxr-xr-x   0 lucbatty   (501) staff       (20)        0 2023-06-20 14:53:15.715255 kurvy-1.0.3/kurvy/
+-rw-r--r--   0 lucbatty   (501) staff       (20)       71 2023-05-19 09:51:28.000000 kurvy-1.0.3/kurvy/__init__.py
+-rw-r--r--   0 lucbatty   (501) staff       (20)    14489 2023-06-20 14:08:40.000000 kurvy-1.0.3/kurvy/plots.py
+-rw-r--r--   0 lucbatty   (501) staff       (20)    28987 2023-06-20 14:08:41.000000 kurvy-1.0.3/kurvy/trig.py
+-rw-r--r--   0 lucbatty   (501) staff       (20)     6692 2023-06-20 14:08:40.000000 kurvy-1.0.3/kurvy/utils.py
+drwxr-xr-x   0 lucbatty   (501) staff       (20)        0 2023-06-20 14:53:15.718561 kurvy-1.0.3/kurvy.egg-info/
+-rw-r--r--   0 lucbatty   (501) staff       (20)     1956 2023-06-20 14:53:15.000000 kurvy-1.0.3/kurvy.egg-info/PKG-INFO
+-rw-r--r--   0 lucbatty   (501) staff       (20)      219 2023-06-20 14:53:15.000000 kurvy-1.0.3/kurvy.egg-info/SOURCES.txt
+-rw-r--r--   0 lucbatty   (501) staff       (20)        1 2023-06-20 14:53:15.000000 kurvy-1.0.3/kurvy.egg-info/dependency_links.txt
+-rw-r--r--   0 lucbatty   (501) staff       (20)        6 2023-06-20 14:53:15.000000 kurvy-1.0.3/kurvy.egg-info/top_level.txt
+-rw-r--r--   0 lucbatty   (501) staff       (20)      231 2023-06-20 08:47:52.000000 kurvy-1.0.3/pyproject.toml
+-rw-r--r--   0 lucbatty   (501) staff       (20)       38 2023-06-20 14:53:15.720459 kurvy-1.0.3/setup.cfg
+-rw-r--r--   0 lucbatty   (501) staff       (20)      700 2023-06-20 14:53:08.000000 kurvy-1.0.3/setup.py
```

### Comparing `kurvy-1.0.2/LICENSE` & `kurvy-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kurvy-1.0.2/kurvy/plots.py` & `kurvy-1.0.3/kurvy/plots.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import numpy as np
 import matplotlib.pyplot as plt
 from tqdm import tqdm
 import copy
-
 from kurvy import utils
 
 
 def simple_plot(X_data, Y_data, test_data=None):
+    """
+    Plots data with test data shown as empty markers, if given.
+    """
+
     fig, ax = plt.subplots(figsize=(12, 4))
 
-    # train data
+    # main data
     ax.scatter(
         X_data,
         Y_data,
         color="white",
         edgecolors="teal",
         alpha=0.5,
         s=20,
@@ -33,15 +36,45 @@
         )
 
     ax.grid(visible=True)
     ax.set_axisbelow(True)
     plt.show()
 
 
-def pred_plot(model, X_data, Y_data, test_data=None):
+def pred_plot(model, X_data, Y_data, test_data=None, results=False):
+    """
+    Plots data and predicted curve with test data shown as empty markers, if
+    given.
+
+    Args:
+    -----
+
+        model (kurvy.trig.TrigModel): initialised TrigModel object.
+
+        X_data (1-D array): X data array.
+
+        Y_data (1-D array): Y data array.
+
+    Kwargs:
+    -------
+
+        test_data (2-D array, default = None): D-stacked X & Y test data. If
+        none, no test data will be plotted.
+
+        results (bool, default = False): whether of not to print the evaluation
+        metrics (MSE loss and R2).
+
+    Returns:
+    --------
+
+        Plot showing the real and predicted data.
+
+        MSE loss and R2 evaluation results, if 'results' is set to True.
+    """
+
     Y_pred = model.predict(X_data)
     mse = np.round(utils.calculate_loss(Y_data, Y_pred), 4)
     r2 = np.round(utils.calculate_r2(Y_data, Y_pred), 4)
 
     X_space = np.linspace(np.min(X_data), np.max(X_data), 300)
     Y_predspace = model.predict(X_space)
 
@@ -83,27 +116,48 @@
 
         Y_pred_test = model.predict(test_data[:, 0])
         test_mse = np.round(
             utils.calculate_loss(test_data[:, 1], Y_pred_test), 4
         )
         test_r2 = np.round(utils.calculate_r2(test_data[:, 1], Y_pred_test), 4)
 
-        ax.set_title(
-            f"Train Loss = {mse}  /  Train R2 = {r2}\nTest Loss = {test_mse}  /  Test R2 = {test_r2}"
-        )
+        if results:
+            print(f"Train Loss = {mse}  /  Train R2 = {r2}")
+            print(f"Test Loss = {test_mse}  /  Test R2 = {test_r2}")
 
     else:
-        ax.set_title(f"Loss = {mse}  /  tR2 = {r2}")
+        if results:
+            print(f"Train Loss = {mse}  /  Train R2 = {r2}")
 
+    ax.set_title("Real vs. Predicted")
     ax.grid(visible=True)
     ax.set_axisbelow(True)
     plt.show()
 
 
 def plot_training(model, metric):
+    """
+    Plots training training history.
+
+    Args:
+    -----
+
+        model (kurvy.trig.TrigModel): initialised and trained TrigModel object.
+
+        metric (str): metric to plot. Acceptable values are:
+            'loss' for MSE loss.
+            'r2' for R-squared value.
+            'both' for both MSE and R2.
+
+    Returns:
+    --------
+
+        Plot showing chosen metric over the training epochs.
+    """
+
     best_loss = model.training_history[model.best_epoch][0]
     best_r2 = model.training_history[model.best_epoch][1]
     epochs = range(model.training_history.shape[0])
     titles = ["Loss", "R-Squared"]
 
     if (metric == "loss") or (metric == "r2"):
         if metric == "loss":
@@ -163,14 +217,38 @@
         plt.show()
 
     else:
         raise ValueError(f"Unkown metric: {metric}.")
 
 
 def loss_vis(model, param_name, markers=False):
+    """
+    Plots parameter and loss value, showing how the value has changed over the
+    training epochs.
+
+    Args:
+    -----
+
+        model (kurvy.trig.TrigModel): initialised and trained TrigModel object.
+
+        param_name (str): One of "a", "b", "c", "d", or "e".
+
+    Kwargs:
+    -------
+
+        markers (bool, default = False): whether or not to show markers for
+        each epoch.
+
+    Returns:
+    --------
+
+        Plot showing the change in loss with respect to the change in parameter
+        value over the training epochs.
+    """
+
     if model.training_history is None:
         raise ValueError("No training history - model has not yet been fit.")
 
     if model.params[param_name]["trainable"]:
         best_overall_loss = model.best_epoch
 
         col = "abcde".find(param_name) + 2
@@ -185,34 +263,42 @@
 
         ax.scatter(
             p_values[0],
             loss_values[0],
             color="white",
             edgecolors="royalblue",
             s=60,
+            label="start",
         )
         if markers:
             ax.plot(
                 p_values,
                 loss_values,
                 color="royalblue",
                 zorder=-1,
                 marker="o",
             )
         else:
             ax.plot(p_values, loss_values, color="royalblue", zorder=-1)
 
-        ax.scatter(p_values[-1], loss_values[-1], color="royalblue", s=60)
+        ax.scatter(
+            p_values[-1], loss_values[-1], color="royalblue", s=60, label="end"
+        )
         ax.scatter(
             best_value_overall,
             best_loss_overall,
             color="red",
             edgecolors="royalblue",
             s=60,
+            label="best",
         )
+        ax.set_xlabel("Parameter Value")
+        ax.set_ylabel("Loss")
+        ax.set_title(f"'{param_name}' Param Value Loss Evolution")
+        ax.legend()
 
         plt.show()
 
     else:
         raise ValueError(f"{param_name} is not a trainable parameter.")
```

### Comparing `kurvy-1.0.2/setup.py` & `kurvy-1.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="kurvy",
-    version="1.0.2",
+    version="1.0.3",
     author="celerygemini",
     description="Curve approximation toolkit",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/celerygemini/kurvy",
     packages=setuptools.find_packages(),
-    classifiers = [
+    classifiers=[
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.9",
```

