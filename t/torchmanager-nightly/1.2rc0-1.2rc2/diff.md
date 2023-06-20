# Comparing `tmp/torchmanager_nightly-1.2rc0.tar.gz` & `tmp/torchmanager_nightly-1.2rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchmanager_nightly-1.2rc0.tar", max compression
+gzip compressed data, was "torchmanager_nightly-1.2rc2.tar", max compression
```

## Comparing `torchmanager_nightly-1.2rc0.tar` & `torchmanager_nightly-1.2rc2.tar`

### file list

```diff
@@ -1,50 +1,52 @@
--rw-r--r--   0        0        0     1318 2023-03-14 14:54:20.813363 torchmanager_nightly-1.2rc0/LICENSE
--rw-r--r--   0        0        0      670 2023-06-09 15:04:44.567465 torchmanager_nightly-1.2rc0/pyproject.toml
--rw-r--r--   0        0        0      290 2023-06-09 15:04:44.567870 torchmanager_nightly-1.2rc0/torchmanager/__init__.py
--rw-r--r--   0        0        0    11928 2023-06-09 15:04:44.568285 torchmanager_nightly-1.2rc0/torchmanager/basic.py
--rw-r--r--   0        0        0      638 2023-06-09 15:04:44.568657 torchmanager_nightly-1.2rc0/torchmanager/callbacks/__init__.py
--rw-r--r--   0        0        0     4444 2023-06-09 15:04:44.568985 torchmanager_nightly-1.2rc0/torchmanager/callbacks/callback.py
--rw-r--r--   0        0        0     4628 2023-06-01 19:00:58.329930 torchmanager_nightly-1.2rc0/torchmanager/callbacks/ckpt.py
--rw-r--r--   0        0        0     3523 2023-06-01 19:00:58.330042 torchmanager_nightly-1.2rc0/torchmanager/callbacks/dynamic.py
--rw-r--r--   0        0        0     1608 2023-06-01 19:00:58.330150 torchmanager_nightly-1.2rc0/torchmanager/callbacks/early_stop.py
--rw-r--r--   0        0        0     4642 2023-06-09 15:04:44.569313 torchmanager_nightly-1.2rc0/torchmanager/callbacks/experiment.py
--rw-r--r--   0        0        0     2224 2023-06-01 19:00:58.330768 torchmanager_nightly-1.2rc0/torchmanager/callbacks/lr.py
--rw-r--r--   0        0        0     2599 2023-06-09 15:04:44.569694 torchmanager_nightly-1.2rc0/torchmanager/callbacks/tensorboard.py
--rw-r--r--   0        0        0      586 2023-06-09 15:04:44.570009 torchmanager_nightly-1.2rc0/torchmanager/compatibility.py
--rw-r--r--   0        0        0       26 2023-06-09 15:04:44.570282 torchmanager_nightly-1.2rc0/torchmanager/configs/__init__.py
--rw-r--r--   0        0        0     2980 2023-06-09 15:04:44.570764 torchmanager_nightly-1.2rc0/torchmanager/configs/basic.py
--rw-r--r--   0        0        0       85 2023-06-01 19:00:58.331061 torchmanager_nightly-1.2rc0/torchmanager/data/__init__.py
--rw-r--r--   0        0        0     6968 2023-06-09 15:04:44.571103 torchmanager_nightly-1.2rc0/torchmanager/data/dataset.py
--rw-r--r--   0        0        0     2238 2023-06-09 15:04:44.571417 torchmanager_nightly-1.2rc0/torchmanager/data/sliding.py
--rw-r--r--   0        0        0      156 2023-06-09 15:04:44.571764 torchmanager_nightly-1.2rc0/torchmanager/losses/__init__.py
--rw-r--r--   0        0        0     5557 2023-06-09 15:04:44.572050 torchmanager_nightly-1.2rc0/torchmanager/losses/cross_entropy.py
--rw-r--r--   0        0        0     1047 2023-06-09 15:04:44.572372 torchmanager_nightly-1.2rc0/torchmanager/losses/dice.py
--rw-r--r--   0        0        0     5740 2023-06-09 15:04:44.572701 torchmanager_nightly-1.2rc0/torchmanager/losses/loss.py
--rw-r--r--   0        0        0     3156 2023-06-09 15:04:44.573084 torchmanager_nightly-1.2rc0/torchmanager/losses/mse.py
--rw-r--r--   0        0        0      351 2023-06-09 15:04:44.573433 torchmanager_nightly-1.2rc0/torchmanager/metrics/__init__.py
--rw-r--r--   0        0        0     4145 2023-06-09 15:04:44.573765 torchmanager_nightly-1.2rc0/torchmanager/metrics/accuracy.py
--rw-r--r--   0        0        0     3769 2023-06-09 15:04:44.574052 torchmanager_nightly-1.2rc0/torchmanager/metrics/conf_met.py
--rw-r--r--   0        0        0     5139 2023-06-09 15:04:44.574289 torchmanager_nightly-1.2rc0/torchmanager/metrics/extractor.py
--rw-r--r--   0        0        0     2070 2023-06-09 15:04:44.574441 torchmanager_nightly-1.2rc0/torchmanager/metrics/iou.py
--rw-r--r--   0        0        0     3937 2023-06-09 15:04:44.574746 torchmanager_nightly-1.2rc0/torchmanager/metrics/metric.py
--rw-r--r--   0        0        0     2307 2023-06-09 15:04:44.574988 torchmanager_nightly-1.2rc0/torchmanager/metrics/similarity.py
--rw-r--r--   0        0        0     8710 2023-06-09 15:04:44.575236 torchmanager_nightly-1.2rc0/torchmanager/testing.py
--rw-r--r--   0        0        0       96 2023-06-09 15:04:44.575522 torchmanager_nightly-1.2rc0/torchmanager/train/__init__.py
--rw-r--r--   0        0        0     4964 2023-06-01 19:00:58.336017 torchmanager_nightly-1.2rc0/torchmanager/train/checkpoint.py
--rw-r--r--   0        0        0      694 2023-06-09 15:04:44.575804 torchmanager_nightly-1.2rc0/torchmanager/train/learning_rate.py
--rw-r--r--   0        0        0    13483 2023-06-09 15:04:44.576140 torchmanager_nightly-1.2rc0/torchmanager/training.py
--rw-r--r--   0        0        0      459 2023-06-09 15:04:44.576450 torchmanager_nightly-1.2rc0/torchmanager_core/__init__.py
--rw-r--r--   0        0        0      109 2023-06-09 15:04:44.576756 torchmanager_nightly-1.2rc0/torchmanager_core/devices/__init__.py
--rw-r--r--   0        0        0     4879 2023-06-09 15:04:44.576905 torchmanager_nightly-1.2rc0/torchmanager_core/devices/device.py
--rw-r--r--   0        0        0      264 2023-06-01 19:00:58.337503 torchmanager_nightly-1.2rc0/torchmanager_core/devices/protocols.py
--rw-r--r--   0        0        0      153 2023-06-01 19:00:58.337794 torchmanager_nightly-1.2rc0/torchmanager_core/errors/__init__.py
--rw-r--r--   0        0        0      350 2023-06-01 19:00:58.338065 torchmanager_nightly-1.2rc0/torchmanager_core/errors/runtime.py
--rw-r--r--   0        0        0      669 2023-06-01 19:00:58.338329 torchmanager_nightly-1.2rc0/torchmanager_core/errors/train.py
--rw-r--r--   0        0        0     3076 2023-06-09 15:04:44.577160 torchmanager_nightly-1.2rc0/torchmanager_core/protocols.py
--rw-r--r--   0        0        0       44 2023-06-09 15:04:44.577391 torchmanager_nightly-1.2rc0/torchmanager_core/random/__init__.py
--rw-r--r--   0        0        0     1029 2023-06-09 15:04:44.577618 torchmanager_nightly-1.2rc0/torchmanager_core/random/seed.py
--rw-r--r--   0        0        0      204 2023-06-01 19:00:58.338499 torchmanager_nightly-1.2rc0/torchmanager_core/typing.py
--rw-r--r--   0        0        0     6017 2023-06-09 15:04:48.647525 torchmanager_nightly-1.2rc0/torchmanager_core/version.py
--rw-r--r--   0        0        0      439 2023-06-09 15:04:44.578258 torchmanager_nightly-1.2rc0/torchmanager_core/view/__init__.py
--rw-r--r--   0        0        0      313 2023-06-01 19:00:58.338878 torchmanager_nightly-1.2rc0/torchmanager_core/view/protocols.py
--rw-r--r--   0        0        0      691 1970-01-01 00:00:00.000000 torchmanager_nightly-1.2rc0/PKG-INFO
+-rw-r--r--   0        0        0     1318 2023-06-12 21:40:08.180158 torchmanager_nightly-1.2rc2/LICENSE
+-rw-r--r--   0        0        0      673 2023-06-20 19:58:26.515706 torchmanager_nightly-1.2rc2/pyproject.toml
+-rw-r--r--   0        0        0      283 2023-06-20 19:58:26.515867 torchmanager_nightly-1.2rc2/torchmanager/__init__.py
+-rw-r--r--   0        0        0    13349 2023-06-20 19:58:26.516087 torchmanager_nightly-1.2rc2/torchmanager/basic.py
+-rw-r--r--   0        0        0      638 2023-06-20 19:58:26.516486 torchmanager_nightly-1.2rc2/torchmanager/callbacks/__init__.py
+-rw-r--r--   0        0        0     4444 2023-06-20 19:58:26.516689 torchmanager_nightly-1.2rc2/torchmanager/callbacks/callback.py
+-rw-r--r--   0        0        0     4650 2023-06-20 19:58:26.516875 torchmanager_nightly-1.2rc2/torchmanager/callbacks/ckpt.py
+-rw-r--r--   0        0        0     3523 2023-06-19 18:22:49.443147 torchmanager_nightly-1.2rc2/torchmanager/callbacks/dynamic.py
+-rw-r--r--   0        0        0     1984 2023-06-20 19:58:32.114054 torchmanager_nightly-1.2rc2/torchmanager/callbacks/early_stop.py
+-rw-r--r--   0        0        0     4642 2023-06-20 19:58:26.517436 torchmanager_nightly-1.2rc2/torchmanager/callbacks/experiment.py
+-rw-r--r--   0        0        0     2224 2023-06-19 18:22:49.443597 torchmanager_nightly-1.2rc2/torchmanager/callbacks/lr.py
+-rw-r--r--   0        0        0     2599 2023-06-20 19:58:26.517599 torchmanager_nightly-1.2rc2/torchmanager/callbacks/tensorboard.py
+-rw-r--r--   0        0        0      586 2023-06-20 19:58:26.517762 torchmanager_nightly-1.2rc2/torchmanager/compatibility.py
+-rw-r--r--   0        0        0       26 2023-06-20 19:58:26.517963 torchmanager_nightly-1.2rc2/torchmanager/configs/__init__.py
+-rw-r--r--   0        0        0     2980 2023-06-20 19:58:26.518077 torchmanager_nightly-1.2rc2/torchmanager/configs/basic.py
+-rw-r--r--   0        0        0       85 2023-06-19 18:22:49.443994 torchmanager_nightly-1.2rc2/torchmanager/data/__init__.py
+-rw-r--r--   0        0        0     6968 2023-06-20 19:58:26.518538 torchmanager_nightly-1.2rc2/torchmanager/data/dataset.py
+-rw-r--r--   0        0        0     2238 2023-06-20 19:58:26.518760 torchmanager_nightly-1.2rc2/torchmanager/data/sliding.py
+-rw-r--r--   0        0        0      156 2023-06-20 19:58:26.518937 torchmanager_nightly-1.2rc2/torchmanager/losses/__init__.py
+-rw-r--r--   0        0        0     5557 2023-06-20 19:58:26.519118 torchmanager_nightly-1.2rc2/torchmanager/losses/cross_entropy.py
+-rw-r--r--   0        0        0     1047 2023-06-20 19:58:26.519270 torchmanager_nightly-1.2rc2/torchmanager/losses/dice.py
+-rw-r--r--   0        0        0     5740 2023-06-20 19:58:26.519444 torchmanager_nightly-1.2rc2/torchmanager/losses/loss.py
+-rw-r--r--   0        0        0     3156 2023-06-20 19:58:26.519597 torchmanager_nightly-1.2rc2/torchmanager/losses/mse.py
+-rw-r--r--   0        0        0      351 2023-06-20 19:58:26.519753 torchmanager_nightly-1.2rc2/torchmanager/metrics/__init__.py
+-rw-r--r--   0        0        0     4145 2023-06-20 19:58:26.519912 torchmanager_nightly-1.2rc2/torchmanager/metrics/accuracy.py
+-rw-r--r--   0        0        0     3769 2023-06-20 19:58:26.520077 torchmanager_nightly-1.2rc2/torchmanager/metrics/conf_met.py
+-rw-r--r--   0        0        0     5139 2023-06-20 19:58:26.520223 torchmanager_nightly-1.2rc2/torchmanager/metrics/extractor.py
+-rw-r--r--   0        0        0     2070 2023-06-20 19:58:26.520381 torchmanager_nightly-1.2rc2/torchmanager/metrics/iou.py
+-rw-r--r--   0        0        0     3981 2023-06-20 19:58:26.520964 torchmanager_nightly-1.2rc2/torchmanager/metrics/metric.py
+-rw-r--r--   0        0        0     2307 2023-06-20 19:58:26.521124 torchmanager_nightly-1.2rc2/torchmanager/metrics/similarity.py
+-rw-r--r--   0        0        0     8710 2023-06-20 19:58:26.521356 torchmanager_nightly-1.2rc2/torchmanager/testing.py
+-rw-r--r--   0        0        0       96 2023-06-20 19:58:26.521538 torchmanager_nightly-1.2rc2/torchmanager/train/__init__.py
+-rw-r--r--   0        0        0       43 2023-06-20 19:58:26.521666 torchmanager_nightly-1.2rc2/torchmanager/train/checkpoint.py
+-rw-r--r--   0        0        0      763 2023-06-20 19:58:26.521813 torchmanager_nightly-1.2rc2/torchmanager/train/learning_rate.py
+-rw-r--r--   0        0        0    12779 2023-06-20 19:58:26.522035 torchmanager_nightly-1.2rc2/torchmanager/training.py
+-rw-r--r--   0        0        0      471 2023-06-20 19:58:26.522203 torchmanager_nightly-1.2rc2/torchmanager_core/__init__.py
+-rw-r--r--   0        0        0       52 2023-06-20 19:58:26.522330 torchmanager_nightly-1.2rc2/torchmanager_core/checkpoint/__init__.py
+-rw-r--r--   0        0        0     5015 2023-06-20 19:58:26.522442 torchmanager_nightly-1.2rc2/torchmanager_core/checkpoint/ckpt.py
+-rw-r--r--   0        0        0      109 2023-06-20 19:58:26.522600 torchmanager_nightly-1.2rc2/torchmanager_core/devices/__init__.py
+-rw-r--r--   0        0        0     4935 2023-06-20 19:58:26.522809 torchmanager_nightly-1.2rc2/torchmanager_core/devices/device.py
+-rw-r--r--   0        0        0      264 2023-06-19 18:22:49.446899 torchmanager_nightly-1.2rc2/torchmanager_core/devices/protocols.py
+-rw-r--r--   0        0        0      153 2023-06-19 18:22:49.447053 torchmanager_nightly-1.2rc2/torchmanager_core/errors/__init__.py
+-rw-r--r--   0        0        0      351 2023-06-20 19:58:26.522973 torchmanager_nightly-1.2rc2/torchmanager_core/errors/runtime.py
+-rw-r--r--   0        0        0      669 2023-06-19 18:22:49.447258 torchmanager_nightly-1.2rc2/torchmanager_core/errors/train.py
+-rw-r--r--   0        0        0     3687 2023-06-20 19:58:26.523137 torchmanager_nightly-1.2rc2/torchmanager_core/protocols.py
+-rw-r--r--   0        0        0       44 2023-06-20 19:58:26.523280 torchmanager_nightly-1.2rc2/torchmanager_core/random/__init__.py
+-rw-r--r--   0        0        0     1029 2023-06-20 19:58:26.523379 torchmanager_nightly-1.2rc2/torchmanager_core/random/seed.py
+-rw-r--r--   0        0        0      204 2023-06-19 18:22:49.447474 torchmanager_nightly-1.2rc2/torchmanager_core/typing.py
+-rw-r--r--   0        0        0     7360 2023-06-20 19:58:26.523557 torchmanager_nightly-1.2rc2/torchmanager_core/version.py
+-rw-r--r--   0        0        0      476 2023-06-20 19:58:26.523817 torchmanager_nightly-1.2rc2/torchmanager_core/view/__init__.py
+-rw-r--r--   0        0        0      313 2023-06-19 18:22:49.447867 torchmanager_nightly-1.2rc2/torchmanager_core/view/protocols.py
+-rw-r--r--   0        0        0      693 1970-01-01 00:00:00.000000 torchmanager_nightly-1.2rc2/PKG-INFO
```

### Comparing `torchmanager_nightly-1.2rc0/LICENSE` & `torchmanager_nightly-1.2rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2rc0/pyproject.toml` & `torchmanager_nightly-1.2rc2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "torchmanager-nightly"
-version = "1.2rc"
-description = "PyTorch Training Manager v1.2 (Release Candidate)"
+version = "1.2rc2"
+description = "PyTorch Training Manager v1.2 (Release Candidate 2)"
 authors = ["Qisheng He <Qisheng.He@wayne.edu>"]
 repository = "https://github.com/kisonho/torchmanager.git"
 packages = [
     { include = "torchmanager" },
     { include = "torchmanager_core" },
 ]
