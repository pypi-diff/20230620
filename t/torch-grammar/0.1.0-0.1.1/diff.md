# Comparing `tmp/torch_grammar-0.1.0.tar.gz` & `tmp/torch_grammar-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_grammar-0.1.0.tar", max compression
+gzip compressed data, was "torch_grammar-0.1.1.tar", max compression
```

## Comparing `torch_grammar-0.1.0.tar` & `torch_grammar-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1855 2023-06-19 17:40:11.452792 torch_grammar-0.1.0/README.md
--rw-r--r--   0        0        0      643 2023-06-20 18:48:47.928565 torch_grammar-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       74 2023-06-19 15:27:17.327365 torch_grammar-0.1.0/torch_grammar/__init__.py
--rw-r--r--   0        0        0     9709 2023-06-19 17:39:52.938166 torch_grammar-0.1.0/torch_grammar/grammar_parser.py
--rw-r--r--   0        0        0     6435 2023-06-20 18:49:37.212473 torch_grammar-0.1.0/torch_grammar/grammar_sampler.py
--rw-r--r--   0        0        0     1208 2023-06-19 17:20:35.685343 torch_grammar-0.1.0/torch_grammar/token_trie.py
--rw-r--r--   0        0        0     2497 1970-01-01 00:00:00.000000 torch_grammar-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1916 2023-06-20 18:58:30.304068 torch_grammar-0.1.1/README.md
+-rw-r--r--   0        0        0      643 2023-06-20 18:58:38.653428 torch_grammar-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       74 2023-06-19 15:27:17.327365 torch_grammar-0.1.1/torch_grammar/__init__.py
+-rw-r--r--   0        0        0     9709 2023-06-19 17:39:52.938166 torch_grammar-0.1.1/torch_grammar/grammar_parser.py
+-rw-r--r--   0        0        0     6435 2023-06-20 18:49:37.212473 torch_grammar-0.1.1/torch_grammar/grammar_sampler.py
+-rw-r--r--   0        0        0     1208 2023-06-19 17:20:35.685343 torch_grammar-0.1.1/torch_grammar/token_trie.py
+-rw-r--r--   0        0        0     2558 1970-01-01 00:00:00.000000 torch_grammar-0.1.1/PKG-INFO
```

### Comparing `torch_grammar-0.1.0/README.md` & `torch_grammar-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 # torch-grammar
 
-**Work in Progress: This won't actually do what you want yet unless you really
-want to get your hands dirty.**
+**Alpha Quality: This might do what you want. It's likely to not do what you
+want. Please open issues!**
 
 Torch-Grammar restricts a model to output a token sequence that conforms to a
 provided EBNF grammar.
 
 For example:
 
 ```python
+import torch
+from torch_grammar import GrammarSampler
+from transformers import LlamaTokenizer
+tokenizer = LlamaTokenizer.from_pretrained("huggyllama/llama-7b")
 
-from transformers import LLaMATokenizer
-tokenizer = LLaMATokenizer.from_pretrained("huggyllama/llama-7b")
-
-with open("grammar.ebnf", "r") as file:
+with open("examples/grammar.ebnf", "r") as file:
     input_text = file.read()
 grammar = GrammarSampler(input_text, "root", tokenizer)
 
+ids = [[1]]
 logits_processor = grammar.logits_processor()
 
 for i in range(10):
-    logits = torch.randn((1,tokenizer.vocab_size))
-    logits = logits_processor(ids, logits)
-    token = torch.argmax(logits).item()
-    logits_processor.accept_token(token)
-    ids[0].append(token)
+  logits = torch.randn((1, tokenizer.vocab_size))
+  logits = logits_processor(ids, logits)
+  token = torch.argmax(logits).item()
+  # logits_processor.accept_token(token)
+  ids[0].append(token)
 print(f"\x1b[1mfirst 10 tokens: \x1b[1;35m{tokenizer.decode(ids[0])}\x1b[0m")
 ```
 
 `logits_processor` is meant to be passed to `model.generate` in a HuggingFace
 transformers model but this integration is not yet super clean. Take a look at
 the notebook in this repo for more info.
```

### Comparing `torch_grammar-0.1.0/pyproject.toml` & `torch_grammar-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "torch-grammar"
-version = "0.1.0"
+version = "0.1.1"
 description = "Restrict LLM generations to a context-free grammar"
 authors = ["Burke Libbey <burke.libbey@shopify.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "torch_grammar"}]
 
 [tool.poetry.dependencies]
```

### Comparing `torch_grammar-0.1.0/torch_grammar/grammar_parser.py` & `torch_grammar-0.1.1/torch_grammar/grammar_parser.py`

 * *Files identical despite different names*

### Comparing `torch_grammar-0.1.0/torch_grammar/grammar_sampler.py` & `torch_grammar-0.1.1/torch_grammar/grammar_sampler.py`

 * *Files identical despite different names*

### Comparing `torch_grammar-0.1.0/torch_grammar/token_trie.py` & `torch_grammar-0.1.1/torch_grammar/token_trie.py`

 * *Files identical despite different names*

### Comparing `torch_grammar-0.1.0/PKG-INFO` & `torch_grammar-0.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-grammar
-Version: 0.1.0
+Version: 0.1.1
 Summary: Restrict LLM generations to a context-free grammar
 License: MIT
 Author: Burke Libbey
 Author-email: burke.libbey@shopify.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -14,39 +14,41 @@
 Requires-Dist: sentencepiece (>=0.1.99,<0.2.0)
 Requires-Dist: torch (>=2.0.1,<3.0.0)
 Requires-Dist: transformers (>=4.30.2,<5.0.0)
 Description-Content-Type: text/markdown
 
 # torch-grammar
 
-**Work in Progress: This won't actually do what you want yet unless you really
-want to get your hands dirty.**
+**Alpha Quality: This might do what you want. It's likely to not do what you
+want. Please open issues!**
 
 Torch-Grammar restricts a model to output a token sequence that conforms to a
 provided EBNF grammar.
 
 For example:
 
 ```python
+import torch
+from torch_grammar import GrammarSampler
+from transformers import LlamaTokenizer
+tokenizer = LlamaTokenizer.from_pretrained("huggyllama/llama-7b")
 
-from transformers import LLaMATokenizer
-tokenizer = LLaMATokenizer.from_pretrained("huggyllama/llama-7b")
-
-with open("grammar.ebnf", "r") as file:
+with open("examples/grammar.ebnf", "r") as file:
     input_text = file.read()
 grammar = GrammarSampler(input_text, "root", tokenizer)
 
+ids = [[1]]
 logits_processor = grammar.logits_processor()
 
 for i in range(10):
-    logits = torch.randn((1,tokenizer.vocab_size))
-    logits = logits_processor(ids, logits)
-    token = torch.argmax(logits).item()
-    logits_processor.accept_token(token)
-    ids[0].append(token)
+  logits = torch.randn((1, tokenizer.vocab_size))
+  logits = logits_processor(ids, logits)
+  token = torch.argmax(logits).item()
+  # logits_processor.accept_token(token)
+  ids[0].append(token)
 print(f"\x1b[1mfirst 10 tokens: \x1b[1;35m{tokenizer.decode(ids[0])}\x1b[0m")
 ```
 
 `logits_processor` is meant to be passed to `model.generate` in a HuggingFace
 transformers model but this integration is not yet super clean. Take a look at
 the notebook in this repo for more info.
```

