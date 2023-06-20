# Comparing `tmp/mlpype-0.4.0.tar.gz` & `tmp/mlpype-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpype-0.4.0.tar", last modified: Fri May  5 10:36:25 2023, max compression
+gzip compressed data, was "mlpype-0.4.1.tar", last modified: Tue Jun 20 16:46:41 2023, max compression
```

## Comparing `mlpype-0.4.0.tar` & `mlpype-0.4.1.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxr-xr-x   0 vandejer (1865779777) 296108113        0 2023-05-05 10:36:25.605174 mlpype-0.4.0/
--rw-r--r--   0 vandejer (1865779777) 296108113      564 2022-12-16 14:17:05.000000 mlpype-0.4.0/LICENSE.txt
--rw-r--r--   0 vandejer (1865779777) 296108113     5741 2023-05-05 10:36:25.605277 mlpype-0.4.0/PKG-INFO
--rw-r--r--   0 vandejer (1865779777) 296108113     5455 2023-05-05 10:24:10.000000 mlpype-0.4.0/README.md
-drwxr-xr-x   0 vandejer (1865779777) 296108113        0 2023-05-05 10:36:25.350810 mlpype-0.4.0/mlpype/
-drwxr-xr-x   0 vandejer (1865779777) 296108113        0 2023-05-05 10:36:25.379740 mlpype-0.4.0/mlpype/base/
--rw-r--r--   0 vandejer (1865779777) 296108113        0 2023-03-31 14:32:04.000000 mlpype-0.4.0/mlpype/base/__init__.py
--rw-r--r--   0 vandejer (1865779777) 296108113      497 2023-04-17 20:12:33.000000 mlpype-0.4.0/mlpype/base/constants.py
-drwxr-xr-x   0 vandejer (1865779777) 296108113        0 2023-05-05 10:36:25.386507 mlpype-0.4.0/mlpype/base/data/
--rw-r--r--   0 vandejer (1865779777) 296108113      135 2023-04-17 20:33:25.000000 mlpype-0.4.0/mlpype/base/data/__init__.py
--rw-r--r--   0 vandejer (1865779777) 296108113     4875 2023-05-05 10:18:55.000000 mlpype-0.4.0/mlpype/base/data/data_catalog.py
--rw-r--r--   0 vandejer (1865779777) 296108113      274 2022-12-16 14:17:05.000000 mlpype-0.4.0/mlpype/base/data/data_sink.py
--rw-r--r--   0 vandejer (1865779777) 296108113      459 2022-10-03 09:01:57.000000 mlpype-0.4.0/mlpype/base/data/data_source.py
--rw-r--r--   0 vandejer (1865779777) 296108113     1724 2022-12-16 16:16:55.000000 mlpype-0.4.0/mlpype/base/data/dataset.py
-drwxr-xr-x   0 vandejer (1865779777) 296108113        0 2023-05-05 10:36:25.393821 mlpype-0.4.0/mlpype/base/deploy/
--rw-r--r--   0 vandejer (1865779777) 296108113       34 2023-04-16 09:57:26.000000 mlpype-0.4.0/mlpype/base/deploy/__init__.py
--rw-r--r--   0 vandejer (1865779777) 296108113     4970 2023-05-05 10:18:55.000000 mlpype-0.4.0/mlpype/base/deploy/inference.py
-drwxr-xr-x   0 vandejer (1865779777) 296108113        0 2023-05-05 10:36:25.399458 mlpype-0.4.0/mlpype/base/deploy/wheel/
--rw-r--r--   0 vandejer (1865779777) 296108113       73 2022-12-16 14:17:05.000000 mlpype-0.4.0/mlpype/base/deploy/wheel/__init__.py
--rw-r--r--   0 vandejer (1865779777) 296108113     5335 2023-05-05 10:18:55.000000 mlpype-0.4.0/mlpype/base/deploy/wheel/builder.py
--rw-r--r--   0 vandejer (1865779777) 296108113     3820 2023-05-05 10:18:55.000000 mlpype-0.4.0/mlpype/base/deploy/wheel/extensions.py
-drwxr-xr-x   0 vandejer (1865779777) 296108113        0 2023-05-05 10:36:25.400691 mlpype-0.4.0/mlpype/base/deploy/wheel/helpers/
--rw-r--r--   0 vandejer (1865779777) 296108113      799 2022-12-16 16:16:55.000000 mlpype-0.4.0/mlpype/base/deploy/wheel/helpers/setup_template.py
--rw-r--r--   0 vandejer (1865779777) 296108113      416 2023-05-05 10:18:55.000000 mlpype-0.4.0/mlpype/base/deploy/wheel/helpers/wheel_main.py
--rw-r--r--   0 vandejer (1865779777) 296108113     3230 2023-05-05 10:18:55.000000 mlpype-0.4.0/mlpype/base/deploy/wheel/wheel.py
-drwxr-xr-x   0 vandejer (1865779777) 296108113        0 2023-05-05 10:36:25.410173 mlpype-0.4.0/mlpype/base/evaluate/
--rw-r--r--   0 vandejer (1865779777) 296108113       75 2023-01-20 12:18:51.000000 mlpype-0.4.0/mlpype/base/evaluate/__init__.py
--rw-r--r--   0 vandejer (1865779777) 296108113     1423 2023-05-05 10:18:55.000000 mlpype-0.4.0/mlpype/base/evaluate/base_evaluator.py
--rw-r--r--   0 vandejer (1865779777) 296108113     2385 2023-05-05 10:18:55.000000 mlpype-0.4.0/mlpype/base/evaluate/evaluator.py
-drwxr-xr-x   0 vandejer (1865779777) 296108113        0 2023-05-05 10:36:25.412011 mlpype-0.4.0/mlpype/base/experiment/
--rw-r--r--   0 vandejer (1865779777) 296108113       35 2022-08-15 14:03:32.000000 mlpype-0.4.0/mlpype/base/experiment/__init__.py
--rw-r--r--   0 vandejer (1865779777) 296108113     8844 2023-05-05 10:18:55.000000 mlpype-0.4.0/mlpype/base/experiment/argument_parsing.py
--rw-r--r--   0 vandejer (1865779777) 296108113    19172 2023-05-05 10:18:55.000000 mlpype-0.4.0/mlpype/base/experiment/experiment.py
-drwxr-xr-x   0 vandejer (1865779777) 296108113        0 2023-05-05 10:36:25.421246 mlpype-0.4.0/mlpype/base/logger/
--rw-r--r--   0 vandejer (1865779777) 296108113       86 2022-08-15 15:00:23.000000 mlpype-0.4.0/mlpype/base/logger/__init__.py
--rw-r--r--   0 vandejer (1865779777) 296108113     4159 2023-05-05 10:18:55.000000 mlpype-0.4.0/mlpype/base/logger/experiment_logger.py
--rw-r--r--   0 vandejer (1865779777) 296108113     1715 2022-12-16 16:16:55.000000 mlpype-0.4.0/mlpype/base/logger/local_logger.py
-drwxr-xr-x   0 vandejer (1865779777) 296108113        0 2023-05-05 10:36:25.423963 mlpype-0.4.0/mlpype/base/model/
--rw-r--r--   0 vandejer (1865779777) 296108113       25 2022-05-07 20:20:49.000000 mlpype-0.4.0/mlpype/base/model/__init__.py
--rw-r--r--   0 vandejer (1865779777) 296108113     5043 2023-05-05 10:18:55.000000 mlpype-0.4.0/mlpype/base/model/model.py
-drwxr-xr-x   0 vandejer (1865779777) 296108113        0 2023-05-05 10:36:25.441268 mlpype-0.4.0/mlpype/base/pipeline/
--rw-r--r--   0 vandejer (1865779777) 296108113      165 2022-12-16 14:17:05.000000 mlpype-0.4.0/mlpype/base/pipeline/__init__.py
--rw-r--r--   0 vandejer (1865779777) 296108113     1305 2022-07-14 14:13:42.000000 mlpype-0.4.0/mlpype/base/pipeline/operator.py
--rw-r--r--   0 vandejer (1865779777) 296108113     6152 2023-05-05 10:18:55.000000 mlpype-0.4.0/mlpype/base/pipeline/pipe.py
--rw-r--r--   0 vandejer (1865779777) 296108113     8683 2023-05-05 10:18:55.000000 mlpype-0.4.0/mlpype/base/pipeline/pipeline.py
--rw-r--r--   0 vandejer (1865779777) 296108113     9044 2023-05-05 10:18:55.000000 mlpype-0.4.0/mlpype/base/pipeline/type_checker.py
-drwxr-xr-x   0 vandejer (1865779777) 296108113        0 2023-05-05 10:36:25.443301 mlpype-0.4.0/mlpype/base/serialiser/
--rw-r--r--   0 vandejer (1865779777) 296108113       83 2022-08-15 14:14:49.000000 mlpype-0.4.0/mlpype/base/serialiser/__init__.py
--rw-r--r--   0 vandejer (1865779777) 296108113      777 2023-05-05 10:18:55.000000 mlpype-0.4.0/mlpype/base/serialiser/joblib_serialiser.py
--rw-r--r--   0 vandejer (1865779777) 296108113     1100 2023-04-17 20:12:33.000000 mlpype-0.4.0/mlpype/base/serialiser/serialiser.py
--rw-r--r--   0 vandejer (1865779777) 296108113      751 2023-05-05 10:18:55.000000 mlpype-0.4.0/mlpype/base/setup.py
-drwxr-xr-x   0 vandejer (1865779777) 296108113        0 2023-05-05 10:36:25.452886 mlpype-0.4.0/mlpype/base/utils/
--rw-r--r--   0 vandejer (1865779777) 296108113       99 2022-12-16 14:17:05.000000 mlpype-0.4.0/mlpype/base/utils/__init__.py
--rw-r--r--   0 vandejer (1865779777) 296108113      670 2022-06-17 13:54:28.000000 mlpype-0.4.0/mlpype/base/utils/parsing.py
--rw-r--r--   0 vandejer (1865779777) 296108113     6003 2023-01-04 17:44:13.000000 mlpype-0.4.0/mlpype/base/utils/workspace.py
-drwxr-xr-x   0 vandejer (1865779777) 296108113        0 2023-05-05 10:36:25.455982 mlpype-0.4.0/mlpype/fastapi/
--rw-r--r--   0 vandejer (1865779777) 296108113        0 2022-12-16 14:17:05.000000 mlpype-0.4.0/mlpype/fastapi/__init__.py
-drwxr-xr-x   0 vandejer (1865779777) 296108113        0 2023-05-05 10:36:25.462993 mlpype-0.4.0/mlpype/fastapi/deploy/
--rw-r--r--   0 vandejer (1865779777) 296108113       73 2023-05-05 10:18:55.000000 mlpype-0.4.0/mlpype/fastapi/deploy/__init__.py
--rw-r--r--   0 vandejer (1865779777) 296108113     4165 2023-05-05 10:18:55.000000 mlpype-0.4.0/mlpype/fastapi/deploy/app.py
-drwxr-xr-x   0 vandejer (1865779777) 296108113        0 2023-05-05 10:36:25.463886 mlpype-0.4.0/mlpype/fastapi/deploy/wheel/
--rw-r--r--   0 vandejer (1865779777) 296108113      695 2023-05-05 10:18:55.000000 mlpype-0.4.0/mlpype/fastapi/deploy/wheel/helpers.py
--rw-r--r--   0 vandejer (1865779777) 296108113      216 2023-05-05 10:18:55.000000 mlpype-0.4.0/mlpype/fastapi/deploy/wheel_extension.py
--rw-r--r--   0 vandejer (1865779777) 296108113      537 2023-05-05 10:18:55.000000 mlpype-0.4.0/mlpype/fastapi/setup.py
-drwxr-xr-x   0 vandejer (1865779777) 296108113        0 2023-05-05 10:36:25.474578 mlpype-0.4.0/mlpype/hyperopt/
--rw-r--r--   0 vandejer (1865779777) 296108113       42 2022-12-16 14:17:05.000000 mlpype-0.4.0/mlpype/hyperopt/__init__.py
--rw-r--r--   0 vandejer (1865779777) 296108113     8355 2023-05-05 10:18:55.000000 mlpype-0.4.0/mlpype/hyperopt/optimise.py
--rw-r--r--   0 vandejer (1865779777) 296108113      492 2023-05-05 10:18:55.000000 mlpype-0.4.0/mlpype/hyperopt/setup.py
-drwxr-xr-x   0 vandejer (1865779777) 296108113        0 2023-05-05 10:36:25.477430 mlpype-0.4.0/mlpype/mlflow/
--rw-r--r--   0 vandejer (1865779777) 296108113        0 2022-12-16 14:17:05.000000 mlpype-0.4.0/mlpype/mlflow/__init__.py
-drwxr-xr-x   0 vandejer (1865779777) 296108113        0 2023-05-05 10:36:25.483201 mlpype-0.4.0/mlpype/mlflow/deploy/
--rw-r--r--   0 vandejer (1865779777) 296108113       57 2022-12-16 14:17:05.000000 mlpype-0.4.0/mlpype/mlflow/deploy/__init__.py
--rw-r--r--   0 vandejer (1865779777) 296108113     1874 2023-05-05 10:18:55.000000 mlpype-0.4.0/mlpype/mlflow/deploy/load_experiment.py
-drwxr-xr-x   0 vandejer (1865779777) 296108113        0 2023-05-05 10:36:25.488465 mlpype-0.4.0/mlpype/mlflow/logger/
--rw-r--r--   0 vandejer (1865779777) 296108113       40 2022-12-16 14:17:05.000000 mlpype-0.4.0/mlpype/mlflow/logger/__init__.py
--rw-r--r--   0 vandejer (1865779777) 296108113     5477 2023-05-05 10:18:55.000000 mlpype-0.4.0/mlpype/mlflow/logger/mlflow_logger.py
--rw-r--r--   0 vandejer (1865779777) 296108113      512 2023-05-05 10:18:55.000000 mlpype-0.4.0/mlpype/mlflow/setup.py
-drwxr-xr-x   0 vandejer (1865779777) 296108113        0 2023-05-05 10:36:25.495395 mlpype-0.4.0/mlpype/sklearn/
--rw-r--r--   0 vandejer (1865779777) 296108113        0 2022-07-12 21:11:23.000000 mlpype-0.4.0/mlpype/sklearn/__init__.py
-drwxr-xr-x   0 vandejer (1865779777) 296108113        0 2023-05-05 10:36:25.506394 mlpype-0.4.0/mlpype/sklearn/data/
--rw-r--r--   0 vandejer (1865779777) 296108113      119 2023-04-16 08:53:11.000000 mlpype-0.4.0/mlpype/sklearn/data/__init__.py
--rw-r--r--   0 vandejer (1865779777) 296108113      743 2023-05-05 10:18:55.000000 mlpype-0.4.0/mlpype/sklearn/data/data_frame_source.py
--rw-r--r--   0 vandejer (1865779777) 296108113       81 2022-12-16 16:16:55.000000 mlpype-0.4.0/mlpype/sklearn/data/sklearn_data.py
--rw-r--r--   0 vandejer (1865779777) 296108113     1206 2023-05-05 10:18:55.000000 mlpype-0.4.0/mlpype/sklearn/data/sql_source.py
-drwxr-xr-x   0 vandejer (1865779777) 296108113        0 2023-05-05 10:36:25.520938 mlpype-0.4.0/mlpype/sklearn/model/
--rw-r--r--   0 vandejer (1865779777) 296108113      214 2022-12-16 14:17:05.000000 mlpype-0.4.0/mlpype/sklearn/model/__init__.py
--rw-r--r--   0 vandejer (1865779777) 296108113      313 2023-05-05 10:18:55.000000 mlpype-0.4.0/mlpype/sklearn/model/linear_regression_model.py
--rw-r--r--   0 vandejer (1865779777) 296108113      323 2023-05-05 10:18:55.000000 mlpype-0.4.0/mlpype/sklearn/model/logistic_regression_model.py
--rw-r--r--   0 vandejer (1865779777) 296108113      443 2023-05-05 10:18:55.000000 mlpype-0.4.0/mlpype/sklearn/model/sklearn_base_type.py
--rw-r--r--   0 vandejer (1865779777) 296108113     4000 2023-05-05 10:18:55.000000 mlpype-0.4.0/mlpype/sklearn/model/sklearn_model.py
-drwxr-xr-x   0 vandejer (1865779777) 296108113        0 2023-05-05 10:36:25.532336 mlpype-0.4.0/mlpype/sklearn/pipeline/
--rw-r--r--   0 vandejer (1865779777) 296108113      100 2022-12-16 14:17:05.000000 mlpype-0.4.0/mlpype/sklearn/pipeline/__init__.py
--rw-r--r--   0 vandejer (1865779777) 296108113     3499 2023-05-05 10:18:55.000000 mlpype-0.4.0/mlpype/sklearn/pipeline/numpy_type_checker.py
--rw-r--r--   0 vandejer (1865779777) 296108113     3891 2023-05-05 10:18:55.000000 mlpype-0.4.0/mlpype/sklearn/pipeline/pandas_type_checker.py
--rw-r--r--   0 vandejer (1865779777) 296108113      533 2023-05-05 10:18:55.000000 mlpype-0.4.0/mlpype/sklearn/setup.py
-drwxr-xr-x   0 vandejer (1865779777) 296108113        0 2023-05-05 10:36:25.534885 mlpype-0.4.0/mlpype/spark/
--rw-r--r--   0 vandejer (1865779777) 296108113        0 2022-12-16 14:17:05.000000 mlpype-0.4.0/mlpype/spark/__init__.py
-drwxr-xr-x   0 vandejer (1865779777) 296108113        0 2023-05-05 10:36:25.547334 mlpype-0.4.0/mlpype/spark/data/
--rw-r--r--   0 vandejer (1865779777) 296108113      143 2022-12-16 14:17:05.000000 mlpype-0.4.0/mlpype/spark/data/__init__.py
--rw-r--r--   0 vandejer (1865779777) 296108113      833 2023-05-05 10:18:55.000000 mlpype-0.4.0/mlpype/spark/data/spark_data_frame_source.py
--rw-r--r--   0 vandejer (1865779777) 296108113     1098 2023-05-05 10:18:55.000000 mlpype-0.4.0/mlpype/spark/data/spark_read.py
--rw-r--r--   0 vandejer (1865779777) 296108113      976 2023-05-05 10:18:55.000000 mlpype-0.4.0/mlpype/spark/data/spark_sql_source.py
-drwxr-xr-x   0 vandejer (1865779777) 296108113        0 2023-05-05 10:36:25.553743 mlpype-0.4.0/mlpype/spark/evaluate/
--rw-r--r--   0 vandejer (1865779777) 296108113       44 2023-01-20 12:18:51.000000 mlpype-0.4.0/mlpype/spark/evaluate/__init__.py
--rw-r--r--   0 vandejer (1865779777) 296108113     2578 2023-05-05 10:18:55.000000 mlpype-0.4.0/mlpype/spark/evaluate/spark_evaluator.py
-drwxr-xr-x   0 vandejer (1865779777) 296108113        0 2023-05-05 10:36:25.562577 mlpype-0.4.0/mlpype/spark/model/
--rw-r--r--   0 vandejer (1865779777) 296108113       85 2022-12-16 14:17:05.000000 mlpype-0.4.0/mlpype/spark/model/__init__.py
--rw-r--r--   0 vandejer (1865779777) 296108113      301 2023-05-05 10:18:55.000000 mlpype-0.4.0/mlpype/spark/model/linear_spark_model.py
--rw-r--r--   0 vandejer (1865779777) 296108113     6953 2023-05-05 10:18:55.000000 mlpype-0.4.0/mlpype/spark/model/spark_model.py
-drwxr-xr-x   0 vandejer (1865779777) 296108113        0 2023-05-05 10:36:25.568664 mlpype-0.4.0/mlpype/spark/pipeline/
--rw-r--r--   0 vandejer (1865779777) 296108113       83 2022-12-16 14:17:05.000000 mlpype-0.4.0/mlpype/spark/pipeline/__init__.py
--rw-r--r--   0 vandejer (1865779777) 296108113     3857 2023-05-05 10:18:55.000000 mlpype-0.4.0/mlpype/spark/pipeline/spark_pipe.py
--rw-r--r--   0 vandejer (1865779777) 296108113     4660 2023-05-05 10:18:55.000000 mlpype-0.4.0/mlpype/spark/pipeline/spark_type_checker.py
-drwxr-xr-x   0 vandejer (1865779777) 296108113        0 2023-05-05 10:36:25.575365 mlpype-0.4.0/mlpype/spark/serialisation/
--rw-r--r--   0 vandejer (1865779777) 296108113       46 2022-12-16 14:17:05.000000 mlpype-0.4.0/mlpype/spark/serialisation/__init__.py
--rw-r--r--   0 vandejer (1865779777) 296108113     4850 2023-05-05 10:18:55.000000 mlpype-0.4.0/mlpype/spark/serialisation/spark_serialiser.py
--rw-r--r--   0 vandejer (1865779777) 296108113      715 2023-05-05 10:18:55.000000 mlpype-0.4.0/mlpype/spark/setup.py
-drwxr-xr-x   0 vandejer (1865779777) 296108113        0 2023-05-05 10:36:25.579294 mlpype-0.4.0/mlpype/tensorflow/
--rw-r--r--   0 vandejer (1865779777) 296108113        0 2022-12-16 14:17:05.000000 mlpype-0.4.0/mlpype/tensorflow/__init__.py
-drwxr-xr-x   0 vandejer (1865779777) 296108113        0 2023-05-05 10:36:25.582327 mlpype-0.4.0/mlpype/tensorflow/data/
--rw-r--r--   0 vandejer (1865779777) 296108113       40 2022-12-16 14:17:05.000000 mlpype-0.4.0/mlpype/tensorflow/data/__init__.py
--rw-r--r--   0 vandejer (1865779777) 296108113      755 2023-05-05 10:18:55.000000 mlpype-0.4.0/mlpype/tensorflow/data/tensor_source.py
-drwxr-xr-x   0 vandejer (1865779777) 296108113        0 2023-05-05 10:36:25.585452 mlpype-0.4.0/mlpype/tensorflow/model/
--rw-r--r--   0 vandejer (1865779777) 296108113      118 2023-05-05 10:27:52.000000 mlpype-0.4.0/mlpype/tensorflow/model/__init__.py
--rw-r--r--   0 vandejer (1865779777) 296108113     5296 2023-05-05 10:29:06.000000 mlpype-0.4.0/mlpype/tensorflow/model/keras_pype_model.py
--rw-r--r--   0 vandejer (1865779777) 296108113     1396 2023-05-05 10:18:55.000000 mlpype-0.4.0/mlpype/tensorflow/model/mlp_keras.py
--rw-r--r--   0 vandejer (1865779777) 296108113      304 2023-05-05 10:29:42.000000 mlpype-0.4.0/mlpype/tensorflow/model/mlp_pype_model.py
-drwxr-xr-x   0 vandejer (1865779777) 296108113        0 2023-05-05 10:36:25.592327 mlpype-0.4.0/mlpype/tensorflow/pipeline/
--rw-r--r--   0 vandejer (1865779777) 296108113       50 2022-12-16 14:17:05.000000 mlpype-0.4.0/mlpype/tensorflow/pipeline/__init__.py
--rw-r--r--   0 vandejer (1865779777) 296108113     3681 2023-05-05 10:18:55.000000 mlpype-0.4.0/mlpype/tensorflow/pipeline/tensor_checker.py
--rw-r--r--   0 vandejer (1865779777) 296108113      623 2023-05-05 10:18:55.000000 mlpype-0.4.0/mlpype/tensorflow/setup.py
-drwxr-xr-x   0 vandejer (1865779777) 296108113        0 2023-05-05 10:36:25.596985 mlpype-0.4.0/mlpype/xgboost/
--rw-r--r--   0 vandejer (1865779777) 296108113        0 2023-01-20 13:01:48.000000 mlpype-0.4.0/mlpype/xgboost/__init__.py
-drwxr-xr-x   0 vandejer (1865779777) 296108113        0 2023-05-05 10:36:25.604378 mlpype-0.4.0/mlpype/xgboost/model/
--rw-r--r--   0 vandejer (1865779777) 296108113      100 2022-12-16 14:17:05.000000 mlpype-0.4.0/mlpype/xgboost/model/__init__.py
--rw-r--r--   0 vandejer (1865779777) 296108113      802 2023-05-05 10:18:55.000000 mlpype-0.4.0/mlpype/xgboost/model/xgboost_classifier.py
--rw-r--r--   0 vandejer (1865779777) 296108113      794 2023-05-05 10:18:55.000000 mlpype-0.4.0/mlpype/xgboost/model/xgboost_regressor.py
--rw-r--r--   0 vandejer (1865779777) 296108113      504 2023-05-05 10:18:55.000000 mlpype-0.4.0/mlpype/xgboost/setup.py
-drwxr-xr-x   0 vandejer (1865779777) 296108113        0 2023-05-05 10:36:25.369770 mlpype-0.4.0/mlpype.egg-info/
--rw-r--r--   0 vandejer (1865779777) 296108113     5741 2023-05-05 10:36:25.000000 mlpype-0.4.0/mlpype.egg-info/PKG-INFO
--rw-r--r--   0 vandejer (1865779777) 296108113     3578 2023-05-05 10:36:25.000000 mlpype-0.4.0/mlpype.egg-info/SOURCES.txt
--rw-r--r--   0 vandejer (1865779777) 296108113        1 2023-05-05 10:36:25.000000 mlpype-0.4.0/mlpype.egg-info/dependency_links.txt
--rw-r--r--   0 vandejer (1865779777) 296108113        7 2023-05-05 10:36:25.000000 mlpype-0.4.0/mlpype.egg-info/top_level.txt
--rw-r--r--   0 vandejer (1865779777) 296108113     1185 2023-05-05 10:18:55.000000 mlpype-0.4.0/pyproject.toml
--rw-r--r--   0 vandejer (1865779777) 296108113      190 2023-05-05 10:36:25.608334 mlpype-0.4.0/setup.cfg
--rw-r--r--   0 vandejer (1865779777) 296108113      298 2023-05-05 10:18:55.000000 mlpype-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:46:41.547265 mlpype-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-20 16:43:35.000000 mlpype-0.4.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-06-20 16:46:41.547265 mlpype-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-06-20 16:43:35.000000 mlpype-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:46:41.507262 mlpype-0.4.1/mlpype/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:46:41.511262 mlpype-0.4.1/mlpype/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/base/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:46:41.511262 mlpype-0.4.1/mlpype/base/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/base/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/base/data/data_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/base/data/data_sink.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/base/data/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/base/data/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:46:41.515263 mlpype-0.4.1/mlpype/base/deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/base/deploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/base/deploy/inference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:46:41.515263 mlpype-0.4.1/mlpype/base/deploy/wheel/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/base/deploy/wheel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/base/deploy/wheel/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/base/deploy/wheel/extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:46:41.515263 mlpype-0.4.1/mlpype/base/deploy/wheel/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/base/deploy/wheel/helpers/setup_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/base/deploy/wheel/helpers/wheel_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/base/deploy/wheel/wheel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:46:41.519263 mlpype-0.4.1/mlpype/base/evaluate/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/base/evaluate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/base/evaluate/base_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/base/evaluate/evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:46:41.519263 mlpype-0.4.1/mlpype/base/experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/base/experiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8844 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/base/experiment/argument_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19171 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/base/experiment/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:46:41.519263 mlpype-0.4.1/mlpype/base/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/base/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/base/logger/experiment_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/base/logger/local_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:46:41.519263 mlpype-0.4.1/mlpype/base/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/base/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/base/model/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:46:41.523263 mlpype-0.4.1/mlpype/base/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/base/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/base/pipeline/operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/base/pipeline/pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8683 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/base/pipeline/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9044 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/base/pipeline/type_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:46:41.523263 mlpype-0.4.1/mlpype/base/serialiser/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/base/serialiser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/base/serialiser/joblib_serialiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/base/serialiser/serialiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/base/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:46:41.523263 mlpype-0.4.1/mlpype/base/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/base/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/base/utils/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/base/utils/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:46:41.527263 mlpype-0.4.1/mlpype/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/fastapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:46:41.527263 mlpype-0.4.1/mlpype/fastapi/deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/fastapi/deploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/fastapi/deploy/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:46:41.527263 mlpype-0.4.1/mlpype/fastapi/deploy/wheel/
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/fastapi/deploy/wheel/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/fastapi/deploy/wheel_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/fastapi/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:46:41.527263 mlpype-0.4.1/mlpype/hyperopt/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/hyperopt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/hyperopt/optimise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/hyperopt/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:46:41.527263 mlpype-0.4.1/mlpype/mlflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/mlflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:46:41.531264 mlpype-0.4.1/mlpype/mlflow/deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/mlflow/deploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/mlflow/deploy/load_experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:46:41.531264 mlpype-0.4.1/mlpype/mlflow/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/mlflow/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/mlflow/logger/mlflow_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/mlflow/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:46:41.531264 mlpype-0.4.1/mlpype/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/sklearn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:46:41.531264 mlpype-0.4.1/mlpype/sklearn/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/sklearn/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/sklearn/data/data_frame_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/sklearn/data/sklearn_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/sklearn/data/sql_source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:46:41.535264 mlpype-0.4.1/mlpype/sklearn/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/sklearn/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/sklearn/model/linear_regression_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/sklearn/model/logistic_regression_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/sklearn/model/sklearn_base_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/sklearn/model/sklearn_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:46:41.535264 mlpype-0.4.1/mlpype/sklearn/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/sklearn/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/sklearn/pipeline/numpy_type_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/sklearn/pipeline/pandas_type_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/sklearn/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:46:41.535264 mlpype-0.4.1/mlpype/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/spark/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:46:41.539264 mlpype-0.4.1/mlpype/spark/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/spark/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/spark/data/spark_data_frame_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/spark/data/spark_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/spark/data/spark_sql_source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:46:41.539264 mlpype-0.4.1/mlpype/spark/evaluate/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/spark/evaluate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/spark/evaluate/spark_evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:46:41.539264 mlpype-0.4.1/mlpype/spark/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/spark/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/spark/model/linear_spark_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6953 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/spark/model/spark_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:46:41.539264 mlpype-0.4.1/mlpype/spark/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/spark/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/spark/pipeline/spark_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/spark/pipeline/spark_type_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:46:41.539264 mlpype-0.4.1/mlpype/spark/serialisation/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/spark/serialisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/spark/serialisation/spark_serialiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/spark/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:46:41.543265 mlpype-0.4.1/mlpype/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/tensorflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:46:41.543265 mlpype-0.4.1/mlpype/tensorflow/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/tensorflow/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/tensorflow/data/tensor_source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:46:41.543265 mlpype-0.4.1/mlpype/tensorflow/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/tensorflow/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/tensorflow/model/keras_pype_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/tensorflow/model/mlp_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/tensorflow/model/mlp_pype_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:46:41.543265 mlpype-0.4.1/mlpype/tensorflow/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/tensorflow/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/tensorflow/pipeline/tensor_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/tensorflow/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:46:41.547265 mlpype-0.4.1/mlpype/xgboost/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/xgboost/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:46:41.547265 mlpype-0.4.1/mlpype/xgboost/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/xgboost/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/xgboost/model/xgboost_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/xgboost/model/xgboost_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-20 16:43:35.000000 mlpype-0.4.1/mlpype/xgboost/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:46:41.511262 mlpype-0.4.1/mlpype.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-06-20 16:46:41.000000 mlpype-0.4.1/mlpype.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-06-20 16:46:41.000000 mlpype-0.4.1/mlpype.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:46:41.000000 mlpype-0.4.1/mlpype.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 16:46:41.000000 mlpype-0.4.1/mlpype.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-20 16:43:35.000000 mlpype-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-20 16:46:41.547265 mlpype-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-20 16:43:35.000000 mlpype-0.4.1/setup.py
```

### Comparing `mlpype-0.4.0/LICENSE.txt` & `mlpype-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.0/PKG-INFO` & `mlpype-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpype
-Version: 0.4.0
+Version: 0.4.1
 Summary: Standardise model training across libraries
 Home-page: https://github.com/jeroenvdhoven/mlpype
 Author: Jeroen van den Hoven
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `mlpype-0.4.0/README.md` & `mlpype-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.0/mlpype/base/data/data_catalog.py` & `mlpype-0.4.1/mlpype/base/data/data_catalog.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import importlib
 from pathlib import Path
-from typing import Any, Callable, Dict, TypeVar, Union
+from typing import Any, Callable, Dict, Optional, TypeVar, Union
 
 import yaml
+from jinja2 import Template
 
 from mlpype.base.data.data_source import DataSource
 from mlpype.base.data.dataset import DataSet
 
 Data = TypeVar("Data")
 
 
 class DataCatalog(Dict[str, DataSource[Data]]):
     """A collection of DataSources that together form a DataSet when loaded."""
 
-    def read(self) -> DataSet[Data]:
+    def read(self) -> DataSet:
         """Read all DataSources and generate a DataSet.
 
         Names of DataSources are preserved when loading the data.
 
         Returns:
-            DataSet[Data]: The DataSet constructed from the DataSources.
+            DataSet: The DataSet constructed from the DataSources.
         """
         return DataSet.from_dict({name: data.read() for name, data in self.items()})
 
     def __str__(self, indents: int = 0) -> str:
         """Create string representation of this DataCatalog.
 
         Args:
@@ -31,23 +32,34 @@
 
         Returns:
             str: A string representation of this DataCatalog.
         """
         tab = "\t" * indents
         return "\n".join([f"{tab}{name}: {source}" for name, source in self.items()])
 
+    def read_one(self, name: str) -> Data:
+        """Read a particular dataset from this DataCatalog.
+
+        Args:
+            name (str): The name of the dataset to read.
+
+        Returns:
+            Data: The data returned by the DataSource tied to `name`.
+        """
+        return self[name].read()
+
     @classmethod
-    def from_yaml(cls, path: Union[str, Path]) -> "DataCatalog":
-        """Read a catalog in from a configuraiton YAML file.
+    def from_yaml(cls, path: Union[str, Path], parameters: Optional[Dict[str, Any]] = None) -> "DataCatalog":
+        """Read a catalog in from a configuration YAML file.
 
         We expect the following format:
         ```
         <dataset name>:
             callable: <python path to class, method on a class, or function.
