# Comparing `tmp/SeqLbToolkit-0.3.4.tar.gz` & `tmp/SeqLbToolkit-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SeqLbToolkit-0.3.4.tar", last modified: Wed Mar 15 20:03:06 2023, max compression
+gzip compressed data, was "SeqLbToolkit-0.3.5.tar", last modified: Tue Jun 20 21:33:59 2023, max compression
```

## Comparing `SeqLbToolkit-0.3.4.tar` & `SeqLbToolkit-0.3.5.tar`

### file list

```diff
@@ -1,41 +1,46 @@
-drwxr-xr-x   0 yli        (501) staff       (20)        0 2023-03-15 20:03:06.234531 SeqLbToolkit-0.3.4/
--rw-r--r--   0 yli        (501) staff       (20)     1074 2023-01-07 15:15:18.000000 SeqLbToolkit-0.3.4/LICENSE
--rw-r--r--   0 yli        (501) staff       (20)     1686 2023-03-15 20:03:06.234405 SeqLbToolkit-0.3.4/PKG-INFO
--rw-r--r--   0 yli        (501) staff       (20)      943 2023-01-31 21:35:27.000000 SeqLbToolkit-0.3.4/README.md
-drwxr-xr-x   0 yli        (501) staff       (20)        0 2023-03-15 20:03:06.228184 SeqLbToolkit-0.3.4/SeqLbToolkit.egg-info/
--rw-r--r--   0 yli        (501) staff       (20)     1686 2023-03-15 20:03:06.000000 SeqLbToolkit-0.3.4/SeqLbToolkit.egg-info/PKG-INFO
--rw-r--r--   0 yli        (501) staff       (20)      864 2023-03-15 20:03:06.000000 SeqLbToolkit-0.3.4/SeqLbToolkit.egg-info/SOURCES.txt
--rw-r--r--   0 yli        (501) staff       (20)        1 2023-03-15 20:03:06.000000 SeqLbToolkit-0.3.4/SeqLbToolkit.egg-info/dependency_links.txt
--rw-r--r--   0 yli        (501) staff       (20)        1 2023-01-07 15:34:32.000000 SeqLbToolkit-0.3.4/SeqLbToolkit.egg-info/not-zip-safe
--rw-r--r--   0 yli        (501) staff       (20)       13 2023-03-15 20:03:06.000000 SeqLbToolkit-0.3.4/SeqLbToolkit.egg-info/top_level.txt
--rw-r--r--   0 yli        (501) staff       (20)       85 2023-01-07 15:15:18.000000 SeqLbToolkit-0.3.4/pyproject.toml
-drwxr-xr-x   0 yli        (501) staff       (20)        0 2023-03-15 20:03:06.229577 SeqLbToolkit-0.3.4/seqlbtoolkit/
--rw-r--r--   0 yli        (501) staff       (20)        0 2023-01-07 15:15:18.000000 SeqLbToolkit-0.3.4/seqlbtoolkit/__init__.py
-drwxr-xr-x   0 yli        (501) staff       (20)        0 2023-03-15 20:03:06.230265 SeqLbToolkit-0.3.4/seqlbtoolkit/bert_ner/
--rw-r--r--   0 yli        (501) staff       (20)        0 2023-01-07 15:15:18.000000 SeqLbToolkit-0.3.4/seqlbtoolkit/bert_ner/__init__.py
--rw-r--r--   0 yli        (501) staff       (20)      612 2023-02-15 19:03:51.000000 SeqLbToolkit-0.3.4/seqlbtoolkit/bert_ner/config.py
--rw-r--r--   0 yli        (501) staff       (20)     9833 2023-02-15 19:03:51.000000 SeqLbToolkit-0.3.4/seqlbtoolkit/bert_ner/dataset.py
-drwxr-xr-x   0 yli        (501) staff       (20)        0 2023-03-15 20:03:06.231359 SeqLbToolkit-0.3.4/seqlbtoolkit/chmm/
--rw-r--r--   0 yli        (501) staff       (20)        0 2023-01-07 15:15:18.000000 SeqLbToolkit-0.3.4/seqlbtoolkit/chmm/__init__.py
--rw-r--r--   0 yli        (501) staff       (20)     1296 2023-02-15 19:03:51.000000 SeqLbToolkit-0.3.4/seqlbtoolkit/chmm/config.py
--rw-r--r--   0 yli        (501) staff       (20)    18833 2023-02-15 19:03:51.000000 SeqLbToolkit-0.3.4/seqlbtoolkit/chmm/dataset.py
--rw-r--r--   0 yli        (501) staff       (20)    19889 2023-02-15 19:03:51.000000 SeqLbToolkit-0.3.4/seqlbtoolkit/chmm/train.py
--rw-r--r--   0 yli        (501) staff       (20)    14384 2023-01-31 22:05:36.000000 SeqLbToolkit-0.3.4/seqlbtoolkit/data.py
--rw-r--r--   0 yli        (501) staff       (20)     8438 2023-01-13 22:29:30.000000 SeqLbToolkit-0.3.4/seqlbtoolkit/embs.py
--rw-r--r--   0 yli        (501) staff       (20)     4777 2023-03-15 20:02:25.000000 SeqLbToolkit-0.3.4/seqlbtoolkit/io.py
--rw-r--r--   0 yli        (501) staff       (20)    12633 2023-01-13 20:09:16.000000 SeqLbToolkit-0.3.4/seqlbtoolkit/text.py
-drwxr-xr-x   0 yli        (501) staff       (20)        0 2023-03-15 20:03:06.233141 SeqLbToolkit-0.3.4/seqlbtoolkit/training/
--rw-r--r--   0 yli        (501) staff       (20)        0 2023-01-07 15:15:18.000000 SeqLbToolkit-0.3.4/seqlbtoolkit/training/__init__.py
--rw-r--r--   0 yli        (501) staff       (20)     5515 2023-02-15 19:08:24.000000 SeqLbToolkit-0.3.4/seqlbtoolkit/training/config.py
--rw-r--r--   0 yli        (501) staff       (20)    11104 2023-02-08 20:30:47.000000 SeqLbToolkit-0.3.4/seqlbtoolkit/training/dataset.py
--rw-r--r--   0 yli        (501) staff       (20)     5827 2023-01-11 17:20:16.000000 SeqLbToolkit-0.3.4/seqlbtoolkit/training/eval.py
--rw-r--r--   0 yli        (501) staff       (20)     4594 2023-01-07 15:15:18.000000 SeqLbToolkit-0.3.4/seqlbtoolkit/training/output.py
--rw-r--r--   0 yli        (501) staff       (20)     4135 2023-02-17 17:51:39.000000 SeqLbToolkit-0.3.4/seqlbtoolkit/training/status.py
--rw-r--r--   0 yli        (501) staff       (20)    10421 2023-02-17 17:45:44.000000 SeqLbToolkit-0.3.4/seqlbtoolkit/training/train.py
--rw-r--r--   0 yli        (501) staff       (20)      132 2023-01-07 15:15:18.000000 SeqLbToolkit-0.3.4/seqlbtoolkit/utils.py
--rw-r--r--   0 yli        (501) staff       (20)       38 2023-03-15 20:03:06.234570 SeqLbToolkit-0.3.4/setup.cfg
--rw-r--r--   0 yli        (501) staff       (20)     1009 2023-03-15 20:02:57.000000 SeqLbToolkit-0.3.4/setup.py
-drwxr-xr-x   0 yli        (501) staff       (20)        0 2023-03-15 20:03:06.234009 SeqLbToolkit-0.3.4/test/
--rw-r--r--   0 yli        (501) staff       (20)     2981 2023-01-13 22:30:10.000000 SeqLbToolkit-0.3.4/test/test_build_embeddings.py
--rw-r--r--   0 yli        (501) staff       (20)      613 2023-02-15 19:03:51.000000 SeqLbToolkit-0.3.4/test/test_ner_metrics.py
--rw-r--r--   0 yli        (501) staff       (20)       94 2023-01-20 19:18:56.000000 SeqLbToolkit-0.3.4/test/test_save_json.py
+drwxr-xr-x   0 yli        (501) staff       (20)        0 2023-06-20 21:33:59.017707 SeqLbToolkit-0.3.5/
+-rw-r--r--   0 yli        (501) staff       (20)     1074 2022-09-08 14:47:31.000000 SeqLbToolkit-0.3.5/LICENSE
+-rw-r--r--   0 yli        (501) staff       (20)     1686 2023-06-20 21:33:59.017581 SeqLbToolkit-0.3.5/PKG-INFO
+-rw-r--r--   0 yli        (501) staff       (20)      943 2023-02-16 19:28:11.000000 SeqLbToolkit-0.3.5/README.md
+drwxr-xr-x   0 yli        (501) staff       (20)        0 2023-06-20 21:33:59.010909 SeqLbToolkit-0.3.5/SeqLbToolkit.egg-info/
+-rw-r--r--   0 yli        (501) staff       (20)     1686 2023-06-20 21:33:59.000000 SeqLbToolkit-0.3.5/SeqLbToolkit.egg-info/PKG-INFO
+-rw-r--r--   0 yli        (501) staff       (20)     1045 2023-06-20 21:33:59.000000 SeqLbToolkit-0.3.5/SeqLbToolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 yli        (501) staff       (20)        1 2023-06-20 21:33:59.000000 SeqLbToolkit-0.3.5/SeqLbToolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 yli        (501) staff       (20)        1 2022-09-08 15:16:57.000000 SeqLbToolkit-0.3.5/SeqLbToolkit.egg-info/not-zip-safe
+-rw-r--r--   0 yli        (501) staff       (20)       13 2023-06-20 21:33:59.000000 SeqLbToolkit-0.3.5/SeqLbToolkit.egg-info/top_level.txt
+-rw-r--r--   0 yli        (501) staff       (20)       85 2022-09-08 14:47:31.000000 SeqLbToolkit-0.3.5/pyproject.toml
+drwxr-xr-x   0 yli        (501) staff       (20)        0 2023-06-20 21:33:59.012144 SeqLbToolkit-0.3.5/seqlbtoolkit/
+-rw-r--r--   0 yli        (501) staff       (20)        0 2022-09-08 14:47:31.000000 SeqLbToolkit-0.3.5/seqlbtoolkit/__init__.py
+drwxr-xr-x   0 yli        (501) staff       (20)        0 2023-06-20 21:33:59.012697 SeqLbToolkit-0.3.5/seqlbtoolkit/bert_ner/
+-rw-r--r--   0 yli        (501) staff       (20)        0 2022-09-08 14:47:31.000000 SeqLbToolkit-0.3.5/seqlbtoolkit/bert_ner/__init__.py
+-rw-r--r--   0 yli        (501) staff       (20)      612 2023-02-16 19:28:11.000000 SeqLbToolkit-0.3.5/seqlbtoolkit/bert_ner/config.py
+-rw-r--r--   0 yli        (501) staff       (20)     9833 2023-02-16 19:28:11.000000 SeqLbToolkit-0.3.5/seqlbtoolkit/bert_ner/dataset.py
+drwxr-xr-x   0 yli        (501) staff       (20)        0 2023-06-20 21:33:59.013379 SeqLbToolkit-0.3.5/seqlbtoolkit/chmm/
+-rw-r--r--   0 yli        (501) staff       (20)        0 2022-09-08 14:47:31.000000 SeqLbToolkit-0.3.5/seqlbtoolkit/chmm/__init__.py
+-rw-r--r--   0 yli        (501) staff       (20)     1296 2023-02-16 19:28:11.000000 SeqLbToolkit-0.3.5/seqlbtoolkit/chmm/config.py
+-rw-r--r--   0 yli        (501) staff       (20)    18833 2023-02-16 19:28:11.000000 SeqLbToolkit-0.3.5/seqlbtoolkit/chmm/dataset.py
+-rw-r--r--   0 yli        (501) staff       (20)    19889 2023-02-16 19:28:11.000000 SeqLbToolkit-0.3.5/seqlbtoolkit/chmm/train.py
+-rw-r--r--   0 yli        (501) staff       (20)    14384 2023-02-16 19:28:11.000000 SeqLbToolkit-0.3.5/seqlbtoolkit/data.py
+-rw-r--r--   0 yli        (501) staff       (20)     8438 2023-01-19 20:41:35.000000 SeqLbToolkit-0.3.5/seqlbtoolkit/embs.py
+-rw-r--r--   0 yli        (501) staff       (20)     4777 2023-06-19 22:15:13.000000 SeqLbToolkit-0.3.5/seqlbtoolkit/io.py
+-rw-r--r--   0 yli        (501) staff       (20)    12633 2023-01-19 20:41:35.000000 SeqLbToolkit-0.3.5/seqlbtoolkit/text.py
+drwxr-xr-x   0 yli        (501) staff       (20)        0 2023-06-20 21:33:59.014420 SeqLbToolkit-0.3.5/seqlbtoolkit/training/
+-rw-r--r--   0 yli        (501) staff       (20)        0 2023-02-16 19:28:11.000000 SeqLbToolkit-0.3.5/seqlbtoolkit/training/__init__.py
+-rw-r--r--   0 yli        (501) staff       (20)     5511 2023-06-20 21:32:24.000000 SeqLbToolkit-0.3.5/seqlbtoolkit/training/config.py
+drwxr-xr-x   0 yli        (501) staff       (20)        0 2023-06-20 21:33:59.016205 SeqLbToolkit-0.3.5/seqlbtoolkit/training/dataset/
+-rw-r--r--   0 yli        (501) staff       (20)      460 2023-06-20 21:32:24.000000 SeqLbToolkit-0.3.5/seqlbtoolkit/training/dataset/__init__.py
+-rw-r--r--   0 yli        (501) staff       (20)     2176 2023-06-20 21:22:37.000000 SeqLbToolkit-0.3.5/seqlbtoolkit/training/dataset/base_dataset.py
+-rw-r--r--   0 yli        (501) staff       (20)     1750 2023-06-20 21:17:23.000000 SeqLbToolkit-0.3.5/seqlbtoolkit/training/dataset/batching.py
+-rw-r--r--   0 yli        (501) staff       (20)     4378 2023-06-20 21:22:37.000000 SeqLbToolkit-0.3.5/seqlbtoolkit/training/dataset/ner_dataset.py
+-rw-r--r--   0 yli        (501) staff       (20)     7688 2023-06-20 21:17:23.000000 SeqLbToolkit-0.3.5/seqlbtoolkit/training/dataset/utils.py
+-rw-r--r--   0 yli        (501) staff       (20)     5798 2023-06-20 21:32:24.000000 SeqLbToolkit-0.3.5/seqlbtoolkit/training/eval.py
+-rw-r--r--   0 yli        (501) staff       (20)     4594 2023-02-16 19:28:11.000000 SeqLbToolkit-0.3.5/seqlbtoolkit/training/output.py
+-rw-r--r--   0 yli        (501) staff       (20)     4135 2023-06-19 22:15:13.000000 SeqLbToolkit-0.3.5/seqlbtoolkit/training/status.py
+-rw-r--r--   0 yli        (501) staff       (20)    10421 2023-02-16 19:28:11.000000 SeqLbToolkit-0.3.5/seqlbtoolkit/training/train.py
+-rw-r--r--   0 yli        (501) staff       (20)      132 2022-09-08 14:47:31.000000 SeqLbToolkit-0.3.5/seqlbtoolkit/utils.py
+-rw-r--r--   0 yli        (501) staff       (20)       38 2023-06-20 21:33:59.017741 SeqLbToolkit-0.3.5/setup.cfg
+-rw-r--r--   0 yli        (501) staff       (20)     1009 2023-06-20 21:32:48.000000 SeqLbToolkit-0.3.5/setup.py
+drwxr-xr-x   0 yli        (501) staff       (20)        0 2023-06-20 21:33:59.017092 SeqLbToolkit-0.3.5/test/
+-rw-r--r--   0 yli        (501) staff       (20)     2981 2023-01-19 20:41:35.000000 SeqLbToolkit-0.3.5/test/test_build_embeddings.py
+-rw-r--r--   0 yli        (501) staff       (20)      613 2023-02-16 19:28:11.000000 SeqLbToolkit-0.3.5/test/test_ner_metrics.py
+-rw-r--r--   0 yli        (501) staff       (20)       94 2023-01-24 20:32:27.000000 SeqLbToolkit-0.3.5/test/test_save_json.py
```

### Comparing `SeqLbToolkit-0.3.4/LICENSE` & `SeqLbToolkit-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `SeqLbToolkit-0.3.4/PKG-INFO` & `SeqLbToolkit-0.3.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: SeqLbToolkit
-Version: 0.3.4
+Version: 0.3.5
 Summary: Commonly-used functions for building sequence labeling models.
 Home-page: https://github.com/Yinghao-Li/seqlbtoolkit
 Author: Yinghao Li
 Author-email: yinghaoli@gatech.edu
 License: MIT
 Keywords: nlp sequence-labeling ml machine-learning natural-language-processing
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Text Processing :: Linguistic
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SeqLbToolkit
 
 This repo realizes Sequence Labeling Toolkits, a toolkit box containing useful functions for accelerating implementing sequences labeling deep learning models such as BiLSTM-CRF or BERT for Token Classification.
```

