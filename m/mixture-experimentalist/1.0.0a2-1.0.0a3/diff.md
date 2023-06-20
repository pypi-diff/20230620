# Comparing `tmp/mixture_experimentalist-1.0.0a2.tar.gz` & `tmp/mixture_experimentalist-1.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mixture_experimentalist-1.0.0a2.tar", last modified: Mon Jun 19 13:20:58 2023, max compression
+gzip compressed data, was "mixture_experimentalist-1.0.0a3.tar", last modified: Tue Jun 20 16:00:46 2023, max compression
```

## Comparing `mixture_experimentalist-1.0.0a2.tar` & `mixture_experimentalist-1.0.0a3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-19 13:20:58.361372 mixture_experimentalist-1.0.0a2/
-drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-19 13:20:58.343318 mixture_experimentalist-1.0.0a2/.github/
-drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-19 13:20:58.348810 mixture_experimentalist-1.0.0a2/.github/workflows/
--rw-r--r--   0 marinadubova   (503) staff       (20)     1077 2023-05-24 16:20:27.000000 mixture_experimentalist-1.0.0a2/.github/workflows/python-publish.yml
--rw-r--r--   0 marinadubova   (503) staff       (20)      938 2023-05-24 16:20:27.000000 mixture_experimentalist-1.0.0a2/.gitignore
--rw-r--r--   0 marinadubova   (503) staff       (20)      674 2023-05-24 16:20:27.000000 mixture_experimentalist-1.0.0a2/.pre-commit-config.yaml
--rw-r--r--   0 marinadubova   (503) staff       (20)     1070 2023-05-24 16:18:58.000000 mixture_experimentalist-1.0.0a2/LICENSE
--rw-r--r--   0 marinadubova   (503) staff       (20)     2655 2023-06-19 13:20:58.360831 mixture_experimentalist-1.0.0a2/PKG-INFO
--rw-r--r--   0 marinadubova   (503) staff       (20)     1961 2023-06-19 13:09:17.000000 mixture_experimentalist-1.0.0a2/README.md
-drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-19 13:20:58.353459 mixture_experimentalist-1.0.0a2/docs/
--rw-r--r--   0 marinadubova   (503) staff       (20)   206968 2023-06-19 13:14:02.000000 mixture_experimentalist-1.0.0a2/docs/basic-usage.ipynb
--rw-r--r--   0 marinadubova   (503) staff       (20)      491 2023-06-19 13:11:31.000000 mixture_experimentalist-1.0.0a2/docs/index.md
-drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-19 13:20:58.354181 mixture_experimentalist-1.0.0a2/docs/javascripts/
--rw-r--r--   0 marinadubova   (503) staff       (20)      313 2023-05-24 16:20:27.000000 mixture_experimentalist-1.0.0a2/docs/javascripts/mathjax.js
--rw-r--r--   0 marinadubova   (503) staff       (20)      420 2023-05-24 16:20:27.000000 mixture_experimentalist-1.0.0a2/docs/quickstart.md
-drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-19 13:20:58.355036 mixture_experimentalist-1.0.0a2/mkdocs/
--rw-r--r--   0 marinadubova   (503) staff       (20)      729 2023-05-24 16:20:27.000000 mixture_experimentalist-1.0.0a2/mkdocs/base.yml
--rw-r--r--   0 marinadubova   (503) staff       (20)      384 2023-06-19 13:09:17.000000 mixture_experimentalist-1.0.0a2/mkdocs.yml
--rw-r--r--   0 marinadubova   (503) staff       (20)      973 2023-06-19 13:19:36.000000 mixture_experimentalist-1.0.0a2/pyproject.toml
--rw-r--r--   0 marinadubova   (503) staff       (20)       38 2023-06-19 13:20:58.361515 mixture_experimentalist-1.0.0a2/setup.cfg
-drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-19 13:20:58.344870 mixture_experimentalist-1.0.0a2/src/
-drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-19 13:20:58.344394 mixture_experimentalist-1.0.0a2/src/autora/
-drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-19 13:20:58.344534 mixture_experimentalist-1.0.0a2/src/autora/experimentalist/
-drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-19 13:20:58.344699 mixture_experimentalist-1.0.0a2/src/autora/experimentalist/sampler/
-drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-19 13:20:58.355755 mixture_experimentalist-1.0.0a2/src/autora/experimentalist/sampler/mixture_experimentalist/
--rw-r--r--   0 marinadubova   (503) staff       (20)     4273 2023-06-19 13:09:17.000000 mixture_experimentalist-1.0.0a2/src/autora/experimentalist/sampler/mixture_experimentalist/__init__.py
-drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-19 13:20:58.358089 mixture_experimentalist-1.0.0a2/src/mixture_experimentalist.egg-info/
--rw-r--r--   0 marinadubova   (503) staff       (20)     2655 2023-06-19 13:20:58.000000 mixture_experimentalist-1.0.0a2/src/mixture_experimentalist.egg-info/PKG-INFO
--rw-r--r--   0 marinadubova   (503) staff       (20)      612 2023-06-19 13:20:58.000000 mixture_experimentalist-1.0.0a2/src/mixture_experimentalist.egg-info/SOURCES.txt
--rw-r--r--   0 marinadubova   (503) staff       (20)        1 2023-06-19 13:20:58.000000 mixture_experimentalist-1.0.0a2/src/mixture_experimentalist.egg-info/dependency_links.txt
--rw-r--r--   0 marinadubova   (503) staff       (20)       49 2023-06-19 13:20:58.000000 mixture_experimentalist-1.0.0a2/src/mixture_experimentalist.egg-info/requires.txt
--rw-r--r--   0 marinadubova   (503) staff       (20)        7 2023-06-19 13:20:58.000000 mixture_experimentalist-1.0.0a2/src/mixture_experimentalist.egg-info/top_level.txt
-drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-19 13:20:58.359852 mixture_experimentalist-1.0.0a2/tests/
--rw-r--r--   0 marinadubova   (503) staff       (20)      841 2023-06-17 08:53:52.000000 mixture_experimentalist-1.0.0a2/tests/README.md
--rw-r--r--   0 marinadubova   (503) staff       (20)        0 2023-05-24 16:20:27.000000 mixture_experimentalist-1.0.0a2/tests/__init__.py
--rw-r--r--   0 marinadubova   (503) staff       (20)     1669 2023-06-19 13:09:17.000000 mixture_experimentalist-1.0.0a2/tests/test_mixture_experimentalist.py
+drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-20 16:00:46.206083 mixture_experimentalist-1.0.0a3/
+drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-20 16:00:46.186544 mixture_experimentalist-1.0.0a3/.github/
+drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-20 16:00:46.192667 mixture_experimentalist-1.0.0a3/.github/workflows/
+-rw-r--r--   0 marinadubova   (503) staff       (20)     1077 2023-05-24 16:20:27.000000 mixture_experimentalist-1.0.0a3/.github/workflows/python-publish.yml
+-rw-r--r--   0 marinadubova   (503) staff       (20)      938 2023-05-24 16:20:27.000000 mixture_experimentalist-1.0.0a3/.gitignore
+-rw-r--r--   0 marinadubova   (503) staff       (20)      674 2023-05-24 16:20:27.000000 mixture_experimentalist-1.0.0a3/.pre-commit-config.yaml
+-rw-r--r--   0 marinadubova   (503) staff       (20)     1070 2023-05-24 16:18:58.000000 mixture_experimentalist-1.0.0a3/LICENSE
+-rw-r--r--   0 marinadubova   (503) staff       (20)     2647 2023-06-20 16:00:46.205221 mixture_experimentalist-1.0.0a3/PKG-INFO
+-rw-r--r--   0 marinadubova   (503) staff       (20)     1953 2023-06-20 15:59:05.000000 mixture_experimentalist-1.0.0a3/README.md
+drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-20 16:00:46.196805 mixture_experimentalist-1.0.0a3/docs/
+-rw-r--r--   0 marinadubova   (503) staff       (20)   206355 2023-06-20 15:59:05.000000 mixture_experimentalist-1.0.0a3/docs/basic-usage.ipynb
+-rw-r--r--   0 marinadubova   (503) staff       (20)      491 2023-06-19 13:11:31.000000 mixture_experimentalist-1.0.0a3/docs/index.md
+drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-20 16:00:46.197697 mixture_experimentalist-1.0.0a3/docs/javascripts/
+-rw-r--r--   0 marinadubova   (503) staff       (20)      313 2023-05-24 16:20:27.000000 mixture_experimentalist-1.0.0a3/docs/javascripts/mathjax.js
+-rw-r--r--   0 marinadubova   (503) staff       (20)      388 2023-06-20 15:59:05.000000 mixture_experimentalist-1.0.0a3/docs/quickstart.md
+drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-20 16:00:46.198557 mixture_experimentalist-1.0.0a3/mkdocs/
+-rw-r--r--   0 marinadubova   (503) staff       (20)      729 2023-05-24 16:20:27.000000 mixture_experimentalist-1.0.0a3/mkdocs/base.yml
+-rw-r--r--   0 marinadubova   (503) staff       (20)      384 2023-06-19 13:09:17.000000 mixture_experimentalist-1.0.0a3/mkdocs.yml
+-rw-r--r--   0 marinadubova   (503) staff       (20)      973 2023-06-20 16:00:13.000000 mixture_experimentalist-1.0.0a3/pyproject.toml
+-rw-r--r--   0 marinadubova   (503) staff       (20)       38 2023-06-20 16:00:46.206281 mixture_experimentalist-1.0.0a3/setup.cfg
+drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-20 16:00:46.188055 mixture_experimentalist-1.0.0a3/src/
+drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-20 16:00:46.187544 mixture_experimentalist-1.0.0a3/src/autora/
+drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-20 16:00:46.187667 mixture_experimentalist-1.0.0a3/src/autora/experimentalist/
+drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-20 16:00:46.187793 mixture_experimentalist-1.0.0a3/src/autora/experimentalist/sampler/
+drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-20 16:00:46.199409 mixture_experimentalist-1.0.0a3/src/autora/experimentalist/sampler/mixture/
+-rw-r--r--   0 marinadubova   (503) staff       (20)     4273 2023-06-20 15:59:05.000000 mixture_experimentalist-1.0.0a3/src/autora/experimentalist/sampler/mixture/__init__.py
+drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-20 16:00:46.202546 mixture_experimentalist-1.0.0a3/src/mixture_experimentalist.egg-info/
+-rw-r--r--   0 marinadubova   (503) staff       (20)     2647 2023-06-20 16:00:46.000000 mixture_experimentalist-1.0.0a3/src/mixture_experimentalist.egg-info/PKG-INFO
+-rw-r--r--   0 marinadubova   (503) staff       (20)      596 2023-06-20 16:00:46.000000 mixture_experimentalist-1.0.0a3/src/mixture_experimentalist.egg-info/SOURCES.txt
+-rw-r--r--   0 marinadubova   (503) staff       (20)        1 2023-06-20 16:00:46.000000 mixture_experimentalist-1.0.0a3/src/mixture_experimentalist.egg-info/dependency_links.txt
+-rw-r--r--   0 marinadubova   (503) staff       (20)       49 2023-06-20 16:00:46.000000 mixture_experimentalist-1.0.0a3/src/mixture_experimentalist.egg-info/requires.txt
+-rw-r--r--   0 marinadubova   (503) staff       (20)        7 2023-06-20 16:00:46.000000 mixture_experimentalist-1.0.0a3/src/mixture_experimentalist.egg-info/top_level.txt
+drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-20 16:00:46.204437 mixture_experimentalist-1.0.0a3/tests/
+-rw-r--r--   0 marinadubova   (503) staff       (20)      841 2023-06-17 08:53:52.000000 mixture_experimentalist-1.0.0a3/tests/README.md
+-rw-r--r--   0 marinadubova   (503) staff       (20)        0 2023-05-24 16:20:27.000000 mixture_experimentalist-1.0.0a3/tests/__init__.py
+-rw-r--r--   0 marinadubova   (503) staff       (20)     1653 2023-06-20 15:59:05.000000 mixture_experimentalist-1.0.0a3/tests/test_mixture_experimentalist.py
```

### Comparing `mixture_experimentalist-1.0.0a2/.github/workflows/python-publish.yml` & `mixture_experimentalist-1.0.0a3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `mixture_experimentalist-1.0.0a2/.gitignore` & `mixture_experimentalist-1.0.0a3/.gitignore`

 * *Files identical despite different names*

