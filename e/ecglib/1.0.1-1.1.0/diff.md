# Comparing `tmp/ecglib-1.0.1.tar.gz` & `tmp/ecglib-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecglib-1.0.1.tar", last modified: Wed Nov  2 17:46:36 2022, max compression
+gzip compressed data, was "ecglib-1.1.0.tar", last modified: Tue Jun 20 10:41:45 2023, max compression
```

## Comparing `ecglib-1.0.1.tar` & `ecglib-1.1.0.tar`

### file list

```diff
@@ -1,36 +1,48 @@
-drwxr-xr-x   0 aram       (501) staff       (20)        0 2022-11-02 17:46:36.982343 ecglib-1.0.1/
--rw-r--r--   0 aram       (501) staff       (20)    11335 2022-11-02 16:02:55.000000 ecglib-1.0.1/LICENSE
--rw-r--r--   0 aram       (501) staff       (20)       36 2022-11-02 16:02:55.000000 ecglib-1.0.1/MANIFEST.in
--rw-r--r--   0 aram       (501) staff       (20)     5492 2022-11-02 17:46:36.982223 ecglib-1.0.1/PKG-INFO
--rw-r--r--   0 aram       (501) staff       (20)     5052 2022-11-02 16:47:58.000000 ecglib-1.0.1/README.md
-drwxr-xr-x   0 aram       (501) staff       (20)        0 2022-11-02 17:46:36.979378 ecglib-1.0.1/ecglib/
--rw-r--r--   0 aram       (501) staff       (20)      138 2022-11-02 16:02:55.000000 ecglib-1.0.1/ecglib/__init__.py
-drwxr-xr-x   0 aram       (501) staff       (20)        0 2022-11-02 17:46:36.980500 ecglib-1.0.1/ecglib/datasets/
--rw-r--r--   0 aram       (501) staff       (20)      104 2022-11-02 16:02:55.000000 ecglib-1.0.1/ecglib/datasets/__init__.py
--rw-r--r--   0 aram       (501) staff       (20)    12700 2022-11-02 16:02:55.000000 ecglib-1.0.1/ecglib/datasets/datasets.py
--rw-r--r--   0 aram       (501) staff       (20)     2390 2022-11-02 16:02:55.000000 ecglib-1.0.1/ecglib/datasets/load_datasets.py
-drwxr-xr-x   0 aram       (501) staff       (20)        0 2022-11-02 17:46:36.980766 ecglib-1.0.1/ecglib/models/
--rw-r--r--   0 aram       (501) staff       (20)       38 2022-11-02 16:02:55.000000 ecglib-1.0.1/ecglib/models/__init__.py
-drwxr-xr-x   0 aram       (501) staff       (20)        0 2022-11-02 17:46:36.980990 ecglib-1.0.1/ecglib/models/architectures/
--rw-r--r--   0 aram       (501) staff       (20)        0 2022-11-02 16:02:55.000000 ecglib-1.0.1/ecglib/models/architectures/__init__.py
--rw-r--r--   0 aram       (501) staff       (20)     5348 2022-11-02 16:02:55.000000 ecglib-1.0.1/ecglib/models/architectures/densenet1d.py
-drwxr-xr-x   0 aram       (501) staff       (20)        0 2022-11-02 17:46:36.981206 ecglib-1.0.1/ecglib/models/config/
--rw-r--r--   0 aram       (501) staff       (20)        0 2022-11-02 16:02:55.000000 ecglib-1.0.1/ecglib/models/config/__init__.py
--rw-r--r--   0 aram       (501) staff       (20)      460 2022-11-02 16:02:55.000000 ecglib-1.0.1/ecglib/models/config/model_configs.py
--rw-r--r--   0 aram       (501) staff       (20)     3231 2022-11-02 16:02:55.000000 ecglib-1.0.1/ecglib/models/create_model.py
-drwxr-xr-x   0 aram       (501) staff       (20)        0 2022-11-02 17:46:36.981492 ecglib-1.0.1/ecglib/models/weights/
--rw-r--r--   0 aram       (501) staff       (20)        0 2022-11-02 16:02:55.000000 ecglib-1.0.1/ecglib/models/weights/__init__.py
--rw-r--r--   0 aram       (501) staff       (20)      832 2022-11-02 16:02:55.000000 ecglib-1.0.1/ecglib/models/weights/model_weights_paths.yaml
-drwxr-xr-x   0 aram       (501) staff       (20)        0 2022-11-02 17:46:36.982039 ecglib-1.0.1/ecglib/preprocessing/
--rw-r--r--   0 aram       (501) staff       (20)      149 2022-11-02 16:02:55.000000 ecglib-1.0.1/ecglib/preprocessing/__init__.py
--rw-r--r--   0 aram       (501) staff       (20)     2968 2022-11-02 16:02:55.000000 ecglib-1.0.1/ecglib/preprocessing/composition.py
--rw-r--r--   0 aram       (501) staff       (20)    10142 2022-11-02 16:02:55.000000 ecglib-1.0.1/ecglib/preprocessing/functional.py
--rw-r--r--   0 aram       (501) staff       (20)    13538 2022-11-02 16:02:55.000000 ecglib-1.0.1/ecglib/preprocessing/preprocess.py
-drwxr-xr-x   0 aram       (501) staff       (20)        0 2022-11-02 17:46:36.980096 ecglib-1.0.1/ecglib.egg-info/
--rw-r--r--   0 aram       (501) staff       (20)     5492 2022-11-02 17:46:36.000000 ecglib-1.0.1/ecglib.egg-info/PKG-INFO
--rw-r--r--   0 aram       (501) staff       (20)      724 2022-11-02 17:46:36.000000 ecglib-1.0.1/ecglib.egg-info/SOURCES.txt
--rw-r--r--   0 aram       (501) staff       (20)        1 2022-11-02 17:46:36.000000 ecglib-1.0.1/ecglib.egg-info/dependency_links.txt
--rw-r--r--   0 aram       (501) staff       (20)       94 2022-11-02 17:46:36.000000 ecglib-1.0.1/ecglib.egg-info/requires.txt
--rw-r--r--   0 aram       (501) staff       (20)        7 2022-11-02 17:46:36.000000 ecglib-1.0.1/ecglib.egg-info/top_level.txt
--rw-r--r--   0 aram       (501) staff       (20)       38 2022-11-02 17:46:36.982382 ecglib-1.0.1/setup.cfg
--rw-r--r--   0 aram       (501) staff       (20)     1130 2022-11-02 17:46:05.000000 ecglib-1.0.1/setup.py
+drwxrwxr-x   0 aram      (1002) aram      (1002)        0 2023-06-20 10:41:45.510172 ecglib-1.1.0/
+-rw-rw-r--   0 aram      (1002) aram      (1002)    11335 2023-06-20 10:32:40.000000 ecglib-1.1.0/LICENSE
+-rw-rw-r--   0 aram      (1002) aram      (1002)       40 2023-06-20 10:32:40.000000 ecglib-1.1.0/MANIFEST.in
+-rw-rw-r--   0 aram      (1002) aram      (1002)      419 2023-06-20 10:41:45.510172 ecglib-1.1.0/PKG-INFO
+-rw-rw-r--   0 aram      (1002) aram      (1002)     6997 2023-06-20 10:32:40.000000 ecglib-1.1.0/README.md
+-rw-rw-r--   0 aram      (1002) aram      (1002)      745 2023-06-20 10:41:45.510172 ecglib-1.1.0/setup.cfg
+-rw-rw-r--   0 aram      (1002) aram      (1002)       37 2023-06-20 10:32:40.000000 ecglib-1.1.0/setup.py
+drwxrwxr-x   0 aram      (1002) aram      (1002)        0 2023-06-20 10:41:45.506172 ecglib-1.1.0/src/
+drwxrwxr-x   0 aram      (1002) aram      (1002)        0 2023-06-20 10:41:45.506172 ecglib-1.1.0/src/ecglib/
+-rw-rw-r--   0 aram      (1002) aram      (1002)      167 2023-06-20 10:32:40.000000 ecglib-1.1.0/src/ecglib/__init__.py
+drwxrwxr-x   0 aram      (1002) aram      (1002)        0 2023-06-20 10:41:45.506172 ecglib-1.1.0/src/ecglib/data/
+-rw-rw-r--   0 aram      (1002) aram      (1002)      149 2023-06-20 10:32:40.000000 ecglib-1.1.0/src/ecglib/data/__init__.py
+-rw-rw-r--   0 aram      (1002) aram      (1002)     7587 2023-06-20 10:32:40.000000 ecglib-1.1.0/src/ecglib/data/datasets.py
+-rw-rw-r--   0 aram      (1002) aram      (1002)     4993 2023-06-20 10:32:40.000000 ecglib-1.1.0/src/ecglib/data/ecg_record.py
+-rw-rw-r--   0 aram      (1002) aram      (1002)     7247 2023-06-20 10:32:40.000000 ecglib-1.1.0/src/ecglib/data/load_datasets.py
+drwxrwxr-x   0 aram      (1002) aram      (1002)        0 2023-06-20 10:41:45.510172 ecglib-1.1.0/src/ecglib/models/
+-rw-rw-r--   0 aram      (1002) aram      (1002)        0 2023-06-20 10:32:40.000000 ecglib-1.1.0/src/ecglib/models/__init__.py
+drwxrwxr-x   0 aram      (1002) aram      (1002)        0 2023-06-20 10:41:45.510172 ecglib-1.1.0/src/ecglib/models/architectures/
+-rw-rw-r--   0 aram      (1002) aram      (1002)        0 2023-06-20 10:32:40.000000 ecglib-1.1.0/src/ecglib/models/architectures/__init__.py
+-rw-rw-r--   0 aram      (1002) aram      (1002)     2068 2023-06-20 10:32:40.000000 ecglib-1.1.0/src/ecglib/models/architectures/cnn_tabular.py
+-rw-rw-r--   0 aram      (1002) aram      (1002)     5809 2023-06-20 10:32:40.000000 ecglib-1.1.0/src/ecglib/models/architectures/densenet1d.py
+-rw-rw-r--   0 aram      (1002) aram      (1002)      555 2023-06-20 10:32:40.000000 ecglib-1.1.0/src/ecglib/models/architectures/model_types.py
+-rw-rw-r--   0 aram      (1002) aram      (1002)     1809 2023-06-20 10:32:40.000000 ecglib-1.1.0/src/ecglib/models/architectures/registred_models.py
+-rw-rw-r--   0 aram      (1002) aram      (1002)     7665 2023-06-20 10:32:40.000000 ecglib-1.1.0/src/ecglib/models/architectures/resnet1d.py
+-rw-rw-r--   0 aram      (1002) aram      (1002)     2019 2023-06-20 10:32:40.000000 ecglib-1.1.0/src/ecglib/models/architectures/tabular.py
+drwxrwxr-x   0 aram      (1002) aram      (1002)        0 2023-06-20 10:41:45.510172 ecglib-1.1.0/src/ecglib/models/config/
+-rw-rw-r--   0 aram      (1002) aram      (1002)        0 2023-06-20 10:32:40.000000 ecglib-1.1.0/src/ecglib/models/config/__init__.py
+-rw-rw-r--   0 aram      (1002) aram      (1002)     2639 2023-06-20 10:32:40.000000 ecglib-1.1.0/src/ecglib/models/config/model_configs.py
+-rw-rw-r--   0 aram      (1002) aram      (1002)     1693 2023-06-20 10:32:40.000000 ecglib-1.1.0/src/ecglib/models/config/registred_configs.py
+-rw-rw-r--   0 aram      (1002) aram      (1002)     8734 2023-06-20 10:32:40.000000 ecglib-1.1.0/src/ecglib/models/model_builder.py
+drwxrwxr-x   0 aram      (1002) aram      (1002)        0 2023-06-20 10:41:45.510172 ecglib-1.1.0/src/ecglib/models/weights/
+-rw-rw-r--   0 aram      (1002) aram      (1002)        0 2023-06-20 10:32:40.000000 ecglib-1.1.0/src/ecglib/models/weights/__init__.py
+-rw-rw-r--   0 aram      (1002) aram      (1002)      637 2023-06-20 10:32:40.000000 ecglib-1.1.0/src/ecglib/models/weights/checkpoint.py
+-rw-rw-r--   0 aram      (1002) aram      (1002)     3175 2023-06-20 10:32:40.000000 ecglib-1.1.0/src/ecglib/models/weights/model_weights_paths.yaml
+drwxrwxr-x   0 aram      (1002) aram      (1002)        0 2023-06-20 10:41:45.510172 ecglib-1.1.0/src/ecglib/predict/
+-rw-rw-r--   0 aram      (1002) aram      (1002)       53 2023-06-20 10:32:40.000000 ecglib-1.1.0/src/ecglib/predict/__init__.py
+-rw-rw-r--   0 aram      (1002) aram      (1002)    10332 2023-06-20 10:32:40.000000 ecglib-1.1.0/src/ecglib/predict/predict.py
+drwxrwxr-x   0 aram      (1002) aram      (1002)        0 2023-06-20 10:41:45.510172 ecglib-1.1.0/src/ecglib/preprocessing/
+-rw-rw-r--   0 aram      (1002) aram      (1002)      150 2023-06-20 10:32:40.000000 ecglib-1.1.0/src/ecglib/preprocessing/__init__.py
+-rw-rw-r--   0 aram      (1002) aram      (1002)     2986 2023-06-20 10:32:40.000000 ecglib-1.1.0/src/ecglib/preprocessing/composition.py
+-rw-rw-r--   0 aram      (1002) aram      (1002)     9729 2023-06-20 10:32:40.000000 ecglib-1.1.0/src/ecglib/preprocessing/functional.py
+-rw-rw-r--   0 aram      (1002) aram      (1002)    24523 2023-06-20 10:32:40.000000 ecglib-1.1.0/src/ecglib/preprocessing/preprocess.py
+drwxrwxr-x   0 aram      (1002) aram      (1002)        0 2023-06-20 10:41:45.506172 ecglib-1.1.0/src/ecglib.egg-info/
+-rw-rw-r--   0 aram      (1002) aram      (1002)      419 2023-06-20 10:41:45.000000 ecglib-1.1.0/src/ecglib.egg-info/PKG-INFO
+-rw-rw-r--   0 aram      (1002) aram      (1002)     1217 2023-06-20 10:41:45.000000 ecglib-1.1.0/src/ecglib.egg-info/SOURCES.txt
+-rw-rw-r--   0 aram      (1002) aram      (1002)        1 2023-06-20 10:41:45.000000 ecglib-1.1.0/src/ecglib.egg-info/dependency_links.txt
+-rw-rw-r--   0 aram      (1002) aram      (1002)      190 2023-06-20 10:41:45.000000 ecglib-1.1.0/src/ecglib.egg-info/requires.txt
+-rw-rw-r--   0 aram      (1002) aram      (1002)        7 2023-06-20 10:41:45.000000 ecglib-1.1.0/src/ecglib.egg-info/top_level.txt
```

### Comparing `ecglib-1.0.1/LICENSE` & `ecglib-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ecglib-1.0.1/ecglib/datasets/datasets.py` & `ecglib-1.1.0/src/ecglib/data/datasets.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,150 +1,123 @@
-from enum import IntEnum
 from pathlib import Path
