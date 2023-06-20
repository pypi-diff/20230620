# Comparing `tmp/philologic-4.7.4.tar.gz` & `tmp/philologic-4.7.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "philologic-4.7.4.tar", last modified: Fri Feb 17 19:27:17 2023, max compression
+gzip compressed data, was "philologic-4.7.4.1.tar", last modified: Tue Jun 20 16:13:28 2023, max compression
```

## Comparing `philologic-4.7.4.tar` & `philologic-4.7.4.1.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 clovis    (1000) artfl     (1003)        0 2023-02-17 19:27:17.029771 philologic-4.7.4/
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)    35141 2022-11-22 20:47:37.000000 philologic-4.7.4/LICENSE
--rw-r--r--   0 clovis    (1000) artfl     (1003)      744 2023-02-17 19:27:17.029771 philologic-4.7.4/PKG-INFO
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)      428 2022-11-22 16:01:26.000000 philologic-4.7.4/README
-drwxr-xr-x   0 clovis    (1000) artfl     (1003)        0 2023-02-17 19:27:17.025771 philologic-4.7.4/philologic/
--rw-r--r--   0 clovis    (1000) artfl     (1003)    36981 2022-12-05 22:36:45.000000 philologic-4.7.4/philologic/Config.py
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)     4469 2022-11-22 16:35:28.000000 philologic-4.7.4/philologic/TagCensus.py
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)      101 2022-11-22 20:47:37.000000 philologic-4.7.4/philologic/__init__.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)      181 2022-11-22 21:05:10.000000 philologic-4.7.4/philologic/_version.py
-drwxr-xr-x   0 clovis    (1000) artfl     (1003)        0 2023-02-17 19:27:17.029771 philologic-4.7.4/philologic/loadtime/
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)    17283 2022-11-22 16:35:28.000000 philologic-4.7.4/philologic/loadtime/LoadFilters.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)    10528 2022-11-24 20:03:41.000000 philologic-4.7.4/philologic/loadtime/LoadOptions.py
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)    42023 2022-12-06 18:52:59.000000 philologic-4.7.4/philologic/loadtime/Loader.py
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)    13674 2023-02-07 19:21:46.000000 philologic-4.7.4/philologic/loadtime/OHCOVector.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)    72525 2022-12-05 20:57:11.000000 philologic-4.7.4/philologic/loadtime/Parser.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     8083 2023-02-07 19:21:34.000000 philologic-4.7.4/philologic/loadtime/PlainTextParser.py
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)    10277 2022-11-28 14:46:21.000000 philologic-4.7.4/philologic/loadtime/PostFilters.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)       49 2022-11-22 16:35:28.000000 philologic-4.7.4/philologic/loadtime/__init__.py
-drwxr-xr-x   0 clovis    (1000) artfl     (1003)        0 2023-02-17 19:27:17.029771 philologic-4.7.4/philologic/runtime/
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)     9410 2022-11-22 16:35:28.000000 philologic-4.7.4/philologic/runtime/DB.py
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)     3776 2022-11-22 16:35:28.000000 philologic-4.7.4/philologic/runtime/FragmentParser.py
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)     9822 2022-11-22 16:35:28.000000 philologic-4.7.4/philologic/runtime/HitList.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     6768 2022-11-22 16:35:28.000000 philologic-4.7.4/philologic/runtime/HitWrapper.py
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)    12990 2022-11-22 16:35:28.000000 philologic-4.7.4/philologic/runtime/MetadataQuery.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)    30583 2023-01-12 15:09:56.000000 philologic-4.7.4/philologic/runtime/ObjectFormatter.py
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)     9792 2022-11-22 16:35:28.000000 philologic-4.7.4/philologic/runtime/Query.py
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)     3493 2022-11-22 16:35:28.000000 philologic-4.7.4/philologic/runtime/QuerySyntax.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     7458 2022-12-19 19:58:22.000000 philologic-4.7.4/philologic/runtime/WSGIHandler.py
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)      951 2022-11-22 16:35:28.000000 philologic-4.7.4/philologic/runtime/__init__.py
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)     6071 2022-11-22 16:35:28.000000 philologic-4.7.4/philologic/runtime/access_control.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     5693 2022-11-22 16:35:28.000000 philologic-4.7.4/philologic/runtime/citations.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)      511 2022-11-22 16:35:28.000000 philologic-4.7.4/philologic/runtime/collocation_scores.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     2412 2022-11-22 16:35:28.000000 philologic-4.7.4/philologic/runtime/find_similar_words.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     3811 2022-11-22 16:35:28.000000 philologic-4.7.4/philologic/runtime/get_text.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     2956 2022-12-09 02:32:30.000000 philologic-4.7.4/philologic/runtime/link.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)      413 2022-11-22 16:35:28.000000 philologic-4.7.4/philologic/runtime/pages.py
-drwxr-xr-x   0 clovis    (1000) artfl     (1003)        0 2023-02-17 19:27:17.029771 philologic-4.7.4/philologic/runtime/reports/
--rw-r--r--   0 clovis    (1000) artfl     (1003)      977 2022-11-22 16:35:28.000000 philologic-4.7.4/philologic/runtime/reports/__init__.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     7673 2022-11-22 16:35:28.000000 philologic-4.7.4/philologic/runtime/reports/aggregation.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     3242 2022-12-19 22:17:21.000000 philologic-4.7.4/philologic/runtime/reports/bibliography.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     5332 2022-12-05 22:33:58.000000 philologic-4.7.4/philologic/runtime/reports/collocation.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     2712 2022-11-22 16:35:28.000000 philologic-4.7.4/philologic/runtime/reports/concordance.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     2627 2022-11-22 16:35:28.000000 philologic-4.7.4/philologic/runtime/reports/filter_word_by_property.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     7830 2022-11-22 16:35:28.000000 philologic-4.7.4/philologic/runtime/reports/frequency.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     2507 2022-11-22 16:35:28.000000 philologic-4.7.4/philologic/runtime/reports/generate_word_frequency.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     3349 2022-11-22 16:35:28.000000 philologic-4.7.4/philologic/runtime/reports/kwic.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     7425 2022-11-22 16:35:28.000000 philologic-4.7.4/philologic/runtime/reports/landing_page.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     3074 2022-11-22 16:35:28.000000 philologic-4.7.4/philologic/runtime/reports/navigation.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     3870 2022-11-22 16:35:28.000000 philologic-4.7.4/philologic/runtime/reports/table_of_contents.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     4925 2022-11-22 16:35:28.000000 philologic-4.7.4/philologic/runtime/reports/time_series.py
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)      894 2022-11-22 16:35:28.000000 philologic-4.7.4/philologic/runtime/web_config.py
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)     6167 2022-11-22 16:35:28.000000 philologic-4.7.4/philologic/shlax.py
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)     8793 2022-11-22 16:35:28.000000 philologic-4.7.4/philologic/shlaxtree.py
-drwxr-xr-x   0 clovis    (1000) artfl     (1003)        0 2023-02-17 19:27:17.029771 philologic-4.7.4/philologic/utils/
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)      221 2022-11-22 16:35:28.000000 philologic-4.7.4/philologic/utils/__init__.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)      762 2022-11-22 16:35:28.000000 philologic-4.7.4/philologic/utils/convert_entities.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)      430 2022-11-22 16:35:28.000000 philologic-4.7.4/philologic/utils/load_module.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     1929 2022-11-22 16:35:28.000000 philologic-4.7.4/philologic/utils/metadata_type_handler.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     1113 2022-11-22 16:35:28.000000 philologic-4.7.4/philologic/utils/pretty_print.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)      581 2022-11-22 16:35:28.000000 philologic-4.7.4/philologic/utils/sort.py
-drwxr-xr-x   0 clovis    (1000) artfl     (1003)        0 2023-02-17 19:27:17.029771 philologic-4.7.4/philologic.egg-info/
--rw-r--r--   0 clovis    (1000) artfl     (1003)      744 2023-02-17 19:27:16.000000 philologic-4.7.4/philologic.egg-info/PKG-INFO
--rw-r--r--   0 clovis    (1000) artfl     (1003)     1975 2023-02-17 19:27:17.000000 philologic-4.7.4/philologic.egg-info/SOURCES.txt
--rw-r--r--   0 clovis    (1000) artfl     (1003)        1 2023-02-17 19:27:16.000000 philologic-4.7.4/philologic.egg-info/dependency_links.txt
--rw-r--r--   0 clovis    (1000) artfl     (1003)       91 2023-02-17 19:27:16.000000 philologic-4.7.4/philologic.egg-info/requires.txt
--rw-r--r--   0 clovis    (1000) artfl     (1003)       11 2023-02-17 19:27:16.000000 philologic-4.7.4/philologic.egg-info/top_level.txt
-drwxr-xr-x   0 clovis    (1000) artfl     (1003)        0 2023-02-17 19:27:17.029771 philologic-4.7.4/scripts/
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)     1361 2022-11-22 17:21:51.000000 philologic-4.7.4/scripts/philoload4
--rw-r--r--   0 clovis    (1000) artfl     (1003)       38 2023-02-17 19:27:17.029771 philologic-4.7.4/setup.cfg
--rw-r--r--   0 clovis    (1000) artfl     (1003)     1137 2022-11-30 18:18:41.000000 philologic-4.7.4/setup.py
+drwxr-xr-x   0 clovis    (1000) artfl     (1003)        0 2023-06-20 16:13:28.603805 philologic-4.7.4.1/
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)    35141 2022-11-22 20:47:37.000000 philologic-4.7.4.1/LICENSE
+-rw-r--r--   0 clovis    (1000) artfl     (1003)      746 2023-06-20 16:13:28.603805 philologic-4.7.4.1/PKG-INFO
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)      428 2022-11-22 16:01:26.000000 philologic-4.7.4.1/README
+drwxr-xr-x   0 clovis    (1000) artfl     (1003)        0 2023-06-20 16:13:28.599805 philologic-4.7.4.1/philologic/
+-rw-r--r--   0 clovis    (1000) artfl     (1003)    36981 2022-12-05 22:36:45.000000 philologic-4.7.4.1/philologic/Config.py
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)     4469 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/TagCensus.py
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)      101 2022-11-22 20:47:37.000000 philologic-4.7.4.1/philologic/__init__.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)      181 2022-11-22 21:05:10.000000 philologic-4.7.4.1/philologic/_version.py
+drwxr-xr-x   0 clovis    (1000) artfl     (1003)        0 2023-06-20 16:13:28.599805 philologic-4.7.4.1/philologic/loadtime/
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)    17283 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/loadtime/LoadFilters.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)    10528 2022-11-24 20:03:41.000000 philologic-4.7.4.1/philologic/loadtime/LoadOptions.py
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)    42023 2022-12-06 18:52:59.000000 philologic-4.7.4.1/philologic/loadtime/Loader.py
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)    13674 2023-02-07 19:21:46.000000 philologic-4.7.4.1/philologic/loadtime/OHCOVector.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)    72525 2022-12-05 20:57:11.000000 philologic-4.7.4.1/philologic/loadtime/Parser.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     8083 2023-02-07 19:21:34.000000 philologic-4.7.4.1/philologic/loadtime/PlainTextParser.py
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)    10370 2023-03-04 17:27:17.000000 philologic-4.7.4.1/philologic/loadtime/PostFilters.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)       49 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/loadtime/__init__.py
+drwxr-xr-x   0 clovis    (1000) artfl     (1003)        0 2023-06-20 16:13:28.603805 philologic-4.7.4.1/philologic/runtime/
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)     9410 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/runtime/DB.py
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)     3776 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/runtime/FragmentParser.py
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)     9822 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/runtime/HitList.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     6768 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/runtime/HitWrapper.py
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)    12990 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/runtime/MetadataQuery.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)    31759 2023-06-20 15:58:40.000000 philologic-4.7.4.1/philologic/runtime/ObjectFormatter.py
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)     9792 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/runtime/Query.py
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)     3493 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/runtime/QuerySyntax.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     7458 2022-12-19 19:58:22.000000 philologic-4.7.4.1/philologic/runtime/WSGIHandler.py
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)      951 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/runtime/__init__.py
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)     6071 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/runtime/access_control.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     5693 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/runtime/citations.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)      511 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/runtime/collocation_scores.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     2412 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/runtime/find_similar_words.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     4044 2023-06-20 14:24:18.000000 philologic-4.7.4.1/philologic/runtime/get_text.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     2956 2022-12-09 02:32:30.000000 philologic-4.7.4.1/philologic/runtime/link.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)      413 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/runtime/pages.py
+drwxr-xr-x   0 clovis    (1000) artfl     (1003)        0 2023-06-20 16:13:28.603805 philologic-4.7.4.1/philologic/runtime/reports/
+-rw-r--r--   0 clovis    (1000) artfl     (1003)      977 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/runtime/reports/__init__.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     7673 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/runtime/reports/aggregation.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     3242 2022-12-19 22:17:21.000000 philologic-4.7.4.1/philologic/runtime/reports/bibliography.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     5332 2022-12-05 22:33:58.000000 philologic-4.7.4.1/philologic/runtime/reports/collocation.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     2712 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/runtime/reports/concordance.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     2627 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/runtime/reports/filter_word_by_property.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     7830 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/runtime/reports/frequency.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     2507 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/runtime/reports/generate_word_frequency.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     3349 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/runtime/reports/kwic.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     7425 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/runtime/reports/landing_page.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     3074 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/runtime/reports/navigation.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     3870 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/runtime/reports/table_of_contents.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     4925 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/runtime/reports/time_series.py
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)      894 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/runtime/web_config.py
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)     6167 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/shlax.py
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)     8793 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/shlaxtree.py
+drwxr-xr-x   0 clovis    (1000) artfl     (1003)        0 2023-06-20 16:13:28.603805 philologic-4.7.4.1/philologic/utils/
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)      221 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/utils/__init__.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)      762 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/utils/convert_entities.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)      430 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/utils/load_module.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     1929 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/utils/metadata_type_handler.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     1113 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/utils/pretty_print.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)      581 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/utils/sort.py
+drwxr-xr-x   0 clovis    (1000) artfl     (1003)        0 2023-06-20 16:13:28.599805 philologic-4.7.4.1/philologic.egg-info/
+-rw-r--r--   0 clovis    (1000) artfl     (1003)      746 2023-06-20 16:13:28.000000 philologic-4.7.4.1/philologic.egg-info/PKG-INFO
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     1975 2023-06-20 16:13:28.000000 philologic-4.7.4.1/philologic.egg-info/SOURCES.txt
+-rw-r--r--   0 clovis    (1000) artfl     (1003)        1 2023-06-20 16:13:28.000000 philologic-4.7.4.1/philologic.egg-info/dependency_links.txt
+-rw-r--r--   0 clovis    (1000) artfl     (1003)       91 2023-06-20 16:13:28.000000 philologic-4.7.4.1/philologic.egg-info/requires.txt
+-rw-r--r--   0 clovis    (1000) artfl     (1003)       11 2023-06-20 16:13:28.000000 philologic-4.7.4.1/philologic.egg-info/top_level.txt
+drwxr-xr-x   0 clovis    (1000) artfl     (1003)        0 2023-06-20 16:13:28.603805 philologic-4.7.4.1/scripts/
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)     1361 2022-11-22 17:21:51.000000 philologic-4.7.4.1/scripts/philoload4
+-rw-r--r--   0 clovis    (1000) artfl     (1003)       38 2023-06-20 16:13:28.603805 philologic-4.7.4.1/setup.cfg
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     1137 2022-11-30 18:18:41.000000 philologic-4.7.4.1/setup.py
```

### Comparing `philologic-4.7.4/LICENSE` & `philologic-4.7.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4/PKG-INFO` & `philologic-4.7.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: philologic
-Version: 4.7.4
+Version: 4.7.4.1
 Summary: A concordance search engine for TEI-XML
 Home-page: https://github.com/ARTFL-Project/PhiloLogic4
 Author: Clovis Gladstone
 Author-email: clovisgladstone@artfl.uchicago.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: philologic Version: 4.7.4 Summary: A concordance