### Comparing `SeqLbToolkit-0.3.4/README.md` & `SeqLbToolkit-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `SeqLbToolkit-0.3.4/SeqLbToolkit.egg-info/PKG-INFO` & `SeqLbToolkit-0.3.5/SeqLbToolkit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: SeqLbToolkit
-Version: 0.3.4
+Version: 0.3.5
 Summary: Commonly-used functions for building sequence labeling models.
 Home-page: https://github.com/Yinghao-Li/seqlbtoolkit
 Author: Yinghao Li
 Author-email: yinghaoli@gatech.edu
 License: MIT
 Keywords: nlp sequence-labeling ml machine-learning natural-language-processing
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Text Processing :: Linguistic
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SeqLbToolkit
 
 This repo realizes Sequence Labeling Toolkits, a toolkit box containing useful functions for accelerating implementing sequences labeling deep learning models such as BiLSTM-CRF or BERT for Token Classification.
```

### Comparing `SeqLbToolkit-0.3.4/SeqLbToolkit.egg-info/SOURCES.txt` & `SeqLbToolkit-0.3.5/SeqLbToolkit.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -18,15 +18,19 @@
 seqlbtoolkit/bert_ner/dataset.py
 seqlbtoolkit/chmm/__init__.py
 seqlbtoolkit/chmm/config.py
 seqlbtoolkit/chmm/dataset.py
 seqlbtoolkit/chmm/train.py
 seqlbtoolkit/training/__init__.py
 seqlbtoolkit/training/config.py
