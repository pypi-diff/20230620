# Comparing `tmp/app_ocr-0.0.6.tar.gz` & `tmp/app_ocr-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "app_ocr-0.0.6.tar", last modified: Tue Jun 20 09:20:00 2023, max compression
+gzip compressed data, was "app_ocr-0.0.7.tar", last modified: Tue Jun 20 09:22:56 2023, max compression
```

## Comparing `app_ocr-0.0.6.tar` & `app_ocr-0.0.7.tar`

### file list

```diff
@@ -1,177 +1,180 @@
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:20:00.593637 app_ocr-0.0.6/
--rw-r--r--   0 macbook    (501) staff       (20)     2567 2023-06-20 09:20:00.593492 app_ocr-0.0.6/PKG-INFO
--rw-r--r--   0 macbook    (501) staff       (20)     2131 2023-04-12 07:19:45.000000 app_ocr-0.0.6/README.md
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:20:00.572206 app_ocr-0.0.6/app/
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:20:00.575166 app_ocr-0.0.6/app/app_ocr.egg-info/
--rw-r--r--   0 macbook    (501) staff       (20)     2567 2023-06-20 09:20:00.000000 app_ocr-0.0.6/app/app_ocr.egg-info/PKG-INFO
--rw-r--r--   0 macbook    (501) staff       (20)     6084 2023-06-20 09:20:00.000000 app_ocr-0.0.6/app/app_ocr.egg-info/SOURCES.txt
--rw-r--r--   0 macbook    (501) staff       (20)        1 2023-06-20 09:20:00.000000 app_ocr-0.0.6/app/app_ocr.egg-info/dependency_links.txt
--rw-r--r--   0 macbook    (501) staff       (20)      864 2023-06-20 09:20:00.000000 app_ocr-0.0.6/app/app_ocr.egg-info/requires.txt
--rw-r--r--   0 macbook    (501) staff       (20)       28 2023-06-20 09:20:00.000000 app_ocr-0.0.6/app/app_ocr.egg-info/top_level.txt
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:20:00.575892 app_ocr-0.0.6/app/config/
--rw-r--r--   0 macbook    (501) staff       (20)      100 2023-06-20 07:14:31.000000 app_ocr-0.0.6/app/config/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)      869 2023-06-20 08:09:34.000000 app_ocr-0.0.6/app/config/config.py
--rw-r--r--   0 macbook    (501) staff       (20)      393 2023-04-12 07:19:45.000000 app_ocr-0.0.6/app/config/config_db.py
--rw-r--r--   0 macbook    (501) staff       (20)     1085 2023-06-20 07:52:59.000000 app_ocr-0.0.6/app/config/logger.py
--rw-r--r--   0 macbook    (501) staff       (20)     4337 2023-05-09 09:10:33.000000 app_ocr-0.0.6/app/config/pydantic_models.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:20:00.576474 app_ocr-0.0.6/app/database/
--rw-r--r--   0 macbook    (501) staff       (20)       71 2023-06-20 07:14:31.000000 app_ocr-0.0.6/app/database/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     4402 2023-06-20 08:06:31.000000 app_ocr-0.0.6/app/database/crud.py
--rw-r--r--   0 macbook    (501) staff       (20)      720 2023-06-20 07:27:46.000000 app_ocr-0.0.6/app/database/data_models.py
--rw-r--r--   0 macbook    (501) staff       (20)      561 2023-06-20 08:05:57.000000 app_ocr-0.0.6/app/database/database.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:20:00.576627 app_ocr-0.0.6/app/face_id/
--rw-r--r--   0 macbook    (501) staff       (20)       66 2023-06-20 07:09:37.000000 app_ocr-0.0.6/app/face_id/__init__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:20:00.576899 app_ocr-0.0.6/app/face_id/commons/
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:20:00.577768 app_ocr-0.0.6/app/face_id/commons/AntiSpoof/
--rw-r--r--   0 macbook    (501) staff       (20)     2206 2023-04-12 07:19:45.000000 app_ocr-0.0.6/app/face_id/commons/AntiSpoof/CDCN_config.py
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 app_ocr-0.0.6/app/face_id/commons/AntiSpoof/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     2037 2023-04-12 07:19:45.000000 app_ocr-0.0.6/app/face_id/commons/AntiSpoof/anti_spoof.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:20:00.578212 app_ocr-0.0.6/app/face_id/commons/AntiSpoof/data_io/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 app_ocr-0.0.6/app/face_id/commons/AntiSpoof/data_io/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)    20275 2023-04-12 07:19:45.000000 app_ocr-0.0.6/app/face_id/commons/AntiSpoof/data_io/functional.py
--rw-r--r--   0 macbook    (501) staff       (20)    11460 2023-06-20 08:12:53.000000 app_ocr-0.0.6/app/face_id/commons/AntiSpoof/data_io/transform.py
--rw-r--r--   0 macbook    (501) staff       (20)      802 2023-04-12 07:19:45.000000 app_ocr-0.0.6/app/face_id/commons/AntiSpoof/liveness_check.py
--rw-r--r--   0 macbook    (501) staff       (20)     1379 2023-06-20 08:00:29.000000 app_ocr-0.0.6/app/face_id/commons/AntiSpoof/liveness_onnx_check.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:20:00.578652 app_ocr-0.0.6/app/face_id/commons/AntiSpoof/model_lib/
--rw-r--r--   0 macbook    (501) staff       (20)    12487 2023-04-12 07:19:45.000000 app_ocr-0.0.6/app/face_id/commons/AntiSpoof/model_lib/MiniFASNet.py
--rw-r--r--   0 macbook    (501) staff       (20)     2803 2023-04-12 07:19:45.000000 app_ocr-0.0.6/app/face_id/commons/AntiSpoof/model_lib/MultiFTNet.py
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 app_ocr-0.0.6/app/face_id/commons/AntiSpoof/model_lib/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)      990 2023-04-12 07:19:45.000000 app_ocr-0.0.6/app/face_id/commons/AntiSpoof/utility.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:20:00.578911 app_ocr-0.0.6/app/face_id/commons/ArcFace/
--rw-r--r--   0 macbook    (501) staff       (20)     2981 2023-06-20 08:00:29.000000 app_ocr-0.0.6/app/face_id/commons/ArcFace/ArcFace_onnx.py
--rw-r--r--   0 macbook    (501) staff       (20)      974 2023-06-20 08:12:40.000000 app_ocr-0.0.6/app/face_id/commons/ArcFace/__init__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:20:00.579457 app_ocr-0.0.6/app/face_id/commons/ArcFace/lib/
--rw-r--r--   0 macbook    (501) staff       (20)      186 2023-04-12 07:19:45.000000 app_ocr-0.0.6/app/face_id/commons/ArcFace/lib/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     3036 2023-04-12 07:19:45.000000 app_ocr-0.0.6/app/face_id/commons/ArcFace/lib/layers.py
--rw-r--r--   0 macbook    (501) staff       (20)     4284 2023-04-12 07:19:45.000000 app_ocr-0.0.6/app/face_id/commons/ArcFace/lib/models.py
--rw-r--r--   0 macbook    (501) staff       (20)     2436 2023-04-12 07:19:45.000000 app_ocr-0.0.6/app/face_id/commons/ArcFace/lib/utils.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:20:00.580294 app_ocr-0.0.6/app/face_id/commons/CloseEyes/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 app_ocr-0.0.6/app/face_id/commons/CloseEyes/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     3114 2023-06-20 07:27:46.000000 app_ocr-0.0.6/app/face_id/commons/CloseEyes/close_eyes.py
--rw-r--r--   0 macbook    (501) staff       (20)     1081 2023-06-20 08:48:14.000000 app_ocr-0.0.6/app/face_id/commons/CloseEyes/close_eyes_v2.py
--rw-r--r--   0 macbook    (501) staff       (20)     1306 2023-06-20 08:14:55.000000 app_ocr-0.0.6/app/face_id/commons/CloseEyes/utils.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:20:00.580587 app_ocr-0.0.6/app/face_id/commons/FaceMask/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 app_ocr-0.0.6/app/face_id/commons/FaceMask/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)      789 2023-06-20 08:00:29.000000 app_ocr-0.0.6/app/face_id/commons/FaceMask/face_mask_onnx.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:20:00.581045 app_ocr-0.0.6/app/face_id/commons/FaceQuality/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 app_ocr-0.0.6/app/face_id/commons/FaceQuality/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     9974 2023-06-01 06:55:11.000000 app_ocr-0.0.6/app/face_id/commons/FaceQuality/dom.py
--rw-r--r--   0 macbook    (501) staff       (20)     1855 2023-06-20 08:14:55.000000 app_ocr-0.0.6/app/face_id/commons/FaceQuality/face_quality_assessment.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:20:00.581361 app_ocr-0.0.6/app/face_id/commons/ScrFd/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 app_ocr-0.0.6/app/face_id/commons/ScrFd/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)    12632 2023-06-01 06:55:11.000000 app_ocr-0.0.6/app/face_id/commons/ScrFd/scrfd.py
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 app_ocr-0.0.6/app/face_id/commons/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     2297 2023-06-19 18:18:48.000000 app_ocr-0.0.6/app/face_id/commons/config.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:20:00.581966 app_ocr-0.0.6/app/face_id/libraries/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 app_ocr-0.0.6/app/face_id/libraries/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     7226 2023-06-20 08:15:16.000000 app_ocr-0.0.6/app/face_id/libraries/face_detection.py
--rw-r--r--   0 macbook    (501) staff       (20)     5298 2023-06-20 08:12:40.000000 app_ocr-0.0.6/app/face_id/libraries/face_id.py
--rw-r--r--   0 macbook    (501) staff       (20)      395 2023-06-20 08:01:32.000000 app_ocr-0.0.6/app/face_id/libraries/face_recognition.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:20:00.582256 app_ocr-0.0.6/app/face_id/testing/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 07:28:07.000000 app_ocr-0.0.6/app/face_id/testing/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)      963 2023-06-20 07:27:46.000000 app_ocr-0.0.6/app/face_id/testing/scrfd_testing.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:20:00.582538 app_ocr-0.0.6/app/face_id/tools/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 app_ocr-0.0.6/app/face_id/tools/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     3946 2023-06-20 08:09:34.000000 app_ocr-0.0.6/app/face_id/tools/modules.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:20:00.582689 app_ocr-0.0.6/app/ocr/
--rw-r--r--   0 macbook    (501) staff       (20)       19 2023-06-20 07:08:18.000000 app_ocr-0.0.6/app/ocr/__init__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:20:00.582839 app_ocr-0.0.6/app/ocr/core/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 07:27:46.000000 app_ocr-0.0.6/app/ocr/core/__init__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:20:00.583803 app_ocr-0.0.6/app/ocr/core/commons/
--rw-r--r--   0 macbook    (501) staff       (20)      814 2023-06-20 08:24:37.000000 app_ocr-0.0.6/app/ocr/core/commons/SpoofingNID.py
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 app_ocr-0.0.6/app/ocr/core/commons/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     5592 2023-06-20 08:19:46.000000 app_ocr-0.0.6/app/ocr/core/commons/config.py
--rw-r--r--   0 macbook    (501) staff       (20)      780 2023-05-30 04:20:28.000000 app_ocr-0.0.6/app/ocr/core/commons/id_card_classification.py
--rw-r--r--   0 macbook    (501) staff       (20)     5667 2023-06-20 08:20:16.000000 app_ocr-0.0.6/app/ocr/core/commons/id_card_onnx.py
--rw-r--r--   0 macbook    (501) staff       (20)     1761 2023-06-20 08:22:16.000000 app_ocr-0.0.6/app/ocr/core/commons/merge_model.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:20:00.584074 app_ocr-0.0.6/app/ocr/core/commons/utils/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 07:28:07.000000 app_ocr-0.0.6/app/ocr/core/commons/utils/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     2504 2023-06-20 08:20:31.000000 app_ocr-0.0.6/app/ocr/core/commons/utils/utils_onnx.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:20:00.584211 app_ocr-0.0.6/app/ocr/core/modules/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.6/app/ocr/core/modules/__init__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:20:00.584564 app_ocr-0.0.6/app/ocr/core/modules/corner_detection/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.6/app/ocr/core/modules/corner_detection/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     2186 2023-06-20 08:22:16.000000 app_ocr-0.0.6/app/ocr/core/modules/corner_detection/id_card_aligment.py
--rw-r--r--   0 macbook    (501) staff       (20)     3973 2023-06-19 14:29:56.000000 app_ocr-0.0.6/app/ocr/core/modules/corner_detection/utils.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:20:00.584828 app_ocr-0.0.6/app/ocr/core/modules/id_card_classification/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.6/app/ocr/core/modules/id_card_classification/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)      914 2023-06-20 08:25:44.000000 app_ocr-0.0.6/app/ocr/core/modules/id_card_classification/classify.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:20:00.585208 app_ocr-0.0.6/app/ocr/core/modules/mrc/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.6/app/ocr/core/modules/mrc/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     2929 2023-06-20 08:27:21.000000 app_ocr-0.0.6/app/ocr/core/modules/mrc/mrc_detection.py
--rw-r--r--   0 macbook    (501) staff       (20)      627 2023-06-20 08:24:11.000000 app_ocr-0.0.6/app/ocr/core/modules/mrc/utils.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:20:00.585690 app_ocr-0.0.6/app/ocr/core/modules/passport/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-18 03:26:14.000000 app_ocr-0.0.6/app/ocr/core/modules/passport/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     9063 2023-06-20 08:29:24.000000 app_ocr-0.0.6/app/ocr/core/modules/passport/passport.py
--rw-r--r--   0 macbook    (501) staff       (20)      510 2023-06-20 08:24:11.000000 app_ocr-0.0.6/app/ocr/core/modules/passport/passport_detection.py
--rw-r--r--   0 macbook    (501) staff       (20)     2288 2023-06-20 08:30:21.000000 app_ocr-0.0.6/app/ocr/core/modules/passport/utils.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:20:00.586030 app_ocr-0.0.6/app/ocr/core/modules/passport/utils_align_passport/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-18 03:26:14.000000 app_ocr-0.0.6/app/ocr/core/modules/passport/utils_align_passport/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     3248 2023-04-18 08:29:08.000000 app_ocr-0.0.6/app/ocr/core/modules/passport/utils_align_passport/passport_utils.py
--rw-r--r--   0 macbook    (501) staff       (20)     4344 2023-04-18 03:26:14.000000 app_ocr-0.0.6/app/ocr/core/modules/passport/utils_align_passport/utils_align.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:20:00.586248 app_ocr-0.0.6/app/ocr/core/modules/passport/utils_detect_passport/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-18 03:26:14.000000 app_ocr-0.0.6/app/ocr/core/modules/passport/utils_detect_passport/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     9659 2023-06-20 08:28:03.000000 app_ocr-0.0.6/app/ocr/core/modules/passport/utils_detect_passport/utils_detect.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:20:00.586528 app_ocr-0.0.6/app/ocr/core/modules/quality_liveness_nid_checking/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-26 09:38:30.000000 app_ocr-0.0.6/app/ocr/core/modules/quality_liveness_nid_checking/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     2918 2023-06-20 08:31:22.000000 app_ocr-0.0.6/app/ocr/core/modules/quality_liveness_nid_checking/nid_quality_liveness_check.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:20:00.586799 app_ocr-0.0.6/app/ocr/core/modules/spell_checking/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.6/app/ocr/core/modules/spell_checking/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     2350 2023-05-10 09:12:33.000000 app_ocr-0.0.6/app/ocr/core/modules/spell_checking/corrector_v2.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:20:00.587044 app_ocr-0.0.6/app/ocr/core/modules/spoofing_nid/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.6/app/ocr/core/modules/spoofing_nid/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)      926 2023-06-20 08:32:08.000000 app_ocr-0.0.6/app/ocr/core/modules/spoofing_nid/spoofing.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:20:00.587456 app_ocr-0.0.6/app/ocr/core/modules/text_detection/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.6/app/ocr/core/modules/text_detection/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     7020 2023-06-20 08:33:20.000000 app_ocr-0.0.6/app/ocr/core/modules/text_detection/dictionary.py
--rw-r--r--   0 macbook    (501) staff       (20)    11593 2023-06-20 08:33:42.000000 app_ocr-0.0.6/app/ocr/core/modules/text_detection/utils.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:20:00.587715 app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     2511 2023-06-20 08:34:11.000000 app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/nlp_onnx.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:20:00.588126 app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/__init__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:20:00.588710 app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/loader/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/loader/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     1735 2023-04-12 07:19:46.000000 app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/loader/aug.py
--rw-r--r--   0 macbook    (501) staff       (20)     6278 2023-04-12 07:19:46.000000 app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/loader/dataloader.py
--rw-r--r--   0 macbook    (501) staff       (20)     5021 2023-04-12 07:19:46.000000 app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/loader/dataloader_v1.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:20:00.589391 app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/model/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/model/__init__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:20:00.590191 app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)      804 2023-06-20 08:38:07.000000 app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/cnn.py
--rw-r--r--   0 macbook    (501) staff       (20)     5311 2023-04-12 07:19:46.000000 app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/resnet.py
--rw-r--r--   0 macbook    (501) staff       (20)     1655 2023-04-12 07:19:46.000000 app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/vgg.py
--rw-r--r--   0 macbook    (501) staff       (20)     3777 2023-04-12 07:19:46.000000 app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/model/beam.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:20:00.590822 app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)    11634 2023-04-12 07:19:46.000000 app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/convseq2seq.py
--rw-r--r--   0 macbook    (501) staff       (20)     5731 2023-04-12 07:19:46.000000 app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/seq2seq.py
--rw-r--r--   0 macbook    (501) staff       (20)     4858 2023-04-12 07:19:46.000000 app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/transformer.py
--rw-r--r--   0 macbook    (501) staff       (20)    13524 2023-04-12 07:19:46.000000 app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/model/trainer.py
--rw-r--r--   0 macbook    (501) staff       (20)     1630 2023-06-20 08:38:07.000000 app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/model/transformerocr.py
--rw-r--r--   0 macbook    (501) staff       (20)      924 2023-05-10 09:12:33.000000 app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/model/vocab.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:20:00.591280 app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/optim/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/optim/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     1006 2023-04-12 07:19:46.000000 app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/optim/labelsmoothingloss.py
--rw-r--r--   0 macbook    (501) staff       (20)     1798 2023-04-12 07:19:46.000000 app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/optim/optim.py
--rw-r--r--   0 macbook    (501) staff       (20)      538 2023-04-12 07:19:46.000000 app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/predict.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:20:00.591562 app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/tests/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/tests/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     1039 2023-04-12 07:19:46.000000 app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/tests/utest.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:20:00.592794 app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/tool/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/tool/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     1216 2023-06-20 08:39:08.000000 app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/tool/config.py
--rw-r--r--   0 macbook    (501) staff       (20)     2754 2023-04-12 07:19:46.000000 app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/tool/create_dataset.py
--rw-r--r--   0 macbook    (501) staff       (20)      325 2023-04-12 07:19:46.000000 app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/tool/logger.py
--rw-r--r--   0 macbook    (501) staff       (20)     1427 2023-04-12 07:19:46.000000 app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/tool/predictor.py
--rw-r--r--   0 macbook    (501) staff       (20)     7313 2023-06-20 08:38:07.000000 app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/tool/translate.py
--rw-r--r--   0 macbook    (501) staff       (20)     2688 2023-04-12 07:19:46.000000 app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/tool/utils.py
--rw-r--r--   0 macbook    (501) staff       (20)      559 2023-04-12 07:19:46.000000 app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/train.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:20:00.593294 app_ocr-0.0.6/app/ocr/core/tools/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 app_ocr-0.0.6/app/ocr/core/tools/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     5552 2023-04-18 03:26:14.000000 app_ocr-0.0.6/app/ocr/core/tools/api_json.py
--rw-r--r--   0 macbook    (501) staff       (20)     5533 2023-06-20 08:41:02.000000 app_ocr-0.0.6/app/ocr/core/tools/dictionaries.py
--rw-r--r--   0 macbook    (501) staff       (20)     2509 2023-06-20 08:40:21.000000 app_ocr-0.0.6/app/ocr/core/tools/functional.py
--rw-r--r--   0 macbook    (501) staff       (20)       38 2023-06-20 09:20:00.593688 app_ocr-0.0.6/setup.cfg
--rw-r--r--   0 macbook    (501) staff       (20)      925 2023-06-20 09:19:59.000000 app_ocr-0.0.6/setup.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:22:56.368498 app_ocr-0.0.7/
+-rw-r--r--   0 macbook    (501) staff       (20)     2567 2023-06-20 09:22:56.368362 app_ocr-0.0.7/PKG-INFO
+-rw-r--r--   0 macbook    (501) staff       (20)     2131 2023-04-12 07:19:45.000000 app_ocr-0.0.7/README.md
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:22:56.348405 app_ocr-0.0.7/app/
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:22:56.350597 app_ocr-0.0.7/app/api/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 09:21:37.000000 app_ocr-0.0.7/app/api/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5366 2023-06-20 09:22:40.000000 app_ocr-0.0.7/app/api/just_scan_api.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:22:56.351305 app_ocr-0.0.7/app/app_ocr.egg-info/
+-rw-r--r--   0 macbook    (501) staff       (20)     2567 2023-06-20 09:22:56.000000 app_ocr-0.0.7/app/app_ocr.egg-info/PKG-INFO
+-rw-r--r--   0 macbook    (501) staff       (20)     6129 2023-06-20 09:22:56.000000 app_ocr-0.0.7/app/app_ocr.egg-info/SOURCES.txt
+-rw-r--r--   0 macbook    (501) staff       (20)        1 2023-06-20 09:22:56.000000 app_ocr-0.0.7/app/app_ocr.egg-info/dependency_links.txt
+-rw-r--r--   0 macbook    (501) staff       (20)      864 2023-06-20 09:22:56.000000 app_ocr-0.0.7/app/app_ocr.egg-info/requires.txt
+-rw-r--r--   0 macbook    (501) staff       (20)       32 2023-06-20 09:22:56.000000 app_ocr-0.0.7/app/app_ocr.egg-info/top_level.txt
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:22:56.351948 app_ocr-0.0.7/app/config/
+-rw-r--r--   0 macbook    (501) staff       (20)      100 2023-06-20 07:14:31.000000 app_ocr-0.0.7/app/config/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)      869 2023-06-20 08:09:34.000000 app_ocr-0.0.7/app/config/config.py
+-rw-r--r--   0 macbook    (501) staff       (20)      393 2023-04-12 07:19:45.000000 app_ocr-0.0.7/app/config/config_db.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1085 2023-06-20 07:52:59.000000 app_ocr-0.0.7/app/config/logger.py
+-rw-r--r--   0 macbook    (501) staff       (20)     4337 2023-05-09 09:10:33.000000 app_ocr-0.0.7/app/config/pydantic_models.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:22:56.352495 app_ocr-0.0.7/app/database/
+-rw-r--r--   0 macbook    (501) staff       (20)       71 2023-06-20 07:14:31.000000 app_ocr-0.0.7/app/database/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     4402 2023-06-20 08:06:31.000000 app_ocr-0.0.7/app/database/crud.py
+-rw-r--r--   0 macbook    (501) staff       (20)      720 2023-06-20 07:27:46.000000 app_ocr-0.0.7/app/database/data_models.py
+-rw-r--r--   0 macbook    (501) staff       (20)      561 2023-06-20 08:05:57.000000 app_ocr-0.0.7/app/database/database.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:22:56.352620 app_ocr-0.0.7/app/face_id/
+-rw-r--r--   0 macbook    (501) staff       (20)       66 2023-06-20 07:09:37.000000 app_ocr-0.0.7/app/face_id/__init__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:22:56.352838 app_ocr-0.0.7/app/face_id/commons/
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:22:56.353557 app_ocr-0.0.7/app/face_id/commons/AntiSpoof/
+-rw-r--r--   0 macbook    (501) staff       (20)     2206 2023-04-12 07:19:45.000000 app_ocr-0.0.7/app/face_id/commons/AntiSpoof/CDCN_config.py
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 app_ocr-0.0.7/app/face_id/commons/AntiSpoof/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2037 2023-04-12 07:19:45.000000 app_ocr-0.0.7/app/face_id/commons/AntiSpoof/anti_spoof.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:22:56.353948 app_ocr-0.0.7/app/face_id/commons/AntiSpoof/data_io/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 app_ocr-0.0.7/app/face_id/commons/AntiSpoof/data_io/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)    20275 2023-04-12 07:19:45.000000 app_ocr-0.0.7/app/face_id/commons/AntiSpoof/data_io/functional.py
+-rw-r--r--   0 macbook    (501) staff       (20)    11460 2023-06-20 08:12:53.000000 app_ocr-0.0.7/app/face_id/commons/AntiSpoof/data_io/transform.py
+-rw-r--r--   0 macbook    (501) staff       (20)      802 2023-04-12 07:19:45.000000 app_ocr-0.0.7/app/face_id/commons/AntiSpoof/liveness_check.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1379 2023-06-20 08:00:29.000000 app_ocr-0.0.7/app/face_id/commons/AntiSpoof/liveness_onnx_check.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:22:56.354371 app_ocr-0.0.7/app/face_id/commons/AntiSpoof/model_lib/
+-rw-r--r--   0 macbook    (501) staff       (20)    12487 2023-04-12 07:19:45.000000 app_ocr-0.0.7/app/face_id/commons/AntiSpoof/model_lib/MiniFASNet.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2803 2023-04-12 07:19:45.000000 app_ocr-0.0.7/app/face_id/commons/AntiSpoof/model_lib/MultiFTNet.py
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 app_ocr-0.0.7/app/face_id/commons/AntiSpoof/model_lib/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)      990 2023-04-12 07:19:45.000000 app_ocr-0.0.7/app/face_id/commons/AntiSpoof/utility.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:22:56.354632 app_ocr-0.0.7/app/face_id/commons/ArcFace/
+-rw-r--r--   0 macbook    (501) staff       (20)     2981 2023-06-20 08:00:29.000000 app_ocr-0.0.7/app/face_id/commons/ArcFace/ArcFace_onnx.py
+-rw-r--r--   0 macbook    (501) staff       (20)      974 2023-06-20 08:12:40.000000 app_ocr-0.0.7/app/face_id/commons/ArcFace/__init__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:22:56.355208 app_ocr-0.0.7/app/face_id/commons/ArcFace/lib/
+-rw-r--r--   0 macbook    (501) staff       (20)      186 2023-04-12 07:19:45.000000 app_ocr-0.0.7/app/face_id/commons/ArcFace/lib/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     3036 2023-04-12 07:19:45.000000 app_ocr-0.0.7/app/face_id/commons/ArcFace/lib/layers.py
+-rw-r--r--   0 macbook    (501) staff       (20)     4284 2023-04-12 07:19:45.000000 app_ocr-0.0.7/app/face_id/commons/ArcFace/lib/models.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2436 2023-04-12 07:19:45.000000 app_ocr-0.0.7/app/face_id/commons/ArcFace/lib/utils.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:22:56.355734 app_ocr-0.0.7/app/face_id/commons/CloseEyes/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 app_ocr-0.0.7/app/face_id/commons/CloseEyes/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     3114 2023-06-20 07:27:46.000000 app_ocr-0.0.7/app/face_id/commons/CloseEyes/close_eyes.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1081 2023-06-20 08:48:14.000000 app_ocr-0.0.7/app/face_id/commons/CloseEyes/close_eyes_v2.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1306 2023-06-20 08:14:55.000000 app_ocr-0.0.7/app/face_id/commons/CloseEyes/utils.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:22:56.356101 app_ocr-0.0.7/app/face_id/commons/FaceMask/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 app_ocr-0.0.7/app/face_id/commons/FaceMask/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)      789 2023-06-20 08:00:29.000000 app_ocr-0.0.7/app/face_id/commons/FaceMask/face_mask_onnx.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:22:56.356594 app_ocr-0.0.7/app/face_id/commons/FaceQuality/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 app_ocr-0.0.7/app/face_id/commons/FaceQuality/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     9974 2023-06-01 06:55:11.000000 app_ocr-0.0.7/app/face_id/commons/FaceQuality/dom.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1855 2023-06-20 08:14:55.000000 app_ocr-0.0.7/app/face_id/commons/FaceQuality/face_quality_assessment.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:22:56.356874 app_ocr-0.0.7/app/face_id/commons/ScrFd/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 app_ocr-0.0.7/app/face_id/commons/ScrFd/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)    12632 2023-06-01 06:55:11.000000 app_ocr-0.0.7/app/face_id/commons/ScrFd/scrfd.py
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 app_ocr-0.0.7/app/face_id/commons/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2297 2023-06-19 18:18:48.000000 app_ocr-0.0.7/app/face_id/commons/config.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:22:56.357427 app_ocr-0.0.7/app/face_id/libraries/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 app_ocr-0.0.7/app/face_id/libraries/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     7226 2023-06-20 08:15:16.000000 app_ocr-0.0.7/app/face_id/libraries/face_detection.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5298 2023-06-20 08:12:40.000000 app_ocr-0.0.7/app/face_id/libraries/face_id.py
+-rw-r--r--   0 macbook    (501) staff       (20)      395 2023-06-20 08:01:32.000000 app_ocr-0.0.7/app/face_id/libraries/face_recognition.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:22:56.357694 app_ocr-0.0.7/app/face_id/testing/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 07:28:07.000000 app_ocr-0.0.7/app/face_id/testing/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)      963 2023-06-20 07:27:46.000000 app_ocr-0.0.7/app/face_id/testing/scrfd_testing.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:22:56.357944 app_ocr-0.0.7/app/face_id/tools/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 app_ocr-0.0.7/app/face_id/tools/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     3946 2023-06-20 08:09:34.000000 app_ocr-0.0.7/app/face_id/tools/modules.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:22:56.358070 app_ocr-0.0.7/app/ocr/
+-rw-r--r--   0 macbook    (501) staff       (20)       19 2023-06-20 07:08:18.000000 app_ocr-0.0.7/app/ocr/__init__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:22:56.358220 app_ocr-0.0.7/app/ocr/core/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 07:27:46.000000 app_ocr-0.0.7/app/ocr/core/__init__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:22:56.358993 app_ocr-0.0.7/app/ocr/core/commons/
+-rw-r--r--   0 macbook    (501) staff       (20)      814 2023-06-20 08:24:37.000000 app_ocr-0.0.7/app/ocr/core/commons/SpoofingNID.py
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 app_ocr-0.0.7/app/ocr/core/commons/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5592 2023-06-20 08:19:46.000000 app_ocr-0.0.7/app/ocr/core/commons/config.py
+-rw-r--r--   0 macbook    (501) staff       (20)      780 2023-05-30 04:20:28.000000 app_ocr-0.0.7/app/ocr/core/commons/id_card_classification.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5667 2023-06-20 08:20:16.000000 app_ocr-0.0.7/app/ocr/core/commons/id_card_onnx.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1761 2023-06-20 08:22:16.000000 app_ocr-0.0.7/app/ocr/core/commons/merge_model.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:22:56.359207 app_ocr-0.0.7/app/ocr/core/commons/utils/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 07:28:07.000000 app_ocr-0.0.7/app/ocr/core/commons/utils/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2504 2023-06-20 08:20:31.000000 app_ocr-0.0.7/app/ocr/core/commons/utils/utils_onnx.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:22:56.359328 app_ocr-0.0.7/app/ocr/core/modules/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.7/app/ocr/core/modules/__init__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:22:56.359650 app_ocr-0.0.7/app/ocr/core/modules/corner_detection/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.7/app/ocr/core/modules/corner_detection/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2186 2023-06-20 08:22:16.000000 app_ocr-0.0.7/app/ocr/core/modules/corner_detection/id_card_aligment.py
+-rw-r--r--   0 macbook    (501) staff       (20)     3973 2023-06-19 14:29:56.000000 app_ocr-0.0.7/app/ocr/core/modules/corner_detection/utils.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:22:56.359870 app_ocr-0.0.7/app/ocr/core/modules/id_card_classification/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.7/app/ocr/core/modules/id_card_classification/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)      914 2023-06-20 08:25:44.000000 app_ocr-0.0.7/app/ocr/core/modules/id_card_classification/classify.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:22:56.360456 app_ocr-0.0.7/app/ocr/core/modules/mrc/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.7/app/ocr/core/modules/mrc/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2929 2023-06-20 08:27:21.000000 app_ocr-0.0.7/app/ocr/core/modules/mrc/mrc_detection.py
+-rw-r--r--   0 macbook    (501) staff       (20)      627 2023-06-20 08:24:11.000000 app_ocr-0.0.7/app/ocr/core/modules/mrc/utils.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:22:56.361025 app_ocr-0.0.7/app/ocr/core/modules/passport/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-18 03:26:14.000000 app_ocr-0.0.7/app/ocr/core/modules/passport/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     9063 2023-06-20 08:29:24.000000 app_ocr-0.0.7/app/ocr/core/modules/passport/passport.py
+-rw-r--r--   0 macbook    (501) staff       (20)      510 2023-06-20 08:24:11.000000 app_ocr-0.0.7/app/ocr/core/modules/passport/passport_detection.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2288 2023-06-20 08:30:21.000000 app_ocr-0.0.7/app/ocr/core/modules/passport/utils.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:22:56.361584 app_ocr-0.0.7/app/ocr/core/modules/passport/utils_align_passport/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-18 03:26:14.000000 app_ocr-0.0.7/app/ocr/core/modules/passport/utils_align_passport/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     3248 2023-04-18 08:29:08.000000 app_ocr-0.0.7/app/ocr/core/modules/passport/utils_align_passport/passport_utils.py
+-rw-r--r--   0 macbook    (501) staff       (20)     4344 2023-04-18 03:26:14.000000 app_ocr-0.0.7/app/ocr/core/modules/passport/utils_align_passport/utils_align.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:22:56.361881 app_ocr-0.0.7/app/ocr/core/modules/passport/utils_detect_passport/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-18 03:26:14.000000 app_ocr-0.0.7/app/ocr/core/modules/passport/utils_detect_passport/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     9659 2023-06-20 08:28:03.000000 app_ocr-0.0.7/app/ocr/core/modules/passport/utils_detect_passport/utils_detect.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:22:56.362168 app_ocr-0.0.7/app/ocr/core/modules/quality_liveness_nid_checking/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-26 09:38:30.000000 app_ocr-0.0.7/app/ocr/core/modules/quality_liveness_nid_checking/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2918 2023-06-20 08:31:22.000000 app_ocr-0.0.7/app/ocr/core/modules/quality_liveness_nid_checking/nid_quality_liveness_check.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:22:56.362449 app_ocr-0.0.7/app/ocr/core/modules/spell_checking/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.7/app/ocr/core/modules/spell_checking/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2350 2023-05-10 09:12:33.000000 app_ocr-0.0.7/app/ocr/core/modules/spell_checking/corrector_v2.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:22:56.362727 app_ocr-0.0.7/app/ocr/core/modules/spoofing_nid/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.7/app/ocr/core/modules/spoofing_nid/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)      926 2023-06-20 08:32:08.000000 app_ocr-0.0.7/app/ocr/core/modules/spoofing_nid/spoofing.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:22:56.363151 app_ocr-0.0.7/app/ocr/core/modules/text_detection/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.7/app/ocr/core/modules/text_detection/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     7020 2023-06-20 08:33:20.000000 app_ocr-0.0.7/app/ocr/core/modules/text_detection/dictionary.py
+-rw-r--r--   0 macbook    (501) staff       (20)    11593 2023-06-20 08:33:42.000000 app_ocr-0.0.7/app/ocr/core/modules/text_detection/utils.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:22:56.363409 app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2511 2023-06-20 08:34:11.000000 app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/nlp_onnx.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:22:56.363839 app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/__init__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:22:56.364391 app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/loader/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/loader/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1735 2023-04-12 07:19:46.000000 app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/loader/aug.py
+-rw-r--r--   0 macbook    (501) staff       (20)     6278 2023-04-12 07:19:46.000000 app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/loader/dataloader.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5021 2023-04-12 07:19:46.000000 app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/loader/dataloader_v1.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:22:56.365149 app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/model/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/model/__init__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:22:56.365685 app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)      804 2023-06-20 08:38:07.000000 app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/cnn.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5311 2023-04-12 07:19:46.000000 app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/resnet.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1655 2023-04-12 07:19:46.000000 app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/vgg.py
+-rw-r--r--   0 macbook    (501) staff       (20)     3777 2023-04-12 07:19:46.000000 app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/model/beam.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:22:56.366244 app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)    11634 2023-04-12 07:19:46.000000 app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/convseq2seq.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5731 2023-04-12 07:19:46.000000 app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/seq2seq.py
+-rw-r--r--   0 macbook    (501) staff       (20)     4858 2023-04-12 07:19:46.000000 app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/transformer.py
+-rw-r--r--   0 macbook    (501) staff       (20)    13524 2023-04-12 07:19:46.000000 app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/model/trainer.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1630 2023-06-20 08:38:07.000000 app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/model/transformerocr.py
+-rw-r--r--   0 macbook    (501) staff       (20)      924 2023-05-10 09:12:33.000000 app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/model/vocab.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:22:56.366649 app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/optim/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/optim/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1006 2023-04-12 07:19:46.000000 app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/optim/labelsmoothingloss.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1798 2023-04-12 07:19:46.000000 app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/optim/optim.py
+-rw-r--r--   0 macbook    (501) staff       (20)      538 2023-04-12 07:19:46.000000 app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/predict.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:22:56.366874 app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/tests/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/tests/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1039 2023-04-12 07:19:46.000000 app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/tests/utest.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:22:56.367695 app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/tool/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/tool/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1216 2023-06-20 08:39:08.000000 app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/tool/config.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2754 2023-04-12 07:19:46.000000 app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/tool/create_dataset.py
+-rw-r--r--   0 macbook    (501) staff       (20)      325 2023-04-12 07:19:46.000000 app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/tool/logger.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1427 2023-04-12 07:19:46.000000 app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/tool/predictor.py
+-rw-r--r--   0 macbook    (501) staff       (20)     7313 2023-06-20 08:38:07.000000 app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/tool/translate.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2688 2023-04-12 07:19:46.000000 app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/tool/utils.py
+-rw-r--r--   0 macbook    (501) staff       (20)      559 2023-04-12 07:19:46.000000 app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/train.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 09:22:56.368153 app_ocr-0.0.7/app/ocr/core/tools/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 app_ocr-0.0.7/app/ocr/core/tools/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5552 2023-04-18 03:26:14.000000 app_ocr-0.0.7/app/ocr/core/tools/api_json.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5533 2023-06-20 08:41:02.000000 app_ocr-0.0.7/app/ocr/core/tools/dictionaries.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2509 2023-06-20 08:40:21.000000 app_ocr-0.0.7/app/ocr/core/tools/functional.py
+-rw-r--r--   0 macbook    (501) staff       (20)       38 2023-06-20 09:22:56.368542 app_ocr-0.0.7/setup.cfg
+-rw-r--r--   0 macbook    (501) staff       (20)      925 2023-06-20 09:22:55.000000 app_ocr-0.0.7/setup.py
```

### Comparing `app_ocr-0.0.6/PKG-INFO` & `app_ocr-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: app_ocr
-Version: 0.0.6
+Version: 0.0.7
 Summary: E-kyc for Industries application
 Home-page: https://github.com/aihackervn
 Author: Theodore
 Author-email: tinprocoder0908@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `app_ocr-0.0.6/README.md` & `app_ocr-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/app_ocr.egg-info/PKG-INFO` & `app_ocr-0.0.7/app/app_ocr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: app-ocr
-Version: 0.0.6
+Version: 0.0.7
 Summary: E-kyc for Industries application
 Home-page: https://github.com/aihackervn
 Author: Theodore
 Author-email: tinprocoder0908@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `app_ocr-0.0.6/app/app_ocr.egg-info/SOURCES.txt` & `app_ocr-0.0.7/app/app_ocr.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 README.md
 setup.py
