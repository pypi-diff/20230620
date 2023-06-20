# Comparing `tmp/google-cloud-bigquery-datapolicies-0.4.0.tar.gz` & `tmp/google-cloud-bigquery-datapolicies-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-bigquery-datapolicies-0.4.0.tar", last modified: Mon Apr 17 10:42:42 2023, max compression
+gzip compressed data, was "google-cloud-bigquery-datapolicies-0.5.0.tar", last modified: Tue Jun 20 13:27:05 2023, max compression
```

## Comparing `google-cloud-bigquery-datapolicies-0.4.0.tar` & `google-cloud-bigquery-datapolicies-0.5.0.tar`

### file list

```diff
@@ -1,75 +1,74 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:42:42.813091 google-cloud-bigquery-datapolicies-0.4.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4849 2023-04-17 10:42:42.813091 google-cloud-bigquery-datapolicies-0.4.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3904 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:42:42.801092 google-cloud-bigquery-datapolicies-0.4.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:42:42.801092 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:42:42.801092 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:42:42.805092 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies/
--rw-rw-r--   0 root         (0)     1003     1625 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       95 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:42:42.805092 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/
--rw-rw-r--   0 root         (0)     1003     1451 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     4125 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       95 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:42:42.805092 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:42:42.809091 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/
--rw-rw-r--   0 root         (0)     1003      781 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    56334 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    63536 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/client.py
--rw-rw-r--   0 root         (0)     1003     5969 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:42:42.809091 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/transports/
--rw-rw-r--   0 root         (0)     1003     1442 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    12955 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    21504 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    21939 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    59846 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:42:42.809091 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/types/
--rw-rw-r--   0 root         (0)     1003     1141 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    11389 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/types/datapolicy.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:42:42.809091 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/
--rw-rw-r--   0 root         (0)     1003     1396 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003     2620 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       95 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:42:42.809091 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:42:42.809091 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/
--rw-rw-r--   0 root         (0)     1003      781 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    51605 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    58819 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/client.py
--rw-rw-r--   0 root         (0)     1003     6014 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:42:42.813091 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/transports/
--rw-rw-r--   0 root         (0)     1003     1220 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    12185 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    20383 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    20782 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:42:42.813091 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/types/
--rw-rw-r--   0 root         (0)     1003     1081 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    10282 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/types/datapolicy.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:42:42.813091 google-cloud-bigquery-datapolicies-0.4.0/google_cloud_bigquery_datapolicies.egg-info/
--rw-r--r--   0 root         (0)     1003     4849 2023-04-17 10:42:42.000000 google-cloud-bigquery-datapolicies-0.4.0/google_cloud_bigquery_datapolicies.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     3168 2023-04-17 10:42:42.000000 google-cloud-bigquery-datapolicies-0.4.0/google_cloud_bigquery_datapolicies.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-04-17 10:42:42.000000 google-cloud-bigquery-datapolicies-0.4.0/google_cloud_bigquery_datapolicies.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       42 2023-04-17 10:42:42.000000 google-cloud-bigquery-datapolicies-0.4.0/google_cloud_bigquery_datapolicies.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-04-17 10:42:42.000000 google-cloud-bigquery-datapolicies-0.4.0/google_cloud_bigquery_datapolicies.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-04-17 10:42:42.000000 google-cloud-bigquery-datapolicies-0.4.0/google_cloud_bigquery_datapolicies.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-04-17 10:42:42.000000 google-cloud-bigquery-datapolicies-0.4.0/google_cloud_bigquery_datapolicies.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-04-17 10:42:42.817091 google-cloud-bigquery-datapolicies-0.4.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3055 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:42:42.813091 google-cloud-bigquery-datapolicies-0.4.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:42:42.813091 google-cloud-bigquery-datapolicies-0.4.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:42:42.813091 google-cloud-bigquery-datapolicies-0.4.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:42:42.813091 google-cloud-bigquery-datapolicies-0.4.0/tests/unit/gapic/datapolicies_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/tests/unit/gapic/datapolicies_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   224205 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/tests/unit/gapic/datapolicies_v1/test_data_policy_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:42:42.813091 google-cloud-bigquery-datapolicies-0.4.0/tests/unit/gapic/datapolicies_v1beta1/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/tests/unit/gapic/datapolicies_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003   123065 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/tests/unit/gapic/datapolicies_v1beta1/test_data_policy_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:05.537786 google-cloud-bigquery-datapolicies-0.5.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-06-20 13:23:47.000000 google-cloud-bigquery-datapolicies-0.5.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-06-20 13:23:47.000000 google-cloud-bigquery-datapolicies-0.5.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4804 2023-06-20 13:27:05.537786 google-cloud-bigquery-datapolicies-0.5.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3868 2023-06-20 13:23:47.000000 google-cloud-bigquery-datapolicies-0.5.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:05.525785 google-cloud-bigquery-datapolicies-0.5.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:05.525785 google-cloud-bigquery-datapolicies-0.5.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:05.529785 google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies/
+-rw-rw-r--   0 root         (0)     1003     1625 2023-06-20 13:23:47.000000 google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-20 13:23:47.000000 google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       95 2023-06-20 13:23:47.000000 google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:05.529785 google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1/
+-rw-rw-r--   0 root         (0)     1003     1451 2023-06-20 13:23:47.000000 google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4125 2023-06-20 13:23:47.000000 google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-20 13:23:47.000000 google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       95 2023-06-20 13:23:47.000000 google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:05.529785 google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-20 13:23:47.000000 google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:05.529785 google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/
+-rw-rw-r--   0 root         (0)     1003      781 2023-06-20 13:23:47.000000 google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    56487 2023-06-20 13:23:47.000000 google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    63689 2023-06-20 13:23:47.000000 google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5969 2023-06-20 13:23:47.000000 google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:05.529785 google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1442 2023-06-20 13:23:47.000000 google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12955 2023-06-20 13:23:47.000000 google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    21504 2023-06-20 13:23:47.000000 google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    21939 2023-06-20 13:23:47.000000 google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    59846 2023-06-20 13:23:47.000000 google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:05.529785 google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1141 2023-06-20 13:23:47.000000 google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11389 2023-06-20 13:23:47.000000 google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1/types/datapolicy.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:05.533786 google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1beta1/
+-rw-rw-r--   0 root         (0)     1003     1396 2023-06-20 13:23:47.000000 google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2620 2023-06-20 13:23:47.000000 google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-20 13:23:47.000000 google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1beta1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       95 2023-06-20 13:23:47.000000 google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:05.533786 google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-20 13:23:47.000000 google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:05.533786 google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/
+-rw-rw-r--   0 root         (0)     1003      781 2023-06-20 13:23:47.000000 google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    51740 2023-06-20 13:23:47.000000 google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    58954 2023-06-20 13:23:47.000000 google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/client.py
+-rw-rw-r--   0 root         (0)     1003     6014 2023-06-20 13:23:47.000000 google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:05.533786 google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1220 2023-06-20 13:23:47.000000 google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12185 2023-06-20 13:23:47.000000 google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    20383 2023-06-20 13:23:47.000000 google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    20782 2023-06-20 13:23:47.000000 google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:05.533786 google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1beta1/types/
+-rw-rw-r--   0 root         (0)     1003     1081 2023-06-20 13:23:47.000000 google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10282 2023-06-20 13:23:47.000000 google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1beta1/types/datapolicy.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:05.533786 google-cloud-bigquery-datapolicies-0.5.0/google_cloud_bigquery_datapolicies.egg-info/
+-rw-r--r--   0 root         (0)     1003     4804 2023-06-20 13:27:05.000000 google-cloud-bigquery-datapolicies-0.5.0/google_cloud_bigquery_datapolicies.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     3204 2023-06-20 13:27:05.000000 google-cloud-bigquery-datapolicies-0.5.0/google_cloud_bigquery_datapolicies.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-06-20 13:27:05.000000 google-cloud-bigquery-datapolicies-0.5.0/google_cloud_bigquery_datapolicies.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-06-20 13:27:05.000000 google-cloud-bigquery-datapolicies-0.5.0/google_cloud_bigquery_datapolicies.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-06-20 13:27:05.000000 google-cloud-bigquery-datapolicies-0.5.0/google_cloud_bigquery_datapolicies.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-06-20 13:27:05.000000 google-cloud-bigquery-datapolicies-0.5.0/google_cloud_bigquery_datapolicies.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-06-20 13:27:05.000000 google-cloud-bigquery-datapolicies-0.5.0/google_cloud_bigquery_datapolicies.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-06-20 13:27:05.537786 google-cloud-bigquery-datapolicies-0.5.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3021 2023-06-20 13:23:47.000000 google-cloud-bigquery-datapolicies-0.5.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:05.537786 google-cloud-bigquery-datapolicies-0.5.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-20 13:23:47.000000 google-cloud-bigquery-datapolicies-0.5.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:05.537786 google-cloud-bigquery-datapolicies-0.5.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-20 13:23:47.000000 google-cloud-bigquery-datapolicies-0.5.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:05.537786 google-cloud-bigquery-datapolicies-0.5.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-20 13:23:47.000000 google-cloud-bigquery-datapolicies-0.5.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:05.537786 google-cloud-bigquery-datapolicies-0.5.0/tests/unit/gapic/bigquery_datapolicies_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-20 13:23:47.000000 google-cloud-bigquery-datapolicies-0.5.0/tests/unit/gapic/bigquery_datapolicies_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   224205 2023-06-20 13:23:47.000000 google-cloud-bigquery-datapolicies-0.5.0/tests/unit/gapic/bigquery_datapolicies_v1/test_data_policy_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:05.537786 google-cloud-bigquery-datapolicies-0.5.0/tests/unit/gapic/bigquery_datapolicies_v1beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-20 13:23:47.000000 google-cloud-bigquery-datapolicies-0.5.0/tests/unit/gapic/bigquery_datapolicies_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   123065 2023-06-20 13:23:47.000000 google-cloud-bigquery-datapolicies-0.5.0/tests/unit/gapic/bigquery_datapolicies_v1beta1/test_data_policy_service.py
```

### Comparing `google-cloud-bigquery-datapolicies-0.4.0/LICENSE` & `google-cloud-bigquery-datapolicies-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.4.0/MANIFEST.in` & `google-cloud-bigquery-datapolicies-0.5.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.4.0/PKG-INFO` & `google-cloud-bigquery-datapolicies-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-bigquery-datapolicies
-Version: 0.4.0
+Version: 0.5.0
 Summary: Google Cloud Bigquery Datapolicies API client library
-Home-page: https://github.com/googleapis/python-bigquery-datapolicies
+Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -18,47 +18,47 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Requires-Python: >=3.7
 License-File: LICENSE
 
-Python Client for BigQuery Data Policy API
-==========================================
+Python Client for BigQuery Data Policy
+======================================
 
 |preview| |pypi| |versions|
 
-`BigQuery Data Policy API`_: Allows users to manage BigQuery data policies.
+`BigQuery Data Policy`_: Allows users to manage BigQuery data policies.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-bigquery-datapolicies.svg
    :target: https://pypi.org/project/google-cloud-bigquery-datapolicies/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-bigquery-datapolicies.svg
    :target: https://pypi.org/project/google-cloud-bigquery-datapolicies/
-.. _BigQuery Data Policy API: https://cloud.google.com/bigquery/docs/reference/bigquerydatapolicy/rest
+.. _BigQuery Data Policy: https://cloud.google.com/bigquery/docs/reference/bigquerydatapolicy/rest
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/bigquerydatapolicy/latest
 .. _Product Documentation:  https://cloud.google.com/bigquery/docs/reference/bigquerydatapolicy/rest
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the BigQuery Data Policy API.`_
+3. `Enable the BigQuery Data Policy.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the BigQuery Data Policy API.:  https://cloud.google.com/bigquery/docs/reference/bigquerydatapolicy/rest
+.. _Enable the BigQuery Data Policy.:  https://cloud.google.com/bigquery/docs/reference/bigquerydatapolicy/rest
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-bigquery-datapolicies
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for BigQuery Data Policy API
+-  Read the `Client Library Documentation`_ for BigQuery Data Policy
    to see other available methods on the client.
