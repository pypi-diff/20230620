# Comparing `tmp/CallingGPT-0.0.0.3.tar.gz` & `tmp/CallingGPT-0.0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CallingGPT-0.0.0.3.tar", last modified: Sun Jun 18 03:03:20 2023, max compression
+gzip compressed data, was "CallingGPT-0.0.0.4.tar", last modified: Tue Jun 20 02:23:47 2023, max compression
```

## Comparing `CallingGPT-0.0.0.3.tar` & `CallingGPT-0.0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-18 03:03:20.119381 CallingGPT-0.0.0.3/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-18 03:03:20.107380 CallingGPT-0.0.0.3/CallingGPT/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-18 03:03:20.115381 CallingGPT-0.0.0.3/CallingGPT/CallingGPT.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3506 2023-06-18 03:03:20.000000 CallingGPT-0.0.0.3/CallingGPT/CallingGPT.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      395 2023-06-18 03:03:20.000000 CallingGPT-0.0.0.3/CallingGPT/CallingGPT.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-18 03:03:20.000000 CallingGPT-0.0.0.3/CallingGPT/CallingGPT.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        7 2023-06-18 03:03:20.000000 CallingGPT-0.0.0.3/CallingGPT/CallingGPT.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       21 2023-06-18 03:03:20.000000 CallingGPT-0.0.0.3/CallingGPT/CallingGPT.egg-info/top_level.txt
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-18 03:03:20.115381 CallingGPT-0.0.0.3/CallingGPT/cli/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1062 2023-06-18 03:02:45.000000 CallingGPT-0.0.0.3/CallingGPT/cli/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-18 03:03:20.115381 CallingGPT-0.0.0.3/CallingGPT/entities/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-17 06:09:28.000000 CallingGPT-0.0.0.3/CallingGPT/entities/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4420 2023-06-17 08:49:00.000000 CallingGPT-0.0.0.3/CallingGPT/entities/namespace.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-18 03:03:20.119381 CallingGPT-0.0.0.3/CallingGPT/session/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-17 07:58:52.000000 CallingGPT-0.0.0.3/CallingGPT/session/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2287 2023-06-18 02:57:27.000000 CallingGPT-0.0.0.3/CallingGPT/session/session.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3506 2023-06-18 03:03:20.119381 CallingGPT-0.0.0.3/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3102 2023-06-18 03:02:22.000000 CallingGPT-0.0.0.3/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-06-18 03:03:20.119381 CallingGPT-0.0.0.3/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      748 2023-06-18 03:03:07.000000 CallingGPT-0.0.0.3/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-20 02:23:47.560138 CallingGPT-0.0.0.4/
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-20 02:23:47.560138 CallingGPT-0.0.0.4/CallingGPT/
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-20 02:23:47.560138 CallingGPT-0.0.0.4/CallingGPT/CallingGPT.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4491 2023-06-20 02:23:47.000000 CallingGPT-0.0.0.4/CallingGPT/CallingGPT.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      395 2023-06-20 02:23:47.000000 CallingGPT-0.0.0.4/CallingGPT/CallingGPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-20 02:23:47.000000 CallingGPT-0.0.0.4/CallingGPT/CallingGPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        7 2023-06-20 02:23:47.000000 CallingGPT-0.0.0.4/CallingGPT/CallingGPT.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       21 2023-06-20 02:23:47.000000 CallingGPT-0.0.0.4/CallingGPT/CallingGPT.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-20 02:23:47.560138 CallingGPT-0.0.0.4/CallingGPT/cli/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1062 2023-06-20 01:46:25.000000 CallingGPT-0.0.0.4/CallingGPT/cli/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-20 02:23:47.560138 CallingGPT-0.0.0.4/CallingGPT/entities/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-17 06:09:28.000000 CallingGPT-0.0.0.4/CallingGPT/entities/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5481 2023-06-20 02:23:14.000000 CallingGPT-0.0.0.4/CallingGPT/entities/namespace.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-20 02:23:47.560138 CallingGPT-0.0.0.4/CallingGPT/session/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-17 07:58:52.000000 CallingGPT-0.0.0.4/CallingGPT/session/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2287 2023-06-18 02:57:27.000000 CallingGPT-0.0.0.4/CallingGPT/session/session.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4491 2023-06-20 02:23:47.560138 CallingGPT-0.0.0.4/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4087 2023-06-18 14:38:18.000000 CallingGPT-0.0.0.4/README.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-06-20 02:23:47.564138 CallingGPT-0.0.0.4/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      748 2023-06-20 02:23:21.000000 CallingGPT-0.0.0.4/setup.py
```

### Comparing `CallingGPT-0.0.0.3/CallingGPT/CallingGPT.egg-info/PKG-INFO` & `CallingGPT-0.0.0.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: CallingGPT
-Version: 0.0.0.3
-Summary: GPT's function calling feature wrapper
-Home-page: https://github.com/RockChinQ/CallingGPT
-Author: RockChinQ
-Author-email: 1010553892@qq.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-
 # CallingGPT
 
 [![PyPi](https://img.shields.io/pypi/v/CallingGPT.svg)](https://pypi.python.org/pypi/CallingGPT)
 
 GPT's Function Calling Demo, a experiment of self-hosted ChatGPT-Plugins-like platform.
 
 > Recommend reading: [function-calling](https://platform.openai.com/docs/guides/gpt/function-calling)
@@ -44,15 +32,15 @@
 
     ```bash
     python main.py <module0> <module1> ...
     ```
 
 ## Example
 
-Use the `example/greet.py`
+Use the `example/greet.py`, provides a `greet` function called when user ask GPT to greet someone.
 
 ```bash
 python main.py example/greet.py
 ```
 
 Then you can talk to the bot.
 
@@ -66,14 +54,42 @@
 >>> and to Alice
 func<examples.greet.greet>: Hello, Alice!
 >>> 
 ```
 
 Type `help` to get help.
 
+### Other Examples
+
+<details>
+<summary>examples/draw.py</summary>
+
+Provides a `dalle_draw` function to use DALL·E model when user ask GPT to draw something.
+
+```bash
+python main.py examples/draw.py
+```
+
+```
+$ python main.py examples/draw.py 
+Using module: examples.draw
+>>> draw cars heading home under the sunset
+func<examples.draw.dalle_draw>: {
+  "created": 1687098971,
+  "data": [
+    {
+      "url": "https://oaidalleapiprodscus.blob.core.windows.net/private/org-VS9HEpJba78GXVfOcmVo7qaM/user-OHa7Jo3kL4XJDg9lo7AzdWNT/img-eAwt4YgHn6ed1cr96MoRWs0d.png?st=2023-06-18T13%3A36%3A11Z&se=2023-06-18T15%3A36%3A11Z&sp=r&sv=2021-08-06&sr=b&rscd=inline&rsct=image/png&skoid=6aaadede-4fb3-4698-a8f6-684d7786b067&sktid=a48cca56-e6da-484e-a814-9c849652bcb3&skt=2023-06-17T20%3A54%3A10Z&ske=2023-06-18T20%3A54%3A10Z&sks=b&skv=2021-08-06&sig=ZY4DTE1fYPyT7/jYBLJLuAgxpNuPsOhjbid1CWTyfKo%3D"
+    }
+  ]
+}
+>>>
+```
+
+</details>
+
 ## For Code
 
 1. Install the package
 
     ```bash
     pip install --upgrade CallingGPT
     ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `CallingGPT-0.0.0.3/CallingGPT/cli/__init__.py` & `CallingGPT-0.0.0.4/CallingGPT/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `CallingGPT-0.0.0.3/CallingGPT/entities/namespace.py` & `CallingGPT-0.0.0.4/CallingGPT/entities/namespace.py`

 * *Files 27% similar despite different names*

```diff
@@ -64,18 +64,17 @@
                 desc = doc_spt[0]
                 args = doc_spt[1] if len(doc_spt) > 1 else ""
                 returns = doc_spt[2] if len(doc_spt) > 2 else ""
 
                 # extract args
                 # delete the first line of args
                 arg_lines = args.split('\n')[1:]
-                arg_doc_list = re.findall(r'(\w+)(\((\w+)\))?:\s*(.*)', args)
                 args_doc = {}
                 for arg_line in arg_lines:
-                    doc_tuple = re.findall(r'(\w+)(\((\w+)\))?:\s*(.*)', arg_line)
+                    doc_tuple = re.findall(r'(\w+)(\(([\w\[\]]+)\))?:\s*(.*)', arg_line)
                     if len(doc_tuple) == 0:
                         continue
                     args_doc[doc_tuple[0][0]] = doc_tuple[0][3]
 
                 # extract returns
                 return_doc_list = re.findall(r'(\w+):\s*(.*)', returns)
 
@@ -85,20 +84,50 @@
                     "required": [],
                     "properties": {},
                 }
 
 
                 for i, param in params:
                     param_type = param.annotation.__name__
-                    if param_type == "str":
-                        param_type = "string"
+
+                    type_name_mapping = {
+                        "str": "string",
+                        "int": "integer",
+                        "float": "number",
+                        "bool": "boolean",
+                        "list": "array",
+                        "dict": "object",
+                    }
+
+                    if param_type in type_name_mapping:
+                        param_type = type_name_mapping[param_type]
+
                     parameters['properties'][param.name] = {
                         "type": param_type,
                         "description": args_doc[param.name],
                     }
+
+                    # add schema for array
+                    if param_type == "array":
+                        # extract type of array, the int of list[int]
+                        # use re
+                        array_type_tuple = re.findall(r'list\[(\w+)\]', str(param.annotation))
+
+                        array_type = 'string'
+
+                        if len(array_type_tuple) > 0:
+                            array_type = array_type_tuple[0]
+                        
+                        if array_type in type_name_mapping:
+                            array_type = type_name_mapping[array_type]
+                        
+                        parameters['properties'][param.name]["items"] = {
+                            "type": array_type,
+                        }
+
                     if param.default is inspect.Parameter.empty:
                         parameters["required"].append(param.name)
 
                 funtion_dict = {
                     "function": function,
                     "description": desc,
                     "parameters": parameters,
```

### Comparing `CallingGPT-0.0.0.3/CallingGPT/session/session.py` & `CallingGPT-0.0.0.4/CallingGPT/session/session.py`

 * *Files identical despite different names*

### Comparing `CallingGPT-0.0.0.3/PKG-INFO` & `CallingGPT-0.0.0.4/CallingGPT/CallingGPT.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CallingGPT
-Version: 0.0.0.3
+Version: 0.0.0.4
 Summary: GPT's function calling feature wrapper
 Home-page: https://github.com/RockChinQ/CallingGPT
 Author: RockChinQ
 Author-email: 1010553892@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -44,15 +44,15 @@
 
     ```bash
     python main.py <module0> <module1> ...
     ```
 
 ## Example
 
-Use the `example/greet.py`
+Use the `example/greet.py`, provides a `greet` function called when user ask GPT to greet someone.
 
 ```bash
 python main.py example/greet.py
 ```
 
 Then you can talk to the bot.
 
@@ -66,14 +66,42 @@
 >>> and to Alice
 func<examples.greet.greet>: Hello, Alice!
 >>> 
 ```
 
 Type `help` to get help.
 
+### Other Examples
+
+<details>
+<summary>examples/draw.py</summary>
+
+Provides a `dalle_draw` function to use DALL·E model when user ask GPT to draw something.
+
+```bash
+python main.py examples/draw.py
+```
+
+```
+$ python main.py examples/draw.py 
+Using module: examples.draw
+>>> draw cars heading home under the sunset
+func<examples.draw.dalle_draw>: {
+  "created": 1687098971,
+  "data": [
+    {
+      "url": "https://oaidalleapiprodscus.blob.core.windows.net/private/org-VS9HEpJba78GXVfOcmVo7qaM/user-OHa7Jo3kL4XJDg9lo7AzdWNT/img-eAwt4YgHn6ed1cr96MoRWs0d.png?st=2023-06-18T13%3A36%3A11Z&se=2023-06-18T15%3A36%3A11Z&sp=r&sv=2021-08-06&sr=b&rscd=inline&rsct=image/png&skoid=6aaadede-4fb3-4698-a8f6-684d7786b067&sktid=a48cca56-e6da-484e-a814-9c849652bcb3&skt=2023-06-17T20%3A54%3A10Z&ske=2023-06-18T20%3A54%3A10Z&sks=b&skv=2021-08-06&sig=ZY4DTE1fYPyT7/jYBLJLuAgxpNuPsOhjbid1CWTyfKo%3D"
+    }
+  ]
+}
+>>>
+```
+
+</details>
+
 ## For Code
 
 1. Install the package
 
     ```bash
     pip install --upgrade CallingGPT
     ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `CallingGPT-0.0.0.3/setup.py` & `CallingGPT-0.0.0.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='CallingGPT',
-    version='0.0.0.3',
+    version='0.0.0.4',
     description="GPT's function calling feature wrapper",
     long_description=open('README.md', encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     install_requires=[
         'openai',
     ],
     author='RockChinQ',
```

