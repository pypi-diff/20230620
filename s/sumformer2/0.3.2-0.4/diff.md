# Comparing `tmp/sumformer2-0.3.2.tar.gz` & `tmp/sumformer2-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sumformer2-0.3.2.tar", last modified: Sun Jun 18 17:35:52 2023, max compression
+gzip compressed data, was "sumformer2-0.4.tar", last modified: Tue Jun 20 10:41:53 2023, max compression
```

## Comparing `sumformer2-0.3.2.tar` & `sumformer2-0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-06-18 17:35:52.988746 sumformer2-0.3.2/
--rw-r--r--   0 ryan       (501) staff       (20)     1065 2023-06-07 16:24:08.000000 sumformer2-0.3.2/LICENSE
--rw-r--r--   0 ryan       (501) staff       (20)      212 2023-06-18 17:35:52.988103 sumformer2-0.3.2/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)       61 2023-06-07 16:24:08.000000 sumformer2-0.3.2/README.md
--rw-r--r--   0 ryan       (501) staff       (20)       38 2023-06-18 17:35:52.988980 sumformer2-0.3.2/setup.cfg
--rw-r--r--   0 ryan       (501) staff       (20)      492 2023-06-18 17:35:39.000000 sumformer2-0.3.2/setup.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-06-18 17:35:52.983643 sumformer2-0.3.2/sumformer2/
--rw-r--r--   0 ryan       (501) staff       (20)        0 2023-06-18 10:03:46.000000 sumformer2-0.3.2/sumformer2/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)    14680 2023-06-18 17:19:05.000000 sumformer2-0.3.2/sumformer2/main.py
--rw-r--r--   0 ryan       (501) staff       (20)     8921 2023-06-18 14:27:38.000000 sumformer2-0.3.2/sumformer2/modules.py
--rw-r--r--   0 ryan       (501) staff       (20)     5889 2023-06-18 14:29:22.000000 sumformer2-0.3.2/sumformer2/transformer.py
--rw-r--r--   0 ryan       (501) staff       (20)     5820 2023-06-18 17:10:08.000000 sumformer2-0.3.2/sumformer2/utils.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-06-18 17:35:52.987219 sumformer2-0.3.2/sumformer2.egg-info/
--rw-r--r--   0 ryan       (501) staff       (20)      212 2023-06-18 17:35:52.000000 sumformer2-0.3.2/sumformer2.egg-info/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)      342 2023-06-18 17:35:52.000000 sumformer2-0.3.2/sumformer2.egg-info/SOURCES.txt
--rw-r--r--   0 ryan       (501) staff       (20)        1 2023-06-18 17:35:52.000000 sumformer2-0.3.2/sumformer2.egg-info/dependency_links.txt
--rw-r--r--   0 ryan       (501) staff       (20)       53 2023-06-18 17:35:52.000000 sumformer2-0.3.2/sumformer2.egg-info/entry_points.txt
--rw-r--r--   0 ryan       (501) staff       (20)     1459 2023-06-18 17:35:52.000000 sumformer2-0.3.2/sumformer2.egg-info/requires.txt
--rw-r--r--   0 ryan       (501) staff       (20)       11 2023-06-18 17:35:52.000000 sumformer2-0.3.2/sumformer2.egg-info/top_level.txt
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-06-20 10:41:53.474206 sumformer2-0.4/
+-rw-r--r--   0 ryan       (501) staff       (20)     1065 2023-06-07 16:24:08.000000 sumformer2-0.4/LICENSE
+-rw-r--r--   0 ryan       (501) staff       (20)      210 2023-06-20 10:41:53.473703 sumformer2-0.4/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)       61 2023-06-07 16:24:08.000000 sumformer2-0.4/README.md
+-rw-r--r--   0 ryan       (501) staff       (20)       38 2023-06-20 10:41:53.474398 sumformer2-0.4/setup.cfg
+-rw-r--r--   0 ryan       (501) staff       (20)      490 2023-06-20 10:41:25.000000 sumformer2-0.4/setup.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-06-20 10:41:53.469984 sumformer2-0.4/sumformer2/
+-rw-r--r--   0 ryan       (501) staff       (20)        0 2023-06-18 10:03:46.000000 sumformer2-0.4/sumformer2/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)    16927 2023-06-20 10:35:09.000000 sumformer2-0.4/sumformer2/main.py
+-rw-r--r--   0 ryan       (501) staff       (20)     8921 2023-06-18 14:27:38.000000 sumformer2-0.4/sumformer2/modules.py
+-rw-r--r--   0 ryan       (501) staff       (20)     5919 2023-06-20 09:07:09.000000 sumformer2-0.4/sumformer2/transformer.py
+-rw-r--r--   0 ryan       (501) staff       (20)     6237 2023-06-20 10:37:03.000000 sumformer2-0.4/sumformer2/utils.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-06-20 10:41:53.472979 sumformer2-0.4/sumformer2.egg-info/
+-rw-r--r--   0 ryan       (501) staff       (20)      210 2023-06-20 10:41:53.000000 sumformer2-0.4/sumformer2.egg-info/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)      342 2023-06-20 10:41:53.000000 sumformer2-0.4/sumformer2.egg-info/SOURCES.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        1 2023-06-20 10:41:53.000000 sumformer2-0.4/sumformer2.egg-info/dependency_links.txt
+-rw-r--r--   0 ryan       (501) staff       (20)       53 2023-06-20 10:41:53.000000 sumformer2-0.4/sumformer2.egg-info/entry_points.txt
+-rw-r--r--   0 ryan       (501) staff       (20)     1459 2023-06-20 10:41:53.000000 sumformer2-0.4/sumformer2.egg-info/requires.txt
+-rw-r--r--   0 ryan       (501) staff       (20)       11 2023-06-20 10:41:53.000000 sumformer2-0.4/sumformer2.egg-info/top_level.txt
```

### Comparing `sumformer2-0.3.2/LICENSE` & `sumformer2-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sumformer2-0.3.2/sumformer2/main.py` & `sumformer2-0.4/sumformer2/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 import random
+import re
 import time
 import fire
 import numpy as np
 import torch
 import wandb
 
 from bert_score import BERTScorer
 from rouge import Rouge
 from torch.cuda.amp import autocast, GradScaler
 from torch.nn.functional import pad
 from torch.optim import AdamW
