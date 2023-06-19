# Comparing `tmp/prefecto-0.0.1.post0.tar.gz` & `tmp/prefecto-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefecto-0.0.1.post0.tar", last modified: Sat Jun 17 22:18:06 2023, max compression
+gzip compressed data, was "prefecto-0.0.2.tar", last modified: Mon Jun 19 23:14:41 2023, max compression
```

## Comparing `prefecto-0.0.1.post0.tar` & `prefecto-0.0.2.tar`

### file list

```diff
@@ -1,30 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:18:06.132142 prefecto-0.0.1.post0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-17 22:17:26.000000 prefecto-0.0.1.post0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-17 22:18:06.132142 prefecto-0.0.1.post0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-17 22:17:26.000000 prefecto-0.0.1.post0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-17 22:17:26.000000 prefecto-0.0.1.post0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-17 22:18:06.132142 prefecto-0.0.1.post0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-06-17 22:17:26.000000 prefecto-0.0.1.post0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:18:06.132142 prefecto-0.0.1.post0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:18:06.132142 prefecto-0.0.1.post0/src/prefecto/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-17 22:17:26.000000 prefecto-0.0.1.post0/src/prefecto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-17 22:18:06.132142 prefecto-0.0.1.post0/src/prefecto/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6994 2023-06-17 22:17:26.000000 prefecto-0.0.1.post0/src/prefecto/concurrency.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-17 22:17:26.000000 prefecto-0.0.1.post0/src/prefecto/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:18:06.132142 prefecto-0.0.1.post0/src/prefecto/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-17 22:17:26.000000 prefecto-0.0.1.post0/src/prefecto/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-06-17 22:17:26.000000 prefecto-0.0.1.post0/src/prefecto/serializers/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-06-17 22:17:26.000000 prefecto-0.0.1.post0/src/prefecto/serializers/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-06-17 22:17:26.000000 prefecto-0.0.1.post0/src/prefecto/serializers/polars.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-17 22:17:26.000000 prefecto-0.0.1.post0/src/prefecto/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:18:06.132142 prefecto-0.0.1.post0/src/prefecto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-17 22:18:06.000000 prefecto-0.0.1.post0/src/prefecto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-17 22:18:06.000000 prefecto-0.0.1.post0/src/prefecto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 22:18:06.000000 prefecto-0.0.1.post0/src/prefecto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-17 22:18:06.000000 prefecto-0.0.1.post0/src/prefecto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-17 22:18:06.000000 prefecto-0.0.1.post0/src/prefecto.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 22:17:32.000000 prefecto-0.0.1.post0/src/prefecto.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:18:06.132142 prefecto-0.0.1.post0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-17 22:17:26.000000 prefecto-0.0.1.post0/tests/test_concurrency.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-17 22:17:26.000000 prefecto-0.0.1.post0/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    83780 2023-06-17 22:17:26.000000 prefecto-0.0.1.post0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 23:14:41.784076 prefecto-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-19 23:13:55.000000 prefecto-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-06-19 23:14:41.784076 prefecto-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-19 23:13:55.000000 prefecto-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-19 23:13:55.000000 prefecto-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-19 23:14:41.784076 prefecto-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-06-19 23:13:55.000000 prefecto-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 23:14:41.780076 prefecto-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 23:14:41.784076 prefecto-0.0.2/src/prefecto/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-19 23:13:55.000000 prefecto-0.0.2/src/prefecto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-19 23:14:41.784076 prefecto-0.0.2/src/prefecto/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-06-19 23:13:55.000000 prefecto-0.0.2/src/prefecto/concurrency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-06-19 23:13:55.000000 prefecto-0.0.2/src/prefecto/filesystems.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-19 23:13:55.000000 prefecto-0.0.2/src/prefecto/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 23:14:41.780076 prefecto-0.0.2/src/prefecto/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-19 23:13:55.000000 prefecto-0.0.2/src/prefecto/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-06-19 23:13:55.000000 prefecto-0.0.2/src/prefecto/serializers/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-06-19 23:13:55.000000 prefecto-0.0.2/src/prefecto/serializers/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-06-19 23:13:55.000000 prefecto-0.0.2/src/prefecto/serializers/polars.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-19 23:13:55.000000 prefecto-0.0.2/src/prefecto/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 23:14:41.780076 prefecto-0.0.2/src/prefecto/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 23:13:55.000000 prefecto-0.0.2/src/prefecto/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-06-19 23:13:55.000000 prefecto-0.0.2/src/prefecto/testing/s3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 23:14:41.780076 prefecto-0.0.2/src/prefecto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-06-19 23:14:41.000000 prefecto-0.0.2/src/prefecto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-19 23:14:41.000000 prefecto-0.0.2/src/prefecto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 23:14:41.000000 prefecto-0.0.2/src/prefecto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-19 23:14:41.000000 prefecto-0.0.2/src/prefecto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-19 23:14:41.000000 prefecto-0.0.2/src/prefecto.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 23:14:02.000000 prefecto-0.0.2/src/prefecto.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 23:14:41.784076 prefecto-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-19 23:13:55.000000 prefecto-0.0.2/tests/test_concurrency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-19 23:13:55.000000 prefecto-0.0.2/tests/test_filesystems.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-19 23:13:55.000000 prefecto-0.0.2/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83780 2023-06-19 23:13:55.000000 prefecto-0.0.2/versioneer.py
```

### Comparing `prefecto-0.0.1.post0/LICENSE` & `prefecto-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `prefecto-0.0.1.post0/PKG-INFO` & `prefecto-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefecto
-Version: 0.0.1.post0
+Version: 0.0.2
 Summary: Prefect development aid.
 Home-page: https://github.com/dominictarro/prefecto
 Author: Dominic Tarro
 Author-email: dtarro@oxfordeconomics.com
 Project-URL: Documentation, https://dominictarro.github.io/prefecto/
 Project-URL: Source, https://github.com/dominictarro/prefecto
 Classifier: Natural Language :: English
@@ -19,20 +19,21 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: pandas
 Provides-Extra: polars
+Provides-Extra: moto
 License-File: LICENSE
 
 # Prefecto
 
 <p align="center">
-    <img src="./docs/assets/Monkeywrench-Data-Pipeline.png">
+    <img src="https://raw.githubusercontent.com/dominictarro/prefecto/main/docs/assets/Monkeywrench-Data-Pipeline.png">
     <br>
     <a href="https://pypi.python.org/pypi/prefecto/" alt="PyPI version">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/prefecto?color=fe7200&labelColor=eeeeee"></a>
     <a href="https://github.com/dominictarro/prefecto/" alt="Stars">
         <img src="https://img.shields.io/github/stars/dominictarro/prefecto?color=fe7200&labelColor=eeeeee" /></a>
     <a href="https://github.com/dominictarro/prefecto/pulse" alt="Activity">
         <img src="https://img.shields.io/github/commit-activity/m/dominictarro/prefecto?color=fe7200&labelColor=eeeeee" /></a>
```