-                Should produce a DataCatalog.
+                Should produce a DataSource.
             args:
                 <name of argument>: <value>
         ```
 
         Values can be a plain value (like string, bool, etc) or a complex object.
         These will follow the same format as the callable-args structure of the
         DataSource's, but don't need to be DataSource's. e.g.:
@@ -70,68 +82,109 @@
 
         To use a method on a class, use `path.to.class:function`. This will only work for
         static or class methods.
 
         For security reasons, please make sure you trust any YAML file you read using this
         method! It will lead to code execution based on the imports, which can be abused.
 
+        Parameters from the optional dictionary will be used for Jinja templating of
+        strings in any of the arguments. To ensure non-string values are properly parsed,
+        make sure they aren't surrounded by quotation marks in the YAML.
+
         Args:
             path (Union[str, Path]): The path to the YAML file.
+            parameters (Optional[Dict[str, Any]]): an optional set of parameters to be used to
+                do jinja templating on the YAML file's strings.
 
         Returns:
             DataCatalog: A DataCatalog with DataSources based on the YAML file.
         """
         data_sources = {}
+        if parameters is None:
+            parameters = {}
 
         path = Path(path)
         with open(path, "r") as f:
-            configuration = yaml.safe_load(f)
+            contents = f.read()
+
+            parsed_contents = Template(contents).render(parameters)
+            configuration = yaml.safe_load(parsed_contents)
         assert isinstance(configuration, dict), "Cannot process YAML as DataCatalog: should be a dictionary."
 
-        for dataset_name, parameters in configuration.items():
-            dataset = cls._parse_object(parameters)
+        for dataset_name, dataset_params in configuration.items():
+            dataset = cls._parse_object(dataset_params)
             assert isinstance(
                 dataset, DataSource
             ), "Please make sure objects in your DataCatalog only translate to DataSources."
             data_sources[dataset_name] = dataset
         return DataCatalog(**data_sources)
 
     @classmethod
     def _parse_object(cls, dct: Dict[str, Any]) -> Any:
+        """Recursively parse a complex dictionary to create objects.
+
+        Args:
+            dct (Dict[str, Any]): A dictionary containing 2 fields:
+                - callable: A python path to a class or static/class method on a class.
+                    Used to initiate the object.
+                - args: a dictionary of args to instantiate the object with or call the
+                    method with. Can be another complex object.
+
+        Returns:
+            Any: The object returned by calling `callable`
+        """
         assert cls._is_valid_parseable_object(
             dct
-        ), "DataCatalog: any dictionary parsed should have a `class` and `args` entry."
+        ), "DataCatalog: any dictionary parsed should have a `callable` and `args` entry."
 
         callable_ = cls._load_class(dct["callable"])
         args = dct["args"]
         assert isinstance(args, dict), "Arguments to a parseable object should be a dict."
 
         # Parse arguments recursively
         parsed_args = {}
         for arg_name, arg_value in args.items():
-            # print(f"{arg_name}: {arg_value}")
             if cls._is_valid_parseable_object(arg_value):
-                parsed_args[arg_name] = cls._parse_object(arg_value)
+                parsed_value = cls._parse_object(arg_value)
             else:
-                parsed_args[arg_name] = arg_value
+                parsed_value = arg_value
+
+            parsed_args[arg_name] = parsed_value
 
         return callable_(**parsed_args)
 
     @staticmethod
     def _load_class(full_path: str) -> Callable:
+        """Load a callable from a Python import path.
+
+        Supported functionality includes:
+        - Importing a class, e.g. pandas.DataFrame.
+        - Importing a static / class method, e.g. ds_range_allocation.data.catalog.DataCatalog:from_yaml
+
+        Args:
+            full_path (str): The path leading to the class or function to import.
+
+        Returns:
+            Callable: The class or function described in the `full_path` variable.
+        """
+        # check if we need to import a method.
         method_split = full_path.split(":")
         assert len(method_split) <= 2, "We do not accept paths with more than 1 `:`"
         callable_path = method_split[0]
 
+        # for importing we need to split out the last part of the string.
         split_path = callable_path.split(".")
         module_path = ".".join(split_path[:-1])
+        class_path = split_path[-1]
 
+        # Import the module and get the class.
         module = importlib.import_module(module_path)
-        callable = getattr(module, split_path[-1])
+        callable = getattr(module, class_path)
 
+        # Return the method if that was requested, otherwise just return the class.
         if len(method_split) > 1:
             return getattr(callable, method_split[1])
         else:
             return callable
 
     @staticmethod
     def _is_valid_parseable_object(dct: Dict[str, Any]) -> bool:
```

