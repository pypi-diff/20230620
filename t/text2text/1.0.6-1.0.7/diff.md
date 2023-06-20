# Comparing `tmp/text2text-1.0.6.tar.gz` & `tmp/text2text-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text2text-1.0.6.tar", last modified: Tue Jun 20 03:56:54 2023, max compression
+gzip compressed data, was "text2text-1.0.7.tar", last modified: Tue Jun 20 04:09:37 2023, max compression
```

## Comparing `text2text-1.0.6.tar` & `text2text-1.0.7.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 03:56:54.010872 text2text-1.0.6/
--rwxr-xr-x   0 root         (0) root         (0)     1418 2023-06-20 01:53:21.000000 text2text-1.0.6/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    60118 2023-06-20 03:56:54.010872 text2text-1.0.6/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)    59304 2023-06-20 03:55:26.000000 text2text-1.0.6/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-20 03:56:54.011872 text2text-1.0.6/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1246 2023-06-20 03:55:52.000000 text2text-1.0.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 03:56:54.006872 text2text-1.0.6/text2text/
--rwxr-xr-x   0 root         (0) root         (0)      666 2023-06-20 02:25:27.000000 text2text-1.0.6/text2text/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7162 2023-06-20 01:53:21.000000 text2text-1.0.6/text2text/abstractor.py
--rw-r--r--   0 root         (0) root         (0)     2157 2023-06-20 01:53:21.000000 text2text-1.0.6/text2text/answerer.py
--rw-r--r--   0 root         (0) root         (0)     2287 2023-06-20 03:27:52.000000 text2text-1.0.6/text2text/assistant.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 03:56:54.008872 text2text-1.0.6/text2text/biunilm/
--rwxr-xr-x   0 root         (0) root         (0)      110 2023-06-20 01:53:21.000000 text2text-1.0.6/text2text/biunilm/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    10937 2023-06-20 01:53:21.000000 text2text-1.0.6/text2text/biunilm/loader_utils.py
--rwxr-xr-x   0 root         (0) root         (0)    17726 2023-06-20 01:53:21.000000 text2text-1.0.6/text2text/biunilm/seq2seq_loader.py
--rw-r--r--   0 root         (0) root         (0)     1533 2023-06-20 01:53:21.000000 text2text-1.0.6/text2text/bm25er.py
--rw-r--r--   0 root         (0) root         (0)      519 2023-06-20 01:53:21.000000 text2text-1.0.6/text2text/counter.py
--rw-r--r--   0 root         (0) root         (0)     1177 2023-06-20 01:53:21.000000 text2text-1.0.6/text2text/fitter.py
--rw-r--r--   0 root         (0) root         (0)     1451 2023-06-20 01:53:21.000000 text2text-1.0.6/text2text/handler.py
--rw-r--r--   0 root         (0) root         (0)     2106 2023-06-20 01:53:21.000000 text2text-1.0.6/text2text/identifier.py
--rw-r--r--   0 root         (0) root         (0)     2010 2023-06-20 03:29:02.000000 text2text-1.0.6/text2text/indexer.py
--rw-r--r--   0 root         (0) root         (0)     1165 2023-06-20 01:53:21.000000 text2text-1.0.6/text2text/measurer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 03:56:54.009872 text2text-1.0.6/text2text/pytorch_pretrained_bert/
--rwxr-xr-x   0 root         (0) root         (0)      120 2023-06-20 01:53:21.000000 text2text-1.0.6/text2text/pytorch_pretrained_bert/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      932 2023-06-20 01:53:21.000000 text2text-1.0.6/text2text/pytorch_pretrained_bert/__main__.py
--rwxr-xr-x   0 root         (0) root         (0)     7964 2023-06-20 01:53:21.000000 text2text-1.0.6/text2text/pytorch_pretrained_bert/file_utils.py
--rwxr-xr-x   0 root         (0) root         (0)     1821 2023-06-20 01:53:21.000000 text2text-1.0.6/text2text/pytorch_pretrained_bert/loss.py
--rwxr-xr-x   0 root         (0) root         (0)   108506 2023-06-20 01:53:21.000000 text2text-1.0.6/text2text/pytorch_pretrained_bert/modeling.py
--rwxr-xr-x   0 root         (0) root         (0)    15035 2023-06-20 01:53:21.000000 text2text-1.0.6/text2text/pytorch_pretrained_bert/tokenization.py
--rw-r--r--   0 root         (0) root         (0)     1782 2023-06-20 01:53:21.000000 text2text-1.0.6/text2text/questioner.py
--rw-r--r--   0 root         (0) root         (0)     2605 2023-06-20 03:20:23.000000 text2text-1.0.6/text2text/responder.py
--rw-r--r--   0 root         (0) root         (0)      984 2023-06-20 01:53:21.000000 text2text-1.0.6/text2text/searcher.py
--rw-r--r--   0 root         (0) root         (0)     1575 2023-06-20 01:53:21.000000 text2text-1.0.6/text2text/server.py
--rw-r--r--   0 root         (0) root         (0)     1103 2023-06-20 01:53:21.000000 text2text-1.0.6/text2text/summarizer.py
--rw-r--r--   0 root         (0) root         (0)     1766 2023-06-20 01:53:21.000000 text2text-1.0.6/text2text/tfidfer.py
--rw-r--r--   0 root         (0) root         (0)      780 2023-06-20 01:53:21.000000 text2text-1.0.6/text2text/tokenizer.py
--rw-r--r--   0 root         (0) root         (0)    12572 2023-06-20 02:51:51.000000 text2text-1.0.6/text2text/transformer.py
--rw-r--r--   0 root         (0) root         (0)     1489 2023-06-20 01:53:21.000000 text2text-1.0.6/text2text/translator.py
--rw-r--r--   0 root         (0) root         (0)      500 2023-06-20 01:53:21.000000 text2text-1.0.6/text2text/variator.py
--rw-r--r--   0 root         (0) root         (0)      816 2023-06-20 01:53:21.000000 text2text-1.0.6/text2text/vectorizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 03:56:54.007872 text2text-1.0.6/text2text.egg-info/
--rw-r--r--   0 root         (0) root         (0)    60118 2023-06-20 03:56:53.000000 text2text-1.0.6/text2text.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1064 2023-06-20 03:56:53.000000 text2text-1.0.6/text2text.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 03:56:53.000000 text2text-1.0.6/text2text.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      134 2023-06-20 03:56:53.000000 text2text-1.0.6/text2text.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-20 03:56:53.000000 text2text-1.0.6/text2text.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 04:09:37.093993 text2text-1.0.7/
+-rwxr-xr-x   0 root         (0) root         (0)     1418 2023-06-20 01:53:21.000000 text2text-1.0.7/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    60454 2023-06-20 04:09:37.093993 text2text-1.0.7/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)    59640 2023-06-20 04:08:26.000000 text2text-1.0.7/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-20 04:09:37.093993 text2text-1.0.7/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1246 2023-06-20 04:08:56.000000 text2text-1.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 04:09:37.089992 text2text-1.0.7/text2text/
+-rwxr-xr-x   0 root         (0) root         (0)      666 2023-06-20 02:25:27.000000 text2text-1.0.7/text2text/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7162 2023-06-20 01:53:21.000000 text2text-1.0.7/text2text/abstractor.py
+-rw-r--r--   0 root         (0) root         (0)     2157 2023-06-20 01:53:21.000000 text2text-1.0.7/text2text/answerer.py
+-rw-r--r--   0 root         (0) root         (0)     2287 2023-06-20 03:27:52.000000 text2text-1.0.7/text2text/assistant.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 04:09:37.091992 text2text-1.0.7/text2text/biunilm/
+-rwxr-xr-x   0 root         (0) root         (0)      110 2023-06-20 01:53:21.000000 text2text-1.0.7/text2text/biunilm/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    10937 2023-06-20 01:53:21.000000 text2text-1.0.7/text2text/biunilm/loader_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)    17726 2023-06-20 01:53:21.000000 text2text-1.0.7/text2text/biunilm/seq2seq_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-06-20 01:53:21.000000 text2text-1.0.7/text2text/bm25er.py
+-rw-r--r--   0 root         (0) root         (0)      519 2023-06-20 01:53:21.000000 text2text-1.0.7/text2text/counter.py
+-rw-r--r--   0 root         (0) root         (0)     1177 2023-06-20 01:53:21.000000 text2text-1.0.7/text2text/fitter.py
+-rw-r--r--   0 root         (0) root         (0)     1451 2023-06-20 01:53:21.000000 text2text-1.0.7/text2text/handler.py
+-rw-r--r--   0 root         (0) root         (0)     2106 2023-06-20 01:53:21.000000 text2text-1.0.7/text2text/identifier.py
+-rw-r--r--   0 root         (0) root         (0)     2010 2023-06-20 03:29:02.000000 text2text-1.0.7/text2text/indexer.py
+-rw-r--r--   0 root         (0) root         (0)     1165 2023-06-20 01:53:21.000000 text2text-1.0.7/text2text/measurer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 04:09:37.092993 text2text-1.0.7/text2text/pytorch_pretrained_bert/
+-rwxr-xr-x   0 root         (0) root         (0)      120 2023-06-20 01:53:21.000000 text2text-1.0.7/text2text/pytorch_pretrained_bert/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      932 2023-06-20 01:53:21.000000 text2text-1.0.7/text2text/pytorch_pretrained_bert/__main__.py
+-rwxr-xr-x   0 root         (0) root         (0)     7964 2023-06-20 01:53:21.000000 text2text-1.0.7/text2text/pytorch_pretrained_bert/file_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)     1821 2023-06-20 01:53:21.000000 text2text-1.0.7/text2text/pytorch_pretrained_bert/loss.py
+-rwxr-xr-x   0 root         (0) root         (0)   108506 2023-06-20 01:53:21.000000 text2text-1.0.7/text2text/pytorch_pretrained_bert/modeling.py
+-rwxr-xr-x   0 root         (0) root         (0)    15035 2023-06-20 01:53:21.000000 text2text-1.0.7/text2text/pytorch_pretrained_bert/tokenization.py
+-rw-r--r--   0 root         (0) root         (0)     1782 2023-06-20 01:53:21.000000 text2text-1.0.7/text2text/questioner.py
+-rw-r--r--   0 root         (0) root         (0)     2605 2023-06-20 03:20:23.000000 text2text-1.0.7/text2text/responder.py
+-rw-r--r--   0 root         (0) root         (0)      984 2023-06-20 01:53:21.000000 text2text-1.0.7/text2text/searcher.py
+-rw-r--r--   0 root         (0) root         (0)     1575 2023-06-20 01:53:21.000000 text2text-1.0.7/text2text/server.py
+-rw-r--r--   0 root         (0) root         (0)     1103 2023-06-20 01:53:21.000000 text2text-1.0.7/text2text/summarizer.py
+-rw-r--r--   0 root         (0) root         (0)     1766 2023-06-20 01:53:21.000000 text2text-1.0.7/text2text/tfidfer.py
+-rw-r--r--   0 root         (0) root         (0)      780 2023-06-20 01:53:21.000000 text2text-1.0.7/text2text/tokenizer.py
+-rw-r--r--   0 root         (0) root         (0)    12572 2023-06-20 02:51:51.000000 text2text-1.0.7/text2text/transformer.py
+-rw-r--r--   0 root         (0) root         (0)     1489 2023-06-20 01:53:21.000000 text2text-1.0.7/text2text/translator.py
+-rw-r--r--   0 root         (0) root         (0)      500 2023-06-20 01:53:21.000000 text2text-1.0.7/text2text/variator.py
+-rw-r--r--   0 root         (0) root         (0)      816 2023-06-20 01:53:21.000000 text2text-1.0.7/text2text/vectorizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 04:09:37.090992 text2text-1.0.7/text2text.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    60454 2023-06-20 04:09:36.000000 text2text-1.0.7/text2text.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1064 2023-06-20 04:09:36.000000 text2text-1.0.7/text2text.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 04:09:36.000000 text2text-1.0.7/text2text.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      134 2023-06-20 04:09:36.000000 text2text-1.0.7/text2text.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-20 04:09:36.000000 text2text-1.0.7/text2text.egg-info/top_level.txt
```

### Comparing `text2text-1.0.6/LICENSE.txt` & `text2text-1.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `text2text-1.0.6/PKG-INFO` & `text2text-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2text
-Version: 1.0.6
+Version: 1.0.7
 Summary: Text2Text: Crosslingual NLP/G toolkit
 Home-page: https://github.com/artitw/text2text
 Author: Artit Wangperawong
 Author-email: artitw@gmail.com
 Keywords: multilingual crosslingual gpt chatgpt bert natural language processing nlp nlg text generation gpt question answer answering information retrieval tfidf tf-idf bm25 search index summary summarizer summarization tokenizer tokenization translation backtranslation data augmentation science machine learning colab embedding levenshtein sub-word edit distance conversational dialog chatbot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -46,47 +46,33 @@
 * [Questions?](https://github.com/artitw/text2text#questions)
 * [Citation](https://github.com/artitw/text2text#citation)
 * [Contributing](https://github.com/artitw/text2text#contributing)
 * [Code of Conduct](https://github.com/artitw/text2text#code-of-conduct)
 
 </details>
 
-## Colab Demo
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1LE_ifTpOGO5QJCKNQYtZe6c_tjbwnulR)
+## Colab Notebooks
+* Assistant with knowledge base [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1hkNgpSmmUA-mzUibqz25xq-E8KYOLuVx?usp=sharing)
+* STF-IDF multilingual search [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1RaWj5SqWvyC2SsCTGg8IAVcl9G5hOB50?usp=sharing)
+* All examples [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1LE_ifTpOGO5QJCKNQYtZe6c_tjbwnulR)
 
 ## How Crosslingual Models Work (click to watch)
 [![Crosslingual Models](http://img.youtube.com/vi/caZLVcJqsqo/0.jpg)](https://youtu.be/caZLVcJqsqo "Cross-Lingual Models")
 
 ## Installation Requirements 
 ```
 pip install -qq -U text2text
 ```
-* All functionality in the demo and examples work with <16 GB RAM, which means they run on Colab.
-  * See [Colab Demo](https://colab.research.google.com/drive/1LE_ifTpOGO5QJCKNQYtZe6c_tjbwnulR) and [Examples](#examples) below
-
-## Class Diagram
-```
-      Indexer    Measurer   Counter -- Tfidfer
-           \          \     /             \
-        Searcher     Tokenizer           Bm25er
-             \_______    |      ________________ Assistant
-              _______Transformer______________
-             /           |                    \
-        Answerer     Translator              Abstractor
-           /         /    |     \              /       \
-  Responder  Vectorizer  Fitter  Variator  Questioner  Summarizer
-                  /
-          Identifier
-```
+* [Examples](#examples) all work with <16 GB RAM, so they run free on [Colab](https://colab.research.google.com/drive/1LE_ifTpOGO5QJCKNQYtZe6c_tjbwnulR).
 
 ## Quick Start Guide
 Functionality | Invocation | Result
 :------------: | :-------------: | :-------------:
 Module Importing | `import text2text as t2t` | Libraries imported
-[Assistant](https://github.com/artitw/text2text#assistant) | `t2t.Handler(["Describe Text2Text in a few words: "]).assist()` | `['Text2Text is an AI-powered text generation tool that creates coherent and continuous text based on prompts.']`
+[Assistant](https://github.com/artitw/text2text#assistant) | `t2t.Handler("Describe Text2Text in a few words: ").assist()` | `['Text2Text is an AI-powered text generation tool that creates coherent and continuous text based on prompts.']`
 Language Model Setting | `t2t.Transformer.PRETRAINED_TRANSLATOR = "facebook/m2m100_418M"` | Change from default
 Text Handler | `h = t2t.Handler(["Hello, World!"], src_lang="en")` | Initialized handler with some text
 [Tokenization](https://github.com/artitw/text2text#tokenization) | `h.tokenize()` | `[['▁Hello', ',', '▁World', '!']]`
 [Embedding](https://github.com/artitw/text2text#embedding--vectorization) | `h.vectorize()` | `array([[0.18745188, 0.05658336, ..., 0.6332584 , 0.43805206]], dtype=float32)`
 [TF-IDF](https://github.com/artitw/text2text#tf-idf) | `h.tfidf()` | `[{'!': 0.5, ',': 0.5, '▁Hello': 0.5, '▁World': 0.5}]`
 [BM25](https://github.com/artitw/text2text#bm25) | `h.bm25()` | `[{'!': 0.3068528194400547, ',': 0.3068528194400547, '▁Hello': 0.3068528194400547, '▁World': 0.3068528194400547}]`
 [Indexer](https://github.com/artitw/text2text#index) | `i = h.index()` | Index object for similarity retrieval
@@ -98,14 +84,29 @@
 [Dialog Response](https://github.com/artitw/text2text#dialog-responder) | `t2t.Handler(["[CONTEXT] Hello EOS How are you?"]).respond()` | `['I am doing great. How are you?']`
 [Question Answering](https://github.com/artitw/text2text#question-answering) | `t2t.Handler(["Hello, World! [SEP] Hello, what?"]).answer()` | `['World']`
 [Distance](https://github.com/artitw/text2text#levenshtein-sub-word-edit-distance) | `t2t.Handler(["Hello, World! [SEP] Hello, what?"]).measure()` | `[2]`
 [Training/Finetuning](https://github.com/artitw/text2text#training--finetuning) | `t2t.Handler(["Hello, World! [TGT] Hello, what?"]).fit()` | Finetuned model saved
 [Identification](https://github.com/artitw/text2text#identification) | `t2t.Handler(["Aj keď sa Buzz Aldrin stal až „druhým človekom“..."]).identify()` | `['sk', 'Slovak']`
 [Web Server](https://github.com/artitw/text2text#serving) | `t2t.Server(host='0.0.0.0', port=80)` | Web server started on host and port
 
+## Class Diagram
+```
+      Indexer    Measurer   Counter -- Tfidfer
+           \          \     /             \
+        Searcher     Tokenizer           Bm25er
+             \_______    |      ________________ Assistant
+              _______Transformer______________
+             /           |                    \
+        Answerer     Translator              Abstractor
+           /         /    |     \              /       \
+  Responder  Vectorizer  Fitter  Variator  Questioner  Summarizer
+                  /
+          Identifier
+```
+
 ## Languages Available
 <details>
   <summary>Show all</summary>
 
 ```
 t2t.Transformer.LANGUAGES