-from transformers import T5Tokenizer
+from transformers import T5Tokenizer, T5ForConditionalGeneration
 
 from .transformer import Sumformer
 from .utils import *
 
 
 INTERVAL = 100  # Init logging interval
 MIN_INPUT_LEN = 50
 MAX_INPUT_LEN = 512
+device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
 
 
 def main(train=True, test=False, epochs=6, batch_size=24, lr=3.4e-4, sched="onecycle", emb_dim=512, max_out_len=30, clip=0.0, sample=None, load=None, pos_enc=False, GLU=False, norm="post", gen="greedy", ignore_pad=False,
          enc_heads=8, enc_hidden=6, enc_depth=8, enc_dropout=0.3,
-         dec_heads=8, dec_hidden=6, dec_depth=8, dec_dropout=0.3):
+         dec_heads=8, dec_hidden=6, dec_depth=8, dec_dropout=0.3,
+         test_model_path=None, baseline=False):
     # Ensure deterministic behavior
     set_seed(69420)
 
     best_val_loss = float("inf")  # Init best loss
     best_val_model_path = None
     best_model = None
     running_time = 0.0  # Init throughput measurements
@@ -71,15 +74,15 @@
         test_dataset = test_dataset.select(range(sample))
     print("Number of rows: ", len(train_dataset))
 
     # Init the T5 tokenizer
     tokenizer = setup_tokenizer()
 
     def collate_fn(batch):