-from typing import Callable, Optional
+from typing import Callable, Optional, Union
 
 import ecg_plot
 import numpy as np
 import pandas as pd
 import torch
 import wfdb
 from ecglib import preprocessing as P
+from .ecg_record import EcgRecord
 from torch.utils.data import Dataset
 
+
 __all__ = [
     "EcgDataset",
-    "TisDataset",
-    "PTBXLDataset",
 ]
 
 
 class EcgDataset(Dataset):
     """
     EcgDataset
     :param ecg_data: dataframe with ecg info
     :param target: a list of targets
     :param frequency: frequency for signal resampling
     :param leads: a list of leads
     :param ecg_length: length of ECG signal after padding / cropping
     :param cut_range: cutting parameters
-    :param pad_mode: padding mode 
+    :param pad_mode: padding mode
     :param classes: number of classes
     :param use_meta: whether to use metadata or not
     :param augmentation: a bunch of augmentations and other preprocessing techniques
     """
 
     def __init__(
         self,
         ecg_data: pd.DataFrame,
         target: list,
         frequency: int = 500,
         leads: list = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11],
-        ecg_length: float = 10,
+        data_type: str = "wfdb",
+        ecg_length: Union[int, float] = 10,
         cut_range: list = [0, 0],
         pad_mode: str = "constant",
         norm_type: str = "z_norm",
         classes: int = 2,