### Comparing `mlpype-0.4.0/mlpype/base/data/dataset.py` & `mlpype-0.4.1/mlpype/base/data/dataset.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.0/mlpype/base/deploy/inference.py` & `mlpype-0.4.1/mlpype/base/deploy/inference.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.0/mlpype/base/deploy/wheel/builder.py` & `mlpype-0.4.1/mlpype/base/deploy/wheel/builder.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.0/mlpype/base/deploy/wheel/extensions.py` & `mlpype-0.4.1/mlpype/base/deploy/wheel/extensions.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.0/mlpype/base/deploy/wheel/helpers/setup_template.py` & `mlpype-0.4.1/mlpype/base/deploy/wheel/helpers/setup_template.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.0/mlpype/base/deploy/wheel/wheel.py` & `mlpype-0.4.1/mlpype/base/deploy/wheel/wheel.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.0/mlpype/base/evaluate/base_evaluator.py` & `mlpype-0.4.1/mlpype/base/evaluate/base_evaluator.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.0/mlpype/base/evaluate/evaluator.py` & `mlpype-0.4.1/mlpype/base/evaluate/evaluator.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.0/mlpype/base/experiment/argument_parsing.py` & `mlpype-0.4.1/mlpype/base/experiment/argument_parsing.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.0/mlpype/base/experiment/experiment.py` & `mlpype-0.4.1/mlpype/base/experiment/experiment.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
             for ds in datasets.values():
                 self.input_type_checker.transform(ds)
 
             self.logger.info("Fit pipeline")
             self.pipeline.fit(datasets["train"])
 
             self.logger.info("Transform data")
