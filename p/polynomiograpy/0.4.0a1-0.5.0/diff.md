# Comparing `tmp/polynomiograpy-0.4.0a1.tar.gz` & `tmp/polynomiograpy-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polynomiograpy-0.4.0a1.tar", max compression
+gzip compressed data, was "polynomiograpy-0.5.0.tar", max compression
```

## Comparing `polynomiograpy-0.4.0a1.tar` & `polynomiograpy-0.5.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1070 2023-05-02 09:33:04.682513 polynomiograpy-0.4.0a1/LICENSE
--rw-r--r--   0        0        0       68 2023-05-02 09:33:04.683048 polynomiograpy-0.4.0a1/README.md
--rw-r--r--   0        0        0      533 2023-05-15 10:04:57.052043 polynomiograpy-0.4.0a1/polynomiograpy/__init__.py
--rw-r--r--   0        0        0     5528 2023-05-15 10:03:47.370593 polynomiograpy-0.4.0a1/polynomiograpy/cli/__init__.py
--rw-r--r--   0        0        0      970 2023-05-02 09:33:04.686106 polynomiograpy-0.4.0a1/polynomiograpy/common/finite_field.py
--rw-r--r--   0        0        0     1458 2023-05-08 09:49:29.117520 polynomiograpy-0.4.0a1/polynomiograpy/common/polynomial.py
--rw-r--r--   0        0        0     3071 2023-05-09 10:59:36.896531 polynomiograpy-0.4.0a1/polynomiograpy/iterations/__init__.py
--rw-r--r--   0        0        0     1266 2023-05-08 09:31:50.010724 polynomiograpy-0.4.0a1/polynomiograpy/iterations/helpers.py
--rw-r--r--   0        0        0     5757 2023-05-09 14:28:28.887254 polynomiograpy-0.4.0a1/polynomiograpy/iterations/methods.py
--rw-r--r--   0        0        0     2186 2023-05-09 11:22:48.376339 polynomiograpy-0.4.0a1/polynomiograpy/roots/__init__.py
--rw-r--r--   0        0        0     2001 2023-05-09 10:22:56.186800 polynomiograpy-0.4.0a1/polynomiograpy/roots/helpers.py
--rw-r--r--   0        0        0      737 2023-05-15 10:04:27.096137 polynomiograpy-0.4.0a1/pyproject.toml
--rw-r--r--   0        0        0      838 1970-01-01 00:00:00.000000 polynomiograpy-0.4.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-02 09:33:04.682513 polynomiograpy-0.5.0/LICENSE
+-rw-r--r--   0        0        0       68 2023-05-02 09:33:04.683048 polynomiograpy-0.5.0/README.md
+-rw-r--r--   0        0        0      530 2023-06-20 16:21:03.986053 polynomiograpy-0.5.0/polynomiograpy/__init__.py
+-rw-r--r--   0        0        0     7886 2023-06-18 22:23:59.389571 polynomiograpy-0.5.0/polynomiograpy/cli/__init__.py
+-rw-r--r--   0        0        0      125 2023-06-18 12:24:50.513682 polynomiograpy-0.5.0/polynomiograpy/common/__init__.py
+-rw-r--r--   0        0        0     2056 2023-06-18 11:13:24.685103 polynomiograpy-0.5.0/polynomiograpy/common/finite_field.py
+-rw-r--r--   0        0        0     3148 2023-06-18 11:15:31.522560 polynomiograpy-0.5.0/polynomiograpy/common/polynomial.py
+-rw-r--r--   0        0        0     8686 2023-06-18 23:06:19.952775 polynomiograpy-0.5.0/polynomiograpy/iterations/__init__.py
+-rw-r--r--   0        0        0    10917 2023-06-18 23:10:50.442430 polynomiograpy-0.5.0/polynomiograpy/iterations/helpers.py
+-rw-r--r--   0        0        0    12991 2023-06-19 11:29:20.132385 polynomiograpy-0.5.0/polynomiograpy/iterations/methods.py
+-rw-r--r--   0        0        0     6462 2023-06-18 11:31:27.746230 polynomiograpy-0.5.0/polynomiograpy/roots/__init__.py
+-rw-r--r--   0        0        0     5911 2023-06-18 12:58:11.933688 polynomiograpy-0.5.0/polynomiograpy/roots/helpers.py
+-rw-r--r--   0        0        0      891 2023-06-20 16:20:53.737609 polynomiograpy-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 polynomiograpy-0.5.0/PKG-INFO
```

### Comparing `polynomiograpy-0.4.0a1/LICENSE` & `polynomiograpy-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `polynomiograpy-0.4.0a1/polynomiograpy/__init__.py` & `polynomiograpy-0.5.0/polynomiograpy/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from polynomiograpy.common.finite_field import FiniteField
 from polynomiograpy.iterations import compute_screen_for_single_poly
 from polynomiograpy.roots import (
     compute_screen_for_finite_field_poly,
     compute_screen_for_finite_field_poly_multi_color,
 )
 
-__version__ = "0.4.0.a1"
+__version__ = "0.5.0"
 
 __all__ = [
     "compute_screen_for_single_poly",
     "compute_screen_for_finite_field_poly",
     "compute_screen_for_finite_field_poly_multi_color",
     "FiniteField",
     "Polynomial",
```