-        use_meta: bool = False,
         augmentation: Callable = None,
     ):
         super().__init__()
         if "fpath" not in ecg_data.columns:
             raise ValueError("column 'fpath' not in ecg_data")
         self.ecg_data = ecg_data
         self.target = target
         self.frequency = frequency
         self.leads = leads
+        self.data_type = data_type
         self.ecg_length = ecg_length
         self.cut_range = cut_range
         self.pad_mode = pad_mode
         self.norm_type = norm_type
         self.classes = classes
-        if use_meta and "ecg_parameters" not in ecg_data.columns:
-            raise ValueError("metadata column 'ecg_parameters' not in ecg_data")
-        self.meta = use_meta
         self.augmentation = augmentation
 
     def __len__(self):
         return self.ecg_data.shape[0]
 
     def get_fpath(self, index: int) -> str:
         """
         Returns path to file with ECG leads
         :param index: Index of ECG in dataset
-        
+
         :return: Path to ECG file
         """
 
         return self.ecg_data.iloc[index]["fpath"]
 
     def get_name(self, index: int) -> str:
         """
         Returns name of ECG file
         :param index: Index of ECG in dataset
-        
+
         :return: ECG file name
         """
 
         return str(Path(self.get_fpath(index)).stem)
 
-
-class TisDataset(EcgDataset):
-    """
-    TisDataset
-    :param ecg_data: dataframe with ecg info
-    :param target: a list of targets
-    :param frequency: frequency for signal resampling
-    :param leads: a list of leads
-    :param ecg_length: length of ECG signal after padding / cropping
-    :param cut_range: cutting parameters
-    :param pad_mode: padding mode 
-    :param classes: number of classes
-    :param use_meta: whether to use metadata or not
-    :param augmentation: a bunch of augmentations and other preprocessing techniques
-    """
-
-    def __init__(
-        self,
-        ecg_data: pd.DataFrame,
-        target: list,
-        frequency: int = 500,
-        leads: list = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11],
-        ecg_length: float = 10,
-        cut_range: list = [0, 0],
-        pad_mode: str = "constant",
-        norm_type: str = "z_norm",
-        classes: int = 2,
-        use_meta: bool = False,
-        augmentation: Callable = None,
+    def read_ecg_record(
+        self, file_path, data_type, leads=[0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11]
     ):
-        super().__init__(
-            ecg_data,
-            target,
-            frequency,
-            leads,
-            ecg_length,
-            cut_range,
-            pad_mode,
-            norm_type,
-            classes,
-            use_meta,
-            augmentation,
-        )
+        if data_type == "npz":
+            ecg_record = np.load(file_path)["arr_0"].astype("float64")
+        elif data_type == "wfdb":
+            ecg_record, _ = wfdb.rdsamp(file_path, channels=leads)
+            ecg_record = ecg_record.T
+            ecg_record = ecg_record.astype("float64")
+        else:
+            raise ValueError(
+                'data_type can have only values from the list ["npz", "wfdb"]'
+            )
+        return ecg_record
 
     def __getitem__(self, index):
-
-        if "frequency" in self.ecg_data.columns:
-            ecg_frequency = float(self.ecg_data.iloc[index]["frequency"])
-        else:
-            ecg_frequency = self.frequency
+        ecg_frequency = float(self.ecg_data.iloc[index]["frequency"])
+        patient_meta = (
+            self.ecg_data.iloc[index]["patient_metadata"]
+            if "patient_metadata" in self.ecg_data.iloc[index]
+            else dict()
+        )
+        ecg_record_meta = (
+            self.ecg_data.iloc[index]["ecg_metadata"]
+            if "ecg_metadata" in self.ecg_data.iloc[index]
+            else dict()
+        )
+        file_path = self.ecg_data.iloc[index]["fpath"]
 
         # data standartization (scaling, resampling, cuts off, normalization and padding/truncation)