```

### Comparing `torchmanager_nightly-1.2rc0/torchmanager/basic.py` & `torchmanager_nightly-1.2rc2/torchmanager/basic.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from torchmanager_core import devices, torch, Version, deprecated, _raise, API_VERSION, VERSION as CURRENT_VERSION
-from torchmanager_core.protocols import VersionConvertible
+from torchmanager_core import devices, errors, torch, Version, deprecated, API_VERSION, VERSION as CURRENT_VERSION
+from torchmanager_core.checkpoint import Checkpoint
+from torchmanager_core.protocols import Resulting, VersionConvertible
 from torchmanager_core.typing import Any, Collection, Dict, Generic, List, Module, Optional, OrderedDict, Self, Tuple, Union
 
 from .losses import Loss, MultiLosses, ParallelLoss
 from .metrics import Metric
-from .train import Checkpoint
 
 
 class BaseManager(Generic[Module]):
     """
     The basic manager
 
     * Implements: `torchmanager_core.devices.DeviceMovable`, `.callbacks.protocols.ModelContainer`
@@ -39,39 +39,44 @@
         - metrics: A `dict` of metrics with a name in `str` as keys and a `Metric` as values
         - model: A target `torch.nn.Module` to be trained
         - optimizer: A `torch.optim.Optimizer` to train the model
         - raw_loss_fn: An optional `Loss` of the non-paralleled loss function
         - raw_model: A non-paralleled target `torch.nn.Module` model
     """
     # properties
