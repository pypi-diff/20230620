# Comparing `tmp/nlp-models-2.3.1.tar.gz` & `tmp/nlp-models-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlp-models-2.3.1.tar", last modified: Mon Jun 19 16:56:23 2023, max compression
+gzip compressed data, was "nlp-models-2.3.2.tar", last modified: Tue Jun 20 16:31:27 2023, max compression
```

## Comparing `nlp-models-2.3.1.tar` & `nlp-models-2.3.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:56:23.718292 nlp-models-2.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-19 16:56:14.000000 nlp-models-2.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-06-19 16:56:23.718292 nlp-models-2.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-19 16:56:14.000000 nlp-models-2.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-19 16:56:14.000000 nlp-models-2.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-19 16:56:23.718292 nlp-models-2.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-19 16:56:14.000000 nlp-models-2.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:56:23.714292 nlp-models-2.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:56:23.714292 nlp-models-2.3.1/src/bert_classifier/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 16:56:14.000000 nlp-models-2.3.1/src/bert_classifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-19 16:56:14.000000 nlp-models-2.3.1/src/bert_classifier/bert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-19 16:56:14.000000 nlp-models-2.3.1/src/bert_classifier/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-06-19 16:56:14.000000 nlp-models-2.3.1/src/bert_classifier/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-19 16:56:14.000000 nlp-models-2.3.1/src/bert_classifier/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-19 16:56:14.000000 nlp-models-2.3.1/src/bert_classifier/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-06-19 16:56:14.000000 nlp-models-2.3.1/src/bert_classifier/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:56:23.718292 nlp-models-2.3.1/src/multi_task_model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 16:56:14.000000 nlp-models-2.3.1/src/multi_task_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-06-19 16:56:14.000000 nlp-models-2.3.1/src/multi_task_model/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-19 16:56:14.000000 nlp-models-2.3.1/src/multi_task_model/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-19 16:56:14.000000 nlp-models-2.3.1/src/multi_task_model/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-06-19 16:56:14.000000 nlp-models-2.3.1/src/multi_task_model/mtl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9589 2023-06-19 16:56:14.000000 nlp-models-2.3.1/src/multi_task_model/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-19 16:56:14.000000 nlp-models-2.3.1/src/multi_task_model/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:56:23.718292 nlp-models-2.3.1/src/nlp_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-06-19 16:56:23.000000 nlp-models-2.3.1/src/nlp_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-19 16:56:23.000000 nlp-models-2.3.1/src/nlp_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 16:56:23.000000 nlp-models-2.3.1/src/nlp_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-19 16:56:23.000000 nlp-models-2.3.1/src/nlp_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-19 16:56:23.000000 nlp-models-2.3.1/src/nlp_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:31:27.967660 nlp-models-2.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-20 16:31:12.000000 nlp-models-2.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-06-20 16:31:27.967660 nlp-models-2.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-20 16:31:12.000000 nlp-models-2.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-20 16:31:12.000000 nlp-models-2.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-20 16:31:27.971660 nlp-models-2.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-20 16:31:12.000000 nlp-models-2.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:31:27.959659 nlp-models-2.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:31:27.963659 nlp-models-2.3.2/src/bert_classifier/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 16:31:12.000000 nlp-models-2.3.2/src/bert_classifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-20 16:31:12.000000 nlp-models-2.3.2/src/bert_classifier/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-06-20 16:31:12.000000 nlp-models-2.3.2/src/bert_classifier/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-06-20 16:31:12.000000 nlp-models-2.3.2/src/bert_classifier/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-20 16:31:12.000000 nlp-models-2.3.2/src/bert_classifier/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-20 16:31:12.000000 nlp-models-2.3.2/src/bert_classifier/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-06-20 16:31:12.000000 nlp-models-2.3.2/src/bert_classifier/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:31:27.967660 nlp-models-2.3.2/src/multi_task_model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 16:31:12.000000 nlp-models-2.3.2/src/multi_task_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-06-20 16:31:12.000000 nlp-models-2.3.2/src/multi_task_model/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-20 16:31:12.000000 nlp-models-2.3.2/src/multi_task_model/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-20 16:31:12.000000 nlp-models-2.3.2/src/multi_task_model/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-06-20 16:31:12.000000 nlp-models-2.3.2/src/multi_task_model/mtl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9619 2023-06-20 16:31:12.000000 nlp-models-2.3.2/src/multi_task_model/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-20 16:31:12.000000 nlp-models-2.3.2/src/multi_task_model/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:31:27.967660 nlp-models-2.3.2/src/nlp_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-06-20 16:31:27.000000 nlp-models-2.3.2/src/nlp_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-20 16:31:27.000000 nlp-models-2.3.2/src/nlp_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:31:27.000000 nlp-models-2.3.2/src/nlp_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-20 16:31:27.000000 nlp-models-2.3.2/src/nlp_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-20 16:31:27.000000 nlp-models-2.3.2/src/nlp_models.egg-info/top_level.txt
```

### Comparing `nlp-models-2.3.1/LICENSE` & `nlp-models-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nlp-models-2.3.1/PKG-INFO` & `nlp-models-2.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlp-models
-Version: 2.3.1
+Version: 2.3.2
 Summary: Transformers based NLP models
 Home-page: https://github.com/minggnim/nlp-models
 Author: Ming Gao
 Author-email: ming_gao@outlook.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nlp-models Version: 2.3.1 Summary: Transformers