-        ecg_record = np.load(self.ecg_data.iloc[index]["fpath"])["arr_0"].astype(
-            "float64"
-        )
+        ecg_record = self.read_ecg_record(file_path, self.data_type, self.leads)
         ecg_record = P.Compose(
             transforms=[
                 P.FrequencyResample(
                     ecg_frequency=ecg_frequency, requested_frequency=self.frequency
                 ),
                 P.EdgeCut(cut_range=self.cut_range, frequency=self.frequency),
                 P.Normalization(norm_type=self.norm_type),
@@ -160,26 +133,42 @@
 
         # data preprocessing if specified (augmentation, filtering)
         if self.augmentation is not None:
             ecg_record = self.augmentation(ecg_record)
 
         target = self.target[index]
 
+        patient_meta = {
+            key: patient_meta[key]
+            if isinstance(patient_meta[key], list)
+            else [patient_meta[key]]
+            for key in patient_meta
+        }
+
+        ecg_record_meta = {
+            key: ecg_record_meta[key]
+            if isinstance(ecg_record_meta[key], list)
+            else [ecg_record_meta[key]]
+            for key in ecg_record_meta
+        }
+
+        full_ecg_record_info = EcgRecord(
+            signal=ecg_record[self.leads, :],
+            frequency=ecg_frequency,
+            name=file_path,
+            lead_order=self.leads,
+            ecg_metadata=ecg_record_meta,
+            patient_metadata=patient_meta,
+        )
+
         result = [
-            torch.tensor(ecg_record[self.leads, :], dtype=torch.float),
+            full_ecg_record_info.to_tensor(),
             torch.tensor(target, dtype=torch.float),
         ]
 
-        if self.meta:
-            result.append(
-                torch.tensor(
-                    self.ecg_data.iloc[index]["ecg_parameters"], dtype=torch.float
-                )
-            )
-
         return (index, result)
 
     def save_as_png(
         self, index: int, dest_path: str, postfix: Optional[str] = None
     ) -> None:
         """
         Saves the image of ecg record
@@ -212,182 +201,36 @@
         if not Path(dest_path).exists():
             Path(dest_path).mkdir(parents=True, exist_ok=True)
 
         ecg_plot.save_as_png(file_name=ecg_fname, path=dest_path)
 
     @staticmethod
     def for_train_from_config(
-        data: pd.DataFrame, target: list, augmentation: Callable, config: dict, classes_num: int
-    ) -> EcgDataset:
-        """
-        A wrapper with just four parameters to create `TisDataset` for training and validation
-        :param data: dataframe with ecg info
-        :param target: a list of targets
-        :param augmentation: a bunch of augmentations and other preprocessing techniques
-        :param config: config dictionary
-        :param classes_num: number of classes
-        
-        :return: TisDataset
-        """
-
-        return TisDataset(
-            data,
-            target,
-            frequency=config.ecg_record_params.resampled_frequency,
-            leads=config.ecg_record_params.leads,
-            ecg_length=config.ecg_record_params.observed_ecg_length,
-            norm_type=config.ecg_record_params.normalization,
-            classes=classes_num,
-            use_meta=config.ecg_metadata.use_metadata,
-            cut_range=config.ecg_record_params.ecg_cut_range,
-            augmentation=augmentation,
-        )
-
-
-class PTBXLDataset(EcgDataset):
-    """
-    PTBXLDataset
-    :param ecg_data: dataframe with ecg info
-    :param target: a list of targets
-    :param frequency: frequency for signal resampling
-    :param leads: a list of leads
-    :param ecg_length: length of ECG signal after padding / cropping
-    :param cut_range: cutting parameters
-    :param pad_mode: padding mode 
-    :param classes: number of classes
-    :param use_meta: whether to use metadata or not
-    :param augmentation: a bunch of augmentations and other preprocessing techniques
-    """
-
-    def __init__(
-        self,
-        ecg_data: pd.DataFrame,
+        data: pd.DataFrame,
         target: list,
-        frequency: int = 500,
-        leads: list = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11],
-        ecg_length: float = 10,
-        cut_range: list = [0, 0],
-        pad_mode: str = "constant",
-        norm_type: str = "z_norm",
-        classes: int = 2,
-        use_meta: bool = False,
-        augmentation: Callable = None,
+        augmentation: Callable,
+        config: dict,
+        classes_num: int,
     ):
-        super().__init__(
-            ecg_data,
-            target,
-            500,
-            leads,
-            10,
-            cut_range,
-            pad_mode,
-            norm_type,
-            classes,
-            False,
-            augmentation,
-        )
-
-    def __getitem__(self, index):
-        if "frequency" in self.ecg_data.columns:
-            ecg_frequency = float(self.ecg_data.iloc[index]["frequency"])
-        else:
-            ecg_frequency = self.frequency
-
-        ecg_record, _ = wfdb.rdsamp(
-            self.ecg_data.iloc[index]["fpath"], channels=self.leads
-        )
-        ecg_record = ecg_record.T
-        ecg_record = ecg_record.astype("float64")
-
-        # data standartization (scaling, resampling, cuts off, normalization and padding/truncation)
-        ecg_record = P.Compose(
-            transforms=[
-                P.FrequencyResample(
-                    ecg_frequency=ecg_frequency, requested_frequency=self.frequency
-                ),
-                P.EdgeCut(cut_range=self.cut_range, frequency=self.frequency),
-                P.Normalization(norm_type=self.norm_type),
-                P.Padding(
-                    observed_ecg_length=self.ecg_length, frequency=self.frequency
-                ),
-            ],
-            p=1.0,
-        )(ecg_record)
-
-        # data preprocessing if specified (augmentation, filtering)
-        if self.augmentation is not None:
-            ecg_record = self.augmentation(ecg_record)
-
-        target = self.target[index]
-
-        result = [
-            torch.tensor(ecg_record[self.leads, :], dtype=torch.float),
-            torch.tensor(target, dtype=torch.float),
-        ]
-
-        return (index, result)
-
-    def save_as_png(
-        self, index: int, dest_path: str, postfix: Optional[str] = None
-    ) -> None:
-        """
-        Saves the image of ecg record
-        :param index: Index of ECG
-        :param dest_path: Directory to save the image
-        :param postfix: Subdirectory where the image will be saved, defaults to None
         """
-
-        if "frequency" in self.ecg_data.columns:
-            frequency = self.ecg_data.iloc[index]["frequency"]
-        else:
-            frequency = self.frequency
-
-        ecg, _ = wfdb.rdsamp(self.ecg_data.iloc[index]["fpath"], channels=self.leads)
-        ecg = ecg.T
-        ecg = ecg.astype("float64")
-
-        ecg = ecg / np.max(
-            ecg
-        )  # added to fit the record to the visible part of the plot
-        ecg_plot.plot(ecg, sample_rate=frequency)
-        ecg_fname = self.get_name(index)
-
-        if postfix:
-            dest_path = str(Path(dest_path).joinpath(postfix))
-
-        dest_path = (
-            "{}/".format(dest_path) if not dest_path.endswith("/") else dest_path
-        )
-
-        if not Path(dest_path).exists():
-            Path(dest_path).mkdir(parents=True, exist_ok=True)
-
-        ecg_plot.save_as_png(file_name=ecg_fname, path=dest_path)
-
-    @staticmethod
-    def for_train_from_config(
-        data: pd.DataFrame, target: list, augmentation: Callable, config: dict, classes_num: int
-    ) -> EcgDataset:
-        """
-        A wrapper with just four parameters to create `PTBXLDataset` for training and validation
+        A wrapper with just four parameters to create `TisDataset` for training and validation
         :param data: dataframe with ecg info
         :param target: a list of targets
         :param augmentation: a bunch of augmentations and other preprocessing techniques
         :param config: config dictionary
         :param classes_num: number of classes
-        
-        :return: PTBXLDataset
+
+        :return: EcgDataset
         """
 
-        return PTBXLDataset(
+        return EcgDataset(
             data,
             target,
             frequency=config.ecg_record_params.resampled_frequency,
             leads=config.ecg_record_params.leads,
+            data_type=config.ecg_record_params.data_type,
             ecg_length=config.ecg_record_params.observed_ecg_length,
             norm_type=config.ecg_record_params.normalization,
             classes=classes_num,
-            use_meta=config.ecg_metadata.use_metadata,
-            cut_range=config.ecg_record_params.edge_cut.ecg_cut_range,
+            cut_range=config.ecg_record_params.ecg_cut_range,
             augmentation=augmentation,
         )
-
```

### Comparing `ecglib-1.0.1/ecglib/models/architectures/densenet1d.py` & `ecglib-1.1.0/src/ecglib/models/architectures/densenet1d.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,56 +1,65 @@
 import torch
 import torch.nn as nn
 
 
 class DenseLayer(nn.Module):
-    ''' Paper: https://arxiv.org/pdf/1608.06993v5.pdf '''
+    """Paper: https://arxiv.org/pdf/1608.06993v5.pdf"""
+
     def __init__(self, input_channels, growth_rate, bottleneck_size, kernel_size):
         super().__init__()
         self.use_bottleneck = bottleneck_size > 0
         self.num_bottleneck_output_filters = growth_rate * bottleneck_size
         if self.use_bottleneck:
             self.bn2 = nn.BatchNorm1d(input_channels)
             self.act2 = nn.ReLU(inplace=True)
             self.conv2 = nn.Conv1d(
                 input_channels,
                 self.num_bottleneck_output_filters,
                 kernel_size=1,
-                stride=1)
+                stride=1,
+            )
         self.bn1 = nn.BatchNorm1d(self.num_bottleneck_output_filters)
         self.act1 = nn.ReLU(inplace=True)
         self.conv1 = nn.Conv1d(
             self.num_bottleneck_output_filters,
             growth_rate,
             kernel_size=kernel_size,
             stride=1,
             dilation=1,
-            padding=kernel_size // 2)
+            padding=kernel_size // 2,
+        )
 
     def forward(self, x):
         if self.use_bottleneck:
             x = self.bn2(x)
             x = self.act2(x)
             x = self.conv2(x)
         x = self.bn1(x)
         x = self.act1(x)
         x = self.conv1(x)
         return x
 
 
 class DenseBlock(nn.ModuleDict):
-    def __init__(self, num_layers, input_channels, growth_rate, kernel_size, bottleneck_size):
+    def __init__(
+        self, num_layers, input_channels, growth_rate, kernel_size, bottleneck_size
+    ):
         super().__init__()
         self.num_layers = num_layers
         for i in range(self.num_layers):
-            self.add_module(f'denselayer{i}',
-                            DenseLayer(input_channels + i * growth_rate,
-                                       growth_rate,
-                                       bottleneck_size,
-                                       kernel_size))
+            self.add_module(
+                f"denselayer{i}",
+                DenseLayer(
+                    input_channels + i * growth_rate,
+                    growth_rate,
+                    bottleneck_size,
+                    kernel_size,
+                ),
+            )
 
     def forward(self, x):
         layer_outputs = [x]
         for _, layer in self.items():
             x = layer(x)
             layer_outputs.append(x)
             x = torch.cat(layer_outputs, dim=1)
@@ -58,66 +67,81 @@
 
 
 class TransitionBlock(nn.Module):
     def __init__(self, input_channels, out_channels):
         super().__init__()
         self.bn = nn.BatchNorm1d(input_channels)
         self.act = nn.ReLU(inplace=True)
-        self.conv = nn.Conv1d(input_channels, out_channels, kernel_size=1, stride=1, dilation=1)
+        self.conv = nn.Conv1d(
+            input_channels, out_channels, kernel_size=1, stride=1, dilation=1
+        )
         self.pool = nn.AvgPool1d(kernel_size=2, stride=2)
 
     def forward(self, x):
         x = self.bn(x)
         x = self.act(x)
         x = self.conv(x)
         x = self.pool(x)
         return x
 
 
 class DenseNet1d(nn.Module):
     def __init__(
-            self,
-            growth_rate: int = 32,
-            block_config: tuple = (6, 12, 24, 16),
-            num_init_features: int = 64,
-            bottleneck_size: int = 4,
-            kernel_size: int = 3,
-            input_channels: int = 3,
-            num_classes: int = 1,
-            reinit: bool = True,
+        self,
+        growth_rate: int = 32,
+        block_config: tuple = (6, 12, 24, 16),
+        num_init_features: int = 64,
+        bottleneck_size: int = 4,
+        kernel_size: int = 3,
+        input_channels: int = 3,
+        num_classes: int = 1,
+        reinit: bool = True,
     ):
         super().__init__()
+        self.stem = None
+        self.backbone = None
+        self.head = None
 
-        self.features = nn.Sequential(
+        # make stem
+        self.stem = nn.Sequential(
             nn.Conv1d(
-                input_channels, num_init_features,
-                kernel_size=7, stride=2, padding=3, dilation=1),
+                input_channels,
+                num_init_features,
+                kernel_size=7,
+                stride=2,
+                padding=3,
+                dilation=1,
+            ),
             nn.BatchNorm1d(num_init_features),
             nn.ReLU(inplace=True),
             nn.MaxPool1d(kernel_size=3, stride=2, padding=1),
         )
 
+        # make backbone
+        self.backbone = nn.Sequential()
         num_features = num_init_features
         for i, num_layers in enumerate(block_config):
             block = DenseBlock(
                 num_layers=num_layers,
                 input_channels=num_features,
                 growth_rate=growth_rate,
                 kernel_size=kernel_size,
                 bottleneck_size=bottleneck_size,
             )
-            self.features.add_module(f'denseblock{i}', block)
+            self.backbone.add_module(f"denseblock{i}", block)
             num_features = num_features + num_layers * growth_rate
             if i != len(block_config) - 1:
                 trans = TransitionBlock(
-                    input_channels=num_features,
-                    out_channels=num_features // 2)
-                self.features.add_module(f'transition{i}', trans)
+                    input_channels=num_features, out_channels=num_features // 2
+                )
+                self.backbone.add_module(f"transition{i}", trans)
                 num_features = num_features // 2
+        self.backbone_out_features = num_features
 
+        # make head
         self.final_bn = nn.BatchNorm1d(num_features)
         self.final_act = nn.ReLU(inplace=True)
         self.final_pool = nn.AdaptiveAvgPool1d(1)
         self.classifier = nn.Linear(num_features, num_classes)
 
         # init
         if reinit:
@@ -126,33 +150,36 @@
                     nn.init.kaiming_normal_(m.weight)
                 elif isinstance(m, nn.BatchNorm1d):
                     nn.init.constant_(m.weight, 1)
                     nn.init.constant_(m.bias, 0)
                 elif isinstance(m, nn.Linear):
                     nn.init.constant_(m.bias, 0)
 
-    def forward_features(self, x):
-        out = self.features(x)
-        out = self.final_bn(out)
-        out = self.final_act(out)
-        out = self.final_pool(out)
-        return out
-
     def forward(self, x):
-        features = self.forward_features(x)
+        # stem
+        features = self.stem(x)
+        # backbone
+        features = self.backbone(features)
+        # head
+        features = self.final_bn(features)
+        features = self.final_act(features)
+        features = self.final_pool(features)
         features = features.squeeze(-1)
         out = self.classifier(features)
         return out
 
     def reset_classifier(self):
         self.classifier = nn.Identity()
 
     def get_classifier(self):
         return self.classifier
 
+    def get_cnn(self):
+        return (nn.Sequential(self.stem, self.backbone), self.backbone_out_features)
+
 
 def densenet121_1d(**kwargs):
     kwargs["block_config"] = (6, 12, 24, 16)
     return DenseNet1d(**kwargs)
 
 
 def densenet201_1d(**kwargs):
```

### Comparing `ecglib-1.0.1/ecglib/preprocessing/composition.py` & `ecglib-1.1.0/src/ecglib/preprocessing/composition.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,16 +27,17 @@
         self.transforms = transforms
         if p > 1.0 or p < 0.0:
             raise ValueError("Probability should be between 0.0 and 1.0")
         else:
             self.p = p
 
     def __call__(self, x):
-        
-        idx = np.random.RandomState(random.randint(0, (1 << 32) - 1)).choice(2, p=[self.p, 1.0-self.p])
+        idx = np.random.RandomState(random.randint(0, (1 << 32) - 1)).choice(
+            2, p=[self.p, 1.0 - self.p]
+        )
         if idx == 0:
             for t in self.transforms:
                 x = t(x)
 
         return x
 
 
@@ -55,54 +56,56 @@
         transforms: list,
         n: int,
         transform_prob: list = None,
     ):
         self.transforms = transforms
         self.n = n
         if transform_prob is None:
