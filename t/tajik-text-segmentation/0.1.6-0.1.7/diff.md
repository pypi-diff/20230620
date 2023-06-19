# Comparing `tmp/tajik_text_segmentation-0.1.6.tar.gz` & `tmp/tajik_text_segmentation-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tajik_text_segmentation-0.1.6.tar", last modified: Sat Jun 17 09:06:20 2023, max compression
+gzip compressed data, was "tajik_text_segmentation-0.1.7.tar", last modified: Mon Jun 19 23:31:25 2023, max compression
```

## Comparing `tajik_text_segmentation-0.1.6.tar` & `tajik_text_segmentation-0.1.7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 09:06:20.009430 tajik_text_segmentation-0.1.6/
--rw-rw-rw-   0        0        0       38 2023-06-16 20:52:08.000000 tajik_text_segmentation-0.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0     6366 2023-06-17 09:06:20.004711 tajik_text_segmentation-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     5611 2023-06-16 20:23:43.000000 tajik_text_segmentation-0.1.6/README.md
--rw-rw-rw-   0        0        0       42 2023-06-17 09:06:20.009430 tajik_text_segmentation-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1204 2023-06-17 09:04:59.000000 tajik_text_segmentation-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-17 09:06:19.909957 tajik_text_segmentation-0.1.6/tajik_text_segmentation/
--rw-rw-rw-   0        0        0       43 2023-06-16 19:33:51.000000 tajik_text_segmentation-0.1.6/tajik_text_segmentation/__init__.py
--rw-rw-rw-   0        0        0     8336 2023-06-16 19:30:58.000000 tajik_text_segmentation-0.1.6/tajik_text_segmentation/annotated.py
--rw-rw-rw-   0        0        0     7106 2023-06-17 09:05:32.000000 tajik_text_segmentation-0.1.6/tajik_text_segmentation/boundary_resolver.py
-drwxrwxrwx   0        0        0        0 2023-06-17 09:06:19.970491 tajik_text_segmentation-0.1.6/tajik_text_segmentation/checkpoints/
--rw-rw-rw-   0        0        0   105452 2023-06-15 21:04:02.000000 tajik_text_segmentation-0.1.6/tajik_text_segmentation/checkpoints/checkpoint.pt
--rw-rw-rw-   0        0        0      557 2023-06-17 08:28:26.000000 tajik_text_segmentation-0.1.6/tajik_text_segmentation/config.json
--rw-rw-rw-   0        0        0     5936 2023-06-16 19:28:56.000000 tajik_text_segmentation-0.1.6/tajik_text_segmentation/heuristic_model.py
-drwxrwxrwx   0        0        0        0 2023-06-17 09:06:19.978757 tajik_text_segmentation-0.1.6/tajik_text_segmentation/nn_model/
--rw-rw-rw-   0        0        0        0 2023-06-16 20:37:57.000000 tajik_text_segmentation-0.1.6/tajik_text_segmentation/nn_model/__init__.py
--rw-rw-rw-   0        0        0     8125 2023-06-17 08:26:48.000000 tajik_text_segmentation-0.1.6/tajik_text_segmentation/nn_model/model.py
--rw-rw-rw-   0        0        0     6834 2023-06-16 19:29:28.000000 tajik_text_segmentation-0.1.6/tajik_text_segmentation/nn_model/vocab.py
--rw-rw-rw-   0        0        0     3588 2023-06-17 08:22:16.000000 tajik_text_segmentation-0.1.6/tajik_text_segmentation/text_segmenter.py
--rw-rw-rw-   0        0        0      551 2023-06-16 19:18:47.000000 tajik_text_segmentation-0.1.6/tajik_text_segmentation/tokenizer.py
-drwxrwxrwx   0        0        0        0 2023-06-17 09:06:19.967970 tajik_text_segmentation-0.1.6/tajik_text_segmentation.egg-info/
--rw-rw-rw-   0        0        0     6366 2023-06-17 09:06:19.000000 tajik_text_segmentation-0.1.6/tajik_text_segmentation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      881 2023-06-17 09:06:19.000000 tajik_text_segmentation-0.1.6/tajik_text_segmentation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 09:06:19.000000 tajik_text_segmentation-0.1.6/tajik_text_segmentation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-06-17 09:06:19.000000 tajik_text_segmentation-0.1.6/tajik_text_segmentation.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-06-17 09:06:19.000000 tajik_text_segmentation-0.1.6/tajik_text_segmentation.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-17 09:06:19.992978 tajik_text_segmentation-0.1.6/tests/
--rw-rw-rw-   0        0        0     1350 2023-06-16 20:26:44.000000 tajik_text_segmentation-0.1.6/tests/test_dataset.py
--rw-rw-rw-   0        0        0     1489 2023-06-16 20:30:33.000000 tajik_text_segmentation-0.1.6/tests/test_evaluate.py
--rw-rw-rw-   0        0        0     4071 2023-06-16 19:38:17.000000 tajik_text_segmentation-0.1.6/tests/test_heuristic_model.py
--rw-rw-rw-   0        0        0     1939 2023-06-16 19:38:23.000000 tajik_text_segmentation-0.1.6/tests/test_tokenizer.py
-drwxrwxrwx   0        0        0        0 2023-06-17 09:06:19.999528 tajik_text_segmentation-0.1.6/training/
--rw-rw-rw-   0        0        0      450 2023-06-16 20:30:59.000000 tajik_text_segmentation-0.1.6/training/dummy_model.py
--rw-rw-rw-   0        0        0     4903 2023-06-17 08:29:26.000000 tajik_text_segmentation-0.1.6/training/evaluate.py
--rw-rw-rw-   0        0        0      498 2023-06-16 19:18:47.000000 tajik_text_segmentation-0.1.6/training/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:31:25.616675 tajik_text_segmentation-0.1.7/
+-rw-rw-rw-   0        0        0       38 2023-06-16 20:52:08.000000 tajik_text_segmentation-0.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     6366 2023-06-19 23:31:25.615196 tajik_text_segmentation-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     5611 2023-06-16 20:23:43.000000 tajik_text_segmentation-0.1.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-19 23:31:25.617250 tajik_text_segmentation-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1204 2023-06-19 23:28:22.000000 tajik_text_segmentation-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:31:25.537461 tajik_text_segmentation-0.1.7/tajik_text_segmentation/
+-rw-rw-rw-   0        0        0       43 2023-06-16 19:33:51.000000 tajik_text_segmentation-0.1.7/tajik_text_segmentation/__init__.py
+-rw-rw-rw-   0        0        0     8336 2023-06-16 19:30:58.000000 tajik_text_segmentation-0.1.7/tajik_text_segmentation/annotated.py
+-rw-rw-rw-   0        0        0     7122 2023-06-19 23:25:48.000000 tajik_text_segmentation-0.1.7/tajik_text_segmentation/boundary_resolver.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:31:25.578481 tajik_text_segmentation-0.1.7/tajik_text_segmentation/checkpoints/
+-rw-rw-rw-   0        0        0   105452 2023-06-15 21:04:02.000000 tajik_text_segmentation-0.1.7/tajik_text_segmentation/checkpoints/checkpoint.pt
+-rw-rw-rw-   0        0        0      557 2023-06-17 08:28:26.000000 tajik_text_segmentation-0.1.7/tajik_text_segmentation/config.json
+-rw-rw-rw-   0        0        0     5936 2023-06-16 19:28:56.000000 tajik_text_segmentation-0.1.7/tajik_text_segmentation/heuristic_model.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:31:25.588188 tajik_text_segmentation-0.1.7/tajik_text_segmentation/nn_model/
+-rw-rw-rw-   0        0        0        0 2023-06-16 20:37:57.000000 tajik_text_segmentation-0.1.7/tajik_text_segmentation/nn_model/__init__.py
+-rw-rw-rw-   0        0        0     8125 2023-06-17 08:26:48.000000 tajik_text_segmentation-0.1.7/tajik_text_segmentation/nn_model/model.py
+-rw-rw-rw-   0        0        0     6834 2023-06-16 19:29:28.000000 tajik_text_segmentation-0.1.7/tajik_text_segmentation/nn_model/vocab.py
+-rw-rw-rw-   0        0        0     3588 2023-06-17 08:22:16.000000 tajik_text_segmentation-0.1.7/tajik_text_segmentation/text_segmenter.py
+-rw-rw-rw-   0        0        0      551 2023-06-16 19:18:47.000000 tajik_text_segmentation-0.1.7/tajik_text_segmentation/tokenizer.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:31:25.575487 tajik_text_segmentation-0.1.7/tajik_text_segmentation.egg-info/
+-rw-rw-rw-   0        0        0     6366 2023-06-19 23:31:25.000000 tajik_text_segmentation-0.1.7/tajik_text_segmentation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      881 2023-06-19 23:31:25.000000 tajik_text_segmentation-0.1.7/tajik_text_segmentation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 23:31:25.000000 tajik_text_segmentation-0.1.7/tajik_text_segmentation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-06-19 23:31:25.000000 tajik_text_segmentation-0.1.7/tajik_text_segmentation.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-06-19 23:31:25.000000 tajik_text_segmentation-0.1.7/tajik_text_segmentation.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 23:31:25.601022 tajik_text_segmentation-0.1.7/tests/
+-rw-rw-rw-   0        0        0     1350 2023-06-16 20:26:44.000000 tajik_text_segmentation-0.1.7/tests/test_dataset.py
+-rw-rw-rw-   0        0        0     1489 2023-06-16 20:30:33.000000 tajik_text_segmentation-0.1.7/tests/test_evaluate.py
+-rw-rw-rw-   0        0        0     4071 2023-06-16 19:38:17.000000 tajik_text_segmentation-0.1.7/tests/test_heuristic_model.py
+-rw-rw-rw-   0        0        0     1939 2023-06-16 19:38:23.000000 tajik_text_segmentation-0.1.7/tests/test_tokenizer.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:31:25.611705 tajik_text_segmentation-0.1.7/training/
+-rw-rw-rw-   0        0        0      450 2023-06-16 20:30:59.000000 tajik_text_segmentation-0.1.7/training/dummy_model.py
+-rw-rw-rw-   0        0        0     4903 2023-06-17 08:29:26.000000 tajik_text_segmentation-0.1.7/training/evaluate.py
+-rw-rw-rw-   0        0        0      498 2023-06-16 19:18:47.000000 tajik_text_segmentation-0.1.7/training/utils.py
```

### Comparing `tajik_text_segmentation-0.1.6/PKG-INFO` & `tajik_text_segmentation-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tajik_text_segmentation
-Version: 0.1.6
+Version: 0.1.7
 Summary: A package for Tajik text segmentation using a heuristic algorithm and neural network.
 Home-page: https://github.com/sobir-git/tajik-text-segmentation
 Author: Sobir Bobiev
 Author-email: sobir.bobiev@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tajik_text_segmentation-0.1.6/README.md` & `tajik_text_segmentation-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `tajik_text_segmentation-0.1.6/setup.py` & `tajik_text_segmentation-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="tajik_text_segmentation",
-    version="0.1.6",
+    version="0.1.7",
     author="Sobir Bobiev",
     author_email="sobir.bobiev@gmail.com",
     description="A package for Tajik text segmentation using a heuristic algorithm and neural network.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/sobir-git/tajik-text-segmentation",
     packages=find_packages(exclude=['training', 'tests']),
```

