# Comparing `tmp/ms2query-1.2.0.tar.gz` & `tmp/ms2query-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ms2query-1.2.0.tar", last modified: Tue May 23 15:41:12 2023, max compression
+gzip compressed data, was "dist/ms2query-1.2.1.tar", last modified: Tue Jun 20 14:43:37 2023, max compression
```

## Comparing `ms2query-1.2.0.tar` & `ms2query-1.2.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:41:12.000000 ms2query-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    24177 2023-05-23 15:41:12.000000 ms2query-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20873 2023-05-23 15:41:01.000000 ms2query-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:41:12.000000 ms2query-1.2.0/ms2query/
--rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-05-23 15:41:01.000000 ms2query-1.2.0/ms2query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-23 15:41:01.000000 ms2query-1.2.0/ms2query/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:41:12.000000 ms2query-1.2.0/ms2query/benchmarking/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:41:01.000000 ms2query-1.2.0/ms2query/benchmarking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21282 2023-05-23 15:41:01.000000 ms2query-1.2.0/ms2query/benchmarking/collect_test_data_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    13050 2023-05-23 15:41:01.000000 ms2query-1.2.0/ms2query/benchmarking/create_accuracy_vs_recall_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-05-23 15:41:01.000000 ms2query-1.2.0/ms2query/benchmarking/k_fold_cross_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-05-23 15:41:01.000000 ms2query-1.2.0/ms2query/benchmarking/visualize_mass_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-23 15:41:01.000000 ms2query-1.2.0/ms2query/benchmarking/visualize_tanimoto_score_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     7264 2023-05-23 15:41:01.000000 ms2query-1.2.0/ms2query/clean_and_filter_spectra.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:41:12.000000 ms2query-1.2.0/ms2query/create_new_library/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:41:01.000000 ms2query-1.2.0/ms2query/create_new_library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-05-23 15:41:01.000000 ms2query-1.2.0/ms2query/create_new_library/add_classifire_classifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-05-23 15:41:01.000000 ms2query-1.2.0/ms2query/create_new_library/calculate_tanimoto_scores.py
--rw-r--r--   0 runner    (1001) docker     (123)    10166 2023-05-23 15:41:01.000000 ms2query-1.2.0/ms2query/create_new_library/create_sqlite_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     8254 2023-05-23 15:41:01.000000 ms2query-1.2.0/ms2query/create_new_library/library_files_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-05-23 15:41:01.000000 ms2query-1.2.0/ms2query/create_new_library/split_data_for_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-05-23 15:41:01.000000 ms2query-1.2.0/ms2query/create_new_library/train_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-05-23 15:41:01.000000 ms2query-1.2.0/ms2query/create_new_library/train_ms2deepscore.py
--rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-05-23 15:41:01.000000 ms2query-1.2.0/ms2query/create_new_library/train_ms2query_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    22515 2023-05-23 15:41:01.000000 ms2query-1.2.0/ms2query/ms2library.py
--rw-r--r--   0 runner    (1001) docker     (123)    13403 2023-05-23 15:41:01.000000 ms2query-1.2.0/ms2query/old_query_from_sqlite_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-05-23 15:41:01.000000 ms2query-1.2.0/ms2query/query_from_sqlite_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     8923 2023-05-23 15:41:01.000000 ms2query-1.2.0/ms2query/results_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     6492 2023-05-23 15:41:01.000000 ms2query-1.2.0/ms2query/run_ms2query.py
--rw-r--r--   0 runner    (1001) docker     (123)    11030 2023-05-23 15:41:01.000000 ms2query-1.2.0/ms2query/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:41:12.000000 ms2query-1.2.0/ms2query.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24177 2023-05-23 15:41:11.000000 ms2query-1.2.0/ms2query.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-23 15:41:12.000000 ms2query-1.2.0/ms2query.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 15:41:11.000000 ms2query-1.2.0/ms2query.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-23 15:41:11.000000 ms2query-1.2.0/ms2query.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 15:41:11.000000 ms2query-1.2.0/ms2query.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-23 15:41:11.000000 ms2query-1.2.0/ms2query.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-23 15:41:11.000000 ms2query-1.2.0/ms2query.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-23 15:41:12.000000 ms2query-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-23 15:41:01.000000 ms2query-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:41:12.000000 ms2query-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:41:01.000000 ms2query-1.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-05-23 15:41:01.000000 ms2query-1.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-23 15:41:01.000000 ms2query-1.2.0/tests/test_add_classifier_annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-05-23 15:41:01.000000 ms2query-1.2.0/tests/test_calculate_tanimoto_scores.py
--rw-r--r--   0 runner    (1001) docker     (123)    10408 2023-05-23 15:41:01.000000 ms2query-1.2.0/tests/test_clean_and_filter_spectra.py
--rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-05-23 15:41:01.000000 ms2query-1.2.0/tests/test_collect_test_data_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-23 15:41:01.000000 ms2query-1.2.0/tests/test_library_files_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-05-23 15:41:01.000000 ms2query-1.2.0/tests/test_ms2library.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-23 15:41:01.000000 ms2query-1.2.0/tests/test_results_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-05-23 15:41:01.000000 ms2query-1.2.0/tests/test_run_ms2query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-23 15:41:01.000000 ms2query-1.2.0/tests/test_split_data_for_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-05-23 15:41:01.000000 ms2query-1.2.0/tests/test_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-23 15:41:01.000000 ms2query-1.2.0/tests/test_train_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-23 15:41:01.000000 ms2query-1.2.0/tests/test_train_ms2deepscore.py
--rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-05-23 15:41:01.000000 ms2query-1.2.0/tests/test_train_ms2query_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-05-23 15:41:01.000000 ms2query-1.2.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:43:37.000000 ms2query-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    24177 2023-06-20 14:43:37.000000 ms2query-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20873 2023-06-20 14:43:25.000000 ms2query-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:43:37.000000 ms2query-1.2.1/ms2query/
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-06-20 14:43:25.000000 ms2query-1.2.1/ms2query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-20 14:43:25.000000 ms2query-1.2.1/ms2query/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:43:37.000000 ms2query-1.2.1/ms2query/benchmarking/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:43:25.000000 ms2query-1.2.1/ms2query/benchmarking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21282 2023-06-20 14:43:25.000000 ms2query-1.2.1/ms2query/benchmarking/collect_test_data_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13050 2023-06-20 14:43:25.000000 ms2query-1.2.1/ms2query/benchmarking/create_accuracy_vs_recall_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-06-20 14:43:25.000000 ms2query-1.2.1/ms2query/benchmarking/k_fold_cross_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-06-20 14:43:25.000000 ms2query-1.2.1/ms2query/benchmarking/visualize_mass_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-06-20 14:43:25.000000 ms2query-1.2.1/ms2query/benchmarking/visualize_tanimoto_score_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7264 2023-06-20 14:43:25.000000 ms2query-1.2.1/ms2query/clean_and_filter_spectra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:43:37.000000 ms2query-1.2.1/ms2query/create_new_library/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:43:25.000000 ms2query-1.2.1/ms2query/create_new_library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-06-20 14:43:25.000000 ms2query-1.2.1/ms2query/create_new_library/add_classifire_classifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-06-20 14:43:25.000000 ms2query-1.2.1/ms2query/create_new_library/calculate_tanimoto_scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10166 2023-06-20 14:43:25.000000 ms2query-1.2.1/ms2query/create_new_library/create_sqlite_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8254 2023-06-20 14:43:25.000000 ms2query-1.2.1/ms2query/create_new_library/library_files_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-06-20 14:43:25.000000 ms2query-1.2.1/ms2query/create_new_library/split_data_for_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-06-20 14:43:25.000000 ms2query-1.2.1/ms2query/create_new_library/train_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-06-20 14:43:25.000000 ms2query-1.2.1/ms2query/create_new_library/train_ms2deepscore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-06-20 14:43:25.000000 ms2query-1.2.1/ms2query/create_new_library/train_ms2query_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22515 2023-06-20 14:43:25.000000 ms2query-1.2.1/ms2query/ms2library.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13403 2023-06-20 14:43:25.000000 ms2query-1.2.1/ms2query/old_query_from_sqlite_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-06-20 14:43:25.000000 ms2query-1.2.1/ms2query/query_from_sqlite_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8923 2023-06-20 14:43:25.000000 ms2query-1.2.1/ms2query/results_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6492 2023-06-20 14:43:25.000000 ms2query-1.2.1/ms2query/run_ms2query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11030 2023-06-20 14:43:25.000000 ms2query-1.2.1/ms2query/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:43:37.000000 ms2query-1.2.1/ms2query.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24177 2023-06-20 14:43:37.000000 ms2query-1.2.1/ms2query.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-20 14:43:37.000000 ms2query-1.2.1/ms2query.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 14:43:37.000000 ms2query-1.2.1/ms2query.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-20 14:43:37.000000 ms2query-1.2.1/ms2query.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 14:43:37.000000 ms2query-1.2.1/ms2query.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-20 14:43:37.000000 ms2query-1.2.1/ms2query.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 14:43:37.000000 ms2query-1.2.1/ms2query.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-20 14:43:37.000000 ms2query-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-20 14:43:25.000000 ms2query-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:43:37.000000 ms2query-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:43:25.000000 ms2query-1.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-06-20 14:43:25.000000 ms2query-1.2.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-20 14:43:25.000000 ms2query-1.2.1/tests/test_add_classifier_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-06-20 14:43:25.000000 ms2query-1.2.1/tests/test_calculate_tanimoto_scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10408 2023-06-20 14:43:25.000000 ms2query-1.2.1/tests/test_clean_and_filter_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-06-20 14:43:25.000000 ms2query-1.2.1/tests/test_collect_test_data_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-06-20 14:43:26.000000 ms2query-1.2.1/tests/test_library_files_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-06-20 14:43:26.000000 ms2query-1.2.1/tests/test_ms2library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-20 14:43:26.000000 ms2query-1.2.1/tests/test_results_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-06-20 14:43:26.000000 ms2query-1.2.1/tests/test_run_ms2query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-06-20 14:43:26.000000 ms2query-1.2.1/tests/test_split_data_for_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-06-20 14:43:26.000000 ms2query-1.2.1/tests/test_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-20 14:43:26.000000 ms2query-1.2.1/tests/test_train_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-20 14:43:26.000000 ms2query-1.2.1/tests/test_train_ms2deepscore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-06-20 14:43:26.000000 ms2query-1.2.1/tests/test_train_ms2query_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-06-20 14:43:26.000000 ms2query-1.2.1/tests/test_utils.py
```

### Comparing `ms2query-1.2.0/PKG-INFO` & `ms2query-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms2query
-Version: 1.2.0
+Version: 1.2.1
 Summary: Tool to query MS/MS spectra against mass spectral library
 Home-page: https://github.com/iomega/ms2query
 Author: Netherlands eScience Center
 Author-email: 
 License: Apache Software License 2.0
 Description: [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/iomega/ms2query/CI_build.yml)](https://github.com/iomega/ms2query/actions/workflows/CI_build.yml)
         ![GitHub](https://img.shields.io/github/license/iomega/ms2query)
```

### Comparing `ms2query-1.2.0/README.md` & `ms2query-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.0/ms2query/__init__.py` & `ms2query-1.2.1/ms2query/__init__.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.0/ms2query/benchmarking/collect_test_data_results.py` & `ms2query-1.2.1/ms2query/benchmarking/collect_test_data_results.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.0/ms2query/benchmarking/create_accuracy_vs_recall_plot.py` & `ms2query-1.2.1/ms2query/benchmarking/create_accuracy_vs_recall_plot.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.0/ms2query/benchmarking/k_fold_cross_validation.py` & `ms2query-1.2.1/ms2query/benchmarking/k_fold_cross_validation.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.0/ms2query/benchmarking/visualize_mass_distribution.py` & `ms2query-1.2.1/ms2query/benchmarking/visualize_mass_distribution.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.0/ms2query/benchmarking/visualize_tanimoto_score_distribution.py` & `ms2query-1.2.1/ms2query/benchmarking/visualize_tanimoto_score_distribution.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.0/ms2query/clean_and_filter_spectra.py` & `ms2query-1.2.1/ms2query/clean_and_filter_spectra.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.0/ms2query/create_new_library/add_classifire_classifications.py` & `ms2query-1.2.1/ms2query/create_new_library/add_classifire_classifications.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.0/ms2query/create_new_library/calculate_tanimoto_scores.py` & `ms2query-1.2.1/ms2query/create_new_library/calculate_tanimoto_scores.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.0/ms2query/create_new_library/create_sqlite_database.py` & `ms2query-1.2.1/ms2query/create_new_library/create_sqlite_database.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.0/ms2query/create_new_library/library_files_creator.py` & `ms2query-1.2.1/ms2query/create_new_library/library_files_creator.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.0/ms2query/create_new_library/split_data_for_training.py` & `ms2query-1.2.1/ms2query/create_new_library/split_data_for_training.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.0/ms2query/create_new_library/train_models.py` & `ms2query-1.2.1/ms2query/create_new_library/train_models.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.0/ms2query/create_new_library/train_ms2deepscore.py` & `ms2query-1.2.1/ms2query/create_new_library/train_ms2deepscore.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.0/ms2query/create_new_library/train_ms2query_model.py` & `ms2query-1.2.1/ms2query/create_new_library/train_ms2query_model.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.0/ms2query/ms2library.py` & `ms2query-1.2.1/ms2query/ms2library.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.0/ms2query/old_query_from_sqlite_functions.py` & `ms2query-1.2.1/ms2query/old_query_from_sqlite_functions.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.0/ms2query/query_from_sqlite_database.py` & `ms2query-1.2.1/ms2query/query_from_sqlite_database.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.0/ms2query/results_table.py` & `ms2query-1.2.1/ms2query/results_table.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.0/ms2query/run_ms2query.py` & `ms2query-1.2.1/ms2query/run_ms2query.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from urllib.request import urlopen, urlretrieve
 from ms2query.ms2library import MS2Library
 from ms2query.utils import load_matchms_spectrum_objects_from_file, SettingsRunMS2Query, return_non_existing_file_name
 
 
 def zenodo_dois(ionisation_mode):
     "Returns the most up to date url for Zenodo"
-    zenodo_DOIs = {"positive": 6124552,
-                   "negative": 7104184}
+    zenodo_DOIs = {"positive": 7947603,
+                   "negative": 7944658}
     assert ionisation_mode in zenodo_DOIs, "Expected 'positive' or 'negative' as input"
     zenodo_doi = zenodo_DOIs[ionisation_mode]
     zenodo_metadata_url = "https://zenodo.org/api/records/" + str(zenodo_doi)
     zenodo_files_url = f"https://zenodo.org/record/{zenodo_doi}/files/"
     return zenodo_metadata_url, zenodo_files_url
```

### Comparing `ms2query-1.2.0/ms2query/utils.py` & `ms2query-1.2.1/ms2query/utils.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.0/ms2query.egg-info/PKG-INFO` & `ms2query-1.2.1/ms2query.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms2query
-Version: 1.2.0
+Version: 1.2.1
 Summary: Tool to query MS/MS spectra against mass spectral library
 Home-page: https://github.com/iomega/ms2query
 Author: Netherlands eScience Center
 Author-email: 
 License: Apache Software License 2.0
 Description: [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/iomega/ms2query/CI_build.yml)](https://github.com/iomega/ms2query/actions/workflows/CI_build.yml)
         ![GitHub](https://img.shields.io/github/license/iomega/ms2query)
```

### Comparing `ms2query-1.2.0/ms2query.egg-info/SOURCES.txt` & `ms2query-1.2.1/ms2query.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.0/setup.py` & `ms2query-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.0/tests/conftest.py` & `ms2query-1.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.0/tests/test_add_classifier_annotations.py` & `ms2query-1.2.1/tests/test_add_classifier_annotations.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.0/tests/test_calculate_tanimoto_scores.py` & `ms2query-1.2.1/tests/test_calculate_tanimoto_scores.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.0/tests/test_clean_and_filter_spectra.py` & `ms2query-1.2.1/tests/test_clean_and_filter_spectra.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.0/tests/test_collect_test_data_results.py` & `ms2query-1.2.1/tests/test_collect_test_data_results.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.0/tests/test_library_files_creator.py` & `ms2query-1.2.1/tests/test_library_files_creator.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.0/tests/test_ms2library.py` & `ms2query-1.2.1/tests/test_ms2library.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.0/tests/test_results_table.py` & `ms2query-1.2.1/tests/test_results_table.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.0/tests/test_run_ms2query.py` & `ms2query-1.2.1/tests/test_run_ms2query.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.0/tests/test_split_data_for_training.py` & `ms2query-1.2.1/tests/test_split_data_for_training.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.0/tests/test_sqlite.py` & `ms2query-1.2.1/tests/test_sqlite.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.0/tests/test_train_models.py` & `ms2query-1.2.1/tests/test_train_models.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.0/tests/test_train_ms2deepscore.py` & `ms2query-1.2.1/tests/test_train_ms2deepscore.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.0/tests/test_train_ms2query_model.py` & `ms2query-1.2.1/tests/test_train_ms2query_model.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.0/tests/test_utils.py` & `ms2query-1.2.1/tests/test_utils.py`

 * *Files identical despite different names*