-            self.transform_prob = [1 / len(self.transforms)]*len(self.transforms)
+            self.transform_prob = [1 / len(self.transforms)] * len(self.transforms)
         else:
             if sum(transform_prob) > 1.0:
                 raise ValueError("Sum of probabilities should be equal to 1.0")
             else:
                 self.transform_prob = transform_prob
 
     def __call__(self, x):
-        
-        idx = np.random.RandomState(random.randint(0, (1 << 32) - 1)).choice(len(self.transforms), size=self.n, p=self.transform_prob, replace=False)
+        idx = np.random.RandomState(random.randint(0, (1 << 32) - 1)).choice(
+            len(self.transforms), size=self.n, p=self.transform_prob, replace=False
+        )
         for i in idx:
             t = self.transforms[i]
             data = t(x)
-            
+
         return data
-    
+
 
 class OneOf:
     """
     Apply one of preprocessing techniques from a given list (normalization, augmentation etc.)
     :param transforms: a list of preprocessing techniques
     :param transform_prob: a list of probabilities
 
     :return: preprocessed data
     """
-    
+
     def __init__(
         self,
         transforms: list,
         transform_prob: list = None,
     ):
         self.transforms = transforms
         if transform_prob is None:
-            self.transform_prob = [1 / len(self.transforms)]*len(self.transforms)
+            self.transform_prob = [1 / len(self.transforms)] * len(self.transforms)
         else:
             if sum(transform_prob) > 1.0:
                 raise ValueError("Sum of probabilities should be equal to 1.0")
             else:
                 self.transform_prob = transform_prob
 
     def __call__(self, x):
