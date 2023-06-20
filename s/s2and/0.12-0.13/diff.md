# Comparing `tmp/s2and-0.12.tar.gz` & `tmp/s2and-0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s2and-0.12.tar", last modified: Tue Jun 20 17:01:48 2023, max compression
+gzip compressed data, was "s2and-0.13.tar", last modified: Tue Jun 20 17:15:48 2023, max compression
```

## Comparing `s2and-0.12.tar` & `s2and-0.13.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-06-20 17:01:48.767552 s2and-0.12/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    13134 2023-06-05 12:41:33.000000 s2and-0.12/LICENSE
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      114 2023-06-20 17:01:48.767364 s2and-0.12/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     9477 2023-06-14 16:26:22.000000 s2and-0.12/README.md
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-06-20 17:01:48.765433 s2and-0.12/s2and/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      272 2023-06-05 12:41:33.000000 s2and-0.12/s2and/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1762 2023-06-05 12:41:33.000000 s2and-0.12/s2and/consts.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    63074 2023-06-18 17:05:48.000000 s2and-0.12/s2and/data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    42585 2023-06-18 18:44:33.000000 s2and-0.12/s2and/eval.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    29361 2023-06-13 11:14:21.000000 s2and-0.12/s2and/featurizer.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4866 2023-06-05 12:41:33.000000 s2and-0.12/s2and/file_cache.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    48434 2023-06-18 16:18:01.000000 s2and-0.12/s2and/model.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     8210 2023-06-05 12:41:33.000000 s2and-0.12/s2and/plotting_utils.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     9806 2023-06-05 12:41:33.000000 s2and-0.12/s2and/s2_funcs.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     3969 2023-06-05 12:41:33.000000 s2and-0.12/s2and/sampling.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    16550 2023-06-05 12:41:33.000000 s2and-0.12/s2and/text.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-06-20 17:01:48.766094 s2and-0.12/s2and.egg-info/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      114 2023-06-20 17:01:48.000000 s2and-0.12/s2and.egg-info/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      587 2023-06-20 17:01:48.000000 s2and-0.12/s2and.egg-info/SOURCES.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-06-20 17:01:48.000000 s2and-0.12/s2and.egg-info/dependency_links.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      260 2023-06-20 17:01:48.000000 s2and-0.12/s2and.egg-info/requires.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       12 2023-06-20 17:01:48.000000 s2and-0.12/s2and.egg-info/top_level.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-06-20 17:01:48.767598 s2and-0.12/setup.cfg
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      444 2023-06-20 17:01:46.000000 s2and-0.12/setup.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-06-20 17:01:48.767207 s2and-0.12/tests/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-06-05 12:41:33.000000 s2and-0.12/tests/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     3035 2023-06-05 12:41:33.000000 s2and-0.12/tests/test_cluster.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2437 2023-06-05 12:41:33.000000 s2and-0.12/tests/test_cluster_incremental.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     3368 2023-06-05 12:41:33.000000 s2and-0.12/tests/test_cluster_incremental_incompatible.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     7541 2023-06-05 12:41:33.000000 s2and-0.12/tests/test_data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-06-05 12:41:33.000000 s2and-0.12/tests/test_eval.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4757 2023-06-05 12:41:33.000000 s2and-0.12/tests/test_featurizer.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2981 2023-06-05 12:41:33.000000 s2and-0.12/tests/test_s2_funcs.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4725 2023-06-05 12:41:33.000000 s2and-0.12/tests/test_text.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-06-20 17:15:48.438523 s2and-0.13/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    13134 2023-06-05 12:41:33.000000 s2and-0.13/LICENSE
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      114 2023-06-20 17:15:48.438320 s2and-0.13/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     9477 2023-06-14 16:26:22.000000 s2and-0.13/README.md
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-06-20 17:15:48.435833 s2and-0.13/s2and/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      272 2023-06-05 12:41:33.000000 s2and-0.13/s2and/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1762 2023-06-05 12:41:33.000000 s2and-0.13/s2and/consts.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    63074 2023-06-18 17:05:48.000000 s2and-0.13/s2and/data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    42585 2023-06-18 18:44:33.000000 s2and-0.13/s2and/eval.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    29361 2023-06-13 11:14:21.000000 s2and-0.13/s2and/featurizer.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4866 2023-06-05 12:41:33.000000 s2and-0.13/s2and/file_cache.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      897 2023-06-20 17:12:18.000000 s2and-0.13/s2and/inference.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    48434 2023-06-18 16:18:01.000000 s2and-0.13/s2and/model.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     8210 2023-06-05 12:41:33.000000 s2and-0.13/s2and/plotting_utils.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     9806 2023-06-05 12:41:33.000000 s2and-0.13/s2and/s2_funcs.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     3969 2023-06-05 12:41:33.000000 s2and-0.13/s2and/sampling.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    16550 2023-06-05 12:41:33.000000 s2and-0.13/s2and/text.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-06-20 17:15:48.436560 s2and-0.13/s2and.egg-info/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      114 2023-06-20 17:15:48.000000 s2and-0.13/s2and.egg-info/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      606 2023-06-20 17:15:48.000000 s2and-0.13/s2and.egg-info/SOURCES.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-06-20 17:15:48.000000 s2and-0.13/s2and.egg-info/dependency_links.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      260 2023-06-20 17:15:48.000000 s2and-0.13/s2and.egg-info/requires.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       12 2023-06-20 17:15:48.000000 s2and-0.13/s2and.egg-info/top_level.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-06-20 17:15:48.438561 s2and-0.13/setup.cfg
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      444 2023-06-20 17:12:38.000000 s2and-0.13/setup.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-06-20 17:15:48.438135 s2and-0.13/tests/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-06-05 12:41:33.000000 s2and-0.13/tests/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     3035 2023-06-05 12:41:33.000000 s2and-0.13/tests/test_cluster.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2437 2023-06-05 12:41:33.000000 s2and-0.13/tests/test_cluster_incremental.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     3368 2023-06-05 12:41:33.000000 s2and-0.13/tests/test_cluster_incremental_incompatible.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     7541 2023-06-05 12:41:33.000000 s2and-0.13/tests/test_data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-06-05 12:41:33.000000 s2and-0.13/tests/test_eval.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4757 2023-06-05 12:41:33.000000 s2and-0.13/tests/test_featurizer.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2981 2023-06-05 12:41:33.000000 s2and-0.13/tests/test_s2_funcs.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4725 2023-06-05 12:41:33.000000 s2and-0.13/tests/test_text.py
```

### Comparing `s2and-0.12/LICENSE` & `s2and-0.13/LICENSE`

 * *Files identical despite different names*

### Comparing `s2and-0.12/README.md` & `s2and-0.13/README.md`

 * *Files identical despite different names*

### Comparing `s2and-0.12/s2and/consts.py` & `s2and-0.13/s2and/consts.py`

 * *Files identical despite different names*

### Comparing `s2and-0.12/s2and/data.py` & `s2and-0.13/s2and/data.py`

 * *Files identical despite different names*

### Comparing `s2and-0.12/s2and/eval.py` & `s2and-0.13/s2and/eval.py`

 * *Files identical despite different names*

### Comparing `s2and-0.12/s2and/featurizer.py` & `s2and-0.13/s2and/featurizer.py`

 * *Files identical despite different names*

### Comparing `s2and-0.12/s2and/file_cache.py` & `s2and-0.13/s2and/file_cache.py`

 * *Files identical despite different names*

### Comparing `s2and-0.12/s2and/model.py` & `s2and-0.13/s2and/model.py`

 * *Files identical despite different names*

### Comparing `s2and-0.12/s2and/plotting_utils.py` & `s2and-0.13/s2and/plotting_utils.py`

 * *Files identical despite different names*

### Comparing `s2and-0.12/s2and/s2_funcs.py` & `s2and-0.13/s2and/s2_funcs.py`

 * *Files identical despite different names*

### Comparing `s2and-0.12/s2and/sampling.py` & `s2and-0.13/s2and/sampling.py`

 * *Files identical despite different names*

### Comparing `s2and-0.12/s2and/text.py` & `s2and-0.13/s2and/text.py`

 * *Files identical despite different names*

### Comparing `s2and-0.12/s2and.egg-info/SOURCES.txt` & `s2and-0.13/s2and.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 setup.py
 s2and/__init__.py
 s2and/consts.py
 s2and/data.py
 s2and/eval.py
 s2and/featurizer.py
 s2and/file_cache.py