--  Read the `BigQuery Data Policy API Product documentation`_ to learn
+-  Read the `BigQuery Data Policy Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _BigQuery Data Policy API Product documentation:  https://cloud.google.com/bigquery/docs/reference/bigquerydatapolicy/rest
+.. _BigQuery Data Policy Product documentation:  https://cloud.google.com/bigquery/docs/reference/bigquerydatapolicy/rest
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-bigquery-datapolicies-0.4.0/README.rst` & `google-cloud-bigquery-datapolicies-0.5.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Python Client for BigQuery Data Policy API
-==========================================
+Python Client for BigQuery Data Policy
+======================================
 
 |preview| |pypi| |versions|
 
-`BigQuery Data Policy API`_: Allows users to manage BigQuery data policies.
+`BigQuery Data Policy`_: Allows users to manage BigQuery data policies.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-bigquery-datapolicies.svg
    :target: https://pypi.org/project/google-cloud-bigquery-datapolicies/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-bigquery-datapolicies.svg
    :target: https://pypi.org/project/google-cloud-bigquery-datapolicies/
-.. _BigQuery Data Policy API: https://cloud.google.com/bigquery/docs/reference/bigquerydatapolicy/rest
+.. _BigQuery Data Policy: https://cloud.google.com/bigquery/docs/reference/bigquerydatapolicy/rest
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/bigquerydatapolicy/latest
 .. _Product Documentation:  https://cloud.google.com/bigquery/docs/reference/bigquerydatapolicy/rest
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the BigQuery Data Policy API.`_
+3. `Enable the BigQuery Data Policy.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the BigQuery Data Policy API.:  https://cloud.google.com/bigquery/docs/reference/bigquerydatapolicy/rest
+.. _Enable the BigQuery Data Policy.:  https://cloud.google.com/bigquery/docs/reference/bigquerydatapolicy/rest
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -92,16 +92,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-bigquery-datapolicies
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for BigQuery Data Policy API
+-  Read the `Client Library Documentation`_ for BigQuery Data Policy
    to see other available methods on the client.
--  Read the `BigQuery Data Policy API Product documentation`_ to learn
+-  Read the `BigQuery Data Policy Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _BigQuery Data Policy API Product documentation:  https://cloud.google.com/bigquery/docs/reference/bigquerydatapolicy/rest
+.. _BigQuery Data Policy Product documentation:  https://cloud.google.com/bigquery/docs/reference/bigquerydatapolicy/rest
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies/__init__.py` & `google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,26 +9,26 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from google.cloud.bigquery.datapolicies import gapic_version as package_version
+from google.cloud.bigquery_datapolicies import gapic_version as package_version
 
 __version__ = package_version.__version__
 
 
