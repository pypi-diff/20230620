# Comparing `tmp/invest_tools-0.2.4.tar.gz` & `tmp/invest_tools-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invest_tools-0.2.4.tar", max compression
+gzip compressed data, was "invest_tools-0.2.5.tar", max compression
```

## Comparing `invest_tools-0.2.4.tar` & `invest_tools-0.2.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1068 2023-03-03 15:06:53.895003 invest_tools-0.2.4/LICENSE
--rw-r--r--   0        0        0     2696 2023-03-03 15:06:53.895003 invest_tools-0.2.4/README.md
--rw-r--r--   0        0        0      106 2023-03-03 15:06:53.895003 invest_tools-0.2.4/invest_tools/__init__.py
--rw-r--r--   0        0        0     1155 2023-03-03 15:06:53.895003 invest_tools-0.2.4/invest_tools/analysis.py
--rw-r--r--   0        0        0      198 2023-03-03 15:06:53.895003 invest_tools-0.2.4/invest_tools/currency.py
--rw-r--r--   0        0        0      572 2023-03-03 15:06:53.895003 invest_tools-0.2.4/invest_tools/log.py
--rw-r--r--   0        0        0      911 2023-03-03 15:06:53.899003 invest_tools-0.2.4/invest_tools/plot.py
--rw-r--r--   0        0        0     8574 2023-03-03 15:06:53.899003 invest_tools-0.2.4/invest_tools/portfolio.py
--rw-r--r--   0        0        0     1887 2023-03-03 15:06:53.899003 invest_tools-0.2.4/invest_tools/validation.py
--rw-r--r--   0        0        0      682 2023-03-03 15:06:53.899003 invest_tools-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     3564 1970-01-01 00:00:00.000000 invest_tools-0.2.4/setup.py
--rw-r--r--   0        0        0     3384 1970-01-01 00:00:00.000000 invest_tools-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-20 16:13:34.001514 invest_tools-0.2.5/LICENSE
+-rw-r--r--   0        0        0     2748 2023-06-20 16:13:34.001514 invest_tools-0.2.5/README.md
+-rw-r--r--   0        0        0      106 2023-06-20 16:13:34.001514 invest_tools-0.2.5/invest_tools/__init__.py
+-rw-r--r--   0        0        0     1155 2023-06-20 16:13:34.001514 invest_tools-0.2.5/invest_tools/analysis.py
+-rw-r--r--   0        0        0      198 2023-06-20 16:13:34.001514 invest_tools-0.2.5/invest_tools/currency.py
+-rw-r--r--   0        0        0      572 2023-06-20 16:13:34.001514 invest_tools-0.2.5/invest_tools/log.py
+-rw-r--r--   0        0        0     1102 2023-06-20 16:13:34.001514 invest_tools-0.2.5/invest_tools/plot.py
+-rw-r--r--   0        0        0    10736 2023-06-20 16:13:34.001514 invest_tools-0.2.5/invest_tools/portfolio.py
+-rw-r--r--   0        0        0     1887 2023-06-20 16:13:34.001514 invest_tools-0.2.5/invest_tools/validation.py
+-rw-r--r--   0        0        0      682 2023-06-20 16:13:34.001514 invest_tools-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     3614 1970-01-01 00:00:00.000000 invest_tools-0.2.5/setup.py
+-rw-r--r--   0        0        0     3436 1970-01-01 00:00:00.000000 invest_tools-0.2.5/PKG-INFO
```

### Comparing `invest_tools-0.2.4/LICENSE` & `invest_tools-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `invest_tools-0.2.4/README.md` & `invest_tools-0.2.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -36,18 +36,14 @@
 
 2. Currency data as a CSV
 
 | Date | Open | High | Low | Close | Adj Close | Volume |
 |------|------|------|-----|-------|-----------|--------|
 | 01/01/2023 | 1 | 1 | 1 | 1 | 1 | 1 |
 
-3. Fama French Data as a CSV
-
-This can be found [here](https://mba.tuck.dartmouth.edu/pages/faculty/ken.french/data_library.html)
-
 ## Example
 
 Build a portfolio of two securities called `EG` and `EG2` with the weighting split 50:50 between the two. One is denominated in GBP and one in USD.
 
 This will output the mean returns of such a portfolio.
 
 ```python
