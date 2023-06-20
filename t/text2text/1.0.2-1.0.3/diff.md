# Comparing `tmp/text2text-1.0.2.tar.gz` & `tmp/text2text-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text2text-1.0.2.tar", last modified: Tue May 30 00:03:29 2023, max compression
+gzip compressed data, was "text2text-1.0.3.tar", last modified: Tue Jun 20 02:32:25 2023, max compression
```

## Comparing `text2text-1.0.2.tar` & `text2text-1.0.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:03:29.633010 text2text-1.0.2/
--rwxr-xr-x   0 root         (0) root         (0)     1418 2023-05-29 23:46:11.000000 text2text-1.0.2/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    60436 2023-05-30 00:03:29.633010 text2text-1.0.2/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)    59622 2023-05-29 23:43:37.000000 text2text-1.0.2/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-30 00:03:29.633010 text2text-1.0.2/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1229 2023-05-29 23:44:03.000000 text2text-1.0.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:03:29.630010 text2text-1.0.2/text2text/
--rwxr-xr-x   0 root         (0) root         (0)      666 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7162 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/abstractor.py
--rw-r--r--   0 root         (0) root         (0)     2157 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/answerer.py
--rw-r--r--   0 root         (0) root         (0)     1497 2023-05-29 23:34:43.000000 text2text-1.0.2/text2text/assistant.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:03:29.631009 text2text-1.0.2/text2text/biunilm/
--rwxr-xr-x   0 root         (0) root         (0)      110 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/biunilm/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    10937 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/biunilm/loader_utils.py
--rwxr-xr-x   0 root         (0) root         (0)    17726 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/biunilm/seq2seq_loader.py
--rw-r--r--   0 root         (0) root         (0)     1533 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/bm25er.py
--rw-r--r--   0 root         (0) root         (0)      519 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/counter.py
--rw-r--r--   0 root         (0) root         (0)     1177 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/fitter.py
--rw-r--r--   0 root         (0) root         (0)     1451 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/handler.py
--rw-r--r--   0 root         (0) root         (0)     2106 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/identifier.py
--rw-r--r--   0 root         (0) root         (0)     2060 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/indexer.py
--rw-r--r--   0 root         (0) root         (0)     1165 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/measurer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:03:29.632010 text2text-1.0.2/text2text/pytorch_pretrained_bert/
--rwxr-xr-x   0 root         (0) root         (0)      120 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/pytorch_pretrained_bert/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      932 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/pytorch_pretrained_bert/__main__.py
--rwxr-xr-x   0 root         (0) root         (0)     7964 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/pytorch_pretrained_bert/file_utils.py
--rwxr-xr-x   0 root         (0) root         (0)     1821 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/pytorch_pretrained_bert/loss.py
--rwxr-xr-x   0 root         (0) root         (0)   108506 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/pytorch_pretrained_bert/modeling.py
--rwxr-xr-x   0 root         (0) root         (0)    15035 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/pytorch_pretrained_bert/tokenization.py
--rw-r--r--   0 root         (0) root         (0)     1782 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/questioner.py
--rw-r--r--   0 root         (0) root         (0)     2605 2023-05-29 23:35:06.000000 text2text-1.0.2/text2text/responder.py
--rw-r--r--   0 root         (0) root         (0)      984 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/searcher.py
--rw-r--r--   0 root         (0) root         (0)     1575 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/server.py
--rw-r--r--   0 root         (0) root         (0)     1103 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/summarizer.py
--rw-r--r--   0 root         (0) root         (0)     1766 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/tfidfer.py
--rw-r--r--   0 root         (0) root         (0)      780 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/tokenizer.py
--rw-r--r--   0 root         (0) root         (0)    12572 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/transformer.py
--rw-r--r--   0 root         (0) root         (0)     1489 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/translator.py
--rw-r--r--   0 root         (0) root         (0)      500 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/variator.py
--rw-r--r--   0 root         (0) root         (0)      816 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/vectorizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:03:29.631009 text2text-1.0.2/text2text.egg-info/
--rw-r--r--   0 root         (0) root         (0)    60436 2023-05-30 00:03:29.000000 text2text-1.0.2/text2text.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1064 2023-05-30 00:03:29.000000 text2text-1.0.2/text2text.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 00:03:29.000000 text2text-1.0.2/text2text.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      124 2023-05-30 00:03:29.000000 text2text-1.0.2/text2text.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-30 00:03:29.000000 text2text-1.0.2/text2text.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:32:25.241954 text2text-1.0.3/
+-rwxr-xr-x   0 root         (0) root         (0)     1418 2023-06-20 01:53:21.000000 text2text-1.0.3/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    60206 2023-06-20 02:32:25.241954 text2text-1.0.3/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)    59392 2023-06-20 02:27:50.000000 text2text-1.0.3/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-20 02:32:25.241954 text2text-1.0.3/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1246 2023-06-20 01:54:38.000000 text2text-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:32:25.238954 text2text-1.0.3/text2text/
+-rwxr-xr-x   0 root         (0) root         (0)      666 2023-06-20 02:25:27.000000 text2text-1.0.3/text2text/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7162 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/abstractor.py
+-rw-r--r--   0 root         (0) root         (0)     2157 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/answerer.py
+-rw-r--r--   0 root         (0) root         (0)     1712 2023-06-20 02:17:18.000000 text2text-1.0.3/text2text/assistant.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:32:25.239954 text2text-1.0.3/text2text/biunilm/
+-rwxr-xr-x   0 root         (0) root         (0)      110 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/biunilm/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    10937 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/biunilm/loader_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)    17726 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/biunilm/seq2seq_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/bm25er.py
+-rw-r--r--   0 root         (0) root         (0)      519 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/counter.py
+-rw-r--r--   0 root         (0) root         (0)     1177 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/fitter.py
+-rw-r--r--   0 root         (0) root         (0)     1451 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/handler.py
+-rw-r--r--   0 root         (0) root         (0)     2106 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/identifier.py
+-rw-r--r--   0 root         (0) root         (0)     2060 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/indexer.py
+-rw-r--r--   0 root         (0) root         (0)     1165 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/measurer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:32:25.240954 text2text-1.0.3/text2text/pytorch_pretrained_bert/
+-rwxr-xr-x   0 root         (0) root         (0)      120 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/pytorch_pretrained_bert/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      932 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/pytorch_pretrained_bert/__main__.py
+-rwxr-xr-x   0 root         (0) root         (0)     7964 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/pytorch_pretrained_bert/file_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)     1821 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/pytorch_pretrained_bert/loss.py
+-rwxr-xr-x   0 root         (0) root         (0)   108506 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/pytorch_pretrained_bert/modeling.py
+-rwxr-xr-x   0 root         (0) root         (0)    15035 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/pytorch_pretrained_bert/tokenization.py
+-rw-r--r--   0 root         (0) root         (0)     1782 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/questioner.py
+-rw-r--r--   0 root         (0) root         (0)     2605 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/responder.py
+-rw-r--r--   0 root         (0) root         (0)      984 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/searcher.py
+-rw-r--r--   0 root         (0) root         (0)     1575 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/server.py
+-rw-r--r--   0 root         (0) root         (0)     1103 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/summarizer.py
+-rw-r--r--   0 root         (0) root         (0)     1766 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/tfidfer.py
+-rw-r--r--   0 root         (0) root         (0)      780 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/tokenizer.py
+-rw-r--r--   0 root         (0) root         (0)    12572 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/transformer.py
+-rw-r--r--   0 root         (0) root         (0)     1489 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/translator.py
+-rw-r--r--   0 root         (0) root         (0)      500 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/variator.py
+-rw-r--r--   0 root         (0) root         (0)      816 2023-06-20 01:53:21.000000 text2text-1.0.3/text2text/vectorizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:32:25.239954 text2text-1.0.3/text2text.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    60206 2023-06-20 02:32:25.000000 text2text-1.0.3/text2text.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1064 2023-06-20 02:32:25.000000 text2text-1.0.3/text2text.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 02:32:25.000000 text2text-1.0.3/text2text.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      134 2023-06-20 02:32:25.000000 text2text-1.0.3/text2text.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-20 02:32:25.000000 text2text-1.0.3/text2text.egg-info/top_level.txt
```

### Comparing `text2text-1.0.2/LICENSE.txt` & `text2text-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `text2text-1.0.2/PKG-INFO` & `text2text-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2text
-Version: 1.0.2
+Version: 1.0.3
 Summary: Text2Text: Crosslingual NLP/G toolkit
 Home-page: https://github.com/artitw/text2text
 Author: Artit Wangperawong
 Author-email: artitw@gmail.com
 Keywords: multilingual crosslingual gpt chatgpt bert natural language processing nlp nlg text generation gpt question answer answering information retrieval tfidf tf-idf bm25 search index summary summarizer summarization tokenizer tokenization translation backtranslation data augmentation science machine learning colab embedding levenshtein sub-word edit distance conversational dialog chatbot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -93,15 +93,15 @@
 [Indexer](https://github.com/artitw/text2text#index) | `i = h.index()` | Index object for similarity retrieval
 [Search](https://github.com/artitw/text2text#search) | `h.search(queries=["Hello"])` | `array([[0.09]])`
 [Translation](https://github.com/artitw/text2text#translation) | `h.translate(tgt_lang="zh")` | `['你好,世界!']`
 [Question Generation](https://github.com/artitw/text2text#question-generation) | `h.question()` | `[('What is the name of the world you are in?', 'The world')]`
 [Summarization](https://github.com/artitw/text2text#summarization) | `h.summarize()` | `["World ' s largest world"]`
 [Data Augmentation](https://github.com/artitw/text2text#data-augmentation--back-translation) | `h.variate()` | `['Hello the world!', 'Welcome to the world.', 'Hello to the world!',...`
 [Dialog Response](https://github.com/artitw/text2text#dialog-responder) | `t2t.Handler(["[CONTEXT] Hello EOS How are you?"]).respond()` | `['I am doing great. How are you?']`
-[Assistant](https://github.com/artitw/text2text#assistant) | `t2t.Handler(["Explain Text2Text in one sentence"]).assist()` | `['Text to text translation uses a deep learning model to generate a text in another language from a given source text.']`
+[Assistant](https://github.com/artitw/text2text#assistant) | `t2t.Handler(["Describe Text2Text in a few words: "]).assist()` | `['Text2Text is an AI-powered text generation tool that creates coherent and continuous text based on prompts.']`
 [Question Answering](https://github.com/artitw/text2text#question-answering) | `t2t.Handler(["Hello, World! [SEP] Hello, what?"]).answer()` | `['World']`
 [Distance](https://github.com/artitw/text2text#levenshtein-sub-word-edit-distance) | `t2t.Handler(["Hello, World! [SEP] Hello, what?"]).measure()` | `[2]`
 [Training/Finetuning](https://github.com/artitw/text2text#training--finetuning) | `t2t.Handler(["Hello, World! [TGT] Hello, what?"]).fit()` | Finetuned model saved
 [Identification](https://github.com/artitw/text2text#identification) | `t2t.Handler(["Aj keď sa Buzz Aldrin stal až „druhým človekom“..."]).identify()` | `['sk', 'Slovak']`
 [Web Server](https://github.com/artitw/text2text#serving) | `t2t.Server(host='0.0.0.0', port=80)` | Web server started on host and port
 
 ## Languages Available
@@ -743,24 +743,21 @@
 input_state = f"{instruction} [CONTEXT] {dialog} {knowledge}"
 
 t2t.Handler([input_state]).respond()
 # ['About 60 different kinds of cats are recognized by various cat registries.']
 ```
 
 ### Assistant
-Based on LLaMA, which is not commercially licensed.
+Based on Vicuna 13B, which is based on LLaMA, which is not commercially licensed.
 ```
-instructions = """
-Generate a JSON output mapping with keys as English characters and values as Greek equivalents.
-{
-"""
+instructions = "Generate a JSON object that maps English characters as keys and Greek equivalents as values: {"
 res = t2t.Handler([instructions]).assist()
-# 1) Find an open source project that you are interested in. You can do this by searching the internet for the project name or using a search engine to find the project page on GitHub.
-# 2) Verify that you have the necessary permissions to make changes to the code. If the project uses basic permissions, you can use git to check out the code. If the code uses more advanced permissions, you can find a way to use those permissions.
-# 3) Perform a code review to ensure that your contributions are properly credits and, if necessary, include a reasoning of your changes.
+#[
+#  '{\n"a": "α",\n"b": "β",\n"c": "γ",\n"d": "δ",\n"e": "ε",\n"f": "φ",\n"g": "χ",\n"h": "ι",\n"i": "η",\n"j": "κ",\n"k": "λ",\n"l": "μ",\n"m": "ν",\n"n": "ξ",\n"o": "ο",\n"p": "π",\n"q": "ρ",\n"r": "σ",\n"s": "τ",\n"t": "υ",\n"u": "ύ",\n"v": "φ",\n"w": "χ",\n"x": "ψ",\n"y": "ω",\n"z": "ζ"\n}'
+#]
 ```
 
 ### Training / Finetuning
 Finetune cross-lingual model on your data
 ```
 result = t2t.Handler(["Hello, World! [TGT] 你好,世界!"], 
             src_lang="en",
```

### Comparing `text2text-1.0.2/README.md` & `text2text-1.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 [Indexer](https://github.com/artitw/text2text#index) | `i = h.index()` | Index object for similarity retrieval
 [Search](https://github.com/artitw/text2text#search) | `h.search(queries=["Hello"])` | `array([[0.09]])`
 [Translation](https://github.com/artitw/text2text#translation) | `h.translate(tgt_lang="zh")` | `['你好,世界!']`
 [Question Generation](https://github.com/artitw/text2text#question-generation) | `h.question()` | `[('What is the name of the world you are in?', 'The world')]`
 [Summarization](https://github.com/artitw/text2text#summarization) | `h.summarize()` | `["World ' s largest world"]`
 [Data Augmentation](https://github.com/artitw/text2text#data-augmentation--back-translation) | `h.variate()` | `['Hello the world!', 'Welcome to the world.', 'Hello to the world!',...`
 [Dialog Response](https://github.com/artitw/text2text#dialog-responder) | `t2t.Handler(["[CONTEXT] Hello EOS How are you?"]).respond()` | `['I am doing great. How are you?']`
-[Assistant](https://github.com/artitw/text2text#assistant) | `t2t.Handler(["Explain Text2Text in one sentence"]).assist()` | `['Text to text translation uses a deep learning model to generate a text in another language from a given source text.']`
+[Assistant](https://github.com/artitw/text2text#assistant) | `t2t.Handler(["Describe Text2Text in a few words: "]).assist()` | `['Text2Text is an AI-powered text generation tool that creates coherent and continuous text based on prompts.']`
 [Question Answering](https://github.com/artitw/text2text#question-answering) | `t2t.Handler(["Hello, World! [SEP] Hello, what?"]).answer()` | `['World']`
 [Distance](https://github.com/artitw/text2text#levenshtein-sub-word-edit-distance) | `t2t.Handler(["Hello, World! [SEP] Hello, what?"]).measure()` | `[2]`
 [Training/Finetuning](https://github.com/artitw/text2text#training--finetuning) | `t2t.Handler(["Hello, World! [TGT] Hello, what?"]).fit()` | Finetuned model saved
 [Identification](https://github.com/artitw/text2text#identification) | `t2t.Handler(["Aj keď sa Buzz Aldrin stal až „druhým človekom“..."]).identify()` | `['sk', 'Slovak']`
 [Web Server](https://github.com/artitw/text2text#serving) | `t2t.Server(host='0.0.0.0', port=80)` | Web server started on host and port
 
 ## Languages Available
@@ -729,24 +729,21 @@
 input_state = f"{instruction} [CONTEXT] {dialog} {knowledge}"
 
 t2t.Handler([input_state]).respond()
 # ['About 60 different kinds of cats are recognized by various cat registries.']
 ```
 
 ### Assistant
-Based on LLaMA, which is not commercially licensed.
+Based on Vicuna 13B, which is based on LLaMA, which is not commercially licensed.
 ```
-instructions = """
-Generate a JSON output mapping with keys as English characters and values as Greek equivalents.
-{
-"""
+instructions = "Generate a JSON object that maps English characters as keys and Greek equivalents as values: {"
 res = t2t.Handler([instructions]).assist()
-# 1) Find an open source project that you are interested in. You can do this by searching the internet for the project name or using a search engine to find the project page on GitHub.
-# 2) Verify that you have the necessary permissions to make changes to the code. If the project uses basic permissions, you can use git to check out the code. If the code uses more advanced permissions, you can find a way to use those permissions.
-# 3) Perform a code review to ensure that your contributions are properly credits and, if necessary, include a reasoning of your changes.
+#[
+#  '{\n"a": "α",\n"b": "β",\n"c": "γ",\n"d": "δ",\n"e": "ε",\n"f": "φ",\n"g": "χ",\n"h": "ι",\n"i": "η",\n"j": "κ",\n"k": "λ",\n"l": "μ",\n"m": "ν",\n"n": "ξ",\n"o": "ο",\n"p": "π",\n"q": "ρ",\n"r": "σ",\n"s": "τ",\n"t": "υ",\n"u": "ύ",\n"v": "φ",\n"w": "χ",\n"x": "ψ",\n"y": "ω",\n"z": "ζ"\n}'
+#]
 ```
 
 ### Training / Finetuning
 Finetune cross-lingual model on your data
 ```
 result = t2t.Handler(["Hello, World! [TGT] 你好,世界!"], 
             src_lang="en",
```

### Comparing `text2text-1.0.2/setup.py` & `text2text-1.0.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="text2text",
-  version="1.0.2",
+  version="1.0.3",
   author="Artit Wangperawong",
   author_email="artitw@gmail.com",
   description="Text2Text: Crosslingual NLP/G toolkit",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/artitw/text2text",
   packages=setuptools.find_packages(),
@@ -17,14 +17,15 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
   ],
   keywords='multilingual crosslingual gpt chatgpt bert natural language processing nlp nlg text generation gpt question answer answering information retrieval tfidf tf-idf bm25 search index summary summarizer summarization tokenizer tokenization translation backtranslation data augmentation science machine learning colab embedding levenshtein sub-word edit distance conversational dialog chatbot',
   install_requires=[
     'accelerate',
+    'auto-gptq',
     'bitsandbytes',
     'peft',
     'faiss-cpu',
     'flask',
     'googledrivedownloader',
     'numpy',
     'pandas',
```

### Comparing `text2text-1.0.2/text2text/__init__.py` & `text2text-1.0.3/text2text/__init__.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.2/text2text/abstractor.py` & `text2text-1.0.3/text2text/abstractor.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.2/text2text/answerer.py` & `text2text-1.0.3/text2text/answerer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.2/text2text/assistant.py` & `text2text-1.0.3/text2text/assistant.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,48 @@
-import torch
 import text2text as t2t
-from peft import PeftModel    
-from transformers import AutoModelForCausalLM, LlamaTokenizer
+from transformers import AutoTokenizer
+from auto_gptq import AutoGPTQForCausalLM
 
 class Assistant(t2t.Transformer):
 
   def __init__(self, **kwargs):
-    model_name = "decapoda-research/llama-7b-hf"
-    adapters_name = 'timdettmers/guanaco-7b'
-    m = AutoModelForCausalLM.from_pretrained(
-        model_name,
-        #load_in_4bit=True,
-        torch_dtype=torch.bfloat16,
-        device_map={"": 0}
+    model_name_or_path = "TheBloke/vicuna-13b-v1.3-GPTQ"
+    model_basename = "vicuna-13b-v1.3-GPTQ-4bit-128g.no-act.order"
+
+    self.__class__.tokenizer = AutoTokenizer.from_pretrained(model_name_or_path, use_fast=True)
+
+    self.__class__.model = AutoGPTQForCausalLM.from_quantized(model_name_or_path,
+      model_basename=model_basename,
+      use_safetensors=True,
+      trust_remote_code=False,
+      device="cuda:0",
+      use_triton=False,
+      quantize_config=None
     )
-    m = PeftModel.from_pretrained(m, adapters_name)
-    self.__class__.model = m.merge_and_unload()
-    self.__class__.tokenizer = LlamaTokenizer.from_pretrained(model_name)
-    self.__class__.tokenizer.bos_token_id = 1
 
   def transform(self, input_lines, src_lang='en', **kwargs):
+    input_lines = [f'''USER: {prompt}\nASSISTANT:''' for prompt in input_lines]
     temperature = kwargs.get('temperature', 0.7)
     top_p = kwargs.get('top_p', 0.9)
     top_k = kwargs.get('top_k', 0)
     repetition_penalty = kwargs.get('repetition_penalty', 1.1)
-    max_new_tokens = kwargs.get('max_new_tokens', 1536)
+    max_new_tokens = kwargs.get('max_new_tokens', 512)
     tok = self.__class__.tokenizer
     m = self.__class__.model
     input_ids = tok(input_lines, return_tensors="pt").input_ids
     input_ids = input_ids.to(m.device)
     generate_kwargs = dict(
         input_ids=input_ids,
         max_new_tokens=max_new_tokens,
         temperature=temperature,
         do_sample=temperature > 0.0,
         top_p=top_p,
         top_k=top_k,
         repetition_penalty=repetition_penalty,
     )
 
-    return tok.batch_decode(m.generate(**generate_kwargs), skip_special_tokens=True) 
+    output_lines = tok.batch_decode(m.generate(**generate_kwargs)) 
+
+    for i in range(len(input_lines)):
+      output_lines[i] = output_lines[i].replace('<s>',"").replace('</s>',"").replace(input_lines[i], "").strip()
     
+    return output_lines
```

### Comparing `text2text-1.0.2/text2text/biunilm/loader_utils.py` & `text2text-1.0.3/text2text/biunilm/loader_utils.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.2/text2text/biunilm/seq2seq_loader.py` & `text2text-1.0.3/text2text/biunilm/seq2seq_loader.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.2/text2text/bm25er.py` & `text2text-1.0.3/text2text/bm25er.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.2/text2text/counter.py` & `text2text-1.0.3/text2text/counter.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.2/text2text/fitter.py` & `text2text-1.0.3/text2text/fitter.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.2/text2text/handler.py` & `text2text-1.0.3/text2text/handler.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.2/text2text/identifier.py` & `text2text-1.0.3/text2text/identifier.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.2/text2text/indexer.py` & `text2text-1.0.3/text2text/indexer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.2/text2text/measurer.py` & `text2text-1.0.3/text2text/measurer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.2/text2text/pytorch_pretrained_bert/__main__.py` & `text2text-1.0.3/text2text/pytorch_pretrained_bert/__main__.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.2/text2text/pytorch_pretrained_bert/file_utils.py` & `text2text-1.0.3/text2text/pytorch_pretrained_bert/file_utils.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.2/text2text/pytorch_pretrained_bert/loss.py` & `text2text-1.0.3/text2text/pytorch_pretrained_bert/loss.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.2/text2text/pytorch_pretrained_bert/modeling.py` & `text2text-1.0.3/text2text/pytorch_pretrained_bert/modeling.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.2/text2text/pytorch_pretrained_bert/tokenization.py` & `text2text-1.0.3/text2text/pytorch_pretrained_bert/tokenization.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.2/text2text/questioner.py` & `text2text-1.0.3/text2text/questioner.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.2/text2text/responder.py` & `text2text-1.0.3/text2text/responder.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.2/text2text/searcher.py` & `text2text-1.0.3/text2text/searcher.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.2/text2text/server.py` & `text2text-1.0.3/text2text/server.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.2/text2text/summarizer.py` & `text2text-1.0.3/text2text/summarizer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.2/text2text/tfidfer.py` & `text2text-1.0.3/text2text/tfidfer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.2/text2text/tokenizer.py` & `text2text-1.0.3/text2text/tokenizer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.2/text2text/transformer.py` & `text2text-1.0.3/text2text/transformer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.2/text2text/translator.py` & `text2text-1.0.3/text2text/translator.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.2/text2text/vectorizer.py` & `text2text-1.0.3/text2text/vectorizer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.2/text2text.egg-info/PKG-INFO` & `text2text-1.0.3/text2text.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2text
-Version: 1.0.2
+Version: 1.0.3
 Summary: Text2Text: Crosslingual NLP/G toolkit
 Home-page: https://github.com/artitw/text2text
 Author: Artit Wangperawong
 Author-email: artitw@gmail.com
 Keywords: multilingual crosslingual gpt chatgpt bert natural language processing nlp nlg text generation gpt question answer answering information retrieval tfidf tf-idf bm25 search index summary summarizer summarization tokenizer tokenization translation backtranslation data augmentation science machine learning colab embedding levenshtein sub-word edit distance conversational dialog chatbot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -93,15 +93,15 @@
 [Indexer](https://github.com/artitw/text2text#index) | `i = h.index()` | Index object for similarity retrieval
 [Search](https://github.com/artitw/text2text#search) | `h.search(queries=["Hello"])` | `array([[0.09]])`
 [Translation](https://github.com/artitw/text2text#translation) | `h.translate(tgt_lang="zh")` | `['你好,世界!']`
 [Question Generation](https://github.com/artitw/text2text#question-generation) | `h.question()` | `[('What is the name of the world you are in?', 'The world')]`
 [Summarization](https://github.com/artitw/text2text#summarization) | `h.summarize()` | `["World ' s largest world"]`
 [Data Augmentation](https://github.com/artitw/text2text#data-augmentation--back-translation) | `h.variate()` | `['Hello the world!', 'Welcome to the world.', 'Hello to the world!',...`
 [Dialog Response](https://github.com/artitw/text2text#dialog-responder) | `t2t.Handler(["[CONTEXT] Hello EOS How are you?"]).respond()` | `['I am doing great. How are you?']`
-[Assistant](https://github.com/artitw/text2text#assistant) | `t2t.Handler(["Explain Text2Text in one sentence"]).assist()` | `['Text to text translation uses a deep learning model to generate a text in another language from a given source text.']`
+[Assistant](https://github.com/artitw/text2text#assistant) | `t2t.Handler(["Describe Text2Text in a few words: "]).assist()` | `['Text2Text is an AI-powered text generation tool that creates coherent and continuous text based on prompts.']`
 [Question Answering](https://github.com/artitw/text2text#question-answering) | `t2t.Handler(["Hello, World! [SEP] Hello, what?"]).answer()` | `['World']`
 [Distance](https://github.com/artitw/text2text#levenshtein-sub-word-edit-distance) | `t2t.Handler(["Hello, World! [SEP] Hello, what?"]).measure()` | `[2]`
 [Training/Finetuning](https://github.com/artitw/text2text#training--finetuning) | `t2t.Handler(["Hello, World! [TGT] Hello, what?"]).fit()` | Finetuned model saved
 [Identification](https://github.com/artitw/text2text#identification) | `t2t.Handler(["Aj keď sa Buzz Aldrin stal až „druhým človekom“..."]).identify()` | `['sk', 'Slovak']`
 [Web Server](https://github.com/artitw/text2text#serving) | `t2t.Server(host='0.0.0.0', port=80)` | Web server started on host and port
 
 ## Languages Available
@@ -743,24 +743,21 @@
 input_state = f"{instruction} [CONTEXT] {dialog} {knowledge}"
 
 t2t.Handler([input_state]).respond()
 # ['About 60 different kinds of cats are recognized by various cat registries.']
 ```
 
 ### Assistant
-Based on LLaMA, which is not commercially licensed.
+Based on Vicuna 13B, which is based on LLaMA, which is not commercially licensed.
 ```
-instructions = """
-Generate a JSON output mapping with keys as English characters and values as Greek equivalents.
-{
-"""
+instructions = "Generate a JSON object that maps English characters as keys and Greek equivalents as values: {"
 res = t2t.Handler([instructions]).assist()
-# 1) Find an open source project that you are interested in. You can do this by searching the internet for the project name or using a search engine to find the project page on GitHub.
-# 2) Verify that you have the necessary permissions to make changes to the code. If the project uses basic permissions, you can use git to check out the code. If the code uses more advanced permissions, you can find a way to use those permissions.
-# 3) Perform a code review to ensure that your contributions are properly credits and, if necessary, include a reasoning of your changes.
+#[
+#  '{\n"a": "α",\n"b": "β",\n"c": "γ",\n"d": "δ",\n"e": "ε",\n"f": "φ",\n"g": "χ",\n"h": "ι",\n"i": "η",\n"j": "κ",\n"k": "λ",\n"l": "μ",\n"m": "ν",\n"n": "ξ",\n"o": "ο",\n"p": "π",\n"q": "ρ",\n"r": "σ",\n"s": "τ",\n"t": "υ",\n"u": "ύ",\n"v": "φ",\n"w": "χ",\n"x": "ψ",\n"y": "ω",\n"z": "ζ"\n}'
+#]
 ```
 
 ### Training / Finetuning
 Finetune cross-lingual model on your data
 ```
 result = t2t.Handler(["Hello, World! [TGT] 你好,世界!"], 
             src_lang="en",
```

### Comparing `text2text-1.0.2/text2text.egg-info/SOURCES.txt` & `text2text-1.0.3/text2text.egg-info/SOURCES.txt`

 * *Files identical despite different names*

