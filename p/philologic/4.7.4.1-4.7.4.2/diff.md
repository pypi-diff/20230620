# Comparing `tmp/philologic-4.7.4.1.tar.gz` & `tmp/philologic-4.7.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "philologic-4.7.4.1.tar", last modified: Tue Jun 20 16:13:28 2023, max compression
+gzip compressed data, was "philologic-4.7.4.2.tar", last modified: Tue Jun 20 17:13:31 2023, max compression
```

## Comparing `philologic-4.7.4.1.tar` & `philologic-4.7.4.2.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 clovis    (1000) artfl     (1003)        0 2023-06-20 16:13:28.603805 philologic-4.7.4.1/
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)    35141 2022-11-22 20:47:37.000000 philologic-4.7.4.1/LICENSE
--rw-r--r--   0 clovis    (1000) artfl     (1003)      746 2023-06-20 16:13:28.603805 philologic-4.7.4.1/PKG-INFO
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)      428 2022-11-22 16:01:26.000000 philologic-4.7.4.1/README
-drwxr-xr-x   0 clovis    (1000) artfl     (1003)        0 2023-06-20 16:13:28.599805 philologic-4.7.4.1/philologic/
--rw-r--r--   0 clovis    (1000) artfl     (1003)    36981 2022-12-05 22:36:45.000000 philologic-4.7.4.1/philologic/Config.py
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)     4469 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/TagCensus.py
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)      101 2022-11-22 20:47:37.000000 philologic-4.7.4.1/philologic/__init__.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)      181 2022-11-22 21:05:10.000000 philologic-4.7.4.1/philologic/_version.py
-drwxr-xr-x   0 clovis    (1000) artfl     (1003)        0 2023-06-20 16:13:28.599805 philologic-4.7.4.1/philologic/loadtime/
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)    17283 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/loadtime/LoadFilters.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)    10528 2022-11-24 20:03:41.000000 philologic-4.7.4.1/philologic/loadtime/LoadOptions.py
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)    42023 2022-12-06 18:52:59.000000 philologic-4.7.4.1/philologic/loadtime/Loader.py
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)    13674 2023-02-07 19:21:46.000000 philologic-4.7.4.1/philologic/loadtime/OHCOVector.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)    72525 2022-12-05 20:57:11.000000 philologic-4.7.4.1/philologic/loadtime/Parser.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     8083 2023-02-07 19:21:34.000000 philologic-4.7.4.1/philologic/loadtime/PlainTextParser.py
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)    10370 2023-03-04 17:27:17.000000 philologic-4.7.4.1/philologic/loadtime/PostFilters.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)       49 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/loadtime/__init__.py
-drwxr-xr-x   0 clovis    (1000) artfl     (1003)        0 2023-06-20 16:13:28.603805 philologic-4.7.4.1/philologic/runtime/
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)     9410 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/runtime/DB.py
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)     3776 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/runtime/FragmentParser.py
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)     9822 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/runtime/HitList.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     6768 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/runtime/HitWrapper.py
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)    12990 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/runtime/MetadataQuery.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)    31759 2023-06-20 15:58:40.000000 philologic-4.7.4.1/philologic/runtime/ObjectFormatter.py
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)     9792 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/runtime/Query.py
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)     3493 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/runtime/QuerySyntax.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     7458 2022-12-19 19:58:22.000000 philologic-4.7.4.1/philologic/runtime/WSGIHandler.py
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)      951 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/runtime/__init__.py
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)     6071 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/runtime/access_control.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     5693 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/runtime/citations.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)      511 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/runtime/collocation_scores.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     2412 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/runtime/find_similar_words.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     4044 2023-06-20 14:24:18.000000 philologic-4.7.4.1/philologic/runtime/get_text.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     2956 2022-12-09 02:32:30.000000 philologic-4.7.4.1/philologic/runtime/link.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)      413 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/runtime/pages.py
-drwxr-xr-x   0 clovis    (1000) artfl     (1003)        0 2023-06-20 16:13:28.603805 philologic-4.7.4.1/philologic/runtime/reports/
--rw-r--r--   0 clovis    (1000) artfl     (1003)      977 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/runtime/reports/__init__.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     7673 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/runtime/reports/aggregation.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     3242 2022-12-19 22:17:21.000000 philologic-4.7.4.1/philologic/runtime/reports/bibliography.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     5332 2022-12-05 22:33:58.000000 philologic-4.7.4.1/philologic/runtime/reports/collocation.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     2712 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/runtime/reports/concordance.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     2627 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/runtime/reports/filter_word_by_property.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     7830 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/runtime/reports/frequency.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     2507 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/runtime/reports/generate_word_frequency.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     3349 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/runtime/reports/kwic.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     7425 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/runtime/reports/landing_page.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     3074 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/runtime/reports/navigation.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     3870 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/runtime/reports/table_of_contents.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     4925 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/runtime/reports/time_series.py
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)      894 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/runtime/web_config.py
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)     6167 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/shlax.py
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)     8793 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/shlaxtree.py
-drwxr-xr-x   0 clovis    (1000) artfl     (1003)        0 2023-06-20 16:13:28.603805 philologic-4.7.4.1/philologic/utils/
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)      221 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/utils/__init__.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)      762 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/utils/convert_entities.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)      430 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/utils/load_module.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     1929 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/utils/metadata_type_handler.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     1113 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/utils/pretty_print.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)      581 2022-11-22 16:35:28.000000 philologic-4.7.4.1/philologic/utils/sort.py
-drwxr-xr-x   0 clovis    (1000) artfl     (1003)        0 2023-06-20 16:13:28.599805 philologic-4.7.4.1/philologic.egg-info/
--rw-r--r--   0 clovis    (1000) artfl     (1003)      746 2023-06-20 16:13:28.000000 philologic-4.7.4.1/philologic.egg-info/PKG-INFO
--rw-r--r--   0 clovis    (1000) artfl     (1003)     1975 2023-06-20 16:13:28.000000 philologic-4.7.4.1/philologic.egg-info/SOURCES.txt
--rw-r--r--   0 clovis    (1000) artfl     (1003)        1 2023-06-20 16:13:28.000000 philologic-4.7.4.1/philologic.egg-info/dependency_links.txt
--rw-r--r--   0 clovis    (1000) artfl     (1003)       91 2023-06-20 16:13:28.000000 philologic-4.7.4.1/philologic.egg-info/requires.txt
--rw-r--r--   0 clovis    (1000) artfl     (1003)       11 2023-06-20 16:13:28.000000 philologic-4.7.4.1/philologic.egg-info/top_level.txt
-drwxr-xr-x   0 clovis    (1000) artfl     (1003)        0 2023-06-20 16:13:28.603805 philologic-4.7.4.1/scripts/
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)     1361 2022-11-22 17:21:51.000000 philologic-4.7.4.1/scripts/philoload4
--rw-r--r--   0 clovis    (1000) artfl     (1003)       38 2023-06-20 16:13:28.603805 philologic-4.7.4.1/setup.cfg
--rw-r--r--   0 clovis    (1000) artfl     (1003)     1137 2022-11-30 18:18:41.000000 philologic-4.7.4.1/setup.py
+drwxr-xr-x   0 clovis    (1000) artfl     (1003)        0 2023-06-20 17:13:31.144586 philologic-4.7.4.2/
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)    35141 2022-11-22 20:47:37.000000 philologic-4.7.4.2/LICENSE
+-rw-r--r--   0 clovis    (1000) artfl     (1003)      746 2023-06-20 17:13:31.144586 philologic-4.7.4.2/PKG-INFO
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)      428 2022-11-22 16:01:26.000000 philologic-4.7.4.2/README
+drwxr-xr-x   0 clovis    (1000) artfl     (1003)        0 2023-06-20 17:13:31.140586 philologic-4.7.4.2/philologic/
+-rw-r--r--   0 clovis    (1000) artfl     (1003)    36981 2022-12-05 22:36:45.000000 philologic-4.7.4.2/philologic/Config.py
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)     4469 2022-11-22 16:35:28.000000 philologic-4.7.4.2/philologic/TagCensus.py
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)      101 2022-11-22 20:47:37.000000 philologic-4.7.4.2/philologic/__init__.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)      181 2022-11-22 21:05:10.000000 philologic-4.7.4.2/philologic/_version.py
+drwxr-xr-x   0 clovis    (1000) artfl     (1003)        0 2023-06-20 17:13:31.140586 philologic-4.7.4.2/philologic/loadtime/
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)    17283 2022-11-22 16:35:28.000000 philologic-4.7.4.2/philologic/loadtime/LoadFilters.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)    10528 2022-11-24 20:03:41.000000 philologic-4.7.4.2/philologic/loadtime/LoadOptions.py
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)    42023 2022-12-06 18:52:59.000000 philologic-4.7.4.2/philologic/loadtime/Loader.py
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)    13674 2023-02-07 19:21:46.000000 philologic-4.7.4.2/philologic/loadtime/OHCOVector.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)    72525 2022-12-05 20:57:11.000000 philologic-4.7.4.2/philologic/loadtime/Parser.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     8083 2023-02-07 19:21:34.000000 philologic-4.7.4.2/philologic/loadtime/PlainTextParser.py
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)    10370 2023-03-04 17:27:17.000000 philologic-4.7.4.2/philologic/loadtime/PostFilters.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)       49 2022-11-22 16:35:28.000000 philologic-4.7.4.2/philologic/loadtime/__init__.py
+drwxr-xr-x   0 clovis    (1000) artfl     (1003)        0 2023-06-20 17:13:31.144586 philologic-4.7.4.2/philologic/runtime/
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)     9410 2022-11-22 16:35:28.000000 philologic-4.7.4.2/philologic/runtime/DB.py
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)     3776 2022-11-22 16:35:28.000000 philologic-4.7.4.2/philologic/runtime/FragmentParser.py
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)     9822 2022-11-22 16:35:28.000000 philologic-4.7.4.2/philologic/runtime/HitList.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     6768 2022-11-22 16:35:28.000000 philologic-4.7.4.2/philologic/runtime/HitWrapper.py
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)    12990 2022-11-22 16:35:28.000000 philologic-4.7.4.2/philologic/runtime/MetadataQuery.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)    31760 2023-06-20 16:50:25.000000 philologic-4.7.4.2/philologic/runtime/ObjectFormatter.py
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)     9792 2022-11-22 16:35:28.000000 philologic-4.7.4.2/philologic/runtime/Query.py
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)     3493 2022-11-22 16:35:28.000000 philologic-4.7.4.2/philologic/runtime/QuerySyntax.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     7458 2022-12-19 19:58:22.000000 philologic-4.7.4.2/philologic/runtime/WSGIHandler.py
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)      951 2022-11-22 16:35:28.000000 philologic-4.7.4.2/philologic/runtime/__init__.py
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)     6071 2022-11-22 16:35:28.000000 philologic-4.7.4.2/philologic/runtime/access_control.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     5693 2022-11-22 16:35:28.000000 philologic-4.7.4.2/philologic/runtime/citations.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)      511 2022-11-22 16:35:28.000000 philologic-4.7.4.2/philologic/runtime/collocation_scores.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     2412 2022-11-22 16:35:28.000000 philologic-4.7.4.2/philologic/runtime/find_similar_words.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     4044 2023-06-20 14:24:18.000000 philologic-4.7.4.2/philologic/runtime/get_text.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     2956 2022-12-09 02:32:30.000000 philologic-4.7.4.2/philologic/runtime/link.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)      413 2022-11-22 16:35:28.000000 philologic-4.7.4.2/philologic/runtime/pages.py
+drwxr-xr-x   0 clovis    (1000) artfl     (1003)        0 2023-06-20 17:13:31.144586 philologic-4.7.4.2/philologic/runtime/reports/
+-rw-r--r--   0 clovis    (1000) artfl     (1003)      977 2022-11-22 16:35:28.000000 philologic-4.7.4.2/philologic/runtime/reports/__init__.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     7673 2022-11-22 16:35:28.000000 philologic-4.7.4.2/philologic/runtime/reports/aggregation.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     3242 2022-12-19 22:17:21.000000 philologic-4.7.4.2/philologic/runtime/reports/bibliography.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     5332 2022-12-05 22:33:58.000000 philologic-4.7.4.2/philologic/runtime/reports/collocation.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     2712 2022-11-22 16:35:28.000000 philologic-4.7.4.2/philologic/runtime/reports/concordance.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     2627 2022-11-22 16:35:28.000000 philologic-4.7.4.2/philologic/runtime/reports/filter_word_by_property.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     7830 2022-11-22 16:35:28.000000 philologic-4.7.4.2/philologic/runtime/reports/frequency.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     2507 2022-11-22 16:35:28.000000 philologic-4.7.4.2/philologic/runtime/reports/generate_word_frequency.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     3349 2022-11-22 16:35:28.000000 philologic-4.7.4.2/philologic/runtime/reports/kwic.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     7425 2022-11-22 16:35:28.000000 philologic-4.7.4.2/philologic/runtime/reports/landing_page.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     3074 2022-11-22 16:35:28.000000 philologic-4.7.4.2/philologic/runtime/reports/navigation.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     3870 2022-11-22 16:35:28.000000 philologic-4.7.4.2/philologic/runtime/reports/table_of_contents.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     4925 2022-11-22 16:35:28.000000 philologic-4.7.4.2/philologic/runtime/reports/time_series.py
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)      894 2022-11-22 16:35:28.000000 philologic-4.7.4.2/philologic/runtime/web_config.py
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)     6167 2022-11-22 16:35:28.000000 philologic-4.7.4.2/philologic/shlax.py
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)     8793 2022-11-22 16:35:28.000000 philologic-4.7.4.2/philologic/shlaxtree.py
+drwxr-xr-x   0 clovis    (1000) artfl     (1003)        0 2023-06-20 17:13:31.144586 philologic-4.7.4.2/philologic/utils/
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)      221 2022-11-22 16:35:28.000000 philologic-4.7.4.2/philologic/utils/__init__.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)      762 2022-11-22 16:35:28.000000 philologic-4.7.4.2/philologic/utils/convert_entities.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)      430 2022-11-22 16:35:28.000000 philologic-4.7.4.2/philologic/utils/load_module.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     1929 2022-11-22 16:35:28.000000 philologic-4.7.4.2/philologic/utils/metadata_type_handler.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     1113 2022-11-22 16:35:28.000000 philologic-4.7.4.2/philologic/utils/pretty_print.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)      581 2022-11-22 16:35:28.000000 philologic-4.7.4.2/philologic/utils/sort.py
+drwxr-xr-x   0 clovis    (1000) artfl     (1003)        0 2023-06-20 17:13:31.140586 philologic-4.7.4.2/philologic.egg-info/
+-rw-r--r--   0 clovis    (1000) artfl     (1003)      746 2023-06-20 17:13:31.000000 philologic-4.7.4.2/philologic.egg-info/PKG-INFO
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     1975 2023-06-20 17:13:31.000000 philologic-4.7.4.2/philologic.egg-info/SOURCES.txt
+-rw-r--r--   0 clovis    (1000) artfl     (1003)        1 2023-06-20 17:13:31.000000 philologic-4.7.4.2/philologic.egg-info/dependency_links.txt
+-rw-r--r--   0 clovis    (1000) artfl     (1003)       91 2023-06-20 17:13:31.000000 philologic-4.7.4.2/philologic.egg-info/requires.txt
+-rw-r--r--   0 clovis    (1000) artfl     (1003)       11 2023-06-20 17:13:31.000000 philologic-4.7.4.2/philologic.egg-info/top_level.txt
+drwxr-xr-x   0 clovis    (1000) artfl     (1003)        0 2023-06-20 17:13:31.144586 philologic-4.7.4.2/scripts/
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)     1361 2022-11-22 17:21:51.000000 philologic-4.7.4.2/scripts/philoload4
+-rw-r--r--   0 clovis    (1000) artfl     (1003)       38 2023-06-20 17:13:31.144586 philologic-4.7.4.2/setup.cfg
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     1137 2022-11-30 18:18:41.000000 philologic-4.7.4.2/setup.py
```

### Comparing `philologic-4.7.4.1/LICENSE` & `philologic-4.7.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.1/PKG-INFO` & `philologic-4.7.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: philologic
-Version: 4.7.4.1
+Version: 4.7.4.2
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
-Metadata-Version: 2.1 Name: philologic Version: 4.7.4.1 Summary: A concordance
+Metadata-Version: 2.1 Name: philologic Version: 4.7.4.2 Summary: A concordance
 search engine for TEI-XML Home-page: https://github.com/ARTFL-Project/
 PhiloLogic4 Author: Clovis Gladstone Author-email:
 clovisgladstone@artfl.uchicago.edu License: UNKNOWN Platform: UNKNOWN Requires-
 Python: >=3.8 License-File: LICENSE These are the Python bindings for the
 PhiloLogic search engine. This package is only useful for the TEI Parser which
 you can import for use outside of PhiloLogic. To get the full functionality of
 PhiloLogic, you need to install the search core as well as the web components.
