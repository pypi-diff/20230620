# Comparing `tmp/CallingGPT-0.0.0.4.tar.gz` & `tmp/CallingGPT-0.0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CallingGPT-0.0.0.4.tar", last modified: Tue Jun 20 02:23:47 2023, max compression
+gzip compressed data, was "CallingGPT-0.0.0.5.tar", last modified: Tue Jun 20 12:30:01 2023, max compression
```

## Comparing `CallingGPT-0.0.0.4.tar` & `CallingGPT-0.0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-20 02:23:47.560138 CallingGPT-0.0.0.4/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-20 02:23:47.560138 CallingGPT-0.0.0.4/CallingGPT/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-20 02:23:47.560138 CallingGPT-0.0.0.4/CallingGPT/CallingGPT.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4491 2023-06-20 02:23:47.000000 CallingGPT-0.0.0.4/CallingGPT/CallingGPT.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      395 2023-06-20 02:23:47.000000 CallingGPT-0.0.0.4/CallingGPT/CallingGPT.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-20 02:23:47.000000 CallingGPT-0.0.0.4/CallingGPT/CallingGPT.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        7 2023-06-20 02:23:47.000000 CallingGPT-0.0.0.4/CallingGPT/CallingGPT.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       21 2023-06-20 02:23:47.000000 CallingGPT-0.0.0.4/CallingGPT/CallingGPT.egg-info/top_level.txt
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-20 02:23:47.560138 CallingGPT-0.0.0.4/CallingGPT/cli/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1062 2023-06-20 01:46:25.000000 CallingGPT-0.0.0.4/CallingGPT/cli/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-20 02:23:47.560138 CallingGPT-0.0.0.4/CallingGPT/entities/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-17 06:09:28.000000 CallingGPT-0.0.0.4/CallingGPT/entities/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5481 2023-06-20 02:23:14.000000 CallingGPT-0.0.0.4/CallingGPT/entities/namespace.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-20 02:23:47.560138 CallingGPT-0.0.0.4/CallingGPT/session/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-17 07:58:52.000000 CallingGPT-0.0.0.4/CallingGPT/session/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2287 2023-06-18 02:57:27.000000 CallingGPT-0.0.0.4/CallingGPT/session/session.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4491 2023-06-20 02:23:47.560138 CallingGPT-0.0.0.4/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4087 2023-06-18 14:38:18.000000 CallingGPT-0.0.0.4/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-06-20 02:23:47.564138 CallingGPT-0.0.0.4/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      748 2023-06-20 02:23:21.000000 CallingGPT-0.0.0.4/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-20 12:30:01.675328 CallingGPT-0.0.0.5/
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-20 12:30:01.667328 CallingGPT-0.0.0.5/CallingGPT/
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-20 12:30:01.671328 CallingGPT-0.0.0.5/CallingGPT/CallingGPT.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4492 2023-06-20 12:30:01.000000 CallingGPT-0.0.0.5/CallingGPT/CallingGPT.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      395 2023-06-20 12:30:01.000000 CallingGPT-0.0.0.5/CallingGPT/CallingGPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-20 12:30:01.000000 CallingGPT-0.0.0.5/CallingGPT/CallingGPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        7 2023-06-20 12:30:01.000000 CallingGPT-0.0.0.5/CallingGPT/CallingGPT.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       21 2023-06-20 12:30:01.000000 CallingGPT-0.0.0.5/CallingGPT/CallingGPT.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-20 12:30:01.671328 CallingGPT-0.0.0.5/CallingGPT/cli/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1887 2023-06-20 11:59:49.000000 CallingGPT-0.0.0.5/CallingGPT/cli/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-20 12:30:01.671328 CallingGPT-0.0.0.5/CallingGPT/entities/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-17 06:09:28.000000 CallingGPT-0.0.0.5/CallingGPT/entities/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6805 2023-06-20 12:29:42.000000 CallingGPT-0.0.0.5/CallingGPT/entities/namespace.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-20 12:30:01.675328 CallingGPT-0.0.0.5/CallingGPT/session/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-17 07:58:52.000000 CallingGPT-0.0.0.5/CallingGPT/session/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1913 2023-06-20 12:29:42.000000 CallingGPT-0.0.0.5/CallingGPT/session/session.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4492 2023-06-20 12:30:01.675328 CallingGPT-0.0.0.5/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4088 2023-06-20 11:59:45.000000 CallingGPT-0.0.0.5/README.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-06-20 12:30:01.675328 CallingGPT-0.0.0.5/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      748 2023-06-20 12:29:49.000000 CallingGPT-0.0.0.5/setup.py
```

### Comparing `CallingGPT-0.0.0.4/CallingGPT/CallingGPT.egg-info/PKG-INFO` & `CallingGPT-0.0.0.5/CallingGPT/CallingGPT.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CallingGPT
-Version: 0.0.0.4
+Version: 0.0.0.5
 Summary: GPT's function calling feature wrapper
 Home-page: https://github.com/RockChinQ/CallingGPT
 Author: RockChinQ
 Author-email: 1010553892@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -146,15 +146,15 @@
 3. Call the wrapper
 
     ```python
     from CallingGPT.session.session import Session
     import your_module_a, your_module_b
     import openai
 
-    openai.apikey = 'your_openai_api_key'
+    openai.api_key = 'your_openai_api_key'
 
     session = Session([your_module_a, your_module_b])
 
     session.ask("your prompt")
     ```
 
     `Session` will automatically manage context for you.
