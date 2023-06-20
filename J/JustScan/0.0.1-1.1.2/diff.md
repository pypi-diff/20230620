# Comparing `tmp/JustScan-0.0.1.tar.gz` & `tmp/JustScan-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JustScan-0.0.1.tar", last modified: Tue Jun 20 17:02:08 2023, max compression
+gzip compressed data, was "JustScan-1.1.2.tar", last modified: Tue Jun 20 17:25:35 2023, max compression
```

## Comparing `JustScan-0.0.1.tar` & `JustScan-1.1.2.tar`

### file list

```diff
@@ -1,183 +1,180 @@
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:02:08.903892 JustScan-0.0.1/
--rw-r--r--   0 macbook    (501) staff       (20)     2568 2023-06-20 17:02:08.903703 JustScan-0.0.1/PKG-INFO
--rw-r--r--   0 macbook    (501) staff       (20)     2131 2023-04-12 07:19:45.000000 JustScan-0.0.1/README.md
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:02:08.874902 JustScan-0.0.1/app/
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:02:08.879907 JustScan-0.0.1/app/JustScan/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 16:58:48.000000 JustScan-0.0.1/app/JustScan/__init__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:02:08.881856 JustScan-0.0.1/app/JustScan/api/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 09:21:37.000000 JustScan-0.0.1/app/JustScan/api/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)      181 2023-06-20 10:57:02.000000 JustScan-0.0.1/app/JustScan/api/itc_cli.py
--rw-r--r--   0 macbook    (501) staff       (20)     5475 2023-06-20 17:01:40.000000 JustScan-0.0.1/app/JustScan/api/just_scan_api.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:02:08.882886 JustScan-0.0.1/app/JustScan/config/
--rw-r--r--   0 macbook    (501) staff       (20)      100 2023-06-20 07:14:31.000000 JustScan-0.0.1/app/JustScan/config/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     1546 2023-06-20 10:29:43.000000 JustScan-0.0.1/app/JustScan/config/config.py
--rw-r--r--   0 macbook    (501) staff       (20)      619 2023-06-20 10:30:42.000000 JustScan-0.0.1/app/JustScan/config/config_db.py
--rw-r--r--   0 macbook    (501) staff       (20)     1872 2023-06-20 10:31:25.000000 JustScan-0.0.1/app/JustScan/config/logger.py
--rw-r--r--   0 macbook    (501) staff       (20)     4337 2023-05-09 09:10:33.000000 JustScan-0.0.1/app/JustScan/config/pydantic_models.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:02:08.883551 JustScan-0.0.1/app/JustScan/database/
--rw-r--r--   0 macbook    (501) staff       (20)       71 2023-06-20 07:14:31.000000 JustScan-0.0.1/app/JustScan/database/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     4402 2023-06-20 08:06:31.000000 JustScan-0.0.1/app/JustScan/database/crud.py
--rw-r--r--   0 macbook    (501) staff       (20)      867 2023-06-20 10:35:51.000000 JustScan-0.0.1/app/JustScan/database/data_models.py
--rw-r--r--   0 macbook    (501) staff       (20)      561 2023-06-20 08:05:57.000000 JustScan-0.0.1/app/JustScan/database/database.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:02:08.883726 JustScan-0.0.1/app/JustScan/face_id/
--rw-r--r--   0 macbook    (501) staff       (20)       66 2023-06-20 07:09:37.000000 JustScan-0.0.1/app/JustScan/face_id/__init__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:02:08.884033 JustScan-0.0.1/app/JustScan/face_id/commons/
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:02:08.885063 JustScan-0.0.1/app/JustScan/face_id/commons/AntiSpoof/
--rw-r--r--   0 macbook    (501) staff       (20)     2206 2023-06-20 10:35:31.000000 JustScan-0.0.1/app/JustScan/face_id/commons/AntiSpoof/CDCN_config.py
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 JustScan-0.0.1/app/JustScan/face_id/commons/AntiSpoof/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     2037 2023-06-20 10:35:31.000000 JustScan-0.0.1/app/JustScan/face_id/commons/AntiSpoof/anti_spoof.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:02:08.885577 JustScan-0.0.1/app/JustScan/face_id/commons/AntiSpoof/data_io/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-0.0.1/app/JustScan/face_id/commons/AntiSpoof/data_io/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)    20275 2023-04-12 07:19:45.000000 JustScan-0.0.1/app/JustScan/face_id/commons/AntiSpoof/data_io/functional.py
--rw-r--r--   0 macbook    (501) staff       (20)    11460 2023-06-20 08:12:53.000000 JustScan-0.0.1/app/JustScan/face_id/commons/AntiSpoof/data_io/transform.py
--rw-r--r--   0 macbook    (501) staff       (20)      802 2023-06-20 10:35:31.000000 JustScan-0.0.1/app/JustScan/face_id/commons/AntiSpoof/liveness_check.py
--rw-r--r--   0 macbook    (501) staff       (20)     1379 2023-06-20 08:00:29.000000 JustScan-0.0.1/app/JustScan/face_id/commons/AntiSpoof/liveness_onnx_check.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:02:08.886091 JustScan-0.0.1/app/JustScan/face_id/commons/AntiSpoof/model_lib/
--rw-r--r--   0 macbook    (501) staff       (20)    12487 2023-04-12 07:19:45.000000 JustScan-0.0.1/app/JustScan/face_id/commons/AntiSpoof/model_lib/MiniFASNet.py
--rw-r--r--   0 macbook    (501) staff       (20)     2739 2023-06-20 16:58:59.000000 JustScan-0.0.1/app/JustScan/face_id/commons/AntiSpoof/model_lib/MultiFTNet.py
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-0.0.1/app/JustScan/face_id/commons/AntiSpoof/model_lib/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)      990 2023-06-20 10:35:31.000000 JustScan-0.0.1/app/JustScan/face_id/commons/AntiSpoof/utility.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:02:08.886411 JustScan-0.0.1/app/JustScan/face_id/commons/ArcFace/
--rw-r--r--   0 macbook    (501) staff       (20)     2981 2023-06-20 08:00:29.000000 JustScan-0.0.1/app/JustScan/face_id/commons/ArcFace/ArcFace_onnx.py
--rw-r--r--   0 macbook    (501) staff       (20)      974 2023-06-20 08:12:40.000000 JustScan-0.0.1/app/JustScan/face_id/commons/ArcFace/__init__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:02:08.887069 JustScan-0.0.1/app/JustScan/face_id/commons/ArcFace/lib/
--rw-r--r--   0 macbook    (501) staff       (20)      213 2023-06-20 16:58:59.000000 JustScan-0.0.1/app/JustScan/face_id/commons/ArcFace/lib/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     3036 2023-04-12 07:19:45.000000 JustScan-0.0.1/app/JustScan/face_id/commons/ArcFace/lib/layers.py
--rw-r--r--   0 macbook    (501) staff       (20)     4293 2023-06-20 16:58:59.000000 JustScan-0.0.1/app/JustScan/face_id/commons/ArcFace/lib/models.py
--rw-r--r--   0 macbook    (501) staff       (20)     2436 2023-04-12 07:19:45.000000 JustScan-0.0.1/app/JustScan/face_id/commons/ArcFace/lib/utils.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:02:08.887546 JustScan-0.0.1/app/JustScan/face_id/commons/CloseEyes/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 JustScan-0.0.1/app/JustScan/face_id/commons/CloseEyes/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     1081 2023-06-20 08:48:14.000000 JustScan-0.0.1/app/JustScan/face_id/commons/CloseEyes/close_eyes_v2.py
--rw-r--r--   0 macbook    (501) staff       (20)     1306 2023-06-20 08:14:55.000000 JustScan-0.0.1/app/JustScan/face_id/commons/CloseEyes/utils.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:02:08.887854 JustScan-0.0.1/app/JustScan/face_id/commons/FaceMask/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 JustScan-0.0.1/app/JustScan/face_id/commons/FaceMask/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)      789 2023-06-20 08:00:29.000000 JustScan-0.0.1/app/JustScan/face_id/commons/FaceMask/face_mask_onnx.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:02:08.888658 JustScan-0.0.1/app/JustScan/face_id/commons/FaceQuality/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 JustScan-0.0.1/app/JustScan/face_id/commons/FaceQuality/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     9974 2023-06-01 06:55:11.000000 JustScan-0.0.1/app/JustScan/face_id/commons/FaceQuality/dom.py
--rw-r--r--   0 macbook    (501) staff       (20)     1855 2023-06-20 08:14:55.000000 JustScan-0.0.1/app/JustScan/face_id/commons/FaceQuality/face_quality_assessment.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:02:08.889053 JustScan-0.0.1/app/JustScan/face_id/commons/ScrFd/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 JustScan-0.0.1/app/JustScan/face_id/commons/ScrFd/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)    12632 2023-06-01 06:55:11.000000 JustScan-0.0.1/app/JustScan/face_id/commons/ScrFd/scrfd.py
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-0.0.1/app/JustScan/face_id/commons/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     2297 2023-06-19 18:18:48.000000 JustScan-0.0.1/app/JustScan/face_id/commons/config.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:02:08.889853 JustScan-0.0.1/app/JustScan/face_id/libraries/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-0.0.1/app/JustScan/face_id/libraries/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     7226 2023-06-20 08:15:16.000000 JustScan-0.0.1/app/JustScan/face_id/libraries/face_detection.py
--rw-r--r--   0 macbook    (501) staff       (20)     5298 2023-06-20 08:12:40.000000 JustScan-0.0.1/app/JustScan/face_id/libraries/face_id.py
--rw-r--r--   0 macbook    (501) staff       (20)      395 2023-06-20 08:01:32.000000 JustScan-0.0.1/app/JustScan/face_id/libraries/face_recognition.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:02:08.890143 JustScan-0.0.1/app/JustScan/face_id/testing/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 07:28:07.000000 JustScan-0.0.1/app/JustScan/face_id/testing/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)      990 2023-06-20 16:58:59.000000 JustScan-0.0.1/app/JustScan/face_id/testing/scrfd_testing.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:02:08.890424 JustScan-0.0.1/app/JustScan/face_id/tools/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-0.0.1/app/JustScan/face_id/tools/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     3946 2023-06-20 08:09:34.000000 JustScan-0.0.1/app/JustScan/face_id/tools/modules.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:02:08.890596 JustScan-0.0.1/app/JustScan/ocr/
--rw-r--r--   0 macbook    (501) staff       (20)       19 2023-06-20 07:08:18.000000 JustScan-0.0.1/app/JustScan/ocr/__init__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:02:08.890750 JustScan-0.0.1/app/JustScan/ocr/core/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 07:27:46.000000 JustScan-0.0.1/app/JustScan/ocr/core/__init__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:02:08.891722 JustScan-0.0.1/app/JustScan/ocr/core/commons/
--rw-r--r--   0 macbook    (501) staff       (20)      814 2023-06-20 08:24:37.000000 JustScan-0.0.1/app/JustScan/ocr/core/commons/SpoofingNID.py
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-0.0.1/app/JustScan/ocr/core/commons/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     5592 2023-06-20 08:19:46.000000 JustScan-0.0.1/app/JustScan/ocr/core/commons/config.py
--rw-r--r--   0 macbook    (501) staff       (20)      780 2023-05-30 04:20:28.000000 JustScan-0.0.1/app/JustScan/ocr/core/commons/id_card_classification.py
--rw-r--r--   0 macbook    (501) staff       (20)     5675 2023-06-20 10:04:38.000000 JustScan-0.0.1/app/JustScan/ocr/core/commons/id_card_onnx.py
--rw-r--r--   0 macbook    (501) staff       (20)     1761 2023-06-20 08:22:16.000000 JustScan-0.0.1/app/JustScan/ocr/core/commons/merge_model.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:02:08.892016 JustScan-0.0.1/app/JustScan/ocr/core/commons/utils/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 07:28:07.000000 JustScan-0.0.1/app/JustScan/ocr/core/commons/utils/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     2504 2023-06-20 08:20:31.000000 JustScan-0.0.1/app/JustScan/ocr/core/commons/utils/utils_onnx.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:02:08.892200 JustScan-0.0.1/app/JustScan/ocr/core/modules/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/__init__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:02:08.892637 JustScan-0.0.1/app/JustScan/ocr/core/modules/corner_detection/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/corner_detection/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     2186 2023-06-20 08:22:16.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/corner_detection/id_card_aligment.py
--rw-r--r--   0 macbook    (501) staff       (20)     3973 2023-06-19 14:29:56.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/corner_detection/utils.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:02:08.892930 JustScan-0.0.1/app/JustScan/ocr/core/modules/id_card_classification/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/id_card_classification/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)      914 2023-06-20 08:25:44.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/id_card_classification/classify.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:02:08.893407 JustScan-0.0.1/app/JustScan/ocr/core/modules/mrc/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/mrc/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     2929 2023-06-20 08:27:21.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/mrc/mrc_detection.py
--rw-r--r--   0 macbook    (501) staff       (20)      627 2023-06-20 08:24:11.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/mrc/utils.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:02:08.894090 JustScan-0.0.1/app/JustScan/ocr/core/modules/passport/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-18 03:26:14.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/passport/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     9063 2023-06-20 08:29:24.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/passport/passport.py
--rw-r--r--   0 macbook    (501) staff       (20)      510 2023-06-20 08:24:11.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/passport/passport_detection.py
--rw-r--r--   0 macbook    (501) staff       (20)     2288 2023-06-20 08:30:21.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/passport/utils.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:02:08.894580 JustScan-0.0.1/app/JustScan/ocr/core/modules/passport/utils_align_passport/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-18 03:26:14.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/passport/utils_align_passport/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     3248 2023-04-18 08:29:08.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/passport/utils_align_passport/passport_utils.py
--rw-r--r--   0 macbook    (501) staff       (20)     4344 2023-04-18 03:26:14.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/passport/utils_align_passport/utils_align.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:02:08.894907 JustScan-0.0.1/app/JustScan/ocr/core/modules/passport/utils_detect_passport/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-18 03:26:14.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/passport/utils_detect_passport/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     9659 2023-06-20 08:28:03.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/passport/utils_detect_passport/utils_detect.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:02:08.895241 JustScan-0.0.1/app/JustScan/ocr/core/modules/quality_liveness_nid_checking/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-26 09:38:30.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/quality_liveness_nid_checking/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     2918 2023-06-20 08:31:22.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/quality_liveness_nid_checking/nid_quality_liveness_check.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:02:08.895578 JustScan-0.0.1/app/JustScan/ocr/core/modules/spell_checking/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/spell_checking/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     2350 2023-05-10 09:12:33.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/spell_checking/corrector_v2.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:02:08.895915 JustScan-0.0.1/app/JustScan/ocr/core/modules/spoofing_nid/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/spoofing_nid/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)      926 2023-06-20 08:32:08.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/spoofing_nid/spoofing.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:02:08.896429 JustScan-0.0.1/app/JustScan/ocr/core/modules/text_detection/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/text_detection/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     7020 2023-06-20 08:33:20.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/text_detection/dictionary.py
--rw-r--r--   0 macbook    (501) staff       (20)    11593 2023-06-20 08:33:42.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/text_detection/utils.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:02:08.896758 JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     2511 2023-06-20 08:34:11.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/nlp_onnx.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:02:08.897523 JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/__init__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:02:08.898276 JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     1735 2023-04-12 07:19:46.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/aug.py
--rw-r--r--   0 macbook    (501) staff       (20)     6278 2023-04-12 07:19:46.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/dataloader.py
--rw-r--r--   0 macbook    (501) staff       (20)     5021 2023-04-12 07:19:46.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/dataloader_v1.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:02:08.899510 JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/__init__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:02:08.900145 JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)      804 2023-06-20 08:38:07.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/cnn.py
--rw-r--r--   0 macbook    (501) staff       (20)     5311 2023-04-12 07:19:46.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/resnet.py
--rw-r--r--   0 macbook    (501) staff       (20)     1655 2023-04-12 07:19:46.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/vgg.py
--rw-r--r--   0 macbook    (501) staff       (20)     3777 2023-04-12 07:19:46.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/beam.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:02:08.900813 JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)    11634 2023-04-12 07:19:46.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/convseq2seq.py
--rw-r--r--   0 macbook    (501) staff       (20)     5731 2023-04-12 07:19:46.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/seq2seq.py
--rw-r--r--   0 macbook    (501) staff       (20)     4858 2023-04-12 07:19:46.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/transformer.py
--rw-r--r--   0 macbook    (501) staff       (20)    13524 2023-04-12 07:19:46.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/trainer.py
--rw-r--r--   0 macbook    (501) staff       (20)     1630 2023-06-20 08:38:07.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/transformerocr.py
--rw-r--r--   0 macbook    (501) staff       (20)      924 2023-05-10 09:12:33.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/vocab.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:02:08.901266 JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/optim/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/optim/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     1006 2023-04-12 07:19:46.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/optim/labelsmoothingloss.py
--rw-r--r--   0 macbook    (501) staff       (20)     1798 2023-04-12 07:19:46.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/optim/optim.py
--rw-r--r--   0 macbook    (501) staff       (20)      538 2023-04-12 07:19:46.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/predict.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:02:08.901553 JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tests/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tests/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     1039 2023-04-12 07:19:46.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tests/utest.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:02:08.902643 JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     1216 2023-06-20 08:39:08.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/config.py
--rw-r--r--   0 macbook    (501) staff       (20)     2754 2023-04-12 07:19:46.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/create_dataset.py
--rw-r--r--   0 macbook    (501) staff       (20)      325 2023-04-12 07:19:46.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/logger.py
--rw-r--r--   0 macbook    (501) staff       (20)     1445 2023-06-20 16:58:59.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/predictor.py
--rw-r--r--   0 macbook    (501) staff       (20)     7313 2023-06-20 08:38:07.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/translate.py
--rw-r--r--   0 macbook    (501) staff       (20)     2688 2023-04-12 07:19:46.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/utils.py
--rw-r--r--   0 macbook    (501) staff       (20)      559 2023-04-12 07:19:46.000000 JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/train.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:02:08.903409 JustScan-0.0.1/app/JustScan/ocr/core/tools/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-0.0.1/app/JustScan/ocr/core/tools/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     5552 2023-04-18 03:26:14.000000 JustScan-0.0.1/app/JustScan/ocr/core/tools/api_json.py
--rw-r--r--   0 macbook    (501) staff       (20)     5533 2023-06-20 08:41:02.000000 JustScan-0.0.1/app/JustScan/ocr/core/tools/dictionaries.py
--rw-r--r--   0 macbook    (501) staff       (20)     2509 2023-06-20 08:40:21.000000 JustScan-0.0.1/app/JustScan/ocr/core/tools/functional.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:02:08.881154 JustScan-0.0.1/app/JustScan.egg-info/
--rw-r--r--   0 macbook    (501) staff       (20)     2568 2023-06-20 17:02:08.000000 JustScan-0.0.1/app/JustScan.egg-info/PKG-INFO
--rw-r--r--   0 macbook    (501) staff       (20)     7307 2023-06-20 17:02:08.000000 JustScan-0.0.1/app/JustScan.egg-info/SOURCES.txt
--rw-r--r--   0 macbook    (501) staff       (20)        1 2023-06-20 17:02:08.000000 JustScan-0.0.1/app/JustScan.egg-info/dependency_links.txt
--rw-r--r--   0 macbook    (501) staff       (20)       44 2023-06-20 17:02:08.000000 JustScan-0.0.1/app/JustScan.egg-info/entry_points.txt
--rw-r--r--   0 macbook    (501) staff       (20)      864 2023-06-20 17:02:08.000000 JustScan-0.0.1/app/JustScan.egg-info/requires.txt
--rw-r--r--   0 macbook    (501) staff       (20)        9 2023-06-20 17:02:08.000000 JustScan-0.0.1/app/JustScan.egg-info/top_level.txt
--rw-r--r--   0 macbook    (501) staff       (20)       38 2023-06-20 17:02:08.903962 JustScan-0.0.1/setup.cfg
--rw-r--r--   0 macbook    (501) staff       (20)     1033 2023-06-20 17:02:04.000000 JustScan-0.0.1/setup.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:25:35.197182 JustScan-1.1.2/
+-rw-r--r--   0 macbook    (501) staff       (20)     2638 2023-06-20 17:25:35.197005 JustScan-1.1.2/PKG-INFO
+-rw-r--r--   0 macbook    (501) staff       (20)     2131 2023-04-12 07:19:45.000000 JustScan-1.1.2/README.md
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:25:35.169164 JustScan-1.1.2/app/
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:25:35.173854 JustScan-1.1.2/app/JustScan/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 17:20:30.000000 JustScan-1.1.2/app/JustScan/__init__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:25:35.175519 JustScan-1.1.2/app/JustScan/api/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 09:21:37.000000 JustScan-1.1.2/app/JustScan/api/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)      181 2023-06-20 10:57:02.000000 JustScan-1.1.2/app/JustScan/api/itc_cli.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5520 2023-06-20 17:06:38.000000 JustScan-1.1.2/app/JustScan/api/just_scan_api.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:25:35.176379 JustScan-1.1.2/app/JustScan/config/
+-rw-r--r--   0 macbook    (501) staff       (20)      100 2023-06-20 07:14:31.000000 JustScan-1.1.2/app/JustScan/config/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1546 2023-06-20 10:29:43.000000 JustScan-1.1.2/app/JustScan/config/config.py
+-rw-r--r--   0 macbook    (501) staff       (20)      619 2023-06-20 10:30:42.000000 JustScan-1.1.2/app/JustScan/config/config_db.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1872 2023-06-20 10:31:25.000000 JustScan-1.1.2/app/JustScan/config/logger.py
+-rw-r--r--   0 macbook    (501) staff       (20)     4337 2023-05-09 09:10:33.000000 JustScan-1.1.2/app/JustScan/config/pydantic_models.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:25:35.177205 JustScan-1.1.2/app/JustScan/database/
+-rw-r--r--   0 macbook    (501) staff       (20)       71 2023-06-20 07:14:31.000000 JustScan-1.1.2/app/JustScan/database/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     4402 2023-06-20 08:06:31.000000 JustScan-1.1.2/app/JustScan/database/crud.py
+-rw-r--r--   0 macbook    (501) staff       (20)      867 2023-06-20 10:35:51.000000 JustScan-1.1.2/app/JustScan/database/data_models.py
+-rw-r--r--   0 macbook    (501) staff       (20)      570 2023-06-20 17:06:38.000000 JustScan-1.1.2/app/JustScan/database/database.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:25:35.177382 JustScan-1.1.2/app/JustScan/face_id/
+-rw-r--r--   0 macbook    (501) staff       (20)       66 2023-06-20 07:09:37.000000 JustScan-1.1.2/app/JustScan/face_id/__init__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:25:35.177713 JustScan-1.1.2/app/JustScan/face_id/commons/
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:25:35.178818 JustScan-1.1.2/app/JustScan/face_id/commons/AntiSpoof/
+-rw-r--r--   0 macbook    (501) staff       (20)     2206 2023-06-20 10:35:31.000000 JustScan-1.1.2/app/JustScan/face_id/commons/AntiSpoof/CDCN_config.py
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 JustScan-1.1.2/app/JustScan/face_id/commons/AntiSpoof/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2037 2023-06-20 10:35:31.000000 JustScan-1.1.2/app/JustScan/face_id/commons/AntiSpoof/anti_spoof.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:25:35.179394 JustScan-1.1.2/app/JustScan/face_id/commons/AntiSpoof/data_io/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-1.1.2/app/JustScan/face_id/commons/AntiSpoof/data_io/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)    20275 2023-04-12 07:19:45.000000 JustScan-1.1.2/app/JustScan/face_id/commons/AntiSpoof/data_io/functional.py
+-rw-r--r--   0 macbook    (501) staff       (20)    11460 2023-06-20 08:12:53.000000 JustScan-1.1.2/app/JustScan/face_id/commons/AntiSpoof/data_io/transform.py
+-rw-r--r--   0 macbook    (501) staff       (20)      802 2023-06-20 10:35:31.000000 JustScan-1.1.2/app/JustScan/face_id/commons/AntiSpoof/liveness_check.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1402 2023-06-20 17:16:54.000000 JustScan-1.1.2/app/JustScan/face_id/commons/AntiSpoof/liveness_onnx_check.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:25:35.179962 JustScan-1.1.2/app/JustScan/face_id/commons/AntiSpoof/model_lib/
+-rw-r--r--   0 macbook    (501) staff       (20)    12487 2023-04-12 07:19:45.000000 JustScan-1.1.2/app/JustScan/face_id/commons/AntiSpoof/model_lib/MiniFASNet.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2739 2023-06-20 16:58:59.000000 JustScan-1.1.2/app/JustScan/face_id/commons/AntiSpoof/model_lib/MultiFTNet.py
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-1.1.2/app/JustScan/face_id/commons/AntiSpoof/model_lib/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)      990 2023-06-20 10:35:31.000000 JustScan-1.1.2/app/JustScan/face_id/commons/AntiSpoof/utility.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:25:35.180302 JustScan-1.1.2/app/JustScan/face_id/commons/ArcFace/
+-rw-r--r--   0 macbook    (501) staff       (20)     3004 2023-06-20 17:16:54.000000 JustScan-1.1.2/app/JustScan/face_id/commons/ArcFace/ArcFace_onnx.py
+-rw-r--r--   0 macbook    (501) staff       (20)      974 2023-06-20 08:12:40.000000 JustScan-1.1.2/app/JustScan/face_id/commons/ArcFace/__init__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:25:35.181043 JustScan-1.1.2/app/JustScan/face_id/commons/ArcFace/lib/
+-rw-r--r--   0 macbook    (501) staff       (20)      213 2023-06-20 16:58:59.000000 JustScan-1.1.2/app/JustScan/face_id/commons/ArcFace/lib/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     3036 2023-04-12 07:19:45.000000 JustScan-1.1.2/app/JustScan/face_id/commons/ArcFace/lib/layers.py
+-rw-r--r--   0 macbook    (501) staff       (20)     4293 2023-06-20 16:58:59.000000 JustScan-1.1.2/app/JustScan/face_id/commons/ArcFace/lib/models.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2436 2023-04-12 07:19:45.000000 JustScan-1.1.2/app/JustScan/face_id/commons/ArcFace/lib/utils.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:25:35.181489 JustScan-1.1.2/app/JustScan/face_id/commons/CloseEyes/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 JustScan-1.1.2/app/JustScan/face_id/commons/CloseEyes/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1096 2023-06-20 17:16:54.000000 JustScan-1.1.2/app/JustScan/face_id/commons/CloseEyes/close_eyes_v2.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1315 2023-06-20 17:16:54.000000 JustScan-1.1.2/app/JustScan/face_id/commons/CloseEyes/utils.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:25:35.181821 JustScan-1.1.2/app/JustScan/face_id/commons/FaceMask/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 JustScan-1.1.2/app/JustScan/face_id/commons/FaceMask/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)      804 2023-06-20 17:16:54.000000 JustScan-1.1.2/app/JustScan/face_id/commons/FaceMask/face_mask_onnx.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:25:35.182273 JustScan-1.1.2/app/JustScan/face_id/commons/FaceQuality/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 JustScan-1.1.2/app/JustScan/face_id/commons/FaceQuality/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     9974 2023-06-01 06:55:11.000000 JustScan-1.1.2/app/JustScan/face_id/commons/FaceQuality/dom.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1855 2023-06-20 08:14:55.000000 JustScan-1.1.2/app/JustScan/face_id/commons/FaceQuality/face_quality_assessment.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:25:35.182571 JustScan-1.1.2/app/JustScan/face_id/commons/ScrFd/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 JustScan-1.1.2/app/JustScan/face_id/commons/ScrFd/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)    12632 2023-06-01 06:55:11.000000 JustScan-1.1.2/app/JustScan/face_id/commons/ScrFd/scrfd.py
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-1.1.2/app/JustScan/face_id/commons/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2297 2023-06-19 18:18:48.000000 JustScan-1.1.2/app/JustScan/face_id/commons/config.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:25:35.183202 JustScan-1.1.2/app/JustScan/face_id/libraries/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-1.1.2/app/JustScan/face_id/libraries/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     7235 2023-06-20 17:16:54.000000 JustScan-1.1.2/app/JustScan/face_id/libraries/face_detection.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5325 2023-06-20 17:16:54.000000 JustScan-1.1.2/app/JustScan/face_id/libraries/face_id.py
+-rw-r--r--   0 macbook    (501) staff       (20)      395 2023-06-20 08:01:32.000000 JustScan-1.1.2/app/JustScan/face_id/libraries/face_recognition.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:25:35.183505 JustScan-1.1.2/app/JustScan/face_id/tools/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-1.1.2/app/JustScan/face_id/tools/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     3955 2023-06-20 17:16:54.000000 JustScan-1.1.2/app/JustScan/face_id/tools/modules.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:25:35.183660 JustScan-1.1.2/app/JustScan/ocr/
+-rw-r--r--   0 macbook    (501) staff       (20)       19 2023-06-20 07:08:18.000000 JustScan-1.1.2/app/JustScan/ocr/__init__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:25:35.183844 JustScan-1.1.2/app/JustScan/ocr/core/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 07:27:46.000000 JustScan-1.1.2/app/JustScan/ocr/core/__init__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:25:35.184821 JustScan-1.1.2/app/JustScan/ocr/core/commons/
+-rw-r--r--   0 macbook    (501) staff       (20)      814 2023-06-20 08:24:37.000000 JustScan-1.1.2/app/JustScan/ocr/core/commons/SpoofingNID.py
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-1.1.2/app/JustScan/ocr/core/commons/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5592 2023-06-20 08:19:46.000000 JustScan-1.1.2/app/JustScan/ocr/core/commons/config.py
+-rw-r--r--   0 macbook    (501) staff       (20)      780 2023-05-30 04:20:28.000000 JustScan-1.1.2/app/JustScan/ocr/core/commons/id_card_classification.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5675 2023-06-20 10:04:38.000000 JustScan-1.1.2/app/JustScan/ocr/core/commons/id_card_onnx.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1761 2023-06-20 08:22:16.000000 JustScan-1.1.2/app/JustScan/ocr/core/commons/merge_model.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:25:35.185172 JustScan-1.1.2/app/JustScan/ocr/core/commons/utils/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 07:28:07.000000 JustScan-1.1.2/app/JustScan/ocr/core/commons/utils/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2513 2023-06-20 17:16:54.000000 JustScan-1.1.2/app/JustScan/ocr/core/commons/utils/utils_onnx.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:25:35.185347 JustScan-1.1.2/app/JustScan/ocr/core/modules/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/__init__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:25:35.185832 JustScan-1.1.2/app/JustScan/ocr/core/modules/corner_detection/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/corner_detection/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1145 2023-06-20 17:16:54.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/corner_detection/id_card_aligment.py
+-rw-r--r--   0 macbook    (501) staff       (20)     3973 2023-06-19 14:29:56.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/corner_detection/utils.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:25:35.186170 JustScan-1.1.2/app/JustScan/ocr/core/modules/id_card_classification/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/id_card_classification/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)      923 2023-06-20 17:16:54.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/id_card_classification/classify.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:25:35.186673 JustScan-1.1.2/app/JustScan/ocr/core/modules/mrc/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/mrc/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2938 2023-06-20 17:16:54.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/mrc/mrc_detection.py
+-rw-r--r--   0 macbook    (501) staff       (20)      627 2023-06-20 08:24:11.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/mrc/utils.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:25:35.187336 JustScan-1.1.2/app/JustScan/ocr/core/modules/passport/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-18 03:26:14.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/passport/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     9072 2023-06-20 17:16:54.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/passport/passport.py
+-rw-r--r--   0 macbook    (501) staff       (20)      510 2023-06-20 08:24:11.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/passport/passport_detection.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2288 2023-06-20 08:30:21.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/passport/utils.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:25:35.187876 JustScan-1.1.2/app/JustScan/ocr/core/modules/passport/utils_align_passport/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-18 03:26:14.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/passport/utils_align_passport/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     3248 2023-04-18 08:29:08.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/passport/utils_align_passport/passport_utils.py
+-rw-r--r--   0 macbook    (501) staff       (20)     4344 2023-04-18 03:26:14.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/passport/utils_align_passport/utils_align.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:25:35.188229 JustScan-1.1.2/app/JustScan/ocr/core/modules/passport/utils_detect_passport/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-18 03:26:14.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/passport/utils_detect_passport/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     9668 2023-06-20 17:16:54.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/passport/utils_detect_passport/utils_detect.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:25:35.188520 JustScan-1.1.2/app/JustScan/ocr/core/modules/quality_liveness_nid_checking/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-26 09:38:30.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/quality_liveness_nid_checking/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2927 2023-06-20 17:16:54.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/quality_liveness_nid_checking/nid_quality_liveness_check.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:25:35.189067 JustScan-1.1.2/app/JustScan/ocr/core/modules/spell_checking/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/spell_checking/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2350 2023-05-10 09:12:33.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/spell_checking/corrector_v2.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:25:35.189440 JustScan-1.1.2/app/JustScan/ocr/core/modules/spoofing_nid/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/spoofing_nid/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)      935 2023-06-20 17:16:54.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/spoofing_nid/spoofing.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:25:35.189948 JustScan-1.1.2/app/JustScan/ocr/core/modules/text_detection/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/text_detection/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     7020 2023-06-20 08:33:20.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/text_detection/dictionary.py
+-rw-r--r--   0 macbook    (501) staff       (20)    11602 2023-06-20 17:16:54.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/text_detection/utils.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:25:35.190276 JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2511 2023-06-20 08:34:11.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/nlp_onnx.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:25:35.190829 JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/__init__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:25:35.191536 JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1735 2023-04-12 07:19:46.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/aug.py
+-rw-r--r--   0 macbook    (501) staff       (20)     6278 2023-04-12 07:19:46.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/dataloader.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5021 2023-04-12 07:19:46.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/dataloader_v1.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:25:35.192423 JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/__init__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:25:35.193140 JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)      804 2023-06-20 08:38:07.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/cnn.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5311 2023-04-12 07:19:46.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/resnet.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1655 2023-04-12 07:19:46.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/vgg.py
+-rw-r--r--   0 macbook    (501) staff       (20)     3777 2023-04-12 07:19:46.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/beam.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:25:35.193914 JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)    11634 2023-04-12 07:19:46.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/convseq2seq.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5731 2023-04-12 07:19:46.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/seq2seq.py
+-rw-r--r--   0 macbook    (501) staff       (20)     4858 2023-04-12 07:19:46.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/transformer.py
+-rw-r--r--   0 macbook    (501) staff       (20)    13524 2023-04-12 07:19:46.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/trainer.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1630 2023-06-20 08:38:07.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/transformerocr.py
+-rw-r--r--   0 macbook    (501) staff       (20)      924 2023-05-10 09:12:33.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/vocab.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:25:35.194578 JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/optim/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/optim/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1006 2023-04-12 07:19:46.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/optim/labelsmoothingloss.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1798 2023-04-12 07:19:46.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/optim/optim.py
+-rw-r--r--   0 macbook    (501) staff       (20)      538 2023-04-12 07:19:46.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/predict.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:25:35.194923 JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tests/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tests/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1039 2023-04-12 07:19:46.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tests/utest.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:25:35.196134 JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1216 2023-06-20 08:39:08.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/config.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2754 2023-04-12 07:19:46.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/create_dataset.py
+-rw-r--r--   0 macbook    (501) staff       (20)      325 2023-04-12 07:19:46.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/logger.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1445 2023-06-20 16:58:59.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/predictor.py
+-rw-r--r--   0 macbook    (501) staff       (20)     7313 2023-06-20 08:38:07.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/translate.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2688 2023-04-12 07:19:46.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/utils.py
+-rw-r--r--   0 macbook    (501) staff       (20)      559 2023-04-12 07:19:46.000000 JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/train.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:25:35.196773 JustScan-1.1.2/app/JustScan/ocr/core/tools/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 JustScan-1.1.2/app/JustScan/ocr/core/tools/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5552 2023-04-18 03:26:14.000000 JustScan-1.1.2/app/JustScan/ocr/core/tools/api_json.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5533 2023-06-20 17:16:54.000000 JustScan-1.1.2/app/JustScan/ocr/core/tools/dictionaries.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2518 2023-06-20 17:16:54.000000 JustScan-1.1.2/app/JustScan/ocr/core/tools/functional.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 17:25:35.174963 JustScan-1.1.2/app/JustScan.egg-info/
+-rw-r--r--   0 macbook    (501) staff       (20)     2638 2023-06-20 17:25:35.000000 JustScan-1.1.2/app/JustScan.egg-info/PKG-INFO
+-rw-r--r--   0 macbook    (501) staff       (20)     7220 2023-06-20 17:25:35.000000 JustScan-1.1.2/app/JustScan.egg-info/SOURCES.txt
+-rw-r--r--   0 macbook    (501) staff       (20)        1 2023-06-20 17:25:35.000000 JustScan-1.1.2/app/JustScan.egg-info/dependency_links.txt
+-rw-r--r--   0 macbook    (501) staff       (20)       58 2023-06-20 17:25:35.000000 JustScan-1.1.2/app/JustScan.egg-info/entry_points.txt
+-rw-r--r--   0 macbook    (501) staff       (20)      864 2023-06-20 17:25:35.000000 JustScan-1.1.2/app/JustScan.egg-info/requires.txt
+-rw-r--r--   0 macbook    (501) staff       (20)        9 2023-06-20 17:25:35.000000 JustScan-1.1.2/app/JustScan.egg-info/top_level.txt
+-rw-r--r--   0 macbook    (501) staff       (20)       38 2023-06-20 17:25:35.197244 JustScan-1.1.2/setup.cfg
+-rw-r--r--   0 macbook    (501) staff       (20)     1158 2023-06-20 17:25:26.000000 JustScan-1.1.2/setup.py
```

### Comparing `JustScan-0.0.1/PKG-INFO` & `JustScan-1.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: JustScan
-Version: 0.0.1
+Version: 1.1.2
 Summary: E-kyc for Industries application
 Home-page: https://github.com/aihackervn
 Author: Theodore
 Author-email: tinprocoder0908@gmail.com
 License: MIT
