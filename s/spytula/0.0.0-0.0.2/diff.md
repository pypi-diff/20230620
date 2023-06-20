# Comparing `tmp/spytula-0.0.0.tar.gz` & `tmp/spytula-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spytula-0.0.0.tar", max compression
+gzip compressed data, was "spytula-0.0.2.tar", max compression
```

## Comparing `spytula-0.0.0.tar` & `spytula-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1098 2023-06-19 17:27:58.711484 spytula-0.0.0/LICENSE.md
--rw-r--r--   0        0        0     2002 2023-06-19 16:47:52.837649 spytula-0.0.0/README.md
--rw-r--r--   0        0        0      559 2023-06-19 15:39:47.170551 spytula-0.0.0/pyproject.toml
--rw-r--r--   0        0        0      612 2023-06-19 17:12:08.480775 spytula-0.0.0/spytula/__init__.py
--rw-r--r--   0        0        0     9615 2023-06-19 16:31:36.058313 spytula-0.0.0/spytula/builder.py
--rw-r--r--   0        0        0     2729 2023-06-19 14:28:49.348514 spytula-0.0.0/spytula/mixins/format.py
--rw-r--r--   0        0        0     2755 1970-01-01 00:00:00.000000 spytula-0.0.0/setup.py
--rw-r--r--   0        0        0     2502 1970-01-01 00:00:00.000000 spytula-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1098 2023-06-19 17:27:58.711484 spytula-0.0.2/LICENSE.md
+-rw-r--r--   0        0        0     2247 2023-06-19 17:59:50.101503 spytula-0.0.2/README.md
+-rw-r--r--   0        0        0     1100 2023-06-20 08:52:03.554832 spytula-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-06-20 08:51:43.346685 spytula-0.0.2/spytula/__init__.py
+-rw-r--r--   0        0        0     9615 2023-06-19 16:31:36.058313 spytula-0.0.2/spytula/builder.py
+-rw-r--r--   0        0        0     2729 2023-06-19 14:28:49.348514 spytula-0.0.2/spytula/mixins/format.py
+-rw-r--r--   0        0        0     3163 1970-01-01 00:00:00.000000 spytula-0.0.2/setup.py
+-rw-r--r--   0        0        0     3302 1970-01-01 00:00:00.000000 spytula-0.0.2/PKG-INFO
```

### Comparing `spytula-0.0.0/LICENSE.md` & `spytula-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `spytula-0.0.0/README.md` & `spytula-0.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Spytula
+# 👩‍🍳 Spytula [![](https://img.shields.io/github/actions/workflow/status/pirhoo/spytula/main.yml)](https://github.com/pirhoo/spytula/actions)
 
 Spytula is a Python library that provides a simple and convenient way to build JSON and YAML data structures using a builder pattern.
 
 ## Installation
 
 Use pip to install the Spytula library:
 
@@ -63,7 +63,11 @@
         "Bamboo Shoots"
     ]
 }
 
 ```
 
 In this example, we create a `SpytulaBuilder` instance and add attributes like name and origin to represent `Ramen`. We use the `nodes()` context manager to create a list of ingredients and add them to the JSON structure. Optional attributes like spiciness and toppings are added conditionally using the `when()` method. Finally, we convert the JSON structure to a JSON-formatted string using `to_json()` with an indentation of 4 spaces.
