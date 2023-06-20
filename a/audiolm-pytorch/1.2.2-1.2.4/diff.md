# Comparing `tmp/audiolm-pytorch-1.2.2.tar.gz` & `tmp/audiolm-pytorch-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiolm-pytorch-1.2.2.tar", last modified: Sat Jun 17 16:56:33 2023, max compression
+gzip compressed data, was "audiolm-pytorch-1.2.4.tar", last modified: Tue Jun 20 19:03:50 2023, max compression
```

## Comparing `audiolm-pytorch-1.2.2.tar` & `audiolm-pytorch-1.2.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 16:56:33.428527 audiolm-pytorch-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-17 16:56:23.000000 audiolm-pytorch-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-17 16:56:33.428527 audiolm-pytorch-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18642 2023-06-17 16:56:23.000000 audiolm-pytorch-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 16:56:33.428527 audiolm-pytorch-1.2.2/audiolm_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-17 16:56:23.000000 audiolm-pytorch-1.2.2/audiolm_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-06-17 16:56:23.000000 audiolm-pytorch-1.2.2/audiolm_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)    66279 2023-06-17 16:56:23.000000 audiolm-pytorch-1.2.2/audiolm_pytorch/audiolm_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-06-17 16:56:23.000000 audiolm-pytorch-1.2.2/audiolm_pytorch/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-06-17 16:56:23.000000 audiolm-pytorch-1.2.2/audiolm_pytorch/encodec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-06-17 16:56:23.000000 audiolm-pytorch-1.2.2/audiolm_pytorch/hubert_kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-17 16:56:23.000000 audiolm-pytorch-1.2.2/audiolm_pytorch/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    30270 2023-06-17 16:56:23.000000 audiolm-pytorch-1.2.2/audiolm_pytorch/soundstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-06-17 16:56:23.000000 audiolm-pytorch-1.2.2/audiolm_pytorch/t5.py
--rw-r--r--   0 runner    (1001) docker     (123)    42491 2023-06-17 16:56:23.000000 audiolm-pytorch-1.2.2/audiolm_pytorch/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-17 16:56:23.000000 audiolm-pytorch-1.2.2/audiolm_pytorch/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-17 16:56:23.000000 audiolm-pytorch-1.2.2/audiolm_pytorch/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-17 16:56:23.000000 audiolm-pytorch-1.2.2/audiolm_pytorch/vq_wav2vec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 16:56:33.428527 audiolm-pytorch-1.2.2/audiolm_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-17 16:56:33.000000 audiolm-pytorch-1.2.2/audiolm_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-17 16:56:33.000000 audiolm-pytorch-1.2.2/audiolm_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 16:56:33.000000 audiolm-pytorch-1.2.2/audiolm_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-17 16:56:33.000000 audiolm-pytorch-1.2.2/audiolm_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-17 16:56:33.000000 audiolm-pytorch-1.2.2/audiolm_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 16:56:33.428527 audiolm-pytorch-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-17 16:56:23.000000 audiolm-pytorch-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:03:50.578380 audiolm-pytorch-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-20 19:03:40.000000 audiolm-pytorch-1.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-20 19:03:50.578380 audiolm-pytorch-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18642 2023-06-20 19:03:40.000000 audiolm-pytorch-1.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:03:50.578380 audiolm-pytorch-1.2.4/audiolm_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-20 19:03:40.000000 audiolm-pytorch-1.2.4/audiolm_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-06-20 19:03:40.000000 audiolm-pytorch-1.2.4/audiolm_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67328 2023-06-20 19:03:40.000000 audiolm-pytorch-1.2.4/audiolm_pytorch/audiolm_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-06-20 19:03:40.000000 audiolm-pytorch-1.2.4/audiolm_pytorch/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-06-20 19:03:40.000000 audiolm-pytorch-1.2.4/audiolm_pytorch/encodec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-06-20 19:03:40.000000 audiolm-pytorch-1.2.4/audiolm_pytorch/hubert_kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-20 19:03:40.000000 audiolm-pytorch-1.2.4/audiolm_pytorch/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30270 2023-06-20 19:03:40.000000 audiolm-pytorch-1.2.4/audiolm_pytorch/soundstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-06-20 19:03:40.000000 audiolm-pytorch-1.2.4/audiolm_pytorch/t5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42491 2023-06-20 19:03:40.000000 audiolm-pytorch-1.2.4/audiolm_pytorch/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-20 19:03:40.000000 audiolm-pytorch-1.2.4/audiolm_pytorch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-20 19:03:40.000000 audiolm-pytorch-1.2.4/audiolm_pytorch/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-20 19:03:40.000000 audiolm-pytorch-1.2.4/audiolm_pytorch/vq_wav2vec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:03:50.578380 audiolm-pytorch-1.2.4/audiolm_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-20 19:03:50.000000 audiolm-pytorch-1.2.4/audiolm_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-20 19:03:50.000000 audiolm-pytorch-1.2.4/audiolm_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 19:03:50.000000 audiolm-pytorch-1.2.4/audiolm_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-20 19:03:50.000000 audiolm-pytorch-1.2.4/audiolm_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-20 19:03:50.000000 audiolm-pytorch-1.2.4/audiolm_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 19:03:50.578380 audiolm-pytorch-1.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-20 19:03:40.000000 audiolm-pytorch-1.2.4/setup.py
```

### Comparing `audiolm-pytorch-1.2.2/LICENSE` & `audiolm-pytorch-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.2/PKG-INFO` & `audiolm-pytorch-1.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiolm-pytorch
-Version: 1.2.2
+Version: 1.2.4
 Summary: AudioLM - Language Modeling Approach to Audio Generation from Google Research - Pytorch
 Home-page: https://github.com/lucidrains/audiolm-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,audio generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `audiolm-pytorch-1.2.2/README.md` & `audiolm-pytorch-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.2/audiolm_pytorch/__init__.py` & `audiolm-pytorch-1.2.4/audiolm_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.2/audiolm_pytorch/attend.py` & `audiolm-pytorch-1.2.4/audiolm_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.2/audiolm_pytorch/audiolm_pytorch.py` & `audiolm-pytorch-1.2.4/audiolm_pytorch/audiolm_pytorch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import math
 from functools import partial, wraps
 
 from beartype.typing import Optional, Union, List
 from beartype import beartype
 
 import torch
