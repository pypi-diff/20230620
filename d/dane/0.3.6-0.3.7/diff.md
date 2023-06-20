# Comparing `tmp/dane-0.3.6.tar.gz` & `tmp/dane-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dane-0.3.6.tar", max compression
+gzip compressed data, was "dane-0.3.7.tar", max compression
```

## Comparing `dane-0.3.6.tar` & `dane-0.3.7.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0    11357 2022-12-20 11:50:37.871142 dane-0.3.6/LICENSE
--rw-r--r--   0        0        0     2362 2022-12-20 11:50:37.871142 dane-0.3.6/README.md
--rw-r--r--   0        0        0      245 2023-06-16 12:16:26.319234 dane-0.3.6/dane/__init__.py
--rw-r--r--   0        0        0    14243 2023-06-16 12:31:16.095021 dane-0.3.6/dane/base_classes.py
--rw-r--r--   0        0        0     3891 2022-12-20 11:50:37.871142 dane-0.3.6/dane/config.py
--rw-r--r--   0        0        0     5679 2022-12-20 11:50:37.871142 dane-0.3.6/dane/document.py
--rw-r--r--   0        0        0     2187 2022-12-20 11:50:37.871142 dane-0.3.6/dane/errors.py
--rw-r--r--   0        0        0     4858 2023-06-16 12:16:26.319234 dane-0.3.6/dane/es_queries.py
--rw-r--r--   0        0        0    39686 2023-06-16 12:34:35.399932 dane-0.3.6/dane/handlers/ESHandler.py
--rw-r--r--   0        0        0     4335 2023-06-16 12:16:26.319234 dane-0.3.6/dane/handlers/RabbitMQHandler.py
--rw-r--r--   0        0        0      213 2022-12-20 11:50:37.871142 dane-0.3.6/dane/handlers/__init__.py
--rw-r--r--   0        0        0     9821 2023-06-16 12:16:26.319234 dane-0.3.6/dane/handlers/base_handler.py
--rw-r--r--   0        0        0     3770 2022-12-20 11:50:37.871142 dane-0.3.6/dane/results.py
--rw-r--r--   0        0        0     1384 2023-06-16 12:16:26.319234 dane-0.3.6/dane/state.py
--rw-r--r--   0        0        0     9860 2023-06-16 12:16:26.319234 dane-0.3.6/dane/tasks.py
--rw-r--r--   0        0        0     1357 2022-12-20 11:50:37.871142 dane-0.3.6/dane/utils.py
--rw-r--r--   0        0        0     1804 2023-06-16 12:16:26.319234 dane-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     3265 1970-01-01 00:00:00.000000 dane-0.3.6/setup.py
--rw-r--r--   0        0        0     3531 1970-01-01 00:00:00.000000 dane-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-12-20 11:50:37.871142 dane-0.3.7/LICENSE
+-rw-r--r--   0        0        0     2362 2022-12-20 11:50:37.871142 dane-0.3.7/README.md
+-rw-r--r--   0        0        0      245 2023-06-19 12:18:27.536564 dane-0.3.7/dane/__init__.py
+-rw-r--r--   0        0        0    14243 2023-06-19 12:18:27.536564 dane-0.3.7/dane/base_classes.py
+-rw-r--r--   0        0        0     4478 2023-06-19 14:20:12.773557 dane-0.3.7/dane/config.py
+-rw-r--r--   0        0        0     5679 2022-12-20 11:50:37.871142 dane-0.3.7/dane/document.py
+-rw-r--r--   0        0        0     2187 2022-12-20 11:50:37.871142 dane-0.3.7/dane/errors.py
+-rw-r--r--   0        0        0     4858 2023-06-19 12:18:27.536564 dane-0.3.7/dane/es_queries.py
+-rw-r--r--   0        0        0    39686 2023-06-19 12:18:27.536564 dane-0.3.7/dane/handlers/ESHandler.py
+-rw-r--r--   0        0        0     4335 2023-06-19 12:18:27.536564 dane-0.3.7/dane/handlers/RabbitMQHandler.py
+-rw-r--r--   0        0        0      213 2022-12-20 11:50:37.871142 dane-0.3.7/dane/handlers/__init__.py
+-rw-r--r--   0        0        0     9821 2023-06-19 12:18:27.536564 dane-0.3.7/dane/handlers/base_handler.py
+-rw-r--r--   0        0        0     3770 2022-12-20 11:50:37.871142 dane-0.3.7/dane/results.py
+-rw-r--r--   0        0        0     1883 2023-06-19 14:20:12.773557 dane-0.3.7/dane/s3_util.py
+-rw-r--r--   0        0        0     1384 2023-06-19 12:18:27.536564 dane-0.3.7/dane/state.py
+-rw-r--r--   0        0        0     9860 2023-06-19 12:18:27.536564 dane-0.3.7/dane/tasks.py
+-rw-r--r--   0        0        0     1357 2022-12-20 11:50:37.871142 dane-0.3.7/dane/utils.py
+-rw-r--r--   0        0        0     1836 2023-06-20 13:31:55.983683 dane-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0     3292 1970-01-01 00:00:00.000000 dane-0.3.7/setup.py
+-rw-r--r--   0        0        0     3572 1970-01-01 00:00:00.000000 dane-0.3.7/PKG-INFO
```

### Comparing `dane-0.3.6/LICENSE` & `dane-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dane-0.3.6/README.md` & `dane-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `dane-0.3.6/dane/base_classes.py` & `dane-0.3.7/dane/base_classes.py`

 * *Files identical despite different names*

