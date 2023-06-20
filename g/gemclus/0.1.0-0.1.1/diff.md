# Comparing `tmp/gemclus-0.1.0.tar.gz` & `tmp/gemclus-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemclus-0.1.0.tar", last modified: Fri May 12 18:02:26 2023, max compression
+gzip compressed data, was "gemclus-0.1.1.tar", last modified: Tue Jun 20 14:36:11 2023, max compression
```

## Comparing `gemclus-0.1.0.tar` & `gemclus-0.1.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-05-12 18:02:26.249091 gemclus-0.1.0/
--rw-rw-r--   0 louis     (1000) louis     (1000)      705 2023-04-27 12:43:01.000000 gemclus-0.1.0/LICENSE
--rw-rw-r--   0 louis     (1000) louis     (1000)       51 2023-04-27 12:04:58.000000 gemclus-0.1.0/MANIFEST.in
--rw-rw-r--   0 louis     (1000) louis     (1000)     3325 2023-05-12 18:02:26.249091 gemclus-0.1.0/PKG-INFO
--rw-rw-r--   0 louis     (1000) louis     (1000)     2010 2023-05-10 08:55:34.000000 gemclus-0.1.0/README.md
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-05-12 18:02:26.245092 gemclus-0.1.0/gemclus/
--rw-rw-r--   0 louis     (1000) louis     (1000)      162 2023-05-12 18:01:12.000000 gemclus-0.1.0/gemclus/__init__.py
--rw-rw-r--   0 louis     (1000) louis     (1000)    18744 2023-05-12 18:00:55.000000 gemclus-0.1.0/gemclus/_base_gemini.py
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-05-12 18:02:26.245092 gemclus-0.1.0/gemclus/data/
--rw-rw-r--   0 louis     (1000) louis     (1000)      116 2023-05-10 08:55:34.000000 gemclus-0.1.0/gemclus/data/__init__.py
--rw-rw-r--   0 louis     (1000) louis     (1000)    11869 2023-05-12 18:00:55.000000 gemclus-0.1.0/gemclus/data/synthetic_data.py
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-05-12 18:02:26.245092 gemclus-0.1.0/gemclus/gemini/
--rw-rw-r--   0 louis     (1000) louis     (1000)      125 2023-05-12 18:00:55.000000 gemclus-0.1.0/gemclus/gemini/__init__.py
--rw-rw-r--   0 louis     (1000) louis     (1000)    15507 2023-05-12 18:00:55.000000 gemclus-0.1.0/gemclus/gemini/_gemini_losses.py
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-05-12 18:02:26.249091 gemclus-0.1.0/gemclus/linear/
--rw-rw-r--   0 louis     (1000) louis     (1000)      116 2023-03-29 14:26:07.000000 gemclus-0.1.0/gemclus/linear/__init__.py
--rw-rw-r--   0 louis     (1000) louis     (1000)    12833 2023-05-12 18:00:55.000000 gemclus-0.1.0/gemclus/linear/_linear_geminis.py
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-05-12 18:02:26.249091 gemclus-0.1.0/gemclus/mlp/
--rw-rw-r--   0 louis     (1000) louis     (1000)       89 2023-03-29 14:26:07.000000 gemclus-0.1.0/gemclus/mlp/__init__.py
--rw-rw-r--   0 louis     (1000) louis     (1000)    11321 2023-05-12 18:00:55.000000 gemclus-0.1.0/gemclus/mlp/_mlp_geminis.py
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-05-12 18:02:26.249091 gemclus-0.1.0/gemclus/nonparametric/
--rw-rw-r--   0 louis     (1000) louis     (1000)      128 2023-05-12 18:00:55.000000 gemclus-0.1.0/gemclus/nonparametric/__init__.py
--rw-rw-r--   0 louis     (1000) louis     (1000)     8172 2023-05-12 18:00:55.000000 gemclus-0.1.0/gemclus/nonparametric/_categorical_models.py
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-05-12 18:02:26.249091 gemclus-0.1.0/gemclus/sparse/
--rw-rw-r--   0 louis     (1000) louis     (1000)      129 2023-03-29 14:26:07.000000 gemclus-0.1.0/gemclus/sparse/__init__.py
--rw-rw-r--   0 louis     (1000) louis     (1000)    24304 2023-05-12 18:00:55.000000 gemclus-0.1.0/gemclus/sparse/_base_sparse.py
--rw-rw-r--   0 louis     (1000) louis     (1000)     5437 2023-05-10 08:55:34.000000 gemclus-0.1.0/gemclus/sparse/_linear_sparse.py
--rw-rw-r--   0 louis     (1000) louis     (1000)     5988 2023-05-12 18:00:55.000000 gemclus-0.1.0/gemclus/sparse/_mlp_sparse.py
--rw-rw-r--   0 louis     (1000) louis     (1000)     2422 2023-05-12 18:00:55.000000 gemclus-0.1.0/gemclus/sparse/_prox_grad.py
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-05-12 18:02:26.249091 gemclus-0.1.0/gemclus/tests/
--rw-rw-r--   0 louis     (1000) louis     (1000)        0 2023-03-29 14:26:07.000000 gemclus-0.1.0/gemclus/tests/__init__.py
--rw-rw-r--   0 louis     (1000) louis     (1000)     2808 2023-05-10 08:55:34.000000 gemclus-0.1.0/gemclus/tests/test_data.py
--rw-rw-r--   0 louis     (1000) louis     (1000)     4508 2023-05-12 18:00:55.000000 gemclus-0.1.0/gemclus/tests/test_default.py
--rw-rw-r--   0 louis     (1000) louis     (1000)     3248 2023-05-12 18:00:55.000000 gemclus-0.1.0/gemclus/tests/test_objectives.py
--rw-rw-r--   0 louis     (1000) louis     (1000)     5708 2023-05-12 18:00:55.000000 gemclus-0.1.0/gemclus/tests/test_path.py
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-05-12 18:02:26.245092 gemclus-0.1.0/gemclus.egg-info/
--rw-rw-r--   0 louis     (1000) louis     (1000)     3325 2023-05-12 18:02:26.000000 gemclus-0.1.0/gemclus.egg-info/PKG-INFO
--rw-rw-r--   0 louis     (1000) louis     (1000)      909 2023-05-12 18:02:26.000000 gemclus-0.1.0/gemclus.egg-info/SOURCES.txt
--rw-rw-r--   0 louis     (1000) louis     (1000)        1 2023-05-12 18:02:26.000000 gemclus-0.1.0/gemclus.egg-info/dependency_links.txt
--rw-rw-r--   0 louis     (1000) louis     (1000)        1 2023-05-12 18:02:26.000000 gemclus-0.1.0/gemclus.egg-info/not-zip-safe
--rw-rw-r--   0 louis     (1000) louis     (1000)      130 2023-05-12 18:02:26.000000 gemclus-0.1.0/gemclus.egg-info/requires.txt
--rw-rw-r--   0 louis     (1000) louis     (1000)        8 2023-05-12 18:02:26.000000 gemclus-0.1.0/gemclus.egg-info/top_level.txt
--rw-rw-r--   0 louis     (1000) louis     (1000)       97 2023-04-27 14:33:43.000000 gemclus-0.1.0/pyproject.toml
--rw-rw-r--   0 louis     (1000) louis     (1000)       50 2023-05-10 08:55:34.000000 gemclus-0.1.0/requirements.txt
--rw-rw-r--   0 louis     (1000) louis     (1000)      147 2023-05-12 18:02:26.249091 gemclus-0.1.0/setup.cfg
--rw-rw-r--   0 louis     (1000) louis     (1000)     2525 2023-04-27 15:56:32.000000 gemclus-0.1.0/setup.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-20 14:36:11.063765 gemclus-0.1.1/
+-rw-rw-r--   0 louis     (1000) louis     (1000)     1562 2023-06-20 14:32:43.000000 gemclus-0.1.1/LICENSE
+-rw-rw-r--   0 louis     (1000) louis     (1000)       51 2023-04-27 12:04:58.000000 gemclus-0.1.1/MANIFEST.in
+-rw-rw-r--   0 louis     (1000) louis     (1000)     3471 2023-06-20 14:36:11.063765 gemclus-0.1.1/PKG-INFO
+-rw-rw-r--   0 louis     (1000) louis     (1000)     2306 2023-06-20 12:36:09.000000 gemclus-0.1.1/README.md
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-20 14:36:11.059765 gemclus-0.1.1/gemclus/
+-rw-rw-r--   0 louis     (1000) louis     (1000)      179 2023-06-20 13:18:52.000000 gemclus-0.1.1/gemclus/__init__.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)    18744 2023-05-12 18:00:55.000000 gemclus-0.1.1/gemclus/_base_gemini.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-20 14:36:11.059765 gemclus-0.1.1/gemclus/data/
+-rw-rw-r--   0 louis     (1000) louis     (1000)      116 2023-05-10 08:55:34.000000 gemclus-0.1.1/gemclus/data/__init__.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)    11852 2023-06-20 12:26:55.000000 gemclus-0.1.1/gemclus/data/synthetic_data.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-20 14:36:11.059765 gemclus-0.1.1/gemclus/gemini/
+-rw-rw-r--   0 louis     (1000) louis     (1000)      125 2023-05-12 18:00:55.000000 gemclus-0.1.1/gemclus/gemini/__init__.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)    15507 2023-05-12 18:00:55.000000 gemclus-0.1.1/gemclus/gemini/_gemini_losses.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-20 14:36:11.059765 gemclus-0.1.1/gemclus/linear/
+-rw-rw-r--   0 louis     (1000) louis     (1000)      116 2023-03-29 14:26:07.000000 gemclus-0.1.1/gemclus/linear/__init__.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)    12833 2023-05-12 18:00:55.000000 gemclus-0.1.1/gemclus/linear/_linear_geminis.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-20 14:36:11.059765 gemclus-0.1.1/gemclus/mlp/
+-rw-rw-r--   0 louis     (1000) louis     (1000)       89 2023-03-29 14:26:07.000000 gemclus-0.1.1/gemclus/mlp/__init__.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)    11321 2023-05-12 18:00:55.000000 gemclus-0.1.1/gemclus/mlp/_mlp_geminis.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-20 14:36:11.059765 gemclus-0.1.1/gemclus/nonparametric/
+-rw-rw-r--   0 louis     (1000) louis     (1000)      128 2023-05-12 18:00:55.000000 gemclus-0.1.1/gemclus/nonparametric/__init__.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)     8172 2023-05-12 18:00:55.000000 gemclus-0.1.1/gemclus/nonparametric/_categorical_models.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-20 14:36:11.059765 gemclus-0.1.1/gemclus/sparse/
+-rw-rw-r--   0 louis     (1000) louis     (1000)      129 2023-03-29 14:26:07.000000 gemclus-0.1.1/gemclus/sparse/__init__.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)    24307 2023-05-16 10:06:41.000000 gemclus-0.1.1/gemclus/sparse/_base_sparse.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)     5437 2023-05-10 08:55:34.000000 gemclus-0.1.1/gemclus/sparse/_linear_sparse.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)     5988 2023-05-12 18:00:55.000000 gemclus-0.1.1/gemclus/sparse/_mlp_sparse.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)     2422 2023-05-12 18:00:55.000000 gemclus-0.1.1/gemclus/sparse/_prox_grad.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-20 14:36:11.063765 gemclus-0.1.1/gemclus/tests/
+-rw-rw-r--   0 louis     (1000) louis     (1000)        0 2023-03-29 14:26:07.000000 gemclus-0.1.1/gemclus/tests/__init__.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)     2808 2023-05-10 08:55:34.000000 gemclus-0.1.1/gemclus/tests/test_data.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)     4508 2023-05-12 18:00:55.000000 gemclus-0.1.1/gemclus/tests/test_default.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)     3248 2023-05-12 18:00:55.000000 gemclus-0.1.1/gemclus/tests/test_objectives.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)     5708 2023-05-12 18:00:55.000000 gemclus-0.1.1/gemclus/tests/test_path.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-20 14:36:11.059765 gemclus-0.1.1/gemclus.egg-info/
+-rw-rw-r--   0 louis     (1000) louis     (1000)     3471 2023-06-20 14:36:11.000000 gemclus-0.1.1/gemclus.egg-info/PKG-INFO
+-rw-rw-r--   0 louis     (1000) louis     (1000)      909 2023-06-20 14:36:11.000000 gemclus-0.1.1/gemclus.egg-info/SOURCES.txt
+-rw-rw-r--   0 louis     (1000) louis     (1000)        1 2023-06-20 14:36:11.000000 gemclus-0.1.1/gemclus.egg-info/dependency_links.txt
+-rw-rw-r--   0 louis     (1000) louis     (1000)        1 2023-05-12 18:02:26.000000 gemclus-0.1.1/gemclus.egg-info/not-zip-safe
+-rw-rw-r--   0 louis     (1000) louis     (1000)      130 2023-06-20 14:36:11.000000 gemclus-0.1.1/gemclus.egg-info/requires.txt
+-rw-rw-r--   0 louis     (1000) louis     (1000)        8 2023-06-20 14:36:11.000000 gemclus-0.1.1/gemclus.egg-info/top_level.txt
+-rw-rw-r--   0 louis     (1000) louis     (1000)       97 2023-04-27 14:33:43.000000 gemclus-0.1.1/pyproject.toml
+-rw-rw-r--   0 louis     (1000) louis     (1000)       50 2023-05-16 13:16:23.000000 gemclus-0.1.1/requirements.txt
+-rw-rw-r--   0 louis     (1000) louis     (1000)      147 2023-06-20 14:36:11.063765 gemclus-0.1.1/setup.cfg
+-rw-rw-r--   0 louis     (1000) louis     (1000)     2357 2023-06-20 12:28:37.000000 gemclus-0.1.1/setup.py
```

### Comparing `gemclus-0.1.0/PKG-INFO` & `gemclus-0.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemclus
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package for performing discriminative clustering with gemini-trained models
 Home-page: https://github.com/gemini-clustering
 Download-URL: https://github.com/gemini-clustering
 Maintainer: Louis Ohl
 Maintainer-email: louis.ohl@inria.fr
 License: GPLv3
 Classifier: Intended Audience :: Science/Research