-from torch import nn, einsum
+from torch import nn, einsum, Tensor
 from torch.autograd import grad as torch_grad
 import torch.nn.functional as F
 from torch.nn.utils.rnn import pad_sequence
 
 from einops import rearrange, repeat, reduce
 from einops.layers.torch import Rearrange
 
@@ -1325,28 +1325,39 @@
     @eval_decorator
     @torch.no_grad()
     @beartype
     def generate(
         self,
         *,
         semantic_token_ids,
+        prime_wave: Optional[Tensor] = None,
         text: Optional[List[str]] = None,
         text_embeds = None,
         max_time_steps = 512,
         cond_scale = 3.,
         filter_thres = 0.9,
         temperature = 1.,
         reconstruct_wave = False,
         **kwargs
     ):
         batch, device = semantic_token_ids.shape[0], self.device
 
         semantic_token_ids = semantic_token_ids.to(device)
 
-        coarse_token_ids = torch.empty((batch, 0), device = device, dtype = torch.long)
+        # initialize coarse token ids
+        # if a prime audio wave was supplied, then start off with appropriate acoustic tokens
+
+        if exists(prime_wave):
+            with torch.no_grad():
+                self.codec.eval()
+                _, indices, _ = self.codec(prime_wave, return_encoded = True)
+                coarse_token_ids = indices[..., :self.num_coarse_quantizers]
+                coarse_token_ids = rearrange(coarse_token_ids, 'b ... -> b (...)')
+        else:
+            coarse_token_ids = torch.empty((batch, 0), device = device, dtype = torch.long)
 
         # derive text embeddings if needed
 
         has_text = exists(text) or exists(text_embeds)
         assert not (self.transformer.has_condition ^ has_text)
 
         if not exists(text_embeds) and exists(text):
