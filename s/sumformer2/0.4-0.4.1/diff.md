# Comparing `tmp/sumformer2-0.4.tar.gz` & `tmp/sumformer2-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sumformer2-0.4.tar", last modified: Tue Jun 20 10:41:53 2023, max compression
+gzip compressed data, was "sumformer2-0.4.1.tar", last modified: Tue Jun 20 18:03:56 2023, max compression
```

## Comparing `sumformer2-0.4.tar` & `sumformer2-0.4.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-06-20 10:41:53.474206 sumformer2-0.4/
--rw-r--r--   0 ryan       (501) staff       (20)     1065 2023-06-07 16:24:08.000000 sumformer2-0.4/LICENSE
--rw-r--r--   0 ryan       (501) staff       (20)      210 2023-06-20 10:41:53.473703 sumformer2-0.4/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)       61 2023-06-07 16:24:08.000000 sumformer2-0.4/README.md
--rw-r--r--   0 ryan       (501) staff       (20)       38 2023-06-20 10:41:53.474398 sumformer2-0.4/setup.cfg
--rw-r--r--   0 ryan       (501) staff       (20)      490 2023-06-20 10:41:25.000000 sumformer2-0.4/setup.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-06-20 10:41:53.469984 sumformer2-0.4/sumformer2/
--rw-r--r--   0 ryan       (501) staff       (20)        0 2023-06-18 10:03:46.000000 sumformer2-0.4/sumformer2/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)    16927 2023-06-20 10:35:09.000000 sumformer2-0.4/sumformer2/main.py
--rw-r--r--   0 ryan       (501) staff       (20)     8921 2023-06-18 14:27:38.000000 sumformer2-0.4/sumformer2/modules.py
--rw-r--r--   0 ryan       (501) staff       (20)     5919 2023-06-20 09:07:09.000000 sumformer2-0.4/sumformer2/transformer.py
--rw-r--r--   0 ryan       (501) staff       (20)     6237 2023-06-20 10:37:03.000000 sumformer2-0.4/sumformer2/utils.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-06-20 10:41:53.472979 sumformer2-0.4/sumformer2.egg-info/
--rw-r--r--   0 ryan       (501) staff       (20)      210 2023-06-20 10:41:53.000000 sumformer2-0.4/sumformer2.egg-info/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)      342 2023-06-20 10:41:53.000000 sumformer2-0.4/sumformer2.egg-info/SOURCES.txt
--rw-r--r--   0 ryan       (501) staff       (20)        1 2023-06-20 10:41:53.000000 sumformer2-0.4/sumformer2.egg-info/dependency_links.txt
--rw-r--r--   0 ryan       (501) staff       (20)       53 2023-06-20 10:41:53.000000 sumformer2-0.4/sumformer2.egg-info/entry_points.txt
--rw-r--r--   0 ryan       (501) staff       (20)     1459 2023-06-20 10:41:53.000000 sumformer2-0.4/sumformer2.egg-info/requires.txt
--rw-r--r--   0 ryan       (501) staff       (20)       11 2023-06-20 10:41:53.000000 sumformer2-0.4/sumformer2.egg-info/top_level.txt
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-06-20 18:03:56.259513 sumformer2-0.4.1/
+-rw-r--r--   0 ryan       (501) staff       (20)     1065 2023-06-07 16:24:08.000000 sumformer2-0.4.1/LICENSE
+-rw-r--r--   0 ryan       (501) staff       (20)      212 2023-06-20 18:03:56.259171 sumformer2-0.4.1/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)       61 2023-06-07 16:24:08.000000 sumformer2-0.4.1/README.md
+-rw-r--r--   0 ryan       (501) staff       (20)       38 2023-06-20 18:03:56.259643 sumformer2-0.4.1/setup.cfg
+-rw-r--r--   0 ryan       (501) staff       (20)      492 2023-06-20 18:03:17.000000 sumformer2-0.4.1/setup.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-06-20 18:03:56.255576 sumformer2-0.4.1/sumformer2/
+-rw-r--r--   0 ryan       (501) staff       (20)        0 2023-06-18 10:03:46.000000 sumformer2-0.4.1/sumformer2/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)    16788 2023-06-20 18:02:54.000000 sumformer2-0.4.1/sumformer2/main.py
+-rw-r--r--   0 ryan       (501) staff       (20)     8921 2023-06-18 14:27:38.000000 sumformer2-0.4.1/sumformer2/modules.py
+-rw-r--r--   0 ryan       (501) staff       (20)     6177 2023-06-20 17:43:41.000000 sumformer2-0.4.1/sumformer2/transformer.py
+-rw-r--r--   0 ryan       (501) staff       (20)     6237 2023-06-20 10:37:03.000000 sumformer2-0.4.1/sumformer2/utils.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-06-20 18:03:56.258578 sumformer2-0.4.1/sumformer2.egg-info/
+-rw-r--r--   0 ryan       (501) staff       (20)      212 2023-06-20 18:03:56.000000 sumformer2-0.4.1/sumformer2.egg-info/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)      342 2023-06-20 18:03:56.000000 sumformer2-0.4.1/sumformer2.egg-info/SOURCES.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        1 2023-06-20 18:03:56.000000 sumformer2-0.4.1/sumformer2.egg-info/dependency_links.txt
+-rw-r--r--   0 ryan       (501) staff       (20)       53 2023-06-20 18:03:56.000000 sumformer2-0.4.1/sumformer2.egg-info/entry_points.txt
+-rw-r--r--   0 ryan       (501) staff       (20)     1459 2023-06-20 18:03:56.000000 sumformer2-0.4.1/sumformer2.egg-info/requires.txt
+-rw-r--r--   0 ryan       (501) staff       (20)       11 2023-06-20 18:03:56.000000 sumformer2-0.4.1/sumformer2.egg-info/top_level.txt
```

### Comparing `sumformer2-0.4/LICENSE` & `sumformer2-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sumformer2-0.4/sumformer2/main.py` & `sumformer2-0.4.1/sumformer2/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 INTERVAL = 100  # Init logging interval
 MIN_INPUT_LEN = 50
 MAX_INPUT_LEN = 512
 device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
 
 