```

### Comparing `CallingGPT-0.0.0.4/CallingGPT/entities/namespace.py` & `CallingGPT-0.0.0.5/CallingGPT/entities/namespace.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,120 @@
 import sys
 import re
 import inspect
 
 
+def get_func_schema(function: callable) -> dict:
+    """
+    Return the data schema of a function.
+    {
+        "function": function,
+        "description": "function description",
+        "parameters": {
+            "type": "object",
+            "properties": {
+                "parameter_a": {
+                    "type": "str",
+                    "description": "parameter_a description"
+                },
+                "parameter_b": {
+                    "type": "int",
+                    "description": "parameter_b description"
+                },
+                "parameter_c": {
+                    "type": "str",
+                    "description": "parameter_c description",
+                    "enum": ["a", "b", "c"]
+                },
+            },
+            "required": ["parameter_a", "parameter_b"]
+        }
+    }
+    """
+    func_doc = function.__doc__
+    # Google Style Docstring
+    if func_doc is None:
+        raise Exception("Function {} has no docstring.".format(function.__name__))
+    func_doc = func_doc.strip().replace('    ','').replace('\t', '')
+    # extract doc of args from docstring
+    doc_spt = func_doc.split('\n\n')
+    desc = doc_spt[0]
+    args = doc_spt[1] if len(doc_spt) > 1 else ""
+    returns = doc_spt[2] if len(doc_spt) > 2 else ""
+
+    # extract args
+    # delete the first line of args
+    arg_lines = args.split('\n')[1:]
+    arg_doc_list = re.findall(r'(\w+)(\((\w+)\))?:\s*(.*)', args)
+    args_doc = {}
+    for arg_line in arg_lines:
+        doc_tuple = re.findall(r'(\w+)(\(([\w\[\]]+)\))?:\s*(.*)', arg_line)
+        if len(doc_tuple) == 0:
+            continue
+        args_doc[doc_tuple[0][0]] = doc_tuple[0][3]
+
+    # extract returns
+    return_doc_list = re.findall(r'(\w+):\s*(.*)', returns)
+
+    params = enumerate(inspect.signature(function).parameters.values())
+    parameters = {
+        "type": "object",
+        "required": [],
+        "properties": {},
+    }
+
+
+    for i, param in params:
+        param_type = param.annotation.__name__
+
+        type_name_mapping = {
+            "str": "string",
+            "int": "integer",
+            "float": "number",
+            "bool": "boolean",
+            "list": "array",
+            "dict": "object",
+        }
+
+        if param_type in type_name_mapping:
+            param_type = type_name_mapping[param_type]
+
+        parameters['properties'][param.name] = {
+            "type": param_type,
+            "description": args_doc[param.name],
+        }
+
+        # add schema for array
+        if param_type == "array":
+            # extract type of array, the int of list[int]
+            # use re
+            array_type_tuple = re.findall(r'list\[(\w+)\]', str(param.annotation))
+
+            array_type = 'string'
+
+            if len(array_type_tuple) > 0:
+                array_type = array_type_tuple[0]
+
+            if array_type in type_name_mapping:
+                array_type = type_name_mapping[array_type]
+
+            parameters['properties'][param.name]["items"] = {
+                "type": array_type,
+            }
+
+        if param.default is inspect.Parameter.empty:
+            parameters["required"].append(param.name)
+
+    return {
+        "function": function,
+        "description": desc,
+        "parameters": parameters,
+    }
+
+
 class Namespace:
     """
     Namespace is a virtual container for functions, generated automatically by CallingGPT
     with user provided modules.
     """
 
     modules: list = []
