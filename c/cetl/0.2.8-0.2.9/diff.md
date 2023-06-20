# Comparing `tmp/cetl-0.2.8.tar.gz` & `tmp/cetl-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cetl-0.2.8.tar", last modified: Mon Mar 27 09:18:50 2023, max compression
+gzip compressed data, was "cetl-0.2.9.tar", last modified: Tue Jun 20 03:40:43 2023, max compression
```

## Comparing `cetl-0.2.8.tar` & `cetl-0.2.9.tar`

### file list

```diff
@@ -1,73 +1,78 @@
-drwxrwxr-x   0 clement   (1000) clement   (1000)        0 2023-03-27 09:18:50.687402 cetl-0.2.8/
--rw-rw-r--   0 clement   (1000) clement   (1000)        0 2023-01-22 03:13:35.000000 cetl-0.2.8/LICENSE
--rw-rw-r--   0 clement   (1000) clement   (1000)     6399 2023-03-27 09:18:50.687402 cetl-0.2.8/PKG-INFO
--rw-rw-r--   0 clement   (1000) clement   (1000)     1305 2023-03-25 01:29:39.000000 cetl-0.2.8/README.md
-drwxrwxr-x   0 clement   (1000) clement   (1000)        0 2023-03-27 09:18:50.679402 cetl-0.2.8/cetl/
--rw-rw-r--   0 clement   (1000) clement   (1000)      554 2023-03-19 10:02:17.000000 cetl-0.2.8/cetl/__init__.py
-drwxrwxr-x   0 clement   (1000) clement   (1000)        0 2023-03-27 09:18:50.679402 cetl-0.2.8/cetl/functional_modules/
--rw-rw-r--   0 clement   (1000) clement   (1000)      169 2023-02-16 01:00:22.000000 cetl-0.2.8/cetl/functional_modules/__init__.py
--rw-rw-r--   0 clement   (1000) clement   (1000)      571 2023-02-23 13:32:11.000000 cetl-0.2.8/cetl/functional_modules/dummy_transformer.py
--rw-rw-r--   0 clement   (1000) clement   (1000)     1342 2023-02-18 15:33:44.000000 cetl-0.2.8/cetl/functional_modules/multithread_transformers.py
--rw-rw-r--   0 clement   (1000) clement   (1000)     1480 2023-03-03 07:01:39.000000 cetl-0.2.8/cetl/functional_modules/parallel_transformer.py
--rw-rw-r--   0 clement   (1000) clement   (1000)      737 2023-03-16 15:14:34.000000 cetl-0.2.8/cetl/functional_modules/pass_dataframe.py
-drwxrwxr-x   0 clement   (1000) clement   (1000)        0 2023-03-27 09:18:50.679402 cetl-0.2.8/cetl/json_modules/
--rw-rw-r--   0 clement   (1000) clement   (1000)       65 2023-02-13 03:46:39.000000 cetl-0.2.8/cetl/json_modules/__init__.py
--rw-rw-r--   0 clement   (1000) clement   (1000)      668 2023-02-19 04:34:46.000000 cetl-0.2.8/cetl/json_modules/drop_columns.py
--rw-rw-r--   0 clement   (1000) clement   (1000)     1079 2023-02-19 04:34:46.000000 cetl-0.2.8/cetl/json_modules/input.py
-drwxrwxr-x   0 clement   (1000) clement   (1000)        0 2023-03-27 09:18:50.683402 cetl-0.2.8/cetl/pandas_modules/
--rw-rw-r--   0 clement   (1000) clement   (1000)      974 2023-03-24 14:26:18.000000 cetl-0.2.8/cetl/pandas_modules/__init__.py
--rw-rw-r--   0 clement   (1000) clement   (1000)    20761 2023-02-19 04:34:46.000000 cetl-0.2.8/cetl/pandas_modules/add_new_column.py
--rw-rw-r--   0 clement   (1000) clement   (1000)      751 2023-02-19 04:34:46.000000 cetl-0.2.8/cetl/pandas_modules/add_row_number.py
--rw-rw-r--   0 clement   (1000) clement   (1000)     1817 2023-02-19 04:34:46.000000 cetl-0.2.8/cetl/pandas_modules/dataframe_mgt.py
--rw-rw-r--   0 clement   (1000) clement   (1000)     2717 2023-02-19 04:34:46.000000 cetl-0.2.8/cetl/pandas_modules/filter.py
--rw-rw-r--   0 clement   (1000) clement   (1000)      914 2023-02-19 04:34:46.000000 cetl-0.2.8/cetl/pandas_modules/input.py
--rw-rw-r--   0 clement   (1000) clement   (1000)     1187 2023-03-24 14:24:51.000000 cetl-0.2.8/cetl/pandas_modules/pass_dataframe.py
--rw-rw-r--   0 clement   (1000) clement   (1000)     3304 2023-02-19 04:34:46.000000 cetl-0.2.8/cetl/pandas_modules/two2one.py
-drwxrwxr-x   0 clement   (1000) clement   (1000)        0 2023-03-27 09:18:50.683402 cetl-0.2.8/cetl/spark_modules/
--rw-rw-r--   0 clement   (1000) clement   (1000)        0 2023-02-16 01:24:42.000000 cetl-0.2.8/cetl/spark_modules/__init__.py
-drwxrwxr-x   0 clement   (1000) clement   (1000)        0 2023-03-27 09:18:50.683402 cetl-0.2.8/cetl/sqlalchemy_modules/
--rw-rw-r--   0 clement   (1000) clement   (1000)        0 2023-02-16 01:24:57.000000 cetl-0.2.8/cetl/sqlalchemy_modules/__init__.py
-drwxrwxr-x   0 clement   (1000) clement   (1000)        0 2023-03-27 09:18:50.683402 cetl-0.2.8/cetl/utils/
--rw-rw-r--   0 clement   (1000) clement   (1000)       71 2023-02-14 09:23:50.000000 cetl-0.2.8/cetl/utils/__init__.py
--rw-rw-r--   0 clement   (1000) clement   (1000)      975 2023-02-03 15:20:22.000000 cetl-0.2.8/cetl/utils/airflow_pipeline.py
--rw-rw-r--   0 clement   (1000) clement   (1000)     1012 2023-03-24 17:31:23.000000 cetl-0.2.8/cetl/utils/base.py
--rw-rw-r--   0 clement   (1000) clement   (1000)     1611 2023-03-17 04:08:20.000000 cetl-0.2.8/cetl/utils/block.py
--rw-rw-r--   0 clement   (1000) clement   (1000)     2742 2023-03-27 09:16:48.000000 cetl-0.2.8/cetl/utils/builder.py
--rw-rw-r--   0 clement   (1000) clement   (1000)     7727 2023-02-16 01:27:48.000000 cetl-0.2.8/cetl/utils/dataframe.py
--rw-rw-r--   0 clement   (1000) clement   (1000)    11585 2023-02-24 13:47:01.000000 cetl-0.2.8/cetl/utils/dot_node.py
--rw-rw-r--   0 clement   (1000) clement   (1000)     1154 2023-03-03 06:57:48.000000 cetl-0.2.8/cetl/utils/file_mgt.py
--rw-rw-r--   0 clement   (1000) clement   (1000)     1329 2023-02-14 09:21:14.000000 cetl-0.2.8/cetl/utils/formating.py
--rw-rw-r--   0 clement   (1000) clement   (1000)       98 2023-03-16 15:02:45.000000 cetl-0.2.8/cetl/utils/kafka.py
--rw-rw-r--   0 clement   (1000) clement   (1000)     4297 2023-03-24 17:57:00.000000 cetl-0.2.8/cetl/utils/kafka_helper.py
--rw-rw-r--   0 clement   (1000) clement   (1000)     8691 2023-03-24 17:23:37.000000 cetl-0.2.8/cetl/utils/kafka_media.py
--rw-rw-r--   0 clement   (1000) clement   (1000)    31016 2023-03-25 07:15:41.000000 cetl-0.2.8/cetl/utils/pipeline.py
--rw-rw-r--   0 clement   (1000) clement   (1000)     1431 2023-01-20 10:46:14.000000 cetl-0.2.8/cetl/utils/registry.py
--rw-rw-r--   0 clement   (1000) clement   (1000)      479 2023-02-14 09:21:34.000000 cetl-0.2.8/cetl/utils/samplings.py
--rw-rw-r--   0 clement   (1000) clement   (1000)     7202 2023-03-23 13:52:56.000000 cetl-0.2.8/cetl/utils/sftp_file_mgt.py
--rw-rw-r--   0 clement   (1000) clement   (1000)     8211 2023-03-24 17:46:09.000000 cetl-0.2.8/cetl/utils/transform_wrapper.py
-drwxrwxr-x   0 clement   (1000) clement   (1000)        0 2023-03-27 09:18:50.679402 cetl-0.2.8/cetl.egg-info/
--rw-rw-r--   0 clement   (1000) clement   (1000)     6399 2023-03-27 09:18:50.000000 cetl-0.2.8/cetl.egg-info/PKG-INFO
--rw-rw-r--   0 clement   (1000) clement   (1000)     1772 2023-03-27 09:18:50.000000 cetl-0.2.8/cetl.egg-info/SOURCES.txt
--rw-rw-r--   0 clement   (1000) clement   (1000)        1 2023-03-27 09:18:50.000000 cetl-0.2.8/cetl.egg-info/dependency_links.txt
--rw-rw-r--   0 clement   (1000) clement   (1000)       32 2023-03-27 09:18:50.000000 cetl-0.2.8/cetl.egg-info/requires.txt
--rw-rw-r--   0 clement   (1000) clement   (1000)       31 2023-03-27 09:18:50.000000 cetl-0.2.8/cetl.egg-info/top_level.txt
--rw-rw-r--   0 clement   (1000) clement   (1000)      102 2023-01-22 03:58:18.000000 cetl-0.2.8/pyproject.toml
-drwxrwxr-x   0 clement   (1000) clement   (1000)        0 2023-03-27 09:18:50.687402 cetl-0.2.8/sample_user_project/
--rw-rw-r--   0 clement   (1000) clement   (1000)        0 2023-03-19 14:50:38.000000 cetl-0.2.8/sample_user_project/__init__.py
--rw-rw-r--   0 clement   (1000) clement   (1000)     3120 2023-03-19 14:42:22.000000 cetl-0.2.8/sample_user_project/app.py
-drwxrwxr-x   0 clement   (1000) clement   (1000)        0 2023-03-27 09:18:50.687402 cetl-0.2.8/sample_user_project/file_modules/
--rw-rw-r--   0 clement   (1000) clement   (1000)       39 2023-03-19 14:24:10.000000 cetl-0.2.8/sample_user_project/file_modules/__init__.py
--rw-rw-r--   0 clement   (1000) clement   (1000)      220 2023-03-19 14:57:03.000000 cetl-0.2.8/sample_user_project/file_modules/builder.py
--rw-rw-r--   0 clement   (1000) clement   (1000)     1081 2023-03-19 15:53:52.000000 cetl-0.2.8/sample_user_project/file_modules/file_compress.py
-drwxrwxr-x   0 clement   (1000) clement   (1000)        0 2023-03-27 09:18:50.687402 cetl-0.2.8/sample_user_project/sample_modules/
--rw-rw-r--   0 clement   (1000) clement   (1000)        0 2023-02-03 02:31:15.000000 cetl-0.2.8/sample_user_project/sample_modules/__init__.py
--rw-rw-r--   0 clement   (1000) clement   (1000)      749 2023-02-14 07:35:22.000000 cetl-0.2.8/sample_user_project/sample_modules/add_new_column.py
--rw-rw-r--   0 clement   (1000) clement   (1000)      963 2023-02-04 15:02:14.000000 cetl-0.2.8/sample_user_project/sample_modules/data_validation_check.py
--rw-rw-r--   0 clement   (1000) clement   (1000)      555 2023-03-21 06:47:38.000000 cetl-0.2.8/sample_user_project/test_file_compress.py
--rw-rw-r--   0 clement   (1000) clement   (1000)       38 2023-03-27 09:18:50.687402 cetl-0.2.8/setup.cfg
--rw-rw-r--   0 clement   (1000) clement   (1000)     1097 2023-03-25 07:11:06.000000 cetl-0.2.8/setup.py
-drwxrwxr-x   0 clement   (1000) clement   (1000)        0 2023-03-27 09:18:50.687402 cetl-0.2.8/tests/
--rw-rw-r--   0 clement   (1000) clement   (1000)        0 2023-02-15 16:02:10.000000 cetl-0.2.8/tests/__init__.py
--rw-rw-r--   0 clement   (1000) clement   (1000)     1210 2023-03-23 14:43:45.000000 cetl-0.2.8/tests/test_kafka_helper.py
--rw-rw-r--   0 clement   (1000) clement   (1000)     1290 2023-02-16 01:05:45.000000 cetl-0.2.8/tests/test_parallel_transformer.py
--rw-rw-r--   0 clement   (1000) clement   (1000)      579 2023-02-15 16:14:53.000000 cetl-0.2.8/tests/test_pass_dataframe.py
+drwxrwxr-x   0 clement   (1000) clement   (1000)        0 2023-06-20 03:40:43.432478 cetl-0.2.9/
+-rw-rw-r--   0 clement   (1000) clement   (1000)        0 2023-01-22 03:13:35.000000 cetl-0.2.9/LICENSE
+-rw-rw-r--   0 clement   (1000) clement   (1000)     6399 2023-06-20 03:40:43.432478 cetl-0.2.9/PKG-INFO
+-rw-rw-r--   0 clement   (1000) clement   (1000)     1305 2023-03-25 01:29:39.000000 cetl-0.2.9/README.md
+drwxrwxr-x   0 clement   (1000) clement   (1000)        0 2023-06-20 03:40:43.428478 cetl-0.2.9/cetl/
+-rw-rw-r--   0 clement   (1000) clement   (1000)      554 2023-03-19 10:02:17.000000 cetl-0.2.9/cetl/__init__.py
+drwxrwxr-x   0 clement   (1000) clement   (1000)        0 2023-06-20 03:40:43.428478 cetl-0.2.9/cetl/functional_modules/
+-rw-rw-r--   0 clement   (1000) clement   (1000)      169 2023-02-16 01:00:22.000000 cetl-0.2.9/cetl/functional_modules/__init__.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)      571 2023-02-23 13:32:11.000000 cetl-0.2.9/cetl/functional_modules/dummy_transformer.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)     1342 2023-02-18 15:33:44.000000 cetl-0.2.9/cetl/functional_modules/multithread_transformers.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)     1480 2023-03-03 07:01:39.000000 cetl-0.2.9/cetl/functional_modules/parallel_transformer.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)      737 2023-03-16 15:14:34.000000 cetl-0.2.9/cetl/functional_modules/pass_dataframe.py
+drwxrwxr-x   0 clement   (1000) clement   (1000)        0 2023-06-20 03:40:43.428478 cetl-0.2.9/cetl/json_modules/
+-rw-rw-r--   0 clement   (1000) clement   (1000)       65 2023-02-13 03:46:39.000000 cetl-0.2.9/cetl/json_modules/__init__.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)      668 2023-02-19 04:34:46.000000 cetl-0.2.9/cetl/json_modules/drop_columns.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)     1079 2023-02-19 04:34:46.000000 cetl-0.2.9/cetl/json_modules/input.py
+drwxrwxr-x   0 clement   (1000) clement   (1000)        0 2023-06-20 03:40:43.428478 cetl-0.2.9/cetl/pandas_modules/
+-rw-rw-r--   0 clement   (1000) clement   (1000)      974 2023-03-24 14:26:18.000000 cetl-0.2.9/cetl/pandas_modules/__init__.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)    20761 2023-02-19 04:34:46.000000 cetl-0.2.9/cetl/pandas_modules/add_new_column.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)      751 2023-02-19 04:34:46.000000 cetl-0.2.9/cetl/pandas_modules/add_row_number.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)     1817 2023-02-19 04:34:46.000000 cetl-0.2.9/cetl/pandas_modules/dataframe_mgt.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)     2717 2023-02-19 04:34:46.000000 cetl-0.2.9/cetl/pandas_modules/filter.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)      914 2023-02-19 04:34:46.000000 cetl-0.2.9/cetl/pandas_modules/input.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)     1187 2023-03-24 14:24:51.000000 cetl-0.2.9/cetl/pandas_modules/pass_dataframe.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)     3304 2023-02-19 04:34:46.000000 cetl-0.2.9/cetl/pandas_modules/two2one.py
+drwxrwxr-x   0 clement   (1000) clement   (1000)        0 2023-06-20 03:40:43.428478 cetl-0.2.9/cetl/spark_modules/
+-rw-rw-r--   0 clement   (1000) clement   (1000)        0 2023-02-16 01:24:42.000000 cetl-0.2.9/cetl/spark_modules/__init__.py
+drwxrwxr-x   0 clement   (1000) clement   (1000)        0 2023-06-20 03:40:43.428478 cetl-0.2.9/cetl/sqlalchemy_modules/
+-rw-rw-r--   0 clement   (1000) clement   (1000)        0 2023-02-16 01:24:57.000000 cetl-0.2.9/cetl/sqlalchemy_modules/__init__.py
+drwxrwxr-x   0 clement   (1000) clement   (1000)        0 2023-06-20 03:40:43.432478 cetl-0.2.9/cetl/utils/
+-rw-rw-r--   0 clement   (1000) clement   (1000)       71 2023-02-14 09:23:50.000000 cetl-0.2.9/cetl/utils/__init__.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)      975 2023-02-03 15:20:22.000000 cetl-0.2.9/cetl/utils/airflow_pipeline.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)     1012 2023-03-24 17:31:23.000000 cetl-0.2.9/cetl/utils/base.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)     1611 2023-03-17 04:08:20.000000 cetl-0.2.9/cetl/utils/block.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)     2742 2023-03-27 09:16:48.000000 cetl-0.2.9/cetl/utils/builder.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)     7727 2023-02-16 01:27:48.000000 cetl-0.2.9/cetl/utils/dataframe.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)    11585 2023-02-24 13:47:01.000000 cetl-0.2.9/cetl/utils/dot_node.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)        0 2023-04-19 03:27:24.000000 cetl-0.2.9/cetl/utils/encryption.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)     1154 2023-03-03 06:57:48.000000 cetl-0.2.9/cetl/utils/file_mgt.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)     1329 2023-02-14 09:21:14.000000 cetl-0.2.9/cetl/utils/formating.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)       98 2023-03-16 15:02:45.000000 cetl-0.2.9/cetl/utils/kafka.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)     4297 2023-03-24 17:57:00.000000 cetl-0.2.9/cetl/utils/kafka_helper.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)     8691 2023-03-24 17:23:37.000000 cetl-0.2.9/cetl/utils/kafka_media.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)    32053 2023-06-20 03:13:41.000000 cetl-0.2.9/cetl/utils/pipeline.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)     1431 2023-01-20 10:46:14.000000 cetl-0.2.9/cetl/utils/registry.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)      479 2023-02-14 09:21:34.000000 cetl-0.2.9/cetl/utils/samplings.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)     7202 2023-03-23 13:52:56.000000 cetl-0.2.9/cetl/utils/sftp_file_mgt.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)     8211 2023-03-24 17:46:09.000000 cetl-0.2.9/cetl/utils/transform_wrapper.py
+drwxrwxr-x   0 clement   (1000) clement   (1000)        0 2023-06-20 03:40:43.428478 cetl-0.2.9/cetl.egg-info/
+-rw-rw-r--   0 clement   (1000) clement   (1000)     6399 2023-06-20 03:40:43.000000 cetl-0.2.9/cetl.egg-info/PKG-INFO
+-rw-rw-r--   0 clement   (1000) clement   (1000)     1943 2023-06-20 03:40:43.000000 cetl-0.2.9/cetl.egg-info/SOURCES.txt
+-rw-rw-r--   0 clement   (1000) clement   (1000)        1 2023-06-20 03:40:43.000000 cetl-0.2.9/cetl.egg-info/dependency_links.txt
+-rw-rw-r--   0 clement   (1000) clement   (1000)       32 2023-06-20 03:40:43.000000 cetl-0.2.9/cetl.egg-info/requires.txt
+-rw-rw-r--   0 clement   (1000) clement   (1000)       31 2023-06-20 03:40:43.000000 cetl-0.2.9/cetl.egg-info/top_level.txt
+-rw-rw-r--   0 clement   (1000) clement   (1000)      102 2023-01-22 03:58:18.000000 cetl-0.2.9/pyproject.toml
+drwxrwxr-x   0 clement   (1000) clement   (1000)        0 2023-06-20 03:40:43.432478 cetl-0.2.9/sample_user_project/
+-rw-rw-r--   0 clement   (1000) clement   (1000)        0 2023-03-19 14:50:38.000000 cetl-0.2.9/sample_user_project/__init__.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)     3120 2023-03-19 14:42:22.000000 cetl-0.2.9/sample_user_project/app.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)     2308 2023-04-28 11:03:30.000000 cetl-0.2.9/sample_user_project/call_api.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)     3438 2023-04-30 06:01:38.000000 cetl-0.2.9/sample_user_project/compress_files.py
+drwxrwxr-x   0 clement   (1000) clement   (1000)        0 2023-06-20 03:40:43.432478 cetl-0.2.9/sample_user_project/file_modules/
+-rw-rw-r--   0 clement   (1000) clement   (1000)      465 2023-04-28 03:46:27.000000 cetl-0.2.9/sample_user_project/file_modules/__init__.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)      220 2023-03-19 14:57:03.000000 cetl-0.2.9/sample_user_project/file_modules/builder.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)    16094 2023-04-28 04:13:44.000000 cetl-0.2.9/sample_user_project/file_modules/file_compress.py
+drwxrwxr-x   0 clement   (1000) clement   (1000)        0 2023-06-20 03:40:43.432478 cetl-0.2.9/sample_user_project/sample_modules/
+-rw-rw-r--   0 clement   (1000) clement   (1000)        0 2023-02-03 02:31:15.000000 cetl-0.2.9/sample_user_project/sample_modules/__init__.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)      749 2023-02-14 07:35:22.000000 cetl-0.2.9/sample_user_project/sample_modules/add_new_column.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)      963 2023-02-04 15:02:14.000000 cetl-0.2.9/sample_user_project/sample_modules/data_validation_check.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)      555 2023-03-21 06:47:38.000000 cetl-0.2.9/sample_user_project/test_file_compress.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)       38 2023-06-20 03:40:43.436478 cetl-0.2.9/setup.cfg
+-rw-rw-r--   0 clement   (1000) clement   (1000)     1097 2023-06-20 03:40:34.000000 cetl-0.2.9/setup.py
+drwxrwxr-x   0 clement   (1000) clement   (1000)        0 2023-06-20 03:40:43.432478 cetl-0.2.9/tests/
+-rw-rw-r--   0 clement   (1000) clement   (1000)        0 2023-02-15 16:02:10.000000 cetl-0.2.9/tests/__init__.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)      360 2023-06-20 03:15:11.000000 cetl-0.2.9/tests/example1_test_build_pipeline.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)     1090 2023-06-20 03:14:58.000000 cetl-0.2.9/tests/example2_test_build_pipeline.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)     1209 2023-06-20 03:16:52.000000 cetl-0.2.9/tests/test_kafka_helper.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)     1282 2023-06-20 03:17:31.000000 cetl-0.2.9/tests/test_parallel_transformer.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)      571 2023-06-20 02:20:51.000000 cetl-0.2.9/tests/test_pass_dataframe.py
```

### Comparing `cetl-0.2.8/PKG-INFO` & `cetl-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cetl
-Version: 0.2.8
+Version: 0.2.9
 Summary: A basic data pipeline tools for data engineer to handle the CRM or loyalty data
 Author: Clement
 Author-email: <cheukub@gmail.com>
 Keywords: python,data pipeline,pipeline
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cetl-0.2.8/README.md` & `cetl-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `cetl-0.2.8/cetl/__init__.py` & `cetl-0.2.9/cetl/__init__.py`

 * *Files identical despite different names*

