# Comparing `tmp/sc2image-1.0.3.tar.gz` & `tmp/sc2image-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sc2image-1.0.3.tar", last modified: Fri Jun 16 20:58:35 2023, max compression
+gzip compressed data, was "dist/sc2image-1.0.4.tar", last modified: Tue Jun 20 03:38:18 2023, max compression
```

## Comparing `sc2image-1.0.3.tar` & `sc2image-1.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 seankulinski   (501) staff       (20)        0 2023-06-16 20:58:35.000000 sc2image-1.0.3/
--rw-r--r--   0 seankulinski   (501) staff       (20)     1067 2023-06-16 17:35:39.000000 sc2image-1.0.3/LICENSE
--rw-r--r--   0 seankulinski   (501) staff       (20)     4261 2023-06-16 20:58:35.000000 sc2image-1.0.3/PKG-INFO
--rw-r--r--   0 seankulinski   (501) staff       (20)     3741 2023-06-16 19:10:56.000000 sc2image-1.0.3/README.md
-drwxr-xr-x   0 seankulinski   (501) staff       (20)        0 2023-06-16 20:58:35.000000 sc2image-1.0.3/sc2image/
--rw-r--r--   0 seankulinski   (501) staff       (20)      134 2023-06-16 19:23:27.000000 sc2image-1.0.3/sc2image/__init__.py
--rw-r--r--   0 seankulinski   (501) staff       (20)    37125 2023-06-16 19:40:13.000000 sc2image-1.0.3/sc2image/dataset.py
-drwxr-xr-x   0 seankulinski   (501) staff       (20)        0 2023-06-16 20:58:35.000000 sc2image-1.0.3/sc2image/utils/
--rw-r--r--   0 seankulinski   (501) staff       (20)        0 2023-06-16 17:35:39.000000 sc2image-1.0.3/sc2image/utils/__init__.py
--rw-r--r--   0 seankulinski   (501) staff       (20)     2421 2023-06-16 18:21:35.000000 sc2image-1.0.3/sc2image/utils/metadata_processing.py
--rw-r--r--   0 seankulinski   (501) staff       (20)     6002 2023-06-16 17:35:39.000000 sc2image-1.0.3/sc2image/utils/sensor_utils.py
--rw-r--r--   0 seankulinski   (501) staff       (20)    24324 2023-06-16 17:35:39.000000 sc2image-1.0.3/sc2image/utils/unit_type_data.py
--rw-r--r--   0 seankulinski   (501) staff       (20)      705 2023-06-16 19:40:41.000000 sc2image-1.0.3/sc2image/version.py
-drwxr-xr-x   0 seankulinski   (501) staff       (20)        0 2023-06-16 20:58:35.000000 sc2image-1.0.3/sc2image.egg-info/
--rw-r--r--   0 seankulinski   (501) staff       (20)     4261 2023-06-16 20:58:35.000000 sc2image-1.0.3/sc2image.egg-info/PKG-INFO
--rw-r--r--   0 seankulinski   (501) staff       (20)      375 2023-06-16 20:58:35.000000 sc2image-1.0.3/sc2image.egg-info/SOURCES.txt
--rw-r--r--   0 seankulinski   (501) staff       (20)        1 2023-06-16 20:58:35.000000 sc2image-1.0.3/sc2image.egg-info/dependency_links.txt
--rw-r--r--   0 seankulinski   (501) staff       (20)      115 2023-06-16 20:58:35.000000 sc2image-1.0.3/sc2image.egg-info/requires.txt
--rw-r--r--   0 seankulinski   (501) staff       (20)        9 2023-06-16 20:58:35.000000 sc2image-1.0.3/sc2image.egg-info/top_level.txt
--rw-r--r--   0 seankulinski   (501) staff       (20)       38 2023-06-16 20:58:35.000000 sc2image-1.0.3/setup.cfg
--rw-r--r--   0 seankulinski   (501) staff       (20)     1184 2023-06-16 19:33:49.000000 sc2image-1.0.3/setup.py
+drwxr-xr-x   0 seankulinski   (501) staff       (20)        0 2023-06-20 03:38:18.000000 sc2image-1.0.4/
+-rw-r--r--   0 seankulinski   (501) staff       (20)     1067 2023-06-16 17:35:39.000000 sc2image-1.0.4/LICENSE
+-rw-r--r--   0 seankulinski   (501) staff       (20)     4956 2023-06-20 03:38:18.000000 sc2image-1.0.4/PKG-INFO
+-rw-r--r--   0 seankulinski   (501) staff       (20)     4417 2023-06-19 16:39:28.000000 sc2image-1.0.4/README.md
+drwxr-xr-x   0 seankulinski   (501) staff       (20)        0 2023-06-20 03:38:18.000000 sc2image-1.0.4/sc2image/
+-rw-r--r--   0 seankulinski   (501) staff       (20)      134 2023-06-16 19:23:27.000000 sc2image-1.0.4/sc2image/__init__.py
+-rw-r--r--   0 seankulinski   (501) staff       (20)    38212 2023-06-20 03:36:15.000000 sc2image-1.0.4/sc2image/dataset.py
+drwxr-xr-x   0 seankulinski   (501) staff       (20)        0 2023-06-20 03:38:18.000000 sc2image-1.0.4/sc2image/utils/
+-rw-r--r--   0 seankulinski   (501) staff       (20)        0 2023-06-16 17:35:39.000000 sc2image-1.0.4/sc2image/utils/__init__.py
+-rw-r--r--   0 seankulinski   (501) staff       (20)     2421 2023-06-16 18:21:35.000000 sc2image-1.0.4/sc2image/utils/metadata_processing.py
+-rw-r--r--   0 seankulinski   (501) staff       (20)     6002 2023-06-16 17:35:39.000000 sc2image-1.0.4/sc2image/utils/sensor_utils.py
+-rw-r--r--   0 seankulinski   (501) staff       (20)    24324 2023-06-16 17:35:39.000000 sc2image-1.0.4/sc2image/utils/unit_type_data.py
+-rw-r--r--   0 seankulinski   (501) staff       (20)      705 2023-06-20 03:37:51.000000 sc2image-1.0.4/sc2image/version.py
+drwxr-xr-x   0 seankulinski   (501) staff       (20)        0 2023-06-20 03:38:18.000000 sc2image-1.0.4/sc2image.egg-info/
+-rw-r--r--   0 seankulinski   (501) staff       (20)     4956 2023-06-20 03:38:18.000000 sc2image-1.0.4/sc2image.egg-info/PKG-INFO
+-rw-r--r--   0 seankulinski   (501) staff       (20)      375 2023-06-20 03:38:18.000000 sc2image-1.0.4/sc2image.egg-info/SOURCES.txt
+-rw-r--r--   0 seankulinski   (501) staff       (20)        1 2023-06-20 03:38:18.000000 sc2image-1.0.4/sc2image.egg-info/dependency_links.txt
+-rw-r--r--   0 seankulinski   (501) staff       (20)      115 2023-06-20 03:38:18.000000 sc2image-1.0.4/sc2image.egg-info/requires.txt
+-rw-r--r--   0 seankulinski   (501) staff       (20)        9 2023-06-20 03:38:18.000000 sc2image-1.0.4/sc2image.egg-info/top_level.txt
+-rw-r--r--   0 seankulinski   (501) staff       (20)       38 2023-06-20 03:38:18.000000 sc2image-1.0.4/setup.cfg
+-rw-r--r--   0 seankulinski   (501) staff       (20)     1184 2023-06-16 19:33:49.000000 sc2image-1.0.4/setup.py
```

### Comparing `sc2image-1.0.3/LICENSE` & `sc2image-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sc2image-1.0.3/PKG-INFO` & `sc2image-1.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: sc2image
-Version: 1.0.3
+Version: 1.0.4
 Summary: The StarCraft Image dataset
 Home-page: https://starcraftdata.davidinouye.com/
 Author: StarCraftImage team
 Author-email: dinouye@purdue.edu
 License: MIT
+Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -21,63 +22,86 @@
 
 --------------------------------------------------------------------------------
 
 [![PyPI](https://img.shields.io/pypi/v/sc2image)](https://pypi.org/project/sc2image/)
 [![License](https://img.shields.io/github/license/inouye-lab/starcraftimage)](https://github.com/inouye-lab/starcraftimage/blob/main/LICENSE)
 
 
-Welcome! This is the repository for the StarCraftImage dataset from the paper: [StarCraftImage: A Dataset For Prototyping Spatial Reasoning Methods For Multi-Agent Environments](https://openaccess.thecvf.com/content/CVPR2023/html/Kulinski_StarCraftImage_A_Dataset_for_Prototyping_Spatial_Reasoning_Methods_for_Multi-Agent_CVPR_2023_paper.html)
+Welcome! This is the repository for the StarCraftImage dataset from the paper: [StarCraftImage: A Dataset For Prototyping Spatial Reasoning Methods For Multi-Agent Environments](https://openaccess.thecvf.com/content/CVPR2023/html/Kulinski_StarCraftImage_A_Dataset_for_Prototyping_Spatial_Reasoning_Methods_for_Multi-Agent_CVPR_2023_paper.html).
+This README has basic installation and quickstart usage but our project webpage has more documentation: [StarCraftImage project webpage](https://starcraftdata.davidinouye.com/). 
+
+If you use this dataset, please cite the following paper:
+```
+@inproceedings{kulinski2023starcraftimage,
+  title={StarCraftImage: A Dataset for Prototyping Spatial Reasoning Methods for Multi-Agent Environments},
+  author={Kulinski, Sean and Waytowich, Nicholas R and Hare, James Z and Inouye, David I},
+  booktitle={Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition},
+  pages={22004--22013},
+  year={2023}
+}
+```
+
+## Installation
+
+We recommend using the `pip` package manager to install `sc2image`.
+
+```bash
+pip install sc2image
+```
+
+Note, this does not include the `dataset-demos` folder which contains jupyter notebooks which show example uses of the dataset.
+To use them, you should install from source via:
+    
+```bash
+git clone git@github.com:inouye-lab/starcraftimage.git
+cd starcraftimage
+pip install -e .
+```
 
 ## Quickstart
 
+:warning: **For more detailed documentation and example uses, visit the [dataset docs](https://starcraftdata.davidinouye.com/docs) for using `sc2image`.**
+
 There are three main StarCraftII datasets. 
 Each dataset includes images summarize a 10 second window (255 frames) of a StarCraftII replay.
 
 1. `StarCraftImage`: This is the main 3.6 million sample dataset which includes multiple image formats:`'sparse-hyperspectral'`, `'dense-hyperspectral'`, `'bag-of-units'`, `'bag-of-units-first'`, and contains all unit positioning information throughout the window.
 This dataset can be used via the following:
 
     ```py
     from sc2image.dataset import StarCraftImage
-    sc2image = StarCraftImage(root_dir=<your_download_path>, download=True)
+    sc2image = StarCraftImage(root="data", download=True)
     ```
 
-    This will download the StarCraftImage dataset to the `<your_download_path>` directory (if it does not already exist there).
+    This will download the StarCraftImage dataset to the `data` directory (if it does not already exist there).
 As this dataset has over 3.6 million samples, this might take a while to download. However, you can use the standalone StarCraftCIFAR10 and StarCraftMNIST versions below.
 
 
 2. `StarCraftCIFAR10`: This is a simplified version of the `StarCraftImage` dataset which exactly matches the setup of the CIFAR10 dataset.
 All images have been condensed into a three channel (RGB) image where the Red channel corresponds to Player 2 units, Green correspond to neutral units, and Blue to Player 1 units.
 The 10 classes equate to: `(map_name, did_window_happen_in_first_half_of_replay)`.
 The dataset can be loaded via:
         
     ```py    
     from sc2image.dataset import StarCraftCIFAR10
-    sc2image_cifar10 = StarCraftCIFAR10(root_dir=<your_download_path>, download=True)
+    sc2image_cifar10 = StarCraftCIFAR10(root="data", download=True)
     ```
 
  3. `StarCraftMNIST`: This is a further simplified version of the `StarCraftImage` dataset which exactly matches the setup of the MNIST dataset. 
  The grayscale images show to the seen last seen timestamps for units each pixel location, and the 10 classes match that of `StarCraftCIFAR10`.
  The dataset can be loaded via:
 
     ```py
     from sc2image.dataset import StarCraftMNIST
-    sc2image_mnist = StarCraftMNIST(root_dir=<your_download_path>, download=True)
+    sc2image_mnist = StarCraftMNIST(root="data", download=True)
     ```
     
 ## Example uses
 Please see the `starcraftimage-quickstart` jupyter notebook in the `dataset-demos` folder to see details on using this dataset!
 
-## Citation
-If you use this dataset, please cite the following paper:
-```
-@inproceedings{kulinski2023starcraftimage,
-  title={StarCraftImage: A Dataset for Prototyping Spatial Reasoning Methods for Multi-Agent Environments},
-  author={Kulinski, Sean and Waytowich, Nicholas R and Hare, James Z and Inouye, David I},
-  booktitle={Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition},
-  pages={22004--22013},
-  year={2023}
-}
-```
+## Bug reports
 
 If you run into any issues, please feel free to open an issue in this repository or email us via the corresponding author email in the [main paper](https://openaccess.thecvf.com/content/CVPR2023/html/Kulinski_StarCraftImage_A_Dataset_for_Prototyping_Spatial_Reasoning_Methods_for_Multi-Agent_CVPR_2023_paper.html).
 
 Cheers!
+
+
```

### Comparing `sc2image-1.0.3/README.md` & `sc2image-1.0.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -5,63 +5,84 @@
 
 --------------------------------------------------------------------------------
 
 [![PyPI](https://img.shields.io/pypi/v/sc2image)](https://pypi.org/project/sc2image/)
 [![License](https://img.shields.io/github/license/inouye-lab/starcraftimage)](https://github.com/inouye-lab/starcraftimage/blob/main/LICENSE)
 
 
-Welcome! This is the repository for the StarCraftImage dataset from the paper: [StarCraftImage: A Dataset For Prototyping Spatial Reasoning Methods For Multi-Agent Environments](https://openaccess.thecvf.com/content/CVPR2023/html/Kulinski_StarCraftImage_A_Dataset_for_Prototyping_Spatial_Reasoning_Methods_for_Multi-Agent_CVPR_2023_paper.html)
+Welcome! This is the repository for the StarCraftImage dataset from the paper: [StarCraftImage: A Dataset For Prototyping Spatial Reasoning Methods For Multi-Agent Environments](https://openaccess.thecvf.com/content/CVPR2023/html/Kulinski_StarCraftImage_A_Dataset_for_Prototyping_Spatial_Reasoning_Methods_for_Multi-Agent_CVPR_2023_paper.html).
+This README has basic installation and quickstart usage but our project webpage has more documentation: [StarCraftImage project webpage](https://starcraftdata.davidinouye.com/). 
+
+If you use this dataset, please cite the following paper:
+```
+@inproceedings{kulinski2023starcraftimage,
+  title={StarCraftImage: A Dataset for Prototyping Spatial Reasoning Methods for Multi-Agent Environments},
+  author={Kulinski, Sean and Waytowich, Nicholas R and Hare, James Z and Inouye, David I},
+  booktitle={Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition},
+  pages={22004--22013},
+  year={2023}
+}
+```
+
+## Installation
+
+We recommend using the `pip` package manager to install `sc2image`.
+
+```bash
+pip install sc2image
+```
+
+Note, this does not include the `dataset-demos` folder which contains jupyter notebooks which show example uses of the dataset.
+To use them, you should install from source via:
+    
+```bash
+git clone git@github.com:inouye-lab/starcraftimage.git
+cd starcraftimage
+pip install -e .
+```
 
 ## Quickstart
 
+:warning: **For more detailed documentation and example uses, visit the [dataset docs](https://starcraftdata.davidinouye.com/docs) for using `sc2image`.**
+
 There are three main StarCraftII datasets. 
 Each dataset includes images summarize a 10 second window (255 frames) of a StarCraftII replay.
 
 1. `StarCraftImage`: This is the main 3.6 million sample dataset which includes multiple image formats:`'sparse-hyperspectral'`, `'dense-hyperspectral'`, `'bag-of-units'`, `'bag-of-units-first'`, and contains all unit positioning information throughout the window.
 This dataset can be used via the following:
 
     ```py
     from sc2image.dataset import StarCraftImage
-    sc2image = StarCraftImage(root_dir=<your_download_path>, download=True)
+    sc2image = StarCraftImage(root="data", download=True)
     ```
 
-    This will download the StarCraftImage dataset to the `<your_download_path>` directory (if it does not already exist there).
+    This will download the StarCraftImage dataset to the `data` directory (if it does not already exist there).
 As this dataset has over 3.6 million samples, this might take a while to download. However, you can use the standalone StarCraftCIFAR10 and StarCraftMNIST versions below.
 
 
 2. `StarCraftCIFAR10`: This is a simplified version of the `StarCraftImage` dataset which exactly matches the setup of the CIFAR10 dataset.
 All images have been condensed into a three channel (RGB) image where the Red channel corresponds to Player 2 units, Green correspond to neutral units, and Blue to Player 1 units.
 The 10 classes equate to: `(map_name, did_window_happen_in_first_half_of_replay)`.
 The dataset can be loaded via:
         
     ```py    
     from sc2image.dataset import StarCraftCIFAR10
-    sc2image_cifar10 = StarCraftCIFAR10(root_dir=<your_download_path>, download=True)
+    sc2image_cifar10 = StarCraftCIFAR10(root="data", download=True)
     ```
 
  3. `StarCraftMNIST`: This is a further simplified version of the `StarCraftImage` dataset which exactly matches the setup of the MNIST dataset. 
  The grayscale images show to the seen last seen timestamps for units each pixel location, and the 10 classes match that of `StarCraftCIFAR10`.
  The dataset can be loaded via:
 
     ```py
     from sc2image.dataset import StarCraftMNIST
-    sc2image_mnist = StarCraftMNIST(root_dir=<your_download_path>, download=True)
+    sc2image_mnist = StarCraftMNIST(root="data", download=True)
     ```
     
 ## Example uses
 Please see the `starcraftimage-quickstart` jupyter notebook in the `dataset-demos` folder to see details on using this dataset!
 
-## Citation
-If you use this dataset, please cite the following paper:
-```
-@inproceedings{kulinski2023starcraftimage,
-  title={StarCraftImage: A Dataset for Prototyping Spatial Reasoning Methods for Multi-Agent Environments},
-  author={Kulinski, Sean and Waytowich, Nicholas R and Hare, James Z and Inouye, David I},
-  booktitle={Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition},
-  pages={22004--22013},
-  year={2023}
-}
-```
+## Bug reports
 
 If you run into any issues, please feel free to open an issue in this repository or email us via the corresponding author email in the [main paper](https://openaccess.thecvf.com/content/CVPR2023/html/Kulinski_StarCraftImage_A_Dataset_for_Prototyping_Spatial_Reasoning_Methods_for_Multi-Agent_CVPR_2023_paper.html).
 
-Cheers!
+Cheers!
```

### Comparing `sc2image-1.0.3/sc2image/dataset.py` & `sc2image-1.0.4/sc2image/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import collections
 from pathlib import Path
+import warnings
 
 import numpy as np
 import pandas as pd
 
 import torch
 import torchvision.transforms.functional
 from torchvision import io
@@ -73,33 +74,34 @@
     _versions_dict = {  # Note, this only includes major and minor versions
                 '1.0': {'download_url': 'https://figshare.com/ndownloader/files/40718405',
                         'md5': '23b691e7f520c3a7df7bfe0204a8fb90'}
             }
     dataset_name = 'starcraft-image-dataset'
     
     def __init__(self,
-                    root_dir,
+                    root=None,  # Path to the root directory of the ``starcraft-image-dataset``  
                     train=True,  # can be True, False, or 'all', where 'all' yields both train and test
                     image_format='dense-hyperspectral',  # other formats are 'sparse-hyperspectral', 'bag-of-units', 'bag-of-units-first'
                     image_size=64,  # The desired image size, which must be <= 64
                     label_kind=None,  # other options are '14-class' or '10-class'
                     return_label=False,  # if True, return the label as well as the image
                     return_dict=False,  # Append a dictionary of metadata to each sample
                     transform=None,  # An optional transform to be applied to the image (note, if bag-of-units, this must take in a tuple of (ids, values))
                     target_transform=None,  # An optional transform to be applied to the label (return_label must be True)
                     dict_transform=None,  # An optional transform to be applied to the dictionary (return_dict must be True)
                     use_metadata_cache=False,  # Use cached metadata to speed up loading
-                    download=False,  # Download the dataset if not found in root_dir
-                    verbose=True # Set to False to suppress non-essential print statements
+                    download=False,  # Download the dataset if not found in root
+                    verbose=True,  # Set to False to suppress non-essential print statements
+                    root_dir=None,  # Alias for ``root``. This is deprecated and `root` should be used.
                     ):
         """
         The main class for the StarCraftImage dataset.
 
         Args:
-            root_dir (str): Path to the root directory where the ``starcraft-image-dataset`` directory exists or will be
+            root (str): Path to the root directory where the ``starcraft-image-dataset`` directory exists or will be
                 saved to if download is set to True.
             train (bool): Whether to return the training or test set. If True, returns the training set. If False, 
                 returns the test set. If 'all', returns the entire dataset.
             image_format (str): The desired image format. Must be ``"dense-hyperspectral"``, ``"sparse-hyperspectral"``, 
                 ``"bag-of-units"``, or ``"bag-of-units-first"``.  
                 The ``dense-hyperspectral`` format returns a (384,``image_size``,``image_size``) dense tensor.
                 The ``sparse-hyperspectral`` format returns a (384,``image_size``,``image_size``) sparse tensor.
@@ -121,15 +123,16 @@
             dict_transform (callable, optional): A function/transform that takes in the metadata dictionary and
                 transforms it.
             return_dict (bool): If True, returns a dictionary of metadata as well as the image (and possibly label).
             use_metadata_cache: Loads the metadata from a cached file if it exists. If False, the metadata is
                 loaded using the metadata.csv file (which is slower)
             download (bool, optional): If true, downloads the dataset from the internet and
                 puts it in root directory. If dataset is already downloaded, it is not
-                downloaded again."""
+                downloaded again.
+            root_dir (str): Alias for ``root``. This is deprecated and `root` should be used."""
         # Validate input parameters
         if return_label:
             assert label_kind in ['10-class', '14-class'], """
             Must specify label_kind if return_label=True.
             Use label_kind="14-class" to set the labels to pertain to the 7 map types + Beginning/End of window.
             Or label_kind="10-class" to set the labels to pertain to 5 of the 7 map types + Beginning/End of window.
             Note: `label_kind="10-class" will drop any samples from the remaining 2 not included maps.
@@ -139,17 +142,26 @@
             assert label_kind is None, 'label_kind must be None if return_label=False'
 
         assert image_format in ['sparse-hyperspectral', 'dense-hyperspectral', 'bag-of-units', 'bag-of-units-first'], \
                     f'Invalid image_format: {image_format}'
         assert train in [True, False, 'all'], f'train must be True, False, or "all" but got {train}'
         if not return_label and target_transform is not None:
             print('\nWarning: target_transform will be ignored since return_label=False\n')
+
+        if root is None and root_dir is None:
+            raise ValueError('The `root` parameter must be specified. (`root_dir` may also be used, but is deprecated.)')
+        if root is not None and root_dir is not None:
+            raise ValueError('`root` and `root_dir` were both specified. Please only use `root`.')
+        if root is None and root_dir is not None:
+            warnings.warn('Use of `root_dir` has been deprecated and will raise an error in later versions. ' + \
+                     'Please use the `root` parameter instead.', DeprecationWarning, stacklevel=2)
+            root = root_dir
         
         self.verbose = verbose
-        self.data_dir = self._initialize_data_dir(root_dir, download)
+        self.data_dir = self._initialize_data_dir(root, download)
         self.image_format = image_format
         self.label_kind = label_kind
         self.transform, self.target_transform, self.dict_transform = transform, target_transform, dict_transform
         self.train = train
         self.data_split = 'train' if train==True else 'test' if train==False else 'all'
         self.return_dict = return_dict
         self.return_label = return_label
@@ -205,23 +217,23 @@
         md_cache_path = Path(self.data_dir) / 'cached-metadata.pkl'
         if md_cache_path.exists():
             md_cache_path.unlink()
             print('Deleted cached metadata at ', str(md_cache_path))
         else:
             print('No cached metadata found at ', str(md_cache_path))
 
-    def _initialize_data_dir(self, root_dir, download_flag):
+    def _initialize_data_dir(self, root, download_flag):
         """
         Initialize the data directory, downloading the dataset if necessary
         """
         latest_version = sorted(list(self._versions_dict.keys()))[-1]  # getting the latest version
 
-        root_dir = Path(root_dir)
-        root_dir.mkdir(exist_ok=True)
-        data_dir = root_dir / f'{self.dataset_name}_v{latest_version.replace(".", "_")}'
+        root = Path(root)
+        root.mkdir(exist_ok=True)
+        data_dir = root / f'{self.dataset_name}_v{latest_version.replace(".", "_")}'
         # see if the dataset already exists
         if data_dir.exists() and len(os.listdir(data_dir)) > 0:
             self._verbose_print('Dataset found in ', str(data_dir))
         else:
             # the dataset does not exist, download it if download_flag is set to true
             if not download_flag:
                 raise FileNotFoundError(
@@ -355,15 +367,17 @@
     def _build_map_state_dict(self, player_map_state, player_idx=1):
         if self.image_size != player_map_state.shape[1]:
             player_map_state = torchvision.transforms.functional.resize(player_map_state,
                                                                 [self.image_size, self.image_size]).type(torch.uint8)
         return {
             f'player_{player_idx}_is_visible': player_map_state[0] != 0,
             f'player_{player_idx}_is_seen': player_map_state[1] != 0,
-            f'player_{player_idx}_creep': player_map_state[2]
+            # check if there is a creep channel (i.e. if one of the players is a Zerg player)
+            f'player_{player_idx}_creep': player_map_state[2] if len(player_map_state) > 2 
+                        else torch.zeros(size=(self.image_size, self.image_size), dtype=torch.uint8),
         }
 
     def _get_window_png_path(self, idx):
         md_row = self.metadata.iloc[idx]
         png_basename = f'idx_{md_row["global_idx"]}__replay_{md_row["replay_name"]}__window_{md_row["window_idx"]}.png'
         png_filepath = os.path.join(self.data_dir, 'png_files', png_basename)
         return png_filepath
@@ -661,15 +675,15 @@
     when using use_sparse=False for StarCraftImage.
     This handles padding the dense tensors so they have the same shape
     in each batch.
 
     `sc_collate` is an alias for this function as well.
 
     Example:
-    >>> scdata = StarCraftImage(root_dir, use_sparse=False)
+    >>> scdata = StarCraftImage(root, use_sparse=False)
     >>> torch.utils.data.DataLoader(scdata, collate_fn=sc_collate, batch_size=32, shuffle=True)
     '''
     elem = batch[0]
     elem_type = type(elem)
     assert isinstance(elem, collections.abc.Mapping), 'Only works for dictionary-like objects'
     
     def pad_as_needed(A, n_target_channels):
```

### Comparing `sc2image-1.0.3/sc2image/utils/metadata_processing.py` & `sc2image-1.0.4/sc2image/utils/metadata_processing.py`

 * *Files identical despite different names*

### Comparing `sc2image-1.0.3/sc2image/utils/sensor_utils.py` & `sc2image-1.0.4/sc2image/utils/sensor_utils.py`

 * *Files identical despite different names*

### Comparing `sc2image-1.0.3/sc2image/utils/unit_type_data.py` & `sc2image-1.0.4/sc2image/utils/unit_type_data.py`

 * *Files identical despite different names*

### Comparing `sc2image-1.0.3/sc2image/version.py` & `sc2image-1.0.4/sc2image/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Adapted from https://github.com/p-lambda/wilds/blob/main/wilds/version.py
 
 import os
 import logging
 from threading import Thread
 
-__version__ = '1.0.3'
+__version__ = '1.0.4'
 
 try:
     os.environ['OUTDATED_IGNORE'] = '1'
     from outdated import check_outdated  # noqa
 except ImportError:
     check_outdated = None
```

### Comparing `sc2image-1.0.3/sc2image.egg-info/PKG-INFO` & `sc2image-1.0.4/sc2image.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: sc2image
-Version: 1.0.3
+Version: 1.0.4
 Summary: The StarCraft Image dataset
 Home-page: https://starcraftdata.davidinouye.com/
 Author: StarCraftImage team
 Author-email: dinouye@purdue.edu
 License: MIT
+Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -21,63 +22,86 @@
 
 --------------------------------------------------------------------------------
 
 [![PyPI](https://img.shields.io/pypi/v/sc2image)](https://pypi.org/project/sc2image/)
 [![License](https://img.shields.io/github/license/inouye-lab/starcraftimage)](https://github.com/inouye-lab/starcraftimage/blob/main/LICENSE)
 
 
-Welcome! This is the repository for the StarCraftImage dataset from the paper: [StarCraftImage: A Dataset For Prototyping Spatial Reasoning Methods For Multi-Agent Environments](https://openaccess.thecvf.com/content/CVPR2023/html/Kulinski_StarCraftImage_A_Dataset_for_Prototyping_Spatial_Reasoning_Methods_for_Multi-Agent_CVPR_2023_paper.html)
+Welcome! This is the repository for the StarCraftImage dataset from the paper: [StarCraftImage: A Dataset For Prototyping Spatial Reasoning Methods For Multi-Agent Environments](https://openaccess.thecvf.com/content/CVPR2023/html/Kulinski_StarCraftImage_A_Dataset_for_Prototyping_Spatial_Reasoning_Methods_for_Multi-Agent_CVPR_2023_paper.html).
+This README has basic installation and quickstart usage but our project webpage has more documentation: [StarCraftImage project webpage](https://starcraftdata.davidinouye.com/). 
+
+If you use this dataset, please cite the following paper:
+```
+@inproceedings{kulinski2023starcraftimage,
+  title={StarCraftImage: A Dataset for Prototyping Spatial Reasoning Methods for Multi-Agent Environments},
+  author={Kulinski, Sean and Waytowich, Nicholas R and Hare, James Z and Inouye, David I},
+  booktitle={Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition},
+  pages={22004--22013},
+  year={2023}
+}
+```
+
+## Installation
+
+We recommend using the `pip` package manager to install `sc2image`.
+
+```bash
+pip install sc2image
+```
+
+Note, this does not include the `dataset-demos` folder which contains jupyter notebooks which show example uses of the dataset.
+To use them, you should install from source via:
+    
+```bash
+git clone git@github.com:inouye-lab/starcraftimage.git
+cd starcraftimage
+pip install -e .
+```
 
 ## Quickstart
 
+:warning: **For more detailed documentation and example uses, visit the [dataset docs](https://starcraftdata.davidinouye.com/docs) for using `sc2image`.**
+
 There are three main StarCraftII datasets. 
 Each dataset includes images summarize a 10 second window (255 frames) of a StarCraftII replay.
 
 1. `StarCraftImage`: This is the main 3.6 million sample dataset which includes multiple image formats:`'sparse-hyperspectral'`, `'dense-hyperspectral'`, `'bag-of-units'`, `'bag-of-units-first'`, and contains all unit positioning information throughout the window.
 This dataset can be used via the following:
 
     ```py
     from sc2image.dataset import StarCraftImage
-    sc2image = StarCraftImage(root_dir=<your_download_path>, download=True)
+    sc2image = StarCraftImage(root="data", download=True)
     ```
 
-    This will download the StarCraftImage dataset to the `<your_download_path>` directory (if it does not already exist there).
+    This will download the StarCraftImage dataset to the `data` directory (if it does not already exist there).
 As this dataset has over 3.6 million samples, this might take a while to download. However, you can use the standalone StarCraftCIFAR10 and StarCraftMNIST versions below.
 
 
 2. `StarCraftCIFAR10`: This is a simplified version of the `StarCraftImage` dataset which exactly matches the setup of the CIFAR10 dataset.
 All images have been condensed into a three channel (RGB) image where the Red channel corresponds to Player 2 units, Green correspond to neutral units, and Blue to Player 1 units.
 The 10 classes equate to: `(map_name, did_window_happen_in_first_half_of_replay)`.
 The dataset can be loaded via:
         
     ```py    
     from sc2image.dataset import StarCraftCIFAR10
-    sc2image_cifar10 = StarCraftCIFAR10(root_dir=<your_download_path>, download=True)
+    sc2image_cifar10 = StarCraftCIFAR10(root="data", download=True)
     ```
 
  3. `StarCraftMNIST`: This is a further simplified version of the `StarCraftImage` dataset which exactly matches the setup of the MNIST dataset. 
  The grayscale images show to the seen last seen timestamps for units each pixel location, and the 10 classes match that of `StarCraftCIFAR10`.
  The dataset can be loaded via:
 
     ```py
     from sc2image.dataset import StarCraftMNIST
-    sc2image_mnist = StarCraftMNIST(root_dir=<your_download_path>, download=True)
+    sc2image_mnist = StarCraftMNIST(root="data", download=True)
     ```
     
 ## Example uses
 Please see the `starcraftimage-quickstart` jupyter notebook in the `dataset-demos` folder to see details on using this dataset!
 
-## Citation
-If you use this dataset, please cite the following paper:
-```
-@inproceedings{kulinski2023starcraftimage,
-  title={StarCraftImage: A Dataset for Prototyping Spatial Reasoning Methods for Multi-Agent Environments},
-  author={Kulinski, Sean and Waytowich, Nicholas R and Hare, James Z and Inouye, David I},
-  booktitle={Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition},
-  pages={22004--22013},
-  year={2023}
-}
-```
+## Bug reports
 
 If you run into any issues, please feel free to open an issue in this repository or email us via the corresponding author email in the [main paper](https://openaccess.thecvf.com/content/CVPR2023/html/Kulinski_StarCraftImage_A_Dataset_for_Prototyping_Spatial_Reasoning_Methods_for_Multi-Agent_CVPR_2023_paper.html).
 
 Cheers!
+
+
```

### Comparing `sc2image-1.0.3/setup.py` & `sc2image-1.0.4/setup.py`

 * *Files identical despite different names*