### Comparing `dane-0.3.6/dane/config.py` & `dane-0.3.7/dane/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -70,14 +70,27 @@
 # If a base.config.yml sets this to true, then a config.yml is required
 cfg.CONFIG.REQUIRED = False
 
 cfg.PATHS = CN(new_allowed=True)
 cfg.PATHS.TEMP_FOLDER = "./TEMP"
 cfg.PATHS.OUT_FOLDER = "./OUT"
 
+# new settings block for how to deal with input
+cfg.INPUT = CN(new_allowed=True)
+cfg.INPUT.DELETE_ON_COMPLETION = False
+
+# new settings block for how to deal with output
+cfg.OUTPUT = CN(new_allowed=True)
+cfg.OUTPUT.DELETE_ON_COMPLETION = False  # delete output y/n
+cfg.OUTPUT.TRANSFER_ON_COMPLETION = False  # transfer output y/n
+# settings for transfer of output (currently S3 only)
+cfg.OUTPUT.S3_ENDPOINT_URL = None  # e.g. "http://s3-host:9000"
+cfg.OUTPUT.S3_BUCKET = None  # bucket reserved for 1 type of output
+cfg.OUTPUT.S3_FOLDER_IN_BUCKET = None  # folder/path within S3_BUCKET
+
 # Does the home dir have a config with additional param?
 # Add them. Or override defaults defined here
 if os.path.exists(os.path.join(cfg.DANE.HOME_DIR, "config.yml")):
     cfg.merge_from_file(os.path.join(cfg.DANE.HOME_DIR, "config.yml"))
 
 # Does the file that is importing this, have a base_config.yml in its dir?
 stack = [s for s in inspect.stack() if s.index is not None]
```

### Comparing `dane-0.3.6/dane/document.py` & `dane-0.3.7/dane/document.py`

 * *Files identical despite different names*

### Comparing `dane-0.3.6/dane/errors.py` & `dane-0.3.7/dane/errors.py`

 * *Files identical despite different names*

### Comparing `dane-0.3.6/dane/es_queries.py` & `dane-0.3.7/dane/es_queries.py`

 * *Files identical despite different names*

### Comparing `dane-0.3.6/dane/handlers/ESHandler.py` & `dane-0.3.7/dane/handlers/ESHandler.py`

 * *Files identical despite different names*

### Comparing `dane-0.3.6/dane/handlers/RabbitMQHandler.py` & `dane-0.3.7/dane/handlers/RabbitMQHandler.py`

 * *Files identical despite different names*

### Comparing `dane-0.3.6/dane/handlers/base_handler.py` & `dane-0.3.7/dane/handlers/base_handler.py`

 * *Files identical despite different names*

### Comparing `dane-0.3.6/dane/results.py` & `dane-0.3.7/dane/results.py`

 * *Files identical despite different names*

### Comparing `dane-0.3.6/dane/state.py` & `dane-0.3.7/dane/state.py`

 * *Files identical despite different names*

### Comparing `dane-0.3.6/dane/tasks.py` & `dane-0.3.7/dane/tasks.py`

 * *Files identical despite different names*

### Comparing `dane-0.3.6/dane/utils.py` & `dane-0.3.7/dane/utils.py`

 * *Files identical despite different names*

### Comparing `dane-0.3.6/pyproject.toml` & `dane-0.3.7/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "DANE"
-version = "0.3.6"
+version = "0.3.7"
 description = "Utils for working with the Distributed Annotation and Enrichment system"
 readme = "README.md"
 authors = [
     "Nanne van Noord <n.j.e.vannoord@uva.nl>",
     "jblom <jblom@beeldengeluid.nl>"
 ]
 license = "Apache License 2.0"
@@ -26,14 +26,15 @@
 [tool.poetry.dependencies]
 python = "^3.10"
 elasticsearch7 = "^7.17.7"
 pika = "^1.3.1"
 yacs = "^0.1.8"
 requests = "^2.28.1"
 urllib3 = "^1.26.12"