### Comparing `cetl-0.2.8/cetl/functional_modules/dummy_transformer.py` & `cetl-0.2.9/cetl/functional_modules/dummy_transformer.py`

 * *Files identical despite different names*

### Comparing `cetl-0.2.8/cetl/functional_modules/multithread_transformers.py` & `cetl-0.2.9/cetl/functional_modules/multithread_transformers.py`

 * *Files identical despite different names*

### Comparing `cetl-0.2.8/cetl/functional_modules/parallel_transformer.py` & `cetl-0.2.9/cetl/functional_modules/parallel_transformer.py`

 * *Files identical despite different names*

### Comparing `cetl-0.2.8/cetl/functional_modules/pass_dataframe.py` & `cetl-0.2.9/cetl/functional_modules/pass_dataframe.py`

 * *Files identical despite different names*

### Comparing `cetl-0.2.8/cetl/json_modules/drop_columns.py` & `cetl-0.2.9/cetl/json_modules/drop_columns.py`

 * *Files identical despite different names*

### Comparing `cetl-0.2.8/cetl/json_modules/input.py` & `cetl-0.2.9/cetl/json_modules/input.py`

 * *Files identical despite different names*

### Comparing `cetl-0.2.8/cetl/pandas_modules/__init__.py` & `cetl-0.2.9/cetl/pandas_modules/__init__.py`

 * *Files identical despite different names*