-        
-        idx = np.random.RandomState(random.randint(0, (1 << 32) - 1)).choice(len(self.transforms), p=self.transform_prob)
+        idx = np.random.RandomState(random.randint(0, (1 << 32) - 1)).choice(
+            len(self.transforms), p=self.transform_prob
+        )
         t = self.transforms[idx]
         x = t(x)
-        
-        return x
+
+        return x
```

### Comparing `ecglib-1.0.1/ecglib/preprocessing/functional.py` & `ecglib-1.1.0/src/ecglib/preprocessing/functional.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,412 +1,369 @@
 import copy
+from typing import Union
 
 import numpy as np
 import pywt
 from scipy import signal
 from scipy.stats import zscore
 
 
 __all__ = [
-    "butterworth_bandpass_filter",
-    "butterworth_highpass_filter",
-    "butterworth_lowpass_filter",
+    "frequency_resample",
+    "cut_ecg",
+    "butterworth_filter",
     "IIR_notch_filter",
-    "elliptic_bandpass_filter",
+    "elliptic_filter",
     "minmax_normalization",
     "z_normalization",
-    "cycle_normalization",
     "DWT_filter",
     "SWT_filter",
     "lead_crop",
     "time_crop",
     "sum_augmentation",
     "convex_augmentation",
-    "reflect_augmentation",
-    "ecg_to_one_frequency",
     "DWT_BW",
-    "cut_ecg",
 ]
 
 