#### html2text {}

```diff
@@ -1,22 +1,24 @@
-Metadata-Version: 2.1 Name: prefecto Version: 0.0.1.post0 Summary: Prefect
+Metadata-Version: 2.1 Name: prefecto Version: 0.0.2 Summary: Prefect
 development aid. Home-page: https://github.com/dominictarro/prefecto Author:
 Dominic Tarro Author-email: dtarro@oxfordeconomics.com Project-URL:
 Documentation, https://dominictarro.github.io/prefecto/ Project-URL: Source,
 https://github.com/dominictarro/prefecto Classifier: Natural Language ::
 English Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: System Administrators Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Topic :: Software Development :: Libraries Requires-
 Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra: dev
-Provides-Extra: pandas Provides-Extra: polars License-File: LICENSE # Prefecto
-                [./docs/assets/Monkeywrench-Data-Pipeline.png]
+Provides-Extra: pandas Provides-Extra: polars Provides-Extra: moto License-
+File: LICENSE # Prefecto
+  [https://raw.githubusercontent.com/dominictarro/prefecto/main/docs/assets/
+                       Monkeywrench-Data-Pipeline.png]
            [PyPI] [https://img.shields.io/github/stars/dominictarro/
 prefecto?color=fe7200&labelColor=eeeeee] [https://img.shields.io/github/commit-
        activity/m/dominictarro/prefecto?color=fe7200&labelColor=eeeeee]
 Prefecto is a collection of tools to extend and augment [Prefect](https://
 www.prefect.io/) capabilities. You can find the documentation [here](https://
 dominictarro.github.io/prefecto/). ## Getting Started Install Prefecto with
 ```bash pip install prefecto ``` *Prefecto is only tested with Python 3.10 and
```

### Comparing `prefecto-0.0.1.post0/README.md` & `prefecto-0.0.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Prefecto
 
 <p align="center">
