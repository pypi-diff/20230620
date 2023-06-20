# Comparing `tmp/autodistill_detic-0.1.2.tar.gz` & `tmp/autodistill_detic-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autodistill_detic-0.1.2.tar", last modified: Thu Jun  8 13:58:17 2023, max compression
+gzip compressed data, was "autodistill_detic-0.1.3.tar", last modified: Tue Jun 20 15:58:49 2023, max compression
```

## Comparing `autodistill_detic-0.1.2.tar` & `autodistill_detic-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-08 13:58:17.212259 autodistill_detic-0.1.2/
--rw-r--r--   0 james      (501) staff       (20)     1055 2023-06-06 11:14:33.000000 autodistill_detic-0.1.2/LICENSE.md
--rw-r--r--   0 james      (501) staff       (20)     2297 2023-06-08 13:58:17.212114 autodistill_detic-0.1.2/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)     1821 2023-06-06 11:15:52.000000 autodistill_detic-0.1.2/README.md
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-08 13:58:17.210645 autodistill_detic-0.1.2/autodistill_detic/
--rw-r--r--   0 james      (501) staff       (20)       71 2023-06-08 13:58:14.000000 autodistill_detic-0.1.2/autodistill_detic/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     4802 2023-06-07 14:22:07.000000 autodistill_detic-0.1.2/autodistill_detic/detic_model.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-08 13:58:17.211565 autodistill_detic-0.1.2/autodistill_detic.egg-info/
--rw-r--r--   0 james      (501) staff       (20)     2297 2023-06-08 13:58:17.000000 autodistill_detic-0.1.2/autodistill_detic.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      315 2023-06-08 13:58:17.000000 autodistill_detic-0.1.2/autodistill_detic.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2023-06-08 13:58:17.000000 autodistill_detic-0.1.2/autodistill_detic.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)       53 2023-06-08 13:58:17.000000 autodistill_detic-0.1.2/autodistill_detic.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)       18 2023-06-08 13:58:17.000000 autodistill_detic-0.1.2/autodistill_detic.egg-info/top_level.txt
--rw-r--r--   0 james      (501) staff       (20)       38 2023-06-08 13:58:17.212307 autodistill_detic-0.1.2/setup.cfg
--rw-r--r--   0 james      (501) staff       (20)     1161 2023-06-07 14:22:41.000000 autodistill_detic-0.1.2/setup.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-08 13:58:17.211720 autodistill_detic-0.1.2/test/
--rw-r--r--   0 james      (501) staff       (20)       91 2023-06-06 09:39:29.000000 autodistill_detic-0.1.2/test/test_hello.py
+drwxr-xr-x   0 arty      (1019) arty      (1020)        0 2023-06-20 15:58:49.594548 autodistill_detic-0.1.3/
+-rw-r--r--   0 arty      (1019) arty      (1020)     1055 2023-06-08 22:41:53.000000 autodistill_detic-0.1.3/LICENSE.md
+-rw-r--r--   0 arty      (1019) arty      (1020)     2297 2023-06-20 15:58:49.594548 autodistill_detic-0.1.3/PKG-INFO
+-rw-r--r--   0 arty      (1019) arty      (1020)     1821 2023-06-08 22:41:53.000000 autodistill_detic-0.1.3/README.md
+drwxr-xr-x   0 arty      (1019) arty      (1020)        0 2023-06-20 15:58:49.590548 autodistill_detic-0.1.3/autodistill_detic/
+-rw-r--r--   0 arty      (1019) arty      (1020)       71 2023-06-20 15:57:28.000000 autodistill_detic-0.1.3/autodistill_detic/__init__.py
+-rw-r--r--   0 arty      (1019) arty      (1020)     3841 2023-06-14 10:46:00.000000 autodistill_detic-0.1.3/autodistill_detic/detic_model.py
+drwxr-xr-x   0 arty      (1019) arty      (1020)        0 2023-06-20 15:58:49.594548 autodistill_detic-0.1.3/autodistill_detic.egg-info/
+-rw-r--r--   0 arty      (1019) arty      (1020)     2297 2023-06-20 15:58:49.000000 autodistill_detic-0.1.3/autodistill_detic.egg-info/PKG-INFO
+-rw-r--r--   0 arty      (1019) arty      (1020)      344 2023-06-20 15:58:49.000000 autodistill_detic-0.1.3/autodistill_detic.egg-info/SOURCES.txt
+-rw-r--r--   0 arty      (1019) arty      (1020)        1 2023-06-20 15:58:49.000000 autodistill_detic-0.1.3/autodistill_detic.egg-info/dependency_links.txt
+-rw-r--r--   0 arty      (1019) arty      (1020)       89 2023-06-20 15:58:49.000000 autodistill_detic-0.1.3/autodistill_detic.egg-info/requires.txt
+-rw-r--r--   0 arty      (1019) arty      (1020)       22 2023-06-20 15:58:49.000000 autodistill_detic-0.1.3/autodistill_detic.egg-info/top_level.txt
+-rw-r--r--   0 arty      (1019) arty      (1020)       38 2023-06-20 15:58:49.594548 autodistill_detic-0.1.3/setup.cfg
+-rw-r--r--   0 arty      (1019) arty      (1020)     1975 2023-06-14 10:49:59.000000 autodistill_detic-0.1.3/setup.py
+drwxr-xr-x   0 arty      (1019) arty      (1020)        0 2023-06-20 15:58:49.594548 autodistill_detic-0.1.3/src/
+-rw-r--r--   0 arty      (1019) arty      (1020)       22 2023-06-08 22:41:53.000000 autodistill_detic-0.1.3/src/__init__.py
+-rw-r--r--   0 arty      (1019) arty      (1020)       39 2023-06-08 22:41:53.000000 autodistill_detic-0.1.3/src/hello.py
+drwxr-xr-x   0 arty      (1019) arty      (1020)        0 2023-06-20 15:58:49.594548 autodistill_detic-0.1.3/test/
+-rw-r--r--   0 arty      (1019) arty      (1020)       91 2023-06-08 22:41:53.000000 autodistill_detic-0.1.3/test/test_hello.py
```

### Comparing `autodistill_detic-0.1.2/LICENSE.md` & `autodistill_detic-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `autodistill_detic-0.1.2/PKG-INFO` & `autodistill_detic-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autodistill_detic
-Version: 0.1.2
+Version: 0.1.3
 Summary: DETIC module for use with Autodistill
 Home-page: https://github.com/autodistill/autodistill-detic
 Author: Roboflow
 Author-email: support@roboflow.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `autodistill_detic-0.1.2/README.md` & `autodistill_detic-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `autodistill_detic-0.1.2/autodistill_detic/detic_model.py` & `autodistill_detic-0.1.3/autodistill_detic/detic_model.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import os
 from dataclasses import dataclass
-
 import numpy as np
 import supervision as sv
 import torch
-import subprocess
 from autodistill.detection import CaptionOntology, DetectionBaseModel
 
 import argparse
 import multiprocessing as mp
 import os
 import sys
 
@@ -51,62 +49,33 @@
     args.cpu = False if torch.cuda.is_available() else True
     args.opts.append("MODEL.WEIGHTS")
     args.opts.append("models/Detic_LCOCOI21k_CLIP_SwinB_896b32_4x_ft4x_max-size.pth")
     args.output = None
     args.webcam = None
     args.video_input = None
     args.custom_vocabulary = ", ".join(ontology.prompts()).rstrip(",")
-
+    print(args.custom_vocabulary)
     args.pred_all_class = False
     cfg = setup_cfg(args)
 
     from detic.predictor import VisualizationDemo
 
     demo = VisualizationDemo(cfg, args)
 
     return demo
 
 HOME = os.path.expanduser("~")
 DEVICE = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
-installation_commands = [
-    "mkdir ~/.cache/autodistill/",
-    "cd ~/.cache/autodistill/",
-    "git clone git@github.com:facebookresearch/detectron2.git",
-    "cd detectron2",
-    "pip install -e .",
-    "pip install -r requirements.txt",
-    "cd ..",
-    "git clone https://github.com/facebookresearch/Detic.git --recurse-submodules",
-    "cd Detic",
-    "pip install -r requirements.txt",
-    "mkdir models",
-    "wget https://dl.fbaipublicfiles.com/detic/Detic_LCOCOI21k_CLIP_SwinB_896b32_4x_ft4x_max-size.pth -O models/Detic_LCOCOI21k_CLIP_SwinB_896b32_4x_ft4x_max-size.pth"
-]
-
-def install_detic():
-    for command in installation_commands:
-        # keep track of pathi
-        if command.startswith("cd"):
-            # re[place ~ with home]
-            command = command.replace("~", HOME)
-            os.chdir(command.split(" ")[1])
-
-        subprocess.run(command, shell=True)
-
-
 @dataclass
 class DETIC(DetectionBaseModel):
     ontology: CaptionOntology
 
     def __init__(self, ontology: CaptionOntology):
         self.ontology = ontology
-        if not os.path.exists(HOME + "/.cache/autodistill/detectron2"):
-            install_detic()
-
         original_dir = os.getcwd()
 
         sys.path.insert(0, HOME + "/.cache/autodistill/Detic/third_party/CenterNet2/")
 
         sys.path.insert(0, HOME + "/.cache/autodistill/Detic/")
         os.chdir(HOME + "/.cache/autodistill/Detic/")
 
@@ -116,15 +85,15 @@
         os.chdir(original_dir)
 
     def predict(self, input: str) -> sv.Detections:
         labels = self.ontology.prompts()
 
         img = read_image(input, format="BGR")
 
-        predictions, _ = self.detic_model.run_on_image(img)
+        predictions, visualized_output = self.detic_model.run_on_image(img)
 
         pred_boxes = predictions["instances"].pred_boxes.tensor.cpu().numpy()
         pred_classes = predictions["instances"].pred_classes.cpu().numpy()
         pred_scores = predictions["instances"].scores.cpu().numpy()
 
         # filter out predictions that are not in the ontology
         final_pred_boxes = []
```

### Comparing `autodistill_detic-0.1.2/autodistill_detic.egg-info/PKG-INFO` & `autodistill_detic-0.1.3/autodistill_detic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autodistill-detic
-Version: 0.1.2
+Version: 0.1.3
 Summary: DETIC module for use with Autodistill
 Home-page: https://github.com/autodistill/autodistill-detic
 Author: Roboflow
 Author-email: support@roboflow.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

