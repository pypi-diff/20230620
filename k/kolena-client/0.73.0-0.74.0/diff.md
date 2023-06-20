# Comparing `tmp/kolena_client-0.73.0.tar.gz` & `tmp/kolena_client-0.74.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kolena_client-0.73.0.tar", max compression
+gzip compressed data, was "kolena_client-0.74.0.tar", max compression
```

## Comparing `kolena_client-0.73.0.tar` & `kolena_client-0.74.0.tar`

### file list

```diff
@@ -1,107 +1,109 @@
--rw-r--r--   0        0        0    11346 2023-06-13 21:32:39.845196 kolena_client-0.73.0/LICENSE
--rw-r--r--   0        0        0      556 2023-06-13 21:32:39.845196 kolena_client-0.73.0/LICENSE_HEADER
--rw-r--r--   0        0        0     2276 2023-06-13 21:32:39.845196 kolena_client-0.73.0/README.md
--rw-r--r--   0        0        0     1356 2023-06-13 21:38:32.867401 kolena_client-0.73.0/kolena/__init__.py
--rw-r--r--   0        0        0      579 2023-06-13 21:32:39.877198 kolena_client-0.73.0/kolena/_api/__init__.py
--rw-r--r--   0        0        0      579 2023-06-13 21:32:39.877198 kolena_client-0.73.0/kolena/_api/v1/__init__.py
--rw-r--r--   0        0        0     1737 2023-06-13 21:32:39.877198 kolena_client-0.73.0/kolena/_api/v1/batched_load.py
--rw-r--r--   0        0        0      878 2023-06-13 21:32:39.877198 kolena_client-0.73.0/kolena/_api/v1/client_log.py
--rw-r--r--   0        0        0     4153 2023-06-13 21:32:39.877198 kolena_client-0.73.0/kolena/_api/v1/core.py
--rw-r--r--   0        0        0     5320 2023-06-13 21:32:39.877198 kolena_client-0.73.0/kolena/_api/v1/detection.py
--rw-r--r--   0        0        0     7531 2023-06-13 21:32:39.877198 kolena_client-0.73.0/kolena/_api/v1/fr.py
--rw-r--r--   0        0        0     5540 2023-06-13 21:32:39.877198 kolena_client-0.73.0/kolena/_api/v1/generic.py
--rw-r--r--   0        0        0      778 2023-06-13 21:32:39.877198 kolena_client-0.73.0/kolena/_api/v1/repository.py
--rw-r--r--   0        0        0      833 2023-06-13 21:32:39.877198 kolena_client-0.73.0/kolena/_api/v1/token.py
--rw-r--r--   0        0        0      738 2023-06-13 21:32:39.877198 kolena_client-0.73.0/kolena/_api/v1/workflow.py
--rw-r--r--   0        0        0      579 2023-06-13 21:32:39.877198 kolena_client-0.73.0/kolena/_experimental/__init__.py
--rw-r--r--   0        0        0      579 2023-06-13 21:32:39.877198 kolena_client-0.73.0/kolena/_experimental/object_detection/__init__.py
--rw-r--r--   0        0        0     2520 2023-06-13 21:32:39.877198 kolena_client-0.73.0/kolena/_experimental/object_detection/utils.py
--rw-r--r--   0        0        0      579 2023-06-13 21:32:39.877198 kolena_client-0.73.0/kolena/_extras/__init__.py
--rw-r--r--   0        0        0      676 2023-06-13 21:32:39.877198 kolena_client-0.73.0/kolena/_extras/metrics/__init__.py
--rw-r--r--   0        0        0      786 2023-06-13 21:32:39.877198 kolena_client-0.73.0/kolena/_extras/metrics/sklearn.py
--rw-r--r--   0        0        0      579 2023-06-13 21:32:39.877198 kolena_client-0.73.0/kolena/_utils/__init__.py
--rw-r--r--   0        0        0     1616 2023-06-13 21:32:39.877198 kolena_client-0.73.0/kolena/_utils/asset_path_mapper.py
--rw-r--r--   0        0        0     5313 2023-06-13 21:32:39.877198 kolena_client-0.73.0/kolena/_utils/batched_load.py
--rw-r--r--   0        0        0     5608 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/_utils/cli.py
--rw-r--r--   0        0        0      783 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/_utils/consts.py
--rw-r--r--   0        0        0      579 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/_utils/dataframes/__init__.py
--rw-r--r--   0        0        0     2826 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/_utils/dataframes/validators.py
--rw-r--r--   0        0        0     1952 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/_utils/datatypes.py
--rw-r--r--   0        0        0     3403 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/_utils/endpoints.py
--rw-r--r--   0        0        0     1690 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/_utils/frozen.py
--rw-r--r--   0        0        0     1183 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/_utils/geometry.py
--rw-r--r--   0        0        0     1087 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/_utils/inference_validators.py
--rw-r--r--   0        0        0     2990 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/_utils/instrumentation.py
--rw-r--r--   0        0        0     4970 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/_utils/krequests.py
--rw-r--r--   0        0        0     3507 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/_utils/log.py
--rw-r--r--   0        0        0     1003 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/_utils/repository.py
--rw-r--r--   0        0        0     2494 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/_utils/serde.py
--rw-r--r--   0        0        0      889 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/_utils/serializable.py
--rw-r--r--   0        0        0     5450 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/_utils/state.py
--rw-r--r--   0        0        0     1942 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/_utils/uninstantiable.py
--rw-r--r--   0        0        0      852 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/_utils/validators.py
--rw-r--r--   0        0        0     1272 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/classification/__init__.py
--rw-r--r--   0        0        0     1475 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/classification/metadata.py
--rw-r--r--   0        0        0     3512 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/classification/model.py
--rw-r--r--   0        0        0     1213 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/classification/multiclass/__init__.py
--rw-r--r--   0        0        0     3354 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/classification/multiclass/_utils.py
--rw-r--r--   0        0        0    15698 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/classification/multiclass/evaluator.py
--rw-r--r--   0        0        0     3573 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/classification/multiclass/test_run.py
--rw-r--r--   0        0        0     3185 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/classification/multiclass/workflow.py
--rw-r--r--   0        0        0     2694 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/classification/test_case.py
--rw-r--r--   0        0        0     2372 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/classification/test_config.py
--rw-r--r--   0        0        0     4480 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/classification/test_image.py
--rw-r--r--   0        0        0     6013 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/classification/test_run.py
--rw-r--r--   0        0        0     3180 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/classification/test_suite.py
--rw-r--r--   0        0        0     1477 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/detection/__init__.py
--rw-r--r--   0        0        0     6819 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/detection/_datatypes.py
--rw-r--r--   0        0        0     1042 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/detection/_internal/__init__.py
--rw-r--r--   0        0        0     1922 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/detection/_internal/datatypes.py
--rw-r--r--   0        0        0      765 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/detection/_internal/ground_truth.py
--rw-r--r--   0        0        0     1035 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/detection/_internal/inference.py
--rw-r--r--   0        0        0     5470 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/detection/_internal/metadata.py
--rw-r--r--   0        0        0     8851 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/detection/_internal/model.py
--rw-r--r--   0        0        0    13920 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/detection/_internal/test_case.py
--rw-r--r--   0        0        0     1201 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/detection/_internal/test_config.py
--rw-r--r--   0        0        0     1761 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/detection/_internal/test_image.py
--rw-r--r--   0        0        0    12390 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/detection/_internal/test_run.py
--rw-r--r--   0        0        0    13600 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/detection/_internal/test_suite.py
--rw-r--r--   0        0        0     5867 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/detection/ground_truth.py
--rw-r--r--   0        0        0     5435 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/detection/inference.py
--rw-r--r--   0        0        0     1460 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/detection/metadata.py
--rw-r--r--   0        0        0     3210 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/detection/model.py
--rw-r--r--   0        0        0     2387 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/detection/test_case.py
--rw-r--r--   0        0        0     3199 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/detection/test_config.py
--rw-r--r--   0        0        0     5967 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/detection/test_image.py
--rw-r--r--   0        0        0     5405 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/detection/test_run.py
--rw-r--r--   0        0        0     2854 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/detection/test_suite.py
--rw-r--r--   0        0        0     2681 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/errors.py
--rw-r--r--   0        0        0     1400 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/fr/__init__.py
--rw-r--r--   0        0        0     2171 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/fr/_utils.py
--rw-r--r--   0        0        0    20960 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/fr/datatypes.py
--rw-r--r--   0        0        0    10130 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/fr/model.py
--rw-r--r--   0        0        0    14750 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/fr/test_case.py
--rw-r--r--   0        0        0    12237 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/fr/test_images.py
--rw-r--r--   0        0        0    16943 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/fr/test_run.py
--rw-r--r--   0        0        0    16125 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/fr/test_suite.py
--rw-r--r--   0        0        0     3865 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/initialize.py
--rw-r--r--   0        0        0     2474 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/workflow/__init__.py
--rw-r--r--   0        0        0    13877 2023-06-13 21:32:39.885199 kolena_client-0.73.0/kolena/workflow/_datatypes.py
--rw-r--r--   0        0        0     6281 2023-06-13 21:32:39.885199 kolena_client-0.73.0/kolena/workflow/_validators.py
--rw-r--r--   0        0        0    10397 2023-06-13 21:32:39.885199 kolena_client-0.73.0/kolena/workflow/annotation.py
--rw-r--r--   0        0        0     4926 2023-06-13 21:32:39.885199 kolena_client-0.73.0/kolena/workflow/asset.py
--rw-r--r--   0        0        0     3469 2023-06-13 21:32:39.885199 kolena_client-0.73.0/kolena/workflow/define_workflow.py
--rw-r--r--   0        0        0    21534 2023-06-13 21:32:39.885199 kolena_client-0.73.0/kolena/workflow/evaluator.py
--rw-r--r--   0        0        0    11232 2023-06-13 21:32:39.885199 kolena_client-0.73.0/kolena/workflow/evaluator_function.py
--rw-r--r--   0        0        0     4421 2023-06-13 21:32:39.885199 kolena_client-0.73.0/kolena/workflow/ground_truth.py
--rw-r--r--   0        0        0     4334 2023-06-13 21:32:39.885199 kolena_client-0.73.0/kolena/workflow/inference.py
--rw-r--r--   0        0        0      964 2023-06-13 21:32:39.885199 kolena_client-0.73.0/kolena/workflow/metrics/__init__.py
--rw-r--r--   0        0        0    15527 2023-06-13 21:32:39.885199 kolena_client-0.73.0/kolena/workflow/metrics/_geometry.py
--rw-r--r--   0        0        0     8265 2023-06-13 21:32:39.885199 kolena_client-0.73.0/kolena/workflow/model.py
--rw-r--r--   0        0        0    14301 2023-06-13 21:32:39.885199 kolena_client-0.73.0/kolena/workflow/test_case.py
--rw-r--r--   0        0        0    22734 2023-06-13 21:32:39.885199 kolena_client-0.73.0/kolena/workflow/test_run.py
--rw-r--r--   0        0        0    10564 2023-06-13 21:32:39.885199 kolena_client-0.73.0/kolena/workflow/test_sample.py
--rw-r--r--   0        0        0    15251 2023-06-13 21:32:39.885199 kolena_client-0.73.0/kolena/workflow/test_suite.py
--rw-r--r--   0        0        0     9419 2023-06-13 21:32:39.885199 kolena_client-0.73.0/kolena/workflow/workflow.py
--rw-r--r--   0        0        0     3048 2023-06-13 21:38:32.867401 kolena_client-0.73.0/pyproject.toml
--rw-r--r--   0        0        0     4658 1970-01-01 00:00:00.000000 kolena_client-0.73.0/PKG-INFO
+-rw-r--r--   0        0        0    11346 2023-06-20 20:05:45.838385 kolena_client-0.74.0/LICENSE
+-rw-r--r--   0        0        0      556 2023-06-20 20:05:45.838385 kolena_client-0.74.0/LICENSE_HEADER
+-rw-r--r--   0        0        0     2276 2023-06-20 20:05:45.838385 kolena_client-0.74.0/README.md
+-rw-r--r--   0        0        0     1356 2023-06-20 20:12:54.023944 kolena_client-0.74.0/kolena/__init__.py
+-rw-r--r--   0        0        0      579 2023-06-20 20:05:45.878385 kolena_client-0.74.0/kolena/_api/__init__.py
+-rw-r--r--   0        0        0      579 2023-06-20 20:05:45.878385 kolena_client-0.74.0/kolena/_api/v1/__init__.py
+-rw-r--r--   0        0        0     1737 2023-06-20 20:05:45.878385 kolena_client-0.74.0/kolena/_api/v1/batched_load.py
+-rw-r--r--   0        0        0      878 2023-06-20 20:05:45.878385 kolena_client-0.74.0/kolena/_api/v1/client_log.py
+-rw-r--r--   0        0        0     4153 2023-06-20 20:05:45.882385 kolena_client-0.74.0/kolena/_api/v1/core.py
+-rw-r--r--   0        0        0     5320 2023-06-20 20:05:45.882385 kolena_client-0.74.0/kolena/_api/v1/detection.py
+-rw-r--r--   0        0        0     7531 2023-06-20 20:05:45.882385 kolena_client-0.74.0/kolena/_api/v1/fr.py
+-rw-r--r--   0        0        0     5540 2023-06-20 20:05:45.882385 kolena_client-0.74.0/kolena/_api/v1/generic.py
+-rw-r--r--   0        0        0      778 2023-06-20 20:05:45.882385 kolena_client-0.74.0/kolena/_api/v1/repository.py
+-rw-r--r--   0        0        0      833 2023-06-20 20:05:45.882385 kolena_client-0.74.0/kolena/_api/v1/token.py
+-rw-r--r--   0        0        0      738 2023-06-20 20:05:45.882385 kolena_client-0.74.0/kolena/_api/v1/workflow.py
+-rw-r--r--   0        0        0      579 2023-06-20 20:05:45.882385 kolena_client-0.74.0/kolena/_experimental/__init__.py
+-rw-r--r--   0        0        0      579 2023-06-20 20:05:45.882385 kolena_client-0.74.0/kolena/_experimental/object_detection/__init__.py
+-rw-r--r--   0        0        0    10497 2023-06-20 20:05:45.882385 kolena_client-0.74.0/kolena/_experimental/object_detection/utils.py
+-rw-r--r--   0        0        0      579 2023-06-20 20:05:45.882385 kolena_client-0.74.0/kolena/_extras/__init__.py
+-rw-r--r--   0        0        0      676 2023-06-20 20:05:45.882385 kolena_client-0.74.0/kolena/_extras/metrics/__init__.py
+-rw-r--r--   0        0        0      783 2023-06-20 20:05:45.882385 kolena_client-0.74.0/kolena/_extras/metrics/sklearn.py
+-rw-r--r--   0        0        0      579 2023-06-20 20:05:45.882385 kolena_client-0.74.0/kolena/_utils/__init__.py
+-rw-r--r--   0        0        0     1616 2023-06-20 20:05:45.882385 kolena_client-0.74.0/kolena/_utils/asset_path_mapper.py
+-rw-r--r--   0        0        0     5313 2023-06-20 20:05:45.882385 kolena_client-0.74.0/kolena/_utils/batched_load.py
+-rw-r--r--   0        0        0     5608 2023-06-20 20:05:45.882385 kolena_client-0.74.0/kolena/_utils/cli.py
+-rw-r--r--   0        0        0      783 2023-06-20 20:05:45.882385 kolena_client-0.74.0/kolena/_utils/consts.py
+-rw-r--r--   0        0        0      579 2023-06-20 20:05:45.882385 kolena_client-0.74.0/kolena/_utils/dataframes/__init__.py
+-rw-r--r--   0        0        0     2826 2023-06-20 20:05:45.882385 kolena_client-0.74.0/kolena/_utils/dataframes/validators.py
+-rw-r--r--   0        0        0     1952 2023-06-20 20:05:45.882385 kolena_client-0.74.0/kolena/_utils/datatypes.py
+-rw-r--r--   0        0        0     3403 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/_utils/endpoints.py
+-rw-r--r--   0        0        0     1690 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/_utils/frozen.py
+-rw-r--r--   0        0        0     1183 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/_utils/geometry.py
+-rw-r--r--   0        0        0     1087 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/_utils/inference_validators.py
+-rw-r--r--   0        0        0     2990 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/_utils/instrumentation.py
+-rw-r--r--   0        0        0     4970 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/_utils/krequests.py
+-rw-r--r--   0        0        0     3507 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/_utils/log.py
+-rw-r--r--   0        0        0     1003 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/_utils/repository.py
+-rw-r--r--   0        0        0     2494 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/_utils/serde.py
+-rw-r--r--   0        0        0      889 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/_utils/serializable.py
+-rw-r--r--   0        0        0     5450 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/_utils/state.py
+-rw-r--r--   0        0        0     1942 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/_utils/uninstantiable.py
+-rw-r--r--   0        0        0      852 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/_utils/validators.py
+-rw-r--r--   0        0        0     1272 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/classification/__init__.py
+-rw-r--r--   0        0        0     1475 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/classification/metadata.py
+-rw-r--r--   0        0        0     3512 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/classification/model.py
+-rw-r--r--   0        0        0     1213 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/classification/multiclass/__init__.py
+-rw-r--r--   0        0        0     3354 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/classification/multiclass/_utils.py
+-rw-r--r--   0        0        0    15698 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/classification/multiclass/evaluator.py
+-rw-r--r--   0        0        0     3573 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/classification/multiclass/test_run.py
+-rw-r--r--   0        0        0     3185 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/classification/multiclass/workflow.py
+-rw-r--r--   0        0        0     2694 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/classification/test_case.py
+-rw-r--r--   0        0        0     2372 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/classification/test_config.py
+-rw-r--r--   0        0        0     4480 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/classification/test_image.py
+-rw-r--r--   0        0        0     6013 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/classification/test_run.py
+-rw-r--r--   0        0        0     3180 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/classification/test_suite.py
+-rw-r--r--   0        0        0     1477 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/detection/__init__.py
+-rw-r--r--   0        0        0     6819 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/detection/_datatypes.py
+-rw-r--r--   0        0        0     1042 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/detection/_internal/__init__.py
+-rw-r--r--   0        0        0     1922 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/detection/_internal/datatypes.py
+-rw-r--r--   0        0        0      765 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/detection/_internal/ground_truth.py
+-rw-r--r--   0        0        0     1035 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/detection/_internal/inference.py
+-rw-r--r--   0        0        0     5470 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/detection/_internal/metadata.py
+-rw-r--r--   0        0        0     8851 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/detection/_internal/model.py
+-rw-r--r--   0        0        0    13920 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/detection/_internal/test_case.py
+-rw-r--r--   0        0        0     1201 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/detection/_internal/test_config.py
+-rw-r--r--   0        0        0     1761 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/detection/_internal/test_image.py
+-rw-r--r--   0        0        0    12390 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/detection/_internal/test_run.py
+-rw-r--r--   0        0        0    13600 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/detection/_internal/test_suite.py
+-rw-r--r--   0        0        0     5867 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/detection/ground_truth.py
+-rw-r--r--   0        0        0     5435 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/detection/inference.py
+-rw-r--r--   0        0        0     1460 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/detection/metadata.py
+-rw-r--r--   0        0        0     3210 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/detection/model.py
+-rw-r--r--   0        0        0     2387 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/detection/test_case.py
+-rw-r--r--   0        0        0     3199 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/detection/test_config.py
+-rw-r--r--   0        0        0     5967 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/detection/test_image.py
+-rw-r--r--   0        0        0     5405 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/detection/test_run.py
+-rw-r--r--   0        0        0     2854 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/detection/test_suite.py
+-rw-r--r--   0        0        0     2681 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/errors.py
+-rw-r--r--   0        0        0     1400 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/fr/__init__.py
+-rw-r--r--   0        0        0     2171 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/fr/_utils.py
+-rw-r--r--   0        0        0    20960 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/fr/datatypes.py
+-rw-r--r--   0        0        0    10130 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/fr/model.py
+-rw-r--r--   0        0        0    14750 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/fr/test_case.py
+-rw-r--r--   0        0        0    12237 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/fr/test_images.py
+-rw-r--r--   0        0        0    16943 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/fr/test_run.py
+-rw-r--r--   0        0        0    16125 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/fr/test_suite.py
+-rw-r--r--   0        0        0     3880 2023-06-20 20:05:45.886385 kolena_client-0.74.0/kolena/initialize.py
+-rw-r--r--   0        0        0     2439 2023-06-20 20:05:45.890385 kolena_client-0.74.0/kolena/workflow/__init__.py
+-rw-r--r--   0        0        0    13877 2023-06-20 20:05:45.890385 kolena_client-0.74.0/kolena/workflow/_datatypes.py
+-rw-r--r--   0        0        0     6281 2023-06-20 20:05:45.890385 kolena_client-0.74.0/kolena/workflow/_validators.py
+-rw-r--r--   0        0        0    10397 2023-06-20 20:05:45.890385 kolena_client-0.74.0/kolena/workflow/annotation.py
+-rw-r--r--   0        0        0     4926 2023-06-20 20:05:45.890385 kolena_client-0.74.0/kolena/workflow/asset.py
+-rw-r--r--   0        0        0     3469 2023-06-20 20:05:45.890385 kolena_client-0.74.0/kolena/workflow/define_workflow.py
+-rw-r--r--   0        0        0    13019 2023-06-20 20:05:45.890385 kolena_client-0.74.0/kolena/workflow/evaluator.py
+-rw-r--r--   0        0        0    11232 2023-06-20 20:05:45.890385 kolena_client-0.74.0/kolena/workflow/evaluator_function.py
+-rw-r--r--   0        0        0     4421 2023-06-20 20:05:45.890385 kolena_client-0.74.0/kolena/workflow/ground_truth.py
+-rw-r--r--   0        0        0     4334 2023-06-20 20:05:45.890385 kolena_client-0.74.0/kolena/workflow/inference.py
+-rw-r--r--   0        0        0     1103 2023-06-20 20:05:45.890385 kolena_client-0.74.0/kolena/workflow/metrics/__init__.py
+-rw-r--r--   0        0        0     2528 2023-06-20 20:05:45.890385 kolena_client-0.74.0/kolena/workflow/metrics/_formula.py
+-rw-r--r--   0        0        0    15527 2023-06-20 20:05:45.890385 kolena_client-0.74.0/kolena/workflow/metrics/_geometry.py
+-rw-r--r--   0        0        0     8265 2023-06-20 20:05:45.890385 kolena_client-0.74.0/kolena/workflow/model.py
+-rw-r--r--   0        0        0    10261 2023-06-20 20:05:45.890385 kolena_client-0.74.0/kolena/workflow/plot.py
+-rw-r--r--   0        0        0    14301 2023-06-20 20:05:45.890385 kolena_client-0.74.0/kolena/workflow/test_case.py
+-rw-r--r--   0        0        0    22734 2023-06-20 20:05:45.890385 kolena_client-0.74.0/kolena/workflow/test_run.py
+-rw-r--r--   0        0        0    10564 2023-06-20 20:05:45.890385 kolena_client-0.74.0/kolena/workflow/test_sample.py
+-rw-r--r--   0        0        0    15251 2023-06-20 20:05:45.890385 kolena_client-0.74.0/kolena/workflow/test_suite.py
+-rw-r--r--   0        0        0     9419 2023-06-20 20:05:45.890385 kolena_client-0.74.0/kolena/workflow/workflow.py
+-rw-r--r--   0        0        0     3042 2023-06-20 20:12:54.023944 kolena_client-0.74.0/pyproject.toml
+-rw-r--r--   0        0        0     4658 1970-01-01 00:00:00.000000 kolena_client-0.74.0/PKG-INFO
```

### Comparing `kolena_client-0.73.0/LICENSE` & `kolena_client-0.74.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/LICENSE_HEADER` & `kolena_client-0.74.0/LICENSE_HEADER`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/README.md` & `kolena_client-0.74.0/README.md`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/__init__.py` & `kolena_client-0.74.0/kolena/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/_api/__init__.py` & `kolena_client-0.74.0/kolena/_api/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/_api/v1/__init__.py` & `kolena_client-0.74.0/kolena/_api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/_api/v1/batched_load.py` & `kolena_client-0.74.0/kolena/_api/v1/batched_load.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/_api/v1/client_log.py` & `kolena_client-0.74.0/kolena/_api/v1/client_log.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/_api/v1/core.py` & `kolena_client-0.74.0/kolena/_api/v1/core.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/_api/v1/detection.py` & `kolena_client-0.74.0/kolena/_api/v1/detection.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/_api/v1/fr.py` & `kolena_client-0.74.0/kolena/_api/v1/fr.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/_api/v1/generic.py` & `kolena_client-0.74.0/kolena/_api/v1/generic.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/_api/v1/repository.py` & `kolena_client-0.74.0/kolena/_api/v1/repository.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/_api/v1/token.py` & `kolena_client-0.74.0/kolena/_api/v1/token.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/_api/v1/workflow.py` & `kolena_client-0.74.0/kolena/_api/v1/workflow.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/_experimental/__init__.py` & `kolena_client-0.74.0/kolena/_experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/_experimental/object_detection/__init__.py` & `kolena_client-0.74.0/kolena/_experimental/object_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/_extras/__init__.py` & `kolena_client-0.74.0/kolena/_extras/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/_extras/metrics/__init__.py` & `kolena_client-0.74.0/kolena/_extras/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/_extras/metrics/sklearn.py` & `kolena_client-0.74.0/kolena/_extras/metrics/sklearn.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 try:
     import sklearn.metrics as sklearn_metrics  # noqa: F401
 
 except ImportError:
-    raise ImportError("Package 'scikit-learn' not found; install 'metrics' extras with `pip install 'kolena[metrics]'`")
+    raise ImportError("Package 'scikit-learn' not found; install 'metrics' extra with `pip install kolena[metrics]`")
```

### Comparing `kolena_client-0.73.0/kolena/_utils/__init__.py` & `kolena_client-0.74.0/kolena/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/_utils/asset_path_mapper.py` & `kolena_client-0.74.0/kolena/_utils/asset_path_mapper.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/_utils/batched_load.py` & `kolena_client-0.74.0/kolena/_utils/batched_load.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/_utils/cli.py` & `kolena_client-0.74.0/kolena/_utils/cli.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/_utils/consts.py` & `kolena_client-0.74.0/kolena/_utils/consts.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/_utils/dataframes/__init__.py` & `kolena_client-0.74.0/kolena/_utils/dataframes/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/_utils/dataframes/validators.py` & `kolena_client-0.74.0/kolena/_utils/dataframes/validators.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/_utils/datatypes.py` & `kolena_client-0.74.0/kolena/_utils/datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/_utils/endpoints.py` & `kolena_client-0.74.0/kolena/_utils/endpoints.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/_utils/frozen.py` & `kolena_client-0.74.0/kolena/_utils/frozen.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/_utils/geometry.py` & `kolena_client-0.74.0/kolena/_utils/geometry.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/_utils/inference_validators.py` & `kolena_client-0.74.0/kolena/_utils/inference_validators.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/_utils/instrumentation.py` & `kolena_client-0.74.0/kolena/_utils/instrumentation.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/_utils/krequests.py` & `kolena_client-0.74.0/kolena/_utils/krequests.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/_utils/log.py` & `kolena_client-0.74.0/kolena/_utils/log.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/_utils/repository.py` & `kolena_client-0.74.0/kolena/_utils/repository.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/_utils/serde.py` & `kolena_client-0.74.0/kolena/_utils/serde.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/_utils/serializable.py` & `kolena_client-0.74.0/kolena/_utils/serializable.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/_utils/state.py` & `kolena_client-0.74.0/kolena/_utils/state.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/_utils/uninstantiable.py` & `kolena_client-0.74.0/kolena/_utils/uninstantiable.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/_utils/validators.py` & `kolena_client-0.74.0/kolena/_utils/validators.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/classification/__init__.py` & `kolena_client-0.74.0/kolena/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/classification/metadata.py` & `kolena_client-0.74.0/kolena/classification/metadata.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/classification/model.py` & `kolena_client-0.74.0/kolena/classification/model.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/classification/multiclass/__init__.py` & `kolena_client-0.74.0/kolena/classification/multiclass/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/classification/multiclass/_utils.py` & `kolena_client-0.74.0/kolena/classification/multiclass/_utils.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/classification/multiclass/evaluator.py` & `kolena_client-0.74.0/kolena/classification/multiclass/evaluator.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/classification/multiclass/test_run.py` & `kolena_client-0.74.0/kolena/classification/multiclass/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/classification/multiclass/workflow.py` & `kolena_client-0.74.0/kolena/classification/multiclass/workflow.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/classification/test_case.py` & `kolena_client-0.74.0/kolena/classification/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/classification/test_config.py` & `kolena_client-0.74.0/kolena/classification/test_config.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/classification/test_image.py` & `kolena_client-0.74.0/kolena/classification/test_image.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/classification/test_run.py` & `kolena_client-0.74.0/kolena/classification/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/classification/test_suite.py` & `kolena_client-0.74.0/kolena/classification/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/detection/__init__.py` & `kolena_client-0.74.0/kolena/detection/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/detection/_datatypes.py` & `kolena_client-0.74.0/kolena/detection/_datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/detection/_internal/__init__.py` & `kolena_client-0.74.0/kolena/detection/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/detection/_internal/datatypes.py` & `kolena_client-0.74.0/kolena/detection/_internal/datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/detection/_internal/ground_truth.py` & `kolena_client-0.74.0/kolena/detection/_internal/ground_truth.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/detection/_internal/inference.py` & `kolena_client-0.74.0/kolena/detection/_internal/inference.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/detection/_internal/metadata.py` & `kolena_client-0.74.0/kolena/detection/_internal/metadata.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/detection/_internal/model.py` & `kolena_client-0.74.0/kolena/detection/_internal/model.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/detection/_internal/test_case.py` & `kolena_client-0.74.0/kolena/detection/_internal/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/detection/_internal/test_config.py` & `kolena_client-0.74.0/kolena/detection/_internal/test_config.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/detection/_internal/test_image.py` & `kolena_client-0.74.0/kolena/detection/_internal/test_image.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/detection/_internal/test_run.py` & `kolena_client-0.74.0/kolena/detection/_internal/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/detection/_internal/test_suite.py` & `kolena_client-0.74.0/kolena/detection/_internal/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/detection/ground_truth.py` & `kolena_client-0.74.0/kolena/detection/ground_truth.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/detection/inference.py` & `kolena_client-0.74.0/kolena/detection/inference.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/detection/metadata.py` & `kolena_client-0.74.0/kolena/detection/metadata.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/detection/model.py` & `kolena_client-0.74.0/kolena/detection/model.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/detection/test_case.py` & `kolena_client-0.74.0/kolena/detection/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/detection/test_config.py` & `kolena_client-0.74.0/kolena/detection/test_config.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/detection/test_image.py` & `kolena_client-0.74.0/kolena/detection/test_image.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/detection/test_run.py` & `kolena_client-0.74.0/kolena/detection/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/detection/test_suite.py` & `kolena_client-0.74.0/kolena/detection/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/errors.py` & `kolena_client-0.74.0/kolena/errors.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/fr/__init__.py` & `kolena_client-0.74.0/kolena/fr/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/fr/_utils.py` & `kolena_client-0.74.0/kolena/fr/_utils.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/fr/datatypes.py` & `kolena_client-0.74.0/kolena/fr/datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/fr/model.py` & `kolena_client-0.74.0/kolena/fr/model.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/fr/test_case.py` & `kolena_client-0.74.0/kolena/fr/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/fr/test_images.py` & `kolena_client-0.74.0/kolena/fr/test_images.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/fr/test_run.py` & `kolena_client-0.74.0/kolena/fr/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/fr/test_suite.py` & `kolena_client-0.74.0/kolena/fr/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/initialize.py` & `kolena_client-0.74.0/kolena/initialize.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     verbose: bool = False,
     proxies: Optional[Dict[str, str]] = None,
     **kwargs: Any,
 ) -> None:
     """
     Initialize a client session.
 
-    Retrieve an API token from [app.kolena.io/~/developer](https://app.kolena.io/redirect/developer) and
+    Retrieve an API token from the [:kolena-developer-16: Developer](https://app.kolena.io/redirect/developer) page and
     populate the `KOLENA_TOKEN` environment variable before initializing:
 
     ```python
     import os
     import kolena
 
     kolena.initialize(os.environ["KOLENA_TOKEN"], verbose=True)
```

### Comparing `kolena_client-0.73.0/kolena/workflow/__init__.py` & `kolena_client-0.74.0/kolena/workflow/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -26,21 +26,21 @@
 from .test_sample import Document
 from .ground_truth import GroundTruth
 from .inference import Inference
 from .workflow import Workflow
 from .test_case import TestCase
 from .test_suite import TestSuite
 from .model import Model
-from .evaluator import AxisConfig
-from .evaluator import Plot
-from .evaluator import Curve
-from .evaluator import CurvePlot
-from .evaluator import ConfusionMatrix
-from .evaluator import Histogram
-from .evaluator import BarPlot
+from .plot import AxisConfig
+from .plot import Plot
+from .plot import Curve
+from .plot import CurvePlot
+from .plot import ConfusionMatrix
+from .plot import Histogram
+from .plot import BarPlot
 from .evaluator import MetricsTestCase
 from .evaluator import MetricsTestSample
 from .evaluator import MetricsTestSuite
 from .evaluator import Evaluator
 from .evaluator import EvaluatorConfiguration
 from .evaluator_function import BasicEvaluatorFunction
 from .evaluator_function import TestCases
```

### Comparing `kolena_client-0.73.0/kolena/workflow/_datatypes.py` & `kolena_client-0.74.0/kolena/workflow/_datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/workflow/_validators.py` & `kolena_client-0.74.0/kolena/workflow/_validators.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/workflow/annotation.py` & `kolena_client-0.74.0/kolena/workflow/annotation.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/workflow/asset.py` & `kolena_client-0.74.0/kolena/workflow/asset.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/workflow/define_workflow.py` & `kolena_client-0.74.0/kolena/workflow/define_workflow.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/workflow/evaluator_function.py` & `kolena_client-0.74.0/kolena/workflow/evaluator_function.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/workflow/ground_truth.py` & `kolena_client-0.74.0/kolena/workflow/ground_truth.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/workflow/inference.py` & `kolena_client-0.74.0/kolena/workflow/inference.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/workflow/metrics/__init__.py` & `kolena_client-0.74.0/kolena/workflow/metrics/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,21 +7,27 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from ._formula import f1_score
+from ._formula import precision
+from ._formula import recall
 from ._geometry import InferenceMatches
 from ._geometry import iou
 from ._geometry import match_inferences
 from ._geometry import match_inferences_multiclass
 from ._geometry import MulticlassInferenceMatches
 
 __all__ = [
+    "precision",
+    "recall",
+    "f1_score",
     "iou",
     "InferenceMatches",
     "match_inferences",
     "MulticlassInferenceMatches",
     "match_inferences_multiclass",
     "MulticlassInferenceMatches",
 ]
```

### Comparing `kolena_client-0.73.0/kolena/workflow/metrics/_geometry.py` & `kolena_client-0.74.0/kolena/workflow/metrics/_geometry.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/workflow/model.py` & `kolena_client-0.74.0/kolena/workflow/model.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/workflow/test_case.py` & `kolena_client-0.74.0/kolena/workflow/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/workflow/test_run.py` & `kolena_client-0.74.0/kolena/workflow/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/workflow/test_sample.py` & `kolena_client-0.74.0/kolena/workflow/test_sample.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/workflow/test_suite.py` & `kolena_client-0.74.0/kolena/workflow/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/kolena/workflow/workflow.py` & `kolena_client-0.74.0/kolena/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.73.0/pyproject.toml` & `kolena_client-0.74.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kolena-client"
-version = "0.73.0"  # version is automatically set to latest git tag during release process
+version = "0.74.0"  # version is automatically set to latest git tag during release process
 description = "Client for Kolena's machine learning (ML) testing and debugging platform."
 authors = ["Kolena Engineering <eng@kolena.io>"]
 homepage = "https://kolena.io"
 documentation = "https://docs.kolena.io"
 readme = "README.md"
 license = "Apache-2.0"
 keywords = ["Kolena", "ML", "testing"]
@@ -65,15 +65,14 @@
 pytest-depends = "^1.0.1"
 mkdocs = "^1.4.3"
 cairosvg = "^2.7.0"
 mkdocs-material = "^9.1.15"  # insiders fork installed out-of-band in docs/setup_insiders.sh
 mkdocstrings = { version = ">0.20,<1", extras = ["python"] }
 mkdocs-git-committers-plugin-2 = "^1.1.2"
 mkdocs-git-revision-date-localized-plugin = "^1.2.0"
-mkdocs-glightbox = "^0.3.4"
 
 [tool.poetry.scripts]
 kolena = 'kolena._utils.cli:run'
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
@@ -82,9 +81,9 @@
 # do not scan 'kolena' for tests, as there are many functions/classes that look like tests
 norecursedirs = "kolena"
 # explicitly disable test classes such that e.g. TestRun is not interpreted as a test
 python_classes = []
 # only collect functions starting with 'test__'
 python_functions = ["test__*"]
 markers = [
-    "metrics: tests that extra dependencies for metrics",
+    "metrics: tests that require the metrics extra dependency such as sklearn",
 ]
```

### Comparing `kolena_client-0.73.0/PKG-INFO` & `kolena_client-0.74.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kolena-client
-Version: 0.73.0
+Version: 0.74.0
 Summary: Client for Kolena's machine learning (ML) testing and debugging platform.
 Home-page: https://kolena.io
 License: Apache-2.0
 Keywords: Kolena,ML,testing
 Author: Kolena Engineering
 Author-email: eng@kolena.io
 Requires-Python: >=3.7.1,<3.12
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kolena-client Version: 0.73.0 Summary: Client for
+Metadata-Version: 2.1 Name: kolena-client Version: 0.74.0 Summary: Client for
 Kolena's machine learning (ML) testing and debugging platform. Home-page:
 https://kolena.io License: Apache-2.0 Keywords: Kolena,ML,testing Author:
 Kolena Engineering Author-email: eng@kolena.io Requires-Python: >=3.7.1,<3.12
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Natural Language
 :: English Classifier: Programming Language :: Python :: 3 Classifier:
```