-        docs = [item['document'] for item in batch]
+        docs = ["summarize: " + item['document'] for item in batch]
         summaries = [item['summary'] for item in batch]
 
         # encode, truncate and pad to the length of the longest sequence in the batch
         encoder_inputs = tokenizer(docs, truncation=True, padding='longest', return_tensors='pt')
         decoder_inputs = tokenizer(summaries, truncation=True, padding='longest', return_tensors='pt')
 
         # TODO: Pad manually cause this doesn't seem to work
@@ -232,32 +235,72 @@
     # -----TESTING-----
     if test:
         print("Testing...")
 
         rouge = Rouge()
         bert_score = BERTScorer(lang="en")
 
+        # Load the model
+        if baseline:
+            print("Testing with T5 as a baseline...")
+            tokenizer = T5Tokenizer.from_pretrained("t5-base")
+            test_model = T5ForConditionalGeneration.from_pretrained("t5-base").to(device)
+        else:
+            print(f"Testing with the {test_model_path} model...")
+            test_model_info = torch.load(test_model_path, map_location=device)
+            test_model = Sumformer(**test_model_info["params"]).to(device)
+
         # Generate summaries for the test set and compare them to the reference summaries
         with torch.no_grad():
-            best_model.eval()
+            test_model.eval()
             all_generated_summaries = []
             all_reference_summaries = []
             for b_idx, (encoder_inputs, decoder_inputs) in enumerate(test_loader):
-                generated_outputs = best_model.greedy(encoder_inputs["input_ids"], start_token=tokenizer.bos_token_id, end_token=tokenizer.eos_token_id, max_len=max_out_len)
+                print("Batch: ", b_idx)
+                if baseline:
+                    # For T5, generate predictions using its internal generation method
+                    generated_outputs = test_model.generate(
+                        input_ids=encoder_inputs["input_ids"].to(device),
+                        attention_mask=encoder_inputs["attention_mask"].to(device),
+                        max_length=max_out_len,
+                        num_beams=2
+                    )
+                else:
+                    generated_outputs = test_model.greedy(encoder_inputs["input_ids"], start_token=tokenizer.bos_token_id, end_token=tokenizer.eos_token_id, max_len=max_out_len)
                 generated_summaries = [tokenizer.decode(g, skip_special_tokens=True) for g in generated_outputs]
                 reference_summaries = [tokenizer.decode(d, skip_special_tokens=True) for d in decoder_inputs["input_ids"]]
                 all_generated_summaries.extend(generated_summaries)
                 all_reference_summaries.extend(reference_summaries)
+        
+        # # After generating summaries
+        # for idx, (gen_summary, ref_summary) in enumerate(zip(all_generated_summaries, all_reference_summaries)):
+        #     print(f"Summary index {idx}:")
+        #     print(f"Generated: {gen_summary}")
+        #     print(f"Reference: {ref_summary}")
+        #     print("--------------------")
+
+        # # Print an example generated summary and its reference summary
+        # print(f"Example generated summary: {all_generated_summaries[5]}")
+        # print(f"Example reference summary: {all_reference_summaries[5]}")
+
+        # Function to determine if a summary is "empty"
+        def is_empty(summary):
+            # A summary is "empty" if it contains only whitespace or non-alphanumeric characters
+            return re.match("^\W*$", summary) is not None
+
+        # Filter out pairs of summaries where either the generated or reference summary is "empty"
+        filtered_generated_summaries = []
+        filtered_reference_summaries = []
+        for gen_summary, ref_summary in zip(all_generated_summaries, all_reference_summaries):
+            if not is_empty(gen_summary) and not is_empty(ref_summary):
+                filtered_generated_summaries.append(gen_summary)
+                filtered_reference_summaries.append(ref_summary)
 
