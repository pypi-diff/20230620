# Comparing `tmp/tomlize-0.1.1.tar.gz` & `tmp/tomlize-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tomlize-0.1.1.tar", last modified: Sat Apr 22 21:53:55 2023, max compression
+gzip compressed data, was "tomlize-0.2.0.tar", last modified: Tue Jun 20 10:46:00 2023, max compression
```

## Comparing `tomlize-0.1.1.tar` & `tomlize-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,27 @@
-drwxr-xr-x   0 mcorcherojim  (1000) mcorcherojim  (1000)        0 2023-04-22 21:53:55.472405 tomlize-0.1.1/
--rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)     1489 2023-04-22 21:53:55.472405 tomlize-0.1.1/PKG-INFO
--rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)      829 2023-04-22 21:52:21.000000 tomlize-0.1.1/README.md
--rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)      808 2023-04-22 21:53:45.000000 tomlize-0.1.1/pyproject.toml
--rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)       38 2023-04-22 21:53:55.472405 tomlize-0.1.1/setup.cfg
-drwxr-xr-x   0 mcorcherojim  (1000) mcorcherojim  (1000)        0 2023-04-22 21:53:55.462405 tomlize-0.1.1/src/
-drwxr-xr-x   0 mcorcherojim  (1000) mcorcherojim  (1000)        0 2023-04-22 21:53:55.462405 tomlize-0.1.1/src/tomlize/
--rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)       63 2023-04-19 11:25:03.000000 tomlize-0.1.1/src/tomlize/__init__.py
--rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)       62 2023-04-19 16:49:30.000000 tomlize-0.1.1/src/tomlize/__main__.py
--rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)      247 2023-04-19 16:51:24.000000 tomlize-0.1.1/src/tomlize/cli.py
--rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)      205 2023-04-19 20:42:21.000000 tomlize-0.1.1/src/tomlize/exceptions.py
-drwxr-xr-x   0 mcorcherojim  (1000) mcorcherojim  (1000)        0 2023-04-22 21:53:55.472405 tomlize-0.1.1/src/tomlize/loaders/
--rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)       54 2023-04-19 20:44:26.000000 tomlize-0.1.1/src/tomlize/loaders/__init__.py
--rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)     5577 2023-04-22 21:31:11.000000 tomlize-0.1.1/src/tomlize/loaders/setup_py.py
--rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)      617 2023-04-19 21:02:37.000000 tomlize-0.1.1/src/tomlize/main.py
-drwxr-xr-x   0 mcorcherojim  (1000) mcorcherojim  (1000)        0 2023-04-22 21:53:55.472405 tomlize-0.1.1/src/tomlize.egg-info/
--rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)     1489 2023-04-22 21:53:55.000000 tomlize-0.1.1/src/tomlize.egg-info/PKG-INFO
--rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)      375 2023-04-22 21:53:55.000000 tomlize-0.1.1/src/tomlize.egg-info/SOURCES.txt
--rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)        1 2023-04-22 21:53:55.000000 tomlize-0.1.1/src/tomlize.egg-info/dependency_links.txt
--rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)       17 2023-04-22 21:53:55.000000 tomlize-0.1.1/src/tomlize.egg-info/requires.txt
--rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)        8 2023-04-22 21:53:55.000000 tomlize-0.1.1/src/tomlize.egg-info/top_level.txt
+drwxr-xr-x   0 mcorcherojim  (1000) mcorcherojim  (1000)        0 2023-06-20 10:46:00.933693 tomlize-0.2.0/
+-rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)     1420 2023-06-20 10:46:00.933693 tomlize-0.2.0/PKG-INFO
+-rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)      760 2023-06-20 10:45:49.000000 tomlize-0.2.0/README.md
+-rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)      878 2023-06-20 10:45:49.000000 tomlize-0.2.0/pyproject.toml
+-rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)       38 2023-06-20 10:46:00.933693 tomlize-0.2.0/setup.cfg
+drwxr-xr-x   0 mcorcherojim  (1000) mcorcherojim  (1000)        0 2023-06-20 10:46:00.933693 tomlize-0.2.0/src/
+drwxr-xr-x   0 mcorcherojim  (1000) mcorcherojim  (1000)        0 2023-06-20 10:46:00.933693 tomlize-0.2.0/src/tomlize/
+-rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)       63 2023-05-07 14:32:30.000000 tomlize-0.2.0/src/tomlize/__init__.py
+-rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)       86 2023-05-23 19:27:58.000000 tomlize-0.2.0/src/tomlize/__main__.py
+-rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)      191 2023-05-23 19:31:43.000000 tomlize-0.2.0/src/tomlize/cli.py
+-rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)      507 2023-05-25 14:04:30.000000 tomlize-0.2.0/src/tomlize/converter.py
+-rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)      373 2023-05-25 15:24:16.000000 tomlize-0.2.0/src/tomlize/exceptions.py
+-rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)      840 2023-06-20 10:45:49.000000 tomlize-0.2.0/src/tomlize/main.py
+-rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)     1545 2023-05-25 17:49:08.000000 tomlize-0.2.0/src/tomlize/merger.py
+drwxr-xr-x   0 mcorcherojim  (1000) mcorcherojim  (1000)        0 2023-06-20 10:46:00.933693 tomlize-0.2.0/src/tomlize/setup_py/
+-rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)       56 2023-05-24 12:16:35.000000 tomlize-0.2.0/src/tomlize/setup_py/__init__.py
+-rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)     2916 2023-05-23 15:40:41.000000 tomlize-0.2.0/src/tomlize/setup_py/fields_mapping.py
+-rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)     1104 2023-05-24 13:12:26.000000 tomlize-0.2.0/src/tomlize/setup_py/reader.py
+-rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)     1948 2023-05-25 13:58:54.000000 tomlize-0.2.0/src/tomlize/setup_py/remover.py
+-rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)     2645 2023-05-25 13:41:40.000000 tomlize-0.2.0/src/tomlize/setup_py/transformer.py
+drwxr-xr-x   0 mcorcherojim  (1000) mcorcherojim  (1000)        0 2023-06-20 10:46:00.933693 tomlize-0.2.0/src/tomlize.egg-info/
+-rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)     1420 2023-06-20 10:46:00.000000 tomlize-0.2.0/src/tomlize.egg-info/PKG-INFO
+-rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)      567 2023-06-20 10:46:00.000000 tomlize-0.2.0/src/tomlize.egg-info/SOURCES.txt
+-rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)        1 2023-06-20 10:46:00.000000 tomlize-0.2.0/src/tomlize.egg-info/dependency_links.txt
+-rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)       46 2023-06-20 10:46:00.000000 tomlize-0.2.0/src/tomlize.egg-info/entry_points.txt
+-rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)       30 2023-06-20 10:46:00.000000 tomlize-0.2.0/src/tomlize.egg-info/requires.txt
+-rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)        8 2023-06-20 10:46:00.000000 tomlize-0.2.0/src/tomlize.egg-info/top_level.txt
```

### Comparing `tomlize-0.1.1/PKG-INFO` & `tomlize-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomlize
-Version: 0.1.1
+Version: 0.2.0
 Summary: Move all your configuration to pyproject.toml
 Author-email: Mario Corchero <mariocj89@gmail.com>
 Project-URL: Code, https://github.com/mariocj89/tomlize
 Project-URL: Issue tracker, https://github.com/mariocj89/tomlize/issues
 Project-URL: Download, https://pypi.org/project/tomlize/#files
 Keywords: pyproject,configuration,python,tool
 Classifier: Programming Language :: Python :: 3.8