### Comparing `cetl-0.2.8/cetl/pandas_modules/add_new_column.py` & `cetl-0.2.9/cetl/pandas_modules/add_new_column.py`

 * *Files identical despite different names*

### Comparing `cetl-0.2.8/cetl/pandas_modules/add_row_number.py` & `cetl-0.2.9/cetl/pandas_modules/add_row_number.py`

 * *Files identical despite different names*

### Comparing `cetl-0.2.8/cetl/pandas_modules/dataframe_mgt.py` & `cetl-0.2.9/cetl/pandas_modules/dataframe_mgt.py`

 * *Files identical despite different names*

### Comparing `cetl-0.2.8/cetl/pandas_modules/filter.py` & `cetl-0.2.9/cetl/pandas_modules/filter.py`

 * *Files identical despite different names*

### Comparing `cetl-0.2.8/cetl/pandas_modules/input.py` & `cetl-0.2.9/cetl/pandas_modules/input.py`

 * *Files identical despite different names*

### Comparing `cetl-0.2.8/cetl/pandas_modules/pass_dataframe.py` & `cetl-0.2.9/cetl/pandas_modules/pass_dataframe.py`

 * *Files identical despite different names*

### Comparing `cetl-0.2.8/cetl/pandas_modules/two2one.py` & `cetl-0.2.9/cetl/pandas_modules/two2one.py`

 * *Files identical despite different names*

