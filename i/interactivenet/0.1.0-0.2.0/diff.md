# Comparing `tmp/interactivenet-0.1.0.tar.gz` & `tmp/interactivenet-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interactivenet-0.1.0.tar", last modified: Wed Jun 14 13:53:55 2023, max compression
+gzip compressed data, was "interactivenet-0.2.0.tar", last modified: Tue Jun 20 12:38:00 2023, max compression
```

## Comparing `interactivenet-0.1.0.tar` & `interactivenet-0.2.0.tar`

### file list

```diff
@@ -1,63 +1,62 @@
-drwxr-xr-x   0 dspaanderman  (1128) bigruser  (1150)        0 2023-06-14 13:53:55.675280 interactivenet-0.1.0/
--rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     1849 2023-03-31 07:37:29.000000 interactivenet-0.1.0/.gitignore
--rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)    11357 2023-06-14 13:36:32.000000 interactivenet-0.1.0/LICENSE.md
--rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)      596 2023-06-14 13:53:55.675280 interactivenet-0.1.0/PKG-INFO
--rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)    13153 2023-06-14 13:43:07.000000 interactivenet-0.1.0/README.md
-drwxr-xr-x   0 dspaanderman  (1128) bigruser  (1150)        0 2023-06-14 13:53:55.308273 interactivenet-0.1.0/documentation/
--rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     6154 2023-03-09 12:42:14.000000 interactivenet-0.1.0/documentation/dataset_conversion.md
--rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)      953 2023-03-30 13:46:30.000000 interactivenet-0.1.0/documentation/env_variables.md
--rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     1023 2023-03-09 12:42:15.000000 interactivenet-0.1.0/documentation/synthetic_interactions.md
-drwxr-xr-x   0 dspaanderman  (1128) bigruser  (1150)        0 2023-06-14 13:53:55.316274 interactivenet-0.1.0/interactivenet/
--rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)       15 2023-03-31 09:10:08.000000 interactivenet-0.1.0/interactivenet/__init__.py
-drwxr-xr-x   0 dspaanderman  (1128) bigruser  (1150)        0 2023-06-14 13:53:55.375275 interactivenet-0.1.0/interactivenet/deploy/
--rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)       15 2023-03-31 09:10:44.000000 interactivenet-0.1.0/interactivenet/deploy/__init__.py
--rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)      172 2023-03-30 14:00:27.000000 interactivenet-0.1.0/interactivenet/deploy/download_model.py
--rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)      172 2023-03-30 14:00:28.000000 interactivenet-0.1.0/interactivenet/deploy/print_models.py
--rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     2059 2023-03-30 18:45:56.000000 interactivenet-0.1.0/interactivenet/deploy/save_model.py
-drwxr-xr-x   0 dspaanderman  (1128) bigruser  (1150)        0 2023-06-14 13:53:55.458276 interactivenet-0.1.0/interactivenet/experiment_planning/
--rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)       15 2023-03-31 09:10:36.000000 interactivenet-0.1.0/interactivenet/experiment_planning/__init__.py
--rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)    17277 2023-03-30 13:50:23.000000 interactivenet-0.1.0/interactivenet/experiment_planning/fingerprinting.py
--rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     6656 2023-03-30 13:50:23.000000 interactivenet-0.1.0/interactivenet/experiment_planning/generate_dataset_json.py
--rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)    19674 2023-03-30 13:59:33.000000 interactivenet-0.1.0/interactivenet/experiment_planning/mimic_annotations.py
--rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     2692 2023-03-30 13:59:33.000000 interactivenet-0.1.0/interactivenet/experiment_planning/plan_and_process.py
--rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     4813 2023-03-30 13:50:23.000000 interactivenet-0.1.0/interactivenet/experiment_planning/preprocessing.py
-drwxr-xr-x   0 dspaanderman  (1128) bigruser  (1150)        0 2023-06-14 13:53:55.478277 interactivenet-0.1.0/interactivenet/networks/
--rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)       15 2023-03-31 09:10:33.000000 interactivenet-0.1.0/interactivenet/networks/__init__.py
--rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     9263 2023-03-30 13:59:33.000000 interactivenet-0.1.0/interactivenet/networks/unet.py
-drwxr-xr-x   0 dspaanderman  (1128) bigruser  (1150)        0 2023-06-14 13:53:55.508277 interactivenet-0.1.0/interactivenet/test/
--rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)       15 2023-03-31 09:10:25.000000 interactivenet-0.1.0/interactivenet/test/__init__.py
--rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     5563 2023-03-30 14:02:07.000000 interactivenet-0.1.0/interactivenet/test/ensemble.py
--rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     9599 2023-03-30 14:00:09.000000 interactivenet-0.1.0/interactivenet/test/inference.py
--rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     6732 2023-03-30 13:59:33.000000 interactivenet-0.1.0/interactivenet/test/predict.py
--rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     9376 2023-03-30 13:59:33.000000 interactivenet-0.1.0/interactivenet/test/refinement.py
--rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     2824 2023-03-30 14:00:37.000000 interactivenet-0.1.0/interactivenet/test/run.py
-drwxr-xr-x   0 dspaanderman  (1128) bigruser  (1150)        0 2023-06-14 13:53:55.536278 interactivenet-0.1.0/interactivenet/training/
--rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)       15 2023-03-31 09:10:13.000000 interactivenet-0.1.0/interactivenet/training/__init__.py
--rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     7912 2023-03-30 13:59:33.000000 interactivenet-0.1.0/interactivenet/training/postprocessing.py
--rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     8076 2023-03-30 13:59:33.000000 interactivenet-0.1.0/interactivenet/training/run.py
-drwxr-xr-x   0 dspaanderman  (1128) bigruser  (1150)        0 2023-06-14 13:53:55.568278 interactivenet-0.1.0/interactivenet/transforms/
--rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)       15 2023-03-31 09:13:16.000000 interactivenet-0.1.0/interactivenet/transforms/__init__.py
--rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     7211 2023-03-30 13:59:33.000000 interactivenet-0.1.0/interactivenet/transforms/set_transforms.py
--rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)    27959 2023-03-31 07:34:40.000000 interactivenet-0.1.0/interactivenet/transforms/transforms.py
-drwxr-xr-x   0 dspaanderman  (1128) bigruser  (1150)        0 2023-06-14 13:53:55.659280 interactivenet-0.1.0/interactivenet/utils/
--rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)       15 2023-03-31 09:11:04.000000 interactivenet-0.1.0/interactivenet/utils/__init__.py
--rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     1515 2023-03-30 13:50:23.000000 interactivenet-0.1.0/interactivenet/utils/callbacks.py
--rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)      449 2023-03-30 13:47:36.000000 interactivenet-0.1.0/interactivenet/utils/dump.py
--rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)      361 2023-03-30 13:47:36.000000 interactivenet-0.1.0/interactivenet/utils/jsonencoders.py
--rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)      907 2023-03-30 13:47:36.000000 interactivenet-0.1.0/interactivenet/utils/mlflow.py
--rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     1176 2023-03-30 13:59:33.000000 interactivenet-0.1.0/interactivenet/utils/postprocessing.py
--rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     4410 2023-03-30 13:47:36.000000 interactivenet-0.1.0/interactivenet/utils/resample.py
--rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     2942 2023-03-30 13:59:53.000000 interactivenet-0.1.0/interactivenet/utils/results.py
--rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     5423 2023-03-30 13:59:33.000000 interactivenet-0.1.0/interactivenet/utils/statistics.py
--rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     1244 2023-03-30 13:44:55.000000 interactivenet-0.1.0/interactivenet/utils/subtypes.py
--rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     7815 2023-03-30 13:59:33.000000 interactivenet-0.1.0/interactivenet/utils/utils.py
--rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     2869 2023-03-30 13:59:33.000000 interactivenet-0.1.0/interactivenet/utils/visualize.py
-drwxr-xr-x   0 dspaanderman  (1128) bigruser  (1150)        0 2023-06-14 13:53:55.328274 interactivenet-0.1.0/interactivenet.egg-info/
--rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)      596 2023-06-14 13:53:55.000000 interactivenet-0.1.0/interactivenet.egg-info/PKG-INFO
--rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     1773 2023-06-14 13:53:55.000000 interactivenet-0.1.0/interactivenet.egg-info/SOURCES.txt
--rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)        1 2023-06-14 13:53:55.000000 interactivenet-0.1.0/interactivenet.egg-info/dependency_links.txt
--rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     1050 2023-06-14 13:53:55.000000 interactivenet-0.1.0/interactivenet.egg-info/entry_points.txt
--rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)      260 2023-06-14 13:53:55.000000 interactivenet-0.1.0/interactivenet.egg-info/requires.txt
--rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)       15 2023-06-14 13:53:55.000000 interactivenet-0.1.0/interactivenet.egg-info/top_level.txt
--rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)       79 2023-06-14 13:53:55.677280 interactivenet-0.1.0/setup.cfg
--rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     2600 2023-06-14 13:51:36.000000 interactivenet-0.1.0/setup.py
+drwxr-xr-x   0 dspaanderman  (1128) bigruser  (1150)        0 2023-06-20 12:38:00.164920 interactivenet-0.2.0/
+-rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     1849 2023-03-31 07:37:29.000000 interactivenet-0.2.0/.gitignore
+-rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)    10172 2023-06-20 12:34:28.000000 interactivenet-0.2.0/LICENSE
+-rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)      634 2023-06-20 12:38:00.164920 interactivenet-0.2.0/PKG-INFO
+-rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)    13560 2023-06-20 12:34:28.000000 interactivenet-0.2.0/README.md
+drwxr-xr-x   0 dspaanderman  (1128) bigruser  (1150)        0 2023-06-20 12:38:00.158920 interactivenet-0.2.0/documentation/
+-rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     6154 2023-03-09 12:42:14.000000 interactivenet-0.2.0/documentation/dataset_conversion.md
+-rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)      953 2023-03-30 13:46:30.000000 interactivenet-0.2.0/documentation/env_variables.md
+-rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     1023 2023-03-09 12:42:15.000000 interactivenet-0.2.0/documentation/synthetic_interactions.md
+drwxr-xr-x   0 dspaanderman  (1128) bigruser  (1150)        0 2023-06-20 12:38:00.158920 interactivenet-0.2.0/interactivenet/
+-rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)      723 2023-06-20 12:34:28.000000 interactivenet-0.2.0/interactivenet/__init__.py
+drwxr-xr-x   0 dspaanderman  (1128) bigruser  (1150)        0 2023-06-20 12:38:00.159920 interactivenet-0.2.0/interactivenet/deploy/
+-rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)      723 2023-06-20 12:34:28.000000 interactivenet-0.2.0/interactivenet/deploy/__init__.py
+-rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     3738 2023-06-20 12:34:28.000000 interactivenet-0.2.0/interactivenet/deploy/download_model.py
+-rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     2767 2023-06-20 12:34:28.000000 interactivenet-0.2.0/interactivenet/deploy/save_model.py
+drwxr-xr-x   0 dspaanderman  (1128) bigruser  (1150)        0 2023-06-20 12:38:00.160920 interactivenet-0.2.0/interactivenet/experiment_planning/
+-rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)      723 2023-06-20 12:34:28.000000 interactivenet-0.2.0/interactivenet/experiment_planning/__init__.py
+-rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)    17985 2023-06-20 12:34:28.000000 interactivenet-0.2.0/interactivenet/experiment_planning/fingerprinting.py
+-rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     7364 2023-06-20 12:34:28.000000 interactivenet-0.2.0/interactivenet/experiment_planning/generate_dataset_json.py
+-rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)    20382 2023-06-20 12:34:28.000000 interactivenet-0.2.0/interactivenet/experiment_planning/mimic_annotations.py
+-rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     3400 2023-06-20 12:34:28.000000 interactivenet-0.2.0/interactivenet/experiment_planning/plan_and_process.py
+-rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     5521 2023-06-20 12:34:28.000000 interactivenet-0.2.0/interactivenet/experiment_planning/preprocessing.py
+drwxr-xr-x   0 dspaanderman  (1128) bigruser  (1150)        0 2023-06-20 12:38:00.161920 interactivenet-0.2.0/interactivenet/networks/
+-rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)      723 2023-06-20 12:34:28.000000 interactivenet-0.2.0/interactivenet/networks/__init__.py
+-rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     9971 2023-06-20 12:34:28.000000 interactivenet-0.2.0/interactivenet/networks/unet.py
+drwxr-xr-x   0 dspaanderman  (1128) bigruser  (1150)        0 2023-06-20 12:38:00.161920 interactivenet-0.2.0/interactivenet/test/
+-rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)      723 2023-06-20 12:34:28.000000 interactivenet-0.2.0/interactivenet/test/__init__.py
+-rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     6271 2023-06-20 12:34:28.000000 interactivenet-0.2.0/interactivenet/test/ensemble.py
+-rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)    10307 2023-06-20 12:34:28.000000 interactivenet-0.2.0/interactivenet/test/inference.py
+-rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     7440 2023-06-20 12:34:28.000000 interactivenet-0.2.0/interactivenet/test/predict.py
+-rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)    10084 2023-06-20 12:34:28.000000 interactivenet-0.2.0/interactivenet/test/refinement.py
+-rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     3532 2023-06-20 12:34:28.000000 interactivenet-0.2.0/interactivenet/test/run.py
+drwxr-xr-x   0 dspaanderman  (1128) bigruser  (1150)        0 2023-06-20 12:38:00.162920 interactivenet-0.2.0/interactivenet/training/
+-rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)      723 2023-06-20 12:34:28.000000 interactivenet-0.2.0/interactivenet/training/__init__.py
+-rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     8620 2023-06-20 12:34:28.000000 interactivenet-0.2.0/interactivenet/training/postprocessing.py
+-rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     8784 2023-06-20 12:34:28.000000 interactivenet-0.2.0/interactivenet/training/run.py
+drwxr-xr-x   0 dspaanderman  (1128) bigruser  (1150)        0 2023-06-20 12:38:00.162920 interactivenet-0.2.0/interactivenet/transforms/
+-rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)      723 2023-06-20 12:34:28.000000 interactivenet-0.2.0/interactivenet/transforms/__init__.py
+-rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     7919 2023-06-20 12:34:28.000000 interactivenet-0.2.0/interactivenet/transforms/set_transforms.py
+-rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)    28667 2023-06-20 12:34:28.000000 interactivenet-0.2.0/interactivenet/transforms/transforms.py
+drwxr-xr-x   0 dspaanderman  (1128) bigruser  (1150)        0 2023-06-20 12:38:00.164920 interactivenet-0.2.0/interactivenet/utils/
+-rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)      723 2023-06-20 12:34:28.000000 interactivenet-0.2.0/interactivenet/utils/__init__.py
+-rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     2223 2023-06-20 12:34:28.000000 interactivenet-0.2.0/interactivenet/utils/callbacks.py
+-rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     1157 2023-06-20 12:34:28.000000 interactivenet-0.2.0/interactivenet/utils/dump.py
+-rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     1069 2023-06-20 12:34:28.000000 interactivenet-0.2.0/interactivenet/utils/jsonencoders.py
+-rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     1615 2023-06-20 12:34:28.000000 interactivenet-0.2.0/interactivenet/utils/mlflow.py
+-rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     1884 2023-06-20 12:34:28.000000 interactivenet-0.2.0/interactivenet/utils/postprocessing.py
+-rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     5118 2023-06-20 12:34:28.000000 interactivenet-0.2.0/interactivenet/utils/resample.py
+-rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     3650 2023-06-20 12:34:28.000000 interactivenet-0.2.0/interactivenet/utils/results.py
+-rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     6131 2023-06-20 12:34:28.000000 interactivenet-0.2.0/interactivenet/utils/statistics.py
+-rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     1952 2023-06-20 12:34:28.000000 interactivenet-0.2.0/interactivenet/utils/subtypes.py
+-rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     8523 2023-06-20 12:34:28.000000 interactivenet-0.2.0/interactivenet/utils/utils.py
+-rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     3577 2023-06-20 12:34:28.000000 interactivenet-0.2.0/interactivenet/utils/visualize.py
+drwxr-xr-x   0 dspaanderman  (1128) bigruser  (1150)        0 2023-06-20 12:38:00.159920 interactivenet-0.2.0/interactivenet.egg-info/
+-rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)      634 2023-06-20 12:38:00.000000 interactivenet-0.2.0/interactivenet.egg-info/PKG-INFO
+-rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     1732 2023-06-20 12:38:00.000000 interactivenet-0.2.0/interactivenet.egg-info/SOURCES.txt
+-rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)        1 2023-06-20 12:38:00.000000 interactivenet-0.2.0/interactivenet.egg-info/dependency_links.txt
+-rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     1103 2023-06-20 12:38:00.000000 interactivenet-0.2.0/interactivenet.egg-info/entry_points.txt
+-rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)      260 2023-06-20 12:38:00.000000 interactivenet-0.2.0/interactivenet.egg-info/requires.txt
+-rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)       15 2023-06-20 12:38:00.000000 interactivenet-0.2.0/interactivenet.egg-info/top_level.txt
+-rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)       79 2023-06-20 12:38:00.165920 interactivenet-0.2.0/setup.cfg
+-rw-r--r--   0 dspaanderman  (1128) bigruser  (1150)     2795 2023-06-20 12:36:38.000000 interactivenet-0.2.0/setup.py
```

### Comparing `interactivenet-0.1.0/.gitignore` & `interactivenet-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `interactivenet-0.1.0/LICENSE.md` & `interactivenet-0.2.0/LICENSE`

 * *Files 4% similar despite different names*

