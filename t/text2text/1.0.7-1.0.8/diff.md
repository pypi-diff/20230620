# Comparing `tmp/text2text-1.0.7.tar.gz` & `tmp/text2text-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text2text-1.0.7.tar", last modified: Tue Jun 20 04:09:37 2023, max compression
+gzip compressed data, was "text2text-1.0.8.tar", last modified: Tue Jun 20 04:13:49 2023, max compression
```

## Comparing `text2text-1.0.7.tar` & `text2text-1.0.8.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 04:09:37.093993 text2text-1.0.7/
--rwxr-xr-x   0 root         (0) root         (0)     1418 2023-06-20 01:53:21.000000 text2text-1.0.7/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    60454 2023-06-20 04:09:37.093993 text2text-1.0.7/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)    59640 2023-06-20 04:08:26.000000 text2text-1.0.7/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-20 04:09:37.093993 text2text-1.0.7/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1246 2023-06-20 04:08:56.000000 text2text-1.0.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 04:09:37.089992 text2text-1.0.7/text2text/
--rwxr-xr-x   0 root         (0) root         (0)      666 2023-06-20 02:25:27.000000 text2text-1.0.7/text2text/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7162 2023-06-20 01:53:21.000000 text2text-1.0.7/text2text/abstractor.py
--rw-r--r--   0 root         (0) root         (0)     2157 2023-06-20 01:53:21.000000 text2text-1.0.7/text2text/answerer.py
--rw-r--r--   0 root         (0) root         (0)     2287 2023-06-20 03:27:52.000000 text2text-1.0.7/text2text/assistant.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 04:09:37.091992 text2text-1.0.7/text2text/biunilm/
--rwxr-xr-x   0 root         (0) root         (0)      110 2023-06-20 01:53:21.000000 text2text-1.0.7/text2text/biunilm/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    10937 2023-06-20 01:53:21.000000 text2text-1.0.7/text2text/biunilm/loader_utils.py
--rwxr-xr-x   0 root         (0) root         (0)    17726 2023-06-20 01:53:21.000000 text2text-1.0.7/text2text/biunilm/seq2seq_loader.py
--rw-r--r--   0 root         (0) root         (0)     1533 2023-06-20 01:53:21.000000 text2text-1.0.7/text2text/bm25er.py
--rw-r--r--   0 root         (0) root         (0)      519 2023-06-20 01:53:21.000000 text2text-1.0.7/text2text/counter.py
--rw-r--r--   0 root         (0) root         (0)     1177 2023-06-20 01:53:21.000000 text2text-1.0.7/text2text/fitter.py
--rw-r--r--   0 root         (0) root         (0)     1451 2023-06-20 01:53:21.000000 text2text-1.0.7/text2text/handler.py
--rw-r--r--   0 root         (0) root         (0)     2106 2023-06-20 01:53:21.000000 text2text-1.0.7/text2text/identifier.py
--rw-r--r--   0 root         (0) root         (0)     2010 2023-06-20 03:29:02.000000 text2text-1.0.7/text2text/indexer.py
--rw-r--r--   0 root         (0) root         (0)     1165 2023-06-20 01:53:21.000000 text2text-1.0.7/text2text/measurer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 04:09:37.092993 text2text-1.0.7/text2text/pytorch_pretrained_bert/
--rwxr-xr-x   0 root         (0) root         (0)      120 2023-06-20 01:53:21.000000 text2text-1.0.7/text2text/pytorch_pretrained_bert/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      932 2023-06-20 01:53:21.000000 text2text-1.0.7/text2text/pytorch_pretrained_bert/__main__.py
--rwxr-xr-x   0 root         (0) root         (0)     7964 2023-06-20 01:53:21.000000 text2text-1.0.7/text2text/pytorch_pretrained_bert/file_utils.py
--rwxr-xr-x   0 root         (0) root         (0)     1821 2023-06-20 01:53:21.000000 text2text-1.0.7/text2text/pytorch_pretrained_bert/loss.py
--rwxr-xr-x   0 root         (0) root         (0)   108506 2023-06-20 01:53:21.000000 text2text-1.0.7/text2text/pytorch_pretrained_bert/modeling.py
--rwxr-xr-x   0 root         (0) root         (0)    15035 2023-06-20 01:53:21.000000 text2text-1.0.7/text2text/pytorch_pretrained_bert/tokenization.py
--rw-r--r--   0 root         (0) root         (0)     1782 2023-06-20 01:53:21.000000 text2text-1.0.7/text2text/questioner.py
--rw-r--r--   0 root         (0) root         (0)     2605 2023-06-20 03:20:23.000000 text2text-1.0.7/text2text/responder.py
--rw-r--r--   0 root         (0) root         (0)      984 2023-06-20 01:53:21.000000 text2text-1.0.7/text2text/searcher.py
--rw-r--r--   0 root         (0) root         (0)     1575 2023-06-20 01:53:21.000000 text2text-1.0.7/text2text/server.py
--rw-r--r--   0 root         (0) root         (0)     1103 2023-06-20 01:53:21.000000 text2text-1.0.7/text2text/summarizer.py
--rw-r--r--   0 root         (0) root         (0)     1766 2023-06-20 01:53:21.000000 text2text-1.0.7/text2text/tfidfer.py
--rw-r--r--   0 root         (0) root         (0)      780 2023-06-20 01:53:21.000000 text2text-1.0.7/text2text/tokenizer.py
--rw-r--r--   0 root         (0) root         (0)    12572 2023-06-20 02:51:51.000000 text2text-1.0.7/text2text/transformer.py
--rw-r--r--   0 root         (0) root         (0)     1489 2023-06-20 01:53:21.000000 text2text-1.0.7/text2text/translator.py
--rw-r--r--   0 root         (0) root         (0)      500 2023-06-20 01:53:21.000000 text2text-1.0.7/text2text/variator.py
--rw-r--r--   0 root         (0) root         (0)      816 2023-06-20 01:53:21.000000 text2text-1.0.7/text2text/vectorizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 04:09:37.090992 text2text-1.0.7/text2text.egg-info/
--rw-r--r--   0 root         (0) root         (0)    60454 2023-06-20 04:09:36.000000 text2text-1.0.7/text2text.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1064 2023-06-20 04:09:36.000000 text2text-1.0.7/text2text.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 04:09:36.000000 text2text-1.0.7/text2text.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      134 2023-06-20 04:09:36.000000 text2text-1.0.7/text2text.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-20 04:09:36.000000 text2text-1.0.7/text2text.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 04:13:49.048786 text2text-1.0.8/
+-rwxr-xr-x   0 root         (0) root         (0)     1418 2023-06-20 01:53:21.000000 text2text-1.0.8/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    60458 2023-06-20 04:13:49.048786 text2text-1.0.8/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)    59644 2023-06-20 04:12:48.000000 text2text-1.0.8/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-20 04:13:49.048786 text2text-1.0.8/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1246 2023-06-20 04:13:17.000000 text2text-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 04:13:49.044786 text2text-1.0.8/text2text/
+-rwxr-xr-x   0 root         (0) root         (0)      666 2023-06-20 02:25:27.000000 text2text-1.0.8/text2text/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7162 2023-06-20 01:53:21.000000 text2text-1.0.8/text2text/abstractor.py
+-rw-r--r--   0 root         (0) root         (0)     2157 2023-06-20 01:53:21.000000 text2text-1.0.8/text2text/answerer.py
+-rw-r--r--   0 root         (0) root         (0)     2287 2023-06-20 03:27:52.000000 text2text-1.0.8/text2text/assistant.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 04:13:49.046786 text2text-1.0.8/text2text/biunilm/
+-rwxr-xr-x   0 root         (0) root         (0)      110 2023-06-20 01:53:21.000000 text2text-1.0.8/text2text/biunilm/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    10937 2023-06-20 01:53:21.000000 text2text-1.0.8/text2text/biunilm/loader_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)    17726 2023-06-20 01:53:21.000000 text2text-1.0.8/text2text/biunilm/seq2seq_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-06-20 01:53:21.000000 text2text-1.0.8/text2text/bm25er.py
+-rw-r--r--   0 root         (0) root         (0)      519 2023-06-20 01:53:21.000000 text2text-1.0.8/text2text/counter.py
+-rw-r--r--   0 root         (0) root         (0)     1177 2023-06-20 01:53:21.000000 text2text-1.0.8/text2text/fitter.py
+-rw-r--r--   0 root         (0) root         (0)     1451 2023-06-20 01:53:21.000000 text2text-1.0.8/text2text/handler.py
+-rw-r--r--   0 root         (0) root         (0)     2106 2023-06-20 01:53:21.000000 text2text-1.0.8/text2text/identifier.py
+-rw-r--r--   0 root         (0) root         (0)     2010 2023-06-20 03:29:02.000000 text2text-1.0.8/text2text/indexer.py
+-rw-r--r--   0 root         (0) root         (0)     1165 2023-06-20 01:53:21.000000 text2text-1.0.8/text2text/measurer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 04:13:49.047786 text2text-1.0.8/text2text/pytorch_pretrained_bert/
+-rwxr-xr-x   0 root         (0) root         (0)      120 2023-06-20 01:53:21.000000 text2text-1.0.8/text2text/pytorch_pretrained_bert/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      932 2023-06-20 01:53:21.000000 text2text-1.0.8/text2text/pytorch_pretrained_bert/__main__.py
+-rwxr-xr-x   0 root         (0) root         (0)     7964 2023-06-20 01:53:21.000000 text2text-1.0.8/text2text/pytorch_pretrained_bert/file_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)     1821 2023-06-20 01:53:21.000000 text2text-1.0.8/text2text/pytorch_pretrained_bert/loss.py
+-rwxr-xr-x   0 root         (0) root         (0)   108506 2023-06-20 01:53:21.000000 text2text-1.0.8/text2text/pytorch_pretrained_bert/modeling.py
+-rwxr-xr-x   0 root         (0) root         (0)    15035 2023-06-20 01:53:21.000000 text2text-1.0.8/text2text/pytorch_pretrained_bert/tokenization.py
+-rw-r--r--   0 root         (0) root         (0)     1782 2023-06-20 01:53:21.000000 text2text-1.0.8/text2text/questioner.py
+-rw-r--r--   0 root         (0) root         (0)     2605 2023-06-20 03:20:23.000000 text2text-1.0.8/text2text/responder.py
+-rw-r--r--   0 root         (0) root         (0)      984 2023-06-20 01:53:21.000000 text2text-1.0.8/text2text/searcher.py
+-rw-r--r--   0 root         (0) root         (0)     1575 2023-06-20 01:53:21.000000 text2text-1.0.8/text2text/server.py
+-rw-r--r--   0 root         (0) root         (0)     1103 2023-06-20 01:53:21.000000 text2text-1.0.8/text2text/summarizer.py
+-rw-r--r--   0 root         (0) root         (0)     1766 2023-06-20 01:53:21.000000 text2text-1.0.8/text2text/tfidfer.py
+-rw-r--r--   0 root         (0) root         (0)      780 2023-06-20 01:53:21.000000 text2text-1.0.8/text2text/tokenizer.py
+-rw-r--r--   0 root         (0) root         (0)    12572 2023-06-20 02:51:51.000000 text2text-1.0.8/text2text/transformer.py
+-rw-r--r--   0 root         (0) root         (0)     1489 2023-06-20 01:53:21.000000 text2text-1.0.8/text2text/translator.py
+-rw-r--r--   0 root         (0) root         (0)      500 2023-06-20 01:53:21.000000 text2text-1.0.8/text2text/variator.py
+-rw-r--r--   0 root         (0) root         (0)      816 2023-06-20 01:53:21.000000 text2text-1.0.8/text2text/vectorizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 04:13:49.045786 text2text-1.0.8/text2text.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    60458 2023-06-20 04:13:48.000000 text2text-1.0.8/text2text.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1064 2023-06-20 04:13:48.000000 text2text-1.0.8/text2text.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 04:13:48.000000 text2text-1.0.8/text2text.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      134 2023-06-20 04:13:48.000000 text2text-1.0.8/text2text.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-20 04:13:48.000000 text2text-1.0.8/text2text.egg-info/top_level.txt
```

### Comparing `text2text-1.0.7/LICENSE.txt` & `text2text-1.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `text2text-1.0.7/PKG-INFO` & `text2text-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2text
-Version: 1.0.7
+Version: 1.0.8
 Summary: Text2Text: Crosslingual NLP/G toolkit
 Home-page: https://github.com/artitw/text2text
 Author: Artit Wangperawong
 Author-email: artitw@gmail.com
 Keywords: multilingual crosslingual gpt chatgpt bert natural language processing nlp nlg text generation gpt question answer answering information retrieval tfidf tf-idf bm25 search index summary summarizer summarization tokenizer tokenization translation backtranslation data augmentation science machine learning colab embedding levenshtein sub-word edit distance conversational dialog chatbot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -14,16 +14,16 @@
 
 # Text2Text: Crosslingual NLP/G toolkit
 Transform texts in a hundred different [languages](https://github.com/artitw/text2text#languages-available)!
 
 <details>
   <summary>Overview</summary>
 
-* [Colab Demo](https://github.com/artitw/text2text#colab-demo)
-* [Cross-Lingual Models](https://github.com/artitw/text2text#how-cross-lingual-nlp-models-work-click-to-watch)
+* [Colab Notebooks](https://github.com/artitw/text2text#colab-notebooks)
+* [Crosslingual Models](https://github.com/artitw/text2text#how-crosslingual-models-work-click-to-watch)
 * [Installation Requirements](https://github.com/artitw/text2text#installation-requirements)
 * [Class Diagram](https://github.com/artitw/text2text#class-diagram)
 * [Quick Start Guide](https://github.com/artitw/text2text#api-quick-start-guide)
 * [Languages Available](https://github.com/artitw/text2text#languages-available)
 * [Requirements & Installation](https://github.com/artitw/text2text#requirements-and-installation)
 * [Examples](https://github.com/artitw/text2text#examples)
   * [Assistant](https://github.com/artitw/text2text#assistant)
```