+Metadata-Version: 2.1 Name: nlp-models Version: 2.3.2 Summary: Transformers
 based NLP models Home-page: https://github.com/minggnim/nlp-models Author: Ming
 Gao Author-email: ming_gao@outlook.com Classifier: Development Status :: 4 -
 Beta Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
```

### Comparing `nlp-models-2.3.1/README.md` & `nlp-models-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `nlp-models-2.3.1/setup.cfg` & `nlp-models-2.3.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nlp-models
-version = 2.3.1
+version = 2.3.2
 author = Ming Gao
 author_email = ming_gao@outlook.com
 url = https://github.com/minggnim/nlp-models
 description = Transformers based NLP models
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers =
```

### Comparing `nlp-models-2.3.1/src/bert_classifier/bert.py` & `nlp-models-2.3.2/src/bert_classifier/bert.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.3.1/src/bert_classifier/data.py` & `nlp-models-2.3.2/src/bert_classifier/data.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 '''
 data modules
 '''
 import torch
 from torch.utils.data import Dataset
-from .bert import bert_encoder
 
 
 class CustomDataset(Dataset):
     '''
     Class to construct torch Dataset from dataframe
     '''
-    def __init__(self, dataframe, data_field, label_field, tokenizer, max_len, multi_label):
+    def __init__(self,
+                 dataframe,
+                 data_field,
+                 label_field,
+                 tokenizer,
+                 max_len,
+                 multi_label=False
+                 ):
         self.max_len = max_len
         self.data = dataframe
         self.tokenizer = tokenizer
         self.content = self.data[data_field]
         self.label = self.data[label_field]
         self.multi_label = multi_label
```

### Comparing `nlp-models-2.3.1/src/bert_classifier/io.py` & `nlp-models-2.3.2/src/bert_classifier/io.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.3.1/src/bert_classifier/metrics.py` & `nlp-models-2.3.2/src/bert_classifier/metrics.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.3.1/src/bert_classifier/predict.py` & `nlp-models-2.3.2/src/bert_classifier/predict.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.3.1/src/bert_classifier/train.py` & `nlp-models-2.3.2/src/bert_classifier/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,20 +19,20 @@
 def loss_fn(outputs, targets):
     '''
     cross entropy loss function
     '''
     return torch.nn.CrossEntropyLoss()(outputs, targets)
 
 
-def optimizer(model, learning_rate):
-    optimizer = torch.optim.AdamW(
+def optimizer_obj(model, learning_rate):
+    opt = torch.optim.AdamW(
         params=model.parameters(),
         lr=learning_rate
     )
-    return optimizer
+    return opt
 
 
 def custom_trainer(model, optimizer, train_dataloader, test_dataloader, epochs=5, device='cpu'):
     '''
     custom training module
     '''
     for epoch in range(epochs):
```

### Comparing `nlp-models-2.3.1/src/multi_task_model/layers.py` & `nlp-models-2.3.2/src/multi_task_model/layers.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.3.1/src/multi_task_model/metrics.py` & `nlp-models-2.3.2/src/multi_task_model/metrics.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     MulticlassAccuracy
 )
 
 
 def hamming_distance(
     outputs,
     targets,
-    multi_label: bool = False, 
-    num_labels: Optional[int] = None, 
+    num_labels: int,
+    multi_label: bool = False,
     device: torch.device = torch.device('cpu'),
     average: Literal['micro', 'macro', 'weighted', 'none'] = 'macro'
 ):
     if not num_labels:
         raise ValueError('num_labels is required')
     if multi_label:
         hamming = MultilabelHammingDistance(num_labels, average=average)
```

### Comparing `nlp-models-2.3.1/src/multi_task_model/mtl.py` & `nlp-models-2.3.2/src/multi_task_model/mtl.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.3.1/src/multi_task_model/trainer.py` & `nlp-models-2.3.2/src/multi_task_model/trainer.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,32 +11,32 @@
 from .loss import cross_entropy_loss_fn
 
 
 @dataclass
 class Configs:
     epochs: int = 1
     optimizer_class = torch.optim.AdamW
-    optimizer_params: Dict[str, float] = field(default_factory = lambda: ({"lr": 2e-5})) 
+    optimizer_params: Dict[str, float] = field(default_factory=lambda: ({"lr": 2e-5}))
     weight_decay: float = 0.01
     scheduler: str = 'WarmupLinear'
     warmup_steps: int = 10000
     multi_label: bool = False
     num_labels: Optional[int] = None
     tune_base_model: bool = True
 
 
 class Trainer:
-    def __init__(self, 
+    def __init__(self,
                  model: torch.nn.Module,
                  train_dataloader: DataLoader,
                  test_dataloader: DataLoader,
                  configs: Configs,
-                 metrics = accuracy,
+                 metrics=accuracy,
                  device: torch.device = torch.device('cpu'),
-                 chkpt_dir = Path('../chkpt')
+                 chkpt_dir=Path('../chkpt')
                  ):
         self.model = model
         self.train_dataloader = train_dataloader
         self.test_dataloader = test_dataloader
         self.configs = configs
         self.metrics = metrics
         self.device = device
@@ -50,27 +50,27 @@
         set parameters to optimize and schedule
         '''
         if not self.configs.tune_base_model:
             for param in self.model.base_model.parameters():
                 param.requires_grad = False
 
         self.optimizer = self.get_optimizer(
-            list(self.model.named_parameters()), 
-            self.configs.optimizer_class, 
-            self.configs.optimizer_params, 
+            list(self.model.named_parameters()),
+            self.configs.optimizer_class,
+            self.configs.optimizer_params,
             self.configs.weight_decay)
         
         self.scheduler = self.get_scheduler(
-            self.optimizer, 
-            self.configs.scheduler, 
-            self.configs.warmup_steps, 
-            len(self.train_dataloader)*self.configs.epochs)
+            self.optimizer,
+            self.configs.scheduler,
+            self.configs.warmup_steps,
+            len(self.train_dataloader) * self.configs.epochs)
     
     def train(self):
