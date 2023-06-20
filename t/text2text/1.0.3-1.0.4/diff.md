# Comparing `tmp/text2text-1.0.3.tar.gz` & `tmp/text2text-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text2text-1.0.3.tar", last modified: Tue Jun 20 02:32:25 2023, max compression
+gzip compressed data, was "text2text-1.0.4.tar", last modified: Tue Jun 20 03:02:44 2023, max compression
```

## Comparing `text2text-1.0.3.tar` & `text2text-1.0.4.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:32:25.241954 text2text-1.0.3/
--rwxr-xr-x   0 root         (0) root         (0)     1418 2023-06-20 01:53:21.000000 text2text-1.0.3/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    60206 2023-06-20 02:32:25.241954 text2text-1.0.3/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)    59392 2023-06-20 02:27:50.000000 text2text-1.0.3/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-20 02:32:25.241954 text2text-1.0.3/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1246 2023-06-20 01:54:38.000000 text2text-1.0.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:32:25.238954 text2text-1.0.3/text2text/
--rwxr-xr-x   0 root         (0) root         (0)      666 2023-06-20 02:25:27.000000 text2text-1.0.3/text2text/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7162 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/abstractor.py
--rw-r--r--   0 root         (0) root         (0)     2157 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/answerer.py
--rw-r--r--   0 root         (0) root         (0)     1712 2023-06-20 02:17:18.000000 text2text-1.0.3/text2text/assistant.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:32:25.239954 text2text-1.0.3/text2text/biunilm/
--rwxr-xr-x   0 root         (0) root         (0)      110 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/biunilm/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    10937 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/biunilm/loader_utils.py
--rwxr-xr-x   0 root         (0) root         (0)    17726 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/biunilm/seq2seq_loader.py
--rw-r--r--   0 root         (0) root         (0)     1533 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/bm25er.py
--rw-r--r--   0 root         (0) root         (0)      519 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/counter.py
--rw-r--r--   0 root         (0) root         (0)     1177 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/fitter.py
--rw-r--r--   0 root         (0) root         (0)     1451 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/handler.py
--rw-r--r--   0 root         (0) root         (0)     2106 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/identifier.py
--rw-r--r--   0 root         (0) root         (0)     2060 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/indexer.py
--rw-r--r--   0 root         (0) root         (0)     1165 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/measurer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:32:25.240954 text2text-1.0.3/text2text/pytorch_pretrained_bert/
--rwxr-xr-x   0 root         (0) root         (0)      120 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/pytorch_pretrained_bert/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      932 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/pytorch_pretrained_bert/__main__.py
--rwxr-xr-x   0 root         (0) root         (0)     7964 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/pytorch_pretrained_bert/file_utils.py
--rwxr-xr-x   0 root         (0) root         (0)     1821 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/pytorch_pretrained_bert/loss.py
--rwxr-xr-x   0 root         (0) root         (0)   108506 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/pytorch_pretrained_bert/modeling.py
--rwxr-xr-x   0 root         (0) root         (0)    15035 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/pytorch_pretrained_bert/tokenization.py
--rw-r--r--   0 root         (0) root         (0)     1782 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/questioner.py
--rw-r--r--   0 root         (0) root         (0)     2605 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/responder.py
--rw-r--r--   0 root         (0) root         (0)      984 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/searcher.py
--rw-r--r--   0 root         (0) root         (0)     1575 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/server.py
--rw-r--r--   0 root         (0) root         (0)     1103 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/summarizer.py
--rw-r--r--   0 root         (0) root         (0)     1766 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/tfidfer.py
--rw-r--r--   0 root         (0) root         (0)      780 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/tokenizer.py
--rw-r--r--   0 root         (0) root         (0)    12572 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/transformer.py
--rw-r--r--   0 root         (0) root         (0)     1489 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/translator.py
--rw-r--r--   0 root         (0) root         (0)      500 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/variator.py
--rw-r--r--   0 root         (0) root         (0)      816 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/vectorizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:32:25.239954 text2text-1.0.3/text2text.egg-info/
--rw-r--r--   0 root         (0) root         (0)    60206 2023-06-20 02:32:25.000000 text2text-1.0.3/text2text.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1064 2023-06-20 02:32:25.000000 text2text-1.0.3/text2text.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 02:32:25.000000 text2text-1.0.3/text2text.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      134 2023-06-20 02:32:25.000000 text2text-1.0.3/text2text.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-20 02:32:25.000000 text2text-1.0.3/text2text.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 03:02:44.501189 text2text-1.0.4/
+-rwxr-xr-x   0 root         (0) root         (0)     1418 2023-06-20 01:53:21.000000 text2text-1.0.4/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    60026 2023-06-20 03:02:44.501189 text2text-1.0.4/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)    59212 2023-06-20 03:01:17.000000 text2text-1.0.4/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-20 03:02:44.501189 text2text-1.0.4/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1246 2023-06-20 03:01:47.000000 text2text-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 03:02:44.496188 text2text-1.0.4/text2text/
+-rwxr-xr-x   0 root         (0) root         (0)      666 2023-06-20 02:25:27.000000 text2text-1.0.4/text2text/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7162 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/abstractor.py
+-rw-r--r--   0 root         (0) root         (0)     2157 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/answerer.py
+-rw-r--r--   0 root         (0) root         (0)     1712 2023-06-20 02:17:18.000000 text2text-1.0.4/text2text/assistant.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 03:02:44.499189 text2text-1.0.4/text2text/biunilm/
+-rwxr-xr-x   0 root         (0) root         (0)      110 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/biunilm/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    10937 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/biunilm/loader_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)    17726 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/biunilm/seq2seq_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/bm25er.py
+-rw-r--r--   0 root         (0) root         (0)      519 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/counter.py
+-rw-r--r--   0 root         (0) root         (0)     1177 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/fitter.py
+-rw-r--r--   0 root         (0) root         (0)     1451 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/handler.py
+-rw-r--r--   0 root         (0) root         (0)     2106 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/identifier.py
+-rw-r--r--   0 root         (0) root         (0)     2060 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/indexer.py
+-rw-r--r--   0 root         (0) root         (0)     1165 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/measurer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 03:02:44.500189 text2text-1.0.4/text2text/pytorch_pretrained_bert/
+-rwxr-xr-x   0 root         (0) root         (0)      120 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/pytorch_pretrained_bert/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      932 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/pytorch_pretrained_bert/__main__.py
+-rwxr-xr-x   0 root         (0) root         (0)     7964 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/pytorch_pretrained_bert/file_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)     1821 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/pytorch_pretrained_bert/loss.py
+-rwxr-xr-x   0 root         (0) root         (0)   108506 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/pytorch_pretrained_bert/modeling.py
+-rwxr-xr-x   0 root         (0) root         (0)    15035 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/pytorch_pretrained_bert/tokenization.py
+-rw-r--r--   0 root         (0) root         (0)     1782 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/questioner.py
+-rw-r--r--   0 root         (0) root         (0)     2605 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/responder.py
+-rw-r--r--   0 root         (0) root         (0)      984 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/searcher.py
+-rw-r--r--   0 root         (0) root         (0)     1575 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/server.py
+-rw-r--r--   0 root         (0) root         (0)     1103 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/summarizer.py
+-rw-r--r--   0 root         (0) root         (0)     1766 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/tfidfer.py
+-rw-r--r--   0 root         (0) root         (0)      780 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/tokenizer.py
+-rw-r--r--   0 root         (0) root         (0)    12572 2023-06-20 02:51:51.000000 text2text-1.0.4/text2text/transformer.py
+-rw-r--r--   0 root         (0) root         (0)     1489 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/translator.py
+-rw-r--r--   0 root         (0) root         (0)      500 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/variator.py
+-rw-r--r--   0 root         (0) root         (0)      816 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/vectorizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 03:02:44.498189 text2text-1.0.4/text2text.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    60026 2023-06-20 03:02:44.000000 text2text-1.0.4/text2text.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1064 2023-06-20 03:02:44.000000 text2text-1.0.4/text2text.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 03:02:44.000000 text2text-1.0.4/text2text.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      134 2023-06-20 03:02:44.000000 text2text-1.0.4/text2text.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-20 03:02:44.000000 text2text-1.0.4/text2text.egg-info/top_level.txt
```

### Comparing `text2text-1.0.3/LICENSE.txt` & `text2text-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `text2text-1.0.3/PKG-INFO` & `text2text-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2text
-Version: 1.0.3
+Version: 1.0.4
 Summary: Text2Text: Crosslingual NLP/G toolkit
 Home-page: https://github.com/artitw/text2text
 Author: Artit Wangperawong
 Author-email: artitw@gmail.com
 Keywords: multilingual crosslingual gpt chatgpt bert natural language processing nlp nlg text generation gpt question answer answering information retrieval tfidf tf-idf bm25 search index summary summarizer summarization tokenizer tokenization translation backtranslation data augmentation science machine learning colab embedding levenshtein sub-word edit distance conversational dialog chatbot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -55,18 +55,17 @@
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1LE_ifTpOGO5QJCKNQYtZe6c_tjbwnulR)
 
 ## How Crosslingual Models Work (click to watch)
 [![Crosslingual Models](http://img.youtube.com/vi/caZLVcJqsqo/0.jpg)](https://youtu.be/caZLVcJqsqo "Cross-Lingual Models")
 
 ## Installation Requirements 
 ```