### Comparing `text2text-1.0.7/README.md` & `text2text-1.0.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Text2Text: Crosslingual NLP/G toolkit
 Transform texts in a hundred different [languages](https://github.com/artitw/text2text#languages-available)!
 
 <details>
   <summary>Overview</summary>
 
-* [Colab Demo](https://github.com/artitw/text2text#colab-demo)
-* [Cross-Lingual Models](https://github.com/artitw/text2text#how-cross-lingual-nlp-models-work-click-to-watch)
+* [Colab Notebooks](https://github.com/artitw/text2text#colab-notebooks)
+* [Crosslingual Models](https://github.com/artitw/text2text#how-crosslingual-models-work-click-to-watch)
 * [Installation Requirements](https://github.com/artitw/text2text#installation-requirements)
 * [Class Diagram](https://github.com/artitw/text2text#class-diagram)
 * [Quick Start Guide](https://github.com/artitw/text2text#api-quick-start-guide)
 * [Languages Available](https://github.com/artitw/text2text#languages-available)
 * [Requirements & Installation](https://github.com/artitw/text2text#requirements-and-installation)
 * [Examples](https://github.com/artitw/text2text#examples)
   * [Assistant](https://github.com/artitw/text2text#assistant)
```

### Comparing `text2text-1.0.7/setup.py` & `text2text-1.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="text2text",
-  version="1.0.7",
+  version="1.0.8",
   author="Artit Wangperawong",
   author_email="artitw@gmail.com",
   description="Text2Text: Crosslingual NLP/G toolkit",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/artitw/text2text",
   packages=setuptools.find_packages(),
```

### Comparing `text2text-1.0.7/text2text/__init__.py` & `text2text-1.0.8/text2text/__init__.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.7/text2text/abstractor.py` & `text2text-1.0.8/text2text/abstractor.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.7/text2text/answerer.py` & `text2text-1.0.8/text2text/answerer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.7/text2text/assistant.py` & `text2text-1.0.8/text2text/assistant.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.7/text2text/biunilm/loader_utils.py` & `text2text-1.0.8/text2text/biunilm/loader_utils.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.7/text2text/biunilm/seq2seq_loader.py` & `text2text-1.0.8/text2text/biunilm/seq2seq_loader.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.7/text2text/bm25er.py` & `text2text-1.0.8/text2text/bm25er.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.7/text2text/counter.py` & `text2text-1.0.8/text2text/counter.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.7/text2text/fitter.py` & `text2text-1.0.8/text2text/fitter.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.7/text2text/handler.py` & `text2text-1.0.8/text2text/handler.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.7/text2text/identifier.py` & `text2text-1.0.8/text2text/identifier.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.7/text2text/indexer.py` & `text2text-1.0.8/text2text/indexer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.7/text2text/measurer.py` & `text2text-1.0.8/text2text/measurer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.7/text2text/pytorch_pretrained_bert/__main__.py` & `text2text-1.0.8/text2text/pytorch_pretrained_bert/__main__.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.7/text2text/pytorch_pretrained_bert/file_utils.py` & `text2text-1.0.8/text2text/pytorch_pretrained_bert/file_utils.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.7/text2text/pytorch_pretrained_bert/loss.py` & `text2text-1.0.8/text2text/pytorch_pretrained_bert/loss.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.7/text2text/pytorch_pretrained_bert/modeling.py` & `text2text-1.0.8/text2text/pytorch_pretrained_bert/modeling.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.7/text2text/pytorch_pretrained_bert/tokenization.py` & `text2text-1.0.8/text2text/pytorch_pretrained_bert/tokenization.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.7/text2text/questioner.py` & `text2text-1.0.8/text2text/questioner.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.7/text2text/responder.py` & `text2text-1.0.8/text2text/responder.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.7/text2text/searcher.py` & `text2text-1.0.8/text2text/searcher.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.7/text2text/server.py` & `text2text-1.0.8/text2text/server.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.7/text2text/summarizer.py` & `text2text-1.0.8/text2text/summarizer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.7/text2text/tfidfer.py` & `text2text-1.0.8/text2text/tfidfer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.7/text2text/tokenizer.py` & `text2text-1.0.8/text2text/tokenizer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.7/text2text/transformer.py` & `text2text-1.0.8/text2text/transformer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.7/text2text/translator.py` & `text2text-1.0.8/text2text/translator.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.7/text2text/vectorizer.py` & `text2text-1.0.8/text2text/vectorizer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.7/text2text.egg-info/PKG-INFO` & `text2text-1.0.8/text2text.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2text
-Version: 1.0.7
+Version: 1.0.8
 Summary: Text2Text: Crosslingual NLP/G toolkit
 Home-page: https://github.com/artitw/text2text
 Author: Artit Wangperawong
 Author-email: artitw@gmail.com
 Keywords: multilingual crosslingual gpt chatgpt bert natural language processing nlp nlg text generation gpt question answer answering information retrieval tfidf tf-idf bm25 search index summary summarizer summarization tokenizer tokenization translation backtranslation data augmentation science machine learning colab embedding levenshtein sub-word edit distance conversational dialog chatbot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -14,16 +14,16 @@
 
 # Text2Text: Crosslingual NLP/G toolkit
 Transform texts in a hundred different [languages](https://github.com/artitw/text2text#languages-available)!
 
 <details>
   <summary>Overview</summary>
 
-* [Colab Demo](https://github.com/artitw/text2text#colab-demo)
-* [Cross-Lingual Models](https://github.com/artitw/text2text#how-cross-lingual-nlp-models-work-click-to-watch)
+* [Colab Notebooks](https://github.com/artitw/text2text#colab-notebooks)
+* [Crosslingual Models](https://github.com/artitw/text2text#how-crosslingual-models-work-click-to-watch)
 * [Installation Requirements](https://github.com/artitw/text2text#installation-requirements)
 * [Class Diagram](https://github.com/artitw/text2text#class-diagram)
 * [Quick Start Guide](https://github.com/artitw/text2text#api-quick-start-guide)
 * [Languages Available](https://github.com/artitw/text2text#languages-available)
 * [Requirements & Installation](https://github.com/artitw/text2text#requirements-and-installation)
 * [Examples](https://github.com/artitw/text2text#examples)
   * [Assistant](https://github.com/artitw/text2text#assistant)
```

### Comparing `text2text-1.0.7/text2text.egg-info/SOURCES.txt` & `text2text-1.0.8/text2text.egg-info/SOURCES.txt`

 * *Files identical despite different names*