### Comparing `cetl-0.2.8/cetl/utils/airflow_pipeline.py` & `cetl-0.2.9/cetl/utils/airflow_pipeline.py`

 * *Files identical despite different names*

### Comparing `cetl-0.2.8/cetl/utils/base.py` & `cetl-0.2.9/cetl/utils/base.py`

 * *Files identical despite different names*

### Comparing `cetl-0.2.8/cetl/utils/block.py` & `cetl-0.2.9/cetl/utils/block.py`

 * *Files identical despite different names*

### Comparing `cetl-0.2.8/cetl/utils/builder.py` & `cetl-0.2.9/cetl/utils/builder.py`

 * *Files identical despite different names*

### Comparing `cetl-0.2.8/cetl/utils/dataframe.py` & `cetl-0.2.9/cetl/utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `cetl-0.2.8/cetl/utils/dot_node.py` & `cetl-0.2.9/cetl/utils/dot_node.py`

 * *Files identical despite different names*

### Comparing `cetl-0.2.8/cetl/utils/file_mgt.py` & `cetl-0.2.9/cetl/utils/file_mgt.py`

 * *Files identical despite different names*

### Comparing `cetl-0.2.8/cetl/utils/formating.py` & `cetl-0.2.9/cetl/utils/formating.py`

 * *Files identical despite different names*