-    loss_fn: Optional[Union[Loss, ParallelLoss]]
-    metric_fns: Dict[str, Metric]
+    loss_fn: Optional[Resulting]
+    """The optional main loss function in `Resulting`"""
+    metric_fns: Dict[str, Resulting]
+    """A `dict` of the metric functions with names as keys in `str` and metric functions as values in `torch.metrics.Metric`"""
     model: Union[Module, torch.nn.DataParallel]
     optimizer: Optional[torch.optim.Optimizer]
     version: Version
 
     @property
     def compiled(self) -> bool:
+        """The `bool` flag of if this manager has been compiled"""
         return True if self.loss_fn is not None and self.optimizer is not None else False
 
     @property
-    def raw_loss_fn(self) -> Optional[Loss]:
+    def raw_loss_fn(self) -> Optional[Resulting]:
+        """The `torchmanager.losses.Loss` controlled by this manager without `torch.nn.DataParallel` wrap"""
         if self.loss_fn is None:
             return self.loss_fn
         elif isinstance(self.loss_fn, ParallelLoss):
             return self.loss_fn.module
         elif isinstance(self.loss_fn._metric_fn, torch.nn.parallel.DataParallel):
             self.loss_fn._metric_fn = self.loss_fn._metric_fn.module
             return self.loss_fn
         else:
             return self.loss_fn
 
     @property
     def raw_model(self) -> Module:
