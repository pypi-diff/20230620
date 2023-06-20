# Comparing `tmp/vision_datasets-0.2.8.tar.gz` & `tmp/vision_datasets-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vision_datasets-0.2.8.tar", last modified: Tue Mar 22 05:50:50 2022, max compression
+gzip compressed data, was "dist\vision_datasets-0.2.9.tar", last modified: Thu Mar 24 17:18:07 2022, max compression
```

## Comparing `vision_datasets-0.2.8.tar` & `vision_datasets-0.2.9.tar`

### file list

```diff
@@ -1,58 +1,60 @@
-drwxrwxrwx   0        0        0        0 2022-03-22 05:50:50.871313 vision_datasets-0.2.8/
--rw-rw-rw-   0        0        0     1340 2022-03-21 19:17:51.000000 vision_datasets-0.2.8/.gitignore
--rw-rw-rw-   0        0        0     3556 2022-03-01 00:28:36.000000 vision_datasets-0.2.8/COCO_DATA_FORMAT.md
--rw-rw-rw-   0        0        0      453 2021-08-24 03:38:08.000000 vision_datasets-0.2.8/CODE_OF_CONDUCT.md
--rw-rw-rw-   0        0        0     3908 2022-03-01 00:28:36.000000 vision_datasets-0.2.8/IRIS_DATA_FORMAT.md
--rw-rw-rw-   0        0        0     1162 2021-08-24 03:38:08.000000 vision_datasets-0.2.8/LICENSE
--rw-rw-rw-   0        0        0     8784 2022-03-22 05:50:50.870312 vision_datasets-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     8023 2022-03-01 00:28:59.000000 vision_datasets-0.2.8/README.md
--rw-rw-rw-   0        0        0       42 2022-03-22 05:50:50.872312 vision_datasets-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0     2814 2022-03-22 05:48:39.000000 vision_datasets-0.2.8/setup.py
-drwxrwxrwx   0        0        0        0 2022-03-22 05:50:50.796312 vision_datasets-0.2.8/tests/
--rw-rw-rw-   0        0        0     2089 2022-02-02 18:03:44.000000 vision_datasets-0.2.8/tests/test_box_alteration.py
--rw-rw-rw-   0        0        0     4468 2021-09-23 23:11:41.000000 vision_datasets-0.2.8/tests/test_dataset_downloader.py
--rw-rw-rw-   0        0        0    50883 2022-03-01 00:28:36.000000 vision_datasets-0.2.8/tests/test_dataset_manifest.py
--rw-rw-rw-   0        0        0     2111 2022-01-19 20:58:58.000000 vision_datasets-0.2.8/tests/test_dataset_registry.py
--rw-rw-rw-   0        0        0     3436 2022-01-06 00:32:28.000000 vision_datasets-0.2.8/tests/test_file_reader.py
--rw-rw-rw-   0        0        0     2926 2022-03-21 19:13:37.000000 vision_datasets-0.2.8/tests/test_manifest_dataset.py
--rw-rw-rw-   0        0        0     1398 2022-02-03 18:13:09.000000 vision_datasets-0.2.8/tests/test_pytorch_dataset.py
--rw-rw-rw-   0        0        0       99 2022-03-21 19:13:25.000000 vision_datasets-0.2.8/tox.ini
-drwxrwxrwx   0        0        0        0 2022-03-22 05:50:50.800315 vision_datasets-0.2.8/vision_datasets/
--rw-rw-rw-   0        0        0      449 2021-09-23 23:11:41.000000 vision_datasets-0.2.8/vision_datasets/__init__.py
-drwxrwxrwx   0        0        0        0 2022-03-22 05:50:50.839313 vision_datasets-0.2.8/vision_datasets/commands/
--rw-rw-rw-   0        0        0        0 2021-09-23 23:11:41.000000 vision_datasets-0.2.8/vision_datasets/commands/__init__.py
--rw-rw-rw-   0        0        0     3216 2022-01-06 00:32:28.000000 vision_datasets-0.2.8/vision_datasets/commands/convert_local_dir_ic_data.py
--rw-rw-rw-   0        0        0     3879 2022-03-21 19:13:46.000000 vision_datasets-0.2.8/vision_datasets/commands/converter_od_to_ic.py
--rw-rw-rw-   0        0        0     5704 2022-01-24 22:44:25.000000 vision_datasets-0.2.8/vision_datasets/commands/converter_tsv_to_coco.py
--rw-rw-rw-   0        0        0     5255 2022-01-24 22:44:25.000000 vision_datasets-0.2.8/vision_datasets/commands/converter_tsv_to_iris.py
--rw-rw-rw-   0        0        0     4854 2021-09-23 23:11:41.000000 vision_datasets-0.2.8/vision_datasets/commands/converter_yolo_darknet_to_cvs.py
--rw-rw-rw-   0        0        0     4101 2022-03-16 15:47:13.000000 vision_datasets-0.2.8/vision_datasets/commands/dataset_check.py
--rw-rw-rw-   0        0        0     3755 2021-09-23 23:11:41.000000 vision_datasets-0.2.8/vision_datasets/commands/download.py
--rw-rw-rw-   0        0        0     1075 2021-09-23 23:11:41.000000 vision_datasets-0.2.8/vision_datasets/commands/generate_image_meta_info.py
--rw-rw-rw-   0        0        0     3269 2022-03-01 00:28:36.000000 vision_datasets-0.2.8/vision_datasets/commands/merge_datasets.py
--rw-rw-rw-   0        0        0     2517 2022-01-24 22:44:25.000000 vision_datasets-0.2.8/vision_datasets/commands/utils.py
-drwxrwxrwx   0        0        0        0 2022-03-22 05:50:50.858311 vision_datasets-0.2.8/vision_datasets/common/
--rw-rw-rw-   0        0        0      504 2021-09-23 23:11:41.000000 vision_datasets-0.2.8/vision_datasets/common/__init__.py
--rw-rw-rw-   0        0        0     1090 2022-02-02 18:03:44.000000 vision_datasets-0.2.8/vision_datasets/common/base_dataset.py
--rw-rw-rw-   0        0        0      904 2022-03-10 19:12:27.000000 vision_datasets-0.2.8/vision_datasets/common/constants.py
--rw-rw-rw-   0        0        0    32933 2022-03-22 05:27:45.000000 vision_datasets-0.2.8/vision_datasets/common/data_manifest.py
--rw-rw-rw-   0        0        0     4562 2022-03-01 00:28:36.000000 vision_datasets-0.2.8/vision_datasets/common/dataset_downloader.py
--rw-rw-rw-   0        0        0     4637 2022-03-21 18:27:58.000000 vision_datasets-0.2.8/vision_datasets/common/dataset_info.py
--rw-rw-rw-   0        0        0     1690 2022-01-19 20:59:43.000000 vision_datasets-0.2.8/vision_datasets/common/dataset_registry.py
--rw-rw-rw-   0        0        0     1412 2021-09-23 23:11:41.000000 vision_datasets-0.2.8/vision_datasets/common/image_loader.py
--rw-rw-rw-   0        0        0    14391 2022-03-21 18:29:15.000000 vision_datasets-0.2.8/vision_datasets/common/manifest_dataset.py
--rw-rw-rw-   0        0        0     2162 2022-01-06 00:32:28.000000 vision_datasets-0.2.8/vision_datasets/common/util.py
-drwxrwxrwx   0        0        0        0 2022-03-22 05:50:50.866314 vision_datasets-0.2.8/vision_datasets/pytorch/
--rw-rw-rw-   0        0        0       71 2021-09-23 23:11:41.000000 vision_datasets-0.2.8/vision_datasets/pytorch/__init__.py
--rw-rw-rw-   0        0        0     1290 2022-02-03 18:13:09.000000 vision_datasets-0.2.8/vision_datasets/pytorch/dataset.py
--rw-rw-rw-   0        0        0     1057 2022-02-03 18:13:09.000000 vision_datasets-0.2.8/vision_datasets/pytorch/torch_dataset.py
-drwxrwxrwx   0        0        0        0 2022-03-22 05:50:50.869313 vision_datasets-0.2.8/vision_datasets/resources/
--rw-rw-rw-   0        0        0       65 2021-09-23 23:11:41.000000 vision_datasets-0.2.8/vision_datasets/resources/__init__.py
--rw-rw-rw-   0        0        0     7133 2022-03-16 15:47:13.000000 vision_datasets-0.2.8/vision_datasets/resources/dataset_hub.py
-drwxrwxrwx   0        0        0        0 2022-03-22 05:50:50.816316 vision_datasets-0.2.8/vision_datasets.egg-info/
--rw-rw-rw-   0        0        0     8784 2022-03-22 05:50:50.000000 vision_datasets-0.2.8/vision_datasets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1665 2022-03-22 05:50:50.000000 vision_datasets-0.2.8/vision_datasets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-03-22 05:50:50.000000 vision_datasets-0.2.8/vision_datasets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      676 2022-03-22 05:50:50.000000 vision_datasets-0.2.8/vision_datasets.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      105 2022-03-22 05:50:50.000000 vision_datasets-0.2.8/vision_datasets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2022-03-22 05:50:50.000000 vision_datasets-0.2.8/vision_datasets.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-03-24 17:18:07.000000 vision_datasets-0.2.9/
+-rw-rw-rw-   0        0        0     1340 2022-03-24 17:18:01.000000 vision_datasets-0.2.9/.gitignore
+-rw-rw-rw-   0        0        0     3556 2022-03-24 17:18:01.000000 vision_datasets-0.2.9/COCO_DATA_FORMAT.md
+-rw-rw-rw-   0        0        0      453 2022-01-06 01:01:48.000000 vision_datasets-0.2.9/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0        0        0     3908 2022-03-24 17:18:01.000000 vision_datasets-0.2.9/IRIS_DATA_FORMAT.md
+-rw-rw-rw-   0        0        0     1162 2022-01-06 01:01:48.000000 vision_datasets-0.2.9/LICENSE
+-rw-rw-rw-   0        0        0     9882 2022-03-24 17:18:07.000000 vision_datasets-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     8023 2022-03-24 17:18:01.000000 vision_datasets-0.2.9/README.md
+-rw-rw-rw-   0        0        0       42 2022-03-24 17:18:07.000000 vision_datasets-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     2814 2022-03-24 17:18:01.000000 vision_datasets-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2022-03-24 17:18:07.000000 vision_datasets-0.2.9/tests/
+-rw-rw-rw-   0        0        0     2089 2022-02-03 08:25:43.000000 vision_datasets-0.2.9/tests/test_box_alteration.py
+-rw-rw-rw-   0        0        0     4468 2022-01-06 01:01:48.000000 vision_datasets-0.2.9/tests/test_dataset_downloader.py
+-rw-rw-rw-   0        0        0    50883 2022-03-24 17:18:01.000000 vision_datasets-0.2.9/tests/test_dataset_manifest.py
+-rw-rw-rw-   0        0        0     2111 2022-01-20 20:09:50.000000 vision_datasets-0.2.9/tests/test_dataset_registry.py
+-rw-rw-rw-   0        0        0     4151 2022-03-24 17:18:01.000000 vision_datasets-0.2.9/tests/test_detection_as_classification.py
+-rw-rw-rw-   0        0        0     3436 2022-01-06 01:01:48.000000 vision_datasets-0.2.9/tests/test_file_reader.py
+-rw-rw-rw-   0        0        0     2271 2022-03-24 17:18:01.000000 vision_datasets-0.2.9/tests/test_fixtures.py
+-rw-rw-rw-   0        0        0     2926 2022-03-24 17:18:01.000000 vision_datasets-0.2.9/tests/test_manifest_dataset.py
+-rw-rw-rw-   0        0        0     1398 2022-02-03 08:25:43.000000 vision_datasets-0.2.9/tests/test_pytorch_dataset.py
+-rw-rw-rw-   0        0        0       99 2022-03-24 17:18:01.000000 vision_datasets-0.2.9/tox.ini
+drwxrwxrwx   0        0        0        0 2022-03-24 17:18:07.000000 vision_datasets-0.2.9/vision_datasets/
+-rw-rw-rw-   0        0        0      449 2022-01-06 01:01:48.000000 vision_datasets-0.2.9/vision_datasets/__init__.py
+drwxrwxrwx   0        0        0        0 2022-03-24 17:18:07.000000 vision_datasets-0.2.9/vision_datasets/commands/
+-rw-rw-rw-   0        0        0        0 2022-01-06 01:01:48.000000 vision_datasets-0.2.9/vision_datasets/commands/__init__.py
+-rw-rw-rw-   0        0        0     3216 2022-01-06 01:01:48.000000 vision_datasets-0.2.9/vision_datasets/commands/convert_local_dir_ic_data.py
+-rw-rw-rw-   0        0        0     3879 2022-03-24 17:18:01.000000 vision_datasets-0.2.9/vision_datasets/commands/converter_od_to_ic.py
+-rw-rw-rw-   0        0        0     5704 2022-02-03 08:25:43.000000 vision_datasets-0.2.9/vision_datasets/commands/converter_tsv_to_coco.py
+-rw-rw-rw-   0        0        0     5255 2022-02-03 08:25:43.000000 vision_datasets-0.2.9/vision_datasets/commands/converter_tsv_to_iris.py
+-rw-rw-rw-   0        0        0     4854 2022-01-06 01:01:48.000000 vision_datasets-0.2.9/vision_datasets/commands/converter_yolo_darknet_to_cvs.py
+-rw-rw-rw-   0        0        0     4101 2022-03-24 17:18:01.000000 vision_datasets-0.2.9/vision_datasets/commands/dataset_check.py
+-rw-rw-rw-   0        0        0     3755 2022-01-06 01:01:48.000000 vision_datasets-0.2.9/vision_datasets/commands/download.py
+-rw-rw-rw-   0        0        0     1075 2022-01-06 01:01:48.000000 vision_datasets-0.2.9/vision_datasets/commands/generate_image_meta_info.py
+-rw-rw-rw-   0        0        0     3269 2022-03-24 17:18:01.000000 vision_datasets-0.2.9/vision_datasets/commands/merge_datasets.py
+-rw-rw-rw-   0        0        0     2517 2022-02-03 08:25:43.000000 vision_datasets-0.2.9/vision_datasets/commands/utils.py
+drwxrwxrwx   0        0        0        0 2022-03-24 17:18:07.000000 vision_datasets-0.2.9/vision_datasets/common/
+-rw-rw-rw-   0        0        0      504 2022-01-06 01:01:48.000000 vision_datasets-0.2.9/vision_datasets/common/__init__.py
+-rw-rw-rw-   0        0        0     1090 2022-02-03 08:25:43.000000 vision_datasets-0.2.9/vision_datasets/common/base_dataset.py
+-rw-rw-rw-   0        0        0      904 2022-03-24 17:18:01.000000 vision_datasets-0.2.9/vision_datasets/common/constants.py
+-rw-rw-rw-   0        0        0    32933 2022-03-24 17:18:01.000000 vision_datasets-0.2.9/vision_datasets/common/data_manifest.py
+-rw-rw-rw-   0        0        0     4562 2022-03-24 17:18:01.000000 vision_datasets-0.2.9/vision_datasets/common/dataset_downloader.py
+-rw-rw-rw-   0        0        0     4637 2022-03-24 17:18:01.000000 vision_datasets-0.2.9/vision_datasets/common/dataset_info.py
+-rw-rw-rw-   0        0        0     1690 2022-01-20 20:09:50.000000 vision_datasets-0.2.9/vision_datasets/common/dataset_registry.py
+-rw-rw-rw-   0        0        0     1412 2022-01-06 01:01:48.000000 vision_datasets-0.2.9/vision_datasets/common/image_loader.py
+-rw-rw-rw-   0        0        0    14368 2022-03-24 17:18:01.000000 vision_datasets-0.2.9/vision_datasets/common/manifest_dataset.py
+-rw-rw-rw-   0        0        0     2162 2022-01-06 01:01:48.000000 vision_datasets-0.2.9/vision_datasets/common/util.py
+drwxrwxrwx   0        0        0        0 2022-03-24 17:18:07.000000 vision_datasets-0.2.9/vision_datasets/pytorch/
+-rw-rw-rw-   0        0        0       71 2022-01-06 01:01:48.000000 vision_datasets-0.2.9/vision_datasets/pytorch/__init__.py
+-rw-rw-rw-   0        0        0     1290 2022-02-03 08:25:43.000000 vision_datasets-0.2.9/vision_datasets/pytorch/dataset.py
+-rw-rw-rw-   0        0        0     1057 2022-02-03 08:25:43.000000 vision_datasets-0.2.9/vision_datasets/pytorch/torch_dataset.py
+drwxrwxrwx   0        0        0        0 2022-03-24 17:18:07.000000 vision_datasets-0.2.9/vision_datasets/resources/
+-rw-rw-rw-   0        0        0       65 2022-01-06 01:01:48.000000 vision_datasets-0.2.9/vision_datasets/resources/__init__.py
+-rw-rw-rw-   0        0        0     7133 2022-03-24 17:18:01.000000 vision_datasets-0.2.9/vision_datasets/resources/dataset_hub.py
+drwxrwxrwx   0        0        0        0 2022-03-24 17:18:07.000000 vision_datasets-0.2.9/vision_datasets.egg-info/
+-rw-rw-rw-   0        0        0     9882 2022-03-24 17:18:06.000000 vision_datasets-0.2.9/vision_datasets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1730 2022-03-24 17:18:07.000000 vision_datasets-0.2.9/vision_datasets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-03-24 17:18:06.000000 vision_datasets-0.2.9/vision_datasets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      676 2022-03-24 17:18:06.000000 vision_datasets-0.2.9/vision_datasets.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      105 2022-03-24 17:18:06.000000 vision_datasets-0.2.9/vision_datasets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2022-03-24 17:18:06.000000 vision_datasets-0.2.9/vision_datasets.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `vision_datasets-0.2.8/.gitignore` & `vision_datasets-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `vision_datasets-0.2.8/COCO_DATA_FORMAT.md` & `vision_datasets-0.2.9/COCO_DATA_FORMAT.md`

 * *Files identical despite different names*

### Comparing `vision_datasets-0.2.8/IRIS_DATA_FORMAT.md` & `vision_datasets-0.2.9/IRIS_DATA_FORMAT.md`

 * *Files identical despite different names*

### Comparing `vision_datasets-0.2.8/LICENSE` & `vision_datasets-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `vision_datasets-0.2.8/PKG-INFO` & `vision_datasets-0.2.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,162 +1,159 @@
 Metadata-Version: 2.1
 Name: vision_datasets
-Version: 0.2.8
+Version: 0.2.9
 Summary: A utility repo for vision dataset access and management.
 Home-page: https://github.com/microsoft/vision-datasets
 Author: Ping Jin, Shohei Ono
 License: MIT
+Description: # Vision Datasets
+        
+        ## Introduction
+        
+        This repo
+        
+        - defines unified contract for dataset for purposes such as training, visualization, and exploration, via `DatasetManifest` and `ImageDataManifest`.
+        - provides API for organizing and accessing datasets, via `DatasetHub`
+        
+        Currently, five `basic` types of data are supported: 
+        - `classification_multiclass`: each image can is only with one label.
+        - `classification_multilabel`: each image can is with one or multiple labels (e.g., 'cat', 'animal', 'pet').
+        - `object_detection`: each image is labeled with bounding boxes surrounding the objects of interest.
+        - `image_caption`: each image is labeled with a few texts describing the images.
+        - `image_text_matching`: each image is associated with a collection of texts describing the image, and whether each text description matches the image or not
+        
+        `multitask` type is a composition type, where one set of images has multiple sets of annotations available for different tasks, where each task can be of any basic type.
+        
+        
+        ## Dataset Contracts
+        
+        - `DatasetManifest` wraps the information about a dataset including labelmap, images (width, height, path to image), and annotations. `ImageDataManifest` encapsulates information about each image.
+        - `ImageDataManifest` encapsulates image-specific information, such as image id, path, labels, and width/height. One thing to note here is that the image path can be
+            1. a local path (absolute `c:\images\1.jpg` or relative `images\1.jpg`)
+            2. a local path in a **non-compressed** zip file (absolute `c:\images.zip@1.jpg` or relative `images.zip@1.jpg`) or
+            3. an url
+        - `ManifestDataset` is an iterable dataset class that consumes the information from `DatasetManifest`.
+        
+        `ManifestDataset` is able to load the data from all three kinds of paths. Both 1. and 2. are good for training, as they access data from local disk while the 3rd one is good for data exploration, if you have the data in azure storage.
+        
+        For `multitask` dataset, the labels stored in the `ImageDataManifest` is a `dict` mapping from task name to that task's labels. The labelmap stored in `DatasetManifest` is also a `dict` mapping from task name to that task's labels.
+        
+        ### Creating DatasetManifest
+        
+        In addition to loading a serialized `DatasetManifest` for instantiation, this repo currently supports two formats of data that can instantiates `DatasetManifest`,
+        using `DatasetManifest.create_dataset_manifest(dataset_info, usage, container_sas_or_root_dir)`: `COCO` and `IRIS` (legacy).
+        
+        `DatasetInfo` as the first arg in the arg list wraps the metainfo about the dataset like the name of the dataset, locations of the images, annotation files, etc. See examples in the sections below
+        for different data formats.
+        
+        Once a `DatasetManifest` is created, you can create a `ManifestDataset` for accessing the data in the dataset, especially the image data, for training, visualization, etc:
+        
+        ```{python}
+        dataset = ManifestDataset(dataset_info, dataset_manifest, coordinates='relative')
+        ```
+        
+        #### Coco format
+        
+        Here is an example with explanation of what a `DatasetInfo` looks like for coco format, when it is serialized into json:
+        
+        ```{json}
+            {
+                "name": "sampled-ms-coco",
+                "version": 1,
+                "description": "A sampled ms-coco dataset.",
+                "type": "object_detection",
+                "format": "coco", // indicating the annotation data are stored in coco format
+                "root_folder": "detection/coco2017_20200401", // a root folder for all files listed
+                "train": {
+                    "index_path": "train.json", // coco json file for training, see next section for example
+                    "files_for_local_usage": [ // associated files including data such as images
+                        "images/train_images.zip"
+                    ]
+                },
+                "val": {
+                    "index_path": "val.json",
+                    "files_for_local_usage": [
+                        "images/val_images.zip"
+                    ]
+                },
+                "test": {
+                    "index_path": "test.json",
+                    "files_for_local_usage": [
+                        "images/test_images.zip"
+                    ]
+                }
+            }
+        ```
+        
+        Coco annotation format details w.r.t. `multiclass/label_classification`, `object_detection`, `image_caption`, `image_text_match` and `multitask`  can be found in `COCO_DATA_FORMAT.md`.
+        
+        
+        #### Iris format
+        
+        Iris format is a legacy format which can be found in `IRIS_DATA_FORMAT.md`. Only `multiclass/label_classification`, `object_detection` and `multitask` are supported.
+        
+        ## Dataset management and access
+        
+        Once you have multiple datasets, it is more convenient to have all the `DatasetInfo` in one place and instantiate `DatasetManifest` or even `ManifestDataset` by just using the dataset name, usage (
+        train, val ,test) and version.
+        
+        This repo offers the class `DatasetHub` for this purpose. Once instantiated with a json including the `DatasetInfo` for all datasets, you can retrieve a `ManifestDataset` by
+        
+        ```{python}
+        import pathlib
+        
+        dataset_infos_json_path = 'datasets.json'
+        dataset_hub = DatasetHub(pathlib.Path(dataset_infos_json_path).read_text())
+        stanford_cars = dataset_hub.create_manifest_dataset(blob_container_sas, local_dir, 'stanford-cars', version=1, usage='train')
+        
+        # note that you can pass multiple datasets.json to DatasetHub, it can combine them all
+        # example: DatasetHub([ds_json1, ds_json2, ...])
+        # note that you can specify multiple usages in create_manifest_dataset call
+        # example dataset_hub.create_manifest_dataset(blob_container_sas, local_dir, 'stanford-cars', version=1, usage=['train', 'val'])
+        
+        for img, targets, sample_idx_str in stanford_cars:
+            img.show()
+            img.close()
+            print(targets)
+        ```
+        
+        Note that this hub class works with data saved in both Azure Blob container and on local disk.
+        
+        If `local_dir`:
+        
+        1. is provided, the hub will look for the resources locally and **download the data** (files included in "
+           files_for_local_usage", the index files, metadata (if iris format), labelmap (if iris format))
+           from `blob_container_sas` if not present locally
+        2. is NOT provided (i.e. `None`), the hub will create a manifest dataset that directly consumes data from the blob
+           indicated by `blob_container_sas`. Note that this does not work, if data are stored in zipped files. You will have to
+           unzip your data in the azure blob. (Index files requires no update, if image paths are for zip files: "a.zip@1.jpg").
+           This kind of azure-based dataset is good for large dataset exploration, but can be slow for training.
+        
+        When data exists on local disk, `blob_container_sas` can be `None`.
+        
+        ### Training with PyTorch
+        
+        Training with PyTorch is easy. After instantiating a `ManifestDataset`, simply passing it in `vision_datasets.pytorch.torch_dataset.TorchDataset` together with the `transform`, then you are good to go with the PyTorch DataLoader for training.
+        
+        ### Managing datasets with DatasetHub on cloud storage
+        
+        If you are using `DatasetHub` to manage datasets in cloud storage, we recommend zipping (with uncompressed mode) the images into one or multiple zip files before uploading it and update the file path in index files to be like `train.zip@1.jpg` from `train\1.jpg`. You can do it with `7zip` (set compression level to 'store') on Windows or [zip](https://superuser.com/questions/411394/zip-files-without-compression) command on Linux.
+        
+        If you upload folders of images directly to cloud storage:
+        
+        - you will need to list all images in `"files_for_local_usage"`, which can be millions of entries
+        - downloading images one by one (even with multithreading) is much slower than downloading a few zip files
+        
+        One more thing is that sometimes when you create a zip file `train.zip`, you might find out that there is only one `train` folder in the zip. This will fail the file loading if the path is `train.zip@1.jpg`, as the image is actually at `train.zip@train\1.jpg`. It is ok to have this extra layer but please make sure the path is correct.
+        
 Keywords: vision datasets classification detection
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: run
-License-File: LICENSE
-
-# Vision Datasets
-
-## Introduction
-
-This repo
-
-- defines unified contract for dataset for purposes such as training, visualization, and exploration, via `DatasetManifest` and `ImageDataManifest`.
-- provides API for organizing and accessing datasets, via `DatasetHub`
-
-Currently, five `basic` types of data are supported: 
-- `classification_multiclass`: each image can is only with one label.
-- `classification_multilabel`: each image can is with one or multiple labels (e.g., 'cat', 'animal', 'pet').
-- `object_detection`: each image is labeled with bounding boxes surrounding the objects of interest.
-- `image_caption`: each image is labeled with a few texts describing the images.
-- `image_text_matching`: each image is associated with a collection of texts describing the image, and whether each text description matches the image or not
-
-`multitask` type is a composition type, where one set of images has multiple sets of annotations available for different tasks, where each task can be of any basic type.
-
-
-## Dataset Contracts
-
-- `DatasetManifest` wraps the information about a dataset including labelmap, images (width, height, path to image), and annotations. `ImageDataManifest` encapsulates information about each image.
-- `ImageDataManifest` encapsulates image-specific information, such as image id, path, labels, and width/height. One thing to note here is that the image path can be
-    1. a local path (absolute `c:\images\1.jpg` or relative `images\1.jpg`)
-    2. a local path in a **non-compressed** zip file (absolute `c:\images.zip@1.jpg` or relative `images.zip@1.jpg`) or
-    3. an url
-- `ManifestDataset` is an iterable dataset class that consumes the information from `DatasetManifest`.
-
-`ManifestDataset` is able to load the data from all three kinds of paths. Both 1. and 2. are good for training, as they access data from local disk while the 3rd one is good for data exploration, if you have the data in azure storage.
-
-For `multitask` dataset, the labels stored in the `ImageDataManifest` is a `dict` mapping from task name to that task's labels. The labelmap stored in `DatasetManifest` is also a `dict` mapping from task name to that task's labels.
-
-### Creating DatasetManifest
-
-In addition to loading a serialized `DatasetManifest` for instantiation, this repo currently supports two formats of data that can instantiates `DatasetManifest`,
-using `DatasetManifest.create_dataset_manifest(dataset_info, usage, container_sas_or_root_dir)`: `COCO` and `IRIS` (legacy).
-
-`DatasetInfo` as the first arg in the arg list wraps the metainfo about the dataset like the name of the dataset, locations of the images, annotation files, etc. See examples in the sections below
-for different data formats.
-
-Once a `DatasetManifest` is created, you can create a `ManifestDataset` for accessing the data in the dataset, especially the image data, for training, visualization, etc:
-
-```{python}
-dataset = ManifestDataset(dataset_info, dataset_manifest, coordinates='relative')
-```
-
-#### Coco format
-
-Here is an example with explanation of what a `DatasetInfo` looks like for coco format, when it is serialized into json:
-
-```{json}
-    {
-        "name": "sampled-ms-coco",
-        "version": 1,
-        "description": "A sampled ms-coco dataset.",
-        "type": "object_detection",
-        "format": "coco", // indicating the annotation data are stored in coco format
-        "root_folder": "detection/coco2017_20200401", // a root folder for all files listed
-        "train": {
-            "index_path": "train.json", // coco json file for training, see next section for example
-            "files_for_local_usage": [ // associated files including data such as images
-                "images/train_images.zip"
-            ]
-        },
-        "val": {
-            "index_path": "val.json",
-            "files_for_local_usage": [
-                "images/val_images.zip"
-            ]
-        },
-        "test": {
-            "index_path": "test.json",
-            "files_for_local_usage": [
-                "images/test_images.zip"
-            ]
-        }
-    }
-```
-
-Coco annotation format details w.r.t. `multiclass/label_classification`, `object_detection`, `image_caption`, `image_text_match` and `multitask`  can be found in `COCO_DATA_FORMAT.md`.
-
-
-#### Iris format
-
-Iris format is a legacy format which can be found in `IRIS_DATA_FORMAT.md`. Only `multiclass/label_classification`, `object_detection` and `multitask` are supported.
-
-## Dataset management and access
-
-Once you have multiple datasets, it is more convenient to have all the `DatasetInfo` in one place and instantiate `DatasetManifest` or even `ManifestDataset` by just using the dataset name, usage (
-train, val ,test) and version.
-
-This repo offers the class `DatasetHub` for this purpose. Once instantiated with a json including the `DatasetInfo` for all datasets, you can retrieve a `ManifestDataset` by
-
-```{python}
-import pathlib
-
-dataset_infos_json_path = 'datasets.json'
-dataset_hub = DatasetHub(pathlib.Path(dataset_infos_json_path).read_text())
-stanford_cars = dataset_hub.create_manifest_dataset(blob_container_sas, local_dir, 'stanford-cars', version=1, usage='train')
-
-# note that you can pass multiple datasets.json to DatasetHub, it can combine them all
-# example: DatasetHub([ds_json1, ds_json2, ...])
-# note that you can specify multiple usages in create_manifest_dataset call
-# example dataset_hub.create_manifest_dataset(blob_container_sas, local_dir, 'stanford-cars', version=1, usage=['train', 'val'])
-
-for img, targets, sample_idx_str in stanford_cars:
-    img.show()
-    img.close()
-    print(targets)
-```
-
-Note that this hub class works with data saved in both Azure Blob container and on local disk.
-
-If `local_dir`:
-
-1. is provided, the hub will look for the resources locally and **download the data** (files included in "
-   files_for_local_usage", the index files, metadata (if iris format), labelmap (if iris format))
-   from `blob_container_sas` if not present locally
-2. is NOT provided (i.e. `None`), the hub will create a manifest dataset that directly consumes data from the blob
-   indicated by `blob_container_sas`. Note that this does not work, if data are stored in zipped files. You will have to
-   unzip your data in the azure blob. (Index files requires no update, if image paths are for zip files: "a.zip@1.jpg").
-   This kind of azure-based dataset is good for large dataset exploration, but can be slow for training.
-
-When data exists on local disk, `blob_container_sas` can be `None`.
-
-### Training with PyTorch
-
-Training with PyTorch is easy. After instantiating a `ManifestDataset`, simply passing it in `vision_datasets.pytorch.torch_dataset.TorchDataset` together with the `transform`, then you are good to go with the PyTorch DataLoader for training.
-
-### Managing datasets with DatasetHub on cloud storage
-
-If you are using `DatasetHub` to manage datasets in cloud storage, we recommend zipping (with uncompressed mode) the images into one or multiple zip files before uploading it and update the file path in index files to be like `train.zip@1.jpg` from `train\1.jpg`. You can do it with `7zip` (set compression level to 'store') on Windows or [zip](https://superuser.com/questions/411394/zip-files-without-compression) command on Linux.
-
-If you upload folders of images directly to cloud storage:
-
-- you will need to list all images in `"files_for_local_usage"`, which can be millions of entries
-- downloading images one by one (even with multithreading) is much slower than downloading a few zip files
-
-One more thing is that sometimes when you create a zip file `train.zip`, you might find out that there is only one `train` folder in the zip. This will fail the file loading if the path is `train.zip@1.jpg`, as the image is actually at `train.zip@train\1.jpg`. It is ok to have this extra layer but please make sure the path is correct.
-
-
```

