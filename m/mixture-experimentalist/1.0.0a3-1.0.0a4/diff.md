# Comparing `tmp/mixture_experimentalist-1.0.0a3.tar.gz` & `tmp/mixture_experimentalist-1.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mixture_experimentalist-1.0.0a3.tar", last modified: Tue Jun 20 16:00:46 2023, max compression
+gzip compressed data, was "mixture_experimentalist-1.0.0a4.tar", last modified: Tue Jun 20 17:48:41 2023, max compression
```

## Comparing `mixture_experimentalist-1.0.0a3.tar` & `mixture_experimentalist-1.0.0a4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-20 16:00:46.206083 mixture_experimentalist-1.0.0a3/
-drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-20 16:00:46.186544 mixture_experimentalist-1.0.0a3/.github/
-drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-20 16:00:46.192667 mixture_experimentalist-1.0.0a3/.github/workflows/
--rw-r--r--   0 marinadubova   (503) staff       (20)     1077 2023-05-24 16:20:27.000000 mixture_experimentalist-1.0.0a3/.github/workflows/python-publish.yml
--rw-r--r--   0 marinadubova   (503) staff       (20)      938 2023-05-24 16:20:27.000000 mixture_experimentalist-1.0.0a3/.gitignore
--rw-r--r--   0 marinadubova   (503) staff       (20)      674 2023-05-24 16:20:27.000000 mixture_experimentalist-1.0.0a3/.pre-commit-config.yaml
--rw-r--r--   0 marinadubova   (503) staff       (20)     1070 2023-05-24 16:18:58.000000 mixture_experimentalist-1.0.0a3/LICENSE
--rw-r--r--   0 marinadubova   (503) staff       (20)     2647 2023-06-20 16:00:46.205221 mixture_experimentalist-1.0.0a3/PKG-INFO
--rw-r--r--   0 marinadubova   (503) staff       (20)     1953 2023-06-20 15:59:05.000000 mixture_experimentalist-1.0.0a3/README.md
-drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-20 16:00:46.196805 mixture_experimentalist-1.0.0a3/docs/
--rw-r--r--   0 marinadubova   (503) staff       (20)   206355 2023-06-20 15:59:05.000000 mixture_experimentalist-1.0.0a3/docs/basic-usage.ipynb
--rw-r--r--   0 marinadubova   (503) staff       (20)      491 2023-06-19 13:11:31.000000 mixture_experimentalist-1.0.0a3/docs/index.md
-drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-20 16:00:46.197697 mixture_experimentalist-1.0.0a3/docs/javascripts/
--rw-r--r--   0 marinadubova   (503) staff       (20)      313 2023-05-24 16:20:27.000000 mixture_experimentalist-1.0.0a3/docs/javascripts/mathjax.js
--rw-r--r--   0 marinadubova   (503) staff       (20)      388 2023-06-20 15:59:05.000000 mixture_experimentalist-1.0.0a3/docs/quickstart.md
-drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-20 16:00:46.198557 mixture_experimentalist-1.0.0a3/mkdocs/
--rw-r--r--   0 marinadubova   (503) staff       (20)      729 2023-05-24 16:20:27.000000 mixture_experimentalist-1.0.0a3/mkdocs/base.yml
--rw-r--r--   0 marinadubova   (503) staff       (20)      384 2023-06-19 13:09:17.000000 mixture_experimentalist-1.0.0a3/mkdocs.yml
--rw-r--r--   0 marinadubova   (503) staff       (20)      973 2023-06-20 16:00:13.000000 mixture_experimentalist-1.0.0a3/pyproject.toml
--rw-r--r--   0 marinadubova   (503) staff       (20)       38 2023-06-20 16:00:46.206281 mixture_experimentalist-1.0.0a3/setup.cfg
-drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-20 16:00:46.188055 mixture_experimentalist-1.0.0a3/src/
-drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-20 16:00:46.187544 mixture_experimentalist-1.0.0a3/src/autora/
-drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-20 16:00:46.187667 mixture_experimentalist-1.0.0a3/src/autora/experimentalist/
-drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-20 16:00:46.187793 mixture_experimentalist-1.0.0a3/src/autora/experimentalist/sampler/
-drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-20 16:00:46.199409 mixture_experimentalist-1.0.0a3/src/autora/experimentalist/sampler/mixture/
--rw-r--r--   0 marinadubova   (503) staff       (20)     4273 2023-06-20 15:59:05.000000 mixture_experimentalist-1.0.0a3/src/autora/experimentalist/sampler/mixture/__init__.py
-drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-20 16:00:46.202546 mixture_experimentalist-1.0.0a3/src/mixture_experimentalist.egg-info/
--rw-r--r--   0 marinadubova   (503) staff       (20)     2647 2023-06-20 16:00:46.000000 mixture_experimentalist-1.0.0a3/src/mixture_experimentalist.egg-info/PKG-INFO
--rw-r--r--   0 marinadubova   (503) staff       (20)      596 2023-06-20 16:00:46.000000 mixture_experimentalist-1.0.0a3/src/mixture_experimentalist.egg-info/SOURCES.txt
--rw-r--r--   0 marinadubova   (503) staff       (20)        1 2023-06-20 16:00:46.000000 mixture_experimentalist-1.0.0a3/src/mixture_experimentalist.egg-info/dependency_links.txt
--rw-r--r--   0 marinadubova   (503) staff       (20)       49 2023-06-20 16:00:46.000000 mixture_experimentalist-1.0.0a3/src/mixture_experimentalist.egg-info/requires.txt
--rw-r--r--   0 marinadubova   (503) staff       (20)        7 2023-06-20 16:00:46.000000 mixture_experimentalist-1.0.0a3/src/mixture_experimentalist.egg-info/top_level.txt
-drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-20 16:00:46.204437 mixture_experimentalist-1.0.0a3/tests/
--rw-r--r--   0 marinadubova   (503) staff       (20)      841 2023-06-17 08:53:52.000000 mixture_experimentalist-1.0.0a3/tests/README.md
--rw-r--r--   0 marinadubova   (503) staff       (20)        0 2023-05-24 16:20:27.000000 mixture_experimentalist-1.0.0a3/tests/__init__.py
--rw-r--r--   0 marinadubova   (503) staff       (20)     1653 2023-06-20 15:59:05.000000 mixture_experimentalist-1.0.0a3/tests/test_mixture_experimentalist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:48:41.313573 mixture_experimentalist-1.0.0a4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:48:41.305573 mixture_experimentalist-1.0.0a4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:48:41.309573 mixture_experimentalist-1.0.0a4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-20 17:48:30.000000 mixture_experimentalist-1.0.0a4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-20 17:48:30.000000 mixture_experimentalist-1.0.0a4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-20 17:48:30.000000 mixture_experimentalist-1.0.0a4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-20 17:48:30.000000 mixture_experimentalist-1.0.0a4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-06-20 17:48:41.313573 mixture_experimentalist-1.0.0a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-06-20 17:48:30.000000 mixture_experimentalist-1.0.0a4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:48:41.309573 mixture_experimentalist-1.0.0a4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   206355 2023-06-20 17:48:30.000000 mixture_experimentalist-1.0.0a4/docs/basic-usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-20 17:48:30.000000 mixture_experimentalist-1.0.0a4/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:48:41.309573 mixture_experimentalist-1.0.0a4/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-20 17:48:30.000000 mixture_experimentalist-1.0.0a4/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-20 17:48:30.000000 mixture_experimentalist-1.0.0a4/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:48:41.309573 mixture_experimentalist-1.0.0a4/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-20 17:48:30.000000 mixture_experimentalist-1.0.0a4/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-20 17:48:30.000000 mixture_experimentalist-1.0.0a4/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-20 17:48:30.000000 mixture_experimentalist-1.0.0a4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 17:48:41.313573 mixture_experimentalist-1.0.0a4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:48:41.305573 mixture_experimentalist-1.0.0a4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:48:41.305573 mixture_experimentalist-1.0.0a4/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:48:41.305573 mixture_experimentalist-1.0.0a4/src/autora/experimentalist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:48:41.305573 mixture_experimentalist-1.0.0a4/src/autora/experimentalist/sampler/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:48:41.309573 mixture_experimentalist-1.0.0a4/src/autora/experimentalist/sampler/mixture/
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-06-20 17:48:30.000000 mixture_experimentalist-1.0.0a4/src/autora/experimentalist/sampler/mixture/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:48:41.309573 mixture_experimentalist-1.0.0a4/src/mixture_experimentalist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-06-20 17:48:41.000000 mixture_experimentalist-1.0.0a4/src/mixture_experimentalist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-20 17:48:41.000000 mixture_experimentalist-1.0.0a4/src/mixture_experimentalist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 17:48:41.000000 mixture_experimentalist-1.0.0a4/src/mixture_experimentalist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-20 17:48:41.000000 mixture_experimentalist-1.0.0a4/src/mixture_experimentalist.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 17:48:41.000000 mixture_experimentalist-1.0.0a4/src/mixture_experimentalist.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:48:41.313573 mixture_experimentalist-1.0.0a4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-20 17:48:30.000000 mixture_experimentalist-1.0.0a4/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 17:48:30.000000 mixture_experimentalist-1.0.0a4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-20 17:48:30.000000 mixture_experimentalist-1.0.0a4/tests/test_mixture_experimentalist.py
```

### Comparing `mixture_experimentalist-1.0.0a3/.github/workflows/python-publish.yml` & `mixture_experimentalist-1.0.0a4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `mixture_experimentalist-1.0.0a3/.gitignore` & `mixture_experimentalist-1.0.0a4/.gitignore`

 * *Files identical despite different names*