-        epochs = tqdm(range(1, self.configs.epochs+1), leave = True, desc="Training...")
+        epochs = tqdm(range(1, self.configs.epochs + 1), leave=True, desc="Training...")
         for epoch in epochs:
             self.model.train()
             epochs.set_description(f"EPOCH {epoch} / {self.configs.epochs} | training...")
             self.train_one_epoch(epoch)
             self.clear()
             
             self.model.eval()
@@ -101,18 +101,20 @@
             loss.backward()
             torch.nn.utils.clip_grad_norm_(self.model.parameters(), 1.0)
             self.optimizer.step()
             self.scheduler.step()
 
             total_train_loss += loss.item()
             total_train_acc += self.metrics(
-                outputs[0], labels, 
-                self.configs.multi_label, 
-                self.configs.num_labels, 
-                self.device).item()
+                outputs[0],
+                labels,
+                self.configs.num_labels,
+                self.configs.multi_label,
+                self.device
+            ).item()
             
             batches.set_description(f"Train Loss Step: {loss.item():.2f}")
         
         self.logger(
             epoch, 
             total_train_acc/len(self.train_dataloader), 
             total_train_loss/len(self.train_dataloader),
@@ -137,18 +139,20 @@
             val_targets = torch.cat((val_targets, labels), 0)
             loss = cross_entropy_loss_fn(outputs[0], labels, self.configs.multi_label).reshape(1)
             val_loss = torch.cat((val_loss, loss), 0)
             batches.set_description(f"Validation Loss Step: {loss.item():.2f}")
         
         avg_val_loss = val_loss.mean().item()
         avg_val_acc = self.metrics(
-            val_outputs, val_targets, 
-            self.configs.multi_label, 
-            self.configs.num_labels, 
-            self.device).item()
+            val_outputs,
+            val_targets,
+            self.configs.num_labels,
+            self.configs.multi_label,
+            self.device
+        ).item()
         
         self.logger(epoch, avg_val_acc, avg_val_loss, 'test')
 
     @staticmethod
     def get_optimizer(param_optimizer,
                       optimizer_class = torch.optim.AdamW,
                       optimizer_params: dict = {'lr': 2e-5},
@@ -207,22 +211,22 @@
             'val_loss': self.val_logs[epoch][f'epoch_{epoch}']['loss'],
             'train_acc': self.train_logs[epoch][f'epoch_{epoch}']['accuracy'],
             'val_acc': self.val_logs[epoch][f'epoch_{epoch}']['accuracy'],
         }, chkpt_path)
         
     def schedule_cold_start(self):
         self.scheduler = self.get_scheduler(
-            self.optimizer, 
-            self.configs.scheduler, 
-            0, 
-            len(self.train_dataloader)*self.configs.epochs)
+            self.optimizer,
+            self.configs.scheduler,
+            0,
+            len(self.train_dataloader) * self.configs.epochs)
 
     def print_per_epoch(self, epoch):
         print(f"\n\n{'-'*30}EPOCH {epoch}/{self.configs.epochs}{'-'*30}")