@@ -1426,20 +1437,22 @@
 
         if not exists(coarse_token_ids):
             assert exists(self.codec), 'Codec must be provided if given raw wave for training'
 
             with torch.no_grad():
                 self.codec.eval()
                 _, indices, _ = self.codec(raw_wave_for_codec, return_encoded = True)
-                batch = raw_wave_for_codec.shape[0]
-                num_timesteps = raw_wave_for_codec.shape[1]
+
+                batch, num_timesteps = raw_wave_for_codec.shape
                 num_frames = int(num_timesteps / self.codec.seq_len_multiple_of)
+
                 assert indices.shape[0] == batch and indices.shape[1] == num_frames, \
                     f'Expected indices to have shape (batch, num_frames, num_coarse_quantizers + num_fine_quantizers), but got {indices.shape}'
-                coarse_token_ids, _ = indices[..., :self.num_coarse_quantizers], indices[..., self.num_coarse_quantizers:]
+
+                coarse_token_ids = indices[..., :self.num_coarse_quantizers]
 
         semantic_token_ids = rearrange(semantic_token_ids, 'b ... -> b (...)')
         coarse_token_ids = rearrange(coarse_token_ids, 'b ... -> b (...)')
 
         if self.training:
             semantic_token_ids = append_eos_id(semantic_token_ids, self.transformer.semantic_eos_id)
             coarse_token_ids = append_eos_id(coarse_token_ids, self.transformer.coarse_eos_id)
@@ -1551,14 +1564,15 @@
     @eval_decorator
     @torch.no_grad()
     @beartype
     def generate(
         self,
         *,
         coarse_token_ids,
+        prime_wave: Optional[Tensor] = None,
         text: Optional[List[str]] = None,
         text_embeds = None,
         cond_scale = 3.,
         filter_thres = 0.9,
         temperature = 1.,
         reconstruct_wave = False,
         mask_out_generated_fine_tokens = False,
@@ -1575,17 +1589,29 @@
         has_text = exists(text) or exists(text_embeds)
         assert not (self.transformer.has_condition ^ has_text)
 
         if not exists(text_embeds) and exists(text):
             with torch.no_grad():
                 text_embeds = self.transformer.embed_text(text, output_device = device)
 
-        # initialize
+        # initialize fine token ids
+        # if a prime wave was supplied, start off with fine acoustic tokens
+
+        if exists(prime_wave):
+            assert exists(self.codec)
+            with torch.no_grad():
+                self.codec.eval()
+                _, token_ids, _ = self.codec(prime_wave, return_encoded = True)
+
+            fine_token_ids = token_ids[..., self.num_coarse_quantizers:]
+            fine_token_ids = rearrange(fine_token_ids, 'b ... -> b (...)')
+        else:
+            fine_token_ids = torch.empty((batch, 0), device = device, dtype = torch.long)
 
-        fine_token_ids = torch.empty((batch, 0), device = device, dtype = torch.long)
+        # calculate number of sampling steps
 
         init_fine_time_step = fine_token_ids.shape[-1]
         max_time_steps = coarse_token_ids.shape[1] // self.num_coarse_quantizers
 
         sampled_fine_token_ids = fine_token_ids.clone()
 
         for time_step in tqdm(range(init_fine_time_step, max_time_steps), desc = 'generating fine'):
@@ -1660,17 +1686,18 @@
 
         if exists(raw_wave):
             assert exists(self.codec), 'Codec must be provided if given raw wave for training'
 
             with torch.no_grad():
                 self.codec.eval()
                 _, token_ids, _ = self.codec(raw_wave, return_encoded = True)
-                batch = raw_wave.shape[0]
-                num_timesteps = raw_wave.shape[1]
+
+                batch, num_timesteps = raw_wave.shape
                 num_frames = int(num_timesteps / self.codec.seq_len_multiple_of)
+
                 assert token_ids.shape == torch.Size((batch, num_frames, self.num_coarse_quantizers + self.num_fine_quantizers)), \
                     f'Expected token ids to have shape (batch, num_frames, num_coarse_quantizers + num_fine_quantizers), but got {token_ids.shape}'
 
         if exists(token_ids):
             coarse_token_ids, fine_token_ids = token_ids[..., :self.num_coarse_quantizers], token_ids[..., self.num_coarse_quantizers:]
 
         coarse_token_ids = rearrange(coarse_token_ids, 'b ... -> b (...)')
@@ -1770,15 +1797,15 @@
             transformer = semantic_transformer,
             audio_conditioner = audio_conditioner,
             unique_consecutive = unique_consecutive
         )
 
         self.coarse = CoarseTransformerWrapper(
             wav2vec = wav2vec,
-            codec= codec,
+            codec = codec,
             transformer = coarse_transformer,
             audio_conditioner = audio_conditioner,
             unique_consecutive = unique_consecutive
         )
 
         self.fine = FineTransformerWrapper(
             codec= codec,
@@ -1793,15 +1820,15 @@
     @eval_decorator
     @torch.no_grad()
     def forward(
         self,
         *,
         batch_size = 1,
         text: Optional[List[str]] = None,
-        text_embeds: Optional[torch.Tensor] = None,
+        text_embeds: Optional[Tensor] = None,
         prime_wave = None,
         max_length = 2048,
         return_coarse_generated_wave = False,
         mask_out_generated_fine_tokens = False
     ):
         assert not (self.needs_text and (not exists(text) and not exists(text_embeds))), 'text needs to be passed in if one of the transformer requires conditioning'
 
@@ -1818,21 +1845,23 @@
             prime_wave = prime_wave,
             max_length = max_length
         )
 
         coarse_token_ids_or_recon_wave = self.coarse.generate(
             text_embeds = text_embeds if self.coarse_has_condition else None,
             semantic_token_ids = semantic_token_ids,
+            prime_wave = prime_wave,
             reconstruct_wave = return_coarse_generated_wave
         )
 
         if return_coarse_generated_wave:
             return coarse_token_ids_or_recon_wave
 
         generated_wave = self.fine.generate(
             text_embeds = text_embeds if self.fine_has_condition else None,
             coarse_token_ids = coarse_token_ids_or_recon_wave,
+            prime_wave = prime_wave,
             reconstruct_wave = True,
             mask_out_generated_fine_tokens = mask_out_generated_fine_tokens
         )
 
         return generated_wave