-from google.cloud.bigquery.datapolicies_v1.services.data_policy_service.async_client import (
+from google.cloud.bigquery_datapolicies_v1.services.data_policy_service.async_client import (
     DataPolicyServiceAsyncClient,
 )
-from google.cloud.bigquery.datapolicies_v1.services.data_policy_service.client import (
+from google.cloud.bigquery_datapolicies_v1.services.data_policy_service.client import (
     DataPolicyServiceClient,
 )
-from google.cloud.bigquery.datapolicies_v1.types.datapolicy import (
+from google.cloud.bigquery_datapolicies_v1.types.datapolicy import (
     CreateDataPolicyRequest,
     DataMaskingPolicy,
     DataPolicy,
     DeleteDataPolicyRequest,
     GetDataPolicyRequest,
     ListDataPoliciesRequest,
     ListDataPoliciesResponse,
```

### Comparing `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies/gapic_version.py` & `google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.4.0"  # {x-release-please-version}
+__version__ = "0.5.0"  # {x-release-please-version}
```

### Comparing `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/__init__.py` & `google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from google.cloud.bigquery.datapolicies_v1 import gapic_version as package_version
+from google.cloud.bigquery_datapolicies_v1 import gapic_version as package_version
 
 __version__ = package_version.__version__
 
 
 from .services.data_policy_service import (
     DataPolicyServiceAsyncClient,
     DataPolicyServiceClient,
```

### Comparing `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/gapic_metadata.json` & `google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1/gapic_metadata.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'libraryPackage'": "'google.cloud.bigquery_datapolicies_v1'"}*

```diff
@@ -1,11 +1,11 @@
 {
     "comment": "This file maps proto services/RPCs to the corresponding library clients/methods",
     "language": "python",
-    "libraryPackage": "google.cloud.bigquery.datapolicies_v1",
+    "libraryPackage": "google.cloud.bigquery_datapolicies_v1",
     "protoPackage": "google.cloud.bigquery.datapolicies.v1",
     "schema": "1.0",
     "services": {
         "DataPolicyService": {
             "clients": {
                 "grpc": {
                     "libraryClient": "DataPolicyServiceClient",
```

### Comparing `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/gapic_version.py` & `google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.4.0"  # {x-release-please-version}
+__version__ = "0.5.0"  # {x-release-please-version}
```

### Comparing `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/services/__init__.py` & `google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/__init__.py` & `google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/async_client.py` & `google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/async_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,27 +31,27 @@
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.api_core.client_options import ClientOptions
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 
-from google.cloud.bigquery.datapolicies_v1 import gapic_version as package_version
+from google.cloud.bigquery_datapolicies_v1 import gapic_version as package_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.iam.v1 import iam_policy_pb2  # type: ignore
 from google.iam.v1 import policy_pb2  # type: ignore
 from google.protobuf import field_mask_pb2  # type: ignore
 
-from google.cloud.bigquery.datapolicies_v1.services.data_policy_service import pagers
-from google.cloud.bigquery.datapolicies_v1.types import datapolicy
+from google.cloud.bigquery_datapolicies_v1.services.data_policy_service import pagers
+from google.cloud.bigquery_datapolicies_v1.types import datapolicy
 
 from .client import DataPolicyServiceClient
 from .transports.base import DEFAULT_CLIENT_INFO, DataPolicyServiceTransport
 from .transports.grpc_asyncio import DataPolicyServiceGrpcAsyncIOTransport
 
 
 class DataPolicyServiceAsyncClient:
@@ -241,64 +241,64 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import datapolicies_v1
+            from google.cloud import bigquery_datapolicies_v1
 
             async def sample_create_data_policy():
                 # Create a client
-                client = datapolicies_v1.DataPolicyServiceAsyncClient()
+                client = bigquery_datapolicies_v1.DataPolicyServiceAsyncClient()
 
                 # Initialize request argument(s)
-                data_policy = datapolicies_v1.DataPolicy()
+                data_policy = bigquery_datapolicies_v1.DataPolicy()
                 data_policy.policy_tag = "policy_tag_value"
                 data_policy.data_masking_policy.predefined_expression = "DEFAULT_MASKING_VALUE"
 
-                request = datapolicies_v1.CreateDataPolicyRequest(
+                request = bigquery_datapolicies_v1.CreateDataPolicyRequest(
                     parent="parent_value",
                     data_policy=data_policy,
                 )
 
                 # Make the request
                 response = await client.create_data_policy(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.datapolicies_v1.types.CreateDataPolicyRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_datapolicies_v1.types.CreateDataPolicyRequest, dict]]):
                 The request object. Request message for the
                 CreateDataPolicy method.
             parent (:class:`str`):
                 Required. Resource name of the project that the data
                 policy will belong to. The format is
                 ``projects/{project_number}/locations/{location_id}``.
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            data_policy (:class:`google.cloud.bigquery.datapolicies_v1.types.DataPolicy`):
+            data_policy (:class:`google.cloud.bigquery_datapolicies_v1.types.DataPolicy`):
                 Required. The data policy to create. The ``name`` field
                 does not need to be provided for the data policy
                 creation.
 
                 This corresponds to the ``data_policy`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.datapolicies_v1.types.DataPolicy:
+            google.cloud.bigquery_datapolicies_v1.types.DataPolicy:
                 Represents the label-policy binding.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, data_policy])
         if request is not None and has_flattened_params:
@@ -369,40 +369,40 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import datapolicies_v1
+            from google.cloud import bigquery_datapolicies_v1
 
             async def sample_update_data_policy():
                 # Create a client
-                client = datapolicies_v1.DataPolicyServiceAsyncClient()
+                client = bigquery_datapolicies_v1.DataPolicyServiceAsyncClient()
 
                 # Initialize request argument(s)
-                data_policy = datapolicies_v1.DataPolicy()
+                data_policy = bigquery_datapolicies_v1.DataPolicy()
                 data_policy.policy_tag = "policy_tag_value"
                 data_policy.data_masking_policy.predefined_expression = "DEFAULT_MASKING_VALUE"
 
-                request = datapolicies_v1.UpdateDataPolicyRequest(
+                request = bigquery_datapolicies_v1.UpdateDataPolicyRequest(
                     data_policy=data_policy,
                 )
 
                 # Make the request
                 response = await client.update_data_policy(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.datapolicies_v1.types.UpdateDataPolicyRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_datapolicies_v1.types.UpdateDataPolicyRequest, dict]]):
                 The request object. Response message for the
                 UpdateDataPolicy method.
-            data_policy (:class:`google.cloud.bigquery.datapolicies_v1.types.DataPolicy`):
+            data_policy (:class:`google.cloud.bigquery_datapolicies_v1.types.DataPolicy`):
                 Required. Update the data policy's metadata.
 
                 The target data policy is determined by the ``name``
                 field. Other fields are updated to the specified values
                 based on the field masks.
 
                 This corresponds to the ``data_policy`` field
@@ -424,15 +424,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.datapolicies_v1.types.DataPolicy:
+            google.cloud.bigquery_datapolicies_v1.types.DataPolicy:
                 Represents the label-policy binding.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([data_policy, update_mask])
         if request is not None and has_flattened_params:
@@ -504,34 +504,34 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import datapolicies_v1
+            from google.cloud import bigquery_datapolicies_v1
 
             async def sample_rename_data_policy():
                 # Create a client
-                client = datapolicies_v1.DataPolicyServiceAsyncClient()
+                client = bigquery_datapolicies_v1.DataPolicyServiceAsyncClient()
 
                 # Initialize request argument(s)
-                request = datapolicies_v1.RenameDataPolicyRequest(
+                request = bigquery_datapolicies_v1.RenameDataPolicyRequest(
                     name="name_value",
                     new_data_policy_id="new_data_policy_id_value",
                 )
 
                 # Make the request
                 response = await client.rename_data_policy(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.datapolicies_v1.types.RenameDataPolicyRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_datapolicies_v1.types.RenameDataPolicyRequest, dict]]):
                 The request object. Request message for the
                 RenameDataPolicy method.
             name (:class:`str`):
                 Required. Resource name of the data policy to rename.
                 The format is
                 ``projects/{project_number}/locations/{location_id}/dataPolicies/{data_policy_id}``
 
@@ -546,15 +546,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.datapolicies_v1.types.DataPolicy:
+            google.cloud.bigquery_datapolicies_v1.types.DataPolicy:
                 Represents the label-policy binding.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name, new_data_policy_id])
         if request is not None and has_flattened_params:
@@ -623,30 +623,30 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import datapolicies_v1
+            from google.cloud import bigquery_datapolicies_v1
 
             async def sample_delete_data_policy():
                 # Create a client
-                client = datapolicies_v1.DataPolicyServiceAsyncClient()
+                client = bigquery_datapolicies_v1.DataPolicyServiceAsyncClient()
 
                 # Initialize request argument(s)
-                request = datapolicies_v1.DeleteDataPolicyRequest(
+                request = bigquery_datapolicies_v1.DeleteDataPolicyRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 await client.delete_data_policy(request=request)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.datapolicies_v1.types.DeleteDataPolicyRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_datapolicies_v1.types.DeleteDataPolicyRequest, dict]]):
                 The request object. Request message for the
                 DeleteDataPolicy method.
             name (:class:`str`):
                 Required. Resource name of the data policy to delete.
                 Format is
                 ``projects/{project_number}/locations/{location_id}/dataPolicies/{data_policy_id}``.
 
@@ -723,33 +723,33 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import datapolicies_v1
+            from google.cloud import bigquery_datapolicies_v1
 
             async def sample_get_data_policy():
                 # Create a client
-                client = datapolicies_v1.DataPolicyServiceAsyncClient()
+                client = bigquery_datapolicies_v1.DataPolicyServiceAsyncClient()
 
                 # Initialize request argument(s)
-                request = datapolicies_v1.GetDataPolicyRequest(
+                request = bigquery_datapolicies_v1.GetDataPolicyRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 response = await client.get_data_policy(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.datapolicies_v1.types.GetDataPolicyRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_datapolicies_v1.types.GetDataPolicyRequest, dict]]):
                 The request object. Request message for the GetDataPolicy
                 method.
             name (:class:`str`):
                 Required. Resource name of the requested data policy.
                 Format is
                 ``projects/{project_number}/locations/{location_id}/dataPolicies/{data_policy_id}``.
 
@@ -759,15 +759,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.datapolicies_v1.types.DataPolicy:
+            google.cloud.bigquery_datapolicies_v1.types.DataPolicy:
                 Represents the label-policy binding.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
@@ -834,34 +834,34 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import datapolicies_v1
+            from google.cloud import bigquery_datapolicies_v1
 
             async def sample_list_data_policies():
                 # Create a client
-                client = datapolicies_v1.DataPolicyServiceAsyncClient()
+                client = bigquery_datapolicies_v1.DataPolicyServiceAsyncClient()
 
                 # Initialize request argument(s)
-                request = datapolicies_v1.ListDataPoliciesRequest(
+                request = bigquery_datapolicies_v1.ListDataPoliciesRequest(
                     parent="parent_value",
                 )
 
                 # Make the request
                 page_result = client.list_data_policies(request=request)
 
                 # Handle the response
                 async for response in page_result:
                     print(response)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.datapolicies_v1.types.ListDataPoliciesRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_datapolicies_v1.types.ListDataPoliciesRequest, dict]]):
                 The request object. Request message for the
                 ListDataPolicies method.
             parent (:class:`str`):
                 Required. Resource name of the project for which to list
                 data policies. Format is
                 ``projects/{project_number}/locations/{location_id}``.
 
@@ -871,15 +871,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.datapolicies_v1.services.data_policy_service.pagers.ListDataPoliciesAsyncPager:
+            google.cloud.bigquery_datapolicies_v1.services.data_policy_service.pagers.ListDataPoliciesAsyncPager:
                 Response message for the
                 ListDataPolicies method.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
@@ -958,20 +958,20 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import datapolicies_v1
+            from google.cloud import bigquery_datapolicies_v1
             from google.iam.v1 import iam_policy_pb2  # type: ignore
 
             async def sample_get_iam_policy():
                 # Create a client
-                client = datapolicies_v1.DataPolicyServiceAsyncClient()
+                client = bigquery_datapolicies_v1.DataPolicyServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = iam_policy_pb2.GetIamPolicyRequest(
                     resource="resource_value",
                 )
 
                 # Make the request
@@ -1109,20 +1109,20 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import datapolicies_v1
+            from google.cloud import bigquery_datapolicies_v1
             from google.iam.v1 import iam_policy_pb2  # type: ignore
 
             async def sample_set_iam_policy():
                 # Create a client
-                client = datapolicies_v1.DataPolicyServiceAsyncClient()
+                client = bigquery_datapolicies_v1.DataPolicyServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = iam_policy_pb2.SetIamPolicyRequest(
                     resource="resource_value",
                 )
 
                 # Make the request
@@ -1261,20 +1261,20 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import datapolicies_v1
+            from google.cloud import bigquery_datapolicies_v1
             from google.iam.v1 import iam_policy_pb2  # type: ignore
 
             async def sample_test_iam_permissions():
                 # Create a client
-                client = datapolicies_v1.DataPolicyServiceAsyncClient()
+                client = bigquery_datapolicies_v1.DataPolicyServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = iam_policy_pb2.TestIamPermissionsRequest(
                     resource="resource_value",
                     permissions=['permissions_value1', 'permissions_value2'],
                 )
```

### Comparing `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/client.py` & `google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,27 +35,27 @@
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.exceptions import MutualTLSChannelError  # type: ignore
 from google.auth.transport import mtls  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 
-from google.cloud.bigquery.datapolicies_v1 import gapic_version as package_version
+from google.cloud.bigquery_datapolicies_v1 import gapic_version as package_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.iam.v1 import iam_policy_pb2  # type: ignore
 from google.iam.v1 import policy_pb2  # type: ignore
 from google.protobuf import field_mask_pb2  # type: ignore
 
-from google.cloud.bigquery.datapolicies_v1.services.data_policy_service import pagers
-from google.cloud.bigquery.datapolicies_v1.types import datapolicy
+from google.cloud.bigquery_datapolicies_v1.services.data_policy_service import pagers
+from google.cloud.bigquery_datapolicies_v1.types import datapolicy
 
 from .transports.base import DEFAULT_CLIENT_INFO, DataPolicyServiceTransport
 from .transports.grpc import DataPolicyServiceGrpcTransport
 from .transports.grpc_asyncio import DataPolicyServiceGrpcAsyncIOTransport
 from .transports.rest import DataPolicyServiceRestTransport
 
 
@@ -470,64 +470,64 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import datapolicies_v1
+            from google.cloud import bigquery_datapolicies_v1
 
             def sample_create_data_policy():
                 # Create a client
-                client = datapolicies_v1.DataPolicyServiceClient()
+                client = bigquery_datapolicies_v1.DataPolicyServiceClient()
 
                 # Initialize request argument(s)
-                data_policy = datapolicies_v1.DataPolicy()
+                data_policy = bigquery_datapolicies_v1.DataPolicy()
                 data_policy.policy_tag = "policy_tag_value"
                 data_policy.data_masking_policy.predefined_expression = "DEFAULT_MASKING_VALUE"
 
-                request = datapolicies_v1.CreateDataPolicyRequest(
+                request = bigquery_datapolicies_v1.CreateDataPolicyRequest(
                     parent="parent_value",
                     data_policy=data_policy,
                 )
 
                 # Make the request
                 response = client.create_data_policy(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.bigquery.datapolicies_v1.types.CreateDataPolicyRequest, dict]):
+            request (Union[google.cloud.bigquery_datapolicies_v1.types.CreateDataPolicyRequest, dict]):
                 The request object. Request message for the
                 CreateDataPolicy method.
             parent (str):
                 Required. Resource name of the project that the data
                 policy will belong to. The format is
                 ``projects/{project_number}/locations/{location_id}``.
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            data_policy (google.cloud.bigquery.datapolicies_v1.types.DataPolicy):
+            data_policy (google.cloud.bigquery_datapolicies_v1.types.DataPolicy):
                 Required. The data policy to create. The ``name`` field
                 does not need to be provided for the data policy
                 creation.
 
                 This corresponds to the ``data_policy`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.datapolicies_v1.types.DataPolicy:
+            google.cloud.bigquery_datapolicies_v1.types.DataPolicy:
                 Represents the label-policy binding.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, data_policy])
         if request is not None and has_flattened_params:
@@ -589,40 +589,40 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import datapolicies_v1
+            from google.cloud import bigquery_datapolicies_v1
 
             def sample_update_data_policy():
                 # Create a client
-                client = datapolicies_v1.DataPolicyServiceClient()
+                client = bigquery_datapolicies_v1.DataPolicyServiceClient()
 
                 # Initialize request argument(s)
-                data_policy = datapolicies_v1.DataPolicy()
+                data_policy = bigquery_datapolicies_v1.DataPolicy()
                 data_policy.policy_tag = "policy_tag_value"
                 data_policy.data_masking_policy.predefined_expression = "DEFAULT_MASKING_VALUE"
 
-                request = datapolicies_v1.UpdateDataPolicyRequest(
+                request = bigquery_datapolicies_v1.UpdateDataPolicyRequest(
                     data_policy=data_policy,
                 )
 
                 # Make the request
                 response = client.update_data_policy(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.bigquery.datapolicies_v1.types.UpdateDataPolicyRequest, dict]):
+            request (Union[google.cloud.bigquery_datapolicies_v1.types.UpdateDataPolicyRequest, dict]):
                 The request object. Response message for the
                 UpdateDataPolicy method.
-            data_policy (google.cloud.bigquery.datapolicies_v1.types.DataPolicy):
+            data_policy (google.cloud.bigquery_datapolicies_v1.types.DataPolicy):
                 Required. Update the data policy's metadata.
 
                 The target data policy is determined by the ``name``
                 field. Other fields are updated to the specified values
                 based on the field masks.
 
                 This corresponds to the ``data_policy`` field
@@ -644,15 +644,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.datapolicies_v1.types.DataPolicy:
+            google.cloud.bigquery_datapolicies_v1.types.DataPolicy:
                 Represents the label-policy binding.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([data_policy, update_mask])
         if request is not None and has_flattened_params:
@@ -715,34 +715,34 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import datapolicies_v1
+            from google.cloud import bigquery_datapolicies_v1
 
             def sample_rename_data_policy():
                 # Create a client
-                client = datapolicies_v1.DataPolicyServiceClient()
+                client = bigquery_datapolicies_v1.DataPolicyServiceClient()
 
                 # Initialize request argument(s)
-                request = datapolicies_v1.RenameDataPolicyRequest(
+                request = bigquery_datapolicies_v1.RenameDataPolicyRequest(
                     name="name_value",
                     new_data_policy_id="new_data_policy_id_value",
                 )
 
                 # Make the request
                 response = client.rename_data_policy(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.bigquery.datapolicies_v1.types.RenameDataPolicyRequest, dict]):
+            request (Union[google.cloud.bigquery_datapolicies_v1.types.RenameDataPolicyRequest, dict]):
                 The request object. Request message for the
                 RenameDataPolicy method.
             name (str):
                 Required. Resource name of the data policy to rename.
                 The format is
                 ``projects/{project_number}/locations/{location_id}/dataPolicies/{data_policy_id}``
 
@@ -757,15 +757,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.datapolicies_v1.types.DataPolicy:
+            google.cloud.bigquery_datapolicies_v1.types.DataPolicy:
                 Represents the label-policy binding.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name, new_data_policy_id])
         if request is not None and has_flattened_params:
@@ -825,30 +825,30 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import datapolicies_v1
+            from google.cloud import bigquery_datapolicies_v1
 
             def sample_delete_data_policy():
                 # Create a client
-                client = datapolicies_v1.DataPolicyServiceClient()
+                client = bigquery_datapolicies_v1.DataPolicyServiceClient()
 
                 # Initialize request argument(s)
-                request = datapolicies_v1.DeleteDataPolicyRequest(
+                request = bigquery_datapolicies_v1.DeleteDataPolicyRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 client.delete_data_policy(request=request)
 
         Args:
-            request (Union[google.cloud.bigquery.datapolicies_v1.types.DeleteDataPolicyRequest, dict]):
+            request (Union[google.cloud.bigquery_datapolicies_v1.types.DeleteDataPolicyRequest, dict]):
                 The request object. Request message for the
                 DeleteDataPolicy method.
             name (str):
                 Required. Resource name of the data policy to delete.
                 Format is
                 ``projects/{project_number}/locations/{location_id}/dataPolicies/{data_policy_id}``.
 
@@ -916,33 +916,33 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import datapolicies_v1
+            from google.cloud import bigquery_datapolicies_v1
 
             def sample_get_data_policy():
                 # Create a client
-                client = datapolicies_v1.DataPolicyServiceClient()
+                client = bigquery_datapolicies_v1.DataPolicyServiceClient()
 
                 # Initialize request argument(s)
-                request = datapolicies_v1.GetDataPolicyRequest(
+                request = bigquery_datapolicies_v1.GetDataPolicyRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 response = client.get_data_policy(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.bigquery.datapolicies_v1.types.GetDataPolicyRequest, dict]):
+            request (Union[google.cloud.bigquery_datapolicies_v1.types.GetDataPolicyRequest, dict]):
                 The request object. Request message for the GetDataPolicy
                 method.
             name (str):
                 Required. Resource name of the requested data policy.
                 Format is
                 ``projects/{project_number}/locations/{location_id}/dataPolicies/{data_policy_id}``.
 
@@ -952,15 +952,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.datapolicies_v1.types.DataPolicy:
+            google.cloud.bigquery_datapolicies_v1.types.DataPolicy:
                 Represents the label-policy binding.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
@@ -1018,34 +1018,34 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import datapolicies_v1
+            from google.cloud import bigquery_datapolicies_v1
 
             def sample_list_data_policies():
                 # Create a client
-                client = datapolicies_v1.DataPolicyServiceClient()
+                client = bigquery_datapolicies_v1.DataPolicyServiceClient()
 
                 # Initialize request argument(s)
-                request = datapolicies_v1.ListDataPoliciesRequest(
+                request = bigquery_datapolicies_v1.ListDataPoliciesRequest(
                     parent="parent_value",
                 )
 
                 # Make the request
                 page_result = client.list_data_policies(request=request)
 
                 # Handle the response
                 for response in page_result:
                     print(response)
 
         Args:
-            request (Union[google.cloud.bigquery.datapolicies_v1.types.ListDataPoliciesRequest, dict]):
+            request (Union[google.cloud.bigquery_datapolicies_v1.types.ListDataPoliciesRequest, dict]):
                 The request object. Request message for the
                 ListDataPolicies method.
             parent (str):
                 Required. Resource name of the project for which to list
                 data policies. Format is
                 ``projects/{project_number}/locations/{location_id}``.
 
@@ -1055,15 +1055,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.datapolicies_v1.services.data_policy_service.pagers.ListDataPoliciesPager:
+            google.cloud.bigquery_datapolicies_v1.services.data_policy_service.pagers.ListDataPoliciesPager:
                 Response message for the
                 ListDataPolicies method.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
@@ -1133,20 +1133,20 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import datapolicies_v1
+            from google.cloud import bigquery_datapolicies_v1
             from google.iam.v1 import iam_policy_pb2  # type: ignore
 
             def sample_get_iam_policy():
                 # Create a client
-                client = datapolicies_v1.DataPolicyServiceClient()
+                client = bigquery_datapolicies_v1.DataPolicyServiceClient()
 
                 # Initialize request argument(s)
                 request = iam_policy_pb2.GetIamPolicyRequest(
                     resource="resource_value",
                 )
 
                 # Make the request
@@ -1274,20 +1274,20 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import datapolicies_v1
+            from google.cloud import bigquery_datapolicies_v1
             from google.iam.v1 import iam_policy_pb2  # type: ignore
 
             def sample_set_iam_policy():
                 # Create a client
-                client = datapolicies_v1.DataPolicyServiceClient()
+                client = bigquery_datapolicies_v1.DataPolicyServiceClient()
 
                 # Initialize request argument(s)
                 request = iam_policy_pb2.SetIamPolicyRequest(
                     resource="resource_value",
                 )
 
                 # Make the request
@@ -1416,20 +1416,20 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import datapolicies_v1
+            from google.cloud import bigquery_datapolicies_v1
             from google.iam.v1 import iam_policy_pb2  # type: ignore
 
             def sample_test_iam_permissions():
                 # Create a client
-                client = datapolicies_v1.DataPolicyServiceClient()
+                client = bigquery_datapolicies_v1.DataPolicyServiceClient()
 
                 # Initialize request argument(s)
                 request = iam_policy_pb2.TestIamPermissionsRequest(
                     resource="resource_value",
                     permissions=['permissions_value1', 'permissions_value2'],
                 )
```

### Comparing `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/pagers.py` & `google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/pagers.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,31 +20,31 @@
     Callable,
     Iterator,
     Optional,
     Sequence,
     Tuple,
 )
 
-from google.cloud.bigquery.datapolicies_v1.types import datapolicy
+from google.cloud.bigquery_datapolicies_v1.types import datapolicy
 
 
 class ListDataPoliciesPager:
     """A pager for iterating through ``list_data_policies`` requests.
 
     This class thinly wraps an initial
-    :class:`google.cloud.bigquery.datapolicies_v1.types.ListDataPoliciesResponse` object, and
+    :class:`google.cloud.bigquery_datapolicies_v1.types.ListDataPoliciesResponse` object, and
     provides an ``__iter__`` method to iterate through its
     ``data_policies`` field.
 
     If there are more pages, the ``__iter__`` method will make additional
     ``ListDataPolicies`` requests and continue to iterate
     through the ``data_policies`` field on the
     corresponding responses.
 
-    All the usual :class:`google.cloud.bigquery.datapolicies_v1.types.ListDataPoliciesResponse`
+    All the usual :class:`google.cloud.bigquery_datapolicies_v1.types.ListDataPoliciesResponse`
     attributes are available on the pager. If multiple requests are made, only
     the most recent response is retained, and thus used for attribute lookup.
     """
 
     def __init__(
         self,
         method: Callable[..., datapolicy.ListDataPoliciesResponse],
@@ -54,17 +54,17 @@
         metadata: Sequence[Tuple[str, str]] = ()
     ):
         """Instantiate the pager.
 
         Args:
             method (Callable): The method that was originally called, and
                 which instantiated this pager.
-            request (google.cloud.bigquery.datapolicies_v1.types.ListDataPoliciesRequest):
+            request (google.cloud.bigquery_datapolicies_v1.types.ListDataPoliciesRequest):
                 The initial request object.
-            response (google.cloud.bigquery.datapolicies_v1.types.ListDataPoliciesResponse):
+            response (google.cloud.bigquery_datapolicies_v1.types.ListDataPoliciesResponse):
                 The initial response object.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         self._method = method
         self._request = datapolicy.ListDataPoliciesRequest(request)
         self._response = response
@@ -89,24 +89,24 @@
         return "{0}<{1!r}>".format(self.__class__.__name__, self._response)
 
 
 class ListDataPoliciesAsyncPager:
     """A pager for iterating through ``list_data_policies`` requests.
 
     This class thinly wraps an initial
-    :class:`google.cloud.bigquery.datapolicies_v1.types.ListDataPoliciesResponse` object, and
+    :class:`google.cloud.bigquery_datapolicies_v1.types.ListDataPoliciesResponse` object, and
     provides an ``__aiter__`` method to iterate through its
     ``data_policies`` field.
 
     If there are more pages, the ``__aiter__`` method will make additional
     ``ListDataPolicies`` requests and continue to iterate
     through the ``data_policies`` field on the
     corresponding responses.
 
-    All the usual :class:`google.cloud.bigquery.datapolicies_v1.types.ListDataPoliciesResponse`
+    All the usual :class:`google.cloud.bigquery_datapolicies_v1.types.ListDataPoliciesResponse`
     attributes are available on the pager. If multiple requests are made, only
     the most recent response is retained, and thus used for attribute lookup.
     """
 
     def __init__(
         self,
         method: Callable[..., Awaitable[datapolicy.ListDataPoliciesResponse]],
@@ -116,17 +116,17 @@
         metadata: Sequence[Tuple[str, str]] = ()
     ):
         """Instantiates the pager.
 
         Args:
             method (Callable): The method that was originally called, and
                 which instantiated this pager.
-            request (google.cloud.bigquery.datapolicies_v1.types.ListDataPoliciesRequest):
+            request (google.cloud.bigquery_datapolicies_v1.types.ListDataPoliciesRequest):
                 The initial request object.
-            response (google.cloud.bigquery.datapolicies_v1.types.ListDataPoliciesResponse):
+            response (google.cloud.bigquery_datapolicies_v1.types.ListDataPoliciesResponse):
                 The initial response object.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         self._method = method
         self._request = datapolicy.ListDataPoliciesRequest(request)
         self._response = response
```

### Comparing `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/transports/__init__.py` & `google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/transports/base.py` & `google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/transports/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.iam.v1 import iam_policy_pb2  # type: ignore
 from google.iam.v1 import policy_pb2  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 from google.protobuf import empty_pb2  # type: ignore
 
-from google.cloud.bigquery.datapolicies_v1 import gapic_version as package_version
-from google.cloud.bigquery.datapolicies_v1.types import datapolicy
+from google.cloud.bigquery_datapolicies_v1 import gapic_version as package_version
+from google.cloud.bigquery_datapolicies_v1.types import datapolicy
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
     gapic_version=package_version.__version__
 )
 
 
 class DataPolicyServiceTransport(abc.ABC):
```

### Comparing `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/transports/grpc.py` & `google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/transports/grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.iam.v1 import iam_policy_pb2  # type: ignore
 from google.iam.v1 import policy_pb2  # type: ignore
 from google.protobuf import empty_pb2  # type: ignore
 import grpc  # type: ignore
 
-from google.cloud.bigquery.datapolicies_v1.types import datapolicy
+from google.cloud.bigquery_datapolicies_v1.types import datapolicy
 
 from .base import DEFAULT_CLIENT_INFO, DataPolicyServiceTransport
 
 
 class DataPolicyServiceGrpcTransport(DataPolicyServiceTransport):
     """gRPC backend transport for DataPolicyService.
```

### Comparing `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/transports/grpc_asyncio.py` & `google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/transports/grpc_asyncio.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.iam.v1 import iam_policy_pb2  # type: ignore
 from google.iam.v1 import policy_pb2  # type: ignore
 from google.protobuf import empty_pb2  # type: ignore
 import grpc  # type: ignore
 from grpc.experimental import aio  # type: ignore
 
-from google.cloud.bigquery.datapolicies_v1.types import datapolicy
+from google.cloud.bigquery_datapolicies_v1.types import datapolicy
 
 from .base import DEFAULT_CLIENT_INFO, DataPolicyServiceTransport
 from .grpc import DataPolicyServiceGrpcTransport
 
 
 class DataPolicyServiceGrpcAsyncIOTransport(DataPolicyServiceTransport):
     """gRPC AsyncIO backend transport for DataPolicyService.
```

### Comparing `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/transports/rest.py` & `google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 
 from google.iam.v1 import iam_policy_pb2  # type: ignore
 from google.iam.v1 import policy_pb2  # type: ignore
 from google.protobuf import empty_pb2  # type: ignore
 
-from google.cloud.bigquery.datapolicies_v1.types import datapolicy
+from google.cloud.bigquery_datapolicies_v1.types import datapolicy
 
 from .base import DEFAULT_CLIENT_INFO as BASE_DEFAULT_CLIENT_INFO
 from .base import DataPolicyServiceTransport
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
     gapic_version=BASE_DEFAULT_CLIENT_INFO.gapic_version,
     grpc_version=None,
```

### Comparing `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/types/__init__.py` & `google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/types/datapolicy.py` & `google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1/types/datapolicy.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     r"""Request message for the CreateDataPolicy method.
 
     Attributes:
         parent (str):
             Required. Resource name of the project that the data policy
             will belong to. The format is
             ``projects/{project_number}/locations/{location_id}``.
-        data_policy (google.cloud.bigquery.datapolicies_v1.types.DataPolicy):
+        data_policy (google.cloud.bigquery_datapolicies_v1.types.DataPolicy):
             Required. The data policy to create. The ``name`` field does
             not need to be provided for the data policy creation.
     """
 
     parent: str = proto.Field(
         proto.STRING,
         number=1,
@@ -60,15 +60,15 @@
     )
 
 
 class UpdateDataPolicyRequest(proto.Message):
     r"""Response message for the UpdateDataPolicy method.
 
     Attributes:
-        data_policy (google.cloud.bigquery.datapolicies_v1.types.DataPolicy):
+        data_policy (google.cloud.bigquery_datapolicies_v1.types.DataPolicy):
             Required. Update the data policy's metadata.
 
             The target data policy is determined by the ``name`` field.
             Other fields are updated to the specified values based on
             the field masks.
         update_mask (google.protobuf.field_mask_pb2.FieldMask):
             The update mask applies to the resource. For the
@@ -190,15 +190,15 @@
     )
 
 
 class ListDataPoliciesResponse(proto.Message):
     r"""Response message for the ListDataPolicies method.
 
     Attributes:
-        data_policies (MutableSequence[google.cloud.bigquery.datapolicies_v1.types.DataPolicy]):
+        data_policies (MutableSequence[google.cloud.bigquery_datapolicies_v1.types.DataPolicy]):
             Data policies that belong to the requested
             project.
         next_page_token (str):
             Token used to retrieve the next page of
             results, or empty if there are no more results.
     """
 
@@ -224,24 +224,24 @@
 
     Attributes:
         policy_tag (str):
             Policy tag resource name, in the format of
             ``projects/{project_number}/locations/{location_id}/taxonomies/{taxonomy_id}/policyTags/{policyTag_id}``.
 
             This field is a member of `oneof`_ ``matching_label``.
-        data_masking_policy (google.cloud.bigquery.datapolicies_v1.types.DataMaskingPolicy):
+        data_masking_policy (google.cloud.bigquery_datapolicies_v1.types.DataMaskingPolicy):
             The data masking policy that specifies the
             data masking rule to use.
 
             This field is a member of `oneof`_ ``policy``.
         name (str):
             Output only. Resource name of this data policy, in the
             format of
             ``projects/{project_number}/locations/{location_id}/dataPolicies/{data_policy_id}``.
-        data_policy_type (google.cloud.bigquery.datapolicies_v1.types.DataPolicy.DataPolicyType):
+        data_policy_type (google.cloud.bigquery_datapolicies_v1.types.DataPolicy.DataPolicyType):
             Type of data policy.
         data_policy_id (str):
             User-assigned (human readable) ID of the data policy that
             needs to be unique within a project. Used as
             {data_policy_id} in part of the resource name.
     """
 
@@ -293,15 +293,15 @@
     r"""The data masking policy that is used to specify data masking
     rule.
 
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
     Attributes:
-        predefined_expression (google.cloud.bigquery.datapolicies_v1.types.DataMaskingPolicy.PredefinedExpression):
+        predefined_expression (google.cloud.bigquery_datapolicies_v1.types.DataMaskingPolicy.PredefinedExpression):
             A predefined masking expression.
 
             This field is a member of `oneof`_ ``masking_expression``.
     """
 
     class PredefinedExpression(proto.Enum):
         r"""The available masking rules. Learn more here:
```

### Comparing `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/__init__.py` & `google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1beta1/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from google.cloud.bigquery.datapolicies_v1beta1 import gapic_version as package_version
+from google.cloud.bigquery_datapolicies_v1beta1 import gapic_version as package_version
 
 __version__ = package_version.__version__
 
 
 from .services.data_policy_service import (
     DataPolicyServiceAsyncClient,
     DataPolicyServiceClient,
```

### Comparing `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/gapic_metadata.json` & `google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1beta1/gapic_metadata.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'libraryPackage'": "'google.cloud.bigquery_datapolicies_v1beta1'"}*

```diff
@@ -1,11 +1,11 @@
 {
     "comment": "This file maps proto services/RPCs to the corresponding library clients/methods",
     "language": "python",
-    "libraryPackage": "google.cloud.bigquery.datapolicies_v1beta1",
+    "libraryPackage": "google.cloud.bigquery_datapolicies_v1beta1",
     "protoPackage": "google.cloud.bigquery.datapolicies.v1beta1",
     "schema": "1.0",
     "services": {
         "DataPolicyService": {
             "clients": {
                 "grpc": {
                     "libraryClient": "DataPolicyServiceClient",
```

### Comparing `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/gapic_version.py` & `google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1beta1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.4.0"  # {x-release-please-version}
+__version__ = "0.5.0"  # {x-release-please-version}
```

### Comparing `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/services/__init__.py` & `google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/__init__.py` & `google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/async_client.py` & `google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/async_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,29 +31,29 @@
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.api_core.client_options import ClientOptions
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 
-from google.cloud.bigquery.datapolicies_v1beta1 import gapic_version as package_version
+from google.cloud.bigquery_datapolicies_v1beta1 import gapic_version as package_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.iam.v1 import iam_policy_pb2  # type: ignore
 from google.iam.v1 import policy_pb2  # type: ignore
 from google.protobuf import field_mask_pb2  # type: ignore
 
-from google.cloud.bigquery.datapolicies_v1beta1.services.data_policy_service import (
+from google.cloud.bigquery_datapolicies_v1beta1.services.data_policy_service import (
     pagers,
 )
-from google.cloud.bigquery.datapolicies_v1beta1.types import datapolicy
+from google.cloud.bigquery_datapolicies_v1beta1.types import datapolicy
 
 from .client import DataPolicyServiceClient
 from .transports.base import DEFAULT_CLIENT_INFO, DataPolicyServiceTransport
 from .transports.grpc_asyncio import DataPolicyServiceGrpcAsyncIOTransport
 
 
 class DataPolicyServiceAsyncClient:
@@ -243,64 +243,64 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import datapolicies_v1beta1
+            from google.cloud import bigquery_datapolicies_v1beta1
 
             async def sample_create_data_policy():
                 # Create a client
-                client = datapolicies_v1beta1.DataPolicyServiceAsyncClient()
+                client = bigquery_datapolicies_v1beta1.DataPolicyServiceAsyncClient()
 
                 # Initialize request argument(s)
-                data_policy = datapolicies_v1beta1.DataPolicy()
+                data_policy = bigquery_datapolicies_v1beta1.DataPolicy()
                 data_policy.policy_tag = "policy_tag_value"
                 data_policy.data_masking_policy.predefined_expression = "DEFAULT_MASKING_VALUE"
 
-                request = datapolicies_v1beta1.CreateDataPolicyRequest(
+                request = bigquery_datapolicies_v1beta1.CreateDataPolicyRequest(
                     parent="parent_value",
                     data_policy=data_policy,
                 )
 
                 # Make the request
                 response = await client.create_data_policy(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.datapolicies_v1beta1.types.CreateDataPolicyRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_datapolicies_v1beta1.types.CreateDataPolicyRequest, dict]]):
                 The request object. Request message for the
                 CreateDataPolicy method.
             parent (:class:`str`):
                 Required. Resource name of the project that the data
                 policy will belong to. The format is
                 ``projects/{project_number}/locations/{location_id}``.
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            data_policy (:class:`google.cloud.bigquery.datapolicies_v1beta1.types.DataPolicy`):
+            data_policy (:class:`google.cloud.bigquery_datapolicies_v1beta1.types.DataPolicy`):
                 Required. The data policy to create. The ``name`` field
                 does not need to be provided for the data policy
                 creation.
 
                 This corresponds to the ``data_policy`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.datapolicies_v1beta1.types.DataPolicy:
+            google.cloud.bigquery_datapolicies_v1beta1.types.DataPolicy:
                 Represents the label-policy binding.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, data_policy])
         if request is not None and has_flattened_params:
@@ -371,40 +371,40 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import datapolicies_v1beta1
+            from google.cloud import bigquery_datapolicies_v1beta1
 
             async def sample_update_data_policy():
                 # Create a client
-                client = datapolicies_v1beta1.DataPolicyServiceAsyncClient()
+                client = bigquery_datapolicies_v1beta1.DataPolicyServiceAsyncClient()
 
                 # Initialize request argument(s)
-                data_policy = datapolicies_v1beta1.DataPolicy()
+                data_policy = bigquery_datapolicies_v1beta1.DataPolicy()
                 data_policy.policy_tag = "policy_tag_value"
                 data_policy.data_masking_policy.predefined_expression = "DEFAULT_MASKING_VALUE"
 
-                request = datapolicies_v1beta1.UpdateDataPolicyRequest(
+                request = bigquery_datapolicies_v1beta1.UpdateDataPolicyRequest(
                     data_policy=data_policy,
                 )
 
                 # Make the request
                 response = await client.update_data_policy(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.datapolicies_v1beta1.types.UpdateDataPolicyRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_datapolicies_v1beta1.types.UpdateDataPolicyRequest, dict]]):
                 The request object. Response message for the
                 UpdateDataPolicy method.
-            data_policy (:class:`google.cloud.bigquery.datapolicies_v1beta1.types.DataPolicy`):
+            data_policy (:class:`google.cloud.bigquery_datapolicies_v1beta1.types.DataPolicy`):
                 Required. Update the data policy's metadata.
 
                 The target data policy is determined by the ``name``
                 field. Other fields are updated to the specified values
                 based on the field masks.
 
                 This corresponds to the ``data_policy`` field
@@ -426,15 +426,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.datapolicies_v1beta1.types.DataPolicy:
+            google.cloud.bigquery_datapolicies_v1beta1.types.DataPolicy:
                 Represents the label-policy binding.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([data_policy, update_mask])
         if request is not None and has_flattened_params:
@@ -505,30 +505,30 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import datapolicies_v1beta1
+            from google.cloud import bigquery_datapolicies_v1beta1
 
             async def sample_delete_data_policy():
                 # Create a client
-                client = datapolicies_v1beta1.DataPolicyServiceAsyncClient()
+                client = bigquery_datapolicies_v1beta1.DataPolicyServiceAsyncClient()
 
                 # Initialize request argument(s)
-                request = datapolicies_v1beta1.DeleteDataPolicyRequest(
+                request = bigquery_datapolicies_v1beta1.DeleteDataPolicyRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 await client.delete_data_policy(request=request)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.datapolicies_v1beta1.types.DeleteDataPolicyRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_datapolicies_v1beta1.types.DeleteDataPolicyRequest, dict]]):
                 The request object. Request message for the
                 DeleteDataPolicy method.
             name (:class:`str`):
                 Required. Resource name of the data policy to delete.
                 Format is
                 ``projects/{project_number}/locations/{location_id}/dataPolicies/{data_policy_id}``.
 
@@ -605,33 +605,33 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import datapolicies_v1beta1
+            from google.cloud import bigquery_datapolicies_v1beta1
 
             async def sample_get_data_policy():
                 # Create a client
-                client = datapolicies_v1beta1.DataPolicyServiceAsyncClient()
+                client = bigquery_datapolicies_v1beta1.DataPolicyServiceAsyncClient()
 
                 # Initialize request argument(s)
-                request = datapolicies_v1beta1.GetDataPolicyRequest(
+                request = bigquery_datapolicies_v1beta1.GetDataPolicyRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 response = await client.get_data_policy(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.datapolicies_v1beta1.types.GetDataPolicyRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_datapolicies_v1beta1.types.GetDataPolicyRequest, dict]]):
                 The request object. Request message for the GetDataPolicy
                 method.
             name (:class:`str`):
                 Required. Resource name of the requested data policy.
                 Format is
                 ``projects/{project_number}/locations/{location_id}/dataPolicies/{data_policy_id}``.
 
@@ -641,15 +641,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.datapolicies_v1beta1.types.DataPolicy:
+            google.cloud.bigquery_datapolicies_v1beta1.types.DataPolicy:
                 Represents the label-policy binding.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
@@ -716,34 +716,34 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import datapolicies_v1beta1
+            from google.cloud import bigquery_datapolicies_v1beta1
 
             async def sample_list_data_policies():
                 # Create a client
-                client = datapolicies_v1beta1.DataPolicyServiceAsyncClient()
+                client = bigquery_datapolicies_v1beta1.DataPolicyServiceAsyncClient()
 
                 # Initialize request argument(s)
-                request = datapolicies_v1beta1.ListDataPoliciesRequest(
+                request = bigquery_datapolicies_v1beta1.ListDataPoliciesRequest(
                     parent="parent_value",
                 )
 
                 # Make the request
                 page_result = client.list_data_policies(request=request)
 
                 # Handle the response
                 async for response in page_result:
                     print(response)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.datapolicies_v1beta1.types.ListDataPoliciesRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_datapolicies_v1beta1.types.ListDataPoliciesRequest, dict]]):
                 The request object. Request message for the
                 ListDataPolicies method.
             parent (:class:`str`):
                 Required. Resource name of the project for which to list
                 data policies. Format is
                 ``projects/{project_number}/locations/{location_id}``.
 
@@ -753,15 +753,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.datapolicies_v1beta1.services.data_policy_service.pagers.ListDataPoliciesAsyncPager:
+            google.cloud.bigquery_datapolicies_v1beta1.services.data_policy_service.pagers.ListDataPoliciesAsyncPager:
                 Response message for the
                 ListDataPolicies method.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
@@ -840,20 +840,20 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import datapolicies_v1beta1
+            from google.cloud import bigquery_datapolicies_v1beta1
             from google.iam.v1 import iam_policy_pb2  # type: ignore
 
             async def sample_get_iam_policy():
                 # Create a client
-                client = datapolicies_v1beta1.DataPolicyServiceAsyncClient()
+                client = bigquery_datapolicies_v1beta1.DataPolicyServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = iam_policy_pb2.GetIamPolicyRequest(
                     resource="resource_value",
                 )
 
                 # Make the request
@@ -991,20 +991,20 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import datapolicies_v1beta1
+            from google.cloud import bigquery_datapolicies_v1beta1
             from google.iam.v1 import iam_policy_pb2  # type: ignore
 
             async def sample_set_iam_policy():
                 # Create a client
-                client = datapolicies_v1beta1.DataPolicyServiceAsyncClient()
+                client = bigquery_datapolicies_v1beta1.DataPolicyServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = iam_policy_pb2.SetIamPolicyRequest(
                     resource="resource_value",
                 )
 
                 # Make the request
@@ -1143,20 +1143,20 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import datapolicies_v1beta1
+            from google.cloud import bigquery_datapolicies_v1beta1
             from google.iam.v1 import iam_policy_pb2  # type: ignore
 
             async def sample_test_iam_permissions():
                 # Create a client
-                client = datapolicies_v1beta1.DataPolicyServiceAsyncClient()
+                client = bigquery_datapolicies_v1beta1.DataPolicyServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = iam_policy_pb2.TestIamPermissionsRequest(
                     resource="resource_value",
                     permissions=['permissions_value1', 'permissions_value2'],
                 )
```

### Comparing `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/client.py` & `google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,29 +35,29 @@
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.exceptions import MutualTLSChannelError  # type: ignore
 from google.auth.transport import mtls  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 
-from google.cloud.bigquery.datapolicies_v1beta1 import gapic_version as package_version
+from google.cloud.bigquery_datapolicies_v1beta1 import gapic_version as package_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.iam.v1 import iam_policy_pb2  # type: ignore
 from google.iam.v1 import policy_pb2  # type: ignore
 from google.protobuf import field_mask_pb2  # type: ignore
 
-from google.cloud.bigquery.datapolicies_v1beta1.services.data_policy_service import (
+from google.cloud.bigquery_datapolicies_v1beta1.services.data_policy_service import (
     pagers,
 )
-from google.cloud.bigquery.datapolicies_v1beta1.types import datapolicy
+from google.cloud.bigquery_datapolicies_v1beta1.types import datapolicy
 
 from .transports.base import DEFAULT_CLIENT_INFO, DataPolicyServiceTransport
 from .transports.grpc import DataPolicyServiceGrpcTransport
 from .transports.grpc_asyncio import DataPolicyServiceGrpcAsyncIOTransport
 
 
 class DataPolicyServiceClientMeta(type):
@@ -470,64 +470,64 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import datapolicies_v1beta1
+            from google.cloud import bigquery_datapolicies_v1beta1
 
             def sample_create_data_policy():
                 # Create a client
-                client = datapolicies_v1beta1.DataPolicyServiceClient()
+                client = bigquery_datapolicies_v1beta1.DataPolicyServiceClient()
 
                 # Initialize request argument(s)
-                data_policy = datapolicies_v1beta1.DataPolicy()
+                data_policy = bigquery_datapolicies_v1beta1.DataPolicy()
                 data_policy.policy_tag = "policy_tag_value"
                 data_policy.data_masking_policy.predefined_expression = "DEFAULT_MASKING_VALUE"
 
-                request = datapolicies_v1beta1.CreateDataPolicyRequest(
+                request = bigquery_datapolicies_v1beta1.CreateDataPolicyRequest(
                     parent="parent_value",
                     data_policy=data_policy,
                 )
 
                 # Make the request
                 response = client.create_data_policy(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.bigquery.datapolicies_v1beta1.types.CreateDataPolicyRequest, dict]):
+            request (Union[google.cloud.bigquery_datapolicies_v1beta1.types.CreateDataPolicyRequest, dict]):
                 The request object. Request message for the
                 CreateDataPolicy method.
             parent (str):
                 Required. Resource name of the project that the data
                 policy will belong to. The format is
                 ``projects/{project_number}/locations/{location_id}``.
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            data_policy (google.cloud.bigquery.datapolicies_v1beta1.types.DataPolicy):
+            data_policy (google.cloud.bigquery_datapolicies_v1beta1.types.DataPolicy):
                 Required. The data policy to create. The ``name`` field
                 does not need to be provided for the data policy
                 creation.
 
                 This corresponds to the ``data_policy`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.datapolicies_v1beta1.types.DataPolicy:
+            google.cloud.bigquery_datapolicies_v1beta1.types.DataPolicy:
                 Represents the label-policy binding.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, data_policy])
         if request is not None and has_flattened_params:
@@ -589,40 +589,40 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import datapolicies_v1beta1
+            from google.cloud import bigquery_datapolicies_v1beta1
 
             def sample_update_data_policy():
                 # Create a client
-                client = datapolicies_v1beta1.DataPolicyServiceClient()
+                client = bigquery_datapolicies_v1beta1.DataPolicyServiceClient()
 
                 # Initialize request argument(s)
-                data_policy = datapolicies_v1beta1.DataPolicy()
+                data_policy = bigquery_datapolicies_v1beta1.DataPolicy()
                 data_policy.policy_tag = "policy_tag_value"
                 data_policy.data_masking_policy.predefined_expression = "DEFAULT_MASKING_VALUE"
 
-                request = datapolicies_v1beta1.UpdateDataPolicyRequest(
+                request = bigquery_datapolicies_v1beta1.UpdateDataPolicyRequest(
                     data_policy=data_policy,
                 )
 
                 # Make the request
                 response = client.update_data_policy(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.bigquery.datapolicies_v1beta1.types.UpdateDataPolicyRequest, dict]):
+            request (Union[google.cloud.bigquery_datapolicies_v1beta1.types.UpdateDataPolicyRequest, dict]):
                 The request object. Response message for the
                 UpdateDataPolicy method.
-            data_policy (google.cloud.bigquery.datapolicies_v1beta1.types.DataPolicy):
+            data_policy (google.cloud.bigquery_datapolicies_v1beta1.types.DataPolicy):
                 Required. Update the data policy's metadata.
 
                 The target data policy is determined by the ``name``
                 field. Other fields are updated to the specified values
                 based on the field masks.
 
                 This corresponds to the ``data_policy`` field
@@ -644,15 +644,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.datapolicies_v1beta1.types.DataPolicy:
+            google.cloud.bigquery_datapolicies_v1beta1.types.DataPolicy:
                 Represents the label-policy binding.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([data_policy, update_mask])
         if request is not None and has_flattened_params:
@@ -714,30 +714,30 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import datapolicies_v1beta1
+            from google.cloud import bigquery_datapolicies_v1beta1
 
             def sample_delete_data_policy():
                 # Create a client
-                client = datapolicies_v1beta1.DataPolicyServiceClient()
+                client = bigquery_datapolicies_v1beta1.DataPolicyServiceClient()
 
                 # Initialize request argument(s)
-                request = datapolicies_v1beta1.DeleteDataPolicyRequest(
+                request = bigquery_datapolicies_v1beta1.DeleteDataPolicyRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 client.delete_data_policy(request=request)
 
         Args:
-            request (Union[google.cloud.bigquery.datapolicies_v1beta1.types.DeleteDataPolicyRequest, dict]):
+            request (Union[google.cloud.bigquery_datapolicies_v1beta1.types.DeleteDataPolicyRequest, dict]):
                 The request object. Request message for the
                 DeleteDataPolicy method.
             name (str):
                 Required. Resource name of the data policy to delete.
                 Format is
                 ``projects/{project_number}/locations/{location_id}/dataPolicies/{data_policy_id}``.
 
@@ -805,33 +805,33 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import datapolicies_v1beta1
+            from google.cloud import bigquery_datapolicies_v1beta1
 
             def sample_get_data_policy():
                 # Create a client
-                client = datapolicies_v1beta1.DataPolicyServiceClient()
+                client = bigquery_datapolicies_v1beta1.DataPolicyServiceClient()
 
                 # Initialize request argument(s)
-                request = datapolicies_v1beta1.GetDataPolicyRequest(
+                request = bigquery_datapolicies_v1beta1.GetDataPolicyRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 response = client.get_data_policy(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.bigquery.datapolicies_v1beta1.types.GetDataPolicyRequest, dict]):
+            request (Union[google.cloud.bigquery_datapolicies_v1beta1.types.GetDataPolicyRequest, dict]):
                 The request object. Request message for the GetDataPolicy
                 method.
             name (str):
                 Required. Resource name of the requested data policy.
                 Format is
                 ``projects/{project_number}/locations/{location_id}/dataPolicies/{data_policy_id}``.
 
@@ -841,15 +841,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.datapolicies_v1beta1.types.DataPolicy:
+            google.cloud.bigquery_datapolicies_v1beta1.types.DataPolicy:
                 Represents the label-policy binding.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
@@ -907,34 +907,34 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import datapolicies_v1beta1
+            from google.cloud import bigquery_datapolicies_v1beta1
 
             def sample_list_data_policies():
                 # Create a client
-                client = datapolicies_v1beta1.DataPolicyServiceClient()
+                client = bigquery_datapolicies_v1beta1.DataPolicyServiceClient()
 
                 # Initialize request argument(s)
-                request = datapolicies_v1beta1.ListDataPoliciesRequest(
+                request = bigquery_datapolicies_v1beta1.ListDataPoliciesRequest(
                     parent="parent_value",
                 )
 
                 # Make the request
                 page_result = client.list_data_policies(request=request)
 
                 # Handle the response
                 for response in page_result:
                     print(response)
 
         Args:
-            request (Union[google.cloud.bigquery.datapolicies_v1beta1.types.ListDataPoliciesRequest, dict]):
+            request (Union[google.cloud.bigquery_datapolicies_v1beta1.types.ListDataPoliciesRequest, dict]):
                 The request object. Request message for the
                 ListDataPolicies method.
             parent (str):
                 Required. Resource name of the project for which to list
                 data policies. Format is
                 ``projects/{project_number}/locations/{location_id}``.
 
@@ -944,15 +944,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.datapolicies_v1beta1.services.data_policy_service.pagers.ListDataPoliciesPager:
+            google.cloud.bigquery_datapolicies_v1beta1.services.data_policy_service.pagers.ListDataPoliciesPager:
                 Response message for the
                 ListDataPolicies method.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
@@ -1022,20 +1022,20 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import datapolicies_v1beta1
+            from google.cloud import bigquery_datapolicies_v1beta1
             from google.iam.v1 import iam_policy_pb2  # type: ignore
 
             def sample_get_iam_policy():
                 # Create a client
-                client = datapolicies_v1beta1.DataPolicyServiceClient()
+                client = bigquery_datapolicies_v1beta1.DataPolicyServiceClient()
 
                 # Initialize request argument(s)
                 request = iam_policy_pb2.GetIamPolicyRequest(
                     resource="resource_value",
                 )
 
                 # Make the request
@@ -1163,20 +1163,20 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import datapolicies_v1beta1
+            from google.cloud import bigquery_datapolicies_v1beta1
             from google.iam.v1 import iam_policy_pb2  # type: ignore
 
             def sample_set_iam_policy():
                 # Create a client
-                client = datapolicies_v1beta1.DataPolicyServiceClient()
+                client = bigquery_datapolicies_v1beta1.DataPolicyServiceClient()
 
                 # Initialize request argument(s)
                 request = iam_policy_pb2.SetIamPolicyRequest(
                     resource="resource_value",
                 )
 
                 # Make the request
@@ -1305,20 +1305,20 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import datapolicies_v1beta1
+            from google.cloud import bigquery_datapolicies_v1beta1
             from google.iam.v1 import iam_policy_pb2  # type: ignore
 
             def sample_test_iam_permissions():
                 # Create a client
-                client = datapolicies_v1beta1.DataPolicyServiceClient()
+                client = bigquery_datapolicies_v1beta1.DataPolicyServiceClient()
 
                 # Initialize request argument(s)
                 request = iam_policy_pb2.TestIamPermissionsRequest(
                     resource="resource_value",
                     permissions=['permissions_value1', 'permissions_value2'],
                 )
```

### Comparing `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/pagers.py` & `google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/pagers.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,31 +20,31 @@
     Callable,
     Iterator,
     Optional,
     Sequence,
     Tuple,
 )
 
-from google.cloud.bigquery.datapolicies_v1beta1.types import datapolicy
+from google.cloud.bigquery_datapolicies_v1beta1.types import datapolicy
 
 
 class ListDataPoliciesPager:
     """A pager for iterating through ``list_data_policies`` requests.
 
     This class thinly wraps an initial
-    :class:`google.cloud.bigquery.datapolicies_v1beta1.types.ListDataPoliciesResponse` object, and
+    :class:`google.cloud.bigquery_datapolicies_v1beta1.types.ListDataPoliciesResponse` object, and
     provides an ``__iter__`` method to iterate through its
     ``data_policies`` field.
 
     If there are more pages, the ``__iter__`` method will make additional
     ``ListDataPolicies`` requests and continue to iterate
     through the ``data_policies`` field on the
     corresponding responses.
 
-    All the usual :class:`google.cloud.bigquery.datapolicies_v1beta1.types.ListDataPoliciesResponse`
+    All the usual :class:`google.cloud.bigquery_datapolicies_v1beta1.types.ListDataPoliciesResponse`
     attributes are available on the pager. If multiple requests are made, only
     the most recent response is retained, and thus used for attribute lookup.
     """
 
     def __init__(
         self,
         method: Callable[..., datapolicy.ListDataPoliciesResponse],
@@ -54,17 +54,17 @@
         metadata: Sequence[Tuple[str, str]] = ()
     ):
         """Instantiate the pager.
 
         Args:
             method (Callable): The method that was originally called, and
                 which instantiated this pager.
-            request (google.cloud.bigquery.datapolicies_v1beta1.types.ListDataPoliciesRequest):
+            request (google.cloud.bigquery_datapolicies_v1beta1.types.ListDataPoliciesRequest):
                 The initial request object.
-            response (google.cloud.bigquery.datapolicies_v1beta1.types.ListDataPoliciesResponse):
+            response (google.cloud.bigquery_datapolicies_v1beta1.types.ListDataPoliciesResponse):
                 The initial response object.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         self._method = method
         self._request = datapolicy.ListDataPoliciesRequest(request)
         self._response = response
@@ -89,24 +89,24 @@
         return "{0}<{1!r}>".format(self.__class__.__name__, self._response)
 
 
 class ListDataPoliciesAsyncPager:
     """A pager for iterating through ``list_data_policies`` requests.
 
     This class thinly wraps an initial
-    :class:`google.cloud.bigquery.datapolicies_v1beta1.types.ListDataPoliciesResponse` object, and
+    :class:`google.cloud.bigquery_datapolicies_v1beta1.types.ListDataPoliciesResponse` object, and
     provides an ``__aiter__`` method to iterate through its
     ``data_policies`` field.
 
     If there are more pages, the ``__aiter__`` method will make additional
     ``ListDataPolicies`` requests and continue to iterate
     through the ``data_policies`` field on the
     corresponding responses.
 
-    All the usual :class:`google.cloud.bigquery.datapolicies_v1beta1.types.ListDataPoliciesResponse`
+    All the usual :class:`google.cloud.bigquery_datapolicies_v1beta1.types.ListDataPoliciesResponse`
     attributes are available on the pager. If multiple requests are made, only
     the most recent response is retained, and thus used for attribute lookup.
     """
 
     def __init__(
         self,
         method: Callable[..., Awaitable[datapolicy.ListDataPoliciesResponse]],
@@ -116,17 +116,17 @@
         metadata: Sequence[Tuple[str, str]] = ()
     ):
         """Instantiates the pager.
 
         Args:
             method (Callable): The method that was originally called, and
                 which instantiated this pager.
-            request (google.cloud.bigquery.datapolicies_v1beta1.types.ListDataPoliciesRequest):
+            request (google.cloud.bigquery_datapolicies_v1beta1.types.ListDataPoliciesRequest):
                 The initial request object.
-            response (google.cloud.bigquery.datapolicies_v1beta1.types.ListDataPoliciesResponse):
+            response (google.cloud.bigquery_datapolicies_v1beta1.types.ListDataPoliciesResponse):
                 The initial response object.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         self._method = method
         self._request = datapolicy.ListDataPoliciesRequest(request)
         self._response = response
```

### Comparing `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/transports/__init__.py` & `google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/transports/base.py` & `google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/transports/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.iam.v1 import iam_policy_pb2  # type: ignore
 from google.iam.v1 import policy_pb2  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 from google.protobuf import empty_pb2  # type: ignore
 
-from google.cloud.bigquery.datapolicies_v1beta1 import gapic_version as package_version
-from google.cloud.bigquery.datapolicies_v1beta1.types import datapolicy
+from google.cloud.bigquery_datapolicies_v1beta1 import gapic_version as package_version
+from google.cloud.bigquery_datapolicies_v1beta1.types import datapolicy
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
     gapic_version=package_version.__version__
 )
 
 
 class DataPolicyServiceTransport(abc.ABC):
```

### Comparing `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/transports/grpc.py` & `google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/transports/grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.iam.v1 import iam_policy_pb2  # type: ignore
 from google.iam.v1 import policy_pb2  # type: ignore
 from google.protobuf import empty_pb2  # type: ignore
 import grpc  # type: ignore
 
-from google.cloud.bigquery.datapolicies_v1beta1.types import datapolicy
+from google.cloud.bigquery_datapolicies_v1beta1.types import datapolicy
 
 from .base import DEFAULT_CLIENT_INFO, DataPolicyServiceTransport
 
 
 class DataPolicyServiceGrpcTransport(DataPolicyServiceTransport):
     """gRPC backend transport for DataPolicyService.
```

### Comparing `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/transports/grpc_asyncio.py` & `google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/transports/grpc_asyncio.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.iam.v1 import iam_policy_pb2  # type: ignore
 from google.iam.v1 import policy_pb2  # type: ignore
 from google.protobuf import empty_pb2  # type: ignore
 import grpc  # type: ignore
 from grpc.experimental import aio  # type: ignore
 
-from google.cloud.bigquery.datapolicies_v1beta1.types import datapolicy
+from google.cloud.bigquery_datapolicies_v1beta1.types import datapolicy
 
 from .base import DEFAULT_CLIENT_INFO, DataPolicyServiceTransport
 from .grpc import DataPolicyServiceGrpcTransport
 
 
 class DataPolicyServiceGrpcAsyncIOTransport(DataPolicyServiceTransport):
     """gRPC AsyncIO backend transport for DataPolicyService.
```

### Comparing `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/types/__init__.py` & `google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/types/datapolicy.py` & `google-cloud-bigquery-datapolicies-0.5.0/google/cloud/bigquery_datapolicies_v1beta1/types/datapolicy.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     r"""Request message for the CreateDataPolicy method.
 
     Attributes:
         parent (str):
             Required. Resource name of the project that the data policy
             will belong to. The format is
             ``projects/{project_number}/locations/{location_id}``.
-        data_policy (google.cloud.bigquery.datapolicies_v1beta1.types.DataPolicy):
+        data_policy (google.cloud.bigquery_datapolicies_v1beta1.types.DataPolicy):
             Required. The data policy to create. The ``name`` field does
             not need to be provided for the data policy creation.
     """
 
     parent: str = proto.Field(
         proto.STRING,
         number=1,
@@ -59,15 +59,15 @@
     )
 
 
 class UpdateDataPolicyRequest(proto.Message):
     r"""Response message for the UpdateDataPolicy method.
 
     Attributes:
-        data_policy (google.cloud.bigquery.datapolicies_v1beta1.types.DataPolicy):
+        data_policy (google.cloud.bigquery_datapolicies_v1beta1.types.DataPolicy):
             Required. Update the data policy's metadata.
 
             The target data policy is determined by the ``name`` field.
             Other fields are updated to the specified values based on
             the field masks.
         update_mask (google.protobuf.field_mask_pb2.FieldMask):
             The update mask applies to the resource. For the
@@ -155,15 +155,15 @@
     )
 
 
 class ListDataPoliciesResponse(proto.Message):
     r"""Response message for the ListDataPolicies method.
 
     Attributes:
-        data_policies (MutableSequence[google.cloud.bigquery.datapolicies_v1beta1.types.DataPolicy]):
+        data_policies (MutableSequence[google.cloud.bigquery_datapolicies_v1beta1.types.DataPolicy]):
             Data policies that belong to the requested
             project.
         next_page_token (str):
             Token used to retrieve the next page of
             results, or empty if there are no more results.
     """
 
@@ -189,24 +189,24 @@
 
     Attributes:
         policy_tag (str):
             Policy tag resource name, in the format of
             ``projects/{project_number}/locations/{location_id}/taxonomies/{taxonomy_id}/policyTags/{policyTag_id}``.
 
             This field is a member of `oneof`_ ``matching_label``.
-        data_masking_policy (google.cloud.bigquery.datapolicies_v1beta1.types.DataMaskingPolicy):
+        data_masking_policy (google.cloud.bigquery_datapolicies_v1beta1.types.DataMaskingPolicy):
             The data masking policy that specifies the
             data masking rule to use.
 
             This field is a member of `oneof`_ ``policy``.
         name (str):
             Output only. Resource name of this data policy, in the
             format of
             ``projects/{project_number}/locations/{location_id}/dataPolicies/{data_policy_id}``.
-        data_policy_type (google.cloud.bigquery.datapolicies_v1beta1.types.DataPolicy.DataPolicyType):
+        data_policy_type (google.cloud.bigquery_datapolicies_v1beta1.types.DataPolicy.DataPolicyType):
             Type of data policy.
         data_policy_id (str):
             User-assigned (human readable) ID of the data policy that
             needs to be unique within a project. Used as
             {data_policy_id} in part of the resource name.
     """
 
@@ -258,15 +258,15 @@
     r"""The data masking policy that is used to specify data masking
     rule.
 
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
     Attributes:
-        predefined_expression (google.cloud.bigquery.datapolicies_v1beta1.types.DataMaskingPolicy.PredefinedExpression):
+        predefined_expression (google.cloud.bigquery_datapolicies_v1beta1.types.DataMaskingPolicy.PredefinedExpression):
             A predefined masking expression.
 
             This field is a member of `oneof`_ ``masking_expression``.
     """
 
     class PredefinedExpression(proto.Enum):
         r"""The available masking rules. Learn more here:
```

### Comparing `google-cloud-bigquery-datapolicies-0.4.0/google_cloud_bigquery_datapolicies.egg-info/PKG-INFO` & `google-cloud-bigquery-datapolicies-0.5.0/google_cloud_bigquery_datapolicies.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-bigquery-datapolicies
-Version: 0.4.0
+Version: 0.5.0
 Summary: Google Cloud Bigquery Datapolicies API client library
-Home-page: https://github.com/googleapis/python-bigquery-datapolicies
+Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -18,47 +18,47 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Requires-Python: >=3.7
 License-File: LICENSE
 
-Python Client for BigQuery Data Policy API
-==========================================
+Python Client for BigQuery Data Policy
+======================================
 
 |preview| |pypi| |versions|
 
-`BigQuery Data Policy API`_: Allows users to manage BigQuery data policies.
+`BigQuery Data Policy`_: Allows users to manage BigQuery data policies.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-bigquery-datapolicies.svg
    :target: https://pypi.org/project/google-cloud-bigquery-datapolicies/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-bigquery-datapolicies.svg
    :target: https://pypi.org/project/google-cloud-bigquery-datapolicies/
-.. _BigQuery Data Policy API: https://cloud.google.com/bigquery/docs/reference/bigquerydatapolicy/rest
+.. _BigQuery Data Policy: https://cloud.google.com/bigquery/docs/reference/bigquerydatapolicy/rest
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/bigquerydatapolicy/latest
 .. _Product Documentation:  https://cloud.google.com/bigquery/docs/reference/bigquerydatapolicy/rest
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the BigQuery Data Policy API.`_
+3. `Enable the BigQuery Data Policy.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the BigQuery Data Policy API.:  https://cloud.google.com/bigquery/docs/reference/bigquerydatapolicy/rest
+.. _Enable the BigQuery Data Policy.:  https://cloud.google.com/bigquery/docs/reference/bigquerydatapolicy/rest
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-bigquery-datapolicies
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for BigQuery Data Policy API
+-  Read the `Client Library Documentation`_ for BigQuery Data Policy
    to see other available methods on the client.
--  Read the `BigQuery Data Policy API Product documentation`_ to learn
+-  Read the `BigQuery Data Policy Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _BigQuery Data Policy API Product documentation:  https://cloud.google.com/bigquery/docs/reference/bigquerydatapolicy/rest
+.. _BigQuery Data Policy Product documentation:  https://cloud.google.com/bigquery/docs/reference/bigquerydatapolicy/rest
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-bigquery-datapolicies-0.4.0/google_cloud_bigquery_datapolicies.egg-info/SOURCES.txt` & `google-cloud-bigquery-datapolicies-0.5.0/google_cloud_bigquery_datapolicies.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 LICENSE
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
-google/cloud/bigquery/datapolicies/__init__.py
-google/cloud/bigquery/datapolicies/gapic_version.py
-google/cloud/bigquery/datapolicies/py.typed
-google/cloud/bigquery/datapolicies_v1/__init__.py
-google/cloud/bigquery/datapolicies_v1/gapic_metadata.json
-google/cloud/bigquery/datapolicies_v1/gapic_version.py
-google/cloud/bigquery/datapolicies_v1/py.typed
-google/cloud/bigquery/datapolicies_v1/services/__init__.py
-google/cloud/bigquery/datapolicies_v1/services/data_policy_service/__init__.py
-google/cloud/bigquery/datapolicies_v1/services/data_policy_service/async_client.py
-google/cloud/bigquery/datapolicies_v1/services/data_policy_service/client.py
-google/cloud/bigquery/datapolicies_v1/services/data_policy_service/pagers.py
-google/cloud/bigquery/datapolicies_v1/services/data_policy_service/transports/__init__.py
-google/cloud/bigquery/datapolicies_v1/services/data_policy_service/transports/base.py
-google/cloud/bigquery/datapolicies_v1/services/data_policy_service/transports/grpc.py
-google/cloud/bigquery/datapolicies_v1/services/data_policy_service/transports/grpc_asyncio.py
-google/cloud/bigquery/datapolicies_v1/services/data_policy_service/transports/rest.py
-google/cloud/bigquery/datapolicies_v1/types/__init__.py
-google/cloud/bigquery/datapolicies_v1/types/datapolicy.py
-google/cloud/bigquery/datapolicies_v1beta1/__init__.py
-google/cloud/bigquery/datapolicies_v1beta1/gapic_metadata.json
-google/cloud/bigquery/datapolicies_v1beta1/gapic_version.py
-google/cloud/bigquery/datapolicies_v1beta1/py.typed
-google/cloud/bigquery/datapolicies_v1beta1/services/__init__.py
-google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/__init__.py
-google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/async_client.py
-google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/client.py
-google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/pagers.py
-google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/transports/__init__.py
-google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/transports/base.py
-google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/transports/grpc.py
-google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/transports/grpc_asyncio.py
-google/cloud/bigquery/datapolicies_v1beta1/types/__init__.py
-google/cloud/bigquery/datapolicies_v1beta1/types/datapolicy.py
+google/cloud/bigquery_datapolicies/__init__.py
+google/cloud/bigquery_datapolicies/gapic_version.py
+google/cloud/bigquery_datapolicies/py.typed
+google/cloud/bigquery_datapolicies_v1/__init__.py
+google/cloud/bigquery_datapolicies_v1/gapic_metadata.json
+google/cloud/bigquery_datapolicies_v1/gapic_version.py
+google/cloud/bigquery_datapolicies_v1/py.typed
+google/cloud/bigquery_datapolicies_v1/services/__init__.py
+google/cloud/bigquery_datapolicies_v1/services/data_policy_service/__init__.py
+google/cloud/bigquery_datapolicies_v1/services/data_policy_service/async_client.py
+google/cloud/bigquery_datapolicies_v1/services/data_policy_service/client.py
+google/cloud/bigquery_datapolicies_v1/services/data_policy_service/pagers.py
+google/cloud/bigquery_datapolicies_v1/services/data_policy_service/transports/__init__.py
+google/cloud/bigquery_datapolicies_v1/services/data_policy_service/transports/base.py
+google/cloud/bigquery_datapolicies_v1/services/data_policy_service/transports/grpc.py
+google/cloud/bigquery_datapolicies_v1/services/data_policy_service/transports/grpc_asyncio.py
+google/cloud/bigquery_datapolicies_v1/services/data_policy_service/transports/rest.py
+google/cloud/bigquery_datapolicies_v1/types/__init__.py
+google/cloud/bigquery_datapolicies_v1/types/datapolicy.py
+google/cloud/bigquery_datapolicies_v1beta1/__init__.py
+google/cloud/bigquery_datapolicies_v1beta1/gapic_metadata.json
+google/cloud/bigquery_datapolicies_v1beta1/gapic_version.py
+google/cloud/bigquery_datapolicies_v1beta1/py.typed
+google/cloud/bigquery_datapolicies_v1beta1/services/__init__.py
+google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/__init__.py
+google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/async_client.py
+google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/client.py
+google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/pagers.py
+google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/transports/__init__.py
+google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/transports/base.py
+google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/transports/grpc.py
+google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/transports/grpc_asyncio.py
+google/cloud/bigquery_datapolicies_v1beta1/types/__init__.py
+google/cloud/bigquery_datapolicies_v1beta1/types/datapolicy.py
 google_cloud_bigquery_datapolicies.egg-info/PKG-INFO
 google_cloud_bigquery_datapolicies.egg-info/SOURCES.txt
 google_cloud_bigquery_datapolicies.egg-info/dependency_links.txt
 google_cloud_bigquery_datapolicies.egg-info/namespace_packages.txt
 google_cloud_bigquery_datapolicies.egg-info/not-zip-safe
 google_cloud_bigquery_datapolicies.egg-info/requires.txt
 google_cloud_bigquery_datapolicies.egg-info/top_level.txt
 tests/__init__.py
 tests/unit/__init__.py
 tests/unit/gapic/__init__.py
-tests/unit/gapic/datapolicies_v1/__init__.py
-tests/unit/gapic/datapolicies_v1/test_data_policy_service.py
-tests/unit/gapic/datapolicies_v1beta1/__init__.py
-tests/unit/gapic/datapolicies_v1beta1/test_data_policy_service.py
+tests/unit/gapic/bigquery_datapolicies_v1/__init__.py
+tests/unit/gapic/bigquery_datapolicies_v1/test_data_policy_service.py
+tests/unit/gapic/bigquery_datapolicies_v1beta1/__init__.py
+tests/unit/gapic/bigquery_datapolicies_v1beta1/test_data_policy_service.py
```

### Comparing `google-cloud-bigquery-datapolicies-0.4.0/setup.py` & `google-cloud-bigquery-datapolicies-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 name = "google-cloud-bigquery-datapolicies"
 
 
 description = "Google Cloud Bigquery Datapolicies API client library"
 
 version = {}
 with open(
-    os.path.join(package_root, "google/cloud/bigquery/datapolicies/gapic_version.py")
+    os.path.join(package_root, "google/cloud/bigquery_datapolicies/gapic_version.py")
 ) as fp:
     exec(fp.read(), version)
 version = version["__version__"]
 
 if version[0] == "0":
     release_status = "Development Status :: 4 - Beta"
 else:
@@ -40,29 +40,29 @@
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
     "grpc-google-iam-v1 >= 0.12.4, <1.0.0dev",
 ]