+Keywords: ITC,AI,E-kyc,Deep Learning,Computer Vision,Yolov5,Interface
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `JustScan-0.0.1/README.md` & `JustScan-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/api/just_scan_api.py` & `JustScan-1.1.2/app/JustScan/api/just_scan_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from fastapi import File, FastAPI
 from typing import List, Dict
-from ...JustScan.face_id.libraries.face_detection import selfie_face_check, check_image_quality, multi_face_check, \
+from JustScan.face_id.libraries.face_detection import selfie_face_check, check_image_quality, multi_face_check, \
     check_image_qual
-from ...JustScan.database.crud import QueryData
-from ...JustScan.ocr.core.tools.functional import get_result_id_card, get_alignment_image
-from ...JustScan.ocr.core.modules.id_card_classification.classify import process_classification
-from ...JustScan.config.pydantic_models import IdOutput, DetectOutput, RegisterOutput, \
+from JustScan.database.crud import QueryData
+from JustScan.ocr.core.tools.functional import get_result_id_card, get_alignment_image
+from JustScan.ocr.core.modules.id_card_classification.classify import process_classification
+from JustScan.config.pydantic_models import IdOutput, DetectOutput, RegisterOutput, \
     RecognizeOutputResult, \
     CompareResult, \
     ImageQualityResult, \
     SelfieCheckResult, \
     SpoofingOutput, \
     MultiFacesCheckResult, \
     NIDQualityLivenessResult
-from ...JustScan.config.config import processing_image
-from face_id.libraries.face_id import get_register, get_recognize, comparing_faces, detect_user
-from ocr.core.modules.mrc.mrc_detection import get_mrc, get_mrc_alignment
-from ocr.core.modules.passport.passport import PassportAutoAlign
-from ocr.core.modules.passport.utils import get_passport
-from ocr.core.modules.spoofing_nid.spoofing import check_spoof_nid
-from config.logger import setup_logger, timeit
-from ocr.core.modules.quality_liveness_nid_checking.nid_quality_liveness_check import NIDQualityLivenessCheck
+from JustScan.config.config import processing_image
+from JustScan.face_id.libraries.face_id import get_register, get_recognize, comparing_faces, detect_user
+from JustScan.ocr.core.modules.mrc.mrc_detection import get_mrc, get_mrc_alignment
+from JustScan.ocr.core.modules.passport.passport import PassportAutoAlign
+from JustScan.ocr.core.modules.passport.utils import get_passport
+from JustScan.ocr.core.modules.spoofing_nid.spoofing import check_spoof_nid
+from JustScan.config.logger import setup_logger, timeit
+from JustScan.ocr.core.modules.quality_liveness_nid_checking.nid_quality_liveness_check import NIDQualityLivenessCheck
 import uvicorn
 
 logging = setup_logger(__name__)
 
 db = QueryData()
 
 app = FastAPI(title='ITC AI', swagger_ui_parameters={
```