-        epoch -= 1 
+        epoch -= 1
         train_loss = self.train_logs[epoch][f'epoch_{epoch}']['loss']
         train_acc = self.train_logs[epoch][f'epoch_{epoch}']['accuracy']
         val_loss = self.val_logs[epoch][f'epoch_{epoch}']['loss']
         val_acc = self.val_logs[epoch][f'epoch_{epoch}']['accuracy']
         print(f"Train -> LOSS: {train_loss} | ACCURACY: {train_acc}")
         print(f"Validation -> LOSS: {val_loss} | ACCURACY: {val_acc}\n\n\n")
```

### Comparing `nlp-models-2.3.1/src/multi_task_model/utils.py` & `nlp-models-2.3.2/src/multi_task_model/utils.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.3.1/src/nlp_models.egg-info/PKG-INFO` & `nlp-models-2.3.2/src/nlp_models.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlp-models
-Version: 2.3.1
+Version: 2.3.2
 Summary: Transformers based NLP models
 Home-page: https://github.com/minggnim/nlp-models
 Author: Ming Gao
 Author-email: ming_gao@outlook.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nlp-models Version: 2.3.1 Summary: Transformers
+Metadata-Version: 2.1 Name: nlp-models Version: 2.3.2 Summary: Transformers
 based NLP models Home-page: https://github.com/minggnim/nlp-models Author: Ming
 Gao Author-email: ming_gao@outlook.com Classifier: Development Status :: 4 -
 Beta Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
```

### Comparing `nlp-models-2.3.1/src/nlp_models.egg-info/SOURCES.txt` & `nlp-models-2.3.2/src/nlp_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