-    <img src="./docs/assets/Monkeywrench-Data-Pipeline.png">
+    <img src="https://raw.githubusercontent.com/dominictarro/prefecto/main/docs/assets/Monkeywrench-Data-Pipeline.png">
     <br>
     <a href="https://pypi.python.org/pypi/prefecto/" alt="PyPI version">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/prefecto?color=fe7200&labelColor=eeeeee"></a>
     <a href="https://github.com/dominictarro/prefecto/" alt="Stars">
         <img src="https://img.shields.io/github/stars/dominictarro/prefecto?color=fe7200&labelColor=eeeeee" /></a>
     <a href="https://github.com/dominictarro/prefecto/pulse" alt="Activity">
         <img src="https://img.shields.io/github/commit-activity/m/dominictarro/prefecto?color=fe7200&labelColor=eeeeee" /></a>
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
 # Prefecto
-                [./docs/assets/Monkeywrench-Data-Pipeline.png]
+  [https://raw.githubusercontent.com/dominictarro/prefecto/main/docs/assets/
+                       Monkeywrench-Data-Pipeline.png]
            [PyPI] [https://img.shields.io/github/stars/dominictarro/
 prefecto?color=fe7200&labelColor=eeeeee] [https://img.shields.io/github/commit-
        activity/m/dominictarro/prefecto?color=fe7200&labelColor=eeeeee]
 Prefecto is a collection of tools to extend and augment [Prefect](https://
 www.prefect.io/) capabilities. You can find the documentation [here](https://
 dominictarro.github.io/prefecto/). ## Getting Started Install Prefecto with
 ```bash pip install prefecto ``` *Prefecto is only tested with Python 3.10 and
```

### Comparing `prefecto-0.0.1.post0/pyproject.toml` & `prefecto-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `prefecto-0.0.1.post0/setup.py` & `prefecto-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 
 pipfile = toml.load("Pipfile")
 
 packages = pipenv_to_requirements(pipfile["packages"])
 dev_packages = pipenv_to_requirements(pipfile["dev-packages"])
 pandas_packages = pipenv_to_requirements(pipfile["pandas"])
 polars_packages = pipenv_to_requirements(pipfile["polars"])
+moto_packages = pipenv_to_requirements(pipfile["moto"])
 
 setup(
     # Package metadata
     name="prefecto",
     description="Prefect development aid.",
     author="Dominic Tarro",
     author_email="dtarro@oxfordeconomics.com",
@@ -74,14 +75,15 @@
     # Requirements
     python_requires=">=3.7",
     install_requires=packages,
     extras_require={
         "dev": dev_packages,
         "pandas": pandas_packages,
         "polars": polars_packages,
+        "moto": moto_packages,
     },
     classifiers=[
         "Natural Language :: English",
         "Intended Audience :: Developers",
         "Intended Audience :: System Administrators",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3 :: Only",
```