+
+## Documentation    
+
+Refer for the [documentation](https://pirhoo.github.io/spytula/) for more details.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `spytula-0.0.0/spytula/builder.py` & `spytula-0.0.2/spytula/builder.py`

 * *Files identical despite different names*

### Comparing `spytula-0.0.0/spytula/mixins/format.py` & `spytula-0.0.2/spytula/mixins/format.py`

 * *Files identical despite different names*

### Comparing `spytula-0.0.0/setup.py` & `spytula-0.0.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 {'': ['*']}
 
 install_requires = \
 ['inflection>=0.5.1,<0.6.0', 'pytest>=7.3.2,<8.0.0', 'pyyaml>=6.0,<7.0']
 
 setup_kwargs = {
     'name': 'spytula',
-    'version': '0.0.0',
-    'description': '',
-    'long_description': '# Spytula\n\nSpytula is a Python library that provides a simple and convenient way to build JSON and YAML data structures using a builder pattern.\n\n## Installation\n\nUse pip to install the Spytula library:\n\n```bash\npip install spytula\n```\n\n## Usage    \n\nImport the `SpytulaBuilder` class from the `spytula.builder` module:\n\n```python\nfrom spytula.builder import SpytulaBuilder\n\n# Create an instance of SpytulaBuilder\nbuilder = SpytulaBuilder()\n\n# Add attributes to the JSON structure\nbuilder.attribute(\'name\', \'Ramen\')\nbuilder.attribute(\'origin\', \'Japan\')\n\n# Create a list of ingredients\nfor builder.each(\'ingredients\') as add_ingredient:    \n    for ingredient in [\'Noodles\', \'Pork\', \'Eggs\', \'Miso\']:\n        with add_ingredient() as ingredient_builder:\n            ingredient_builder.attribute(\'name\', ingredient)\n\n# Add optional attributes conditionally\nbuilder.when(\'spiciness\', \'Medium\', True)\nbuilder.when(\'extra_toppings\', [\'Green Onions\', \'Nori\', \'Bamboo Shoots\'], True)\n\n# Configure the key to use camelcase\nbuilder.key_format(camelize={\'uppercase_first_letter\': False})\n\n# Convert the JSON structure to JSON-formatted string\njson_output = builder.to_json(indent=4)\n\n# Print the JSON output\nprint(json_output)\n```\n\nThis will output:\n\n```json\n{\n    "name": "Ramen",\n    "origin": "Japan",\n    "ingredients": [\n        { "name": "Noodles" },\n        { "name": "Pork" },\n        { "name": "Eggs" },\n        { "name": "Miso" }\n    ],\n    "spiciness": "Medium",\n    "extraToppings": [\n        "Green Onions",\n        "Nori",\n        "Bamboo Shoots"\n    ]\n}\n\n```\n\nIn this example, we create a `SpytulaBuilder` instance and add attributes like name and origin to represent `Ramen`. We use the `nodes()` context manager to create a list of ingredients and add them to the JSON structure. Optional attributes like spiciness and toppings are added conditionally using the `when()` method. Finally, we convert the JSON structure to a JSON-formatted string using `to_json()` with an indentation of 4 spaces.\n',
-    'author': 'ICIJ',
-    'author_email': 'engineering@icij.org',
+    'version': '0.0.2',
+    'description': 'A Python library that provides a simple and convenient way to build JSON and YAML data structures using a builder pattern.',
+    'long_description': '# 👩\u200d🍳 Spytula [![](https://img.shields.io/github/actions/workflow/status/pirhoo/spytula/main.yml)](https://github.com/pirhoo/spytula/actions)\n\nSpytula is a Python library that provides a simple and convenient way to build JSON and YAML data structures using a builder pattern.\n\n## Installation\n\nUse pip to install the Spytula library:\n\n```bash\npip install spytula\n```\n\n## Usage    \n\nImport the `SpytulaBuilder` class from the `spytula.builder` module:\n\n```python\nfrom spytula.builder import SpytulaBuilder\n\n# Create an instance of SpytulaBuilder\nbuilder = SpytulaBuilder()\n\n# Add attributes to the JSON structure\nbuilder.attribute(\'name\', \'Ramen\')\nbuilder.attribute(\'origin\', \'Japan\')\n\n# Create a list of ingredients\nfor builder.each(\'ingredients\') as add_ingredient:    \n    for ingredient in [\'Noodles\', \'Pork\', \'Eggs\', \'Miso\']:\n        with add_ingredient() as ingredient_builder:\n            ingredient_builder.attribute(\'name\', ingredient)\n\n# Add optional attributes conditionally\nbuilder.when(\'spiciness\', \'Medium\', True)\nbuilder.when(\'extra_toppings\', [\'Green Onions\', \'Nori\', \'Bamboo Shoots\'], True)\n\n# Configure the key to use camelcase\nbuilder.key_format(camelize={\'uppercase_first_letter\': False})\n\n# Convert the JSON structure to JSON-formatted string\njson_output = builder.to_json(indent=4)\n\n# Print the JSON output\nprint(json_output)\n```\n\nThis will output:\n\n```json\n{\n    "name": "Ramen",\n    "origin": "Japan",\n    "ingredients": [\n        { "name": "Noodles" },\n        { "name": "Pork" },\n        { "name": "Eggs" },\n        { "name": "Miso" }\n    ],\n    "spiciness": "Medium",\n    "extraToppings": [\n        "Green Onions",\n        "Nori",\n        "Bamboo Shoots"\n    ]\n}\n\n```\n\nIn this example, we create a `SpytulaBuilder` instance and add attributes like name and origin to represent `Ramen`. We use the `nodes()` context manager to create a list of ingredients and add them to the JSON structure. Optional attributes like spiciness and toppings are added conditionally using the `when()` method. Finally, we convert the JSON structure to a JSON-formatted string using `to_json()` with an indentation of 4 spaces.\n\n## Documentation    \n\nRefer for the [documentation](https://pirhoo.github.io/spytula/) for more details.',
+    'author': 'Pierre Romera',
+    'author_email': 'hello@pirhoo.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'None',
+    'url': 'https://github.com/pirhoo/spytula/',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.8.1,<4.0.0',
 }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `spytula-0.0.0/PKG-INFO` & `spytula-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,33 @@
 Metadata-Version: 2.1
 Name: spytula
-Version: 0.0.0
-Summary: 
-Author: ICIJ
-Author-email: engineering@icij.org
+Version: 0.0.2
+Summary: A Python library that provides a simple and convenient way to build JSON and YAML data structures using a builder pattern.
+Home-page: https://github.com/pirhoo/spytula/
+License: MIT
+Keywords: JSON,YAML,DSL
+Author: Pierre Romera
+Author-email: hello@pirhoo.com
 Requires-Python: >=3.8.1,<4.0.0
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: File Formats :: JSON
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: inflection (>=0.5.1,<0.6.0)
 Requires-Dist: pytest (>=7.3.2,<8.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
+Project-URL: Documentation, https://pirhoo.github.io/spytula/
+Project-URL: Repository, https://github.com/pirhoo/spytula/
 Description-Content-Type: text/markdown
 
-# Spytula
+# 👩‍🍳 Spytula [![](https://img.shields.io/github/actions/workflow/status/pirhoo/spytula/main.yml)](https://github.com/pirhoo/spytula/actions)
 
 Spytula is a Python library that provides a simple and convenient way to build JSON and YAML data structures using a builder pattern.
 
 ## Installation
 
 Use pip to install the Spytula library:
 
@@ -80,7 +89,10 @@
     ]
 }
 
 ```
 
 In this example, we create a `SpytulaBuilder` instance and add attributes like name and origin to represent `Ramen`. We use the `nodes()` context manager to create a list of ingredients and add them to the JSON structure. Optional attributes like spiciness and toppings are added conditionally using the `when()` method. Finally, we convert the JSON structure to a JSON-formatted string using `to_json()` with an indentation of 4 spaces.
 
+## Documentation    
+
+Refer for the [documentation](https://pirhoo.github.io/spytula/) for more details.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