-url = "https://github.com/googleapis/python-bigquery-datapolicies"
+url = "https://github.com/googleapis/google-cloud-python"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
 
 packages = [
     package
     for package in setuptools.PEP420PackageFinder.find()
     if package.startswith("google")
 ]
 
-namespaces = ["google", "google.cloud", "google.cloud.bigquery"]
+namespaces = ["google", "google.cloud"]
 
 setuptools.setup(
     name=name,
     version=version,
     description=description,
     long_description=readme,
     author="Google LLC",
```

### Comparing `google-cloud-bigquery-datapolicies-0.4.0/tests/__init__.py` & `google-cloud-bigquery-datapolicies-0.5.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.4.0/tests/unit/__init__.py` & `google-cloud-bigquery-datapolicies-0.5.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.4.0/tests/unit/gapic/__init__.py` & `google-cloud-bigquery-datapolicies-0.5.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.4.0/tests/unit/gapic/datapolicies_v1/__init__.py` & `google-cloud-bigquery-datapolicies-0.5.0/tests/unit/gapic/bigquery_datapolicies_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.4.0/tests/unit/gapic/datapolicies_v1/test_data_policy_service.py` & `google-cloud-bigquery-datapolicies-0.5.0/tests/unit/gapic/bigquery_datapolicies_v1/test_data_policy_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,21 +43,21 @@
 from grpc.experimental import aio
 from proto.marshal.rules import wrappers
 from proto.marshal.rules.dates import DurationRule, TimestampRule
 import pytest
 from requests import PreparedRequest, Request, Response
 from requests.sessions import Session
 
-from google.cloud.bigquery.datapolicies_v1.services.data_policy_service import (
+from google.cloud.bigquery_datapolicies_v1.services.data_policy_service import (
     DataPolicyServiceAsyncClient,
     DataPolicyServiceClient,
     pagers,
     transports,
 )
-from google.cloud.bigquery.datapolicies_v1.types import datapolicy
+from google.cloud.bigquery_datapolicies_v1.types import datapolicy
 
 
 def client_cert_source_callback():
     return b"cert bytes", b"key bytes"
 
 
 # If default endpoint is localhost, then default mtls endpoint will be the same.
@@ -647,15 +647,15 @@
             always_use_jwt_access=True,
             api_audience=None,
         )
 
 
 def test_data_policy_service_client_client_options_from_dict():
     with mock.patch(
-        "google.cloud.bigquery.datapolicies_v1.services.data_policy_service.transports.DataPolicyServiceGrpcTransport.__init__"
+        "google.cloud.bigquery_datapolicies_v1.services.data_policy_service.transports.DataPolicyServiceGrpcTransport.__init__"
     ) as grpc_transport:
         grpc_transport.return_value = None
         client = DataPolicyServiceClient(
             client_options={"api_endpoint": "squid.clam.whelk"}
         )
         grpc_transport.assert_called_once_with(
             credentials=None,
@@ -5580,15 +5580,15 @@
             credentials_file="credentials.json",
         )
 
 
 def test_data_policy_service_base_transport():
     # Instantiate the base transport.
     with mock.patch(
-        "google.cloud.bigquery.datapolicies_v1.services.data_policy_service.transports.DataPolicyServiceTransport.__init__"
+        "google.cloud.bigquery_datapolicies_v1.services.data_policy_service.transports.DataPolicyServiceTransport.__init__"
     ) as Transport:
         Transport.return_value = None
         transport = transports.DataPolicyServiceTransport(
             credentials=ga_credentials.AnonymousCredentials(),
         )
 
     # Every method on the transport should just blindly
@@ -5621,15 +5621,15 @@
 
 
 def test_data_policy_service_base_transport_with_credentials_file():
     # Instantiate the base transport with a credentials file
     with mock.patch.object(
         google.auth, "load_credentials_from_file", autospec=True
     ) as load_creds, mock.patch(
-        "google.cloud.bigquery.datapolicies_v1.services.data_policy_service.transports.DataPolicyServiceTransport._prep_wrapped_messages"
+        "google.cloud.bigquery_datapolicies_v1.services.data_policy_service.transports.DataPolicyServiceTransport._prep_wrapped_messages"
     ) as Transport:
         Transport.return_value = None
         load_creds.return_value = (ga_credentials.AnonymousCredentials(), None)
         transport = transports.DataPolicyServiceTransport(
             credentials_file="credentials.json",
             quota_project_id="octopus",
         )
@@ -5643,15 +5643,15 @@
             quota_project_id="octopus",
         )
 
 
 def test_data_policy_service_base_transport_with_adc():
     # Test the default credentials are used if credentials and credentials_file are None.
     with mock.patch.object(google.auth, "default", autospec=True) as adc, mock.patch(
-        "google.cloud.bigquery.datapolicies_v1.services.data_policy_service.transports.DataPolicyServiceTransport._prep_wrapped_messages"
+        "google.cloud.bigquery_datapolicies_v1.services.data_policy_service.transports.DataPolicyServiceTransport._prep_wrapped_messages"
     ) as Transport:
         Transport.return_value = None
         adc.return_value = (ga_credentials.AnonymousCredentials(), None)
         transport = transports.DataPolicyServiceTransport()
         adc.assert_called_once()