@@ -16,47 +16,56 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE
 
 # GEMCLUS - A package for discriminative clustering using GEMINI
 
 The **gemclus**  package provides simple tools to perform discriminative clustering using the generalised mutual
 information (GEMINI).
 The package was written to be a scikit-learn compatible extension.
 
-You can find the complete documentation of the package here: `Link to be announced`
+You can find the complete documentation of the package here: `https://gemini-clustering.github.io/`
 
 ## Installation
 
+### Official package
+
 Use the following instruction for installing the package:
 
 ```commandline
 pip install gemclus
 ```
 
 The library requires a couple scientific package to run:
 
 + NumPy
 + Scipy
 + POT
 + Scikit-learn
 
+### Latest version
+
+You may download the latest version of the package by installing the content of the repo.
+
+```commandline
+git clone https://github.com/gemini-clustering/GemClus
+cd GemClus
+pip install .
+```
+
 ## Reference
 
 If this work helped you, please cite our original NeurIPS work:
 
 ```
 Ohl, L., Mattei, P. A., Bouveyron, C., Harchaoui, W., Leclercq, M., Droit, A., & Precioso, F.
 (2022, October).
@@ -81,8 +90,9 @@
 
 This work has been supported by the French government, through the 3IA Côte d'Azur, Investment in the Future, project
 managed by the National Research Agency (ANR) with the reference number ANR-19-P3IA-0002. We would also like to thank
 the France Canada Research Fund (FFCR) for their contribution to the project. This work was partly supported by
 EU Horizon 2020 project AI4Media, under contract no. 951911.
 
 Also many many thanks to Pierre-Alexandre Mattei, Frederic Precioso and Charles Bouveyron for their contribution
-in the GEMINI project. Thanks as well go to Jhonatan Torres for his insights on the development.
+in the GEMINI project, as well as Mickaël Leclercq and Arnaud Droit. Special thanks go to Jhonatan Torres for his
+insights on the development.
```