-seqlbtoolkit/training/dataset.py
 seqlbtoolkit/training/eval.py
 seqlbtoolkit/training/output.py
 seqlbtoolkit/training/status.py
 seqlbtoolkit/training/train.py
+seqlbtoolkit/training/dataset/__init__.py
+seqlbtoolkit/training/dataset/base_dataset.py
+seqlbtoolkit/training/dataset/batching.py
+seqlbtoolkit/training/dataset/ner_dataset.py
+seqlbtoolkit/training/dataset/utils.py
 test/test_build_embeddings.py
 test/test_ner_metrics.py
 test/test_save_json.py
```

### Comparing `SeqLbToolkit-0.3.4/seqlbtoolkit/bert_ner/config.py` & `SeqLbToolkit-0.3.5/seqlbtoolkit/bert_ner/config.py`

 * *Files identical despite different names*

### Comparing `SeqLbToolkit-0.3.4/seqlbtoolkit/bert_ner/dataset.py` & `SeqLbToolkit-0.3.5/seqlbtoolkit/bert_ner/dataset.py`

 * *Files identical despite different names*

### Comparing `SeqLbToolkit-0.3.4/seqlbtoolkit/chmm/config.py` & `SeqLbToolkit-0.3.5/seqlbtoolkit/chmm/config.py`

 * *Files identical despite different names*

### Comparing `SeqLbToolkit-0.3.4/seqlbtoolkit/chmm/dataset.py` & `SeqLbToolkit-0.3.5/seqlbtoolkit/chmm/dataset.py`

 * *Files identical despite different names*

### Comparing `SeqLbToolkit-0.3.4/seqlbtoolkit/chmm/train.py` & `SeqLbToolkit-0.3.5/seqlbtoolkit/chmm/train.py`

 * *Files identical despite different names*

### Comparing `SeqLbToolkit-0.3.4/seqlbtoolkit/data.py` & `SeqLbToolkit-0.3.5/seqlbtoolkit/data.py`

 * *Files identical despite different names*

### Comparing `SeqLbToolkit-0.3.4/seqlbtoolkit/embs.py` & `SeqLbToolkit-0.3.5/seqlbtoolkit/embs.py`

 * *Files identical despite different names*

### Comparing `SeqLbToolkit-0.3.4/seqlbtoolkit/io.py` & `SeqLbToolkit-0.3.5/seqlbtoolkit/io.py`

 * *Files identical despite different names*

### Comparing `SeqLbToolkit-0.3.4/seqlbtoolkit/text.py` & `SeqLbToolkit-0.3.5/seqlbtoolkit/text.py`

 * *Files identical despite different names*

### Comparing `SeqLbToolkit-0.3.4/seqlbtoolkit/training/config.py` & `SeqLbToolkit-0.3.5/seqlbtoolkit/training/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,15 @@
                 setattr(self, attr, value)
             except AttributeError:
                 pass
         return self
 
 
 @dataclass