```

### Comparing `philologic-4.7.4.1/philologic/Config.py` & `philologic-4.7.4.2/philologic/Config.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.1/philologic/TagCensus.py` & `philologic-4.7.4.2/philologic/TagCensus.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.1/philologic/loadtime/LoadFilters.py` & `philologic-4.7.4.2/philologic/loadtime/LoadFilters.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.1/philologic/loadtime/LoadOptions.py` & `philologic-4.7.4.2/philologic/loadtime/LoadOptions.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.1/philologic/loadtime/Loader.py` & `philologic-4.7.4.2/philologic/loadtime/Loader.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.1/philologic/loadtime/OHCOVector.py` & `philologic-4.7.4.2/philologic/loadtime/OHCOVector.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.1/philologic/loadtime/Parser.py` & `philologic-4.7.4.2/philologic/loadtime/Parser.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.1/philologic/loadtime/PlainTextParser.py` & `philologic-4.7.4.2/philologic/loadtime/PlainTextParser.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.1/philologic/loadtime/PostFilters.py` & `philologic-4.7.4.2/philologic/loadtime/PostFilters.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.1/philologic/runtime/DB.py` & `philologic-4.7.4.2/philologic/runtime/DB.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.1/philologic/runtime/FragmentParser.py` & `philologic-4.7.4.2/philologic/runtime/FragmentParser.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.1/philologic/runtime/HitList.py` & `philologic-4.7.4.2/philologic/runtime/HitList.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.1/philologic/runtime/HitWrapper.py` & `philologic-4.7.4.2/philologic/runtime/HitWrapper.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.1/philologic/runtime/MetadataQuery.py` & `philologic-4.7.4.2/philologic/runtime/MetadataQuery.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.1/philologic/runtime/ObjectFormatter.py` & `philologic-4.7.4.2/philologic/runtime/ObjectFormatter.py`

 * *Files 1% similar despite different names*

```diff
@@ -594,15 +594,15 @@
                     parent.insert(parent.index(el) + 1, text_element_wrapper)
 
         except Exception as exception:
             pass
 
     if start_end_pairs:
         # Make sure we did not miss element tails