@@ -21,26 +21,24 @@
 ![PyPI](https://img.shields.io/pypi/v/tomlize)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/tomlize)
 ![Code Style](https://img.shields.io/badge/code%20style-black,%20isort-000000.svg)
 
 Move the configuration of all your tools to `pyproject.toml`.
 
 ```
-$ python -m tomlize --help
-usage: __main__.py [-h] input_file [output_file]
+$ tomlize --help
+usage: tomlize [-h] input_file
 
 positional arguments:
   input_file
-  output_file
 
 options:
-  -h, --help   show this help message and exit
-
+  -h, --help  show this help message and exit
 ```
 
 The tool can be used to port the configuration from the following files:
 
 ## `setup.py`
 
 ```
-python -m tomlize setup.py pyproject.toml
+tomlize setup.py
 ```
```

### Comparing `tomlize-0.1.1/README.md` & `tomlize-0.2.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -5,26 +5,24 @@
 ![PyPI](https://img.shields.io/pypi/v/tomlize)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/tomlize)
 ![Code Style](https://img.shields.io/badge/code%20style-black,%20isort-000000.svg)
 
 Move the configuration of all your tools to `pyproject.toml`.
 
 ```
-$ python -m tomlize --help
-usage: __main__.py [-h] input_file [output_file]
+$ tomlize --help
+usage: tomlize [-h] input_file
 
 positional arguments:
   input_file
-  output_file
 
 options:
-  -h, --help   show this help message and exit
-
+  -h, --help  show this help message and exit
 ```
 
 The tool can be used to port the configuration from the following files:
 
 ## `setup.py`
 
 ```
-python -m tomlize setup.py pyproject.toml
+tomlize setup.py
 ```
```

### Comparing `tomlize-0.1.1/pyproject.toml` & `tomlize-0.2.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 [build-system]
 requires = ["setuptools>62"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tomlize"
-version = "0.1.1"
+version = "0.2.0"
 authors = [
     {name = "Mario Corchero", email = "mariocj89@gmail.com"},
 ]
 description = "Move all your configuration to pyproject.toml"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["pyproject", "configuration", "python", "tool"]
 classifiers = [
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
-    "toml",
+    "tomlkit",
     "coloredlogs",
+    "packaging",
 ]
 
 [project.urls]
 "Code" = "https://github.com/mariocj89/tomlize"
 "Issue tracker" = "https://github.com/mariocj89/tomlize/issues"
 "Download" = "https://pypi.org/project/tomlize/#files"
+
+[project.scripts]
+tomlize = "tomlize.main:main"
+
```

### Comparing `tomlize-0.1.1/src/tomlize.egg-info/PKG-INFO` & `tomlize-0.2.0/src/tomlize.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomlize
-Version: 0.1.1
+Version: 0.2.0
 Summary: Move all your configuration to pyproject.toml
 Author-email: Mario Corchero <mariocj89@gmail.com>
 Project-URL: Code, https://github.com/mariocj89/tomlize
 Project-URL: Issue tracker, https://github.com/mariocj89/tomlize/issues
 Project-URL: Download, https://pypi.org/project/tomlize/#files
 Keywords: pyproject,configuration,python,tool
 Classifier: Programming Language :: Python :: 3.8
@@ -21,26 +21,24 @@
 ![PyPI](https://img.shields.io/pypi/v/tomlize)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/tomlize)
 ![Code Style](https://img.shields.io/badge/code%20style-black,%20isort-000000.svg)
 
 Move the configuration of all your tools to `pyproject.toml`.
 
 ```
-$ python -m tomlize --help
-usage: __main__.py [-h] input_file [output_file]
+$ tomlize --help
+usage: tomlize [-h] input_file
 
 positional arguments:
   input_file
-  output_file
 
 options:
-  -h, --help   show this help message and exit
-
+  -h, --help  show this help message and exit
 ```
 
 The tool can be used to port the configuration from the following files:
 
 ## `setup.py`
 
 ```
-python -m tomlize setup.py pyproject.toml
+tomlize setup.py
 ```
```