+Metadata-Version: 2.1 Name: philologic Version: 4.7.4.1 Summary: A concordance
 search engine for TEI-XML Home-page: https://github.com/ARTFL-Project/
 PhiloLogic4 Author: Clovis Gladstone Author-email:
 clovisgladstone@artfl.uchicago.edu License: UNKNOWN Platform: UNKNOWN Requires-
 Python: >=3.8 License-File: LICENSE These are the Python bindings for the
 PhiloLogic search engine. This package is only useful for the TEI Parser which
 you can import for use outside of PhiloLogic. To get the full functionality of
 PhiloLogic, you need to install the search core as well as the web components.
```

### Comparing `philologic-4.7.4/philologic/Config.py` & `philologic-4.7.4.1/philologic/Config.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4/philologic/TagCensus.py` & `philologic-4.7.4.1/philologic/TagCensus.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4/philologic/loadtime/LoadFilters.py` & `philologic-4.7.4.1/philologic/loadtime/LoadFilters.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4/philologic/loadtime/LoadOptions.py` & `philologic-4.7.4.1/philologic/loadtime/LoadOptions.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4/philologic/loadtime/Loader.py` & `philologic-4.7.4.1/philologic/loadtime/Loader.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4/philologic/loadtime/OHCOVector.py` & `philologic-4.7.4.1/philologic/loadtime/OHCOVector.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4/philologic/loadtime/Parser.py` & `philologic-4.7.4.1/philologic/loadtime/Parser.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4/philologic/loadtime/PlainTextParser.py` & `philologic-4.7.4.1/philologic/loadtime/PlainTextParser.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4/philologic/loadtime/PostFilters.py` & `philologic-4.7.4.1/philologic/loadtime/PostFilters.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,14 +96,15 @@
             cursor.execute("CREATE TABLE IF NOT EXISTS sentences(philo_id text, words blob)")
             line_count = sum(
                 sum(1 for _ in lz4.frame.open(raw_words.path))
                 for raw_words in os.scandir(f"{datadir}/words_and_philo_ids")
             )
             with tqdm(total=line_count, leave=False) as pbar:
                 for raw_words in os.scandir(f"{datadir}/words_and_philo_ids"):
