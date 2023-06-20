# Comparing `tmp/salesgpt-0.0.1.tar.gz` & `tmp/salesgpt-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salesgpt-0.0.1.tar", last modified: Mon Jun 19 23:44:33 2023, max compression
+gzip compressed data, was "salesgpt-0.0.2.tar", last modified: Tue Jun 20 00:06:28 2023, max compression
```

## Comparing `salesgpt-0.0.1.tar` & `salesgpt-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 filipmichalsky   (501) staff       (20)        0 2023-06-19 23:44:33.805763 salesgpt-0.0.1/
--rw-r--r--   0 filipmichalsky   (501) staff       (20)    11348 2023-06-19 20:25:54.000000 salesgpt-0.0.1/LICENSE
--rw-r--r--   0 filipmichalsky   (501) staff       (20)     6762 2023-06-19 23:44:33.805311 salesgpt-0.0.1/PKG-INFO
--rw-r--r--   0 filipmichalsky   (501) staff       (20)     5977 2023-06-19 21:49:25.000000 salesgpt-0.0.1/README.md
-drwxr-xr-x   0 filipmichalsky   (501) staff       (20)        0 2023-06-19 23:44:33.802570 salesgpt-0.0.1/salesgpt/
--rw-r--r--   0 filipmichalsky   (501) staff       (20)        0 2023-06-19 20:44:34.000000 salesgpt-0.0.1/salesgpt/__init__.py
--rw-r--r--   0 filipmichalsky   (501) staff       (20)     7853 2023-06-19 21:56:51.000000 salesgpt-0.0.1/salesgpt/agents.py
--rw-r--r--   0 filipmichalsky   (501) staff       (20)     6447 2023-06-19 21:56:32.000000 salesgpt-0.0.1/salesgpt/chains.py
--rw-r--r--   0 filipmichalsky   (501) staff       (20)     1119 2023-06-19 21:56:51.000000 salesgpt-0.0.1/salesgpt/logger.py
--rw-r--r--   0 filipmichalsky   (501) staff       (20)     1606 2023-06-19 21:56:32.000000 salesgpt-0.0.1/salesgpt/stages.py
--rw-r--r--   0 filipmichalsky   (501) staff       (20)       50 2023-06-19 23:42:58.000000 salesgpt-0.0.1/salesgpt/version.py
-drwxr-xr-x   0 filipmichalsky   (501) staff       (20)        0 2023-06-19 23:44:33.804429 salesgpt-0.0.1/salesgpt.egg-info/
--rw-r--r--   0 filipmichalsky   (501) staff       (20)     6762 2023-06-19 23:44:33.000000 salesgpt-0.0.1/salesgpt.egg-info/PKG-INFO
--rw-r--r--   0 filipmichalsky   (501) staff       (20)      325 2023-06-19 23:44:33.000000 salesgpt-0.0.1/salesgpt.egg-info/SOURCES.txt
--rw-r--r--   0 filipmichalsky   (501) staff       (20)        1 2023-06-19 23:44:33.000000 salesgpt-0.0.1/salesgpt.egg-info/dependency_links.txt
--rw-r--r--   0 filipmichalsky   (501) staff       (20)      157 2023-06-19 23:44:33.000000 salesgpt-0.0.1/salesgpt.egg-info/requires.txt
--rw-r--r--   0 filipmichalsky   (501) staff       (20)        9 2023-06-19 23:44:33.000000 salesgpt-0.0.1/salesgpt.egg-info/top_level.txt
--rw-r--r--   0 filipmichalsky   (501) staff       (20)       38 2023-06-19 23:44:33.805839 salesgpt-0.0.1/setup.cfg
--rw-r--r--   0 filipmichalsky   (501) staff       (20)     1936 2023-06-19 23:42:45.000000 salesgpt-0.0.1/setup.py
-drwxr-xr-x   0 filipmichalsky   (501) staff       (20)        0 2023-06-19 23:44:33.804747 salesgpt-0.0.1/tests/
--rw-r--r--   0 filipmichalsky   (501) staff       (20)     1585 2023-06-19 21:57:47.000000 salesgpt-0.0.1/tests/test_salesgpt.py
+drwxr-xr-x   0 filipmichalsky   (501) staff       (20)        0 2023-06-20 00:06:28.434035 salesgpt-0.0.2/
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)     1071 2023-06-19 23:47:34.000000 salesgpt-0.0.2/LICENSE
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)       24 2023-06-20 00:03:48.000000 salesgpt-0.0.2/MANIFEST.in
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)     6750 2023-06-20 00:06:28.433789 salesgpt-0.0.2/PKG-INFO
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)     5977 2023-06-19 21:49:25.000000 salesgpt-0.0.2/README.md
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)      103 2023-06-19 21:56:21.000000 salesgpt-0.0.2/requirements.txt
+drwxr-xr-x   0 filipmichalsky   (501) staff       (20)        0 2023-06-20 00:06:28.431345 salesgpt-0.0.2/salesgpt/
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)        0 2023-06-19 20:44:34.000000 salesgpt-0.0.2/salesgpt/__init__.py
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)     7853 2023-06-19 21:56:51.000000 salesgpt-0.0.2/salesgpt/agents.py
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)     6447 2023-06-19 21:56:32.000000 salesgpt-0.0.2/salesgpt/chains.py
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)     1119 2023-06-19 21:56:51.000000 salesgpt-0.0.2/salesgpt/logger.py
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)     1606 2023-06-19 21:56:32.000000 salesgpt-0.0.2/salesgpt/stages.py
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)       50 2023-06-20 00:06:07.000000 salesgpt-0.0.2/salesgpt/version.py
+drwxr-xr-x   0 filipmichalsky   (501) staff       (20)        0 2023-06-20 00:06:28.432909 salesgpt-0.0.2/salesgpt.egg-info/
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)     6750 2023-06-20 00:06:28.000000 salesgpt-0.0.2/salesgpt.egg-info/PKG-INFO
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)      354 2023-06-20 00:06:28.000000 salesgpt-0.0.2/salesgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)        1 2023-06-20 00:06:28.000000 salesgpt-0.0.2/salesgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)      157 2023-06-20 00:06:28.000000 salesgpt-0.0.2/salesgpt.egg-info/requires.txt
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)        9 2023-06-20 00:06:28.000000 salesgpt-0.0.2/salesgpt.egg-info/top_level.txt
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)       38 2023-06-20 00:06:28.434287 salesgpt-0.0.2/setup.cfg
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)     1924 2023-06-20 00:03:32.000000 salesgpt-0.0.2/setup.py
+drwxr-xr-x   0 filipmichalsky   (501) staff       (20)        0 2023-06-20 00:06:28.433184 salesgpt-0.0.2/tests/
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)     1585 2023-06-19 21:57:47.000000 salesgpt-0.0.2/tests/test_salesgpt.py
```

### Comparing `salesgpt-0.0.1/PKG-INFO` & `salesgpt-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: salesgpt
-Version: 0.0.1
+Version: 0.0.2
 Summary: SalesGPT - Your Context-Aware AI Sales Assistant
 Home-page: https://github.com/filip-michalsky/SalesGPT
 Author: Filip Michalsky
 License: Apache 2.0
 Keywords: openai sales gpt autonomous agi
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `salesgpt-0.0.1/README.md` & `salesgpt-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `salesgpt-0.0.1/salesgpt/agents.py` & `salesgpt-0.0.2/salesgpt/agents.py`

 * *Files identical despite different names*

### Comparing `salesgpt-0.0.1/salesgpt/chains.py` & `salesgpt-0.0.2/salesgpt/chains.py`

 * *Files identical despite different names*

### Comparing `salesgpt-0.0.1/salesgpt/logger.py` & `salesgpt-0.0.2/salesgpt/logger.py`

 * *Files identical despite different names*

### Comparing `salesgpt-0.0.1/salesgpt/stages.py` & `salesgpt-0.0.2/salesgpt/stages.py`

 * *Files identical despite different names*

### Comparing `salesgpt-0.0.1/salesgpt.egg-info/PKG-INFO` & `salesgpt-0.0.2/salesgpt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: salesgpt
-Version: 0.0.1
+Version: 0.0.2
 Summary: SalesGPT - Your Context-Aware AI Sales Assistant
 Home-page: https://github.com/filip-michalsky/SalesGPT
 Author: Filip Michalsky
 License: Apache 2.0
 Keywords: openai sales gpt autonomous agi
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `salesgpt-0.0.1/setup.py` & `salesgpt-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     author="Filip Michalsky",
     url="https://github.com/filip-michalsky/SalesGPT",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
-        "License :: OSI Approved :: Apache Software License",
+        "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
     ],
     keywords="openai sales gpt autonomous agi",
```

### Comparing `salesgpt-0.0.1/tests/test_salesgpt.py` & `salesgpt-0.0.2/tests/test_salesgpt.py`

 * *Files identical despite different names*