### Comparing `JustScan-0.0.1/app/JustScan/config/config.py` & `JustScan-1.1.2/app/JustScan/config/config.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/config/config_db.py` & `JustScan-1.1.2/app/JustScan/config/config_db.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/config/logger.py` & `JustScan-1.1.2/app/JustScan/config/logger.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/config/pydantic_models.py` & `JustScan-1.1.2/app/JustScan/config/pydantic_models.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/database/crud.py` & `JustScan-1.1.2/app/JustScan/database/crud.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/database/data_models.py` & `JustScan-1.1.2/app/JustScan/database/data_models.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/database/database.py` & `JustScan-1.1.2/app/JustScan/database/database.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from sqlalchemy import create_engine
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.orm import sessionmaker
 from sqlalchemy.engine import URL
-from config.config_db import SettingLocal, SettingDev
+from JustScan.config.config_db import SettingLocal, SettingDev
 
 setting = SettingDev()
 
 SQLALCHEMY_DATABASE_URL = URL.create(
     "postgresql",
     username=setting.USERNAME_,
     password=setting.PASSWORD,
```

### Comparing `JustScan-0.0.1/app/JustScan/face_id/commons/AntiSpoof/CDCN_config.py` & `JustScan-1.1.2/app/JustScan/face_id/commons/AntiSpoof/CDCN_config.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/face_id/commons/AntiSpoof/anti_spoof.py` & `JustScan-1.1.2/app/JustScan/face_id/commons/AntiSpoof/anti_spoof.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/face_id/commons/AntiSpoof/data_io/functional.py` & `JustScan-1.1.2/app/JustScan/face_id/commons/AntiSpoof/data_io/functional.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/face_id/commons/AntiSpoof/data_io/transform.py` & `JustScan-1.1.2/app/JustScan/face_id/commons/AntiSpoof/data_io/transform.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/face_id/commons/AntiSpoof/liveness_check.py` & `JustScan-1.1.2/app/JustScan/face_id/commons/AntiSpoof/liveness_check.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/face_id/commons/AntiSpoof/liveness_onnx_check.py` & `JustScan-1.1.2/app/JustScan/face_id/commons/AntiSpoof/liveness_onnx_check.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import onnxruntime as ort
 import cv2
-from ..config import config
+from JustScan.face_id.commons.config import config
 
 model_path = config['face_liveness']
 
 
 def onnx_predict(img, model_paths=model_path):
     img = cv2.resize(img, (112, 112))
     dummy_face = np.expand_dims(np.array(img, dtype=np.float32), axis=0)
```

### Comparing `JustScan-0.0.1/app/JustScan/face_id/commons/AntiSpoof/model_lib/MiniFASNet.py` & `JustScan-1.1.2/app/JustScan/face_id/commons/AntiSpoof/model_lib/MiniFASNet.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/face_id/commons/AntiSpoof/model_lib/MultiFTNet.py` & `JustScan-1.1.2/app/JustScan/face_id/commons/AntiSpoof/model_lib/MultiFTNet.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/face_id/commons/AntiSpoof/utility.py` & `JustScan-1.1.2/app/JustScan/face_id/commons/AntiSpoof/utility.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/face_id/commons/ArcFace/ArcFace_onnx.py` & `JustScan-1.1.2/app/JustScan/face_id/commons/ArcFace/ArcFace_onnx.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import cv2
 import onnx
 import onnxruntime
-from ..config import config
+from JustScan.face_id.commons.config import config
 __all__ = [
     'ArcFaceONNX',
 ]
 
 import warnings
 
 warnings.filterwarnings('ignore')
```

### Comparing `JustScan-0.0.1/app/JustScan/face_id/commons/ArcFace/__init__.py` & `JustScan-1.1.2/app/JustScan/face_id/commons/ArcFace/__init__.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/face_id/commons/ArcFace/lib/layers.py` & `JustScan-1.1.2/app/JustScan/face_id/commons/ArcFace/lib/layers.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/face_id/commons/ArcFace/lib/models.py` & `JustScan-1.1.2/app/JustScan/face_id/commons/ArcFace/lib/models.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/face_id/commons/ArcFace/lib/utils.py` & `JustScan-1.1.2/app/JustScan/face_id/commons/ArcFace/lib/utils.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/face_id/commons/CloseEyes/close_eyes_v2.py` & `JustScan-1.1.2/app/JustScan/face_id/commons/CloseEyes/close_eyes_v2.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import cv2
 import onnxruntime
 from .utils import extract_eye
-from ..config import config
+from JustScan.face_id.config import config
 
 
 # 0: Close 1: Open
 
 def preprocessing(image):
     # img = image[:,:,::-1]
     img = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
```

### Comparing `JustScan-0.0.1/app/JustScan/face_id/commons/CloseEyes/utils.py` & `JustScan-1.1.2/app/JustScan/face_id/commons/CloseEyes/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from fastapi import HTTPException
 import numpy as np
-from config.logger import setup_logger, timeit
+from JustScan.config.logger import setup_logger, timeit
 
 logging = setup_logger(__name__)
 
 
 def extract_eye(image: np.array, left_eye_point, right_eye_point, rectangle_size=55) -> np.array:
     try:
         left_eye_rect = (
```

### Comparing `JustScan-0.0.1/app/JustScan/face_id/commons/FaceMask/face_mask_onnx.py` & `JustScan-1.1.2/app/JustScan/face_id/commons/FaceMask/face_mask_onnx.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import onnxruntime
 import numpy as np
 import cv2
-from ..config import config
+from JustScan.face_id.config import config
 
 
 class FaceMask:
     def __init__(self, model_file=config['face_mask'], session=None):
         assert model_file is not None
         self.model_file = model_file
         self.session = session
```

### Comparing `JustScan-0.0.1/app/JustScan/face_id/commons/FaceQuality/dom.py` & `JustScan-1.1.2/app/JustScan/face_id/commons/FaceQuality/dom.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/face_id/commons/FaceQuality/face_quality_assessment.py` & `JustScan-1.1.2/app/JustScan/face_id/commons/FaceQuality/face_quality_assessment.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/face_id/commons/ScrFd/scrfd.py` & `JustScan-1.1.2/app/JustScan/face_id/commons/ScrFd/scrfd.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/face_id/commons/config.py` & `JustScan-1.1.2/app/JustScan/face_id/commons/config.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/face_id/libraries/face_detection.py` & `JustScan-1.1.2/app/JustScan/face_id/libraries/face_detection.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from ..commons.AntiSpoof.liveness_check import livenesss_predict
 from ..commons.AntiSpoof.liveness_onnx_check import onnx_predict
 from ..commons.CloseEyes.close_eyes_v2 import CloseEyes, crop_eye
 from ..commons.FaceQuality.face_quality_assessment import QualityCheck
 from ..commons.AntiSpoof.CDCN_config import predict_liveness
 from fastapi import HTTPException
 import base64
-from config.logger import setup_logger, timeit
+from JustScan.config.logger import setup_logger, timeit
 
 logging = setup_logger(__name__)
 detector = SCRFD(config['face_detection'])
 check_mask = FaceMask()
 eyes = CloseEyes()
 detector.prepare(0)
```

### Comparing `JustScan-0.0.1/app/JustScan/face_id/libraries/face_id.py` & `JustScan-1.1.2/app/JustScan/face_id/libraries/face_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from collections import defaultdict
 from typing import Tuple
 from ..tools.modules import *
 from ..commons.ArcFace.ArcFace_onnx import ArcFaceONNX
-from database.crud import QueryData
+from JustScan.database.crud import QueryData
 from .face_detection import get_face_location
 from .face_recognition import calculate_embedding, get_feature
-from config.config import RECOGNITION_INIT
-from config.logger import setup_logger, timeit
+from JustScan.config.config import RECOGNITION_INIT
+from JustScan.config.logger import setup_logger, timeit
 
 logging = setup_logger(__name__)
 db = QueryData()
 embedding = ArcFaceONNX()
 
 @timeit(logging)
 def detect_user(image: np.array) -> dict:
```

### Comparing `JustScan-0.0.1/app/JustScan/face_id/tools/modules.py` & `JustScan-1.1.2/app/JustScan/face_id/tools/modules.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from PIL import Image
 import cv2
 import math
 import base64
 import numpy as np
 import onnxruntime as ort
 from fastapi import HTTPException
-from config.logger import setup_logger, timeit
+from JustScan.config.logger import setup_logger, timeit
 
 logging = setup_logger(__name__)
 
 
 def image_bgr(image) -> np.array:
     img_BGR = cv2.imdecode(image, cv2.IMREAD_COLOR)
     return img_BGR
```

### Comparing `JustScan-0.0.1/app/JustScan/ocr/core/commons/SpoofingNID.py` & `JustScan-1.1.2/app/JustScan/ocr/core/commons/SpoofingNID.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/ocr/core/commons/config.py` & `JustScan-1.1.2/app/JustScan/ocr/core/commons/config.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/ocr/core/commons/id_card_classification.py` & `JustScan-1.1.2/app/JustScan/ocr/core/commons/id_card_classification.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/ocr/core/commons/id_card_onnx.py` & `JustScan-1.1.2/app/JustScan/ocr/core/commons/id_card_onnx.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/ocr/core/commons/merge_model.py` & `JustScan-1.1.2/app/JustScan/ocr/core/commons/merge_model.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/ocr/core/commons/utils/utils_onnx.py` & `JustScan-1.1.2/app/JustScan/ocr/core/commons/utils/utils_onnx.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 from fastapi import HTTPException
-from config.logger import setup_logger
+from JustScan.config.logger import setup_logger
 
 logging = setup_logger(__name__)
 
 
 def nms(boxes, scores, iou_threshold):
     sorted_indices = np.argsort(scores)[::-1]
```

### Comparing `JustScan-0.0.1/app/JustScan/ocr/core/modules/corner_detection/id_card_aligment.py` & `JustScan-1.1.2/app/JustScan/ocr/core/modules/corner_detection/id_card_aligment.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,16 @@
 from .utils import *
 from fastapi import HTTPException
-from config.logger import setup_logger
+from JustScan.config.logger import setup_logger
 
 logging = setup_logger(__name__)
 
 
-# def align_image(image, boxes_crop, df_crop):
-#     label_boxes, _ = check_label(boxes_crop, df_crop['class_name'])
-#     if len(label_boxes) == 3:
-#         coordinate_dict = calculate_missed_coord_corner(label_boxes)
-#         source_points = np.float32(
-#             [coordinate_dict['top_left'], coordinate_dict['top_right'], coordinate_dict['bottom_right'],
-#              coordinate_dict['bottom_left']])
-#         return perspective_transform(image, source_points)
-#
-#     elif len(label_boxes) == 4:
-#         source_points = np.float32(
-#             [label_boxes['top_left'], label_boxes['top_right'], label_boxes['bottom_right'],
-#              label_boxes['bottom_left']])
-#         return perspective_transform(image, source_points)
-#     else:
-#         logging.error(f'error at running {align_image.__name__}, cannot align id card')
-#         raise HTTPException(status_code=400,
-#                             detail={'status': 400, 'code': 'ID_CARD_NOT_ALIGN',
-#                                     'error': 'Cannot align id card'})
-
 def align_image(image, boxes_crop, df_crop):
-    label_boxes, _ = check_label(boxes_crop, df_crop[:,0])
+    label_boxes, _ = check_label(boxes_crop, df_crop[:, 0])
     if len(label_boxes) == 3:
         coordinate_dict = calculate_missed_coord_corner(label_boxes)
         source_points = np.float32(
             [coordinate_dict['top_left'], coordinate_dict['top_right'], coordinate_dict['bottom_right'],
              coordinate_dict['bottom_left']])
         return perspective_transform(image, source_points)
 
@@ -39,8 +19,8 @@
             [label_boxes['top_left'], label_boxes['top_right'], label_boxes['bottom_right'],
              label_boxes['bottom_left']])
         return perspective_transform(image, source_points)
     else:
         logging.error(f'error at running {align_image.__name__}, cannot align id card')
         raise HTTPException(status_code=400,
                             detail={'status': 400, 'code': 'ID_CARD_NOT_ALIGN',
-                                    'error': 'Cannot align id card'})
+                                    'error': 'Cannot align id card'})
```

### Comparing `JustScan-0.0.1/app/JustScan/ocr/core/modules/corner_detection/utils.py` & `JustScan-1.1.2/app/JustScan/ocr/core/modules/corner_detection/utils.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/ocr/core/modules/id_card_classification/classify.py` & `JustScan-1.1.2/app/JustScan/ocr/core/modules/id_card_classification/classify.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from fastapi import HTTPException
 from typing import Tuple
 from ...commons.merge_model import MergeIdCardModel
 import numpy as np