-def butterworth_bandpass_filter(
-    s: np.ndarray, 
-    n: int = 10, 
-    Wn: list = [3, 30], 
-    fs: float = 500,
+def frequency_resample(
+    ecg_record: np.ndarray,
+    ecg_frequency: int,
+    requested_frequency: int,
 ) -> np.ndarray:
     """
-    Butterworth bandpass filter augmentation
-    :param s: one lead signal
-    :param n: filter order
-    :param Wn: cutoff frequencies
-    :param fs: filtered signal frequency
+    Frequency resample
+    :param record: signal
+    :param ecg_frequency: sampling frequency of a signal
+    :param requested_frequency: sampling frequency of a preprocessed signal
 
     :return: preprocessed data
     """
-    
-    sos = signal.butter(N=n, btype='bandpass', Wn=Wn, fs=fs, output='sos')
-    filtered_signal = signal.sosfiltfilt(sos, s)
-    return filtered_signal
+
+    if ecg_frequency == requested_frequency:
+        return ecg_record
+    ecg_record = signal.resample(
+        ecg_record,
+        int(ecg_record.shape[1] * requested_frequency / ecg_frequency),
+        axis=1,
+    )
+    return ecg_record
 
 
-def butterworth_highpass_filter(
-    s: np.ndarray, 
-    n: int = 7, 
-    Wn: float = 0.5, 
-    fs: int = 500,
+def cut_ecg(
+    data: np.ndarray,
+    cut_range: list,
+    frequency: int,
 ) -> np.ndarray:
     """
-    Butterworth highpass filter augmentation
-    :param s: one lead signal
-    :param n: filter order
-    :param Wn: cutoff frequency
-    :param fs: filtered signal frequency
+    Cut signal edges
+    :param data: signal
+    :param cut_range: cutting parameters
+    :param frequency: sampling frequency of a signal
 
     :return: preprocessed data
     """
-    
-    sos = signal.butter(N=n, btype='highpass', Wn=Wn, fs=fs, output='sos')
-    filtered_signal = signal.sosfiltfilt(sos, s)
-    return filtered_signal
 
+    cut_data = []
+    start = int(cut_range[0] * frequency)
+    for rec in data:
+        end = -int(cut_range[1] * frequency) if cut_range[1] != 0 else len(rec)
+        cut_data.append(rec[start:end])
 
-def butterworth_lowpass_filter(
-    s: np.ndarray, 
-    n: int = 6, 
-    Wn: float = 20, 
-    fs: int = 500,
+    return np.array(cut_data)
+
+
+def butterworth_filter(
+    s: np.ndarray,
+    leads: list,
+    btype: str = "bandpass",
+    n: int = 10,
+    Wn: Union[float, int, list] = [3, 30],
+    fs: float = 500,
 ) -> np.ndarray:
     """
-    Butterworth lowpass filter augmentation
-    :param s: one lead signal
+    Butterworth bandpass filter augmentation
+    :param s: ECG signal
+    :param leads: leads to be filtered
+    :param btype: type of Butterworth filter ('bandpass', 'lowpass' or 'highpass')
     :param n: filter order
-    :param Wn: cutoff frequency
+    :param Wn: cutoff frequency(ies)
     :param fs: filtered signal frequency
 
     :return: preprocessed data
     """
-    
-    sos = signal.butter(N=n, btype='lowpass', Wn=Wn, fs=fs, output='sos')
-    filtered_signal = signal.sosfiltfilt(sos, s)
-    return filtered_signal
+    if btype == "bandpass" and not isinstance(Wn, list):
+        raise ValueError("Wn must be list type in case of bandpass filter")
+    elif (btype == "highpass" or btype == "lowpass") and not isinstance(
+        Wn, (int, float)
+    ):
+        raise ValueError(f"Wn must be a scalar in case of {btype} filter")
+    sos = signal.butter(N=n, btype=btype, Wn=Wn, fs=fs, output="sos")
+    s[leads, :] = signal.sosfiltfilt(sos, s[leads, :])
+    return s
 
 
 def IIR_notch_filter(
-    s: np.ndarray, 
-    w0: float = 50, 
-    Q: float = 30, 
+    s: np.ndarray,
+    leads: list,
+    w0: float = 50,
+    Q: float = 30,
     fs: int = 500,
 ) -> np.ndarray:
     """
     IIR notch filter augmentation
-    :param s: one lead signal
+    :param s: ECG signal
+    :param leads: leads to be filtered
     :param w0: frequency to remove from a signal
     :param Q: quality factor
     :param fs: sampling frequency of a signal
 
     :return: preprocessed data
     """
-    
     b, a = signal.iirnotch(w0=w0, Q=Q, fs=fs)
-    filtered_signal = signal.filtfilt(b, a, s)
-    return filtered_signal
+    s[leads, :] = signal.filtfilt(b, a, s[leads, :])
+    return s
 
 
-def elliptic_bandpass_filter(
-    s: np.ndarray, 
-    n: int = 10, 
-    rp: float = 4, 
-    rs: float = 5, 
-    Wn: list = [0.5, 50], 
+def elliptic_filter(
+    s: np.ndarray,
+    leads: list,
+    btype: str = "bandpass",
+    n: int = 10,
+    rp: float = 4,
+    rs: float = 5,
+    Wn: Union[float, int, list] = [0.5, 50],
     fs: int = 500,
 ) -> np.ndarray:
     """
-    Elliptic bandpass filter
-    :param s: one lead signal
+    Elliptic filter
+    :param s: ECG signal
+    :param leads: leads to be filtered
+    :param btype: type of elliptic filter ('bandpass', 'lowpass' or 'highpass')
     :param n: filter order
     :param rp: maximum ripple allowed below unity gain in the passband
     :param rs: minimum attenuation required in the stop band
-    :param Wn: cutoff frequencies
+    :param Wn: cutoff frequency(ies)
     :param fs: filtered signal frequency
-    
+
     :return: preprocessed data
     """
-    
-    sos = signal.ellip(N=n, btype='bandpass', rp=rp, rs=rs, Wn=Wn, fs=fs, output='sos')
-    filtered_signal = signal.sosfiltfilt(sos, s)
-    return filtered_signal
+    if btype == "bandpass" and not isinstance(Wn, list):
+        raise ValueError("Wn must be list type in case of bandpass filter")
+    elif (btype == "highpass" or btype == "lowpass") and not isinstance(
+        Wn, (int, float)
+    ):
+        raise ValueError(f"Wn must be a scalar in case of {btype} filter")
+    sos = signal.ellip(N=n, btype=btype, rp=rp, rs=rs, Wn=Wn, fs=fs, output="sos")
+    s[leads, :] = signal.sosfiltfilt(sos, s[leads, :])
+    return s
 
 
 def minmax_normalization(
     s: np.ndarray,
 ) -> np.ndarray:
     """
     minmax_normalization
     :param s: signal
 
     :return: preprocessed data
     """
-    
-    return (s-np.min(s))/(np.max(s)-np.min(s))
+    smin = np.min(s)
+    smax = np.max(s)
+    s = (s - smin) / (smax - smin)
+    return s
 
 
 def z_normalization(
     s: np.ndarray,
+    handle_constant_axis: bool=False,
 ) -> np.ndarray:
     """
     Z-normalization
     :param s: signal
+    :param handle_constant_axis: Flag indicating whether to handle constant values in the signal.
 
     :return: preprocessed data
     """
-    
-    return zscore(s, axis=1, nan_policy='raise')
-
-
-def cycle_normalization(
-    s: np.ndarray,
-) -> np.ndarray:
-    """
-    Cycle normalization
-    :param s: one lead signal
-
-    :return: preprocessed data
-    """
-
-    smin = np.min(s)
-    smax = np.max(s)
-    n = len(s) - 1
-    i = np.arange(len(s))
-    return ((n - i) / n) * ((s - smin) / (smax - smin)) + (i / n) * ((s - smin) / (smax - smin))
+    s_norm = zscore(s, axis=1, nan_policy="raise")
+    if handle_constant_axis:
+        same_values = np.all(s == s[:, 0][:, np.newaxis], axis=1)
+        s_norm[same_values] = 0
+    return s_norm
 
 
 def DWT_filter(
-    s: np.ndarray, 
-    wavelet: str = 'db4', 
-    level: int = 3, 
-    threshold: float = 2, 
+    s: np.ndarray,
+    wavelet: str = "db4",
+    level: int = 3,
+    threshold: float = 2,
     low: float = 1e6,
 ) -> np.ndarray:
     """
     Discrete wavelet transform augmentation
     :param s: one lead signal
     :param wavelet: wavelet name
     :param level: decomposition level
     :param threshold: thresholding value for all coefficients except the first one
     :param low: thresholding value for the first coefficient
 
     :return: preprocessed data
     """
-    
+
     w = pywt.Wavelet(wavelet)
     maxlev = pywt.dwt_max_level(len(s), w.dec_len)
 
     assert maxlev >= level
 
     coeffs = pywt.wavedec(s, w, level=level)
     for i in range(1, len(coeffs)):
-        coeffs[i] = pywt.threshold(coeffs[i], threshold * np.sqrt(np.log2(len(coeffs[i]))), mode='soft')
-    coeffs[0] = pywt.threshold(coeffs[0], low, mode='less')
-    return pywt.waverec(coeffs, wavelet, mode='periodic')
+        coeffs[i] = pywt.threshold(
+            coeffs[i], threshold * np.sqrt(np.log2(len(coeffs[i]))), mode="soft"
+        )
+    coeffs[0] = pywt.threshold(coeffs[0], low, mode="less")
+    return pywt.waverec(coeffs, wavelet, mode="periodic")
 
 
 def SWT_filter(
-    s: np.ndarray, 
-    wavelet: str = 'db4', 
+    s: np.ndarray,
+    wavelet: str = "db4",
     level: int = 6,
 ) -> np.ndarray:
     """
     Stationary wavelet transform augmentation
     :param s: one lead signal
     :param wavelet: wavelet name
     :param level: decomposition level
 
     :return: preprocessed data
     """
-    
+
     if len(s) % 2 == 0:
-        width = (2**int(np.ceil(np.log2(len(s)))) - len(s)) // 2
-        s_padded = np.pad(s, pad_width=width, mode='symmetric')
+        width = (2 ** int(np.ceil(np.log2(len(s)))) - len(s)) // 2
+        s_padded = np.pad(s, pad_width=width, mode="symmetric")
     else:
-        width1 = (2**int(np.ceil(np.log2(len(s)))) - len(s)) // 2
-        width2 = (2**int(np.ceil(np.log2(len(s)))) - len(s)) // 2 + 1
-        s_padded = np.pad(s, pad_width=(width1, width2), mode='symmetric')
-    
+        width1 = (2 ** int(np.ceil(np.log2(len(s)))) - len(s)) // 2
+        width2 = (2 ** int(np.ceil(np.log2(len(s)))) - len(s)) // 2 + 1
+        s_padded = np.pad(s, pad_width=(width1, width2), mode="symmetric")
+
     w = pywt.Wavelet(wavelet)
     maxlev = pywt.swt_max_level(len(s_padded))
 
     assert maxlev >= level
 
     coeffs = pywt.swt(s_padded, w, level=level, trim_approx=True, norm=True)
     return pywt.iswt(coeffs, wavelet, norm=True)
 
 
 def lead_crop(
-    record: np.ndarray, 
+    record: np.ndarray,
     leads: list,
 ) -> np.ndarray:
     """
     Lead crop augmentation
     :param record: signal
     :param leads: leads to be cropped
 
     :return: preprocessed data
     """
-    
+
     record[leads, :] = np.zeros(record.shape[1])
     return record
 
 
 def time_crop(
-    record: np.ndarray, 
-    time: int, 
+    record: np.ndarray,
+    time: int,
     leads: list,
 ) -> np.ndarray:
     """
     Time crop augmentation
     :param record: signal
     :param time: length of time segment to be cropped (the same units as signal)
     :param leads: leads to be cropped
 
     :return: preprocessed data
     """
-    
+
     assert time <= record.shape[1]
     for lead in leads:
-        ls = np.arange(0, len(record[lead])-time, dtype="int")
+        ls = np.arange(0, len(record[lead]) - time, dtype="int")
         start = np.random.choice(ls)
-        record[lead, start:start+time] = 0
+        record[lead, start : start + time] = 0
     return record
 
 
 def sum_augmentation(
     record: np.ndarray,
     leads: list,
 ) -> np.ndarray:
     """
     Signal summation augmentation
-    
+
     :param record: signal
     :param leads: leads to be replaced by sum of all leads
 
     :return: preprocessed data
     """
-    
+
     record[leads, :] = np.sum(record, axis=0)
     return record
 
 
-def reflect_augmentation(
-    record: np.ndarray,
-) -> np.ndarray:
-    """
-    Reflection augmentation
-    
-    :param record: signal
-
-    :return: preprocessed data
-    :rtype: numpy 2d array
-    """
-    
-    return -record
-
-
 def convex_augmentation(
     record: np.ndarray,
     leads: list,
 ) -> np.ndarray:
     """
     Convex augmentation
-    
+
     :param record: signal
     :param leads: leads to be replaced by convex combination of some leads (chosen randomly)
 
     :return: preprocessed data
     """
-    
+
     result = copy.deepcopy(record)
-    ls = np.arange(12, dtype='int')
+    ls = np.arange(12, dtype="int")
     for ltr in leads:
-        ln = np.random.randint(12, size=1)[0]
+        ln = np.random.randint(1, 13, size=1)[0]
         leads_to_sum = np.random.choice(ls, size=ln, replace=False)
         convex_coeffs = np.random.dirichlet(np.ones(ln), size=1)[0]
         if ln != 0:
             result[ltr, :] = np.dot(convex_coeffs, record[leads_to_sum, :])
     return result
 
 
-def ecg_to_one_frequency(
-    ecg_record: np.ndarray, 
-    ecg_frequency: int, 
-    requested_frequency: int,
-) -> np.ndarray:
-    """
-    Frequency resample
-    :param record: signal
-    :param ecg_frequency: sampling frequency of a signal
-    :param requested_frequency: sampling frequency of a preprocessed signal
-
-    :return: preprocessed data
-    """
-    
-    if ecg_frequency == requested_frequency:
-        return ecg_record
-    ecg_record = signal.resample(ecg_record, int(ecg_record.shape[1] * requested_frequency / ecg_frequency), axis=1)
-    return ecg_record
-
-
 def DWT_BW(
-    s: np.ndarray, 
-    wavelet: str = 'db4',
-)-> np.ndarray:
+    s: np.ndarray,
+    wavelet: str = "db4",
+) -> np.ndarray:
     """
     Remove baseline wander using wavelets (see article https://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.308.6789&rep=rep1&type=pdf)
     :param s: one lead signal
     :param wavelet: wavelet name
 
     :return: preprocessed data
     """
-    
+
     w = pywt.Wavelet(wavelet)
     maxlev = pywt.dwt_max_level(len(s), w.dec_len)
-    
+
     diffs = []
     for i in range(1, maxlev + 1):
-        coeffs = pywt.wavedec(s, w, level=i, mode='periodic')
-        diff = np.sum(np.square(coeffs[0])) - np.sum([np.sum(np.square(coeffs[j])) for j in range(1, i)])
+        coeffs = pywt.wavedec(s, w, level=i, mode="periodic")
+        diff = np.sum(np.square(coeffs[0])) - np.sum(
+            [np.sum(np.square(coeffs[j])) for j in range(1, i)]
+        )
         diffs.append(diff)
     diffs = np.array(diffs)
     if np.max(diffs) > 6500:
         ixs = np.where(diffs > 6500)[0]
         ix = ixs[np.argmin(diffs[ixs])]
-        coeffs = pywt.wavedec(s, w, level=ix, mode='periodic')
-        coeffs[0] = np.array([0]* len(coeffs[0]))
+        coeffs = pywt.wavedec(s, w, level=ix, mode="periodic")
+        coeffs[0] = np.array([0] * len(coeffs[0]))
     else:
         ix = np.argmin(diffs[-3:])
         ix += len(diffs) - 3
-        coeffs = pywt.wavedec(s, w, level=ix, mode='periodic')
-        coeffs[0] = np.array([0]* len(coeffs[0]))
-    return pywt.waverec(coeffs, wavelet, mode='periodic')
-
-
-def cut_ecg(
-    data: np.ndarray, 
-    cut_range: list, 
-    frequency: int,
-) -> np.ndarray:
-    """
-    Cut signal edges 
-    :param data: signal
-    :param cut_range: cutting parameters
-    :param frequency: sampling frequency of a signal
-
-    :return: preprocessed data
-    """
-    
-    cut_data = []
-    start = int(cut_range[0]*frequency)
-    for rec in data:
-        end = -int(cut_range[1]*frequency) if cut_range[1] != 0 else len(rec)
-        cut_data.append(rec[start: end])
-
-    return np.array(cut_data)
+        coeffs = pywt.wavedec(s, w, level=ix, mode="periodic")
+        coeffs[0] = np.array([0] * len(coeffs[0]))
+    return pywt.waverec(coeffs, wavelet, mode="periodic")
```