-            transformed = {name: self.pipeline.transform(data, is_inference=False) for name, data in datasets.items()}
+            transformed = {name: self.pipeline.transform(data, is_inference=True) for name, data in datasets.items()}
 
             self.logger.info("Fit model")
             self.model.fit(transformed["train"])
 
             self.logger.info("Evaluate model")
             metrics = {name: self.evaluator.evaluate(self.model, data) for name, data in transformed.items()}
```

### Comparing `mlpype-0.4.0/mlpype/base/logger/experiment_logger.py` & `mlpype-0.4.1/mlpype/base/logger/experiment_logger.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.0/mlpype/base/logger/local_logger.py` & `mlpype-0.4.1/mlpype/base/logger/local_logger.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.0/mlpype/base/model/model.py` & `mlpype-0.4.1/mlpype/base/model/model.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.0/mlpype/base/pipeline/operator.py` & `mlpype-0.4.1/mlpype/base/pipeline/operator.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.0/mlpype/base/pipeline/pipe.py` & `mlpype-0.4.1/mlpype/base/pipeline/pipe.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.0/mlpype/base/pipeline/pipeline.py` & `mlpype-0.4.1/mlpype/base/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.0/mlpype/base/pipeline/type_checker.py` & `mlpype-0.4.1/mlpype/base/pipeline/type_checker.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.0/mlpype/base/serialiser/joblib_serialiser.py` & `mlpype-0.4.1/mlpype/base/serialiser/joblib_serialiser.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.0/mlpype/base/serialiser/serialiser.py` & `mlpype-0.4.1/mlpype/base/serialiser/serialiser.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.0/mlpype/base/setup.py` & `mlpype-0.4.1/mlpype/base/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,22 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == "__main__":
-    version = "0.4.0"
+    version = "0.4.1"
 
     dev_deps = ["pre-commit", "build==0.8.0", "pypiserver==1.5.1", "twine==4.0.1", "pdoc==13.1.0"]
     test_deps = ["pytest", "pytest-cov"]