### Comparing `gemclus-0.1.0/README.md` & `gemclus-0.1.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,42 @@
 # GEMCLUS - A package for discriminative clustering using GEMINI
 
 The **gemclus**  package provides simple tools to perform discriminative clustering using the generalised mutual
 information (GEMINI).
 The package was written to be a scikit-learn compatible extension.
 
-You can find the complete documentation of the package here: `Link to be announced`
+You can find the complete documentation of the package here: `https://gemini-clustering.github.io/`
 
 ## Installation
 
+### Official package
+
 Use the following instruction for installing the package:
 
 ```commandline
 pip install gemclus
 ```
 
 The library requires a couple scientific package to run:
 
 + NumPy
 + Scipy
 + POT
 + Scikit-learn
 
+### Latest version
+
+You may download the latest version of the package by installing the content of the repo.
+
+```commandline
+git clone https://github.com/gemini-clustering/GemClus
+cd GemClus
+pip install .
+```
+
 ## Reference
 
 If this work helped you, please cite our original NeurIPS work:
 
 ```
 Ohl, L., Mattei, P. A., Bouveyron, C., Harchaoui, W., Leclercq, M., Droit, A., & Precioso, F.
 (2022, October).
@@ -49,8 +61,9 @@
 
 This work has been supported by the French government, through the 3IA Côte d'Azur, Investment in the Future, project
 managed by the National Research Agency (ANR) with the reference number ANR-19-P3IA-0002. We would also like to thank
 the France Canada Research Fund (FFCR) for their contribution to the project. This work was partly supported by
 EU Horizon 2020 project AI4Media, under contract no. 951911.
 
 Also many many thanks to Pierre-Alexandre Mattei, Frederic Precioso and Charles Bouveyron for their contribution
-in the GEMINI project. Thanks as well go to Jhonatan Torres for his insights on the development.
+in the GEMINI project, as well as Mickaël Leclercq and Arnaud Droit. Special thanks go to Jhonatan Torres for his
+insights on the development.
```

