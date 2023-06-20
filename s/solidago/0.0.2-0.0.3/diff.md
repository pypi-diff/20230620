# Comparing `tmp/solidago-0.0.2.tar.gz` & `tmp/solidago-0.0.3.tar.gz`

## Comparing `solidago-0.0.2.tar` & `solidago-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,15 @@
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 solidago-0.0.2/src/solidago/__init__.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 solidago-0.0.2/src/solidago/__version__.py
--rw-r--r--   0        0        0     4554 2020-02-02 00:00:00.000000 solidago-0.0.2/src/solidago/optimize.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 solidago-0.0.2/src/solidago/mehestan/__init__.py
--rw-r--r--   0        0        0     3349 2020-02-02 00:00:00.000000 solidago-0.0.2/src/solidago/mehestan/primitives.py
--rw-r--r--   0        0        0     3762 2020-02-02 00:00:00.000000 solidago-0.0.2/tests/test_mehestan_primitives.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 solidago-0.0.2/.gitignore
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 solidago-0.0.2/README.md
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 solidago-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 solidago-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 solidago-0.0.3/src/solidago/__init__.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 solidago-0.0.3/src/solidago/__version__.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 solidago-0.0.3/src/solidago/comparisons_to_scores/__init__.py
+-rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 solidago-0.0.3/src/solidago/comparisons_to_scores/base.py
+-rw-r--r--   0        0        0     5069 2020-02-02 00:00:00.000000 solidago-0.0.3/src/solidago/comparisons_to_scores/continuous_bradley_terry.py
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 solidago-0.0.3/src/solidago/comparisons_to_scores/hooke_individual_scores.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 solidago-0.0.3/src/solidago/resilient_primitives/__init__.py
+-rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 solidago-0.0.3/src/solidago/resilient_primitives/_primitives.py
+-rw-r--r--   0        0        0     4554 2020-02-02 00:00:00.000000 solidago-0.0.3/src/solidago/solvers/optimize.py
+-rw-r--r--   0        0        0     5223 2020-02-02 00:00:00.000000 solidago-0.0.3/tests/test_comparisons_to_scores.py
+-rw-r--r--   0        0        0     3799 2020-02-02 00:00:00.000000 solidago-0.0.3/tests/test_resilient_primitives.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 solidago-0.0.3/.gitignore
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 solidago-0.0.3/README.md
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 solidago-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 solidago-0.0.3/PKG-INFO
```

### Comparing `solidago-0.0.2/src/solidago/optimize.py` & `solidago-0.0.3/src/solidago/solvers/optimize.py`

 * *Files identical despite different names*

### Comparing `solidago-0.0.2/src/solidago/mehestan/primitives.py` & `solidago-0.0.3/src/solidago/resilient_primitives/_primitives.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from typing import Union
 
 import numpy as np
+import numpy.typing as npt
 import pandas as pd
 from numba import njit
 
-from solidago.optimize import brentq
+from solidago.solvers.optimize import brentq
 
 EPSILON = 1e-6  # convergence tolerance
 
 
 @njit
 def L_prime(m: float, W: float, w, x, delta_2):
     x_minus_m = x - m
     return W * m - np.sum(w * x_minus_m / np.sqrt(delta_2 + x_minus_m**2))
 
 
 @njit
