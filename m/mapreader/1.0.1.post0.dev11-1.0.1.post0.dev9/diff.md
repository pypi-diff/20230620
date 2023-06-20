# Comparing `tmp/mapreader-1.0.1.post0.dev11.tar.gz` & `tmp/mapreader-1.0.1.post0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapreader-1.0.1.post0.dev11.tar", last modified: Tue Jun 20 19:27:18 2023, max compression
+gzip compressed data, was "mapreader-1.0.1.post0.dev9.tar", last modified: Wed Jun  7 12:38:11 2023, max compression
```

## Comparing `mapreader-1.0.1.post0.dev11.tar` & `mapreader-1.0.1.post0.dev9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:27:18.197604 mapreader-1.0.1.post0.dev11/
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-20 19:27:01.000000 mapreader-1.0.1.post0.dev11/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-06-20 19:27:18.197604 mapreader-1.0.1.post0.dev11/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-06-20 19:27:01.000000 mapreader-1.0.1.post0.dev11/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:27:18.201604 mapreader-1.0.1.post0.dev11/mapreader/
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-20 19:27:01.000000 mapreader-1.0.1.post0.dev11/mapreader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-20 19:27:18.201604 mapreader-1.0.1.post0.dev11/mapreader/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:27:18.193603 mapreader-1.0.1.post0.dev11/mapreader/annotate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 19:27:01.000000 mapreader-1.0.1.post0.dev11/mapreader/annotate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24794 2023-06-20 19:27:01.000000 mapreader-1.0.1.post0.dev11/mapreader/annotate/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:27:18.197604 mapreader-1.0.1.post0.dev11/mapreader/classify/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 19:27:01.000000 mapreader-1.0.1.post0.dev11/mapreader/classify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    73307 2023-06-20 19:27:01.000000 mapreader-1.0.1.post0.dev11/mapreader/classify/classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    27268 2023-06-20 19:27:01.000000 mapreader-1.0.1.post0.dev11/mapreader/classify/classifier_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-06-20 19:27:01.000000 mapreader-1.0.1.post0.dev11/mapreader/classify/custom_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    28572 2023-06-20 19:27:01.000000 mapreader-1.0.1.post0.dev11/mapreader/classify/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    25048 2023-06-20 19:27:01.000000 mapreader-1.0.1.post0.dev11/mapreader/classify/load_annotations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:27:18.197604 mapreader-1.0.1.post0.dev11/mapreader/download/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 19:27:01.000000 mapreader-1.0.1.post0.dev11/mapreader/download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-06-20 19:27:01.000000 mapreader-1.0.1.post0.dev11/mapreader/download/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-06-20 19:27:01.000000 mapreader-1.0.1.post0.dev11/mapreader/download/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-06-20 19:27:01.000000 mapreader-1.0.1.post0.dev11/mapreader/download/downloader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    38174 2023-06-20 19:27:01.000000 mapreader-1.0.1.post0.dev11/mapreader/download/sheet_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-06-20 19:27:01.000000 mapreader-1.0.1.post0.dev11/mapreader/download/tile_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-06-20 19:27:01.000000 mapreader-1.0.1.post0.dev11/mapreader/download/tile_merging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:27:18.197604 mapreader-1.0.1.post0.dev11/mapreader/load/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-20 19:27:01.000000 mapreader-1.0.1.post0.dev11/mapreader/load/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-06-20 19:27:01.000000 mapreader-1.0.1.post0.dev11/mapreader/load/geo_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    86859 2023-06-20 19:27:01.000000 mapreader-1.0.1.post0.dev11/mapreader/load/images.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-06-20 19:27:01.000000 mapreader-1.0.1.post0.dev11/mapreader/load/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:27:18.197604 mapreader-1.0.1.post0.dev11/mapreader/process/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 19:27:01.000000 mapreader-1.0.1.post0.dev11/mapreader/process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-06-20 19:27:01.000000 mapreader-1.0.1.post0.dev11/mapreader/process/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:27:18.197604 mapreader-1.0.1.post0.dev11/mapreader/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 19:27:01.000000 mapreader-1.0.1.post0.dev11/mapreader/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-20 19:27:01.000000 mapreader-1.0.1.post0.dev11/mapreader/utils/compute_and_save_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-20 19:27:01.000000 mapreader-1.0.1.post0.dev11/mapreader/utils/slice_parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:27:18.193603 mapreader-1.0.1.post0.dev11/mapreader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-06-20 19:27:18.000000 mapreader-1.0.1.post0.dev11/mapreader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-20 19:27:18.000000 mapreader-1.0.1.post0.dev11/mapreader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 19:27:18.000000 mapreader-1.0.1.post0.dev11/mapreader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-20 19:27:18.000000 mapreader-1.0.1.post0.dev11/mapreader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 19:27:17.000000 mapreader-1.0.1.post0.dev11/mapreader.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-20 19:27:18.000000 mapreader-1.0.1.post0.dev11/mapreader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-20 19:27:18.000000 mapreader-1.0.1.post0.dev11/mapreader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-20 19:27:18.197604 mapreader-1.0.1.post0.dev11/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-06-20 19:27:01.000000 mapreader-1.0.1.post0.dev11/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:27:18.197604 mapreader-1.0.1.post0.dev11/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-06-20 19:27:02.000000 mapreader-1.0.1.post0.dev11/tests/test_annotations_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-06-20 19:27:02.000000 mapreader-1.0.1.post0.dev11/tests/test_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-20 19:27:02.000000 mapreader-1.0.1.post0.dev11/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)    14024 2023-06-20 19:27:02.000000 mapreader-1.0.1.post0.dev11/tests/test_sheet_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-06-20 19:27:02.000000 mapreader-1.0.1.post0.dev11/versioneer.py
+drwxr-xr-x   0 rwood      (504) staff       (20)        0 2023-06-07 12:38:11.913844 mapreader-1.0.1.post0.dev9/
+-rw-r--r--   0 rwood      (504) staff       (20)     1216 2023-03-22 14:17:08.000000 mapreader-1.0.1.post0.dev9/LICENSE
+-rw-r--r--   0 rwood      (504) staff       (20)     7277 2023-06-07 12:38:11.913897 mapreader-1.0.1.post0.dev9/PKG-INFO
+-rw-r--r--   0 rwood      (504) staff       (20)     5949 2023-06-06 16:21:10.000000 mapreader-1.0.1.post0.dev9/README.md
+drwxr-xr-x   0 rwood      (504) staff       (20)        0 2023-06-07 12:38:11.914221 mapreader-1.0.1.post0.dev9/mapreader/
+-rw-r--r--   0 rwood      (504) staff       (20)      867 2023-06-05 15:21:44.000000 mapreader-1.0.1.post0.dev9/mapreader/__init__.py
+-rw-r--r--   0 rwood      (504) staff       (20)      508 2023-06-07 12:38:11.914250 mapreader-1.0.1.post0.dev9/mapreader/_version.py
+drwxr-xr-x   0 rwood      (504) staff       (20)        0 2023-06-07 12:38:11.910724 mapreader-1.0.1.post0.dev9/mapreader/annotate/
+-rw-r--r--   0 rwood      (504) staff       (20)        0 2023-05-24 14:03:30.000000 mapreader-1.0.1.post0.dev9/mapreader/annotate/__init__.py
+-rw-r--r--   0 rwood      (504) staff       (20)    24794 2023-06-05 15:21:44.000000 mapreader-1.0.1.post0.dev9/mapreader/annotate/utils.py
+drwxr-xr-x   0 rwood      (504) staff       (20)        0 2023-06-07 12:38:11.911521 mapreader-1.0.1.post0.dev9/mapreader/classify/
+-rw-r--r--   0 rwood      (504) staff       (20)        0 2023-06-05 15:21:44.000000 mapreader-1.0.1.post0.dev9/mapreader/classify/__init__.py
+-rw-r--r--   0 rwood      (504) staff       (20)    73307 2023-06-05 15:21:44.000000 mapreader-1.0.1.post0.dev9/mapreader/classify/classifier.py
+-rw-r--r--   0 rwood      (504) staff       (20)    27268 2023-06-05 15:21:44.000000 mapreader-1.0.1.post0.dev9/mapreader/classify/classifier_context.py
+-rw-r--r--   0 rwood      (504) staff       (20)     1991 2023-06-05 15:21:44.000000 mapreader-1.0.1.post0.dev9/mapreader/classify/custom_models.py
+-rw-r--r--   0 rwood      (504) staff       (20)    28572 2023-06-05 15:21:44.000000 mapreader-1.0.1.post0.dev9/mapreader/classify/datasets.py
+-rw-r--r--   0 rwood      (504) staff       (20)    25048 2023-06-05 15:21:44.000000 mapreader-1.0.1.post0.dev9/mapreader/classify/load_annotations.py
+drwxr-xr-x   0 rwood      (504) staff       (20)        0 2023-06-07 12:38:11.912334 mapreader-1.0.1.post0.dev9/mapreader/download/
+-rw-r--r--   0 rwood      (504) staff       (20)        0 2023-05-04 15:10:34.000000 mapreader-1.0.1.post0.dev9/mapreader/download/__init__.py
+-rw-r--r--   0 rwood      (504) staff       (20)     2285 2023-05-24 14:03:30.000000 mapreader-1.0.1.post0.dev9/mapreader/download/data_structures.py
+-rw-r--r--   0 rwood      (504) staff       (20)     4564 2023-05-24 14:03:30.000000 mapreader-1.0.1.post0.dev9/mapreader/download/downloader.py
+-rw-r--r--   0 rwood      (504) staff       (20)     4553 2023-05-24 14:03:30.000000 mapreader-1.0.1.post0.dev9/mapreader/download/downloader_utils.py
+-rw-r--r--   0 rwood      (504) staff       (20)    38174 2023-05-24 14:03:30.000000 mapreader-1.0.1.post0.dev9/mapreader/download/sheet_downloader.py
+-rw-r--r--   0 rwood      (504) staff       (20)     6430 2023-05-24 14:03:30.000000 mapreader-1.0.1.post0.dev9/mapreader/download/tile_loading.py
+-rw-r--r--   0 rwood      (504) staff       (20)     5832 2023-05-24 14:03:30.000000 mapreader-1.0.1.post0.dev9/mapreader/download/tile_merging.py
+drwxr-xr-x   0 rwood      (504) staff       (20)        0 2023-06-07 12:38:11.912820 mapreader-1.0.1.post0.dev9/mapreader/load/
+-rw-r--r--   0 rwood      (504) staff       (20)      132 2023-05-24 14:03:30.000000 mapreader-1.0.1.post0.dev9/mapreader/load/__init__.py
+-rw-r--r--   0 rwood      (504) staff       (20)     3676 2023-05-24 14:03:30.000000 mapreader-1.0.1.post0.dev9/mapreader/load/geo_utils.py
+-rw-r--r--   0 rwood      (504) staff       (20)    86859 2023-06-05 15:21:44.000000 mapreader-1.0.1.post0.dev9/mapreader/load/images.py
+-rw-r--r--   0 rwood      (504) staff       (20)     4846 2023-06-05 15:21:44.000000 mapreader-1.0.1.post0.dev9/mapreader/load/loader.py
+drwxr-xr-x   0 rwood      (504) staff       (20)        0 2023-06-07 12:38:11.913008 mapreader-1.0.1.post0.dev9/mapreader/process/
+-rw-r--r--   0 rwood      (504) staff       (20)        0 2023-03-22 14:17:08.000000 mapreader-1.0.1.post0.dev9/mapreader/process/__init__.py
+-rw-r--r--   0 rwood      (504) staff       (20)     7669 2023-05-09 12:50:40.000000 mapreader-1.0.1.post0.dev9/mapreader/process/process.py
+drwxr-xr-x   0 rwood      (504) staff       (20)        0 2023-06-07 12:38:11.913318 mapreader-1.0.1.post0.dev9/mapreader/utils/
+-rw-r--r--   0 rwood      (504) staff       (20)        0 2023-03-22 14:17:08.000000 mapreader-1.0.1.post0.dev9/mapreader/utils/__init__.py
+-rw-r--r--   0 rwood      (504) staff       (20)      967 2023-05-09 12:50:40.000000 mapreader-1.0.1.post0.dev9/mapreader/utils/compute_and_save_stats.py
+-rw-r--r--   0 rwood      (504) staff       (20)     1654 2023-04-25 09:23:09.000000 mapreader-1.0.1.post0.dev9/mapreader/utils/slice_parallel.py
+drwxr-xr-x   0 rwood      (504) staff       (20)        0 2023-06-07 12:38:11.910527 mapreader-1.0.1.post0.dev9/mapreader.egg-info/
+-rw-r--r--   0 rwood      (504) staff       (20)     7277 2023-06-07 12:38:11.000000 mapreader-1.0.1.post0.dev9/mapreader.egg-info/PKG-INFO
+-rw-r--r--   0 rwood      (504) staff       (20)     1224 2023-06-07 12:38:11.000000 mapreader-1.0.1.post0.dev9/mapreader.egg-info/SOURCES.txt
+-rw-r--r--   0 rwood      (504) staff       (20)        1 2023-06-07 12:38:11.000000 mapreader-1.0.1.post0.dev9/mapreader.egg-info/dependency_links.txt
+-rw-r--r--   0 rwood      (504) staff       (20)       55 2023-06-07 12:38:11.000000 mapreader-1.0.1.post0.dev9/mapreader.egg-info/entry_points.txt
+-rw-r--r--   0 rwood      (504) staff       (20)        1 2023-03-23 14:47:41.000000 mapreader-1.0.1.post0.dev9/mapreader.egg-info/not-zip-safe
+-rw-r--r--   0 rwood      (504) staff       (20)      603 2023-06-07 12:38:11.000000 mapreader-1.0.1.post0.dev9/mapreader.egg-info/requires.txt
+-rw-r--r--   0 rwood      (504) staff       (20)       10 2023-06-07 12:38:11.000000 mapreader-1.0.1.post0.dev9/mapreader.egg-info/top_level.txt
+-rw-r--r--   0 rwood      (504) staff       (20)      211 2023-06-07 12:38:11.914097 mapreader-1.0.1.post0.dev9/setup.cfg
+-rw-r--r--   0 rwood      (504) staff       (20)     2764 2023-06-06 16:21:10.000000 mapreader-1.0.1.post0.dev9/setup.py
+drwxr-xr-x   0 rwood      (504) staff       (20)        0 2023-06-07 12:38:11.913750 mapreader-1.0.1.post0.dev9/tests/
+-rw-r--r--   0 rwood      (504) staff       (20)     3993 2023-06-05 15:21:45.000000 mapreader-1.0.1.post0.dev9/tests/test_annotations_loader.py
+-rw-r--r--   0 rwood      (504) staff       (20)     5335 2023-06-05 15:21:45.000000 mapreader-1.0.1.post0.dev9/tests/test_classifier.py
+-rw-r--r--   0 rwood      (504) staff       (20)      577 2023-06-05 15:21:45.000000 mapreader-1.0.1.post0.dev9/tests/test_import.py
+-rw-r--r--   0 rwood      (504) staff       (20)    14024 2023-05-24 14:03:30.000000 mapreader-1.0.1.post0.dev9/tests/test_sheet_downloader.py
+-rw-r--r--   0 rwood      (504) staff       (20)    83607 2023-04-25 09:23:09.000000 mapreader-1.0.1.post0.dev9/versioneer.py
```

### Comparing `mapreader-1.0.1.post0.dev11/LICENSE` & `mapreader-1.0.1.post0.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.1.post0.dev11/PKG-INFO` & `mapreader-1.0.1.post0.dev9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapreader
-Version: 1.0.1.post0.dev11
+Version: 1.0.1.post0.dev9
 Summary: A computer vision pipeline for the semantic exploration of maps/images at scale
 Home-page: https://github.com/Living-with-machines/MapReader
 Download-URL: https://github.com/Living-with-machines/MapReader/archive/refs/heads/main.zip
 Author: MapReader team
 License: MIT License
 Keywords: Computer Vision,Classification,Deep Learning,living with machines
 Platform: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mapreader Version: 1.0.1.post0.dev11 Summary: A