-from config.logger import setup_logger
+from JustScan.config.logger import setup_logger
 logging = setup_logger(__name__)
 
 
 def process_classification(image: np.array) -> Tuple[np.ndarray, list, float]:
     # return label, confidence
     label, confidence = MergeIdCardModel().classify_card(image)
     if label is None or label in [1, 3] or confidence < 0.8:
```

### Comparing `JustScan-0.0.1/app/JustScan/ocr/core/modules/mrc/mrc_detection.py` & `JustScan-1.1.2/app/JustScan/ocr/core/modules/mrc/mrc_detection.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from ..text_detection.dictionary import IDcardPreprocessing
 from ...commons.merge_model import MergeIdCardModel
 from ..text_detection.utils import *
 from ...tools.api_json import *
 from typing import Tuple
-from config.logger import setup_logger
+from JustScan.config.logger import setup_logger
 logging = setup_logger(__name__)
 
 
 def get_mrc_alignment(image: np.array) -> Tuple[np.array, dict]:
     try:
         crop_model = MergeIdCardModel().detect_corner(image, mrc=True)
         return crop_model
```

### Comparing `JustScan-0.0.1/app/JustScan/ocr/core/modules/mrc/utils.py` & `JustScan-1.1.2/app/JustScan/ocr/core/modules/mrc/utils.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/ocr/core/modules/passport/passport.py` & `JustScan-1.1.2/app/JustScan/ocr/core/modules/passport/passport.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import time
 import onnxruntime
 from fastapi import HTTPException
 from ...commons.config import config
 from ..passport.utils_align_passport.utils_align import *
 from ..passport.utils_align_passport.passport_utils import xywh2xyxy, nms, sigmoid, \
     get_label
