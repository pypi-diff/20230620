# Comparing `tmp/app_ocr-0.0.2.tar.gz` & `tmp/app_ocr-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "app_ocr-0.0.2.tar", last modified: Tue Jun 20 07:39:02 2023, max compression
+gzip compressed data, was "app_ocr-0.0.3.tar", last modified: Tue Jun 20 08:01:36 2023, max compression
```

## Comparing `app_ocr-0.0.2.tar` & `app_ocr-0.0.3.tar`

### file list

```diff
@@ -1,177 +1,177 @@
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 07:39:02.175768 app_ocr-0.0.2/
--rw-r--r--   0 macbook    (501) staff       (20)     2567 2023-06-20 07:39:02.175623 app_ocr-0.0.2/PKG-INFO
--rw-r--r--   0 macbook    (501) staff       (20)     2131 2023-04-12 07:19:45.000000 app_ocr-0.0.2/README.md
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 07:39:02.154573 app_ocr-0.0.2/app/
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 07:39:02.157242 app_ocr-0.0.2/app/app_ocr.egg-info/
--rw-r--r--   0 macbook    (501) staff       (20)     2567 2023-06-20 07:39:02.000000 app_ocr-0.0.2/app/app_ocr.egg-info/PKG-INFO
--rw-r--r--   0 macbook    (501) staff       (20)     6084 2023-06-20 07:39:02.000000 app_ocr-0.0.2/app/app_ocr.egg-info/SOURCES.txt
--rw-r--r--   0 macbook    (501) staff       (20)        1 2023-06-20 07:39:02.000000 app_ocr-0.0.2/app/app_ocr.egg-info/dependency_links.txt
--rw-r--r--   0 macbook    (501) staff       (20)      864 2023-06-20 07:39:02.000000 app_ocr-0.0.2/app/app_ocr.egg-info/requires.txt
--rw-r--r--   0 macbook    (501) staff       (20)       28 2023-06-20 07:39:02.000000 app_ocr-0.0.2/app/app_ocr.egg-info/top_level.txt
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 07:39:02.157903 app_ocr-0.0.2/app/config/
--rw-r--r--   0 macbook    (501) staff       (20)      100 2023-06-20 07:14:31.000000 app_ocr-0.0.2/app/config/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     1306 2023-06-01 06:55:11.000000 app_ocr-0.0.2/app/config/config.py
--rw-r--r--   0 macbook    (501) staff       (20)      393 2023-04-12 07:19:45.000000 app_ocr-0.0.2/app/config/config_db.py
--rw-r--r--   0 macbook    (501) staff       (20)     1080 2023-06-01 06:55:11.000000 app_ocr-0.0.2/app/config/logger.py
--rw-r--r--   0 macbook    (501) staff       (20)     4337 2023-05-09 09:10:33.000000 app_ocr-0.0.2/app/config/pydantic_models.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 07:39:02.158438 app_ocr-0.0.2/app/database/
--rw-r--r--   0 macbook    (501) staff       (20)       71 2023-06-20 07:14:31.000000 app_ocr-0.0.2/app/database/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     4406 2023-04-12 07:19:45.000000 app_ocr-0.0.2/app/database/crud.py
--rw-r--r--   0 macbook    (501) staff       (20)      720 2023-06-20 07:27:46.000000 app_ocr-0.0.2/app/database/data_models.py
--rw-r--r--   0 macbook    (501) staff       (20)      565 2023-04-21 09:57:32.000000 app_ocr-0.0.2/app/database/database.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 07:39:02.158569 app_ocr-0.0.2/app/face_id/
--rw-r--r--   0 macbook    (501) staff       (20)       66 2023-06-20 07:09:37.000000 app_ocr-0.0.2/app/face_id/__init__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 07:39:02.158826 app_ocr-0.0.2/app/face_id/commons/
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 07:39:02.159615 app_ocr-0.0.2/app/face_id/commons/AntiSpoof/
--rw-r--r--   0 macbook    (501) staff       (20)     2206 2023-04-12 07:19:45.000000 app_ocr-0.0.2/app/face_id/commons/AntiSpoof/CDCN_config.py
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 app_ocr-0.0.2/app/face_id/commons/AntiSpoof/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     2037 2023-04-12 07:19:45.000000 app_ocr-0.0.2/app/face_id/commons/AntiSpoof/anti_spoof.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 07:39:02.160014 app_ocr-0.0.2/app/face_id/commons/AntiSpoof/data_io/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 app_ocr-0.0.2/app/face_id/commons/AntiSpoof/data_io/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)    20275 2023-04-12 07:19:45.000000 app_ocr-0.0.2/app/face_id/commons/AntiSpoof/data_io/functional.py
--rw-r--r--   0 macbook    (501) staff       (20)    11464 2023-04-12 07:19:45.000000 app_ocr-0.0.2/app/face_id/commons/AntiSpoof/data_io/transform.py
--rw-r--r--   0 macbook    (501) staff       (20)      802 2023-04-12 07:19:45.000000 app_ocr-0.0.2/app/face_id/commons/AntiSpoof/liveness_check.py
--rw-r--r--   0 macbook    (501) staff       (20)     1397 2023-06-20 07:27:46.000000 app_ocr-0.0.2/app/face_id/commons/AntiSpoof/liveness_onnx_check.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 07:39:02.160442 app_ocr-0.0.2/app/face_id/commons/AntiSpoof/model_lib/
--rw-r--r--   0 macbook    (501) staff       (20)    12487 2023-04-12 07:19:45.000000 app_ocr-0.0.2/app/face_id/commons/AntiSpoof/model_lib/MiniFASNet.py
--rw-r--r--   0 macbook    (501) staff       (20)     2803 2023-04-12 07:19:45.000000 app_ocr-0.0.2/app/face_id/commons/AntiSpoof/model_lib/MultiFTNet.py
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 app_ocr-0.0.2/app/face_id/commons/AntiSpoof/model_lib/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)      990 2023-04-12 07:19:45.000000 app_ocr-0.0.2/app/face_id/commons/AntiSpoof/utility.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 07:39:02.160720 app_ocr-0.0.2/app/face_id/commons/ArcFace/
--rw-r--r--   0 macbook    (501) staff       (20)     2999 2023-06-20 07:27:46.000000 app_ocr-0.0.2/app/face_id/commons/ArcFace/ArcFace_onnx.py
--rw-r--r--   0 macbook    (501) staff       (20)      978 2023-04-12 07:19:45.000000 app_ocr-0.0.2/app/face_id/commons/ArcFace/__init__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 07:39:02.161235 app_ocr-0.0.2/app/face_id/commons/ArcFace/lib/
--rw-r--r--   0 macbook    (501) staff       (20)      186 2023-04-12 07:19:45.000000 app_ocr-0.0.2/app/face_id/commons/ArcFace/lib/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     3036 2023-04-12 07:19:45.000000 app_ocr-0.0.2/app/face_id/commons/ArcFace/lib/layers.py
--rw-r--r--   0 macbook    (501) staff       (20)     4284 2023-04-12 07:19:45.000000 app_ocr-0.0.2/app/face_id/commons/ArcFace/lib/models.py
--rw-r--r--   0 macbook    (501) staff       (20)     2436 2023-04-12 07:19:45.000000 app_ocr-0.0.2/app/face_id/commons/ArcFace/lib/utils.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 07:39:02.161800 app_ocr-0.0.2/app/face_id/commons/CloseEyes/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 app_ocr-0.0.2/app/face_id/commons/CloseEyes/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     3114 2023-06-20 07:27:46.000000 app_ocr-0.0.2/app/face_id/commons/CloseEyes/close_eyes.py
--rw-r--r--   0 macbook    (501) staff       (20)     1128 2023-06-20 07:27:46.000000 app_ocr-0.0.2/app/face_id/commons/CloseEyes/close_eyes_v2.py
--rw-r--r--   0 macbook    (501) staff       (20)     1310 2023-06-20 07:27:46.000000 app_ocr-0.0.2/app/face_id/commons/CloseEyes/utils.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 07:39:02.162271 app_ocr-0.0.2/app/face_id/commons/FaceMask/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 app_ocr-0.0.2/app/face_id/commons/FaceMask/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)      807 2023-06-20 07:27:46.000000 app_ocr-0.0.2/app/face_id/commons/FaceMask/face_mask_onnx.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 07:39:02.162874 app_ocr-0.0.2/app/face_id/commons/FaceQuality/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 app_ocr-0.0.2/app/face_id/commons/FaceQuality/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     9974 2023-06-01 06:55:11.000000 app_ocr-0.0.2/app/face_id/commons/FaceQuality/dom.py
--rw-r--r--   0 macbook    (501) staff       (20)     1886 2023-06-20 07:27:46.000000 app_ocr-0.0.2/app/face_id/commons/FaceQuality/face_quality_assessment.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 07:39:02.163182 app_ocr-0.0.2/app/face_id/commons/ScrFd/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 app_ocr-0.0.2/app/face_id/commons/ScrFd/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)    12632 2023-06-01 06:55:11.000000 app_ocr-0.0.2/app/face_id/commons/ScrFd/scrfd.py
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 app_ocr-0.0.2/app/face_id/commons/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     2297 2023-06-19 18:18:48.000000 app_ocr-0.0.2/app/face_id/commons/config.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 07:39:02.163791 app_ocr-0.0.2/app/face_id/libraries/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 app_ocr-0.0.2/app/face_id/libraries/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     7320 2023-06-20 07:27:46.000000 app_ocr-0.0.2/app/face_id/libraries/face_detection.py
--rw-r--r--   0 macbook    (501) staff       (20)     5372 2023-05-30 04:20:28.000000 app_ocr-0.0.2/app/face_id/libraries/face_id.py
--rw-r--r--   0 macbook    (501) staff       (20)      415 2023-04-12 07:19:45.000000 app_ocr-0.0.2/app/face_id/libraries/face_recognition.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 07:39:02.164062 app_ocr-0.0.2/app/face_id/testing/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 07:28:07.000000 app_ocr-0.0.2/app/face_id/testing/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)      963 2023-06-20 07:27:46.000000 app_ocr-0.0.2/app/face_id/testing/scrfd_testing.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 07:39:02.164327 app_ocr-0.0.2/app/face_id/tools/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 app_ocr-0.0.2/app/face_id/tools/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     4042 2023-04-12 07:19:46.000000 app_ocr-0.0.2/app/face_id/tools/modules.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 07:39:02.164453 app_ocr-0.0.2/app/ocr/
--rw-r--r--   0 macbook    (501) staff       (20)       19 2023-06-20 07:08:18.000000 app_ocr-0.0.2/app/ocr/__init__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 07:39:02.164679 app_ocr-0.0.2/app/ocr/core/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 07:27:46.000000 app_ocr-0.0.2/app/ocr/core/__init__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 07:39:02.165522 app_ocr-0.0.2/app/ocr/core/commons/
--rw-r--r--   0 macbook    (501) staff       (20)      825 2023-06-19 13:32:54.000000 app_ocr-0.0.2/app/ocr/core/commons/SpoofingNID.py
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 app_ocr-0.0.2/app/ocr/core/commons/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     5614 2023-06-19 17:59:34.000000 app_ocr-0.0.2/app/ocr/core/commons/config.py
--rw-r--r--   0 macbook    (501) staff       (20)      780 2023-05-30 04:20:28.000000 app_ocr-0.0.2/app/ocr/core/commons/id_card_classification.py
--rw-r--r--   0 macbook    (501) staff       (20)     5687 2023-06-19 17:59:06.000000 app_ocr-0.0.2/app/ocr/core/commons/id_card_onnx.py
--rw-r--r--   0 macbook    (501) staff       (20)     1805 2023-06-01 06:55:11.000000 app_ocr-0.0.2/app/ocr/core/commons/merge_model.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 07:39:02.165777 app_ocr-0.0.2/app/ocr/core/commons/utils/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 07:28:07.000000 app_ocr-0.0.2/app/ocr/core/commons/utils/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     2508 2023-05-30 04:20:28.000000 app_ocr-0.0.2/app/ocr/core/commons/utils/utils_onnx.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 07:39:02.165927 app_ocr-0.0.2/app/ocr/core/modules/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.2/app/ocr/core/modules/__init__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 07:39:02.166291 app_ocr-0.0.2/app/ocr/core/modules/corner_detection/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.2/app/ocr/core/modules/corner_detection/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     2227 2023-06-15 03:28:33.000000 app_ocr-0.0.2/app/ocr/core/modules/corner_detection/id_card_aligment.py
--rw-r--r--   0 macbook    (501) staff       (20)     3973 2023-06-19 14:29:56.000000 app_ocr-0.0.2/app/ocr/core/modules/corner_detection/utils.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 07:39:02.166568 app_ocr-0.0.2/app/ocr/core/modules/id_card_classification/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.2/app/ocr/core/modules/id_card_classification/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)      928 2023-06-15 07:52:38.000000 app_ocr-0.0.2/app/ocr/core/modules/id_card_classification/classify.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 07:39:02.166944 app_ocr-0.0.2/app/ocr/core/modules/mrc/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.2/app/ocr/core/modules/mrc/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     2991 2023-06-15 07:52:38.000000 app_ocr-0.0.2/app/ocr/core/modules/mrc/mrc_detection.py
--rw-r--r--   0 macbook    (501) staff       (20)      647 2023-04-12 07:19:46.000000 app_ocr-0.0.2/app/ocr/core/modules/mrc/utils.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 07:39:02.167543 app_ocr-0.0.2/app/ocr/core/modules/passport/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-18 03:26:14.000000 app_ocr-0.0.2/app/ocr/core/modules/passport/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     9115 2023-06-19 13:30:20.000000 app_ocr-0.0.2/app/ocr/core/modules/passport/passport.py
--rw-r--r--   0 macbook    (501) staff       (20)      530 2023-06-19 13:30:20.000000 app_ocr-0.0.2/app/ocr/core/modules/passport/passport_detection.py
--rw-r--r--   0 macbook    (501) staff       (20)     2346 2023-06-15 07:52:38.000000 app_ocr-0.0.2/app/ocr/core/modules/passport/utils.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 07:39:02.167996 app_ocr-0.0.2/app/ocr/core/modules/passport/utils_align_passport/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-18 03:26:14.000000 app_ocr-0.0.2/app/ocr/core/modules/passport/utils_align_passport/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     3248 2023-04-18 08:29:08.000000 app_ocr-0.0.2/app/ocr/core/modules/passport/utils_align_passport/passport_utils.py
--rw-r--r--   0 macbook    (501) staff       (20)     4344 2023-04-18 03:26:14.000000 app_ocr-0.0.2/app/ocr/core/modules/passport/utils_align_passport/utils_align.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 07:39:02.168285 app_ocr-0.0.2/app/ocr/core/modules/passport/utils_detect_passport/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-18 03:26:14.000000 app_ocr-0.0.2/app/ocr/core/modules/passport/utils_detect_passport/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     9663 2023-06-19 14:29:46.000000 app_ocr-0.0.2/app/ocr/core/modules/passport/utils_detect_passport/utils_detect.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 07:39:02.168599 app_ocr-0.0.2/app/ocr/core/modules/quality_liveness_nid_checking/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-26 09:38:30.000000 app_ocr-0.0.2/app/ocr/core/modules/quality_liveness_nid_checking/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     2936 2023-06-01 06:55:11.000000 app_ocr-0.0.2/app/ocr/core/modules/quality_liveness_nid_checking/nid_quality_liveness_check.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 07:39:02.168879 app_ocr-0.0.2/app/ocr/core/modules/spell_checking/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.2/app/ocr/core/modules/spell_checking/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     2350 2023-05-10 09:12:33.000000 app_ocr-0.0.2/app/ocr/core/modules/spell_checking/corrector_v2.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 07:39:02.169180 app_ocr-0.0.2/app/ocr/core/modules/spoofing_nid/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.2/app/ocr/core/modules/spoofing_nid/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)      940 2023-04-21 08:38:53.000000 app_ocr-0.0.2/app/ocr/core/modules/spoofing_nid/spoofing.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 07:39:02.169628 app_ocr-0.0.2/app/ocr/core/modules/text_detection/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.2/app/ocr/core/modules/text_detection/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     7125 2023-06-19 13:32:54.000000 app_ocr-0.0.2/app/ocr/core/modules/text_detection/dictionary.py
--rw-r--r--   0 macbook    (501) staff       (20)    11597 2023-06-19 14:29:12.000000 app_ocr-0.0.2/app/ocr/core/modules/text_detection/utils.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 07:39:02.169919 app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     2549 2023-05-30 04:20:28.000000 app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/nlp_onnx.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 07:39:02.170341 app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/__init__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 07:39:02.170970 app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/loader/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/loader/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     1735 2023-04-12 07:19:46.000000 app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/loader/aug.py
--rw-r--r--   0 macbook    (501) staff       (20)     6278 2023-04-12 07:19:46.000000 app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/loader/dataloader.py
--rw-r--r--   0 macbook    (501) staff       (20)     5021 2023-04-12 07:19:46.000000 app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/loader/dataloader_v1.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 07:39:02.171741 app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/model/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/model/__init__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 07:39:02.172327 app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)      888 2023-04-12 07:19:46.000000 app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/cnn.py
--rw-r--r--   0 macbook    (501) staff       (20)     5311 2023-04-12 07:19:46.000000 app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/resnet.py
--rw-r--r--   0 macbook    (501) staff       (20)     1655 2023-04-12 07:19:46.000000 app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/vgg.py
--rw-r--r--   0 macbook    (501) staff       (20)     3777 2023-04-12 07:19:46.000000 app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/model/beam.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 07:39:02.172925 app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)    11634 2023-04-12 07:19:46.000000 app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/convseq2seq.py
--rw-r--r--   0 macbook    (501) staff       (20)     5731 2023-04-12 07:19:46.000000 app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/seq2seq.py
--rw-r--r--   0 macbook    (501) staff       (20)     4858 2023-04-12 07:19:46.000000 app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/transformer.py
--rw-r--r--   0 macbook    (501) staff       (20)    13524 2023-04-12 07:19:46.000000 app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/model/trainer.py
--rw-r--r--   0 macbook    (501) staff       (20)     1762 2023-04-12 07:19:46.000000 app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/model/transformerocr.py
--rw-r--r--   0 macbook    (501) staff       (20)      924 2023-05-10 09:12:33.000000 app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/model/vocab.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 07:39:02.173377 app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/optim/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/optim/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     1006 2023-04-12 07:19:46.000000 app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/optim/labelsmoothingloss.py
--rw-r--r--   0 macbook    (501) staff       (20)     1798 2023-04-12 07:19:46.000000 app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/optim/optim.py
--rw-r--r--   0 macbook    (501) staff       (20)      538 2023-04-12 07:19:46.000000 app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/predict.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 07:39:02.173658 app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/tests/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/tests/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     1039 2023-04-12 07:19:46.000000 app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/tests/utest.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 07:39:02.174756 app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/tool/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/tool/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     1258 2023-04-12 07:19:46.000000 app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/tool/config.py
--rw-r--r--   0 macbook    (501) staff       (20)     2754 2023-04-12 07:19:46.000000 app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/tool/create_dataset.py
--rw-r--r--   0 macbook    (501) staff       (20)      325 2023-04-12 07:19:46.000000 app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/tool/logger.py
--rw-r--r--   0 macbook    (501) staff       (20)     1427 2023-04-12 07:19:46.000000 app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/tool/predictor.py
--rw-r--r--   0 macbook    (501) staff       (20)     7412 2023-06-01 06:55:11.000000 app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/tool/translate.py
--rw-r--r--   0 macbook    (501) staff       (20)     2688 2023-04-12 07:19:46.000000 app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/tool/utils.py
--rw-r--r--   0 macbook    (501) staff       (20)      559 2023-04-12 07:19:46.000000 app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/train.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 07:39:02.175420 app_ocr-0.0.2/app/ocr/core/tools/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 app_ocr-0.0.2/app/ocr/core/tools/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     5552 2023-04-18 03:26:14.000000 app_ocr-0.0.2/app/ocr/core/tools/api_json.py
--rw-r--r--   0 macbook    (501) staff       (20)     5584 2023-06-01 06:55:11.000000 app_ocr-0.0.2/app/ocr/core/tools/dictionaries.py
--rw-r--r--   0 macbook    (501) staff       (20)     2542 2023-06-01 06:55:11.000000 app_ocr-0.0.2/app/ocr/core/tools/functional.py
--rw-r--r--   0 macbook    (501) staff       (20)       38 2023-06-20 07:39:02.175814 app_ocr-0.0.2/setup.cfg
--rw-r--r--   0 macbook    (501) staff       (20)      925 2023-06-20 07:38:49.000000 app_ocr-0.0.2/setup.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 08:01:36.210596 app_ocr-0.0.3/
+-rw-r--r--   0 macbook    (501) staff       (20)     2567 2023-06-20 08:01:36.210453 app_ocr-0.0.3/PKG-INFO
+-rw-r--r--   0 macbook    (501) staff       (20)     2131 2023-04-12 07:19:45.000000 app_ocr-0.0.3/README.md
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 08:01:36.188723 app_ocr-0.0.3/app/
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 08:01:36.191796 app_ocr-0.0.3/app/app_ocr.egg-info/
+-rw-r--r--   0 macbook    (501) staff       (20)     2567 2023-06-20 08:01:36.000000 app_ocr-0.0.3/app/app_ocr.egg-info/PKG-INFO
+-rw-r--r--   0 macbook    (501) staff       (20)     6084 2023-06-20 08:01:36.000000 app_ocr-0.0.3/app/app_ocr.egg-info/SOURCES.txt
+-rw-r--r--   0 macbook    (501) staff       (20)        1 2023-06-20 08:01:36.000000 app_ocr-0.0.3/app/app_ocr.egg-info/dependency_links.txt
+-rw-r--r--   0 macbook    (501) staff       (20)      864 2023-06-20 08:01:36.000000 app_ocr-0.0.3/app/app_ocr.egg-info/requires.txt
+-rw-r--r--   0 macbook    (501) staff       (20)       28 2023-06-20 08:01:36.000000 app_ocr-0.0.3/app/app_ocr.egg-info/top_level.txt
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 08:01:36.192603 app_ocr-0.0.3/app/config/
+-rw-r--r--   0 macbook    (501) staff       (20)      100 2023-06-20 07:14:31.000000 app_ocr-0.0.3/app/config/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1295 2023-06-20 07:54:35.000000 app_ocr-0.0.3/app/config/config.py
+-rw-r--r--   0 macbook    (501) staff       (20)      393 2023-04-12 07:19:45.000000 app_ocr-0.0.3/app/config/config_db.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1085 2023-06-20 07:52:59.000000 app_ocr-0.0.3/app/config/logger.py
+-rw-r--r--   0 macbook    (501) staff       (20)     4337 2023-05-09 09:10:33.000000 app_ocr-0.0.3/app/config/pydantic_models.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 08:01:36.193229 app_ocr-0.0.3/app/database/
+-rw-r--r--   0 macbook    (501) staff       (20)       71 2023-06-20 07:14:31.000000 app_ocr-0.0.3/app/database/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     4404 2023-06-20 07:55:12.000000 app_ocr-0.0.3/app/database/crud.py
+-rw-r--r--   0 macbook    (501) staff       (20)      720 2023-06-20 07:27:46.000000 app_ocr-0.0.3/app/database/data_models.py
+-rw-r--r--   0 macbook    (501) staff       (20)      563 2023-06-20 08:00:29.000000 app_ocr-0.0.3/app/database/database.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 08:01:36.193385 app_ocr-0.0.3/app/face_id/
+-rw-r--r--   0 macbook    (501) staff       (20)       66 2023-06-20 07:09:37.000000 app_ocr-0.0.3/app/face_id/__init__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 08:01:36.193673 app_ocr-0.0.3/app/face_id/commons/
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 08:01:36.194590 app_ocr-0.0.3/app/face_id/commons/AntiSpoof/
+-rw-r--r--   0 macbook    (501) staff       (20)     2206 2023-04-12 07:19:45.000000 app_ocr-0.0.3/app/face_id/commons/AntiSpoof/CDCN_config.py
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 app_ocr-0.0.3/app/face_id/commons/AntiSpoof/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2037 2023-04-12 07:19:45.000000 app_ocr-0.0.3/app/face_id/commons/AntiSpoof/anti_spoof.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 08:01:36.195033 app_ocr-0.0.3/app/face_id/commons/AntiSpoof/data_io/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 app_ocr-0.0.3/app/face_id/commons/AntiSpoof/data_io/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)    20275 2023-04-12 07:19:45.000000 app_ocr-0.0.3/app/face_id/commons/AntiSpoof/data_io/functional.py
+-rw-r--r--   0 macbook    (501) staff       (20)    11464 2023-04-12 07:19:45.000000 app_ocr-0.0.3/app/face_id/commons/AntiSpoof/data_io/transform.py
+-rw-r--r--   0 macbook    (501) staff       (20)      802 2023-04-12 07:19:45.000000 app_ocr-0.0.3/app/face_id/commons/AntiSpoof/liveness_check.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1379 2023-06-20 08:00:29.000000 app_ocr-0.0.3/app/face_id/commons/AntiSpoof/liveness_onnx_check.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 08:01:36.195479 app_ocr-0.0.3/app/face_id/commons/AntiSpoof/model_lib/
+-rw-r--r--   0 macbook    (501) staff       (20)    12487 2023-04-12 07:19:45.000000 app_ocr-0.0.3/app/face_id/commons/AntiSpoof/model_lib/MiniFASNet.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2803 2023-04-12 07:19:45.000000 app_ocr-0.0.3/app/face_id/commons/AntiSpoof/model_lib/MultiFTNet.py
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 app_ocr-0.0.3/app/face_id/commons/AntiSpoof/model_lib/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)      990 2023-04-12 07:19:45.000000 app_ocr-0.0.3/app/face_id/commons/AntiSpoof/utility.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 08:01:36.195749 app_ocr-0.0.3/app/face_id/commons/ArcFace/
+-rw-r--r--   0 macbook    (501) staff       (20)     2981 2023-06-20 08:00:29.000000 app_ocr-0.0.3/app/face_id/commons/ArcFace/ArcFace_onnx.py
+-rw-r--r--   0 macbook    (501) staff       (20)      978 2023-04-12 07:19:45.000000 app_ocr-0.0.3/app/face_id/commons/ArcFace/__init__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 08:01:36.196391 app_ocr-0.0.3/app/face_id/commons/ArcFace/lib/
+-rw-r--r--   0 macbook    (501) staff       (20)      186 2023-04-12 07:19:45.000000 app_ocr-0.0.3/app/face_id/commons/ArcFace/lib/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     3036 2023-04-12 07:19:45.000000 app_ocr-0.0.3/app/face_id/commons/ArcFace/lib/layers.py
+-rw-r--r--   0 macbook    (501) staff       (20)     4284 2023-04-12 07:19:45.000000 app_ocr-0.0.3/app/face_id/commons/ArcFace/lib/models.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2436 2023-04-12 07:19:45.000000 app_ocr-0.0.3/app/face_id/commons/ArcFace/lib/utils.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 08:01:36.197262 app_ocr-0.0.3/app/face_id/commons/CloseEyes/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 app_ocr-0.0.3/app/face_id/commons/CloseEyes/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     3114 2023-06-20 07:27:46.000000 app_ocr-0.0.3/app/face_id/commons/CloseEyes/close_eyes.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1080 2023-06-20 08:00:29.000000 app_ocr-0.0.3/app/face_id/commons/CloseEyes/close_eyes_v2.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1310 2023-06-20 07:27:46.000000 app_ocr-0.0.3/app/face_id/commons/CloseEyes/utils.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 08:01:36.197594 app_ocr-0.0.3/app/face_id/commons/FaceMask/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 app_ocr-0.0.3/app/face_id/commons/FaceMask/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)      789 2023-06-20 08:00:29.000000 app_ocr-0.0.3/app/face_id/commons/FaceMask/face_mask_onnx.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 08:01:36.198006 app_ocr-0.0.3/app/face_id/commons/FaceQuality/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 app_ocr-0.0.3/app/face_id/commons/FaceQuality/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     9974 2023-06-01 06:55:11.000000 app_ocr-0.0.3/app/face_id/commons/FaceQuality/dom.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1854 2023-06-20 08:00:29.000000 app_ocr-0.0.3/app/face_id/commons/FaceQuality/face_quality_assessment.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 08:01:36.198263 app_ocr-0.0.3/app/face_id/commons/ScrFd/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:45.000000 app_ocr-0.0.3/app/face_id/commons/ScrFd/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)    12632 2023-06-01 06:55:11.000000 app_ocr-0.0.3/app/face_id/commons/ScrFd/scrfd.py
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 app_ocr-0.0.3/app/face_id/commons/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2297 2023-06-19 18:18:48.000000 app_ocr-0.0.3/app/face_id/commons/config.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 08:01:36.198762 app_ocr-0.0.3/app/face_id/libraries/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 app_ocr-0.0.3/app/face_id/libraries/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     7229 2023-06-20 08:00:29.000000 app_ocr-0.0.3/app/face_id/libraries/face_detection.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5305 2023-06-20 08:00:29.000000 app_ocr-0.0.3/app/face_id/libraries/face_id.py
+-rw-r--r--   0 macbook    (501) staff       (20)      395 2023-06-20 08:01:32.000000 app_ocr-0.0.3/app/face_id/libraries/face_recognition.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 08:01:36.199013 app_ocr-0.0.3/app/face_id/testing/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 07:28:07.000000 app_ocr-0.0.3/app/face_id/testing/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)      963 2023-06-20 07:27:46.000000 app_ocr-0.0.3/app/face_id/testing/scrfd_testing.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 08:01:36.199270 app_ocr-0.0.3/app/face_id/tools/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 app_ocr-0.0.3/app/face_id/tools/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     4040 2023-06-20 08:01:32.000000 app_ocr-0.0.3/app/face_id/tools/modules.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 08:01:36.199415 app_ocr-0.0.3/app/ocr/
+-rw-r--r--   0 macbook    (501) staff       (20)       19 2023-06-20 07:08:18.000000 app_ocr-0.0.3/app/ocr/__init__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 08:01:36.199541 app_ocr-0.0.3/app/ocr/core/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 07:27:46.000000 app_ocr-0.0.3/app/ocr/core/__init__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 08:01:36.200326 app_ocr-0.0.3/app/ocr/core/commons/
+-rw-r--r--   0 macbook    (501) staff       (20)      825 2023-06-19 13:32:54.000000 app_ocr-0.0.3/app/ocr/core/commons/SpoofingNID.py
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 app_ocr-0.0.3/app/ocr/core/commons/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5614 2023-06-19 17:59:34.000000 app_ocr-0.0.3/app/ocr/core/commons/config.py
+-rw-r--r--   0 macbook    (501) staff       (20)      780 2023-05-30 04:20:28.000000 app_ocr-0.0.3/app/ocr/core/commons/id_card_classification.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5687 2023-06-19 17:59:06.000000 app_ocr-0.0.3/app/ocr/core/commons/id_card_onnx.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1805 2023-06-01 06:55:11.000000 app_ocr-0.0.3/app/ocr/core/commons/merge_model.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 08:01:36.200589 app_ocr-0.0.3/app/ocr/core/commons/utils/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 07:28:07.000000 app_ocr-0.0.3/app/ocr/core/commons/utils/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2508 2023-05-30 04:20:28.000000 app_ocr-0.0.3/app/ocr/core/commons/utils/utils_onnx.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 08:01:36.200947 app_ocr-0.0.3/app/ocr/core/modules/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.3/app/ocr/core/modules/__init__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 08:01:36.201462 app_ocr-0.0.3/app/ocr/core/modules/corner_detection/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.3/app/ocr/core/modules/corner_detection/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2227 2023-06-15 03:28:33.000000 app_ocr-0.0.3/app/ocr/core/modules/corner_detection/id_card_aligment.py
+-rw-r--r--   0 macbook    (501) staff       (20)     3973 2023-06-19 14:29:56.000000 app_ocr-0.0.3/app/ocr/core/modules/corner_detection/utils.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 08:01:36.201791 app_ocr-0.0.3/app/ocr/core/modules/id_card_classification/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.3/app/ocr/core/modules/id_card_classification/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)      928 2023-06-15 07:52:38.000000 app_ocr-0.0.3/app/ocr/core/modules/id_card_classification/classify.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 08:01:36.202249 app_ocr-0.0.3/app/ocr/core/modules/mrc/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.3/app/ocr/core/modules/mrc/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2991 2023-06-15 07:52:38.000000 app_ocr-0.0.3/app/ocr/core/modules/mrc/mrc_detection.py
+-rw-r--r--   0 macbook    (501) staff       (20)      647 2023-04-12 07:19:46.000000 app_ocr-0.0.3/app/ocr/core/modules/mrc/utils.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 08:01:36.202858 app_ocr-0.0.3/app/ocr/core/modules/passport/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-18 03:26:14.000000 app_ocr-0.0.3/app/ocr/core/modules/passport/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     9115 2023-06-19 13:30:20.000000 app_ocr-0.0.3/app/ocr/core/modules/passport/passport.py
+-rw-r--r--   0 macbook    (501) staff       (20)      530 2023-06-19 13:30:20.000000 app_ocr-0.0.3/app/ocr/core/modules/passport/passport_detection.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2346 2023-06-15 07:52:38.000000 app_ocr-0.0.3/app/ocr/core/modules/passport/utils.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 08:01:36.203299 app_ocr-0.0.3/app/ocr/core/modules/passport/utils_align_passport/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-18 03:26:14.000000 app_ocr-0.0.3/app/ocr/core/modules/passport/utils_align_passport/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     3248 2023-04-18 08:29:08.000000 app_ocr-0.0.3/app/ocr/core/modules/passport/utils_align_passport/passport_utils.py
+-rw-r--r--   0 macbook    (501) staff       (20)     4344 2023-04-18 03:26:14.000000 app_ocr-0.0.3/app/ocr/core/modules/passport/utils_align_passport/utils_align.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 08:01:36.203585 app_ocr-0.0.3/app/ocr/core/modules/passport/utils_detect_passport/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-18 03:26:14.000000 app_ocr-0.0.3/app/ocr/core/modules/passport/utils_detect_passport/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     9663 2023-06-19 14:29:46.000000 app_ocr-0.0.3/app/ocr/core/modules/passport/utils_detect_passport/utils_detect.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 08:01:36.203871 app_ocr-0.0.3/app/ocr/core/modules/quality_liveness_nid_checking/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-26 09:38:30.000000 app_ocr-0.0.3/app/ocr/core/modules/quality_liveness_nid_checking/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2936 2023-06-01 06:55:11.000000 app_ocr-0.0.3/app/ocr/core/modules/quality_liveness_nid_checking/nid_quality_liveness_check.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 08:01:36.204175 app_ocr-0.0.3/app/ocr/core/modules/spell_checking/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.3/app/ocr/core/modules/spell_checking/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2350 2023-05-10 09:12:33.000000 app_ocr-0.0.3/app/ocr/core/modules/spell_checking/corrector_v2.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 08:01:36.204460 app_ocr-0.0.3/app/ocr/core/modules/spoofing_nid/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.3/app/ocr/core/modules/spoofing_nid/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)      940 2023-04-21 08:38:53.000000 app_ocr-0.0.3/app/ocr/core/modules/spoofing_nid/spoofing.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 08:01:36.204851 app_ocr-0.0.3/app/ocr/core/modules/text_detection/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.3/app/ocr/core/modules/text_detection/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     7125 2023-06-19 13:32:54.000000 app_ocr-0.0.3/app/ocr/core/modules/text_detection/dictionary.py
+-rw-r--r--   0 macbook    (501) staff       (20)    11597 2023-06-19 14:29:12.000000 app_ocr-0.0.3/app/ocr/core/modules/text_detection/utils.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 08:01:36.205150 app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2549 2023-05-30 04:20:28.000000 app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/nlp_onnx.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 08:01:36.205583 app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/__init__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 08:01:36.206222 app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/loader/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/loader/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1735 2023-04-12 07:19:46.000000 app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/loader/aug.py
+-rw-r--r--   0 macbook    (501) staff       (20)     6278 2023-04-12 07:19:46.000000 app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/loader/dataloader.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5021 2023-04-12 07:19:46.000000 app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/loader/dataloader_v1.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 08:01:36.207064 app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/model/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/model/__init__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 08:01:36.207653 app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)      888 2023-04-12 07:19:46.000000 app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/cnn.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5311 2023-04-12 07:19:46.000000 app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/resnet.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1655 2023-04-12 07:19:46.000000 app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/vgg.py
+-rw-r--r--   0 macbook    (501) staff       (20)     3777 2023-04-12 07:19:46.000000 app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/model/beam.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 08:01:36.208243 app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)    11634 2023-04-12 07:19:46.000000 app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/convseq2seq.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5731 2023-04-12 07:19:46.000000 app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/seq2seq.py
+-rw-r--r--   0 macbook    (501) staff       (20)     4858 2023-04-12 07:19:46.000000 app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/transformer.py
+-rw-r--r--   0 macbook    (501) staff       (20)    13524 2023-04-12 07:19:46.000000 app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/model/trainer.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1762 2023-04-12 07:19:46.000000 app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/model/transformerocr.py
+-rw-r--r--   0 macbook    (501) staff       (20)      924 2023-05-10 09:12:33.000000 app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/model/vocab.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 08:01:36.208680 app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/optim/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/optim/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1006 2023-04-12 07:19:46.000000 app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/optim/labelsmoothingloss.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1798 2023-04-12 07:19:46.000000 app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/optim/optim.py
+-rw-r--r--   0 macbook    (501) staff       (20)      538 2023-04-12 07:19:46.000000 app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/predict.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 08:01:36.208917 app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/tests/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/tests/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1039 2023-04-12 07:19:46.000000 app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/tests/utest.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 08:01:36.209785 app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/tool/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/tool/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1258 2023-04-12 07:19:46.000000 app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/tool/config.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2754 2023-04-12 07:19:46.000000 app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/tool/create_dataset.py
+-rw-r--r--   0 macbook    (501) staff       (20)      325 2023-04-12 07:19:46.000000 app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/tool/logger.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1427 2023-04-12 07:19:46.000000 app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/tool/predictor.py
+-rw-r--r--   0 macbook    (501) staff       (20)     7412 2023-06-01 06:55:11.000000 app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/tool/translate.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2688 2023-04-12 07:19:46.000000 app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/tool/utils.py
+-rw-r--r--   0 macbook    (501) staff       (20)      559 2023-04-12 07:19:46.000000 app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/train.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-20 08:01:36.210263 app_ocr-0.0.3/app/ocr/core/tools/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-20 06:30:22.000000 app_ocr-0.0.3/app/ocr/core/tools/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5552 2023-04-18 03:26:14.000000 app_ocr-0.0.3/app/ocr/core/tools/api_json.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5584 2023-06-01 06:55:11.000000 app_ocr-0.0.3/app/ocr/core/tools/dictionaries.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2542 2023-06-01 06:55:11.000000 app_ocr-0.0.3/app/ocr/core/tools/functional.py
+-rw-r--r--   0 macbook    (501) staff       (20)       38 2023-06-20 08:01:36.210642 app_ocr-0.0.3/setup.cfg
+-rw-r--r--   0 macbook    (501) staff       (20)      925 2023-06-20 08:01:32.000000 app_ocr-0.0.3/setup.py
```

### Comparing `app_ocr-0.0.2/PKG-INFO` & `app_ocr-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: app_ocr
-Version: 0.0.2
+Version: 0.0.3
 Summary: E-kyc for Industries application
 Home-page: https://github.com/aihackervn
 Author: Theodore
 Author-email: tinprocoder0908@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `app_ocr-0.0.2/README.md` & `app_ocr-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/app_ocr.egg-info/PKG-INFO` & `app_ocr-0.0.3/app/app_ocr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: app-ocr
-Version: 0.0.2
+Version: 0.0.3
 Summary: E-kyc for Industries application
 Home-page: https://github.com/aihackervn
 Author: Theodore
 Author-email: tinprocoder0908@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `app_ocr-0.0.2/app/app_ocr.egg-info/SOURCES.txt` & `app_ocr-0.0.3/app/app_ocr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/app_ocr.egg-info/requires.txt` & `app_ocr-0.0.3/app/app_ocr.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/config/config.py` & `app_ocr-0.0.3/app/config/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import yaml
 import cv2
 import io
 import numpy as np
 import base64
 from fastapi import HTTPException
