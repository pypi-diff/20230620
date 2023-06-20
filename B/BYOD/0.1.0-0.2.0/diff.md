# Comparing `tmp/BYOD-0.1.0.tar.gz` & `tmp/BYOD-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BYOD-0.1.0.tar", last modified: Tue Jun 20 04:06:49 2023, max compression
+gzip compressed data, was "BYOD-0.2.0.tar", last modified: Tue Jun 20 04:01:09 2023, max compression
```

## Comparing `BYOD-0.1.0.tar` & `BYOD-0.2.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 njain17  (14198) njain17  (14198)        0 2023-06-20 04:06:49.119668 BYOD-0.1.0/
-drwxr-xr-x   0 njain17  (14198) njain17  (14198)        0 2023-06-20 04:06:49.025713 BYOD-0.1.0/BYOD/
-drwxr-xr-x   0 njain17  (14198) njain17  (14198)        0 2023-06-20 04:06:49.073258 BYOD-0.1.0/BYOD/List-of-Dirty-Naughty-Obscene-and-Otherwise-Bad-Words/
--rw-r--r--   0 njain17  (14198) njain17  (14198)     3776 2023-06-20 02:54:23.000000 BYOD-0.1.0/BYOD/List-of-Dirty-Naughty-Obscene-and-Otherwise-Bad-Words/en.txt
--rw-r--r--   0 njain17  (14198) njain17  (14198)      380 2023-06-20 02:54:23.000000 BYOD-0.1.0/BYOD/__init__.py
--rw-r--r--   0 njain17  (14198) njain17  (14198)     3683 2023-06-20 02:54:23.000000 BYOD-0.1.0/BYOD/context_sensitivity.py
--rw-r--r--   0 njain17  (14198) njain17  (14198)     3545 2023-06-20 02:54:23.000000 BYOD-0.1.0/BYOD/negations.py
--rw-r--r--   0 njain17  (14198) njain17  (14198)     6287 2023-06-20 02:54:23.000000 BYOD-0.1.0/BYOD/tokenization_robustness.py
--rw-r--r--   0 njain17  (14198) njain17  (14198)    10631 2023-06-20 02:54:23.000000 BYOD-0.1.0/BYOD/toxicity.py
-drwxr-xr-x   0 njain17  (14198) njain17  (14198)        0 2023-06-20 04:06:49.096834 BYOD-0.1.0/BYOD/utils/
--rw-r--r--   0 njain17  (14198) njain17  (14198)      558 2023-06-20 02:54:23.000000 BYOD-0.1.0/BYOD/utils/JSD.py
--rw-r--r--   0 njain17  (14198) njain17  (14198)      137 2023-06-20 02:54:23.000000 BYOD-0.1.0/BYOD/utils/__init__.py
--rw-r--r--   0 njain17  (14198) njain17  (14198)     4163 2023-06-20 02:54:23.000000 BYOD-0.1.0/BYOD/utils/hf_utils.py
--rw-r--r--   0 njain17  (14198) njain17  (14198)     4540 2023-06-20 02:54:23.000000 BYOD-0.1.0/BYOD/utils/wikiDataset.py
--rw-r--r--   0 njain17  (14198) njain17  (14198)     4196 2023-06-20 02:54:23.000000 BYOD-0.1.0/BYOD/word_order.py
-drwxr-xr-x   0 njain17  (14198) njain17  (14198)        0 2023-06-20 04:06:49.066442 BYOD-0.1.0/BYOD.egg-info/
--rw-r--r--   0 njain17  (14198) njain17  (14198)     3168 2023-06-20 04:06:48.000000 BYOD-0.1.0/BYOD.egg-info/PKG-INFO
--rw-r--r--   0 njain17  (14198) njain17  (14198)      630 2023-06-20 04:06:48.000000 BYOD-0.1.0/BYOD.egg-info/SOURCES.txt
--rw-r--r--   0 njain17  (14198) njain17  (14198)        1 2023-06-20 04:06:48.000000 BYOD-0.1.0/BYOD.egg-info/dependency_links.txt
--rw-r--r--   0 njain17  (14198) njain17  (14198)        1 2023-06-20 04:06:48.000000 BYOD-0.1.0/BYOD.egg-info/not-zip-safe
--rw-r--r--   0 njain17  (14198) njain17  (14198)       97 2023-06-20 04:06:48.000000 BYOD-0.1.0/BYOD.egg-info/requires.txt
--rw-r--r--   0 njain17  (14198) njain17  (14198)        5 2023-06-20 04:06:48.000000 BYOD-0.1.0/BYOD.egg-info/top_level.txt
--rw-r--r--   0 njain17  (14198) njain17  (14198)     1066 2023-06-20 02:49:32.000000 BYOD-0.1.0/LICENSE
--rw-r--r--   0 njain17  (14198) njain17  (14198)      246 2023-06-20 03:56:35.000000 BYOD-0.1.0/MANIFEST.in
--rw-r--r--   0 njain17  (14198) njain17  (14198)     3168 2023-06-20 04:06:49.121344 BYOD-0.1.0/PKG-INFO
--rw-r--r--   0 njain17  (14198) njain17  (14198)     2578 2023-06-20 02:54:23.000000 BYOD-0.1.0/README.md
-drwxr-xr-x   0 njain17  (14198) njain17  (14198)        0 2023-06-20 04:06:49.104041 BYOD-0.1.0/images/
--rw-r--r--   0 njain17  (14198) njain17  (14198)   245636 2023-06-20 02:54:23.000000 BYOD-0.1.0/images/Teaser.png
--rw-r--r--   0 njain17  (14198) njain17  (14198)      113 2023-06-20 02:54:23.000000 BYOD-0.1.0/pyproject.toml
--rw-r--r--   0 njain17  (14198) njain17  (14198)       96 2023-06-20 02:54:23.000000 BYOD-0.1.0/requirements.txt
--rw-r--r--   0 njain17  (14198) njain17  (14198)     2506 2023-06-20 02:54:23.000000 BYOD-0.1.0/run_lrs.py
--rw-r--r--   0 njain17  (14198) njain17  (14198)     2674 2023-06-20 02:54:23.000000 BYOD-0.1.0/run_negations.py
--rw-r--r--   0 njain17  (14198) njain17  (14198)     3285 2023-06-20 02:54:23.000000 BYOD-0.1.0/run_tokenization_split.py
--rw-r--r--   0 njain17  (14198) njain17  (14198)     3145 2023-06-20 02:54:23.000000 BYOD-0.1.0/run_toxicity.py
--rw-r--r--   0 njain17  (14198) njain17  (14198)     2498 2023-06-20 02:54:23.000000 BYOD-0.1.0/run_word_order.py
--rw-r--r--   0 njain17  (14198) njain17  (14198)     1561 2023-06-20 04:06:49.125818 BYOD-0.1.0/setup.cfg
+drwxr-xr-x   0 njain17  (14198) njain17  (14198)        0 2023-06-20 04:01:09.004843 BYOD-0.2.0/
+drwxr-xr-x   0 njain17  (14198) njain17  (14198)        0 2023-06-20 04:01:08.718091 BYOD-0.2.0/BYOD/
+drwxr-xr-x   0 njain17  (14198) njain17  (14198)        0 2023-06-20 04:01:08.855538 BYOD-0.2.0/BYOD/List-of-Dirty-Naughty-Obscene-and-Otherwise-Bad-Words/
+-rw-r--r--   0 njain17  (14198) njain17  (14198)     3776 2023-06-20 02:54:23.000000 BYOD-0.2.0/BYOD/List-of-Dirty-Naughty-Obscene-and-Otherwise-Bad-Words/en.txt
+-rw-r--r--   0 njain17  (14198) njain17  (14198)      380 2023-06-20 02:54:23.000000 BYOD-0.2.0/BYOD/__init__.py
+-rw-r--r--   0 njain17  (14198) njain17  (14198)     3683 2023-06-20 02:54:23.000000 BYOD-0.2.0/BYOD/context_sensitivity.py
+-rw-r--r--   0 njain17  (14198) njain17  (14198)     3545 2023-06-20 02:54:23.000000 BYOD-0.2.0/BYOD/negations.py
+-rw-r--r--   0 njain17  (14198) njain17  (14198)     6287 2023-06-20 02:54:23.000000 BYOD-0.2.0/BYOD/tokenization_robustness.py
+-rw-r--r--   0 njain17  (14198) njain17  (14198)    10631 2023-06-20 02:54:23.000000 BYOD-0.2.0/BYOD/toxicity.py
+drwxr-xr-x   0 njain17  (14198) njain17  (14198)        0 2023-06-20 04:01:08.946089 BYOD-0.2.0/BYOD/utils/
+-rw-r--r--   0 njain17  (14198) njain17  (14198)      558 2023-06-20 02:54:23.000000 BYOD-0.2.0/BYOD/utils/JSD.py
+-rw-r--r--   0 njain17  (14198) njain17  (14198)      137 2023-06-20 02:54:23.000000 BYOD-0.2.0/BYOD/utils/__init__.py
+-rw-r--r--   0 njain17  (14198) njain17  (14198)     4163 2023-06-20 02:54:23.000000 BYOD-0.2.0/BYOD/utils/hf_utils.py
+-rw-r--r--   0 njain17  (14198) njain17  (14198)     4540 2023-06-20 02:54:23.000000 BYOD-0.2.0/BYOD/utils/wikiDataset.py
+-rw-r--r--   0 njain17  (14198) njain17  (14198)     4196 2023-06-20 02:54:23.000000 BYOD-0.2.0/BYOD/word_order.py
+drwxr-xr-x   0 njain17  (14198) njain17  (14198)        0 2023-06-20 04:01:08.818096 BYOD-0.2.0/BYOD.egg-info/
+-rw-r--r--   0 njain17  (14198) njain17  (14198)     3168 2023-06-20 04:01:08.000000 BYOD-0.2.0/BYOD.egg-info/PKG-INFO
+-rw-r--r--   0 njain17  (14198) njain17  (14198)      630 2023-06-20 04:01:08.000000 BYOD-0.2.0/BYOD.egg-info/SOURCES.txt
+-rw-r--r--   0 njain17  (14198) njain17  (14198)        1 2023-06-20 04:01:08.000000 BYOD-0.2.0/BYOD.egg-info/dependency_links.txt
+-rw-r--r--   0 njain17  (14198) njain17  (14198)        1 2023-06-20 04:01:08.000000 BYOD-0.2.0/BYOD.egg-info/not-zip-safe
+-rw-r--r--   0 njain17  (14198) njain17  (14198)       97 2023-06-20 04:01:08.000000 BYOD-0.2.0/BYOD.egg-info/requires.txt
+-rw-r--r--   0 njain17  (14198) njain17  (14198)        5 2023-06-20 04:01:08.000000 BYOD-0.2.0/BYOD.egg-info/top_level.txt
+-rw-r--r--   0 njain17  (14198) njain17  (14198)     1066 2023-06-20 02:49:32.000000 BYOD-0.2.0/LICENSE
+-rw-r--r--   0 njain17  (14198) njain17  (14198)      246 2023-06-20 03:56:35.000000 BYOD-0.2.0/MANIFEST.in
+-rw-r--r--   0 njain17  (14198) njain17  (14198)     3168 2023-06-20 04:01:09.006555 BYOD-0.2.0/PKG-INFO
+-rw-r--r--   0 njain17  (14198) njain17  (14198)     2578 2023-06-20 02:54:23.000000 BYOD-0.2.0/README.md
+drwxr-xr-x   0 njain17  (14198) njain17  (14198)        0 2023-06-20 04:01:08.960950 BYOD-0.2.0/images/
+-rw-r--r--   0 njain17  (14198) njain17  (14198)   245636 2023-06-20 02:54:23.000000 BYOD-0.2.0/images/Teaser.png
+-rw-r--r--   0 njain17  (14198) njain17  (14198)      113 2023-06-20 02:54:23.000000 BYOD-0.2.0/pyproject.toml
+-rw-r--r--   0 njain17  (14198) njain17  (14198)       96 2023-06-20 02:54:23.000000 BYOD-0.2.0/requirements.txt
+-rw-r--r--   0 njain17  (14198) njain17  (14198)     2506 2023-06-20 02:54:23.000000 BYOD-0.2.0/run_lrs.py
+-rw-r--r--   0 njain17  (14198) njain17  (14198)     2674 2023-06-20 02:54:23.000000 BYOD-0.2.0/run_negations.py
+-rw-r--r--   0 njain17  (14198) njain17  (14198)     3285 2023-06-20 02:54:23.000000 BYOD-0.2.0/run_tokenization_split.py
+-rw-r--r--   0 njain17  (14198) njain17  (14198)     3145 2023-06-20 02:54:23.000000 BYOD-0.2.0/run_toxicity.py
+-rw-r--r--   0 njain17  (14198) njain17  (14198)     2498 2023-06-20 02:54:23.000000 BYOD-0.2.0/run_word_order.py
+-rw-r--r--   0 njain17  (14198) njain17  (14198)     1561 2023-06-20 04:01:09.010976 BYOD-0.2.0/setup.cfg
```

### Comparing `BYOD-0.1.0/BYOD/List-of-Dirty-Naughty-Obscene-and-Otherwise-Bad-Words/en.txt` & `BYOD-0.2.0/BYOD/List-of-Dirty-Naughty-Obscene-and-Otherwise-Bad-Words/en.txt`

 * *Files identical despite different names*

### Comparing `BYOD-0.1.0/BYOD/context_sensitivity.py` & `BYOD-0.2.0/BYOD/context_sensitivity.py`

 * *Files identical despite different names*

### Comparing `BYOD-0.1.0/BYOD/negations.py` & `BYOD-0.2.0/BYOD/negations.py`

 * *Files identical despite different names*

### Comparing `BYOD-0.1.0/BYOD/tokenization_robustness.py` & `BYOD-0.2.0/BYOD/tokenization_robustness.py`

 * *Files identical despite different names*

### Comparing `BYOD-0.1.0/BYOD/toxicity.py` & `BYOD-0.2.0/BYOD/toxicity.py`

 * *Files identical despite different names*

### Comparing `BYOD-0.1.0/BYOD/utils/JSD.py` & `BYOD-0.2.0/BYOD/utils/JSD.py`

 * *Files identical despite different names*

### Comparing `BYOD-0.1.0/BYOD/utils/hf_utils.py` & `BYOD-0.2.0/BYOD/utils/hf_utils.py`

 * *Files identical despite different names*

### Comparing `BYOD-0.1.0/BYOD/utils/wikiDataset.py` & `BYOD-0.2.0/BYOD/utils/wikiDataset.py`

 * *Files identical despite different names*

### Comparing `BYOD-0.1.0/BYOD/word_order.py` & `BYOD-0.2.0/BYOD/word_order.py`

 * *Files identical despite different names*

### Comparing `BYOD-0.1.0/BYOD.egg-info/PKG-INFO` & `BYOD-0.2.0/BYOD.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BYOD
-Version: 0.1.0
+Version: 0.2.0
 Summary: Bring Your Own Data! A Framework for Self-Supervised Evaluation of Large Language Models
 Home-page: https://github.com/neelsjain/BYOD
 Author: Neel Jain, Khalid Saifullah, Jonas Geiping
 Author-email: njain17@umd.edu
 License: MIT
 Keywords: todo
 Platform: any