### Comparing `cetl-0.2.8/cetl/utils/kafka_helper.py` & `cetl-0.2.9/cetl/utils/kafka_helper.py`

 * *Files identical despite different names*

### Comparing `cetl-0.2.8/cetl/utils/kafka_media.py` & `cetl-0.2.9/cetl/utils/kafka_media.py`

 * *Files identical despite different names*

### Comparing `cetl-0.2.8/cetl/utils/pipeline.py` & `cetl-0.2.9/cetl/utils/pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -115,24 +115,25 @@
                     assert sub_trans_name!="parallelTransformer", "parallel is not acceptable in parallelTransfomer"
                     ######################### END
 
                     #add note pair
                     index = index + 1
                     sub_breakpoint = sub_trans_cfg.pop("breakpoint") if "breakpoint" in sub_trans_cfg else 0
                     description = sub_trans_cfg.pop("description") if "description" in sub_trans_cfg else ""
+                    # --- get Registry
                     module_type = sub_trans_cfg.pop("module_type") if "module_type" in sub_trans_cfg else ""
                     TRANSFORMERS = get_register(module_type, pipeline_settings.default_type)
                     # print(TRANSFORMERS)
                     transformer = build_transformer_from_cfg(sub_trans_cfg, TRANSFORMERS)
                     transformer.pre_node_name = node_name
                     transformer.index = index
                     transformer.node_name = f"{str(index)}.{sub_trans_name}"
