# Comparing `tmp/pandasai-0.6.1.tar.gz` & `tmp/pandasai-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasai-0.6.1.tar", max compression
+gzip compressed data, was "pandasai-0.6.2.tar", max compression
```

## Comparing `pandasai-0.6.1.tar` & `pandasai-0.6.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1055 2023-06-19 08:52:18.570412 pandasai-0.6.1/LICENSE
--rw-r--r--   0        0        0     7705 2023-06-19 08:52:18.574412 pandasai-0.6.1/README.md
--rw-r--r--   0        0        0    23083 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/__init__.py
--rw-r--r--   0        0        0     1440 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/constants.py
--rw-r--r--   0        0        0     1509 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0     3814 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/helpers/_optional.py
--rw-r--r--   0        0        0     5434 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/helpers/anonymizer.py
--rw-r--r--   0        0        0     1742 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/helpers/cache.py
--rw-r--r--   0        0        0      566 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/helpers/from_excel.py
--rw-r--r--   0        0        0     1493 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/helpers/notebook.py
--rw-r--r--   0        0        0     3252 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/helpers/save_chart.py
--rw-r--r--   0        0        0     4369 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/helpers/shortcuts.py
--rw-r--r--   0        0        0        0 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     4354 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/llm/azure_openai.py
--rw-r--r--   0        0        0    10885 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/llm/base.py
--rw-r--r--   0        0        0      542 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/llm/fake.py
--rw-r--r--   0        0        0     1213 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/llm/falcon.py
--rw-r--r--   0        0        0     1828 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/llm/google_palm.py
--rw-r--r--   0        0        0      577 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/llm/langchain.py
--rw-r--r--   0        0        0     1482 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/llm/open_assistant.py
--rw-r--r--   0        0        0     2932 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/llm/openai.py
--rw-r--r--   0        0        0     1220 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/llm/starcoder.py
--rw-r--r--   0        0        0        0 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/middlewares/__init__.py
--rw-r--r--   0        0        0      663 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/middlewares/base.py
--rw-r--r--   0        0        0      558 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/middlewares/charts.py
--rw-r--r--   0        0        0      653 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/middlewares/streamlit.py
--rw-r--r--   0        0        0        0 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/prompts/__init__.py
--rw-r--r--   0        0        0      647 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/prompts/base.py
--rw-r--r--   0        0        0     1697 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/prompts/correct_error_prompt.py
--rw-r--r--   0        0        0     1262 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/prompts/correct_multiples_prompt.py
--rw-r--r--   0        0        0     1514 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/prompts/generate_python_code.py
--rw-r--r--   0        0        0      460 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/prompts/generate_response.py
--rw-r--r--   0        0        0     1343 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/prompts/multiple_dataframes.py
--rw-r--r--   0        0        0     1712 2023-06-19 08:52:18.582413 pandasai-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     8807 1970-01-01 00:00:00.000000 pandasai-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-06-19 23:45:08.536893 pandasai-0.6.2/LICENSE
+-rw-r--r--   0        0        0     7705 2023-06-19 23:45:08.536893 pandasai-0.6.2/README.md
+-rw-r--r--   0        0        0    23288 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/__init__.py
+-rw-r--r--   0        0        0     1440 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/constants.py
+-rw-r--r--   0        0        0     1509 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0     3814 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/helpers/_optional.py
+-rw-r--r--   0        0        0     5434 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/helpers/anonymizer.py
+-rw-r--r--   0        0        0     1742 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/helpers/cache.py
+-rw-r--r--   0        0        0      566 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/helpers/from_excel.py
+-rw-r--r--   0        0        0     1493 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/helpers/notebook.py
+-rw-r--r--   0        0        0     3252 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/helpers/save_chart.py
+-rw-r--r--   0        0        0     4369 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/helpers/shortcuts.py
+-rw-r--r--   0        0        0        0 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     4354 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/llm/azure_openai.py
+-rw-r--r--   0        0        0    10885 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/llm/base.py
+-rw-r--r--   0        0        0      542 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/llm/fake.py
+-rw-r--r--   0        0        0     1213 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/llm/falcon.py
+-rw-r--r--   0        0        0     1828 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/llm/google_palm.py
+-rw-r--r--   0        0        0      577 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/llm/langchain.py
+-rw-r--r--   0        0        0     1482 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/llm/open_assistant.py
+-rw-r--r--   0        0        0     2932 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/llm/openai.py
+-rw-r--r--   0        0        0     1220 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/llm/starcoder.py
+-rw-r--r--   0        0        0        0 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/middlewares/__init__.py
+-rw-r--r--   0        0        0      663 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/middlewares/base.py
+-rw-r--r--   0        0        0      558 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/middlewares/charts.py
+-rw-r--r--   0        0        0      653 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/middlewares/streamlit.py
+-rw-r--r--   0        0        0        0 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/prompts/__init__.py
+-rw-r--r--   0        0        0      647 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/prompts/base.py
+-rw-r--r--   0        0        0     1697 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/prompts/correct_error_prompt.py
+-rw-r--r--   0        0        0     1262 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/prompts/correct_multiples_prompt.py
+-rw-r--r--   0        0        0     1514 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/prompts/generate_python_code.py
+-rw-r--r--   0        0        0      460 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/prompts/generate_response.py
+-rw-r--r--   0        0        0     1343 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/prompts/multiple_dataframes.py
+-rw-r--r--   0        0        0     1712 2023-06-19 23:45:08.544894 pandasai-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     8807 1970-01-01 00:00:00.000000 pandasai-0.6.2/PKG-INFO
```

### Comparing `pandasai-0.6.1/LICENSE` & `pandasai-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.1/README.md` & `pandasai-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.1/pandasai/__init__.py` & `pandasai-0.6.2/pandasai/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,14 +130,15 @@
     _cache: Cache = None
     _enable_cache: bool = True
     _prompt_id: Optional[str] = None
     _middlewares: List[Middleware] = [ChartsMiddleware()]
     _additional_dependencies: List[dict] = []
     _custom_whitelisted_dependencies: List[str] = []
     _start_time: float = 0