-        return self.model.module if isinstance(self.model, torch.nn.parallel.DataParallel) else self.model  # type: ignore
+        """The `Module` controlled by this manager without `torch.nn.DataParallel` wrap"""
+        return self.model.module if isinstance(self.model, torch.nn.DataParallel) else self.model  # type: ignore
 
     def __init__(self, model: Module, optimizer: Optional[torch.optim.Optimizer] = None, loss_fn: Optional[Union[Loss, Dict[str, Loss]]] = None, metrics: Dict[str, Metric] = {}) -> None:
         """
         Constructor
 
         - Parameters:
             - loss_fn: An optional `Loss` object to calculate the loss for single loss or a `dict` of losses in `Loss` with their names in `str` to calculate multiple losses
@@ -118,24 +123,51 @@
         - Parameters:
             - loss_fn: A `Loss` object to calculate the loss for single loss or a `dict` of losses in `Loss` with their names in `str` to calculate multiple losses
             - metrics: A `dict` of metrics with a name in `str` and a `Metric` object to calculate the metric
             - optimizer: A `torch.optim.Optimizer` to train the model
         """
         self._compile(optimizer, loss_fn, metrics)
 
+    def convert(self, from_version: Version) -> None:
+        """
+        Convert from a version to current version
+
+        - Parameters:
+            - from_version: A `torchmanager.version.Version` to convert from
+        """
+        # check manager version
+        if from_version < API_VERSION:
+            # convert loss version
+            if isinstance(self.raw_loss_fn, VersionConvertible):
+                self.raw_loss_fn.convert(from_version)
+        
+            # convert metrics version
+            for m in self.metric_fns.items():
+                if isinstance(m, VersionConvertible):
+                    m.convert(from_version)
+
+            # set version
+            self.version = API_VERSION
+
     def data_parallel(self, target_devices: List[torch.device]) -> bool:
         """
         Data parallel all available models
 
         - Parameters:
             - target_devices: The target multiple devices for data parallel
         - Returns: A `bool` flag of if use multi GPUs
         """
+        # multi gpus support for loss
+        assert isinstance(self.raw_loss_fn, Loss), errors._raise(TypeError("The loss function is not a valid `Loss` object."))
+        paralleled_loss_fn, use_multi_gpus = devices.data_parallel(self.raw_loss_fn, devices=target_devices, parallel_type=ParallelLoss)
+        assert isinstance(paralleled_loss_fn, ParallelLoss) or isinstance(paralleled_loss_fn, Loss), errors._raise(TypeError("Paralleled function is not a valid `ParallelLoss` or `Loss` after parallel."))
+        self.loss_fn = paralleled_loss_fn
+
         # multi gpus support for model