-def main(train=True, test=False, epochs=6, batch_size=24, lr=3.4e-4, sched="onecycle", emb_dim=512, max_out_len=30, clip=0.0, sample=None, load=None, pos_enc=False, GLU=False, norm="post", gen="greedy", ignore_pad=False,
+def main(train=True, test=False, epochs=6, batch_size=24, lr=3.4e-4, sched="onecycle", emb_dim=512, max_out_len=30, clip=0.0, sample=None, load=None, pos_enc=False, GLU=False, norm="post", checkpoint=False, gen="greedy", ignore_pad=True,
          enc_heads=8, enc_hidden=6, enc_depth=8, enc_dropout=0.3,
          dec_heads=8, dec_hidden=6, dec_depth=8, dec_dropout=0.3,
          test_model_path=None, baseline=False):
     # Ensure deterministic behavior
     set_seed(69420)
 
     best_val_loss = float("inf")  # Init best loss
@@ -96,15 +96,15 @@
     train_loader = create_data_loader(train_dataset, batch_size, collate_fn)
     val_loader = create_data_loader(val_dataset, batch_size, collate_fn)
     test_loader = create_data_loader(test_dataset, batch_size, collate_fn)
 
     scaler = GradScaler()  # Init gradient scaler for mixed precision training
 
     if train:
-        model = Sumformer(device, emb_dim, len(tokenizer.get_vocab()), max(MAX_INPUT_LEN, max_out_len), pos_enc, GLU, norm, enc_heads, enc_hidden, enc_depth, enc_dropout, dec_heads, dec_hidden, dec_depth, dec_dropout).to(device)
+        model = Sumformer(device, emb_dim, len(tokenizer.get_vocab()), max(MAX_INPUT_LEN, max_out_len), pos_enc, GLU, norm, checkpoint, enc_heads, enc_hidden, enc_depth, enc_dropout, dec_heads, dec_hidden, dec_depth, dec_dropout).to(device)
         optimizer = AdamW(model.parameters(), lr)
         criterion = torch.nn.CrossEntropyLoss(ignore_index=tokenizer.pad_token_id if ignore_pad else -100, reduction='mean')  # * see without padding mask in decoder
         scheduler = init_schedule(optimizer, sched, train_loader, lr, epochs, emb_dim)
 
         for epoch in range(epochs):
             # torch.autograd.set_detect_anomaly(True)  # ! REMOVE WHEN NOT NEEDED
             # -----TRAINING-----
@@ -216,14 +216,15 @@
                     'device': device,
                     'emb_dim': emb_dim,
                     'vocab_size': tokenizer.vocab_size,
                     'max_len': max(MAX_INPUT_LEN, max_out_len),
                     'pos_encoding': pos_enc,
                     'GLU': GLU,
                     'norm': norm,
+
                     'enc_heads': enc_heads,
                     'enc_hidden': enc_hidden,
                     'enc_depth': enc_depth,
                     'enc_dropout': enc_dropout,
                     'dec_heads': dec_heads,
                     'dec_hidden': dec_hidden,
                     'dec_depth': dec_depth,
@@ -241,25 +242,29 @@
 
         # Load the model
         if baseline:
             print("Testing with T5 as a baseline...")
             tokenizer = T5Tokenizer.from_pretrained("t5-base")
             test_model = T5ForConditionalGeneration.from_pretrained("t5-base").to(device)
         else:
-            print(f"Testing with the {test_model_path} model...")
-            test_model_info = torch.load(test_model_path, map_location=device)
-            test_model = Sumformer(**test_model_info["params"]).to(device)
+            if test_model_path is None:
+                print("Testing with the eval best model...")
+                test_model = best_model
+            else:
+                print(f"Testing with the {test_model_path} model...")
+                test_model_info = torch.load(test_model_path, map_location=device)
+                test_model = Sumformer(**test_model_info["params"]).to(device)
 
         # Generate summaries for the test set and compare them to the reference summaries
         with torch.no_grad():
             test_model.eval()
             all_generated_summaries = []
             all_reference_summaries = []
             for b_idx, (encoder_inputs, decoder_inputs) in enumerate(test_loader):
-                print("Batch: ", b_idx)
+                print("Testing Batch: ", b_idx)
                 if baseline:
                     # For T5, generate predictions using its internal generation method
                     generated_outputs = test_model.generate(
                         input_ids=encoder_inputs["input_ids"].to(device),
                         attention_mask=encoder_inputs["attention_mask"].to(device),
                         max_length=max_out_len,
                         num_beams=2
@@ -267,24 +272,17 @@
                 else:
                     generated_outputs = test_model.greedy(encoder_inputs["input_ids"], start_token=tokenizer.bos_token_id, end_token=tokenizer.eos_token_id, max_len=max_out_len)
                 generated_summaries = [tokenizer.decode(g, skip_special_tokens=True) for g in generated_outputs]
                 reference_summaries = [tokenizer.decode(d, skip_special_tokens=True) for d in decoder_inputs["input_ids"]]
                 all_generated_summaries.extend(generated_summaries)
                 all_reference_summaries.extend(reference_summaries)
         
-        # # After generating summaries
-        # for idx, (gen_summary, ref_summary) in enumerate(zip(all_generated_summaries, all_reference_summaries)):
-        #     print(f"Summary index {idx}:")
-        #     print(f"Generated: {gen_summary}")
-        #     print(f"Reference: {ref_summary}")
-        #     print("--------------------")
-
-        # # Print an example generated summary and its reference summary
-        # print(f"Example generated summary: {all_generated_summaries[5]}")
-        # print(f"Example reference summary: {all_reference_summaries[5]}")
+        # Print an example generated summary and its reference summary
+        print(f"Example generated summary: {all_generated_summaries[0]}")
+        print(f"Example reference summary: {all_reference_summaries[0]}")
 
         # Function to determine if a summary is "empty"
         def is_empty(summary):
             # A summary is "empty" if it contains only whitespace or non-alphanumeric characters
             return re.match("^\W*$", summary) is not None
 
         # Filter out pairs of summaries where either the generated or reference summary is "empty"
```

### Comparing `sumformer2-0.4/sumformer2/modules.py` & `sumformer2-0.4.1/sumformer2/modules.py`

 * *Files identical despite different names*

### Comparing `sumformer2-0.4/sumformer2/transformer.py` & `sumformer2-0.4.1/sumformer2/transformer.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,22 +4,23 @@
 
 from torch.utils.checkpoint import checkpoint
 
 from .modules import *
 
 class Sumformer(nn.Module):
     """Text summarization transformer."""
-    def __init__(self, device, emb_dim, vocab_size, max_len, pos_encoding, GLU, norm, enc_heads, enc_hidden, enc_depth, enc_dropout, dec_heads, dec_hidden, dec_depth, dec_dropout):
+    def __init__(self, device, emb_dim, vocab_size, max_len, pos_encoding, GLU, norm, checkpoint, enc_heads, enc_hidden, enc_depth, enc_dropout, dec_heads, dec_hidden, dec_depth, dec_dropout):
         super().__init__()
 
         self.device = device
         self.emb_dim = emb_dim
         self.vocab_size = vocab_size
         self.max_len = max_len
         self.norm = norm
+        self.checkpoint = checkpoint
 
         self.token_embedding = nn.Embedding(num_embeddings=vocab_size, embedding_dim=emb_dim).to(device)
         if pos_encoding:
             self.pos_embedding = self.compute_encodings(max_len, emb_dim).to(device)
         else:
             self.pos_embedding = nn.Embedding(num_embeddings=max_len, embedding_dim=emb_dim).to(device)
 
@@ -43,24 +44,30 @@
 
     def encode(self, source, source_mask=None):
         tokens_source = self.token_embedding(source.to(self.device))
         b, t_s, k = tokens_source.size()
         positions_source = self.pos_embedding(torch.arange(t_s, device=self.device))[None, :, :].expand(b, t_s, k)
         x = tokens_source + positions_source
         for enc_layer in self.encoder:
-            x = checkpoint(enc_layer, x, source_mask)
+            if self.checkpoint:
+                x = checkpoint(enc_layer, x, source_mask)
+            else:
+                x = enc_layer(x, source_mask)
         return x
     
     def decode(self, target, context, target_mask=None):
         tokens_target = self.token_embedding(target.to(self.device))
         b, t_t, k = tokens_target.size()
         positions_target = self.pos_embedding(torch.arange(t_t, device=self.device))[None, :, :].expand(b, t_t, k)
         y = tokens_target + positions_target
         for dec_layer in self.decoder:
-            y = checkpoint(dec_layer, y, context, target_mask)
+            if self.checkpoint:
+                y = checkpoint(dec_layer, y, context, target_mask)
+            else:
+                y = dec_layer(y, context, target_mask)
         return self.toProbs(y)
 
     def forward(self, source, target, source_mask=None, target_mask=None):
         context = self.encode(source, source_mask)
         return self.decode(target, context, target_mask)
     
     def greedy(self, source, start_token=0, end_token=1, max_len=256, source_mask=None, logits=False):
```

### Comparing `sumformer2-0.4/sumformer2/utils.py` & `sumformer2-0.4.1/sumformer2/utils.py`

 * *Files identical despite different names*

### Comparing `sumformer2-0.4/sumformer2.egg-info/requires.txt` & `sumformer2-0.4.1/sumformer2.egg-info/requires.txt`

 * *Files identical despite different names*