+boto3 = "^1.26.155"
 
 [tool.poetry.dev-dependencies]
 mockito = "^1.4.0"
 pytest = "^7.2.0"
 mypy = "^0.982"
 black = "^22.10.0"
 flake8 = "^5.0.4"
@@ -82,9 +83,10 @@
 [[tool.mypy.overrides]]
 module = [
   'dane.*',
   'mockito',
   'pika',
   'yaml',
   'yacs.*',
+  "boto3",
 ]
-ignore_missing_imports = true
+ignore_missing_imports = true
```

### Comparing `dane-0.3.6/setup.py` & `dane-0.3.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,24 @@
 packages = \
 ['dane', 'dane.handlers']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['elasticsearch7>=7.17.7,<8.0.0',
+['boto3>=1.26.155,<2.0.0',
+ 'elasticsearch7>=7.17.7,<8.0.0',
  'pika>=1.3.1,<2.0.0',
  'requests>=2.28.1,<3.0.0',
  'urllib3>=1.26.12,<2.0.0',
  'yacs>=0.1.8,<0.2.0']
 
 setup_kwargs = {
     'name': 'dane',
-    'version': '0.3.6',
+    'version': '0.3.7',
     'description': 'Utils for working with the Distributed Annotation and Enrichment system',
     'long_description': "# DANE\nThe Distributed Annotation 'n' Enrichment (DANE) system handles compute task assignment and file storage for the automatic annotation of content.\n\nThis repository contains contains the building blocks for with DANE, such as creating custom analysis workers or submitting new task.\n\n## Installation\n\nThis package can be installed through pip:\n\n    pip install dane\n\n### Configuration\n\nDANE components are configured through the dane.config module, which is described here: https://dane.readthedocs.io/en/latest/intro.html#configuration \nIt is however noteable that, because all DANE components are expected to rely on it, some of the DANE-server, ElasticSearch and RabbitMQ configuration \nare included in the default config. As such it is recommended that you create a `$HOME/.dane/config.yml` or `$DANE_HOME/config.yml` which contain machine-wide settings for how to connect to these services, which involves specifying the following settings:\n\n```\nDANE:\n    API_URL: 'http://localhost:5500/DANE/'\n    MANAGE_URL: 'http://localhost:5500/manage/'\nRABBITMQ:\n    HOST: 'localhost'\n    PORT: 5672\n    EXCHANGE: 'DANE-exchange'\n    RESPONSE_QUEUE: 'DANE-response-queue'\n    USER: 'guest'\n    PASSWORD: 'guest'\nELASTICSEARCH:\n    HOST: ['localhost']\n    PORT: 9200\n    USER: 'elastic'\n    PASSWORD: 'changeme'\n    SCHEME: 'http'\n    INDEX: 'your_dane_index'\n```\n\nThe values given here are the default values.\n\n### Usage\n\nExamples of how to use DANE can be found in the `examples/` directory.\n\n## Local Development\n\nWe moved from `setup.py` & `requirements.txt` to a single `pyproject.toml`. For local builds and publishing we use [poetry](https://python-poetry.org/).\n\nFor local installation:\n\n```bash\npoetry install\npoetry shell\n```\n\nAfter installation the following unit test should succeed:\n\n```bash\npython -m test.test_dane\n```\n\nTo build a wheel + source package (will end up in `dist` directory):\n\n```bash\npoetry build\n```\n\nThe wheel can be conveniently tested in e.g. your own DANE worker by installing it e.g. using `pip`:\n\n```bash\npip install path_to_dane_wheel_file\n```\n\nor with poetry\n\n```bash\npoetry add path_to_dane_wheel_file\n```\n\n### Breaking changes after 0.3.1 \n\nSince version 0.3.1 DANE must be imported in lowercase letters:\n\n```python\nimport dane\n```\n\nBefore version 0.3.1 you should import using uppercase letters:\n\n```python\nimport DANE\n```",
     'author': 'Nanne van Noord',
     'author_email': 'n.j.e.vannoord@uva.nl',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/CLARIAH/DANE',
```

### Comparing `dane-0.3.6/PKG-INFO` & `dane-0.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dane
-Version: 0.3.6
+Version: 0.3.7
 Summary: Utils for working with the Distributed Annotation and Enrichment system
 Home-page: https://github.com/CLARIAH/DANE
 License: Apache-2.0
 Author: Nanne van Noord
 Author-email: n.j.e.vannoord@uva.nl
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Video
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: boto3 (>=1.26.155,<2.0.0)
 Requires-Dist: elasticsearch7 (>=7.17.7,<8.0.0)
 Requires-Dist: pika (>=1.3.1,<2.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: urllib3 (>=1.26.12,<2.0.0)
 Requires-Dist: yacs (>=0.1.8,<0.2.0)
 Project-URL: Repository, https://github.com/CLARIAH/DANE
 Description-Content-Type: text/markdown
```