### Comparing `polynomiograpy-0.4.0a1/polynomiograpy/common/finite_field.py` & `polynomiograpy-0.5.0/polynomiograpy/common/finite_field.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,54 @@
 import numpy as np
 
 __all__ = ["FiniteField"]
 
 
 class FiniteField:
+    """
+    Represents a finite field and provides methods for generating polynomials over the
+    field.
+    """
+
     def __init__(self, elements):
+        """
+        Initialize the finite field with the specified elements.
+
+        Args:
+            elements (List[int]): The elements of the finite field.
+        """
         self.elements = elements
 
     def generate_polynomials(self, degree) -> list[np.polynomial.Polynomial]:
+        """
+        Generates polynomials of the specified degree over the finite field.
+
+        Args:
+            degree (int): The degree of the polynomials to generate.
+
+        Returns:
+            List[poly.Polynomial]: A list of polynomials over the finite field.
+        """
         polynomials = []
         coefs = self._generate_coeffs(degree, False)
         for coef in coefs:
             polynomials.append(np.polynomial.Polynomial(coef=coef))
         return polynomials
 
     def _generate_coeffs(self, degree, allow_zero):
+        """
+        Generates the coefficients for polynomials of the specified degree.
+
+        Args:
+            degree (int): The degree of the polynomials.
+            allow_zero (bool): Flag indicating whether to allow zero coefficients.
+
+        Returns:
+            List[List[int]]: A list of coefficient lists for the polynomials.
+        """
         leading_coeffs = (
             self.elements
             if allow_zero
             else list(filter(lambda x: x != 0, self.elements))
         )
         res = []
         for leading_coef in leading_coeffs:
@@ -26,8 +56,14 @@
                 res.append([leading_coef])
             else:
                 for coefs in self._generate_coeffs(degree - 1, True):
                     res.append([*coefs, leading_coef])
         return res
 
     def __str__(self):
+        """
+        Returns a string representation of the finite field.
+
+        Returns:
+            str: A string representation of the finite field.
+        """
         return str(self.elements)
```

### Comparing `polynomiograpy-0.4.0a1/pyproject.toml` & `polynomiograpy-0.5.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "polynomiograpy"
-version = "0.4.0.a1"
+version = "0.5.0"
 description = ""
 authors = ["İsmail Tapan <ismltpn@gmail.com>"]
 maintainers = ["İsmail Tapan <ismltpn@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = ""
 repository = "https://github.com/ismltpn/polynomiograpy/"
@@ -15,22 +15,28 @@
     "Visual Art"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 numpy = "^1.24.2"
 pillow = "^9.4.0"
+dearpygui = {version = "^1.9.1", extras = ["gui"]}
 
 [tool.poetry.dev-dependencies]
 black = "^23.1.0"
 isort = "^5.12.0"
 flake8 = "^6.0.0"
 
 [tool.poetry.scripts]
 polynomiograpy_cli = 'polynomiograpy.cli:run'
+polynomiograpy_gui = 'gui:run'
+
+[tool.poetry.group.dev.dependencies]
+sphinx = "^7.0.1"
+rst2pdf = "^0.100"
 
 [tool.isort]
 profile = "black"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `polynomiograpy-0.4.0a1/PKG-INFO` & `polynomiograpy-0.5.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: polynomiograpy
-Version: 0.4.0a1
+Version: 0.5.0
 Summary: 
 Home-page: https://github.com/ismltpn/polynomiograpy/
 License: MIT
 Keywords: Polynomiography,Polynomials,Visual Art
 Author: İsmail Tapan
 Author-email: ismltpn@gmail.com
 Maintainer: İsmail Tapan
 Maintainer-email: ismltpn@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: dearpygui[gui] (>=1.9.1,<2.0.0)
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Requires-Dist: pillow (>=9.4.0,<10.0.0)
 Project-URL: Repository, https://github.com/ismltpn/polynomiograpy/
 Description-Content-Type: text/markdown
 
 # PolynomiograPy
```