### Comparing `gemclus-0.1.0/gemclus/_base_gemini.py` & `gemclus-0.1.1/gemclus/_base_gemini.py`

 * *Files identical despite different names*

### Comparing `gemclus-0.1.0/gemclus/data/synthetic_data.py` & `gemclus-0.1.1/gemclus/data/synthetic_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 @validate_params(
     {
         "n": [Interval(Integral, 1, None, closed="left")],
         "loc": ["array-like"],
         "scale": ["array-like"],
-        "pvals": ["array-like", Iterable[float]],
+        "pvals": ["array-like"],
         "random_state": ["random_state"]
     }
 )
 def draw_gmm(n, loc, scale, pvals, random_state=None) -> Tuple[np.ndarray, np.ndarray]:
     """
     Returns :math:`n` samples drawn from a mixture of Gaussian distributions. The number of components
     is determined by the number of elements in the lists of the parameters.
```

### Comparing `gemclus-0.1.0/gemclus/gemini/_gemini_losses.py` & `gemclus-0.1.1/gemclus/gemini/_gemini_losses.py`

 * *Files identical despite different names*

### Comparing `gemclus-0.1.0/gemclus/linear/_linear_geminis.py` & `gemclus-0.1.1/gemclus/linear/_linear_geminis.py`

 * *Files identical despite different names*

### Comparing `gemclus-0.1.0/gemclus/mlp/_mlp_geminis.py` & `gemclus-0.1.1/gemclus/mlp/_mlp_geminis.py`

 * *Files identical despite different names*

### Comparing `gemclus-0.1.0/gemclus/nonparametric/_categorical_models.py` & `gemclus-0.1.1/gemclus/nonparametric/_categorical_models.py`

 * *Files identical despite different names*

### Comparing `gemclus-0.1.0/gemclus/sparse/_base_sparse.py` & `gemclus-0.1.1/gemclus/sparse/_base_sparse.py`

 * *Files 0% similar despite different names*

```diff
@@ -479,15 +479,15 @@
         Retrieves the indices of features that were selected by the model.
 
         Returns
         -------
         ind: ndarray
             The indices of the selected features.
         """