-class BaseNERConfig(BaseConfig):
+class NERConfig(BaseConfig):
 
     entity_types: Optional[List[str]] = None
     bio_label_types: Optional[List[str]] = None
 
     @property
     def n_lbs(self) -> "int":
         """
```

### Comparing `SeqLbToolkit-0.3.4/seqlbtoolkit/training/dataset.py` & `SeqLbToolkit-0.3.5/seqlbtoolkit/training/dataset/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,154 +1,29 @@
+
 import os
 import regex
 import json
 import logging
-from typing import Optional, List
+from typing import Optional
 from string import printable
-from dataclasses import dataclass
 
 import torch
 import numpy as np
 
-from .config import BaseNERConfig
-from ..data import (
+from seqlbtoolkit.training.config import BaseNERConfig
+from seqlbtoolkit.data import (
     span_to_label,
     span_list_to_dict,
     entity_to_bio_labels,
     one_hot,
 )
 
 logger = logging.getLogger(__name__)
 
 
-@dataclass
-class DataInstance:
-    def __setitem__(self, k, v):
-        self.__dict__.update(zip(k, v) if type(k) is tuple else [(k, v)])
-
-
-class BaseDataset(torch.utils.data.Dataset):
-    def __init__(self):
-        super().__init__()
-        # Whether the text and lbs sequences are separated according to maximum BERT input lengths
-        self.data_instances = None
-
-    def __len__(self):
-        return len(self.data_instances) if self.data_instances else 0
-
-    def __getitem__(self, idx):
-        return self.data_instances[idx]
-
-    def prepare(self, config, partition: str):
-        """
-        Load data from disk
-        Parameters
-        ----------
-        config: configurations
-        partition: dataset partition; in [train, valid, test]
-        Returns
-        -------
-        self (MultiSrcNERDataset)
-        """
-        raise NotImplementedError
-
-    def prepare_debug(self, n_inst: Optional[int] = 100):
-        for attr in self.__dict__.keys():
-            if regex.match(f"^_[a-z]", attr):
-                try:
-                    setattr(self, attr, getattr(self, attr)[:n_inst])
-                except TypeError:
-                    pass
-
-        return self
-
-    def save(self, file_path: str):
-        """
-        Save the entire dataset for future usage
-        Parameters
-        ----------
-        file_path: path to the saved file
-        Returns
-        -------
-        self
-        """
-        attr_dict = dict()
-        for attr, value in self.__dict__.items():
-            if regex.match(f"^_[a-z]", attr):
-                attr_dict[attr] = value
-
-        os.makedirs(os.path.dirname(os.path.normpath(file_path)), exist_ok=True)
-        torch.save(attr_dict, file_path)
-
-        return self
-
-    def load(self, file_path: str):
-        """
-        Load the entire dataset from disk
-        Parameters
-        ----------
-        file_path: path to the saved file
-        Returns
-        -------
-        self
-        """
-        attr_dict = torch.load(file_path)
-
-        for attr, value in attr_dict.items():
-            if attr not in self.__dict__:
-                logger.warning(f"Attribute {attr} is not natively defined in dataset!")
-
-            setattr(self, attr, value)
-
-        return self
-
-
-def feature_lists_to_instance_list(instance_class, **kwargs):
-    data_points = list()
-    keys = tuple(kwargs.keys())
-
-    for feature_point_list in zip(*tuple(kwargs.values())):
-        inst = instance_class()
-        inst[keys] = feature_point_list
-        data_points.append(inst)
-
-    return data_points
-
-
-def instance_list_to_feature_lists(instance_list: list, feature_names: Optional[List[str]] = None):
-    if not feature_names:
-        feature_names = list(instance_list[0].__dict__.keys())
-
-    features_lists = list()
-    for name in feature_names:
-        features_lists.append([getattr(inst, name) for inst in instance_list])
-
-    return features_lists
-
-
-class Batch:
-    def __init__(self, **kwargs):
-        super().__init__()
-        for k, v in kwargs.items():
-            setattr(self, k, v)
-
-    def to(self, device):
-        for k, v in self.__dict__.items():
-            try:
-                setattr(self, k, v.to(device))
-            except AttributeError:
-                pass
-        return self
-
-    def __len__(self):
-        for v in list(self.__dict__.values()):
-            if isinstance(v, torch.Tensor):
-                return v.shape[0]
-
-
 def load_data_from_json(file_dir: str, config: Optional[BaseNERConfig] = None):
     """
     Load data stored in the current data format.
 
 
     Parameters
     ----------
