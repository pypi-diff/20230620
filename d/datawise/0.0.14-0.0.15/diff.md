# Comparing `tmp/datawise-0.0.14.tar.gz` & `tmp/datawise-0.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datawise-0.0.14.tar", max compression
+gzip compressed data, was "datawise-0.0.15.tar", max compression
```

## Comparing `datawise-0.0.14.tar` & `datawise-0.0.15.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-06-16 12:22:48.812559 datawise-0.0.14/LICENSE
--rw-r--r--   0        0        0     6055 2023-06-19 13:50:52.816983 datawise-0.0.14/README.md
--rw-r--r--   0        0        0     3134 2023-06-19 03:44:24.613208 datawise-0.0.14/datawise/__init__.py
--rw-r--r--   0        0        0      481 2023-06-18 12:46:33.125357 datawise-0.0.14/datawise/exceptions.py
--rw-r--r--   0        0        0      594 2023-06-19 13:51:02.252466 datawise-0.0.14/pyproject.toml
--rw-r--r--   0        0        0     6658 1970-01-01 00:00:00.000000 datawise-0.0.14/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-16 12:22:48.812559 datawise-0.0.15/LICENSE
+-rw-r--r--   0        0        0     6818 2023-06-20 04:10:21.992731 datawise-0.0.15/README.md
+-rw-r--r--   0        0        0     5433 2023-06-20 04:01:43.116353 datawise-0.0.15/datawise/__init__.py
+-rw-r--r--   0        0        0      481 2023-06-18 12:46:33.125357 datawise-0.0.15/datawise/exceptions.py
+-rw-r--r--   0        0        0      634 2023-06-20 04:04:41.402374 datawise-0.0.15/pyproject.toml
+-rw-r--r--   0        0        0     7421 1970-01-01 00:00:00.000000 datawise-0.0.15/PKG-INFO
```

### Comparing `datawise-0.0.14/LICENSE` & `datawise-0.0.15/LICENSE`

 * *Files identical despite different names*

### Comparing `datawise-0.0.14/README.md` & `datawise-0.0.15/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # DataWise
 
 ### DataWise is your co-pilot for performing data analysis and visualization in Python.
 
 ## Capabilities
 * Use SQL to transform Pandas dataframes
-* Coming soon: Use English to visualize Pandas dataframes
+* Use English to visualize Pandas dataframes (beta)
 
 ## Limitations
 * May occasionally generate incorrect results
 
 ## 🔍 Demo
 Try out DataWise in your browser:
 
@@ -110,16 +110,31 @@
 
 ### Limitations of using SQL to transform Pandas dataframes
 * May occasionally generate incorrect results
 * Ordering of rows is not strict unless ORDER BY clause is specified
 * No support for Window functions: https://www.sqlite.org/windowfunctions.html
 * If SQL query contains WHERE clause with `LIKE` operator, incorrect result might be generated
 
-## Use English to visualize Pandas dataframes
-Coming soon!
+## Use English to visualize Pandas dataframes (beta)
+You can write English to describe how you want to visualize your dataframe.
+This feature is available as beta feature so accurate result is not guaranteed.
+
+```python
+from datawise import DataWise
+import pandas as pd
+
+countries = pd.DataFrame({
+    "country": ["United States", "United Kingdom", "France", "Germany", "Italy", "Spain", "Canada", "Australia", "Japan", "China"],
+    "gdp": [19294482071552, 2891615567872, 2411255037952, 3435817336832, 1745433788416, 1181205135360, 1607402389504, 1490967855104, 4380756541440, 14631844184064],
+    "happiness_index": [6.94, 7.16, 6.66, 7.07, 6.38, 6.4, 7.23, 7.22, 5.87, 5.12]
+})
+
+dw = DataWise(api_key="you_api_key_here")
+dw.viz("Show me bar chart with country's gdp sorted by gdp descending", { "countries": countries })
+```
 
 ## Printing out translated code
 You can ask DataWise to print translated code to console using `code=True` flag.
 ```python
 import logging
 import sys
```

### Comparing `datawise-0.0.14/datawise/__init__.py` & `datawise-0.0.15/datawise/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -15,15 +15,14 @@
     self, 
     api_base="https://datawise.vercel.app/api",
     api_key=None
   ):
     load_dotenv()
     self.api_base = api_base if api_base else os.getenv("DATAWISE_API_BASE")
     self.api_key = api_key if api_key else os.getenv("DATAWISE_API_KEY")
