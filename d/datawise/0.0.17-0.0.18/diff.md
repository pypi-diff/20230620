# Comparing `tmp/datawise-0.0.17.tar.gz` & `tmp/datawise-0.0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datawise-0.0.17.tar", max compression
+gzip compressed data, was "datawise-0.0.18.tar", max compression
```

## Comparing `datawise-0.0.17.tar` & `datawise-0.0.18.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-06-16 12:22:48.812559 datawise-0.0.17/LICENSE
--rw-r--r--   0        0        0     6649 2023-06-20 12:17:27.028479 datawise-0.0.17/README.md
--rw-r--r--   0        0        0     5600 2023-06-20 11:36:16.459385 datawise-0.0.17/datawise/__init__.py
--rw-r--r--   0        0        0      636 2023-06-20 11:29:08.510434 datawise-0.0.17/datawise/exceptions.py
--rw-r--r--   0        0        0      634 2023-06-20 12:17:31.537149 datawise-0.0.17/pyproject.toml
--rw-r--r--   0        0        0     7252 1970-01-01 00:00:00.000000 datawise-0.0.17/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-16 12:22:48.812559 datawise-0.0.18/LICENSE
+-rw-r--r--   0        0        0     6747 2023-06-20 15:41:21.140673 datawise-0.0.18/README.md
+-rw-r--r--   0        0        0     5600 2023-06-20 11:36:16.459385 datawise-0.0.18/datawise/__init__.py
+-rw-r--r--   0        0        0      636 2023-06-20 11:29:08.510434 datawise-0.0.18/datawise/exceptions.py
+-rw-r--r--   0        0        0      634 2023-06-20 15:41:23.699345 datawise-0.0.18/pyproject.toml
+-rw-r--r--   0        0        0     7350 1970-01-01 00:00:00.000000 datawise-0.0.18/PKG-INFO
```

### Comparing `datawise-0.0.17/LICENSE` & `datawise-0.0.18/LICENSE`

 * *Files identical despite different names*

### Comparing `datawise-0.0.17/README.md` & `datawise-0.0.18/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # DataWise
 
 ### DataWise is your co-pilot for performing data analysis and visualization in Python.
 
-## Capabilities
-* Use SQL to transform Pandas dataframes
-* Use English to visualize Pandas dataframes (beta)
+| Capabilities                                      | Limitations                                 |
+|---------------------------------------------------|---------------------------------------------|
+| Use SQL to transform Pandas dataframes            | May occasionally generate incorrect results |
+| Use English to visualize Pandas dataframes (beta) |                                             |
 