```

### Comparing `SeqLbToolkit-0.3.4/seqlbtoolkit/training/eval.py` & `SeqLbToolkit-0.3.5/seqlbtoolkit/training/eval.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,14 @@
         popped attribute
         """
         attr = getattr(self, k)
         setattr(self, k, None)
         return attr
 
 
-# noinspection PyTypeChecker
 def get_ner_metrics(true_lbs,
                     pred_lbs,
                     mode: Optional[str] = 'strict',
                     scheme: Optional = IOB2,
                     detailed: Optional[bool] = False):
     """
     Get NER metrics including precision, recall and f1
```

### Comparing `SeqLbToolkit-0.3.4/seqlbtoolkit/training/output.py` & `SeqLbToolkit-0.3.5/seqlbtoolkit/training/output.py`

 * *Files identical despite different names*

### Comparing `SeqLbToolkit-0.3.4/seqlbtoolkit/training/status.py` & `SeqLbToolkit-0.3.5/seqlbtoolkit/training/status.py`

 * *Files identical despite different names*

### Comparing `SeqLbToolkit-0.3.4/seqlbtoolkit/training/train.py` & `SeqLbToolkit-0.3.5/seqlbtoolkit/training/train.py`

 * *Files identical despite different names*

### Comparing `SeqLbToolkit-0.3.4/setup.py` & `SeqLbToolkit-0.3.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='SeqLbToolkit',
-    version='0.3.4',
+    version='0.3.5',
     author='Yinghao Li',
     author_email='yinghaoli@gatech.edu',
     license='MIT',
     url='https://github.com/Yinghao-Li/seqlbtoolkit',
     description='Commonly-used functions for building sequence labeling models.',
     long_description=long_description,
     long_description_content_type="text/markdown",
@@ -21,9 +21,9 @@
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
         'Topic :: Text Processing',
         'Topic :: Text Processing :: Linguistic',
     ],
     packages=find_packages(),
-    python_requires=">=3.6",
+    python_requires=">=3.9",
 )
```

### Comparing `SeqLbToolkit-0.3.4/test/test_build_embeddings.py` & `SeqLbToolkit-0.3.5/test/test_build_embeddings.py`

 * *Files identical despite different names*

### Comparing `SeqLbToolkit-0.3.4/test/test_ner_metrics.py` & `SeqLbToolkit-0.3.5/test/test_ner_metrics.py`

 * *Files identical despite different names*