```diff
@@ -169,33 +169,8 @@
       License. However, in accepting such obligations, You may act only
       on Your own behalf and on Your sole responsibility, not on behalf
       of any other Contributor, and only if You agree to indemnify,
       defend, and hold each Contributor harmless for any liability
       incurred by, or claims asserted against, such Contributor by reason
       of your accepting any such warranty or additional liability.
 
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+   END OF TERMS AND CONDITIONS
```

### Comparing `interactivenet-0.1.0/PKG-INFO` & `interactivenet-0.2.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 1.2
 Name: interactivenet
-Version: 0.1.0
+Version: 0.2.0
 Summary: InteractiveNet, a framework for minimally interactive medical image segmentation.
 Home-page: https://github.com/Douwe-Spaanderman/InteractiveNet
-Author: Douwe J. Spaanderman
+Author: Biomedical Imaging Group Rotterdam (BIGR)
 Author-email: d.spaanderman@erasmusmc.nl
-License: APACHE 2.0
-Download-URL: https://github.com/Douwe-Spaanderman/InteractiveNet/archive/refs/tags/v0.1.0.tar.gz
+License: Apache License, Version 2.0
+Download-URL: https://github.com/Douwe-Spaanderman/InteractiveNet/archive/refs/tags/v0.2.0.tar.gz
 Description: UNKNOWN
 Keywords: deep learning,medical image analysis,interactive segmentation,medical image segmentation,soft-tissue tumors,interactivenet
 Platform: UNKNOWN
 Requires-Python: >3.9.0