-pip install -q -U text2text
+pip install -qq -U text2text
 ```
-* Default model: >16 GB RAM
-* Smaller models: <16 GB RAM 
+* By default, all functionality in the demo and examples below work with less than 16 GB RAM, which means it runs on Colab.
   * See [Colab Demo](https://colab.research.google.com/drive/1LE_ifTpOGO5QJCKNQYtZe6c_tjbwnulR) and [Examples](#examples) below
 
 ## Class Diagram
 ```
       Indexer    Measurer   Counter -- Tfidfer
            \          \     /             \
         Searcher     Tokenizer           Bm25er
@@ -80,15 +79,15 @@
           Identifier
 ```
 
 ## Quick Start Guide
 Functionality | Invocation | Result
 :------------: | :-------------: | :-------------:
 Module Importing | `import text2text as t2t` | Libraries imported
-Language Model Setting | `t2t.Transformer.PRETRAINED_TRANSLATOR = "facebook/m2m100_418M"` | Override default with smaller model
+Language Model Setting | `t2t.Transformer.PRETRAINED_TRANSLATOR = "facebook/m2m100_418M"` | Default model
 Intialization | `h = t2t.Handler(["Hello, World!"], src_lang="en")` | Initialized handler with some text
 [Tokenization](https://github.com/artitw/text2text#tokenization) | `h.tokenize()` | `[['▁Hello', ',', '▁World', '!']]`
 [Embedding](https://github.com/artitw/text2text#embedding--vectorization) | `h.vectorize()` | `array([[0.18745188, 0.05658336, ..., 0.6332584 , 0.43805206]], dtype=float32)`
 [TF-IDF](https://github.com/artitw/text2text#tf-idf) | `h.tfidf()` | `[{'!': 0.5, ',': 0.5, '▁Hello': 0.5, '▁World': 0.5}]`
 [BM25](https://github.com/artitw/text2text#bm25) | `h.bm25()` | `[{'!': 0.3068528194400547, ',': 0.3068528194400547, '▁Hello': 0.3068528194400547, '▁World': 0.3068528194400547}]`
 [Indexer](https://github.com/artitw/text2text#index) | `i = h.index()` | Index object for similarity retrieval
 [Search](https://github.com/artitw/text2text#search) | `h.search(queries=["Hello"])` | `array([[0.09]])`
@@ -458,29 +457,22 @@
 ['联合国秘书长说,叙利亚没有军事解决方案。',
  '与大多数其他大学一样,Notre Dame的学生运行的新闻媒体渠道的数量。九个学生 - 运行的渠道包括三份报纸,两台广播电视台,以及几本杂志和杂志。 开始作为一个一页的杂志在1876年9月,该杂志的Schoolistic发行了每月两次,并声称是美国最古老的连续的大学新闻出版物,和其他杂志,TheJuggler,每年发行两次,并专注于学生文学和艺术作品。 多姆年刊每年发行。 报纸有不同的出版利益,与The Observer发表每日,主要报道大学和其他新闻,并由学生从Notre Dame和圣玛丽的学院。 与Scholastic和The Dome不同,The Observer是一个独立的公众作品,但没有教师顾',
  '细菌是生物细胞的一种类型. 它们构成一个大范围的亲生微生物. 通常几微米长,细菌有许多形状,从球到杖和螺旋。 细菌是地球上出现的第一个生命形式之一,并且存在于其大多数栖息地。',
  '生物学是研究生命的科学. 究竟什么是生命? 这可能听起来像一个愚蠢的问题,有一个显而易见的答案,但它并不容易定义生命. 例如,一个名为病毒学的生物学分支研究病毒,这些病毒表现出一些活体的特征,但缺乏其他。']
 ```
 
 #### BYOT: Bring Your Own Translator