### Comparing `vision_datasets-0.2.8/README.md` & `vision_datasets-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `vision_datasets-0.2.8/setup.py` & `vision_datasets-0.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 from os import path
 
-VERSION = '0.2.8'
+VERSION = '0.2.9'
 
 # Get the long description from the README file
 here = path.abspath(path.dirname(__file__))
 with open(path.join(here, 'README.md'), 'r') as f:
     long_description = f.read()
 
 setuptools.setup(name='vision_datasets',
```

### Comparing `vision_datasets-0.2.8/tests/test_box_alteration.py` & `vision_datasets-0.2.9/tests/test_box_alteration.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-0.2.8/tests/test_dataset_downloader.py` & `vision_datasets-0.2.9/tests/test_dataset_downloader.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-0.2.8/tests/test_dataset_manifest.py` & `vision_datasets-0.2.9/tests/test_dataset_manifest.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-0.2.8/tests/test_dataset_registry.py` & `vision_datasets-0.2.9/tests/test_dataset_registry.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-0.2.8/tests/test_file_reader.py` & `vision_datasets-0.2.9/tests/test_file_reader.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-0.2.8/tests/test_manifest_dataset.py` & `vision_datasets-0.2.9/tests/test_manifest_dataset.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-0.2.8/tests/test_pytorch_dataset.py` & `vision_datasets-0.2.9/tests/test_pytorch_dataset.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-0.2.8/vision_datasets/commands/convert_local_dir_ic_data.py` & `vision_datasets-0.2.9/vision_datasets/commands/convert_local_dir_ic_data.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-0.2.8/vision_datasets/commands/converter_od_to_ic.py` & `vision_datasets-0.2.9/vision_datasets/commands/converter_od_to_ic.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-0.2.8/vision_datasets/commands/converter_tsv_to_coco.py` & `vision_datasets-0.2.9/vision_datasets/commands/converter_tsv_to_coco.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-0.2.8/vision_datasets/commands/converter_tsv_to_iris.py` & `vision_datasets-0.2.9/vision_datasets/commands/converter_tsv_to_iris.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-0.2.8/vision_datasets/commands/converter_yolo_darknet_to_cvs.py` & `vision_datasets-0.2.9/vision_datasets/commands/converter_yolo_darknet_to_cvs.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-0.2.8/vision_datasets/commands/dataset_check.py` & `vision_datasets-0.2.9/vision_datasets/commands/dataset_check.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-0.2.8/vision_datasets/commands/download.py` & `vision_datasets-0.2.9/vision_datasets/commands/download.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-0.2.8/vision_datasets/commands/generate_image_meta_info.py` & `vision_datasets-0.2.9/vision_datasets/commands/generate_image_meta_info.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-0.2.8/vision_datasets/commands/merge_datasets.py` & `vision_datasets-0.2.9/vision_datasets/commands/merge_datasets.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-0.2.8/vision_datasets/commands/utils.py` & `vision_datasets-0.2.9/vision_datasets/commands/utils.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-0.2.8/vision_datasets/common/base_dataset.py` & `vision_datasets-0.2.9/vision_datasets/common/base_dataset.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-0.2.8/vision_datasets/common/constants.py` & `vision_datasets-0.2.9/vision_datasets/common/constants.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-0.2.8/vision_datasets/common/data_manifest.py` & `vision_datasets-0.2.9/vision_datasets/common/data_manifest.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-0.2.8/vision_datasets/common/dataset_downloader.py` & `vision_datasets-0.2.9/vision_datasets/common/dataset_downloader.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-0.2.8/vision_datasets/common/dataset_info.py` & `vision_datasets-0.2.9/vision_datasets/common/dataset_info.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-0.2.8/vision_datasets/common/dataset_registry.py` & `vision_datasets-0.2.9/vision_datasets/common/dataset_registry.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-0.2.8/vision_datasets/common/image_loader.py` & `vision_datasets-0.2.9/vision_datasets/common/image_loader.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-0.2.8/vision_datasets/common/manifest_dataset.py` & `vision_datasets-0.2.9/vision_datasets/common/manifest_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,17 +160,16 @@
                 'shift_relative_bounds': lower/upper bounds of relative ratio wrt box width and height that a box can shift, e.g., (-0.3, 0.1)
                 'rnd_seed' [optional]: rnd seed used for box crop zoom and shift, default being 0
         """
         super().__init__(detection_dataset, DatasetTypes.IC_MULTICLASS)
 
         self._n_booxes = 0
         self._box_abs_id_to_img_rel_id = {}
-        for img_id, x in enumerate(self._dataset):
-            boxes = x[1]
-            for i in range(len(boxes)):
+        for img_id, x in enumerate(self._dataset.dataset_manifest.images):
+            for i in range(len(x.labels)):
                 self._box_abs_id_to_img_rel_id[self._n_booxes] = (img_id, i)
                 self._n_booxes += 1
         self._box_aug_params = box_aug_params
 
         self._box_aug_rnd = random.Random(self._box_aug_params.get('rnd_seed', 0)) if box_aug_params else None
         self._box_pick_rnd = random.Random(0)
 
@@ -180,18 +179,15 @@
     def _get_single_item(self, index):
         img_idx, box_rel_idx = self._box_abs_id_to_img_rel_id[index]
 
         img, boxes, _ = self._dataset[img_idx]
         c_id, left, t, r, b = boxes[box_rel_idx]
         if self._dataset.coordinates == 'relative':
             w, h = img.size
-            left *= w
-            t *= h
-            r *= w
-            b *= h
+            left, t, r, b = left * w, t * h, r * w, b * h
 
         box_img = DetectionAsClassificationByCroppingDataset.crop(img, left, t, r, b, self._box_aug_params, self._box_aug_rnd)
         return box_img, [c_id], str(index)
 
     @staticmethod
     def crop(img, left, t, r, b, aug_params=None, rnd: random.Random = None):
         if aug_params:
```

### Comparing `vision_datasets-0.2.8/vision_datasets/common/util.py` & `vision_datasets-0.2.9/vision_datasets/common/util.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-0.2.8/vision_datasets/pytorch/dataset.py` & `vision_datasets-0.2.9/vision_datasets/pytorch/dataset.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-0.2.8/vision_datasets/pytorch/torch_dataset.py` & `vision_datasets-0.2.9/vision_datasets/pytorch/torch_dataset.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-0.2.8/vision_datasets/resources/dataset_hub.py` & `vision_datasets-0.2.9/vision_datasets/resources/dataset_hub.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-0.2.8/vision_datasets.egg-info/PKG-INFO` & `vision_datasets-0.2.9/vision_datasets.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,162 +1,159 @@
 Metadata-Version: 2.1
 Name: vision-datasets
-Version: 0.2.8
+Version: 0.2.9
 Summary: A utility repo for vision dataset access and management.
 Home-page: https://github.com/microsoft/vision-datasets
 Author: Ping Jin, Shohei Ono
 License: MIT
+Description: # Vision Datasets
+        
+        ## Introduction
+        
+        This repo
+        
+        - defines unified contract for dataset for purposes such as training, visualization, and exploration, via `DatasetManifest` and `ImageDataManifest`.
+        - provides API for organizing and accessing datasets, via `DatasetHub`
+        
+        Currently, five `basic` types of data are supported: 
+        - `classification_multiclass`: each image can is only with one label.
+        - `classification_multilabel`: each image can is with one or multiple labels (e.g., 'cat', 'animal', 'pet').
+        - `object_detection`: each image is labeled with bounding boxes surrounding the objects of interest.
+        - `image_caption`: each image is labeled with a few texts describing the images.
+        - `image_text_matching`: each image is associated with a collection of texts describing the image, and whether each text description matches the image or not
+        
+        `multitask` type is a composition type, where one set of images has multiple sets of annotations available for different tasks, where each task can be of any basic type.
+        
+        
+        ## Dataset Contracts
+        
+        - `DatasetManifest` wraps the information about a dataset including labelmap, images (width, height, path to image), and annotations. `ImageDataManifest` encapsulates information about each image.
+        - `ImageDataManifest` encapsulates image-specific information, such as image id, path, labels, and width/height. One thing to note here is that the image path can be
+            1. a local path (absolute `c:\images\1.jpg` or relative `images\1.jpg`)
+            2. a local path in a **non-compressed** zip file (absolute `c:\images.zip@1.jpg` or relative `images.zip@1.jpg`) or
+            3. an url
+        - `ManifestDataset` is an iterable dataset class that consumes the information from `DatasetManifest`.
+        
+        `ManifestDataset` is able to load the data from all three kinds of paths. Both 1. and 2. are good for training, as they access data from local disk while the 3rd one is good for data exploration, if you have the data in azure storage.
+        
+        For `multitask` dataset, the labels stored in the `ImageDataManifest` is a `dict` mapping from task name to that task's labels. The labelmap stored in `DatasetManifest` is also a `dict` mapping from task name to that task's labels.
+        
+        ### Creating DatasetManifest
+        
+        In addition to loading a serialized `DatasetManifest` for instantiation, this repo currently supports two formats of data that can instantiates `DatasetManifest`,
+        using `DatasetManifest.create_dataset_manifest(dataset_info, usage, container_sas_or_root_dir)`: `COCO` and `IRIS` (legacy).
+        
+        `DatasetInfo` as the first arg in the arg list wraps the metainfo about the dataset like the name of the dataset, locations of the images, annotation files, etc. See examples in the sections below
+        for different data formats.
+        
+        Once a `DatasetManifest` is created, you can create a `ManifestDataset` for accessing the data in the dataset, especially the image data, for training, visualization, etc:
+        
+        ```{python}
+        dataset = ManifestDataset(dataset_info, dataset_manifest, coordinates='relative')
+        ```
+        
+        #### Coco format
+        
+        Here is an example with explanation of what a `DatasetInfo` looks like for coco format, when it is serialized into json:
+        
+        ```{json}
+            {
+                "name": "sampled-ms-coco",
+                "version": 1,
+                "description": "A sampled ms-coco dataset.",
+                "type": "object_detection",
+                "format": "coco", // indicating the annotation data are stored in coco format
+                "root_folder": "detection/coco2017_20200401", // a root folder for all files listed
+                "train": {
+                    "index_path": "train.json", // coco json file for training, see next section for example
+                    "files_for_local_usage": [ // associated files including data such as images
+                        "images/train_images.zip"
+                    ]
+                },
+                "val": {
+                    "index_path": "val.json",
+                    "files_for_local_usage": [
+                        "images/val_images.zip"
+                    ]
+                },
+                "test": {
+                    "index_path": "test.json",
+                    "files_for_local_usage": [
+                        "images/test_images.zip"
+                    ]
+                }
+            }
+        ```
+        
+        Coco annotation format details w.r.t. `multiclass/label_classification`, `object_detection`, `image_caption`, `image_text_match` and `multitask`  can be found in `COCO_DATA_FORMAT.md`.
+        
+        
+        #### Iris format
+        
+        Iris format is a legacy format which can be found in `IRIS_DATA_FORMAT.md`. Only `multiclass/label_classification`, `object_detection` and `multitask` are supported.
+        
+        ## Dataset management and access
+        
+        Once you have multiple datasets, it is more convenient to have all the `DatasetInfo` in one place and instantiate `DatasetManifest` or even `ManifestDataset` by just using the dataset name, usage (
+        train, val ,test) and version.
+        
+        This repo offers the class `DatasetHub` for this purpose. Once instantiated with a json including the `DatasetInfo` for all datasets, you can retrieve a `ManifestDataset` by
+        
+        ```{python}
+        import pathlib
+        
+        dataset_infos_json_path = 'datasets.json'
+        dataset_hub = DatasetHub(pathlib.Path(dataset_infos_json_path).read_text())
+        stanford_cars = dataset_hub.create_manifest_dataset(blob_container_sas, local_dir, 'stanford-cars', version=1, usage='train')
+        
+        # note that you can pass multiple datasets.json to DatasetHub, it can combine them all
+        # example: DatasetHub([ds_json1, ds_json2, ...])
+        # note that you can specify multiple usages in create_manifest_dataset call
+        # example dataset_hub.create_manifest_dataset(blob_container_sas, local_dir, 'stanford-cars', version=1, usage=['train', 'val'])
+        
+        for img, targets, sample_idx_str in stanford_cars:
+            img.show()
+            img.close()
+            print(targets)
+        ```
+        
+        Note that this hub class works with data saved in both Azure Blob container and on local disk.
+        
+        If `local_dir`:
+        
+        1. is provided, the hub will look for the resources locally and **download the data** (files included in "
+           files_for_local_usage", the index files, metadata (if iris format), labelmap (if iris format))
+           from `blob_container_sas` if not present locally
+        2. is NOT provided (i.e. `None`), the hub will create a manifest dataset that directly consumes data from the blob
+           indicated by `blob_container_sas`. Note that this does not work, if data are stored in zipped files. You will have to
+           unzip your data in the azure blob. (Index files requires no update, if image paths are for zip files: "a.zip@1.jpg").
+           This kind of azure-based dataset is good for large dataset exploration, but can be slow for training.
+        
+        When data exists on local disk, `blob_container_sas` can be `None`.
+        
+        ### Training with PyTorch
+        
+        Training with PyTorch is easy. After instantiating a `ManifestDataset`, simply passing it in `vision_datasets.pytorch.torch_dataset.TorchDataset` together with the `transform`, then you are good to go with the PyTorch DataLoader for training.
+        
+        ### Managing datasets with DatasetHub on cloud storage
+        
+        If you are using `DatasetHub` to manage datasets in cloud storage, we recommend zipping (with uncompressed mode) the images into one or multiple zip files before uploading it and update the file path in index files to be like `train.zip@1.jpg` from `train\1.jpg`. You can do it with `7zip` (set compression level to 'store') on Windows or [zip](https://superuser.com/questions/411394/zip-files-without-compression) command on Linux.
+        
+        If you upload folders of images directly to cloud storage:
+        
+        - you will need to list all images in `"files_for_local_usage"`, which can be millions of entries
+        - downloading images one by one (even with multithreading) is much slower than downloading a few zip files
+        
+        One more thing is that sometimes when you create a zip file `train.zip`, you might find out that there is only one `train` folder in the zip. This will fail the file loading if the path is `train.zip@1.jpg`, as the image is actually at `train.zip@train\1.jpg`. It is ok to have this extra layer but please make sure the path is correct.
+        
 Keywords: vision datasets classification detection
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: run
-License-File: LICENSE
-
-# Vision Datasets
-
-## Introduction
-
-This repo
-
-- defines unified contract for dataset for purposes such as training, visualization, and exploration, via `DatasetManifest` and `ImageDataManifest`.
-- provides API for organizing and accessing datasets, via `DatasetHub`
-
-Currently, five `basic` types of data are supported: 
-- `classification_multiclass`: each image can is only with one label.
-- `classification_multilabel`: each image can is with one or multiple labels (e.g., 'cat', 'animal', 'pet').
-- `object_detection`: each image is labeled with bounding boxes surrounding the objects of interest.
-- `image_caption`: each image is labeled with a few texts describing the images.
-- `image_text_matching`: each image is associated with a collection of texts describing the image, and whether each text description matches the image or not
-
-`multitask` type is a composition type, where one set of images has multiple sets of annotations available for different tasks, where each task can be of any basic type.
-
-
-## Dataset Contracts
-
-- `DatasetManifest` wraps the information about a dataset including labelmap, images (width, height, path to image), and annotations. `ImageDataManifest` encapsulates information about each image.
-- `ImageDataManifest` encapsulates image-specific information, such as image id, path, labels, and width/height. One thing to note here is that the image path can be
-    1. a local path (absolute `c:\images\1.jpg` or relative `images\1.jpg`)
-    2. a local path in a **non-compressed** zip file (absolute `c:\images.zip@1.jpg` or relative `images.zip@1.jpg`) or
-    3. an url
-- `ManifestDataset` is an iterable dataset class that consumes the information from `DatasetManifest`.
-
-`ManifestDataset` is able to load the data from all three kinds of paths. Both 1. and 2. are good for training, as they access data from local disk while the 3rd one is good for data exploration, if you have the data in azure storage.
-
-For `multitask` dataset, the labels stored in the `ImageDataManifest` is a `dict` mapping from task name to that task's labels. The labelmap stored in `DatasetManifest` is also a `dict` mapping from task name to that task's labels.
-
-### Creating DatasetManifest
-
-In addition to loading a serialized `DatasetManifest` for instantiation, this repo currently supports two formats of data that can instantiates `DatasetManifest`,
-using `DatasetManifest.create_dataset_manifest(dataset_info, usage, container_sas_or_root_dir)`: `COCO` and `IRIS` (legacy).
-
-`DatasetInfo` as the first arg in the arg list wraps the metainfo about the dataset like the name of the dataset, locations of the images, annotation files, etc. See examples in the sections below
-for different data formats.
-
-Once a `DatasetManifest` is created, you can create a `ManifestDataset` for accessing the data in the dataset, especially the image data, for training, visualization, etc:
-
-```{python}
-dataset = ManifestDataset(dataset_info, dataset_manifest, coordinates='relative')
-```
-
-#### Coco format
-
-Here is an example with explanation of what a `DatasetInfo` looks like for coco format, when it is serialized into json:
-
-```{json}
-    {
-        "name": "sampled-ms-coco",
-        "version": 1,
-        "description": "A sampled ms-coco dataset.",
-        "type": "object_detection",
-        "format": "coco", // indicating the annotation data are stored in coco format
-        "root_folder": "detection/coco2017_20200401", // a root folder for all files listed
-        "train": {
-            "index_path": "train.json", // coco json file for training, see next section for example
-            "files_for_local_usage": [ // associated files including data such as images
-                "images/train_images.zip"
-            ]
-        },
-        "val": {
-            "index_path": "val.json",
-            "files_for_local_usage": [
-                "images/val_images.zip"
-            ]
-        },
-        "test": {
-            "index_path": "test.json",
-            "files_for_local_usage": [
-                "images/test_images.zip"
-            ]
-        }
-    }
-```
-
-Coco annotation format details w.r.t. `multiclass/label_classification`, `object_detection`, `image_caption`, `image_text_match` and `multitask`  can be found in `COCO_DATA_FORMAT.md`.
-
-
-#### Iris format
-
-Iris format is a legacy format which can be found in `IRIS_DATA_FORMAT.md`. Only `multiclass/label_classification`, `object_detection` and `multitask` are supported.
-
-## Dataset management and access
-
-Once you have multiple datasets, it is more convenient to have all the `DatasetInfo` in one place and instantiate `DatasetManifest` or even `ManifestDataset` by just using the dataset name, usage (
-train, val ,test) and version.
-
-This repo offers the class `DatasetHub` for this purpose. Once instantiated with a json including the `DatasetInfo` for all datasets, you can retrieve a `ManifestDataset` by
-
-```{python}
-import pathlib
-
-dataset_infos_json_path = 'datasets.json'
-dataset_hub = DatasetHub(pathlib.Path(dataset_infos_json_path).read_text())
-stanford_cars = dataset_hub.create_manifest_dataset(blob_container_sas, local_dir, 'stanford-cars', version=1, usage='train')
-
-# note that you can pass multiple datasets.json to DatasetHub, it can combine them all
-# example: DatasetHub([ds_json1, ds_json2, ...])
-# note that you can specify multiple usages in create_manifest_dataset call
-# example dataset_hub.create_manifest_dataset(blob_container_sas, local_dir, 'stanford-cars', version=1, usage=['train', 'val'])
-
-for img, targets, sample_idx_str in stanford_cars:
-    img.show()
-    img.close()
-    print(targets)
-```
-
-Note that this hub class works with data saved in both Azure Blob container and on local disk.
-
-If `local_dir`:
-
-1. is provided, the hub will look for the resources locally and **download the data** (files included in "
-   files_for_local_usage", the index files, metadata (if iris format), labelmap (if iris format))
-   from `blob_container_sas` if not present locally
-2. is NOT provided (i.e. `None`), the hub will create a manifest dataset that directly consumes data from the blob
-   indicated by `blob_container_sas`. Note that this does not work, if data are stored in zipped files. You will have to
-   unzip your data in the azure blob. (Index files requires no update, if image paths are for zip files: "a.zip@1.jpg").
-   This kind of azure-based dataset is good for large dataset exploration, but can be slow for training.
-
-When data exists on local disk, `blob_container_sas` can be `None`.
-
-### Training with PyTorch
-
-Training with PyTorch is easy. After instantiating a `ManifestDataset`, simply passing it in `vision_datasets.pytorch.torch_dataset.TorchDataset` together with the `transform`, then you are good to go with the PyTorch DataLoader for training.
-
-### Managing datasets with DatasetHub on cloud storage
-
-If you are using `DatasetHub` to manage datasets in cloud storage, we recommend zipping (with uncompressed mode) the images into one or multiple zip files before uploading it and update the file path in index files to be like `train.zip@1.jpg` from `train\1.jpg`. You can do it with `7zip` (set compression level to 'store') on Windows or [zip](https://superuser.com/questions/411394/zip-files-without-compression) command on Linux.
-
-If you upload folders of images directly to cloud storage:
-
-- you will need to list all images in `"files_for_local_usage"`, which can be millions of entries
-- downloading images one by one (even with multithreading) is much slower than downloading a few zip files
-
-One more thing is that sometimes when you create a zip file `train.zip`, you might find out that there is only one `train` folder in the zip. This will fail the file loading if the path is `train.zip@1.jpg`, as the image is actually at `train.zip@train\1.jpg`. It is ok to have this extra layer but please make sure the path is correct.
-
-
```

### Comparing `vision_datasets-0.2.8/vision_datasets.egg-info/SOURCES.txt` & `vision_datasets-0.2.9/vision_datasets.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 README.md
 setup.py
 tox.ini
 tests/test_box_alteration.py
 tests/test_dataset_downloader.py
 tests/test_dataset_manifest.py
 tests/test_dataset_registry.py
+tests/test_detection_as_classification.py
 tests/test_file_reader.py
+tests/test_fixtures.py
 tests/test_manifest_dataset.py
 tests/test_pytorch_dataset.py
 vision_datasets/__init__.py
 vision_datasets.egg-info/PKG-INFO
 vision_datasets.egg-info/SOURCES.txt
 vision_datasets.egg-info/dependency_links.txt
 vision_datasets.egg-info/entry_points.txt
```

### Comparing `vision_datasets-0.2.8/vision_datasets.egg-info/entry_points.txt` & `vision_datasets-0.2.9/vision_datasets.egg-info/entry_points.txt`

 * *Files identical despite different names*