### Comparing `mixture_experimentalist-1.0.0a2/.pre-commit-config.yaml` & `mixture_experimentalist-1.0.0a3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mixture_experimentalist-1.0.0a2/LICENSE` & `mixture_experimentalist-1.0.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `mixture_experimentalist-1.0.0a2/PKG-INFO` & `mixture_experimentalist-1.0.0a3/src/mixture_experimentalist.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mixture_experimentalist
-Version: 1.0.0a2
+Name: mixture-experimentalist
+Version: 1.0.0a3
 Summary: The goal of this project is to examine the performance of a mixture experimentalist–a hybrid of different experimental sampling strategies–in terms of its ability to recover a ground-truth model from synthetic data.
 Author-email: Marina Dubova <marina.dubova.97@gmail.com>
 License: MIT license
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/blinodelka/mixture_experimental_strategies
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
@@ -23,21 +23,21 @@
 You will need:
 
 - Python 3.8 or greater: https://www.python.org/downloads/
 
 Mixture Experimentalist is a part of the AutoRA package:
 
 ```bash
-pip install -U autora["mixture_experimentalist"]
+pip install -U autora["experimentalist-sampler-mixture"]
 ```
 
 Check your installation by running:
 
 ```bash
-python -c "from autora.experimentalist.sampler.mixture_experimentalist import mixture_sample"
+python -c "from autora.experimentalist.sampler.mixture import mixture_sample"
 ```
 
 ## Usage
 
 The Mixture Experimentalist can be used to select experimental conditions based on a mixture of different strategies. Here's a basic example:
 
 ```python
```