+Metadata-Version: 2.1 Name: mapreader Version: 1.0.1.post0.dev9 Summary: A
 computer vision pipeline for the semantic exploration of maps/images at scale
 Home-page: https://github.com/Living-with-machines/MapReader Download-URL:
 https://github.com/Living-with-machines/MapReader/archive/refs/heads/main.zip
 Author: MapReader team License: MIT License Keywords: Computer
 Vision,Classification,Deep Learning,living with machines Platform: OS
 Independent Classifier: Development Status :: 3 - Alpha Classifier: License ::
 OSI Approved :: MIT License Classifier: Natural Language :: English Classifier:
```

### Comparing `mapreader-1.0.1.post0.dev11/README.md` & `mapreader-1.0.1.post0.dev9/README.md`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.1.post0.dev11/mapreader/__init__.py` & `mapreader-1.0.1.post0.dev9/mapreader/__init__.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.1.post0.dev11/mapreader/annotate/utils.py` & `mapreader-1.0.1.post0.dev9/mapreader/annotate/utils.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.1.post0.dev11/mapreader/classify/classifier.py` & `mapreader-1.0.1.post0.dev9/mapreader/classify/classifier.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.1.post0.dev11/mapreader/classify/classifier_context.py` & `mapreader-1.0.1.post0.dev9/mapreader/classify/classifier_context.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.1.post0.dev11/mapreader/classify/custom_models.py` & `mapreader-1.0.1.post0.dev9/mapreader/classify/custom_models.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.1.post0.dev11/mapreader/classify/datasets.py` & `mapreader-1.0.1.post0.dev9/mapreader/classify/datasets.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.1.post0.dev11/mapreader/classify/load_annotations.py` & `mapreader-1.0.1.post0.dev9/mapreader/classify/load_annotations.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.1.post0.dev11/mapreader/download/data_structures.py` & `mapreader-1.0.1.post0.dev9/mapreader/download/data_structures.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.1.post0.dev11/mapreader/download/downloader.py` & `mapreader-1.0.1.post0.dev9/mapreader/download/downloader.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.1.post0.dev11/mapreader/download/downloader_utils.py` & `mapreader-1.0.1.post0.dev9/mapreader/download/downloader_utils.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.1.post0.dev11/mapreader/download/sheet_downloader.py` & `mapreader-1.0.1.post0.dev9/mapreader/download/sheet_downloader.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.1.post0.dev11/mapreader/download/tile_loading.py` & `mapreader-1.0.1.post0.dev9/mapreader/download/tile_loading.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.1.post0.dev11/mapreader/download/tile_merging.py` & `mapreader-1.0.1.post0.dev9/mapreader/download/tile_merging.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.1.post0.dev11/mapreader/load/geo_utils.py` & `mapreader-1.0.1.post0.dev9/mapreader/load/geo_utils.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.1.post0.dev11/mapreader/load/images.py` & `mapreader-1.0.1.post0.dev9/mapreader/load/images.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.1.post0.dev11/mapreader/load/loader.py` & `mapreader-1.0.1.post0.dev9/mapreader/load/loader.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.1.post0.dev11/mapreader/process/process.py` & `mapreader-1.0.1.post0.dev9/mapreader/process/process.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.1.post0.dev11/mapreader/utils/compute_and_save_stats.py` & `mapreader-1.0.1.post0.dev9/mapreader/utils/compute_and_save_stats.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.1.post0.dev11/mapreader/utils/slice_parallel.py` & `mapreader-1.0.1.post0.dev9/mapreader/utils/slice_parallel.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.1.post0.dev11/mapreader.egg-info/PKG-INFO` & `mapreader-1.0.1.post0.dev9/mapreader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapreader
-Version: 1.0.1.post0.dev11
+Version: 1.0.1.post0.dev9
 Summary: A computer vision pipeline for the semantic exploration of maps/images at scale
 Home-page: https://github.com/Living-with-machines/MapReader
 Download-URL: https://github.com/Living-with-machines/MapReader/archive/refs/heads/main.zip
 Author: MapReader team
 License: MIT License
 Keywords: Computer Vision,Classification,Deep Learning,living with machines
 Platform: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mapreader Version: 1.0.1.post0.dev11 Summary: A
+Metadata-Version: 2.1 Name: mapreader Version: 1.0.1.post0.dev9 Summary: A
 computer vision pipeline for the semantic exploration of maps/images at scale
 Home-page: https://github.com/Living-with-machines/MapReader Download-URL:
 https://github.com/Living-with-machines/MapReader/archive/refs/heads/main.zip
 Author: MapReader team License: MIT License Keywords: Computer
 Vision,Classification,Deep Learning,living with machines Platform: OS
 Independent Classifier: Development Status :: 3 - Alpha Classifier: License ::
 OSI Approved :: MIT License Classifier: Natural Language :: English Classifier:
```

### Comparing `mapreader-1.0.1.post0.dev11/mapreader.egg-info/SOURCES.txt` & `mapreader-1.0.1.post0.dev9/mapreader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.1.post0.dev11/mapreader.egg-info/requires.txt` & `mapreader-1.0.1.post0.dev9/mapreader.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.1.post0.dev11/setup.py` & `mapreader-1.0.1.post0.dev9/setup.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.1.post0.dev11/tests/test_annotations_loader.py` & `mapreader-1.0.1.post0.dev9/tests/test_annotations_loader.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.1.post0.dev11/tests/test_classifier.py` & `mapreader-1.0.1.post0.dev9/tests/test_classifier.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.1.post0.dev11/tests/test_import.py` & `mapreader-1.0.1.post0.dev9/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.1.post0.dev11/tests/test_sheet_downloader.py` & `mapreader-1.0.1.post0.dev9/tests/test_sheet_downloader.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.0.1.post0.dev11/versioneer.py` & `mapreader-1.0.1.post0.dev9/versioneer.py`

 * *Files identical despite different names*

