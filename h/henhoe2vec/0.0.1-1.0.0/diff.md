# Comparing `tmp/henhoe2vec-0.0.1.tar.gz` & `tmp/henhoe2vec-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "henhoe2vec-0.0.1.tar", last modified: Tue Jun 20 08:08:18 2023, max compression
+gzip compressed data, was "henhoe2vec-1.0.0.tar", last modified: Tue Jun 20 08:11:48 2023, max compression
```

## Comparing `henhoe2vec-0.0.1.tar` & `henhoe2vec-1.0.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 bob        (501) staff       (20)        0 2023-06-20 08:08:18.638977 henhoe2vec-0.0.1/
--rw-r--r--   0 bob        (501) staff       (20)     1071 2023-06-08 16:39:49.000000 henhoe2vec-0.0.1/LICENSE.txt
--rw-r--r--   0 bob        (501) staff       (20)     6892 2023-06-20 08:08:18.638815 henhoe2vec-0.0.1/PKG-INFO
--rw-r--r--   0 bob        (501) staff       (20)     4741 2023-06-13 09:45:20.000000 henhoe2vec-0.0.1/README.md
--rw-r--r--   0 bob        (501) staff       (20)     1199 2023-06-20 08:07:51.000000 henhoe2vec-0.0.1/pyproject.toml
--rw-r--r--   0 bob        (501) staff       (20)       38 2023-06-20 08:08:18.639022 henhoe2vec-0.0.1/setup.cfg
--rw-r--r--   0 bob        (501) staff       (20)       38 2023-06-13 07:41:13.000000 henhoe2vec-0.0.1/setup.py
-drwxr-xr-x   0 bob        (501) staff       (20)        0 2023-06-20 08:08:18.634440 henhoe2vec-0.0.1/src/
-drwxr-xr-x   0 bob        (501) staff       (20)        0 2023-06-20 08:08:18.636026 henhoe2vec-0.0.1/src/henhoe2vec/
--rw-r--r--   0 bob        (501) staff       (20)       78 2023-06-11 08:46:34.000000 henhoe2vec-0.0.1/src/henhoe2vec/__init__.py
--rw-r--r--   0 bob        (501) staff       (20)     2188 2023-06-10 19:24:50.000000 henhoe2vec-0.0.1/src/henhoe2vec/alias_sampling.py
--rw-r--r--   0 bob        (501) staff       (20)     1820 2023-06-11 08:32:37.000000 henhoe2vec-0.0.1/src/henhoe2vec/embeddings.py
--rw-r--r--   0 bob        (501) staff       (20)     9515 2023-06-13 08:03:06.000000 henhoe2vec-0.0.1/src/henhoe2vec/henhoe2vec.py
--rw-r--r--   0 bob        (501) staff       (20)    12288 2023-06-10 22:17:49.000000 henhoe2vec-0.0.1/src/henhoe2vec/henhoe2vec_walks.py
--rw-r--r--   0 bob        (501) staff       (20)      573 2023-06-10 21:52:42.000000 henhoe2vec-0.0.1/src/henhoe2vec/napkin.py
--rw-r--r--   0 bob        (501) staff       (20)     5262 2023-06-17 08:10:10.000000 henhoe2vec-0.0.1/src/henhoe2vec/utils.py
-drwxr-xr-x   0 bob        (501) staff       (20)        0 2023-06-20 08:08:18.636679 henhoe2vec-0.0.1/src/henhoe2vec.egg-info/
--rw-r--r--   0 bob        (501) staff       (20)     6892 2023-06-20 08:08:18.000000 henhoe2vec-0.0.1/src/henhoe2vec.egg-info/PKG-INFO
--rw-r--r--   0 bob        (501) staff       (20)      566 2023-06-20 08:08:18.000000 henhoe2vec-0.0.1/src/henhoe2vec.egg-info/SOURCES.txt
--rw-r--r--   0 bob        (501) staff       (20)        1 2023-06-20 08:08:18.000000 henhoe2vec-0.0.1/src/henhoe2vec.egg-info/dependency_links.txt
--rw-r--r--   0 bob        (501) staff       (20)       76 2023-06-20 08:08:18.000000 henhoe2vec-0.0.1/src/henhoe2vec.egg-info/requires.txt
--rw-r--r--   0 bob        (501) staff       (20)       11 2023-06-20 08:08:18.000000 henhoe2vec-0.0.1/src/henhoe2vec.egg-info/top_level.txt
-drwxr-xr-x   0 bob        (501) staff       (20)        0 2023-06-20 08:08:18.638439 henhoe2vec-0.0.1/tests/
--rw-r--r--   0 bob        (501) staff       (20)     1095 2023-06-10 22:18:24.000000 henhoe2vec-0.0.1/tests/test_alias_sampling.py
--rw-r--r--   0 bob        (501) staff       (20)      764 2023-06-10 22:18:24.000000 henhoe2vec-0.0.1/tests/test_embeddings.py
--rw-r--r--   0 bob        (501) staff       (20)     2171 2023-06-14 09:26:45.000000 henhoe2vec-0.0.1/tests/test_henhoe2vec.py
--rw-r--r--   0 bob        (501) staff       (20)     3913 2023-06-10 22:18:24.000000 henhoe2vec-0.0.1/tests/test_henhoe2vec_walks.py
--rw-r--r--   0 bob        (501) staff       (20)     4215 2023-06-17 08:08:24.000000 henhoe2vec-0.0.1/tests/test_utils.py
+drwxr-xr-x   0 bob        (501) staff       (20)        0 2023-06-20 08:11:48.688804 henhoe2vec-1.0.0/
+-rw-r--r--   0 bob        (501) staff       (20)     1071 2023-06-08 16:39:49.000000 henhoe2vec-1.0.0/LICENSE.txt
+-rw-r--r--   0 bob        (501) staff       (20)     6892 2023-06-20 08:11:48.688666 henhoe2vec-1.0.0/PKG-INFO
+-rw-r--r--   0 bob        (501) staff       (20)     4741 2023-06-13 09:45:20.000000 henhoe2vec-1.0.0/README.md
+-rw-r--r--   0 bob        (501) staff       (20)     1199 2023-06-20 08:11:39.000000 henhoe2vec-1.0.0/pyproject.toml
+-rw-r--r--   0 bob        (501) staff       (20)       38 2023-06-20 08:11:48.688850 henhoe2vec-1.0.0/setup.cfg
+-rw-r--r--   0 bob        (501) staff       (20)       38 2023-06-13 07:41:13.000000 henhoe2vec-1.0.0/setup.py
+drwxr-xr-x   0 bob        (501) staff       (20)        0 2023-06-20 08:11:48.685393 henhoe2vec-1.0.0/src/
+drwxr-xr-x   0 bob        (501) staff       (20)        0 2023-06-20 08:11:48.686903 henhoe2vec-1.0.0/src/henhoe2vec/
+-rw-r--r--   0 bob        (501) staff       (20)       78 2023-06-11 08:46:34.000000 henhoe2vec-1.0.0/src/henhoe2vec/__init__.py
+-rw-r--r--   0 bob        (501) staff       (20)     2188 2023-06-10 19:24:50.000000 henhoe2vec-1.0.0/src/henhoe2vec/alias_sampling.py
+-rw-r--r--   0 bob        (501) staff       (20)     1820 2023-06-11 08:32:37.000000 henhoe2vec-1.0.0/src/henhoe2vec/embeddings.py
+-rw-r--r--   0 bob        (501) staff       (20)     9515 2023-06-13 08:03:06.000000 henhoe2vec-1.0.0/src/henhoe2vec/henhoe2vec.py
+-rw-r--r--   0 bob        (501) staff       (20)    12288 2023-06-10 22:17:49.000000 henhoe2vec-1.0.0/src/henhoe2vec/henhoe2vec_walks.py
+-rw-r--r--   0 bob        (501) staff       (20)      573 2023-06-10 21:52:42.000000 henhoe2vec-1.0.0/src/henhoe2vec/napkin.py
+-rw-r--r--   0 bob        (501) staff       (20)     5262 2023-06-17 08:10:10.000000 henhoe2vec-1.0.0/src/henhoe2vec/utils.py
+drwxr-xr-x   0 bob        (501) staff       (20)        0 2023-06-20 08:11:48.687690 henhoe2vec-1.0.0/src/henhoe2vec.egg-info/
+-rw-r--r--   0 bob        (501) staff       (20)     6892 2023-06-20 08:11:48.000000 henhoe2vec-1.0.0/src/henhoe2vec.egg-info/PKG-INFO
+-rw-r--r--   0 bob        (501) staff       (20)      566 2023-06-20 08:11:48.000000 henhoe2vec-1.0.0/src/henhoe2vec.egg-info/SOURCES.txt
+-rw-r--r--   0 bob        (501) staff       (20)        1 2023-06-20 08:11:48.000000 henhoe2vec-1.0.0/src/henhoe2vec.egg-info/dependency_links.txt
+-rw-r--r--   0 bob        (501) staff       (20)       76 2023-06-20 08:11:48.000000 henhoe2vec-1.0.0/src/henhoe2vec.egg-info/requires.txt
+-rw-r--r--   0 bob        (501) staff       (20)       11 2023-06-20 08:11:48.000000 henhoe2vec-1.0.0/src/henhoe2vec.egg-info/top_level.txt
+drwxr-xr-x   0 bob        (501) staff       (20)        0 2023-06-20 08:11:48.688421 henhoe2vec-1.0.0/tests/
+-rw-r--r--   0 bob        (501) staff       (20)     1095 2023-06-10 22:18:24.000000 henhoe2vec-1.0.0/tests/test_alias_sampling.py
+-rw-r--r--   0 bob        (501) staff       (20)      764 2023-06-10 22:18:24.000000 henhoe2vec-1.0.0/tests/test_embeddings.py
+-rw-r--r--   0 bob        (501) staff       (20)     2171 2023-06-14 09:26:45.000000 henhoe2vec-1.0.0/tests/test_henhoe2vec.py
+-rw-r--r--   0 bob        (501) staff       (20)     3913 2023-06-10 22:18:24.000000 henhoe2vec-1.0.0/tests/test_henhoe2vec_walks.py
+-rw-r--r--   0 bob        (501) staff       (20)     4215 2023-06-17 08:08:24.000000 henhoe2vec-1.0.0/tests/test_utils.py
```

### Comparing `henhoe2vec-0.0.1/LICENSE.txt` & `henhoe2vec-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `henhoe2vec-0.0.1/PKG-INFO` & `henhoe2vec-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: henhoe2vec
-Version: 0.0.1
+Version: 1.0.0
 Summary: Implementation of the HeNHoE-2vec algorithm by Valentini et al. (2021).
 Author-email: Robert Giesler <robert.giesler@rwth-aachen.de>
 License: MIT License
         
         Copyright (c) 2023 Robert Giesler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `henhoe2vec-0.0.1/README.md` & `henhoe2vec-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `henhoe2vec-0.0.1/pyproject.toml` & `henhoe2vec-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "henhoe2vec"
-version = "0.0.1"
+version = "1.0.0"
 description = "Implementation of the HeNHoE-2vec algorithm by Valentini et al. (2021)."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE.txt"}
 authors = [
     {name = "Robert Giesler", email = "robert.giesler@rwth-aachen.de"}
 ]
```

