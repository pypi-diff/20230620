# Comparing `tmp/text2text-1.0.8.tar.gz` & `tmp/text2text-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text2text-1.0.8.tar", last modified: Tue Jun 20 04:13:49 2023, max compression
+gzip compressed data, was "text2text-1.0.9.tar", last modified: Tue Jun 20 14:39:49 2023, max compression
```

## Comparing `text2text-1.0.8.tar` & `text2text-1.0.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 04:13:49.048786 text2text-1.0.8/
--rwxr-xr-x   0 root         (0) root         (0)     1418 2023-06-20 01:53:21.000000 text2text-1.0.8/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    60458 2023-06-20 04:13:49.048786 text2text-1.0.8/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)    59644 2023-06-20 04:12:48.000000 text2text-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-20 04:13:49.048786 text2text-1.0.8/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1246 2023-06-20 04:13:17.000000 text2text-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 04:13:49.044786 text2text-1.0.8/text2text/
--rwxr-xr-x   0 root         (0) root         (0)      666 2023-06-20 02:25:27.000000 text2text-1.0.8/text2text/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7162 2023-06-20 01:53:21.000000 text2text-1.0.8/text2text/abstractor.py
--rw-r--r--   0 root         (0) root         (0)     2157 2023-06-20 01:53:21.000000 text2text-1.0.8/text2text/answerer.py
--rw-r--r--   0 root         (0) root         (0)     2287 2023-06-20 03:27:52.000000 text2text-1.0.8/text2text/assistant.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 04:13:49.046786 text2text-1.0.8/text2text/biunilm/
--rwxr-xr-x   0 root         (0) root         (0)      110 2023-06-20 01:53:21.000000 text2text-1.0.8/text2text/biunilm/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    10937 2023-06-20 01:53:21.000000 text2text-1.0.8/text2text/biunilm/loader_utils.py
--rwxr-xr-x   0 root         (0) root         (0)    17726 2023-06-20 01:53:21.000000 text2text-1.0.8/text2text/biunilm/seq2seq_loader.py
--rw-r--r--   0 root         (0) root         (0)     1533 2023-06-20 01:53:21.000000 text2text-1.0.8/text2text/bm25er.py
--rw-r--r--   0 root         (0) root         (0)      519 2023-06-20 01:53:21.000000 text2text-1.0.8/text2text/counter.py
--rw-r--r--   0 root         (0) root         (0)     1177 2023-06-20 01:53:21.000000 text2text-1.0.8/text2text/fitter.py
--rw-r--r--   0 root         (0) root         (0)     1451 2023-06-20 01:53:21.000000 text2text-1.0.8/text2text/handler.py
--rw-r--r--   0 root         (0) root         (0)     2106 2023-06-20 01:53:21.000000 text2text-1.0.8/text2text/identifier.py
--rw-r--r--   0 root         (0) root         (0)     2010 2023-06-20 03:29:02.000000 text2text-1.0.8/text2text/indexer.py
--rw-r--r--   0 root         (0) root         (0)     1165 2023-06-20 01:53:21.000000 text2text-1.0.8/text2text/measurer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 04:13:49.047786 text2text-1.0.8/text2text/pytorch_pretrained_bert/
--rwxr-xr-x   0 root         (0) root         (0)      120 2023-06-20 01:53:21.000000 text2text-1.0.8/text2text/pytorch_pretrained_bert/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      932 2023-06-20 01:53:21.000000 text2text-1.0.8/text2text/pytorch_pretrained_bert/__main__.py
--rwxr-xr-x   0 root         (0) root         (0)     7964 2023-06-20 01:53:21.000000 text2text-1.0.8/text2text/pytorch_pretrained_bert/file_utils.py
--rwxr-xr-x   0 root         (0) root         (0)     1821 2023-06-20 01:53:21.000000 text2text-1.0.8/text2text/pytorch_pretrained_bert/loss.py
--rwxr-xr-x   0 root         (0) root         (0)   108506 2023-06-20 01:53:21.000000 text2text-1.0.8/text2text/pytorch_pretrained_bert/modeling.py
--rwxr-xr-x   0 root         (0) root         (0)    15035 2023-06-20 01:53:21.000000 text2text-1.0.8/text2text/pytorch_pretrained_bert/tokenization.py
--rw-r--r--   0 root         (0) root         (0)     1782 2023-06-20 01:53:21.000000 text2text-1.0.8/text2text/questioner.py
--rw-r--r--   0 root         (0) root         (0)     2605 2023-06-20 03:20:23.000000 text2text-1.0.8/text2text/responder.py
--rw-r--r--   0 root         (0) root         (0)      984 2023-06-20 01:53:21.000000 text2text-1.0.8/text2text/searcher.py
--rw-r--r--   0 root         (0) root         (0)     1575 2023-06-20 01:53:21.000000 text2text-1.0.8/text2text/server.py
--rw-r--r--   0 root         (0) root         (0)     1103 2023-06-20 01:53:21.000000 text2text-1.0.8/text2text/summarizer.py
--rw-r--r--   0 root         (0) root         (0)     1766 2023-06-20 01:53:21.000000 text2text-1.0.8/text2text/tfidfer.py
--rw-r--r--   0 root         (0) root         (0)      780 2023-06-20 01:53:21.000000 text2text-1.0.8/text2text/tokenizer.py
--rw-r--r--   0 root         (0) root         (0)    12572 2023-06-20 02:51:51.000000 text2text-1.0.8/text2text/transformer.py
--rw-r--r--   0 root         (0) root         (0)     1489 2023-06-20 01:53:21.000000 text2text-1.0.8/text2text/translator.py
--rw-r--r--   0 root         (0) root         (0)      500 2023-06-20 01:53:21.000000 text2text-1.0.8/text2text/variator.py
--rw-r--r--   0 root         (0) root         (0)      816 2023-06-20 01:53:21.000000 text2text-1.0.8/text2text/vectorizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 04:13:49.045786 text2text-1.0.8/text2text.egg-info/
--rw-r--r--   0 root         (0) root         (0)    60458 2023-06-20 04:13:48.000000 text2text-1.0.8/text2text.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1064 2023-06-20 04:13:48.000000 text2text-1.0.8/text2text.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 04:13:48.000000 text2text-1.0.8/text2text.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      134 2023-06-20 04:13:48.000000 text2text-1.0.8/text2text.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-20 04:13:48.000000 text2text-1.0.8/text2text.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 14:39:49.415699 text2text-1.0.9/
+-rwxr-xr-x   0 root         (0) root         (0)     1418 2023-06-20 14:28:32.000000 text2text-1.0.9/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    60412 2023-06-20 14:39:49.414699 text2text-1.0.9/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)    59598 2023-06-20 14:37:55.000000 text2text-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-20 14:39:49.415699 text2text-1.0.9/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1246 2023-06-20 14:38:43.000000 text2text-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 14:39:49.411698 text2text-1.0.9/text2text/
+-rwxr-xr-x   0 root         (0) root         (0)      666 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7162 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/abstractor.py
+-rw-r--r--   0 root         (0) root         (0)     2157 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/answerer.py
+-rw-r--r--   0 root         (0) root         (0)     2299 2023-06-20 14:34:46.000000 text2text-1.0.9/text2text/assistant.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 14:39:49.413699 text2text-1.0.9/text2text/biunilm/
+-rwxr-xr-x   0 root         (0) root         (0)      110 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/biunilm/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    10937 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/biunilm/loader_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)    17726 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/biunilm/seq2seq_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/bm25er.py
+-rw-r--r--   0 root         (0) root         (0)      519 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/counter.py
+-rw-r--r--   0 root         (0) root         (0)     1177 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/fitter.py
+-rw-r--r--   0 root         (0) root         (0)     1451 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/handler.py
+-rw-r--r--   0 root         (0) root         (0)     2106 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/identifier.py
+-rw-r--r--   0 root         (0) root         (0)     2010 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/indexer.py
+-rw-r--r--   0 root         (0) root         (0)     1165 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/measurer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 14:39:49.414699 text2text-1.0.9/text2text/pytorch_pretrained_bert/
+-rwxr-xr-x   0 root         (0) root         (0)      120 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/pytorch_pretrained_bert/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      932 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/pytorch_pretrained_bert/__main__.py
+-rwxr-xr-x   0 root         (0) root         (0)     7964 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/pytorch_pretrained_bert/file_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)     1821 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/pytorch_pretrained_bert/loss.py
+-rwxr-xr-x   0 root         (0) root         (0)   108506 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/pytorch_pretrained_bert/modeling.py
+-rwxr-xr-x   0 root         (0) root         (0)    15035 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/pytorch_pretrained_bert/tokenization.py
+-rw-r--r--   0 root         (0) root         (0)     1782 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/questioner.py
+-rw-r--r--   0 root         (0) root         (0)     2605 2023-06-20 14:30:51.000000 text2text-1.0.9/text2text/responder.py
+-rw-r--r--   0 root         (0) root         (0)      984 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/searcher.py
+-rw-r--r--   0 root         (0) root         (0)     1575 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/server.py
+-rw-r--r--   0 root         (0) root         (0)     1103 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/summarizer.py
+-rw-r--r--   0 root         (0) root         (0)     1766 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/tfidfer.py
+-rw-r--r--   0 root         (0) root         (0)      780 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/tokenizer.py
+-rw-r--r--   0 root         (0) root         (0)    12572 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/transformer.py
+-rw-r--r--   0 root         (0) root         (0)     1489 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/translator.py
+-rw-r--r--   0 root         (0) root         (0)      500 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/variator.py
+-rw-r--r--   0 root         (0) root         (0)      816 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/vectorizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 14:39:49.412699 text2text-1.0.9/text2text.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    60412 2023-06-20 14:39:49.000000 text2text-1.0.9/text2text.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1064 2023-06-20 14:39:49.000000 text2text-1.0.9/text2text.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 14:39:49.000000 text2text-1.0.9/text2text.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      134 2023-06-20 14:39:49.000000 text2text-1.0.9/text2text.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-20 14:39:49.000000 text2text-1.0.9/text2text.egg-info/top_level.txt
```

### Comparing `text2text-1.0.8/LICENSE.txt` & `text2text-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `text2text-1.0.8/PKG-INFO` & `text2text-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2text
-Version: 1.0.8
+Version: 1.0.9
 Summary: Text2Text: Crosslingual NLP/G toolkit
 Home-page: https://github.com/artitw/text2text
 Author: Artit Wangperawong
 Author-email: artitw@gmail.com
 Keywords: multilingual crosslingual gpt chatgpt bert natural language processing nlp nlg text generation gpt question answer answering information retrieval tfidf tf-idf bm25 search index summary summarizer summarization tokenizer tokenization translation backtranslation data augmentation science machine learning colab embedding levenshtein sub-word edit distance conversational dialog chatbot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -17,16 +17,16 @@
 
 <details>
   <summary>Overview</summary>
 
 * [Colab Notebooks](https://github.com/artitw/text2text#colab-notebooks)
 * [Crosslingual Models](https://github.com/artitw/text2text#how-crosslingual-models-work-click-to-watch)
 * [Installation Requirements](https://github.com/artitw/text2text#installation-requirements)
-* [Class Diagram](https://github.com/artitw/text2text#class-diagram)
 * [Quick Start Guide](https://github.com/artitw/text2text#api-quick-start-guide)
+* [Class Diagram](https://github.com/artitw/text2text#class-diagram)
 * [Languages Available](https://github.com/artitw/text2text#languages-available)
 * [Requirements & Installation](https://github.com/artitw/text2text#requirements-and-installation)
 * [Examples](https://github.com/artitw/text2text#examples)
   * [Assistant](https://github.com/artitw/text2text#assistant)
   * [Tokenization](https://github.com/artitw/text2text#tokenization)
   * [Embedding](https://github.com/artitw/text2text#embedding--vectorization)
   * [TF-IDF](https://github.com/artitw/text2text#tf-idf)
@@ -54,19 +54,19 @@
 * Assistant with knowledge base [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1hkNgpSmmUA-mzUibqz25xq-E8KYOLuVx?usp=sharing)
 * STF-IDF multilingual search [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1RaWj5SqWvyC2SsCTGg8IAVcl9G5hOB50?usp=sharing)
 * All examples [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1LE_ifTpOGO5QJCKNQYtZe6c_tjbwnulR)
 
 ## How Crosslingual Models Work (click to watch)
 [![Crosslingual Models](http://img.youtube.com/vi/caZLVcJqsqo/0.jpg)](https://youtu.be/caZLVcJqsqo "Cross-Lingual Models")
 
-## Installation Requirements 
+## Installation Requirements
 ```
 pip install -qq -U text2text
 ```
-* [Examples](#examples) all work with <16 GB RAM, so they run free on [Colab](https://colab.research.google.com/drive/1LE_ifTpOGO5QJCKNQYtZe6c_tjbwnulR).
+* [Examples](#examples) can run with <16 GB RAM on free [Colab GPUs](https://colab.research.google.com/drive/1LE_ifTpOGO5QJCKNQYtZe6c_tjbwnulR).
 
 ## Quick Start Guide
 Functionality | Invocation | Result
 :------------: | :-------------: | :-------------:
 Module Importing | `import text2text as t2t` | Libraries imported
 [Assistant](https://github.com/artitw/text2text#assistant) | `t2t.Handler("Describe Text2Text in a few words: ").assist()` | `['Text2Text is an AI-powered text generation tool that creates coherent and continuous text based on prompts.']`
 Language Model Setting | `t2t.Transformer.PRETRAINED_TRANSLATOR = "facebook/m2m100_418M"` | Change from default
@@ -229,30 +229,30 @@
 #  '{\n"a": "α",\n"b": "β",\n"c": "γ",\n"d": "δ",\n"e": "ε",\n"f": "φ",\n"g": "χ",\n"h": "ι",\n"i": "η",\n"j": "κ",\n"k": "λ",\n"l": "μ",\n"m": "ν",\n"n": "ξ",\n"o": "ο",\n"p": "π",\n"q": "ρ",\n"r": "σ",\n"s": "τ",\n"t": "υ",\n"u": "ύ",\n"v": "φ",\n"w": "χ",\n"x": "ψ",\n"y": "ω",\n"z": "ζ"\n}'
 #]
 ```
 
 ### Tokenization
 ```
 t2t.Handler([
-         "Let's go hiking tomorrow", 
-         "안녕하세요.", 
+         "Let's go hiking tomorrow",
+         "안녕하세요.",
          "돼지꿈을 꾸세요~~"
          ]).tokenize()
 
 # Sub-word tokens
 [['▁Let', "'", 's', '▁go', '▁hik', 'ing', '▁tom', 'orrow'],
  ['▁안녕', '하세요', '.'],
  ['▁', '돼', '지', '꿈', '을', '▁꾸', '세요', '~~']]
 ```
 
 ### Embedding / Vectorization
 ```
 t2t.Handler([
-         "Let's go hiking tomorrow", 
-         "안녕하세요.", 
+         "Let's go hiking tomorrow",
+         "안녕하세요.",
          "돼지꿈을 꾸세요~~"
          ]).vectorize()
 
 # Embeddings
 array([[-0.00352954,  0.0260059 ,  0.00407429, ..., -0.04830331,
         -0.02540749, -0.00924972],
        [ 0.00043362,  0.00249816,  0.01755436, ...,  0.04451273,
@@ -260,16 +260,16 @@
        [-0.03563676, -0.04856304,  0.00518898, ..., -0.00311068,
          0.00071953, -0.00216325]])
 ```
 
 ### TF-IDF
 ```
 t2t.Handler([
-         "Let's go hiking tomorrow", 
-         "안녕하세요.", 
+         "Let's go hiking tomorrow",
+         "안녕하세요.",
          "돼지꿈을 꾸세요~~"
          ]).tfidf()
 
 # TF-IDF values
 [{'!': 0.22360679774997894,
   "'": 0.44721359549995787,
   ',': 0.22360679774997894,
@@ -293,16 +293,16 @@
   '을': 0.3535533905932738,
   '지': 0.3535533905932738}]
 ```
 
 ### BM25
 ```
 t2t.Handler([
-         "Let's go hiking tomorrow", 
-         "안녕하세요.", 
+         "Let's go hiking tomorrow",
+         "안녕하세요.",
          "돼지꿈을 꾸세요~~"
          ]).bm25()
 
 # BM25 values
 [{"'": 1.2792257271403649,
   'ing': 1.2792257271403649,
   'orrow': 1.2792257271403649,
@@ -322,26 +322,26 @@
   '지': 1.2792257271403649}]
 ```
 
 ### Index
 [![STF-IDF Demo](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1RaWj5SqWvyC2SsCTGg8IAVcl9G5hOB50?usp=sharing)
 ```
 index = t2t.Handler([
-         "Let's go hiking tomorrow, let's go!", 
-         "안녕하세요.", 
+         "Let's go hiking tomorrow, let's go!",
+         "안녕하세요.",
          "돼지꿈을 꾸세요~~",
          ]).index(ids=[100, 101, 102])
 
 index.search(["돼지", "안녕", "let's go"], k=1)
 
 # Matching L2 distances and corresponding ids
 (
   array([[0.7752551],
         [0.8452994],
-        [0.4347524]], dtype=float32), 
+        [0.4347524]], dtype=float32),
   array([[102],
         [101],
         [100]])
 )
 
 # Add documents incrementing on ids if none specified
 index.add(["Hello, World! 你好,世界!"])
@@ -356,16 +356,16 @@
  array([[103, 100, 102]]))
 ```
 To learn more, see [STF-IDF](https://arxiv.org/abs/2209.14281).
 
 ### Search
 ```
 t2t.Handler([
-         "Let's go hiking tomorrow, let's go!", 
-         "안녕하세요.", 
+         "Let's go hiking tomorrow, let's go!",
+         "안녕하세요.",
          "돼지꿈을 꾸세요~~",
          ]).search(queries=["go", "안녕"])
 
 # Cosine similarity scores matrix
 array([[0.4472136 , 0.        , 0.        ],
        [0.        , 0.57735027, 0.        ]])
 ```
@@ -377,92 +377,92 @@
 notre_dame_str = "As at most other universities, Notre Dame's students run a number of news media outlets. The nine student - run outlets include three newspapers, both a radio and television station, and several magazines and journals. Begun as a one - page journal in September 1876, the Scholastic magazine is issued twice monthly and claims to be the oldest continuous collegiate publication in the United States. The other magazine, The Juggler, is released twice a year and focuses on student literature and artwork. The Dome yearbook is published annually. The newspapers have varying publication interests, with The Observer published daily and mainly reporting university and other news, and staffed by students from both Notre Dame and Saint Mary's College. Unlike Scholastic and The Dome, The Observer is an independent publication and does not have a faculty advisor or any editorial oversight from the University. In 1987, when some students believed that The Observer began to show a conservative bias, a liberal newspaper, Common Sense was published. Likewise, in 2003, when other students believed that the paper showed a liberal bias, the conservative paper Irish Rover went into production. Neither paper is published as often as The Observer; however, all three are distributed to all students. Finally, in Spring 2008 an undergraduate journal for political science research, Beyond Politics, made its debut."
 
 bacteria_str = "Bacteria are a type of biological cell. They constitute a large domain of prokaryotic microorganisms. Typically a few micrometres in length, bacteria have a number of shapes, ranging from spheres to rods and spirals. Bacteria were among the first life forms to appear on Earth, and are present in most of its habitats."
 
 bio_str = "Biology is the science that studies life. What exactly is life? This may sound like a silly question with an obvious answer, but it is not easy to define life. For example, a branch of biology called virology studies viruses, which exhibit some of the characteristics of living entities but lack others. It turns out that although viruses can attack living organisms, cause diseases, and even reproduce, they do not meet the criteria that biologists use to define life."
 
 bm25_index = t2t.Handler([
-                       article_en, 
-                       notre_dame_str, 
-                       bacteria_str, 
+                       article_en,
+                       notre_dame_str,
+                       bacteria_str,
                        bio_str
                        ]).bm25(output="matrix")
 
 search_results_bm25 = t2t.Handler().search(
-    queries=["wonderful life", "university students"], 
+    queries=["wonderful life", "university students"],
     vector_class=t2t.Bm25er,
     index=bm25_index)
 
 search_results_bm25_2 = t2t.Handler().search(
-    queries=["Earth creatures are cool", "United Nations"], 
+    queries=["Earth creatures are cool", "United Nations"],
     vector_class=t2t.Bm25er,
     index=bm25_index)
 ```
 
 #### Using TF-DF embeddings index
 ```
 tfidf_index = t2t.Handler([
-                       article_en, 
-                       notre_dame_str, 
-                       bacteria_str, 
+                       article_en,
+                       notre_dame_str,
+                       bacteria_str,
                        bio_str
                        ]).tfidf(output="matrix")
 
 search_results_tf = t2t.Handler().search(
-    queries=["wonderful life", "university students"], 
+    queries=["wonderful life", "university students"],
     vector_class=t2t.Tfidfer,
     index=tfidf_index)
 ```
 
 #### Using neural embeddings index
 ```
 embedding_index = t2t.Handler([
-                       article_en, 
-                       notre_dame_str, 
-                       bacteria_str, 
+                       article_en,
+                       notre_dame_str,
+                       bacteria_str,
                        bio_str
                        ]).vectorize()
 
 search_results_em = t2t.Handler().search(
     queries=["wonderful life", "university students"],
     vector_class=t2t.Vectorizer,
     index=embedding_index)
 ```
 
-#### Blending bm25, tf-idf and neural embeddings 
+#### Blending bm25, tf-idf and neural embeddings
 ```
-np.mean( 
+np.mean(
     np.array([
               search_results_bm25,
               search_results_tf,
               search_results_em,
               ]), axis=0)
 
 # averaged scores matrix
 #matrix([[ 0.00486117, -0.01890325,  0.53769584,  0.82506883],
 #        [ 0.0435048 ,  1.68977281,  0.01238902,  0.01266839]])
 ```
 
 ### Levenshtein Sub-word Edit Distance
 ```
 t2t.Handler([
-         "Hello, World! [SEP] Hello, what?", 
+         "Hello, World! [SEP] Hello, what?",
          "안녕하세요. [SEP] 돼지꿈을 꾸세요~~"
         ]).measure(metric="levenshtein_distance")
 
 # Distances
  [2, 8]
 ```
 
 ### Translation
 ```
 t2t.Handler([
-         article_en, 
-         notre_dame_str, 
-         bacteria_str, 
+         article_en,
+         notre_dame_str,
+         bacteria_str,
          bio_str
          ], src_lang='en').translate(tgt_lang='zh')
 
 # Translations
 ['联合国秘书长说,叙利亚没有军事解决方案。',
  '与大多数其他大学一样,Notre Dame的学生运行的新闻媒体渠道的数量。九个学生 - 运行的渠道包括三份报纸,两台广播电视台,以及几本杂志和杂志。 开始作为一个一页的杂志在1876年9月,该杂志的Schoolistic发行了每月两次,并声称是美国最古老的连续的大学新闻出版物,和其他杂志,TheJuggler,每年发行两次,并专注于学生文学和艺术作品。 多姆年刊每年发行。 报纸有不同的出版利益,与The Observer发表每日,主要报道大学和其他新闻,并由学生从Notre Dame和圣玛丽的学院。 与Scholastic和The Dome不同,The Observer是一个独立的公众作品,但没有教师顾',
  '细菌是生物细胞的一种类型. 它们构成一个大范围的亲生微生物. 通常几微米长,细菌有许多形状,从球到杖和螺旋。 细菌是地球上出现的第一个生命形式之一,并且存在于其大多数栖息地。',
@@ -529,27 +529,27 @@
   'tr_TR': 'Turkish',
   'uk_UA': 'Ukrainian',
   'ur_PK': 'Urdu',
   'vi_VN': 'Vietnamese',
   'xh_ZA': 'Xhosa',
   'zh_CN': 'Chinese'
 }
-t2t.Handler(["I would like to go hiking tomorrow."], 
+t2t.Handler(["I would like to go hiking tomorrow."],
         src_lang="en_XX"
         ).translate(tgt_lang='zh_CN')
 ['我想明天去徒步旅行。']
 ```
 
 </details>
 
 ### Question Answering
 Question must follow context with ` [SEP] ` in between.
 ```
 t2t.Handler([
-         "Hello, this is Text2Text! [SEP] What is this?", 
+         "Hello, this is Text2Text! [SEP] What is this?",
          "It works very well. It's awesome! [SEP] How is it?"
          ]).answer()
 
 t2t.Handler([
              "很喜欢陈慧琳唱歌。[SEP] 喜欢做什么?"
              ], src_lang="zh").answer()
 
@@ -746,18 +746,18 @@
 t2t.Handler([input_state]).respond()
 # ['About 60 different kinds of cats are recognized by various cat registries.']
 ```
 
 ### Training / Finetuning
 Finetune cross-lingual model on your data
 ```
-result = t2t.Handler(["Hello, World! [TGT] 你好,世界!"], 
+result = t2t.Handler(["Hello, World! [TGT] 你好,世界!"],
             src_lang="en",
             tgt_lang="zh",
-            num_epochs=10, 
+            num_epochs=10,
             save_directory="model_dir"
             ).fit()
 
 # load and use model from saved directory
 t2t.Transformer.PRETRAINED_TRANSLATOR = "model_dir"
 t2t.Handler("Hello, World!").translate(tgt_lang="zh")
 ```
@@ -781,15 +781,15 @@
 import socket
 import requests
 
 address = socket.gethostbyname(socket.getfqdn(socket.gethostname()))
 url = f"http://{address}"
 transform = "translate"
 payload = {
-  "input_lines": ["hello", "world"], 
+  "input_lines": ["hello", "world"],
   "src_lang": "en",
   "tgt_lang": "ko",
 }
 r = requests.post(f"{url}/{transform}", json=payload)
 print(r.json()) #{'result': ['안녕하세요', '세계']}
 
 # Indexer actions
```

### Comparing `text2text-1.0.8/README.md` & `text2text-1.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 <details>
   <summary>Overview</summary>
 
 * [Colab Notebooks](https://github.com/artitw/text2text#colab-notebooks)
 * [Crosslingual Models](https://github.com/artitw/text2text#how-crosslingual-models-work-click-to-watch)
 * [Installation Requirements](https://github.com/artitw/text2text#installation-requirements)
-* [Class Diagram](https://github.com/artitw/text2text#class-diagram)
 * [Quick Start Guide](https://github.com/artitw/text2text#api-quick-start-guide)
+* [Class Diagram](https://github.com/artitw/text2text#class-diagram)
 * [Languages Available](https://github.com/artitw/text2text#languages-available)
 * [Requirements & Installation](https://github.com/artitw/text2text#requirements-and-installation)
 * [Examples](https://github.com/artitw/text2text#examples)
   * [Assistant](https://github.com/artitw/text2text#assistant)
   * [Tokenization](https://github.com/artitw/text2text#tokenization)
   * [Embedding](https://github.com/artitw/text2text#embedding--vectorization)
   * [TF-IDF](https://github.com/artitw/text2text#tf-idf)
@@ -40,19 +40,19 @@
 * Assistant with knowledge base [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1hkNgpSmmUA-mzUibqz25xq-E8KYOLuVx?usp=sharing)
 * STF-IDF multilingual search [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1RaWj5SqWvyC2SsCTGg8IAVcl9G5hOB50?usp=sharing)
 * All examples [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1LE_ifTpOGO5QJCKNQYtZe6c_tjbwnulR)
 
 ## How Crosslingual Models Work (click to watch)
 [![Crosslingual Models](http://img.youtube.com/vi/caZLVcJqsqo/0.jpg)](https://youtu.be/caZLVcJqsqo "Cross-Lingual Models")
 
-## Installation Requirements 
+## Installation Requirements
 ```
 pip install -qq -U text2text
 ```
-* [Examples](#examples) all work with <16 GB RAM, so they run free on [Colab](https://colab.research.google.com/drive/1LE_ifTpOGO5QJCKNQYtZe6c_tjbwnulR).
+* [Examples](#examples) can run with <16 GB RAM on free [Colab GPUs](https://colab.research.google.com/drive/1LE_ifTpOGO5QJCKNQYtZe6c_tjbwnulR).
 
 ## Quick Start Guide
 Functionality | Invocation | Result
 :------------: | :-------------: | :-------------:
 Module Importing | `import text2text as t2t` | Libraries imported
 [Assistant](https://github.com/artitw/text2text#assistant) | `t2t.Handler("Describe Text2Text in a few words: ").assist()` | `['Text2Text is an AI-powered text generation tool that creates coherent and continuous text based on prompts.']`
 Language Model Setting | `t2t.Transformer.PRETRAINED_TRANSLATOR = "facebook/m2m100_418M"` | Change from default
@@ -215,30 +215,30 @@
 #  '{\n"a": "α",\n"b": "β",\n"c": "γ",\n"d": "δ",\n"e": "ε",\n"f": "φ",\n"g": "χ",\n"h": "ι",\n"i": "η",\n"j": "κ",\n"k": "λ",\n"l": "μ",\n"m": "ν",\n"n": "ξ",\n"o": "ο",\n"p": "π",\n"q": "ρ",\n"r": "σ",\n"s": "τ",\n"t": "υ",\n"u": "ύ",\n"v": "φ",\n"w": "χ",\n"x": "ψ",\n"y": "ω",\n"z": "ζ"\n}'
 #]
 ```
 
 ### Tokenization
 ```
 t2t.Handler([
-         "Let's go hiking tomorrow", 
-         "안녕하세요.", 
+         "Let's go hiking tomorrow",
+         "안녕하세요.",
          "돼지꿈을 꾸세요~~"
          ]).tokenize()
 
 # Sub-word tokens
 [['▁Let', "'", 's', '▁go', '▁hik', 'ing', '▁tom', 'orrow'],
  ['▁안녕', '하세요', '.'],
  ['▁', '돼', '지', '꿈', '을', '▁꾸', '세요', '~~']]
 ```
 
 ### Embedding / Vectorization
 ```
 t2t.Handler([
-         "Let's go hiking tomorrow", 
-         "안녕하세요.", 
+         "Let's go hiking tomorrow",
+         "안녕하세요.",
          "돼지꿈을 꾸세요~~"
          ]).vectorize()
 
 # Embeddings
 array([[-0.00352954,  0.0260059 ,  0.00407429, ..., -0.04830331,
         -0.02540749, -0.00924972],
        [ 0.00043362,  0.00249816,  0.01755436, ...,  0.04451273,
@@ -246,16 +246,16 @@
        [-0.03563676, -0.04856304,  0.00518898, ..., -0.00311068,
          0.00071953, -0.00216325]])
 ```
 
 ### TF-IDF
 ```
 t2t.Handler([
-         "Let's go hiking tomorrow", 
-         "안녕하세요.", 
+         "Let's go hiking tomorrow",
+         "안녕하세요.",
          "돼지꿈을 꾸세요~~"
          ]).tfidf()
 
 # TF-IDF values
 [{'!': 0.22360679774997894,
   "'": 0.44721359549995787,
   ',': 0.22360679774997894,
@@ -279,16 +279,16 @@
   '을': 0.3535533905932738,
   '지': 0.3535533905932738}]
 ```
 
 ### BM25
 ```
 t2t.Handler([
-         "Let's go hiking tomorrow", 
-         "안녕하세요.", 
+         "Let's go hiking tomorrow",
+         "안녕하세요.",
          "돼지꿈을 꾸세요~~"
          ]).bm25()
 
 # BM25 values
 [{"'": 1.2792257271403649,
   'ing': 1.2792257271403649,
   'orrow': 1.2792257271403649,
@@ -308,26 +308,26 @@
   '지': 1.2792257271403649}]
 ```
 
 ### Index
 [![STF-IDF Demo](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1RaWj5SqWvyC2SsCTGg8IAVcl9G5hOB50?usp=sharing)
 ```
 index = t2t.Handler([
-         "Let's go hiking tomorrow, let's go!", 
-         "안녕하세요.", 
+         "Let's go hiking tomorrow, let's go!",
+         "안녕하세요.",
          "돼지꿈을 꾸세요~~",
          ]).index(ids=[100, 101, 102])
 
 index.search(["돼지", "안녕", "let's go"], k=1)
 
 # Matching L2 distances and corresponding ids
 (
   array([[0.7752551],
         [0.8452994],
-        [0.4347524]], dtype=float32), 
+        [0.4347524]], dtype=float32),
   array([[102],
         [101],
         [100]])
 )
 
 # Add documents incrementing on ids if none specified
 index.add(["Hello, World! 你好,世界!"])
@@ -342,16 +342,16 @@
  array([[103, 100, 102]]))
 ```
 To learn more, see [STF-IDF](https://arxiv.org/abs/2209.14281).
 
 ### Search
 ```
 t2t.Handler([
-         "Let's go hiking tomorrow, let's go!", 
-         "안녕하세요.", 
+         "Let's go hiking tomorrow, let's go!",
+         "안녕하세요.",
          "돼지꿈을 꾸세요~~",
          ]).search(queries=["go", "안녕"])
 
 # Cosine similarity scores matrix
 array([[0.4472136 , 0.        , 0.        ],
        [0.        , 0.57735027, 0.        ]])
 ```
@@ -363,92 +363,92 @@
 notre_dame_str = "As at most other universities, Notre Dame's students run a number of news media outlets. The nine student - run outlets include three newspapers, both a radio and television station, and several magazines and journals. Begun as a one - page journal in September 1876, the Scholastic magazine is issued twice monthly and claims to be the oldest continuous collegiate publication in the United States. The other magazine, The Juggler, is released twice a year and focuses on student literature and artwork. The Dome yearbook is published annually. The newspapers have varying publication interests, with The Observer published daily and mainly reporting university and other news, and staffed by students from both Notre Dame and Saint Mary's College. Unlike Scholastic and The Dome, The Observer is an independent publication and does not have a faculty advisor or any editorial oversight from the University. In 1987, when some students believed that The Observer began to show a conservative bias, a liberal newspaper, Common Sense was published. Likewise, in 2003, when other students believed that the paper showed a liberal bias, the conservative paper Irish Rover went into production. Neither paper is published as often as The Observer; however, all three are distributed to all students. Finally, in Spring 2008 an undergraduate journal for political science research, Beyond Politics, made its debut."
 
 bacteria_str = "Bacteria are a type of biological cell. They constitute a large domain of prokaryotic microorganisms. Typically a few micrometres in length, bacteria have a number of shapes, ranging from spheres to rods and spirals. Bacteria were among the first life forms to appear on Earth, and are present in most of its habitats."
 
 bio_str = "Biology is the science that studies life. What exactly is life? This may sound like a silly question with an obvious answer, but it is not easy to define life. For example, a branch of biology called virology studies viruses, which exhibit some of the characteristics of living entities but lack others. It turns out that although viruses can attack living organisms, cause diseases, and even reproduce, they do not meet the criteria that biologists use to define life."
 
 bm25_index = t2t.Handler([
-                       article_en, 
-                       notre_dame_str, 
-                       bacteria_str, 
+                       article_en,
+                       notre_dame_str,
+                       bacteria_str,
                        bio_str
                        ]).bm25(output="matrix")
 
 search_results_bm25 = t2t.Handler().search(
-    queries=["wonderful life", "university students"], 
+    queries=["wonderful life", "university students"],
     vector_class=t2t.Bm25er,
     index=bm25_index)
 
 search_results_bm25_2 = t2t.Handler().search(
-    queries=["Earth creatures are cool", "United Nations"], 
+    queries=["Earth creatures are cool", "United Nations"],
     vector_class=t2t.Bm25er,
     index=bm25_index)
 ```
 
 #### Using TF-DF embeddings index
 ```
 tfidf_index = t2t.Handler([
-                       article_en, 
-                       notre_dame_str, 
-                       bacteria_str, 
+                       article_en,
+                       notre_dame_str,
+                       bacteria_str,
                        bio_str
                        ]).tfidf(output="matrix")
 
 search_results_tf = t2t.Handler().search(
-    queries=["wonderful life", "university students"], 
+    queries=["wonderful life", "university students"],
     vector_class=t2t.Tfidfer,
     index=tfidf_index)
 ```
 
 #### Using neural embeddings index
 ```
 embedding_index = t2t.Handler([
-                       article_en, 
-                       notre_dame_str, 
-                       bacteria_str, 
+                       article_en,
+                       notre_dame_str,
+                       bacteria_str,
                        bio_str
                        ]).vectorize()
 
 search_results_em = t2t.Handler().search(
     queries=["wonderful life", "university students"],
     vector_class=t2t.Vectorizer,
     index=embedding_index)
 ```
 
-#### Blending bm25, tf-idf and neural embeddings 
+#### Blending bm25, tf-idf and neural embeddings
 ```
-np.mean( 
+np.mean(
     np.array([
               search_results_bm25,
               search_results_tf,
               search_results_em,
               ]), axis=0)
 
 # averaged scores matrix
 #matrix([[ 0.00486117, -0.01890325,  0.53769584,  0.82506883],
 #        [ 0.0435048 ,  1.68977281,  0.01238902,  0.01266839]])
 ```
 
 ### Levenshtein Sub-word Edit Distance
 ```
 t2t.Handler([
-         "Hello, World! [SEP] Hello, what?", 
+         "Hello, World! [SEP] Hello, what?",
          "안녕하세요. [SEP] 돼지꿈을 꾸세요~~"
         ]).measure(metric="levenshtein_distance")
 
 # Distances
  [2, 8]
 ```
 
 ### Translation
 ```
 t2t.Handler([
-         article_en, 
-         notre_dame_str, 
-         bacteria_str, 
+         article_en,
+         notre_dame_str,
+         bacteria_str,
          bio_str
          ], src_lang='en').translate(tgt_lang='zh')
 
 # Translations
 ['联合国秘书长说,叙利亚没有军事解决方案。',
  '与大多数其他大学一样,Notre Dame的学生运行的新闻媒体渠道的数量。九个学生 - 运行的渠道包括三份报纸,两台广播电视台,以及几本杂志和杂志。 开始作为一个一页的杂志在1876年9月,该杂志的Schoolistic发行了每月两次,并声称是美国最古老的连续的大学新闻出版物,和其他杂志,TheJuggler,每年发行两次,并专注于学生文学和艺术作品。 多姆年刊每年发行。 报纸有不同的出版利益,与The Observer发表每日,主要报道大学和其他新闻,并由学生从Notre Dame和圣玛丽的学院。 与Scholastic和The Dome不同,The Observer是一个独立的公众作品,但没有教师顾',
  '细菌是生物细胞的一种类型. 它们构成一个大范围的亲生微生物. 通常几微米长,细菌有许多形状,从球到杖和螺旋。 细菌是地球上出现的第一个生命形式之一,并且存在于其大多数栖息地。',
@@ -515,27 +515,27 @@
   'tr_TR': 'Turkish',
   'uk_UA': 'Ukrainian',
   'ur_PK': 'Urdu',
   'vi_VN': 'Vietnamese',
   'xh_ZA': 'Xhosa',
   'zh_CN': 'Chinese'
 }
-t2t.Handler(["I would like to go hiking tomorrow."], 
+t2t.Handler(["I would like to go hiking tomorrow."],
         src_lang="en_XX"
         ).translate(tgt_lang='zh_CN')
 ['我想明天去徒步旅行。']
 ```
 
 </details>
 
 ### Question Answering
 Question must follow context with ` [SEP] ` in between.
 ```
 t2t.Handler([
-         "Hello, this is Text2Text! [SEP] What is this?", 
+         "Hello, this is Text2Text! [SEP] What is this?",
          "It works very well. It's awesome! [SEP] How is it?"
          ]).answer()
 
 t2t.Handler([
              "很喜欢陈慧琳唱歌。[SEP] 喜欢做什么?"
              ], src_lang="zh").answer()
 
@@ -732,18 +732,18 @@
 t2t.Handler([input_state]).respond()
 # ['About 60 different kinds of cats are recognized by various cat registries.']
 ```
 
 ### Training / Finetuning
 Finetune cross-lingual model on your data
 ```
-result = t2t.Handler(["Hello, World! [TGT] 你好,世界!"], 
+result = t2t.Handler(["Hello, World! [TGT] 你好,世界!"],
             src_lang="en",
             tgt_lang="zh",
-            num_epochs=10, 
+            num_epochs=10,
             save_directory="model_dir"
             ).fit()
 
 # load and use model from saved directory
 t2t.Transformer.PRETRAINED_TRANSLATOR = "model_dir"
 t2t.Handler("Hello, World!").translate(tgt_lang="zh")
 ```
@@ -767,15 +767,15 @@
 import socket
 import requests
 
 address = socket.gethostbyname(socket.getfqdn(socket.gethostname()))
 url = f"http://{address}"
 transform = "translate"
 payload = {
-  "input_lines": ["hello", "world"], 
+  "input_lines": ["hello", "world"],
   "src_lang": "en",
   "tgt_lang": "ko",
 }
 r = requests.post(f"{url}/{transform}", json=payload)
 print(r.json()) #{'result': ['안녕하세요', '세계']}
 
 # Indexer actions
```

### Comparing `text2text-1.0.8/setup.py` & `text2text-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="text2text",
-  version="1.0.8",
+  version="1.0.9",
   author="Artit Wangperawong",
   author_email="artitw@gmail.com",
   description="Text2Text: Crosslingual NLP/G toolkit",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/artitw/text2text",
   packages=setuptools.find_packages(),
```

### Comparing `text2text-1.0.8/text2text/__init__.py` & `text2text-1.0.9/text2text/__init__.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.8/text2text/abstractor.py` & `text2text-1.0.9/text2text/abstractor.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.8/text2text/answerer.py` & `text2text-1.0.9/text2text/answerer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.8/text2text/assistant.py` & `text2text-1.0.9/text2text/assistant.py`

 * *Files 9% similar despite different names*

```diff
@@ -47,13 +47,11 @@
         temperature=temperature,
         do_sample=temperature > 0.0,
         top_p=top_p,
         top_k=top_k,
         repetition_penalty=repetition_penalty,
     )
 
-    output_lines = tok.batch_decode(m.generate(**generate_kwargs)) 
+    df["output_line"] = tok.batch_decode(m.generate(**generate_kwargs)) 
+    df["output_line"] = df.apply(lambda row: row["output_line"].replace('<s>',"").replace('</s>',"").replace(row["input_line"], "").strip(), axis=1)
 
-    for i in range(len(input_lines)):
-      output_lines[i] = output_lines[i].replace('<s>',"").replace('</s>',"").replace(input_lines[i], "").strip()
-    
-    return output_lines
+    return df["output_line"].tolist()
```

### Comparing `text2text-1.0.8/text2text/biunilm/loader_utils.py` & `text2text-1.0.9/text2text/biunilm/loader_utils.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.8/text2text/biunilm/seq2seq_loader.py` & `text2text-1.0.9/text2text/biunilm/seq2seq_loader.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.8/text2text/bm25er.py` & `text2text-1.0.9/text2text/bm25er.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.8/text2text/counter.py` & `text2text-1.0.9/text2text/counter.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.8/text2text/fitter.py` & `text2text-1.0.9/text2text/fitter.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.8/text2text/handler.py` & `text2text-1.0.9/text2text/handler.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.8/text2text/identifier.py` & `text2text-1.0.9/text2text/identifier.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.8/text2text/indexer.py` & `text2text-1.0.9/text2text/indexer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.8/text2text/measurer.py` & `text2text-1.0.9/text2text/measurer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.8/text2text/pytorch_pretrained_bert/__main__.py` & `text2text-1.0.9/text2text/pytorch_pretrained_bert/__main__.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.8/text2text/pytorch_pretrained_bert/file_utils.py` & `text2text-1.0.9/text2text/pytorch_pretrained_bert/file_utils.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.8/text2text/pytorch_pretrained_bert/loss.py` & `text2text-1.0.9/text2text/pytorch_pretrained_bert/loss.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.8/text2text/pytorch_pretrained_bert/modeling.py` & `text2text-1.0.9/text2text/pytorch_pretrained_bert/modeling.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.8/text2text/pytorch_pretrained_bert/tokenization.py` & `text2text-1.0.9/text2text/pytorch_pretrained_bert/tokenization.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.8/text2text/questioner.py` & `text2text-1.0.9/text2text/questioner.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.8/text2text/responder.py` & `text2text-1.0.9/text2text/responder.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.8/text2text/searcher.py` & `text2text-1.0.9/text2text/searcher.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.8/text2text/server.py` & `text2text-1.0.9/text2text/server.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.8/text2text/summarizer.py` & `text2text-1.0.9/text2text/summarizer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.8/text2text/tfidfer.py` & `text2text-1.0.9/text2text/tfidfer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.8/text2text/tokenizer.py` & `text2text-1.0.9/text2text/tokenizer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.8/text2text/transformer.py` & `text2text-1.0.9/text2text/transformer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.8/text2text/translator.py` & `text2text-1.0.9/text2text/translator.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.8/text2text/vectorizer.py` & `text2text-1.0.9/text2text/vectorizer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.8/text2text.egg-info/PKG-INFO` & `text2text-1.0.9/text2text.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2text
-Version: 1.0.8
+Version: 1.0.9
 Summary: Text2Text: Crosslingual NLP/G toolkit
 Home-page: https://github.com/artitw/text2text
 Author: Artit Wangperawong
 Author-email: artitw@gmail.com
 Keywords: multilingual crosslingual gpt chatgpt bert natural language processing nlp nlg text generation gpt question answer answering information retrieval tfidf tf-idf bm25 search index summary summarizer summarization tokenizer tokenization translation backtranslation data augmentation science machine learning colab embedding levenshtein sub-word edit distance conversational dialog chatbot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -17,16 +17,16 @@
 
 <details>
   <summary>Overview</summary>
 
 * [Colab Notebooks](https://github.com/artitw/text2text#colab-notebooks)
 * [Crosslingual Models](https://github.com/artitw/text2text#how-crosslingual-models-work-click-to-watch)
 * [Installation Requirements](https://github.com/artitw/text2text#installation-requirements)
-* [Class Diagram](https://github.com/artitw/text2text#class-diagram)
 * [Quick Start Guide](https://github.com/artitw/text2text#api-quick-start-guide)
+* [Class Diagram](https://github.com/artitw/text2text#class-diagram)
 * [Languages Available](https://github.com/artitw/text2text#languages-available)
 * [Requirements & Installation](https://github.com/artitw/text2text#requirements-and-installation)
 * [Examples](https://github.com/artitw/text2text#examples)
   * [Assistant](https://github.com/artitw/text2text#assistant)
   * [Tokenization](https://github.com/artitw/text2text#tokenization)
   * [Embedding](https://github.com/artitw/text2text#embedding--vectorization)
   * [TF-IDF](https://github.com/artitw/text2text#tf-idf)
@@ -54,19 +54,19 @@
 * Assistant with knowledge base [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1hkNgpSmmUA-mzUibqz25xq-E8KYOLuVx?usp=sharing)
 * STF-IDF multilingual search [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1RaWj5SqWvyC2SsCTGg8IAVcl9G5hOB50?usp=sharing)
 * All examples [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1LE_ifTpOGO5QJCKNQYtZe6c_tjbwnulR)
 
 ## How Crosslingual Models Work (click to watch)
 [![Crosslingual Models](http://img.youtube.com/vi/caZLVcJqsqo/0.jpg)](https://youtu.be/caZLVcJqsqo "Cross-Lingual Models")
 
-## Installation Requirements 
+## Installation Requirements
 ```
 pip install -qq -U text2text
 ```
-* [Examples](#examples) all work with <16 GB RAM, so they run free on [Colab](https://colab.research.google.com/drive/1LE_ifTpOGO5QJCKNQYtZe6c_tjbwnulR).
+* [Examples](#examples) can run with <16 GB RAM on free [Colab GPUs](https://colab.research.google.com/drive/1LE_ifTpOGO5QJCKNQYtZe6c_tjbwnulR).
 
 ## Quick Start Guide
 Functionality | Invocation | Result
 :------------: | :-------------: | :-------------:
 Module Importing | `import text2text as t2t` | Libraries imported
 [Assistant](https://github.com/artitw/text2text#assistant) | `t2t.Handler("Describe Text2Text in a few words: ").assist()` | `['Text2Text is an AI-powered text generation tool that creates coherent and continuous text based on prompts.']`
 Language Model Setting | `t2t.Transformer.PRETRAINED_TRANSLATOR = "facebook/m2m100_418M"` | Change from default
@@ -229,30 +229,30 @@
 #  '{\n"a": "α",\n"b": "β",\n"c": "γ",\n"d": "δ",\n"e": "ε",\n"f": "φ",\n"g": "χ",\n"h": "ι",\n"i": "η",\n"j": "κ",\n"k": "λ",\n"l": "μ",\n"m": "ν",\n"n": "ξ",\n"o": "ο",\n"p": "π",\n"q": "ρ",\n"r": "σ",\n"s": "τ",\n"t": "υ",\n"u": "ύ",\n"v": "φ",\n"w": "χ",\n"x": "ψ",\n"y": "ω",\n"z": "ζ"\n}'
 #]
 ```
 
 ### Tokenization
 ```
 t2t.Handler([
-         "Let's go hiking tomorrow", 
-         "안녕하세요.", 
+         "Let's go hiking tomorrow",
+         "안녕하세요.",
          "돼지꿈을 꾸세요~~"
          ]).tokenize()
 
 # Sub-word tokens
 [['▁Let', "'", 's', '▁go', '▁hik', 'ing', '▁tom', 'orrow'],
  ['▁안녕', '하세요', '.'],
  ['▁', '돼', '지', '꿈', '을', '▁꾸', '세요', '~~']]
 ```
 
 ### Embedding / Vectorization
 ```
 t2t.Handler([
-         "Let's go hiking tomorrow", 
-         "안녕하세요.", 
+         "Let's go hiking tomorrow",
+         "안녕하세요.",
          "돼지꿈을 꾸세요~~"
          ]).vectorize()
 
 # Embeddings
 array([[-0.00352954,  0.0260059 ,  0.00407429, ..., -0.04830331,
         -0.02540749, -0.00924972],
        [ 0.00043362,  0.00249816,  0.01755436, ...,  0.04451273,
@@ -260,16 +260,16 @@
        [-0.03563676, -0.04856304,  0.00518898, ..., -0.00311068,
          0.00071953, -0.00216325]])
 ```
 
 ### TF-IDF
 ```
 t2t.Handler([
-         "Let's go hiking tomorrow", 
-         "안녕하세요.", 
+         "Let's go hiking tomorrow",
+         "안녕하세요.",
          "돼지꿈을 꾸세요~~"
          ]).tfidf()
 
 # TF-IDF values
 [{'!': 0.22360679774997894,
   "'": 0.44721359549995787,
   ',': 0.22360679774997894,
@@ -293,16 +293,16 @@
   '을': 0.3535533905932738,
   '지': 0.3535533905932738}]
 ```
 
 ### BM25
 ```
 t2t.Handler([
-         "Let's go hiking tomorrow", 
-         "안녕하세요.", 
+         "Let's go hiking tomorrow",
+         "안녕하세요.",
          "돼지꿈을 꾸세요~~"
          ]).bm25()
 
 # BM25 values
 [{"'": 1.2792257271403649,
   'ing': 1.2792257271403649,
   'orrow': 1.2792257271403649,
@@ -322,26 +322,26 @@
   '지': 1.2792257271403649}]
 ```
 
 ### Index
 [![STF-IDF Demo](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1RaWj5SqWvyC2SsCTGg8IAVcl9G5hOB50?usp=sharing)
 ```
 index = t2t.Handler([
-         "Let's go hiking tomorrow, let's go!", 
-         "안녕하세요.", 
+         "Let's go hiking tomorrow, let's go!",
+         "안녕하세요.",
          "돼지꿈을 꾸세요~~",
          ]).index(ids=[100, 101, 102])
 
 index.search(["돼지", "안녕", "let's go"], k=1)
 
 # Matching L2 distances and corresponding ids
 (
   array([[0.7752551],
         [0.8452994],
-        [0.4347524]], dtype=float32), 
+        [0.4347524]], dtype=float32),
   array([[102],
         [101],
         [100]])
 )
 
 # Add documents incrementing on ids if none specified
 index.add(["Hello, World! 你好,世界!"])
@@ -356,16 +356,16 @@
  array([[103, 100, 102]]))
 ```
 To learn more, see [STF-IDF](https://arxiv.org/abs/2209.14281).
 
 ### Search
 ```
 t2t.Handler([
-         "Let's go hiking tomorrow, let's go!", 
-         "안녕하세요.", 
+         "Let's go hiking tomorrow, let's go!",
+         "안녕하세요.",
          "돼지꿈을 꾸세요~~",
          ]).search(queries=["go", "안녕"])
 
 # Cosine similarity scores matrix
 array([[0.4472136 , 0.        , 0.        ],
        [0.        , 0.57735027, 0.        ]])
 ```
@@ -377,92 +377,92 @@
 notre_dame_str = "As at most other universities, Notre Dame's students run a number of news media outlets. The nine student - run outlets include three newspapers, both a radio and television station, and several magazines and journals. Begun as a one - page journal in September 1876, the Scholastic magazine is issued twice monthly and claims to be the oldest continuous collegiate publication in the United States. The other magazine, The Juggler, is released twice a year and focuses on student literature and artwork. The Dome yearbook is published annually. The newspapers have varying publication interests, with The Observer published daily and mainly reporting university and other news, and staffed by students from both Notre Dame and Saint Mary's College. Unlike Scholastic and The Dome, The Observer is an independent publication and does not have a faculty advisor or any editorial oversight from the University. In 1987, when some students believed that The Observer began to show a conservative bias, a liberal newspaper, Common Sense was published. Likewise, in 2003, when other students believed that the paper showed a liberal bias, the conservative paper Irish Rover went into production. Neither paper is published as often as The Observer; however, all three are distributed to all students. Finally, in Spring 2008 an undergraduate journal for political science research, Beyond Politics, made its debut."
 
 bacteria_str = "Bacteria are a type of biological cell. They constitute a large domain of prokaryotic microorganisms. Typically a few micrometres in length, bacteria have a number of shapes, ranging from spheres to rods and spirals. Bacteria were among the first life forms to appear on Earth, and are present in most of its habitats."
 
 bio_str = "Biology is the science that studies life. What exactly is life? This may sound like a silly question with an obvious answer, but it is not easy to define life. For example, a branch of biology called virology studies viruses, which exhibit some of the characteristics of living entities but lack others. It turns out that although viruses can attack living organisms, cause diseases, and even reproduce, they do not meet the criteria that biologists use to define life."
 
 bm25_index = t2t.Handler([
-                       article_en, 
-                       notre_dame_str, 
-                       bacteria_str, 
+                       article_en,
+                       notre_dame_str,
+                       bacteria_str,
                        bio_str
                        ]).bm25(output="matrix")
 
 search_results_bm25 = t2t.Handler().search(
-    queries=["wonderful life", "university students"], 
+    queries=["wonderful life", "university students"],
     vector_class=t2t.Bm25er,
     index=bm25_index)
 
 search_results_bm25_2 = t2t.Handler().search(
-    queries=["Earth creatures are cool", "United Nations"], 
+    queries=["Earth creatures are cool", "United Nations"],
     vector_class=t2t.Bm25er,
     index=bm25_index)
 ```
 
 #### Using TF-DF embeddings index
 ```
 tfidf_index = t2t.Handler([
-                       article_en, 
-                       notre_dame_str, 
-                       bacteria_str, 
+                       article_en,
+                       notre_dame_str,
+                       bacteria_str,
                        bio_str
                        ]).tfidf(output="matrix")
 
 search_results_tf = t2t.Handler().search(
-    queries=["wonderful life", "university students"], 
+    queries=["wonderful life", "university students"],
     vector_class=t2t.Tfidfer,
     index=tfidf_index)
 ```
 
 #### Using neural embeddings index
 ```
 embedding_index = t2t.Handler([
-                       article_en, 
-                       notre_dame_str, 
-                       bacteria_str, 
+                       article_en,
+                       notre_dame_str,
+                       bacteria_str,
                        bio_str
                        ]).vectorize()
 
 search_results_em = t2t.Handler().search(
     queries=["wonderful life", "university students"],
     vector_class=t2t.Vectorizer,
     index=embedding_index)
 ```
 
-#### Blending bm25, tf-idf and neural embeddings 
+#### Blending bm25, tf-idf and neural embeddings
 ```
-np.mean( 
+np.mean(
     np.array([
               search_results_bm25,
               search_results_tf,
               search_results_em,
               ]), axis=0)
 
 # averaged scores matrix
 #matrix([[ 0.00486117, -0.01890325,  0.53769584,  0.82506883],
 #        [ 0.0435048 ,  1.68977281,  0.01238902,  0.01266839]])
 ```
 
 ### Levenshtein Sub-word Edit Distance
 ```
 t2t.Handler([
-         "Hello, World! [SEP] Hello, what?", 
+         "Hello, World! [SEP] Hello, what?",
          "안녕하세요. [SEP] 돼지꿈을 꾸세요~~"
         ]).measure(metric="levenshtein_distance")
 
 # Distances
  [2, 8]
 ```
 
 ### Translation
 ```
 t2t.Handler([
-         article_en, 
-         notre_dame_str, 
-         bacteria_str, 
+         article_en,
+         notre_dame_str,
+         bacteria_str,
          bio_str
          ], src_lang='en').translate(tgt_lang='zh')
 
 # Translations
 ['联合国秘书长说,叙利亚没有军事解决方案。',
  '与大多数其他大学一样,Notre Dame的学生运行的新闻媒体渠道的数量。九个学生 - 运行的渠道包括三份报纸,两台广播电视台,以及几本杂志和杂志。 开始作为一个一页的杂志在1876年9月,该杂志的Schoolistic发行了每月两次,并声称是美国最古老的连续的大学新闻出版物,和其他杂志,TheJuggler,每年发行两次,并专注于学生文学和艺术作品。 多姆年刊每年发行。 报纸有不同的出版利益,与The Observer发表每日,主要报道大学和其他新闻,并由学生从Notre Dame和圣玛丽的学院。 与Scholastic和The Dome不同,The Observer是一个独立的公众作品,但没有教师顾',
  '细菌是生物细胞的一种类型. 它们构成一个大范围的亲生微生物. 通常几微米长,细菌有许多形状,从球到杖和螺旋。 细菌是地球上出现的第一个生命形式之一,并且存在于其大多数栖息地。',
@@ -529,27 +529,27 @@
   'tr_TR': 'Turkish',
   'uk_UA': 'Ukrainian',
   'ur_PK': 'Urdu',
   'vi_VN': 'Vietnamese',
   'xh_ZA': 'Xhosa',
   'zh_CN': 'Chinese'
 }
-t2t.Handler(["I would like to go hiking tomorrow."], 
+t2t.Handler(["I would like to go hiking tomorrow."],
         src_lang="en_XX"
         ).translate(tgt_lang='zh_CN')
 ['我想明天去徒步旅行。']
 ```
 
 </details>
 
 ### Question Answering
 Question must follow context with ` [SEP] ` in between.
 ```
 t2t.Handler([
-         "Hello, this is Text2Text! [SEP] What is this?", 
+         "Hello, this is Text2Text! [SEP] What is this?",
          "It works very well. It's awesome! [SEP] How is it?"
          ]).answer()
 
 t2t.Handler([
              "很喜欢陈慧琳唱歌。[SEP] 喜欢做什么?"
              ], src_lang="zh").answer()
 
@@ -746,18 +746,18 @@
 t2t.Handler([input_state]).respond()
 # ['About 60 different kinds of cats are recognized by various cat registries.']
 ```
 
 ### Training / Finetuning
 Finetune cross-lingual model on your data
 ```
-result = t2t.Handler(["Hello, World! [TGT] 你好,世界!"], 
+result = t2t.Handler(["Hello, World! [TGT] 你好,世界!"],
             src_lang="en",
             tgt_lang="zh",
-            num_epochs=10, 
+            num_epochs=10,
             save_directory="model_dir"
             ).fit()
 
 # load and use model from saved directory
 t2t.Transformer.PRETRAINED_TRANSLATOR = "model_dir"
 t2t.Handler("Hello, World!").translate(tgt_lang="zh")
 ```
@@ -781,15 +781,15 @@
 import socket
 import requests
 
 address = socket.gethostbyname(socket.getfqdn(socket.gethostname()))
 url = f"http://{address}"
 transform = "translate"
 payload = {
-  "input_lines": ["hello", "world"], 
+  "input_lines": ["hello", "world"],
   "src_lang": "en",
   "tgt_lang": "ko",
 }
 r = requests.post(f"{url}/{transform}", json=payload)
 print(r.json()) #{'result': ['안녕하세요', '세계']}
 
 # Indexer actions
```

### Comparing `text2text-1.0.8/text2text.egg-info/SOURCES.txt` & `text2text-1.0.9/text2text.egg-info/SOURCES.txt`

 * *Files identical despite different names*