### Comparing `mixture_experimentalist-1.0.0a2/README.md` & `mixture_experimentalist-1.0.0a3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: mixture_experimentalist
+Version: 1.0.0a3
+Summary: The goal of this project is to examine the performance of a mixture experimentalist–a hybrid of different experimental sampling strategies–in terms of its ability to recover a ground-truth model from synthetic data.
+Author-email: Marina Dubova <marina.dubova.97@gmail.com>
+License: MIT license
+Project-URL: homepage, http://www.empiricalresearch.ai
+Project-URL: repository, https://github.com/blinodelka/mixture_experimental_strategies
+Project-URL: documentation, https://autoresearch.github.io/autora/
+Requires-Python: <4,>=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 # AutoRA Mixture Experimentalist
 
 The Mixture Experimentalist identifies novel experimental conditions under which a hybrid of different experimental sampling strategies is used. 
 This mixture can include any custom strategies such as falsification, novelty, crucial experimentation, uncertainty, elimination, aesthetic preferences, and arbitrary preferred/dispreferred regions of the space. The selection of conditions is based on a weighted sum of the scores obtained from these strategies.
  
 
 ## Quickstart Guide
@@ -9,21 +23,21 @@
 You will need:
 
 - Python 3.8 or greater: https://www.python.org/downloads/
 
 Mixture Experimentalist is a part of the AutoRA package:
 
 ```bash
-pip install -U autora["mixture_experimentalist"]
+pip install -U autora["experimentalist-sampler-mixture"]
 ```
 
 Check your installation by running:
 
 ```bash
-python -c "from autora.experimentalist.sampler.mixture_experimentalist import mixture_sample"
+python -c "from autora.experimentalist.sampler.mixture import mixture_sample"
 ```
 
 ## Usage
 
 The Mixture Experimentalist can be used to select experimental conditions based on a mixture of different strategies. Here's a basic example:
 
 ```python
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mixture_experimentalist-1.0.0a2/docs/basic-usage.ipynb` & `mixture_experimentalist-1.0.0a3/docs/basic-usage.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9935%*

 * *Differences: {"'cells'": "{2: {'execution_count': None, 'outputs': [], 'source': ['from "*

 * *            "autora.experimentalist.sampler.mixture import mixture_sample']}, insert: [(1, "*

 * *            "OrderedDict([('cell_type', 'code'), ('execution_count', None), ('metadata', "*

 * *            "OrderedDict()), ('outputs', []), ('source', ['# Uncomment the following lines when "*

 * *            "running on Google Colab\\n', '# !pip install "*

 * *            "autora[experimentalits-sampler-mixture]\\n', '# !pip install "*

 * *            "auto […]*

```diff
@@ -9,33 +9,33 @@
                 "The goal of this notebook is to demonstrate the usage of the `mixture_sample` function, which combines different sampling strategies to select experimental conditions. The `mixture_sample` function takes a pool of experimental conditions, a temperature parameter, a list of samplers with their weights, a dictionary of parameters for the samplers, and an optional number of samples to return.\n",
                 "\n",
                 "We begin with importing the necessary packages."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Uncomment the following lines when running on Google Colab\n",