+                    sentence_id = ""
                     with lz4.frame.open(raw_words.path) as input_file:
                         current_sentence = None
                         words = []
                         for line in input_file:
                             word_obj = loads(line.decode("utf8"))
                             if word_obj["philo_type"] == "word":
                                 sentence_id = " ".join(word_obj["position"].split()[:6]) + " 0"
@@ -113,18 +114,19 @@
                                             "insert into sentences values(?, ?)",
                                             (current_sentence, lz4.frame.compress(msgpack.dumps(words))),
                                         )
                                         words = []
                                     current_sentence = sentence_id
                                 words.append({"word": word_obj["token"], "start_byte": word_obj["start_byte"]})
                             pbar.update()
-                        cursor.execute(  # insert last sentence in doc
-                            "insert into sentences values(?, ?)",
-                            (sentence_id, lz4.frame.compress(msgpack.dumps(words))),
-                        )
+                        if sentence_id:
+                            cursor.execute(  # insert last sentence in doc
+                                "insert into sentences values(?, ?)",
+                                (sentence_id, lz4.frame.compress(msgpack.dumps(words))),
+                            )
             cursor.execute("create index sentence_index on sentences (philo_id)")
             conn.commit()
 
     return inner_make_sentences
 
 
 def word_frequencies(loader_obj):