-
   
   def sql(self, query, dataframes, code=False):
     """
     Transforms given dataframes based on given SQL query.
 
     Parameters:
     -----------
@@ -81,8 +80,66 @@
         data["error"] = "Is not a pandas dataframe. Please return dataframe."
         return_df = self._sql(query, dataframes, error=data["error"], code=code, num_retries=num_retries, prev_code=python_code)
     except Exception as e:
       num_retries += 1
       data["error"] = f"Threw exception: `{e}`"
       return_df = self._sql(query, dataframes, error=data["error"], code=code, num_retries=num_retries, prev_code=python_code)
     
-    return return_df
+    return return_df
+  
+  def viz(self, prompt, dataframes, code=False):
+    """
+    Creates visualization based on given prompt.
+
+    Parameters:
+    -----------
+    prompt: str
+      Prompt to be used for visualization.
+    dataframes: Pandas dataframes
+      Dictionary of dataframes to be transformed.
+      The key is the dataframe name and the value is the dataframe itself.
+      Example:
+      {"customers_df": customers_df, "employees_df": employees_df}
+    Code: bool
+      Whether to print/log the pandas code used to generate visualization or not.
+    """
+    return self._viz(prompt, dataframes, code=code)
+
+  @retry(exceptions=(RequestException, DataWiseInternalError), tries=3, delay=2)
+  def _viz(self, prompt, dataframes, code=False, error=None, num_retries=0, prev_code=None):
+    if not (type(dataframes) is dict): raise Exception("dataframes needs to be a dictionary with key being dataframe name and value being the dataframe.")
+
+    if num_retries >= 2:
+      logging.error(f"We couldn't translate your prompt into visualization. Here is python code we attempted to generate: \n{prev_code}")
+      raise TranslationError()
+    
+    data = {
+      "dataframe": "\n".join([f"{idx+1}. Dataframe named {key} with columns={value.columns.tolist()} {'and index=[' + value.index.name + ']' if value.index.name else ''}." for idx, (key, value) in enumerate(dataframes.items())]),
+      "nl": prompt,
+      "error": error
+    }
+
+    response = requests.post(
+      self.api_base + "/nl2seaborn", 
+      data=json.dumps(data), 
+      headers={
+        "Authorization": "Bearer " + self.api_key,
+        "content-type": "application/json"
+      }
+    )
+
+    if (response.status_code == 400): raise AuthorizationError()
+    if (response.status_code >= 500): raise DataWiseInternalError()
+
+    python_code = response.json()
+
+    import matplotlib.pyplot as plt
+    import seaborn as sns
+    globals = { "plt": plt, "sns": sns }
+    locals = dataframes.copy()
+    try:
+      exec(python_code, globals, locals)
+      if code: logging.info(f"Given prompt: \n{prompt} \nOutput code: \n{python_code}\n")
+    except Exception as e:
+      num_retries += 1
+      data["error"] = f"Threw exception: `{e}`"
+      self._viz(prompt, dataframes, error=data["error"], code=code, num_retries=num_retries, prev_code=python_code)
```

### Comparing `datawise-0.0.14/pyproject.toml` & `datawise-0.0.15/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 [tool.poetry]
 name = "datawise"
-version = "0.0.14"
+version = "0.0.15"
 description = "DataWise is your co-pilot for performing data analysis and visualization in Python."
 authors = ["DataWise Team"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9.0"
 python-dotenv = "^1.0.0"
 requests = "2.31.0"
 retry = "^0.9.2"
 urllib3 = "^1.26.6"
 
 [tool.poetry.dev-dependencies]
 black = "^21.9b0"
-pandas = "^2.0.2"
 numpy = "^1.25.0"
+matplotlib = "3.7.1"
+pandas = "^2.0.2"
 pytest = "^6.2.5"
 pytest-cov = "^2.12.1"
 pytest-sugar = "^0.9.4"
 pytest-watch = "^4.2.0"
+seaborn = "0.12.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `datawise-0.0.14/PKG-INFO` & `datawise-0.0.15/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datawise
-Version: 0.0.14
+Version: 0.0.15
 Summary: DataWise is your co-pilot for performing data analysis and visualization in Python.
 Author: DataWise Team
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -16,15 +16,15 @@
 
 # DataWise
 
 ### DataWise is your co-pilot for performing data analysis and visualization in Python.
 
 ## Capabilities
 * Use SQL to transform Pandas dataframes
-* Coming soon: Use English to visualize Pandas dataframes
+* Use English to visualize Pandas dataframes (beta)
 
 ## Limitations
 * May occasionally generate incorrect results
 
 ## 🔍 Demo
 Try out DataWise in your browser:
 
@@ -126,16 +126,31 @@
 
 ### Limitations of using SQL to transform Pandas dataframes
 * May occasionally generate incorrect results
 * Ordering of rows is not strict unless ORDER BY clause is specified
 * No support for Window functions: https://www.sqlite.org/windowfunctions.html
 * If SQL query contains WHERE clause with `LIKE` operator, incorrect result might be generated
 
-## Use English to visualize Pandas dataframes
-Coming soon!
+## Use English to visualize Pandas dataframes (beta)
+You can write English to describe how you want to visualize your dataframe.
+This feature is available as beta feature so accurate result is not guaranteed.
+
+```python
+from datawise import DataWise
+import pandas as pd
+
+countries = pd.DataFrame({
+    "country": ["United States", "United Kingdom", "France", "Germany", "Italy", "Spain", "Canada", "Australia", "Japan", "China"],
+    "gdp": [19294482071552, 2891615567872, 2411255037952, 3435817336832, 1745433788416, 1181205135360, 1607402389504, 1490967855104, 4380756541440, 14631844184064],
+    "happiness_index": [6.94, 7.16, 6.66, 7.07, 6.38, 6.4, 7.23, 7.22, 5.87, 5.12]
+})
+
+dw = DataWise(api_key="you_api_key_here")
+dw.viz("Show me bar chart with country's gdp sorted by gdp descending", { "countries": countries })
+```
 
 ## Printing out translated code
 You can ask DataWise to print translated code to console using `code=True` flag.
 ```python
 import logging
 import sys
```

