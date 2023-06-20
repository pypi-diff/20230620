# Comparing `tmp/bluecast-0.1.tar.gz` & `tmp/bluecast-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluecast-0.1.tar", max compression
+gzip compressed data, was "bluecast-0.2.tar", max compression
```

## Comparing `bluecast-0.1.tar` & `bluecast-0.2.tar`

### file list

```diff
@@ -1,81 +1,81 @@
--rw-r--r--   0        0        0     1076 2023-06-09 18:08:15.669820 bluecast-0.1/LICENSE
--rw-r--r--   0        0        0    11163 2023-06-09 18:08:15.670297 bluecast-0.1/README.md
--rw-r--r--   0        0        0        0 2023-06-07 04:56:12.514815 bluecast-0.1/bluecast/__init__.py
--rw-r--r--   0        0        0        0 2023-06-07 04:56:12.515058 bluecast-0.1/bluecast/blueprints/__init__.py
--rw-r--r--   0        0        0      168 2023-06-07 04:56:37.021684 bluecast-0.1/bluecast/blueprints/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     7764 2023-06-08 18:49:56.097612 bluecast-0.1/bluecast/blueprints/__pycache__/cast.cpython-310.pyc
--rw-r--r--   0        0        0    10432 2023-06-09 18:08:15.670743 bluecast-0.1/bluecast/blueprints/cast.py
--rw-r--r--   0        0        0        0 2023-06-07 04:56:12.515460 bluecast-0.1/bluecast/config/__init__.py
--rw-r--r--   0        0        0      164 2023-06-07 04:56:37.023862 bluecast-0.1/bluecast/config/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3462 2023-06-08 18:49:56.099991 bluecast-0.1/bluecast/config/__pycache__/training_config.cpython-310.pyc
--rw-r--r--   0        0        0     2726 2023-06-07 20:39:31.707082 bluecast-0.1/bluecast/config/training_config.py
--rw-r--r--   0        0        0        0 2023-06-07 04:56:12.515862 bluecast-0.1/bluecast/evaluation/__init__.py
--rw-r--r--   0        0        0      168 2023-06-07 04:56:37.055926 bluecast-0.1/bluecast/evaluation/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1598 2023-06-08 18:49:56.584677 bluecast-0.1/bluecast/evaluation/__pycache__/eval_metrics.cpython-310.pyc
--rw-r--r--   0        0        0     1418 2023-06-08 18:50:02.325344 bluecast-0.1/bluecast/evaluation/__pycache__/shap_values.cpython-310.pyc
--rw-r--r--   0        0        0     1979 2023-06-07 20:39:31.701364 bluecast-0.1/bluecast/evaluation/eval_metrics.py
--rw-r--r--   0        0        0     1389 2023-06-09 18:08:15.671080 bluecast-0.1/bluecast/evaluation/shap_values.py
--rw-r--r--   0        0        0        0 2023-06-07 20:14:40.570845 bluecast-0.1/bluecast/general_utils/__init__.py
--rw-r--r--   0        0        0      171 2023-06-08 18:50:02.038695 bluecast-0.1/bluecast/general_utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2440 2023-06-08 18:50:02.041457 bluecast-0.1/bluecast/general_utils/__pycache__/general_utils.cpython-310.pyc
--rw-r--r--   0        0        0     2248 2023-06-07 20:39:31.698812 bluecast-0.1/bluecast/general_utils/general_utils.py
--rw-r--r--   0        0        0        0 2023-06-07 04:56:12.516548 bluecast-0.1/bluecast/ml_modelling/__init__.py
--rw-r--r--   0        0        0      170 2023-06-07 04:56:37.978742 bluecast-0.1/bluecast/ml_modelling/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1440 2023-06-08 18:50:12.014936 bluecast-0.1/bluecast/ml_modelling/__pycache__/base_classes.cpython-310.pyc
--rw-r--r--   0        0        0     8492 2023-06-08 18:50:09.692583 bluecast-0.1/bluecast/ml_modelling/__pycache__/xgboost.cpython-310.pyc
--rw-r--r--   0        0        0      982 2023-06-07 20:39:31.678131 bluecast-0.1/bluecast/ml_modelling/base_classes.py
--rw-r--r--   0        0        0    12506 2023-06-08 18:43:33.722773 bluecast-0.1/bluecast/ml_modelling/xgboost.py
--rw-r--r--   0        0        0        0 2023-06-07 04:56:12.517425 bluecast-0.1/bluecast/preprocessing/__init__.py
--rw-r--r--   0        0        0      171 2023-06-07 04:56:37.505605 bluecast-0.1/bluecast/preprocessing/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1428 2023-06-08 18:50:12.016504 bluecast-0.1/bluecast/preprocessing/__pycache__/custom.cpython-310.pyc
--rw-r--r--   0        0        0     1543 2023-06-08 18:50:12.017272 bluecast-0.1/bluecast/preprocessing/__pycache__/datetime_features.cpython-310.pyc
--rw-r--r--   0        0        0     3675 2023-06-08 18:50:12.018392 bluecast-0.1/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-310.pyc
--rw-r--r--   0        0        0     4584 2023-06-08 18:50:12.019409 bluecast-0.1/bluecast/preprocessing/__pycache__/feature_types.cpython-310.pyc
--rw-r--r--   0        0        0     6527 2023-06-07 04:56:37.506887 bluecast-0.1/bluecast/preprocessing/__pycache__/general_utils.cpython-310.pyc
--rw-r--r--   0        0        0     1176 2023-06-08 18:50:12.020042 bluecast-0.1/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-310.pyc
--rw-r--r--   0        0        0     1957 2023-06-08 18:50:12.020557 bluecast-0.1/bluecast/preprocessing/__pycache__/schema_checks.cpython-310.pyc
--rw-r--r--   0        0        0     4940 2023-06-08 18:50:12.021396 bluecast-0.1/bluecast/preprocessing/__pycache__/target_encoding.cpython-310.pyc
--rw-r--r--   0        0        0     1823 2023-06-08 18:50:12.961492 bluecast-0.1/bluecast/preprocessing/__pycache__/train_test_split.cpython-310.pyc
--rw-r--r--   0        0        0      961 2023-06-08 18:43:33.722893 bluecast-0.1/bluecast/preprocessing/custom.py
--rw-r--r--   0        0        0     1424 2023-06-07 20:39:31.712452 bluecast-0.1/bluecast/preprocessing/datetime_features.py
--rw-r--r--   0        0        0     3122 2023-06-07 20:39:31.689572 bluecast-0.1/bluecast/preprocessing/encode_target_labels.py
--rw-r--r--   0        0        0     6054 2023-06-07 20:39:31.704291 bluecast-0.1/bluecast/preprocessing/feature_types.py
--rw-r--r--   0        0        0      862 2023-06-07 20:39:31.683729 bluecast-0.1/bluecast/preprocessing/nulls_and_infs.py
--rw-r--r--   0        0        0     1452 2023-06-08 18:43:33.723008 bluecast-0.1/bluecast/preprocessing/schema_checks.py
--rw-r--r--   0        0        0     4561 2023-06-07 20:39:31.709912 bluecast-0.1/bluecast/preprocessing/target_encoding.py
--rw-r--r--   0        0        0     1748 2023-06-07 20:39:31.680865 bluecast-0.1/bluecast/preprocessing/train_test_split.py
--rw-r--r--   0        0        0        0 2023-06-07 04:56:12.518803 bluecast-0.1/bluecast/tests/__init__.py
--rw-r--r--   0        0        0      163 2023-06-07 04:56:36.657919 bluecast-0.1/bluecast/tests/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3729 2023-06-08 18:49:52.784669 bluecast-0.1/bluecast/tests/__pycache__/test_cast.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     3165 2023-06-08 18:50:12.966095 bluecast-0.1/bluecast/tests/__pycache__/test_check_gpu_support.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     1146 2023-06-07 04:56:38.295009 bluecast-0.1/bluecast/tests/__pycache__/test_datetime_features.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     2401 2023-06-07 04:56:38.296223 bluecast-0.1/bluecast/tests/__pycache__/test_encode_target_labels.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     4812 2023-06-08 18:50:12.971333 bluecast-0.1/bluecast/tests/__pycache__/test_feature_type_detector.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     1702 2023-06-08 18:50:12.972854 bluecast-0.1/bluecast/tests/__pycache__/test_load_for_production.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     4598 2023-06-07 04:56:38.302111 bluecast-0.1/bluecast/tests/__pycache__/test_nulls_and_infs.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     2057 2023-06-08 18:50:12.974781 bluecast-0.1/bluecast/tests/__pycache__/test_save_to_production.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     2108 2023-06-08 18:50:12.976223 bluecast-0.1/bluecast/tests/__pycache__/test_schema_checks.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     1528 2023-06-07 04:56:38.303245 bluecast-0.1/bluecast/tests/__pycache__/test_shap_explanations.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     1886 2023-06-07 04:56:38.304347 bluecast-0.1/bluecast/tests/__pycache__/test_target_encoding_binary.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     1458 2023-06-07 04:56:38.305381 bluecast-0.1/bluecast/tests/__pycache__/test_target_encoding_multiclass.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     2157 2023-06-07 04:56:38.307410 bluecast-0.1/bluecast/tests/__pycache__/test_train_test_split.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0        0 2023-06-07 04:56:12.519076 bluecast-0.1/bluecast/tests/make_data/__init__.py
--rw-r--r--   0        0        0      173 2023-06-07 04:56:38.291659 bluecast-0.1/bluecast/tests/make_data/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1132 2023-06-07 04:56:38.292287 bluecast-0.1/bluecast/tests/make_data/__pycache__/create_data.cpython-310.pyc
--rw-r--r--   0        0        0     1289 2023-06-07 04:56:12.519593 bluecast-0.1/bluecast/tests/make_data/create_data.py
--rw-r--r--   0        0        0     4286 2023-06-09 18:08:15.671327 bluecast-0.1/bluecast/tests/test_cast.py
--rw-r--r--   0        0        0     1328 2023-06-07 20:14:40.740928 bluecast-0.1/bluecast/tests/test_check_gpu_support.py
--rw-r--r--   0        0        0     1789 2023-06-09 18:08:15.671451 bluecast-0.1/bluecast/tests/test_custom_processing_base_class.py
--rw-r--r--   0        0        0     1097 2023-06-07 04:56:12.520160 bluecast-0.1/bluecast/tests/test_datetime_features.py
--rw-r--r--   0        0        0     1996 2023-06-07 04:56:12.520372 bluecast-0.1/bluecast/tests/test_encode_target_labels.py
--rw-r--r--   0        0        0     2608 2023-06-07 20:14:40.770936 bluecast-0.1/bluecast/tests/test_feature_type_detector.py
--rw-r--r--   0        0        0     1482 2023-06-08 19:05:45.011986 bluecast-0.1/bluecast/tests/test_load_for_production.py
--rw-r--r--   0        0        0     1575 2023-06-07 04:56:12.521016 bluecast-0.1/bluecast/tests/test_nulls_and_infs.py
--rw-r--r--   0        0        0     1020 2023-06-08 19:13:52.772067 bluecast-0.1/bluecast/tests/test_save_to_production.py
--rw-r--r--   0        0        0     2080 2023-06-08 18:43:33.723332 bluecast-0.1/bluecast/tests/test_schema_checks.py
--rw-r--r--   0        0        0     2204 2023-06-09 18:08:15.671913 bluecast-0.1/bluecast/tests/test_shap_explanations.py
--rw-r--r--   0        0        0     1337 2023-06-07 04:56:12.521411 bluecast-0.1/bluecast/tests/test_target_encoding_binary.py
--rw-r--r--   0        0        0      735 2023-06-07 04:56:12.521599 bluecast-0.1/bluecast/tests/test_target_encoding_multiclass.py
--rw-r--r--   0        0        0     1051 2023-06-07 04:56:12.521767 bluecast-0.1/bluecast/tests/test_train_test_split.py
--rw-r--r--   0        0        0     1455 2023-06-09 18:08:15.673787 bluecast-0.1/pyproject.toml
--rw-r--r--   0        0        0    12293 1970-01-01 00:00:00.000000 bluecast-0.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-09 18:08:15.669820 bluecast-0.2/LICENSE
+-rw-r--r--   0        0        0    14338 2023-06-20 20:04:49.529175 bluecast-0.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-07 04:56:12.514815 bluecast-0.2/bluecast/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-07 04:56:12.515058 bluecast-0.2/bluecast/blueprints/__init__.py
+-rw-r--r--   0        0        0      168 2023-06-07 04:56:37.021684 bluecast-0.2/bluecast/blueprints/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     7764 2023-06-08 18:49:56.097612 bluecast-0.2/bluecast/blueprints/__pycache__/cast.cpython-310.pyc
+-rw-r--r--   0        0        0    12209 2023-06-20 20:04:49.529837 bluecast-0.2/bluecast/blueprints/cast.py
+-rw-r--r--   0        0        0        0 2023-06-07 04:56:12.515460 bluecast-0.2/bluecast/config/__init__.py
+-rw-r--r--   0        0        0      164 2023-06-07 04:56:37.023862 bluecast-0.2/bluecast/config/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3462 2023-06-08 18:49:56.099991 bluecast-0.2/bluecast/config/__pycache__/training_config.cpython-310.pyc
+-rw-r--r--   0        0        0     2792 2023-06-15 02:48:46.492822 bluecast-0.2/bluecast/config/training_config.py
+-rw-r--r--   0        0        0        0 2023-06-07 04:56:12.515862 bluecast-0.2/bluecast/evaluation/__init__.py
+-rw-r--r--   0        0        0      168 2023-06-07 04:56:37.055926 bluecast-0.2/bluecast/evaluation/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1598 2023-06-08 18:49:56.584677 bluecast-0.2/bluecast/evaluation/__pycache__/eval_metrics.cpython-310.pyc
+-rw-r--r--   0        0        0     1418 2023-06-08 18:50:02.325344 bluecast-0.2/bluecast/evaluation/__pycache__/shap_values.cpython-310.pyc
+-rw-r--r--   0        0        0     1979 2023-06-07 20:39:31.701364 bluecast-0.2/bluecast/evaluation/eval_metrics.py
+-rw-r--r--   0        0        0     1389 2023-06-09 18:08:15.671080 bluecast-0.2/bluecast/evaluation/shap_values.py
+-rw-r--r--   0        0        0        0 2023-06-07 20:14:40.570845 bluecast-0.2/bluecast/general_utils/__init__.py
+-rw-r--r--   0        0        0      171 2023-06-08 18:50:02.038695 bluecast-0.2/bluecast/general_utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2440 2023-06-08 18:50:02.041457 bluecast-0.2/bluecast/general_utils/__pycache__/general_utils.cpython-310.pyc
+-rw-r--r--   0        0        0     2248 2023-06-07 20:39:31.698812 bluecast-0.2/bluecast/general_utils/general_utils.py
+-rw-r--r--   0        0        0        0 2023-06-07 04:56:12.516548 bluecast-0.2/bluecast/ml_modelling/__init__.py
+-rw-r--r--   0        0        0      170 2023-06-07 04:56:37.978742 bluecast-0.2/bluecast/ml_modelling/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1440 2023-06-08 18:50:12.014936 bluecast-0.2/bluecast/ml_modelling/__pycache__/base_classes.cpython-310.pyc
+-rw-r--r--   0        0        0     8492 2023-06-08 18:50:09.692583 bluecast-0.2/bluecast/ml_modelling/__pycache__/xgboost.cpython-310.pyc
+-rw-r--r--   0        0        0      982 2023-06-07 20:39:31.678131 bluecast-0.2/bluecast/ml_modelling/base_classes.py
+-rw-r--r--   0        0        0    12506 2023-06-08 18:43:33.722773 bluecast-0.2/bluecast/ml_modelling/xgboost.py
+-rw-r--r--   0        0        0        0 2023-06-07 04:56:12.517425 bluecast-0.2/bluecast/preprocessing/__init__.py
+-rw-r--r--   0        0        0      171 2023-06-07 04:56:37.505605 bluecast-0.2/bluecast/preprocessing/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1428 2023-06-08 18:50:12.016504 bluecast-0.2/bluecast/preprocessing/__pycache__/custom.cpython-310.pyc
+-rw-r--r--   0        0        0     1543 2023-06-08 18:50:12.017272 bluecast-0.2/bluecast/preprocessing/__pycache__/datetime_features.cpython-310.pyc
+-rw-r--r--   0        0        0     3675 2023-06-08 18:50:12.018392 bluecast-0.2/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-310.pyc
+-rw-r--r--   0        0        0     4584 2023-06-08 18:50:12.019409 bluecast-0.2/bluecast/preprocessing/__pycache__/feature_types.cpython-310.pyc
+-rw-r--r--   0        0        0     6527 2023-06-07 04:56:37.506887 bluecast-0.2/bluecast/preprocessing/__pycache__/general_utils.cpython-310.pyc
+-rw-r--r--   0        0        0     1176 2023-06-08 18:50:12.020042 bluecast-0.2/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-310.pyc
+-rw-r--r--   0        0        0     1957 2023-06-08 18:50:12.020557 bluecast-0.2/bluecast/preprocessing/__pycache__/schema_checks.cpython-310.pyc
+-rw-r--r--   0        0        0     4940 2023-06-08 18:50:12.021396 bluecast-0.2/bluecast/preprocessing/__pycache__/target_encoding.cpython-310.pyc
+-rw-r--r--   0        0        0     1823 2023-06-08 18:50:12.961492 bluecast-0.2/bluecast/preprocessing/__pycache__/train_test_split.cpython-310.pyc
+-rw-r--r--   0        0        0     1402 2023-06-20 20:04:49.530190 bluecast-0.2/bluecast/preprocessing/custom.py
+-rw-r--r--   0        0        0     1424 2023-06-07 20:39:31.712452 bluecast-0.2/bluecast/preprocessing/datetime_features.py
+-rw-r--r--   0        0        0     3122 2023-06-07 20:39:31.689572 bluecast-0.2/bluecast/preprocessing/encode_target_labels.py
+-rw-r--r--   0        0        0     6190 2023-06-20 20:04:49.530725 bluecast-0.2/bluecast/preprocessing/feature_types.py
+-rw-r--r--   0        0        0      862 2023-06-07 20:39:31.683729 bluecast-0.2/bluecast/preprocessing/nulls_and_infs.py
+-rw-r--r--   0        0        0     1452 2023-06-08 18:43:33.723008 bluecast-0.2/bluecast/preprocessing/schema_checks.py
+-rw-r--r--   0        0        0     4561 2023-06-07 20:39:31.709912 bluecast-0.2/bluecast/preprocessing/target_encoding.py
+-rw-r--r--   0        0        0     2871 2023-06-20 20:04:49.531175 bluecast-0.2/bluecast/preprocessing/train_test_split.py
+-rw-r--r--   0        0        0        0 2023-06-07 04:56:12.518803 bluecast-0.2/bluecast/tests/__init__.py
+-rw-r--r--   0        0        0      163 2023-06-07 04:56:36.657919 bluecast-0.2/bluecast/tests/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3729 2023-06-08 18:49:52.784669 bluecast-0.2/bluecast/tests/__pycache__/test_cast.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     3165 2023-06-08 18:50:12.966095 bluecast-0.2/bluecast/tests/__pycache__/test_check_gpu_support.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     1146 2023-06-07 04:56:38.295009 bluecast-0.2/bluecast/tests/__pycache__/test_datetime_features.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     2401 2023-06-07 04:56:38.296223 bluecast-0.2/bluecast/tests/__pycache__/test_encode_target_labels.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     4812 2023-06-08 18:50:12.971333 bluecast-0.2/bluecast/tests/__pycache__/test_feature_type_detector.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     1702 2023-06-08 18:50:12.972854 bluecast-0.2/bluecast/tests/__pycache__/test_load_for_production.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     4598 2023-06-07 04:56:38.302111 bluecast-0.2/bluecast/tests/__pycache__/test_nulls_and_infs.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     2057 2023-06-08 18:50:12.974781 bluecast-0.2/bluecast/tests/__pycache__/test_save_to_production.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     2108 2023-06-08 18:50:12.976223 bluecast-0.2/bluecast/tests/__pycache__/test_schema_checks.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     1528 2023-06-07 04:56:38.303245 bluecast-0.2/bluecast/tests/__pycache__/test_shap_explanations.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     1886 2023-06-07 04:56:38.304347 bluecast-0.2/bluecast/tests/__pycache__/test_target_encoding_binary.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     1458 2023-06-07 04:56:38.305381 bluecast-0.2/bluecast/tests/__pycache__/test_target_encoding_multiclass.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     2157 2023-06-07 04:56:38.307410 bluecast-0.2/bluecast/tests/__pycache__/test_train_test_split.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0        0 2023-06-07 04:56:12.519076 bluecast-0.2/bluecast/tests/make_data/__init__.py
+-rw-r--r--   0        0        0      173 2023-06-07 04:56:38.291659 bluecast-0.2/bluecast/tests/make_data/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1132 2023-06-07 04:56:38.292287 bluecast-0.2/bluecast/tests/make_data/__pycache__/create_data.cpython-310.pyc
+-rw-r--r--   0        0        0     1289 2023-06-07 04:56:12.519593 bluecast-0.2/bluecast/tests/make_data/create_data.py
+-rw-r--r--   0        0        0     4333 2023-06-20 04:25:58.592640 bluecast-0.2/bluecast/tests/test_cast.py
+-rw-r--r--   0        0        0     1328 2023-06-07 20:14:40.740928 bluecast-0.2/bluecast/tests/test_check_gpu_support.py
+-rw-r--r--   0        0        0     1789 2023-06-09 18:08:15.671451 bluecast-0.2/bluecast/tests/test_custom_processing_base_class.py
+-rw-r--r--   0        0        0     1097 2023-06-07 04:56:12.520160 bluecast-0.2/bluecast/tests/test_datetime_features.py
+-rw-r--r--   0        0        0     1996 2023-06-07 04:56:12.520372 bluecast-0.2/bluecast/tests/test_encode_target_labels.py
+-rw-r--r--   0        0        0     2608 2023-06-07 20:14:40.770936 bluecast-0.2/bluecast/tests/test_feature_type_detector.py
+-rw-r--r--   0        0        0     1482 2023-06-08 19:05:45.011986 bluecast-0.2/bluecast/tests/test_load_for_production.py
+-rw-r--r--   0        0        0     1575 2023-06-07 04:56:12.521016 bluecast-0.2/bluecast/tests/test_nulls_and_infs.py
+-rw-r--r--   0        0        0     1020 2023-06-08 19:13:52.772067 bluecast-0.2/bluecast/tests/test_save_to_production.py
+-rw-r--r--   0        0        0     2080 2023-06-08 18:43:33.723332 bluecast-0.2/bluecast/tests/test_schema_checks.py
+-rw-r--r--   0        0        0     2204 2023-06-09 18:08:15.671913 bluecast-0.2/bluecast/tests/test_shap_explanations.py
+-rw-r--r--   0        0        0     1337 2023-06-07 04:56:12.521411 bluecast-0.2/bluecast/tests/test_target_encoding_binary.py
+-rw-r--r--   0        0        0      735 2023-06-07 04:56:12.521599 bluecast-0.2/bluecast/tests/test_target_encoding_multiclass.py
+-rw-r--r--   0        0        0     1051 2023-06-07 04:56:12.521767 bluecast-0.2/bluecast/tests/test_train_test_split.py
+-rw-r--r--   0        0        0     1457 2023-06-15 02:48:46.497087 bluecast-0.2/pyproject.toml
+-rw-r--r--   0        0        0    15454 1970-01-01 00:00:00.000000 bluecast-0.2/PKG-INFO
```

### Comparing `bluecast-0.1/LICENSE` & `bluecast-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/README.md` & `bluecast-0.2/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 [![codecov](https://codecov.io/gh/ThomasMeissnerDS/BlueCast/branch/main/graph/badge.svg?token=XRIS04O097)](https://codecov.io/gh/ThomasMeissnerDS/BlueCast)
 [![Codecov workflow](https://github.com/ThomasMeissnerDS/BlueCast/actions/workflows/workflow.yaml/badge.svg)](https://github.com/ThomasMeissnerDS/BlueCast/actions/workflows/workflow.yaml)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![pydocstyle](https://img.shields.io/badge/pydocstyle-enabled-AD4CD3)](http://www.pydocstyle.org/en/stable/)
 [![Documentation Status](https://readthedocs.org/projects/bluecast/badge/?version=latest)](https://bluecast.readthedocs.io/en/latest/?badge=latest)
+[![PyPI version](https://badge.fury.io/py/bluecast.svg)](https://pypi.python.org/pypi/bluecast/)
+![Known Vulnerabilities](https://snyk.io/test/github/ThomasMeissnerDS/BlueCast/main/badge.svg)
+[![Optuna](https://img.shields.io/badge/Optuna-integrated-blue)](https://optuna.org)
 [![python](https://img.shields.io/badge/Python-3.9-3776AB.svg?style=flat&logo=python&logoColor=white)](https://www.python.org)
 [![python](https://img.shields.io/badge/Python-3.10-3776AB.svg?style=flat&logo=python&logoColor=white)](https://www.python.org)
 [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com)
 
 A lightweight and fast auto-ml library. This is the successor of the
 e2eml automl library. While e2eml tried to cover many model
 architectures and a lot of different preprocessing options,
@@ -26,15 +29,15 @@
   * [Installation for end users](#installation-for-end-users)
   * [Installation for developers](#installation-for-developers)
 * [General usage](#general-usage)
   * [Basic usage](#basic-usage)
   * [Advanced usage](#advanced-usage)
     * [Custom training configuration](#custom--training-configuration)
     * [Custom preprocessing](#custom-preprocessing)
-* [Custom ML model](#custom-ml-model)
+    * [Custom ML model](#custom-ml-model)
 * [Convenience features](#convenience-features)
 * [Code quality](#code-quality)
 * [Documentation](#documentation)
 * [How to contribute](#how-to-contribute)
 * [Meta](#meta)
 
 <!-- tocstop -->
@@ -115,17 +118,19 @@
 y_probs, y_classes = automl.predict(df_val)
 ```
 
 #### Custom preprocessing
 
 The `BlueCast` class also allows for custom preprocessing. This is done by
 an abstract class that can be inherited and passed into the `BlueCast` class.
-The custom preprocessing will be called before the model training or prediction
-starts and allows users to execute last computations (i.e. sub sampling
-or final calculations).
+BlueCast provides two entry points to inject custom preprocessing. The
+attribute `custom_preprocessor` is called right after the train_test_split.
+The attribute `custom_last_mile_computation` will be called before the model
+training or prediction starts (when only numerical features are present anymore)
+and allows users to execute last computations (i.e. sub sampling or final calculations).
 
 ```sh
 from bluecast.blueprints.cast import BlueCast
 from bluecast.preprocessing.custom import CustomPreprocessing
 
 # Create a custom tuning config and adjust hyperparameter search space
 xgboost_param_config = XgboostTuneParamsConfig()
@@ -133,57 +138,110 @@
 xgboost_param_config.num_leaves_max = 16
 # Create a custom training config and adjust general training parameters
 train_config = TrainingConfig()
 train_config.hyperparameter_tuning_rounds = 10
 train_config.autotune_model = False # we want to run just normal training, no hyperparameter tuning
 # We could even just overwrite the final Xgboost params using the XgboostFinalParamConfig class
 
-# add custom last mile computation
 class MyCustomPreprocessing(CustomPreprocessing):
+    def __init__(self):
+        self.trained_patterns = {}
+
+    def fit_transform(
+        self, df: pd.DataFrame, target: pd.Series
+    ) -> Tuple[pd.DataFrame, pd.Series]:
+        num_columns = df.drop(['Beta', 'Gamma', 'Delta', 'Alpha', 'EJ'], axis=1).columns
+        cat_df = df[['Beta', 'Gamma', 'Delta', 'Alpha', 'EJ']].copy()
+
+        zscores = Zscores()
+        zscores.fit_all(df, ['Beta', 'Gamma', 'Delta', 'Alpha', 'EJ'])
+        df = zscores.transform_all(df, ['Beta', 'Gamma', 'Delta', 'Alpha', 'EJ'])
+        self.trained_patterns["zscores"] = zscores
+
+        imp_mean = SimpleImputer(missing_values=np.nan, strategy='median')
+        num_columns = df.drop(['Beta', 'Gamma', 'Delta', 'Alpha', 'EJ'], axis=1).columns
+        imp_mean.fit(df.loc[:, num_columns])
+        df = imp_mean.transform(df.loc[:, num_columns])
+        self.trained_patterns["imputation"] = imp_mean
+
+        df = pd.DataFrame(df, columns=num_columns).merge(cat_df, left_index=True, right_index=True, how="left")
+
+        df = df.drop(['Beta', 'Gamma', 'Delta', 'Alpha'], axis=1)
+
+        return df, target
+
+    def transform(
+        self,
+        df: pd.DataFrame,
+        target: Optional[pd.Series] = None,
+        predicton_mode: bool = False,
+    ) -> Tuple[pd.DataFrame, Optional[pd.Series]]:
+        num_columns = df.drop(['Beta', 'Gamma', 'Delta', 'Alpha', 'EJ'], axis=1).columns
+        cat_df = df[['Beta', 'Gamma', 'Delta', 'Alpha', 'EJ']].copy()
+
+        df = self.trained_patterns["zscores"].transform_all(df, ['Beta', 'Gamma', 'Delta', 'Alpha', 'EJ'])
+
+        imp_mean = self.trained_patterns["imputation"]
+        num_columns = df.drop(['Beta', 'Gamma', 'Delta', 'Alpha', 'EJ'], axis=1).columns
+        df.loc[:, num_columns] = df.loc[:, num_columns].replace([np.inf, -np.inf], np.nan)
+        df = imp_mean.transform(df.loc[:, num_columns])
+
+        df = pd.DataFrame(df, columns=num_columns).merge(cat_df, left_index=True, right_index=True, how="left")
+
+        df = df.drop(['Beta', 'Gamma', 'Delta', 'Alpha'], axis=1)
+
+        return df, target
+
+# add custom last mile computation
+class MyCustomLastMilePreprocessing(CustomPreprocessing):
     def custom_function(self, df: pd.DataFrame) -> pd.DataFrame:
         df = df / 2
         df["custom_col"] = 5
         return df
 
+    # Please note: The base class enforces that the fit_transform method is implemented
     def fit_transform(
         self, df: pd.DataFrame, target: pd.Series
     ) -> Tuple[pd.DataFrame, pd.Series]:
         df = self.custom_function(df)
         df = df.head(1000)
         target = target.head(1000)
         return df, target
 
+    # Please note: The base class enforces that the fit_transform method is implemented
     def transform(
         self,
         df: pd.DataFrame,
         target: Optional[pd.Series] = None,
         predicton_mode: bool = False,
     ) -> Tuple[pd.DataFrame, Optional[pd.Series]]:
         df = self.custom_function(df)
         if not predicton_mode and isinstance(target, pd.Series):
             df = df.head(100)
             target = target.head(100)
         return df, targe
 
+custom_last_mile_computation = MyCustomLastMilePreprocessing()
 custom_preprocessor = MyCustomPreprocessing()
 
 # Pass the custom configs to the BlueCast class
 automl = BlueCast(
         class_problem="binary",
         target_column="target"
         conf_training=train_config,
         conf_xgboost=xgboost_param_config,
-        custom_preprocessor=custom_preprocessor,
+        custom_preprocessor=custom_preprocessor, # this takes place right after test_train_split
+        custom_last_mile_computation=custom_last_mile_computation, # last step before model training/prediction
     )
 
 automl.fit(df_train, target_col="target")
 y_probs, y_classes = automl.predict(df_val)
 ```
 
-## Custom ML model
+#### Custom ML model
 
 For some users it might just be convenient to use the BlueCast class to
 enjoy convenience features (details see below), but use a custom ML model.
 This is possible by passing a custom model to the BlueCast class. The needed properties
 are defined via the BaseClassMlModel class. Here is an example:
 
 ```sh
@@ -232,14 +290,17 @@
 x_train["target"] = y_trai
 # Fit the BlueCast model using the custom model
 bluecast.fit(x_train, "target"
 # Predict on the test data using the custom model
 predicted_probas, predicted_classes = bluecast.predict(x_test)
 ```
 
+Please note that custom ML models require user defined hyperparameter tuning. Pre-defined
+configurations are not available for custom models.
+
 ## Convenience features
 
 Despite being a lightweight library, BlueCast also includes some convenience
 with the following features:
 
 * automatic feature type detection and casting
 * automatic DataFrame schema detection: checks if unseen data has new or
@@ -284,15 +345,15 @@
 
 Documentation is provided via [Read the Docs](https://bluecast.readthedocs.io/en/latest/)
 
 ## How to contribute
 
 Contributions are welcome. Please follow the following steps:
 
-* Create a new branch
+* Create a new branch from develop branch
 * Add your feature or fix
 * Add unit tests for new features
 * Run pre-commit checks and unit tests (using Pytest)
 * Adjust the `docs/source/index.md` file
 * Copy paste the content of the `docs/source/index.md` file into the
   `README.md` file
 * Push your changes and create a pull request
```

### Comparing `bluecast-0.1/bluecast/blueprints/__pycache__/cast.cpython-310.pyc` & `bluecast-0.2/bluecast/blueprints/__pycache__/cast.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/bluecast/blueprints/cast.py` & `bluecast-0.2/bluecast/blueprints/cast.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,18 +26,15 @@
 from bluecast.preprocessing.feature_types import FeatureTypeDetector
 from bluecast.preprocessing.nulls_and_infs import fill_infinite_values
 from bluecast.preprocessing.schema_checks import SchemaDetector
 from bluecast.preprocessing.target_encoding import (
     BinaryClassTargetEncoder,
     MultiClassTargetEncoder,
 )
-from bluecast.preprocessing.train_test_split import (
-    train_test_split_cross,
-    train_test_split_time,
-)
+from bluecast.preprocessing.train_test_split import train_test_split
 
 
 class BlueCast:
     """Run fully configured classification blueprint.
 
     Customization via class attributes is possible. Configs can be instantiated and provided to change Xgboost training.
     Default hyperparameter search space is relatively light-weight to speed up the prototyping.
@@ -47,24 +44,29 @@
     BlueCast will infer these automaically.
     :param :date_columns: Takes a list of strings containing the names of the date columns. If not provided,
     BlueCast will infer these automaically.
     :param :time_split_column: Takes a string containing the name of the time split column. If not provided,
     BlueCast will not split the data by time or order, but do a random split instead.
     :param :ml_model: Takes an instance of a XgboostModel class. If not provided, BlueCast will instantiate one.
     This is an API to pass any model class. Inherit the baseclass from ml_modelling.base_model.BaseModel.
+    :param custom_preprocessor: Takes an instance of a CustomPreprocessing class. Allows users to inject custom
+    preprocessing steps which take place right after the train test spit.
+    :param custom_last_mile_computation: Takes an instance of a CustomPreprocessing class. Allows users to inject custom
+    preprocessing steps which take place right before the model training.
     """
 
     def __init__(
         self,
         class_problem: Literal["binary", "multiclass"],
         target_column: Union[str, float, int],
         cat_columns: Optional[List[Union[str, float, int]]] = None,
         date_columns: Optional[List[Union[str, float, int]]] = None,
         time_split_column: Optional[str] = None,
         ml_model: Optional[Union[XgboostModel, Any]] = None,
+        custom_last_mile_computation: Optional[CustomPreprocessing] = None,
         custom_preprocessor: Optional[CustomPreprocessing] = None,
         conf_training: Optional[TrainingConfig] = None,
         conf_xgboost: Optional[XgboostTuneParamsConfig] = None,
         conf_params_xgboost: Optional[XgboostFinalParamConfig] = None,
     ):
         self.class_problem = class_problem
         self.prediction_mode: bool = False
@@ -78,62 +80,89 @@
         self.feat_type_detector: Optional[FeatureTypeDetector] = None
         self.cat_encoder: Optional[
             Union[BinaryClassTargetEncoder, MultiClassTargetEncoder]
         ] = None
         self.target_label_encoder: Optional[TargetLabelEncoder] = None
         self.schema_detector: Optional[SchemaDetector] = None
         self.ml_model: Optional[XgboostModel] = ml_model
+        self.custom_last_mile_computation = custom_last_mile_computation
         self.custom_preprocessor = custom_preprocessor
         self.shap_values: Optional[np.ndarray] = None
 
     def fit(self, df: pd.DataFrame, target_col: str) -> None:
         """Train a full ML pipeline."""
         check_gpu_support()
-        self.feat_type_detector = FeatureTypeDetector()
-        df = self.feat_type_detector.fit_transform_feature_types(df)
+        feat_type_detector = FeatureTypeDetector()
+        df = feat_type_detector.fit_transform_feature_types(df)
+        self.feat_type_detector = feat_type_detector
 
         if self.feat_type_detector.cat_columns:
             if self.target_column in self.feat_type_detector.cat_columns:
                 self.target_label_encoder = TargetLabelEncoder()
                 df[
                     self.target_column
                 ] = self.target_label_encoder.fit_transform_target_labels(
                     df[self.target_column]
                 )
 
         self.cat_columns = self.feat_type_detector.cat_columns
         self.date_columns = self.feat_type_detector.date_columns
 
-        df = fill_infinite_values(df)
-        df = date_converter(df, self.date_columns)
+        if not self.conf_training:
+            self.conf_training = TrainingConfig()
 
-        if self.time_split_column is not None:
-            x_train, x_test, y_train, y_test = train_test_split_time(
-                df, target_col, self.time_split_column
+        x_train, x_test, y_train, y_test = train_test_split(
+            df,
+            target_col,
+            self.time_split_column,
+            self.conf_training.train_size,
+            self.conf_training.global_random_state,
+            self.conf_training.train_split_stratify,
+        )
+
+        if self.custom_preprocessor:
+            x_train, y_train = self.custom_preprocessor.fit_transform(x_train, y_train)
+            x_test, y_test = self.custom_preprocessor.transform(
+                x_test, y_test, predicton_mode=False
+            )
+            feat_type_detector = FeatureTypeDetector()
+            _ = feat_type_detector.fit_transform_feature_types(x_train)
+            x_train, y_train = x_train.reset_index(drop=True), y_train.reset_index(
+                drop=True
             )
-        else:
-            x_train, x_test, y_train, y_test = train_test_split_cross(df, target_col)
+            x_test, y_test = x_test.reset_index(drop=True), y_test.reset_index(
+                drop=True
+            )
+            if target_col in feat_type_detector.cat_columns:
+                feat_type_detector.cat_columns.remove(target_col)
+
+        x_train, x_test = fill_infinite_values(x_train), fill_infinite_values(x_test)
+        x_train, x_test = date_converter(x_train, self.date_columns), date_converter(
+            x_test, self.date_columns
+        )
 
         self.schema_detector = SchemaDetector()
         self.schema_detector.fit(x_train)
         x_test = self.schema_detector.transform(x_test)
 
         if self.cat_columns is not None and self.class_problem == "binary":
-            self.cat_encoder = BinaryClassTargetEncoder(self.cat_columns)
+            self.cat_encoder = BinaryClassTargetEncoder(feat_type_detector.cat_columns)
             x_train = self.cat_encoder.fit_target_encode_binary_class(x_train, y_train)
             x_test = self.cat_encoder.transform_target_encode_binary_class(x_test)
         elif self.cat_columns is not None and self.class_problem == "multiclass":
-            self.cat_encoder = MultiClassTargetEncoder(self.cat_columns)
+            self.cat_encoder = MultiClassTargetEncoder(feat_type_detector.cat_columns)
             x_train = self.cat_encoder.fit_target_encode_multiclass(x_train, y_train)
             x_test = self.cat_encoder.transform_target_encode_multiclass(x_test)
 
-        if self.custom_preprocessor:
-            x_train, y_train = self.custom_preprocessor.fit_transform(x_train, y_train)
-            x_test, y_test = self.custom_preprocessor.transform(
-                x_test, y_train, predicton_mode=False
+        if self.custom_last_mile_computation:
+            x_train, y_train = self.custom_last_mile_computation.fit_transform(
+                x_train, y_train
+            )
+            x_test, y_test = self.custom_last_mile_computation.transform(
+                x_test, y_test, predicton_mode=False
             )
 
         if not self.ml_model:
             self.ml_model = XgboostModel(
                 self.class_problem,
                 conf_training=self.conf_training,
                 conf_xgboost=self.conf_xgboost,
@@ -170,14 +199,19 @@
         check_gpu_support()
         if not self.feat_type_detector:
             raise Exception("Feature type converter could not be found.")
 
         df = self.feat_type_detector.transform_feature_types(
             df, ignore_cols=[self.target_column]
         )
+
+        if self.custom_preprocessor:
+            df, _ = self.custom_preprocessor.transform(df, predicton_mode=True)
+            df = df.reset_index(drop=True)
+
         df = fill_infinite_values(df)
         df = date_converter(df, self.date_columns)
 
         if self.schema_detector:
             df = self.schema_detector.transform(df)
 
         if (
@@ -191,16 +225,16 @@
             self.cat_columns
             and self.cat_encoder
             and self.class_problem == "multiclass"
             and isinstance(self.cat_encoder, MultiClassTargetEncoder)
         ):
             df = self.cat_encoder.transform_target_encode_multiclass(df)
 
-        if self.custom_preprocessor:
-            df, _ = self.custom_preprocessor.transform(df, predicton_mode=True)
+        if self.custom_last_mile_computation:
+            df, _ = self.custom_last_mile_computation.transform(df, predicton_mode=True)
         return df
 
     def predict(self, df: pd.DataFrame) -> Tuple[np.ndarray, np.ndarray]:
         """Predict on unseen data.
 
         Return the predicted probabilities and the predicted classes:
         y_probs, y_classes = predict(df)
```

### Comparing `bluecast-0.1/bluecast/config/__pycache__/training_config.cpython-310.pyc` & `bluecast-0.2/bluecast/config/__pycache__/training_config.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/bluecast/config/training_config.py` & `bluecast-0.2/bluecast/config/training_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,16 @@
     shuffle_during_training: bool = True
     hyperparameter_tuning_rounds: int = 100
     hyperparameter_tuning_max_runtime_secs: int = 3600
     hypertuning_cv_folds: int = 1
     early_stopping_rounds: int = 10
     autotune_model: bool = True
     calculate_shap_values: bool = True
+    train_size: float = 0.8
+    train_split_stratify: bool = True
 
 
 @dataclass
 class XgboostTuneParamsConfig:
     """Define hyperparameter tuning search space."""
 
     max_depth_min: int = 2
```

### Comparing `bluecast-0.1/bluecast/evaluation/__pycache__/eval_metrics.cpython-310.pyc` & `bluecast-0.2/bluecast/evaluation/__pycache__/eval_metrics.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/bluecast/evaluation/__pycache__/shap_values.cpython-310.pyc` & `bluecast-0.2/bluecast/evaluation/__pycache__/shap_values.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/bluecast/evaluation/eval_metrics.py` & `bluecast-0.2/bluecast/evaluation/eval_metrics.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/bluecast/evaluation/shap_values.py` & `bluecast-0.2/bluecast/evaluation/shap_values.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/bluecast/general_utils/__pycache__/general_utils.cpython-310.pyc` & `bluecast-0.2/bluecast/general_utils/__pycache__/general_utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/bluecast/general_utils/general_utils.py` & `bluecast-0.2/bluecast/general_utils/general_utils.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/bluecast/ml_modelling/__pycache__/base_classes.cpython-310.pyc` & `bluecast-0.2/bluecast/ml_modelling/__pycache__/base_classes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/bluecast/ml_modelling/__pycache__/xgboost.cpython-310.pyc` & `bluecast-0.2/bluecast/ml_modelling/__pycache__/xgboost.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/bluecast/ml_modelling/base_classes.py` & `bluecast-0.2/bluecast/ml_modelling/base_classes.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/bluecast/ml_modelling/xgboost.py` & `bluecast-0.2/bluecast/ml_modelling/xgboost.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/bluecast/preprocessing/__pycache__/custom.cpython-310.pyc` & `bluecast-0.2/bluecast/preprocessing/__pycache__/custom.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/bluecast/preprocessing/__pycache__/datetime_features.cpython-310.pyc` & `bluecast-0.2/bluecast/preprocessing/__pycache__/datetime_features.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-310.pyc` & `bluecast-0.2/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/bluecast/preprocessing/__pycache__/feature_types.cpython-310.pyc` & `bluecast-0.2/bluecast/preprocessing/__pycache__/feature_types.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/bluecast/preprocessing/__pycache__/general_utils.cpython-310.pyc` & `bluecast-0.2/bluecast/preprocessing/__pycache__/general_utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-310.pyc` & `bluecast-0.2/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/bluecast/preprocessing/__pycache__/schema_checks.cpython-310.pyc` & `bluecast-0.2/bluecast/preprocessing/__pycache__/schema_checks.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/bluecast/preprocessing/__pycache__/target_encoding.cpython-310.pyc` & `bluecast-0.2/bluecast/preprocessing/__pycache__/target_encoding.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/bluecast/preprocessing/__pycache__/train_test_split.cpython-310.pyc` & `bluecast-0.2/bluecast/preprocessing/__pycache__/train_test_split.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/bluecast/preprocessing/datetime_features.py` & `bluecast-0.2/bluecast/preprocessing/datetime_features.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/bluecast/preprocessing/encode_target_labels.py` & `bluecast-0.2/bluecast/preprocessing/encode_target_labels.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/bluecast/preprocessing/feature_types.py` & `bluecast-0.2/bluecast/preprocessing/feature_types.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,42 @@
 """
 Feature type detection and casting.
 
 This is a convenience class to detect and cast feature types in a DataFrame. It can be used to detect numerical,
 categorical and datetime columns. It also casts columns to a specific type.
 """
-from typing import Dict, List, Optional, Tuple, Union
+from typing import Dict, List, Tuple, Union
 
 import pandas as pd
 
 
 class FeatureTypeDetector:
     """Detect and cast feature types in DataFrame.
 
     Column names for individual feature types can be provided. Otherwise types will be inferred and casted accordingly.
     """
 
     def __init__(
         self,
-        num_columns: Optional[List[Union[str, int, float]]] = None,
-        cat_columns: Optional[List[Union[str, int, float]]] = None,
-        date_columns: Optional[List[Union[str, int, float]]] = None,
+        num_columns: List[Union[str, int, float]] = None,
+        cat_columns: List[Union[str, int, float]] = None,
+        date_columns: List[Union[str, int, float]] = None,
     ):
+        if not num_columns:
+            num_columns = []
         self.num_columns = num_columns
+
+        if not cat_columns:
+            cat_columns = []
         self.cat_columns = cat_columns
+
+        if not date_columns:
+            date_columns = []
         self.date_columns = date_columns
+
         self.detected_col_types: Dict[str, str] = {}
         self.num_dtypes = [
             "int8",
             "int16",
             "int32",
             "int64",
             "float16",
```

### Comparing `bluecast-0.1/bluecast/preprocessing/nulls_and_infs.py` & `bluecast-0.2/bluecast/preprocessing/nulls_and_infs.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/bluecast/preprocessing/schema_checks.py` & `bluecast-0.2/bluecast/preprocessing/schema_checks.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/bluecast/preprocessing/target_encoding.py` & `bluecast-0.2/bluecast/preprocessing/target_encoding.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/bluecast/preprocessing/train_test_split.py` & `bluecast-0.2/bluecast/preprocessing/train_test_split.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,41 +2,50 @@
 This module contains functions to split data into train and test sets.
 
 The train-test split can be done in two ways:
     - Randomly
     - Based on a provided order (i.e. time)
 """
 from datetime import datetime
+from typing import Optional
 
 import pandas as pd
 from sklearn import model_selection
 
 from bluecast.general_utils.general_utils import logger
 
 
 def train_test_split_cross(
     df: pd.DataFrame,
     target_col: str,
     train_size=0.80,
     random_state: int = 100,
-    stratify_col: str = None,
+    stratify: bool = False,
 ):
     """Split data into train and test. Stratification is possible."""
     logger(
         f"{datetime.utcnow()}: Start executing train-test split with train size of {train_size}."
     )
     target = df[target_col].copy()
     df = df.drop(target_col, axis=1)
+    if stratify:
+        stratify_data = target
+    else:
+        stratify_data = None
+
     x_train, x_test, y_train, y_test = model_selection.train_test_split(
         df,
         target,
         train_size=train_size,
         random_state=random_state,
-        stratify=stratify_col,
+        stratify=stratify_data,
     )
+    if target_col in x_train.columns:
+        x_train = x_train.drop(target_col, axis=1)
+        x_test = x_test.drop(target_col, axis=1)
     return x_train, x_test, y_train, y_test
 
 
 def train_test_split_time(
     df: pd.DataFrame, target_col: str, split_by_col: str, train_size: float = 0.80
 ):
     """Split data into train and test based on a provided order (i.e. time)."""
@@ -52,8 +61,38 @@
         df = df.sort_values(by=[split_by_col])
     else:
         pass
     x_train = df.head(train_length)
     x_test = df.tail(test_length)
     y_train = x_train[target_col]
     y_test = x_test[target_col]
+    # remove target column from x_train and x_test
+    if target_col in x_train.columns:
+        x_train = x_train.drop(target_col, axis=1)
+        x_test = x_test.drop(target_col, axis=1)
+    return x_train, x_test, y_train, y_test
+
+
+def train_test_split(
+    df: pd.DataFrame,
+    target_col: str,
+    split_by_col: Optional[str] = None,
+    train_size: float = 0.80,
+    random_state: int = 0,
+    stratify: bool = False,
+):
+    if split_by_col is not None:
+        x_train, x_test, y_train, y_test = train_test_split_time(
+            df,
+            target_col,
+            split_by_col,
+            train_size=train_size,
+        )
+    else:
+        x_train, x_test, y_train, y_test = train_test_split_cross(
+            df,
+            target_col,
+            train_size=train_size,
+            random_state=random_state,
+            stratify=stratify,
+        )
     return x_train, x_test, y_train, y_test
```

### Comparing `bluecast-0.1/bluecast/tests/__pycache__/test_cast.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.2/bluecast/tests/__pycache__/test_cast.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/bluecast/tests/__pycache__/test_check_gpu_support.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.2/bluecast/tests/__pycache__/test_check_gpu_support.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/bluecast/tests/__pycache__/test_datetime_features.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.2/bluecast/tests/__pycache__/test_datetime_features.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/bluecast/tests/__pycache__/test_encode_target_labels.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.2/bluecast/tests/__pycache__/test_encode_target_labels.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/bluecast/tests/__pycache__/test_feature_type_detector.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.2/bluecast/tests/__pycache__/test_feature_type_detector.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/bluecast/tests/__pycache__/test_load_for_production.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.2/bluecast/tests/__pycache__/test_load_for_production.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/bluecast/tests/__pycache__/test_nulls_and_infs.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.2/bluecast/tests/__pycache__/test_nulls_and_infs.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/bluecast/tests/__pycache__/test_save_to_production.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.2/bluecast/tests/__pycache__/test_save_to_production.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/bluecast/tests/__pycache__/test_schema_checks.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.2/bluecast/tests/__pycache__/test_schema_checks.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/bluecast/tests/__pycache__/test_shap_explanations.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.2/bluecast/tests/__pycache__/test_shap_explanations.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/bluecast/tests/__pycache__/test_target_encoding_binary.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.2/bluecast/tests/__pycache__/test_target_encoding_binary.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/bluecast/tests/__pycache__/test_target_encoding_multiclass.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.2/bluecast/tests/__pycache__/test_target_encoding_multiclass.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/bluecast/tests/__pycache__/test_train_test_split.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.2/bluecast/tests/__pycache__/test_train_test_split.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/bluecast/tests/make_data/__pycache__/create_data.cpython-310.pyc` & `bluecast-0.2/bluecast/tests/make_data/__pycache__/create_data.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/bluecast/tests/make_data/create_data.py` & `bluecast-0.2/bluecast/tests/make_data/create_data.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/bluecast/tests/test_cast.py` & `bluecast-0.2/bluecast/tests/test_cast.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Optional, Tuple
 
 import numpy as np
 import pandas as pd
 import pytest
-from sklearn.linear_model import LogisticRegression
+from sklearn.ensemble import RandomForestClassifier
 
 from bluecast.blueprints.cast import BlueCast
 from bluecast.config.training_config import TrainingConfig, XgboostTuneParamsConfig
 from bluecast.ml_modelling.base_classes import (
     BaseClassMlModel,
     PredictedClasses,
     PredictedProbas,
@@ -30,15 +30,15 @@
     xgboost_param_config = XgboostTuneParamsConfig()
     xgboost_param_config.steps_max = 100
     xgboost_param_config.num_leaves_max = 16
     train_config = TrainingConfig()
     train_config.hyperparameter_tuning_rounds = 10
 
     # add custom last mile computation
-    class MyCustomPreprocessing(CustomPreprocessing):
+    class MyCustomLastMilePreprocessing(CustomPreprocessing):
         def custom_function(self, df: pd.DataFrame) -> pd.DataFrame:
             df = df / 2
             df["custom_col"] = 5
             return df
 
         def fit_transform(
             self, df: pd.DataFrame, target: pd.Series
@@ -56,22 +56,22 @@
         ) -> Tuple[pd.DataFrame, Optional[pd.Series]]:
             df = self.custom_function(df)
             if not predicton_mode and isinstance(target, pd.Series):
                 df = df.head(100)
                 target = target.head(100)
             return df, target
 
-    custom_preprocessor = MyCustomPreprocessing()
+    custom_last_mile_computation = MyCustomLastMilePreprocessing()
 
     automl = BlueCast(
         class_problem="binary",
         target_column="target",
         conf_training=train_config,
         conf_xgboost=xgboost_param_config,
-        custom_preprocessor=custom_preprocessor,
+        custom_last_mile_computation=custom_last_mile_computation,
     )
     automl.fit(df_train, target_col="target")
     print("Autotuning successful.")
     y_probs, y_classes = automl.predict(df_val.drop("target", axis=1))
     print("Predicting successful.")
     assert len(y_probs) == len(df_val.index)
     assert len(y_classes) == len(df_val.index)
@@ -84,15 +84,15 @@
     def fit(
         self,
         x_train: pd.DataFrame,
         x_test: pd.DataFrame,
         y_train: pd.Series,
         y_test: pd.Series,
     ) -> None:
-        self.model = LogisticRegression()
+        self.model = RandomForestClassifier()
         self.model.fit(x_train, y_train)
 
     def predict(self, df: pd.DataFrame) -> Tuple[PredictedProbas, PredictedClasses]:
         predicted_probas = self.model.predict_proba(df)
         predicted_classes = self.model.predict(df)
         return predicted_probas, predicted_classes
```

### Comparing `bluecast-0.1/bluecast/tests/test_check_gpu_support.py` & `bluecast-0.2/bluecast/tests/test_check_gpu_support.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/bluecast/tests/test_custom_processing_base_class.py` & `bluecast-0.2/bluecast/tests/test_custom_processing_base_class.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/bluecast/tests/test_datetime_features.py` & `bluecast-0.2/bluecast/tests/test_datetime_features.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/bluecast/tests/test_encode_target_labels.py` & `bluecast-0.2/bluecast/tests/test_encode_target_labels.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/bluecast/tests/test_feature_type_detector.py` & `bluecast-0.2/bluecast/tests/test_feature_type_detector.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/bluecast/tests/test_load_for_production.py` & `bluecast-0.2/bluecast/tests/test_load_for_production.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/bluecast/tests/test_nulls_and_infs.py` & `bluecast-0.2/bluecast/tests/test_nulls_and_infs.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/bluecast/tests/test_save_to_production.py` & `bluecast-0.2/bluecast/tests/test_save_to_production.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/bluecast/tests/test_schema_checks.py` & `bluecast-0.2/bluecast/tests/test_schema_checks.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/bluecast/tests/test_shap_explanations.py` & `bluecast-0.2/bluecast/tests/test_shap_explanations.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/bluecast/tests/test_target_encoding_binary.py` & `bluecast-0.2/bluecast/tests/test_target_encoding_binary.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/bluecast/tests/test_target_encoding_multiclass.py` & `bluecast-0.2/bluecast/tests/test_target_encoding_multiclass.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/bluecast/tests/test_train_test_split.py` & `bluecast-0.2/bluecast/tests/test_train_test_split.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.1/pyproject.toml` & `bluecast-0.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bluecast"
-version = "0.1"
+version = "0.2"
 description = "A lightweight and fast automl framework"
 authors = ["Thomas Meißner <meissnercorporation@gmx.de>"]
 license = "GPL-3.0-only"
 classifiers = [
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
@@ -15,17 +15,17 @@
     { include = "bluecast" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"# lower not possible: https://github.com/python-poetry/poetry/issues/5628
 category_encoders = "^2.3.0"
 dill = "^0.3.3"
-matplotlib = "^3.1.3" # pinned due to cannot import _png error
+matplotlib = ">=3.1.3" # pinned due to cannot import _png error
 numpy = "<1.24.0" # otherwise: AttributeError: module 'numpy' has no attribute 'int'
-optuna = "^2.8.0"
+optuna = ">=2.8.0"
 pandas = "^1.1.5"
 plotly = "^5"
 pydantic = "^1.8.2"
 scikit-learn = "^1.0.1"
 shap = "^0"
 xgboost = "^1.5.3"
```

### Comparing `bluecast-0.1/PKG-INFO` & `bluecast-0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluecast
-Version: 0.1
+Version: 0.2
 Summary: A lightweight and fast automl framework
 Home-page: https://github.com/ThomasMeissnerDS/BlueCast
 License: GPL-3.0-only
 Author: Thomas Meißner
 Author-email: meissnercorporation@gmx.de
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -12,17 +12,17 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: full
 Provides-Extra: jupyter
 Requires-Dist: category_encoders (>=2.3.0,<3.0.0)
 Requires-Dist: dill (>=0.3.3,<0.4.0)
-Requires-Dist: matplotlib (>=3.1.3,<4.0.0)
+Requires-Dist: matplotlib (>=3.1.3)
 Requires-Dist: numpy (<1.24.0)
-Requires-Dist: optuna (>=2.8.0,<3.0.0)
+Requires-Dist: optuna (>=2.8.0)
 Requires-Dist: pandas (>=1.1.5,<2.0.0)
 Requires-Dist: plotly (>=5,<6)
 Requires-Dist: pydantic (>=1.8.2,<2.0.0)
 Requires-Dist: scikit-learn (>=1.0.1,<2.0.0)
 Requires-Dist: shap (>=0,<1)
 Requires-Dist: xgboost (>=1.5.3,<2.0.0)
 Project-URL: Repository, https://github.com/ThomasMeissnerDS/BlueCast
@@ -33,14 +33,17 @@
 [![codecov](https://codecov.io/gh/ThomasMeissnerDS/BlueCast/branch/main/graph/badge.svg?token=XRIS04O097)](https://codecov.io/gh/ThomasMeissnerDS/BlueCast)
 [![Codecov workflow](https://github.com/ThomasMeissnerDS/BlueCast/actions/workflows/workflow.yaml/badge.svg)](https://github.com/ThomasMeissnerDS/BlueCast/actions/workflows/workflow.yaml)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![pydocstyle](https://img.shields.io/badge/pydocstyle-enabled-AD4CD3)](http://www.pydocstyle.org/en/stable/)
 [![Documentation Status](https://readthedocs.org/projects/bluecast/badge/?version=latest)](https://bluecast.readthedocs.io/en/latest/?badge=latest)
+[![PyPI version](https://badge.fury.io/py/bluecast.svg)](https://pypi.python.org/pypi/bluecast/)
+![Known Vulnerabilities](https://snyk.io/test/github/ThomasMeissnerDS/BlueCast/main/badge.svg)
+[![Optuna](https://img.shields.io/badge/Optuna-integrated-blue)](https://optuna.org)
 [![python](https://img.shields.io/badge/Python-3.9-3776AB.svg?style=flat&logo=python&logoColor=white)](https://www.python.org)
 [![python](https://img.shields.io/badge/Python-3.10-3776AB.svg?style=flat&logo=python&logoColor=white)](https://www.python.org)
 [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com)
 
 A lightweight and fast auto-ml library. This is the successor of the
 e2eml automl library. While e2eml tried to cover many model
 architectures and a lot of different preprocessing options,
@@ -56,15 +59,15 @@
   * [Installation for end users](#installation-for-end-users)
   * [Installation for developers](#installation-for-developers)
 * [General usage](#general-usage)
   * [Basic usage](#basic-usage)
   * [Advanced usage](#advanced-usage)
     * [Custom training configuration](#custom--training-configuration)
     * [Custom preprocessing](#custom-preprocessing)
-* [Custom ML model](#custom-ml-model)
+    * [Custom ML model](#custom-ml-model)
 * [Convenience features](#convenience-features)
 * [Code quality](#code-quality)
 * [Documentation](#documentation)
 * [How to contribute](#how-to-contribute)
 * [Meta](#meta)
 
 <!-- tocstop -->
@@ -145,17 +148,19 @@
 y_probs, y_classes = automl.predict(df_val)
 ```
 
 #### Custom preprocessing
 
 The `BlueCast` class also allows for custom preprocessing. This is done by
 an abstract class that can be inherited and passed into the `BlueCast` class.
-The custom preprocessing will be called before the model training or prediction
-starts and allows users to execute last computations (i.e. sub sampling
-or final calculations).
+BlueCast provides two entry points to inject custom preprocessing. The
+attribute `custom_preprocessor` is called right after the train_test_split.
+The attribute `custom_last_mile_computation` will be called before the model
+training or prediction starts (when only numerical features are present anymore)
+and allows users to execute last computations (i.e. sub sampling or final calculations).
 
 ```sh
 from bluecast.blueprints.cast import BlueCast
 from bluecast.preprocessing.custom import CustomPreprocessing
 
 # Create a custom tuning config and adjust hyperparameter search space
 xgboost_param_config = XgboostTuneParamsConfig()
@@ -163,57 +168,110 @@
 xgboost_param_config.num_leaves_max = 16
 # Create a custom training config and adjust general training parameters
 train_config = TrainingConfig()
 train_config.hyperparameter_tuning_rounds = 10
 train_config.autotune_model = False # we want to run just normal training, no hyperparameter tuning
 # We could even just overwrite the final Xgboost params using the XgboostFinalParamConfig class
 
-# add custom last mile computation
 class MyCustomPreprocessing(CustomPreprocessing):
+    def __init__(self):
+        self.trained_patterns = {}
+
+    def fit_transform(
+        self, df: pd.DataFrame, target: pd.Series
+    ) -> Tuple[pd.DataFrame, pd.Series]:
+        num_columns = df.drop(['Beta', 'Gamma', 'Delta', 'Alpha', 'EJ'], axis=1).columns
+        cat_df = df[['Beta', 'Gamma', 'Delta', 'Alpha', 'EJ']].copy()
+
+        zscores = Zscores()
+        zscores.fit_all(df, ['Beta', 'Gamma', 'Delta', 'Alpha', 'EJ'])
+        df = zscores.transform_all(df, ['Beta', 'Gamma', 'Delta', 'Alpha', 'EJ'])
+        self.trained_patterns["zscores"] = zscores
+
+        imp_mean = SimpleImputer(missing_values=np.nan, strategy='median')
+        num_columns = df.drop(['Beta', 'Gamma', 'Delta', 'Alpha', 'EJ'], axis=1).columns
+        imp_mean.fit(df.loc[:, num_columns])
+        df = imp_mean.transform(df.loc[:, num_columns])
+        self.trained_patterns["imputation"] = imp_mean
+
+        df = pd.DataFrame(df, columns=num_columns).merge(cat_df, left_index=True, right_index=True, how="left")
+
+        df = df.drop(['Beta', 'Gamma', 'Delta', 'Alpha'], axis=1)
+
+        return df, target
+
+    def transform(
+        self,
+        df: pd.DataFrame,
+        target: Optional[pd.Series] = None,
+        predicton_mode: bool = False,
+    ) -> Tuple[pd.DataFrame, Optional[pd.Series]]:
+        num_columns = df.drop(['Beta', 'Gamma', 'Delta', 'Alpha', 'EJ'], axis=1).columns
+        cat_df = df[['Beta', 'Gamma', 'Delta', 'Alpha', 'EJ']].copy()
+
+        df = self.trained_patterns["zscores"].transform_all(df, ['Beta', 'Gamma', 'Delta', 'Alpha', 'EJ'])
+
+        imp_mean = self.trained_patterns["imputation"]
+        num_columns = df.drop(['Beta', 'Gamma', 'Delta', 'Alpha', 'EJ'], axis=1).columns
+        df.loc[:, num_columns] = df.loc[:, num_columns].replace([np.inf, -np.inf], np.nan)
+        df = imp_mean.transform(df.loc[:, num_columns])
+
+        df = pd.DataFrame(df, columns=num_columns).merge(cat_df, left_index=True, right_index=True, how="left")
+
+        df = df.drop(['Beta', 'Gamma', 'Delta', 'Alpha'], axis=1)
+
+        return df, target
+
+# add custom last mile computation
+class MyCustomLastMilePreprocessing(CustomPreprocessing):
     def custom_function(self, df: pd.DataFrame) -> pd.DataFrame:
         df = df / 2
         df["custom_col"] = 5
         return df
 
+    # Please note: The base class enforces that the fit_transform method is implemented
     def fit_transform(
         self, df: pd.DataFrame, target: pd.Series
     ) -> Tuple[pd.DataFrame, pd.Series]:
         df = self.custom_function(df)
         df = df.head(1000)
         target = target.head(1000)
         return df, target
 
+    # Please note: The base class enforces that the fit_transform method is implemented
     def transform(
         self,
         df: pd.DataFrame,
         target: Optional[pd.Series] = None,
         predicton_mode: bool = False,
     ) -> Tuple[pd.DataFrame, Optional[pd.Series]]:
         df = self.custom_function(df)
         if not predicton_mode and isinstance(target, pd.Series):
             df = df.head(100)
             target = target.head(100)
         return df, targe
 
+custom_last_mile_computation = MyCustomLastMilePreprocessing()
 custom_preprocessor = MyCustomPreprocessing()
 
 # Pass the custom configs to the BlueCast class
 automl = BlueCast(
         class_problem="binary",
         target_column="target"
         conf_training=train_config,
         conf_xgboost=xgboost_param_config,
-        custom_preprocessor=custom_preprocessor,
+        custom_preprocessor=custom_preprocessor, # this takes place right after test_train_split
+        custom_last_mile_computation=custom_last_mile_computation, # last step before model training/prediction
     )
 
 automl.fit(df_train, target_col="target")
 y_probs, y_classes = automl.predict(df_val)
 ```
 
-## Custom ML model
+#### Custom ML model
 
 For some users it might just be convenient to use the BlueCast class to
 enjoy convenience features (details see below), but use a custom ML model.
 This is possible by passing a custom model to the BlueCast class. The needed properties
 are defined via the BaseClassMlModel class. Here is an example:
 
 ```sh
@@ -262,14 +320,17 @@
 x_train["target"] = y_trai
 # Fit the BlueCast model using the custom model
 bluecast.fit(x_train, "target"
 # Predict on the test data using the custom model
 predicted_probas, predicted_classes = bluecast.predict(x_test)
 ```
 
+Please note that custom ML models require user defined hyperparameter tuning. Pre-defined
+configurations are not available for custom models.
+
 ## Convenience features
 
 Despite being a lightweight library, BlueCast also includes some convenience
 with the following features:
 
 * automatic feature type detection and casting
 * automatic DataFrame schema detection: checks if unseen data has new or
@@ -314,15 +375,15 @@
 
 Documentation is provided via [Read the Docs](https://bluecast.readthedocs.io/en/latest/)
 
 ## How to contribute
 
 Contributions are welcome. Please follow the following steps:
 
-* Create a new branch
+* Create a new branch from develop branch
 * Add your feature or fix
 * Add unit tests for new features
 * Run pre-commit checks and unit tests (using Pytest)
 * Adjust the `docs/source/index.md` file
 * Copy paste the content of the `docs/source/index.md` file into the
   `README.md` file
 * Push your changes and create a pull request
```

