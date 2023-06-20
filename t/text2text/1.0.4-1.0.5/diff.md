# Comparing `tmp/text2text-1.0.4.tar.gz` & `tmp/text2text-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text2text-1.0.4.tar", last modified: Tue Jun 20 03:02:44 2023, max compression
+gzip compressed data, was "text2text-1.0.5.tar", last modified: Tue Jun 20 03:42:18 2023, max compression
```

## Comparing `text2text-1.0.4.tar` & `text2text-1.0.5.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 03:02:44.501189 text2text-1.0.4/
--rwxr-xr-x   0 root         (0) root         (0)     1418 2023-06-20 01:53:21.000000 text2text-1.0.4/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    60026 2023-06-20 03:02:44.501189 text2text-1.0.4/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)    59212 2023-06-20 03:01:17.000000 text2text-1.0.4/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-20 03:02:44.501189 text2text-1.0.4/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1246 2023-06-20 03:01:47.000000 text2text-1.0.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 03:02:44.496188 text2text-1.0.4/text2text/
--rwxr-xr-x   0 root         (0) root         (0)      666 2023-06-20 02:25:27.000000 text2text-1.0.4/text2text/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7162 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/abstractor.py
--rw-r--r--   0 root         (0) root         (0)     2157 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/answerer.py
--rw-r--r--   0 root         (0) root         (0)     1712 2023-06-20 02:17:18.000000 text2text-1.0.4/text2text/assistant.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 03:02:44.499189 text2text-1.0.4/text2text/biunilm/
--rwxr-xr-x   0 root         (0) root         (0)      110 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/biunilm/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    10937 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/biunilm/loader_utils.py
--rwxr-xr-x   0 root         (0) root         (0)    17726 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/biunilm/seq2seq_loader.py
--rw-r--r--   0 root         (0) root         (0)     1533 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/bm25er.py
--rw-r--r--   0 root         (0) root         (0)      519 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/counter.py
--rw-r--r--   0 root         (0) root         (0)     1177 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/fitter.py
--rw-r--r--   0 root         (0) root         (0)     1451 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/handler.py
--rw-r--r--   0 root         (0) root         (0)     2106 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/identifier.py
--rw-r--r--   0 root         (0) root         (0)     2060 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/indexer.py
--rw-r--r--   0 root         (0) root         (0)     1165 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/measurer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 03:02:44.500189 text2text-1.0.4/text2text/pytorch_pretrained_bert/
--rwxr-xr-x   0 root         (0) root         (0)      120 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/pytorch_pretrained_bert/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      932 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/pytorch_pretrained_bert/__main__.py
--rwxr-xr-x   0 root         (0) root         (0)     7964 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/pytorch_pretrained_bert/file_utils.py
--rwxr-xr-x   0 root         (0) root         (0)     1821 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/pytorch_pretrained_bert/loss.py
--rwxr-xr-x   0 root         (0) root         (0)   108506 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/pytorch_pretrained_bert/modeling.py
--rwxr-xr-x   0 root         (0) root         (0)    15035 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/pytorch_pretrained_bert/tokenization.py
--rw-r--r--   0 root         (0) root         (0)     1782 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/questioner.py
--rw-r--r--   0 root         (0) root         (0)     2605 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/responder.py
--rw-r--r--   0 root         (0) root         (0)      984 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/searcher.py
--rw-r--r--   0 root         (0) root         (0)     1575 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/server.py
--rw-r--r--   0 root         (0) root         (0)     1103 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/summarizer.py
--rw-r--r--   0 root         (0) root         (0)     1766 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/tfidfer.py
--rw-r--r--   0 root         (0) root         (0)      780 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/tokenizer.py
--rw-r--r--   0 root         (0) root         (0)    12572 2023-06-20 02:51:51.000000 text2text-1.0.4/text2text/transformer.py
--rw-r--r--   0 root         (0) root         (0)     1489 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/translator.py
--rw-r--r--   0 root         (0) root         (0)      500 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/variator.py
--rw-r--r--   0 root         (0) root         (0)      816 2023-06-20 01:53:21.000000 text2text-1.0.4/text2text/vectorizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 03:02:44.498189 text2text-1.0.4/text2text.egg-info/
--rw-r--r--   0 root         (0) root         (0)    60026 2023-06-20 03:02:44.000000 text2text-1.0.4/text2text.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1064 2023-06-20 03:02:44.000000 text2text-1.0.4/text2text.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 03:02:44.000000 text2text-1.0.4/text2text.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      134 2023-06-20 03:02:44.000000 text2text-1.0.4/text2text.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-20 03:02:44.000000 text2text-1.0.4/text2text.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 03:42:18.389214 text2text-1.0.5/
+-rwxr-xr-x   0 root         (0) root         (0)     1418 2023-06-20 01:53:21.000000 text2text-1.0.5/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    60233 2023-06-20 03:42:18.389214 text2text-1.0.5/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)    59419 2023-06-20 03:41:03.000000 text2text-1.0.5/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-20 03:42:18.389214 text2text-1.0.5/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1246 2023-06-20 03:41:58.000000 text2text-1.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 03:42:18.385214 text2text-1.0.5/text2text/
+-rwxr-xr-x   0 root         (0) root         (0)      666 2023-06-20 02:25:27.000000 text2text-1.0.5/text2text/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7162 2023-06-20 01:53:21.000000 text2text-1.0.5/text2text/abstractor.py
+-rw-r--r--   0 root         (0) root         (0)     2157 2023-06-20 01:53:21.000000 text2text-1.0.5/text2text/answerer.py
+-rw-r--r--   0 root         (0) root         (0)     2287 2023-06-20 03:27:52.000000 text2text-1.0.5/text2text/assistant.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 03:42:18.387214 text2text-1.0.5/text2text/biunilm/
+-rwxr-xr-x   0 root         (0) root         (0)      110 2023-06-20 01:53:21.000000 text2text-1.0.5/text2text/biunilm/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    10937 2023-06-20 01:53:21.000000 text2text-1.0.5/text2text/biunilm/loader_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)    17726 2023-06-20 01:53:21.000000 text2text-1.0.5/text2text/biunilm/seq2seq_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-06-20 01:53:21.000000 text2text-1.0.5/text2text/bm25er.py
+-rw-r--r--   0 root         (0) root         (0)      519 2023-06-20 01:53:21.000000 text2text-1.0.5/text2text/counter.py
+-rw-r--r--   0 root         (0) root         (0)     1177 2023-06-20 01:53:21.000000 text2text-1.0.5/text2text/fitter.py
+-rw-r--r--   0 root         (0) root         (0)     1451 2023-06-20 01:53:21.000000 text2text-1.0.5/text2text/handler.py
+-rw-r--r--   0 root         (0) root         (0)     2106 2023-06-20 01:53:21.000000 text2text-1.0.5/text2text/identifier.py
+-rw-r--r--   0 root         (0) root         (0)     2010 2023-06-20 03:29:02.000000 text2text-1.0.5/text2text/indexer.py
+-rw-r--r--   0 root         (0) root         (0)     1165 2023-06-20 01:53:21.000000 text2text-1.0.5/text2text/measurer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 03:42:18.388214 text2text-1.0.5/text2text/pytorch_pretrained_bert/
+-rwxr-xr-x   0 root         (0) root         (0)      120 2023-06-20 01:53:21.000000 text2text-1.0.5/text2text/pytorch_pretrained_bert/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      932 2023-06-20 01:53:21.000000 text2text-1.0.5/text2text/pytorch_pretrained_bert/__main__.py
+-rwxr-xr-x   0 root         (0) root         (0)     7964 2023-06-20 01:53:21.000000 text2text-1.0.5/text2text/pytorch_pretrained_bert/file_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)     1821 2023-06-20 01:53:21.000000 text2text-1.0.5/text2text/pytorch_pretrained_bert/loss.py
+-rwxr-xr-x   0 root         (0) root         (0)   108506 2023-06-20 01:53:21.000000 text2text-1.0.5/text2text/pytorch_pretrained_bert/modeling.py
+-rwxr-xr-x   0 root         (0) root         (0)    15035 2023-06-20 01:53:21.000000 text2text-1.0.5/text2text/pytorch_pretrained_bert/tokenization.py
+-rw-r--r--   0 root         (0) root         (0)     1782 2023-06-20 01:53:21.000000 text2text-1.0.5/text2text/questioner.py
+-rw-r--r--   0 root         (0) root         (0)     2605 2023-06-20 03:20:23.000000 text2text-1.0.5/text2text/responder.py
+-rw-r--r--   0 root         (0) root         (0)      984 2023-06-20 01:53:21.000000 text2text-1.0.5/text2text/searcher.py
+-rw-r--r--   0 root         (0) root         (0)     1575 2023-06-20 01:53:21.000000 text2text-1.0.5/text2text/server.py
+-rw-r--r--   0 root         (0) root         (0)     1103 2023-06-20 01:53:21.000000 text2text-1.0.5/text2text/summarizer.py
+-rw-r--r--   0 root         (0) root         (0)     1766 2023-06-20 01:53:21.000000 text2text-1.0.5/text2text/tfidfer.py
+-rw-r--r--   0 root         (0) root         (0)      780 2023-06-20 01:53:21.000000 text2text-1.0.5/text2text/tokenizer.py
+-rw-r--r--   0 root         (0) root         (0)    12572 2023-06-20 02:51:51.000000 text2text-1.0.5/text2text/transformer.py
+-rw-r--r--   0 root         (0) root         (0)     1489 2023-06-20 01:53:21.000000 text2text-1.0.5/text2text/translator.py
+-rw-r--r--   0 root         (0) root         (0)      500 2023-06-20 01:53:21.000000 text2text-1.0.5/text2text/variator.py
+-rw-r--r--   0 root         (0) root         (0)      816 2023-06-20 01:53:21.000000 text2text-1.0.5/text2text/vectorizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 03:42:18.386214 text2text-1.0.5/text2text.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    60233 2023-06-20 03:42:18.000000 text2text-1.0.5/text2text.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1064 2023-06-20 03:42:18.000000 text2text-1.0.5/text2text.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 03:42:18.000000 text2text-1.0.5/text2text.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      134 2023-06-20 03:42:18.000000 text2text-1.0.5/text2text.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-20 03:42:18.000000 text2text-1.0.5/text2text.egg-info/top_level.txt
```

### Comparing `text2text-1.0.4/LICENSE.txt` & `text2text-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `text2text-1.0.4/PKG-INFO` & `text2text-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2text
-Version: 1.0.4
+Version: 1.0.5
 Summary: Text2Text: Crosslingual NLP/G toolkit
 Home-page: https://github.com/artitw/text2text
 Author: Artit Wangperawong
 Author-email: artitw@gmail.com
 Keywords: multilingual crosslingual gpt chatgpt bert natural language processing nlp nlg text generation gpt question answer answering information retrieval tfidf tf-idf bm25 search index summary summarizer summarization tokenizer tokenization translation backtranslation data augmentation science machine learning colab embedding levenshtein sub-word edit distance conversational dialog chatbot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -35,16 +35,16 @@
   * [Search](https://github.com/artitw/text2text#search)
   * [Distance](https://github.com/artitw/text2text#levenshtein-sub-word-edit-distance)
   * [Translation](https://github.com/artitw/text2text#translation)
   * [Question Answering](https://github.com/artitw/text2text#question-answering)
   * [Question Generation](https://github.com/artitw/text2text#question-generation)
   * [Summarization](https://github.com/artitw/text2text#summarization)
   * [Data Augmentation](https://github.com/artitw/text2text#data-augmentation--back-translation)
-  * [Dialog Responder](https://github.com/artitw/text2text#dialog-responder)
   * [Assistant](https://github.com/artitw/text2text#assistant)
+  * [Dialog Responder](https://github.com/artitw/text2text#dialog-responder)
   * [Finetuning](https://github.com/artitw/text2text#training--finetuning)
   * [Identification](https://github.com/artitw/text2text#identification)
   * [Web Server](https://github.com/artitw/text2text#serving)
 * [Questions?](https://github.com/artitw/text2text#questions)
 * [Citation](https://github.com/artitw/text2text#citation)
 * [Contributing](https://github.com/artitw/text2text#contributing)
 * [Code of Conduct](https://github.com/artitw/text2text#code-of-conduct)
@@ -91,16 +91,16 @@
 [BM25](https://github.com/artitw/text2text#bm25) | `h.bm25()` | `[{'!': 0.3068528194400547, ',': 0.3068528194400547, '▁Hello': 0.3068528194400547, '▁World': 0.3068528194400547}]`
 [Indexer](https://github.com/artitw/text2text#index) | `i = h.index()` | Index object for similarity retrieval
 [Search](https://github.com/artitw/text2text#search) | `h.search(queries=["Hello"])` | `array([[0.09]])`
 [Translation](https://github.com/artitw/text2text#translation) | `h.translate(tgt_lang="zh")` | `['你好,世界!']`
 [Question Generation](https://github.com/artitw/text2text#question-generation) | `h.question()` | `[('What is the name of the world you are in?', 'The world')]`
 [Summarization](https://github.com/artitw/text2text#summarization) | `h.summarize()` | `["World ' s largest world"]`
 [Data Augmentation](https://github.com/artitw/text2text#data-augmentation--back-translation) | `h.variate()` | `['Hello the world!', 'Welcome to the world.', 'Hello to the world!',...`
-[Dialog Response](https://github.com/artitw/text2text#dialog-responder) | `t2t.Handler(["[CONTEXT] Hello EOS How are you?"]).respond()` | `['I am doing great. How are you?']`
 [Assistant](https://github.com/artitw/text2text#assistant) | `t2t.Handler(["Describe Text2Text in a few words: "]).assist()` | `['Text2Text is an AI-powered text generation tool that creates coherent and continuous text based on prompts.']`
+[Dialog Response](https://github.com/artitw/text2text#dialog-responder) | `t2t.Handler(["[CONTEXT] Hello EOS How are you?"]).respond()` | `['I am doing great. How are you?']`
 [Question Answering](https://github.com/artitw/text2text#question-answering) | `t2t.Handler(["Hello, World! [SEP] Hello, what?"]).answer()` | `['World']`
 [Distance](https://github.com/artitw/text2text#levenshtein-sub-word-edit-distance) | `t2t.Handler(["Hello, World! [SEP] Hello, what?"]).measure()` | `[2]`
 [Training/Finetuning](https://github.com/artitw/text2text#training--finetuning) | `t2t.Handler(["Hello, World! [TGT] Hello, what?"]).fit()` | Finetuned model saved
 [Identification](https://github.com/artitw/text2text#identification) | `t2t.Handler(["Aj keď sa Buzz Aldrin stal až „druhým človekom“..."]).identify()` | `['sk', 'Slovak']`
 [Web Server](https://github.com/artitw/text2text#serving) | `t2t.Server(host='0.0.0.0', port=80)` | Web server started on host and port
 
 ## Languages Available
@@ -713,14 +713,26 @@
  'Bakteries are a type of biological cell. They were the best of prokaryotic microorganisms. They were one of the many micrometres, the bacteria are a lot of processes, from processes and processes. Bakteries are one of the processes of processes that are processed on Earth, and they are processed in all processes.',
  'Bacteria are a type of biocells, they make up a large area of probiotic microorganisms, usually several meters long bacteria have several shapes, from branches to roots and spirals, bacteria are one of the first forms of life that appear on Earth and are present in most of their habitats.',
  'The bacteria is a type of biological cells. The bacteria is a large area of prokaryotic microorganisms. The bacteria is a long micrometres, the bacteria is a spheres in roads and spirals. The bacteria is among the data, data, data, data and data.']
 ```
 
 </details>
 
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
+```
+
 ### Dialog Responder
 Respond to given instructions, knowledge base, and dialog context.
 To use a dynamic knowledge base, see [![Q&A Dialog Demo](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/19zaOzY-VU7pYkjCUlnxLzV-b51ZqASFq?usp=sharing)
 ```
 instruction = ''
 knowledge = 'Domestic cats are valued by humans for companionship and their ability to kill rodents. About 60 cat breeds are recognized by various cat registries.'
 dialog = [
@@ -734,25 +746,14 @@
 dialog = ' EOS '.join(dialog)
 input_state = f"{instruction} [CONTEXT] {dialog} {knowledge}"
 
 t2t.Handler([input_state]).respond()
 # ['About 60 different kinds of cats are recognized by various cat registries.']
 ```
 
-### Assistant
-Based on Vicuna 13B, which is based on LLaMA, which is not commercially licensed.
-Not ChatGPT level but it works well
-```
-instructions = "Generate a JSON object that maps English characters as keys and Greek equivalents as values: {"
-res = t2t.Handler([instructions]).assist()
-#[
-#  '{\n"a": "α",\n"b": "β",\n"c": "γ",\n"d": "δ",\n"e": "ε",\n"f": "φ",\n"g": "χ",\n"h": "ι",\n"i": "η",\n"j": "κ",\n"k": "λ",\n"l": "μ",\n"m": "ν",\n"n": "ξ",\n"o": "ο",\n"p": "π",\n"q": "ρ",\n"r": "σ",\n"s": "τ",\n"t": "υ",\n"u": "ύ",\n"v": "φ",\n"w": "χ",\n"x": "ψ",\n"y": "ω",\n"z": "ζ"\n}'
-#]
-```
-
 ### Training / Finetuning
 Finetune cross-lingual model on your data
 ```
 result = t2t.Handler(["Hello, World! [TGT] 你好,世界!"], 
             src_lang="en",
             tgt_lang="zh",
             num_epochs=10,
```

### Comparing `text2text-1.0.4/README.md` & `text2text-1.0.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -21,16 +21,16 @@
   * [Search](https://github.com/artitw/text2text#search)
   * [Distance](https://github.com/artitw/text2text#levenshtein-sub-word-edit-distance)
   * [Translation](https://github.com/artitw/text2text#translation)
   * [Question Answering](https://github.com/artitw/text2text#question-answering)
   * [Question Generation](https://github.com/artitw/text2text#question-generation)
   * [Summarization](https://github.com/artitw/text2text#summarization)
   * [Data Augmentation](https://github.com/artitw/text2text#data-augmentation--back-translation)
-  * [Dialog Responder](https://github.com/artitw/text2text#dialog-responder)
   * [Assistant](https://github.com/artitw/text2text#assistant)
+  * [Dialog Responder](https://github.com/artitw/text2text#dialog-responder)
   * [Finetuning](https://github.com/artitw/text2text#training--finetuning)
   * [Identification](https://github.com/artitw/text2text#identification)
   * [Web Server](https://github.com/artitw/text2text#serving)
 * [Questions?](https://github.com/artitw/text2text#questions)
 * [Citation](https://github.com/artitw/text2text#citation)
 * [Contributing](https://github.com/artitw/text2text#contributing)
 * [Code of Conduct](https://github.com/artitw/text2text#code-of-conduct)
@@ -77,16 +77,16 @@
 [BM25](https://github.com/artitw/text2text#bm25) | `h.bm25()` | `[{'!': 0.3068528194400547, ',': 0.3068528194400547, '▁Hello': 0.3068528194400547, '▁World': 0.3068528194400547}]`
 [Indexer](https://github.com/artitw/text2text#index) | `i = h.index()` | Index object for similarity retrieval
 [Search](https://github.com/artitw/text2text#search) | `h.search(queries=["Hello"])` | `array([[0.09]])`
 [Translation](https://github.com/artitw/text2text#translation) | `h.translate(tgt_lang="zh")` | `['你好,世界!']`
 [Question Generation](https://github.com/artitw/text2text#question-generation) | `h.question()` | `[('What is the name of the world you are in?', 'The world')]`
 [Summarization](https://github.com/artitw/text2text#summarization) | `h.summarize()` | `["World ' s largest world"]`
 [Data Augmentation](https://github.com/artitw/text2text#data-augmentation--back-translation) | `h.variate()` | `['Hello the world!', 'Welcome to the world.', 'Hello to the world!',...`
-[Dialog Response](https://github.com/artitw/text2text#dialog-responder) | `t2t.Handler(["[CONTEXT] Hello EOS How are you?"]).respond()` | `['I am doing great. How are you?']`
 [Assistant](https://github.com/artitw/text2text#assistant) | `t2t.Handler(["Describe Text2Text in a few words: "]).assist()` | `['Text2Text is an AI-powered text generation tool that creates coherent and continuous text based on prompts.']`
+[Dialog Response](https://github.com/artitw/text2text#dialog-responder) | `t2t.Handler(["[CONTEXT] Hello EOS How are you?"]).respond()` | `['I am doing great. How are you?']`
 [Question Answering](https://github.com/artitw/text2text#question-answering) | `t2t.Handler(["Hello, World! [SEP] Hello, what?"]).answer()` | `['World']`
 [Distance](https://github.com/artitw/text2text#levenshtein-sub-word-edit-distance) | `t2t.Handler(["Hello, World! [SEP] Hello, what?"]).measure()` | `[2]`
 [Training/Finetuning](https://github.com/artitw/text2text#training--finetuning) | `t2t.Handler(["Hello, World! [TGT] Hello, what?"]).fit()` | Finetuned model saved
 [Identification](https://github.com/artitw/text2text#identification) | `t2t.Handler(["Aj keď sa Buzz Aldrin stal až „druhým človekom“..."]).identify()` | `['sk', 'Slovak']`
 [Web Server](https://github.com/artitw/text2text#serving) | `t2t.Server(host='0.0.0.0', port=80)` | Web server started on host and port
 
 ## Languages Available
@@ -699,14 +699,26 @@
  'Bakteries are a type of biological cell. They were the best of prokaryotic microorganisms. They were one of the many micrometres, the bacteria are a lot of processes, from processes and processes. Bakteries are one of the processes of processes that are processed on Earth, and they are processed in all processes.',
  'Bacteria are a type of biocells, they make up a large area of probiotic microorganisms, usually several meters long bacteria have several shapes, from branches to roots and spirals, bacteria are one of the first forms of life that appear on Earth and are present in most of their habitats.',
  'The bacteria is a type of biological cells. The bacteria is a large area of prokaryotic microorganisms. The bacteria is a long micrometres, the bacteria is a spheres in roads and spirals. The bacteria is among the data, data, data, data and data.']
 ```
 
 </details>
 
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
+```
+
 ### Dialog Responder
 Respond to given instructions, knowledge base, and dialog context.
 To use a dynamic knowledge base, see [![Q&A Dialog Demo](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/19zaOzY-VU7pYkjCUlnxLzV-b51ZqASFq?usp=sharing)
 ```
 instruction = ''
 knowledge = 'Domestic cats are valued by humans for companionship and their ability to kill rodents. About 60 cat breeds are recognized by various cat registries.'
 dialog = [
@@ -720,25 +732,14 @@
 dialog = ' EOS '.join(dialog)
 input_state = f"{instruction} [CONTEXT] {dialog} {knowledge}"
 
 t2t.Handler([input_state]).respond()
 # ['About 60 different kinds of cats are recognized by various cat registries.']
 ```
 
-### Assistant
-Based on Vicuna 13B, which is based on LLaMA, which is not commercially licensed.
-Not ChatGPT level but it works well
-```
-instructions = "Generate a JSON object that maps English characters as keys and Greek equivalents as values: {"
-res = t2t.Handler([instructions]).assist()
-#[
-#  '{\n"a": "α",\n"b": "β",\n"c": "γ",\n"d": "δ",\n"e": "ε",\n"f": "φ",\n"g": "χ",\n"h": "ι",\n"i": "η",\n"j": "κ",\n"k": "λ",\n"l": "μ",\n"m": "ν",\n"n": "ξ",\n"o": "ο",\n"p": "π",\n"q": "ρ",\n"r": "σ",\n"s": "τ",\n"t": "υ",\n"u": "ύ",\n"v": "φ",\n"w": "χ",\n"x": "ψ",\n"y": "ω",\n"z": "ζ"\n}'
-#]
-```
-
 ### Training / Finetuning
 Finetune cross-lingual model on your data
 ```
 result = t2t.Handler(["Hello, World! [TGT] 你好,世界!"], 
             src_lang="en",
             tgt_lang="zh",
             num_epochs=10,
```

### Comparing `text2text-1.0.4/setup.py` & `text2text-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="text2text",
-  version="1.0.4",
+  version="1.0.5",
   author="Artit Wangperawong",
   author_email="artitw@gmail.com",
   description="Text2Text: Crosslingual NLP/G toolkit",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/artitw/text2text",
   packages=setuptools.find_packages(),
```

### Comparing `text2text-1.0.4/text2text/__init__.py` & `text2text-1.0.5/text2text/__init__.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.4/text2text/abstractor.py` & `text2text-1.0.5/text2text/abstractor.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.4/text2text/answerer.py` & `text2text-1.0.5/text2text/answerer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.4/text2text/assistant.py` & `text2text-1.0.5/text2text/assistant.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import pandas as pd
 import text2text as t2t
 from transformers import AutoTokenizer
 from auto_gptq import AutoGPTQForCausalLM
 
 class Assistant(t2t.Transformer):
 
   def __init__(self, **kwargs):
@@ -15,24 +16,34 @@
       use_safetensors=True,
       trust_remote_code=False,
       device="cuda:0",
       use_triton=False,
       quantize_config=None
     )
 
-  def transform(self, input_lines, src_lang='en', **kwargs):
-    input_lines = [f'''USER: {prompt}\nASSISTANT:''' for prompt in input_lines]
+  def transform(self, input_lines, src_lang='en', knowledge_base=None, **kwargs):
+    input_lines = t2t.Transformer.transform(self, input_lines, src_lang, **kwargs)
+    df = pd.DataFrame({"input_line": input_lines})
+    if src_lang != 'en':
+      df["input_line"] = self._translate_lines(df["input_line"].tolist(), src_lang, 'en')
+    if knowledge_base:
+      corpus, index = knowledge_base
+      article_ids = index.search(df["input_line"].str.lower().tolist(), k=1)[1]
+      df["knowledge"] = [corpus[i[0]] for i in article_ids]
+      df["input_line"] = df["knowledge"] + " - " + df["input_line"]
+    df["input_line"] = "USER: " + df["input_line"] + "\nASSISTANT:"
     temperature = kwargs.get('temperature', 0.7)
     top_p = kwargs.get('top_p', 0.9)
     top_k = kwargs.get('top_k', 0)
     repetition_penalty = kwargs.get('repetition_penalty', 1.1)
     max_new_tokens = kwargs.get('max_new_tokens', 512)
     tok = self.__class__.tokenizer
     m = self.__class__.model
-    input_ids = tok(input_lines, return_tensors="pt").input_ids
+
+    input_ids = tok(df["input_line"].tolist(), return_tensors="pt", padding=True).input_ids
     input_ids = input_ids.to(m.device)
     generate_kwargs = dict(
         input_ids=input_ids,
         max_new_tokens=max_new_tokens,
         temperature=temperature,
         do_sample=temperature > 0.0,
         top_p=top_p,
```

### Comparing `text2text-1.0.4/text2text/biunilm/loader_utils.py` & `text2text-1.0.5/text2text/biunilm/loader_utils.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.4/text2text/biunilm/seq2seq_loader.py` & `text2text-1.0.5/text2text/biunilm/seq2seq_loader.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.4/text2text/bm25er.py` & `text2text-1.0.5/text2text/bm25er.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.4/text2text/counter.py` & `text2text-1.0.5/text2text/counter.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.4/text2text/fitter.py` & `text2text-1.0.5/text2text/fitter.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.4/text2text/handler.py` & `text2text-1.0.5/text2text/handler.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.4/text2text/identifier.py` & `text2text-1.0.5/text2text/identifier.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.4/text2text/indexer.py` & `text2text-1.0.5/text2text/indexer.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,12 +41,11 @@
       return []
     xq = self.get_formatted_matrix(input_lines, src_lang=src_lang, **kwargs)
     return self.index.search(xq, k)
 
   def transform(self, input_lines, src_lang='en', ids=[], encoders=[t2t.Tfidfer], **kwargs):
     self.encoders = encoders
     d = self.get_formatted_matrix(["DUMMY"], src_lang=src_lang, **kwargs).shape[-1]
-    print(f"Creating index with {d} dimensions.")
     self.index = faiss.IndexIDMap2(faiss.IndexFlatL2(d))
     if not input_lines:
       return self
     return self.add(input_lines, src_lang=src_lang, ids=ids, **kwargs)
```

### Comparing `text2text-1.0.4/text2text/measurer.py` & `text2text-1.0.5/text2text/measurer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.4/text2text/pytorch_pretrained_bert/__main__.py` & `text2text-1.0.5/text2text/pytorch_pretrained_bert/__main__.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.4/text2text/pytorch_pretrained_bert/file_utils.py` & `text2text-1.0.5/text2text/pytorch_pretrained_bert/file_utils.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.4/text2text/pytorch_pretrained_bert/loss.py` & `text2text-1.0.5/text2text/pytorch_pretrained_bert/loss.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.4/text2text/pytorch_pretrained_bert/modeling.py` & `text2text-1.0.5/text2text/pytorch_pretrained_bert/modeling.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.4/text2text/pytorch_pretrained_bert/tokenization.py` & `text2text-1.0.5/text2text/pytorch_pretrained_bert/tokenization.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.4/text2text/questioner.py` & `text2text-1.0.5/text2text/questioner.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.4/text2text/responder.py` & `text2text-1.0.5/text2text/responder.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.4/text2text/searcher.py` & `text2text-1.0.5/text2text/searcher.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.4/text2text/server.py` & `text2text-1.0.5/text2text/server.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.4/text2text/summarizer.py` & `text2text-1.0.5/text2text/summarizer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.4/text2text/tfidfer.py` & `text2text-1.0.5/text2text/tfidfer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.4/text2text/tokenizer.py` & `text2text-1.0.5/text2text/tokenizer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.4/text2text/transformer.py` & `text2text-1.0.5/text2text/transformer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.4/text2text/translator.py` & `text2text-1.0.5/text2text/translator.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.4/text2text/vectorizer.py` & `text2text-1.0.5/text2text/vectorizer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.4/text2text.egg-info/PKG-INFO` & `text2text-1.0.5/text2text.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2text
-Version: 1.0.4
+Version: 1.0.5
 Summary: Text2Text: Crosslingual NLP/G toolkit
 Home-page: https://github.com/artitw/text2text
 Author: Artit Wangperawong
 Author-email: artitw@gmail.com
 Keywords: multilingual crosslingual gpt chatgpt bert natural language processing nlp nlg text generation gpt question answer answering information retrieval tfidf tf-idf bm25 search index summary summarizer summarization tokenizer tokenization translation backtranslation data augmentation science machine learning colab embedding levenshtein sub-word edit distance conversational dialog chatbot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -35,16 +35,16 @@
   * [Search](https://github.com/artitw/text2text#search)
   * [Distance](https://github.com/artitw/text2text#levenshtein-sub-word-edit-distance)
   * [Translation](https://github.com/artitw/text2text#translation)
   * [Question Answering](https://github.com/artitw/text2text#question-answering)
   * [Question Generation](https://github.com/artitw/text2text#question-generation)
   * [Summarization](https://github.com/artitw/text2text#summarization)
   * [Data Augmentation](https://github.com/artitw/text2text#data-augmentation--back-translation)
-  * [Dialog Responder](https://github.com/artitw/text2text#dialog-responder)
   * [Assistant](https://github.com/artitw/text2text#assistant)
+  * [Dialog Responder](https://github.com/artitw/text2text#dialog-responder)
   * [Finetuning](https://github.com/artitw/text2text#training--finetuning)
   * [Identification](https://github.com/artitw/text2text#identification)
   * [Web Server](https://github.com/artitw/text2text#serving)
 * [Questions?](https://github.com/artitw/text2text#questions)
 * [Citation](https://github.com/artitw/text2text#citation)
 * [Contributing](https://github.com/artitw/text2text#contributing)
 * [Code of Conduct](https://github.com/artitw/text2text#code-of-conduct)
@@ -91,16 +91,16 @@
 [BM25](https://github.com/artitw/text2text#bm25) | `h.bm25()` | `[{'!': 0.3068528194400547, ',': 0.3068528194400547, '▁Hello': 0.3068528194400547, '▁World': 0.3068528194400547}]`
 [Indexer](https://github.com/artitw/text2text#index) | `i = h.index()` | Index object for similarity retrieval
 [Search](https://github.com/artitw/text2text#search) | `h.search(queries=["Hello"])` | `array([[0.09]])`
 [Translation](https://github.com/artitw/text2text#translation) | `h.translate(tgt_lang="zh")` | `['你好,世界!']`
 [Question Generation](https://github.com/artitw/text2text#question-generation) | `h.question()` | `[('What is the name of the world you are in?', 'The world')]`
 [Summarization](https://github.com/artitw/text2text#summarization) | `h.summarize()` | `["World ' s largest world"]`
 [Data Augmentation](https://github.com/artitw/text2text#data-augmentation--back-translation) | `h.variate()` | `['Hello the world!', 'Welcome to the world.', 'Hello to the world!',...`
-[Dialog Response](https://github.com/artitw/text2text#dialog-responder) | `t2t.Handler(["[CONTEXT] Hello EOS How are you?"]).respond()` | `['I am doing great. How are you?']`
 [Assistant](https://github.com/artitw/text2text#assistant) | `t2t.Handler(["Describe Text2Text in a few words: "]).assist()` | `['Text2Text is an AI-powered text generation tool that creates coherent and continuous text based on prompts.']`
+[Dialog Response](https://github.com/artitw/text2text#dialog-responder) | `t2t.Handler(["[CONTEXT] Hello EOS How are you?"]).respond()` | `['I am doing great. How are you?']`
 [Question Answering](https://github.com/artitw/text2text#question-answering) | `t2t.Handler(["Hello, World! [SEP] Hello, what?"]).answer()` | `['World']`
 [Distance](https://github.com/artitw/text2text#levenshtein-sub-word-edit-distance) | `t2t.Handler(["Hello, World! [SEP] Hello, what?"]).measure()` | `[2]`
 [Training/Finetuning](https://github.com/artitw/text2text#training--finetuning) | `t2t.Handler(["Hello, World! [TGT] Hello, what?"]).fit()` | Finetuned model saved
 [Identification](https://github.com/artitw/text2text#identification) | `t2t.Handler(["Aj keď sa Buzz Aldrin stal až „druhým človekom“..."]).identify()` | `['sk', 'Slovak']`
 [Web Server](https://github.com/artitw/text2text#serving) | `t2t.Server(host='0.0.0.0', port=80)` | Web server started on host and port
 
 ## Languages Available
@@ -713,14 +713,26 @@
  'Bakteries are a type of biological cell. They were the best of prokaryotic microorganisms. They were one of the many micrometres, the bacteria are a lot of processes, from processes and processes. Bakteries are one of the processes of processes that are processed on Earth, and they are processed in all processes.',
  'Bacteria are a type of biocells, they make up a large area of probiotic microorganisms, usually several meters long bacteria have several shapes, from branches to roots and spirals, bacteria are one of the first forms of life that appear on Earth and are present in most of their habitats.',
  'The bacteria is a type of biological cells. The bacteria is a large area of prokaryotic microorganisms. The bacteria is a long micrometres, the bacteria is a spheres in roads and spirals. The bacteria is among the data, data, data, data and data.']
 ```
 
 </details>
 
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
+```
+
 ### Dialog Responder
 Respond to given instructions, knowledge base, and dialog context.
 To use a dynamic knowledge base, see [![Q&A Dialog Demo](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/19zaOzY-VU7pYkjCUlnxLzV-b51ZqASFq?usp=sharing)
 ```
 instruction = ''
 knowledge = 'Domestic cats are valued by humans for companionship and their ability to kill rodents. About 60 cat breeds are recognized by various cat registries.'
 dialog = [
@@ -734,25 +746,14 @@
 dialog = ' EOS '.join(dialog)
 input_state = f"{instruction} [CONTEXT] {dialog} {knowledge}"
 
 t2t.Handler([input_state]).respond()
 # ['About 60 different kinds of cats are recognized by various cat registries.']
 ```
 
-### Assistant
-Based on Vicuna 13B, which is based on LLaMA, which is not commercially licensed.
-Not ChatGPT level but it works well
-```
-instructions = "Generate a JSON object that maps English characters as keys and Greek equivalents as values: {"
-res = t2t.Handler([instructions]).assist()
-#[
-#  '{\n"a": "α",\n"b": "β",\n"c": "γ",\n"d": "δ",\n"e": "ε",\n"f": "φ",\n"g": "χ",\n"h": "ι",\n"i": "η",\n"j": "κ",\n"k": "λ",\n"l": "μ",\n"m": "ν",\n"n": "ξ",\n"o": "ο",\n"p": "π",\n"q": "ρ",\n"r": "σ",\n"s": "τ",\n"t": "υ",\n"u": "ύ",\n"v": "φ",\n"w": "χ",\n"x": "ψ",\n"y": "ω",\n"z": "ζ"\n}'
-#]
-```
-
 ### Training / Finetuning
 Finetune cross-lingual model on your data
 ```
 result = t2t.Handler(["Hello, World! [TGT] 你好,世界!"], 
             src_lang="en",
             tgt_lang="zh",
             num_epochs=10,
```

### Comparing `text2text-1.0.4/text2text.egg-info/SOURCES.txt` & `text2text-1.0.5/text2text.egg-info/SOURCES.txt`

 * *Files identical despite different names*