-## Limitations
-* May occasionally generate incorrect results
 
 ## 🔍 Demo
 Try out DataWise in your browser:
 
 [![Open in Colab](https://camo.githubusercontent.com/84f0493939e0c4de4e6dbe113251b4bfb5353e57134ffd9fcab6b8714514d4d1/68747470733a2f2f636f6c61622e72657365617263682e676f6f676c652e636f6d2f6173736574732f636f6c61622d62616467652e737667)](https://colab.research.google.com/drive/1onQI_V6NrAnEDY-o6N068xLyvsFojynf?usp=sharing)
 
 ## 🔧 Quick install
@@ -30,25 +29,20 @@
 ```python
 from datawise import DataWise
 
 dw = DataWise(api_key="you_api_key_here")
 ```
 
 ## Use SQL to transform Pandas dataframes
-You can use SQLite style SQL query to transform Pandas dataframes. Example:
-```sql
-SELECT * FROM countries LEFT JOIN country_populations ON countries.country = country_populations.country
-```
-
 You need to install `pandas` and `numpy` packages as pre-requisites for SQL query.
 ```bash
 pip install pandas numpy
 ```
 
-To transform, simply call `sql` function.
+To transform, simply call `sql` function. You can use SQLite style SQL query to transform Pandas dataframes.
 ```python
 from datawise import DataWise
 import pandas as pd
 
 countries = pd.DataFrame({
     "country": ["United States", "United Kingdom", "France", "Germany", "Italy", "Spain", "Canada", "Australia", "Japan", "China"],
     "gdp": [19294482071552, 2891615567872, 2411255037952, 3435817336832, 1745433788416, 1181205135360, 1607402389504, 1490967855104, 4380756541440, 14631844184064],
@@ -61,15 +55,15 @@
 })
 print(df)
 ```
 
 The above code will return the following dataframe:
 
 ```
-   count
+        count
 0          10
 ```
 
 You can also do joins of multiple dataframes:
 ```python
 from datawise import DataWise
 import pandas as pd
@@ -125,15 +119,15 @@
 
 To visualize, simply call `viz` function.
 ```python
 from datawise import DataWise
 
 dw = DataWise(api_key="you_api_key_here")
 tips = sns.load_dataset("tips")
-dw.viz("Show me relationship between total bill and tip. Each day should have different colour. Title is: Total Bill vs Tip", { "tips": tips }, code=True)
+dw.viz("Show me relationship between total bill and tip. Each day should have different colour. Title is: Total Bill vs Tip", { "tips": tips })
 ```
 
 ## Printing out translated code
 You can ask DataWise to print translated code to console using `code=True` flag.
 ```python
 import logging
 import sys
```

### Comparing `datawise-0.0.17/datawise/__init__.py` & `datawise-0.0.18/datawise/__init__.py`

 * *Files identical despite different names*

### Comparing `datawise-0.0.17/datawise/exceptions.py` & `datawise-0.0.18/datawise/exceptions.py`

 * *Files identical despite different names*

### Comparing `datawise-0.0.17/pyproject.toml` & `datawise-0.0.18/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datawise"
-version = "0.0.17"
+version = "0.0.18"
 description = "DataWise is your co-pilot for performing data analysis and visualization in Python."
 authors = ["DataWise Team"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9.0"
 python-dotenv = "^1.0.0"
```

### Comparing `datawise-0.0.17/PKG-INFO` & `datawise-0.0.18/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datawise
-Version: 0.0.17
+Version: 0.0.18
 Summary: DataWise is your co-pilot for performing data analysis and visualization in Python.
 Author: DataWise Team
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -14,20 +14,19 @@
 Requires-Dist: urllib3 (>=1.26.6,<2.0.0)
 Description-Content-Type: text/markdown
 
 # DataWise
 
 ### DataWise is your co-pilot for performing data analysis and visualization in Python.
 
-## Capabilities
-* Use SQL to transform Pandas dataframes
-* Use English to visualize Pandas dataframes (beta)
+| Capabilities                                      | Limitations                                 |
+|---------------------------------------------------|---------------------------------------------|
+| Use SQL to transform Pandas dataframes            | May occasionally generate incorrect results |
+| Use English to visualize Pandas dataframes (beta) |                                             |
 
-## Limitations
-* May occasionally generate incorrect results
 
 ## 🔍 Demo
 Try out DataWise in your browser:
 
 [![Open in Colab](https://camo.githubusercontent.com/84f0493939e0c4de4e6dbe113251b4bfb5353e57134ffd9fcab6b8714514d4d1/68747470733a2f2f636f6c61622e72657365617263682e676f6f676c652e636f6d2f6173736574732f636f6c61622d62616467652e737667)](https://colab.research.google.com/drive/1onQI_V6NrAnEDY-o6N068xLyvsFojynf?usp=sharing)
 
 ## 🔧 Quick install
@@ -46,25 +45,20 @@
 ```python
 from datawise import DataWise
 
 dw = DataWise(api_key="you_api_key_here")
 ```
 
 ## Use SQL to transform Pandas dataframes
-You can use SQLite style SQL query to transform Pandas dataframes. Example:
-```sql
-SELECT * FROM countries LEFT JOIN country_populations ON countries.country = country_populations.country
-```
-
 You need to install `pandas` and `numpy` packages as pre-requisites for SQL query.
 ```bash
 pip install pandas numpy
 ```
 
-To transform, simply call `sql` function.
+To transform, simply call `sql` function. You can use SQLite style SQL query to transform Pandas dataframes.
 ```python
 from datawise import DataWise
 import pandas as pd
 
 countries = pd.DataFrame({
     "country": ["United States", "United Kingdom", "France", "Germany", "Italy", "Spain", "Canada", "Australia", "Japan", "China"],
     "gdp": [19294482071552, 2891615567872, 2411255037952, 3435817336832, 1745433788416, 1181205135360, 1607402389504, 1490967855104, 4380756541440, 14631844184064],
@@ -77,15 +71,15 @@
 })
 print(df)
 ```
 
 The above code will return the following dataframe:
 
 ```
-   count
+        count
 0          10
 ```
 
 You can also do joins of multiple dataframes:
 ```python
 from datawise import DataWise
 import pandas as pd
@@ -141,15 +135,15 @@
 
 To visualize, simply call `viz` function.
 ```python
 from datawise import DataWise
 
 dw = DataWise(api_key="you_api_key_here")
 tips = sns.load_dataset("tips")
-dw.viz("Show me relationship between total bill and tip. Each day should have different colour. Title is: Total Bill vs Tip", { "tips": tips }, code=True)
+dw.viz("Show me relationship between total bill and tip. Each day should have different colour. Title is: Total Bill vs Tip", { "tips": tips })
 ```
 
 ## Printing out translated code
 You can ask DataWise to print translated code to console using `code=True` flag.
 ```python
 import logging
 import sys
```

