# Comparing `tmp/tensor_parallel-1.2.5.tar.gz` & `tmp/tensor_parallel-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensor_parallel-1.2.5.tar", last modified: Wed Jun 14 15:41:36 2023, max compression
+gzip compressed data, was "tensor_parallel-1.2.6.tar", last modified: Mon Jun 19 17:08:16 2023, max compression
```

## Comparing `tensor_parallel-1.2.5.tar` & `tensor_parallel-1.2.6.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:41:36.726256 tensor_parallel-1.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-14 15:41:22.000000 tensor_parallel-1.2.5/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-06-14 15:41:36.726256 tensor_parallel-1.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-06-14 15:41:22.000000 tensor_parallel-1.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-14 15:41:22.000000 tensor_parallel-1.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-06-14 15:41:36.726256 tensor_parallel-1.2.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:41:36.722256 tensor_parallel-1.2.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:41:36.726256 tensor_parallel-1.2.5/src/tensor_parallel/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-14 15:41:22.000000 tensor_parallel-1.2.5/src/tensor_parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-06-14 15:41:22.000000 tensor_parallel-1.2.5/src/tensor_parallel/autoconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-14 15:41:22.000000 tensor_parallel-1.2.5/src/tensor_parallel/aux_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-06-14 15:41:22.000000 tensor_parallel-1.2.5/src/tensor_parallel/communications.py
--rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-06-14 15:41:22.000000 tensor_parallel-1.2.5/src/tensor_parallel/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-06-14 15:41:22.000000 tensor_parallel-1.2.5/src/tensor_parallel/cross_device_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     6093 2023-06-14 15:41:22.000000 tensor_parallel-1.2.5/src/tensor_parallel/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-06-14 15:41:22.000000 tensor_parallel-1.2.5/src/tensor_parallel/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-14 15:41:22.000000 tensor_parallel-1.2.5/src/tensor_parallel/imports.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-14 15:41:22.000000 tensor_parallel-1.2.5/src/tensor_parallel/per_device_tensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     8050 2023-06-14 15:41:22.000000 tensor_parallel-1.2.5/src/tensor_parallel/pretrained_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-06-14 15:41:22.000000 tensor_parallel-1.2.5/src/tensor_parallel/shard.py
--rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-06-14 15:41:22.000000 tensor_parallel-1.2.5/src/tensor_parallel/sharding.py
--rw-r--r--   0 runner    (1001) docker     (123)    18906 2023-06-14 15:41:22.000000 tensor_parallel-1.2.5/src/tensor_parallel/slicing_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-06-14 15:41:22.000000 tensor_parallel-1.2.5/src/tensor_parallel/state_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11969 2023-06-14 15:41:22.000000 tensor_parallel-1.2.5/src/tensor_parallel/tensor_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-06-14 15:41:22.000000 tensor_parallel-1.2.5/src/tensor_parallel/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-06-14 15:41:22.000000 tensor_parallel-1.2.5/src/tensor_parallel/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:41:36.726256 tensor_parallel-1.2.5/src/tensor_parallel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-06-14 15:41:36.000000 tensor_parallel-1.2.5/src/tensor_parallel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-14 15:41:36.000000 tensor_parallel-1.2.5/src/tensor_parallel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 15:41:36.000000 tensor_parallel-1.2.5/src/tensor_parallel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-14 15:41:36.000000 tensor_parallel-1.2.5/src/tensor_parallel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-14 15:41:36.000000 tensor_parallel-1.2.5/src/tensor_parallel.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:41:36.726256 tensor_parallel-1.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-06-14 15:41:22.000000 tensor_parallel-1.2.5/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-14 15:41:22.000000 tensor_parallel-1.2.5/tests/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-06-14 15:41:22.000000 tensor_parallel-1.2.5/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-06-14 15:41:22.000000 tensor_parallel-1.2.5/tests/test_saving.py
--rw-r--r--   0 runner    (1001) docker     (123)    11391 2023-06-14 15:41:22.000000 tensor_parallel-1.2.5/tests/test_transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:08:16.085980 tensor_parallel-1.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-19 17:08:06.000000 tensor_parallel-1.2.6/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-06-19 17:08:16.085980 tensor_parallel-1.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-06-19 17:08:06.000000 tensor_parallel-1.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-19 17:08:06.000000 tensor_parallel-1.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-06-19 17:08:16.085980 tensor_parallel-1.2.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:08:16.081979 tensor_parallel-1.2.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:08:16.085980 tensor_parallel-1.2.6/src/tensor_parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-19 17:08:06.000000 tensor_parallel-1.2.6/src/tensor_parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-06-19 17:08:06.000000 tensor_parallel-1.2.6/src/tensor_parallel/autoconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-19 17:08:06.000000 tensor_parallel-1.2.6/src/tensor_parallel/aux_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-06-19 17:08:06.000000 tensor_parallel-1.2.6/src/tensor_parallel/communications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-06-19 17:08:06.000000 tensor_parallel-1.2.6/src/tensor_parallel/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-06-19 17:08:06.000000 tensor_parallel-1.2.6/src/tensor_parallel/cross_device_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-06-19 17:08:06.000000 tensor_parallel-1.2.6/src/tensor_parallel/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-06-19 17:08:06.000000 tensor_parallel-1.2.6/src/tensor_parallel/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-19 17:08:06.000000 tensor_parallel-1.2.6/src/tensor_parallel/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-19 17:08:06.000000 tensor_parallel-1.2.6/src/tensor_parallel/per_device_tensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8050 2023-06-19 17:08:06.000000 tensor_parallel-1.2.6/src/tensor_parallel/pretrained_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-06-19 17:08:06.000000 tensor_parallel-1.2.6/src/tensor_parallel/shard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-06-19 17:08:06.000000 tensor_parallel-1.2.6/src/tensor_parallel/sharding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18906 2023-06-19 17:08:06.000000 tensor_parallel-1.2.6/src/tensor_parallel/slicing_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-06-19 17:08:06.000000 tensor_parallel-1.2.6/src/tensor_parallel/state_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11969 2023-06-19 17:08:06.000000 tensor_parallel-1.2.6/src/tensor_parallel/tensor_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-06-19 17:08:06.000000 tensor_parallel-1.2.6/src/tensor_parallel/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-06-19 17:08:06.000000 tensor_parallel-1.2.6/src/tensor_parallel/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:08:16.085980 tensor_parallel-1.2.6/src/tensor_parallel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-06-19 17:08:16.000000 tensor_parallel-1.2.6/src/tensor_parallel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-19 17:08:16.000000 tensor_parallel-1.2.6/src/tensor_parallel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 17:08:16.000000 tensor_parallel-1.2.6/src/tensor_parallel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-19 17:08:16.000000 tensor_parallel-1.2.6/src/tensor_parallel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-19 17:08:16.000000 tensor_parallel-1.2.6/src/tensor_parallel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:08:16.085980 tensor_parallel-1.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-06-19 17:08:06.000000 tensor_parallel-1.2.6/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-19 17:08:06.000000 tensor_parallel-1.2.6/tests/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-06-19 17:08:06.000000 tensor_parallel-1.2.6/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6989 2023-06-19 17:08:06.000000 tensor_parallel-1.2.6/tests/test_saving.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11391 2023-06-19 17:08:06.000000 tensor_parallel-1.2.6/tests/test_transformers.py
```

### Comparing `tensor_parallel-1.2.5/LICENCE` & `tensor_parallel-1.2.6/LICENCE`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.5/PKG-INFO` & `tensor_parallel-1.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensor_parallel
-Version: 1.2.5
+Version: 1.2.6
 Summary: Automatically shard your large model between multiple GPUs, works without torch.distributed
 Home-page: https://github.com/BlackSamorez/tensor_parallel
 Author: Andrei Panferov and Yaroslav Lisnyak
 Author-email: yalisnyak@nes.com
 Project-URL: Bug Tracker, https://github.com/BlackSamorez/tensor_parallel/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tensor_parallel Version: 1.2.5 Summary:
+Metadata-Version: 2.1 Name: tensor_parallel Version: 1.2.6 Summary:
 Automatically shard your large model between multiple GPUs, works without
 torch.distributed Home-page: https://github.com/BlackSamorez/tensor_parallel
 Author: Andrei Panferov and Yaroslav Lisnyak Author-email: yalisnyak@nes.com
 Project-URL: Bug Tracker, https://github.com/BlackSamorez/tensor_parallel/
 issues Classifier: Development Status :: 4 - Beta Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
```