-from app.config.logger import setup_logger
+from logger import setup_logger
 logging = setup_logger(__name__)
 
 
 RECOGNITION_INIT = 0.2
 
 
 def load_face_id_model():
```

### Comparing `app_ocr-0.0.2/app/config/logger.py` & `app_ocr-0.0.3/app/config/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 from functools import wraps
 import time
+
 loggers = {}
 
-def setup_logger(name, log_level=logging.ERROR, log_file=None):
 
+def setup_logger(name, log_level=logging.ERROR, log_file=None):
     global loggers
 
     if loggers.get(name):
         return loggers.get(name)
 
     else:
         logger = logging.getLogger(name)
@@ -22,18 +23,21 @@
         )
         console_handler.setFormatter(formatter)
 
         logger.addHandler(console_handler)
         loggers[name] = logger
         return logger
 
+
 def timeit(logging):
     def operate(func):
         @wraps(func)
         def wrapper(*args, **kwargs):
             start = time.perf_counter()
             result = func(*args, **kwargs)
             end = time.perf_counter()
             logging.info(f'{func.__name__} finished in {(end - start):.2f}s')
             return result
+
         return wrapper
-    return operate
+
+    return operate
```

### Comparing `app_ocr-0.0.2/app/config/pydantic_models.py` & `app_ocr-0.0.3/app/config/pydantic_models.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/database/crud.py` & `app_ocr-0.0.3/app/database/crud.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import uuid
 import base64
 from sqlalchemy import func