-from config.logger import setup_logger
+from JustScan.config.logger import setup_logger
 from scipy.ndimage import interpolation as inter
 
 logging = setup_logger(__name__)
 
 
 class Passport:
```

### Comparing `JustScan-0.0.1/app/JustScan/ocr/core/modules/passport/utils.py` & `JustScan-1.1.2/app/JustScan/ocr/core/modules/passport/utils.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/ocr/core/modules/passport/utils_align_passport/passport_utils.py` & `JustScan-1.1.2/app/JustScan/ocr/core/modules/passport/utils_align_passport/passport_utils.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/ocr/core/modules/passport/utils_align_passport/utils_align.py` & `JustScan-1.1.2/app/JustScan/ocr/core/modules/passport/utils_align_passport/utils_align.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/ocr/core/modules/passport/utils_detect_passport/utils_detect.py` & `JustScan-1.1.2/app/JustScan/ocr/core/modules/passport/utils_detect_passport/utils_detect.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from fastapi import HTTPException
 import numpy as np
 import cv2
-from config.logger import setup_logger
+from JustScan.config.logger import setup_logger
 logging = setup_logger(__name__)
 
 
 def non_max_suppression_fast(boxes, labels, confidence, ids, overlapThresh):
     outs = dict()
     if len(boxes) == 0:
         out = {
```

### Comparing `JustScan-0.0.1/app/JustScan/ocr/core/modules/quality_liveness_nid_checking/nid_quality_liveness_check.py` & `JustScan-1.1.2/app/JustScan/ocr/core/modules/quality_liveness_nid_checking/nid_quality_liveness_check.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import cv2
 import numpy as np
 import math
 from face_id.commons.FaceQuality.dom import DOM
 from ...commons.SpoofingNID import SpoofingNIDModel
 from fastapi import HTTPException
-from config.logger import setup_logger
+from JustScan.config.logger import setup_logger
 
 logging = setup_logger(__name__)
 
 MIN_SHARPNESS = 0.46
 MIN_CONTRAST = 0.35
 MIN_BRIGHTNESS = 0.3
 MIN_BLUR = 100
```

### Comparing `JustScan-0.0.1/app/JustScan/ocr/core/modules/spell_checking/corrector_v2.py` & `JustScan-1.1.2/app/JustScan/ocr/core/modules/spell_checking/corrector_v2.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/ocr/core/modules/spoofing_nid/spoofing.py` & `JustScan-1.1.2/app/JustScan/ocr/core/modules/spoofing_nid/spoofing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from ...commons.SpoofingNID import SpoofingNIDModel
 from fastapi import HTTPException
-from config.logger import setup_logger
+from JustScan.config.logger import setup_logger
 
 logging = setup_logger(__name__)
 
 
 def check_spoof_nid(image):
     label_spoof, confidence_spoof = SpoofingNIDModel().predict(image)
     try:
```

### Comparing `JustScan-0.0.1/app/JustScan/ocr/core/modules/text_detection/dictionary.py` & `JustScan-1.1.2/app/JustScan/ocr/core/modules/text_detection/dictionary.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/ocr/core/modules/text_detection/utils.py` & `JustScan-1.1.2/app/JustScan/ocr/core/modules/text_detection/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from fastapi import HTTPException
-from config.logger import setup_logger
+from JustScan.config.logger import setup_logger
 from datetime import datetime
 import numpy as np
 import cv2
 import re
 
 logging = setup_logger(__name__)
```

### Comparing `JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/nlp_onnx.py` & `JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/nlp_onnx.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/aug.py` & `JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/aug.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/dataloader.py` & `JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/dataloader.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/dataloader_v1.py` & `JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/loader/dataloader_v1.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/cnn.py` & `JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/cnn.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/resnet.py` & `JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/resnet.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/vgg.py` & `JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/vgg.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/beam.py` & `JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/beam.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/convseq2seq.py` & `JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/convseq2seq.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/seq2seq.py` & `JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/seq2seq.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/transformer.py` & `JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/transformer.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/trainer.py` & `JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/trainer.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/transformerocr.py` & `JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/transformerocr.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/vocab.py` & `JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/model/vocab.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/optim/labelsmoothingloss.py` & `JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/optim/labelsmoothingloss.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/optim/optim.py` & `JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/optim/optim.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/predict.py` & `JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/predict.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tests/utest.py` & `JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tests/utest.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/config.py` & `JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/config.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/create_dataset.py` & `JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/create_dataset.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/predictor.py` & `JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/predictor.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/translate.py` & `JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/translate.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/utils.py` & `JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/tool/utils.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/train.py` & `JustScan-1.1.2/app/JustScan/ocr/core/modules/vietnamese_nlp/vietocr/train.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/ocr/core/tools/api_json.py` & `JustScan-1.1.2/app/JustScan/ocr/core/tools/api_json.py`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/app/JustScan/ocr/core/tools/dictionaries.py` & `JustScan-1.1.2/app/JustScan/ocr/core/tools/dictionaries.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from ..modules.text_detection.dictionary import IDcardPreprocessing
 from ..modules.text_detection.utils import *
-from .api_json import *
 from ..commons.merge_model import MergeIdCardModel
+from .api_json import *
 from fastapi import HTTPException
 
 
 class DictionaryCCCD(object):
     def __init__(self):
         pass
```

### Comparing `JustScan-0.0.1/app/JustScan/ocr/core/tools/functional.py` & `JustScan-1.1.2/app/JustScan/ocr/core/tools/functional.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .dictionaries import DictionaryCCCD
 from fastapi import HTTPException
 from typing import Tuple
 from scipy.ndimage import interpolation as inter
 from ..commons.merge_model import MergeIdCardModel
-from config.logger import setup_logger
+from JustScan.config.logger import setup_logger
 import numpy as np
 import cv2
 
 logging = setup_logger(__name__)
 
 
 def correct_skew(image, delta=1, limit=5):
```

### Comparing `JustScan-0.0.1/app/JustScan.egg-info/PKG-INFO` & `JustScan-1.1.2/app/JustScan.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: JustScan
-Version: 0.0.1
+Version: 1.1.2
 Summary: E-kyc for Industries application
 Home-page: https://github.com/aihackervn
 Author: Theodore
 Author-email: tinprocoder0908@gmail.com
 License: MIT
+Keywords: ITC,AI,E-kyc,Deep Learning,Computer Vision,Yolov5,Interface
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `JustScan-0.0.1/app/JustScan.egg-info/SOURCES.txt` & `JustScan-1.1.2/app/JustScan.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -50,16 +50,14 @@
 app/JustScan/face_id/commons/FaceQuality/face_quality_assessment.py
 app/JustScan/face_id/commons/ScrFd/__init__.py
 app/JustScan/face_id/commons/ScrFd/scrfd.py
 app/JustScan/face_id/libraries/__init__.py
 app/JustScan/face_id/libraries/face_detection.py
 app/JustScan/face_id/libraries/face_id.py
 app/JustScan/face_id/libraries/face_recognition.py
-app/JustScan/face_id/testing/__init__.py
-app/JustScan/face_id/testing/scrfd_testing.py
 app/JustScan/face_id/tools/__init__.py
 app/JustScan/face_id/tools/modules.py
 app/JustScan/ocr/__init__.py
 app/JustScan/ocr/core/__init__.py
 app/JustScan/ocr/core/commons/SpoofingNID.py
 app/JustScan/ocr/core/commons/__init__.py
 app/JustScan/ocr/core/commons/config.py
```

### Comparing `JustScan-0.0.1/app/JustScan.egg-info/requires.txt` & `JustScan-1.1.2/app/JustScan.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `JustScan-0.0.1/setup.py` & `JustScan-1.1.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 from setuptools import find_packages, setup
 with open("README.md", "r") as f:
     long_description = f.read()
 with open("requirements.txt", "r") as f:
     install_requires = [line.strip() for line in f if line.strip()]
 setup(
     name="JustScan",
-    version="0.0.1",
+    version="1.1.2",
     description="E-kyc for Industries application",
     package_dir={"": "app"},
     packages=find_packages(where="./app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aihackervn",
     author="Theodore",
     author_email="tinprocoder0908@gmail.com",
+    keywords=["ITC", "AI", "E-kyc", "Deep Learning", "Computer Vision", "Yolov5",
+              "Interface"],
+
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.9",
         "Operating System :: OS Independent",
     ],
     install_requires=install_requires,
     entry_points={
         'console_scripts': [
-            'itc_ai = api.itc_cli:main',
+            'itc_service = JustScan.api.itc_cli:main',
         ],
     },
     extras_require={
         "dev": ["pytest>=7.0", "twine>=4.0.2"],
     },
     python_requires=">=3.9"
 )
```