+app/api/__init__.py
+app/api/just_scan_api.py
 app/app_ocr.egg-info/PKG-INFO
 app/app_ocr.egg-info/SOURCES.txt
 app/app_ocr.egg-info/dependency_links.txt
 app/app_ocr.egg-info/requires.txt
 app/app_ocr.egg-info/top_level.txt
 app/config/__init__.py
 app/config/config.py
```

### Comparing `app_ocr-0.0.6/app/app_ocr.egg-info/requires.txt` & `app_ocr-0.0.7/app/app_ocr.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/config/config.py` & `app_ocr-0.0.7/app/config/config.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/config/logger.py` & `app_ocr-0.0.7/app/config/logger.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/config/pydantic_models.py` & `app_ocr-0.0.7/app/config/pydantic_models.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/database/crud.py` & `app_ocr-0.0.7/app/database/crud.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/database/data_models.py` & `app_ocr-0.0.7/app/database/data_models.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/database/database.py` & `app_ocr-0.0.7/app/database/database.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/face_id/commons/AntiSpoof/CDCN_config.py` & `app_ocr-0.0.7/app/face_id/commons/AntiSpoof/CDCN_config.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/face_id/commons/AntiSpoof/anti_spoof.py` & `app_ocr-0.0.7/app/face_id/commons/AntiSpoof/anti_spoof.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/face_id/commons/AntiSpoof/data_io/functional.py` & `app_ocr-0.0.7/app/face_id/commons/AntiSpoof/data_io/functional.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/face_id/commons/AntiSpoof/data_io/transform.py` & `app_ocr-0.0.7/app/face_id/commons/AntiSpoof/data_io/transform.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/face_id/commons/AntiSpoof/liveness_check.py` & `app_ocr-0.0.7/app/face_id/commons/AntiSpoof/liveness_check.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/face_id/commons/AntiSpoof/liveness_onnx_check.py` & `app_ocr-0.0.7/app/face_id/commons/AntiSpoof/liveness_onnx_check.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/face_id/commons/AntiSpoof/model_lib/MiniFASNet.py` & `app_ocr-0.0.7/app/face_id/commons/AntiSpoof/model_lib/MiniFASNet.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/face_id/commons/AntiSpoof/model_lib/MultiFTNet.py` & `app_ocr-0.0.7/app/face_id/commons/AntiSpoof/model_lib/MultiFTNet.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/face_id/commons/AntiSpoof/utility.py` & `app_ocr-0.0.7/app/face_id/commons/AntiSpoof/utility.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/face_id/commons/ArcFace/ArcFace_onnx.py` & `app_ocr-0.0.7/app/face_id/commons/ArcFace/ArcFace_onnx.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/face_id/commons/ArcFace/__init__.py` & `app_ocr-0.0.7/app/face_id/commons/ArcFace/__init__.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/face_id/commons/ArcFace/lib/layers.py` & `app_ocr-0.0.7/app/face_id/commons/ArcFace/lib/layers.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/face_id/commons/ArcFace/lib/models.py` & `app_ocr-0.0.7/app/face_id/commons/ArcFace/lib/models.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/face_id/commons/ArcFace/lib/utils.py` & `app_ocr-0.0.7/app/face_id/commons/ArcFace/lib/utils.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/face_id/commons/CloseEyes/close_eyes.py` & `app_ocr-0.0.7/app/face_id/commons/CloseEyes/close_eyes.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/face_id/commons/CloseEyes/close_eyes_v2.py` & `app_ocr-0.0.7/app/face_id/commons/CloseEyes/close_eyes_v2.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/face_id/commons/CloseEyes/utils.py` & `app_ocr-0.0.7/app/face_id/commons/CloseEyes/utils.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/face_id/commons/FaceMask/face_mask_onnx.py` & `app_ocr-0.0.7/app/face_id/commons/FaceMask/face_mask_onnx.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/face_id/commons/FaceQuality/dom.py` & `app_ocr-0.0.7/app/face_id/commons/FaceQuality/dom.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/face_id/commons/FaceQuality/face_quality_assessment.py` & `app_ocr-0.0.7/app/face_id/commons/FaceQuality/face_quality_assessment.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/face_id/commons/ScrFd/scrfd.py` & `app_ocr-0.0.7/app/face_id/commons/ScrFd/scrfd.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/face_id/commons/config.py` & `app_ocr-0.0.7/app/face_id/commons/config.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/face_id/libraries/face_detection.py` & `app_ocr-0.0.7/app/face_id/libraries/face_detection.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/face_id/libraries/face_id.py` & `app_ocr-0.0.7/app/face_id/libraries/face_id.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/face_id/testing/scrfd_testing.py` & `app_ocr-0.0.7/app/face_id/testing/scrfd_testing.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/face_id/tools/modules.py` & `app_ocr-0.0.7/app/face_id/tools/modules.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/ocr/core/commons/SpoofingNID.py` & `app_ocr-0.0.7/app/ocr/core/commons/SpoofingNID.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/ocr/core/commons/config.py` & `app_ocr-0.0.7/app/ocr/core/commons/config.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/ocr/core/commons/id_card_classification.py` & `app_ocr-0.0.7/app/ocr/core/commons/id_card_classification.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/ocr/core/commons/id_card_onnx.py` & `app_ocr-0.0.7/app/ocr/core/commons/id_card_onnx.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/ocr/core/commons/merge_model.py` & `app_ocr-0.0.7/app/ocr/core/commons/merge_model.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/ocr/core/commons/utils/utils_onnx.py` & `app_ocr-0.0.7/app/ocr/core/commons/utils/utils_onnx.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/ocr/core/modules/corner_detection/id_card_aligment.py` & `app_ocr-0.0.7/app/ocr/core/modules/corner_detection/id_card_aligment.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/ocr/core/modules/corner_detection/utils.py` & `app_ocr-0.0.7/app/ocr/core/modules/corner_detection/utils.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/ocr/core/modules/id_card_classification/classify.py` & `app_ocr-0.0.7/app/ocr/core/modules/id_card_classification/classify.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/ocr/core/modules/mrc/mrc_detection.py` & `app_ocr-0.0.7/app/ocr/core/modules/mrc/mrc_detection.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/ocr/core/modules/mrc/utils.py` & `app_ocr-0.0.7/app/ocr/core/modules/mrc/utils.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/ocr/core/modules/passport/passport.py` & `app_ocr-0.0.7/app/ocr/core/modules/passport/passport.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/ocr/core/modules/passport/utils.py` & `app_ocr-0.0.7/app/ocr/core/modules/passport/utils.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/ocr/core/modules/passport/utils_align_passport/passport_utils.py` & `app_ocr-0.0.7/app/ocr/core/modules/passport/utils_align_passport/passport_utils.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/ocr/core/modules/passport/utils_align_passport/utils_align.py` & `app_ocr-0.0.7/app/ocr/core/modules/passport/utils_align_passport/utils_align.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/ocr/core/modules/passport/utils_detect_passport/utils_detect.py` & `app_ocr-0.0.7/app/ocr/core/modules/passport/utils_detect_passport/utils_detect.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/ocr/core/modules/quality_liveness_nid_checking/nid_quality_liveness_check.py` & `app_ocr-0.0.7/app/ocr/core/modules/quality_liveness_nid_checking/nid_quality_liveness_check.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/ocr/core/modules/spell_checking/corrector_v2.py` & `app_ocr-0.0.7/app/ocr/core/modules/spell_checking/corrector_v2.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/ocr/core/modules/spoofing_nid/spoofing.py` & `app_ocr-0.0.7/app/ocr/core/modules/spoofing_nid/spoofing.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/ocr/core/modules/text_detection/dictionary.py` & `app_ocr-0.0.7/app/ocr/core/modules/text_detection/dictionary.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/ocr/core/modules/text_detection/utils.py` & `app_ocr-0.0.7/app/ocr/core/modules/text_detection/utils.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/nlp_onnx.py` & `app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/nlp_onnx.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/loader/aug.py` & `app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/loader/aug.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/loader/dataloader.py` & `app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/loader/dataloader.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/loader/dataloader_v1.py` & `app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/loader/dataloader_v1.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/cnn.py` & `app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/cnn.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/resnet.py` & `app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/resnet.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/vgg.py` & `app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/vgg.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/model/beam.py` & `app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/model/beam.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/convseq2seq.py` & `app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/convseq2seq.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/seq2seq.py` & `app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/seq2seq.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/transformer.py` & `app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/transformer.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/model/trainer.py` & `app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/model/trainer.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/model/transformerocr.py` & `app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/model/transformerocr.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/model/vocab.py` & `app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/model/vocab.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/optim/labelsmoothingloss.py` & `app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/optim/labelsmoothingloss.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/optim/optim.py` & `app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/optim/optim.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/predict.py` & `app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/predict.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/tests/utest.py` & `app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/tests/utest.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/tool/config.py` & `app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/tool/config.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/tool/create_dataset.py` & `app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/tool/create_dataset.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/tool/predictor.py` & `app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/tool/predictor.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/tool/translate.py` & `app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/tool/translate.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/tool/utils.py` & `app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/tool/utils.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/ocr/core/modules/vietnamese_nlp/vietocr/train.py` & `app_ocr-0.0.7/app/ocr/core/modules/vietnamese_nlp/vietocr/train.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/ocr/core/tools/api_json.py` & `app_ocr-0.0.7/app/ocr/core/tools/api_json.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/ocr/core/tools/dictionaries.py` & `app_ocr-0.0.7/app/ocr/core/tools/dictionaries.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/app/ocr/core/tools/functional.py` & `app_ocr-0.0.7/app/ocr/core/tools/functional.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.6/setup.py` & `app_ocr-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 with open("README.md", "r") as f:
     long_description = f.read()
 with open("requirements.txt", "r") as f:
     install_requires = [line.strip() for line in f if line.strip()]
 setup(
     name="app_ocr",
-    version="0.0.6",
+    version="0.0.7",
     description="E-kyc for Industries application",
     package_dir={"": "app"},
     packages=find_packages(where="./app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aihackervn",
     author="Theodore",
```