```

### Comparing `interactivenet-0.1.0/README.md` & `interactivenet-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # InteractiveNet
 
  PyPi                          |Citing InteractiveNet          |
 -------------------------------|---------------------|
 [![][pypi]][pypi-lnk]         | [![][DOI]][DOI-lnk] |
 
-[pypi]: https://badge.fury.io/py/WORC.svg
-[pypi-lnk]: https://badge.fury.io/py/WORC
+[pypi]: https://badge.fury.io/py/interactivenet.svg
+[pypi-lnk]: https://badge.fury.io/py/interactivenet
 
 [DOI]: https://zenodo.org/badge/469761094.svg
 [DOI-lnk]: https://zenodo.org/badge/latestdoi/469761094
 
 Automatic segmentation has success in a variety of application throughout medical imaging. However, there could be a couple of reasons for automatic segmentation to fall short of providing accurate segmentations:
 - Object are irregular and/or lobulated, which creates difficult segmentation task.
 - It is impossible to encompass all heterogeneity from the patient population in a training dataset.
@@ -31,15 +31,15 @@
     - [Testing](#Testing)
     - [Inference](#Inference)
 - [Deploy](#Deploy)
 - [Pretrained model](#Pretrained-model)
 - [Graphical User Interface](#Graphical-User-Interface)
 
 ## License
-This package is covered by the open source [APACHE 2.0 License](LICENSE.md).
+This package is covered by the open source [APACHE 2.0 License](LICENSE).
 
 When using InteractiveNet, please cite the paper describing InteractiveNet as as follows:
 
 ```bibtex
 @article{spaanderman2023softtissuesegmentation,
    title={Minimally Interactive Segmentation of Soft-Tissue Tumors on CT and MRI using Deep Learning}, 
    author={Douwe J. Spaanderman, Martijn P. A. Starmans, Gonnie C. M. van Erp, David F. Hanff, Judith Sluijter, Anne-Rose W. Schut, Geert J. L. H. van Leenders, Cornelis Verhoef, Dirk J. Grünhagen, Wiro J. Niessen, Jacob J. Visser, and Stefan Klein},
@@ -171,15 +171,22 @@
 
 A new folder will be made in the specified ```interactivenet_results``` folder named according to the TaskXXX_YOURTASK, which includes everything needed to run the pipeline. You can share this folder with whoever you like and they will be able to run your trained models!
 
 In order to run your deployed models, simply use ```interactive_inference``` as described above.
 
 # Pretrained model
 
-Due to the blinded nature of journal reviewing process, we cannot currently share the pretrained models, as they are on our institute gdrive, however we will do so when the paper is accepted. 
+Pretrained models can be found [here](https://zenodo.org/record/8054038). All available can also be printed using ```interactivenet_available_models```. 
+
+In order to download and install pretrained models you can use the following provided command:
+```
+interactivenet_download_model -t TaskXXX_YOURTASK
+```
+
+```-t``` or ```--task``` defines the model which will be download. All available models can be found as described above or by checking the options under ```-h``` or ```--help```. In order to run pretrained models, simply use ```interactive_inference``` as described above. 
 
 # Graphical User Interface
 
 We have implemented the interactive segmentation pipeline in [monailabel](https://github.com/Project-MONAI/MONAILabel). Therefore, you can directly use interactivenet in 3D slicer/OHIF vierwer. This will allow you to load in samples, make interactions, and run the pretrained segmentation pipeline. Deployed models, as described above, can be used in the Graphical User Interface (GUI). Checkout the [Graphical User Interface](GUI) for more information, and see below for an example of interactivenet in 3D slicer.
 
 ![GUI_example](GUI_example.png)
```

### Comparing `interactivenet-0.1.0/documentation/dataset_conversion.md` & `interactivenet-0.2.0/documentation/dataset_conversion.md`

 * *Files identical despite different names*

### Comparing `interactivenet-0.1.0/documentation/env_variables.md` & `interactivenet-0.2.0/documentation/env_variables.md`

 * *Files identical despite different names*

### Comparing `interactivenet-0.1.0/documentation/synthetic_interactions.md` & `interactivenet-0.2.0/documentation/synthetic_interactions.md`

 * *Files identical despite different names*

### Comparing `interactivenet-0.1.0/interactivenet/experiment_planning/fingerprinting.py` & `interactivenet-0.2.0/interactivenet/experiment_planning/fingerprinting.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+#   Copyright 2023 Biomedical Imaging Group Rotterdam, Departments of
+#   Radiology and Nuclear Medicine, Erasmus MC, Rotterdam, The Netherlands
+#
+#   Licensed under the Apache License, Version 2.0 (the "License");
+#   you may not use this file except in compliance with the License.
+#   You may obtain a copy of the License at
+#   
+#   http://www.apache.org/licenses/LICENSE-2.0
+
+#   Unless required by applicable law or agreed to in writing, software
+#   distributed under the License is distributed on an "AS IS" BASIS,
+#   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#   See the License for the specific language governing permissions and
+#   limitations under the License.
+
 from typing import List, Dict, Tuple, Union
 from pathlib import Path
 import math
 import random
 import json
 
 import argparse
```

### Comparing `interactivenet-0.1.0/interactivenet/experiment_planning/generate_dataset_json.py` & `interactivenet-0.2.0/interactivenet/experiment_planning/generate_dataset_json.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+#   Copyright 2023 Biomedical Imaging Group Rotterdam, Departments of
+#   Radiology and Nuclear Medicine, Erasmus MC, Rotterdam, The Netherlands
+#
+#   Licensed under the Apache License, Version 2.0 (the "License");
+#   you may not use this file except in compliance with the License.
+#   You may obtain a copy of the License at
+#   
+#   http://www.apache.org/licenses/LICENSE-2.0
+
+#   Unless required by applicable law or agreed to in writing, software
+#   distributed under the License is distributed on an "AS IS" BASIS,
+#   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#   See the License for the specific language governing permissions and
+#   limitations under the License.
+
 import os
 import json
 import argparse
 import numpy as np
 import warnings
 from pathlib import Path
 import SimpleITK as sitk
```

### Comparing `interactivenet-0.1.0/interactivenet/experiment_planning/mimic_annotations.py` & `interactivenet-0.2.0/interactivenet/experiment_planning/mimic_annotations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+#   Copyright 2023 Biomedical Imaging Group Rotterdam, Departments of
+#   Radiology and Nuclear Medicine, Erasmus MC, Rotterdam, The Netherlands
+#
+#   Licensed under the Apache License, Version 2.0 (the "License");
+#   you may not use this file except in compliance with the License.
+#   You may obtain a copy of the License at
+#   
+#   http://www.apache.org/licenses/LICENSE-2.0
+
+#   Unless required by applicable law or agreed to in writing, software
+#   distributed under the License is distributed on an "AS IS" BASIS,
+#   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#   See the License for the specific language governing permissions and
+#   limitations under the License.
+
 import os
 import random
 import warnings
 import json
 import argparse
 import SimpleITK as sitk
 import numpy as np
```

### Comparing `interactivenet-0.1.0/interactivenet/experiment_planning/preprocessing.py` & `interactivenet-0.2.0/interactivenet/experiment_planning/preprocessing.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+#   Copyright 2023 Biomedical Imaging Group Rotterdam, Departments of
+#   Radiology and Nuclear Medicine, Erasmus MC, Rotterdam, The Netherlands
+#
+#   Licensed under the Apache License, Version 2.0 (the "License");
+#   you may not use this file except in compliance with the License.
+#   You may obtain a copy of the License at
+#   
+#   http://www.apache.org/licenses/LICENSE-2.0
+
+#   Unless required by applicable law or agreed to in writing, software
+#   distributed under the License is distributed on an "AS IS" BASIS,
+#   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#   See the License for the specific language governing permissions and
+#   limitations under the License.
+
 from typing import List, Tuple, Dict, Union
 from pathlib import Path
 import pickle
 
 import numpy as np
 import os
 import argparse
```

### Comparing `interactivenet-0.1.0/interactivenet/networks/unet.py` & `interactivenet-0.2.0/interactivenet/networks/unet.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+#   Copyright 2023 Biomedical Imaging Group Rotterdam, Departments of
+#   Radiology and Nuclear Medicine, Erasmus MC, Rotterdam, The Netherlands
+#
+#   Licensed under the Apache License, Version 2.0 (the "License");
+#   you may not use this file except in compliance with the License.
+#   You may obtain a copy of the License at
+#   
+#   http://www.apache.org/licenses/LICENSE-2.0
+
+#   Unless required by applicable law or agreed to in writing, software
+#   distributed under the License is distributed on an "AS IS" BASIS,
+#   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#   See the License for the specific language governing permissions and
+#   limitations under the License.
+
 import warnings
 from typing import Optional, Sequence, Union
 
 import torch
 import torch.nn as nn
```

### Comparing `interactivenet-0.1.0/interactivenet/test/ensemble.py` & `interactivenet-0.2.0/interactivenet/test/ensemble.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+#   Copyright 2023 Biomedical Imaging Group Rotterdam, Departments of
+#   Radiology and Nuclear Medicine, Erasmus MC, Rotterdam, The Netherlands
+#
+#   Licensed under the Apache License, Version 2.0 (the "License");
+#   you may not use this file except in compliance with the License.
+#   You may obtain a copy of the License at
+#   
+#   http://www.apache.org/licenses/LICENSE-2.0
+
+#   Unless required by applicable law or agreed to in writing, software
+#   distributed under the License is distributed on an "AS IS" BASIS,
+#   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#   See the License for the specific language governing permissions and
+#   limitations under the License.
+
 import argparse
 
 import os
 from typing import List, Dict, Optional, Union
 
 from pathlib import Path
 import argparse
```

### Comparing `interactivenet-0.1.0/interactivenet/test/inference.py` & `interactivenet-0.2.0/interactivenet/test/inference.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+#   Copyright 2023 Biomedical Imaging Group Rotterdam, Departments of
+#   Radiology and Nuclear Medicine, Erasmus MC, Rotterdam, The Netherlands
+#
+#   Licensed under the Apache License, Version 2.0 (the "License");
+#   you may not use this file except in compliance with the License.
+#   You may obtain a copy of the License at
+#   
+#   http://www.apache.org/licenses/LICENSE-2.0
+
+#   Unless required by applicable law or agreed to in writing, software
+#   distributed under the License is distributed on an "AS IS" BASIS,
+#   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#   See the License for the specific language governing permissions and
+#   limitations under the License.
+
 from pathlib import Path
 import argparse
 import os
 from typing import List, Dict, Optional, Union
 import numpy as np
 import torch
 from collections import Counter
```

### Comparing `interactivenet-0.1.0/interactivenet/test/predict.py` & `interactivenet-0.2.0/interactivenet/test/predict.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+#   Copyright 2023 Biomedical Imaging Group Rotterdam, Departments of
+#   Radiology and Nuclear Medicine, Erasmus MC, Rotterdam, The Netherlands
+#
+#   Licensed under the Apache License, Version 2.0 (the "License");
+#   you may not use this file except in compliance with the License.
+#   You may obtain a copy of the License at
+#   
+#   http://www.apache.org/licenses/LICENSE-2.0
+
+#   Unless required by applicable law or agreed to in writing, software
+#   distributed under the License is distributed on an "AS IS" BASIS,
+#   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#   See the License for the specific language governing permissions and
+#   limitations under the License.
+
 import argparse
 
 import os
 from typing import List, Dict, Optional, Union
 
 from pathlib import Path
```

### Comparing `interactivenet-0.1.0/interactivenet/test/refinement.py` & `interactivenet-0.2.0/interactivenet/test/refinement.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+#   Copyright 2023 Biomedical Imaging Group Rotterdam, Departments of
+#   Radiology and Nuclear Medicine, Erasmus MC, Rotterdam, The Netherlands
+#
+#   Licensed under the Apache License, Version 2.0 (the "License");
+#   you may not use this file except in compliance with the License.
+#   You may obtain a copy of the License at
+#   
+#   http://www.apache.org/licenses/LICENSE-2.0
+
+#   Unless required by applicable law or agreed to in writing, software
+#   distributed under the License is distributed on an "AS IS" BASIS,
+#   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#   See the License for the specific language governing permissions and
+#   limitations under the License.
+
 ##################################
 ##################################
 ## ALL CODE HERE IS OUTDATED!!! ##
 ##################################
 ##################################
 ##################################
```

### Comparing `interactivenet-0.1.0/interactivenet/training/postprocessing.py` & `interactivenet-0.2.0/interactivenet/training/postprocessing.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+#   Copyright 2023 Biomedical Imaging Group Rotterdam, Departments of
+#   Radiology and Nuclear Medicine, Erasmus MC, Rotterdam, The Netherlands
+#
+#   Licensed under the Apache License, Version 2.0 (the "License");
+#   you may not use this file except in compliance with the License.
+#   You may obtain a copy of the License at
+#   
+#   http://www.apache.org/licenses/LICENSE-2.0
+
+#   Unless required by applicable law or agreed to in writing, software
+#   distributed under the License is distributed on an "AS IS" BASIS,
+#   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#   See the License for the specific language governing permissions and
+#   limitations under the License.
+
 from typing import List, Dict, Optional, Union
 
 from pathlib import Path
 import numpy as np
 import os
 import argparse
```

### Comparing `interactivenet-0.1.0/interactivenet/training/run.py` & `interactivenet-0.2.0/interactivenet/training/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+#   Copyright 2023 Biomedical Imaging Group Rotterdam, Departments of
+#   Radiology and Nuclear Medicine, Erasmus MC, Rotterdam, The Netherlands
+#
+#   Licensed under the Apache License, Version 2.0 (the "License");
+#   you may not use this file except in compliance with the License.
+#   You may obtain a copy of the License at
+#   
+#   http://www.apache.org/licenses/LICENSE-2.0
+
+#   Unless required by applicable law or agreed to in writing, software
+#   distributed under the License is distributed on an "AS IS" BASIS,
+#   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#   See the License for the specific language governing permissions and
+#   limitations under the License.
+
 from typing import List, Dict
 
 from pathlib import Path
 import os
 import argparse
 
 from monai.utils import set_determinism
```

### Comparing `interactivenet-0.1.0/interactivenet/transforms/set_transforms.py` & `interactivenet-0.2.0/interactivenet/transforms/set_transforms.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+#   Copyright 2023 Biomedical Imaging Group Rotterdam, Departments of
+#   Radiology and Nuclear Medicine, Erasmus MC, Rotterdam, The Netherlands
+#
+#   Licensed under the Apache License, Version 2.0 (the "License");
+#   you may not use this file except in compliance with the License.
+#   You may obtain a copy of the License at
+#   
+#   http://www.apache.org/licenses/LICENSE-2.0
+
+#   Unless required by applicable law or agreed to in writing, software
+#   distributed under the License is distributed on an "AS IS" BASIS,
+#   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#   See the License for the specific language governing permissions and
+#   limitations under the License.
+
 import os
 from typing import List, Tuple, Optional, Union
 
 import numpy as np
 from monai.utils import set_determinism
 from monai.transforms import (
     Compose,
```

### Comparing `interactivenet-0.1.0/interactivenet/transforms/transforms.py` & `interactivenet-0.2.0/interactivenet/transforms/transforms.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+#   Copyright 2023 Biomedical Imaging Group Rotterdam, Departments of
+#   Radiology and Nuclear Medicine, Erasmus MC, Rotterdam, The Netherlands
+#
+#   Licensed under the Apache License, Version 2.0 (the "License");
+#   you may not use this file except in compliance with the License.
+#   You may obtain a copy of the License at
+#   
+#   http://www.apache.org/licenses/LICENSE-2.0
+
+#   Unless required by applicable law or agreed to in writing, software
+#   distributed under the License is distributed on an "AS IS" BASIS,
+#   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#   See the License for the specific language governing permissions and
+#   limitations under the License.
+
 from typing import Optional, Union, Dict, List, Tuple
 import os
 
 import warnings
 import pickle
 import math
 from pathlib import Path
```

### Comparing `interactivenet-0.1.0/interactivenet/utils/mlflow.py` & `interactivenet-0.2.0/interactivenet/utils/mlflow.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+#   Copyright 2023 Biomedical Imaging Group Rotterdam, Departments of
+#   Radiology and Nuclear Medicine, Erasmus MC, Rotterdam, The Netherlands
+#
+#   Licensed under the Apache License, Version 2.0 (the "License");
+#   you may not use this file except in compliance with the License.
+#   You may obtain a copy of the License at
+#   
+#   http://www.apache.org/licenses/LICENSE-2.0
+
+#   Unless required by applicable law or agreed to in writing, software
+#   distributed under the License is distributed on an "AS IS" BASIS,
+#   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#   See the License for the specific language governing permissions and
+#   limitations under the License.
+
 import mlflow
 import os
 from pathlib import Path
 
 
 def mlflow_get_runs(name):
     results = Path(os.environ["interactivenet_results"], "mlruns")
```

### Comparing `interactivenet-0.1.0/interactivenet/utils/resample.py` & `interactivenet-0.2.0/interactivenet/utils/resample.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+#   Copyright 2023 Biomedical Imaging Group Rotterdam, Departments of
+#   Radiology and Nuclear Medicine, Erasmus MC, Rotterdam, The Netherlands
+#
+#   Licensed under the Apache License, Version 2.0 (the "License");
+#   you may not use this file except in compliance with the License.
+#   You may obtain a copy of the License at
+#   
+#   http://www.apache.org/licenses/LICENSE-2.0
+
+#   Unless required by applicable law or agreed to in writing, software
+#   distributed under the License is distributed on an "AS IS" BASIS,
+#   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#   See the License for the specific language governing permissions and
+#   limitations under the License.
+
 from typing import List, Union
 import numpy as np
 import torch
 
 from skimage.transform import resize
 from nibabel import affines
 import numpy.linalg as npl
```

### Comparing `interactivenet-0.1.0/interactivenet/utils/results.py` & `interactivenet-0.2.0/interactivenet/utils/results.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+#   Copyright 2023 Biomedical Imaging Group Rotterdam, Departments of
+#   Radiology and Nuclear Medicine, Erasmus MC, Rotterdam, The Netherlands
+#
+#   Licensed under the Apache License, Version 2.0 (the "License");
+#   you may not use this file except in compliance with the License.
+#   You may obtain a copy of the License at
+#   
+#   http://www.apache.org/licenses/LICENSE-2.0
+
+#   Unless required by applicable law or agreed to in writing, software
+#   distributed under the License is distributed on an "AS IS" BASIS,
+#   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#   See the License for the specific language governing permissions and
+#   limitations under the License.
+
 from pathlib import Path
 import numpy as np
 import matplotlib.pyplot as plt
 
 from monai.transforms import AsDiscrete
 
 from interactivenet.utils.visualize import ImagePlot
```

### Comparing `interactivenet-0.1.0/interactivenet/utils/statistics.py` & `interactivenet-0.2.0/interactivenet/utils/statistics.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+#   Copyright 2023 Biomedical Imaging Group Rotterdam, Departments of
+#   Radiology and Nuclear Medicine, Erasmus MC, Rotterdam, The Netherlands
+#
+#   Licensed under the Apache License, Version 2.0 (the "License");
+#   you may not use this file except in compliance with the License.
+#   You may obtain a copy of the License at
+#   
+#   http://www.apache.org/licenses/LICENSE-2.0
+
+#   Unless required by applicable law or agreed to in writing, software
+#   distributed under the License is distributed on an "AS IS" BASIS,
+#   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#   See the License for the specific language governing permissions and
+#   limitations under the License.
+
 from typing import Union, Dict
 
 import pandas as pd
 import numpy as np
 import torch
 
 from monai.metrics import (
```

### Comparing `interactivenet-0.1.0/interactivenet.egg-info/PKG-INFO` & `interactivenet-0.2.0/interactivenet.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 1.2
 Name: interactivenet
-Version: 0.1.0
+Version: 0.2.0
 Summary: InteractiveNet, a framework for minimally interactive medical image segmentation.
 Home-page: https://github.com/Douwe-Spaanderman/InteractiveNet
-Author: Douwe J. Spaanderman
+Author: Biomedical Imaging Group Rotterdam (BIGR)
 Author-email: d.spaanderman@erasmusmc.nl
-License: APACHE 2.0
-Download-URL: https://github.com/Douwe-Spaanderman/InteractiveNet/archive/refs/tags/v0.1.0.tar.gz
+License: Apache License, Version 2.0
+Download-URL: https://github.com/Douwe-Spaanderman/InteractiveNet/archive/refs/tags/v0.2.0.tar.gz
 Description: UNKNOWN
 Keywords: deep learning,medical image analysis,interactive segmentation,medical image segmentation,soft-tissue tumors,interactivenet
 Platform: UNKNOWN
 Requires-Python: >3.9.0
```

### Comparing `interactivenet-0.1.0/interactivenet.egg-info/SOURCES.txt` & `interactivenet-0.2.0/interactivenet.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .gitignore
-LICENSE.md
+LICENSE
 README.md
 setup.cfg
 setup.py
 documentation/dataset_conversion.md
 documentation/env_variables.md
 documentation/synthetic_interactions.md
 interactivenet/__init__.py
@@ -11,15 +11,14 @@
 interactivenet.egg-info/SOURCES.txt
 interactivenet.egg-info/dependency_links.txt
 interactivenet.egg-info/entry_points.txt
 interactivenet.egg-info/requires.txt
 interactivenet.egg-info/top_level.txt
 interactivenet/deploy/__init__.py
 interactivenet/deploy/download_model.py
-interactivenet/deploy/print_models.py
 interactivenet/deploy/save_model.py
 interactivenet/experiment_planning/__init__.py
 interactivenet/experiment_planning/fingerprinting.py
 interactivenet/experiment_planning/generate_dataset_json.py
 interactivenet/experiment_planning/mimic_annotations.py
 interactivenet/experiment_planning/plan_and_process.py
 interactivenet/experiment_planning/preprocessing.py
```

### Comparing `interactivenet-0.1.0/interactivenet.egg-info/entry_points.txt` & `interactivenet-0.2.0/interactivenet.egg-info/entry_points.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [console_scripts]
-interactivenet_available_models = interactivenet.deploy.print_models:main
+interactivenet_available_models = interactivenet.deploy.download_model:print_available_pretrained_models
 interactivenet_deploy = interactivenet.deploy.save_model:main
-interactivenet_download_model = interactivenet.deploy.download_model:main
+interactivenet_download_model = interactivenet.deploy.download_model:download_and_install_model
 interactivenet_ensemble = interactivenet.test.ensemble:main
 interactivenet_fingerprinting = interactivenet.experiment_planning.fingerprinting:main
 interactivenet_generate_dataset_json = interactivenet.experiment_planning.generate_dataset_json:main
 interactivenet_inference = interactivenet.test.inference:main
 interactivenet_mimic_interactions = interactivenet.experiment_planning.mimic_annotations:main
 interactivenet_plan_and_process = interactivenet.experiment_planning.plan_and_process:main
 interactivenet_postprocessing = interactivenet.training.postprocessing:main
```

### Comparing `interactivenet-0.1.0/setup.py` & `interactivenet-0.2.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 from setuptools import setup, find_packages
 
+#with open('README.rst', 'r') as fh:
+#    _description = fh.read()
+
 setup(
     name='interactivenet',
-    version='0.1.0',
-    author = 'Douwe J. Spaanderman',
-    license='APACHE 2.0',
+    version='0.2.0',
+    author = 'Biomedical Imaging Group Rotterdam (BIGR)',
+    license='Apache License, Version 2.0',
     author_email='d.spaanderman@erasmusmc.nl',
     description='InteractiveNet, a framework for minimally interactive medical image segmentation.',
+    #long_description=_description,
     url='https://github.com/Douwe-Spaanderman/InteractiveNet',
-    download_url = 'https://github.com/Douwe-Spaanderman/InteractiveNet/archive/refs/tags/v0.1.0.tar.gz',
+    download_url = 'https://github.com/Douwe-Spaanderman/InteractiveNet/archive/refs/tags/v0.2.0.tar.gz',
     packages=find_packages(include=['interactivenet', 'interactivenet.*']),
     python_requires='>3.9.0',
     install_requires=[
         "SimpleITK>=2.1.1.2",
         "GeodisTK>=0.1.7",
         "matplotlib>=3.5.1",
         "mlflow>=1.24.0",
@@ -39,16 +43,16 @@
             'interactivenet_train=interactivenet.training.run:main',
             'interactivenet_postprocessing=interactivenet.training.postprocessing:main',
             'interactivenet_ensemble=interactivenet.test.ensemble:main',
             'interactivenet_inference=interactivenet.test.inference:main',
             'interactivenet_predict=interactivenet.test.predict:main',
             'interactivenet_test=interactivenet.test.run:main',
             'interactivenet_deploy=interactivenet.deploy.save_model:main',
-            'interactivenet_available_models=interactivenet.deploy.print_models:main',
-            'interactivenet_download_model=interactivenet.deploy.download_model:main',
+            'interactivenet_available_models=interactivenet.deploy.download_model:print_available_pretrained_models',
+            'interactivenet_download_model=interactivenet.deploy.download_model:download_and_install_model',
             ]
     },
     keywords=[
         "deep learning",
         "medical image analysis",
         "interactive segmentation",
         "medical image segmentation",
```

