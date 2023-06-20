# Comparing `tmp/kurvy-1.0.0.tar.gz` & `tmp/kurvy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kurvy-1.0.0.tar", last modified: Fri May 19 09:53:39 2023, max compression
+gzip compressed data, was "kurvy-1.0.1.tar", last modified: Tue Jun 20 08:44:25 2023, max compression
```

## Comparing `kurvy-1.0.0.tar` & `kurvy-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 lucbatty   (501) staff       (20)        0 2023-05-19 09:53:39.154419 kurvy-1.0.0/
--rw-r--r--   0 lucbatty   (501) staff       (20)     1069 2023-05-19 09:22:17.000000 kurvy-1.0.0/LICENSE
--rw-r--r--   0 lucbatty   (501) staff       (20)      396 2023-05-19 09:53:39.153768 kurvy-1.0.0/PKG-INFO
--rw-r--r--   0 lucbatty   (501) staff       (20)        7 2023-05-19 09:22:17.000000 kurvy-1.0.0/README.md
-drwxr-xr-x   0 lucbatty   (501) staff       (20)        0 2023-05-19 09:53:39.149197 kurvy-1.0.0/kurvy/
--rw-r--r--   0 lucbatty   (501) staff       (20)       71 2023-05-19 09:51:28.000000 kurvy-1.0.0/kurvy/__init__.py
--rw-r--r--   0 lucbatty   (501) staff       (20)    12799 2023-05-19 09:51:29.000000 kurvy-1.0.0/kurvy/plots.py
--rw-r--r--   0 lucbatty   (501) staff       (20)    11813 2023-05-19 09:51:29.000000 kurvy-1.0.0/kurvy/trig.py
--rw-r--r--   0 lucbatty   (501) staff       (20)    23789 2023-05-19 09:51:29.000000 kurvy-1.0.0/kurvy/utils.py
-drwxr-xr-x   0 lucbatty   (501) staff       (20)        0 2023-05-19 09:53:39.152873 kurvy-1.0.0/kurvy.egg-info/
--rw-r--r--   0 lucbatty   (501) staff       (20)      396 2023-05-19 09:53:39.000000 kurvy-1.0.0/kurvy.egg-info/PKG-INFO
--rw-r--r--   0 lucbatty   (501) staff       (20)      219 2023-05-19 09:53:39.000000 kurvy-1.0.0/kurvy.egg-info/SOURCES.txt
--rw-r--r--   0 lucbatty   (501) staff       (20)        1 2023-05-19 09:53:39.000000 kurvy-1.0.0/kurvy.egg-info/dependency_links.txt
--rw-r--r--   0 lucbatty   (501) staff       (20)        6 2023-05-19 09:53:39.000000 kurvy-1.0.0/kurvy.egg-info/top_level.txt
--rw-r--r--   0 lucbatty   (501) staff       (20)      231 2023-05-19 09:51:14.000000 kurvy-1.0.0/pyproject.toml
--rw-r--r--   0 lucbatty   (501) staff       (20)       38 2023-05-19 09:53:39.154662 kurvy-1.0.0/setup.cfg
--rw-r--r--   0 lucbatty   (501) staff       (20)      598 2023-05-19 09:51:08.000000 kurvy-1.0.0/setup.py
+drwxr-xr-x   0 lucbatty   (501) staff       (20)        0 2023-06-20 08:44:25.328637 kurvy-1.0.1/
+-rw-r--r--   0 lucbatty   (501) staff       (20)     1069 2023-05-19 09:22:17.000000 kurvy-1.0.1/LICENSE
+-rw-r--r--   0 lucbatty   (501) staff       (20)      727 2023-06-20 08:44:25.328112 kurvy-1.0.1/PKG-INFO
+-rw-r--r--   0 lucbatty   (501) staff       (20)      338 2023-06-20 08:31:42.000000 kurvy-1.0.1/README.md
+drwxr-xr-x   0 lucbatty   (501) staff       (20)        0 2023-06-20 08:44:25.324926 kurvy-1.0.1/kurvy/
+-rw-r--r--   0 lucbatty   (501) staff       (20)       71 2023-05-19 09:51:28.000000 kurvy-1.0.1/kurvy/__init__.py
+-rw-r--r--   0 lucbatty   (501) staff       (20)    12401 2023-05-23 12:33:36.000000 kurvy-1.0.1/kurvy/plots.py
+-rw-r--r--   0 lucbatty   (501) staff       (20)    17670 2023-05-23 12:33:36.000000 kurvy-1.0.1/kurvy/trig.py
+-rw-r--r--   0 lucbatty   (501) staff       (20)     4475 2023-05-23 12:32:06.000000 kurvy-1.0.1/kurvy/utils.py
+drwxr-xr-x   0 lucbatty   (501) staff       (20)        0 2023-06-20 08:44:25.327336 kurvy-1.0.1/kurvy.egg-info/
+-rw-r--r--   0 lucbatty   (501) staff       (20)      727 2023-06-20 08:44:25.000000 kurvy-1.0.1/kurvy.egg-info/PKG-INFO
+-rw-r--r--   0 lucbatty   (501) staff       (20)      219 2023-06-20 08:44:25.000000 kurvy-1.0.1/kurvy.egg-info/SOURCES.txt
+-rw-r--r--   0 lucbatty   (501) staff       (20)        1 2023-06-20 08:44:25.000000 kurvy-1.0.1/kurvy.egg-info/dependency_links.txt
+-rw-r--r--   0 lucbatty   (501) staff       (20)        6 2023-06-20 08:44:25.000000 kurvy-1.0.1/kurvy.egg-info/top_level.txt
+-rw-r--r--   0 lucbatty   (501) staff       (20)      380 2023-06-20 08:41:26.000000 kurvy-1.0.1/pyproject.toml
+-rw-r--r--   0 lucbatty   (501) staff       (20)       38 2023-06-20 08:44:25.328849 kurvy-1.0.1/setup.cfg
+-rw-r--r--   0 lucbatty   (501) staff       (20)      598 2023-06-20 08:43:58.000000 kurvy-1.0.1/setup.py
```

### Comparing `kurvy-1.0.0/LICENSE` & `kurvy-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kurvy-1.0.0/kurvy/plots.py` & `kurvy-1.0.1/kurvy/plots.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,103 +5,101 @@
 
 from kurvy import utils
 
 
 def simple_plot(X_data, Y_data, test_data=None):
     fig, ax = plt.subplots(figsize=(12, 4))
 
