# Comparing `tmp/lrbenchmark-0.1.1.tar.gz` & `tmp/lrbenchmark-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lrbenchmark-0.1.1.tar", last modified: Wed Jun  7 09:00:49 2023, max compression
+gzip compressed data, was "lrbenchmark-0.1.2.tar", last modified: Tue Jun 20 09:19:46 2023, max compression
```

## Comparing `lrbenchmark-0.1.1.tar` & `lrbenchmark-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:00:49.832677 lrbenchmark-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-06-07 09:00:38.000000 lrbenchmark-0.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-06-07 09:00:49.832677 lrbenchmark-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-06-07 09:00:38.000000 lrbenchmark-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:00:49.832677 lrbenchmark-0.1.1/lrbenchmark/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 09:00:38.000000 lrbenchmark-0.1.1/lrbenchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-06-07 09:00:38.000000 lrbenchmark-0.1.1/lrbenchmark/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-06-07 09:00:38.000000 lrbenchmark-0.1.1/lrbenchmark/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-07 09:00:38.000000 lrbenchmark-0.1.1/lrbenchmark/transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-07 09:00:38.000000 lrbenchmark-0.1.1/lrbenchmark/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-07 09:00:38.000000 lrbenchmark-0.1.1/lrbenchmark/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:00:49.832677 lrbenchmark-0.1.1/lrbenchmark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-06-07 09:00:49.000000 lrbenchmark-0.1.1/lrbenchmark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-07 09:00:49.000000 lrbenchmark-0.1.1/lrbenchmark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 09:00:49.000000 lrbenchmark-0.1.1/lrbenchmark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-07 09:00:49.000000 lrbenchmark-0.1.1/lrbenchmark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-07 09:00:49.000000 lrbenchmark-0.1.1/lrbenchmark.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 09:00:49.832677 lrbenchmark-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-07 09:00:38.000000 lrbenchmark-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:00:49.832677 lrbenchmark-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-07 09:00:38.000000 lrbenchmark-0.1.1/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-07 09:00:38.000000 lrbenchmark-0.1.1/tests/test_transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:19:46.238809 lrbenchmark-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-06-20 09:19:35.000000 lrbenchmark-0.1.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-06-20 09:19:46.234809 lrbenchmark-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-06-20 09:19:35.000000 lrbenchmark-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:19:46.234809 lrbenchmark-0.1.2/lrbenchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 09:19:35.000000 lrbenchmark-0.1.2/lrbenchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-06-20 09:19:35.000000 lrbenchmark-0.1.2/lrbenchmark/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-06-20 09:19:35.000000 lrbenchmark-0.1.2/lrbenchmark/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-20 09:19:35.000000 lrbenchmark-0.1.2/lrbenchmark/transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-20 09:19:35.000000 lrbenchmark-0.1.2/lrbenchmark/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-20 09:19:35.000000 lrbenchmark-0.1.2/lrbenchmark/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:19:46.234809 lrbenchmark-0.1.2/lrbenchmark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-06-20 09:19:46.000000 lrbenchmark-0.1.2/lrbenchmark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-20 09:19:46.000000 lrbenchmark-0.1.2/lrbenchmark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 09:19:46.000000 lrbenchmark-0.1.2/lrbenchmark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-20 09:19:46.000000 lrbenchmark-0.1.2/lrbenchmark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-20 09:19:46.000000 lrbenchmark-0.1.2/lrbenchmark.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 09:19:46.238809 lrbenchmark-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-20 09:19:35.000000 lrbenchmark-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:19:46.234809 lrbenchmark-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-20 09:19:35.000000 lrbenchmark-0.1.2/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-20 09:19:35.000000 lrbenchmark-0.1.2/tests/test_transformers.py
```

### Comparing `lrbenchmark-0.1.1/LICENSE.txt` & `lrbenchmark-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lrbenchmark-0.1.1/PKG-INFO` & `lrbenchmark-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lrbenchmark
-Version: 0.1.1
+Version: 0.1.2
 Summary: Benchmarking Likelihood Ratio systems
 Author: Netherlands Forensics Institute
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 LRBenchmark
 =====
```

### Comparing `lrbenchmark-0.1.1/README.md` & `lrbenchmark-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `lrbenchmark-0.1.1/lrbenchmark/dataset.py` & `lrbenchmark-0.1.2/lrbenchmark/dataset.py`

 * *Files identical despite different names*

### Comparing `lrbenchmark-0.1.1/lrbenchmark/evaluation.py` & `lrbenchmark-0.1.2/lrbenchmark/evaluation.py`

 * *Files identical despite different names*

### Comparing `lrbenchmark-0.1.1/lrbenchmark/transformers.py` & `lrbenchmark-0.1.2/lrbenchmark/transformers.py`

 * *Files identical despite different names*

### Comparing `lrbenchmark-0.1.1/lrbenchmark/utils.py` & `lrbenchmark-0.1.2/lrbenchmark/utils.py`

 * *Files identical despite different names*

### Comparing `lrbenchmark-0.1.1/lrbenchmark.egg-info/PKG-INFO` & `lrbenchmark-0.1.2/lrbenchmark.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lrbenchmark
-Version: 0.1.1
+Version: 0.1.2
 Summary: Benchmarking Likelihood Ratio systems
 Author: Netherlands Forensics Institute
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 LRBenchmark
 =====
```

### Comparing `lrbenchmark-0.1.1/setup.py` & `lrbenchmark-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 long_description = (Path(__file__).parent / 'README.md').read_text()
 
 
 dependencies = (
     'confidence',
     'pytest',
     'matplotlib',
-    'sklearn',
+    'scikit-learn',
     'lir',
     'pandas',
     'xgboost',
     'more-itertools'
 )
 
 
 setup(
     name='lrbenchmark',
-    version='0.1.1',
+    version='0.1.2',
     author='Netherlands Forensics Institute',
     description='Benchmarking Likelihood Ratio systems',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=dependencies,
 )
```

### Comparing `lrbenchmark-0.1.1/tests/test_dataset.py` & `lrbenchmark-0.1.2/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `lrbenchmark-0.1.1/tests/test_transformers.py` & `lrbenchmark-0.1.2/tests/test_transformers.py`

 * *Files identical despite different names*

