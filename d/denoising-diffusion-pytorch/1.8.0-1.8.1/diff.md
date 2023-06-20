# Comparing `tmp/denoising-diffusion-pytorch-1.8.0.tar.gz` & `tmp/denoising-diffusion-pytorch-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "denoising-diffusion-pytorch-1.8.0.tar", last modified: Mon Jun 19 16:26:16 2023, max compression
+gzip compressed data, was "denoising-diffusion-pytorch-1.8.1.tar", last modified: Tue Jun 20 20:51:00 2023, max compression
```

## Comparing `denoising-diffusion-pytorch-1.8.0.tar` & `denoising-diffusion-pytorch-1.8.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:26:16.061913 denoising-diffusion-pytorch-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-19 16:26:07.000000 denoising-diffusion-pytorch-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-19 16:26:16.061913 denoising-diffusion-pytorch-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10500 2023-06-19 16:26:07.000000 denoising-diffusion-pytorch-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:26:16.061913 denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-19 16:26:07.000000 denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-06-19 16:26:07.000000 denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)    27823 2023-06-19 16:26:07.000000 denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/classifier_free_guidance.py
--rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-06-19 16:26:07.000000 denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    36127 2023-06-19 16:26:07.000000 denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)    29665 2023-06-19 16:26:07.000000 denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-06-19 16:26:07.000000 denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/elucidated_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-06-19 16:26:07.000000 denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/fid_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)    35629 2023-06-19 16:26:07.000000 denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/guided_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-06-19 16:26:07.000000 denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    21236 2023-06-19 16:26:07.000000 denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/simple_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-06-19 16:26:07.000000 denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-19 16:26:07.000000 denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-19 16:26:07.000000 denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:26:16.061913 denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-19 16:26:15.000000 denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-19 16:26:16.000000 denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 16:26:15.000000 denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-19 16:26:15.000000 denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-19 16:26:15.000000 denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 16:26:16.065913 denoising-diffusion-pytorch-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-19 16:26:07.000000 denoising-diffusion-pytorch-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:51:00.510675 denoising-diffusion-pytorch-1.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-20 20:50:50.000000 denoising-diffusion-pytorch-1.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-20 20:51:00.510675 denoising-diffusion-pytorch-1.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10546 2023-06-20 20:50:50.000000 denoising-diffusion-pytorch-1.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:51:00.510675 denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-20 20:50:50.000000 denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-06-20 20:50:50.000000 denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27823 2023-06-20 20:50:50.000000 denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/classifier_free_guidance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-06-20 20:50:50.000000 denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36132 2023-06-20 20:50:50.000000 denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29665 2023-06-20 20:50:50.000000 denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-06-20 20:50:50.000000 denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/elucidated_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-06-20 20:50:50.000000 denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/fid_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35629 2023-06-20 20:50:50.000000 denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/guided_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-06-20 20:50:50.000000 denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21236 2023-06-20 20:50:50.000000 denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/simple_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-06-20 20:50:50.000000 denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-20 20:50:50.000000 denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-20 20:50:50.000000 denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:51:00.510675 denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-20 20:51:00.000000 denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-20 20:51:00.000000 denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 20:51:00.000000 denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-20 20:51:00.000000 denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-20 20:51:00.000000 denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 20:51:00.510675 denoising-diffusion-pytorch-1.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-20 20:50:50.000000 denoising-diffusion-pytorch-1.8.1/setup.py
```

### Comparing `denoising-diffusion-pytorch-1.8.0/LICENSE` & `denoising-diffusion-pytorch-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.0/PKG-INFO` & `denoising-diffusion-pytorch-1.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 1.8.0
+Version: 1.8.1
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising-diffusion-pytorch-1.8.0/README.md` & `denoising-diffusion-pytorch-1.8.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,16 @@
 
 ```python
 import torch
 from denoising_diffusion_pytorch import Unet, GaussianDiffusion
 
 model = Unet(
     dim = 64,
-    dim_mults = (1, 2, 4, 8)
+    dim_mults = (1, 2, 4, 8),
+    flash_attn = True
 )
 
 diffusion = GaussianDiffusion(
     model,
     image_size = 128,
     timesteps = 1000    # number of steps
 )
@@ -53,15 +54,16 @@
 Or, if you simply want to pass in a folder name and the desired image dimensions, you can use the `Trainer` class to easily train a model.
 
 ```python
 from denoising_diffusion_pytorch import Unet, GaussianDiffusion, Trainer
 
 model = Unet(
     dim = 64,
-    dim_mults = (1, 2, 4, 8)
+    dim_mults = (1, 2, 4, 8),
+    flash_attn = True
 )
 
 diffusion = GaussianDiffusion(
     model,
     image_size = 128,
     timesteps = 1000,           # number of steps
     sampling_timesteps = 250    # number of sampling timesteps (using ddim for faster inference [see citation for ddim paper])
```

#### html2text {}

```diff
@@ -8,40 +8,40 @@
 with_Letitia | Outlier Flax_implementation from YiYi_Xu Annotated_code by
 Research Scientists / Engineers from ð¤_Huggingface Update: Turns out none of
 the technicalities really matters at all | "Cold_Diffusion"_paper | Muse [./
 images/sample.png][Image] [![PyPI version](https://badge.fury.io/py/denoising-
 diffusion-pytorch.svg)](https://badge.fury.io/py/denoising-diffusion-pytorch)
 ## Install ```bash $ pip install denoising_diffusion_pytorch ``` ## Usage
 ```python import torch from denoising_diffusion_pytorch import Unet,
-GaussianDiffusion model = Unet( dim = 64, dim_mults = (1, 2, 4, 8) ) diffusion
-= GaussianDiffusion( model, image_size = 128, timesteps = 1000 # number of
-steps ) training_images = torch.rand(8, 3, 128, 128) # images are normalized
-from 0 to 1 loss = diffusion(training_images) loss.backward() # after a lot of
-training sampled_images = diffusion.sample(batch_size = 4) sampled_images.shape
-# (4, 3, 128, 128) ``` Or, if you simply want to pass in a folder name and the
-desired image dimensions, you can use the `Trainer` class to easily train a
-model. ```python from denoising_diffusion_pytorch import Unet,
-GaussianDiffusion, Trainer model = Unet( dim = 64, dim_mults = (1, 2, 4, 8) )
-diffusion = GaussianDiffusion( model, image_size = 128, timesteps = 1000, #
-number of steps sampling_timesteps = 250 # number of sampling timesteps (using
-ddim for faster inference [see citation for ddim paper]) ) trainer = Trainer
-( diffusion, 'path/to/your/images', train_batch_size = 32, train_lr = 8e-5,
-train_num_steps = 700000, # total training steps gradient_accumulate_every = 2,
-# gradient accumulation steps ema_decay = 0.995, # exponential moving average
-decay amp = True, # turn on mixed precision calculate_fid = True # whether to
-calculate fid during training ) trainer.train() ``` Samples and model
-checkpoints will be logged to `./results` periodically ## Multi-GPU Training
-The `Trainer` class is now equipped with ð¤_Accelerator. You can easily do
-multi-gpu training in two steps using their `accelerate` CLI At the project
-root directory, where the training script is, run ```python $ accelerate config
-``` Then, in the same directory ```python $ accelerate launch train.py ``` ##
-Miscellaneous ### 1D Sequence By popular request, a 1D Unet + Gaussian
-Diffusion implementation. ```python import torch from
-denoising_diffusion_pytorch import Unet1D, GaussianDiffusion1D, Trainer1D model
-= Unet1D( dim = 64, dim_mults = (1, 2, 4, 8), channels = 32 ) diffusion =
+GaussianDiffusion model = Unet( dim = 64, dim_mults = (1, 2, 4, 8), flash_attn
+= True ) diffusion = GaussianDiffusion( model, image_size = 128, timesteps =
+1000 # number of steps ) training_images = torch.rand(8, 3, 128, 128) # images
+are normalized from 0 to 1 loss = diffusion(training_images) loss.backward() #
+after a lot of training sampled_images = diffusion.sample(batch_size = 4)
+sampled_images.shape # (4, 3, 128, 128) ``` Or, if you simply want to pass in a
+folder name and the desired image dimensions, you can use the `Trainer` class
+to easily train a model. ```python from denoising_diffusion_pytorch import
+Unet, GaussianDiffusion, Trainer model = Unet( dim = 64, dim_mults = (1, 2, 4,
+8), flash_attn = True ) diffusion = GaussianDiffusion( model, image_size = 128,
+timesteps = 1000, # number of steps sampling_timesteps = 250 # number of
+sampling timesteps (using ddim for faster inference [see citation for ddim
+paper]) ) trainer = Trainer( diffusion, 'path/to/your/images', train_batch_size
+= 32, train_lr = 8e-5, train_num_steps = 700000, # total training steps
+gradient_accumulate_every = 2, # gradient accumulation steps ema_decay = 0.995,
+# exponential moving average decay amp = True, # turn on mixed precision
+calculate_fid = True # whether to calculate fid during training ) trainer.train
+() ``` Samples and model checkpoints will be logged to `./results` periodically
+## Multi-GPU Training The `Trainer` class is now equipped with ð¤
+Accelerator. You can easily do multi-gpu training in two steps using their
+`accelerate` CLI At the project root directory, where the training script is,
+run ```python $ accelerate config ``` Then, in the same directory ```python $
+accelerate launch train.py ``` ## Miscellaneous ### 1D Sequence By popular
+request, a 1D Unet + Gaussian Diffusion implementation. ```python import torch
+from denoising_diffusion_pytorch import Unet1D, GaussianDiffusion1D, Trainer1D
+model = Unet1D( dim = 64, dim_mults = (1, 2, 4, 8), channels = 32 ) diffusion =
 GaussianDiffusion1D( model, seq_length = 128, timesteps = 1000, objective =
 'pred_v' ) training_seq = torch.rand(64, 32, 128) # features are normalized
 from 0 to 1 loss = diffusion(training_seq) loss.backward() # Or using trainer
 trainer = Trainer1D( diffusion, dataset = training_seq, train_batch_size = 32,
 train_lr = 8e-5, train_num_steps = 700000, # total training steps
 gradient_accumulate_every = 2, # gradient accumulation steps ema_decay = 0.995,
 # exponential moving average decay amp = True, # turn on mixed precision )
```

### Comparing `denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/__init__.py` & `denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/attend.py` & `denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/classifier_free_guidance.py` & `denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/classifier_free_guidance.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py` & `denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py`

 * *Files 0% similar despite different names*

```diff
@@ -908,16 +908,16 @@
 
         # prepare model, dataloader, optimizer with accelerator
 
         self.model, self.opt = self.accelerator.prepare(self.model, self.opt)
 
         # FID-score computation
 
+        self.calculate_fid = calculate_fid
         if calculate_fid:
-            self.calculate_fid = True
             if not self.model.is_ddim_sampling:
                 self.accelerator.print(
                     "WARNING: Robust FID computation requires a lot of generated samples and can therefore be very time consuming."\
                     "Consider using DDIM sampling to save time."
                 )
             self.fid_scorer = FIDEvaluation(
                 batch_size=self.batch_size,
```

### Comparing `denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py` & `denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/elucidated_diffusion.py` & `denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/elucidated_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/fid_evaluation.py` & `denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/fid_evaluation.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/guided_diffusion.py` & `denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/guided_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/learned_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/learned_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/simple_diffusion.py` & `denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/simple_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch.egg-info/PKG-INFO` & `denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 1.8.0
+Version: 1.8.1
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch.egg-info/SOURCES.txt` & `denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.0/setup.py` & `denoising-diffusion-pytorch-1.8.1/setup.py`

 * *Files identical despite different names*

