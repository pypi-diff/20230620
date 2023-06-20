# Comparing `tmp/autora-experimentalist-sampler-novelty-1.0.1.tar.gz` & `tmp/autora-experimentalist-sampler-novelty-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-experimentalist-sampler-novelty-1.0.1.tar", last modified: Thu Jun  8 17:11:27 2023, max compression
+gzip compressed data, was "autora-experimentalist-sampler-novelty-1.0.2.tar", last modified: Tue Jun 20 18:18:50 2023, max compression
```

## Comparing `autora-experimentalist-sampler-novelty-1.0.1.tar` & `autora-experimentalist-sampler-novelty-1.0.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:11:27.512856 autora-experimentalist-sampler-novelty-1.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:11:27.508856 autora-experimentalist-sampler-novelty-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:11:27.508856 autora-experimentalist-sampler-novelty-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-08 17:11:14.000000 autora-experimentalist-sampler-novelty-1.0.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-08 17:11:14.000000 autora-experimentalist-sampler-novelty-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-08 17:11:14.000000 autora-experimentalist-sampler-novelty-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-06-08 17:11:27.512856 autora-experimentalist-sampler-novelty-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-06-08 17:11:14.000000 autora-experimentalist-sampler-novelty-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:11:27.508856 autora-experimentalist-sampler-novelty-1.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-06-08 17:11:14.000000 autora-experimentalist-sampler-novelty-1.0.1/docs/Basic Usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-06-08 17:11:14.000000 autora-experimentalist-sampler-novelty-1.0.1/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:11:27.508856 autora-experimentalist-sampler-novelty-1.0.1/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-08 17:11:14.000000 autora-experimentalist-sampler-novelty-1.0.1/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-08 17:11:14.000000 autora-experimentalist-sampler-novelty-1.0.1/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:11:27.508856 autora-experimentalist-sampler-novelty-1.0.1/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-08 17:11:14.000000 autora-experimentalist-sampler-novelty-1.0.1/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-08 17:11:14.000000 autora-experimentalist-sampler-novelty-1.0.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-08 17:11:14.000000 autora-experimentalist-sampler-novelty-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 17:11:27.512856 autora-experimentalist-sampler-novelty-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:11:27.508856 autora-experimentalist-sampler-novelty-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:11:27.508856 autora-experimentalist-sampler-novelty-1.0.1/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:11:27.508856 autora-experimentalist-sampler-novelty-1.0.1/src/autora/experimentalist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:11:27.508856 autora-experimentalist-sampler-novelty-1.0.1/src/autora/experimentalist/sampler/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:11:27.508856 autora-experimentalist-sampler-novelty-1.0.1/src/autora/experimentalist/sampler/novelty/
--rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-06-08 17:11:14.000000 autora-experimentalist-sampler-novelty-1.0.1/src/autora/experimentalist/sampler/novelty/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:11:27.512856 autora-experimentalist-sampler-novelty-1.0.1/src/autora_experimentalist_sampler_novelty.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-06-08 17:11:27.000000 autora-experimentalist-sampler-novelty-1.0.1/src/autora_experimentalist_sampler_novelty.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-08 17:11:27.000000 autora-experimentalist-sampler-novelty-1.0.1/src/autora_experimentalist_sampler_novelty.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 17:11:27.000000 autora-experimentalist-sampler-novelty-1.0.1/src/autora_experimentalist_sampler_novelty.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-08 17:11:27.000000 autora-experimentalist-sampler-novelty-1.0.1/src/autora_experimentalist_sampler_novelty.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 17:11:27.000000 autora-experimentalist-sampler-novelty-1.0.1/src/autora_experimentalist_sampler_novelty.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:11:27.512856 autora-experimentalist-sampler-novelty-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 17:11:14.000000 autora-experimentalist-sampler-novelty-1.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-06-08 17:11:14.000000 autora-experimentalist-sampler-novelty-1.0.1/tests/test_exp_novelty_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:18:50.638142 autora-experimentalist-sampler-novelty-1.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:18:50.638142 autora-experimentalist-sampler-novelty-1.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:18:50.638142 autora-experimentalist-sampler-novelty-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-20 18:18:40.000000 autora-experimentalist-sampler-novelty-1.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-20 18:18:40.000000 autora-experimentalist-sampler-novelty-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-20 18:18:40.000000 autora-experimentalist-sampler-novelty-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-06-20 18:18:50.638142 autora-experimentalist-sampler-novelty-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-06-20 18:18:40.000000 autora-experimentalist-sampler-novelty-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:18:50.638142 autora-experimentalist-sampler-novelty-1.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-06-20 18:18:40.000000 autora-experimentalist-sampler-novelty-1.0.2/docs/Basic Usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-20 18:18:40.000000 autora-experimentalist-sampler-novelty-1.0.2/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:18:50.638142 autora-experimentalist-sampler-novelty-1.0.2/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-20 18:18:40.000000 autora-experimentalist-sampler-novelty-1.0.2/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-20 18:18:40.000000 autora-experimentalist-sampler-novelty-1.0.2/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:18:50.638142 autora-experimentalist-sampler-novelty-1.0.2/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-20 18:18:40.000000 autora-experimentalist-sampler-novelty-1.0.2/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-20 18:18:40.000000 autora-experimentalist-sampler-novelty-1.0.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-20 18:18:40.000000 autora-experimentalist-sampler-novelty-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 18:18:50.638142 autora-experimentalist-sampler-novelty-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:18:50.638142 autora-experimentalist-sampler-novelty-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:18:50.638142 autora-experimentalist-sampler-novelty-1.0.2/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:18:50.638142 autora-experimentalist-sampler-novelty-1.0.2/src/autora/experimentalist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:18:50.638142 autora-experimentalist-sampler-novelty-1.0.2/src/autora/experimentalist/sampler/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:18:50.638142 autora-experimentalist-sampler-novelty-1.0.2/src/autora/experimentalist/sampler/novelty/
+-rw-r--r--   0 runner    (1001) docker     (123)     5964 2023-06-20 18:18:40.000000 autora-experimentalist-sampler-novelty-1.0.2/src/autora/experimentalist/sampler/novelty/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:18:50.638142 autora-experimentalist-sampler-novelty-1.0.2/src/autora_experimentalist_sampler_novelty.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-06-20 18:18:50.000000 autora-experimentalist-sampler-novelty-1.0.2/src/autora_experimentalist_sampler_novelty.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-20 18:18:50.000000 autora-experimentalist-sampler-novelty-1.0.2/src/autora_experimentalist_sampler_novelty.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 18:18:50.000000 autora-experimentalist-sampler-novelty-1.0.2/src/autora_experimentalist_sampler_novelty.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-20 18:18:50.000000 autora-experimentalist-sampler-novelty-1.0.2/src/autora_experimentalist_sampler_novelty.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 18:18:50.000000 autora-experimentalist-sampler-novelty-1.0.2/src/autora_experimentalist_sampler_novelty.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:18:50.638142 autora-experimentalist-sampler-novelty-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 18:18:40.000000 autora-experimentalist-sampler-novelty-1.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-06-20 18:18:40.000000 autora-experimentalist-sampler-novelty-1.0.2/tests/test_exp_novelty_sampler.py
```

### Comparing `autora-experimentalist-sampler-novelty-1.0.1/.github/workflows/python-publish.yml` & `autora-experimentalist-sampler-novelty-1.0.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-novelty-1.0.1/.gitignore` & `autora-experimentalist-sampler-novelty-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-novelty-1.0.1/.pre-commit-config.yaml` & `autora-experimentalist-sampler-novelty-1.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-novelty-1.0.1/PKG-INFO` & `autora-experimentalist-sampler-novelty-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experimentalist-sampler-novelty
-Version: 1.0.1
+Version: 1.0.2
 Summary: AutoRA Novelty Experimentalist
 Author-email: Sebastian Musslick <sebastian@musslick.de>
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-experimentalist-sampler-novelty
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8.10
```

### Comparing `autora-experimentalist-sampler-novelty-1.0.1/README.md` & `autora-experimentalist-sampler-novelty-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-novelty-1.0.1/docs/Basic Usage.ipynb` & `autora-experimentalist-sampler-novelty-1.0.2/docs/Basic Usage.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.985546875%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(1, "The novelty sampler selects $n$ novel experimental '*

 * *            "conditions from a pool of candidate experimental conditions $X'$. The choice is "*

 * *            "informed based on the similarity of the candidate conditions $X'$ with respect to "*

 * *            'previously examined experiment conditions $X$.\\n")], delete: [1]}}, 2: {\'source\': '*

 * *            "{insert: [(0, 'from autora.experimentalist.sampler.novelty import novelty_sample, "*

 * *            "novelty_scor […]*

```diff
@@ -7,30 +7,40 @@
                 "collapsed": false,
                 "pycharm": {
                     "name": "#%% md\n"
                 }
             },
             "source": [
                 "# Basic Usage\n",
-                "The novelty sampler selects $n$ novel experimental conditions from a pool of candidate experimental conditions $X'$. The choice is informed based on the similarity of the candidate conditons $X'$ with respect to previously examined experiment conditons $X$.\n",
+                "The novelty sampler selects $n$ novel experimental conditions from a pool of candidate experimental conditions $X'$. The choice is informed based on the similarity of the candidate conditions $X'$ with respect to previously examined experiment conditions $X$.\n",
                 "We begin with importing the relevant packages."
             ]
         },
         {
             "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Uncomment the following line when running on Google Colab\n",
+                "# !pip install \"autora[experimentalist-sampler-novelty]\""
+            ]
+        },
+        {
+            "cell_type": "code",
             "execution_count": 1,
             "metadata": {
                 "collapsed": false,
                 "pycharm": {
                     "name": "#%%\n"
                 }
             },
             "outputs": [],
             "source": [
-                "from autora.experimentalist.sampler.novelty import novelty_sampler, novelty_score_sampler\n",
+                "from autora.experimentalist.sampler.novelty import novelty_sample, novelty_score_sample\n",
                 "import numpy as np"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false,
@@ -136,15 +146,15 @@
                     "text": [
                         "[[10]\n",
                         " [ 9]]\n"
                     ]
                 }
             ],
             "source": [
-                "X_sampled = novelty_sampler(condition_pool = X_prime, reference_conditions = X, num_samples = n, metric = \"euclidean\", integration = \"sum\")\n",
+                "X_sampled = novelty_sample(condition_pool = X_prime, reference_conditions = X, num_samples = n, metric = \"euclidean\", integration = \"sum\")\n",
                 "print(X_sampled)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false,
@@ -208,15 +218,15 @@
                     "output_type": "stream",
                     "text": [
                         "[[10 11 12]]\n"
                     ]
                 }
             ],
             "source": [
-                "X_sampled = novelty_sampler(condition_pool = X_prime, reference_conditions = X, num_samples = 1, metric = \"euclidean\", integration = \"sum\")\n",
+                "X_sampled = novelty_sample(condition_pool = X_prime, reference_conditions = X, num_samples = 1, metric = \"euclidean\", integration = \"sum\")\n",
                 "print(X_sampled)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false,
@@ -245,15 +255,15 @@
                         "[[10 11 12]\n",
                         " [ 7  8  9]]\n",
                         "[1.35401943 0.43928867]\n"
                     ]
                 }
             ],
             "source": [
-                "X_sampled, scores = novelty_score_sampler(condition_pool = X_prime, reference_conditions = X, num_samples = 2, metric = \"euclidean\", integration = \"sum\")\n",
+                "X_sampled, scores = novelty_score_sample(condition_pool = X_prime, reference_conditions = X, num_samples = 2, metric = \"euclidean\", integration = \"sum\")\n",
                 "print(X_sampled)\n",
                 "print(scores)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
@@ -261,26 +271,14 @@
                 "pycharm": {
                     "name": "#%% md\n"
                 }
             },
             "source": [
                 "The novelty scores align with the sampled experiment conditions (in descending order of the novelty score)."
             ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%%\n"
-                }
-            },
-            "outputs": [],
-            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
             "language": "python",
             "name": "python3"
```

### Comparing `autora-experimentalist-sampler-novelty-1.0.1/docs/index.md` & `autora-experimentalist-sampler-novelty-1.0.2/docs/index.md`

 * *Files 1% similar despite different names*

```diff
@@ -43,24 +43,24 @@
 If the novelty sampler is tasked to identify two novel conditions, it will select
 the last two candidate conditions $x'_{1,j}$ and $x'_{2,j}$ because they have the greatest
 minimal distance to all existing conditions $x_{i,j}$:
 
 ### Example Code
 ```python
 import numpy as np
-from autora.experimentalist.sampler.novelty import novelty_sampler, novelty_score_sampler
+from autora.experimentalist.sampler.novelty import novelty_sample, novelty_score_sample
 
 # Specify X and X'
 X = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9], [10, 11, 12]])
 X_prime = np.array([[1, 1, 1], [2, 2, 2], [3, 3, 3]])
 
 # Here, we choose to identify two novel conditions
 n = 2