```

### Comparing `philologic-4.7.4/philologic/runtime/DB.py` & `philologic-4.7.4.1/philologic/runtime/DB.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4/philologic/runtime/FragmentParser.py` & `philologic-4.7.4.1/philologic/runtime/FragmentParser.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4/philologic/runtime/HitList.py` & `philologic-4.7.4.1/philologic/runtime/HitList.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4/philologic/runtime/HitWrapper.py` & `philologic-4.7.4.1/philologic/runtime/HitWrapper.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4/philologic/runtime/MetadataQuery.py` & `philologic-4.7.4.1/philologic/runtime/MetadataQuery.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4/philologic/runtime/ObjectFormatter.py` & `philologic-4.7.4.1/philologic/runtime/ObjectFormatter.py`

 * *Files 3% similar despite different names*

```diff
@@ -369,34 +369,37 @@
                 el.tag = "span"
                 el.attrib["class"] = "xml-q"
             elif el.tag == "table":
                 el.tag = "span"
                 el.attrib["class"] = "xml-table"
             elif el.tag == "ref" or el.tag == "xref":
                 if el.attrib["type"] == "note" or el.attrib["type"] == "footnote":
-                    target = el.attrib["target"]
-                    link = make_absolute_query_link(config, request, script_name="/scripts/get_notes.py", target=target)
-                    if "n" in el.attrib:
-                        el.text = el.attrib["n"]
-                    else:
-                        el.text = "*"
-                    if el.text == "":
-                        el.text = "*"
-                    el.tag = "span"
-                    el.attrib["data-ref"] = link
-                    el.attrib["id"] = target.replace("#", "") + "-link-back"
-                    # attributes for popover note
-                    el.attrib["class"] = "note-ref"
-                    el.attrib["tabindex"] = "0"
-                    el.attrib["data-toggle"] = "popover"
-                    el.attrib["data-container"] = "body"
-                    el.attrib["data-placement"] = "right"
-                    el.attrib["data-trigger"] = "focus"
-                    el.attrib["data-html"] = "true"
-                    el.attrib["data-animation"] = "true"
+                    if "target" in el.attrib:
+                        target = el.attrib["target"]
+                        link = make_absolute_query_link(
+                            config, request, script_name="/scripts/get_notes.py", target=target
+                        )
+                        if "n" in el.attrib:
+                            el.text = el.attrib["n"]
+                        else:
+                            el.text = "*"
+                        if el.text == "":
+                            el.text = "*"
+                        el.tag = "span"
+                        el.attrib["data-ref"] = link
+                        el.attrib["id"] = target.replace("#", "") + "-link-back"
+                        # attributes for popover note
+                        el.attrib["class"] = "note-ref"
+                        el.attrib["tabindex"] = "0"
+                        el.attrib["data-toggle"] = "popover"
+                        el.attrib["data-container"] = "body"
+                        el.attrib["data-placement"] = "right"
+                        el.attrib["data-trigger"] = "focus"
+                        el.attrib["data-html"] = "true"
+                        el.attrib["data-animation"] = "true"
                 elif el.attrib["type"] == "cross":
                     c.execute("SELECT philo_id FROM toms WHERE id=? LIMIT 1", (el.attrib["target"],))
                     try:
                         object_id = c.fetchone()[0]
                     except IndexError:
                         el.tag = "span"
                         continue