+                "# !pip install autora[experimentalits-sampler-mixture]\n",
+                "# !pip install autora[experimentalist-falsification]\n",
+                "# !pip install autora[experimentalist-sampler-inequality]"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
             "metadata": {
                 "collapsed": true
             },
-            "outputs": [
-                {
-                    "ename": "ModuleNotFoundError",
-                    "evalue": "No module named 'autora.experimentalist.sampler.mixture_experimentalist'",
-                    "output_type": "error",
-                    "traceback": [
-                        "\u001b[0;31m---------------------------------------------------------------------------\u001b[0m",
-                        "\u001b[0;31mModuleNotFoundError\u001b[0m                       Traceback (most recent call last)",
-                        "Cell \u001b[0;32mIn[2], line 1\u001b[0m\n\u001b[0;32m----> 1\u001b[0m \u001b[38;5;28;01mfrom\u001b[39;00m \u001b[38;5;21;01mautora\u001b[39;00m\u001b[38;5;21;01m.\u001b[39;00m\u001b[38;5;21;01mexperimentalist\u001b[39;00m\u001b[38;5;21;01m.\u001b[39;00m\u001b[38;5;21;01msampler\u001b[39;00m\u001b[38;5;21;01m.\u001b[39;00m\u001b[38;5;21;01mmixture_experimentalist\u001b[39;00m \u001b[38;5;28;01mimport\u001b[39;00m mixture_sampler\n",
-                        "\u001b[0;31mModuleNotFoundError\u001b[0m: No module named 'autora.experimentalist.sampler.mixture_experimentalist'"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
-                "from autora.experimentalist.sampler.mixture_experimentalist import mixture_sample"
+                "from autora.experimentalist.sampler.mixture import mixture_sample"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 132,
             "metadata": {},
             "outputs": [],
```

### Comparing `mixture_experimentalist-1.0.0a2/mkdocs/base.yml` & `mixture_experimentalist-1.0.0a3/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `mixture_experimentalist-1.0.0a2/pyproject.toml` & `mixture_experimentalist-1.0.0a3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 # UPDATE THIS BEFORE PUBLISHING
 name = "mixture_experimentalist"
 description = "The goal of this project is to examine the performance of a mixture experimentalist–a hybrid of different experimental sampling strategies–in terms of its ability to recover a ground-truth model from synthetic data."
 authors = [{ name = "Marina Dubova", email = "marina.dubova.97@gmail.com" }]
-version = "1.0.0a2"
+version = "1.0.0a3"
 
 readme = "README.md"
 license = { text = "MIT license" }
 requires-python = ">=3.8,<4"
 
 # ADD NEW DEPENDENCIES HERE
 dependencies = [
```

### Comparing `mixture_experimentalist-1.0.0a2/src/autora/experimentalist/sampler/mixture_experimentalist/__init__.py` & `mixture_experimentalist-1.0.0a3/src/autora/experimentalist/sampler/mixture/__init__.py`

 * *Files identical despite different names*

### Comparing `mixture_experimentalist-1.0.0a2/src/mixture_experimentalist.egg-info/PKG-INFO` & `mixture_experimentalist-1.0.0a3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: mixture-experimentalist
-Version: 1.0.0a2
-Summary: The goal of this project is to examine the performance of a mixture experimentalist–a hybrid of different experimental sampling strategies–in terms of its ability to recover a ground-truth model from synthetic data.
-Author-email: Marina Dubova <marina.dubova.97@gmail.com>
-License: MIT license
-Project-URL: homepage, http://www.empiricalresearch.ai
-Project-URL: repository, https://github.com/blinodelka/mixture_experimental_strategies
-Project-URL: documentation, https://autoresearch.github.io/autora/
-Requires-Python: <4,>=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # AutoRA Mixture Experimentalist
 
 The Mixture Experimentalist identifies novel experimental conditions under which a hybrid of different experimental sampling strategies is used. 
 This mixture can include any custom strategies such as falsification, novelty, crucial experimentation, uncertainty, elimination, aesthetic preferences, and arbitrary preferred/dispreferred regions of the space. The selection of conditions is based on a weighted sum of the scores obtained from these strategies.
  
 
 ## Quickstart Guide
@@ -23,21 +9,21 @@
 You will need:
 
 - Python 3.8 or greater: https://www.python.org/downloads/
 
 Mixture Experimentalist is a part of the AutoRA package:
 
 ```bash
-pip install -U autora["mixture_experimentalist"]
+pip install -U autora["experimentalist-sampler-mixture"]
 ```
 
 Check your installation by running:
 
 ```bash
-python -c "from autora.experimentalist.sampler.mixture_experimentalist import mixture_sample"
+python -c "from autora.experimentalist.sampler.mixture import mixture_sample"
 ```
 
 ## Usage
 
 The Mixture Experimentalist can be used to select experimental conditions based on a mixture of different strategies. Here's a basic example:
 
 ```python
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mixture_experimentalist-1.0.0a2/src/mixture_experimentalist.egg-info/SOURCES.txt` & `mixture_experimentalist-1.0.0a3/src/mixture_experimentalist.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 pyproject.toml
 .github/workflows/python-publish.yml
 docs/basic-usage.ipynb
 docs/index.md
 docs/quickstart.md
 docs/javascripts/mathjax.js
 mkdocs/base.yml
-src/autora/experimentalist/sampler/mixture_experimentalist/__init__.py
+src/autora/experimentalist/sampler/mixture/__init__.py
 src/mixture_experimentalist.egg-info/PKG-INFO
 src/mixture_experimentalist.egg-info/SOURCES.txt
 src/mixture_experimentalist.egg-info/dependency_links.txt
 src/mixture_experimentalist.egg-info/requires.txt
 src/mixture_experimentalist.egg-info/top_level.txt
 tests/README.md
 tests/__init__.py
```

### Comparing `mixture_experimentalist-1.0.0a2/tests/README.md` & `mixture_experimentalist-1.0.0a3/tests/README.md`

 * *Files identical despite different names*

### Comparing `mixture_experimentalist-1.0.0a2/tests/test_mixture_experimentalist.py` & `mixture_experimentalist-1.0.0a3/tests/test_mixture_experimentalist.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from autora.experimentalist.sampler.mixture_experimentalist import mixture_sample
+from autora.experimentalist.sampler.mixture import mixture_sample
 import numpy as np
 import pytest
 
 def mock_sampler(condition_pool, **kwargs):
     return condition_pool, np.random.rand(len(condition_pool))
 
 def test_mixture_sample():
```