### Comparing `mixture_experimentalist-1.0.0a3/.pre-commit-config.yaml` & `mixture_experimentalist-1.0.0a4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mixture_experimentalist-1.0.0a3/LICENSE` & `mixture_experimentalist-1.0.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `mixture_experimentalist-1.0.0a3/PKG-INFO` & `mixture_experimentalist-1.0.0a4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mixture_experimentalist
-Version: 1.0.0a3
+Version: 1.0.0a4
 Summary: The goal of this project is to examine the performance of a mixture experimentalist–a hybrid of different experimental sampling strategies–in terms of its ability to recover a ground-truth model from synthetic data.
 Author-email: Marina Dubova <marina.dubova.97@gmail.com>
 License: MIT license
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/blinodelka/mixture_experimental_strategies
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
```

### Comparing `mixture_experimentalist-1.0.0a3/README.md` & `mixture_experimentalist-1.0.0a4/README.md`

 * *Files identical despite different names*

### Comparing `mixture_experimentalist-1.0.0a3/docs/basic-usage.ipynb` & `mixture_experimentalist-1.0.0a4/docs/basic-usage.ipynb`

 * *Files identical despite different names*

### Comparing `mixture_experimentalist-1.0.0a3/mkdocs/base.yml` & `mixture_experimentalist-1.0.0a4/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `mixture_experimentalist-1.0.0a3/pyproject.toml` & `mixture_experimentalist-1.0.0a4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 # UPDATE THIS BEFORE PUBLISHING
 name = "mixture_experimentalist"
 description = "The goal of this project is to examine the performance of a mixture experimentalist–a hybrid of different experimental sampling strategies–in terms of its ability to recover a ground-truth model from synthetic data."
 authors = [{ name = "Marina Dubova", email = "marina.dubova.97@gmail.com" }]
-version = "1.0.0a3"
+dynamic = ["version"]
 
 readme = "README.md"
 license = { text = "MIT license" }
 requires-python = ">=3.8,<4"
 
 # ADD NEW DEPENDENCIES HERE
 dependencies = [
```