### Comparing `henhoe2vec-0.0.1/src/henhoe2vec/alias_sampling.py` & `henhoe2vec-1.0.0/src/henhoe2vec/alias_sampling.py`

 * *Files identical despite different names*

### Comparing `henhoe2vec-0.0.1/src/henhoe2vec/embeddings.py` & `henhoe2vec-1.0.0/src/henhoe2vec/embeddings.py`

 * *Files identical despite different names*

### Comparing `henhoe2vec-0.0.1/src/henhoe2vec/henhoe2vec.py` & `henhoe2vec-1.0.0/src/henhoe2vec/henhoe2vec.py`

 * *Files identical despite different names*

### Comparing `henhoe2vec-0.0.1/src/henhoe2vec/henhoe2vec_walks.py` & `henhoe2vec-1.0.0/src/henhoe2vec/henhoe2vec_walks.py`

 * *Files identical despite different names*

### Comparing `henhoe2vec-0.0.1/src/henhoe2vec/napkin.py` & `henhoe2vec-1.0.0/src/henhoe2vec/napkin.py`

 * *Files identical despite different names*

### Comparing `henhoe2vec-0.0.1/src/henhoe2vec/utils.py` & `henhoe2vec-1.0.0/src/henhoe2vec/utils.py`

 * *Files identical despite different names*

