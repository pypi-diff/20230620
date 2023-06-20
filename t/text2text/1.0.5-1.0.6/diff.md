# Comparing `tmp/text2text-1.0.5.tar.gz` & `tmp/text2text-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text2text-1.0.5.tar", last modified: Tue Jun 20 03:42:18 2023, max compression
+gzip compressed data, was "text2text-1.0.6.tar", last modified: Tue Jun 20 03:56:54 2023, max compression
```

## Comparing `text2text-1.0.5.tar` & `text2text-1.0.6.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 03:42:18.389214 text2text-1.0.5/
--rwxr-xr-x   0 root         (0) root         (0)     1418 2023-06-20 01:53:21.000000 text2text-1.0.5/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    60233 2023-06-20 03:42:18.389214 text2text-1.0.5/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)    59419 2023-06-20 03:41:03.000000 text2text-1.0.5/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-20 03:42:18.389214 text2text-1.0.5/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1246 2023-06-20 03:41:58.000000 text2text-1.0.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 03:42:18.385214 text2text-1.0.5/text2text/
--rwxr-xr-x   0 root         (0) root         (0)      666 2023-06-20 02:25:27.000000 text2text-1.0.5/text2text/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7162 2023-06-20 01:53:21.000000 text2text-1.0.5/text2text/abstractor.py
--rw-r--r--   0 root         (0) root         (0)     2157 2023-06-20 01:53:21.000000 text2text-1.0.5/text2text/answerer.py
--rw-r--r--   0 root         (0) root         (0)     2287 2023-06-20 03:27:52.000000 text2text-1.0.5/text2text/assistant.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 03:42:18.387214 text2text-1.0.5/text2text/biunilm/
--rwxr-xr-x   0 root         (0) root         (0)      110 2023-06-20 01:53:21.000000 text2text-1.0.5/text2text/biunilm/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    10937 2023-06-20 01:53:21.000000 text2text-1.0.5/text2text/biunilm/loader_utils.py
--rwxr-xr-x   0 root         (0) root         (0)    17726 2023-06-20 01:53:21.000000 text2text-1.0.5/text2text/biunilm/seq2seq_loader.py
--rw-r--r--   0 root         (0) root         (0)     1533 2023-06-20 01:53:21.000000 text2text-1.0.5/text2text/bm25er.py
--rw-r--r--   0 root         (0) root         (0)      519 2023-06-20 01:53:21.000000 text2text-1.0.5/text2text/counter.py
--rw-r--r--   0 root         (0) root         (0)     1177 2023-06-20 01:53:21.000000 text2text-1.0.5/text2text/fitter.py
--rw-r--r--   0 root         (0) root         (0)     1451 2023-06-20 01:53:21.000000 text2text-1.0.5/text2text/handler.py
--rw-r--r--   0 root         (0) root         (0)     2106 2023-06-20 01:53:21.000000 text2text-1.0.5/text2text/identifier.py
--rw-r--r--   0 root         (0) root         (0)     2010 2023-06-20 03:29:02.000000 text2text-1.0.5/text2text/indexer.py
--rw-r--r--   0 root         (0) root         (0)     1165 2023-06-20 01:53:21.000000 text2text-1.0.5/text2text/measurer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 03:42:18.388214 text2text-1.0.5/text2text/pytorch_pretrained_bert/
--rwxr-xr-x   0 root         (0) root         (0)      120 2023-06-20 01:53:21.000000 text2text-1.0.5/text2text/pytorch_pretrained_bert/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      932 2023-06-20 01:53:21.000000 text2text-1.0.5/text2text/pytorch_pretrained_bert/__main__.py
--rwxr-xr-x   0 root         (0) root         (0)     7964 2023-06-20 01:53:21.000000 text2text-1.0.5/text2text/pytorch_pretrained_bert/file_utils.py
--rwxr-xr-x   0 root         (0) root         (0)     1821 2023-06-20 01:53:21.000000 text2text-1.0.5/text2text/pytorch_pretrained_bert/loss.py
--rwxr-xr-x   0 root         (0) root         (0)   108506 2023-06-20 01:53:21.000000 text2text-1.0.5/text2text/pytorch_pretrained_bert/modeling.py
--rwxr-xr-x   0 root         (0) root         (0)    15035 2023-06-20 01:53:21.000000 text2text-1.0.5/text2text/pytorch_pretrained_bert/tokenization.py
--rw-r--r--   0 root         (0) root         (0)     1782 2023-06-20 01:53:21.000000 text2text-1.0.5/text2text/questioner.py
--rw-r--r--   0 root         (0) root         (0)     2605 2023-06-20 03:20:23.000000 text2text-1.0.5/text2text/responder.py
--rw-r--r--   0 root         (0) root         (0)      984 2023-06-20 01:53:21.000000 text2text-1.0.5/text2text/searcher.py
--rw-r--r--   0 root         (0) root         (0)     1575 2023-06-20 01:53:21.000000 text2text-1.0.5/text2text/server.py
--rw-r--r--   0 root         (0) root         (0)     1103 2023-06-20 01:53:21.000000 text2text-1.0.5/text2text/summarizer.py
--rw-r--r--   0 root         (0) root         (0)     1766 2023-06-20 01:53:21.000000 text2text-1.0.5/text2text/tfidfer.py
--rw-r--r--   0 root         (0) root         (0)      780 2023-06-20 01:53:21.000000 text2text-1.0.5/text2text/tokenizer.py
--rw-r--r--   0 root         (0) root         (0)    12572 2023-06-20 02:51:51.000000 text2text-1.0.5/text2text/transformer.py
--rw-r--r--   0 root         (0) root         (0)     1489 2023-06-20 01:53:21.000000 text2text-1.0.5/text2text/translator.py
--rw-r--r--   0 root         (0) root         (0)      500 2023-06-20 01:53:21.000000 text2text-1.0.5/text2text/variator.py
--rw-r--r--   0 root         (0) root         (0)      816 2023-06-20 01:53:21.000000 text2text-1.0.5/text2text/vectorizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 03:42:18.386214 text2text-1.0.5/text2text.egg-info/
--rw-r--r--   0 root         (0) root         (0)    60233 2023-06-20 03:42:18.000000 text2text-1.0.5/text2text.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1064 2023-06-20 03:42:18.000000 text2text-1.0.5/text2text.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 03:42:18.000000 text2text-1.0.5/text2text.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      134 2023-06-20 03:42:18.000000 text2text-1.0.5/text2text.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-20 03:42:18.000000 text2text-1.0.5/text2text.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 03:56:54.010872 text2text-1.0.6/
+-rwxr-xr-x   0 root         (0) root         (0)     1418 2023-06-20 01:53:21.000000 text2text-1.0.6/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    60118 2023-06-20 03:56:54.010872 text2text-1.0.6/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)    59304 2023-06-20 03:55:26.000000 text2text-1.0.6/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-20 03:56:54.011872 text2text-1.0.6/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1246 2023-06-20 03:55:52.000000 text2text-1.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 03:56:54.006872 text2text-1.0.6/text2text/
+-rwxr-xr-x   0 root         (0) root         (0)      666 2023-06-20 02:25:27.000000 text2text-1.0.6/text2text/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7162 2023-06-20 01:53:21.000000 text2text-1.0.6/text2text/abstractor.py
+-rw-r--r--   0 root         (0) root         (0)     2157 2023-06-20 01:53:21.000000 text2text-1.0.6/text2text/answerer.py
+-rw-r--r--   0 root         (0) root         (0)     2287 2023-06-20 03:27:52.000000 text2text-1.0.6/text2text/assistant.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 03:56:54.008872 text2text-1.0.6/text2text/biunilm/
+-rwxr-xr-x   0 root         (0) root         (0)      110 2023-06-20 01:53:21.000000 text2text-1.0.6/text2text/biunilm/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    10937 2023-06-20 01:53:21.000000 text2text-1.0.6/text2text/biunilm/loader_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)    17726 2023-06-20 01:53:21.000000 text2text-1.0.6/text2text/biunilm/seq2seq_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-06-20 01:53:21.000000 text2text-1.0.6/text2text/bm25er.py
+-rw-r--r--   0 root         (0) root         (0)      519 2023-06-20 01:53:21.000000 text2text-1.0.6/text2text/counter.py
+-rw-r--r--   0 root         (0) root         (0)     1177 2023-06-20 01:53:21.000000 text2text-1.0.6/text2text/fitter.py
+-rw-r--r--   0 root         (0) root         (0)     1451 2023-06-20 01:53:21.000000 text2text-1.0.6/text2text/handler.py
+-rw-r--r--   0 root         (0) root         (0)     2106 2023-06-20 01:53:21.000000 text2text-1.0.6/text2text/identifier.py
+-rw-r--r--   0 root         (0) root         (0)     2010 2023-06-20 03:29:02.000000 text2text-1.0.6/text2text/indexer.py
+-rw-r--r--   0 root         (0) root         (0)     1165 2023-06-20 01:53:21.000000 text2text-1.0.6/text2text/measurer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 03:56:54.009872 text2text-1.0.6/text2text/pytorch_pretrained_bert/
+-rwxr-xr-x   0 root         (0) root         (0)      120 2023-06-20 01:53:21.000000 text2text-1.0.6/text2text/pytorch_pretrained_bert/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      932 2023-06-20 01:53:21.000000 text2text-1.0.6/text2text/pytorch_pretrained_bert/__main__.py
+-rwxr-xr-x   0 root         (0) root         (0)     7964 2023-06-20 01:53:21.000000 text2text-1.0.6/text2text/pytorch_pretrained_bert/file_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)     1821 2023-06-20 01:53:21.000000 text2text-1.0.6/text2text/pytorch_pretrained_bert/loss.py
+-rwxr-xr-x   0 root         (0) root         (0)   108506 2023-06-20 01:53:21.000000 text2text-1.0.6/text2text/pytorch_pretrained_bert/modeling.py
+-rwxr-xr-x   0 root         (0) root         (0)    15035 2023-06-20 01:53:21.000000 text2text-1.0.6/text2text/pytorch_pretrained_bert/tokenization.py
+-rw-r--r--   0 root         (0) root         (0)     1782 2023-06-20 01:53:21.000000 text2text-1.0.6/text2text/questioner.py
+-rw-r--r--   0 root         (0) root         (0)     2605 2023-06-20 03:20:23.000000 text2text-1.0.6/text2text/responder.py
+-rw-r--r--   0 root         (0) root         (0)      984 2023-06-20 01:53:21.000000 text2text-1.0.6/text2text/searcher.py
+-rw-r--r--   0 root         (0) root         (0)     1575 2023-06-20 01:53:21.000000 text2text-1.0.6/text2text/server.py
+-rw-r--r--   0 root         (0) root         (0)     1103 2023-06-20 01:53:21.000000 text2text-1.0.6/text2text/summarizer.py
+-rw-r--r--   0 root         (0) root         (0)     1766 2023-06-20 01:53:21.000000 text2text-1.0.6/text2text/tfidfer.py
+-rw-r--r--   0 root         (0) root         (0)      780 2023-06-20 01:53:21.000000 text2text-1.0.6/text2text/tokenizer.py
+-rw-r--r--   0 root         (0) root         (0)    12572 2023-06-20 02:51:51.000000 text2text-1.0.6/text2text/transformer.py
+-rw-r--r--   0 root         (0) root         (0)     1489 2023-06-20 01:53:21.000000 text2text-1.0.6/text2text/translator.py
+-rw-r--r--   0 root         (0) root         (0)      500 2023-06-20 01:53:21.000000 text2text-1.0.6/text2text/variator.py
+-rw-r--r--   0 root         (0) root         (0)      816 2023-06-20 01:53:21.000000 text2text-1.0.6/text2text/vectorizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 03:56:54.007872 text2text-1.0.6/text2text.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    60118 2023-06-20 03:56:53.000000 text2text-1.0.6/text2text.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1064 2023-06-20 03:56:53.000000 text2text-1.0.6/text2text.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 03:56:53.000000 text2text-1.0.6/text2text.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      134 2023-06-20 03:56:53.000000 text2text-1.0.6/text2text.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-20 03:56:53.000000 text2text-1.0.6/text2text.egg-info/top_level.txt
```

### Comparing `text2text-1.0.5/LICENSE.txt` & `text2text-1.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `text2text-1.0.5/PKG-INFO` & `text2text-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2text
-Version: 1.0.5
+Version: 1.0.6
 Summary: Text2Text: Crosslingual NLP/G toolkit
 Home-page: https://github.com/artitw/text2text
 Author: Artit Wangperawong
 Author-email: artitw@gmail.com
 Keywords: multilingual crosslingual gpt chatgpt bert natural language processing nlp nlg text generation gpt question answer answering information retrieval tfidf tf-idf bm25 search index summary summarizer summarization tokenizer tokenization translation backtranslation data augmentation science machine learning colab embedding levenshtein sub-word edit distance conversational dialog chatbot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -22,28 +22,27 @@
 * [Cross-Lingual Models](https://github.com/artitw/text2text#how-cross-lingual-nlp-models-work-click-to-watch)
 * [Installation Requirements](https://github.com/artitw/text2text#installation-requirements)
 * [Class Diagram](https://github.com/artitw/text2text#class-diagram)
 * [Quick Start Guide](https://github.com/artitw/text2text#api-quick-start-guide)
 * [Languages Available](https://github.com/artitw/text2text#languages-available)
 * [Requirements & Installation](https://github.com/artitw/text2text#requirements-and-installation)
 * [Examples](https://github.com/artitw/text2text#examples)
-  * [Sample Texts](https://github.com/artitw/text2text#sample-texts)
+  * [Assistant](https://github.com/artitw/text2text#assistant)
   * [Tokenization](https://github.com/artitw/text2text#tokenization)
   * [Embedding](https://github.com/artitw/text2text#embedding--vectorization)
   * [TF-IDF](https://github.com/artitw/text2text#tf-idf)
   * [BM25](https://github.com/artitw/text2text#bm25)
   * [Index](https://github.com/artitw/text2text#index)
   * [Search](https://github.com/artitw/text2text#search)
   * [Distance](https://github.com/artitw/text2text#levenshtein-sub-word-edit-distance)
   * [Translation](https://github.com/artitw/text2text#translation)
   * [Question Answering](https://github.com/artitw/text2text#question-answering)
   * [Question Generation](https://github.com/artitw/text2text#question-generation)
   * [Summarization](https://github.com/artitw/text2text#summarization)
   * [Data Augmentation](https://github.com/artitw/text2text#data-augmentation--back-translation)
-  * [Assistant](https://github.com/artitw/text2text#assistant)
   * [Dialog Responder](https://github.com/artitw/text2text#dialog-responder)
   * [Finetuning](https://github.com/artitw/text2text#training--finetuning)
   * [Identification](https://github.com/artitw/text2text#identification)
   * [Web Server](https://github.com/artitw/text2text#serving)
 * [Questions?](https://github.com/artitw/text2text#questions)
 * [Citation](https://github.com/artitw/text2text#citation)
 * [Contributing](https://github.com/artitw/text2text#contributing)
@@ -57,15 +56,15 @@
 ## How Crosslingual Models Work (click to watch)
 [![Crosslingual Models](http://img.youtube.com/vi/caZLVcJqsqo/0.jpg)](https://youtu.be/caZLVcJqsqo "Cross-Lingual Models")
 
 ## Installation Requirements 
 ```
 pip install -qq -U text2text
 ```
-* By default, all functionality in the demo and examples below work with less than 16 GB RAM, which means it runs on Colab.
+* All functionality in the demo and examples work with <16 GB RAM, which means they run on Colab.
   * See [Colab Demo](https://colab.research.google.com/drive/1LE_ifTpOGO5QJCKNQYtZe6c_tjbwnulR) and [Examples](#examples) below
 
 ## Class Diagram
 ```
       Indexer    Measurer   Counter -- Tfidfer
            \          \     /             \
         Searcher     Tokenizer           Bm25er
