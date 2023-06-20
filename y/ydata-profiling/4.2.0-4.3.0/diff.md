# Comparing `tmp/ydata-profiling-4.2.0.tar.gz` & `tmp/ydata-profiling-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ydata-profiling-4.2.0.tar", last modified: Wed May 24 08:07:13 2023, max compression
+gzip compressed data, was "ydata-profiling-4.3.0.tar", last modified: Tue Jun 20 07:29:23 2023, max compression
```

## Comparing `ydata-profiling-4.2.0.tar` & `ydata-profiling-4.3.0.tar`

### file list

```diff
@@ -1,263 +1,264 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:07:13.900820 ydata-profiling-4.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    20736 2023-05-24 08:07:13.900820 ydata-profiling-4.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17440 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/requirements-spark.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 08:07:13.900820 ydata-profiling-4.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:07:13.852819 ydata-profiling-4.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:07:13.856819 ydata-profiling-4.2.0/src/pandas_profiling/
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/pandas_profiling/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:07:13.860819 ydata-profiling-4.2.0/src/ydata_profiling/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13025 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/compare_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)    12726 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/config_default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/config_minimal.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:07:13.860819 ydata-profiling-4.2.0/src/ydata_profiling/controller/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/controller/console.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/controller/pandas_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/expectations_report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:07:13.864819 ydata-profiling-4.2.0/src/ydata_profiling/model/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20409 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/correlations.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     6199 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/describe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/description.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/duplicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/expectation_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/missing.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/pairwise.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:07:13.868819 ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/correlations_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/dataframe_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/describe_boolean_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     9285 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/describe_categorical_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/describe_counts_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/describe_date_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/describe_file_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/describe_generic_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/describe_image_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/describe_numeric_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/describe_path_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/describe_supported_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/describe_text_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/describe_timeseries_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/describe_url_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/discretize_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/duplicates_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/imbalance_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/missing_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/sample_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/summary_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/table_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/utils_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:07:13.868819 ydata-profiling-4.2.0/src/ydata_profiling/model/spark/
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/spark/correlations_spark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/spark/dataframe_spark.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/spark/describe_boolean_spark.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/spark/describe_categorical_spark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/spark/describe_counts_spark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/spark/describe_date_spark.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/spark/describe_generic_spark.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/spark/describe_numeric_spark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/spark/describe_supported_spark.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/spark/describe_text_spark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/spark/duplicates_spark.py
--rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/spark/missing_spark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/spark/sample_spark.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/spark/summary_spark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/spark/table_spark.py
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/summarizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/summary_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/table.py
--rw-r--r--   0 runner    (1001) docker     (123)    11164 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/typeset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/typeset_relations.py
--rw-r--r--   0 runner    (1001) docker     (123)    19411 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/profile_report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:07:13.868819 ydata-profiling-4.2.0/src/ydata_profiling/report/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9093 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/formatters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:07:13.868819 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:07:13.872819 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/collapse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/container.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/correlation_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/dropdown.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/duplicate.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/frequency_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/frequency_table_small.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/html.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/image.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/item_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/renderable.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/root.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/table.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/toggle_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/variable_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:07:13.872819 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/flavours.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:07:13.876819 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/collapse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/container.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/correlation_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/dropdown.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/duplicate.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/frequency_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/frequency_table_small.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/html.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/image.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/root.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:07:13.876819 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:07:13.884820 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_constant.html
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_constant_length.html
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_duplicates.html
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_empty.html
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_high_cardinality.html
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_high_correlation.html
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_imbalance.html
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_infinite.html
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_missing.html
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_non_stationary.html
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_seasonal.html
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_skewed.html
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_truncated.html
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_type_date.html
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_uniform.html
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_unique.html
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_unsupported.html
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_zeros.html
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts.html
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/collapse.html
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/correlation_table.html
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/diagram.html
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/dropdown.html
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/duplicate.html
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/frequency_table.html
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/frequency_table_small.html
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/report.html
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/sample.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:07:13.884820 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/batch_grid.html
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/grid.html
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/list.html
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/named_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/sections.html
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/select.html
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/tabs.html
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/table.html
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/toggle_button.html
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/variable.html
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/variable_info.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:07:13.884820 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:07:13.888820 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    23409 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/bootstrap-theme.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   121200 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    37045 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   125618 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/cosmo.bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   127321 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/flatly.bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    97163 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/jquery-1.12.4.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/script.js
--rw-r--r--   0 runner    (1001) docker     (123)   127551 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/simplex.bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/style.css
--rw-r--r--   0 runner    (1001) docker     (123)   122851 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/united.bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/javascript.html
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/navigation.html
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/style.html
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/toggle_button.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/variable_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:07:13.888820 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/collapse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/container.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/correlation_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/dropdown.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/duplicate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/frequency_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/frequency_table_small.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/html.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/root.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/table.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/toggle_button.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/variable_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/frequency_table_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:07:13.892820 ydata-profiling-4.2.0/src/ydata_profiling/report/structure/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/structure/correlations.py
--rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/structure/overview.py
--rw-r--r--   0 runner    (1001) docker     (123)    14934 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/structure/report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:07:13.892820 ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_boolean.py
--rw-r--r--   0 runner    (1001) docker     (123)    17888 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_complex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6950 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     9487 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_real.py
--rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     9246 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/serialize_report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:07:13.896820 ydata-profiling-4.2.0/src/ydata_profiling/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/utils/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/utils/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/utils/imghdr_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/utils/notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/utils/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/utils/progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-24 08:07:13.000000 ydata-profiling-4.2.0/src/ydata_profiling/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:07:13.896820 ydata-profiling-4.2.0/src/ydata_profiling/visualisation/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/visualisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/visualisation/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/visualisation/missing.py
--rw-r--r--   0 runner    (1001) docker     (123)    29573 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/visualisation/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/visualisation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:07:13.860819 ydata-profiling-4.2.0/src/ydata_profiling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20736 2023-05-24 08:07:13.000000 ydata-profiling-4.2.0/src/ydata_profiling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14162 2023-05-24 08:07:13.000000 ydata-profiling-4.2.0/src/ydata_profiling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 08:07:13.000000 ydata-profiling-4.2.0/src/ydata_profiling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-24 08:07:13.000000 ydata-profiling-4.2.0/src/ydata_profiling.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-24 08:07:13.000000 ydata-profiling-4.2.0/src/ydata_profiling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-24 08:07:13.000000 ydata-profiling-4.2.0/src/ydata_profiling.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:07:13.896820 ydata-profiling-4.2.0/venv/
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/venv/spark.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:29:23.744413 ydata-profiling-4.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    21073 2023-06-20 07:29:23.744413 ydata-profiling-4.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17713 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/requirements-spark.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 07:29:23.744413 ydata-profiling-4.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:29:23.716413 ydata-profiling-4.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:29:23.716413 ydata-profiling-4.3.0/src/pandas_profiling/
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/pandas_profiling/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:29:23.720413 ydata-profiling-4.3.0/src/ydata_profiling/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13025 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/compare_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12726 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/config_default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/config_minimal.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:29:23.720413 ydata-profiling-4.3.0/src/ydata_profiling/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/controller/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/controller/pandas_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/expectations_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:29:23.720413 ydata-profiling-4.3.0/src/ydata_profiling/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20409 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/correlations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6199 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/describe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/description.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/duplicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/expectation_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/pairwise.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:29:23.724413 ydata-profiling-4.3.0/src/ydata_profiling/model/pandas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/pandas/correlations_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/pandas/dataframe_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/pandas/describe_boolean_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9285 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/pandas/describe_categorical_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/pandas/describe_counts_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/pandas/describe_date_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/pandas/describe_file_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/pandas/describe_generic_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/pandas/describe_image_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/pandas/describe_numeric_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/pandas/describe_path_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/pandas/describe_supported_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/pandas/describe_text_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/pandas/describe_timeseries_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/pandas/describe_url_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/pandas/discretize_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/pandas/duplicates_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/pandas/imbalance_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/pandas/missing_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/pandas/sample_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/pandas/summary_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/pandas/table_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/pandas/utils_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:29:23.724413 ydata-profiling-4.3.0/src/ydata_profiling/model/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/spark/correlations_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/spark/dataframe_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/spark/describe_boolean_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/spark/describe_categorical_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/spark/describe_counts_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/spark/describe_date_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/spark/describe_generic_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/spark/describe_numeric_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/spark/describe_supported_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/spark/describe_text_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/spark/duplicates_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/spark/missing_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/spark/sample_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/spark/summary_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/spark/table_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/summarizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/summary_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11595 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/typeset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/model/typeset_relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19411 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/profile_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:29:23.724413 ydata-profiling-4.3.0/src/ydata_profiling/report/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9093 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/formatters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:29:23.724413 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:29:23.728413 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/core/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/core/collapse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/core/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/core/correlation_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/core/dropdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/core/duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/core/frequency_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/core/frequency_table_small.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/core/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/core/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/core/item_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/core/renderable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/core/root.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/core/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/core/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/core/toggle_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/core/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/core/variable_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:29:23.728413 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/flavours.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:29:23.728413 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/collapse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/correlation_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/dropdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/frequency_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/frequency_table_small.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/root.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:29:23.732413 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:29:23.732413 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_constant.html
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_constant_length.html
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_duplicates.html
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_empty.html
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_high_cardinality.html
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_high_correlation.html
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_imbalance.html
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_infinite.html
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_missing.html
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_non_stationary.html
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_seasonal.html
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_skewed.html
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_truncated.html
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_type_date.html
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_uniform.html
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_unique.html
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_unsupported.html
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_zeros.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts.html
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/collapse.html
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/correlation_table.html
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/diagram.html
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/duplicate.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/frequency_table.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/frequency_table_small.html
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/report.html
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/sample.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:29:23.736413 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/batch_grid.html
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/grid.html
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/named_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/sections.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/select.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/tabs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/table.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/toggle_button.html
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/variable.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/variable_info.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:29:23.736413 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:29:23.736413 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    23409 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/bootstrap-theme.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   121200 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    37045 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   125618 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/cosmo.bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   127321 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/flatly.bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    97163 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/jquery-1.12.4.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/script.js
+-rw-r--r--   0 runner    (1001) docker     (123)   127551 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/simplex.bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/style.css
+-rw-r--r--   0 runner    (1001) docker     (123)   122851 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/united.bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/javascript.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/navigation.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/style.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/toggle_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/variable_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:29:23.740413 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/widget/
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/widget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/widget/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/widget/collapse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/widget/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/widget/correlation_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/widget/dropdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/widget/duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/widget/frequency_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/widget/frequency_table_small.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/widget/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/widget/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/widget/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/widget/root.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/widget/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/widget/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/widget/toggle_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/widget/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/widget/variable_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/frequency_table_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:29:23.740413 ydata-profiling-4.3.0/src/ydata_profiling/report/structure/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/structure/correlations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/structure/overview.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14934 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/structure/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:29:23.740413 ydata-profiling-4.3.0/src/ydata_profiling/report/structure/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/structure/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/structure/variables/render_boolean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17888 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/structure/variables/render_categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/structure/variables/render_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/structure/variables/render_complex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/structure/variables/render_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/structure/variables/render_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/structure/variables/render_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/structure/variables/render_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6950 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/structure/variables/render_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/structure/variables/render_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9487 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/structure/variables/render_real.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/structure/variables/render_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9246 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/structure/variables/render_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/report/structure/variables/render_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/serialize_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:29:23.744413 ydata-profiling-4.3.0/src/ydata_profiling/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/utils/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/utils/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/utils/imghdr_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/utils/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/utils/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/utils/progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/utils/versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-20 07:29:23.000000 ydata-profiling-4.3.0/src/ydata_profiling/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:29:23.744413 ydata-profiling-4.3.0/src/ydata_profiling/visualisation/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/visualisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/visualisation/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/visualisation/missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29580 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/visualisation/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/src/ydata_profiling/visualisation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:29:23.720413 ydata-profiling-4.3.0/src/ydata_profiling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21073 2023-06-20 07:29:23.000000 ydata-profiling-4.3.0/src/ydata_profiling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14200 2023-06-20 07:29:23.000000 ydata-profiling-4.3.0/src/ydata_profiling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 07:29:23.000000 ydata-profiling-4.3.0/src/ydata_profiling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-20 07:29:23.000000 ydata-profiling-4.3.0/src/ydata_profiling.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-20 07:29:23.000000 ydata-profiling-4.3.0/src/ydata_profiling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-20 07:29:23.000000 ydata-profiling-4.3.0/src/ydata_profiling.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:29:23.744413 ydata-profiling-4.3.0/venv/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-20 07:26:40.000000 ydata-profiling-4.3.0/venv/spark.yml
```

### Comparing `ydata-profiling-4.2.0/CONTRIBUTING.md` & `ydata-profiling-4.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/LICENSE` & `ydata-profiling-4.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/MANIFEST.in` & `ydata-profiling-4.3.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/Makefile` & `ydata-profiling-4.3.0/Makefile`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/PKG-INFO` & `ydata-profiling-4.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ydata-profiling
-Version: 4.2.0
+Version: 4.3.0
 Summary: Generate profile report for pandas DataFrame
 Home-page: https://github.com/ydataai/ydata-profiling
 Author: YData Labs Inc
 Author-email: opensource@ydata.ai
 License: MIT
 Description: # ydata-profiling
         
@@ -255,19 +255,27 @@
         - [GitHub Issues](https://github.com/ydataai/ydata-profiling/issues): bugs, proposals for changes, feature requests
         - [Discord](https://discord.com/invite/mw7xjJ7b7s): ideal for projects discussions, ask questions, collaborations, general chat
         - [Email](mailto:developers@ydata.ai): project collaborations or sponsoring
         
         > ❗ Before reporting an issue on GitHub, check out [Common Issues](https://ydata-profiling.ydata.ai/docs/master/pages/support_contrib/common_issues.html).
         
         ## 🤝🏽 Contributing
-        
         Learn how to get involved in the [Contribution Guide](https://ydata-profiling.ydata.ai/docs/master/pages/support_contrib/contribution_guidelines.html).
         
         A low-threshold place to ask questions or start contributing is the [Data Centric AI Community's Discord](https://discord.com/invite/mw7xjJ7b7s).
         
+        
+        A big thank you to all our amazing contributors! 
+        
+        <a href="https://github.com/ydataai/ydata-profiling/graphs/contributors">
+          <img src="https://contrib.rocks/image?repo=ydataai/ydata-profiling" />
+        </a>
+        
+        Contributors wall made with [contrib.rocks](https://contrib.rocks).
+        
 Keywords: pandas data-science data-analysis python jupyter ipython
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ydata-profiling Version: 4.2.0 Summary: Generate
+Metadata-Version: 2.1 Name: ydata-profiling Version: 4.3.0 Summary: Generate
 profile report for pandas DataFrame Home-page: https://github.com/ydataai/
 ydata-profiling Author: YData Labs Inc Author-email: opensource@ydata.ai
 License: MIT Description: # ydata-profiling [![Build Status](https://
 github.com/ydataai/pandas-profiling/actions/workflows/tests.yml/
 badge.svg?branch=master)](https://github.com/ydataai/pandas-profiling/actions/
 workflows/tests.yml) [![PyPI download month](https://img.shields.io/pypi/dm/
 ydata-profiling.svg)](https://pypi.python.org/pypi/ydata-profiling/) [![]
@@ -218,21 +218,24 @@
 questions, collaborations, general chat - [Email](mailto:developers@ydata.ai):
 project collaborations or sponsoring > â Before reporting an issue on GitHub,
 check out [Common Issues](https://ydata-profiling.ydata.ai/docs/master/pages/
 support_contrib/common_issues.html). ## ð¤ð½ Contributing Learn how to get
 involved in the [Contribution Guide](https://ydata-profiling.ydata.ai/docs/
 master/pages/support_contrib/contribution_guidelines.html). A low-threshold
 place to ask questions or start contributing is the [Data Centric AI
-Community's Discord](https://discord.com/invite/mw7xjJ7b7s). Keywords: pandas
-data-science data-analysis python jupyter ipython Platform: UNKNOWN Classifier:
-Development Status :: 5 - Production/Stable Classifier: Topic :: Software
-Development :: Build Tools Classifier: License :: OSI Approved :: MIT License
-Classifier: Environment :: Console Classifier: Operating System :: OS
-Independent Classifier: Intended Audience :: Science/Research Classifier:
-Intended Audience :: Developers Classifier: Intended Audience :: Financial and
-Insurance Industry Classifier: Intended Audience :: Healthcare Industry
-Classifier: Topic :: Scientific/Engineering Classifier: Framework :: IPython
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Requires-Python: >=3.7, <3.12 Description-Content-
-Type: text/markdown Provides-Extra: notebook Provides-Extra: unicode
+Community's Discord](https://discord.com/invite/mw7xjJ7b7s). A big thank you to
+all our amazing contributors! [https://contrib.rocks/image?repo=ydataai/ydata-
+profiling] Contributors wall made with [contrib.rocks](https://contrib.rocks).
+Keywords: pandas data-science data-analysis python jupyter ipython Platform:
+UNKNOWN Classifier: Development Status :: 5 - Production/Stable Classifier:
+Topic :: Software Development :: Build Tools Classifier: License :: OSI
+Approved :: MIT License Classifier: Environment :: Console Classifier:
+Operating System :: OS Independent Classifier: Intended Audience :: Science/
+Research Classifier: Intended Audience :: Developers Classifier: Intended
+Audience :: Financial and Insurance Industry Classifier: Intended Audience ::
+Healthcare Industry Classifier: Topic :: Scientific/Engineering Classifier:
+Framework :: IPython Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Requires-Python: >=3.7,
+<3.12 Description-Content-Type: text/markdown Provides-Extra: notebook
+Provides-Extra: unicode
```