### Comparing `henhoe2vec-0.0.1/src/henhoe2vec.egg-info/PKG-INFO` & `henhoe2vec-1.0.0/src/henhoe2vec.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: henhoe2vec
-Version: 0.0.1
+Version: 1.0.0
 Summary: Implementation of the HeNHoE-2vec algorithm by Valentini et al. (2021).
 Author-email: Robert Giesler <robert.giesler@rwth-aachen.de>
 License: MIT License
         
         Copyright (c) 2023 Robert Giesler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `henhoe2vec-0.0.1/src/henhoe2vec.egg-info/SOURCES.txt` & `henhoe2vec-1.0.0/src/henhoe2vec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `henhoe2vec-0.0.1/tests/test_alias_sampling.py` & `henhoe2vec-1.0.0/tests/test_alias_sampling.py`

 * *Files identical despite different names*

### Comparing `henhoe2vec-0.0.1/tests/test_embeddings.py` & `henhoe2vec-1.0.0/tests/test_embeddings.py`

 * *Files identical despite different names*

### Comparing `henhoe2vec-0.0.1/tests/test_henhoe2vec.py` & `henhoe2vec-1.0.0/tests/test_henhoe2vec.py`

 * *Files identical despite different names*

### Comparing `henhoe2vec-0.0.1/tests/test_henhoe2vec_walks.py` & `henhoe2vec-1.0.0/tests/test_henhoe2vec_walks.py`

 * *Files identical despite different names*

### Comparing `henhoe2vec-0.0.1/tests/test_utils.py` & `henhoe2vec-1.0.0/tests/test_utils.py`

 * *Files identical despite different names*