### Comparing `mixture_experimentalist-1.0.0a3/src/autora/experimentalist/sampler/mixture/__init__.py` & `mixture_experimentalist-1.0.0a4/src/autora/experimentalist/sampler/mixture/__init__.py`

 * *Files identical despite different names*

### Comparing `mixture_experimentalist-1.0.0a3/src/mixture_experimentalist.egg-info/PKG-INFO` & `mixture_experimentalist-1.0.0a4/src/mixture_experimentalist.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mixture-experimentalist
-Version: 1.0.0a3
+Version: 1.0.0a4
 Summary: The goal of this project is to examine the performance of a mixture experimentalist–a hybrid of different experimental sampling strategies–in terms of its ability to recover a ground-truth model from synthetic data.
 Author-email: Marina Dubova <marina.dubova.97@gmail.com>
 License: MIT license
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/blinodelka/mixture_experimental_strategies
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
```

### Comparing `mixture_experimentalist-1.0.0a3/src/mixture_experimentalist.egg-info/SOURCES.txt` & `mixture_experimentalist-1.0.0a4/src/mixture_experimentalist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mixture_experimentalist-1.0.0a3/tests/README.md` & `mixture_experimentalist-1.0.0a4/tests/README.md`

 * *Files identical despite different names*

### Comparing `mixture_experimentalist-1.0.0a3/tests/test_mixture_experimentalist.py` & `mixture_experimentalist-1.0.0a4/tests/test_mixture_experimentalist.py`

 * *Files identical despite different names*