-X_sampled = novelty_sampler(condition_pool=X_prime, reference_conditions=X, num_samples=n)
+X_sampled = novelty_sample(condition_pool=X_prime, reference_conditions=X, num_samples=n)
 
 # We may also obtain samples along with their z-scored novelty scores  
-(X_sampled, scores) = novelty_score_sampler(condition_pool=X_prime, reference_conditions=X, num_samples=n)
+(X_sampled, scores) = novelty_score_sample(condition_pool=X_prime, reference_conditions=X, num_samples=n)
 ```
```

### Comparing `autora-experimentalist-sampler-novelty-1.0.1/mkdocs/base.yml` & `autora-experimentalist-sampler-novelty-1.0.2/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-novelty-1.0.1/pyproject.toml` & `autora-experimentalist-sampler-novelty-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-novelty-1.0.1/src/autora/experimentalist/sampler/novelty/__init__.py` & `autora-experimentalist-sampler-novelty-1.0.2/src/autora/experimentalist/sampler/novelty/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     "russellrao",
     "sokalmichener",
     "sokalsneath",
     "yule",
 ]
 
 
-def novelty_sampler(
+def novelty_sample(
     condition_pool: np.ndarray,
     reference_conditions: np.ndarray,
     num_samples: Optional[int] = None,
     metric: AllowedMetrics = "euclidean",
     integration: str = "min",
 ) -> np.ndarray:
     """
@@ -56,15 +56,15 @@
             'kulsinski', 'rogerstanimoto', 'russellrao', 'sokalmichener',
             'sokalsneath', 'yule'. See [sklearn.metrics.DistanceMetric][] for more details.
 
     Returns:
         Sampled pool of conditions
     """
 
-    new_conditions, distance_scores = novelty_score_sampler(condition_pool, reference_conditions, num_samples, metric, integration)
+    new_conditions, distance_scores = novelty_score_sample(condition_pool, reference_conditions, num_samples, metric, integration)
 
     return new_conditions
 
 
 def novelty_score_sample(
     condition_pool: np.ndarray,
     reference_conditions: np.ndarray,
@@ -143,8 +143,9 @@
 
     # order rows in Y from highest to lowest
     sorted_condition_pool = condition_pool[np.argsort(integrated_distance)[::-1]]
     sorted_score = score[np.argsort(score)[::-1]]
 
     return sorted_condition_pool[:num_samples], sorted_score[:num_samples]
 
+novelty_sampler = deprecated_alias(novelty_sample, "novelty_sampler")
 novelty_score_sampler = deprecated_alias(novelty_score_sample, "novelty_score_sampler")
```

### Comparing `autora-experimentalist-sampler-novelty-1.0.1/src/autora_experimentalist_sampler_novelty.egg-info/PKG-INFO` & `autora-experimentalist-sampler-novelty-1.0.2/src/autora_experimentalist_sampler_novelty.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experimentalist-sampler-novelty
-Version: 1.0.1
+Version: 1.0.2
 Summary: AutoRA Novelty Experimentalist
 Author-email: Sebastian Musslick <sebastian@musslick.de>
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-experimentalist-sampler-novelty
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8.10
```

### Comparing `autora-experimentalist-sampler-novelty-1.0.1/src/autora_experimentalist_sampler_novelty.egg-info/SOURCES.txt` & `autora-experimentalist-sampler-novelty-1.0.2/src/autora_experimentalist_sampler_novelty.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-novelty-1.0.1/tests/test_exp_novelty_sampler.py` & `autora-experimentalist-sampler-novelty-1.0.2/tests/test_exp_novelty_sampler.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-from autora.experimentalist.sampler.novelty import novelty_sampler, novelty_score_sampler
+from autora.experimentalist.sampler.novelty import novelty_sample, novelty_score_sample
 import numpy as np
 
 # Note: We encourage you to write more functionality tests for your sampler.
 
 def test_output_dimensions():
     condition_pool = np.array([[1, 2, 3, 4], [5, 6, 7, 8], [9, 10, 11, 12]])
     reference_conditions = np.array([[0, 0, 0, 0], [1, 1, 1, 1]])
     n = 2
-    condition_pool_new = novelty_sampler(condition_pool, reference_conditions, n)
+    condition_pool_new = novelty_sample(condition_pool, reference_conditions, n)
 
     # Check that the sampler returns n experiment conditions
     assert condition_pool_new.shape == (n, condition_pool.shape[1])
 
-def test_novelty_sampler_1D():
+def test_novelty_sample_1D():
 
     num_samples = 2
 
     # define two matrices
     matrix1 = np.array([1, 2, 3, 4, 5, 6, 7, 8, 9, 10])
     matrix2 = np.array([1, 2, 3])
 
     # reorder matrix1 according to its distances to matrix2
-    reordered_matrix1 = novelty_sampler(condition_pool = matrix1,
+    reordered_matrix1 = novelty_sample(condition_pool = matrix1,
                                         reference_conditions = matrix2,
                                         num_samples = num_samples)
 
     assert reordered_matrix1.shape[0] == num_samples
     assert reordered_matrix1.shape[1] == 1
     assert np.array_equal(reordered_matrix1, np.array([[10], [9]]))
 
 
-def test_novelty_sampler_ND():
+def test_novelty_sample_ND():
     # define two matrices
     matrix1 = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9], [10, 11, 12]])
     matrix2 = np.array([[1, 1, 1], [2, 2, 2], [3, 3, 3]])
     num_samples = 2
 
     # reorder matrix1 according to its distances to matrix2
-    reordered_matrix1 = novelty_sampler(condition_pool = matrix1,
+    reordered_matrix1 = novelty_sample(condition_pool = matrix1,
                                         reference_conditions = matrix2,
                                         num_samples = num_samples)
 
     assert reordered_matrix1.shape[0] == 2
     assert reordered_matrix1.shape[1] == 3
     assert np.array_equal(reordered_matrix1, np.array([[10, 11, 12], [7, 8, 9]]))
 
-def test_novelty_score_sampler_ND():
+def test_novelty_score_sample_ND():
     # define two matrices
     matrix1 = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9], [10, 11, 12]])
     matrix2 = np.array([[1, 1, 1], [2, 2, 2], [3, 3, 3]])
     num_samples = 3
 
     # reorder matrix1 according to its distances to matrix2, and obtain distance score
-    (reordered_matrix1, score) = novelty_score_sampler(condition_pool=matrix1,
+    (reordered_matrix1, score) = novelty_score_sample(condition_pool=matrix1,
                                         reference_conditions=matrix2,
                                         num_samples=num_samples)
 
     assert score[0] > score[1]  and score[1] > score[2]
```