+    _enable_logging: bool = True
     last_code_generated: Optional[str] = None
     last_code_executed: Optional[str] = None
     code_output: Optional[str] = None
     last_error: Optional[str] = None
 
     def __init__(
         self,
@@ -145,14 +146,15 @@
         conversational=False,
         verbose=False,
         enforce_privacy=False,
         save_charts=False,
         enable_cache=True,
         middlewares=None,
         custom_whitelisted_dependencies=None,
+        enable_logging=True,
     ):
         """
 
         __init__ method of the Class PandasAI
 
         Args:
             llm (object): LLMs option to be used for API access. Default is None
@@ -165,20 +167,25 @@
             save_charts (bool): Save the charts generated in the notebook.
             Default to False
             enable_cache (bool): Enable the cache to store the results.
             Default to True
             middlewares (list): List of middlewares to be used. Default to None
             custom_whitelisted_dependencies (list): List of custom dependencies to
             be used. Default to None
+            enable_logging (bool): Enable the logging. Default to True
         """
 
         # configure the logging
         # noinspection PyArgumentList
         # https://stackoverflow.com/questions/61226587/pycharm-does-not-recognize-logging-basicconfig-handlers-argument
-        handlers = [logging.FileHandler("pandasai.log")]
+        if enable_logging:
+            handlers = [logging.FileHandler("pandasai.log")]
+        else:
+            handlers = []
+
         if verbose:
             handlers.append(logging.StreamHandler(sys.stdout))
         logging.basicConfig(
             level=logging.INFO,
             format="%(asctime)s [%(levelname)s] %(message)s",
             datefmt="%Y-%m-%d %H:%M:%S",
             handlers=handlers,
```

### Comparing `pandasai-0.6.1/pandasai/constants.py` & `pandasai-0.6.2/pandasai/constants.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.1/pandasai/exceptions.py` & `pandasai-0.6.2/pandasai/exceptions.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.1/pandasai/helpers/_optional.py` & `pandasai-0.6.2/pandasai/helpers/_optional.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.1/pandasai/helpers/anonymizer.py` & `pandasai-0.6.2/pandasai/helpers/anonymizer.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.1/pandasai/helpers/cache.py` & `pandasai-0.6.2/pandasai/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.1/pandasai/helpers/from_excel.py` & `pandasai-0.6.2/pandasai/helpers/from_excel.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.1/pandasai/helpers/notebook.py` & `pandasai-0.6.2/pandasai/helpers/notebook.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.1/pandasai/helpers/save_chart.py` & `pandasai-0.6.2/pandasai/helpers/save_chart.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.1/pandasai/helpers/shortcuts.py` & `pandasai-0.6.2/pandasai/helpers/shortcuts.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.1/pandasai/llm/azure_openai.py` & `pandasai-0.6.2/pandasai/llm/azure_openai.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.1/pandasai/llm/base.py` & `pandasai-0.6.2/pandasai/llm/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.1/pandasai/llm/fake.py` & `pandasai-0.6.2/pandasai/llm/fake.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.1/pandasai/llm/falcon.py` & `pandasai-0.6.2/pandasai/llm/falcon.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.1/pandasai/llm/google_palm.py` & `pandasai-0.6.2/pandasai/llm/google_palm.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.1/pandasai/llm/langchain.py` & `pandasai-0.6.2/pandasai/llm/langchain.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.1/pandasai/llm/open_assistant.py` & `pandasai-0.6.2/pandasai/llm/open_assistant.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.1/pandasai/llm/openai.py` & `pandasai-0.6.2/pandasai/llm/openai.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.1/pandasai/llm/starcoder.py` & `pandasai-0.6.2/pandasai/llm/starcoder.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.1/pandasai/middlewares/base.py` & `pandasai-0.6.2/pandasai/middlewares/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.1/pandasai/middlewares/charts.py` & `pandasai-0.6.2/pandasai/middlewares/charts.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.1/pandasai/middlewares/streamlit.py` & `pandasai-0.6.2/pandasai/middlewares/streamlit.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.1/pandasai/prompts/base.py` & `pandasai-0.6.2/pandasai/prompts/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.1/pandasai/prompts/correct_error_prompt.py` & `pandasai-0.6.2/pandasai/prompts/correct_error_prompt.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.1/pandasai/prompts/correct_multiples_prompt.py` & `pandasai-0.6.2/pandasai/prompts/correct_multiples_prompt.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.1/pandasai/prompts/generate_python_code.py` & `pandasai-0.6.2/pandasai/prompts/generate_python_code.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.1/pandasai/prompts/multiple_dataframes.py` & `pandasai-0.6.2/pandasai/prompts/multiple_dataframes.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.1/pyproject.toml` & `pandasai-0.6.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pandasai"
-version = "0.6.1"
+version = "0.6.2"
 description = "Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational."
 authors = ["Gabriele Venturi"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"}]
 
 [tool.poetry.dependencies]
```

### Comparing `pandasai-0.6.1/PKG-INFO` & `pandasai-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasai
-Version: 0.6.1
+Version: 0.6.2
 Summary: Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational.
 License: MIT
 Author: Gabriele Venturi
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