@@ -15,26 +123,29 @@
     """Store functions with structure as follows:
     {
         "module_name_a": {
             "function_name_a": {
                 "function": function_a,
                 "description": "function_a description",
                 "parameters": {
-                    "parameter_a": {
-                        "type": "str",
-                        "description": "parameter_a description"
-                    },
-                    "parameter_b": {
-                        "type": "int",
-                        "description": "parameter_b description"
-                    },
-                    "parameter_c": {
-                        "type": "str",
-                        "description": "parameter_c description",
-                        "enum": ["a", "b", "c"]
+                    "type": "object",
+                    "properties": {
+                        "parameter_a": {
+                            "type": "str",
+                            "description": "parameter_a description"
+                        },
+                        "parameter_b": {
+                            "type": "int",
+                            "description": "parameter_b description"
+                        },
+                        "parameter_c": {
+                            "type": "str",
+                            "description": "parameter_c description",
+                            "enum": ["a", "b", "c"]
+                        },
                     },
                     "required": ["parameter_a", "parameter_b"]
                 }
             },
         }
     }
 
@@ -49,93 +160,15 @@
             functions = {k: v for k, v in module.__dict__.items() if callable(v)}
             # ignore private functions
             functions = {k: v for k, v in functions.items() if not k.startswith('_')}
 
             self.functions[module.__name__.replace(".","-")] = {}
 
             for name, function in functions.items():
-                
-                func_doc = function.__doc__
-                # Google Style Docstring
-                if func_doc is None:
-                    raise Exception("Function {} has no docstring.".format(name))
-                func_doc = func_doc.strip().replace('    ','').replace('\t', '')
-                # extract doc of args from docstring
-                doc_spt = func_doc.split('\n\n')
-                desc = doc_spt[0]
-                args = doc_spt[1] if len(doc_spt) > 1 else ""
-                returns = doc_spt[2] if len(doc_spt) > 2 else ""
-
-                # extract args
-                # delete the first line of args
-                arg_lines = args.split('\n')[1:]
-                args_doc = {}
-                for arg_line in arg_lines:
-                    doc_tuple = re.findall(r'(\w+)(\(([\w\[\]]+)\))?:\s*(.*)', arg_line)
-                    if len(doc_tuple) == 0:
-                        continue
-                    args_doc[doc_tuple[0][0]] = doc_tuple[0][3]
-
-                # extract returns
-                return_doc_list = re.findall(r'(\w+):\s*(.*)', returns)
-
-                params = enumerate(inspect.signature(function).parameters.values())
-                parameters = {
-                    "type": "object",
-                    "required": [],
-                    "properties": {},
-                }
-
-
-                for i, param in params:
-                    param_type = param.annotation.__name__
-
-                    type_name_mapping = {
-                        "str": "string",
-                        "int": "integer",
-                        "float": "number",
-                        "bool": "boolean",
-                        "list": "array",
-                        "dict": "object",
-                    }
-
-                    if param_type in type_name_mapping:
-                        param_type = type_name_mapping[param_type]
-
-                    parameters['properties'][param.name] = {
-                        "type": param_type,
-                        "description": args_doc[param.name],
-                    }
-
-                    # add schema for array
-                    if param_type == "array":
-                        # extract type of array, the int of list[int]
-                        # use re
-                        array_type_tuple = re.findall(r'list\[(\w+)\]', str(param.annotation))
-
-                        array_type = 'string'
-
-                        if len(array_type_tuple) > 0:
-                            array_type = array_type_tuple[0]
-                        
-                        if array_type in type_name_mapping:
-                            array_type = type_name_mapping[array_type]
-                        
-                        parameters['properties'][param.name]["items"] = {
-                            "type": array_type,
-                        }
-
-                    if param.default is inspect.Parameter.empty:
-                        parameters["required"].append(param.name)
-
-                funtion_dict = {
-                    "function": function,
-                    "description": desc,
-                    "parameters": parameters,
-                }
+                funtion_dict = get_func_schema(function)
 
                 self.functions[module.__name__.replace(".","-")][name] = funtion_dict
 
     def __init__(self, modules: list):
         self.modules = modules
         self._retrieve_functions()
 
@@ -146,7 +179,43 @@
             for function_name, function in module.items():
                 func = function.copy()
                 func["name"] = "{}-{}".format(module_name, function_name)
                 del func["function"]
                 result.append(func)
 
         return result
+    
+    def call_function(self, function_name: str, args: dict):
+        """
+        Call a function by name.
+        """
+        result = {}
+
+        # split the function name
+        fn_spt = function_name.split('-')
+        module_name = '-'.join(fn_spt[:-1])
+        function_name = fn_spt[-1]
+
+        # get the function
+        function = self.functions[module_name][function_name]['function']
+
+        # call the function
+        result = function(**args)
+
+        return result
+    
+    def add_function(self, module_name: str, function: callable):
+        """
+        Add a function to namespace.
+        """
+        # assert isinstance(function, callable)
+        if module_name not in self.functions:
+            self.functions[module_name] = {}
+        self.functions[module_name][function.__name__] = get_func_schema(function)
+
+    def add_modules(self, modules: list):
+        """
+        Add a module to namespace.
+        """
+        self.modules.extend(modules)
+        self._retrieve_functions()
+
```

### Comparing `CallingGPT-0.0.0.4/PKG-INFO` & `CallingGPT-0.0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CallingGPT
-Version: 0.0.0.4
+Version: 0.0.0.5
 Summary: GPT's function calling feature wrapper
 Home-page: https://github.com/RockChinQ/CallingGPT
 Author: RockChinQ
 Author-email: 1010553892@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -146,15 +146,15 @@
 3. Call the wrapper
 
     ```python
     from CallingGPT.session.session import Session
     import your_module_a, your_module_b
     import openai
 
-    openai.apikey = 'your_openai_api_key'
+    openai.api_key = 'your_openai_api_key'
 
     session = Session([your_module_a, your_module_b])
 
     session.ask("your prompt")
     ```
 
     `Session` will automatically manage context for you.
```

### Comparing `CallingGPT-0.0.0.4/README.md` & `CallingGPT-0.0.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
 3. Call the wrapper
 
     ```python
     from CallingGPT.session.session import Session
     import your_module_a, your_module_b
     import openai
 
-    openai.apikey = 'your_openai_api_key'
+    openai.api_key = 'your_openai_api_key'
 
     session = Session([your_module_a, your_module_b])
 
     session.ask("your prompt")
     ```
 
     `Session` will automatically manage context for you.
```

### Comparing `CallingGPT-0.0.0.4/setup.py` & `CallingGPT-0.0.0.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='CallingGPT',
-    version='0.0.0.4',
+    version='0.0.0.5',
     description="GPT's function calling feature wrapper",
     long_description=open('README.md', encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     install_requires=[
         'openai',
     ],
     author='RockChinQ',
```

