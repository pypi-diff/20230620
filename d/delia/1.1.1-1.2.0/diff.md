# Comparing `tmp/delia-1.1.1.tar.gz` & `tmp/delia-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delia-1.1.1.tar", last modified: Fri May 12 19:34:15 2023, max compression
+gzip compressed data, was "delia-1.2.0.tar", last modified: Tue Jun 20 15:28:16 2023, max compression
```

## Comparing `delia-1.1.1.tar` & `delia-1.2.0.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 19:34:15.826714 delia-1.1.1/
--rw-rw-rw-   0        0        0    11549 2022-03-24 18:12:27.000000 delia-1.1.1/LICENSE
--rw-rw-rw-   0        0        0    14855 2023-05-12 19:34:15.826714 delia-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0    14223 2023-05-05 16:16:03.000000 delia-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-12 19:34:15.717804 delia-1.1.1/delia/
--rw-rw-rw-   0        0        0      583 2023-05-12 19:33:13.000000 delia-1.1.1/delia/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 19:34:15.724553 delia-1.1.1/delia/databases/
--rw-rw-rw-   0        0        0       49 2022-11-08 03:00:14.000000 delia-1.1.1/delia/databases/__init__.py
--rw-rw-rw-   0        0        0    13270 2023-05-05 16:07:22.000000 delia-1.1.1/delia/databases/patients_database.py
-drwxrwxrwx   0        0        0        0 2023-05-12 19:34:15.725571 delia-1.1.1/delia/extractors/
--rw-rw-rw-   0        0        0      187 2023-05-04 17:50:19.000000 delia-1.1.1/delia/extractors/__init__.py
--rw-rw-rw-   0        0        0    14755 2023-05-05 16:07:22.000000 delia-1.1.1/delia/extractors/patients_data_extractor.py
-drwxrwxrwx   0        0        0        0 2023-05-12 19:34:15.730246 delia-1.1.1/delia/radiomics/
--rw-rw-rw-   0        0        0      158 2023-05-04 17:50:19.000000 delia-1.1.1/delia/radiomics/__init__.py
--rw-rw-rw-   0        0        0    11691 2023-05-05 16:07:22.000000 delia-1.1.1/delia/radiomics/radiomics_dataset.py
-drwxrwxrwx   0        0        0        0 2023-05-12 19:34:15.732959 delia-1.1.1/delia/readers/
--rw-rw-rw-   0        0        0       65 2022-11-08 03:03:57.000000 delia-1.1.1/delia/readers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 19:34:15.736288 delia-1.1.1/delia/readers/image/
--rw-rw-rw-   0        0        0        0 2022-02-08 18:32:16.000000 delia-1.1.1/delia/readers/image/__init__.py
--rw-rw-rw-   0        0        0    10880 2023-05-05 16:07:22.000000 delia-1.1.1/delia/readers/image/dicom_reader.py
-drwxrwxrwx   0        0        0        0 2023-05-12 19:34:15.743658 delia-1.1.1/delia/readers/patient_data/
--rw-rw-rw-   0        0        0        0 2022-02-08 18:32:16.000000 delia-1.1.1/delia/readers/patient_data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 19:34:15.749970 delia-1.1.1/delia/readers/patient_data/factories/
--rw-rw-rw-   0        0        0        0 2022-02-08 18:32:16.000000 delia-1.1.1/delia/readers/patient_data/factories/__init__.py
--rw-rw-rw-   0        0        0     4887 2022-11-15 18:06:34.000000 delia-1.1.1/delia/readers/patient_data/factories/base_patient_data_factory.py
--rw-rw-rw-   0        0        0     7615 2022-11-15 18:06:34.000000 delia-1.1.1/delia/readers/patient_data/factories/patient_data_factories.py
--rw-rw-rw-   0        0        0     3783 2022-11-15 18:06:34.000000 delia-1.1.1/delia/readers/patient_data/patient_data_query_context.py
--rw-rw-rw-   0        0        0      963 2022-11-03 14:49:27.000000 delia-1.1.1/delia/readers/patient_data/patient_data_query_strategy.py
--rw-rw-rw-   0        0        0    10002 2023-05-05 16:07:22.000000 delia-1.1.1/delia/readers/patient_data/patient_data_reader.py
-drwxrwxrwx   0        0        0        0 2023-05-12 19:34:15.757412 delia-1.1.1/delia/readers/segmentation/
--rw-rw-rw-   0        0        0        0 2022-02-08 18:32:16.000000 delia-1.1.1/delia/readers/segmentation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 19:34:15.768954 delia-1.1.1/delia/readers/segmentation/factories/
--rw-rw-rw-   0        0        0        0 2022-02-08 18:32:16.000000 delia-1.1.1/delia/readers/segmentation/factories/__init__.py
--rw-rw-rw-   0        0        0     2042 2022-11-08 03:20:33.000000 delia-1.1.1/delia/readers/segmentation/factories/base_segmentation_factory.py
--rw-rw-rw-   0        0        0     6278 2022-11-08 03:20:33.000000 delia-1.1.1/delia/readers/segmentation/factories/dicom_segmentation_factories.py
--rw-rw-rw-   0        0        0     1260 2022-07-27 14:35:42.000000 delia-1.1.1/delia/readers/segmentation/factories/segment.py
--rw-rw-rw-   0        0        0     2830 2022-02-08 18:32:16.000000 delia-1.1.1/delia/readers/segmentation/factories/segmentation.py
--rw-rw-rw-   0        0        0     4772 2023-05-05 16:07:22.000000 delia-1.1.1/delia/readers/segmentation/segmentation_context.py
--rw-rw-rw-   0        0        0     2801 2023-03-16 14:44:58.000000 delia-1.1.1/delia/readers/segmentation/segmentation_reader.py
--rw-rw-rw-   0        0        0     2217 2023-05-05 16:07:22.000000 delia-1.1.1/delia/readers/segmentation/segmentation_strategy.py
-drwxrwxrwx   0        0        0        0 2023-05-12 19:34:15.774518 delia-1.1.1/delia/transforms/
--rw-rw-rw-   0        0        0      120 2023-03-16 15:36:25.000000 delia-1.1.1/delia/transforms/__init__.py
--rw-rw-rw-   0        0        0    13213 2023-03-16 17:06:08.000000 delia-1.1.1/delia/transforms/applications.py
-drwxrwxrwx   0        0        0        0 2023-05-12 19:34:15.785193 delia-1.1.1/delia/transforms/array_space/
--rw-rw-rw-   0        0        0      293 2023-03-16 15:36:25.000000 delia-1.1.1/delia/transforms/array_space/__init__.py
--rw-rw-rw-   0        0        0     5103 2023-03-16 17:56:25.000000 delia-1.1.1/delia/transforms/array_space/matching_centroid_spatial_crop.py
--rw-rw-rw-   0        0        0     3132 2023-03-27 00:28:53.000000 delia-1.1.1/delia/transforms/array_space/matching_crop_foreground.py
--rw-rw-rw-   0        0        0     1043 2023-03-16 16:39:24.000000 delia-1.1.1/delia/transforms/array_space/tools.py
--rw-rw-rw-   0        0        0     2562 2023-03-16 16:29:22.000000 delia-1.1.1/delia/transforms/array_space/transform.py
-drwxrwxrwx   0        0        0        0 2023-05-12 19:34:15.790192 delia-1.1.1/delia/transforms/data/
--rw-rw-rw-   0        0        0      115 2023-03-16 15:36:25.000000 delia-1.1.1/delia/transforms/data/__init__.py
--rw-rw-rw-   0        0        0     4594 2023-05-05 16:10:26.000000 delia-1.1.1/delia/transforms/data/copy_segmentations.py
--rw-rw-rw-   0        0        0     1882 2022-11-15 18:06:34.000000 delia-1.1.1/delia/transforms/data/transform.py
-drwxrwxrwx   0        0        0        0 2023-05-12 19:34:15.802447 delia-1.1.1/delia/transforms/physical_space/
--rw-rw-rw-   0        0        0      269 2023-03-27 00:27:35.000000 delia-1.1.1/delia/transforms/physical_space/__init__.py
--rw-rw-rw-   0        0        0     3378 2023-05-12 19:28:03.000000 delia-1.1.1/delia/transforms/physical_space/matching_resample.py
--rw-rw-rw-   0        0        0     9826 2023-05-05 16:10:26.000000 delia-1.1.1/delia/transforms/physical_space/pet_to_suv.py
--rw-rw-rw-   0        0        0     3712 2023-05-12 19:30:41.000000 delia-1.1.1/delia/transforms/physical_space/resample.py
--rw-rw-rw-   0        0        0     3010 2023-03-16 16:29:21.000000 delia-1.1.1/delia/transforms/physical_space/transform.py
--rw-rw-rw-   0        0        0     2430 2023-03-16 16:29:21.000000 delia-1.1.1/delia/transforms/tools.py
-drwxrwxrwx   0        0        0        0 2023-05-12 19:34:15.811922 delia-1.1.1/delia/utils/
--rw-rw-rw-   0        0        0       42 2022-11-08 03:52:44.000000 delia-1.1.1/delia/utils/__init__.py
--rw-rw-rw-   0        0        0     4101 2023-03-16 14:44:58.000000 delia-1.1.1/delia/utils/data_model.py
--rw-rw-rw-   0        0        0     1329 2022-03-25 22:07:08.000000 delia-1.1.1/delia/utils/tools.py
--rw-rw-rw-   0        0        0     2131 2022-11-08 03:00:14.000000 delia-1.1.1/delia/utils/transforms_history.py
-drwxrwxrwx   0        0        0        0 2023-05-12 19:34:15.723389 delia-1.1.1/delia.egg-info/
--rw-rw-rw-   0        0        0    14855 2023-05-12 19:34:15.000000 delia-1.1.1/delia.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2252 2023-05-12 19:34:15.000000 delia-1.1.1/delia.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 19:34:15.000000 delia-1.1.1/delia.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       83 2023-05-12 19:34:15.000000 delia-1.1.1/delia.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-12 19:34:15.000000 delia-1.1.1/delia.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-12 19:34:15.824970 delia-1.1.1/examples/
--rw-rw-rw-   0        0        0       38 2022-03-26 17:30:16.000000 delia-1.1.1/examples/__init__.py
--rw-rw-rw-   0        0        0      712 2022-03-29 17:53:18.000000 delia-1.1.1/examples/env_examples.py
--rw-rw-rw-   0        0        0     3460 2023-05-12 19:24:41.000000 delia-1.1.1/examples/ex01.py
--rw-rw-rw-   0        0        0     3106 2023-05-12 19:24:41.000000 delia-1.1.1/examples/ex02.py
--rw-rw-rw-   0        0        0     2748 2023-05-12 19:28:03.000000 delia-1.1.1/examples/ex03.py
--rw-rw-rw-   0        0        0     5641 2022-11-15 18:06:34.000000 delia-1.1.1/examples/ex04.py
--rw-rw-rw-   0        0        0      108 2022-01-10 21:30:41.000000 delia-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-12 19:34:15.826714 delia-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1049 2023-05-12 19:33:13.000000 delia-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:28:16.416128 delia-1.2.0/
+-rw-rw-rw-   0        0        0    11549 2022-03-24 18:12:27.000000 delia-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0    15339 2023-06-20 15:28:16.416128 delia-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0    14707 2023-06-20 15:23:09.000000 delia-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 15:28:16.315293 delia-1.2.0/delia/
+-rw-rw-rw-   0        0        0      583 2023-06-20 15:27:34.000000 delia-1.2.0/delia/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:28:16.324396 delia-1.2.0/delia/databases/
+-rw-rw-rw-   0        0        0       49 2022-11-08 03:00:14.000000 delia-1.2.0/delia/databases/__init__.py
+-rw-rw-rw-   0        0        0    13272 2023-06-20 15:23:09.000000 delia-1.2.0/delia/databases/patients_database.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:28:16.327416 delia-1.2.0/delia/extractors/
+-rw-rw-rw-   0        0        0      187 2023-05-04 17:50:19.000000 delia-1.2.0/delia/extractors/__init__.py
+-rw-rw-rw-   0        0        0    14578 2023-06-20 15:23:09.000000 delia-1.2.0/delia/extractors/patients_data_extractor.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:28:16.331461 delia-1.2.0/delia/radiomics/
+-rw-rw-rw-   0        0        0      158 2023-05-04 17:50:19.000000 delia-1.2.0/delia/radiomics/__init__.py
+-rw-rw-rw-   0        0        0    11664 2023-06-20 15:23:09.000000 delia-1.2.0/delia/radiomics/radiomics_dataset.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:28:16.333458 delia-1.2.0/delia/readers/
+-rw-rw-rw-   0        0        0       65 2022-11-08 03:03:57.000000 delia-1.2.0/delia/readers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:28:16.335998 delia-1.2.0/delia/readers/image/
+-rw-rw-rw-   0        0        0        0 2022-02-08 18:32:16.000000 delia-1.2.0/delia/readers/image/__init__.py
+-rw-rw-rw-   0        0        0    11258 2023-06-20 15:23:09.000000 delia-1.2.0/delia/readers/image/dicom_reader.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:28:16.342644 delia-1.2.0/delia/readers/patient_data/
+-rw-rw-rw-   0        0        0        0 2022-02-08 18:32:16.000000 delia-1.2.0/delia/readers/patient_data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:28:16.346924 delia-1.2.0/delia/readers/patient_data/factories/
+-rw-rw-rw-   0        0        0        0 2022-02-08 18:32:16.000000 delia-1.2.0/delia/readers/patient_data/factories/__init__.py
+-rw-rw-rw-   0        0        0     5110 2023-06-20 15:23:09.000000 delia-1.2.0/delia/readers/patient_data/factories/base_patient_data_factory.py
+-rw-rw-rw-   0        0        0     8114 2023-06-20 15:23:09.000000 delia-1.2.0/delia/readers/patient_data/factories/patient_data_factories.py
+-rw-rw-rw-   0        0        0     3974 2023-06-20 15:23:09.000000 delia-1.2.0/delia/readers/patient_data/patient_data_query_context.py
+-rw-rw-rw-   0        0        0      943 2023-06-20 15:23:09.000000 delia-1.2.0/delia/readers/patient_data/patient_data_query_strategy.py
+-rw-rw-rw-   0        0        0    10030 2023-06-20 15:23:09.000000 delia-1.2.0/delia/readers/patient_data/patient_data_reader.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:28:16.354035 delia-1.2.0/delia/readers/segmentation/
+-rw-rw-rw-   0        0        0        0 2022-02-08 18:32:16.000000 delia-1.2.0/delia/readers/segmentation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:28:16.363035 delia-1.2.0/delia/readers/segmentation/factories/
+-rw-rw-rw-   0        0        0        0 2022-02-08 18:32:16.000000 delia-1.2.0/delia/readers/segmentation/factories/__init__.py
+-rw-rw-rw-   0        0        0     2042 2022-11-08 03:20:33.000000 delia-1.2.0/delia/readers/segmentation/factories/base_segmentation_factory.py
+-rw-rw-rw-   0        0        0     6278 2022-11-08 03:20:33.000000 delia-1.2.0/delia/readers/segmentation/factories/dicom_segmentation_factories.py
+-rw-rw-rw-   0        0        0     1260 2022-07-27 14:35:42.000000 delia-1.2.0/delia/readers/segmentation/factories/segment.py
+-rw-rw-rw-   0        0        0     2830 2022-02-08 18:32:16.000000 delia-1.2.0/delia/readers/segmentation/factories/segmentation.py
+-rw-rw-rw-   0        0        0     4772 2023-05-05 16:07:22.000000 delia-1.2.0/delia/readers/segmentation/segmentation_context.py
+-rw-rw-rw-   0        0        0     2801 2023-03-16 14:44:58.000000 delia-1.2.0/delia/readers/segmentation/segmentation_reader.py
+-rw-rw-rw-   0        0        0     2217 2023-05-05 16:07:22.000000 delia-1.2.0/delia/readers/segmentation/segmentation_strategy.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:28:16.369205 delia-1.2.0/delia/transforms/
+-rw-rw-rw-   0        0        0      120 2023-03-16 15:36:25.000000 delia-1.2.0/delia/transforms/__init__.py
+-rw-rw-rw-   0        0        0    13141 2023-06-20 15:23:09.000000 delia-1.2.0/delia/transforms/applications.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:28:16.379481 delia-1.2.0/delia/transforms/array_space/
+-rw-rw-rw-   0        0        0      293 2023-03-16 15:36:25.000000 delia-1.2.0/delia/transforms/array_space/__init__.py
+-rw-rw-rw-   0        0        0     5085 2023-06-20 15:23:09.000000 delia-1.2.0/delia/transforms/array_space/matching_centroid_spatial_crop.py
+-rw-rw-rw-   0        0        0     3096 2023-06-20 15:23:09.000000 delia-1.2.0/delia/transforms/array_space/matching_crop_foreground.py
+-rw-rw-rw-   0        0        0     1043 2023-03-16 16:39:24.000000 delia-1.2.0/delia/transforms/array_space/tools.py
+-rw-rw-rw-   0        0        0     2544 2023-06-20 15:23:09.000000 delia-1.2.0/delia/transforms/array_space/transform.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:28:16.385077 delia-1.2.0/delia/transforms/data/
+-rw-rw-rw-   0        0        0      115 2023-03-16 15:36:25.000000 delia-1.2.0/delia/transforms/data/__init__.py
+-rw-rw-rw-   0        0        0     4558 2023-06-20 15:23:09.000000 delia-1.2.0/delia/transforms/data/copy_segmentations.py
+-rw-rw-rw-   0        0        0     1864 2023-06-20 15:23:09.000000 delia-1.2.0/delia/transforms/data/transform.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:28:16.395067 delia-1.2.0/delia/transforms/physical_space/
+-rw-rw-rw-   0        0        0      269 2023-03-27 00:27:35.000000 delia-1.2.0/delia/transforms/physical_space/__init__.py
+-rw-rw-rw-   0        0        0     3360 2023-06-20 15:23:09.000000 delia-1.2.0/delia/transforms/physical_space/matching_resample.py
+-rw-rw-rw-   0        0        0     9808 2023-06-20 15:23:09.000000 delia-1.2.0/delia/transforms/physical_space/pet_to_suv.py
+-rw-rw-rw-   0        0        0     3694 2023-06-20 15:23:09.000000 delia-1.2.0/delia/transforms/physical_space/resample.py
+-rw-rw-rw-   0        0        0     2992 2023-06-20 15:23:09.000000 delia-1.2.0/delia/transforms/physical_space/transform.py
+-rw-rw-rw-   0        0        0     2403 2023-06-20 15:23:09.000000 delia-1.2.0/delia/transforms/tools.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:28:16.403067 delia-1.2.0/delia/utils/
+-rw-rw-rw-   0        0        0       42 2022-11-08 03:52:44.000000 delia-1.2.0/delia/utils/__init__.py
+-rw-rw-rw-   0        0        0     4101 2023-03-16 14:44:58.000000 delia-1.2.0/delia/utils/data_model.py
+-rw-rw-rw-   0        0        0     1329 2022-03-25 22:07:08.000000 delia-1.2.0/delia/utils/tools.py
+-rw-rw-rw-   0        0        0     2131 2022-11-08 03:00:14.000000 delia-1.2.0/delia/utils/transforms_history.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:28:16.319297 delia-1.2.0/delia.egg-info/
+-rw-rw-rw-   0        0        0    15339 2023-06-20 15:28:16.000000 delia-1.2.0/delia.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2252 2023-06-20 15:28:16.000000 delia-1.2.0/delia.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 15:28:16.000000 delia-1.2.0/delia.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       83 2023-06-20 15:28:16.000000 delia-1.2.0/delia.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-20 15:28:16.000000 delia-1.2.0/delia.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 15:28:16.414692 delia-1.2.0/examples/
+-rw-rw-rw-   0        0        0       38 2022-03-26 17:30:16.000000 delia-1.2.0/examples/__init__.py
+-rw-rw-rw-   0        0        0      712 2022-03-29 17:53:18.000000 delia-1.2.0/examples/env_examples.py
+-rw-rw-rw-   0        0        0     3440 2023-06-20 15:23:09.000000 delia-1.2.0/examples/ex01.py
+-rw-rw-rw-   0        0        0     3085 2023-06-20 15:23:09.000000 delia-1.2.0/examples/ex02.py
+-rw-rw-rw-   0        0        0     2726 2023-06-20 15:23:09.000000 delia-1.2.0/examples/ex03.py
+-rw-rw-rw-   0        0        0     5348 2023-06-20 15:23:09.000000 delia-1.2.0/examples/ex04.py
+-rw-rw-rw-   0        0        0      108 2022-01-10 21:30:41.000000 delia-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-20 15:28:16.416128 delia-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1049 2023-06-20 15:27:44.000000 delia-1.2.0/setup.py
```

### Comparing `delia-1.1.1/LICENSE` & `delia-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `delia-1.1.1/PKG-INFO` & `delia-1.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delia
-Version: 1.1.1
+Version: 1.2.0
 Summary: DICOM Extraction for Large-scale Image Analysis (DELIA).
 Home-page: https://github.com/MaxenceLarose/delia
 Author: Maxence Larose
 Author-email: maxence.larose.1@ulaval.ca
 License: Apache License 2.0
 Keywords: dicom hdf5 medical image segmentation pre-processing python3 radiomics deep-learning dicom-seg rt-struct
 Classifier: Programming Language :: Python :: 3
@@ -109,34 +109,34 @@
 
 ### File format
 
 Images files must be in standard [**DICOM**](https://www.dicomstandard.org/) format and segmentation files must be in [DICOM-SEG](https://dicom.nema.org/medical/dicom/current/output/chtml/part03/sect_C.8.20.html) or [RTStruct](https://dicom.nema.org/dicom/2013/output/chtml/part03/sect_A.19.html) format.
 
 If your segmentation files are in a research file format (`.nrrd`, `.nii`, etc.), you need to convert them into the standardized [DICOM-SEG](https://dicom.nema.org/medical/dicom/current/output/chtml/part03/sect_C.8.20.html) or [RTStruct](https://dicom.nema.org/dicom/2013/output/chtml/part03/sect_A.19.html) format. You can use the [pydicom-seg](https://pypi.org/project/pydicom-seg/) library to create the DICOM-SEG files OR use the [itkimage2dicomSEG](https://github.com/MaxenceLarose/itkimage2dicomSEG) python module, which provide a complete pipeline to perform this conversion. Also, you can use the [RT-Utils](https://github.com/qurit/rt-utils) library to create the RTStruct files.
 
-### Series descriptions (Optional)
+### Tag values (Optional)
 
-*This dictionary is **not** mandatory for the code to work and therefore its default value is `None`. Note that if no `series_descriptions` dictionary is given, i.e. `series_descriptions = None`, then all images will be added to the database.*
+*This dictionary is **not** mandatory for the code to work and therefore its default value is `None`. Note that if no `tag_values` dictionary is given, i.e. `tag_values = None`, then all images will be added to the database.*
 
-The series descriptions are specified as a **dictionary** that contains the series descriptions of the images that needs to be extracted from the patients' files. Keys are arbitrary names given to the images we want to add and values are lists of series descriptions. The images associated with these series descriptions do not need to have a corresponding segmentation volume. If none of the descriptions match the series in a patient's files, a warning is raised and the patient is added to the list of patients for whom the pipeline has failed.
+The tag values are specified as a **dictionary** that contains the values for the tag specified when creating the PatientsDataExtractor object of the images that need to be extracted from the patients' files. Keys are arbitrary names given to the images we want to add and values are lists of values for the desired tag. The images associated with these tag values do not need to have a corresponding segmentation volume. If none of the descriptions match the series in a patient's files, a warning is raised and the patient is added to the list of patients for whom the pipeline has failed.
 
-Note that the series descriptions can be specified as a classic dictionary or as a path to a **json file** that contains the series descriptions. Both methods are presented below.
+Note that the tag values can be specified as a python dictionary or as a path to a **json file** that contains the desired values. Both methods are presented below.
 
 <details>
   <summary>Using a json file</summary>
 
-Create a json file containing only the dictionary of the names given to the images we want to add (keys) and lists of series descriptions (values). Place this file in your data folder.
+Create a json file containing only the dictionary of the names given to the images we want to add (keys) and lists of tag values (values). Place this file in your data folder.
 
 Here is an example of a json file configured as expected :
 
 ```json
 {
-    "TEP": [
-        "TEP WB CORR (AC)",
-        "TEP WB XL CORR (AC)"
+    "PT": [
+        "PT WB CORR (AC)",
+        "PT WB XL CORR (AC)"
     ],
     "CT": [
         "CT 2.5 WB",
         "AC CT 2.5 WB"
     ]
 }
 ```
@@ -146,18 +146,18 @@
   <summary>Using a Python dictionary</summary>
 
 Create the organs dictionary in your main.py python file.
 
 Here is an example of a python dictionary instanced as expected :
 
 ```python
-series_descriptions = {
-    "TEP": [
-        "TEP WB CORR (AC)",
-        "TEP WB XL CORR (AC)"
+tag_values = {
+    "PT": [
+        "PT WB CORR (AC)",
+        "PT WB XL CORR (AC)"
     ],
     "CT": [
         "CT 2.5 WB",
         "AC CT 2.5 WB"
     ]
 }
 ```
@@ -167,15 +167,15 @@
 
 It is important to configure the directory structure correctly to ensure that the module interacts correctly with the data files. The `patients` folder, must be structured as follows. *Note that all DICOM files in the patients' folder will be read.*
 
 ```
 |_📂 Project directory/
   |_📄 main.py
   |_📂 data/
-    |_📄 series_descriptions.json
+    |_📄 tag_values.json
     |_📂 patients/
       |_📂 patient1/
        	|_📄 ...
        	|_📂 ...
       |_📂 patient2/
        	|_📄 ...
        	|_📂 ...
@@ -216,23 +216,23 @@
     Compose,
     ScaleIntensityD,
     ThresholdIntensityD
 )
 
 patients_data_extractor = PatientsDataExtractor(
     path_to_patients_folder="data/patients",
-    series_descriptions="data/series_descriptions.json",
+    tag_values="data/tag_values.json",
     transforms=Compose(
         [
-            ResampleD(keys=["CT_THORAX", "TEP", "Heart"], out_spacing=(1.5, 1.5, 1.5)),
-            CenterSpatialCropD(keys=["CT_THORAX", "TEP", "Heart"], roi_size=(1000, 160, 160)),
+            ResampleD(keys=["CT_THORAX", "PT", "Heart"], out_spacing=(1.5, 1.5, 1.5)),
+            CenterSpatialCropD(keys=["CT_THORAX", "PT", "Heart"], roi_size=(1000, 160, 160)),
             ThresholdIntensityD(keys=["CT_THORAX"], threshold=-250, above=True, cval=-250),
             ThresholdIntensityD(keys=["CT_THORAX"], threshold=500, above=False, cval=500),
             ScaleIntensityD(keys=["CT_THORAX"], minv=0, maxv=1),
-            PETtoSUVD(keys=["TEP"])
+            PETtoSUVD(keys=["PT"])
         ]
     )
 )
 
 database = PatientsDatabase(path_to_database="data/patients_database.h5")
 
 database.create(
@@ -254,26 +254,26 @@
 ```python
 from delia.extractors import PatientsDataExtractor
 from delia.transforms import Compose, CopySegmentationsD, PETtoSUVD, ResampleD
 import SimpleITK as sitk
 
 patients_data_extractor = PatientsDataExtractor(
     path_to_patients_folder="data/patients",
-    series_descriptions="data/series_descriptions.json",
+    tag_values="data/tag_values.json",
     transforms=Compose(
         [
             ResampleD(keys=["CT_THORAX", "Heart"], out_spacing=(1.5, 1.5, 1.5)),
-            PETtoSUVD(keys=["TEP"]),
-            CopySegmentationsD(segmented_image_key="CT_THORAX", unsegmented_image_key="TEP")
+            PETtoSUVD(keys=["PT"]),
+            CopySegmentationsD(segmented_image_key="CT_THORAX", unsegmented_image_key="PT")
         ]
     )
 )
 
 for patient_dataset in patients_data_extractor:
-	print(f"Patient ID: {patient_data.patient_id}")
+    print(f"Patient ID: {patient_dataset.patient_id}")
 
     for patient_image_data in patient_dataset.data:
         dicom_header = patient_image_data.image.dicom_header
         simple_itk_image = patient_image_data.image.simple_itk_image
         numpy_array_image = sitk.GetArrayFromImage(simple_itk_image)
 
         """Perform any tasks on images on-the-fly."""
@@ -282,21 +282,23 @@
 
 ## Need more examples?
 
 You can find more in the [examples folder](https://github.com/MaxenceLarose/delia/tree/main/examples).
 
 # A deeper look into the `PatientsDataExtractor` object
 
-The `PatientsDataExtractor` has 3 important variables:  a `path_to_patients_folder` (which dictates the path to the folder that contains all patient records), a `series_descriptions` (which dictates the images that needs to be extracted from the patient records) and `transforms` that defines a sequence of transformations to apply on images or segmentations. For each patient/folder available in the `path_to_patients_folder`, all DICOM files in their folder are read. If the series descriptions of a certain volume match one of the descriptions present in the given `series_descriptions` dictionary, this volume and its segmentation (if available) are automatically added to the `PatientDataModel`. Note that if no `series_descriptions` dictionary is given (`series_descriptions = None`), then all images (and associated segmentations) will be added to the database. 
+The `PatientsDataExtractor` has 4 important variables:  a `path_to_patients_folder` (which dictates the path to the folder that contains all patient records), a `tag` (which specifies which tag to use when choosing which images need to be extracted, if no value is given, this defaults to `SeriesDescription`), a `tag_values` (which dictates the images that needs to be extracted from the patient records) and `transforms` that defines a sequence of transformations to apply on images or segmentations. For each patient/folder available in the `path_to_patients_folder`, all DICOM files in their folder are read. If the specified tag's value of a certain volume match one of the descriptions present in the given `tag_values` dictionary, this volume and its segmentation (if available) are automatically added to the `PatientDataModel`. Note that if no `tag_values` dictionary is given (`tag_values = None`), then all images (and associated segmentations) will be added to the database. 
 
 The `PatientsDataExtractor` can therefore be used to iteratively perform tasks on each of the patients, such as displaying certain images, transforming images into numpy arrays, or creating an HDF5 database using the `PatientsDatabase`. It is this last task that is highlighted in this package, but it must be understood that the data extraction is performed in a very general manner by the `PatientsDataExtractor` and is therefore not limited to this single application. For example, someone could easily develop a `Numpydatabase` whose creation would be ensured by the `PatientsDataExtractor`, similar to the current `PatientsDatabase` based on the HDF5 format.
 
 # TODO
 
-- [ ] Generalize the use of arbitrary tags to choose images to extract. At the moment, the only tag available is `series_descriptions`.
+- [x] Generalize the use of arbitrary tags to choose images to extract. At the moment, the only tag available is `series_descriptions`.
+- [ ] Find which DICOM tags act in unusual ways such as having data associated with .repval and .value which differ by more than just their type. For now, both are used to obtain the same value in delia/readers/patient_data/factories/patient_data_factories.py (152-155) and delia/readers/image/dicom_reader.py (113-116).
+- [ ] Allow for more comprehensive use of tags such as using AND, OR and NOT between tags and their values. 
 - [ ] Loosen monai version requirements (monai==1.0.1) to allow for more recent versions. This needs a redefinition of the way transforms are applied.
 
 
 # License
 
 This code is provided under the [Apache License 2.0](https://github.com/MaxenceLarose/delia/blob/main/LICENSE).
```

### Comparing `delia-1.1.1/README.md` & `delia-1.2.0/delia.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: delia
+Version: 1.2.0
+Summary: DICOM Extraction for Large-scale Image Analysis (DELIA).
+Home-page: https://github.com/MaxenceLarose/delia
+Author: Maxence Larose
+Author-email: maxence.larose.1@ulaval.ca
+License: Apache License 2.0
+Keywords: dicom hdf5 medical image segmentation pre-processing python3 radiomics deep-learning dicom-seg rt-struct
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <p align="center" width="100%">
     <img width="100%" src="https://github.com/MaxenceLarose/delia/raw/main/images/logo/delia_banner.svg">
 </p>
 <p align="center"><i>DELIA facilitates data extraction from DICOM files to support large-scale image analysis workflows.</i></p>
 
 # Notable features
 
@@ -93,34 +109,34 @@
 
 ### File format
 
 Images files must be in standard [**DICOM**](https://www.dicomstandard.org/) format and segmentation files must be in [DICOM-SEG](https://dicom.nema.org/medical/dicom/current/output/chtml/part03/sect_C.8.20.html) or [RTStruct](https://dicom.nema.org/dicom/2013/output/chtml/part03/sect_A.19.html) format.
 
 If your segmentation files are in a research file format (`.nrrd`, `.nii`, etc.), you need to convert them into the standardized [DICOM-SEG](https://dicom.nema.org/medical/dicom/current/output/chtml/part03/sect_C.8.20.html) or [RTStruct](https://dicom.nema.org/dicom/2013/output/chtml/part03/sect_A.19.html) format. You can use the [pydicom-seg](https://pypi.org/project/pydicom-seg/) library to create the DICOM-SEG files OR use the [itkimage2dicomSEG](https://github.com/MaxenceLarose/itkimage2dicomSEG) python module, which provide a complete pipeline to perform this conversion. Also, you can use the [RT-Utils](https://github.com/qurit/rt-utils) library to create the RTStruct files.
 
-### Series descriptions (Optional)
+### Tag values (Optional)
 
-*This dictionary is **not** mandatory for the code to work and therefore its default value is `None`. Note that if no `series_descriptions` dictionary is given, i.e. `series_descriptions = None`, then all images will be added to the database.*
+*This dictionary is **not** mandatory for the code to work and therefore its default value is `None`. Note that if no `tag_values` dictionary is given, i.e. `tag_values = None`, then all images will be added to the database.*
 
-The series descriptions are specified as a **dictionary** that contains the series descriptions of the images that needs to be extracted from the patients' files. Keys are arbitrary names given to the images we want to add and values are lists of series descriptions. The images associated with these series descriptions do not need to have a corresponding segmentation volume. If none of the descriptions match the series in a patient's files, a warning is raised and the patient is added to the list of patients for whom the pipeline has failed.
+The tag values are specified as a **dictionary** that contains the values for the tag specified when creating the PatientsDataExtractor object of the images that need to be extracted from the patients' files. Keys are arbitrary names given to the images we want to add and values are lists of values for the desired tag. The images associated with these tag values do not need to have a corresponding segmentation volume. If none of the descriptions match the series in a patient's files, a warning is raised and the patient is added to the list of patients for whom the pipeline has failed.
 
-Note that the series descriptions can be specified as a classic dictionary or as a path to a **json file** that contains the series descriptions. Both methods are presented below.
+Note that the tag values can be specified as a python dictionary or as a path to a **json file** that contains the desired values. Both methods are presented below.
 
 <details>
   <summary>Using a json file</summary>
 
-Create a json file containing only the dictionary of the names given to the images we want to add (keys) and lists of series descriptions (values). Place this file in your data folder.
+Create a json file containing only the dictionary of the names given to the images we want to add (keys) and lists of tag values (values). Place this file in your data folder.
 
 Here is an example of a json file configured as expected :
 
 ```json
 {
-    "TEP": [
-        "TEP WB CORR (AC)",
-        "TEP WB XL CORR (AC)"
+    "PT": [
+        "PT WB CORR (AC)",
+        "PT WB XL CORR (AC)"
     ],
     "CT": [
         "CT 2.5 WB",
         "AC CT 2.5 WB"
     ]
 }
 ```
@@ -130,18 +146,18 @@
   <summary>Using a Python dictionary</summary>
 
 Create the organs dictionary in your main.py python file.
 
 Here is an example of a python dictionary instanced as expected :
 
 ```python
-series_descriptions = {
-    "TEP": [
-        "TEP WB CORR (AC)",
-        "TEP WB XL CORR (AC)"
+tag_values = {
+    "PT": [
+        "PT WB CORR (AC)",
+        "PT WB XL CORR (AC)"
     ],
     "CT": [
         "CT 2.5 WB",
         "AC CT 2.5 WB"
     ]
 }
 ```
@@ -151,15 +167,15 @@
 
 It is important to configure the directory structure correctly to ensure that the module interacts correctly with the data files. The `patients` folder, must be structured as follows. *Note that all DICOM files in the patients' folder will be read.*
 
 ```
 |_📂 Project directory/
   |_📄 main.py
   |_📂 data/
-    |_📄 series_descriptions.json
+    |_📄 tag_values.json
     |_📂 patients/
       |_📂 patient1/
        	|_📄 ...
        	|_📂 ...
       |_📂 patient2/
        	|_📄 ...
        	|_📂 ...
@@ -200,23 +216,23 @@
     Compose,
     ScaleIntensityD,
     ThresholdIntensityD
 )
 
 patients_data_extractor = PatientsDataExtractor(
     path_to_patients_folder="data/patients",
-    series_descriptions="data/series_descriptions.json",
+    tag_values="data/tag_values.json",
     transforms=Compose(
         [
-            ResampleD(keys=["CT_THORAX", "TEP", "Heart"], out_spacing=(1.5, 1.5, 1.5)),
-            CenterSpatialCropD(keys=["CT_THORAX", "TEP", "Heart"], roi_size=(1000, 160, 160)),
+            ResampleD(keys=["CT_THORAX", "PT", "Heart"], out_spacing=(1.5, 1.5, 1.5)),
+            CenterSpatialCropD(keys=["CT_THORAX", "PT", "Heart"], roi_size=(1000, 160, 160)),
             ThresholdIntensityD(keys=["CT_THORAX"], threshold=-250, above=True, cval=-250),
             ThresholdIntensityD(keys=["CT_THORAX"], threshold=500, above=False, cval=500),
             ScaleIntensityD(keys=["CT_THORAX"], minv=0, maxv=1),
-            PETtoSUVD(keys=["TEP"])
+            PETtoSUVD(keys=["PT"])
         ]
     )
 )
 
 database = PatientsDatabase(path_to_database="data/patients_database.h5")
 
 database.create(
@@ -238,26 +254,26 @@
 ```python
 from delia.extractors import PatientsDataExtractor
 from delia.transforms import Compose, CopySegmentationsD, PETtoSUVD, ResampleD
 import SimpleITK as sitk
 
 patients_data_extractor = PatientsDataExtractor(
     path_to_patients_folder="data/patients",
-    series_descriptions="data/series_descriptions.json",
+    tag_values="data/tag_values.json",
     transforms=Compose(
         [
             ResampleD(keys=["CT_THORAX", "Heart"], out_spacing=(1.5, 1.5, 1.5)),
-            PETtoSUVD(keys=["TEP"]),
-            CopySegmentationsD(segmented_image_key="CT_THORAX", unsegmented_image_key="TEP")
+            PETtoSUVD(keys=["PT"]),
+            CopySegmentationsD(segmented_image_key="CT_THORAX", unsegmented_image_key="PT")
         ]
     )
 )
 
 for patient_dataset in patients_data_extractor:
-	print(f"Patient ID: {patient_data.patient_id}")
+    print(f"Patient ID: {patient_dataset.patient_id}")
 
     for patient_image_data in patient_dataset.data:
         dicom_header = patient_image_data.image.dicom_header
         simple_itk_image = patient_image_data.image.simple_itk_image
         numpy_array_image = sitk.GetArrayFromImage(simple_itk_image)
 
         """Perform any tasks on images on-the-fly."""
@@ -266,21 +282,23 @@
 
 ## Need more examples?
 
 You can find more in the [examples folder](https://github.com/MaxenceLarose/delia/tree/main/examples).
 
 # A deeper look into the `PatientsDataExtractor` object
 
-The `PatientsDataExtractor` has 3 important variables:  a `path_to_patients_folder` (which dictates the path to the folder that contains all patient records), a `series_descriptions` (which dictates the images that needs to be extracted from the patient records) and `transforms` that defines a sequence of transformations to apply on images or segmentations. For each patient/folder available in the `path_to_patients_folder`, all DICOM files in their folder are read. If the series descriptions of a certain volume match one of the descriptions present in the given `series_descriptions` dictionary, this volume and its segmentation (if available) are automatically added to the `PatientDataModel`. Note that if no `series_descriptions` dictionary is given (`series_descriptions = None`), then all images (and associated segmentations) will be added to the database. 
+The `PatientsDataExtractor` has 4 important variables:  a `path_to_patients_folder` (which dictates the path to the folder that contains all patient records), a `tag` (which specifies which tag to use when choosing which images need to be extracted, if no value is given, this defaults to `SeriesDescription`), a `tag_values` (which dictates the images that needs to be extracted from the patient records) and `transforms` that defines a sequence of transformations to apply on images or segmentations. For each patient/folder available in the `path_to_patients_folder`, all DICOM files in their folder are read. If the specified tag's value of a certain volume match one of the descriptions present in the given `tag_values` dictionary, this volume and its segmentation (if available) are automatically added to the `PatientDataModel`. Note that if no `tag_values` dictionary is given (`tag_values = None`), then all images (and associated segmentations) will be added to the database. 
 
 The `PatientsDataExtractor` can therefore be used to iteratively perform tasks on each of the patients, such as displaying certain images, transforming images into numpy arrays, or creating an HDF5 database using the `PatientsDatabase`. It is this last task that is highlighted in this package, but it must be understood that the data extraction is performed in a very general manner by the `PatientsDataExtractor` and is therefore not limited to this single application. For example, someone could easily develop a `Numpydatabase` whose creation would be ensured by the `PatientsDataExtractor`, similar to the current `PatientsDatabase` based on the HDF5 format.
 
 # TODO
 
-- [ ] Generalize the use of arbitrary tags to choose images to extract. At the moment, the only tag available is `series_descriptions`.
+- [x] Generalize the use of arbitrary tags to choose images to extract. At the moment, the only tag available is `series_descriptions`.
+- [ ] Find which DICOM tags act in unusual ways such as having data associated with .repval and .value which differ by more than just their type. For now, both are used to obtain the same value in delia/readers/patient_data/factories/patient_data_factories.py (152-155) and delia/readers/image/dicom_reader.py (113-116).
+- [ ] Allow for more comprehensive use of tags such as using AND, OR and NOT between tags and their values. 
 - [ ] Loosen monai version requirements (monai==1.0.1) to allow for more recent versions. This needs a redefinition of the way transforms are applied.
 
 
 # License
 
 This code is provided under the [Apache License 2.0](https://github.com/MaxenceLarose/delia/blob/main/LICENSE).
```

### Comparing `delia-1.1.1/delia/__init__.py` & `delia-1.2.0/delia/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,14 @@
 from .utils import PatientDataModel
 
 stream_handler = logging.StreamHandler()
 stream_handler.setLevel(logging.WARNING)
 logging.getLogger(__name__).addHandler(stream_handler)
 
 __author__ = "Maxence Larose"
-__version__ = "1.1.1"
+__version__ = "1.2.0"
 __copyright__ = "Copyright 2022, Maxence Larose"
 __credits__ = ["Maxence Larose"]
 __license__ = "Apache License 2.0"
 __maintainer__ = "Maxence Larose"
 __email__ = "maxence.larose.1@ulaval.ca"
 __status__ = "Production"
```

### Comparing `delia-1.1.1/delia/databases/patients_database.py` & `delia-1.2.0/delia/databases/patients_database.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         ----------
         path_to_database : str
             Path to database.
         """
         self.path_to_database = path_to_database
 
         if os.path.exists(path_to_database):
-            self._file = h5py.File(path_to_database, mode="r")
+            self._file = h5py.File(path_to_database, mode="r+")
         else:
             self._file = None
 
     @property
     def path_to_database(self) -> str:
         """
         Path to database.
@@ -311,15 +311,15 @@
                     )
 
                 _logger.info(f"Progress : {patient_idx + 1}/{number_of_patients} patients added to database.")
 
             patients_data_extractor.close()
             patients_data_extractor.reset()
 
-        self._file = h5py.File(self.path_to_database, "r")
+        self._file = h5py.File(self.path_to_database, "r+")
 
         return patients_data_extractor.patients_who_failed
 
     def close(self):
         """
         Closes the hdf5 file database.
         """
```

### Comparing `delia-1.1.1/delia/extractors/patients_data_extractor.py` & `delia-1.2.0/delia/extractors/patients_data_extractor.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from collections.abc import Generator
 from copy import deepcopy
 import json
 import logging
 import os
-from typing import Dict, List, NamedTuple, Optional, Union
+from typing import Dict, List, NamedTuple, Optional, Tuple, Union
 
 from monai.transforms import Compose
 from monai.transforms import MapTransform as MonaiMapTransform
 
 from delia.readers.patient_data.patient_data_reader import PatientDataReader
 from delia.transforms.data.transform import DataTransform
 from delia.transforms.physical_space.transform import PhysicalSpaceTransform
@@ -27,69 +27,74 @@
 
 _logger = logging.getLogger(__name__)
 
 
 class PatientWhoFailed(NamedTuple):
     id: str
     failed_images: Dict[str, List[str]]
-    available_series_descriptions: List[str]
+    available_tag_values: List[str]
 
 
 class PatientsDataExtractor(Generator):
     """
     A class used to iterate on multiple patients' dicom files and segmentation files using the PatientDataReader to
     obtain all patients' data. The PatientsDataGenerator inherits from the Generator abstract class.
     """
 
     def __init__(
             self,
             path_to_patients_folder: str,
-            series_descriptions: Optional[Union[str, Dict[str, List[str]]]] = None,
+            tag: Union[str, Tuple[int, int]] = "SeriesDescription",
+            tag_values: Optional[Union[str, Dict[str, List[str]]]] = None,
             transforms: Optional[Union[Compose, DataTransform, MonaiMapTransform, PhysicalSpaceTransform]] = None,
             erase_unused_dicom_files: bool = False
     ) -> None:
         """
-        Used to get the paths to the images and segmentations folders. Also used to check if either the series
-        descriptions or the path to the series description json dictionary is None.
+        Used to get the paths to the images and segmentations folders. Also used to check if either the tag values or
+        the path to the tag value json dictionary is None.
 
         Parameters
         ----------
         path_to_patients_folder : str
             The path to the folder that contains all the patients' folders.
-        series_descriptions : Optional[Union[str, Dict[str, List[str]]]], default = None.
-            A dictionary that contains the series descriptions of the images that needs to be extracted from the
-            patient's file. Keys are arbitrary names given to the images we want to add and values are lists of
-            series descriptions. The images associated with these series descriptions do not need to have a
+        tag : Union[str, Tuple[int, int]] = "SeriesDescription"
+            Keyword or tuple of the DICOM tag to use while selecting which files to extract. Uses SeriesDescription
+            as a default.
+        tag_values : Optional[Union[str, Dict[str, List[str]]]], default = None.
+            A dictionary that contains the desired tag's values for the images that absolutely needs to be extracted
+            from the patient's file. Keys are arbitrary names given to the images we want to add and values are lists of
+            values associated with the specified tag. The images associated with these values do not need to have a
             corresponding segmentation. Note that it can be specified as a path to a json dictionary that contains the
-            series descriptions.
+            desired values for the tag.
         transforms : Union[Compose, DataTransform, MonaiMapTransform, PhysicalSpaceTransform]
             A sequence of transformations to apply. PhysicalSpaceTransform are applied in the physical space, i.e on
             the SimpleITK image, while MonaiMapTransform are applied in the array space, i.e on the numpy array that
             represents the image. DataTransform transforms the data using other a patient's other images or
-            segmentations. The keys for images are assumed to be the arbitrary series key set in 'series_descriptions'.
-            For segmentation, keys are organ names. Note that if 'series_descriptions' is None, the keys for images are
+            segmentations. The keys for images are assumed to be the arbitrary series key set in 'tag_values'.
+            For segmentation, keys are organ names. Note that if 'tag_values' is None, the keys for images are
             assumed to be modalities.
         erase_unused_dicom_files: bool = False
             Whether to delete unused DICOM files or not. Use with EXTREME caution!
         """
         self._path_to_patients_folder = path_to_patients_folder
         self._erase_unused_dicom_files = erase_unused_dicom_files
         self._transforms = self._validate_transforms(transforms)
+        self.tag = tag
 
-        if isinstance(series_descriptions, str):
-            self.path_to_series_description_json = series_descriptions
-        elif isinstance(series_descriptions, dict):
-            self.series_descriptions = series_descriptions
-            self._path_to_series_description_json = None
-        elif series_descriptions is None:
-            self._series_descriptions = None
-            self._path_to_series_description_json = None
+        if isinstance(tag_values, str):
+            self.path_to_tag_value_json = tag_values
+        elif isinstance(tag_values, dict):
+            self.tag_values = tag_values
+            self._path_to_tag_value_json = None
+        elif tag_values is None:
+            self._tag_values = None
+            self._path_to_tag_value_json = None
         else:
             raise TypeError(
-                f"Given series descriptions {series_descriptions} doesn't have the right type. Allowed types are str, "
+                f"Given values {tag_values} for the tag {tag} doesn't have the right type. Allowed types are str, "
                 f"dict and None."
             )
 
         self._current_index = 0
         self._patients_who_failed = []
 
     def __len__(self) -> int:
@@ -120,80 +125,80 @@
                 patient_folder_name
             )
             paths_to_folders.append(path_to_folder)
 
         return paths_to_folders
 
     @property
-    def series_descriptions(self) -> Dict[str, List[str]]:
+    def tag_values(self) -> Dict[str, List[str]]:
         """
-        Series descriptions.
+        Tag values.
 
         Returns
         -------
-        series_descriptions : Dict[str, List[str]]
-            A dictionary that contains the series descriptions of the images that absolutely needs to be extracted from
-            the patient's file. Keys are arbitrary names given to the images we want to add and values are lists of
-            series descriptions.
+        tag_values : Dict[str, List[str]]
+            A dictionary that contains the desired tag's values for the images that absolutely needs to be extracted
+            from the patient's file. Keys are arbitrary names given to the images we want to add and values are lists of
+            values associated with the specified tag.
         """
-        return self._series_descriptions
+        return self._tag_values
 
-    @series_descriptions.setter
-    def series_descriptions(self, series_descriptions: Dict[str, List[str]]) -> None:
+    @tag_values.setter
+    def tag_values(self, tag_values: Dict[str, List[str]]) -> None:
         """
-        Series descriptions setter.
+        Tag values setter.
 
         Parameters
         ----------
-        series_descriptions : Dict[str, List[str]]
-            A dictionary that contains the series descriptions of the images that absolutely needs to be extracted from
-            the patient's file. Keys are arbitrary names given to the images we want to add and values are lists of
-            series descriptions.
+        tag_values : Dict[str, List[str]]
+            A dictionary that contains the desired tag's values for the images that absolutely needs to be extracted
+            from the patient's file. Keys are arbitrary names given to the images we want to add and values are lists of
+            values associated with the specified tag.
         """
-        items = list(series_descriptions.items())
+        items = list(tag_values.items())
         for previous_items, current_items in zip(items, items[1:]):
             set_intersection = set(previous_items[1]) & set(current_items[1])
 
             if bool(set_intersection):
                 raise AssertionError(
-                    f"\nThe dictionary of series descriptions should not contain the same series names for different "
+                    f"\nThe dictionary of tag values should not contain the same series names for different "
                     f"images/modalities. \nHowever, here we find the series names {previous_items[1]} for the "
                     f"{previous_items[0]} image and {current_items[1]} for the {current_items[0]} image. \nClearly, "
                     f"the images series values are overlapping because of the series named {set_intersection}."
                 )
 
-        self._series_descriptions = series_descriptions
+        self._tag_values = tag_values
 
     @property
-    def path_to_series_description_json(self) -> Union[str, None]:
+    def path_to_tag_value_json(self) -> Union[str, None]:
         """
-        Path to series description json.
+        Path to tag values json.
 
         Returns
         -------
-        path_to_series_description_json : Union[str, None]
-            Path to the json dictionary that contains the series descriptions.
+        path_to_tag_value_json : Union[str, None]
+            Path to the json dictionary that contains the tag values.
         """
-        return self._path_to_series_description_json
+        return self._path_to_tag_value_json
 
-    @path_to_series_description_json.setter
-    def path_to_series_description_json(self, path_to_series_description_json: str) -> None:
+    @path_to_tag_value_json.setter
+    def path_to_tag_value_json(self, path_to_tag_value_json: str) -> None:
         """
-        Path to series description json setter. This is used to set the series descriptions attribute using the
+        Path to tag values json setter. This is used to set the tag values attribute using the
         dictionary read from the json file.
 
         Parameters
         ----------
-        path_to_series_description_json : str
-            Path to the json dictionary that contains the series descriptions.
+        path_to_tag_value_json : str
+            Path to the json dictionary that contains the tag values.
         """
-        with open(path_to_series_description_json, "r") as json_file:
-            self.series_descriptions = deepcopy(json.load(json_file))
+        with open(path_to_tag_value_json, "r") as json_file:
+            self.tag_values = deepcopy(json.load(json_file))
 
-        self._path_to_series_description_json = path_to_series_description_json
+        self._path_to_tag_value_json = path_to_tag_value_json
 
     @property
     def patients_who_failed(self) -> List[PatientWhoFailed]:
         """
         List of patients with one or more images not added to the HDF5 dataset due to the absence of the series in
         the patient record.
 
@@ -214,26 +219,26 @@
 
         Parameters
         ----------
         transforms : Union[Compose, DataTransform, MonaiMapTransform, PhysicalSpaceTransform]
             A sequence of transformations to apply. PhysicalSpaceTransform are applied in the physical space, i.e on
             the SimpleITK image, while MonaiMapTransform are applied in the array space, i.e on the numpy array that
             represents the image. DataTransform transforms the data using other a patient's other images or
-            segmentations. The keys for images are assumed to be the arbitrary series key set in 'series_descriptions'.
-            For segmentation, keys are organ names. Note that if 'series_descriptions' is None, the keys for images are
+            segmentations. The keys for images are assumed to be the arbitrary series key set in 'tag_values'.
+            For segmentation, keys are organ names. Note that if 'tag_values' is None, the keys for images are
             assumed to be modalities.
 
         Returns
         -------
         transforms : Union[Compose, DataTransform, MonaiMapTransform, PhysicalSpaceTransform]
             A sequence of transformations to apply. PhysicalSpaceTransform are applied in the physical space, i.e on
             the SimpleITK image, while MonaiMapTransform are applied in the array space, i.e on the numpy array that
             represents the image. DataTransform transforms the data using other a patient's other images or
-            segmentations. The keys for images are assumed to be the arbitrary series key set in 'series_descriptions'.
-            For segmentation, keys are organ names. Note that if 'series_descriptions' is None, the keys for images are
+            segmentations. The keys for images are assumed to be the arbitrary series key set in 'tag_values'.
+            For segmentation, keys are organ names. Note that if 'tag_values' is None, the keys for images are
             assumed to be modalities.
         """
         if transforms is None:
             return transforms
         elif isinstance(transforms, Compose):
             for t in transforms.transforms:
                 if not isinstance(t, (DataTransform, PhysicalSpaceTransform, MonaiMapTransform)):
@@ -248,25 +253,25 @@
             return transforms
         else:
             raise AssertionError(
                 "'transforms' must either be of type 'Compose', 'DataTransform', 'PhysicalSpaceTransform' or "
                 "'MonaiMapTransform'."
             )
 
-    def save_series_descriptions_to_json(self, path: str) -> None:
+    def save_tag_values_to_json(self, path: str) -> None:
         """
-        Saves the dictionary of series descriptions in a json format at the given path.
+        Saves the dictionary of tag values in a json format at the given path.
 
         Parameters
         ----------
         path : str
-            Path to the json dictionary that will contain the series descriptions.
+            Path to the json dictionary that will contain the tag values.
         """
         with open(path, 'w', encoding='utf-8') as json_file:
-            json.dump(self.series_descriptions, json_file, ensure_ascii=False, indent=4)
+            json.dump(self.tag_values, json_file, ensure_ascii=False, indent=4)
 
     def reset(self) -> None:
         """
         Resets the generator.
         """
         self._current_index = 0
         self._patients_who_failed = []
@@ -287,30 +292,31 @@
             self.throw()
 
         _logger.info(f"Downloading Patient {self._current_index + 1}/{len(self)}")
         _logger.info(f"Path to patient folder : {self.paths_to_patients_folders[self._current_index]}")
 
         patient_data_reader = PatientDataReader(
             path_to_patient_folder=self.paths_to_patients_folders[self._current_index],
-            series_descriptions=self.series_descriptions,
+            tag_values=self.tag_values,
+            tag=self.tag,
             erase_unused_dicom_files=self._erase_unused_dicom_files
         )
 
-        if self._series_descriptions is not None:
-            self.series_descriptions = patient_data_reader.series_descriptions
-        if self.path_to_series_description_json:
-            self.save_series_descriptions_to_json(path=self._path_to_series_description_json)
+        if self._tag_values is not None:
+            self.tag_values = patient_data_reader.tag_values
+        if self.path_to_tag_value_json:
+            self.save_tag_values_to_json(path=self._path_to_tag_value_json)
         if patient_data_reader.failed_images:
-            failed_images = {image: self.series_descriptions[image] for image in patient_data_reader.failed_images}
+            failed_images = {image: self.tag_values[image] for image in patient_data_reader.failed_images}
 
             self._patients_who_failed.append(
                 PatientWhoFailed(
                     id=patient_data_reader.patient_id,
                     failed_images=failed_images,
-                    available_series_descriptions=patient_data_reader.available_series_descriptions
+                    available_tag_values=patient_data_reader.available_tag_values
                 )
             )
 
         self._current_index += 1
 
         return patient_data_reader.get_patient_dataset(transforms=self._transforms)
```

### Comparing `delia-1.1.1/delia/radiomics/radiomics_dataset.py` & `delia-1.2.0/delia/radiomics/radiomics_dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -169,18 +169,18 @@
         ----------
         patients_data_extractor : PatientsDataExtractor
             An object used to iterate on multiple patients' dicom files and segmentation files using the
             PatientDataReader to obtain all patients' data.
         organ : str
             The organ specifies the segment of the mask from which the radiomics features are to be acquired.
         image_name : Optional[str]
-            Arbitrary name given to the image in the 'series_descriptions' dictionary. If 'series_descriptions' is
+            Arbitrary name given to the image in the 'tag_values' dictionary. If 'tag_values' is
             None, use 'image_modality'.
         image_modality : Optional[str]
-            Image modality. If 'series_descriptions' is NOT None, use 'image_name'.
+            Image modality. If 'tag_values' is NOT None, use 'image_name'.
         segmentation_modality_to_prioritize : str
             If there is multiple segmentation of the same organ for the same patient, this parameter sets the modality
             of the segmentation to prioritize, i.e. "SEG" or "RTSTRUCT". Default = "SEG".
         overwrite_dataset : bool
             Overwrite existing dataset, default = False.
         kwargs : {
             geometry_tolerance : float
```

### Comparing `delia-1.1.1/delia/readers/image/dicom_reader.py` & `delia-1.2.0/delia/readers/image/dicom_reader.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
                         folder.
 """
 
 from collections import defaultdict
 from glob import glob
 import logging
 import os
-from typing import Dict, List, NamedTuple, Set
+from typing import Dict, List, NamedTuple, Set, Tuple, Union
 
 import pydicom
 import SimpleITK as sitk
 
 from delia.utils.data_model import ImageDataModel
 from delia.readers.segmentation.segmentation_strategy import SegmentationStrategies
 from delia.utils.tools import is_path_valid
@@ -30,36 +30,40 @@
     A class used to read dicom files contained in a given folder.
     """
 
     UNKNOWN = "Unknown"
 
     class SeriesData(NamedTuple):
         """
-        Series description namedtuple to simplify management of values.
+        Tag value namedtuple to simplify management of values.
         """
-        series_description: str
+        tag_value: str
         paths_to_dicoms_from_series: List[str]
         dicom_header: pydicom.dataset.FileDataset
 
     def __init__(
             self,
-            path_to_patient_folder: str
+            path_to_patient_folder: str,
+            tag: Union[str, Tuple[int, int]]
     ):
         """
         Constructor of the class DicomReader.
 
         Parameters
         ----------
         path_to_patient_folder : str
             Path to the folder containing the patient DICOM files.
+        tag : Union[str, Tuple[int, int]]
+            Keyword or tuple of the DICOM tag to use while selecting which files to extract.
         """
         super(DicomReader, self).__init__()
 
         is_path_valid(path=path_to_patient_folder)
         self._path_to_patient_folder = path_to_patient_folder
+        self.tag = tag
 
         self._images_series_data_dict = {}
         self._segmentations_series_data_dict = {}
         self.__series_data_dict = self.__get_series_data_dict()
 
     @staticmethod
     def get_dicom_header(
@@ -85,30 +89,35 @@
 
         if show:
             _logger.info(loaded_dicom)
 
         return loaded_dicom
 
     @staticmethod
-    def _get_series_description(dicom_header: pydicom.FileDataset) -> str:
+    def _get_tag_value(dicom_header: pydicom.FileDataset, tag: Union[str, Tuple[int, int]]) -> str:
         """
-        Get Series Description of given DICOM header.
+        Get tag value of given DICOM header.
 
         Parameters
         ----------
         dicom_header : pydicom.dataset.FileDataset
             Loaded DICOM dataset.
+        tag : Union[str, Tuple[int, int]]
+            Keyword or tuple of the DICOM tag to use while selecting which files to extract.
 
         Returns
         -------
-        series_description : str
-            Series Description.
+        tag_value : str
+            tag value.
         """
-        if hasattr(dicom_header, "SeriesDescription"):
-            return dicom_header.SeriesDescription
+        if hasattr(dicom_header, tag):
+            if isinstance(dicom_header[tag].value, str):
+                return dicom_header[tag].value
+            else:
+                return dicom_header[tag].repval
         else:
             return DicomReader.UNKNOWN
 
     def __get_paths_to_dicoms_from_series(self, path_to_dicom_folder: str) -> Dict[str, List[str]]:
         """
         Get all series IDs from a patient's dicom folder.
 
@@ -160,15 +169,15 @@
         all_patient_ids: Set[str] = set()
         for series_id, paths in self.__get_paths_to_dicoms_from_series(self._path_to_patient_folder).items():
             path_to_first_dicom_of_series = paths[0]
             loaded_dicom_header = self.get_dicom_header(path_to_dicom=path_to_first_dicom_of_series)
             all_patient_ids.add(loaded_dicom_header.PatientID)
 
             series_data = self.SeriesData(
-                series_description=self._get_series_description(loaded_dicom_header),
+                tag_value=self._get_tag_value(loaded_dicom_header, self.tag),
                 paths_to_dicoms_from_series=paths,
                 dicom_header=loaded_dicom_header
             )
             series_data_dict[series_id] = series_data
 
         if len(all_patient_ids) == 0:
             raise AssertionError(f"The patient folder must contain DICOM files. This is not the case for the patient "
@@ -227,15 +236,15 @@
         """
         dicom_headers = []
         for idx, series_data in enumerate(self.__series_data_dict.values()):
             if idx == 0:
                 _logger.info(f"Patient ID : {series_data.dicom_header.PatientID}")
                 _logger.debug(f"Path to images folder : {self._path_to_patient_folder}")
 
-            _logger.debug(f"  Series description : {series_data.series_description}")
+            _logger.debug(f"  {self.tag} : {series_data.tag_value}")
 
             if not remove_segmentations:
                 dicom_headers.append(series_data.dicom_header)
             elif remove_segmentations:
                 if series_data.dicom_header.Modality not in SegmentationStrategies.get_available_modalities():
                     dicom_headers.append(series_data.dicom_header)
 
@@ -258,21 +267,21 @@
         -------
         image_data_list : List[ImageDataModel]
             A list of the patient's images data.
         """
         images_data = []
         for idx, series_data in enumerate(self.__series_data_dict.values()):
             if idx == 0:
-                _logger.info(f"Series description found in the patient's images folder :")
-            _logger.info(f"  Series description {idx + 1}: {series_data.series_description}")
+                _logger.info(f"Tag values found in the patient's images folder :")
+            _logger.info(f"  {self.tag} {idx + 1}: {series_data.tag_value}")
 
             if remove_segmentations and (series_data.dicom_header.Modality in
                                          SegmentationStrategies.get_available_modalities()):
                 pass
-            elif series_data.series_description == DicomReader.UNKNOWN:
+            elif series_data.tag_value == DicomReader.UNKNOWN:
                 pass
             else:
                 try:
                     image = self.__get_3d_sitk_image_from_dicom_series(
                         paths_to_dicoms_from_series=series_data.paths_to_dicoms_from_series
                     )
 
@@ -283,11 +292,11 @@
                     )
 
                     images_data.append(image_data)
 
                 except RuntimeError as e:
                     _logger.error(
                         f"      RuntimeError : {e}. Simple ITK raised an error while loading the series named "
-                        f"{series_data.series_description}. This series is therefore ignored."
+                        f"{series_data.tag_value}. This series is therefore ignored."
                     )
 
         return images_data
```

### Comparing `delia-1.1.1/delia/readers/patient_data/factories/base_patient_data_factory.py` & `delia-1.2.0/delia/readers/patient_data/factories/base_patient_data_factory.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     @Description:       This file contains the class BasePatientDataFactory that is used as an abstract class used as a
                         reference for all other patient data factories.
 """
 
 from abc import ABC, abstractmethod
 from os import remove
-from typing import Dict, List, Optional
+from typing import Dict, List, Optional, Tuple, Union
 
 import pydicom
 
 from delia.readers.image.dicom_reader import DicomReader
 from delia.utils.data_model import ImageDataModel, PatientDataModel
 
 
@@ -24,39 +24,43 @@
     An abstract class that is used as a reference for all other patient data factories.
     """
 
     def __init__(
             self,
             path_to_patient_folder: str,
             paths_to_segmentations: Optional[List[str]],
-            series_descriptions: Optional[Dict[str, List[str]]],
+            tag_values: Optional[Dict[str, List[str]]],
+            tag: Union[str, Tuple[int, int]],
             erase_unused_dicom_files: bool = False
     ):
         """
         Constructor of the class BasePatientDataFactory.
 
         Parameters
         ----------
         path_to_patient_folder : str
             Path to the folder containing the patient's image files.
         paths_to_segmentations : Optional[List[str]]
             List of paths to the patient's segmentation files.
-        series_descriptions : Optional[Dict[str, List[str]]]
-            A dictionary that contains the series descriptions of the images that absolutely needs to be extracted from
-            the patient's file. Keys are arbitrary names given to the images we want to add and values are lists of
-            series descriptions.
+        tag_values : Optional[Dict[str, List[str]]]
+            A dictionary that contains the desired tag's values for the images that absolutely needs to be extracted
+            from the patient's file. Keys are arbitrary names given to the images we want to add and values are lists of
+            values associated with the specified tag.
+        tag : Union[str, Tuple[int, int]]
+            Keyword or tuple of the DICOM tag to use while selecting which files to extract.
         erase_unused_dicom_files: bool = False
             Whether to delete unused DICOM files or not. Use with caution.
         """
         self._path_to_patient_folder = path_to_patient_folder
         self._paths_to_segmentations = paths_to_segmentations
-        self._series_descriptions = series_descriptions
+        self._tag_values = tag_values
         self._erase_unused_dicom_files = erase_unused_dicom_files
+        self.tag = tag
 
-        dicom_reader = DicomReader(path_to_patient_folder=self._path_to_patient_folder)
+        dicom_reader = DicomReader(path_to_patient_folder=self._path_to_patient_folder, tag=self.tag)
         self._images_data = dicom_reader.get_images_data(remove_segmentations=True)
 
     @property
     def patient_id(self) -> str:
         """
         Patient ID.
```

### Comparing `delia-1.1.1/delia/readers/patient_data/factories/patient_data_factories.py` & `delia-1.2.0/delia/readers/patient_data/factories/patient_data_factories.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
     @Creation Date:     01/2022
     @Last modification: 03/2022
 
     @Description:       This file contains all factories that inherit from the BasePatientDataFactory class.
 """
 
-from typing import Dict, List, Optional
+from typing import Dict, List, Optional, Tuple, Union
 
 from delia.readers.patient_data.factories.base_patient_data_factory import BasePatientDataFactory
 from delia.readers.image.dicom_reader import DicomReader
 from delia.readers.segmentation.segmentation_reader import SegmentationReader
 from delia.utils.data_model import ImageAndSegmentationDataModel, PatientDataModel
 
 
@@ -22,37 +22,41 @@
     the images.
     """
 
     def __init__(
             self,
             path_to_patient_folder: str,
             paths_to_segmentations: Optional[List[str]],
-            series_descriptions: Optional[Dict[str, List[str]]],
+            tag_values: Optional[Dict[str, List[str]]],
+            tag: Union[str, Tuple[int, int]],
             erase_unused_dicom_files: bool = False
     ):
         """
         Constructor of the class DefaultPatientDataFactory.
 
         Parameters
         ----------
         path_to_patient_folder : str
             Path to the folder containing the patient's image files.
         paths_to_segmentations : Optional[List[str]]
             List of paths to the patient's segmentation files.
-        series_descriptions : Optional[Dict[str, List[str]]]
-            A dictionary that contains the series descriptions of the images that absolutely needs to be extracted from
-            the patient's file. Keys are arbitrary names given to the images we want to add and values are lists of
-            series descriptions.
+        tag_values : Optional[Dict[str, List[str]]]
+            A dictionary that contains the desired tag's values for the images that absolutely needs to be extracted
+            from the patient's file. Keys are arbitrary names given to the images we want to add and values are lists of
+            values associated with the specified tag.
+        tag : Union[str, Tuple[int, int]]
+            Keyword or tuple of the DICOM tag to use while selecting which files to extract.
         erase_unused_dicom_files: bool = False
             Whether to delete unused DICOM files or not. Use with caution.
         """
         super().__init__(
             path_to_patient_folder=path_to_patient_folder,
             paths_to_segmentations=paths_to_segmentations,
-            series_descriptions=series_descriptions,
+            tag_values=tag_values,
+            tag=tag,
             erase_unused_dicom_files=erase_unused_dicom_files
         )
 
     def create_patient_data(self) -> PatientDataModel:
         """
         Creates a tuple containing all the patient's data.
 
@@ -91,45 +95,49 @@
             data=data
         )
         return patient_data
 
 
 class SeriesDescriptionPatientDataFactory(BasePatientDataFactory):
     """
-    Class that defines the methods that are used to get the patient data. The series description patient data factory
-    consists in obtaining only the images that have the given series descriptions and their corresponding segmentations.
+    Class that defines the methods that are used to get the patient data. The tag value patient data factory
+    consists in obtaining only the images that have the given tag's desired value and their corresponding segmentations.
     """
 
     def __init__(
             self,
             path_to_patient_folder: str,
             paths_to_segmentations: Optional[List[str]],
-            series_descriptions: Optional[Dict[str, List[str]]],
+            tag_values: Optional[Dict[str, List[str]]],
+            tag: Union[str, Tuple[int, int]],
             erase_unused_dicom_files: bool = False
     ):
         """
         Constructor of the class SeriesDescriptionPatientDataFactory.
 
         Parameters
         ----------
         path_to_patient_folder : str
             Path to the folder containing the patient's image files.
         paths_to_segmentations : Optional[List[str]]
             List of paths to the patient's segmentation files.
-        series_descriptions : Optional[Dict[str, List[str]]]
-            A dictionary that contains the series descriptions of the images that absolutely needs to be extracted from
-            the patient's file. Keys are arbitrary names given to the images we want to add and values are lists of
-            series descriptions.
+        tag_values : Optional[Dict[str, List[str]]]
+            A dictionary that contains the desired tag's values for the images that absolutely needs to be extracted
+            from the patient's file. Keys are arbitrary names given to the images we want to add and values are lists of
+            values associated with the specified tag.
+        tag : Union[str, Tuple[int, int]]
+            Keyword or tuple of the DICOM tag to use while selecting which files to extract.
         erase_unused_dicom_files: bool = False
             Whether to delete unused DICOM files or not. Use with caution.
         """
         super().__init__(
             path_to_patient_folder=path_to_patient_folder,
             paths_to_segmentations=paths_to_segmentations,
-            series_descriptions=series_descriptions,
+            tag_values=tag_values,
+            tag=tag,
             erase_unused_dicom_files=erase_unused_dicom_files
         )
 
     def create_patient_data(self) -> PatientDataModel:
         """
         Creates a tuple containing all the patient's data.
 
@@ -137,18 +145,20 @@
         -------
         patient_data: PatientDataModel
             Patient data.
         """
         data = []
         for image_idx, image in enumerate(self._images_data):
             image_added = False
-            series_description = image.dicom_header.SeriesDescription
-
-            for series_key, list_of_series_descriptions in self._series_descriptions.items():
-                if series_description in list_of_series_descriptions:
+            if isinstance(image.dicom_header[self.tag].value, str):
+                tag_value = image.dicom_header[self.tag].value
+            else:
+                tag_value = image.dicom_header[self.tag].repval
+            for series_key, list_of_tag_values in self._tag_values.items():
+                if tag_value in list_of_tag_values:
                     image.series_key = series_key
 
                     segmentations = []
                     for path_to_segmentation in self._paths_to_segmentations:
                         seg_header = DicomReader.get_dicom_header(path_to_dicom=path_to_segmentation)
                         reference_uid = self.get_segmentation_reference_uid(seg_header)
```

### Comparing `delia-1.1.1/delia/readers/patient_data/patient_data_query_context.py` & `delia-1.2.0/delia/readers/patient_data/patient_data_query_context.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     @Creation Date:     01/2022
     @Last modification: 03/2022
 
     @Description:       This file contains the class PatientDataQueryContext that is used as a context class where
                         strategies are types of requests the client could ask the PatientDataReader class.
 """
 
-from typing import Dict, List, Optional
+from typing import Dict, List, Optional, Tuple, Union
 
 from delia.utils.data_model import PatientDataModel
 from .patient_data_query_strategy import PatientDataQueryStrategy, PatientDataQueryStrategies
 
 
 class PatientDataQueryContext:
     """
@@ -21,50 +21,54 @@
     PatientDataReader class to get the patient's data.
     """
 
     def __init__(
             self,
             path_to_patient_folder: str,
             paths_to_segmentations: Optional[List[str]],
-            series_descriptions: Dict[str, List[str]],
+            tag_values: Dict[str, List[str]],
+            tag: Union[str, Tuple[int, int]],
             erase_unused_dicom_files: bool = False
     ):
         """
         Constructor of the PatientDataQueryContext class.
 
         Parameters
         ----------
         path_to_patient_folder : str
             Path to the folder containing the patient's DICOM files.
         paths_to_segmentations : Optional[List[str]]
             List of paths to the patient's segmentation files.
-        series_descriptions : Dict[str, List[str]]
-            A dictionary that contains the series descriptions of the images that absolutely needs to be extracted from
-            the patient's file. Keys are arbitrary names given to the images we want to add and values are lists of
-            series descriptions.
+        tag_values : Dict[str, List[str]]
+            A dictionary that contains the desired tag's values for the images that absolutely needs to be extracted
+            from the patient's file. Keys are arbitrary names given to the images we want to add and values are lists of
+            values associated with the specified tag.
+        tag : Union[str, Tuple[int, int]]
+            Keyword or tuple of the DICOM tag to use while selecting which files to extract.
         erase_unused_dicom_files: bool = False
             Whether to delete unused DICOM files or not. Use with caution.
         """
         self._path_to_patient_folder = path_to_patient_folder
         self._paths_to_segmentations = paths_to_segmentations
-        self._series_descriptions = series_descriptions
+        self._tag_values = tag_values
         self._erase_unused_dicom_files = erase_unused_dicom_files
+        self.tag = tag
 
     @property
     def patient_data_query_strategy(self) -> PatientDataQueryStrategy:
         """
-        Patient data query strategy corresponding to the given series descriptions configuration.
+        Patient data query strategy corresponding to the given tag values configuration.
 
         Returns
         -------
         patient_data_query_strategy : PatientDataQueryStrategy
             Patient data query strategy.
         """
-        if self._series_descriptions:
-            return PatientDataQueryStrategies.SERIES_DESCRIPTION.value
+        if self._tag_values:
+            return PatientDataQueryStrategies.TAG_VALUE.value
         else:
             return PatientDataQueryStrategies.DEFAULT.value
 
     @property
     def _patient_data_factory_instance(self) -> PatientDataQueryStrategy.factory:
         """
         The factory class instance corresponding to the class of the given patient data strategy.
@@ -73,15 +77,16 @@
         -------
         _patient_data_factory_instance : PatientDataQueryStrategy.factory
             Factory class instance used to get a patient's data.
         """
         patient_data_factory_instance = self.patient_data_query_strategy.factory(
             path_to_patient_folder=self._path_to_patient_folder,
             paths_to_segmentations=self._paths_to_segmentations,
-            series_descriptions=self._series_descriptions,
+            tag_values=self._tag_values,
+            tag=self.tag,
             erase_unused_dicom_files=self._erase_unused_dicom_files
         )
 
         return patient_data_factory_instance
 
     def create_patient_data(self) -> PatientDataModel:
         """
```

### Comparing `delia-1.1.1/delia/readers/patient_data/patient_data_query_strategy.py` & `delia-1.2.0/delia/readers/patient_data/patient_data_query_strategy.py`

 * *Files 21% similar despite different names*

```diff
@@ -23,12 +23,11 @@
 class PatientDataQueryStrategies(Enum):
 
     DEFAULT = PatientDataQueryStrategy(
         name="Default",
         factory=DefaultPatientDataFactory
     )
 
-    SERIES_DESCRIPTION = PatientDataQueryStrategy(
-        name="Series description",
+    TAG_VALUE = PatientDataQueryStrategy(
+        name="Tag value",
         factory=SeriesDescriptionPatientDataFactory
     )
-
```

### Comparing `delia-1.1.1/delia/readers/segmentation/factories/base_segmentation_factory.py` & `delia-1.2.0/delia/readers/segmentation/factories/base_segmentation_factory.py`

 * *Files identical despite different names*

### Comparing `delia-1.1.1/delia/readers/segmentation/factories/dicom_segmentation_factories.py` & `delia-1.2.0/delia/readers/segmentation/factories/dicom_segmentation_factories.py`

 * *Files identical despite different names*

### Comparing `delia-1.1.1/delia/readers/segmentation/factories/segment.py` & `delia-1.2.0/delia/readers/segmentation/factories/segment.py`

 * *Files identical despite different names*

### Comparing `delia-1.1.1/delia/readers/segmentation/factories/segmentation.py` & `delia-1.2.0/delia/readers/segmentation/factories/segmentation.py`

 * *Files identical despite different names*

### Comparing `delia-1.1.1/delia/readers/segmentation/segmentation_context.py` & `delia-1.2.0/delia/readers/segmentation/segmentation_context.py`

 * *Files identical despite different names*

### Comparing `delia-1.1.1/delia/readers/segmentation/segmentation_reader.py` & `delia-1.2.0/delia/readers/segmentation/segmentation_reader.py`

 * *Files identical despite different names*

### Comparing `delia-1.1.1/delia/readers/segmentation/segmentation_strategy.py` & `delia-1.2.0/delia/readers/segmentation/segmentation_strategy.py`

 * *Files identical despite different names*

### Comparing `delia-1.1.1/delia/transforms/applications.py` & `delia-1.2.0/delia/transforms/applications.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,16 +42,16 @@
     patient_dataset : PatientDataModel
         A named tuple grouping the patient's data extracted from its DICOM files and the patient's medical image
         segmentation data extracted from the segmentation files.
     transforms : Union[Compose, DataTransform, MonaiMapTransform, PhysicalSpaceTransform]
         A sequence of transformations to apply. PhysicalSpaceTransform are applied in the physical space, i.e on the
         SimpleITK image, while MonaiMapTransform are applied in the array space, i.e on the numpy array that represents
         the image. DataTransform transforms the data using other a patient's other images or segmentations. The keys
-        for images are assumed to be the arbitrary series key set in 'series_descriptions'. For segmentation, keys are
-        organ names. Note that if 'series_descriptions' is None, the keys for images are assumed to be modalities.
+        for images are assumed to be the arbitrary series key set in 'tag_values'. For segmentation, keys are
+        organ names. Note that if 'tag_values' is None, the keys for images are assumed to be modalities.
     """
     set_transforms_keys(patient_dataset=patient_dataset)
 
     if isinstance(transforms, Compose):
         for t in transforms.transforms:
             if isinstance(t, DataTransform):
                 _apply_data_transform(
@@ -117,16 +117,16 @@
     ----------
     patient_dataset : PatientDataModel
         A named tuple grouping the patient's data extracted from its DICOM files and the patient's medical image
         segmentation data extracted from the segmentation files.
     transform : Union[MonaiMapTransform, PhysicalSpaceTransform]
         A transformation to apply on images. PhysicalSpaceTransform are applied in the physical space, i.e on the
         SimpleITK image, while MonaiMapTransform are applied in the array space, i.e on the numpy array that represents
-        the image. The keys for images are assumed to be the arbitrary series key set in 'series_descriptions'. For
-        segmentation, keys are organ names. Note that if 'series_descriptions' is None, the keys for images are
+        the image. The keys for images are assumed to be the arbitrary series key set in 'tag_values'. For
+        segmentation, keys are organ names. Note that if 'tag_values' is None, the keys for images are
         assumed to be modalities.
     """
     images = {
         data.image.transforms_key: ImageData(
             simple_itk_image=data.image.simple_itk_image,
             dicom_header=data.image.dicom_header
         )
@@ -150,16 +150,16 @@
     ----------
     patient_dataset : PatientDataModel
         A named tuple grouping the patient's data extracted from its DICOM files and the patient's medical image
         segmentation data extracted from the segmentation files.
     transform : Union[MonaiMapTransform, PhysicalSpaceTransform]
         A transformation to apply on segmentations. PhysicalSpaceTransform are applied in the physical space, i.e on the
         SimpleITK image, while MonaiMapTransform are applied in the array space, i.e on the numpy array that represents
-        the image. Image keys are assumed to be arbitrary series keys defined in 'series_descriptions'. For the
-        label maps, the keys are organ names. Note that if 'series_descriptions' is None, the image keys are
+        the image. Image keys are assumed to be arbitrary series keys defined in 'tag_values'. For the
+        label maps, the keys are organ names. Note that if 'tag_values' is None, the image keys are
         assumed to be modality names.
     """
     images = {
         data.image.transforms_key: ImageData(
             simple_itk_image=data.image.simple_itk_image,
             dicom_header=data.image.dicom_header
         )
@@ -194,16 +194,16 @@
     Parameters
     ----------
     data : Dict[str, ImageData]
         A Python dictionary that contains ImageData to be transformed.
     transform : Union[MonaiMapTransform, PhysicalSpaceTransform]
         A transformation to apply. PhysicalSpaceTransform are applied in the physical space, i.e on the SimpleITK image,
         while MonaiMapTransform are applied in the array space, i.e on the numpy array that represents the image. The
-        keys for images are assumed to be the arbitrary series key set in 'series_descriptions'. For segmentation,
-        keys are organ names. Note that if 'series_descriptions' is None, the keys for images are assumed to be
+        keys for images are assumed to be the arbitrary series key set in 'tag_values'. For segmentation,
+        keys are organ names. Note that if 'tag_values' is None, the keys for images are assumed to be
         modalities.
     mode : Mode
         The mode.
 
     Returns
     -------
     transformed_data : Dict[Hashable, sitk.Image]
```

### Comparing `delia-1.1.1/delia/transforms/array_space/matching_centroid_spatial_crop.py` & `delia-1.2.0/delia/transforms/array_space/matching_centroid_spatial_crop.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         ----------
         segmentation_key : str
             Key of the segmentation from which to crop around the centroid and to get coordinates of the spatial
             bounding box. Segmentation keys are organ names.
         matching_keys : KeysCollection
             Keys of the corresponding items to be transformed using the calculated coordinates of the spatial bounding
             box around the centroid of the segmentation. Image keys are assumed to be arbitrary series keys defined in
-            'series_descriptions'. For the label maps, the keys are organ names. Note that if 'series_descriptions' is
+            'tag_values'. For the label maps, the keys are organ names. Note that if 'tag_values' is
             None, the image keys are assumed to be modality names.
         roi_size : Union[Sequence[int], int]
             The size of the crop region e.g. [224,224,128]. If a dimension of ROI size is larger than image size, will
             not crop that dimension of the image. If its components have non-positive values, the corresponding size of
             input image will be used. For example: if the spatial size of input data is [40, 40, 40] and
             `roi_size=[32, 64, -1]`, the spatial size of output data will be [32, 40, 40].
         """
```

### Comparing `delia-1.1.1/delia/transforms/array_space/matching_crop_foreground.py` & `delia-1.2.0/delia/transforms/array_space/matching_crop_foreground.py`

 * *Files 17% similar despite different names*

```diff
@@ -32,20 +32,20 @@
         """
         Initialize output spacing.
 
         Parameters
         ----------
         reference_image_key : str
             Key of the image from which to crop foreground and to get coordinates of spatial bounding box for
-            foreground. Image keys are assumed to be arbitrary series keys defined in 'series_descriptions'. Note that
-            if 'series_descriptions' is None, the image keys are assumed to be modality names.
+            foreground. Image keys are assumed to be arbitrary series keys defined in 'tag_values'. Note that
+            if 'tag_values' is None, the image keys are assumed to be modality names.
         matching_keys : KeysCollection
             Keys of the corresponding items to be transformed using the calculated coordinates of spatial bounding box
             for foreground on the image. Image keys are assumed to be arbitrary series keys defined in
-            'series_descriptions'. For the label maps, the keys are organ names. Note that if 'series_descriptions' is
+            'tag_values'. For the label maps, the keys are organ names. Note that if 'tag_values' is
             None, the image keys are assumed to be modality names.
         """
         keys = [key for key in matching_keys] + [reference_image_key]
         super().__init__(keys=keys)
 
         self._reference_image_key = reference_image_key
         self._crop_foreground = CropForeground(return_coords=True)
```

### Comparing `delia-1.1.1/delia/transforms/array_space/tools.py` & `delia-1.2.0/delia/transforms/array_space/tools.py`

 * *Files identical despite different names*

### Comparing `delia-1.1.1/delia/transforms/array_space/transform.py` & `delia-1.2.0/delia/transforms/array_space/transform.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,16 +29,16 @@
         """
         Initialize transform keys.
 
         Parameters
         ----------
         keys : KeysCollection
             Keys of the corresponding items to be transformed. Image keys are assumed to be arbitrary series keys
-            defined in 'series_descriptions'. For the label maps, the keys are organ names. Note that if
-            'series_descriptions' is None, the image keys are assumed to be modality names.
+            defined in 'tag_values'. For the label maps, the keys are organ names. Note that if
+            'tag_values' is None, the image keys are assumed to be modality names.
         """
         super().__init__(keys=keys, allow_missing_keys=True)
         self._mode = Mode.NONE
 
     @property
     def mode(self) -> Mode:
         """
```

### Comparing `delia-1.1.1/delia/transforms/data/copy_segmentations.py` & `delia-1.2.0/delia/transforms/data/copy_segmentations.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,19 +31,19 @@
         """
         Initialize transform.
 
         Parameters
         ----------
         segmented_image_key : str
             Key of the segmented image from which to copy the segmentations. Image keys are assumed to be arbitrary
-            series keys defined in 'series_descriptions'. Note that if 'series_descriptions' is None, the image keys
+            series keys defined in 'tag_values'. Note that if 'tag_values' is None, the image keys
             are assumed to be modality names.
         unsegmented_image_key : str
             Key of the unsegmented image on which to copy the segmentations. Image keys are assumed to be arbitrary
-            series keys defined in 'series_descriptions'. Note that if 'series_descriptions' is None, the image keys
+            series keys defined in 'tag_values'. Note that if 'tag_values' is None, the image keys
             are assumed to be modality names.
         """
         super().__init__(keys=[segmented_image_key, unsegmented_image_key])
 
         self._segmented_image_key = segmented_image_key
         self._unsegmented_image_key = unsegmented_image_key
```

### Comparing `delia-1.1.1/delia/transforms/data/transform.py` & `delia-1.2.0/delia/transforms/data/transform.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,16 +28,16 @@
         """
         Initialize transform keys.
 
         Parameters
         ----------
         keys : KeysCollection
             Keys of the corresponding items to be transformed. Image keys are assumed to be arbitrary series keys
-            defined in 'series_descriptions'. For the label maps, the keys are organ names. Note that if
-            'series_descriptions' is None, the image keys are assumed to be modality names.
+            defined in 'tag_values'. For the label maps, the keys are organ names. Note that if
+            'tag_values' is None, the image keys are assumed to be modality names.
         """
         super().__init__(keys=keys, allow_missing_keys=True)
 
     @abstractmethod
     def __call__(self, data: Dict[str, ImageAndSegmentationDataModel]) -> Dict[Hashable, ImageAndSegmentationDataModel]:
         """
         Apply the transformation.
```

### Comparing `delia-1.1.1/delia/transforms/physical_space/matching_resample.py` & `delia-1.2.0/delia/transforms/physical_space/matching_resample.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         Parameters
         ----------
         reference_image_key : str
             Key of the image from which the spacing, size, origin and direction are taken.
         matching_keys : KeysCollection
             Keys of the corresponding items to be transformed using the calculated coordinates of spatial bounding box
             for foreground on the image. Image keys are assumed to be arbitrary series keys defined in
-            'series_descriptions'. For the label maps, the keys are organ names. Note that if 'series_descriptions' is
+            'tag_values'. For the label maps, the keys are organ names. Note that if 'tag_values' is
             None, the image keys are assumed to be modality names.
         interpolator : Callable
             The interpolator to be used for resampling the images. Default = sitk.sitkBSpline.
         """
         keys = [key for key in matching_keys] + [reference_image_key]
         super().__init__(keys=keys)
         self._reference_image_key = reference_image_key
```

### Comparing `delia-1.1.1/delia/transforms/physical_space/pet_to_suv.py` & `delia-1.2.0/delia/transforms/physical_space/pet_to_suv.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,16 +42,16 @@
         """
         Initialize transform.
 
         Parameters
         ----------
         keys : KeysCollection
             Keys of the corresponding items to be transformed. Image keys are assumed to be arbitrary series keys
-            defined in 'series_descriptions'. For the label maps, the keys are organ names. Note that if
-            'series_descriptions' is None, the image keys are assumed to be modality names.
+            defined in 'tag_values'. For the label maps, the keys are organ names. Note that if
+            'tag_values' is None, the image keys are assumed to be modality names.
         """
         super().__init__(keys=keys)
 
     @staticmethod
     def get_patient_weight(header: pydicom.dataset.FileDataset) -> float:
         """
         Get patient weight or estimate it.
```

### Comparing `delia-1.1.1/delia/transforms/physical_space/resample.py` & `delia-1.2.0/delia/transforms/physical_space/resample.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,16 +30,16 @@
         """
         Initialize output spacing.
 
         Parameters
         ----------
         keys : KeysCollection
             Keys of the corresponding items to be transformed. Image keys are assumed to be arbitrary series keys
-            defined in 'series_descriptions'. For the label maps, the keys are organ names. Note that if
-            'series_descriptions' is None, the image keys are assumed to be modality names.
+            defined in 'tag_values'. For the label maps, the keys are organ names. Note that if
+            'tag_values' is None, the image keys are assumed to be modality names.
         out_spacing : Tuple[int, int, int], default = (1.0, 1.0, 1.0)
             The desired spacing in the physical space. Default = (1.0 mm, 1.0 mm, 1.0 mm).
         interpolator : Callable
             The interpolator to be used for resampling the images. Default = sitk.sitkBSpline.
         """
         super().__init__(keys=keys)
         self._out_spacing = out_spacing
```

### Comparing `delia-1.1.1/delia/transforms/physical_space/transform.py` & `delia-1.2.0/delia/transforms/physical_space/transform.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,16 +45,16 @@
         """
         Initialize transform keys.
 
         Parameters
         ----------
         keys : KeysCollection
             Keys of the corresponding items to be transformed. Image keys are assumed to be arbitrary series keys
-            defined in 'series_descriptions'. For the label maps, the keys are organ names. Note that if
-            'series_descriptions' is None, the image keys are assumed to be modality names.
+            defined in 'tag_values'. For the label maps, the keys are organ names. Note that if
+            'tag_values' is None, the image keys are assumed to be modality names.
         """
         super().__init__(keys=keys, allow_missing_keys=True)
         self._mode = Mode.NONE
 
     @property
     def mode(self) -> Mode:
         """
```

### Comparing `delia-1.1.1/delia/transforms/tools.py` & `delia-1.2.0/delia/transforms/tools.py`

 * *Files 19% similar despite different names*

```diff
@@ -42,17 +42,17 @@
             raise AssertionError(f"Series key {series_key} already in dict. To use 'transforms', there must be only "
                                  f"one image associated to a given series key.")
         elif series_key:
             image_and_segmentation_data.image.transforms_key = series_key
             keys.append(series_key)
         elif modality in keys:
             raise AssertionError(f"Modality {modality} already in dict. To use 'transforms' without using "
-                                 f"'series_descriptions', there must be only one image associated to a given modality. "
-                                 f"Otherwise, use 'series_descriptions' to specify the images' names as keys in the"
-                                 f"'series_descriptions' dictionary.")
+                                 f"'tag_values', there must be only one image associated to a given modality. "
+                                 f"Otherwise, use 'tag_values' to specify the images' names as keys in the"
+                                 f"'tag_values' dictionary.")
         else:
             image_and_segmentation_data.image.transforms_key = modality
             keys.append(modality)
 
 
 def convert_to_numpy(array: Union[MetaTensor, np.ndarray]) -> np.ndarray:
     """
```

### Comparing `delia-1.1.1/delia/utils/data_model.py` & `delia-1.2.0/delia/utils/data_model.py`

 * *Files identical despite different names*

### Comparing `delia-1.1.1/delia/utils/tools.py` & `delia-1.2.0/delia/utils/tools.py`

 * *Files identical despite different names*

### Comparing `delia-1.1.1/delia/utils/transforms_history.py` & `delia-1.2.0/delia/utils/transforms_history.py`

 * *Files identical despite different names*

### Comparing `delia-1.1.1/delia.egg-info/PKG-INFO` & `delia-1.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: delia
-Version: 1.1.1
-Summary: DICOM Extraction for Large-scale Image Analysis (DELIA).
-Home-page: https://github.com/MaxenceLarose/delia
-Author: Maxence Larose
-Author-email: maxence.larose.1@ulaval.ca
-License: Apache License 2.0
-Keywords: dicom hdf5 medical image segmentation pre-processing python3 radiomics deep-learning dicom-seg rt-struct
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <p align="center" width="100%">
     <img width="100%" src="https://github.com/MaxenceLarose/delia/raw/main/images/logo/delia_banner.svg">
 </p>
 <p align="center"><i>DELIA facilitates data extraction from DICOM files to support large-scale image analysis workflows.</i></p>
 
 # Notable features
 
@@ -109,34 +93,34 @@
 
 ### File format
 
 Images files must be in standard [**DICOM**](https://www.dicomstandard.org/) format and segmentation files must be in [DICOM-SEG](https://dicom.nema.org/medical/dicom/current/output/chtml/part03/sect_C.8.20.html) or [RTStruct](https://dicom.nema.org/dicom/2013/output/chtml/part03/sect_A.19.html) format.
 
 If your segmentation files are in a research file format (`.nrrd`, `.nii`, etc.), you need to convert them into the standardized [DICOM-SEG](https://dicom.nema.org/medical/dicom/current/output/chtml/part03/sect_C.8.20.html) or [RTStruct](https://dicom.nema.org/dicom/2013/output/chtml/part03/sect_A.19.html) format. You can use the [pydicom-seg](https://pypi.org/project/pydicom-seg/) library to create the DICOM-SEG files OR use the [itkimage2dicomSEG](https://github.com/MaxenceLarose/itkimage2dicomSEG) python module, which provide a complete pipeline to perform this conversion. Also, you can use the [RT-Utils](https://github.com/qurit/rt-utils) library to create the RTStruct files.
 
-### Series descriptions (Optional)
+### Tag values (Optional)
 
-*This dictionary is **not** mandatory for the code to work and therefore its default value is `None`. Note that if no `series_descriptions` dictionary is given, i.e. `series_descriptions = None`, then all images will be added to the database.*
+*This dictionary is **not** mandatory for the code to work and therefore its default value is `None`. Note that if no `tag_values` dictionary is given, i.e. `tag_values = None`, then all images will be added to the database.*
 
-The series descriptions are specified as a **dictionary** that contains the series descriptions of the images that needs to be extracted from the patients' files. Keys are arbitrary names given to the images we want to add and values are lists of series descriptions. The images associated with these series descriptions do not need to have a corresponding segmentation volume. If none of the descriptions match the series in a patient's files, a warning is raised and the patient is added to the list of patients for whom the pipeline has failed.
+The tag values are specified as a **dictionary** that contains the values for the tag specified when creating the PatientsDataExtractor object of the images that need to be extracted from the patients' files. Keys are arbitrary names given to the images we want to add and values are lists of values for the desired tag. The images associated with these tag values do not need to have a corresponding segmentation volume. If none of the descriptions match the series in a patient's files, a warning is raised and the patient is added to the list of patients for whom the pipeline has failed.
 
-Note that the series descriptions can be specified as a classic dictionary or as a path to a **json file** that contains the series descriptions. Both methods are presented below.
+Note that the tag values can be specified as a python dictionary or as a path to a **json file** that contains the desired values. Both methods are presented below.
 
 <details>
   <summary>Using a json file</summary>
 
-Create a json file containing only the dictionary of the names given to the images we want to add (keys) and lists of series descriptions (values). Place this file in your data folder.
+Create a json file containing only the dictionary of the names given to the images we want to add (keys) and lists of tag values (values). Place this file in your data folder.
 
 Here is an example of a json file configured as expected :
 
 ```json
 {
-    "TEP": [
-        "TEP WB CORR (AC)",
-        "TEP WB XL CORR (AC)"
+    "PT": [
+        "PT WB CORR (AC)",
+        "PT WB XL CORR (AC)"
     ],
     "CT": [
         "CT 2.5 WB",
         "AC CT 2.5 WB"
     ]
 }
 ```
@@ -146,18 +130,18 @@
   <summary>Using a Python dictionary</summary>
 
 Create the organs dictionary in your main.py python file.
 
 Here is an example of a python dictionary instanced as expected :
 
 ```python
-series_descriptions = {
-    "TEP": [
-        "TEP WB CORR (AC)",
-        "TEP WB XL CORR (AC)"
+tag_values = {
+    "PT": [
+        "PT WB CORR (AC)",
+        "PT WB XL CORR (AC)"
     ],
     "CT": [
         "CT 2.5 WB",
         "AC CT 2.5 WB"
     ]
 }
 ```
@@ -167,15 +151,15 @@
 
 It is important to configure the directory structure correctly to ensure that the module interacts correctly with the data files. The `patients` folder, must be structured as follows. *Note that all DICOM files in the patients' folder will be read.*
 
 ```
 |_📂 Project directory/
   |_📄 main.py
   |_📂 data/
-    |_📄 series_descriptions.json
+    |_📄 tag_values.json
     |_📂 patients/
       |_📂 patient1/
        	|_📄 ...
        	|_📂 ...
       |_📂 patient2/
        	|_📄 ...
        	|_📂 ...
@@ -216,23 +200,23 @@
     Compose,
     ScaleIntensityD,
     ThresholdIntensityD
 )
 
 patients_data_extractor = PatientsDataExtractor(
     path_to_patients_folder="data/patients",
-    series_descriptions="data/series_descriptions.json",
+    tag_values="data/tag_values.json",
     transforms=Compose(
         [
-            ResampleD(keys=["CT_THORAX", "TEP", "Heart"], out_spacing=(1.5, 1.5, 1.5)),
-            CenterSpatialCropD(keys=["CT_THORAX", "TEP", "Heart"], roi_size=(1000, 160, 160)),
+            ResampleD(keys=["CT_THORAX", "PT", "Heart"], out_spacing=(1.5, 1.5, 1.5)),
+            CenterSpatialCropD(keys=["CT_THORAX", "PT", "Heart"], roi_size=(1000, 160, 160)),
             ThresholdIntensityD(keys=["CT_THORAX"], threshold=-250, above=True, cval=-250),
             ThresholdIntensityD(keys=["CT_THORAX"], threshold=500, above=False, cval=500),
             ScaleIntensityD(keys=["CT_THORAX"], minv=0, maxv=1),
-            PETtoSUVD(keys=["TEP"])
+            PETtoSUVD(keys=["PT"])
         ]
     )
 )
 
 database = PatientsDatabase(path_to_database="data/patients_database.h5")
 
 database.create(
@@ -254,26 +238,26 @@
 ```python
 from delia.extractors import PatientsDataExtractor
 from delia.transforms import Compose, CopySegmentationsD, PETtoSUVD, ResampleD
 import SimpleITK as sitk
 
 patients_data_extractor = PatientsDataExtractor(
     path_to_patients_folder="data/patients",
-    series_descriptions="data/series_descriptions.json",
+    tag_values="data/tag_values.json",
     transforms=Compose(
         [
             ResampleD(keys=["CT_THORAX", "Heart"], out_spacing=(1.5, 1.5, 1.5)),
-            PETtoSUVD(keys=["TEP"]),
-            CopySegmentationsD(segmented_image_key="CT_THORAX", unsegmented_image_key="TEP")
+            PETtoSUVD(keys=["PT"]),
+            CopySegmentationsD(segmented_image_key="CT_THORAX", unsegmented_image_key="PT")
         ]
     )
 )
 
 for patient_dataset in patients_data_extractor:
-	print(f"Patient ID: {patient_data.patient_id}")
+    print(f"Patient ID: {patient_dataset.patient_id}")
 
     for patient_image_data in patient_dataset.data:
         dicom_header = patient_image_data.image.dicom_header
         simple_itk_image = patient_image_data.image.simple_itk_image
         numpy_array_image = sitk.GetArrayFromImage(simple_itk_image)
 
         """Perform any tasks on images on-the-fly."""
@@ -282,21 +266,23 @@
 
 ## Need more examples?
 
 You can find more in the [examples folder](https://github.com/MaxenceLarose/delia/tree/main/examples).
 
 # A deeper look into the `PatientsDataExtractor` object
 
-The `PatientsDataExtractor` has 3 important variables:  a `path_to_patients_folder` (which dictates the path to the folder that contains all patient records), a `series_descriptions` (which dictates the images that needs to be extracted from the patient records) and `transforms` that defines a sequence of transformations to apply on images or segmentations. For each patient/folder available in the `path_to_patients_folder`, all DICOM files in their folder are read. If the series descriptions of a certain volume match one of the descriptions present in the given `series_descriptions` dictionary, this volume and its segmentation (if available) are automatically added to the `PatientDataModel`. Note that if no `series_descriptions` dictionary is given (`series_descriptions = None`), then all images (and associated segmentations) will be added to the database. 
+The `PatientsDataExtractor` has 4 important variables:  a `path_to_patients_folder` (which dictates the path to the folder that contains all patient records), a `tag` (which specifies which tag to use when choosing which images need to be extracted, if no value is given, this defaults to `SeriesDescription`), a `tag_values` (which dictates the images that needs to be extracted from the patient records) and `transforms` that defines a sequence of transformations to apply on images or segmentations. For each patient/folder available in the `path_to_patients_folder`, all DICOM files in their folder are read. If the specified tag's value of a certain volume match one of the descriptions present in the given `tag_values` dictionary, this volume and its segmentation (if available) are automatically added to the `PatientDataModel`. Note that if no `tag_values` dictionary is given (`tag_values = None`), then all images (and associated segmentations) will be added to the database. 
 
 The `PatientsDataExtractor` can therefore be used to iteratively perform tasks on each of the patients, such as displaying certain images, transforming images into numpy arrays, or creating an HDF5 database using the `PatientsDatabase`. It is this last task that is highlighted in this package, but it must be understood that the data extraction is performed in a very general manner by the `PatientsDataExtractor` and is therefore not limited to this single application. For example, someone could easily develop a `Numpydatabase` whose creation would be ensured by the `PatientsDataExtractor`, similar to the current `PatientsDatabase` based on the HDF5 format.
 
 # TODO
 
-- [ ] Generalize the use of arbitrary tags to choose images to extract. At the moment, the only tag available is `series_descriptions`.
+- [x] Generalize the use of arbitrary tags to choose images to extract. At the moment, the only tag available is `series_descriptions`.
+- [ ] Find which DICOM tags act in unusual ways such as having data associated with .repval and .value which differ by more than just their type. For now, both are used to obtain the same value in delia/readers/patient_data/factories/patient_data_factories.py (152-155) and delia/readers/image/dicom_reader.py (113-116).
+- [ ] Allow for more comprehensive use of tags such as using AND, OR and NOT between tags and their values. 
 - [ ] Loosen monai version requirements (monai==1.0.1) to allow for more recent versions. This needs a redefinition of the way transforms are applied.
 
 
 # License
 
 This code is provided under the [Apache License 2.0](https://github.com/MaxenceLarose/delia/blob/main/LICENSE).
```

### Comparing `delia-1.1.1/delia.egg-info/SOURCES.txt` & `delia-1.2.0/delia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `delia-1.1.1/examples/env_examples.py` & `delia-1.2.0/examples/env_examples.py`

 * *Files identical despite different names*

### Comparing `delia-1.1.1/examples/ex01.py` & `delia-1.2.0/examples/ex01.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,26 +19,26 @@
     env_examples.configure_logging("logging_conf.yaml")
 
     # ----------------------------------------------------------------------------------------------------------- #
     #                                      Create patients data extractor                                         #
     # ----------------------------------------------------------------------------------------------------------- #
     patients_data_extractor = PatientsDataExtractor(
         path_to_patients_folder="data/patients",
-        series_descriptions="data/series_descriptions.json",
+        tag_values="data/tag_values.json",
         transforms=Compose(
             [
                 ResampleD(keys=["CT_THORAX", "Heart"], out_spacing=(1.5, 1.5, 1.5)),
                 MatchingCentroidSpatialCropD(
                     segmentation_key="Heart",
                     matching_keys=["CT_THORAX"],
                     roi_size=(96, 96, 96)
                 ),
-                PETtoSUVD(keys=["PET"]),
+                PETtoSUVD(keys=["PT"]),
                 KeepLargestConnectedComponentD(keys=["Heart"]),
-                CopySegmentationsD(segmented_image_key="CT_THORAX", unsegmented_image_key="PET")
+                CopySegmentationsD(segmented_image_key="CT_THORAX", unsegmented_image_key="PT")
             ]
         )
     )
 
     # ----------------------------------------------------------------------------------------------------------- #
     #                                    Perform on-thy-fly tasks on images                                       #
     # ----------------------------------------------------------------------------------------------------------- #
```

### Comparing `delia-1.1.1/examples/ex02.py` & `delia-1.2.0/examples/ex02.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,19 +18,19 @@
     env_examples.configure_logging("logging_conf.yaml")
 
     # ----------------------------------------------------------------------------------------------------------- #
     #                                      Create patients data extractor                                         #
     # ----------------------------------------------------------------------------------------------------------- #
     patients_data_extractor = PatientsDataExtractor(
         path_to_patients_folder="data/patients",
-        series_descriptions="data/radiomics_series_descriptions.json",
+        tag_values="data/radiomics_tag_values.json",
         transforms=Compose(
             [
-                PETtoSUVD(keys=["PET"]),
-                CopySegmentationsD(segmented_image_key="CT_THORAX", unsegmented_image_key="PET")
+                PETtoSUVD(keys=["PT"]),
+                CopySegmentationsD(segmented_image_key="CT_THORAX", unsegmented_image_key="PT")
             ]
         )
     )
 
     # ----------------------------------------------------------------------------------------------------------- #
     #       Extract radiomics features of the CT image from the segmentation of the heart made on the CT image    #
     # ----------------------------------------------------------------------------------------------------------- #
@@ -57,9 +57,9 @@
         path_to_params="features_extractor_params_PT.yaml",
         geometryTolerance=1e-4
     )
 
     PT_radiomics_dataset.create(
         patients_data_extractor=patients_data_extractor,
         organ="Heart",
-        image_name="PET"
+        image_name="PT"
     )
```

### Comparing `delia-1.1.1/examples/ex03.py` & `delia-1.2.0/examples/ex03.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,22 +27,22 @@
     env_examples.configure_logging("logging_conf.yaml")
 
     # ----------------------------------------------------------------------------------------------------------- #
     #                                      Create patients data extractor                                         #
     # ----------------------------------------------------------------------------------------------------------- #
     patients_data_extractor = PatientsDataExtractor(
         path_to_patients_folder="data/patients",
-        series_descriptions="data/series_descriptions.json",
+        tag_values="data/tag_values.json",
         transforms=Compose(
             [
-                ResampleD(keys=["CT_THORAX", "PET", "Heart"], out_spacing=(1.5, 1.5, 1.5)),
-                MatchingResampleD(reference_image_key="CT_THORAX", matching_keys=["PET", "Heart"]),
-                CenterSpatialCropD(keys=["CT_THORAX", "PET", "Heart"], roi_size=(1000, 160, 160)),
+                ResampleD(keys=["CT_THORAX", "PT", "Heart"], out_spacing=(1.5, 1.5, 1.5)),
+                MatchingResampleD(reference_image_key="CT_THORAX", matching_keys=["PT", "Heart"]),
+                CenterSpatialCropD(keys=["CT_THORAX", "PT", "Heart"], roi_size=(1000, 160, 160)),
                 ScaleIntensityRangeD(keys=["CT_THORAX"], a_min=-250, a_max=500, b_min=0, b_max=1, clip=True),
-                PETtoSUVD(keys=["PET"])
+                PETtoSUVD(keys=["PT"])
             ]
         )
     )
 
     # ----------------------------------------------------------------------------------------------------------- #
     #                                                Create database                                              #
     # ----------------------------------------------------------------------------------------------------------- #
```

### Comparing `delia-1.1.1/setup.py` & `delia-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="delia",
-    version="1.1.1",
+    version="1.2.0",
     author="Maxence Larose",
     author_email="maxence.larose.1@ulaval.ca",
     description="DICOM Extraction for Large-scale Image Analysis (DELIA).",
     long_description=open('README.md', "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/MaxenceLarose/delia",
     license="Apache License 2.0",
```

