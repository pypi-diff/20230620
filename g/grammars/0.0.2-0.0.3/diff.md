# Comparing `tmp/grammars-0.0.2.tar.gz` & `tmp/grammars-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grammars-0.0.2.tar", max compression
+gzip compressed data, was "grammars-0.0.3.tar", max compression
```

## Comparing `grammars-0.0.2.tar` & `grammars-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1068 2023-06-19 21:58:06.150146 grammars-0.0.2/LICENSE
--rw-r--r--   0        0        0     6784 2023-06-19 22:45:20.879351 grammars-0.0.2/README.md
--rw-r--r--   0        0        0       79 2023-06-19 16:15:08.373081 grammars-0.0.2/grammars/__init__.py
--rw-r--r--   0        0        0        0 2023-06-19 14:15:01.125215 grammars-0.0.2/grammars/decode/__init__.py
--rw-r--r--   0        0        0     2008 2023-06-19 22:47:06.275395 grammars-0.0.2/grammars/decode/decode.py
--rw-r--r--   0        0        0     3322 2023-06-19 22:47:06.288800 grammars-0.0.2/grammars/decode/generate.py
--rw-r--r--   0        0        0     4208 2023-06-19 22:47:06.281054 grammars-0.0.2/grammars/decode/modes.py
--rw-r--r--   0        0        0     3852 2023-06-19 22:47:06.295864 grammars-0.0.2/grammars/decode/rank.py
--rw-r--r--   0        0        0     2669 2023-06-19 19:38:12.441884 grammars-0.0.2/grammars/decode/visualize.py
--rw-r--r--   0        0        0       37 2023-06-19 19:38:12.224937 grammars-0.0.2/grammars/parse/__init__.py
--rw-r--r--   0        0        0     8238 2023-06-19 22:46:10.845722 grammars-0.0.2/grammars/parse/parsers.py
--rw-r--r--   0        0        0     1360 2023-06-19 22:47:15.867873 grammars-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     8089 1970-01-01 00:00:00.000000 grammars-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-19 21:58:06.150146 grammars-0.0.3/LICENSE
+-rw-r--r--   0        0        0     6784 2023-06-19 22:45:20.879351 grammars-0.0.3/README.md
+-rw-r--r--   0        0        0       79 2023-06-19 16:15:08.373081 grammars-0.0.3/grammars/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-19 14:15:01.125215 grammars-0.0.3/grammars/decode/__init__.py
+-rw-r--r--   0        0        0     2008 2023-06-19 22:47:06.275395 grammars-0.0.3/grammars/decode/decode.py
+-rw-r--r--   0        0        0     3322 2023-06-19 22:47:06.288800 grammars-0.0.3/grammars/decode/generate.py
+-rw-r--r--   0        0        0     4208 2023-06-19 22:47:06.281054 grammars-0.0.3/grammars/decode/modes.py
+-rw-r--r--   0        0        0     3852 2023-06-19 22:47:06.295864 grammars-0.0.3/grammars/decode/rank.py
+-rw-r--r--   0        0        0     2669 2023-06-19 19:38:12.441884 grammars-0.0.3/grammars/decode/visualize.py
+-rw-r--r--   0        0        0       37 2023-06-19 19:38:12.224937 grammars-0.0.3/grammars/parse/__init__.py
+-rw-r--r--   0        0        0     8244 2023-06-19 22:49:43.664734 grammars-0.0.3/grammars/parse/parsers.py
+-rw-r--r--   0        0        0     1360 2023-06-19 22:49:47.548280 grammars-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     8089 1970-01-01 00:00:00.000000 grammars-0.0.3/PKG-INFO
```

### Comparing `grammars-0.0.2/LICENSE` & `grammars-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `grammars-0.0.2/README.md` & `grammars-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `grammars-0.0.2/grammars/decode/decode.py` & `grammars-0.0.3/grammars/decode/decode.py`

 * *Files identical despite different names*

### Comparing `grammars-0.0.2/grammars/decode/generate.py` & `grammars-0.0.3/grammars/decode/generate.py`

 * *Files identical despite different names*

### Comparing `grammars-0.0.2/grammars/decode/modes.py` & `grammars-0.0.3/grammars/decode/modes.py`

 * *Files identical despite different names*

### Comparing `grammars-0.0.2/grammars/decode/rank.py` & `grammars-0.0.3/grammars/decode/rank.py`

 * *Files identical despite different names*

### Comparing `grammars-0.0.2/grammars/decode/visualize.py` & `grammars-0.0.3/grammars/decode/visualize.py`

 * *Files identical despite different names*

### Comparing `grammars-0.0.2/grammars/parse/parsers.py` & `grammars-0.0.3/grammars/parse/parsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import itertools
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
-from typing import Optional, Tuple
+from typing import Optional, Tuple, List
 
 import regex
 
 
 class Parser(ABC):
     completed: bool
     can_continue: bool
```

### Comparing `grammars-0.0.2/pyproject.toml` & `grammars-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grammars"
-version = "0.0.2"
+version = "0.0.3"
 description = "Enforce language model output using a grammar"
 authors = ["Dave Nachman <dave.nachman.dev@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 packages = [{include = "grammars"}]
 keywords = [
   "ai",
```

### Comparing `grammars-0.0.2/PKG-INFO` & `grammars-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grammars
-Version: 0.0.2
+Version: 0.0.3
 Summary: Enforce language model output using a grammar
 License: MIT
 Keywords: ai,large language models,llm,parser,prompt
 Author: Dave Nachman
 Author-email: dave.nachman.dev@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
```

