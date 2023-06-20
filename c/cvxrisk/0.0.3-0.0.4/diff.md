# Comparing `tmp/cvxrisk-0.0.3.tar.gz` & `tmp/cvxrisk-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxrisk-0.0.3.tar", max compression
+gzip compressed data, was "cvxrisk-0.0.4.tar", max compression
```

## Comparing `cvxrisk-0.0.3.tar` & `cvxrisk-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,18 @@
--rw-r--r--   0        0        0    11375 2023-06-15 00:11:52.856834 cvxrisk-0.0.3/LICENSE
--rw-r--r--   0        0        0     4832 2023-06-15 00:11:52.856834 cvxrisk-0.0.3/README.md
--rw-r--r--   0        0        0       97 2023-06-15 00:11:52.860834 cvxrisk-0.0.3/cvx/risk/__init__.py
--rw-r--r--   0        0        0       83 2023-06-15 00:11:52.860834 cvxrisk-0.0.3/cvx/risk/cvar/__init__.py
--rw-r--r--   0        0        0      705 2023-06-15 00:11:52.860834 cvxrisk-0.0.3/cvx/risk/cvar/cvar.py
--rw-r--r--   0        0        0      162 2023-06-15 00:11:52.860834 cvxrisk-0.0.3/cvx/risk/factor/__init__.py
--rw-r--r--   0        0        0      755 2023-06-15 00:11:52.860834 cvxrisk-0.0.3/cvx/risk/factor/_model.py
--rw-r--r--   0        0        0      498 2023-06-15 00:11:52.860834 cvxrisk-0.0.3/cvx/risk/factor/fundamental.py
--rw-r--r--   0        0        0        0 2023-06-15 00:11:52.860834 cvxrisk-0.0.3/cvx/risk/factor/linalg/__init__.py
--rw-r--r--   0        0        0      820 2023-06-15 00:11:52.860834 cvxrisk-0.0.3/cvx/risk/factor/linalg/pca.py
--rw-r--r--   0        0        0     1655 2023-06-15 00:11:52.860834 cvxrisk-0.0.3/cvx/risk/factor/timeseries.py
--rw-r--r--   0        0        0      343 2023-06-15 00:11:52.860834 cvxrisk-0.0.3/cvx/risk/model.py
--rw-r--r--   0        0        0      142 2023-06-15 00:11:52.860834 cvxrisk-0.0.3/cvx/risk/sample/__init__.py
--rw-r--r--   0        0        0      914 2023-06-15 00:11:52.860834 cvxrisk-0.0.3/cvx/risk/sample/sample.py
--rw-r--r--   0        0        0      581 2023-06-15 00:12:25.752431 cvxrisk-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     5440 1970-01-01 00:00:00.000000 cvxrisk-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11375 2023-06-20 16:02:07.344632 cvxrisk-0.0.4/LICENSE
+-rw-r--r--   0        0        0     4710 2023-06-20 16:02:07.344632 cvxrisk-0.0.4/README.md
+-rw-r--r--   0        0        0       97 2023-06-20 16:02:07.368631 cvxrisk-0.0.4/cvx/risk/__init__.py
+-rw-r--r--   0        0        0       83 2023-06-20 16:02:07.368631 cvxrisk-0.0.4/cvx/risk/cvar/__init__.py
+-rw-r--r--   0        0        0     1596 2023-06-20 16:02:07.368631 cvxrisk-0.0.4/cvx/risk/cvar/cvar.py
+-rw-r--r--   0        0        0       92 2023-06-20 16:02:07.368631 cvxrisk-0.0.4/cvx/risk/factor/__init__.py
+-rw-r--r--   0        0        0     1995 2023-06-20 16:02:07.368631 cvxrisk-0.0.4/cvx/risk/factor/factor.py
+-rw-r--r--   0        0        0      137 2023-06-20 16:02:07.368631 cvxrisk-0.0.4/cvx/risk/linalg/__init__.py
+-rw-r--r--   0        0        0      252 2023-06-20 16:02:07.368631 cvxrisk-0.0.4/cvx/risk/linalg/cholesky.py
+-rw-r--r--   0        0        0     1301 2023-06-20 16:02:07.368631 cvxrisk-0.0.4/cvx/risk/linalg/pca.py
+-rw-r--r--   0        0        0      512 2023-06-20 16:02:07.368631 cvxrisk-0.0.4/cvx/risk/linalg/valid.py
+-rw-r--r--   0        0        0      492 2023-06-20 16:02:07.368631 cvxrisk-0.0.4/cvx/risk/model.py
+-rw-r--r--   0        0        0       91 2023-06-20 16:02:07.368631 cvxrisk-0.0.4/cvx/risk/random/__init__.py
+-rw-r--r--   0        0        0      159 2023-06-20 16:02:07.368631 cvxrisk-0.0.4/cvx/risk/random/rand_cov.py
+-rw-r--r--   0        0        0       97 2023-06-20 16:02:07.368631 cvxrisk-0.0.4/cvx/risk/sample/__init__.py
+-rw-r--r--   0        0        0     1725 2023-06-20 16:02:07.368631 cvxrisk-0.0.4/cvx/risk/sample/sample.py
+-rw-r--r--   0        0        0      581 2023-06-20 16:02:32.720575 cvxrisk-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     5318 1970-01-01 00:00:00.000000 cvxrisk-0.0.4/PKG-INFO
```

### Comparing `cvxrisk-0.0.3/LICENSE` & `cvxrisk-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxrisk-0.0.3/README.md` & `cvxrisk-0.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # [cvxrisk](http://www.cvxgrp.org/cvxrisk/)
 
 [![PyPI version](https://badge.fury.io/py/cvxrisk.svg)](https://badge.fury.io/py/cvxrisk)
 [![Apache 2.0 License](https://img.shields.io/badge/License-APACHEv2-brightgreen.svg)](https://github.com/cvxgrp/simulator/blob/master/LICENSE)
 [![PyPI download month](https://img.shields.io/pypi/dm/cvxrisk.svg)](https://pypi.python.org/pypi/cvxrisk/)
 
 We provide an abstract `RiskModel` class. The class is designed to be used in conjunction with [cvxpy](https://github.com/cvxpy/cvxpy).
-Using this class, we can formulate a function computing a standard minimum variance portfolio as
+Using this class, we can formulate a function computing a standard minimum risk portfolio as
 
 ```python
 import cvxpy as cp
 
 from cvx.risk import RiskModel
 
-def minimum_variance(w: cp.Variable, risk_model: RiskModel) -> cp.Problem:
+def minimum_risk(w: cp.Variable, risk_model: RiskModel) -> cp.Problem:
     """Constructs a minimum variance portfolio.
 
     Args:
         w: cp.Variable representing the portfolio weights.
         risk_model: A risk model.
 
     Returns:
@@ -40,56 +40,51 @@
 ```python
 import numpy as np
 import cvxpy as cp
 
 from cvx.risk.sample import SampleCovariance
 
 riskmodel = SampleCovariance(num=2)
-riskmodel.cov.value = np.array([[1.0, 0.5], [0.5, 2.0]])
-
 w = cp.Variable(2)
+problem = minimum_risk(w, riskmodel)
 
-minimum_variance(w, riskmodel).solve()
+riskmodel.update_data(cov=np.array([[1.0, 0.5], [0.5, 2.0]]))
+problem.solve()
 print(w.value)
 ```
 
 The risk model and the actual optimization problem are decoupled.
 This is good practice and keeps the code clean and maintainable.
 
+In a backtest we don't have to reconstruct the problem in every iteration.
+We can simply update the risk model with the new data and solve the problem again.
+If the dimension of the problem is changing during the test we expect
+a new problem has to be constructed though.
+
 ## Risk models
 
 ### Sample covariance
 
-We offer two variants of the sample covariance risk model.
-The first variant is the `SampleCovariance` class.
-It relies on cxxpy's `quad_form` function to compute the variance
-```math
-w^T \Sigma w.
-```
-The second variant is the `SampleCovariance_product` class.
-It relies on cxxpy's `sum_of_squares` function to compute the variance using
-```math
-\| \Sigma^{1/2} w \|_2.
-```
+We offer a `SampleCovariance` class as seen above.
 
 
 ### Factor risk models
 
 Factor risk models use the projection of the weight vector into a lower
 dimensional subspace, e.g. each asset is the linear combination of $k$ factors.
 ```math
 r_i = \sum_{j=1}^k f_j \beta_{ji} + \epsilon_i
 ```
-The factor time series are $f_1, \ldots, f_k$. The loadings are the coefficients $\beta_{ji}$.
+The factor time series are $f_1, \ldots, f_k$. The loadings are the coefficients
+$\beta_{ji}$.
 The residual returns $\epsilon_i$ are assumed to be uncorrelated with the factors.
 
 Any position $w$ in weight space projects to a position $y = \beta w$ in factor space.
-Factor space has only $k$ dimensions, whereas weight space has $n$ dimensions.
 The variance for a position $w$ is the sum of the variance of the
-systemic returns explained by the factors and the variance by the idiosyncratic returns.
+systematic returns explained by the factors and the variance of the idiosyncratic returns.
 
 ```math
 Var(r) = Var(\beta w) + Var(\epsilon w)
 ```
 
 We assume the residual returns are uncorrelated and hence
 
@@ -100,15 +95,15 @@
 where $\Sigma_f$ is the covariance matrix of the factors and $Var(\epsilon_i)$
 is the variance of the idiosyncratic returns.
 
 Again we offer two variants of the factor risk model reflecting what is widely used in practice.
 The first variant is the `FundamentalFactorRiskModel` class.
 Here the user provides the factor covariance matrix $\Sigma_f$,
 the loadings $\beta$ and the volatilities of the idiosyncratic returns $\epsilon_i$. Often such
-data is provided by the external parties, e.g. Barra or Axioma.
+data is provided by external parties, e.g. Barra or Axioma.
 
 The second variant is the `TimeseriesFactorRiskModel` class.
 Here the user provides the factor time series $f_1, \ldots, f_k$, usually obtained from
 a principal component analysis (PCA) of the asset returns. The loadings $\beta$ are computed
 via a linear regression of the asset returns on the factor time series.
 The volatilities of the idiosyncratic returns $\epsilon_i$ are computed as the standard deviation
 of the residuals of the linear regression.
```

### Comparing `cvxrisk-0.0.3/pyproject.toml` & `cvxrisk-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cvxrisk"
-version = "v0.0.3"
+version = "v0.0.4"
 description = "Simple riskengine for cvxpy"
 authors = ["Thomas Schmelzer"]
 readme = "README.md"
 repository = "https://github.com/cvxgrp/cvxrisk"
 packages = [{include = "cvx"}]
 
 [tool.poetry.dependencies]
```

### Comparing `cvxrisk-0.0.3/PKG-INFO` & `cvxrisk-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxrisk
-Version: 0.0.3
+Version: 0.0.4
 Summary: Simple riskengine for cvxpy
 Home-page: https://github.com/cvxgrp/cvxrisk
 Author: Thomas Schmelzer
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -19,22 +19,22 @@
 # [cvxrisk](http://www.cvxgrp.org/cvxrisk/)
 
 [![PyPI version](https://badge.fury.io/py/cvxrisk.svg)](https://badge.fury.io/py/cvxrisk)
 [![Apache 2.0 License](https://img.shields.io/badge/License-APACHEv2-brightgreen.svg)](https://github.com/cvxgrp/simulator/blob/master/LICENSE)
 [![PyPI download month](https://img.shields.io/pypi/dm/cvxrisk.svg)](https://pypi.python.org/pypi/cvxrisk/)
 
 We provide an abstract `RiskModel` class. The class is designed to be used in conjunction with [cvxpy](https://github.com/cvxpy/cvxpy).
-Using this class, we can formulate a function computing a standard minimum variance portfolio as
+Using this class, we can formulate a function computing a standard minimum risk portfolio as
 
 ```python
 import cvxpy as cp
 
 from cvx.risk import RiskModel
 
-def minimum_variance(w: cp.Variable, risk_model: RiskModel) -> cp.Problem:
+def minimum_risk(w: cp.Variable, risk_model: RiskModel) -> cp.Problem:
     """Constructs a minimum variance portfolio.
 
     Args:
         w: cp.Variable representing the portfolio weights.
         risk_model: A risk model.
 
     Returns:
@@ -58,56 +58,51 @@
 ```python
 import numpy as np
 import cvxpy as cp
 
 from cvx.risk.sample import SampleCovariance
 
 riskmodel = SampleCovariance(num=2)
-riskmodel.cov.value = np.array([[1.0, 0.5], [0.5, 2.0]])
-
 w = cp.Variable(2)
+problem = minimum_risk(w, riskmodel)
 
-minimum_variance(w, riskmodel).solve()
+riskmodel.update_data(cov=np.array([[1.0, 0.5], [0.5, 2.0]]))
+problem.solve()
 print(w.value)
 ```
 
 The risk model and the actual optimization problem are decoupled.
 This is good practice and keeps the code clean and maintainable.
 
+In a backtest we don't have to reconstruct the problem in every iteration.
+We can simply update the risk model with the new data and solve the problem again.
+If the dimension of the problem is changing during the test we expect
+a new problem has to be constructed though.
+
 ## Risk models
 
 ### Sample covariance
 
-We offer two variants of the sample covariance risk model.
-The first variant is the `SampleCovariance` class.
-It relies on cxxpy's `quad_form` function to compute the variance
-```math
-w^T \Sigma w.
-```
-The second variant is the `SampleCovariance_product` class.
-It relies on cxxpy's `sum_of_squares` function to compute the variance using
-```math
-\| \Sigma^{1/2} w \|_2.
-```
+We offer a `SampleCovariance` class as seen above.
 
 
 ### Factor risk models
 
 Factor risk models use the projection of the weight vector into a lower
 dimensional subspace, e.g. each asset is the linear combination of $k$ factors.
 ```math
 r_i = \sum_{j=1}^k f_j \beta_{ji} + \epsilon_i
 ```
-The factor time series are $f_1, \ldots, f_k$. The loadings are the coefficients $\beta_{ji}$.
+The factor time series are $f_1, \ldots, f_k$. The loadings are the coefficients
+$\beta_{ji}$.
 The residual returns $\epsilon_i$ are assumed to be uncorrelated with the factors.
 
 Any position $w$ in weight space projects to a position $y = \beta w$ in factor space.
-Factor space has only $k$ dimensions, whereas weight space has $n$ dimensions.
 The variance for a position $w$ is the sum of the variance of the
-systemic returns explained by the factors and the variance by the idiosyncratic returns.
+systematic returns explained by the factors and the variance of the idiosyncratic returns.
 
 ```math
 Var(r) = Var(\beta w) + Var(\epsilon w)
 ```
 
 We assume the residual returns are uncorrelated and hence
 
@@ -118,15 +113,15 @@
 where $\Sigma_f$ is the covariance matrix of the factors and $Var(\epsilon_i)$
 is the variance of the idiosyncratic returns.
 
 Again we offer two variants of the factor risk model reflecting what is widely used in practice.
 The first variant is the `FundamentalFactorRiskModel` class.
 Here the user provides the factor covariance matrix $\Sigma_f$,
 the loadings $\beta$ and the volatilities of the idiosyncratic returns $\epsilon_i$. Often such
-data is provided by the external parties, e.g. Barra or Axioma.
+data is provided by external parties, e.g. Barra or Axioma.
 
 The second variant is the `TimeseriesFactorRiskModel` class.
 Here the user provides the factor time series $f_1, \ldots, f_k$, usually obtained from
 a principal component analysis (PCA) of the asset returns. The loadings $\beta$ are computed
 via a linear regression of the asset returns on the factor time series.
 The volatilities of the idiosyncratic returns $\epsilon_i$ are computed as the standard deviation
 of the residuals of the linear regression.
```

