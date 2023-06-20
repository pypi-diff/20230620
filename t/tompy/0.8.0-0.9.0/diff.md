# Comparing `tmp/tompy-0.8.0.tar.gz` & `tmp/tompy-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tompy-0.8.0.tar", max compression
+gzip compressed data, was "tompy-0.9.0.tar", max compression
```

## Comparing `tompy-0.8.0.tar` & `tompy-0.9.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1060 2022-08-12 04:01:30.882686 tompy-0.8.0/LICENSE
--rw-r--r--   0        0        0     1009 2022-08-13 06:34:36.128015 tompy-0.8.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-08-12 10:40:45.560979 tompy-0.8.0/tompy/__init__.py
--rw-r--r--   0        0        0     2709 2022-08-12 10:40:45.560979 tompy-0.8.0/tompy/data.py
--rw-r--r--   0        0        0     9221 2022-08-12 10:40:45.560979 tompy-0.8.0/tompy/dataframe.py
--rw-r--r--   0        0        0     1763 2022-08-12 10:40:45.560979 tompy-0.8.0/tompy/datetime.py
--rw-r--r--   0        0        0     2265 2022-08-12 10:40:45.560979 tompy-0.8.0/tompy/decimal.py
--rw-r--r--   0        0        0    11854 2022-08-12 10:40:45.560979 tompy-0.8.0/tompy/matrix.py
--rw-r--r--   0        0        0     3121 2022-08-12 10:40:45.560979 tompy-0.8.0/tompy/portfolio.py
--rw-r--r--   0        0        0        0 2022-08-12 10:40:45.560979 tompy-0.8.0/tompy/py.typed
--rw-r--r--   0        0        0      775 2022-08-12 10:40:45.560979 tompy-0.8.0/tompy/scalar.py
--rw-r--r--   0        0        0     6069 2022-08-12 10:40:45.560979 tompy-0.8.0/tompy/series.py
--rw-r--r--   0        0        0      168 2022-08-12 10:40:45.560979 tompy-0.8.0/tompy/settings.py
--rw-r--r--   0        0        0    15781 2022-08-12 10:40:45.560979 tompy-0.8.0/tompy/vector.py
--rw-r--r--   0        0        0      818 2022-08-13 06:35:10.568301 tompy-0.8.0/setup.py
--rw-r--r--   0        0        0      617 2022-08-13 06:35:10.568536 tompy-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1060 2022-08-12 04:01:30.882686 tompy-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1009 2022-08-15 11:00:43.892399 tompy-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-08-12 10:40:45.560979 tompy-0.9.0/tompy/__init__.py
+-rw-r--r--   0        0        0     2709 2022-08-12 10:40:45.560979 tompy-0.9.0/tompy/data.py
+-rw-r--r--   0        0        0     9221 2022-08-12 10:40:45.560979 tompy-0.9.0/tompy/dataframe.py
+-rw-r--r--   0        0        0     1763 2022-08-12 10:40:45.560979 tompy-0.9.0/tompy/datetime.py
+-rw-r--r--   0        0        0     2170 2022-08-15 11:00:43.892399 tompy-0.9.0/tompy/decimal.py
+-rw-r--r--   0        0        0    11854 2022-08-12 10:40:45.560979 tompy-0.9.0/tompy/matrix.py
+-rw-r--r--   0        0        0     3121 2022-08-12 10:40:45.560979 tompy-0.9.0/tompy/portfolio.py
+-rw-r--r--   0        0        0        0 2022-08-12 10:40:45.560979 tompy-0.9.0/tompy/py.typed
+-rw-r--r--   0        0        0      775 2022-08-12 10:40:45.560979 tompy-0.9.0/tompy/scalar.py
+-rw-r--r--   0        0        0     6069 2022-08-12 10:40:45.560979 tompy-0.9.0/tompy/series.py
+-rw-r--r--   0        0        0      168 2022-08-12 10:40:45.560979 tompy-0.9.0/tompy/settings.py
+-rw-r--r--   0        0        0    15781 2022-08-12 10:40:45.560979 tompy-0.9.0/tompy/vector.py
+-rw-r--r--   0        0        0      818 2022-08-15 11:01:08.968227 tompy-0.9.0/setup.py
+-rw-r--r--   0        0        0      617 2022-08-15 11:01:08.968415 tompy-0.9.0/PKG-INFO
```

### Comparing `tompy-0.8.0/LICENSE` & `tompy-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tompy-0.8.0/pyproject.toml` & `tompy-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tompy"
-version = "0.8.0"
+version = "0.9.0"
 description = "Python Time Series Library"
 authors = ["Tom <nanticj@users.noreply.github.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
 Bottleneck = "^1.3.5"
 finance-datareader = "^0.9.34"
```

### Comparing `tompy-0.8.0/tompy/data.py` & `tompy-0.9.0/tompy/data.py`

 * *Files identical despite different names*

### Comparing `tompy-0.8.0/tompy/dataframe.py` & `tompy-0.9.0/tompy/dataframe.py`

 * *Files identical despite different names*

### Comparing `tompy-0.8.0/tompy/datetime.py` & `tompy-0.9.0/tompy/datetime.py`

 * *Files identical despite different names*

### Comparing `tompy-0.8.0/tompy/decimal.py` & `tompy-0.9.0/tompy/decimal.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,20 +74,16 @@
     /,
     price: Decimal,
     *,
     cash_leverage: Decimal,
     contract_unit: Decimal,
     qtyunit: Decimal,
     risk_point: Decimal,
-    risk_multiplier: Decimal,
     risk_target: Decimal,
 ) -> Decimal:
     return qty_unit(
         min(
             div(cash * cash_leverage, price * contract_unit),
-            div(
-                cash * risk_target,
-                risk_point * risk_multiplier * contract_unit,
-            ),
+            div(cash * risk_target, risk_point * contract_unit),
         ),
         qtyunit,
     )
```

### Comparing `tompy-0.8.0/tompy/matrix.py` & `tompy-0.9.0/tompy/matrix.py`

 * *Files identical despite different names*

### Comparing `tompy-0.8.0/tompy/portfolio.py` & `tompy-0.9.0/tompy/portfolio.py`

 * *Files identical despite different names*

### Comparing `tompy-0.8.0/tompy/scalar.py` & `tompy-0.9.0/tompy/scalar.py`

 * *Files identical despite different names*

### Comparing `tompy-0.8.0/tompy/series.py` & `tompy-0.9.0/tompy/series.py`

 * *Files identical despite different names*

### Comparing `tompy-0.8.0/tompy/vector.py` & `tompy-0.9.0/tompy/vector.py`

 * *Files identical despite different names*

### Comparing `tompy-0.8.0/setup.py` & `tompy-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'pydantic>=1.9.2,<2.0.0',
  'python-dotenv>=0.20.0,<0.21.0',
  'pytz>=2022.2.1,<2023.0.0',
  'scipy>=1.9.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'tompy',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'Python Time Series Library',
     'long_description': None,
     'author': 'Tom',
     'author_email': 'nanticj@users.noreply.github.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `tompy-0.8.0/PKG-INFO` & `tompy-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tompy
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python Time Series Library
 Author: Tom
 Author-email: nanticj@users.noreply.github.com
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: Bottleneck (>=1.3.5,<2.0.0)
```

