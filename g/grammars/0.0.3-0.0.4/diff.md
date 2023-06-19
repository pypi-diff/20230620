# Comparing `tmp/grammars-0.0.3.tar.gz` & `tmp/grammars-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grammars-0.0.3.tar", max compression
+gzip compressed data, was "grammars-0.0.4.tar", max compression
```

## Comparing `grammars-0.0.3.tar` & `grammars-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1068 2023-06-19 21:58:06.150146 grammars-0.0.3/LICENSE
--rw-r--r--   0        0        0     6784 2023-06-19 22:45:20.879351 grammars-0.0.3/README.md
--rw-r--r--   0        0        0       79 2023-06-19 16:15:08.373081 grammars-0.0.3/grammars/__init__.py
--rw-r--r--   0        0        0        0 2023-06-19 14:15:01.125215 grammars-0.0.3/grammars/decode/__init__.py
--rw-r--r--   0        0        0     2008 2023-06-19 22:47:06.275395 grammars-0.0.3/grammars/decode/decode.py
--rw-r--r--   0        0        0     3322 2023-06-19 22:47:06.288800 grammars-0.0.3/grammars/decode/generate.py
--rw-r--r--   0        0        0     4208 2023-06-19 22:47:06.281054 grammars-0.0.3/grammars/decode/modes.py
--rw-r--r--   0        0        0     3852 2023-06-19 22:47:06.295864 grammars-0.0.3/grammars/decode/rank.py
--rw-r--r--   0        0        0     2669 2023-06-19 19:38:12.441884 grammars-0.0.3/grammars/decode/visualize.py
--rw-r--r--   0        0        0       37 2023-06-19 19:38:12.224937 grammars-0.0.3/grammars/parse/__init__.py
--rw-r--r--   0        0        0     8244 2023-06-19 22:49:43.664734 grammars-0.0.3/grammars/parse/parsers.py
--rw-r--r--   0        0        0     1360 2023-06-19 22:49:47.548280 grammars-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     8089 1970-01-01 00:00:00.000000 grammars-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-19 21:58:06.150146 grammars-0.0.4/LICENSE
+-rw-r--r--   0        0        0     6784 2023-06-19 22:45:20.879351 grammars-0.0.4/README.md
+-rw-r--r--   0        0        0       79 2023-06-19 16:15:08.373081 grammars-0.0.4/grammars/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-19 14:15:01.125215 grammars-0.0.4/grammars/decode/__init__.py
+-rw-r--r--   0        0        0     2008 2023-06-19 22:47:06.275395 grammars-0.0.4/grammars/decode/decode.py
+-rw-r--r--   0        0        0     3322 2023-06-19 22:47:06.288800 grammars-0.0.4/grammars/decode/generate.py
+-rw-r--r--   0        0        0     4208 2023-06-19 22:47:06.281054 grammars-0.0.4/grammars/decode/modes.py
+-rw-r--r--   0        0        0     3852 2023-06-19 22:47:06.295864 grammars-0.0.4/grammars/decode/rank.py
+-rw-r--r--   0        0        0     2669 2023-06-19 19:38:12.441884 grammars-0.0.4/grammars/decode/visualize.py
+-rw-r--r--   0        0        0       37 2023-06-19 19:38:12.224937 grammars-0.0.4/grammars/parse/__init__.py
+-rw-r--r--   0        0        0     8244 2023-06-19 22:49:43.664734 grammars-0.0.4/grammars/parse/parsers.py
+-rw-r--r--   0        0        0     1427 2023-06-19 22:53:38.965258 grammars-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     8155 1970-01-01 00:00:00.000000 grammars-0.0.4/PKG-INFO
```

### Comparing `grammars-0.0.3/LICENSE` & `grammars-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `grammars-0.0.3/README.md` & `grammars-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `grammars-0.0.3/grammars/decode/decode.py` & `grammars-0.0.4/grammars/decode/decode.py`

 * *Files identical despite different names*

### Comparing `grammars-0.0.3/grammars/decode/generate.py` & `grammars-0.0.4/grammars/decode/generate.py`

 * *Files identical despite different names*

### Comparing `grammars-0.0.3/grammars/decode/modes.py` & `grammars-0.0.4/grammars/decode/modes.py`

 * *Files identical despite different names*

### Comparing `grammars-0.0.3/grammars/decode/rank.py` & `grammars-0.0.4/grammars/decode/rank.py`

 * *Files identical despite different names*

### Comparing `grammars-0.0.3/grammars/decode/visualize.py` & `grammars-0.0.4/grammars/decode/visualize.py`

 * *Files identical despite different names*

### Comparing `grammars-0.0.3/grammars/parse/parsers.py` & `grammars-0.0.4/grammars/parse/parsers.py`

 * *Files identical despite different names*

### Comparing `grammars-0.0.3/pyproject.toml` & `grammars-0.0.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grammars"
-version = "0.0.3"
+version = "0.0.4"
 description = "Enforce language model output using a grammar"
 authors = ["Dave Nachman <dave.nachman.dev@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 packages = [{include = "grammars"}]
 keywords = [
   "ai",
@@ -26,14 +26,15 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Text Processing :: Linguistic",
 ]
+urls = { repository = "https://github.com/dave-nachman/grammars" }
 
 [tool.poetry.dependencies]
 python = "^3.8"
 transformers = "^4.30.2"
 torch = "^2.0.1"
 tqdm = "^4.65.0"
 regex = "^2023.6.3"
```

### Comparing `grammars-0.0.3/PKG-INFO` & `grammars-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grammars
-Version: 0.0.3
+Version: 0.0.4
 Summary: Enforce language model output using a grammar
 License: MIT
 Keywords: ai,large language models,llm,parser,prompt
 Author: Dave Nachman
 Author-email: dave.nachman.dev@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -23,14 +23,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Linguistic
 Requires-Dist: graphviz (>=0.20.1,<0.21.0)
 Requires-Dist: regex (>=2023.6.3,<2024.0.0)
 Requires-Dist: torch (>=2.0.1,<3.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: transformers (>=4.30.2,<5.0.0)
+Project-URL: repository, https://github.com/dave-nachman/grammars
 Description-Content-Type: text/markdown
 
 # Grammars
 
 **Grammars** is an experimental, early stage Python library for constraining the output of [Transformers](https://github.com/huggingface/transformers) language models using [formal grammars](https://en.wikipedia.org/wiki/Formal_grammar) specified via [parser combinators](https://en.wikipedia.org/wiki/Parser_combinator).
```

