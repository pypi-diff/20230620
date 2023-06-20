# Comparing `tmp/datawise-0.0.16.tar.gz` & `tmp/datawise-0.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datawise-0.0.16.tar", max compression
+gzip compressed data, was "datawise-0.0.17.tar", max compression
```

## Comparing `datawise-0.0.16.tar` & `datawise-0.0.17.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-06-16 12:22:48.812559 datawise-0.0.16/LICENSE
--rw-r--r--   0        0        0     6818 2023-06-20 04:10:21.992731 datawise-0.0.16/README.md
--rw-r--r--   0        0        0     5600 2023-06-20 11:36:16.459385 datawise-0.0.16/datawise/__init__.py
--rw-r--r--   0        0        0      636 2023-06-20 11:29:08.510434 datawise-0.0.16/datawise/exceptions.py
--rw-r--r--   0        0        0      634 2023-06-20 11:46:57.003406 datawise-0.0.16/pyproject.toml
--rw-r--r--   0        0        0     7421 1970-01-01 00:00:00.000000 datawise-0.0.16/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-16 12:22:48.812559 datawise-0.0.17/LICENSE
+-rw-r--r--   0        0        0     6649 2023-06-20 12:17:27.028479 datawise-0.0.17/README.md
+-rw-r--r--   0        0        0     5600 2023-06-20 11:36:16.459385 datawise-0.0.17/datawise/__init__.py
+-rw-r--r--   0        0        0      636 2023-06-20 11:29:08.510434 datawise-0.0.17/datawise/exceptions.py
+-rw-r--r--   0        0        0      634 2023-06-20 12:17:31.537149 datawise-0.0.17/pyproject.toml
+-rw-r--r--   0        0        0     7252 1970-01-01 00:00:00.000000 datawise-0.0.17/PKG-INFO
```

### Comparing `datawise-0.0.16/LICENSE` & `datawise-0.0.17/LICENSE`

 * *Files identical despite different names*

### Comparing `datawise-0.0.16/README.md` & `datawise-0.0.17/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -114,26 +114,26 @@
 * No support for Window functions: https://www.sqlite.org/windowfunctions.html
 * If SQL query contains WHERE clause with `LIKE` operator, incorrect result might be generated
 
 ## Use English to visualize Pandas dataframes (beta)
 You can write English to describe how you want to visualize your dataframe.
 This feature is available as beta feature so accurate result is not guaranteed.
 
+You need to install `matplotlib` and `seaborn` packages as pre-requisites for SQL query.
+```bash
+pip install matplotlib seaborn
+```
+
+To visualize, simply call `viz` function.
 ```python
 from datawise import DataWise
-import pandas as pd
-
-countries = pd.DataFrame({
-    "country": ["United States", "United Kingdom", "France", "Germany", "Italy", "Spain", "Canada", "Australia", "Japan", "China"],
-    "gdp": [19294482071552, 2891615567872, 2411255037952, 3435817336832, 1745433788416, 1181205135360, 1607402389504, 1490967855104, 4380756541440, 14631844184064],
-    "happiness_index": [6.94, 7.16, 6.66, 7.07, 6.38, 6.4, 7.23, 7.22, 5.87, 5.12]
-})
 
 dw = DataWise(api_key="you_api_key_here")
-dw.viz("Show me bar chart with country's gdp sorted by gdp descending", { "countries": countries })
+tips = sns.load_dataset("tips")
+dw.viz("Show me relationship between total bill and tip. Each day should have different colour. Title is: Total Bill vs Tip", { "tips": tips }, code=True)
 ```
 
 ## Printing out translated code
 You can ask DataWise to print translated code to console using `code=True` flag.
 ```python
 import logging
 import sys
```

### Comparing `datawise-0.0.16/datawise/__init__.py` & `datawise-0.0.17/datawise/__init__.py`

 * *Files identical despite different names*

### Comparing `datawise-0.0.16/datawise/exceptions.py` & `datawise-0.0.17/datawise/exceptions.py`

 * *Files identical despite different names*

### Comparing `datawise-0.0.16/pyproject.toml` & `datawise-0.0.17/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datawise"
-version = "0.0.16"
+version = "0.0.17"
 description = "DataWise is your co-pilot for performing data analysis and visualization in Python."
 authors = ["DataWise Team"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9.0"
 python-dotenv = "^1.0.0"
```

### Comparing `datawise-0.0.16/PKG-INFO` & `datawise-0.0.17/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datawise
-Version: 0.0.16
+Version: 0.0.17
 Summary: DataWise is your co-pilot for performing data analysis and visualization in Python.
 Author: DataWise Team
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -130,26 +130,26 @@
 * No support for Window functions: https://www.sqlite.org/windowfunctions.html
 * If SQL query contains WHERE clause with `LIKE` operator, incorrect result might be generated
 
 ## Use English to visualize Pandas dataframes (beta)
 You can write English to describe how you want to visualize your dataframe.
 This feature is available as beta feature so accurate result is not guaranteed.
 
+You need to install `matplotlib` and `seaborn` packages as pre-requisites for SQL query.
+```bash
+pip install matplotlib seaborn
+```
+
+To visualize, simply call `viz` function.
 ```python
 from datawise import DataWise
-import pandas as pd
-
-countries = pd.DataFrame({
-    "country": ["United States", "United Kingdom", "France", "Germany", "Italy", "Spain", "Canada", "Australia", "Japan", "China"],
-    "gdp": [19294482071552, 2891615567872, 2411255037952, 3435817336832, 1745433788416, 1181205135360, 1607402389504, 1490967855104, 4380756541440, 14631844184064],
-    "happiness_index": [6.94, 7.16, 6.66, 7.07, 6.38, 6.4, 7.23, 7.22, 5.87, 5.12]
-})
 
 dw = DataWise(api_key="you_api_key_here")
-dw.viz("Show me bar chart with country's gdp sorted by gdp descending", { "countries": countries })
+tips = sns.load_dataset("tips")
+dw.viz("Show me relationship between total bill and tip. Each day should have different colour. Title is: Total Bill vs Tip", { "tips": tips }, code=True)
 ```
 
 ## Printing out translated code
 You can ask DataWise to print translated code to console using `code=True` flag.
 ```python
 import logging
 import sys
```