```

### Comparing `google-cloud-bigquery-datapolicies-0.4.0/tests/unit/gapic/datapolicies_v1beta1/__init__.py` & `google-cloud-bigquery-datapolicies-0.5.0/tests/unit/gapic/bigquery_datapolicies_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.4.0/tests/unit/gapic/datapolicies_v1beta1/test_data_policy_service.py` & `google-cloud-bigquery-datapolicies-0.5.0/tests/unit/gapic/bigquery_datapolicies_v1beta1/test_data_policy_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,21 +38,21 @@
 from google.type import expr_pb2  # type: ignore
 import grpc
 from grpc.experimental import aio
 from proto.marshal.rules import wrappers
 from proto.marshal.rules.dates import DurationRule, TimestampRule
 import pytest
 
-from google.cloud.bigquery.datapolicies_v1beta1.services.data_policy_service import (
+from google.cloud.bigquery_datapolicies_v1beta1.services.data_policy_service import (
     DataPolicyServiceAsyncClient,
     DataPolicyServiceClient,
     pagers,
     transports,
 )
-from google.cloud.bigquery.datapolicies_v1beta1.types import datapolicy
+from google.cloud.bigquery_datapolicies_v1beta1.types import datapolicy
 
 
 def client_cert_source_callback():
     return b"cert bytes", b"key bytes"
 
 
 # If default endpoint is localhost, then default mtls endpoint will be the same.
@@ -610,15 +610,15 @@
             always_use_jwt_access=True,
             api_audience=None,
         )
 
 
 def test_data_policy_service_client_client_options_from_dict():
     with mock.patch(
-        "google.cloud.bigquery.datapolicies_v1beta1.services.data_policy_service.transports.DataPolicyServiceGrpcTransport.__init__"
+        "google.cloud.bigquery_datapolicies_v1beta1.services.data_policy_service.transports.DataPolicyServiceGrpcTransport.__init__"
     ) as grpc_transport:
         grpc_transport.return_value = None
         client = DataPolicyServiceClient(
             client_options={"api_endpoint": "squid.clam.whelk"}
         )
         grpc_transport.assert_called_once_with(
             credentials=None,
@@ -2819,15 +2819,15 @@
             credentials_file="credentials.json",
         )
 
 
 def test_data_policy_service_base_transport():
     # Instantiate the base transport.
     with mock.patch(
-        "google.cloud.bigquery.datapolicies_v1beta1.services.data_policy_service.transports.DataPolicyServiceTransport.__init__"
+        "google.cloud.bigquery_datapolicies_v1beta1.services.data_policy_service.transports.DataPolicyServiceTransport.__init__"
     ) as Transport:
         Transport.return_value = None
         transport = transports.DataPolicyServiceTransport(
             credentials=ga_credentials.AnonymousCredentials(),
         )
 
     # Every method on the transport should just blindly