-from app.face_id.tools.modules import byte2array
+from ..face_id.tools.modules import byte2array
 from .database import engine, Base, Session
 from .data_models import FaceModel, ImageModel
 from functools import wraps
 
 
 class QueryData:
     def __init__(self) -> None:
```

### Comparing `app_ocr-0.0.2/app/database/data_models.py` & `app_ocr-0.0.3/app/database/data_models.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/database/database.py` & `app_ocr-0.0.3/app/database/database.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from sqlalchemy import create_engine
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.orm import sessionmaker
 from sqlalchemy.engine import URL
-from app.config.config_db import SettingLocal, SettingDev
+from ..config.config_db import SettingLocal, SettingDev
 
 setting = SettingDev()
 
 SQLALCHEMY_DATABASE_URL = URL.create(
     "postgresql",
     username=setting.USERNAME_,
     password=setting.PASSWORD,
```

### Comparing `app_ocr-0.0.2/app/face_id/commons/AntiSpoof/CDCN_config.py` & `app_ocr-0.0.3/app/face_id/commons/AntiSpoof/CDCN_config.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/face_id/commons/AntiSpoof/anti_spoof.py` & `app_ocr-0.0.3/app/face_id/commons/AntiSpoof/anti_spoof.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/face_id/commons/AntiSpoof/data_io/functional.py` & `app_ocr-0.0.3/app/face_id/commons/AntiSpoof/data_io/functional.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/face_id/commons/AntiSpoof/data_io/transform.py` & `app_ocr-0.0.3/app/face_id/commons/AntiSpoof/data_io/transform.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/face_id/commons/AntiSpoof/liveness_check.py` & `app_ocr-0.0.3/app/face_id/commons/AntiSpoof/liveness_check.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/face_id/commons/AntiSpoof/liveness_onnx_check.py` & `app_ocr-0.0.3/app/face_id/commons/AntiSpoof/liveness_onnx_check.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import onnxruntime as ort
 import cv2
-from app.face_id.commons.config import config
+from ..config import config
 
 model_path = config['face_liveness']
 
 
 def onnx_predict(img, model_paths=model_path):
     img = cv2.resize(img, (112, 112))
     dummy_face = np.expand_dims(np.array(img, dtype=np.float32), axis=0)
```

### Comparing `app_ocr-0.0.2/app/face_id/commons/AntiSpoof/model_lib/MiniFASNet.py` & `app_ocr-0.0.3/app/face_id/commons/AntiSpoof/model_lib/MiniFASNet.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/face_id/commons/AntiSpoof/model_lib/MultiFTNet.py` & `app_ocr-0.0.3/app/face_id/commons/AntiSpoof/model_lib/MultiFTNet.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/face_id/commons/AntiSpoof/utility.py` & `app_ocr-0.0.3/app/face_id/commons/AntiSpoof/utility.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/face_id/commons/ArcFace/ArcFace_onnx.py` & `app_ocr-0.0.3/app/face_id/commons/ArcFace/ArcFace_onnx.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import cv2
 import onnx
 import onnxruntime
-from app.face_id.commons.config import config
+from ..config import config
 __all__ = [
     'ArcFaceONNX',
 ]
 
 import warnings
 
 warnings.filterwarnings('ignore')
```

### Comparing `app_ocr-0.0.2/app/face_id/commons/ArcFace/__init__.py` & `app_ocr-0.0.3/app/face_id/commons/ArcFace/__init__.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/face_id/commons/ArcFace/lib/layers.py` & `app_ocr-0.0.3/app/face_id/commons/ArcFace/lib/layers.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/face_id/commons/ArcFace/lib/models.py` & `app_ocr-0.0.3/app/face_id/commons/ArcFace/lib/models.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/face_id/commons/ArcFace/lib/utils.py` & `app_ocr-0.0.3/app/face_id/commons/ArcFace/lib/utils.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/face_id/commons/CloseEyes/close_eyes.py` & `app_ocr-0.0.3/app/face_id/commons/CloseEyes/close_eyes.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/face_id/commons/CloseEyes/close_eyes_v2.py` & `app_ocr-0.0.3/app/face_id/commons/CloseEyes/close_eyes_v2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import cv2
 import onnxruntime
-from app.face_id.commons.CloseEyes.utils import extract_eye
-from app.face_id.commons.config import config
+from utils import extract_eye
+from ..config import config
 
 
 # 0: Close 1: Open
 
 def preprocessing(image):
     # img = image[:,:,::-1]
     img = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
```

### Comparing `app_ocr-0.0.2/app/face_id/commons/CloseEyes/utils.py` & `app_ocr-0.0.3/app/face_id/commons/CloseEyes/utils.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/face_id/commons/FaceMask/face_mask_onnx.py` & `app_ocr-0.0.3/app/face_id/commons/FaceMask/face_mask_onnx.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import onnxruntime
 import numpy as np
 import cv2
-from app.face_id.commons.config import config
+from ..config import config
 
 
 class FaceMask:
     def __init__(self, model_file=config['face_mask'], session=None):
         assert model_file is not None
         self.model_file = model_file
         self.session = session
```

### Comparing `app_ocr-0.0.2/app/face_id/commons/FaceQuality/dom.py` & `app_ocr-0.0.3/app/face_id/commons/FaceQuality/dom.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/face_id/commons/FaceQuality/face_quality_assessment.py` & `app_ocr-0.0.3/app/face_id/commons/FaceQuality/face_quality_assessment.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import cv2
 import numpy as np
 import math
-from app.face_id.commons.FaceQuality.dom import DOM
+from dom import DOM
 
 MIN_SHARPNESS = 0.46
 MIN_CONTRAST = 0.35
 MIN_BRIGHTNESS = 0.3
 MIN_BLUR = 100
```

### Comparing `app_ocr-0.0.2/app/face_id/commons/ScrFd/scrfd.py` & `app_ocr-0.0.3/app/face_id/commons/ScrFd/scrfd.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/face_id/commons/config.py` & `app_ocr-0.0.3/app/face_id/commons/config.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/face_id/libraries/face_detection.py` & `app_ocr-0.0.3/app/face_id/libraries/face_detection.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import numpy as np
-from app.face_id.commons.ScrFd.scrfd import SCRFD
-from app.face_id.commons.config import config
-from app.face_id.tools.modules import to_base64, alignment_procedure
-from app.face_id.commons.FaceMask.face_mask_onnx import FaceMask
-from app.face_id.commons.AntiSpoof.liveness_check import livenesss_predict
-from app.face_id.commons.AntiSpoof.liveness_onnx_check import onnx_predict
-from app.face_id.commons.CloseEyes.close_eyes_v2 import CloseEyes, crop_eye
-from app.face_id.commons.FaceQuality.face_quality_assessment import QualityCheck
-from app.face_id.commons.AntiSpoof.CDCN_config import predict_liveness
+from ..commons.ScrFd.scrfd import SCRFD
+from ..commons.config import config
+from ..tools.modules import to_base64, alignment_procedure
+from ..commons.FaceMask.face_mask_onnx import FaceMask
+from ..commons.AntiSpoof.liveness_check import livenesss_predict
+from ..commons.AntiSpoof.liveness_onnx_check import onnx_predict
+from ..commons.CloseEyes.close_eyes_v2 import CloseEyes, crop_eye
+from ..commons.FaceQuality.face_quality_assessment import QualityCheck
+from ..commons.AntiSpoof.CDCN_config import predict_liveness
 from fastapi import HTTPException
 import base64
-from app.config.logger import setup_logger, timeit
+from ...config.logger import setup_logger, timeit
 
 logging = setup_logger(__name__)
 detector = SCRFD(config['face_detection'])
 check_mask = FaceMask()
 eyes = CloseEyes()
 detector.prepare(0)
```

### Comparing `app_ocr-0.0.2/app/face_id/libraries/face_id.py` & `app_ocr-0.0.3/app/face_id/libraries/face_id.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from collections import defaultdict
 from typing import Tuple
-from app.face_id.tools.modules import *
-from app.face_id.commons.ArcFace.ArcFace_onnx import ArcFaceONNX
-from app.database.crud import QueryData
-from app.face_id.libraries.face_detection import get_face_location
-from app.face_id.libraries.face_recognition import calculate_embedding, get_feature
-from app.config.config import RECOGNITION_INIT
-from app.config.logger import setup_logger, timeit
+from ..tools.modules import *
+from ..commons.ArcFace.ArcFace_onnx import ArcFaceONNX
+from ...database.crud import QueryData
+from face_detection import get_face_location
+from face_recognition import calculate_embedding, get_feature
+from ...config.config import RECOGNITION_INIT
+from ...config.logger import setup_logger, timeit
 
 logging = setup_logger(__name__)
 db = QueryData()
 embedding = ArcFaceONNX()
 
 @timeit(logging)
 def detect_user(image: np.array) -> dict:
```

### Comparing `app_ocr-0.0.2/app/face_id/testing/scrfd_testing.py` & `app_ocr-0.0.3/app/face_id/testing/scrfd_testing.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/face_id/tools/modules.py` & `app_ocr-0.0.3/app/face_id/tools/modules.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from app.config.config import load_face_id_model
+from ...config.config import load_face_id_model
 from PIL import Image
 import cv2
 import math
 import base64
 import numpy as np
 import onnxruntime as ort
 from fastapi import HTTPException
-from app.config.logger import setup_logger, timeit
+from ...config.logger import setup_logger, timeit
 
 logging = setup_logger(__name__)
 retinaface, arcface = load_face_id_model()
 
 
 def image_bgr(image) -> np.array:
     img_BGR = cv2.imdecode(image, cv2.IMREAD_COLOR)
```

### Comparing `app_ocr-0.0.2/app/ocr/core/commons/SpoofingNID.py` & `app_ocr-0.0.3/app/ocr/core/commons/SpoofingNID.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/ocr/core/commons/config.py` & `app_ocr-0.0.3/app/ocr/core/commons/config.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/ocr/core/commons/id_card_classification.py` & `app_ocr-0.0.3/app/ocr/core/commons/id_card_classification.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/ocr/core/commons/id_card_onnx.py` & `app_ocr-0.0.3/app/ocr/core/commons/id_card_onnx.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/ocr/core/commons/merge_model.py` & `app_ocr-0.0.3/app/ocr/core/commons/merge_model.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/ocr/core/commons/utils/utils_onnx.py` & `app_ocr-0.0.3/app/ocr/core/commons/utils/utils_onnx.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/ocr/core/modules/corner_detection/id_card_aligment.py` & `app_ocr-0.0.3/app/ocr/core/modules/corner_detection/id_card_aligment.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/ocr/core/modules/corner_detection/utils.py` & `app_ocr-0.0.3/app/ocr/core/modules/corner_detection/utils.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/ocr/core/modules/id_card_classification/classify.py` & `app_ocr-0.0.3/app/ocr/core/modules/id_card_classification/classify.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/ocr/core/modules/mrc/mrc_detection.py` & `app_ocr-0.0.3/app/ocr/core/modules/mrc/mrc_detection.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/ocr/core/modules/mrc/utils.py` & `app_ocr-0.0.3/app/ocr/core/modules/mrc/utils.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/ocr/core/modules/passport/passport.py` & `app_ocr-0.0.3/app/ocr/core/modules/passport/passport.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/ocr/core/modules/passport/passport_detection.py` & `app_ocr-0.0.3/app/ocr/core/modules/passport/passport_detection.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/ocr/core/modules/passport/utils.py` & `app_ocr-0.0.3/app/ocr/core/modules/passport/utils.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/ocr/core/modules/passport/utils_align_passport/passport_utils.py` & `app_ocr-0.0.3/app/ocr/core/modules/passport/utils_align_passport/passport_utils.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/ocr/core/modules/passport/utils_align_passport/utils_align.py` & `app_ocr-0.0.3/app/ocr/core/modules/passport/utils_align_passport/utils_align.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/ocr/core/modules/passport/utils_detect_passport/utils_detect.py` & `app_ocr-0.0.3/app/ocr/core/modules/passport/utils_detect_passport/utils_detect.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/ocr/core/modules/quality_liveness_nid_checking/nid_quality_liveness_check.py` & `app_ocr-0.0.3/app/ocr/core/modules/quality_liveness_nid_checking/nid_quality_liveness_check.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/ocr/core/modules/spell_checking/corrector_v2.py` & `app_ocr-0.0.3/app/ocr/core/modules/spell_checking/corrector_v2.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/ocr/core/modules/spoofing_nid/spoofing.py` & `app_ocr-0.0.3/app/ocr/core/modules/spoofing_nid/spoofing.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/ocr/core/modules/text_detection/dictionary.py` & `app_ocr-0.0.3/app/ocr/core/modules/text_detection/dictionary.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/ocr/core/modules/text_detection/utils.py` & `app_ocr-0.0.3/app/ocr/core/modules/text_detection/utils.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/nlp_onnx.py` & `app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/nlp_onnx.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/loader/aug.py` & `app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/loader/aug.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/loader/dataloader.py` & `app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/loader/dataloader.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/loader/dataloader_v1.py` & `app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/loader/dataloader_v1.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/cnn.py` & `app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/cnn.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/resnet.py` & `app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/resnet.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/vgg.py` & `app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/model/backbone/vgg.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/model/beam.py` & `app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/model/beam.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/convseq2seq.py` & `app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/convseq2seq.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/seq2seq.py` & `app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/seq2seq.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/transformer.py` & `app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/model/seqmodel/transformer.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/model/trainer.py` & `app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/model/trainer.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/model/transformerocr.py` & `app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/model/transformerocr.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/model/vocab.py` & `app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/model/vocab.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/optim/labelsmoothingloss.py` & `app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/optim/labelsmoothingloss.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/optim/optim.py` & `app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/optim/optim.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/predict.py` & `app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/predict.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/tests/utest.py` & `app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/tests/utest.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/tool/config.py` & `app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/tool/config.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/tool/create_dataset.py` & `app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/tool/create_dataset.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/tool/predictor.py` & `app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/tool/predictor.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/tool/translate.py` & `app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/tool/translate.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/tool/utils.py` & `app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/tool/utils.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/ocr/core/modules/vietnamese_nlp/vietocr/train.py` & `app_ocr-0.0.3/app/ocr/core/modules/vietnamese_nlp/vietocr/train.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/ocr/core/tools/api_json.py` & `app_ocr-0.0.3/app/ocr/core/tools/api_json.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/ocr/core/tools/dictionaries.py` & `app_ocr-0.0.3/app/ocr/core/tools/dictionaries.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/app/ocr/core/tools/functional.py` & `app_ocr-0.0.3/app/ocr/core/tools/functional.py`

 * *Files identical despite different names*

### Comparing `app_ocr-0.0.2/setup.py` & `app_ocr-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 with open("README.md", "r") as f:
     long_description = f.read()
 with open("requirements.txt", "r") as f:
     install_requires = [line.strip() for line in f if line.strip()]
 setup(
     name="app_ocr",
-    version="0.0.2",
+    version="0.0.3",
     description="E-kyc for Industries application",
     package_dir={"": "app"},
     packages=find_packages(where="./app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aihackervn",
     author="Theodore",
```