-def QrMed_inner(W: float, w: Union[pd.Series, float], x: pd.Series, delta: pd.Series):
+def QrMed_inner(W: float, w: Union[npt.NDArray, float], x: npt.NDArray, delta: npt.NDArray):
     """
     Quadratically regularized median.
     It behaves like a weighted median biased towards 0.
 
     Parameters:
         * `W`: Byzantine resilience parameter.
             The influence of a single contributor 'i' is bounded by (w_i/W)
@@ -38,32 +39,32 @@
     while L_prime(m_up, W, w, x, delta_2) < 0:
         m_up *= 2
 
     # Brent’s method is used as a faster alternative to usual bisection
     return brentq(L_prime, m_low, m_up, args=(W, w, x, delta_2), xtol=EPSILON)
 
 
-def QrMed(W: float, w: Union[pd.Series, float], x: pd.Series, delta: pd.Series):
+def QrMed(W: float, w: Union[npt.ArrayLike, float], x: npt.ArrayLike, delta: npt.ArrayLike):
     if len(x) == 0:
         return 0.0
     if isinstance(w, pd.Series):
         w = w.to_numpy()
     if isinstance(x, pd.Series):
         x = x.to_numpy()
     if isinstance(delta, pd.Series):
         delta = delta.to_numpy()
     return QrMed_inner(W, w, x, delta)
 
 
 def QrDev(
     W: float,
     default_dev: float,
-    w: Union[pd.Series, float],
-    x: pd.Series,
-    delta: pd.Series,
+    w: Union[npt.ArrayLike, float],
+    x: npt.ArrayLike,
+    delta: npt.ArrayLike,
     qr_med=None,
 ):
     """
     Quadratically regularized deviation, between x and their QrMed.
     Can be understood as a measure of polarization.
     It is like a secure version of the median deviation from the median.
     """
@@ -71,17 +72,17 @@
         qr_med = QrMed(W, w, x, delta)
     return default_dev + QrMed(W, w, np.abs(x - qr_med) - default_dev, delta)
 
 
 def QrUnc(
     W: float,
     default_dev: float,
-    w: pd.Series,
-    x: pd.Series,
-    delta: pd.Series,
+    w: npt.ArrayLike,
+    x: npt.ArrayLike,
+    delta: npt.ArrayLike,
     qr_med=None,
 ):
     """
     Quadratically regularized uncertainty
     TODO : search for a better formula for QrUnc if possible
     """
     if isinstance(w, pd.Series):
```

### Comparing `solidago-0.0.2/tests/test_mehestan_primitives.py` & `solidago-0.0.3/tests/test_resilient_primitives.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,119 +1,119 @@
 from unittest import TestCase
 
 import numpy as np
 
-from solidago.mehestan.primitives import QrDev, QrMed, QrUnc
+from solidago.resilient_primitives import QrDev, QrMed, QrUnc
 
 
 class QrMedTest(TestCase):
     def test_qrmed(self):
         W = 2
         weight = 1
         self.assertAlmostEqual(
             QrMed(
                 W,
                 w=weight,
                 x=np.array([-10.0, 1.0, 10.0]),
                 delta=np.array([1e-3, 1e-3, 1e-3]),
             ),
-            0.5, # influence of the median contributor is bounded by weight / W
-            places=3
+            0.5,  # influence of the median contributor is bounded by weight / W
+            places=3,
         )
 
     def test_qrmed_with_W_equals_zero(self):
         """Setting W to 0 is like removing the bias towards 0"""
         W = 0
         weight = 1
         self.assertAlmostEqual(
             QrMed(
                 W,
                 w=weight,
                 x=np.array([-10.0, 1.0, 10.0]),
                 delta=np.array([1e-3, 1e-3, 1e-3]),
             ),
             1.0,
-            places=3
+            places=3,
         )
 
     def test_qrmed_with_high_uncertainty(self):
         """Each score with a high uncertainty will have less effect on QrMed."""
         self.assertAlmostEqual(
             QrMed(
-                W=1.,
-                w=1.,
-                x=np.array([-10., 1., 10.]),
-                delta=1000000.,
+                W=1.0,
+                w=1.0,
+                x=np.array([-10.0, 1.0, 10.0]),
+                delta=1000000.0,
             ),
-            0.,
-            places=5
+            0.0,
+            places=5,
         )
 
 
 class QrDevTest(TestCase):
     def test_qrdev_default(self):
-        default_deviation = 3.
+        default_deviation = 3.0
         self.assertEqual(
             QrDev(
-                W=2.,
+                W=2.0,
                 default_dev=default_deviation,
-                w=1.,
+                w=1.0,
                 x=np.array([]),
                 delta=np.array([]),
             ),
             default_deviation,
         )
 
     def test_qrdev_with_high_weight(self):
-        x = np.array([-6., 0., 15.])
+        x = np.array([-6.0, 0.0, 15.0])
         self.assertAlmostEqual(
             QrDev(
-                W=2.,
-                default_dev=1.,
-                w=100000.,
+                W=2.0,
+                default_dev=1.0,
+                w=100000.0,
                 x=x,
-                delta=0.,
+                delta=0.0,
             ),
             float(np.median(np.abs(x))),  # = 6.
-            places=5
+            places=5,
         )
 
     def test_qrdev_with_W_equals_0(self):
         """Setting W to 0 is like removing the bias towards default_dev"""
-        x = np.array([-6., 0., 15.])
+        x = np.array([-6.0, 0.0, 15.0])
         self.assertAlmostEqual(
             QrDev(
-                W=0.,
-                default_dev=1.,
-                w=1.,
+                W=0.0,
+                default_dev=1.0,
+                w=1.0,
                 x=x,
-                delta=0.,
+                delta=0.0,
             ),
             float(np.median(np.abs(x))),  # = 6.
             places=5,
         )
 
     def test_qrdev_with_high_uncertainty(self):
         """
         Each score with a high uncertainty will have less
         effect on QrMed, and thus also on QrDev, which will
         thus not change much from its default deviation.
         """
         default_deviation = 3
-        x = np.array([-6., 0., 15.])
+        x = np.array([-6.0, 0.0, 15.0])
         self.assertAlmostEqual(
             QrDev(
-                W=2.,
+                W=2.0,
                 default_dev=default_deviation,
-                w=1.,
+                w=1.0,
                 x=x,
-                delta=100000000.,
+                delta=100000000.0,
             ),
             default_deviation,
-            places=5
+            places=5,
         )
 
 
 class QrUncTest(TestCase):
     def test_qrunc(self):
         W = 2
         weight = 1
```

### Comparing `solidago-0.0.2/README.md` & `solidago-0.0.3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ## Usage
 
 > **Warning**  
 > This library is WIP; its API may change in the near future.
 
 ```py
 import numpy as np
-from solidago.mehestan import QrMed
+from solidago.resilient_primitives import QrMed
 
 score = QrMed(W=1, w=1, x=np.array([-1.0, 1.0, 2.0]), delta=np.array([1.0, 1.0, 1.0]))
 ```
 
 ## Publish a new release
 
 1. In a Pull Request, update the version number in [`./src/solidago/__version__.py`](./src/solidago/__version__.py)
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 # Solidago **Solid** **A**lgorithmic **Go**vernance, used by the Tournesol
 platform [Package_version] ## Usage > **Warning** > This library is WIP; its
 API may change in the near future. ```py import numpy as np from
-solidago.mehestan import QrMed score = QrMed(W=1, w=1, x=np.array([-1.0, 1.0,
-2.0]), delta=np.array([1.0, 1.0, 1.0])) ``` ## Publish a new release 1. In a
-Pull Request, update the version number in [`./src/solidago/__version__.py`](./
-src/solidago/__version__.py) 2. The package will be published automatically
-when the new version is merged into "main", by [this Github Action](../.github/
-workflows/solidago-publish.yml).
+solidago.resilient_primitives import QrMed score = QrMed(W=1, w=1, x=np.array(
+[-1.0, 1.0, 2.0]), delta=np.array([1.0, 1.0, 1.0])) ``` ## Publish a new
+release 1. In a Pull Request, update the version number in [`./src/solidago/
+__version__.py`](./src/solidago/__version__.py) 2. The package will be
+published automatically when the new version is merged into "main", by [this
+Github Action](../.github/workflows/solidago-publish.yml).
```

### Comparing `solidago-0.0.2/pyproject.toml` & `solidago-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `solidago-0.0.2/PKG-INFO` & `solidago-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solidago
-Version: 0.0.2
+Version: 0.0.3
 Summary: Algorithms for Secure Algorithmic Governance
 Project-URL: Homepage, https://github.com/tournesol-app/tournesol/tree/main/solidago
 Project-URL: Bug Tracker, https://github.com/tournesol-app/tournesol/issues
 Author-email: Tournesol Association <hello@tournesol.app>
 Keywords: collaborative recommendations,comparison based,judgement aggregation,mehestan,tournesol
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -28,15 +28,15 @@
 ## Usage
 
 > **Warning**  
 > This library is WIP; its API may change in the near future.
 
 ```py
 import numpy as np
-from solidago.mehestan import QrMed
+from solidago.resilient_primitives import QrMed
 
 score = QrMed(W=1, w=1, x=np.array([-1.0, 1.0, 2.0]), delta=np.array([1.0, 1.0, 1.0]))
 ```
 
 ## Publish a new release
 
 1. In a Pull Request, update the version number in [`./src/solidago/__version__.py`](./src/solidago/__version__.py)
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: solidago Version: 0.0.2 Summary: Algorithms for
+Metadata-Version: 2.1 Name: solidago Version: 0.0.3 Summary: Algorithms for
 Secure Algorithmic Governance Project-URL: Homepage, https://github.com/
 tournesol-app/tournesol/tree/main/solidago Project-URL: Bug Tracker, https://
 github.com/tournesol-app/tournesol/issues Author-email: Tournesol Association
 tournesol.app> Keywords: collaborative recommendations,comparison
 based,judgement aggregation,mehestan,tournesol Classifier: License :: OSI
 Approved :: GNU Affero General Public License v3 Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 3 Requires-
 Python: >=3.9 Requires-Dist: numba==0.57.0 Requires-Dist: numpy<1.25,>=1.24.3
 Requires-Dist: pandas<2.0,>=1.5.3 Provides-Extra: test Requires-Dist:
 pytest<8.0.0,>=7.1.3; extra == 'test' Description-Content-Type: text/markdown #
 Solidago **Solid** **A**lgorithmic **Go**vernance, used by the Tournesol
 platform [Package_version] ## Usage > **Warning** > This library is WIP; its
 API may change in the near future. ```py import numpy as np from
-solidago.mehestan import QrMed score = QrMed(W=1, w=1, x=np.array([-1.0, 1.0,
-2.0]), delta=np.array([1.0, 1.0, 1.0])) ``` ## Publish a new release 1. In a
-Pull Request, update the version number in [`./src/solidago/__version__.py`](./
-src/solidago/__version__.py) 2. The package will be published automatically
-when the new version is merged into "main", by [this Github Action](../.github/
-workflows/solidago-publish.yml).
+solidago.resilient_primitives import QrMed score = QrMed(W=1, w=1, x=np.array(
+[-1.0, 1.0, 2.0]), delta=np.array([1.0, 1.0, 1.0])) ``` ## Publish a new
+release 1. In a Pull Request, update the version number in [`./src/solidago/
+__version__.py`](./src/solidago/__version__.py) 2. The package will be
+published automatically when the new version is merged into "main", by [this
+Github Action](../.github/workflows/solidago-publish.yml).
```