@@ -2859,15 +2859,15 @@
 
 
 def test_data_policy_service_base_transport_with_credentials_file():
     # Instantiate the base transport with a credentials file
     with mock.patch.object(
         google.auth, "load_credentials_from_file", autospec=True
     ) as load_creds, mock.patch(
-        "google.cloud.bigquery.datapolicies_v1beta1.services.data_policy_service.transports.DataPolicyServiceTransport._prep_wrapped_messages"
+        "google.cloud.bigquery_datapolicies_v1beta1.services.data_policy_service.transports.DataPolicyServiceTransport._prep_wrapped_messages"
     ) as Transport:
         Transport.return_value = None
         load_creds.return_value = (ga_credentials.AnonymousCredentials(), None)
         transport = transports.DataPolicyServiceTransport(
             credentials_file="credentials.json",
             quota_project_id="octopus",
         )
@@ -2881,15 +2881,15 @@
             quota_project_id="octopus",
         )
 
 
 def test_data_policy_service_base_transport_with_adc():
     # Test the default credentials are used if credentials and credentials_file are None.
     with mock.patch.object(google.auth, "default", autospec=True) as adc, mock.patch(
-        "google.cloud.bigquery.datapolicies_v1beta1.services.data_policy_service.transports.DataPolicyServiceTransport._prep_wrapped_messages"
+        "google.cloud.bigquery_datapolicies_v1beta1.services.data_policy_service.transports.DataPolicyServiceTransport._prep_wrapped_messages"
     ) as Transport:
         Transport.return_value = None
         adc.return_value = (ga_credentials.AnonymousCredentials(), None)
         transport = transports.DataPolicyServiceTransport()
         adc.assert_called_once()
```