@@ -585,44 +588,70 @@
                 elif el.tail:
                     text_element_wrapper = create_element(
                         f"""<span class="passage-{passage_number}" n="{passage_number}">{el.tail[:]}</span>"""
                     )
                     el.tail = ""
                     parent = el.getparent()
                     parent.insert(parent.index(el) + 1, text_element_wrapper)
+
         except Exception as exception:
             pass
 
     if start_end_pairs:
         # Make sure we did not miss element tails
+        in_passage = True
+        n_marker = ""
         for el in xml.iter():
             match = False
             class_name = ""
-            n = ""
+            if "class" in el.attrib and el.attrib["class"] == "passage-marker":
+                in_passage = True
+                n_marker = el.attrib["n"]
+                continue
+            elif "id" in el.attrib and el.attrib["id"].startswith("end-passage"):
+                in_passage = False
+                continue
             for child in el:
                 if "class" in child.attrib and child.attrib["class"].startswith("passage-"):
                     if el.tail:
                         match = True
                         class_name = child.attrib["class"]
-                        n = child.attrib["n"]
+                        try:
+                            n_marker = child.attrib["n"]
+                        except KeyError:
+                            pass
                     if "id " in child.attrib and child.attrib["id"].startswith("end-passage-"):
                         match = False
             if match:
                 if isinstance(el.tail, str) and el.tail.strip():