```

### Comparing `text2text-1.0.6/README.md` & `text2text-1.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -32,47 +32,33 @@
 * [Questions?](https://github.com/artitw/text2text#questions)
 * [Citation](https://github.com/artitw/text2text#citation)
 * [Contributing](https://github.com/artitw/text2text#contributing)
 * [Code of Conduct](https://github.com/artitw/text2text#code-of-conduct)
 
 </details>
 
-## Colab Demo
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1LE_ifTpOGO5QJCKNQYtZe6c_tjbwnulR)
+## Colab Notebooks
+* Assistant with knowledge base [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1hkNgpSmmUA-mzUibqz25xq-E8KYOLuVx?usp=sharing)
+* STF-IDF multilingual search [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1RaWj5SqWvyC2SsCTGg8IAVcl9G5hOB50?usp=sharing)
+* All examples [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1LE_ifTpOGO5QJCKNQYtZe6c_tjbwnulR)
 
 ## How Crosslingual Models Work (click to watch)
 [![Crosslingual Models](http://img.youtube.com/vi/caZLVcJqsqo/0.jpg)](https://youtu.be/caZLVcJqsqo "Cross-Lingual Models")
 
 ## Installation Requirements 
 ```
 pip install -qq -U text2text
 ```
-* All functionality in the demo and examples work with <16 GB RAM, which means they run on Colab.
-  * See [Colab Demo](https://colab.research.google.com/drive/1LE_ifTpOGO5QJCKNQYtZe6c_tjbwnulR) and [Examples](#examples) below
-
-## Class Diagram
-```
-      Indexer    Measurer   Counter -- Tfidfer
-           \          \     /             \
-        Searcher     Tokenizer           Bm25er
-             \_______    |      ________________ Assistant
-              _______Transformer______________
-             /           |                    \
-        Answerer     Translator              Abstractor
-           /         /    |     \              /       \
-  Responder  Vectorizer  Fitter  Variator  Questioner  Summarizer
-                  /
-          Identifier
-```
+* [Examples](#examples) all work with <16 GB RAM, so they run free on [Colab](https://colab.research.google.com/drive/1LE_ifTpOGO5QJCKNQYtZe6c_tjbwnulR).
 
 ## Quick Start Guide
 Functionality | Invocation | Result
 :------------: | :-------------: | :-------------:
 Module Importing | `import text2text as t2t` | Libraries imported
-[Assistant](https://github.com/artitw/text2text#assistant) | `t2t.Handler(["Describe Text2Text in a few words: "]).assist()` | `['Text2Text is an AI-powered text generation tool that creates coherent and continuous text based on prompts.']`
+[Assistant](https://github.com/artitw/text2text#assistant) | `t2t.Handler("Describe Text2Text in a few words: ").assist()` | `['Text2Text is an AI-powered text generation tool that creates coherent and continuous text based on prompts.']`
 Language Model Setting | `t2t.Transformer.PRETRAINED_TRANSLATOR = "facebook/m2m100_418M"` | Change from default
 Text Handler | `h = t2t.Handler(["Hello, World!"], src_lang="en")` | Initialized handler with some text
 [Tokenization](https://github.com/artitw/text2text#tokenization) | `h.tokenize()` | `[['▁Hello', ',', '▁World', '!']]`
 [Embedding](https://github.com/artitw/text2text#embedding--vectorization) | `h.vectorize()` | `array([[0.18745188, 0.05658336, ..., 0.6332584 , 0.43805206]], dtype=float32)`
 [TF-IDF](https://github.com/artitw/text2text#tf-idf) | `h.tfidf()` | `[{'!': 0.5, ',': 0.5, '▁Hello': 0.5, '▁World': 0.5}]`
 [BM25](https://github.com/artitw/text2text#bm25) | `h.bm25()` | `[{'!': 0.3068528194400547, ',': 0.3068528194400547, '▁Hello': 0.3068528194400547, '▁World': 0.3068528194400547}]`
 [Indexer](https://github.com/artitw/text2text#index) | `i = h.index()` | Index object for similarity retrieval
@@ -84,14 +70,29 @@
 [Dialog Response](https://github.com/artitw/text2text#dialog-responder) | `t2t.Handler(["[CONTEXT] Hello EOS How are you?"]).respond()` | `['I am doing great. How are you?']`
 [Question Answering](https://github.com/artitw/text2text#question-answering) | `t2t.Handler(["Hello, World! [SEP] Hello, what?"]).answer()` | `['World']`
 [Distance](https://github.com/artitw/text2text#levenshtein-sub-word-edit-distance) | `t2t.Handler(["Hello, World! [SEP] Hello, what?"]).measure()` | `[2]`
 [Training/Finetuning](https://github.com/artitw/text2text#training--finetuning) | `t2t.Handler(["Hello, World! [TGT] Hello, what?"]).fit()` | Finetuned model saved
 [Identification](https://github.com/artitw/text2text#identification) | `t2t.Handler(["Aj keď sa Buzz Aldrin stal až „druhým človekom“..."]).identify()` | `['sk', 'Slovak']`
 [Web Server](https://github.com/artitw/text2text#serving) | `t2t.Server(host='0.0.0.0', port=80)` | Web server started on host and port
 
+## Class Diagram
+```
+      Indexer    Measurer   Counter -- Tfidfer
+           \          \     /             \
+        Searcher     Tokenizer           Bm25er
+             \_______    |      ________________ Assistant
+              _______Transformer______________
+             /           |                    \
+        Answerer     Translator              Abstractor
+           /         /    |     \              /       \
+  Responder  Vectorizer  Fitter  Variator  Questioner  Summarizer
+                  /
+          Identifier
+```
+
 ## Languages Available
 <details>
   <summary>Show all</summary>
 
 ```
 t2t.Transformer.LANGUAGES
```

### Comparing `text2text-1.0.6/setup.py` & `text2text-1.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="text2text",
-  version="1.0.6",
+  version="1.0.7",
   author="Artit Wangperawong",
   author_email="artitw@gmail.com",
   description="Text2Text: Crosslingual NLP/G toolkit",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/artitw/text2text",
   packages=setuptools.find_packages(),
```

### Comparing `text2text-1.0.6/text2text/__init__.py` & `text2text-1.0.7/text2text/__init__.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.6/text2text/abstractor.py` & `text2text-1.0.7/text2text/abstractor.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.6/text2text/answerer.py` & `text2text-1.0.7/text2text/answerer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.6/text2text/assistant.py` & `text2text-1.0.7/text2text/assistant.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.6/text2text/biunilm/loader_utils.py` & `text2text-1.0.7/text2text/biunilm/loader_utils.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.6/text2text/biunilm/seq2seq_loader.py` & `text2text-1.0.7/text2text/biunilm/seq2seq_loader.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.6/text2text/bm25er.py` & `text2text-1.0.7/text2text/bm25er.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.6/text2text/counter.py` & `text2text-1.0.7/text2text/counter.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.6/text2text/fitter.py` & `text2text-1.0.7/text2text/fitter.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.6/text2text/handler.py` & `text2text-1.0.7/text2text/handler.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.6/text2text/identifier.py` & `text2text-1.0.7/text2text/identifier.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.6/text2text/indexer.py` & `text2text-1.0.7/text2text/indexer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.6/text2text/measurer.py` & `text2text-1.0.7/text2text/measurer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.6/text2text/pytorch_pretrained_bert/__main__.py` & `text2text-1.0.7/text2text/pytorch_pretrained_bert/__main__.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.6/text2text/pytorch_pretrained_bert/file_utils.py` & `text2text-1.0.7/text2text/pytorch_pretrained_bert/file_utils.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.6/text2text/pytorch_pretrained_bert/loss.py` & `text2text-1.0.7/text2text/pytorch_pretrained_bert/loss.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.6/text2text/pytorch_pretrained_bert/modeling.py` & `text2text-1.0.7/text2text/pytorch_pretrained_bert/modeling.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.6/text2text/pytorch_pretrained_bert/tokenization.py` & `text2text-1.0.7/text2text/pytorch_pretrained_bert/tokenization.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.6/text2text/questioner.py` & `text2text-1.0.7/text2text/questioner.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.6/text2text/responder.py` & `text2text-1.0.7/text2text/responder.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.6/text2text/searcher.py` & `text2text-1.0.7/text2text/searcher.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.6/text2text/server.py` & `text2text-1.0.7/text2text/server.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.6/text2text/summarizer.py` & `text2text-1.0.7/text2text/summarizer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.6/text2text/tfidfer.py` & `text2text-1.0.7/text2text/tfidfer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.6/text2text/tokenizer.py` & `text2text-1.0.7/text2text/tokenizer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.6/text2text/transformer.py` & `text2text-1.0.7/text2text/transformer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.6/text2text/translator.py` & `text2text-1.0.7/text2text/translator.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.6/text2text/vectorizer.py` & `text2text-1.0.7/text2text/vectorizer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.6/text2text.egg-info/PKG-INFO` & `text2text-1.0.7/text2text.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2text
-Version: 1.0.6
+Version: 1.0.7
 Summary: Text2Text: Crosslingual NLP/G toolkit
 Home-page: https://github.com/artitw/text2text
 Author: Artit Wangperawong
 Author-email: artitw@gmail.com
 Keywords: multilingual crosslingual gpt chatgpt bert natural language processing nlp nlg text generation gpt question answer answering information retrieval tfidf tf-idf bm25 search index summary summarizer summarization tokenizer tokenization translation backtranslation data augmentation science machine learning colab embedding levenshtein sub-word edit distance conversational dialog chatbot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -46,47 +46,33 @@
 * [Questions?](https://github.com/artitw/text2text#questions)
 * [Citation](https://github.com/artitw/text2text#citation)
 * [Contributing](https://github.com/artitw/text2text#contributing)
 * [Code of Conduct](https://github.com/artitw/text2text#code-of-conduct)
 
 </details>
 
-## Colab Demo
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1LE_ifTpOGO5QJCKNQYtZe6c_tjbwnulR)
+## Colab Notebooks
+* Assistant with knowledge base [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1hkNgpSmmUA-mzUibqz25xq-E8KYOLuVx?usp=sharing)
+* STF-IDF multilingual search [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1RaWj5SqWvyC2SsCTGg8IAVcl9G5hOB50?usp=sharing)
+* All examples [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1LE_ifTpOGO5QJCKNQYtZe6c_tjbwnulR)
 
 ## How Crosslingual Models Work (click to watch)
 [![Crosslingual Models](http://img.youtube.com/vi/caZLVcJqsqo/0.jpg)](https://youtu.be/caZLVcJqsqo "Cross-Lingual Models")
 
 ## Installation Requirements 
 ```
 pip install -qq -U text2text
 ```
-* All functionality in the demo and examples work with <16 GB RAM, which means they run on Colab.
-  * See [Colab Demo](https://colab.research.google.com/drive/1LE_ifTpOGO5QJCKNQYtZe6c_tjbwnulR) and [Examples](#examples) below
-
-## Class Diagram
-```
-      Indexer    Measurer   Counter -- Tfidfer
-           \          \     /             \
-        Searcher     Tokenizer           Bm25er
-             \_______    |      ________________ Assistant
-              _______Transformer______________
-             /           |                    \
-        Answerer     Translator              Abstractor
-           /         /    |     \              /       \
-  Responder  Vectorizer  Fitter  Variator  Questioner  Summarizer
-                  /
-          Identifier
-```
+* [Examples](#examples) all work with <16 GB RAM, so they run free on [Colab](https://colab.research.google.com/drive/1LE_ifTpOGO5QJCKNQYtZe6c_tjbwnulR).
 
 ## Quick Start Guide
 Functionality | Invocation | Result
 :------------: | :-------------: | :-------------:
 Module Importing | `import text2text as t2t` | Libraries imported
-[Assistant](https://github.com/artitw/text2text#assistant) | `t2t.Handler(["Describe Text2Text in a few words: "]).assist()` | `['Text2Text is an AI-powered text generation tool that creates coherent and continuous text based on prompts.']`
+[Assistant](https://github.com/artitw/text2text#assistant) | `t2t.Handler("Describe Text2Text in a few words: ").assist()` | `['Text2Text is an AI-powered text generation tool that creates coherent and continuous text based on prompts.']`
 Language Model Setting | `t2t.Transformer.PRETRAINED_TRANSLATOR = "facebook/m2m100_418M"` | Change from default
 Text Handler | `h = t2t.Handler(["Hello, World!"], src_lang="en")` | Initialized handler with some text
 [Tokenization](https://github.com/artitw/text2text#tokenization) | `h.tokenize()` | `[['▁Hello', ',', '▁World', '!']]`
 [Embedding](https://github.com/artitw/text2text#embedding--vectorization) | `h.vectorize()` | `array([[0.18745188, 0.05658336, ..., 0.6332584 , 0.43805206]], dtype=float32)`
 [TF-IDF](https://github.com/artitw/text2text#tf-idf) | `h.tfidf()` | `[{'!': 0.5, ',': 0.5, '▁Hello': 0.5, '▁World': 0.5}]`
 [BM25](https://github.com/artitw/text2text#bm25) | `h.bm25()` | `[{'!': 0.3068528194400547, ',': 0.3068528194400547, '▁Hello': 0.3068528194400547, '▁World': 0.3068528194400547}]`
 [Indexer](https://github.com/artitw/text2text#index) | `i = h.index()` | Index object for similarity retrieval
@@ -98,14 +84,29 @@
 [Dialog Response](https://github.com/artitw/text2text#dialog-responder) | `t2t.Handler(["[CONTEXT] Hello EOS How are you?"]).respond()` | `['I am doing great. How are you?']`
 [Question Answering](https://github.com/artitw/text2text#question-answering) | `t2t.Handler(["Hello, World! [SEP] Hello, what?"]).answer()` | `['World']`
 [Distance](https://github.com/artitw/text2text#levenshtein-sub-word-edit-distance) | `t2t.Handler(["Hello, World! [SEP] Hello, what?"]).measure()` | `[2]`
 [Training/Finetuning](https://github.com/artitw/text2text#training--finetuning) | `t2t.Handler(["Hello, World! [TGT] Hello, what?"]).fit()` | Finetuned model saved
 [Identification](https://github.com/artitw/text2text#identification) | `t2t.Handler(["Aj keď sa Buzz Aldrin stal až „druhým človekom“..."]).identify()` | `['sk', 'Slovak']`
 [Web Server](https://github.com/artitw/text2text#serving) | `t2t.Server(host='0.0.0.0', port=80)` | Web server started on host and port
 
+## Class Diagram
+```
+      Indexer    Measurer   Counter -- Tfidfer
+           \          \     /             \
+        Searcher     Tokenizer           Bm25er
+             \_______    |      ________________ Assistant
+              _______Transformer______________
+             /           |                    \
+        Answerer     Translator              Abstractor
+           /         /    |     \              /       \
+  Responder  Vectorizer  Fitter  Variator  Questioner  Summarizer
+                  /
+          Identifier
+```
+
 ## Languages Available
 <details>
   <summary>Show all</summary>
 
 ```
 t2t.Transformer.LANGUAGES
```

### Comparing `text2text-1.0.6/text2text.egg-info/SOURCES.txt` & `text2text-1.0.7/text2text.egg-info/SOURCES.txt`

 * *Files identical despite different names*