```

### Comparing `audiolm-pytorch-1.2.2/audiolm_pytorch/data.py` & `audiolm-pytorch-1.2.4/audiolm_pytorch/data.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.2/audiolm_pytorch/encodec.py` & `audiolm-pytorch-1.2.4/audiolm_pytorch/encodec.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.2/audiolm_pytorch/hubert_kmeans.py` & `audiolm-pytorch-1.2.4/audiolm_pytorch/hubert_kmeans.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.2/audiolm_pytorch/optimizer.py` & `audiolm-pytorch-1.2.4/audiolm_pytorch/optimizer.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.2/audiolm_pytorch/soundstream.py` & `audiolm-pytorch-1.2.4/audiolm_pytorch/soundstream.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.2/audiolm_pytorch/t5.py` & `audiolm-pytorch-1.2.4/audiolm_pytorch/t5.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.2/audiolm_pytorch/trainer.py` & `audiolm-pytorch-1.2.4/audiolm_pytorch/trainer.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.2/audiolm_pytorch/vq_wav2vec.py` & `audiolm-pytorch-1.2.4/audiolm_pytorch/vq_wav2vec.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.2/audiolm_pytorch.egg-info/PKG-INFO` & `audiolm-pytorch-1.2.4/audiolm_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiolm-pytorch
-Version: 1.2.2
+Version: 1.2.4
 Summary: AudioLM - Language Modeling Approach to Audio Generation from Google Research - Pytorch
 Home-page: https://github.com/lucidrains/audiolm-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,audio generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `audiolm-pytorch-1.2.2/audiolm_pytorch.egg-info/SOURCES.txt` & `audiolm-pytorch-1.2.4/audiolm_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.2/setup.py` & `audiolm-pytorch-1.2.4/setup.py`

 * *Files identical despite different names*