-                    text_element_wrapper = create_element(f"""<span class="{class_name}" n="{n}">{el.tail[:]}</span>""")
+                    text_element_wrapper = create_element(
+                        f"""<span class="{class_name}" n="{n_marker}">{el.tail[:]}</span>"""
+                    )
                     el.tail = ""
                     parent = el.getparent()
                     parent.insert(parent.index(el) + 1, text_element_wrapper)
+            if in_passage is True and el.tail:
+                text_element_wrapper = create_element(
+                    f"""<span class="passage-{n_marker}" n="{n_marker}">{el.tail[:]}</span>"""
+                )
+                el.tail = ""
+                parent = el.getparent()
+                parent.insert(parent.index(el) + 1, text_element_wrapper)
         # Make sure we do not have trailing spans after end marker
         passages_done = set()
         for el in xml.iter():
             if "id" in el.attrib and el.attrib["id"].startswith("end-passage"):
                 passages_done.add(el.attrib["n"])
                 continue
-            if "class" in el.attrib and el.attrib["class"].startswith("passage") and el.attrib["n"] in passages_done:
+            if all(("n" in el.attrib, "class" in el.attrib)) and all(
+                (
+                    el.attrib["class"].startswith("passage"),
+                    el.attrib["n"] in passages_done,
+                )
+            ):
                 del el.attrib["class"]
                 del el.attrib["n"]
 
     output = etree.tostring(xml, encoding="unicode")
     output = convert_entities(output)
 
     if note:  ## Notes don't need to fetch images