@@ -75,23 +71,25 @@
 port.plot_returns_data()
 ```
 
 ## Roadmap
 
 - [x] Add an input validator
 - [x] Add logging
+- [ ] Update risk free calculation to use new data outputs
 - [ ] Add deeper analysis methods
     - [ ] Coppock Curve
     - [ ] Fama French
     - [ ] Excess Returns
     - [ ] Maximum Drawdown
     - [ ] Calculate Moments
 - [ ] Add further testing
 - [ ] Make the package more generic
 - [ ] Investigate using [Polars](https://www.pola.rs/)
+- [ ] Add func to calculate number of shares to buy to achieve portfolio make up (need to take in cash total for portfolio)
 
 ## License
 
 [MIT](LICENSE)
 
 ## Contact
```

### Comparing `invest_tools-0.2.4/invest_tools/analysis.py` & `invest_tools-0.2.5/invest_tools/analysis.py`

 * *Files identical despite different names*

### Comparing `invest_tools-0.2.4/invest_tools/log.py` & `invest_tools-0.2.5/invest_tools/log.py`

 * *Files identical despite different names*

### Comparing `invest_tools-0.2.4/invest_tools/portfolio.py` & `invest_tools-0.2.5/invest_tools/portfolio.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,14 +12,24 @@
     "High": float,
     "Low": float,
     "Close": float,
     "Volume": float,
     "Adjustment": float,
 }
 