-                    # transformer.__name__
                     transformer.description = description
                     transformer.breakpoint = sub_breakpoint
+                    # --- kafka setting ---
                     transformer.bootstrap_servers=pipeline_settings.bootstrap_servers
                     transformer.print_task_result = pipeline_settings.print_task_result
                     transformer.exchange_media = pipeline_settings.exchange_media
                     transformer.fernet_key = pipeline_settings.fernet_key
                     transformer.pipe_topic_name = pipeline_settings.pipe_topic_name
                     transformers_list.append(transformer)
                     # update nodename2transformer
@@ -170,14 +171,15 @@
             previous_node, latest_node = update_node(latest_nodes, parallel_latest_node)
             # update node_pairs
             node_pairs.append(parallel_node_pairs)
             # add steps
             # module_type = trans_cfg.pop("module_type") if "module_type" in trans_cfg else ""
             # TRANSFORMERS = get_register(module_type)
             # print(transformers_list)
+            # --- parallel transformer setting
             parallel_transformer = build_transformer_from_cfg(trans_cfg, 
                                                               FUNCTIONAL_TRANSFORMERS, 
                                                               transformers_list)
             parallel_transformer.breakpoint = breakpoint
             parallel_transformer.print_task_result = pipeline_settings.print_task_result
             parallel_transformer.node_name = parallel_node_name
             steps.append(parallel_transformer)
@@ -235,14 +237,16 @@
             transformer.pre_node_name = pre_node_name
             # update node_pairs
             if isinstance(latest_node, str):
                 node_pairs.append((latest_node, node_name))
             elif isinstance(latest_node, list):
                 for item in latest_node:
                     node_pairs.append((item, node_name))
+
+            # add current node name to the node_name_set
             node_name_set.add(node_name)
             #update latest_node
             latest_node = node_name
 
     # remove empty node in node pair
     # simple_node_pairs = [item for item in simple_node_pairs if item[0]!=""]
     node_name_set = set([node_name for node_name in node_name_set if node_name!=""])
@@ -548,21 +552,21 @@
                                     node_name_set, 
                                     node_pairs, 
                                     node_name,
                                     latest_node, 
                                     index, 
                                     parallel_index, 
                                     nodename2transformer,