### Comparing `tensor_parallel-1.2.5/README.md` & `tensor_parallel-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.5/setup.cfg` & `tensor_parallel-1.2.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tensor_parallel
-version = 1.2.5
+version = 1.2.6
 author = Andrei Panferov and Yaroslav Lisnyak
 author_email = yalisnyak@nes.com
 description = Automatically shard your large model between multiple GPUs, works without torch.distributed
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/BlackSamorez/tensor_parallel
 project_urls =
```

### Comparing `tensor_parallel-1.2.5/src/tensor_parallel/__init__.py` & `tensor_parallel-1.2.6/src/tensor_parallel/__init__.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.5/src/tensor_parallel/autoconfig.py` & `tensor_parallel-1.2.6/src/tensor_parallel/autoconfig.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.5/src/tensor_parallel/aux_actions.py` & `tensor_parallel-1.2.6/src/tensor_parallel/aux_actions.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.5/src/tensor_parallel/communications.py` & `tensor_parallel-1.2.6/src/tensor_parallel/communications.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.5/src/tensor_parallel/config.py` & `tensor_parallel-1.2.6/src/tensor_parallel/config.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.5/src/tensor_parallel/cross_device_ops.py` & `tensor_parallel-1.2.6/src/tensor_parallel/cross_device_ops.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.5/src/tensor_parallel/dispatch.py` & `tensor_parallel-1.2.6/src/tensor_parallel/dispatch.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,17 +34,19 @@
 
 
 def infer_sharded_data_device_id(name: str):
     if name.find("_sanity_check_params.") != -1:
         shard_id_start = name.find("_sanity_check_params.") + len("_sanity_check_params.")
     elif name.find("module_shards.") != -1:
         shard_id_start = name.find("module_shards.") + len("module_shards.")