+BENCHMARK_DATATYPES = {
+    "Date": "string",
+    "Open": float,
+    "High": float,
+    "Low": float,
+    "Close": float,
+    "Volume": float,
+    "Adjustment": float,
+}
+
 CURRENCY_DATATYPES = {
     "Date": "string",
     "Open": float,
     "High": float,
     "Low": float,
     "Close": float,
     "Adj Close": float,
@@ -67,14 +77,15 @@
         validation.validate_portfolio_definition(portfolio_definition)
         logger.info("validated portfolio definition")
         self.portfolio_definition = portfolio_definition
         self.backtest = pd.DataFrame()
         self.prices = pd.DataFrame()
         self.gbpusd = pd.DataFrame()
         self.usdgbp = pd.DataFrame()
+        self.benchmark = pd.DataFrame()
         self.currency = currency
         self.clean_returns = pd.Series(dtype=float)
         self.percentage_returns = pd.Series(dtype=float)
         self.analysis = {}
 
     def ping(self):
         logger.info("PING")
@@ -133,14 +144,41 @@
         valid = validation.validate_columns(df, PRICES_DATATYPES.keys())
         valid = validation.validate_datatypes(df, PRICES_DATATYPES)
         logger.debug(f"passed validation: {valid}")
         df["Date"] = pd.to_datetime(df["Date"], format="%d/%m/%Y")
         self.prices = df
         return df
 
+    def get_benchmark(self, benchmark_csv: str) -> pd.Series:
+        """
+        Take in a string pointing to a csv file containing an appropriate benchmark
+
+        The CSV should be in the following format:
+
+        | Date | Open | High | Low | Close | Volume | Adjustment |
+        |------|------|------|-----|-------|--------|------------|
+
+        The Date column should be in the format of "%d/%m/%Y".
+
+        :returns: Pandas dataframe of the portfolio benchmark
+        :rtype: pd.DataFrame
+        """
+        logger.info(f"Loading data from {benchmark_csv}")
+        df = pd.read_csv(benchmark_csv)
+        valid = validation.validate_columns(df, BENCHMARK_DATATYPES.keys())
+        valid = validation.validate_datatypes(df, BENCHMARK_DATATYPES)
+        logger.debug(f"passed validation: {valid}")
+        df["Date"] = pd.to_datetime(df["Date"], format="%d/%m/%Y")
+        df["returns"] = (df.Close / 100).pct_change()
+        df["benchmark_returns"] = df.returns.dropna()
+        df = df.set_index("Date")
+        df = df[["benchmark_returns"]]
+        self.backtest = self.backtest.join(df)
+        return df
+
     # TODO make this generic for currency
     def get_usd_converter(self, conversion_csv: str) -> pd.DataFrame:
         """
         Get a dataframe of USD to GBP to convert the prices between currencies.
         All portfolio prices and returns should be in GBP.
 
         The CSV should be in the following format:
@@ -217,19 +255,38 @@
 
         self.analysis = analysis_results
         self.percentage_returns = percentage_returns
 
         logger.info("Analysis loaded")
         return analysis_results
 
-    def plot_correlation_heatmap(self) -> None:
+    def benchmark_analysis(self) -> pd.DataFrame:
+        cumulative_returns = self.backtest[["portfolio_returns", "benchmark_returns"]]
+        cumulative_returns = cumulative_returns.assign(
+            excess_returns=cumulative_returns.portfolio_returns
+            - cumulative_returns.benchmark_returns
+        )
+        cumulative_returns = (
+            1 + cumulative_returns[["portfolio_returns", "excess_returns"]]
+        ).cumprod() - 1
+        self.benchmark = cumulative_returns
+        return cumulative_returns
+
+    def plot_correlation_heatmap(self, save=False) -> None:
         if len(self.backtest) < 1:
             logger.warn("please run `.build()` before plotting")
         stock_returns = self.backtest.drop("portfolio_returns", axis=1)
         correlation_matrix = stock_returns.corr()
         logger.info("calculating portfolio correlation")
-        plot.plot_heatmap(correlation_matrix, "Portfolio Correlation")
+        plot.plot_heatmap(correlation_matrix, "Portfolio Correlation", save)
 
-    def plot_returns_data(self) -> None:
+    def plot_returns_data(self, save=False) -> None:
         if len(self.backtest) < 1:
             logger.warn("please run `.build()` before plotting")
-        plot.plot_histogram(self.clean_returns, self.percentage_returns, "Returns data")
+        plot.plot_histogram(
+            self.clean_returns, self.percentage_returns, "Returns data", save
+        )
+
+    def plot_benchmark(self, save=False) -> None:
+        if len(self.benchmark) < 1:
+            logger.warn("please run `.benchmark_analysis()` before plotting")
+        plot.plot_excess_returns(self.benchmark, "Portfolio Returns", save)
```

### Comparing `invest_tools-0.2.4/invest_tools/validation.py` & `invest_tools-0.2.5/invest_tools/validation.py`

 * *Files identical despite different names*

### Comparing `invest_tools-0.2.4/pyproject.toml` & `invest_tools-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "invest-tools"
-version = "0.2.4"
+version = "0.2.5"
 description = "Tools to manage portfolio risk analysis"
 authors = ["leo <leojpedwards@gmail.com>"]
 readme = "README.md"
 packages = [{include = "invest_tools"}]
 license = "MIT"
 
 [tool.poetry.dependencies]
```

### Comparing `invest_tools-0.2.4/setup.py` & `invest_tools-0.2.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,17 +13,17 @@
  'pandas>=1.5.3,<2.0.0',
  'scipy>=1.10.1,<2.0.0',
  'seaborn>=0.12.2,<0.13.0',
  'statsmodels>=0.13.5,<0.14.0']
 
 setup_kwargs = {
     'name': 'invest-tools',
-    'version': '0.2.4',
+    'version': '0.2.5',
     'description': 'Tools to manage portfolio risk analysis',
-    'long_description': '# invest-tools\n\n[![PyPI version](https://badge.fury.io/py/invest-tools.svg)](https://badge.fury.io/py/invest-tools)\n[![codecov](https://codecov.io/gh/leo-jp-edwards/invest-tools/graph/badge.svg?token=C1W8MZFS80)](https://codecov.io/gh/leo-jp-edwards/invest-tools)\n[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n**Tools to manage portfolio risk analysis**\n\n## Installation\n\nAs a python package this should be installable through:\n\n> `pip install invest-tools`\n\nOr:\n\n> `poetry add invest-tools`\n\n### Dependencies\n\nThe dependencies of this project can be seen in the `pyproject.toml` file. However for completeness there is a dependcy on `pandas`, `statsmodels` and `matplotlib` as the basics.\n\n## Data Inputs\n\nThere are three data inputs which should be present for the package to work as expected. \n\nThe path strings to the csvs can be passed in. \n\n1. Portfolio price data as a CSV\n\n| TIDM | Date | Open | High | Low | Close | Volume | Adjustment |\n|------|------|------|------|-----|-------|--------|------------|\n| EG | 01/01/2023 | 1 | 1 | 1 | 1 | 1 | 1 |\n| EG2 | 01/01/2023 | 1 | 1 | 1 | 1 | 1 | 1 |\n\n2. Currency data as a CSV\n\n| Date | Open | High | Low | Close | Adj Close | Volume |\n|------|------|------|-----|-------|-----------|--------|\n| 01/01/2023 | 1 | 1 | 1 | 1 | 1 | 1 |\n\n3. Fama French Data as a CSV\n\nThis can be found [here](https://mba.tuck.dartmouth.edu/pages/faculty/ken.french/data_library.html)\n\n## Example\n\nBuild a portfolio of two securities called `EG` and `EG2` with the weighting split 50:50 between the two. One is denominated in GBP and one in USD.\n\nThis will output the mean returns of such a portfolio.\n\n```python\nimport numpy as np\nfrom invest_tools import portfolio\n\nportfolio_definition = {\n    "EG": {\n        "weight": 0.5,\n        "currency": "gbp"\n    },\n    "EG2": {\n        "weight": 0.5,\n        "currency": "usd"\n    }\n}\n\nport = portfolio.Portfolio(portfolio_definition, portfolio.Currency.GBP)\nport.get_usd_converter("path/to/csv")\nport.get_prices("path/to/csv")\nport.build()\nport.analyse()\nprint(port.analysis)\nport.plot_correlation_heatmap()\nport.plot_returns_data()\n```\n\n## Roadmap\n\n- [x] Add an input validator\n- [x] Add logging\n- [ ] Add deeper analysis methods\n    - [ ] Coppock Curve\n    - [ ] Fama French\n    - [ ] Excess Returns\n    - [ ] Maximum Drawdown\n    - [ ] Calculate Moments\n- [ ] Add further testing\n- [ ] Make the package more generic\n- [ ] Investigate using [Polars](https://www.pola.rs/)\n\n## License\n\n[MIT](LICENSE)\n\n## Contact\n\nJust open an issue I guess?',
+    'long_description': '# invest-tools\n\n[![PyPI version](https://badge.fury.io/py/invest-tools.svg)](https://badge.fury.io/py/invest-tools)\n[![codecov](https://codecov.io/gh/leo-jp-edwards/invest-tools/graph/badge.svg?token=C1W8MZFS80)](https://codecov.io/gh/leo-jp-edwards/invest-tools)\n[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n**Tools to manage portfolio risk analysis**\n\n## Installation\n\nAs a python package this should be installable through:\n\n> `pip install invest-tools`\n\nOr:\n\n> `poetry add invest-tools`\n\n### Dependencies\n\nThe dependencies of this project can be seen in the `pyproject.toml` file. However for completeness there is a dependcy on `pandas`, `statsmodels` and `matplotlib` as the basics.\n\n## Data Inputs\n\nThere are three data inputs which should be present for the package to work as expected. \n\nThe path strings to the csvs can be passed in. \n\n1. Portfolio price data as a CSV\n\n| TIDM | Date | Open | High | Low | Close | Volume | Adjustment |\n|------|------|------|------|-----|-------|--------|------------|\n| EG | 01/01/2023 | 1 | 1 | 1 | 1 | 1 | 1 |\n| EG2 | 01/01/2023 | 1 | 1 | 1 | 1 | 1 | 1 |\n\n2. Currency data as a CSV\n\n| Date | Open | High | Low | Close | Adj Close | Volume |\n|------|------|------|-----|-------|-----------|--------|\n| 01/01/2023 | 1 | 1 | 1 | 1 | 1 | 1 |\n\n## Example\n\nBuild a portfolio of two securities called `EG` and `EG2` with the weighting split 50:50 between the two. One is denominated in GBP and one in USD.\n\nThis will output the mean returns of such a portfolio.\n\n```python\nimport numpy as np\nfrom invest_tools import portfolio\n\nportfolio_definition = {\n    "EG": {\n        "weight": 0.5,\n        "currency": "gbp"\n    },\n    "EG2": {\n        "weight": 0.5,\n        "currency": "usd"\n    }\n}\n\nport = portfolio.Portfolio(portfolio_definition, portfolio.Currency.GBP)\nport.get_usd_converter("path/to/csv")\nport.get_prices("path/to/csv")\nport.build()\nport.analyse()\nprint(port.analysis)\nport.plot_correlation_heatmap()\nport.plot_returns_data()\n```\n\n## Roadmap\n\n- [x] Add an input validator\n- [x] Add logging\n- [ ] Update risk free calculation to use new data outputs\n- [ ] Add deeper analysis methods\n    - [ ] Coppock Curve\n    - [ ] Fama French\n    - [ ] Excess Returns\n    - [ ] Maximum Drawdown\n    - [ ] Calculate Moments\n- [ ] Add further testing\n- [ ] Make the package more generic\n- [ ] Investigate using [Polars](https://www.pola.rs/)\n- [ ] Add func to calculate number of shares to buy to achieve portfolio make up (need to take in cash total for portfolio)\n\n## License\n\n[MIT](LICENSE)\n\n## Contact\n\nJust open an issue I guess?',
     'author': 'leo',
     'author_email': 'leojpedwards@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `invest_tools-0.2.4/PKG-INFO` & `invest_tools-0.2.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invest-tools
-Version: 0.2.4
+Version: 0.2.5
 Summary: Tools to manage portfolio risk analysis
 License: MIT
 Author: leo
 Author-email: leojpedwards@gmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -56,18 +56,14 @@
 
 2. Currency data as a CSV
 
 | Date | Open | High | Low | Close | Adj Close | Volume |
 |------|------|------|-----|-------|-----------|--------|
 | 01/01/2023 | 1 | 1 | 1 | 1 | 1 | 1 |
 
-3. Fama French Data as a CSV
-
-This can be found [here](https://mba.tuck.dartmouth.edu/pages/faculty/ken.french/data_library.html)
-
 ## Example
 
 Build a portfolio of two securities called `EG` and `EG2` with the weighting split 50:50 between the two. One is denominated in GBP and one in USD.
 
 This will output the mean returns of such a portfolio.
 
 ```python
@@ -95,23 +91,25 @@
 port.plot_returns_data()
 ```
 
 ## Roadmap
 
 - [x] Add an input validator
 - [x] Add logging
+- [ ] Update risk free calculation to use new data outputs
 - [ ] Add deeper analysis methods
     - [ ] Coppock Curve
     - [ ] Fama French
     - [ ] Excess Returns
     - [ ] Maximum Drawdown
     - [ ] Calculate Moments
 - [ ] Add further testing
 - [ ] Make the package more generic
 - [ ] Investigate using [Polars](https://www.pola.rs/)
+- [ ] Add func to calculate number of shares to buy to achieve portfolio make up (need to take in cash total for portfolio)
 
 ## License
 
 [MIT](LICENSE)
 
 ## Contact
```