-        self.model, use_multi_gpus = devices.data_parallel(self.model, devices=target_devices)
+        self.model, use_multi_gpus = devices.data_parallel(self.raw_model, devices=target_devices)
         return use_multi_gpus
 
     @classmethod
     def from_checkpoint(cls, ckpt: Union[Checkpoint[Any], str], map_location: Optional[torch.device] = None):
         """
         Method to load a manager from a saved `Checkpoint`. The manager will not be compiled with a loss function and its metrics.
 
@@ -153,62 +185,52 @@
             manager = cls(ckpt.model, ckpt.optimizer, loss_fn=ckpt.loss_fn, metrics=ckpt.metrics)  # type: ignore
         elif isinstance(ckpt.model, BaseManager):
             manager = ckpt.model
             if isinstance(manager.model, torch.nn.parallel.DataParallel):
                 manager.model = manager.model.module
             if manager.loss_fn is not None and hasattr(manager.loss_fn, "_metric_fn"):
                 if isinstance(manager.loss_fn._metric_fn, torch.nn.parallel.DataParallel):
-                    assert isinstance(manager.loss_fn._metric_fn.module, Loss), _raise(TypeError("Loss function is not a valid `Loss`."))
+                    assert isinstance(manager.loss_fn._metric_fn.module, Loss), errors._raise(TypeError("Loss function is not a valid `Loss`."))
                     manager.loss_fn = manager.loss_fn._metric_fn.module
             else:
                 manager.loss_fn = None
         else:
             raise TypeError(f"The saved checkpoint contains a model with type of {type(ckpt.model)} that cannot be recoverred to a `Manager`.")
         
         # initialize manager version
         if not hasattr(manager, "version"):
             manager.version = Version("v1.0")
 
-        # check manager version
-        if manager.version < API_VERSION:
-            if isinstance(manager.raw_loss_fn, VersionConvertible):
-                manager.raw_loss_fn.convert(manager.version)
-        
-            # convert metrics version
-            for m in manager.metric_fns.items():
-                if isinstance(m, VersionConvertible):
-                    m.convert(manager.version)
-
-        # set to current version
-        manager.version = CURRENT_VERSION
+        # convert to current version
+        manager.convert(manager.version)
         return manager
 
     def load_state_dict(self, state_dict: OrderedDict[str, Any], strict: bool = True) -> None:
         # load state dict elements
-        assert "model" in state_dict, _raise(KeyError("The given dictionary does not have 'model' element."))
-        assert "optimizer" in state_dict, _raise(KeyError("The given dictionary does not have 'optimizer' element."))
-        assert "loss_fn" in state_dict, _raise(KeyError("The given dictionary does not have 'loss_fn' element."))
-        assert "metrics" in state_dict, _raise(KeyError("The given dictionary does not have 'metrics' element."))
+        assert "model" in state_dict, errors._raise(KeyError("The given dictionary does not have 'model' element."))
+        assert "optimizer" in state_dict, errors._raise(KeyError("The given dictionary does not have 'optimizer' element."))
+        assert "loss_fn" in state_dict, errors._raise(KeyError("The given dictionary does not have 'loss_fn' element."))
+        assert "metrics" in state_dict, errors._raise(KeyError("The given dictionary does not have 'metrics' element."))
         model: OrderedDict[str, Any] = state_dict["model"]
         optimizer: Optional[Dict[str, Any]] = state_dict["optimizer"]
         loss_fn: Optional[OrderedDict[str, Any]] = state_dict["loss_fn"]
         metrics: Dict[str, OrderedDict[str, Any]] = state_dict["metrics"]
 
         # load state dict to current model, optimizer, loss_fn, and metrics
         self.model.load_state_dict(model, strict=strict)  # type: ignore
         if optimizer is not None:
-            assert self.optimizer is not None, _raise(ValueError("The manager has not been compiled with 'optimizer' given."))
+            assert self.optimizer is not None, errors._raise(ValueError("The manager has not been compiled with 'optimizer' given."))
             self.optimizer.load_state_dict(optimizer)
         if loss_fn is not None:
-            assert self.loss_fn is not None, _raise(ValueError("The manager has not been compiled with 'loss_fn' given."))
-            self.loss_fn.load_state_dict(loss_fn)
-        assert metrics is not None, _raise(ValueError("The given dictionary must have 'metrics' element not to be None."))
+            assert self.loss_fn is not None, errors._raise(ValueError("The manager has not been compiled with 'loss_fn' given."))
+            self.loss_fn.load_state_dict(state_dict=loss_fn)
+        assert metrics is not None, errors._raise(ValueError("The given dictionary must have 'metrics' element not to be None."))
         for k, m in metrics.items():
-            assert k in self.metric_fns, _raise(KeyError(f"The manager does not have a metric named '{k}'."))
-            self.metric_fns[k].load_state_dict(m)
+            assert k in self.metric_fns, errors._raise(KeyError(f"The manager does not have a metric named '{k}'."))
+            self.metric_fns[k].load_state_dict(state_dict=m)
 
     def reset(self, cpu: torch.device = devices.CPU) -> None:
         """
         Reset model and loss functions, move all to CPU and empty device cache
 
         - Parameters:
             - cpu: The CPU in `torch.device`
```

### Comparing `torchmanager_nightly-1.2rc0/torchmanager/callbacks/__init__.py` & `torchmanager_nightly-1.2rc2/torchmanager/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2rc0/torchmanager/callbacks/callback.py` & `torchmanager_nightly-1.2rc2/torchmanager/callbacks/callback.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2rc0/torchmanager/callbacks/ckpt.py` & `torchmanager_nightly-1.2rc2/torchmanager/callbacks/ckpt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from torchmanager_core import os, torch, _raise
+from torchmanager_core.checkpoint import Checkpoint as Ckpt
 from torchmanager_core.protocols import ModelContainer, MonitorType, StateDictLoadable
 from torchmanager_core.typing import Any, Dict, Generic, Optional, TypeVar
 
-from ..train import Checkpoint as Ckpt
 from .callback import Callback
 
 T = TypeVar('T', bound=StateDictLoadable)
 
 class _Checkpoint(Callback, Generic[T]):
     """
     The callback to save the last checkpoint during training
@@ -124,8 +124,8 @@
             best_ckpt: Ckpt[StateDictLoadable] = Ckpt.from_saved(self.ckpt_path)
 
             # load to model
             if isinstance(best_ckpt.model, ModelContainer):
                 ckpt_model = best_ckpt.model.model
             else: ckpt_model = best_ckpt.model
             try: model.load_state_dict(ckpt_model.state_dict())
-            except: raise TypeError(f"Reload best checkpoint to model failed: supposed to have {type(model)} in checkpoint, got {type(ckpt_model)}.")
+            except: raise TypeError(f"Reload best checkpoint to model failed: supposed to have {type(model)} in checkpoint, got {type(ckpt_model)}.")
```

### Comparing `torchmanager_nightly-1.2rc0/torchmanager/callbacks/dynamic.py` & `torchmanager_nightly-1.2rc2/torchmanager/callbacks/dynamic.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2rc0/torchmanager/callbacks/early_stop.py` & `torchmanager_nightly-1.2rc2/torchmanager/callbacks/early_stop.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,15 +26,21 @@
         self.__metrics = [sys.float_info.min if monitor_type == MonitorType.MAX else sys.float_info.max]
         self.monitor = monitor
         self.monitor_type = monitor_type
         self.steps = steps
 
     def on_epoch_end(self, epoch: int, summary: Dict[str, float] = ..., val_summary: Optional[Dict[str, float]] = None) -> None:
         # load monitoring value
-        if val_summary is not None: summary = val_summary
+        summary = val_summary if val_summary is not None else summary
         monitoring_value = summary[self.monitor]
 
         # compare with recorded metrics
-        max_value = max(self.__metrics)
-        if monitoring_value < max_value and len(self._metrics) >= self.steps: raise errors.StopTraining(epoch)
-        elif len(self._metrics) >= self.steps: self._metrics.pop()
-        self._metrics.insert(0, monitoring_value)
+        value = self._metrics[0]
+        if self.monitor_type == MonitorType.MAX and monitoring_value <= value and len(self._metrics) >= self.steps:
+            raise errors.StopTraining(epoch)
+        elif self.monitor_type == MonitorType.MAX and monitoring_value > value:
+            self._metrics.clear()
+        elif self.monitor_type == MonitorType.MIN and monitoring_value >= value and len(self._metrics) >= self.steps:
+            raise errors.StopTraining(epoch)
+        elif self.monitor_type == MonitorType.MIN and monitoring_value < value:
+            self._metrics.clear()
+        self._metrics.append(monitoring_value)
```

### Comparing `torchmanager_nightly-1.2rc0/torchmanager/callbacks/experiment.py` & `torchmanager_nightly-1.2rc2/torchmanager/callbacks/experiment.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2rc0/torchmanager/callbacks/lr.py` & `torchmanager_nightly-1.2rc2/torchmanager/callbacks/lr.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2rc0/torchmanager/callbacks/tensorboard.py` & `torchmanager_nightly-1.2rc2/torchmanager/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2rc0/torchmanager/compatibility.py` & `torchmanager_nightly-1.2rc2/torchmanager/compatibility.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2rc0/torchmanager/configs/basic.py` & `torchmanager_nightly-1.2rc2/torchmanager/configs/basic.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2rc0/torchmanager/data/dataset.py` & `torchmanager_nightly-1.2rc2/torchmanager/data/dataset.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2rc0/torchmanager/data/sliding.py` & `torchmanager_nightly-1.2rc2/torchmanager/data/sliding.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2rc0/torchmanager/losses/cross_entropy.py` & `torchmanager_nightly-1.2rc2/torchmanager/losses/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2rc0/torchmanager/losses/dice.py` & `torchmanager_nightly-1.2rc2/torchmanager/losses/dice.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2rc0/torchmanager/losses/loss.py` & `torchmanager_nightly-1.2rc2/torchmanager/losses/loss.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2rc0/torchmanager/losses/mse.py` & `torchmanager_nightly-1.2rc2/torchmanager/losses/mse.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2rc0/torchmanager/metrics/accuracy.py` & `torchmanager_nightly-1.2rc2/torchmanager/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2rc0/torchmanager/metrics/conf_met.py` & `torchmanager_nightly-1.2rc2/torchmanager/metrics/conf_met.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2rc0/torchmanager/metrics/extractor.py` & `torchmanager_nightly-1.2rc2/torchmanager/metrics/extractor.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2rc0/torchmanager/metrics/iou.py` & `torchmanager_nightly-1.2rc2/torchmanager/metrics/iou.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2rc0/torchmanager/metrics/metric.py` & `torchmanager_nightly-1.2rc2/torchmanager/metrics/metric.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from torchmanager_core import torch, _raise
-from torchmanager_core.typing import Any, Callable, Enum, List, Optional
+from torchmanager_core.protocols import Reduction
+from torchmanager_core.typing import Any, Callable, List, Optional
 
 
 class Metric(torch.nn.Module):
     """
     The basic metric class
 
     * extends: `torch.nn.Module`