+    elif name.find("flat_shards.") != -1:
+        shard_id_start = name.find("flat_shards.") + len("flat_shards.")
     else:
         raise KeyError(
-            "Can't decide where to put {name} in a sharded model state dict. Are you sure it's a sharded dict?"
+            f"Can't decide where to put {name}. Are you sure you passed a tensor_parallel parameter was passed?"
         )
 
     shard_id_end = name.find(".", shard_id_start)
     return int(name[shard_id_start:shard_id_end]) if shard_id_end > 0 else int(name[shard_id_start:])
 
 
 def infer_sharded_device_map(tp_model: Union[TensorParallel, TensorParallelPreTrainedModel]) -> dict:
```

### Comparing `tensor_parallel-1.2.5/src/tensor_parallel/factory.py` & `tensor_parallel-1.2.6/src/tensor_parallel/factory.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.5/src/tensor_parallel/per_device_tensors.py` & `tensor_parallel-1.2.6/src/tensor_parallel/per_device_tensors.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.5/src/tensor_parallel/pretrained_model.py` & `tensor_parallel-1.2.6/src/tensor_parallel/pretrained_model.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.5/src/tensor_parallel/shard.py` & `tensor_parallel-1.2.6/src/tensor_parallel/shard.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.5/src/tensor_parallel/sharding.py` & `tensor_parallel-1.2.6/src/tensor_parallel/sharding.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.5/src/tensor_parallel/slicing_configs.py` & `tensor_parallel-1.2.6/src/tensor_parallel/slicing_configs.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.5/src/tensor_parallel/state_actions.py` & `tensor_parallel-1.2.6/src/tensor_parallel/state_actions.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.5/src/tensor_parallel/tensor_parallel.py` & `tensor_parallel-1.2.6/src/tensor_parallel/tensor_parallel.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.5/src/tensor_parallel/utils.py` & `tensor_parallel-1.2.6/src/tensor_parallel/utils.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.5/src/tensor_parallel/wrapper.py` & `tensor_parallel-1.2.6/src/tensor_parallel/wrapper.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.5/src/tensor_parallel.egg-info/PKG-INFO` & `tensor_parallel-1.2.6/src/tensor_parallel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensor-parallel
-Version: 1.2.5
+Version: 1.2.6
 Summary: Automatically shard your large model between multiple GPUs, works without torch.distributed
 Home-page: https://github.com/BlackSamorez/tensor_parallel
 Author: Andrei Panferov and Yaroslav Lisnyak
 Author-email: yalisnyak@nes.com
 Project-URL: Bug Tracker, https://github.com/BlackSamorez/tensor_parallel/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tensor-parallel Version: 1.2.5 Summary:
+Metadata-Version: 2.1 Name: tensor-parallel Version: 1.2.6 Summary:
 Automatically shard your large model between multiple GPUs, works without
 torch.distributed Home-page: https://github.com/BlackSamorez/tensor_parallel
 Author: Andrei Panferov and Yaroslav Lisnyak Author-email: yalisnyak@nes.com
 Project-URL: Bug Tracker, https://github.com/BlackSamorez/tensor_parallel/
 issues Classifier: Development Status :: 4 - Beta Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
```

### Comparing `tensor_parallel-1.2.5/src/tensor_parallel.egg-info/SOURCES.txt` & `tensor_parallel-1.2.6/src/tensor_parallel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.5/tests/test_basic.py` & `tensor_parallel-1.2.6/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.5/tests/test_factory.py` & `tensor_parallel-1.2.6/tests/test_factory.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.5/tests/test_integration.py` & `tensor_parallel-1.2.6/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.5/tests/test_saving.py` & `tensor_parallel-1.2.6/tests/test_saving.py`

 * *Files 9% similar despite different names*

```diff
@@ -99,35 +99,55 @@
         model_tp = TensorParallelPreTrainedModel(model, devices)
     else:
         model_tp = TensorParallel(model, devices)
 
     model_tp.load_state_dict(model_tp.state_dict())
 
 
+def get_tensor_parallel(model: torch.nn.Module, devices, pretrained: bool, zero3: bool):
+    if pretrained:
+        model_tp = TensorParallelPreTrainedModel(model, devices)
+        if zero3:
+            model_tp.wrapped_model = Sharded(model_tp.wrapped_model)
+    else:
+        model_tp = TensorParallel(model, devices)
+        if zero3:
+            model_tp = Sharded(model_tp)
+    return model_tp
+
+
 @pytest.mark.parametrize("devices", [("cpu",) * 2, ("cpu",) * 3])
 @pytest.mark.parametrize(
     "model_name", ["bert-base-uncased", "hf-internal-testing/tiny-random-t5", "hf-internal-testing/tiny-random-bloom"]
 )
-@pytest.mark.parametrize("pretrained", [True])
-def test_save_shards_load_shards(devices, model_name, pretrained):
+@pytest.mark.parametrize("pretrained", [True, False])
+@pytest.mark.parametrize("zero3", [True, False])
+@pytest.mark.parametrize("meta", [True, False])
+def test_save_shards_load_shards(devices, model_name, pretrained, zero3, meta):
     devices = [torch.device(device) for device in devices]
 
     model = AutoModel.from_pretrained(model_name).to(devices[0]).half()
-    shraded_class = TensorParallelPreTrainedModel if pretrained else TensorParallel
-    model_tp = shraded_class(model, devices)
+    model_tp = get_tensor_parallel(model, devices, pretrained, zero3)
 
     if pretrained:
         half_the_model = f"{sum([p.numel() for p in model_tp.parameters()]) // 1_000_000 // 2}MB"
         model_tp.save_pretrained(PATH_TO_SAVE, max_shard_size=half_the_model)
     else:
         torch.save(model_tp.state_dict(), PATH_TO_SAVE + "test_save_shards_load_shards.bin")
     del model_tp
 
-    with init_empty_weights():
-        model_tp = shraded_class(AutoModel.from_config(AutoConfig.from_pretrained(model_name)).half(), devices)
+    if meta:
+        if zero3:
+            pytest.skip("Can't use zero3 with meta")
+        with init_empty_weights():
+            model_tp = get_tensor_parallel(
+                AutoModel.from_config(AutoConfig.from_pretrained(model_name)).half(), devices, pretrained, zero3
+            )
+    else:
+        model_tp = get_tensor_parallel(AutoModel.from_pretrained(model_name).half(), devices, pretrained, zero3)
 
     checkpoint = PATH_TO_SAVE + ("pytorch_model.bin.index.json" if pretrained else "test_save_shards_load_shards.bin")
     load_checkpoint_in_model(
         model_tp,
         checkpoint=checkpoint,
         device_map=infer_sharded_device_map(model_tp),
     )
```

### Comparing `tensor_parallel-1.2.5/tests/test_transformers.py` & `tensor_parallel-1.2.6/tests/test_transformers.py`

 * *Files identical despite different names*