```

### Comparing `philologic-4.7.4/philologic/runtime/Query.py` & `philologic-4.7.4.1/philologic/runtime/Query.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4/philologic/runtime/QuerySyntax.py` & `philologic-4.7.4.1/philologic/runtime/QuerySyntax.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4/philologic/runtime/WSGIHandler.py` & `philologic-4.7.4.1/philologic/runtime/WSGIHandler.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4/philologic/runtime/__init__.py` & `philologic-4.7.4.1/philologic/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4/philologic/runtime/access_control.py` & `philologic-4.7.4.1/philologic/runtime/access_control.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4/philologic/runtime/citations.py` & `philologic-4.7.4.1/philologic/runtime/citations.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4/philologic/runtime/find_similar_words.py` & `philologic-4.7.4.1/philologic/runtime/find_similar_words.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4/philologic/runtime/get_text.py` & `philologic-4.7.4.1/philologic/runtime/get_text.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,38 +7,41 @@
 from philologic.runtime.DB import DB
 from philologic.runtime.HitWrapper import ObjectWrapper
 
 from .ObjectFormatter import adjust_bytes, format_concordance, format_text_object
 
 
 def get_text(hit, start_byte, length, path):
+    """Returns the text of a hit as a string."""
     file_path = path + "/data/TEXT/" + hit.doc.filename
     with open(file_path, "rb") as text_file:
         text_file.seek(start_byte)
         return text_file.read(length)
 
 
 def get_concordance_text(db, hit, path, context_size):
-    ## Determine length of text needed
+    """Returns the text of a concordance as a string."""
+    # Determine length of text needed
     byte_offsets = sorted(hit.bytes)
     byte_distance = byte_offsets[-1] - byte_offsets[0]
     length = context_size + byte_distance + context_size
     byte_offsets, start_byte = adjust_bytes(byte_offsets, context_size)
     conc_text = get_text(hit, start_byte, length, path)
     conc_text = format_concordance(conc_text, db.locals["token_regex"], byte_offsets)
     return conc_text
 
 
 def get_text_obj(obj, config, request, word_regex, note=False, images=True):
+    """Returns the text of an object as a string, formatted according to the request parameters."""
     path = config.db_path
     filename = obj.doc.filename
     if filename and os.path.exists(path + "/data/TEXT/" + filename):
         path += "/data/TEXT/" + filename
     else:
-        ## workaround for when no filename is returned with the full philo_id of the object
+        # workaround for when no filename is returned with the full philo_id of the object
         philo_id = str(obj.philo_id[0]) + " 0 0 0 0 0 0"
         c = obj.db.dbh.cursor()
         c.execute("select filename from toms where philo_type='doc' and philo_id =? limit 1", (philo_id,))
         path += "/data/TEXT/" + c.fetchone()["filename"]
     with open(path, "rb") as file:
         obj_start_byte = int(obj.start_byte)
         file.seek(obj_start_byte)
@@ -73,25 +76,25 @@
     if images:
         return formatted_text, imgs
     else:
         return formatted_text
 
 
 def get_tei_header(request, config):
+    """Returns the TEI header of a text as a string."""
     path = config.db_path
     db = DB(path + "/data")
     obj = ObjectWrapper(request["philo_id"].split(), db)
     filename = path + "/data/TEXT/" + obj.filename
     parser = etree.XMLParser(remove_blank_text=True, recover=True)
     xml_tree = etree.parse(filename, parser)
     header = xml_tree.find("teiHeader")
     try:
         header_text = etree.tostring(header, pretty_print=True).decode("utf8")