-                                    pipeline_settings,
-                                    kafka_media):
+                                    pipeline_settings):
 
     for step_tuple in steps:
 
         trans_name = step_tuple[0]
         transformer = step_tuple[1]
+        breakpoint = transformer.breakpoint if transformer.breakpoint else 0
 
 
         if isinstance(transformer, parallelTransformer):
 
             parallel_name = "parallel"
             parallel_index +=1
             parallel_node_name = f"{parallel_name}_no.{parallel_index}"
@@ -601,30 +605,34 @@
                     nodename2transformer = recursive_build_node_from_steps( sub_transformer.steps,
                                                                             node_name_set,
                                                                             node_pairs, 
                                                                             latest_node, 
                                                                             index, 
                                                                             parallel_index, 
                                                                             nodename2transformer,
-                                                                            pipeline_settings,
-                                                                            kafka_media)
+                                                                            pipeline_settings)
                     node_pairs.append(_node_pairs)
 
                 else:
                 ####################################### dealing with real transformer
                     index = index + 1
+                    sub_breakpoint = sub_transformer.breakpoint if sub_transformer.breakpoint else 0
                     description = sub_transformer.description if sub_transformer.description else ""
                     sub_transformer.pre_node_name = node_name
                     sub_transformer.index = index
                     _tuple = _name_estimators([sub_transformer])
                     sub_transformer.node_name = f"{str(index)}.{_tuple[0][0]}"
                     sub_transformer.description = description
+                    sub_transformer.breakpoint = sub_breakpoint
+                    # --- kafka setting ---
+                    sub_transformer.bootstrap_servers=pipeline_settings.bootstrap_servers
                     sub_transformer.print_task_result = pipeline_settings.print_task_result
                     sub_transformer.exchange_media = pipeline_settings.exchange_media
-                    sub_transformer.kafka_media = kafka_media
+                    sub_transformer.fernet_key = pipeline_settings.fernet_key
+                    sub_transformer.pipe_topic_name = pipeline_settings.pipe_topic_name
                     transformers_list.append(sub_transformer)
                     # update nodename2transformer
                     nodename2transformer[sub_transformer.node_name] = sub_transformer
                     # update steps list
                     previous_node, _latest_node = update_node(latest_node, sub_transformer.node_name)
                     parallel_node_pairs[f"process_no.{str(i)}"] = (previous_node, _latest_node)
                     node_name_set.add(_latest_node)
@@ -633,15 +641,22 @@
 
 
             ################################################# dealing with the parallelTransformer
             # update latest_node
             previous_node, latest_node = update_node(latest_node, parallel_latest_node)
             # update node_pairs
             node_pairs.append(parallel_node_pairs)
-            nodename2transformer[parallel_node_name] = transformer
+            # --- no need to add to steps, coz already have transformers in input
+            parallel_transformer = transformer
+            # parallel_transformer.breakpoint = breakpoint
+            # parallel_transformer.print_task_result = pipeline_settings.print_task_result
+            # parallel_transformer.node_name = parallel_node_name
+            # steps.append(parallel_transformer)
+
+            nodename2transformer[parallel_node_name] = parallel_transformer
 
         elif isinstance(transformer, DataPipeline):
             node_name_set, \
             _node_pairs, \
             node_name, \
             latest_node, \
             index, \
@@ -649,44 +664,47 @@
             nodename2transformer = recursive_build_node_from_steps( sub_transformer.steps,
                                                                     node_name_set,
                                                                     [], 
                                                                     latest_node, 
                                                                     index, 
                                                                     parallel_index, 
                                                                     nodename2transformer,
-                                                                    pipeline_settings,
-                                                                    kafka_media)
+                                                                    pipeline_settings)
             node_pairs.append(_node_pairs)
         
         else:
 
             index = index + 1
             pre_node_name = node_name
+            transformer.node_name = f"{str(index)}.{trans_name}"
+            # breakpoint = transformer.breakpoint if transformer.breakoint else ""
             description = transformer.description if transformer.description else ""
             transformer.index = index
-            transformer.node_name = f"{str(index)}.{trans_name}"
             transformer.description = description
+            transformer.breakpoint = breakpoint
             transformer.print_task_result = pipeline_settings.print_task_result
             transformer.exchange_media = pipeline_settings.exchange_media
-            transformer.kafka_media = kafka_media
+            transformer.bootstrap_servers=pipeline_settings.bootstrap_servers
+            transformer.fernet_key = pipeline_settings.fernet_key
+            transformer.pipe_topic_name = pipeline_settings.pipe_topic_name
+            
 
             # update nodename2transformer
             nodename2transformer[transformer.node_name] = transformer
             # set pre_node_name
             transformer.pre_node_name = pre_node_name
             # update node_pairs
             if isinstance(latest_node, str):
                 node_pairs.append((latest_node, transformer.node_name))
             elif isinstance(latest_node, list):
                 for item in latest_node:
                     node_pairs.append((item, transformer.node_name))
 
             # add current node name to the node_name_set
             node_name_set.add(transformer.node_name)
-
             #update latest_node
             latest_node = transformer.node_name
         
     node_name_set = set([node_name for node_name in node_name_set if node_name!=""])
 
     return node_name_set, node_pairs, latest_node, index, parallel_index, nodename2transformer
 
@@ -707,15 +725,14 @@
                                                                     self._node_name_set,
                                                                     self._node_pairs, 
                                                                     "",
                                                                     self._latest_node, 
                                                                     self._index,
                                                                     self._parallel_index,
                                                                     self._nodename2transformer,