-        return np.nonzero(np.linalg.norm(self.W_, axis=1, ord=2))
+        return np.nonzero(np.linalg.norm(self.W_, axis=1, ord=2))[0]
 
     def _group_lasso_penalty(self):
         return np.linalg.norm(self.W_, axis=1, ord=2).sum()
 
     def path(self, X, alpha_multiplier=1.05, min_features=2, keep_threshold=0.9, restore_best_weights=True,
              early_stopping_factor=0.99, max_patience=10):
         """
```

### Comparing `gemclus-0.1.0/gemclus/sparse/_linear_sparse.py` & `gemclus-0.1.1/gemclus/sparse/_linear_sparse.py`

 * *Files identical despite different names*

### Comparing `gemclus-0.1.0/gemclus/sparse/_mlp_sparse.py` & `gemclus-0.1.1/gemclus/sparse/_mlp_sparse.py`

 * *Files identical despite different names*

### Comparing `gemclus-0.1.0/gemclus/sparse/_prox_grad.py` & `gemclus-0.1.1/gemclus/sparse/_prox_grad.py`

 * *Files identical despite different names*

### Comparing `gemclus-0.1.0/gemclus/tests/test_data.py` & `gemclus-0.1.1/gemclus/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `gemclus-0.1.0/gemclus/tests/test_default.py` & `gemclus-0.1.1/gemclus/tests/test_default.py`

 * *Files identical despite different names*

### Comparing `gemclus-0.1.0/gemclus/tests/test_objectives.py` & `gemclus-0.1.1/gemclus/tests/test_objectives.py`

 * *Files identical despite different names*

### Comparing `gemclus-0.1.0/gemclus/tests/test_path.py` & `gemclus-0.1.1/gemclus/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `gemclus-0.1.0/gemclus.egg-info/PKG-INFO` & `gemclus-0.1.1/gemclus.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemclus
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package for performing discriminative clustering with gemini-trained models
 Home-page: https://github.com/gemini-clustering
 Download-URL: https://github.com/gemini-clustering
 Maintainer: Louis Ohl
 Maintainer-email: louis.ohl@inria.fr
 License: GPLv3
 Classifier: Intended Audience :: Science/Research
@@ -16,47 +16,56 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE
 
 # GEMCLUS - A package for discriminative clustering using GEMINI
 
 The **gemclus**  package provides simple tools to perform discriminative clustering using the generalised mutual
 information (GEMINI).
 The package was written to be a scikit-learn compatible extension.
 
-You can find the complete documentation of the package here: `Link to be announced`
+You can find the complete documentation of the package here: `https://gemini-clustering.github.io/`
 
 ## Installation
 
+### Official package
+
 Use the following instruction for installing the package:
 
 ```commandline
 pip install gemclus
 ```
 
 The library requires a couple scientific package to run:
 
 + NumPy
 + Scipy
 + POT
 + Scikit-learn
 
+### Latest version
+
+You may download the latest version of the package by installing the content of the repo.
+
+```commandline
+git clone https://github.com/gemini-clustering/GemClus
+cd GemClus
+pip install .
+```
+
 ## Reference
 
 If this work helped you, please cite our original NeurIPS work:
 
 ```
 Ohl, L., Mattei, P. A., Bouveyron, C., Harchaoui, W., Leclercq, M., Droit, A., & Precioso, F.
 (2022, October).
@@ -81,8 +90,9 @@
 
 This work has been supported by the French government, through the 3IA Côte d'Azur, Investment in the Future, project
 managed by the National Research Agency (ANR) with the reference number ANR-19-P3IA-0002. We would also like to thank
 the France Canada Research Fund (FFCR) for their contribution to the project. This work was partly supported by
 EU Horizon 2020 project AI4Media, under contract no. 951911.
 
 Also many many thanks to Pierre-Alexandre Mattei, Frederic Precioso and Charles Bouveyron for their contribution
-in the GEMINI project. Thanks as well go to Jhonatan Torres for his insights on the development.
+in the GEMINI project, as well as Mickaël Leclercq and Arnaud Droit. Special thanks go to Jhonatan Torres for his
+insights on the development.
```

### Comparing `gemclus-0.1.0/gemclus.egg-info/SOURCES.txt` & `gemclus-0.1.1/gemclus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gemclus-0.1.0/setup.py` & `gemclus-0.1.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,17 +33,14 @@
                'Topic :: Scientific/Engineering',
                'Topic :: Scientific/Engineering :: Artificial Intelligence',
                'Topic :: Scientific/Engineering :: Information Analysis',
                'Operating System :: Microsoft :: Windows',
                'Operating System :: POSIX',
                'Operating System :: Unix',
                'Operating System :: MacOS',
-               'Programming Language :: Python :: 3.5',
-               'Programming Language :: Python :: 3.6',
-               'Programming Language :: Python :: 3.7',
                'Programming Language :: Python :: 3.8',
                'Programming Language :: Python :: 3.9',
                'Programming Language :: Python :: 3.10']
 EXTRAS_REQUIRE = {
     'tests': [
         'pytest',
         'pytest-cov'],
```