```

### Comparing `torchmanager_nightly-1.2rc0/torchmanager/metrics/similarity.py` & `torchmanager_nightly-1.2rc2/torchmanager/metrics/similarity.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2rc0/torchmanager/testing.py` & `torchmanager_nightly-1.2rc2/torchmanager/testing.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2rc0/torchmanager/train/checkpoint.py` & `torchmanager_nightly-1.2rc2/torchmanager_core/checkpoint/ckpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from torchmanager_core import os, torch, _raise
+import os, torch
 from torchmanager_core.protocols import StateDictLoadable
 from torchmanager_core.typing import Any, Dict, Generic, List, Optional, OrderedDict, TypeVar
 
 T = TypeVar("T", bound=StateDictLoadable)
 
 
 class Checkpoint(Generic[T]):
@@ -53,28 +53,29 @@
             - ckpt_path: A `str` of file path
             - model: Any object to be loaded
         """
         # load checkpint dictionary
         ckpt: Dict[str, Any] = torch.load(ckpt_path, map_location=map_location)
 
         # load model
-        if ckpt["save_weights_only"] is True:
-            assert model is not None, _raise(TypeError("Model must be given to load this checkpoint because `save_weights_only` was set to be `True`."))
+        if model is not None and ckpt["save_weights_only"] is True:
             state_dict: OrderedDict[str, Any] = ckpt["model"]
-            model.load_state_dict(state_dict)
+            model.load_state_dict(state_dict=state_dict)
             ckpt["model"] = model
+        elif model is None and ckpt["save_weights_only"] is True:
+            raise TypeError("Model must be given to load this checkpoint because `save_weights_only` was set to be `True`.")
         else:
             # remove data parallel wrap
             if isinstance(ckpt["model"], torch.nn.parallel.DataParallel):
                 ckpt["model"] = ckpt["model"].module
 
             # load model structure with checkpoint weights
             if model is not None:
                 saved_model: StateDictLoadable = ckpt["model"]  # type: ignore
-                model.load_state_dict(OrderedDict(saved_model.state_dict()))
+                model.load_state_dict(state_dict=OrderedDict(saved_model.state_dict()))
                 ckpt["model"] = model
         return cls(**ckpt)
 
     def save(self, epoch: int, ckpt_path: str) -> None:
         """
         Saves current checkpoint
```

### Comparing `torchmanager_nightly-1.2rc0/torchmanager/train/learning_rate.py` & `torchmanager_nightly-1.2rc2/torchmanager/train/learning_rate.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+from torchmanager_core import deprecated
 from torchmanager_core.protocols import LrSteping
 from torchmanager_core.typing import Dict
 
 
+@deprecated("v1.3", "v1.4")
 def update_lr(lr_scheduler: LrSteping) -> Dict[str, float]:
     """
     Update lr scheduler and returns the current learning rate as a summary
 
     - Parameters:
         - lr_scheduler: A `torch.optim.lr_scheduler._LRScheduler` to update
     - Returns: A `dict` of lr summary
```

### Comparing `torchmanager_nightly-1.2rc0/torchmanager/training.py` & `torchmanager_nightly-1.2rc2/torchmanager/training.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from torch.utils.data import DataLoader
 from torchmanager_core import devices, errors, math, torch, view, _raise
+from torchmanager_core.checkpoint import Checkpoint
 from torchmanager_core.protocols import Resulting
 from torchmanager_core.typing import Any, Collection, Dict, List, Module, Optional, Self, Union
 
 from .callbacks import Callback
 from .data import Dataset
-from .losses import Loss, ParallelLoss
+from .losses import Loss
 from .metrics import Metric
-from .train import Checkpoint
 from .testing import Manager as _Manager
 
 
 class Manager(_Manager[Module]):
     """
     A training manager
 