-                                                                    self._pipeline_settings,
-                                                                    self.kafka_media)
+                                                                    self._pipeline_settings)
 
     # self.nodes_text = init_nodes_text(self._nodename2transformer)
 
     self._pipeline = make_pipeline(*steps)
     
     return self
```

### Comparing `cetl-0.2.8/cetl/utils/registry.py` & `cetl-0.2.9/cetl/utils/registry.py`

 * *Files identical despite different names*

### Comparing `cetl-0.2.8/cetl/utils/sftp_file_mgt.py` & `cetl-0.2.9/cetl/utils/sftp_file_mgt.py`

 * *Files identical despite different names*

### Comparing `cetl-0.2.8/cetl/utils/transform_wrapper.py` & `cetl-0.2.9/cetl/utils/transform_wrapper.py`

 * *Files identical despite different names*

### Comparing `cetl-0.2.8/cetl.egg-info/PKG-INFO` & `cetl-0.2.9/cetl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cetl
-Version: 0.2.8
+Version: 0.2.9
 Summary: A basic data pipeline tools for data engineer to handle the CRM or loyalty data
 Author: Clement
 Author-email: <cheukub@gmail.com>
 Keywords: python,data pipeline,pipeline
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cetl-0.2.8/cetl.egg-info/SOURCES.txt` & `cetl-0.2.9/cetl.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -29,30 +29,35 @@
 cetl/utils/__init__.py
 cetl/utils/airflow_pipeline.py
 cetl/utils/base.py
 cetl/utils/block.py
 cetl/utils/builder.py
 cetl/utils/dataframe.py
 cetl/utils/dot_node.py
+cetl/utils/encryption.py
 cetl/utils/file_mgt.py
 cetl/utils/formating.py
 cetl/utils/kafka.py
 cetl/utils/kafka_helper.py
 cetl/utils/kafka_media.py
 cetl/utils/pipeline.py
 cetl/utils/registry.py
 cetl/utils/samplings.py
 cetl/utils/sftp_file_mgt.py
 cetl/utils/transform_wrapper.py
 sample_user_project/__init__.py
 sample_user_project/app.py
+sample_user_project/call_api.py
+sample_user_project/compress_files.py
 sample_user_project/test_file_compress.py
 sample_user_project/file_modules/__init__.py
 sample_user_project/file_modules/builder.py
 sample_user_project/file_modules/file_compress.py
 sample_user_project/sample_modules/__init__.py
 sample_user_project/sample_modules/add_new_column.py
 sample_user_project/sample_modules/data_validation_check.py
 tests/__init__.py
+tests/example1_test_build_pipeline.py
+tests/example2_test_build_pipeline.py
 tests/test_kafka_helper.py
 tests/test_parallel_transformer.py
 tests/test_pass_dataframe.py
```

### Comparing `cetl-0.2.8/sample_user_project/app.py` & `cetl-0.2.9/sample_user_project/app.py`

 * *Files identical despite different names*

### Comparing `cetl-0.2.8/sample_user_project/sample_modules/add_new_column.py` & `cetl-0.2.9/sample_user_project/sample_modules/add_new_column.py`

 * *Files identical despite different names*

### Comparing `cetl-0.2.8/sample_user_project/sample_modules/data_validation_check.py` & `cetl-0.2.9/sample_user_project/sample_modules/data_validation_check.py`

 * *Files identical despite different names*

### Comparing `cetl-0.2.8/sample_user_project/test_file_compress.py` & `cetl-0.2.9/sample_user_project/test_file_compress.py`

 * *Files identical despite different names*

### Comparing `cetl-0.2.8/setup.py` & `cetl-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with codecs.open(os.path.join(readme_dir, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read() + "\n this version will solve the issue of UnboundLocalError: \n"+\
                         "local variable 'pre_transformer_key' referenced before assignment"
 
 # Setting up
 setup(
     name="cetl",
-    version='0.2.8',
+    version='0.2.9',
     author="Clement",
     author_email="<cheukub@gmail.com>",
     description='A basic data pipeline tools for data engineer to handle the CRM or loyalty data',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=['flask', 'SQLalchemy', 'pyspark', 'pandas'],
```

### Comparing `cetl-0.2.8/tests/test_kafka_helper.py` & `cetl-0.2.9/tests/test_kafka_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,14 @@
     # create instance of encryption
     encrypted_data = kh.fernet.encrypt(serialized_data)
     # print(encrypted_data)
 
     # send the data to kafka topic
     kh.send(key=task_id, value=encrypted_data)
 
-
     # received message
     message = kh.receive(task_id)
 
     # decrypt the message
     decrypted_data = kh.fernet.decrypt(message)
 
     # decode by pickle
```

### Comparing `cetl-0.2.8/tests/test_parallel_transformer.py` & `cetl-0.2.9/tests/test_parallel_transformer.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 def test_parallel_transformer2():
 
     answer = pd.concat([generateDataFrame().transform(""), 
                         generateDataFrame().transform("")])
     # print(answer)
 
-    cfg = {"pipeline":[ {"type":"dummyStart", "data_container_type":"functional"},
+    cfg = {"pipeline":[ {"type":"dummyStart", "module_type":"functional"},
                         {"type":"parallelTransformer", "transformers":[
                             {"type":"generateDataFrame"},
                             {"type":"generateDataFrame"}
                         ]},
                         {"type":"unionAll"}
     ]}
```