-    ax.scatter(X_data, Y_data, color="teal", alpha=0.5, s=20)
+    # train data
+    ax.scatter(
+        X_data,
+        Y_data,
+        color="white",
+        edgecolors="teal",
+        alpha=0.5,
+        s=20,
+        zorder=-1,
+    )
 
+    # test data
     if test_data is not None:
-        # plot test data with big dots
         ax.scatter(
             test_data[:, 0],
             test_data[:, 1],
             color="mediumturquoise",
-            s=30,
             edgecolors="teal",
+            alpha=0.8,
+            s=20,
+            zorder=1,
         )
 
     ax.grid(visible=True)
     ax.set_axisbelow(True)
     plt.show()
 
 
-def pred_plot(model, X_data, Y_data, test_data=None, dots=True):
+def pred_plot(model, X_data, Y_data, test_data=None):
     Y_pred = model.predict(X_data)
     mse = np.round(utils.calculate_loss(Y_data, Y_pred), 4)
     r2 = np.round(utils.calculate_r2(Y_data, Y_pred), 4)
 
-    X_space = np.linspace(X_data[0], X_data[-1], 300)
+    X_space = np.linspace(np.min(X_data), np.max(X_data), 300)
     Y_predspace = model.predict(X_space)
 
-    plt.figure(figsize=(12, 4))
+    fig, ax = plt.subplots(figsize=(12, 4))
 
-    plt.plot(
+    # estimator
+    ax.plot(
         X_space,
         Y_predspace,
-        color="tomato",
-        linewidth=4,
-        alpha=0.7,
+        color="cyan",
+        linewidth=5,
+        alpha=0.8,
         solid_capstyle="round",
+        zorder=2,
     )
 
-    if test_data is None:
-        if dots:
-            plt.scatter(X_data, Y_data, color="teal", alpha=0.5, s=20)
-
-        else:
-            plt.plot(X_data, Y_data, color="teal", solid_capstyle="round")
-
-        plt.title(f"Loss = {mse}; R2 = {r2}")
-
-    else:
-        XY_train_recombined = np.dstack((X_data, Y_data))[0]
-
-        XY_recombined = np.vstack((XY_train_recombined, test_data))
-        XY_recombined = XY_recombined[np.argsort(XY_recombined[:, 0])]
-
-        if dots:
-            plt.scatter(
-                XY_recombined[:, 0],
-                XY_recombined[:, 1],
-                color="teal",
-                s=20,
-                alpha=0.5,
-            )
-
-        else:
-            plt.plot(
-                XY_recombined[:, 0],
-                XY_recombined[:, 1],
-                color="teal",
-                solid_capstyle="round",
-                zorder=-1,
-            )
+    # train data
+    ax.scatter(
+        X_data,
+        Y_data,
+        color="white",
+        edgecolors="teal",
+        alpha=0.5,
+        s=20,
+        zorder=-1,
+    )
 
-        # plot test data with big dots
-        plt.scatter(
+    # test data
+    if test_data is not None:
+        ax.scatter(
             test_data[:, 0],
             test_data[:, 1],
             color="mediumturquoise",
-            s=30,
             edgecolors="teal",
+            alpha=0.8,
+            s=20,
+            zorder=1,
         )
 
         Y_pred_test = model.predict(test_data[:, 0])
         test_mse = np.round(
             utils.calculate_loss(test_data[:, 1], Y_pred_test), 4
         )
         test_r2 = np.round(utils.calculate_r2(test_data[:, 1], Y_pred_test), 4)
 
-        plt.title(
-            f"Train Loss = {mse}; Train R2 = {r2}\nTest Loss = {test_mse}; Test R2 = {test_r2}"
+        ax.set_title(
+            f"Train Loss = {mse}  /  Train R2 = {r2}\nTest Loss = {test_mse}  /  Test R2 = {test_r2}"
         )
 
-    plt.grid(visible=True)
+    else:
+        ax.set_title(f"Loss = {mse}  /  tR2 = {r2}")
+
+    ax.grid(visible=True)
+    ax.set_axisbelow(True)
     plt.show()
 
 
 def plot_training(model, metric):
     best_loss = model.training_history[model.best_epoch][0]
     best_r2 = model.training_history[model.best_epoch][1]
     epochs = range(model.training_history.shape[0])
```

### Comparing `kurvy-1.0.0/setup.py` & `kurvy-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="kurvy",
-    version="1.0.0",
+    version="1.0.1",
     author="celerygemini",
     description="Curve approximation toolkit",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/celerygemini/kurvy",
     packages=setuptools.find_packages(),
     classifiers=[
```