-        # Print an example generated summary and its reference summary
-        print(f"Example generated summary: {all_generated_summaries[5]}")
-        print(f"Example reference summary: {all_reference_summaries[5]}")
-
-        # Calculate and print the Rouge scores
-        rouge_scores = rouge.get_scores(all_generated_summaries, all_reference_summaries, avg=True)
+        # Now calculate ROUGE scores
+        rouge_scores = rouge.get_scores(filtered_generated_summaries, filtered_reference_summaries, avg=True)
         for metric, score_dict in rouge_scores.items():
             f1_score = score_dict['f']
             wandb.log({f"{metric} F1 Score": f1_score})
 
         # Print F1 rouge_scores nicely
         for metric, score_dict in rouge_scores.items():
             f1_score = score_dict['f']
```

### Comparing `sumformer2-0.3.2/sumformer2/modules.py` & `sumformer2-0.4/sumformer2/modules.py`

 * *Files identical despite different names*

### Comparing `sumformer2-0.3.2/sumformer2/transformer.py` & `sumformer2-0.4/sumformer2/transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 
         self.token_embedding = nn.Embedding(num_embeddings=vocab_size, embedding_dim=emb_dim).to(device)
         if pos_encoding:
             self.pos_embedding = self.compute_encodings(max_len, emb_dim).to(device)
         else:
             self.pos_embedding = nn.Embedding(num_embeddings=max_len, embedding_dim=emb_dim).to(device)
 
-        self.encoder = [EncoderBlock(emb_dim, enc_heads, enc_hidden, enc_dropout, GLU, norm) for _ in range(enc_depth)]
+        self.encoder = nn.ModuleList([EncoderBlock(emb_dim, enc_heads, enc_hidden, enc_dropout, GLU, norm) for _ in range(enc_depth)])
         for module in self.encoder: module.to(device)
-        self.decoder = [DecoderBlock(emb_dim, dec_heads, dec_hidden, dec_dropout, GLU, norm) for _ in range(dec_depth)]
+        self.decoder = nn.ModuleList([DecoderBlock(emb_dim, dec_heads, dec_hidden, dec_dropout, GLU, norm) for _ in range(dec_depth)])
         for module in self.decoder: module.to(device)
 
         self.toProbs = nn.Linear(emb_dim, vocab_size).to(device)  # convert to probabilities over vocab
 
     def compute_encodings(self, max_len, emb_dim):
         """Initialise positional encodings."""
         pos_encodings = torch.zeros(max_len, emb_dim).float()
```

### Comparing `sumformer2-0.3.2/sumformer2/utils.py` & `sumformer2-0.4/sumformer2/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,19 @@
 
 def load_xsum():
     """Load the XSum dataset and split into train, validation, and test sets. Keep only the docs and their summary."""
     train_dataset = load_dataset("xsum", split="train")
     val_dataset = load_dataset("xsum", split="validation")
     test_dataset = load_dataset("xsum", split="test")
 
+    # Filter out columns with empty documents or summaries
+    train_dataset = train_dataset.filter(lambda x: len(x['summary']) > 0 and len(x['document']) > 1.5*len(x['summary']))
+    val_dataset = val_dataset.filter(lambda x: len(x['summary']) > 0 and len(x['document']) > 1.5*len(x['summary']))
+    test_dataset = test_dataset.filter(lambda x: len(x['summary']) > 0 and len(x['document']) > 1.5*len(x['summary']))
+
     # Adding a the doc length of each instance
     train_dataset = train_dataset.map(lambda x: {'doc_len': len(x['document'])})
     val_dataset = val_dataset.map(lambda x: {'doc_len': len(x['document'])})
     test_dataset = test_dataset.map(lambda x: {'doc_len': len(x['document'])})
 
     # Sort the datasets by document length
     train_dataset = train_dataset.sort('doc_len')
```

### Comparing `sumformer2-0.3.2/sumformer2.egg-info/requires.txt` & `sumformer2-0.4/sumformer2.egg-info/requires.txt`

 * *Files identical despite different names*