-        in_passage = True
+        in_passage = False
         n_marker = ""
         for el in xml.iter():
             match = False
             class_name = ""
             if "class" in el.attrib and el.attrib["class"] == "passage-marker":
                 in_passage = True
                 n_marker = el.attrib["n"]
```

### Comparing `philologic-4.7.4.1/philologic/runtime/Query.py` & `philologic-4.7.4.2/philologic/runtime/Query.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.1/philologic/runtime/QuerySyntax.py` & `philologic-4.7.4.2/philologic/runtime/QuerySyntax.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.1/philologic/runtime/WSGIHandler.py` & `philologic-4.7.4.2/philologic/runtime/WSGIHandler.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.1/philologic/runtime/__init__.py` & `philologic-4.7.4.2/philologic/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.1/philologic/runtime/access_control.py` & `philologic-4.7.4.2/philologic/runtime/access_control.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.1/philologic/runtime/citations.py` & `philologic-4.7.4.2/philologic/runtime/citations.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.1/philologic/runtime/find_similar_words.py` & `philologic-4.7.4.2/philologic/runtime/find_similar_words.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.1/philologic/runtime/get_text.py` & `philologic-4.7.4.2/philologic/runtime/get_text.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.1/philologic/runtime/link.py` & `philologic-4.7.4.2/philologic/runtime/link.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.1/philologic/runtime/reports/__init__.py` & `philologic-4.7.4.2/philologic/runtime/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.1/philologic/runtime/reports/aggregation.py` & `philologic-4.7.4.2/philologic/runtime/reports/aggregation.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.1/philologic/runtime/reports/bibliography.py` & `philologic-4.7.4.2/philologic/runtime/reports/bibliography.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.1/philologic/runtime/reports/collocation.py` & `philologic-4.7.4.2/philologic/runtime/reports/collocation.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.1/philologic/runtime/reports/concordance.py` & `philologic-4.7.4.2/philologic/runtime/reports/concordance.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.1/philologic/runtime/reports/filter_word_by_property.py` & `philologic-4.7.4.2/philologic/runtime/reports/filter_word_by_property.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.1/philologic/runtime/reports/frequency.py` & `philologic-4.7.4.2/philologic/runtime/reports/frequency.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.1/philologic/runtime/reports/generate_word_frequency.py` & `philologic-4.7.4.2/philologic/runtime/reports/generate_word_frequency.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.1/philologic/runtime/reports/kwic.py` & `philologic-4.7.4.2/philologic/runtime/reports/kwic.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.1/philologic/runtime/reports/landing_page.py` & `philologic-4.7.4.2/philologic/runtime/reports/landing_page.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.1/philologic/runtime/reports/navigation.py` & `philologic-4.7.4.2/philologic/runtime/reports/navigation.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.1/philologic/runtime/reports/table_of_contents.py` & `philologic-4.7.4.2/philologic/runtime/reports/table_of_contents.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.1/philologic/runtime/reports/time_series.py` & `philologic-4.7.4.2/philologic/runtime/reports/time_series.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.1/philologic/runtime/web_config.py` & `philologic-4.7.4.2/philologic/runtime/web_config.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.1/philologic/shlax.py` & `philologic-4.7.4.2/philologic/shlax.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.1/philologic/shlaxtree.py` & `philologic-4.7.4.2/philologic/shlaxtree.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.1/philologic/utils/convert_entities.py` & `philologic-4.7.4.2/philologic/utils/convert_entities.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.1/philologic/utils/metadata_type_handler.py` & `philologic-4.7.4.2/philologic/utils/metadata_type_handler.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.1/philologic/utils/pretty_print.py` & `philologic-4.7.4.2/philologic/utils/pretty_print.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.1/philologic/utils/sort.py` & `philologic-4.7.4.2/philologic/utils/sort.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.1/philologic.egg-info/PKG-INFO` & `philologic-4.7.4.2/philologic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: philologic
-Version: 4.7.4.1
+Version: 4.7.4.2
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
-Metadata-Version: 2.1 Name: philologic Version: 4.7.4.1 Summary: A concordance
+Metadata-Version: 2.1 Name: philologic Version: 4.7.4.2 Summary: A concordance
 search engine for TEI-XML Home-page: https://github.com/ARTFL-Project/
 PhiloLogic4 Author: Clovis Gladstone Author-email:
 clovisgladstone@artfl.uchicago.edu License: UNKNOWN Platform: UNKNOWN Requires-
 Python: >=3.8 License-File: LICENSE These are the Python bindings for the
 PhiloLogic search engine. This package is only useful for the TEI Parser which
 you can import for use outside of PhiloLogic. To get the full functionality of
 PhiloLogic, you need to install the search core as well as the web components.
```

### Comparing `philologic-4.7.4.1/philologic.egg-info/SOURCES.txt` & `philologic-4.7.4.2/philologic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.1/scripts/philoload4` & `philologic-4.7.4.2/scripts/philoload4`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.1/setup.py` & `philologic-4.7.4.2/setup.py`

 * *Files identical despite different names*