### Comparing `prefecto-0.0.1.post0/src/prefecto/concurrency.py` & `prefecto-0.0.2/src/prefecto/concurrency.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Tools to improve Prefect concurrently.
+Tools to improve Prefect concurrency.
 
 """
 from __future__ import annotations
 
 from typing import Any, TypeVar
 
 from prefect.futures import PrefectFuture
```

### Comparing `prefecto-0.0.1.post0/src/prefecto/logging.py` & `prefecto-0.0.2/src/prefecto/logging.py`

 * *Files identical despite different names*

### Comparing `prefecto-0.0.1.post0/src/prefecto/serializers/core.py` & `prefecto-0.0.2/src/prefecto/serializers/core.py`

 * *Files identical despite different names*

### Comparing `prefecto-0.0.1.post0/src/prefecto/serializers/pandas.py` & `prefecto-0.0.2/src/prefecto/serializers/pandas.py`

 * *Files identical despite different names*

### Comparing `prefecto-0.0.1.post0/src/prefecto/serializers/polars.py` & `prefecto-0.0.2/src/prefecto/serializers/polars.py`

 * *Files identical despite different names*

### Comparing `prefecto-0.0.1.post0/src/prefecto/states.py` & `prefecto-0.0.2/src/prefecto/states.py`

 * *Files identical despite different names*

### Comparing `prefecto-0.0.1.post0/src/prefecto.egg-info/PKG-INFO` & `prefecto-0.0.2/src/prefecto.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefecto
-Version: 0.0.1.post0
+Version: 0.0.2
 Summary: Prefect development aid.
 Home-page: https://github.com/dominictarro/prefecto
 Author: Dominic Tarro
 Author-email: dtarro@oxfordeconomics.com
 Project-URL: Documentation, https://dominictarro.github.io/prefecto/
 Project-URL: Source, https://github.com/dominictarro/prefecto
 Classifier: Natural Language :: English
@@ -19,20 +19,21 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: pandas
 Provides-Extra: polars
+Provides-Extra: moto
 License-File: LICENSE
 
 # Prefecto
 
 <p align="center">
-    <img src="./docs/assets/Monkeywrench-Data-Pipeline.png">
+    <img src="https://raw.githubusercontent.com/dominictarro/prefecto/main/docs/assets/Monkeywrench-Data-Pipeline.png">
     <br>
     <a href="https://pypi.python.org/pypi/prefecto/" alt="PyPI version">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/prefecto?color=fe7200&labelColor=eeeeee"></a>
     <a href="https://github.com/dominictarro/prefecto/" alt="Stars">
         <img src="https://img.shields.io/github/stars/dominictarro/prefecto?color=fe7200&labelColor=eeeeee" /></a>
     <a href="https://github.com/dominictarro/prefecto/pulse" alt="Activity">
         <img src="https://img.shields.io/github/commit-activity/m/dominictarro/prefecto?color=fe7200&labelColor=eeeeee" /></a>
```

#### html2text {}

```diff
@@ -1,22 +1,24 @@
-Metadata-Version: 2.1 Name: prefecto Version: 0.0.1.post0 Summary: Prefect
+Metadata-Version: 2.1 Name: prefecto Version: 0.0.2 Summary: Prefect
 development aid. Home-page: https://github.com/dominictarro/prefecto Author:
 Dominic Tarro Author-email: dtarro@oxfordeconomics.com Project-URL:
 Documentation, https://dominictarro.github.io/prefecto/ Project-URL: Source,
 https://github.com/dominictarro/prefecto Classifier: Natural Language ::
 English Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: System Administrators Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Topic :: Software Development :: Libraries Requires-
 Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra: dev
-Provides-Extra: pandas Provides-Extra: polars License-File: LICENSE # Prefecto
-                [./docs/assets/Monkeywrench-Data-Pipeline.png]
+Provides-Extra: pandas Provides-Extra: polars Provides-Extra: moto License-
+File: LICENSE # Prefecto
+  [https://raw.githubusercontent.com/dominictarro/prefecto/main/docs/assets/
+                       Monkeywrench-Data-Pipeline.png]
            [PyPI] [https://img.shields.io/github/stars/dominictarro/
 prefecto?color=fe7200&labelColor=eeeeee] [https://img.shields.io/github/commit-
        activity/m/dominictarro/prefecto?color=fe7200&labelColor=eeeeee]
 Prefecto is a collection of tools to extend and augment [Prefect](https://
 www.prefect.io/) capabilities. You can find the documentation [here](https://
 dominictarro.github.io/prefecto/). ## Getting Started Install Prefecto with
 ```bash pip install prefecto ``` *Prefecto is only tested with Python 3.10 and
```

### Comparing `prefecto-0.0.1.post0/src/prefecto.egg-info/SOURCES.txt` & `prefecto-0.0.2/src/prefecto.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -3,21 +3,25 @@
 pyproject.toml
 setup.cfg
 setup.py
 versioneer.py
 src/prefecto/__init__.py
 src/prefecto/_version.py
 src/prefecto/concurrency.py
+src/prefecto/filesystems.py
 src/prefecto/logging.py
 src/prefecto/states.py
 src/prefecto.egg-info/PKG-INFO
 src/prefecto.egg-info/SOURCES.txt
 src/prefecto.egg-info/dependency_links.txt
 src/prefecto.egg-info/requires.txt
 src/prefecto.egg-info/top_level.txt
 src/prefecto.egg-info/zip-safe
 src/prefecto/serializers/__init__.py
 src/prefecto/serializers/core.py
 src/prefecto/serializers/pandas.py
 src/prefecto/serializers/polars.py
+src/prefecto/testing/__init__.py
+src/prefecto/testing/s3.py
 tests/test_concurrency.py
+tests/test_filesystems.py
 tests/test_logging.py
```

### Comparing `prefecto-0.0.1.post0/tests/test_concurrency.py` & `prefecto-0.0.2/tests/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `prefecto-0.0.1.post0/versioneer.py` & `prefecto-0.0.2/versioneer.py`

 * *Files identical despite different names*