### Comparing `tajik_text_segmentation-0.1.6/tajik_text_segmentation/annotated.py` & `tajik_text_segmentation-0.1.7/tajik_text_segmentation/annotated.py`

 * *Files identical despite different names*

### Comparing `tajik_text_segmentation-0.1.6/tajik_text_segmentation/boundary_resolver.py` & `tajik_text_segmentation-0.1.7/tajik_text_segmentation/boundary_resolver.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         # beginning (dp[i][0]) or end (dp[i][1])
         dp = [[-float('inf')]*2 for _ in range(len(logp))]
 
         # used for backtracking the best segmentation
         prev = [[None]*2 for _ in range(len(logp))]
 
         # candidate list which contains candidate "start" indices
-        candidates = list(range(max_gap+1))  # the start index can be 0, ... , max_gap
+        candidates = list(range(min(max_gap+1, len(logp))))  # the start index can be 0, ... , max_gap
         
         # logprobability threshold for considering an index as a candidate
         logp_threshold = np.log(self.candidate_threshold)
 
         # initialize initial values
         dp[0][0] = logp[0][0]   # --> the log-likelihood of the segmentation up to start of the 0th token
```

### Comparing `tajik_text_segmentation-0.1.6/tajik_text_segmentation/checkpoints/checkpoint.pt` & `tajik_text_segmentation-0.1.7/tajik_text_segmentation/checkpoints/checkpoint.pt`

 * *Files identical despite different names*

### Comparing `tajik_text_segmentation-0.1.6/tajik_text_segmentation/config.json` & `tajik_text_segmentation-0.1.7/tajik_text_segmentation/config.json`

 * *Files identical despite different names*

### Comparing `tajik_text_segmentation-0.1.6/tajik_text_segmentation/heuristic_model.py` & `tajik_text_segmentation-0.1.7/tajik_text_segmentation/heuristic_model.py`

 * *Files identical despite different names*

### Comparing `tajik_text_segmentation-0.1.6/tajik_text_segmentation/nn_model/model.py` & `tajik_text_segmentation-0.1.7/tajik_text_segmentation/nn_model/model.py`

 * *Files identical despite different names*

### Comparing `tajik_text_segmentation-0.1.6/tajik_text_segmentation/nn_model/vocab.py` & `tajik_text_segmentation-0.1.7/tajik_text_segmentation/nn_model/vocab.py`

 * *Files identical despite different names*

### Comparing `tajik_text_segmentation-0.1.6/tajik_text_segmentation/text_segmenter.py` & `tajik_text_segmentation-0.1.7/tajik_text_segmentation/text_segmenter.py`

 * *Files identical despite different names*

### Comparing `tajik_text_segmentation-0.1.6/tajik_text_segmentation/tokenizer.py` & `tajik_text_segmentation-0.1.7/tajik_text_segmentation/tokenizer.py`

 * *Files identical despite different names*

### Comparing `tajik_text_segmentation-0.1.6/tajik_text_segmentation.egg-info/PKG-INFO` & `tajik_text_segmentation-0.1.7/tajik_text_segmentation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tajik-text-segmentation
-Version: 0.1.6
+Version: 0.1.7
 Summary: A package for Tajik text segmentation using a heuristic algorithm and neural network.
 Home-page: https://github.com/sobir-git/tajik-text-segmentation
 Author: Sobir Bobiev
 Author-email: sobir.bobiev@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tajik_text_segmentation-0.1.6/tajik_text_segmentation.egg-info/SOURCES.txt` & `tajik_text_segmentation-0.1.7/tajik_text_segmentation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tajik_text_segmentation-0.1.6/tests/test_dataset.py` & `tajik_text_segmentation-0.1.7/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `tajik_text_segmentation-0.1.6/tests/test_evaluate.py` & `tajik_text_segmentation-0.1.7/tests/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `tajik_text_segmentation-0.1.6/tests/test_heuristic_model.py` & `tajik_text_segmentation-0.1.7/tests/test_heuristic_model.py`

 * *Files identical despite different names*

### Comparing `tajik_text_segmentation-0.1.6/tests/test_tokenizer.py` & `tajik_text_segmentation-0.1.7/tests/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `tajik_text_segmentation-0.1.6/training/evaluate.py` & `tajik_text_segmentation-0.1.7/training/evaluate.py`

 * *Files identical despite different names*