@@ -79,27 +78,27 @@
           Identifier
 ```
 
 ## Quick Start Guide
 Functionality | Invocation | Result
 :------------: | :-------------: | :-------------:
 Module Importing | `import text2text as t2t` | Libraries imported
-Language Model Setting | `t2t.Transformer.PRETRAINED_TRANSLATOR = "facebook/m2m100_418M"` | Default model
-Intialization | `h = t2t.Handler(["Hello, World!"], src_lang="en")` | Initialized handler with some text
+[Assistant](https://github.com/artitw/text2text#assistant) | `t2t.Handler(["Describe Text2Text in a few words: "]).assist()` | `['Text2Text is an AI-powered text generation tool that creates coherent and continuous text based on prompts.']`
+Language Model Setting | `t2t.Transformer.PRETRAINED_TRANSLATOR = "facebook/m2m100_418M"` | Change from default
+Text Handler | `h = t2t.Handler(["Hello, World!"], src_lang="en")` | Initialized handler with some text
 [Tokenization](https://github.com/artitw/text2text#tokenization) | `h.tokenize()` | `[['▁Hello', ',', '▁World', '!']]`
 [Embedding](https://github.com/artitw/text2text#embedding--vectorization) | `h.vectorize()` | `array([[0.18745188, 0.05658336, ..., 0.6332584 , 0.43805206]], dtype=float32)`
 [TF-IDF](https://github.com/artitw/text2text#tf-idf) | `h.tfidf()` | `[{'!': 0.5, ',': 0.5, '▁Hello': 0.5, '▁World': 0.5}]`
 [BM25](https://github.com/artitw/text2text#bm25) | `h.bm25()` | `[{'!': 0.3068528194400547, ',': 0.3068528194400547, '▁Hello': 0.3068528194400547, '▁World': 0.3068528194400547}]`
 [Indexer](https://github.com/artitw/text2text#index) | `i = h.index()` | Index object for similarity retrieval
 [Search](https://github.com/artitw/text2text#search) | `h.search(queries=["Hello"])` | `array([[0.09]])`
 [Translation](https://github.com/artitw/text2text#translation) | `h.translate(tgt_lang="zh")` | `['你好,世界!']`
 [Question Generation](https://github.com/artitw/text2text#question-generation) | `h.question()` | `[('What is the name of the world you are in?', 'The world')]`
 [Summarization](https://github.com/artitw/text2text#summarization) | `h.summarize()` | `["World ' s largest world"]`
 [Data Augmentation](https://github.com/artitw/text2text#data-augmentation--back-translation) | `h.variate()` | `['Hello the world!', 'Welcome to the world.', 'Hello to the world!',...`
-[Assistant](https://github.com/artitw/text2text#assistant) | `t2t.Handler(["Describe Text2Text in a few words: "]).assist()` | `['Text2Text is an AI-powered text generation tool that creates coherent and continuous text based on prompts.']`
 [Dialog Response](https://github.com/artitw/text2text#dialog-responder) | `t2t.Handler(["[CONTEXT] Hello EOS How are you?"]).respond()` | `['I am doing great. How are you?']`
 [Question Answering](https://github.com/artitw/text2text#question-answering) | `t2t.Handler(["Hello, World! [SEP] Hello, what?"]).answer()` | `['World']`
 [Distance](https://github.com/artitw/text2text#levenshtein-sub-word-edit-distance) | `t2t.Handler(["Hello, World! [SEP] Hello, what?"]).measure()` | `[2]`
 [Training/Finetuning](https://github.com/artitw/text2text#training--finetuning) | `t2t.Handler(["Hello, World! [TGT] Hello, what?"]).fit()` | Finetuned model saved
 [Identification](https://github.com/artitw/text2text#identification) | `t2t.Handler(["Aj keď sa Buzz Aldrin stal až „druhým človekom“..."]).identify()` | `['sk', 'Slovak']`
 [Web Server](https://github.com/artitw/text2text#serving) | `t2t.Server(host='0.0.0.0', port=80)` | Web server started on host and port
 
@@ -213,24 +212,25 @@
  'zh': 'Chinese',
  'zu': 'Zulu'}
 ```
 
 </details>
 
 ## Examples
-### Sample Texts
-```
-article_en = 'The Secretary-General of the United Nations says there is no military solution in Syria.'
-
-notre_dame_str = "As at most other universities, Notre Dame's students run a number of news media outlets. The nine student - run outlets include three newspapers, both a radio and television station, and several magazines and journals. Begun as a one - page journal in September 1876, the Scholastic magazine is issued twice monthly and claims to be the oldest continuous collegiate publication in the United States. The other magazine, The Juggler, is released twice a year and focuses on student literature and artwork. The Dome yearbook is published annually. The newspapers have varying publication interests, with The Observer published daily and mainly reporting university and other news, and staffed by students from both Notre Dame and Saint Mary's College. Unlike Scholastic and The Dome, The Observer is an independent publication and does not have a faculty advisor or any editorial oversight from the University. In 1987, when some students believed that The Observer began to show a conservative bias, a liberal newspaper, Common Sense was published. Likewise, in 2003, when other students believed that the paper showed a liberal bias, the conservative paper Irish Rover went into production. Neither paper is published as often as The Observer; however, all three are distributed to all students. Finally, in Spring 2008 an undergraduate journal for political science research, Beyond Politics, made its debut."
-
-bacteria_str = "Bacteria are a type of biological cell. They constitute a large domain of prokaryotic microorganisms. Typically a few micrometres in length, bacteria have a number of shapes, ranging from spheres to rods and spirals. Bacteria were among the first life forms to appear on Earth, and are present in most of its habitats."
-
-bio_str = "Biology is the science that studies life. What exactly is life? This may sound like a silly question with an obvious answer, but it is not easy to define life. For example, a branch of biology called virology studies viruses, which exhibit some of the characteristics of living entities but lack others. It turns out that although viruses can attack living organisms, cause diseases, and even reproduce, they do not meet the criteria that biologists use to define life."
 
+### Assistant
+Based on Vicuna 13B, which is based on LLaMA, which is not commercially licensed.
+Not ChatGPT level but it works well.
+To use a dynamic knowledge base, see [![Q&A Assistant Demo](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1hkNgpSmmUA-mzUibqz25xq-E8KYOLuVx?usp=sharing)
+```
+instructions = "Generate a JSON object that maps English characters as keys and Greek equivalents as values: {"
+res = t2t.Handler([instructions]).assist()
+#[
+#  '{\n"a": "α",\n"b": "β",\n"c": "γ",\n"d": "δ",\n"e": "ε",\n"f": "φ",\n"g": "χ",\n"h": "ι",\n"i": "η",\n"j": "κ",\n"k": "λ",\n"l": "μ",\n"m": "ν",\n"n": "ξ",\n"o": "ο",\n"p": "π",\n"q": "ρ",\n"r": "σ",\n"s": "τ",\n"t": "υ",\n"u": "ύ",\n"v": "φ",\n"w": "χ",\n"x": "ψ",\n"y": "ω",\n"z": "ζ"\n}'
+#]
 ```
 
 ### Tokenization
 ```
 t2t.Handler([
          "Let's go hiking tomorrow", 
          "안녕하세요.", 
@@ -367,14 +367,22 @@
 # Cosine similarity scores matrix
 array([[0.4472136 , 0.        , 0.        ],
        [0.        , 0.57735027, 0.        ]])
 ```
 
 #### Multiple queries on a single index
 ```
+article_en = 'The Secretary-General of the United Nations says there is no military solution in Syria.'
+
+notre_dame_str = "As at most other universities, Notre Dame's students run a number of news media outlets. The nine student - run outlets include three newspapers, both a radio and television station, and several magazines and journals. Begun as a one - page journal in September 1876, the Scholastic magazine is issued twice monthly and claims to be the oldest continuous collegiate publication in the United States. The other magazine, The Juggler, is released twice a year and focuses on student literature and artwork. The Dome yearbook is published annually. The newspapers have varying publication interests, with The Observer published daily and mainly reporting university and other news, and staffed by students from both Notre Dame and Saint Mary's College. Unlike Scholastic and The Dome, The Observer is an independent publication and does not have a faculty advisor or any editorial oversight from the University. In 1987, when some students believed that The Observer began to show a conservative bias, a liberal newspaper, Common Sense was published. Likewise, in 2003, when other students believed that the paper showed a liberal bias, the conservative paper Irish Rover went into production. Neither paper is published as often as The Observer; however, all three are distributed to all students. Finally, in Spring 2008 an undergraduate journal for political science research, Beyond Politics, made its debut."
+
+bacteria_str = "Bacteria are a type of biological cell. They constitute a large domain of prokaryotic microorganisms. Typically a few micrometres in length, bacteria have a number of shapes, ranging from spheres to rods and spirals. Bacteria were among the first life forms to appear on Earth, and are present in most of its habitats."
+
+bio_str = "Biology is the science that studies life. What exactly is life? This may sound like a silly question with an obvious answer, but it is not easy to define life. For example, a branch of biology called virology studies viruses, which exhibit some of the characteristics of living entities but lack others. It turns out that although viruses can attack living organisms, cause diseases, and even reproduce, they do not meet the criteria that biologists use to define life."
+
 bm25_index = t2t.Handler([
                        article_en, 
                        notre_dame_str, 
                        bacteria_str, 
                        bio_str
                        ]).bm25(output="matrix")
 
@@ -713,26 +721,14 @@
  'Bakteries are a type of biological cell. They were the best of prokaryotic microorganisms. They were one of the many micrometres, the bacteria are a lot of processes, from processes and processes. Bakteries are one of the processes of processes that are processed on Earth, and they are processed in all processes.',
  'Bacteria are a type of biocells, they make up a large area of probiotic microorganisms, usually several meters long bacteria have several shapes, from branches to roots and spirals, bacteria are one of the first forms of life that appear on Earth and are present in most of their habitats.',
  'The bacteria is a type of biological cells. The bacteria is a large area of prokaryotic microorganisms. The bacteria is a long micrometres, the bacteria is a spheres in roads and spirals. The bacteria is among the data, data, data, data and data.']
 ```
 
 </details>
 
-### Assistant
-Based on Vicuna 13B, which is based on LLaMA, which is not commercially licensed.
-Not ChatGPT level but it works well.
-To use a dynamic knowledge base, see [![Q&A Assistant Demo](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1hkNgpSmmUA-mzUibqz25xq-E8KYOLuVx?usp=sharing)
-```
-instructions = "Generate a JSON object that maps English characters as keys and Greek equivalents as values: {"
-res = t2t.Handler([instructions]).assist()
-#[
-#  '{\n"a": "α",\n"b": "β",\n"c": "γ",\n"d": "δ",\n"e": "ε",\n"f": "φ",\n"g": "χ",\n"h": "ι",\n"i": "η",\n"j": "κ",\n"k": "λ",\n"l": "μ",\n"m": "ν",\n"n": "ξ",\n"o": "ο",\n"p": "π",\n"q": "ρ",\n"r": "σ",\n"s": "τ",\n"t": "υ",\n"u": "ύ",\n"v": "φ",\n"w": "χ",\n"x": "ψ",\n"y": "ω",\n"z": "ζ"\n}'
-#]
-```
-
 ### Dialog Responder
 Respond to given instructions, knowledge base, and dialog context.
 To use a dynamic knowledge base, see [![Q&A Dialog Demo](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/19zaOzY-VU7pYkjCUlnxLzV-b51ZqASFq?usp=sharing)
 ```
 instruction = ''
 knowledge = 'Domestic cats are valued by humans for companionship and their ability to kill rodents. About 60 cat breeds are recognized by various cat registries.'
 dialog = [
```

### Comparing `text2text-1.0.5/README.md` & `text2text-1.0.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -8,28 +8,27 @@
 * [Cross-Lingual Models](https://github.com/artitw/text2text#how-cross-lingual-nlp-models-work-click-to-watch)
 * [Installation Requirements](https://github.com/artitw/text2text#installation-requirements)
 * [Class Diagram](https://github.com/artitw/text2text#class-diagram)
 * [Quick Start Guide](https://github.com/artitw/text2text#api-quick-start-guide)
 * [Languages Available](https://github.com/artitw/text2text#languages-available)
 * [Requirements & Installation](https://github.com/artitw/text2text#requirements-and-installation)
 * [Examples](https://github.com/artitw/text2text#examples)
-  * [Sample Texts](https://github.com/artitw/text2text#sample-texts)
+  * [Assistant](https://github.com/artitw/text2text#assistant)
   * [Tokenization](https://github.com/artitw/text2text#tokenization)
   * [Embedding](https://github.com/artitw/text2text#embedding--vectorization)
   * [TF-IDF](https://github.com/artitw/text2text#tf-idf)
   * [BM25](https://github.com/artitw/text2text#bm25)
   * [Index](https://github.com/artitw/text2text#index)
   * [Search](https://github.com/artitw/text2text#search)
   * [Distance](https://github.com/artitw/text2text#levenshtein-sub-word-edit-distance)
   * [Translation](https://github.com/artitw/text2text#translation)
   * [Question Answering](https://github.com/artitw/text2text#question-answering)
   * [Question Generation](https://github.com/artitw/text2text#question-generation)
   * [Summarization](https://github.com/artitw/text2text#summarization)
   * [Data Augmentation](https://github.com/artitw/text2text#data-augmentation--back-translation)
-  * [Assistant](https://github.com/artitw/text2text#assistant)
   * [Dialog Responder](https://github.com/artitw/text2text#dialog-responder)
   * [Finetuning](https://github.com/artitw/text2text#training--finetuning)
   * [Identification](https://github.com/artitw/text2text#identification)
   * [Web Server](https://github.com/artitw/text2text#serving)
 * [Questions?](https://github.com/artitw/text2text#questions)
 * [Citation](https://github.com/artitw/text2text#citation)
 * [Contributing](https://github.com/artitw/text2text#contributing)
@@ -43,15 +42,15 @@
 ## How Crosslingual Models Work (click to watch)
 [![Crosslingual Models](http://img.youtube.com/vi/caZLVcJqsqo/0.jpg)](https://youtu.be/caZLVcJqsqo "Cross-Lingual Models")
 
 ## Installation Requirements 
 ```
 pip install -qq -U text2text
 ```
-* By default, all functionality in the demo and examples below work with less than 16 GB RAM, which means it runs on Colab.
+* All functionality in the demo and examples work with <16 GB RAM, which means they run on Colab.
   * See [Colab Demo](https://colab.research.google.com/drive/1LE_ifTpOGO5QJCKNQYtZe6c_tjbwnulR) and [Examples](#examples) below
 
 ## Class Diagram
 ```
       Indexer    Measurer   Counter -- Tfidfer
            \          \     /             \
         Searcher     Tokenizer           Bm25er
@@ -65,27 +64,27 @@
           Identifier
 ```
 
 ## Quick Start Guide
 Functionality | Invocation | Result
 :------------: | :-------------: | :-------------:
 Module Importing | `import text2text as t2t` | Libraries imported
-Language Model Setting | `t2t.Transformer.PRETRAINED_TRANSLATOR = "facebook/m2m100_418M"` | Default model
-Intialization | `h = t2t.Handler(["Hello, World!"], src_lang="en")` | Initialized handler with some text
+[Assistant](https://github.com/artitw/text2text#assistant) | `t2t.Handler(["Describe Text2Text in a few words: "]).assist()` | `['Text2Text is an AI-powered text generation tool that creates coherent and continuous text based on prompts.']`
+Language Model Setting | `t2t.Transformer.PRETRAINED_TRANSLATOR = "facebook/m2m100_418M"` | Change from default
+Text Handler | `h = t2t.Handler(["Hello, World!"], src_lang="en")` | Initialized handler with some text
 [Tokenization](https://github.com/artitw/text2text#tokenization) | `h.tokenize()` | `[['▁Hello', ',', '▁World', '!']]`
 [Embedding](https://github.com/artitw/text2text#embedding--vectorization) | `h.vectorize()` | `array([[0.18745188, 0.05658336, ..., 0.6332584 , 0.43805206]], dtype=float32)`
 [TF-IDF](https://github.com/artitw/text2text#tf-idf) | `h.tfidf()` | `[{'!': 0.5, ',': 0.5, '▁Hello': 0.5, '▁World': 0.5}]`
 [BM25](https://github.com/artitw/text2text#bm25) | `h.bm25()` | `[{'!': 0.3068528194400547, ',': 0.3068528194400547, '▁Hello': 0.3068528194400547, '▁World': 0.3068528194400547}]`
 [Indexer](https://github.com/artitw/text2text#index) | `i = h.index()` | Index object for similarity retrieval
 [Search](https://github.com/artitw/text2text#search) | `h.search(queries=["Hello"])` | `array([[0.09]])`
 [Translation](https://github.com/artitw/text2text#translation) | `h.translate(tgt_lang="zh")` | `['你好,世界!']`
 [Question Generation](https://github.com/artitw/text2text#question-generation) | `h.question()` | `[('What is the name of the world you are in?', 'The world')]`
 [Summarization](https://github.com/artitw/text2text#summarization) | `h.summarize()` | `["World ' s largest world"]`
 [Data Augmentation](https://github.com/artitw/text2text#data-augmentation--back-translation) | `h.variate()` | `['Hello the world!', 'Welcome to the world.', 'Hello to the world!',...`
-[Assistant](https://github.com/artitw/text2text#assistant) | `t2t.Handler(["Describe Text2Text in a few words: "]).assist()` | `['Text2Text is an AI-powered text generation tool that creates coherent and continuous text based on prompts.']`
 [Dialog Response](https://github.com/artitw/text2text#dialog-responder) | `t2t.Handler(["[CONTEXT] Hello EOS How are you?"]).respond()` | `['I am doing great. How are you?']`
 [Question Answering](https://github.com/artitw/text2text#question-answering) | `t2t.Handler(["Hello, World! [SEP] Hello, what?"]).answer()` | `['World']`
 [Distance](https://github.com/artitw/text2text#levenshtein-sub-word-edit-distance) | `t2t.Handler(["Hello, World! [SEP] Hello, what?"]).measure()` | `[2]`
 [Training/Finetuning](https://github.com/artitw/text2text#training--finetuning) | `t2t.Handler(["Hello, World! [TGT] Hello, what?"]).fit()` | Finetuned model saved
 [Identification](https://github.com/artitw/text2text#identification) | `t2t.Handler(["Aj keď sa Buzz Aldrin stal až „druhým človekom“..."]).identify()` | `['sk', 'Slovak']`
 [Web Server](https://github.com/artitw/text2text#serving) | `t2t.Server(host='0.0.0.0', port=80)` | Web server started on host and port
 
@@ -199,24 +198,25 @@
  'zh': 'Chinese',
  'zu': 'Zulu'}
 ```
 
 </details>
 
 ## Examples
-### Sample Texts
-```
-article_en = 'The Secretary-General of the United Nations says there is no military solution in Syria.'
-
-notre_dame_str = "As at most other universities, Notre Dame's students run a number of news media outlets. The nine student - run outlets include three newspapers, both a radio and television station, and several magazines and journals. Begun as a one - page journal in September 1876, the Scholastic magazine is issued twice monthly and claims to be the oldest continuous collegiate publication in the United States. The other magazine, The Juggler, is released twice a year and focuses on student literature and artwork. The Dome yearbook is published annually. The newspapers have varying publication interests, with The Observer published daily and mainly reporting university and other news, and staffed by students from both Notre Dame and Saint Mary's College. Unlike Scholastic and The Dome, The Observer is an independent publication and does not have a faculty advisor or any editorial oversight from the University. In 1987, when some students believed that The Observer began to show a conservative bias, a liberal newspaper, Common Sense was published. Likewise, in 2003, when other students believed that the paper showed a liberal bias, the conservative paper Irish Rover went into production. Neither paper is published as often as The Observer; however, all three are distributed to all students. Finally, in Spring 2008 an undergraduate journal for political science research, Beyond Politics, made its debut."
-
-bacteria_str = "Bacteria are a type of biological cell. They constitute a large domain of prokaryotic microorganisms. Typically a few micrometres in length, bacteria have a number of shapes, ranging from spheres to rods and spirals. Bacteria were among the first life forms to appear on Earth, and are present in most of its habitats."
-
-bio_str = "Biology is the science that studies life. What exactly is life? This may sound like a silly question with an obvious answer, but it is not easy to define life. For example, a branch of biology called virology studies viruses, which exhibit some of the characteristics of living entities but lack others. It turns out that although viruses can attack living organisms, cause diseases, and even reproduce, they do not meet the criteria that biologists use to define life."
 
+### Assistant
+Based on Vicuna 13B, which is based on LLaMA, which is not commercially licensed.
+Not ChatGPT level but it works well.
+To use a dynamic knowledge base, see [![Q&A Assistant Demo](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1hkNgpSmmUA-mzUibqz25xq-E8KYOLuVx?usp=sharing)
+```
+instructions = "Generate a JSON object that maps English characters as keys and Greek equivalents as values: {"
+res = t2t.Handler([instructions]).assist()
+#[
+#  '{\n"a": "α",\n"b": "β",\n"c": "γ",\n"d": "δ",\n"e": "ε",\n"f": "φ",\n"g": "χ",\n"h": "ι",\n"i": "η",\n"j": "κ",\n"k": "λ",\n"l": "μ",\n"m": "ν",\n"n": "ξ",\n"o": "ο",\n"p": "π",\n"q": "ρ",\n"r": "σ",\n"s": "τ",\n"t": "υ",\n"u": "ύ",\n"v": "φ",\n"w": "χ",\n"x": "ψ",\n"y": "ω",\n"z": "ζ"\n}'
+#]
 ```
 
 ### Tokenization
 ```
 t2t.Handler([
          "Let's go hiking tomorrow", 
          "안녕하세요.", 
@@ -353,14 +353,22 @@
 # Cosine similarity scores matrix
 array([[0.4472136 , 0.        , 0.        ],
        [0.        , 0.57735027, 0.        ]])
 ```
 
 #### Multiple queries on a single index
 ```
+article_en = 'The Secretary-General of the United Nations says there is no military solution in Syria.'
+
+notre_dame_str = "As at most other universities, Notre Dame's students run a number of news media outlets. The nine student - run outlets include three newspapers, both a radio and television station, and several magazines and journals. Begun as a one - page journal in September 1876, the Scholastic magazine is issued twice monthly and claims to be the oldest continuous collegiate publication in the United States. The other magazine, The Juggler, is released twice a year and focuses on student literature and artwork. The Dome yearbook is published annually. The newspapers have varying publication interests, with The Observer published daily and mainly reporting university and other news, and staffed by students from both Notre Dame and Saint Mary's College. Unlike Scholastic and The Dome, The Observer is an independent publication and does not have a faculty advisor or any editorial oversight from the University. In 1987, when some students believed that The Observer began to show a conservative bias, a liberal newspaper, Common Sense was published. Likewise, in 2003, when other students believed that the paper showed a liberal bias, the conservative paper Irish Rover went into production. Neither paper is published as often as The Observer; however, all three are distributed to all students. Finally, in Spring 2008 an undergraduate journal for political science research, Beyond Politics, made its debut."
+
+bacteria_str = "Bacteria are a type of biological cell. They constitute a large domain of prokaryotic microorganisms. Typically a few micrometres in length, bacteria have a number of shapes, ranging from spheres to rods and spirals. Bacteria were among the first life forms to appear on Earth, and are present in most of its habitats."
+
+bio_str = "Biology is the science that studies life. What exactly is life? This may sound like a silly question with an obvious answer, but it is not easy to define life. For example, a branch of biology called virology studies viruses, which exhibit some of the characteristics of living entities but lack others. It turns out that although viruses can attack living organisms, cause diseases, and even reproduce, they do not meet the criteria that biologists use to define life."
+
 bm25_index = t2t.Handler([
                        article_en, 
                        notre_dame_str, 
                        bacteria_str, 
                        bio_str
                        ]).bm25(output="matrix")
 
@@ -699,26 +707,14 @@
  'Bakteries are a type of biological cell. They were the best of prokaryotic microorganisms. They were one of the many micrometres, the bacteria are a lot of processes, from processes and processes. Bakteries are one of the processes of processes that are processed on Earth, and they are processed in all processes.',
  'Bacteria are a type of biocells, they make up a large area of probiotic microorganisms, usually several meters long bacteria have several shapes, from branches to roots and spirals, bacteria are one of the first forms of life that appear on Earth and are present in most of their habitats.',
  'The bacteria is a type of biological cells. The bacteria is a large area of prokaryotic microorganisms. The bacteria is a long micrometres, the bacteria is a spheres in roads and spirals. The bacteria is among the data, data, data, data and data.']
 ```
 
 </details>
 
-### Assistant
-Based on Vicuna 13B, which is based on LLaMA, which is not commercially licensed.
-Not ChatGPT level but it works well.
-To use a dynamic knowledge base, see [![Q&A Assistant Demo](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1hkNgpSmmUA-mzUibqz25xq-E8KYOLuVx?usp=sharing)
-```
-instructions = "Generate a JSON object that maps English characters as keys and Greek equivalents as values: {"
-res = t2t.Handler([instructions]).assist()
-#[
-#  '{\n"a": "α",\n"b": "β",\n"c": "γ",\n"d": "δ",\n"e": "ε",\n"f": "φ",\n"g": "χ",\n"h": "ι",\n"i": "η",\n"j": "κ",\n"k": "λ",\n"l": "μ",\n"m": "ν",\n"n": "ξ",\n"o": "ο",\n"p": "π",\n"q": "ρ",\n"r": "σ",\n"s": "τ",\n"t": "υ",\n"u": "ύ",\n"v": "φ",\n"w": "χ",\n"x": "ψ",\n"y": "ω",\n"z": "ζ"\n}'
-#]
-```
-
 ### Dialog Responder
 Respond to given instructions, knowledge base, and dialog context.
 To use a dynamic knowledge base, see [![Q&A Dialog Demo](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/19zaOzY-VU7pYkjCUlnxLzV-b51ZqASFq?usp=sharing)
 ```
 instruction = ''
 knowledge = 'Domestic cats are valued by humans for companionship and their ability to kill rodents. About 60 cat breeds are recognized by various cat registries.'
 dialog = [
```

### Comparing `text2text-1.0.5/setup.py` & `text2text-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="text2text",
-  version="1.0.5",
+  version="1.0.6",
   author="Artit Wangperawong",
   author_email="artitw@gmail.com",
   description="Text2Text: Crosslingual NLP/G toolkit",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/artitw/text2text",
   packages=setuptools.find_packages(),
```

### Comparing `text2text-1.0.5/text2text/__init__.py` & `text2text-1.0.6/text2text/__init__.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.5/text2text/abstractor.py` & `text2text-1.0.6/text2text/abstractor.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.5/text2text/answerer.py` & `text2text-1.0.6/text2text/answerer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.5/text2text/assistant.py` & `text2text-1.0.6/text2text/assistant.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.5/text2text/biunilm/loader_utils.py` & `text2text-1.0.6/text2text/biunilm/loader_utils.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.5/text2text/biunilm/seq2seq_loader.py` & `text2text-1.0.6/text2text/biunilm/seq2seq_loader.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.5/text2text/bm25er.py` & `text2text-1.0.6/text2text/bm25er.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.5/text2text/counter.py` & `text2text-1.0.6/text2text/counter.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.5/text2text/fitter.py` & `text2text-1.0.6/text2text/fitter.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.5/text2text/handler.py` & `text2text-1.0.6/text2text/handler.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.5/text2text/identifier.py` & `text2text-1.0.6/text2text/identifier.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.5/text2text/indexer.py` & `text2text-1.0.6/text2text/indexer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.5/text2text/measurer.py` & `text2text-1.0.6/text2text/measurer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.5/text2text/pytorch_pretrained_bert/__main__.py` & `text2text-1.0.6/text2text/pytorch_pretrained_bert/__main__.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.5/text2text/pytorch_pretrained_bert/file_utils.py` & `text2text-1.0.6/text2text/pytorch_pretrained_bert/file_utils.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.5/text2text/pytorch_pretrained_bert/loss.py` & `text2text-1.0.6/text2text/pytorch_pretrained_bert/loss.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.5/text2text/pytorch_pretrained_bert/modeling.py` & `text2text-1.0.6/text2text/pytorch_pretrained_bert/modeling.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.5/text2text/pytorch_pretrained_bert/tokenization.py` & `text2text-1.0.6/text2text/pytorch_pretrained_bert/tokenization.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.5/text2text/questioner.py` & `text2text-1.0.6/text2text/questioner.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.5/text2text/responder.py` & `text2text-1.0.6/text2text/responder.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.5/text2text/searcher.py` & `text2text-1.0.6/text2text/searcher.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.5/text2text/server.py` & `text2text-1.0.6/text2text/server.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.5/text2text/summarizer.py` & `text2text-1.0.6/text2text/summarizer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.5/text2text/tfidfer.py` & `text2text-1.0.6/text2text/tfidfer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.5/text2text/tokenizer.py` & `text2text-1.0.6/text2text/tokenizer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.5/text2text/transformer.py` & `text2text-1.0.6/text2text/transformer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.5/text2text/translator.py` & `text2text-1.0.6/text2text/translator.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.5/text2text/vectorizer.py` & `text2text-1.0.6/text2text/vectorizer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.5/text2text.egg-info/PKG-INFO` & `text2text-1.0.6/text2text.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2text
-Version: 1.0.5
+Version: 1.0.6
 Summary: Text2Text: Crosslingual NLP/G toolkit
 Home-page: https://github.com/artitw/text2text
 Author: Artit Wangperawong
 Author-email: artitw@gmail.com
 Keywords: multilingual crosslingual gpt chatgpt bert natural language processing nlp nlg text generation gpt question answer answering information retrieval tfidf tf-idf bm25 search index summary summarizer summarization tokenizer tokenization translation backtranslation data augmentation science machine learning colab embedding levenshtein sub-word edit distance conversational dialog chatbot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -22,28 +22,27 @@
 * [Cross-Lingual Models](https://github.com/artitw/text2text#how-cross-lingual-nlp-models-work-click-to-watch)
 * [Installation Requirements](https://github.com/artitw/text2text#installation-requirements)
 * [Class Diagram](https://github.com/artitw/text2text#class-diagram)
 * [Quick Start Guide](https://github.com/artitw/text2text#api-quick-start-guide)
 * [Languages Available](https://github.com/artitw/text2text#languages-available)
 * [Requirements & Installation](https://github.com/artitw/text2text#requirements-and-installation)
 * [Examples](https://github.com/artitw/text2text#examples)
-  * [Sample Texts](https://github.com/artitw/text2text#sample-texts)
+  * [Assistant](https://github.com/artitw/text2text#assistant)
   * [Tokenization](https://github.com/artitw/text2text#tokenization)
   * [Embedding](https://github.com/artitw/text2text#embedding--vectorization)
   * [TF-IDF](https://github.com/artitw/text2text#tf-idf)
   * [BM25](https://github.com/artitw/text2text#bm25)
   * [Index](https://github.com/artitw/text2text#index)
   * [Search](https://github.com/artitw/text2text#search)
   * [Distance](https://github.com/artitw/text2text#levenshtein-sub-word-edit-distance)
   * [Translation](https://github.com/artitw/text2text#translation)
   * [Question Answering](https://github.com/artitw/text2text#question-answering)
   * [Question Generation](https://github.com/artitw/text2text#question-generation)
   * [Summarization](https://github.com/artitw/text2text#summarization)
   * [Data Augmentation](https://github.com/artitw/text2text#data-augmentation--back-translation)
-  * [Assistant](https://github.com/artitw/text2text#assistant)
   * [Dialog Responder](https://github.com/artitw/text2text#dialog-responder)
   * [Finetuning](https://github.com/artitw/text2text#training--finetuning)
   * [Identification](https://github.com/artitw/text2text#identification)
   * [Web Server](https://github.com/artitw/text2text#serving)
 * [Questions?](https://github.com/artitw/text2text#questions)
 * [Citation](https://github.com/artitw/text2text#citation)
 * [Contributing](https://github.com/artitw/text2text#contributing)
@@ -57,15 +56,15 @@
 ## How Crosslingual Models Work (click to watch)
 [![Crosslingual Models](http://img.youtube.com/vi/caZLVcJqsqo/0.jpg)](https://youtu.be/caZLVcJqsqo "Cross-Lingual Models")
 
 ## Installation Requirements 
 ```
 pip install -qq -U text2text
 ```
-* By default, all functionality in the demo and examples below work with less than 16 GB RAM, which means it runs on Colab.
+* All functionality in the demo and examples work with <16 GB RAM, which means they run on Colab.
   * See [Colab Demo](https://colab.research.google.com/drive/1LE_ifTpOGO5QJCKNQYtZe6c_tjbwnulR) and [Examples](#examples) below
 
 ## Class Diagram
 ```
       Indexer    Measurer   Counter -- Tfidfer
            \          \     /             \
         Searcher     Tokenizer           Bm25er
@@ -79,27 +78,27 @@
           Identifier
 ```
 
 ## Quick Start Guide
 Functionality | Invocation | Result
 :------------: | :-------------: | :-------------:
 Module Importing | `import text2text as t2t` | Libraries imported
-Language Model Setting | `t2t.Transformer.PRETRAINED_TRANSLATOR = "facebook/m2m100_418M"` | Default model
-Intialization | `h = t2t.Handler(["Hello, World!"], src_lang="en")` | Initialized handler with some text
+[Assistant](https://github.com/artitw/text2text#assistant) | `t2t.Handler(["Describe Text2Text in a few words: "]).assist()` | `['Text2Text is an AI-powered text generation tool that creates coherent and continuous text based on prompts.']`
+Language Model Setting | `t2t.Transformer.PRETRAINED_TRANSLATOR = "facebook/m2m100_418M"` | Change from default
+Text Handler | `h = t2t.Handler(["Hello, World!"], src_lang="en")` | Initialized handler with some text
 [Tokenization](https://github.com/artitw/text2text#tokenization) | `h.tokenize()` | `[['▁Hello', ',', '▁World', '!']]`
 [Embedding](https://github.com/artitw/text2text#embedding--vectorization) | `h.vectorize()` | `array([[0.18745188, 0.05658336, ..., 0.6332584 , 0.43805206]], dtype=float32)`
 [TF-IDF](https://github.com/artitw/text2text#tf-idf) | `h.tfidf()` | `[{'!': 0.5, ',': 0.5, '▁Hello': 0.5, '▁World': 0.5}]`
 [BM25](https://github.com/artitw/text2text#bm25) | `h.bm25()` | `[{'!': 0.3068528194400547, ',': 0.3068528194400547, '▁Hello': 0.3068528194400547, '▁World': 0.3068528194400547}]`
 [Indexer](https://github.com/artitw/text2text#index) | `i = h.index()` | Index object for similarity retrieval
 [Search](https://github.com/artitw/text2text#search) | `h.search(queries=["Hello"])` | `array([[0.09]])`
 [Translation](https://github.com/artitw/text2text#translation) | `h.translate(tgt_lang="zh")` | `['你好,世界!']`
 [Question Generation](https://github.com/artitw/text2text#question-generation) | `h.question()` | `[('What is the name of the world you are in?', 'The world')]`
 [Summarization](https://github.com/artitw/text2text#summarization) | `h.summarize()` | `["World ' s largest world"]`
 [Data Augmentation](https://github.com/artitw/text2text#data-augmentation--back-translation) | `h.variate()` | `['Hello the world!', 'Welcome to the world.', 'Hello to the world!',...`
-[Assistant](https://github.com/artitw/text2text#assistant) | `t2t.Handler(["Describe Text2Text in a few words: "]).assist()` | `['Text2Text is an AI-powered text generation tool that creates coherent and continuous text based on prompts.']`
 [Dialog Response](https://github.com/artitw/text2text#dialog-responder) | `t2t.Handler(["[CONTEXT] Hello EOS How are you?"]).respond()` | `['I am doing great. How are you?']`
 [Question Answering](https://github.com/artitw/text2text#question-answering) | `t2t.Handler(["Hello, World! [SEP] Hello, what?"]).answer()` | `['World']`
 [Distance](https://github.com/artitw/text2text#levenshtein-sub-word-edit-distance) | `t2t.Handler(["Hello, World! [SEP] Hello, what?"]).measure()` | `[2]`
 [Training/Finetuning](https://github.com/artitw/text2text#training--finetuning) | `t2t.Handler(["Hello, World! [TGT] Hello, what?"]).fit()` | Finetuned model saved
 [Identification](https://github.com/artitw/text2text#identification) | `t2t.Handler(["Aj keď sa Buzz Aldrin stal až „druhým človekom“..."]).identify()` | `['sk', 'Slovak']`
 [Web Server](https://github.com/artitw/text2text#serving) | `t2t.Server(host='0.0.0.0', port=80)` | Web server started on host and port
 
@@ -213,24 +212,25 @@
  'zh': 'Chinese',
  'zu': 'Zulu'}
 ```
 
 </details>
 
 ## Examples
-### Sample Texts
-```
-article_en = 'The Secretary-General of the United Nations says there is no military solution in Syria.'
-
-notre_dame_str = "As at most other universities, Notre Dame's students run a number of news media outlets. The nine student - run outlets include three newspapers, both a radio and television station, and several magazines and journals. Begun as a one - page journal in September 1876, the Scholastic magazine is issued twice monthly and claims to be the oldest continuous collegiate publication in the United States. The other magazine, The Juggler, is released twice a year and focuses on student literature and artwork. The Dome yearbook is published annually. The newspapers have varying publication interests, with The Observer published daily and mainly reporting university and other news, and staffed by students from both Notre Dame and Saint Mary's College. Unlike Scholastic and The Dome, The Observer is an independent publication and does not have a faculty advisor or any editorial oversight from the University. In 1987, when some students believed that The Observer began to show a conservative bias, a liberal newspaper, Common Sense was published. Likewise, in 2003, when other students believed that the paper showed a liberal bias, the conservative paper Irish Rover went into production. Neither paper is published as often as The Observer; however, all three are distributed to all students. Finally, in Spring 2008 an undergraduate journal for political science research, Beyond Politics, made its debut."
-
-bacteria_str = "Bacteria are a type of biological cell. They constitute a large domain of prokaryotic microorganisms. Typically a few micrometres in length, bacteria have a number of shapes, ranging from spheres to rods and spirals. Bacteria were among the first life forms to appear on Earth, and are present in most of its habitats."
-
-bio_str = "Biology is the science that studies life. What exactly is life? This may sound like a silly question with an obvious answer, but it is not easy to define life. For example, a branch of biology called virology studies viruses, which exhibit some of the characteristics of living entities but lack others. It turns out that although viruses can attack living organisms, cause diseases, and even reproduce, they do not meet the criteria that biologists use to define life."
 
+### Assistant
+Based on Vicuna 13B, which is based on LLaMA, which is not commercially licensed.
+Not ChatGPT level but it works well.
+To use a dynamic knowledge base, see [![Q&A Assistant Demo](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1hkNgpSmmUA-mzUibqz25xq-E8KYOLuVx?usp=sharing)
+```
+instructions = "Generate a JSON object that maps English characters as keys and Greek equivalents as values: {"
+res = t2t.Handler([instructions]).assist()
+#[
+#  '{\n"a": "α",\n"b": "β",\n"c": "γ",\n"d": "δ",\n"e": "ε",\n"f": "φ",\n"g": "χ",\n"h": "ι",\n"i": "η",\n"j": "κ",\n"k": "λ",\n"l": "μ",\n"m": "ν",\n"n": "ξ",\n"o": "ο",\n"p": "π",\n"q": "ρ",\n"r": "σ",\n"s": "τ",\n"t": "υ",\n"u": "ύ",\n"v": "φ",\n"w": "χ",\n"x": "ψ",\n"y": "ω",\n"z": "ζ"\n}'
+#]
 ```
 
 ### Tokenization
 ```
 t2t.Handler([
          "Let's go hiking tomorrow", 
          "안녕하세요.", 
@@ -367,14 +367,22 @@
 # Cosine similarity scores matrix
 array([[0.4472136 , 0.        , 0.        ],
        [0.        , 0.57735027, 0.        ]])
 ```
 
 #### Multiple queries on a single index
 ```
+article_en = 'The Secretary-General of the United Nations says there is no military solution in Syria.'
+
+notre_dame_str = "As at most other universities, Notre Dame's students run a number of news media outlets. The nine student - run outlets include three newspapers, both a radio and television station, and several magazines and journals. Begun as a one - page journal in September 1876, the Scholastic magazine is issued twice monthly and claims to be the oldest continuous collegiate publication in the United States. The other magazine, The Juggler, is released twice a year and focuses on student literature and artwork. The Dome yearbook is published annually. The newspapers have varying publication interests, with The Observer published daily and mainly reporting university and other news, and staffed by students from both Notre Dame and Saint Mary's College. Unlike Scholastic and The Dome, The Observer is an independent publication and does not have a faculty advisor or any editorial oversight from the University. In 1987, when some students believed that The Observer began to show a conservative bias, a liberal newspaper, Common Sense was published. Likewise, in 2003, when other students believed that the paper showed a liberal bias, the conservative paper Irish Rover went into production. Neither paper is published as often as The Observer; however, all three are distributed to all students. Finally, in Spring 2008 an undergraduate journal for political science research, Beyond Politics, made its debut."
+
+bacteria_str = "Bacteria are a type of biological cell. They constitute a large domain of prokaryotic microorganisms. Typically a few micrometres in length, bacteria have a number of shapes, ranging from spheres to rods and spirals. Bacteria were among the first life forms to appear on Earth, and are present in most of its habitats."
+
+bio_str = "Biology is the science that studies life. What exactly is life? This may sound like a silly question with an obvious answer, but it is not easy to define life. For example, a branch of biology called virology studies viruses, which exhibit some of the characteristics of living entities but lack others. It turns out that although viruses can attack living organisms, cause diseases, and even reproduce, they do not meet the criteria that biologists use to define life."
+
 bm25_index = t2t.Handler([
                        article_en, 
                        notre_dame_str, 
                        bacteria_str, 
                        bio_str
                        ]).bm25(output="matrix")
 
@@ -713,26 +721,14 @@
  'Bakteries are a type of biological cell. They were the best of prokaryotic microorganisms. They were one of the many micrometres, the bacteria are a lot of processes, from processes and processes. Bakteries are one of the processes of processes that are processed on Earth, and they are processed in all processes.',
  'Bacteria are a type of biocells, they make up a large area of probiotic microorganisms, usually several meters long bacteria have several shapes, from branches to roots and spirals, bacteria are one of the first forms of life that appear on Earth and are present in most of their habitats.',
  'The bacteria is a type of biological cells. The bacteria is a large area of prokaryotic microorganisms. The bacteria is a long micrometres, the bacteria is a spheres in roads and spirals. The bacteria is among the data, data, data, data and data.']
 ```
 
 </details>
 
-### Assistant
-Based on Vicuna 13B, which is based on LLaMA, which is not commercially licensed.
-Not ChatGPT level but it works well.
-To use a dynamic knowledge base, see [![Q&A Assistant Demo](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1hkNgpSmmUA-mzUibqz25xq-E8KYOLuVx?usp=sharing)
-```
-instructions = "Generate a JSON object that maps English characters as keys and Greek equivalents as values: {"
-res = t2t.Handler([instructions]).assist()
-#[
-#  '{\n"a": "α",\n"b": "β",\n"c": "γ",\n"d": "δ",\n"e": "ε",\n"f": "φ",\n"g": "χ",\n"h": "ι",\n"i": "η",\n"j": "κ",\n"k": "λ",\n"l": "μ",\n"m": "ν",\n"n": "ξ",\n"o": "ο",\n"p": "π",\n"q": "ρ",\n"r": "σ",\n"s": "τ",\n"t": "υ",\n"u": "ύ",\n"v": "φ",\n"w": "χ",\n"x": "ψ",\n"y": "ω",\n"z": "ζ"\n}'
-#]
-```
-
 ### Dialog Responder
 Respond to given instructions, knowledge base, and dialog context.
 To use a dynamic knowledge base, see [![Q&A Dialog Demo](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/19zaOzY-VU7pYkjCUlnxLzV-b51ZqASFq?usp=sharing)
 ```
 instruction = ''
 knowledge = 'Domestic cats are valued by humans for companionship and their ability to kill rodents. About 60 cat breeds are recognized by various cat registries.'
 dialog = [
```

### Comparing `text2text-1.0.5/text2text.egg-info/SOURCES.txt` & `text2text-1.0.6/text2text.egg-info/SOURCES.txt`

 * *Files identical despite different names*

