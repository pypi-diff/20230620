# Comparing `tmp/hamzaGlyph-0.1.tar.gz` & `tmp/hamzaGlyph-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\hamzaGlyph-0.1.tar", last modified: Wed May  3 20:44:35 2023, max compression
+gzip compressed data, was "dist\hamzaGlyph-1.1.0.tar", last modified: Tue Jun 20 15:22:30 2023, max compression
```

## Comparing `hamzaGlyph-0.1.tar` & `hamzaGlyph-1.1.0.tar`

### file list

```diff
@@ -1,9 +1,58 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 20:44:35.971456 hamzaGlyph-0.1/
--rw-rw-rw-   0        0        0      571 2023-05-03 20:44:35.970453 hamzaGlyph-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-03 20:44:35.968461 hamzaGlyph-0.1/hamzaGlyph.egg-info/
--rw-rw-rw-   0        0        0      571 2023-05-03 20:44:35.000000 hamzaGlyph-0.1/hamzaGlyph.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      144 2023-05-03 20:44:35.000000 hamzaGlyph-0.1/hamzaGlyph.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 20:44:35.000000 hamzaGlyph-0.1/hamzaGlyph.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 20:44:35.000000 hamzaGlyph-0.1/hamzaGlyph.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 20:44:35.972449 hamzaGlyph-0.1/setup.cfg
--rw-rw-rw-   0        0        0      716 2023-05-03 20:43:36.000000 hamzaGlyph-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:22:30.072409 hamzaGlyph-1.1.0/
+-rw-rw-rw-   0        0        0    34523 2023-04-16 00:29:34.000000 hamzaGlyph-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0      182 2023-06-20 15:22:30.072409 hamzaGlyph-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    39776 2023-04-16 00:29:34.000000 hamzaGlyph-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 15:22:29.991521 hamzaGlyph-1.1.0/hamzaGlyph.egg-info/
+-rw-rw-rw-   0        0        0      182 2023-06-20 15:22:29.000000 hamzaGlyph-1.1.0/hamzaGlyph.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1089 2023-06-20 15:22:29.000000 hamzaGlyph-1.1.0/hamzaGlyph.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 15:22:29.000000 hamzaGlyph-1.1.0/hamzaGlyph.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-20 15:22:29.000000 hamzaGlyph-1.1.0/hamzaGlyph.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-20 15:22:29.000000 hamzaGlyph-1.1.0/hamzaGlyph.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 15:22:30.001876 hamzaGlyph-1.1.0/models/
+-rw-rw-rw-   0        0        0        0 2023-04-16 00:29:34.000000 hamzaGlyph-1.1.0/models/__init__.py
+-rw-rw-rw-   0        0        0    41703 2023-04-16 00:29:34.000000 hamzaGlyph-1.1.0/models/common.py
+-rw-rw-rw-   0        0        0     4320 2023-04-16 00:29:34.000000 hamzaGlyph-1.1.0/models/experimental.py
+-rw-rw-rw-   0        0        0    27019 2023-04-16 00:29:34.000000 hamzaGlyph-1.1.0/models/tf.py
+-rw-rw-rw-   0        0        0    17767 2023-04-16 00:29:34.000000 hamzaGlyph-1.1.0/models/yolo.py
+-rw-rw-rw-   0        0        0      743 2023-06-20 15:22:30.075534 hamzaGlyph-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      389 2023-06-20 15:18:41.000000 hamzaGlyph-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:22:30.037091 hamzaGlyph-1.1.0/utils/
+-rw-rw-rw-   0        0        0     2433 2023-04-16 00:29:34.000000 hamzaGlyph-1.1.0/utils/__init__.py
+-rw-rw-rw-   0        0        0     3450 2023-04-16 00:29:34.000000 hamzaGlyph-1.1.0/utils/activations.py
+-rw-rw-rw-   0        0        0    17031 2023-04-16 00:29:34.000000 hamzaGlyph-1.1.0/utils/augmentations.py
+-rw-rw-rw-   0        0        0     7421 2023-04-16 00:29:34.000000 hamzaGlyph-1.1.0/utils/autoanchor.py
+-rw-rw-rw-   0        0        0     2990 2023-04-16 00:29:34.000000 hamzaGlyph-1.1.0/utils/autobatch.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:22:30.040086 hamzaGlyph-1.1.0/utils/aws/
+-rw-rw-rw-   0        0        0        0 2023-04-16 00:29:34.000000 hamzaGlyph-1.1.0/utils/aws/__init__.py
+-rw-rw-rw-   0        0        0     1198 2023-04-16 00:29:34.000000 hamzaGlyph-1.1.0/utils/aws/resume.py
+-rw-rw-rw-   0        0        0     2662 2023-04-16 00:29:34.000000 hamzaGlyph-1.1.0/utils/callbacks.py
+-rw-rw-rw-   0        0        0    55810 2023-04-16 00:29:34.000000 hamzaGlyph-1.1.0/utils/dataloaders.py
+-rw-rw-rw-   0        0        0    16998 2023-04-22 23:51:30.000000 hamzaGlyph-1.1.0/utils/detectBeforeCar.py
+-rw-rw-rw-   0        0        0     4957 2023-04-16 00:29:34.000000 hamzaGlyph-1.1.0/utils/downloads.py
+-rw-rw-rw-   0        0        0    47788 2023-04-16 00:29:34.000000 hamzaGlyph-1.1.0/utils/general.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:22:30.042104 hamzaGlyph-1.1.0/utils/loggers/
+-rw-rw-rw-   0        0        0    16734 2023-04-16 00:29:34.000000 hamzaGlyph-1.1.0/utils/loggers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:22:30.047070 hamzaGlyph-1.1.0/utils/loggers/clearml/
+-rw-rw-rw-   0        0        0        0 2023-04-16 00:29:34.000000 hamzaGlyph-1.1.0/utils/loggers/clearml/__init__.py
+-rw-rw-rw-   0        0        0     8034 2023-04-16 00:29:34.000000 hamzaGlyph-1.1.0/utils/loggers/clearml/clearml_utils.py
+-rw-rw-rw-   0        0        0     5271 2023-04-16 00:29:34.000000 hamzaGlyph-1.1.0/utils/loggers/clearml/hpo.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:22:30.054070 hamzaGlyph-1.1.0/utils/loggers/comet/
+-rw-rw-rw-   0        0        0    18731 2023-04-16 00:29:34.000000 hamzaGlyph-1.1.0/utils/loggers/comet/__init__.py
+-rw-rw-rw-   0        0        0     4751 2023-04-16 00:29:34.000000 hamzaGlyph-1.1.0/utils/loggers/comet/comet_utils.py
+-rw-rw-rw-   0        0        0     6653 2023-04-16 00:29:34.000000 hamzaGlyph-1.1.0/utils/loggers/comet/hpo.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:22:30.057064 hamzaGlyph-1.1.0/utils/loggers/wandb/
+-rw-rw-rw-   0        0        0        0 2023-04-16 00:29:34.000000 hamzaGlyph-1.1.0/utils/loggers/wandb/__init__.py
+-rw-rw-rw-   0        0        0     8253 2023-04-16 00:29:34.000000 hamzaGlyph-1.1.0/utils/loggers/wandb/wandb_utils.py
+-rw-rw-rw-   0        0        0     9920 2023-04-16 00:29:34.000000 hamzaGlyph-1.1.0/utils/loss.py
+-rw-rw-rw-   0        0        0    14569 2023-04-16 00:29:34.000000 hamzaGlyph-1.1.0/utils/metrics.py
+-rw-rw-rw-   0        0        0    24488 2023-04-16 00:29:34.000000 hamzaGlyph-1.1.0/utils/plots.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:22:30.071420 hamzaGlyph-1.1.0/utils/segment/
+-rw-rw-rw-   0        0        0        0 2023-04-16 00:29:34.000000 hamzaGlyph-1.1.0/utils/segment/__init__.py
+-rw-rw-rw-   0        0        0     3757 2023-04-16 00:29:34.000000 hamzaGlyph-1.1.0/utils/segment/augmentations.py
+-rw-rw-rw-   0        0        0    13836 2023-04-16 00:29:34.000000 hamzaGlyph-1.1.0/utils/segment/dataloaders.py
+-rw-rw-rw-   0        0        0     5813 2023-04-16 00:29:34.000000 hamzaGlyph-1.1.0/utils/segment/general.py
+-rw-rw-rw-   0        0        0     8591 2023-04-16 00:29:34.000000 hamzaGlyph-1.1.0/utils/segment/loss.py
+-rw-rw-rw-   0        0        0     5458 2023-04-16 00:29:34.000000 hamzaGlyph-1.1.0/utils/segment/metrics.py
+-rw-rw-rw-   0        0        0     6386 2023-04-16 00:29:34.000000 hamzaGlyph-1.1.0/utils/segment/plots.py
+-rw-rw-rw-   0        0        0    19642 2023-04-16 00:29:34.000000 hamzaGlyph-1.1.0/utils/torch_utils.py
+-rw-rw-rw-   0        0        0     3635 2023-04-16 00:29:34.000000 hamzaGlyph-1.1.0/utils/triton.py
```