-    deps = [f"mlpype=={version}", "docstring_parser>=0.14.1", "pydantic>=1.9.1", "joblib>=1.1.0", "PyYAML==6.0"]
+    deps = [
+        f"mlpype=={version}",
+        "docstring_parser>=0.14.1",
+        "pydantic>=1.9.1",
+        "joblib>=1.1.0",
+        "PyYAML==6.0",
+        "jinja2==3.1.2",
+    ]
     strict_deps = [s.replace(">=", "==") for s in deps]
 
     setup(
         name="mlpype-base",
         install_requires=deps,
         extras_require={
             "dev": strict_deps + dev_deps + test_deps,
```

### Comparing `mlpype-0.4.0/mlpype/base/utils/parsing.py` & `mlpype-0.4.1/mlpype/base/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.0/mlpype/base/utils/workspace.py` & `mlpype-0.4.1/mlpype/base/utils/workspace.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.0/mlpype/fastapi/deploy/app.py` & `mlpype-0.4.1/mlpype/fastapi/deploy/app.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.0/mlpype/fastapi/deploy/wheel/helpers.py` & `mlpype-0.4.1/mlpype/fastapi/deploy/wheel/helpers.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.0/mlpype/fastapi/setup.py` & `mlpype-0.4.1/mlpype/fastapi/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List
 
 from setuptools import find_namespace_packages, setup
 
 if __name__ == "__main__":
-    version = "0.4.0"
+    version = "0.4.1"
     deps: List[str] = [f"mlpype-base=={version}", "fastapi>=0.79.0"]
     dev_deps = ["uvicorn==0.18.2"]
     strict_deps = [s.replace(">=", "==") for s in deps]
 
     setup(
         name="mlpype-fastapi",
         install_requires=deps,
```

### Comparing `mlpype-0.4.0/mlpype/hyperopt/optimise.py` & `mlpype-0.4.1/mlpype/hyperopt/optimise.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.0/mlpype/mlflow/deploy/load_experiment.py` & `mlpype-0.4.1/mlpype/mlflow/deploy/load_experiment.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.0/mlpype/mlflow/logger/mlflow_logger.py` & `mlpype-0.4.1/mlpype/mlflow/logger/mlflow_logger.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.0/mlpype/mlflow/setup.py` & `mlpype-0.4.1/mlpype/mlflow/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == "__main__":
-    version = "0.4.0"
+    version = "0.4.1"
 
     deps = [
         f"mlpype-base=={version}",
         "mlflow>=1.28.0, <2.0",
         "GitPython>=3.1.27",
     ]
     strict_deps = [s.replace(">=", "==") for s in deps]
```

### Comparing `mlpype-0.4.0/mlpype/sklearn/data/data_frame_source.py` & `mlpype-0.4.1/mlpype/sklearn/data/data_frame_source.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.0/mlpype/sklearn/data/sql_source.py` & `mlpype-0.4.1/mlpype/sklearn/data/sql_source.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.0/mlpype/sklearn/model/sklearn_model.py` & `mlpype-0.4.1/mlpype/sklearn/model/sklearn_model.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.0/mlpype/sklearn/pipeline/numpy_type_checker.py` & `mlpype-0.4.1/mlpype/sklearn/pipeline/numpy_type_checker.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.0/mlpype/sklearn/pipeline/pandas_type_checker.py` & `mlpype-0.4.1/mlpype/sklearn/pipeline/pandas_type_checker.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.0/mlpype/sklearn/setup.py` & `mlpype-0.4.1/mlpype/sklearn/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == "__main__":
-    version = "0.4.0"
+    version = "0.4.1"
 
     deps = [
         f"mlpype-base=={version}",
         "numpy>=1.23.0",
         "scikit-learn>=1.1.1",
         "pandas>=1.4.3",
     ]
```

### Comparing `mlpype-0.4.0/mlpype/spark/data/spark_data_frame_source.py` & `mlpype-0.4.1/mlpype/spark/data/spark_data_frame_source.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.0/mlpype/spark/data/spark_read.py` & `mlpype-0.4.1/mlpype/spark/data/spark_read.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.0/mlpype/spark/data/spark_sql_source.py` & `mlpype-0.4.1/mlpype/spark/data/spark_sql_source.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.0/mlpype/spark/evaluate/spark_evaluator.py` & `mlpype-0.4.1/mlpype/spark/evaluate/spark_evaluator.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.0/mlpype/spark/model/spark_model.py` & `mlpype-0.4.1/mlpype/spark/model/spark_model.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.0/mlpype/spark/pipeline/spark_pipe.py` & `mlpype-0.4.1/mlpype/spark/pipeline/spark_pipe.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.0/mlpype/spark/pipeline/spark_type_checker.py` & `mlpype-0.4.1/mlpype/spark/pipeline/spark_type_checker.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.0/mlpype/spark/serialisation/spark_serialiser.py` & `mlpype-0.4.1/mlpype/spark/serialisation/spark_serialiser.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.0/mlpype/spark/setup.py` & `mlpype-0.4.1/mlpype/spark/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == "__main__":
-    version = "0.4.0"
+    version = "0.4.1"
 
     deps = [
         f"mlpype-base=={version}",
         # We will provide absolute no guarantees that our integration will work with
         # EVERY version of pyspark. This has been developed under pyspark==3.2.1.
         "pyspark>=3.2.1",
     ]
```

### Comparing `mlpype-0.4.0/mlpype/tensorflow/data/tensor_source.py` & `mlpype-0.4.1/mlpype/tensorflow/data/tensor_source.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.0/mlpype/tensorflow/model/keras_pype_model.py` & `mlpype-0.4.1/mlpype/tensorflow/model/keras_pype_model.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.0/mlpype/tensorflow/model/mlp_keras.py` & `mlpype-0.4.1/mlpype/tensorflow/model/mlp_keras.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.0/mlpype/tensorflow/pipeline/tensor_checker.py` & `mlpype-0.4.1/mlpype/tensorflow/pipeline/tensor_checker.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.0/mlpype/tensorflow/setup.py` & `mlpype-0.4.1/mlpype/tensorflow/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == "__main__":
-    version = "0.4.0"
+    version = "0.4.1"
 
     deps = [
         f"mlpype-base=={version}",
         # on mac, it is recommended to use conda/mamba or source to install tensorflow
         "tensorflow>=2.12",
         "numpy>=1.23.0",
         "protobuf>=3.20.3",
```

### Comparing `mlpype-0.4.0/mlpype/xgboost/model/xgboost_classifier.py` & `mlpype-0.4.1/mlpype/xgboost/model/xgboost_classifier.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.0/mlpype/xgboost/model/xgboost_regressor.py` & `mlpype-0.4.1/mlpype/xgboost/model/xgboost_regressor.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.0/mlpype.egg-info/PKG-INFO` & `mlpype-0.4.1/mlpype.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpype
-Version: 0.4.0
+Version: 0.4.1
 Summary: Standardise model training across libraries
 Home-page: https://github.com/jeroenvdhoven/mlpype
 Author: Jeroen van den Hoven
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `mlpype-0.4.0/mlpype.egg-info/SOURCES.txt` & `mlpype-0.4.1/mlpype.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.0/pyproject.toml` & `mlpype-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 name = "mlpype"
 authors = [
     {name = "Jeroen van den Hoven"},
 ]
 description = "Standardise model training across libraries"
 readme = "README.md"
 requires-python = ">=3.8"
-version = "0.4.0"
+version = "0.4.1"
 dynamic = ["license"]
 
 [tool.kedro]
 package_name = "data_cube_pipeline"
 project_name = "Data Cube Pipeline"
 project_version = "0.17.0"
```