- * The default translator requires more than 16GB of memory.
- * You can specify smaller pretrained translators at your own risk.
+ * The default translator requires no more than 16GB of memory.
+ * You can specify other pretrained translators at your own risk.
  * Make sure src_lang and tgt_lang codes conform to that model.
- * Below are some tested examples, which use less memory.
 
 <details>
   <summary>BYOT examples</summary>
 
 ```
-t2t.Transformer.PRETRAINED_TRANSLATOR = "facebook/m2m100_418M"
-t2t.Handler(["I would like to go hiking tomorrow."], 
-        src_lang="en"
-        ).translate(tgt_lang='zh')
-['我想明天去散步。']
-
 t2t.Transformer.PRETRAINED_TRANSLATOR = "facebook/mbart-large-50-many-to-many-mmt"
 t2t.Transformer.LANGUAGES = {
   'af_ZA': 'Afrikaans',
   'ar_AR': 'Arabic',
   'az_AZ': 'Azerbaijani',
   'bn_IN': 'Bengali',
   'cs_CZ': 'Czech',
@@ -744,14 +736,15 @@
 
 t2t.Handler([input_state]).respond()
 # ['About 60 different kinds of cats are recognized by various cat registries.']
 ```
 
 ### Assistant
 Based on Vicuna 13B, which is based on LLaMA, which is not commercially licensed.
+Not ChatGPT level but it works well
 ```
 instructions = "Generate a JSON object that maps English characters as keys and Greek equivalents as values: {"
 res = t2t.Handler([instructions]).assist()
 #[
 #  '{\n"a": "α",\n"b": "β",\n"c": "γ",\n"d": "δ",\n"e": "ε",\n"f": "φ",\n"g": "χ",\n"h": "ι",\n"i": "η",\n"j": "κ",\n"k": "λ",\n"l": "μ",\n"m": "ν",\n"n": "ξ",\n"o": "ο",\n"p": "π",\n"q": "ρ",\n"r": "σ",\n"s": "τ",\n"t": "υ",\n"u": "ύ",\n"v": "φ",\n"w": "χ",\n"x": "ψ",\n"y": "ω",\n"z": "ζ"\n}'
 #]
 ```