@@ -137,22 +137,14 @@
         - Parameters:
             - loss: A `torch.Tensor` of loss value
         """
         self.compiled_optimizer.zero_grad()
         loss.backward()
         self.compiled_optimizer.step()
 
-    def data_parallel(self, target_devices: List[torch.device]) -> bool:
-        # multi gpus support for loss
-        assert isinstance(self.compiled_losses, Loss), errors._raise(TypeError("The compiled loss function is not a valid `Loss` object."))
-        paralleled_loss_fn, use_multi_gpus = devices.data_parallel(self.compiled_losses, devices=target_devices, parallel_type=ParallelLoss)
-        assert isinstance(paralleled_loss_fn, ParallelLoss) or isinstance(paralleled_loss_fn, Loss), errors._raise(TypeError("Paralleled function is not a valid `ParallelLoss` or `Loss` after parallel."))
-        self.loss_fn = paralleled_loss_fn
-        return super().data_parallel(target_devices) and use_multi_gpus
-
     def fit(self, training_dataset: Union[DataLoader[Any], Dataset[Any], Collection], /, epochs: Optional[int] = None, val_dataset: Optional[Union[DataLoader[Any], Dataset[Any], Collection]] = None, callbacks_list: List[Callback] = [], *, iterations: Optional[int] = None, initial_epoch: Optional[int] = None, device: Optional[Union[torch.device, List[torch.device]]] = None, use_multi_gpus: bool = False, **kwargs) -> Module:
         """
         Training algorithm
 
         - Parameters:
             - training_dataset: Any kind of training dataset in `torch.utils.data.DataLoader` or `.data.Dataset`
             - epochs: An optional `int` number of training epochs (`iterations` must be not given)
```

### Comparing `torchmanager_nightly-1.2rc0/torchmanager_core/devices/device.py` & `torchmanager_nightly-1.2rc2/torchmanager_core/devices/device.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-import torch, warnings
+import torch
+import warnings
 from typing import Any, Dict, Iterable, List, Optional, Tuple, Type, TypeVar, Union
 
 from .protocols import DeviceMovable
 
 CPU = torch.device('cpu')
 '''The main CPU'''
 
@@ -23,14 +24,15 @@
 except:
     DEFAULT = CPU
     GPU = NotImplemented
     GPUS = []
 
 Module = TypeVar('Module', bound=torch.nn.Module)
 
+
 def data_parallel(raw_model: Module, /, devices: List[torch.device] = GPUS, *, output_device: Optional[torch.device] = None, parallel_type: Type = torch.nn.parallel.DataParallel) -> Tuple[Union[Module, torch.nn.parallel.DataParallel], bool]:
     """
     Make a `torch.nn.Module` data parallel
 
     - Parameters:
         - raw_model: A target `torch.nn.Module`
         - devices: A `list` of target `torch.device`
@@ -44,17 +46,20 @@
         device_ids = [d.index for d in devices]
         model = parallel_type(raw_model, device_ids=device_ids, output_device=output_device)
         return model, True
     else:
         warnings.warn(f"CUDA is not available, unable to use multi-GPUs.", ResourceWarning)
         return raw_model, False
 
+
 def empty_cache() -> None:
     """Empty CUDA cache"""
-    if GPU is not NotImplemented: torch.cuda.empty_cache()
+    if GPU is not NotImplemented:
+        torch.cuda.empty_cache()
+
 
 def search(specified: Optional[Union[torch.device, List[torch.device]]] = None) -> Tuple[torch.device, torch.device, List[torch.device]]:
     """
     Find available devices
 
     - Pameters:
         - specified: An optional `torch.device` of specified
@@ -71,33 +76,38 @@
         specified = [specified]
     elif len(specified) > 0:
         # set default device
         device = torch.device(specified[0].type)
 
         # check for each device
         for d in specified:
-            if d.type != specified[0].type: raise SystemError("All devices in the specified list must have the same device type.")
-            if d.index is None: raise SystemError("All devices in the specified list must have a device index.")
-    else: raise SystemError("Specified device list must not be empty")
+            if d.type != specified[0].type:
+                raise SystemError("All devices in the specified list must have the same device type.")
+            if d.index is None:
+                raise SystemError("All devices in the specified list must have a device index.")
+    else:
+        raise SystemError("Specified device list must not be empty")
     return CPU, device, specified
 
+
 def move_to_device(target: Union[DeviceMovable,  Dict[str, Union[DeviceMovable,  Any]], List[Union[DeviceMovable,  Any]]], /, device: torch.device, *, recursive: bool = False) -> Union[DeviceMovable,  Dict[str, Union[DeviceMovable,  Any]], List[Union[DeviceMovable,  Any]]]:
     """
     Recurrently move a target variable to device if elements perform to `DeviceMovable` protocol
-    
+
     - Parameters:
         - target: Either a target in `DeviceMovable`, a `dict` of targets in `DeviceMovable`, or a `list` of targets in `DeviceMovable`, targets in a `list` or `dict` that does not perform to `DeviceMovable` protocol will be returned without changing
         - device: A `torch.device` of target device
         - recursive: A `bool` flag of if move to device recursively
     - Returns: The same type of target but moved to target device
     """
     if isinstance(target, DeviceMovable):
         target = target.to(device)
     elif isinstance(target, dict):
         target = {k: move_to_device(t, device) if isinstance(t, DeviceMovable) or recursive else t for k, t in target.items()}
     elif isinstance(target, Iterable):
         target = [move_to_device(t, device) if isinstance(t, DeviceMovable) or recursive else t for t in target]
     return target
 
+
 def set_default(d: torch.device) -> None:
     if d.index is not None and d.type == "cuda":
-        torch.cuda.set_device(d)
+        torch.cuda.set_device(d)
```

### Comparing `torchmanager_nightly-1.2rc0/torchmanager_core/errors/train.py` & `torchmanager_nightly-1.2rc2/torchmanager_core/errors/train.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2rc0/torchmanager_core/protocols.py` & `torchmanager_nightly-1.2rc2/torchmanager_core/protocols.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import abc, torch, sys
 from enum import Enum
-from typing import Any, Dict, List, Optional, OrderedDict, Protocol, runtime_checkable
+from typing import Any, Callable, Dict, List, Optional, OrderedDict, Protocol, runtime_checkable
 from typing_extensions import Self
 
 from .devices.protocols import DeviceMovable
 from .version import Version
 from .view.protocols import VerboseControllable
 
 
@@ -77,25 +77,37 @@
 
 class Reduction(Enum):
     NONE = 0
     MEAN = 1
     SUM = 2
 
 
-class Resulting(StateDictLoadable, Trainable, Protocol):
+class Resulting(DeviceMovable, StateDictLoadable, Trainable, Protocol):
     """An object that have result available with reset method"""