+s2and/inference.py
 s2and/model.py
 s2and/plotting_utils.py
 s2and/s2_funcs.py
 s2and/sampling.py
 s2and/text.py
 s2and.egg-info/PKG-INFO
 s2and.egg-info/SOURCES.txt
```

### Comparing `s2and-0.12/tests/test_cluster.py` & `s2and-0.13/tests/test_cluster.py`

 * *Files identical despite different names*

### Comparing `s2and-0.12/tests/test_cluster_incremental.py` & `s2and-0.13/tests/test_cluster_incremental.py`

 * *Files identical despite different names*

### Comparing `s2and-0.12/tests/test_cluster_incremental_incompatible.py` & `s2and-0.13/tests/test_cluster_incremental_incompatible.py`

 * *Files identical despite different names*

### Comparing `s2and-0.12/tests/test_data.py` & `s2and-0.13/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `s2and-0.12/tests/test_eval.py` & `s2and-0.13/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `s2and-0.12/tests/test_featurizer.py` & `s2and-0.13/tests/test_featurizer.py`

 * *Files identical despite different names*

### Comparing `s2and-0.12/tests/test_s2_funcs.py` & `s2and-0.13/tests/test_s2_funcs.py`

 * *Files identical despite different names*

### Comparing `s2and-0.12/tests/test_text.py` & `s2and-0.13/tests/test_text.py`

 * *Files identical despite different names*