```

### Comparing `BYOD-0.1.0/BYOD.egg-info/SOURCES.txt` & `BYOD-0.2.0/BYOD.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BYOD-0.1.0/LICENSE` & `BYOD-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `BYOD-0.1.0/PKG-INFO` & `BYOD-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BYOD
-Version: 0.1.0
+Version: 0.2.0
 Summary: Bring Your Own Data! A Framework for Self-Supervised Evaluation of Large Language Models
 Home-page: https://github.com/neelsjain/BYOD
 Author: Neel Jain, Khalid Saifullah, Jonas Geiping
 Author-email: njain17@umd.edu
 License: MIT
 Keywords: todo
 Platform: any
```

### Comparing `BYOD-0.1.0/README.md` & `BYOD-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `BYOD-0.1.0/images/Teaser.png` & `BYOD-0.2.0/images/Teaser.png`

 * *Files identical despite different names*

### Comparing `BYOD-0.1.0/run_lrs.py` & `BYOD-0.2.0/run_lrs.py`

 * *Files identical despite different names*

### Comparing `BYOD-0.1.0/run_negations.py` & `BYOD-0.2.0/run_negations.py`

 * *Files identical despite different names*

### Comparing `BYOD-0.1.0/run_tokenization_split.py` & `BYOD-0.2.0/run_tokenization_split.py`

 * *Files identical despite different names*

### Comparing `BYOD-0.1.0/run_toxicity.py` & `BYOD-0.2.0/run_toxicity.py`

 * *Files identical despite different names*

### Comparing `BYOD-0.1.0/run_word_order.py` & `BYOD-0.2.0/run_word_order.py`

 * *Files identical despite different names*

### Comparing `BYOD-0.1.0/setup.cfg` & `BYOD-0.2.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = BYOD
-version = 0.1.0
+version = 0.2.0
 author = Neel Jain, Khalid Saifullah, Jonas Geiping
 author_email = njain17@umd.edu
 url = https://github.com/neelsjain/BYOD
 description = Bring Your Own Data! A Framework for Self-Supervised Evaluation of Large Language Models
 long_description = file: README.md, LICENSE.md
 long_description_content_type = text/markdown
 license = MIT
```