-    except TypeError as e:  # workaround for when lxml doesn't find the header for whatever reason
-        start = False
+    except TypeError:  # workaround for when lxml doesn't find the header for whatever reason
         header_text = ""
         with open(filename, encoding="utf8") as file:
             file_content = file.read()
             try:
                 start_header_index = re.search(r"<teiheader", file_content, re.I).start()
                 end_header_index = re.search(r"</teiheader>", file_content, re.I).end()
             except AttributeError:  # tag not found
```

### Comparing `philologic-4.7.4/philologic/runtime/link.py` & `philologic-4.7.4.1/philologic/runtime/link.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4/philologic/runtime/reports/__init__.py` & `philologic-4.7.4.1/philologic/runtime/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4/philologic/runtime/reports/aggregation.py` & `philologic-4.7.4.1/philologic/runtime/reports/aggregation.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4/philologic/runtime/reports/bibliography.py` & `philologic-4.7.4.1/philologic/runtime/reports/bibliography.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4/philologic/runtime/reports/collocation.py` & `philologic-4.7.4.1/philologic/runtime/reports/collocation.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4/philologic/runtime/reports/concordance.py` & `philologic-4.7.4.1/philologic/runtime/reports/concordance.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4/philologic/runtime/reports/filter_word_by_property.py` & `philologic-4.7.4.1/philologic/runtime/reports/filter_word_by_property.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4/philologic/runtime/reports/frequency.py` & `philologic-4.7.4.1/philologic/runtime/reports/frequency.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4/philologic/runtime/reports/generate_word_frequency.py` & `philologic-4.7.4.1/philologic/runtime/reports/generate_word_frequency.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4/philologic/runtime/reports/kwic.py` & `philologic-4.7.4.1/philologic/runtime/reports/kwic.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4/philologic/runtime/reports/landing_page.py` & `philologic-4.7.4.1/philologic/runtime/reports/landing_page.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4/philologic/runtime/reports/navigation.py` & `philologic-4.7.4.1/philologic/runtime/reports/navigation.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4/philologic/runtime/reports/table_of_contents.py` & `philologic-4.7.4.1/philologic/runtime/reports/table_of_contents.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4/philologic/runtime/reports/time_series.py` & `philologic-4.7.4.1/philologic/runtime/reports/time_series.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4/philologic/runtime/web_config.py` & `philologic-4.7.4.1/philologic/runtime/web_config.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4/philologic/shlax.py` & `philologic-4.7.4.1/philologic/shlax.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4/philologic/shlaxtree.py` & `philologic-4.7.4.1/philologic/shlaxtree.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4/philologic/utils/convert_entities.py` & `philologic-4.7.4.1/philologic/utils/convert_entities.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4/philologic/utils/metadata_type_handler.py` & `philologic-4.7.4.1/philologic/utils/metadata_type_handler.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4/philologic/utils/pretty_print.py` & `philologic-4.7.4.1/philologic/utils/pretty_print.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4/philologic/utils/sort.py` & `philologic-4.7.4.1/philologic/utils/sort.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4/philologic.egg-info/PKG-INFO` & `philologic-4.7.4.1/philologic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: philologic
-Version: 4.7.4
+Version: 4.7.4.1
 Summary: A concordance search engine for TEI-XML
 Home-page: https://github.com/ARTFL-Project/PhiloLogic4
 Author: Clovis Gladstone
 Author-email: clovisgladstone@artfl.uchicago.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: philologic Version: 4.7.4 Summary: A concordance
+Metadata-Version: 2.1 Name: philologic Version: 4.7.4.1 Summary: A concordance
 search engine for TEI-XML Home-page: https://github.com/ARTFL-Project/
 PhiloLogic4 Author: Clovis Gladstone Author-email:
 clovisgladstone@artfl.uchicago.edu License: UNKNOWN Platform: UNKNOWN Requires-
 Python: >=3.8 License-File: LICENSE These are the Python bindings for the
 PhiloLogic search engine. This package is only useful for the TEI Parser which
 you can import for use outside of PhiloLogic. To get the full functionality of
 PhiloLogic, you need to install the search core as well as the web components.
```

### Comparing `philologic-4.7.4/philologic.egg-info/SOURCES.txt` & `philologic-4.7.4.1/philologic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4/scripts/philoload4` & `philologic-4.7.4.1/scripts/philoload4`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4/setup.py` & `philologic-4.7.4.1/setup.py`

 * *Files identical despite different names*