-    @property
-    @abc.abstractmethod
-    def _target(self) -> Optional[str]:
-        return NotImplemented
-
-    @_target.setter
-    @abc.abstractmethod
-    def _target(self, t: Optional[str]) -> None:
-        pass
+    _metric_fn: Optional[Callable[[Any, Any], torch.Tensor]]
+    _target: Optional[str]
+    # @property
+    # @abc.abstractmethod
+    # def _metric_fn(self) -> Optional[Callable[[Any, Any], torch.Tensor]]:
+    #     return NotImplemented
+    
+    # @_metric_fn.setter
+    # @abc.abstractmethod
+    # def _metric_fn(self, fn: Optional[Callable[[Any, Any], torch.Tensor]]) -> None:
+    #     pass
+
+    # @property
+    # @abc.abstractmethod
+    # def _target(self) -> Optional[str]:
+    #     return NotImplemented
+
+    # @_target.setter
+    # @abc.abstractmethod
+    # def _target(self, t: Optional[str]) -> None:
+        # pass
 
     @property
     @abc.abstractmethod
     def result(self) -> torch.Tensor:
         return NotImplemented
 
     @abc.abstractmethod
@@ -117,14 +129,20 @@
 
 @runtime_checkable
 class VersionConvertible(Protocol):
     """The protocol that can convert from previous version"""
 
     @abc.abstractmethod
     def convert(self, from_version: Version) -> None:
+        """
+        Convert from a version to current version
+
+        - Parameters:
+            - from_version: A `torchmanager.version.Version` to convert from
+        """
         pass
 
 
 class Weighted(Protocol):
     """A weigthted protocol that contains `weight` as its property"""
 
     weight: Any
```

### Comparing `torchmanager_nightly-1.2rc0/torchmanager_core/random/seed.py` & `torchmanager_nightly-1.2rc2/torchmanager_core/random/seed.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2rc0/torchmanager_core/version.py` & `torchmanager_nightly-1.2rc2/torchmanager_core/version.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,80 @@
 import functools
 
-from .typing import Any, Optional
+from .typing import Any, Enum, Optional
 from .view import warnings
 
 
+class PreRelease(Enum):
+    ALPHA = 'a'
+    BETA = 'b'
+    RELEASE_CANDIDATE = "rc"
+
+    def __gt__(self, pre_release: Any) -> bool:
+        # convert pre release
+        if not isinstance(pre_release, PreRelease):
+            pre_release = PreRelease(pre_release)
+
+        # check pre release version
+        if self == pre_release:
+            return False
+        elif self == PreRelease.RELEASE_CANDIDATE:
+            return True
+        elif self == PreRelease.BETA and pre_release == PreRelease.ALPHA:
+            return True
+        else:
+            return False
+
+    def __lt__(self, pre_release: Any) -> bool:
+        # convert pre release
+        if not isinstance(pre_release, PreRelease):
+            pre_release = PreRelease(pre_release)
+
+        # check pre release version
+        if self == pre_release:
+            return False
+        elif pre_release == PreRelease.RELEASE_CANDIDATE:
+            return True
+        elif pre_release == PreRelease.BETA and self == PreRelease.ALPHA:
+            return True
+        else:
+            return False
+
+    def __le__(self, other: Any) -> bool:
+        return self == other or self < other
+
+    def __ge__(self, other: Any) -> bool:
+        return self == other or self > other
+
+
 class Version:
     main_version: int
     minor_version: int
-    pre_release: Optional[str]
+    pre_release: Optional[PreRelease]
     pre_release_version: int
     sub_version: int
 
     def __init__(self, v: Any, /) -> None:
         # convert to string
         version_str = str(v)
 
         # format version
         if version_str.startswith('v'):
             version_str = version_str[1:]
 
         # split pre-release version
         if 'a' in version_str:
             pre_release_parts = version_str.split('a')
-            self.pre_release = 'a'
+            self.pre_release = PreRelease.ALPHA
         elif 'b' in version_str:
             pre_release_parts = version_str.split('b')
-            self.pre_release = 'b'
+            self.pre_release = PreRelease.BETA
         elif 'rc' in version_str:
             pre_release_parts = version_str.split('rc')
-            self.pre_release = 'rc'
+            self.pre_release = PreRelease.RELEASE_CANDIDATE
         else:
             pre_release_parts = [version_str, "0"]
             self.pre_release = None
         version_str = pre_release_parts[0]
         self.pre_release_version = int(pre_release_parts[1]) if pre_release_parts[1] != '' else 1
 
         # split version
@@ -44,15 +86,15 @@
     def __repr__(self) -> str:
         version_str = f"v{self.main_version}"
         if self.minor_version > 0 or self.sub_version > 0:
             version_str += f".{self.minor_version}"
         if self.sub_version > 0:
             version_str += f".{self.sub_version}"
         if self.pre_release is not None:
-            version_str += self.pre_release
+            version_str += f"{self.pre_release.value}{self.pre_release_version}"
         return version_str
 
     def __eq__(self, other: Any) -> bool:
         if isinstance(other, Version):
             return self.main_version == other.main_version and self.minor_version == other.minor_version and self.sub_version == other.sub_version and self.pre_release == other.pre_release and self.pre_release_version == other.pre_release_version
         else:
             other = Version(str(other))
@@ -98,15 +140,15 @@
         return self == other or self < other
 
     def __ge__(self, other: Any) -> bool:
         return self == other or self > other
 
 
 API = Version("v1.2")
-CURRENT = Version("v1.2rc")
+CURRENT = Version("v1.2rc2")
 DESCRIPTION: str = "PyTorch Training Manager {CURRENT}"
 
 
 class VersionError(SystemError):
     def __init__(self, method_name: str, maximum_supported_version: str) -> None:
         super().__init__(f"`{method_name}` has been deprecated and removed from version {maximum_supported_version}. Current version: {CURRENT}.")
```

### Comparing `torchmanager_nightly-1.2rc0/PKG-INFO` & `torchmanager_nightly-1.2rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: torchmanager-nightly
-Version: 1.2rc0
-Summary: PyTorch Training Manager v1.2 (Release Candidate)
+Version: 1.2rc2
+Summary: PyTorch Training Manager v1.2 (Release Candidate 2)
 Home-page: https://github.com/kisonho/torchmanager.git
 Author: Qisheng He
 Author-email: Qisheng.He@wayne.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