### Comparing `ydata-profiling-4.2.0/README.md` & `ydata-profiling-4.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -247,11 +247,19 @@
 - [GitHub Issues](https://github.com/ydataai/ydata-profiling/issues): bugs, proposals for changes, feature requests
 - [Discord](https://discord.com/invite/mw7xjJ7b7s): ideal for projects discussions, ask questions, collaborations, general chat
 - [Email](mailto:developers@ydata.ai): project collaborations or sponsoring
 
 > ❗ Before reporting an issue on GitHub, check out [Common Issues](https://ydata-profiling.ydata.ai/docs/master/pages/support_contrib/common_issues.html).
 
 ## 🤝🏽 Contributing
-
 Learn how to get involved in the [Contribution Guide](https://ydata-profiling.ydata.ai/docs/master/pages/support_contrib/contribution_guidelines.html).
 
 A low-threshold place to ask questions or start contributing is the [Data Centric AI Community's Discord](https://discord.com/invite/mw7xjJ7b7s).
+
+
+A big thank you to all our amazing contributors! 
+
+<a href="https://github.com/ydataai/ydata-profiling/graphs/contributors">
+  <img src="https://contrib.rocks/image?repo=ydataai/ydata-profiling" />
+</a>
+
+Contributors wall made with [contrib.rocks](https://contrib.rocks).
```

#### html2text {}

```diff
@@ -214,8 +214,10 @@
 questions, collaborations, general chat - [Email](mailto:developers@ydata.ai):
 project collaborations or sponsoring > â Before reporting an issue on GitHub,
 check out [Common Issues](https://ydata-profiling.ydata.ai/docs/master/pages/
 support_contrib/common_issues.html). ## ð¤ð½ Contributing Learn how to get
 involved in the [Contribution Guide](https://ydata-profiling.ydata.ai/docs/
 master/pages/support_contrib/contribution_guidelines.html). A low-threshold
 place to ask questions or start contributing is the [Data Centric AI
-Community's Discord](https://discord.com/invite/mw7xjJ7b7s).
+Community's Discord](https://discord.com/invite/mw7xjJ7b7s). A big thank you to
+all our amazing contributors! [https://contrib.rocks/image?repo=ydataai/ydata-
+profiling] Contributors wall made with [contrib.rocks](https://contrib.rocks).
```

### Comparing `ydata-profiling-4.2.0/make.bat` & `ydata-profiling-4.3.0/make.bat`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/setup.py` & `ydata-profiling-4.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/pandas_profiling/__init__.py` & `ydata-profiling-4.3.0/src/pandas_profiling/__init__.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/__init__.py` & `ydata-profiling-4.3.0/src/ydata_profiling/__init__.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/compare_reports.py` & `ydata-profiling-4.3.0/src/ydata_profiling/compare_reports.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/config.py` & `ydata-profiling-4.3.0/src/ydata_profiling/config.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/config_default.yaml` & `ydata-profiling-4.3.0/src/ydata_profiling/config_default.yaml`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/config_minimal.yaml` & `ydata-profiling-4.3.0/src/ydata_profiling/config_minimal.yaml`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/controller/console.py` & `ydata-profiling-4.3.0/src/ydata_profiling/controller/console.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/expectations_report.py` & `ydata-profiling-4.3.0/src/ydata_profiling/expectations_report.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/model/alerts.py` & `ydata-profiling-4.3.0/src/ydata_profiling/model/alerts.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/model/correlations.py` & `ydata-profiling-4.3.0/src/ydata_profiling/model/correlations.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/model/describe.py` & `ydata-profiling-4.3.0/src/ydata_profiling/model/describe.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/model/description.py` & `ydata-profiling-4.3.0/src/ydata_profiling/model/description.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/model/expectation_algorithms.py` & `ydata-profiling-4.3.0/src/ydata_profiling/model/expectation_algorithms.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/model/handler.py` & `ydata-profiling-4.3.0/src/ydata_profiling/model/handler.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/model/missing.py` & `ydata-profiling-4.3.0/src/ydata_profiling/model/missing.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/model/pairwise.py` & `ydata-profiling-4.3.0/src/ydata_profiling/model/pairwise.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/__init__.py` & `ydata-profiling-4.3.0/src/ydata_profiling/model/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/correlations_pandas.py` & `ydata-profiling-4.3.0/src/ydata_profiling/model/pandas/correlations_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/dataframe_pandas.py` & `ydata-profiling-4.3.0/src/ydata_profiling/model/pandas/dataframe_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/describe_boolean_pandas.py` & `ydata-profiling-4.3.0/src/ydata_profiling/model/pandas/describe_boolean_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/describe_categorical_pandas.py` & `ydata-profiling-4.3.0/src/ydata_profiling/model/pandas/describe_categorical_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/describe_counts_pandas.py` & `ydata-profiling-4.3.0/src/ydata_profiling/model/pandas/describe_counts_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/describe_date_pandas.py` & `ydata-profiling-4.3.0/src/ydata_profiling/model/pandas/describe_date_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/describe_file_pandas.py` & `ydata-profiling-4.3.0/src/ydata_profiling/model/pandas/describe_file_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/describe_generic_pandas.py` & `ydata-profiling-4.3.0/src/ydata_profiling/model/pandas/describe_generic_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/describe_image_pandas.py` & `ydata-profiling-4.3.0/src/ydata_profiling/model/pandas/describe_image_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/describe_numeric_pandas.py` & `ydata-profiling-4.3.0/src/ydata_profiling/model/pandas/describe_numeric_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/describe_path_pandas.py` & `ydata-profiling-4.3.0/src/ydata_profiling/model/pandas/describe_path_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/describe_supported_pandas.py` & `ydata-profiling-4.3.0/src/ydata_profiling/model/pandas/describe_supported_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/describe_text_pandas.py` & `ydata-profiling-4.3.0/src/ydata_profiling/model/pandas/describe_text_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/describe_timeseries_pandas.py` & `ydata-profiling-4.3.0/src/ydata_profiling/model/pandas/describe_timeseries_pandas.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 
     Returns:
         outlier threshold, peaks, selected peaks.
     """
     pos_fft = fft.loc[fft["ampl"] > 0]
     median = pos_fft["ampl"].median()
     pos_fft_above_med = pos_fft[pos_fft["ampl"] > median]
-    mad = pos_fft_above_med["ampl"].mad()
+    mad = abs(pos_fft_above_med["ampl"] - pos_fft_above_med["ampl"].mean()).mean()
 
     threshold = median + mad * mad_threshold
 
     peak_indices = find_peaks(fft["ampl"], threshold=0.1)
     peaks = fft.loc[peak_indices[0], :]
 
     orig_peaks = peaks.copy()
```

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/describe_url_pandas.py` & `ydata-profiling-4.3.0/src/ydata_profiling/model/pandas/describe_url_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/discretize_pandas.py` & `ydata-profiling-4.3.0/src/ydata_profiling/model/pandas/discretize_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/duplicates_pandas.py` & `ydata-profiling-4.3.0/src/ydata_profiling/model/pandas/duplicates_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/imbalance_pandas.py` & `ydata-profiling-4.3.0/src/ydata_profiling/model/pandas/imbalance_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/missing_pandas.py` & `ydata-profiling-4.3.0/src/ydata_profiling/model/pandas/missing_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/sample_pandas.py` & `ydata-profiling-4.3.0/src/ydata_profiling/model/pandas/sample_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/summary_pandas.py` & `ydata-profiling-4.3.0/src/ydata_profiling/model/pandas/summary_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/table_pandas.py` & `ydata-profiling-4.3.0/src/ydata_profiling/model/pandas/table_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/utils_pandas.py` & `ydata-profiling-4.3.0/src/ydata_profiling/model/pandas/utils_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/model/sample.py` & `ydata-profiling-4.3.0/src/ydata_profiling/model/sample.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/model/spark/__init__.py` & `ydata-profiling-4.3.0/src/ydata_profiling/model/spark/__init__.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/model/spark/correlations_spark.py` & `ydata-profiling-4.3.0/src/ydata_profiling/model/spark/correlations_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/model/spark/dataframe_spark.py` & `ydata-profiling-4.3.0/src/ydata_profiling/model/spark/dataframe_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/model/spark/describe_boolean_spark.py` & `ydata-profiling-4.3.0/src/ydata_profiling/model/spark/describe_boolean_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/model/spark/describe_categorical_spark.py` & `ydata-profiling-4.3.0/src/ydata_profiling/model/spark/describe_categorical_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/model/spark/describe_counts_spark.py` & `ydata-profiling-4.3.0/src/ydata_profiling/model/spark/describe_counts_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/model/spark/describe_date_spark.py` & `ydata-profiling-4.3.0/src/ydata_profiling/model/spark/describe_date_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/model/spark/describe_generic_spark.py` & `ydata-profiling-4.3.0/src/ydata_profiling/model/spark/describe_generic_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/model/spark/describe_numeric_spark.py` & `ydata-profiling-4.3.0/src/ydata_profiling/model/spark/describe_numeric_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/model/spark/describe_supported_spark.py` & `ydata-profiling-4.3.0/src/ydata_profiling/model/spark/describe_supported_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/model/spark/describe_text_spark.py` & `ydata-profiling-4.3.0/src/ydata_profiling/model/spark/describe_text_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/model/spark/duplicates_spark.py` & `ydata-profiling-4.3.0/src/ydata_profiling/model/spark/duplicates_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/model/spark/missing_spark.py` & `ydata-profiling-4.3.0/src/ydata_profiling/model/spark/missing_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/model/spark/sample_spark.py` & `ydata-profiling-4.3.0/src/ydata_profiling/model/spark/sample_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/model/spark/summary_spark.py` & `ydata-profiling-4.3.0/src/ydata_profiling/model/spark/summary_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/model/spark/table_spark.py` & `ydata-profiling-4.3.0/src/ydata_profiling/model/spark/table_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/model/summarizer.py` & `ydata-profiling-4.3.0/src/ydata_profiling/model/summarizer.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/model/summary.py` & `ydata-profiling-4.3.0/src/ydata_profiling/model/summary.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/model/summary_algorithms.py` & `ydata-profiling-4.3.0/src/ydata_profiling/model/summary_algorithms.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/model/typeset.py` & `ydata-profiling-4.3.0/src/ydata_profiling/model/typeset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import datetime
 import imghdr
 import os
 import warnings
 from functools import partial, wraps
 from typing import Callable, Sequence, Set
 from urllib.parse import urlparse
 
@@ -116,15 +117,19 @@
             ]
 
         @staticmethod
         @multimethod
         @series_not_empty
         @series_handle_nulls
         def contains_op(series: pd.Series, state: dict) -> bool:
-            return pdt.is_string_dtype(series) and series_is_string(series, state)
+            return (
+                not pdt.is_categorical_dtype(series)
+                and pdt.is_string_dtype(series)
+                and series_is_string(series, state)
+            )
 
     class DateTime(visions.VisionsBaseType):
         @staticmethod
         def get_relations() -> Sequence[TypeRelation]:
             return [
                 IdentityRelation(Unsupported),
                 InferenceRelation(
@@ -135,15 +140,24 @@
             ]
 
         @staticmethod
         @multimethod
         @series_not_empty
         @series_handle_nulls
         def contains_op(series: pd.Series, state: dict) -> bool:
-            return pdt.is_datetime64_any_dtype(series)
+            is_datetime = pdt.is_datetime64_any_dtype(series)
+            if is_datetime:
+                return True
+            has_builtin_datetime = (
+                series.dropna()
+                .apply(type)
+                .isin([datetime.date, datetime.datetime])
+                .all()
+            )
+            return has_builtin_datetime
 
     class Categorical(visions.VisionsBaseType):
         """Type for categorical columns.
         Categorical columns in pandas categorical format
         and columns in string format with small count of unique values.
 
         Can be transformed from:
```

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/model/typeset_relations.py` & `ydata-profiling-4.3.0/src/ydata_profiling/model/typeset_relations.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import numpy as np
 import pandas as pd
 from pandas.api import types as pdt
 from visions.backends.pandas.series_utils import series_handle_nulls
 
 from ydata_profiling.config import Settings
+from ydata_profiling.utils.versions import is_pandas_1
 
 
 def is_nullable(series: pd.Series, state: dict) -> bool:
     return series.count() > 0
 
 
 def try_func(fn: Callable) -> Callable:
@@ -63,33 +64,37 @@
         return (series.astype(str).values == series.values).all()
     except (TypeError, ValueError):
         return False
 
 
 @series_handle_nulls
 def string_is_category(series: pd.Series, state: dict, k: Settings) -> bool:
-    """String is category, if following conditions are met
+    """String is category, if the following conditions are met
     - has at least one and less or equal distinct values as threshold
     - (distinct values / count of all values) is less than threshold
     - is not bool"""
     n_unique = series.nunique()
     unique_threshold = k.vars.text.percentage_cat_threshold
     threshold = k.vars.text.categorical_threshold
     return (
         1 <= n_unique <= threshold
-        and n_unique / series.size < unique_threshold
+        and (
+            n_unique / series.size < unique_threshold
+            if unique_threshold <= 1
+            else n_unique / series.size <= unique_threshold
+        )
         and not string_is_bool(series, state, k.vars.bool.mappings)
     )
 
 
 @series_handle_nulls
 def string_is_datetime(series: pd.Series, state: dict) -> bool:
     """If we can transform data to datetime and at least one is valid date."""
     try:
-        return not series.astype("datetime64").isna().all()
+        return not string_to_datetime(series, state).isna().all()
     except:  # noqa: E722
         return False
 
 
 @series_handle_nulls
 def string_is_numeric(series: pd.Series, state: dict, k: Settings) -> bool:
     if pdt.is_bool_dtype(series) or object_is_bool(series, state):
@@ -103,15 +108,17 @@
     except:  # noqa: E722
         return False
 
     return not numeric_is_category(series, state, k)
 
 
 def string_to_datetime(series: pd.Series, state: dict) -> pd.Series:
-    return series.astype("datetime64")
+    if is_pandas_1():
+        return series.astype("datetime64")
+    return pd.to_datetime(series, format="mixed")
 
 
 def string_to_numeric(series: pd.Series, state: dict) -> pd.Series:
     return pd.to_numeric(series, errors="coerce")
 
 
 hasnan_bool_name = "boolean"
```

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/profile_report.py` & `ydata-profiling-4.3.0/src/ydata_profiling/profile_report.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/formatters.py` & `ydata-profiling-4.3.0/src/ydata_profiling/report/formatters.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/__init__.py` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/core/__init__.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/alerts.py` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/core/alerts.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/collapse.py` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/core/collapse.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/container.py` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/core/container.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/correlation_table.py` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/core/correlation_table.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/dropdown.py` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/core/dropdown.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/image.py` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/core/image.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/renderable.py` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/core/renderable.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/root.py` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/core/root.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/sample.py` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/core/sample.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/table.py` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/core/table.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/variable.py` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/core/variable.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/variable_info.py` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/core/variable_info.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/flavours.py` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/flavours.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/__init__.py` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/__init__.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/alerts.py` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/alerts.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/container.py` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/container.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/correlation_table.py` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/correlation_table.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/duplicate.py` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/duplicate.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/frequency_table.py` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/frequency_table.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/frequency_table_small.py` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/frequency_table_small.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts.html` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts.html`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
                 {% if a.alert_type.name != "REJECTED" %}
                     <tr{% if loop.first %} style="border-top:0"{% endif %}>
                         {% for alert in value %}
                             <td>
                                 {% if not alert._is_empty %}
                                     {% include 'alerts/alert_' + alert.alert_type.name | lower  + '.html'  %}
                                 {% else %}
-                                    <em>Alert not present in {{ style._labels[idx] }}</em>
+                                    <em>Alert not present in this dataset</em>
                                 {% endif %}
                             </td>
                         {% endfor %}
                         <td>
                             <span class="label label-{{ styles[a.alert_type.name | lower] }}">{{ a.alert_type_name }}</span>
                         </td>
                     </tr>
```

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/frequency_table.html` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/frequency_table.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/frequency_table_small.html` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/frequency_table_small.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/report.html` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/report.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/batch_grid.html` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/batch_grid.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/grid.html` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/grid.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/sections.html` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/sections.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/select.html` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/select.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/tabs.html` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/tabs.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/table.html` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/table.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/toggle_button.html` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/toggle_button.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/variable_info.html` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/variable_info.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <p class="h4" title="{{ var_name }}">
     <a href="#pp_var_{{ anchor_id }}">{{ var_name }}</a>
     <br/>
     <small>{{ var_type }}</small>
 </p>
-{% if alerts | length > 1 %}
+{% if alerts | length > 0 %}
     {% if alerts[0].__class__.__name__ == 'list' %}
         {% set n_labels = style.labels | length %}
         <table width="100%">
             <thead>
                 <tr>
                     {% for idx in range(n_labels) %}
                         <th width="{{ 100 / n_labels }}%" style="color: {{ style.primary_colors[idx] }}">{{ style.labels[idx] }}</th>
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 {{_var_name_}}
 {{ var_type }}
-{% if alerts | length > 1 %} {% if alerts[0].__class__.__name__ == 'list' %} {%
+{% if alerts | length > 0 %} {% if alerts[0].__class__.__name__ == 'list' %} {%
 set n_labels = style.labels | length %}
 {{ style.labels[idx] }}
 {% if alerts[idx] | length > 0 %}
 {% for alert in alerts[idx] %} {{ alert }}  {% endfor %}
 {% else %} No alerts {% endif %}
 {% else %} {% if alerts | length > 0 %}
 {% for alert in alerts %} {{ alert }}  {% endfor %}
```

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/bootstrap-theme.min.css` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/bootstrap.min.css` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/bootstrap.min.js` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/cosmo.bootstrap.min.css` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/cosmo.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/flatly.bootstrap.min.css` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/flatly.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/jquery-1.12.4.min.js` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/jquery-1.12.4.min.js`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/script.js` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/script.js`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/simplex.bootstrap.min.css` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/simplex.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/style.css` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/style.css`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/united.bootstrap.min.css` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/united.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/javascript.html` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/javascript.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/navigation.html` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/navigation.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/style.html` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/style.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates.py` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/html/templates.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/__init__.py` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/widget/__init__.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/alerts.py` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/widget/alerts.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/collapse.py` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/widget/collapse.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/container.py` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/widget/container.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/dropdown.py` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/widget/dropdown.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/frequency_table.py` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/widget/frequency_table.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/frequency_table_small.py` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/widget/frequency_table_small.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/image.py` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/widget/image.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/notebook.py` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/widget/notebook.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/table.py` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/widget/table.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/toggle_button.py` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/flavours/widget/toggle_button.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/frequency_table_utils.py` & `ydata-profiling-4.3.0/src/ydata_profiling/report/presentation/frequency_table_utils.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/structure/correlations.py` & `ydata-profiling-4.3.0/src/ydata_profiling/report/structure/correlations.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/structure/overview.py` & `ydata-profiling-4.3.0/src/ydata_profiling/report/structure/overview.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/structure/report.py` & `ydata-profiling-4.3.0/src/ydata_profiling/report/structure/report.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/__init__.py` & `ydata-profiling-4.3.0/src/ydata_profiling/report/structure/variables/__init__.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_boolean.py` & `ydata-profiling-4.3.0/src/ydata_profiling/report/structure/variables/render_boolean.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_categorical.py` & `ydata-profiling-4.3.0/src/ydata_profiling/report/structure/variables/render_categorical.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_common.py` & `ydata-profiling-4.3.0/src/ydata_profiling/report/structure/variables/render_common.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_complex.py` & `ydata-profiling-4.3.0/src/ydata_profiling/report/structure/variables/render_complex.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_count.py` & `ydata-profiling-4.3.0/src/ydata_profiling/report/structure/variables/render_count.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_date.py` & `ydata-profiling-4.3.0/src/ydata_profiling/report/structure/variables/render_date.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_file.py` & `ydata-profiling-4.3.0/src/ydata_profiling/report/structure/variables/render_file.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_generic.py` & `ydata-profiling-4.3.0/src/ydata_profiling/report/structure/variables/render_generic.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_image.py` & `ydata-profiling-4.3.0/src/ydata_profiling/report/structure/variables/render_image.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_path.py` & `ydata-profiling-4.3.0/src/ydata_profiling/report/structure/variables/render_path.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_real.py` & `ydata-profiling-4.3.0/src/ydata_profiling/report/structure/variables/render_real.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_text.py` & `ydata-profiling-4.3.0/src/ydata_profiling/report/structure/variables/render_text.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_timeseries.py` & `ydata-profiling-4.3.0/src/ydata_profiling/report/structure/variables/render_timeseries.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_url.py` & `ydata-profiling-4.3.0/src/ydata_profiling/report/structure/variables/render_url.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/serialize_report.py` & `ydata-profiling-4.3.0/src/ydata_profiling/serialize_report.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/utils/cache.py` & `ydata-profiling-4.3.0/src/ydata_profiling/utils/cache.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/utils/common.py` & `ydata-profiling-4.3.0/src/ydata_profiling/utils/common.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/utils/dataframe.py` & `ydata-profiling-4.3.0/src/ydata_profiling/utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/utils/imghdr_patch.py` & `ydata-profiling-4.3.0/src/ydata_profiling/utils/imghdr_patch.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/utils/paths.py` & `ydata-profiling-4.3.0/src/ydata_profiling/utils/paths.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/visualisation/context.py` & `ydata-profiling-4.3.0/src/ydata_profiling/visualisation/context.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/visualisation/missing.py` & `ydata-profiling-4.3.0/src/ydata_profiling/visualisation/missing.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/visualisation/plot.py` & `ydata-profiling-4.3.0/src/ydata_profiling/visualisation/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -708,15 +708,16 @@
     nbins = np.min([50, df[sortbykey].nunique()])
 
     df["__bins"] = pd.cut(
         df[sortbykey], bins=nbins, include_lowest=True, labels=range(nbins)
     )
 
     df = df.groupby([entity_column, "__bins"])[sortbykey].count()
-    df = df.reset_index().pivot(entity_column, "__bins", sortbykey).T
+    df = df.reset_index().pivot_table(entity_column, "__bins", sortbykey).T
+
     if selected_entities:
         df = df[selected_entities].T
     else:
         df = df.T[:max_entities]
 
     return df
```

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling/visualisation/utils.py` & `ydata-profiling-4.3.0/src/ydata_profiling/visualisation/utils.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling.egg-info/PKG-INFO` & `ydata-profiling-4.3.0/src/ydata_profiling.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ydata-profiling
-Version: 4.2.0
+Version: 4.3.0
 Summary: Generate profile report for pandas DataFrame
 Home-page: https://github.com/ydataai/ydata-profiling
 Author: YData Labs Inc
 Author-email: opensource@ydata.ai
 License: MIT
 Description: # ydata-profiling
         
@@ -255,19 +255,27 @@
         - [GitHub Issues](https://github.com/ydataai/ydata-profiling/issues): bugs, proposals for changes, feature requests
         - [Discord](https://discord.com/invite/mw7xjJ7b7s): ideal for projects discussions, ask questions, collaborations, general chat
         - [Email](mailto:developers@ydata.ai): project collaborations or sponsoring
         
         > ❗ Before reporting an issue on GitHub, check out [Common Issues](https://ydata-profiling.ydata.ai/docs/master/pages/support_contrib/common_issues.html).
         
         ## 🤝🏽 Contributing
-        
         Learn how to get involved in the [Contribution Guide](https://ydata-profiling.ydata.ai/docs/master/pages/support_contrib/contribution_guidelines.html).
         
         A low-threshold place to ask questions or start contributing is the [Data Centric AI Community's Discord](https://discord.com/invite/mw7xjJ7b7s).
         
+        
+        A big thank you to all our amazing contributors! 
+        
+        <a href="https://github.com/ydataai/ydata-profiling/graphs/contributors">
+          <img src="https://contrib.rocks/image?repo=ydataai/ydata-profiling" />
+        </a>
+        
+        Contributors wall made with [contrib.rocks](https://contrib.rocks).
+        
 Keywords: pandas data-science data-analysis python jupyter ipython
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ydata-profiling Version: 4.2.0 Summary: Generate
+Metadata-Version: 2.1 Name: ydata-profiling Version: 4.3.0 Summary: Generate
 profile report for pandas DataFrame Home-page: https://github.com/ydataai/
 ydata-profiling Author: YData Labs Inc Author-email: opensource@ydata.ai
 License: MIT Description: # ydata-profiling [![Build Status](https://
 github.com/ydataai/pandas-profiling/actions/workflows/tests.yml/
 badge.svg?branch=master)](https://github.com/ydataai/pandas-profiling/actions/
 workflows/tests.yml) [![PyPI download month](https://img.shields.io/pypi/dm/
 ydata-profiling.svg)](https://pypi.python.org/pypi/ydata-profiling/) [![]
@@ -218,21 +218,24 @@
 questions, collaborations, general chat - [Email](mailto:developers@ydata.ai):
 project collaborations or sponsoring > â Before reporting an issue on GitHub,
 check out [Common Issues](https://ydata-profiling.ydata.ai/docs/master/pages/
 support_contrib/common_issues.html). ## ð¤ð½ Contributing Learn how to get
 involved in the [Contribution Guide](https://ydata-profiling.ydata.ai/docs/
 master/pages/support_contrib/contribution_guidelines.html). A low-threshold
 place to ask questions or start contributing is the [Data Centric AI
-Community's Discord](https://discord.com/invite/mw7xjJ7b7s). Keywords: pandas
-data-science data-analysis python jupyter ipython Platform: UNKNOWN Classifier:
-Development Status :: 5 - Production/Stable Classifier: Topic :: Software
-Development :: Build Tools Classifier: License :: OSI Approved :: MIT License
-Classifier: Environment :: Console Classifier: Operating System :: OS
-Independent Classifier: Intended Audience :: Science/Research Classifier:
-Intended Audience :: Developers Classifier: Intended Audience :: Financial and
-Insurance Industry Classifier: Intended Audience :: Healthcare Industry
-Classifier: Topic :: Scientific/Engineering Classifier: Framework :: IPython
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Requires-Python: >=3.7, <3.12 Description-Content-
-Type: text/markdown Provides-Extra: notebook Provides-Extra: unicode
+Community's Discord](https://discord.com/invite/mw7xjJ7b7s). A big thank you to
+all our amazing contributors! [https://contrib.rocks/image?repo=ydataai/ydata-
+profiling] Contributors wall made with [contrib.rocks](https://contrib.rocks).
+Keywords: pandas data-science data-analysis python jupyter ipython Platform:
+UNKNOWN Classifier: Development Status :: 5 - Production/Stable Classifier:
+Topic :: Software Development :: Build Tools Classifier: License :: OSI
+Approved :: MIT License Classifier: Environment :: Console Classifier:
+Operating System :: OS Independent Classifier: Intended Audience :: Science/
+Research Classifier: Intended Audience :: Developers Classifier: Intended
+Audience :: Financial and Insurance Industry Classifier: Intended Audience ::
+Healthcare Industry Classifier: Topic :: Scientific/Engineering Classifier:
+Framework :: IPython Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Requires-Python: >=3.7,
+<3.12 Description-Content-Type: text/markdown Provides-Extra: notebook
+Provides-Extra: unicode
```

### Comparing `ydata-profiling-4.2.0/src/ydata_profiling.egg-info/SOURCES.txt` & `ydata-profiling-4.3.0/src/ydata_profiling.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -224,13 +224,14 @@
 src/ydata_profiling/utils/common.py
 src/ydata_profiling/utils/compat.py
 src/ydata_profiling/utils/dataframe.py
 src/ydata_profiling/utils/imghdr_patch.py
 src/ydata_profiling/utils/notebook.py
 src/ydata_profiling/utils/paths.py
 src/ydata_profiling/utils/progress_bar.py
+src/ydata_profiling/utils/versions.py
 src/ydata_profiling/visualisation/__init__.py
 src/ydata_profiling/visualisation/context.py
 src/ydata_profiling/visualisation/missing.py
 src/ydata_profiling/visualisation/plot.py
 src/ydata_profiling/visualisation/utils.py
 venv/spark.yml
```