```

### Comparing `text2text-1.0.3/README.md` & `text2text-1.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -41,18 +41,17 @@
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1LE_ifTpOGO5QJCKNQYtZe6c_tjbwnulR)
 
 ## How Crosslingual Models Work (click to watch)
 [![Crosslingual Models](http://img.youtube.com/vi/caZLVcJqsqo/0.jpg)](https://youtu.be/caZLVcJqsqo "Cross-Lingual Models")
 
 ## Installation Requirements 
 ```
-pip install -q -U text2text
+pip install -qq -U text2text
 ```
-* Default model: >16 GB RAM
-* Smaller models: <16 GB RAM 
+* By default, all functionality in the demo and examples below work with less than 16 GB RAM, which means it runs on Colab.
   * See [Colab Demo](https://colab.research.google.com/drive/1LE_ifTpOGO5QJCKNQYtZe6c_tjbwnulR) and [Examples](#examples) below
 
 ## Class Diagram
 ```
       Indexer    Measurer   Counter -- Tfidfer
            \          \     /             \
         Searcher     Tokenizer           Bm25er
@@ -66,15 +65,15 @@
           Identifier
 ```
 
 ## Quick Start Guide
 Functionality | Invocation | Result
 :------------: | :-------------: | :-------------:
 Module Importing | `import text2text as t2t` | Libraries imported
-Language Model Setting | `t2t.Transformer.PRETRAINED_TRANSLATOR = "facebook/m2m100_418M"` | Override default with smaller model
+Language Model Setting | `t2t.Transformer.PRETRAINED_TRANSLATOR = "facebook/m2m100_418M"` | Default model
 Intialization | `h = t2t.Handler(["Hello, World!"], src_lang="en")` | Initialized handler with some text
 [Tokenization](https://github.com/artitw/text2text#tokenization) | `h.tokenize()` | `[['▁Hello', ',', '▁World', '!']]`
 [Embedding](https://github.com/artitw/text2text#embedding--vectorization) | `h.vectorize()` | `array([[0.18745188, 0.05658336, ..., 0.6332584 , 0.43805206]], dtype=float32)`
 [TF-IDF](https://github.com/artitw/text2text#tf-idf) | `h.tfidf()` | `[{'!': 0.5, ',': 0.5, '▁Hello': 0.5, '▁World': 0.5}]`
 [BM25](https://github.com/artitw/text2text#bm25) | `h.bm25()` | `[{'!': 0.3068528194400547, ',': 0.3068528194400547, '▁Hello': 0.3068528194400547, '▁World': 0.3068528194400547}]`
 [Indexer](https://github.com/artitw/text2text#index) | `i = h.index()` | Index object for similarity retrieval
 [Search](https://github.com/artitw/text2text#search) | `h.search(queries=["Hello"])` | `array([[0.09]])`
@@ -444,29 +443,22 @@
 ['联合国秘书长说,叙利亚没有军事解决方案。',
  '与大多数其他大学一样,Notre Dame的学生运行的新闻媒体渠道的数量。九个学生 - 运行的渠道包括三份报纸,两台广播电视台,以及几本杂志和杂志。 开始作为一个一页的杂志在1876年9月,该杂志的Schoolistic发行了每月两次,并声称是美国最古老的连续的大学新闻出版物,和其他杂志,TheJuggler,每年发行两次,并专注于学生文学和艺术作品。 多姆年刊每年发行。 报纸有不同的出版利益,与The Observer发表每日,主要报道大学和其他新闻,并由学生从Notre Dame和圣玛丽的学院。 与Scholastic和The Dome不同,The Observer是一个独立的公众作品,但没有教师顾',
  '细菌是生物细胞的一种类型. 它们构成一个大范围的亲生微生物. 通常几微米长,细菌有许多形状,从球到杖和螺旋。 细菌是地球上出现的第一个生命形式之一,并且存在于其大多数栖息地。',
  '生物学是研究生命的科学. 究竟什么是生命? 这可能听起来像一个愚蠢的问题,有一个显而易见的答案,但它并不容易定义生命. 例如,一个名为病毒学的生物学分支研究病毒,这些病毒表现出一些活体的特征,但缺乏其他。']
 ```
 
 #### BYOT: Bring Your Own Translator
- * The default translator requires more than 16GB of memory.
- * You can specify smaller pretrained translators at your own risk.
+ * The default translator requires no more than 16GB of memory.
+ * You can specify other pretrained translators at your own risk.
  * Make sure src_lang and tgt_lang codes conform to that model.
- * Below are some tested examples, which use less memory.
 
 <details>
   <summary>BYOT examples</summary>
 
 ```
-t2t.Transformer.PRETRAINED_TRANSLATOR = "facebook/m2m100_418M"
-t2t.Handler(["I would like to go hiking tomorrow."], 
-        src_lang="en"
-        ).translate(tgt_lang='zh')
-['我想明天去散步。']
-
 t2t.Transformer.PRETRAINED_TRANSLATOR = "facebook/mbart-large-50-many-to-many-mmt"
 t2t.Transformer.LANGUAGES = {
   'af_ZA': 'Afrikaans',
   'ar_AR': 'Arabic',
   'az_AZ': 'Azerbaijani',
   'bn_IN': 'Bengali',
   'cs_CZ': 'Czech',
@@ -730,14 +722,15 @@
 
 t2t.Handler([input_state]).respond()
 # ['About 60 different kinds of cats are recognized by various cat registries.']
 ```
 
 ### Assistant
 Based on Vicuna 13B, which is based on LLaMA, which is not commercially licensed.
+Not ChatGPT level but it works well
 ```
 instructions = "Generate a JSON object that maps English characters as keys and Greek equivalents as values: {"
 res = t2t.Handler([instructions]).assist()
 #[
 #  '{\n"a": "α",\n"b": "β",\n"c": "γ",\n"d": "δ",\n"e": "ε",\n"f": "φ",\n"g": "χ",\n"h": "ι",\n"i": "η",\n"j": "κ",\n"k": "λ",\n"l": "μ",\n"m": "ν",\n"n": "ξ",\n"o": "ο",\n"p": "π",\n"q": "ρ",\n"r": "σ",\n"s": "τ",\n"t": "υ",\n"u": "ύ",\n"v": "φ",\n"w": "χ",\n"x": "ψ",\n"y": "ω",\n"z": "ζ"\n}'
 #]
 ```
```

### Comparing `text2text-1.0.3/setup.py` & `text2text-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="text2text",
-  version="1.0.3",
+  version="1.0.4",
   author="Artit Wangperawong",
   author_email="artitw@gmail.com",
   description="Text2Text: Crosslingual NLP/G toolkit",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/artitw/text2text",
   packages=setuptools.find_packages(),
```

### Comparing `text2text-1.0.3/text2text/__init__.py` & `text2text-1.0.4/text2text/__init__.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.3/text2text/abstractor.py` & `text2text-1.0.4/text2text/abstractor.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.3/text2text/answerer.py` & `text2text-1.0.4/text2text/answerer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.3/text2text/assistant.py` & `text2text-1.0.4/text2text/assistant.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.3/text2text/biunilm/loader_utils.py` & `text2text-1.0.4/text2text/biunilm/loader_utils.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.3/text2text/biunilm/seq2seq_loader.py` & `text2text-1.0.4/text2text/biunilm/seq2seq_loader.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.3/text2text/bm25er.py` & `text2text-1.0.4/text2text/bm25er.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.3/text2text/counter.py` & `text2text-1.0.4/text2text/counter.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.3/text2text/fitter.py` & `text2text-1.0.4/text2text/fitter.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.3/text2text/handler.py` & `text2text-1.0.4/text2text/handler.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.3/text2text/identifier.py` & `text2text-1.0.4/text2text/identifier.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.3/text2text/indexer.py` & `text2text-1.0.4/text2text/indexer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.3/text2text/measurer.py` & `text2text-1.0.4/text2text/measurer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.3/text2text/pytorch_pretrained_bert/__main__.py` & `text2text-1.0.4/text2text/pytorch_pretrained_bert/__main__.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.3/text2text/pytorch_pretrained_bert/file_utils.py` & `text2text-1.0.4/text2text/pytorch_pretrained_bert/file_utils.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.3/text2text/pytorch_pretrained_bert/loss.py` & `text2text-1.0.4/text2text/pytorch_pretrained_bert/loss.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.3/text2text/pytorch_pretrained_bert/modeling.py` & `text2text-1.0.4/text2text/pytorch_pretrained_bert/modeling.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.3/text2text/pytorch_pretrained_bert/tokenization.py` & `text2text-1.0.4/text2text/pytorch_pretrained_bert/tokenization.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.3/text2text/questioner.py` & `text2text-1.0.4/text2text/questioner.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.3/text2text/responder.py` & `text2text-1.0.4/text2text/responder.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.3/text2text/searcher.py` & `text2text-1.0.4/text2text/searcher.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.3/text2text/server.py` & `text2text-1.0.4/text2text/server.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.3/text2text/summarizer.py` & `text2text-1.0.4/text2text/summarizer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.3/text2text/tfidfer.py` & `text2text-1.0.4/text2text/tfidfer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.3/text2text/tokenizer.py` & `text2text-1.0.4/text2text/tokenizer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.3/text2text/transformer.py` & `text2text-1.0.4/text2text/transformer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 class Transformer(object):
   """
   Base class for text transformers
   """
   STOP_WORDS = {"0o", "0s", "3a", "3b", "3d", "6b", "6o", "a", "a1", "a2", "a3", "a4", "ab", "able", "about", "above", "abst", "ac", "accordance", "according", "accordingly", "across", "act", "actually", "ad", "added", "adj", "ae", "af", "affected", "affecting", "affects", "after", "afterwards", "ag", "again", "against", "ah", "ain", "ain't", "aj", "al", "all", "allow", "allows", "almost", "alone", "along", "already", "also", "although", "always", "am", "among", "amongst", "amoungst", "amount", "an", "and", "announce", "another", "any", "anybody", "anyhow", "anymore", "anyone", "anything", "anyway", "anyways", "anywhere", "ao", "ap", "apart", "apparently", "appear", "appreciate", "appropriate", "approximately", "ar", "are", "aren", "arent", "aren't", "arise", "around", "as", "a's", "aside", "ask", "asking", "associated", "at", "au", "auth", "av", "available", "aw", "away", "awfully", "ax", "ay", "az", "b", "b1", "b2", "b3", "ba", "back", "bc", "bd", "be", "became", "because", "become", "becomes", "becoming", "been", "before", "beforehand", "begin", "beginning", "beginnings", "begins", "behind", "being", "believe", "below", "beside", "besides", "best", "better", "between", "beyond", "bi", "bill", "biol", "bj", "bk", "bl", "bn", "both", "bottom", "bp", "br", "brief", "briefly", "bs", "bt", "bu", "but", "bx", "by", "c", "c1", "c2", "c3", "ca", "call", "came", "can", "cannot", "cant", "can't", "cause", "causes", "cc", "cd", "ce", "certain", "certainly", "cf", "cg", "ch", "changes", "ci", "cit", "cj", "cl", "clearly", "cm", "c'mon", "cn", "co", "com", "come", "comes", "con", "concerning", "consequently", "consider", "considering", "contain", "containing", "contains", "corresponding", "could", "couldn", "couldnt", "couldn't", "course", "cp", "cq", "cr", "cry", "cs", "c's", "ct", "cu", "currently", "cv", "cx", "cy", "cz", "d", "d2", "da", "date", "dc", "dd", "de", "definitely", "describe", "described", "despite", "detail", "df", "di", "did", "didn", "didn't", "different", "dj", "dk", "dl", "do", "does", "doesn", "doesn't", "doing", "don", "done", "don't", "down", "downwards", "dp", "dr", "ds", "dt", "du", "due", "during", "dx", "dy", "e", "e2", "e3", "ea", "each", "ec", "ed", "edu", "ee", "ef", "effect", "eg", "ei", "eight", "eighty", "either", "ej", "el", "eleven", "else", "elsewhere", "em", "empty", "en", "end", "ending", "enough", "entirely", "eo", "ep", "eq", "er", "es", "especially", "est", "et", "et-al", "etc", "eu", "ev", "even", "ever", "every", "everybody", "everyone", "everything", "everywhere", "ex", "exactly", "example", "except", "ey", "f", "f2", "fa", "far", "fc", "few", "ff", "fi", "fifteen", "fifth", "fify", "fill", "find", "fire", "first", "five", "fix", "fj", "fl", "fn", "fo", "followed", "following", "follows", "for", "former", "formerly", "forth", "forty", "found", "four", "fr", "from", "front", "fs", "ft", "fu", "full", "further", "furthermore", "fy", "g", "ga", "gave", "ge", "get", "gets", "getting", "gi", "give", "given", "gives", "giving", "gj", "gl", "go", "goes", "going", "gone", "got", "gotten", "gr", "greetings", "gs", "gy", "h", "h2", "h3", "had", "hadn", "hadn't", "happens", "hardly", "has", "hasn", "hasnt", "hasn't", "have", "haven", "haven't", "having", "he", "hed", "he'd", "he'll", "hello", "help", "hence", "her", "here", "hereafter", "hereby", "herein", "heres", "here's", "hereupon", "hers", "herself", "hes", "he's", "hh", "hi", "hid", "him", "himself", "his", "hither", "hj", "ho", "home", "hopefully", "how", "howbeit", "however", "how's", "hr", "hs", "http", "hu", "hundred", "hy", "i", "i2", "i3", "i4", "i6", "i7", "i8", "ia", "ib", "ibid", "ic", "id", "i'd", "ie", "if", "ig", "ignored", "ih", "ii", "ij", "il", "i'll", "im", "i'm", "immediate", "immediately", "importance", "important", "in", "inasmuch", "inc", "indeed", "index", "indicate", "indicated", "indicates", "information", "inner", "insofar", "instead", "interest", "into", "invention", "inward", "io", "ip", "iq", "ir", "is", "isn", "isn't", "it", "itd", "it'd", "it'll", "its", "it's", "itself", "iv", "i've", "ix", "iy", "iz", "j", "jj", "jr", "js", "jt", "ju", "just", "k", "ke", "keep", "keeps", "kept", "kg", "kj", "km", "know", "known", "knows", "ko", "l", "l2", "la", "largely", "last", "lately", "later", "latter", "latterly", "lb", "lc", "le", "least", "les", "less", "lest", "let", "lets", "let's", "lf", "like", "liked", "likely", "line", "little", "lj", "ll", "ll", "ln", "lo", "look", "looking", "looks", "los", "lr", "ls", "lt", "ltd", "m", "m2", "ma", "made", "mainly", "make", "makes", "many", "may", "maybe", "me", "mean", "means", "meantime", "meanwhile", "merely", "mg", "might", "mightn", "mightn't", "mill", "million", "mine", "miss", "ml", "mn", "mo", "more", "moreover", "most", "mostly", "move", "mr", "mrs", "ms", "mt", "mu", "much", "mug", "must", "mustn", "mustn't", "my", "myself", "n", "n2", "na", "name", "namely", "nay", "nc", "nd", "ne", "near", "nearly", "necessarily", "necessary", "need", "needn", "needn't", "needs", "neither", "never", "nevertheless", "new", "next", "ng", "ni", "nine", "ninety", "nj", "nl", "nn", "no", "nobody", "non", "none", "nonetheless", "noone", "nor", "normally", "nos", "not", "noted", "nothing", "novel", "now", "nowhere", "nr", "ns", "nt", "ny", "o", "oa", "ob", "obtain", "obtained", "obviously", "oc", "od", "of", "off", "often", "og", "oh", "oi", "oj", "ok", "okay", "ol", "old", "om", "omitted", "on", "once", "one", "ones", "only", "onto", "oo", "op", "oq", "or", "ord", "os", "ot", "other", "others", "otherwise", "ou", "ought", "our", "ours", "ourselves", "out", "outside", "over", "overall", "ow", "owing", "own", "ox", "oz", "p", "p1", "p2", "p3", "page", "pagecount", "pages", "par", "part", "particular", "particularly", "pas", "past", "pc", "pd", "pe", "per", "perhaps", "pf", "ph", "pi", "pj", "pk", "pl", "placed", "please", "plus", "pm", "pn", "po", "poorly", "possible", "possibly", "potentially", "pp", "pq", "pr", "predominantly", "present", "presumably", "previously", "primarily", "probably", "promptly", "proud", "provides", "ps", "pt", "pu", "put", "py", "q", "qj", "qu", "que", "quickly", "quite", "qv", "r", "r2", "ra", "ran", "rather", "rc", "rd", "re", "readily", "really", "reasonably", "recent", "recently", "ref", "refs", "regarding", "regardless", "regards", "related", "relatively", "research", "research-articl", "respectively", "resulted", "resulting", "results", "rf", "rh", "ri", "right", "rj", "rl", "rm", "rn", "ro", "rq", "rr", "rs", "rt", "ru", "run", "rv", "ry", "s", "s2", "sa", "said", "same", "saw", "say", "saying", "says", "sc", "sd", "se", "sec", "second", "secondly", "section", "see", "seeing", "seem", "seemed", "seeming", "seems", "seen", "self", "selves", "sensible", "sent", "serious", "seriously", "seven", "several", "sf", "shall", "shan", "shan't", "she", "shed", "she'd", "she'll", "shes", "she's", "should", "shouldn", "shouldn't", "should've", "show", "showed", "shown", "showns", "shows", "si", "side", "significant", "significantly", "similar", "similarly", "since", "sincere", "six", "sixty", "sj", "sl", "slightly", "sm", "sn", "so", "some", "somebody", "somehow", "someone", "somethan", "something", "sometime", "sometimes", "somewhat", "somewhere", "soon", "sorry", "sp", "specifically", "specified", "specify", "specifying", "sq", "sr", "ss", "st", "still", "stop", "strongly", "sub", "substantially", "successfully", "such", "sufficiently", "suggest", "sup", "sure", "sy", "system", "sz", "t", "t1", "t2", "t3", "take", "taken", "taking", "tb", "tc", "td", "te", "tell", "ten", "tends", "tf", "th", "than", "thank", "thanks", "thanx", "that", "that'll", "thats", "that's", "that've", "the", "their", "theirs", "them", "themselves", "then", "thence", "there", "thereafter", "thereby", "thered", "therefore", "therein", "there'll", "thereof", "therere", "theres", "there's", "thereto", "thereupon", "there've", "these", "they", "theyd", "they'd", "they'll", "theyre", "they're", "they've", "thickv", "thin", "think", "third", "this", "thorough", "thoroughly", "those", "thou", "though", "thoughh", "thousand", "three", "throug", "through", "throughout", "thru", "thus", "ti", "til", "tip", "tj", "tl", "tm", "tn", "to", "together", "too", "took", "top", "toward", "towards", "tp", "tq", "tr", "tried", "tries", "truly", "try", "trying", "ts", "t's", "tt", "tv", "twelve", "twenty", "twice", "two", "tx", "u", "u201d", "ue", "ui", "uj", "uk", "um", "un", "under", "unfortunately", "unless", "unlike", "unlikely", "until", "unto", "uo", "up", "upon", "ups", "ur", "us", "use", "used", "useful", "usefully", "usefulness", "uses", "using", "usually", "ut", "v", "va", "value", "various", "vd", "ve", "ve", "very", "via", "viz", "vj", "vo", "vol", "vols", "volumtype", "vq", "vs", "vt", "vu", "w", "wa", "want", "wants", "was", "wasn", "wasnt", "wasn't", "way", "we", "wed", "we'd", "welcome", "well", "we'll", "well-b", "went", "were", "we're", "weren", "werent", "weren't", "we've", "what", "whatever", "what'll", "whats", "what's", "when", "whence", "whenever", "when's", "where", "whereafter", "whereas", "whereby", "wherein", "wheres", "where's", "whereupon", "wherever", "whether", "which", "while", "whim", "whither", "who", "whod", "whoever", "whole", "who'll", "whom", "whomever", "whos", "who's", "whose", "why", "why's", "wi", "widely", "will", "willing", "wish", "with", "within", "without", "wo", "won", "wonder", "wont", "won't", "words", "world", "would", "wouldn", "wouldnt", "wouldn't", "www", "x", "x1", "x2", "x3", "xf", "xi", "xj", "xk", "xl", "xn", "xo", "xs", "xt", "xv", "xx", "y", "y2", "yes", "yet", "yj", "yl", "you", "youd", "you'd", "you'll", "your", "youre", "you're", "yours", "yourself", "yourselves", "you've", "yr", "ys", "yt", "z", "zero", "zi", "zz",}
-  PRETRAINED_TRANSLATOR = "facebook/m2m100_1.2B"
+  PRETRAINED_TRANSLATOR = "facebook/m2m100_418M"
   LANGUAGES = {
     'af': 'Afrikaans',
     'am': 'Amharic',
     'ar': 'Arabic',
     'ast': 'Asturian',
     'az': 'Azerbaijani',
     'ba': 'Bashkir',
```

### Comparing `text2text-1.0.3/text2text/translator.py` & `text2text-1.0.4/text2text/translator.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.3/text2text/vectorizer.py` & `text2text-1.0.4/text2text/vectorizer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.3/text2text.egg-info/PKG-INFO` & `text2text-1.0.4/text2text.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2text
-Version: 1.0.3
+Version: 1.0.4
 Summary: Text2Text: Crosslingual NLP/G toolkit
 Home-page: https://github.com/artitw/text2text
 Author: Artit Wangperawong
 Author-email: artitw@gmail.com
 Keywords: multilingual crosslingual gpt chatgpt bert natural language processing nlp nlg text generation gpt question answer answering information retrieval tfidf tf-idf bm25 search index summary summarizer summarization tokenizer tokenization translation backtranslation data augmentation science machine learning colab embedding levenshtein sub-word edit distance conversational dialog chatbot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -55,18 +55,17 @@
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1LE_ifTpOGO5QJCKNQYtZe6c_tjbwnulR)
 
 ## How Crosslingual Models Work (click to watch)
 [![Crosslingual Models](http://img.youtube.com/vi/caZLVcJqsqo/0.jpg)](https://youtu.be/caZLVcJqsqo "Cross-Lingual Models")
 
 ## Installation Requirements 
 ```
-pip install -q -U text2text
+pip install -qq -U text2text
 ```
-* Default model: >16 GB RAM
-* Smaller models: <16 GB RAM 
+* By default, all functionality in the demo and examples below work with less than 16 GB RAM, which means it runs on Colab.
   * See [Colab Demo](https://colab.research.google.com/drive/1LE_ifTpOGO5QJCKNQYtZe6c_tjbwnulR) and [Examples](#examples) below
 
 ## Class Diagram
 ```
       Indexer    Measurer   Counter -- Tfidfer
            \          \     /             \
         Searcher     Tokenizer           Bm25er
@@ -80,15 +79,15 @@
           Identifier
 ```
 
 ## Quick Start Guide
 Functionality | Invocation | Result
 :------------: | :-------------: | :-------------:
 Module Importing | `import text2text as t2t` | Libraries imported
-Language Model Setting | `t2t.Transformer.PRETRAINED_TRANSLATOR = "facebook/m2m100_418M"` | Override default with smaller model
+Language Model Setting | `t2t.Transformer.PRETRAINED_TRANSLATOR = "facebook/m2m100_418M"` | Default model
 Intialization | `h = t2t.Handler(["Hello, World!"], src_lang="en")` | Initialized handler with some text
 [Tokenization](https://github.com/artitw/text2text#tokenization) | `h.tokenize()` | `[['▁Hello', ',', '▁World', '!']]`
 [Embedding](https://github.com/artitw/text2text#embedding--vectorization) | `h.vectorize()` | `array([[0.18745188, 0.05658336, ..., 0.6332584 , 0.43805206]], dtype=float32)`
 [TF-IDF](https://github.com/artitw/text2text#tf-idf) | `h.tfidf()` | `[{'!': 0.5, ',': 0.5, '▁Hello': 0.5, '▁World': 0.5}]`
 [BM25](https://github.com/artitw/text2text#bm25) | `h.bm25()` | `[{'!': 0.3068528194400547, ',': 0.3068528194400547, '▁Hello': 0.3068528194400547, '▁World': 0.3068528194400547}]`
 [Indexer](https://github.com/artitw/text2text#index) | `i = h.index()` | Index object for similarity retrieval
 [Search](https://github.com/artitw/text2text#search) | `h.search(queries=["Hello"])` | `array([[0.09]])`
@@ -458,29 +457,22 @@
 ['联合国秘书长说,叙利亚没有军事解决方案。',
  '与大多数其他大学一样,Notre Dame的学生运行的新闻媒体渠道的数量。九个学生 - 运行的渠道包括三份报纸,两台广播电视台,以及几本杂志和杂志。 开始作为一个一页的杂志在1876年9月,该杂志的Schoolistic发行了每月两次,并声称是美国最古老的连续的大学新闻出版物,和其他杂志,TheJuggler,每年发行两次,并专注于学生文学和艺术作品。 多姆年刊每年发行。 报纸有不同的出版利益,与The Observer发表每日,主要报道大学和其他新闻,并由学生从Notre Dame和圣玛丽的学院。 与Scholastic和The Dome不同,The Observer是一个独立的公众作品,但没有教师顾',
  '细菌是生物细胞的一种类型. 它们构成一个大范围的亲生微生物. 通常几微米长,细菌有许多形状,从球到杖和螺旋。 细菌是地球上出现的第一个生命形式之一,并且存在于其大多数栖息地。',
  '生物学是研究生命的科学. 究竟什么是生命? 这可能听起来像一个愚蠢的问题,有一个显而易见的答案,但它并不容易定义生命. 例如,一个名为病毒学的生物学分支研究病毒,这些病毒表现出一些活体的特征,但缺乏其他。']
 ```
 
 #### BYOT: Bring Your Own Translator
- * The default translator requires more than 16GB of memory.
- * You can specify smaller pretrained translators at your own risk.
+ * The default translator requires no more than 16GB of memory.
+ * You can specify other pretrained translators at your own risk.
  * Make sure src_lang and tgt_lang codes conform to that model.
- * Below are some tested examples, which use less memory.
 
 <details>
   <summary>BYOT examples</summary>
 
 ```
-t2t.Transformer.PRETRAINED_TRANSLATOR = "facebook/m2m100_418M"
-t2t.Handler(["I would like to go hiking tomorrow."], 
-        src_lang="en"
-        ).translate(tgt_lang='zh')
-['我想明天去散步。']
-
 t2t.Transformer.PRETRAINED_TRANSLATOR = "facebook/mbart-large-50-many-to-many-mmt"
 t2t.Transformer.LANGUAGES = {
   'af_ZA': 'Afrikaans',
   'ar_AR': 'Arabic',
   'az_AZ': 'Azerbaijani',
   'bn_IN': 'Bengali',
   'cs_CZ': 'Czech',
@@ -744,14 +736,15 @@
 
 t2t.Handler([input_state]).respond()
 # ['About 60 different kinds of cats are recognized by various cat registries.']
 ```
 
 ### Assistant
 Based on Vicuna 13B, which is based on LLaMA, which is not commercially licensed.
+Not ChatGPT level but it works well
 ```
 instructions = "Generate a JSON object that maps English characters as keys and Greek equivalents as values: {"
 res = t2t.Handler([instructions]).assist()
 #[
 #  '{\n"a": "α",\n"b": "β",\n"c": "γ",\n"d": "δ",\n"e": "ε",\n"f": "φ",\n"g": "χ",\n"h": "ι",\n"i": "η",\n"j": "κ",\n"k": "λ",\n"l": "μ",\n"m": "ν",\n"n": "ξ",\n"o": "ο",\n"p": "π",\n"q": "ρ",\n"r": "σ",\n"s": "τ",\n"t": "υ",\n"u": "ύ",\n"v": "φ",\n"w": "χ",\n"x": "ψ",\n"y": "ω",\n"z": "ζ"\n}'
 #]
 ```
```

### Comparing `text2text-1.0.3/text2text.egg-info/SOURCES.txt` & `text2text-1.0.4/text2text.egg-info/SOURCES.txt`

 * *Files identical despite different names*

