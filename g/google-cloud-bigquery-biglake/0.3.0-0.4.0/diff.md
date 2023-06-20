# Comparing `tmp/google-cloud-bigquery-biglake-0.3.0.tar.gz` & `tmp/google-cloud-bigquery-biglake-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-bigquery-biglake-0.3.0.tar", last modified: Wed Apr 12 14:13:15 2023, max compression
+gzip compressed data, was "google-cloud-bigquery-biglake-0.4.0.tar", last modified: Tue Jun 20 13:27:00 2023, max compression
```

## Comparing `google-cloud-bigquery-biglake-0.3.0.tar` & `google-cloud-bigquery-biglake-0.4.0.tar`

### file list

```diff
@@ -1,76 +1,75 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:15.330016 google-cloud-bigquery-biglake-0.3.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4685 2023-04-12 14:13:15.330016 google-cloud-bigquery-biglake-0.3.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3759 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:15.318014 google-cloud-bigquery-biglake-0.3.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:15.318014 google-cloud-bigquery-biglake-0.3.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:15.318014 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:15.322015 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake/
--rw-rw-r--   0 root         (0)     1003     2242 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake/__init__.py
--rw-rw-r--   0 root         (0)     1003      653 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       90 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:15.322015 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/
--rw-rw-r--   0 root         (0)     1003     2085 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     6058 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      653 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       90 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:15.322015 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:15.322015 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/services/metastore_service/
--rw-rw-r--   0 root         (0)     1003      777 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/services/metastore_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    77802 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/services/metastore_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    90452 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/services/metastore_service/client.py
--rw-rw-r--   0 root         (0)     1003    15709 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/services/metastore_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:15.322015 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/services/metastore_service/transports/
--rw-rw-r--   0 root         (0)     1003     1428 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/services/metastore_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    11893 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/services/metastore_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    27356 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/services/metastore_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    28003 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/services/metastore_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    82223 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/services/metastore_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:15.326015 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/types/
--rw-rw-r--   0 root         (0)     1003     1786 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    26313 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/types/metastore.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:15.326015 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/
--rw-rw-r--   0 root         (0)     1003     2349 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/__init__.py
--rw-rw-r--   0 root         (0)     1003     7450 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      653 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       90 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:15.326015 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:15.326015 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/
--rw-rw-r--   0 root         (0)     1003      777 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    95360 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/async_client.py
--rw-rw-r--   0 root         (0)     1003   109333 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/client.py
--rw-rw-r--   0 root         (0)     1003    20793 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:15.326015 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/transports/
--rw-rw-r--   0 root         (0)     1003     1428 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    13545 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    31716 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    32496 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   101231 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:15.326015 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/types/
--rw-rw-r--   0 root         (0)     1003     2044 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    32213 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/types/metastore.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:15.330016 google-cloud-bigquery-biglake-0.3.0/google_cloud_bigquery_biglake.egg-info/
--rw-r--r--   0 root         (0)     1003     4685 2023-04-12 14:13:15.000000 google-cloud-bigquery-biglake-0.3.0/google_cloud_bigquery_biglake.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2995 2023-04-12 14:13:15.000000 google-cloud-bigquery-biglake-0.3.0/google_cloud_bigquery_biglake.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-04-12 14:13:15.000000 google-cloud-bigquery-biglake-0.3.0/google_cloud_bigquery_biglake.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       42 2023-04-12 14:13:15.000000 google-cloud-bigquery-biglake-0.3.0/google_cloud_bigquery_biglake.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-04-12 14:13:15.000000 google-cloud-bigquery-biglake-0.3.0/google_cloud_bigquery_biglake.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-04-12 14:13:15.000000 google-cloud-bigquery-biglake-0.3.0/google_cloud_bigquery_biglake.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-04-12 14:13:15.000000 google-cloud-bigquery-biglake-0.3.0/google_cloud_bigquery_biglake.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2023-04-12 14:13:15.330016 google-cloud-bigquery-biglake-0.3.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2984 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:15.330016 google-cloud-bigquery-biglake-0.3.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:15.330016 google-cloud-bigquery-biglake-0.3.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:15.330016 google-cloud-bigquery-biglake-0.3.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:15.330016 google-cloud-bigquery-biglake-0.3.0/tests/unit/gapic/biglake_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/tests/unit/gapic/biglake_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   369886 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/tests/unit/gapic/biglake_v1/test_metastore_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:15.330016 google-cloud-bigquery-biglake-0.3.0/tests/unit/gapic/biglake_v1alpha1/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/tests/unit/gapic/biglake_v1alpha1/__init__.py
--rw-rw-r--   0 root         (0)     1003   451218 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/tests/unit/gapic/biglake_v1alpha1/test_metastore_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:00.489223 google-cloud-bigquery-biglake-0.4.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4685 2023-06-20 13:27:00.485222 google-cloud-bigquery-biglake-0.4.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3759 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:00.473221 google-cloud-bigquery-biglake-0.4.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:00.473221 google-cloud-bigquery-biglake-0.4.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:00.477221 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake/
+-rw-rw-r--   0 root         (0)     1003     2242 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       90 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:00.477221 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/
+-rw-rw-r--   0 root         (0)     1003     2085 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6058 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       90 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:00.477221 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:00.477221 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/services/metastore_service/
+-rw-rw-r--   0 root         (0)     1003      777 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/services/metastore_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    78072 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/services/metastore_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    90722 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/services/metastore_service/client.py
+-rw-rw-r--   0 root         (0)     1003    15709 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/services/metastore_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:00.477221 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/services/metastore_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1428 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/services/metastore_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11893 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/services/metastore_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    27356 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/services/metastore_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    28003 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/services/metastore_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    82223 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/services/metastore_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:00.481222 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1786 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    26313 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/types/metastore.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:00.481222 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/
+-rw-rw-r--   0 root         (0)     1003     2349 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7450 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       90 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:00.481222 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:00.481222 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/
+-rw-rw-r--   0 root         (0)     1003      777 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    95711 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003   109684 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/client.py
+-rw-rw-r--   0 root         (0)     1003    20793 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:00.481222 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1428 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    13545 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    31716 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    32496 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   101231 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:00.481222 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/types/
+-rw-rw-r--   0 root         (0)     1003     2044 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    32213 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/types/metastore.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:00.485222 google-cloud-bigquery-biglake-0.4.0/google_cloud_bigquery_biglake.egg-info/
+-rw-r--r--   0 root         (0)     1003     4685 2023-06-20 13:27:00.000000 google-cloud-bigquery-biglake-0.4.0/google_cloud_bigquery_biglake.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     3031 2023-06-20 13:27:00.000000 google-cloud-bigquery-biglake-0.4.0/google_cloud_bigquery_biglake.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-06-20 13:27:00.000000 google-cloud-bigquery-biglake-0.4.0/google_cloud_bigquery_biglake.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-06-20 13:27:00.000000 google-cloud-bigquery-biglake-0.4.0/google_cloud_bigquery_biglake.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-06-20 13:27:00.000000 google-cloud-bigquery-biglake-0.4.0/google_cloud_bigquery_biglake.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-06-20 13:27:00.000000 google-cloud-bigquery-biglake-0.4.0/google_cloud_bigquery_biglake.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-06-20 13:27:00.000000 google-cloud-bigquery-biglake-0.4.0/google_cloud_bigquery_biglake.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2023-06-20 13:27:00.489223 google-cloud-bigquery-biglake-0.4.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2959 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:00.485222 google-cloud-bigquery-biglake-0.4.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:00.485222 google-cloud-bigquery-biglake-0.4.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:00.485222 google-cloud-bigquery-biglake-0.4.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:00.485222 google-cloud-bigquery-biglake-0.4.0/tests/unit/gapic/bigquery_biglake_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/tests/unit/gapic/bigquery_biglake_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   369886 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/tests/unit/gapic/bigquery_biglake_v1/test_metastore_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:00.485222 google-cloud-bigquery-biglake-0.4.0/tests/unit/gapic/bigquery_biglake_v1alpha1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/tests/unit/gapic/bigquery_biglake_v1alpha1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   451218 2023-06-20 13:23:47.000000 google-cloud-bigquery-biglake-0.4.0/tests/unit/gapic/bigquery_biglake_v1alpha1/test_metastore_service.py
```

### Comparing `google-cloud-bigquery-biglake-0.3.0/LICENSE` & `google-cloud-bigquery-biglake-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.3.0/MANIFEST.in` & `google-cloud-bigquery-biglake-0.4.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.3.0/PKG-INFO` & `google-cloud-bigquery-biglake-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-bigquery-biglake
-Version: 0.3.0
+Version: 0.4.0
 Summary: Google Cloud Bigquery Biglake API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-bigquery-biglake-0.3.0/README.rst` & `google-cloud-bigquery-biglake-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake/__init__.py` & `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,26 +9,26 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from google.cloud.bigquery.biglake import gapic_version as package_version
+from google.cloud.bigquery_biglake import gapic_version as package_version
 
 __version__ = package_version.__version__
 
 
-from google.cloud.bigquery.biglake_v1.services.metastore_service.async_client import (
+from google.cloud.bigquery_biglake_v1.services.metastore_service.async_client import (
     MetastoreServiceAsyncClient,
 )
-from google.cloud.bigquery.biglake_v1.services.metastore_service.client import (
+from google.cloud.bigquery_biglake_v1.services.metastore_service.client import (
     MetastoreServiceClient,
 )
-from google.cloud.bigquery.biglake_v1.types.metastore import (
+from google.cloud.bigquery_biglake_v1.types.metastore import (
     Catalog,
     CreateCatalogRequest,
     CreateDatabaseRequest,
     CreateTableRequest,
     Database,
     DeleteCatalogRequest,
     DeleteDatabaseRequest,
```

### Comparing `google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake/gapic_version.py` & `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake/gapic_version.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-
-__version__ = "0.3.0"  # {x-release-please-version}
+__version__ = "0.4.0"  # {x-release-please-version}
```

### Comparing `google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/__init__.py` & `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from google.cloud.bigquery.biglake_v1 import gapic_version as package_version
+from google.cloud.bigquery_biglake_v1 import gapic_version as package_version
 
 __version__ = package_version.__version__
 
 
 from .services.metastore_service import (
     MetastoreServiceAsyncClient,
     MetastoreServiceClient,
```

### Comparing `google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/gapic_metadata.json` & `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/gapic_metadata.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'libraryPackage'": "'google.cloud.bigquery_biglake_v1'"}*

```diff
@@ -1,11 +1,11 @@
 {
     "comment": "This file maps proto services/RPCs to the corresponding library clients/methods",
     "language": "python",
-    "libraryPackage": "google.cloud.bigquery.biglake_v1",
+    "libraryPackage": "google.cloud.bigquery_biglake_v1",
     "protoPackage": "google.cloud.bigquery.biglake.v1",
     "schema": "1.0",
     "services": {
         "MetastoreService": {
             "clients": {
                 "grpc": {
                     "libraryClient": "MetastoreServiceClient",
```

### Comparing `google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/gapic_version.py` & `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/gapic_version.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-
-__version__ = "0.3.0"  # {x-release-please-version}
+__version__ = "0.4.0"  # {x-release-please-version}
```

### Comparing `google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/services/__init__.py` & `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/services/metastore_service/__init__.py` & `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/services/metastore_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/services/metastore_service/async_client.py` & `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/services/metastore_service/async_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,26 +31,26 @@
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.api_core.client_options import ClientOptions
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 
-from google.cloud.bigquery.biglake_v1 import gapic_version as package_version
+from google.cloud.bigquery_biglake_v1 import gapic_version as package_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.protobuf import field_mask_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 
-from google.cloud.bigquery.biglake_v1.services.metastore_service import pagers
-from google.cloud.bigquery.biglake_v1.types import metastore
+from google.cloud.bigquery_biglake_v1.services.metastore_service import pagers
+from google.cloud.bigquery_biglake_v1.types import metastore
 
 from .client import MetastoreServiceClient
 from .transports.base import DEFAULT_CLIENT_INFO, MetastoreServiceTransport
 from .transports.grpc_asyncio import MetastoreServiceGrpcAsyncIOTransport
 
 
 class MetastoreServiceAsyncClient:
@@ -250,45 +250,45 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1
+            from google.cloud import bigquery_biglake_v1
 
             async def sample_create_catalog():
                 # Create a client
-                client = biglake_v1.MetastoreServiceAsyncClient()
+                client = bigquery_biglake_v1.MetastoreServiceAsyncClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1.CreateCatalogRequest(
+                request = bigquery_biglake_v1.CreateCatalogRequest(
                     parent="parent_value",
                     catalog_id="catalog_id_value",
                 )
 
                 # Make the request
                 response = await client.create_catalog(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.biglake_v1.types.CreateCatalogRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_biglake_v1.types.CreateCatalogRequest, dict]]):
                 The request object. Request message for the CreateCatalog
                 method.
             parent (:class:`str`):
                 Required. The parent resource where this catalog will be
                 created. Format:
                 projects/{project_id_or_number}/locations/{location_id}
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            catalog (:class:`google.cloud.bigquery.biglake_v1.types.Catalog`):
+            catalog (:class:`google.cloud.bigquery_biglake_v1.types.Catalog`):
                 Required. The catalog to create. The ``name`` field does
                 not need to be provided.
 
                 This corresponds to the ``catalog`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             catalog_id (:class:`str`):
@@ -303,15 +303,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1.types.Catalog:
+            google.cloud.bigquery_biglake_v1.types.Catalog:
                 Catalog is the container of
                 databases.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
@@ -375,33 +375,33 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1
+            from google.cloud import bigquery_biglake_v1
 
             async def sample_delete_catalog():
                 # Create a client
-                client = biglake_v1.MetastoreServiceAsyncClient()
+                client = bigquery_biglake_v1.MetastoreServiceAsyncClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1.DeleteCatalogRequest(
+                request = bigquery_biglake_v1.DeleteCatalogRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 response = await client.delete_catalog(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.biglake_v1.types.DeleteCatalogRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_biglake_v1.types.DeleteCatalogRequest, dict]]):
                 The request object. Request message for the DeleteCatalog
                 method.
             name (:class:`str`):
                 Required. The name of the catalog to delete. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}
 
                 This corresponds to the ``name`` field
@@ -410,15 +410,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1.types.Catalog:
+            google.cloud.bigquery_biglake_v1.types.Catalog:
                 Catalog is the container of
                 databases.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
@@ -477,33 +477,33 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1
+            from google.cloud import bigquery_biglake_v1
 
             async def sample_get_catalog():
                 # Create a client
-                client = biglake_v1.MetastoreServiceAsyncClient()
+                client = bigquery_biglake_v1.MetastoreServiceAsyncClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1.GetCatalogRequest(
+                request = bigquery_biglake_v1.GetCatalogRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 response = await client.get_catalog(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.biglake_v1.types.GetCatalogRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_biglake_v1.types.GetCatalogRequest, dict]]):
                 The request object. Request message for the GetCatalog
                 method.
             name (:class:`str`):
                 Required. The name of the catalog to retrieve. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}
 
                 This corresponds to the ``name`` field
@@ -512,15 +512,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1.types.Catalog:
+            google.cloud.bigquery_biglake_v1.types.Catalog:
                 Catalog is the container of
                 databases.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
@@ -579,34 +579,34 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1
+            from google.cloud import bigquery_biglake_v1
 
             async def sample_list_catalogs():
                 # Create a client
-                client = biglake_v1.MetastoreServiceAsyncClient()
+                client = bigquery_biglake_v1.MetastoreServiceAsyncClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1.ListCatalogsRequest(
+                request = bigquery_biglake_v1.ListCatalogsRequest(
                     parent="parent_value",
                 )
 
                 # Make the request
                 page_result = client.list_catalogs(request=request)
 
                 # Handle the response
                 async for response in page_result:
                     print(response)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.biglake_v1.types.ListCatalogsRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_biglake_v1.types.ListCatalogsRequest, dict]]):
                 The request object. Request message for the ListCatalogs
                 method.
             parent (:class:`str`):
                 Required. The parent, which owns this collection of
                 catalogs. Format:
                 projects/{project_id_or_number}/locations/{location_id}
 
@@ -616,15 +616,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1.services.metastore_service.pagers.ListCatalogsAsyncPager:
+            google.cloud.bigquery_biglake_v1.services.metastore_service.pagers.ListCatalogsAsyncPager:
                 Response message for the ListCatalogs
                 method.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
@@ -697,45 +697,45 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1
+            from google.cloud import bigquery_biglake_v1
 
             async def sample_create_database():
                 # Create a client
-                client = biglake_v1.MetastoreServiceAsyncClient()
+                client = bigquery_biglake_v1.MetastoreServiceAsyncClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1.CreateDatabaseRequest(
+                request = bigquery_biglake_v1.CreateDatabaseRequest(
                     parent="parent_value",
                     database_id="database_id_value",
                 )
 
                 # Make the request
                 response = await client.create_database(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.biglake_v1.types.CreateDatabaseRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_biglake_v1.types.CreateDatabaseRequest, dict]]):
                 The request object. Request message for the
                 CreateDatabase method.
             parent (:class:`str`):
                 Required. The parent resource where this database will
                 be created. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            database (:class:`google.cloud.bigquery.biglake_v1.types.Database`):
+            database (:class:`google.cloud.bigquery_biglake_v1.types.Database`):
                 Required. The database to create. The ``name`` field
                 does not need to be provided.
 
                 This corresponds to the ``database`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             database_id (:class:`str`):
@@ -750,15 +750,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1.types.Database:
+            google.cloud.bigquery_biglake_v1.types.Database:
                 Database is the container of tables.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, database, database_id])
         if request is not None and has_flattened_params:
@@ -820,33 +820,33 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1
+            from google.cloud import bigquery_biglake_v1
 
             async def sample_delete_database():
                 # Create a client
-                client = biglake_v1.MetastoreServiceAsyncClient()
+                client = bigquery_biglake_v1.MetastoreServiceAsyncClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1.DeleteDatabaseRequest(
+                request = bigquery_biglake_v1.DeleteDatabaseRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 response = await client.delete_database(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.biglake_v1.types.DeleteDatabaseRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_biglake_v1.types.DeleteDatabaseRequest, dict]]):
                 The request object. Request message for the
                 DeleteDatabase method.
             name (:class:`str`):
                 Required. The name of the database to delete. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}
 
                 This corresponds to the ``name`` field
@@ -855,15 +855,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1.types.Database:
+            google.cloud.bigquery_biglake_v1.types.Database:
                 Database is the container of tables.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
@@ -922,35 +922,35 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1
+            from google.cloud import bigquery_biglake_v1
 
             async def sample_update_database():
                 # Create a client
-                client = biglake_v1.MetastoreServiceAsyncClient()
+                client = bigquery_biglake_v1.MetastoreServiceAsyncClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1.UpdateDatabaseRequest(
+                request = bigquery_biglake_v1.UpdateDatabaseRequest(
                 )
 
                 # Make the request
                 response = await client.update_database(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.biglake_v1.types.UpdateDatabaseRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_biglake_v1.types.UpdateDatabaseRequest, dict]]):
                 The request object. Request message for the
                 UpdateDatabase method.
-            database (:class:`google.cloud.bigquery.biglake_v1.types.Database`):
+            database (:class:`google.cloud.bigquery_biglake_v1.types.Database`):
                 Required. The database to update.
 
                 The database's ``name`` field is used to identify the
                 database to update. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}
 
                 This corresponds to the ``database`` field
@@ -970,15 +970,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1.types.Database:
+            google.cloud.bigquery_biglake_v1.types.Database:
                 Database is the container of tables.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([database, update_mask])
         if request is not None and has_flattened_params:
@@ -1039,33 +1039,33 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1
+            from google.cloud import bigquery_biglake_v1
 
             async def sample_get_database():
                 # Create a client
-                client = biglake_v1.MetastoreServiceAsyncClient()
+                client = bigquery_biglake_v1.MetastoreServiceAsyncClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1.GetDatabaseRequest(
+                request = bigquery_biglake_v1.GetDatabaseRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 response = await client.get_database(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.biglake_v1.types.GetDatabaseRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_biglake_v1.types.GetDatabaseRequest, dict]]):
                 The request object. Request message for the GetDatabase
                 method.
             name (:class:`str`):
                 Required. The name of the database to retrieve. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}
 
                 This corresponds to the ``name`` field
@@ -1074,15 +1074,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1.types.Database:
+            google.cloud.bigquery_biglake_v1.types.Database:
                 Database is the container of tables.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
@@ -1139,34 +1139,34 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1
+            from google.cloud import bigquery_biglake_v1
 
             async def sample_list_databases():
                 # Create a client
-                client = biglake_v1.MetastoreServiceAsyncClient()
+                client = bigquery_biglake_v1.MetastoreServiceAsyncClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1.ListDatabasesRequest(
+                request = bigquery_biglake_v1.ListDatabasesRequest(
                     parent="parent_value",
                 )
 
                 # Make the request
                 page_result = client.list_databases(request=request)
 
                 # Handle the response
                 async for response in page_result:
                     print(response)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.biglake_v1.types.ListDatabasesRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_biglake_v1.types.ListDatabasesRequest, dict]]):
                 The request object. Request message for the ListDatabases
                 method.
             parent (:class:`str`):
                 Required. The parent, which owns this collection of
                 databases. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}
 
@@ -1176,15 +1176,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1.services.metastore_service.pagers.ListDatabasesAsyncPager:
+            google.cloud.bigquery_biglake_v1.services.metastore_service.pagers.ListDatabasesAsyncPager:
                 Response message for the
                 ListDatabases method.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
@@ -1257,45 +1257,45 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1
+            from google.cloud import bigquery_biglake_v1
 
             async def sample_create_table():
                 # Create a client
-                client = biglake_v1.MetastoreServiceAsyncClient()
+                client = bigquery_biglake_v1.MetastoreServiceAsyncClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1.CreateTableRequest(
+                request = bigquery_biglake_v1.CreateTableRequest(
                     parent="parent_value",
                     table_id="table_id_value",
                 )
 
                 # Make the request
                 response = await client.create_table(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.biglake_v1.types.CreateTableRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_biglake_v1.types.CreateTableRequest, dict]]):
                 The request object. Request message for the CreateTable
                 method.
             parent (:class:`str`):
                 Required. The parent resource where this table will be
                 created. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            table (:class:`google.cloud.bigquery.biglake_v1.types.Table`):
+            table (:class:`google.cloud.bigquery_biglake_v1.types.Table`):
                 Required. The table to create. The ``name`` field does
                 not need to be provided for the table creation.
 
                 This corresponds to the ``table`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             table_id (:class:`str`):
@@ -1309,15 +1309,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1.types.Table:
+            google.cloud.bigquery_biglake_v1.types.Table:
                 Represents a table.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, table, table_id])
         if request is not None and has_flattened_params:
@@ -1378,33 +1378,33 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1
+            from google.cloud import bigquery_biglake_v1
 
             async def sample_delete_table():
                 # Create a client
-                client = biglake_v1.MetastoreServiceAsyncClient()
+                client = bigquery_biglake_v1.MetastoreServiceAsyncClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1.DeleteTableRequest(
+                request = bigquery_biglake_v1.DeleteTableRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 response = await client.delete_table(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.biglake_v1.types.DeleteTableRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_biglake_v1.types.DeleteTableRequest, dict]]):
                 The request object. Request message for the DeleteTable
                 method.
             name (:class:`str`):
                 Required. The name of the table to delete. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}/tables/{table_id}
 
                 This corresponds to the ``name`` field
@@ -1413,15 +1413,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1.types.Table:
+            google.cloud.bigquery_biglake_v1.types.Table:
                 Represents a table.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
@@ -1479,35 +1479,35 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1
+            from google.cloud import bigquery_biglake_v1
 
             async def sample_update_table():
                 # Create a client
-                client = biglake_v1.MetastoreServiceAsyncClient()
+                client = bigquery_biglake_v1.MetastoreServiceAsyncClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1.UpdateTableRequest(
+                request = bigquery_biglake_v1.UpdateTableRequest(
                 )
 
                 # Make the request
                 response = await client.update_table(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.biglake_v1.types.UpdateTableRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_biglake_v1.types.UpdateTableRequest, dict]]):
                 The request object. Request message for the UpdateTable
                 method.
-            table (:class:`google.cloud.bigquery.biglake_v1.types.Table`):
+            table (:class:`google.cloud.bigquery_biglake_v1.types.Table`):
                 Required. The table to update.
 
                 The table's ``name`` field is used to identify the table
                 to update. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}/tables/{table_id}
 
                 This corresponds to the ``table`` field
@@ -1527,15 +1527,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1.types.Table:
+            google.cloud.bigquery_biglake_v1.types.Table:
                 Represents a table.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([table, update_mask])
         if request is not None and has_flattened_params:
@@ -1597,34 +1597,34 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1
+            from google.cloud import bigquery_biglake_v1
 
             async def sample_rename_table():
                 # Create a client
-                client = biglake_v1.MetastoreServiceAsyncClient()
+                client = bigquery_biglake_v1.MetastoreServiceAsyncClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1.RenameTableRequest(
+                request = bigquery_biglake_v1.RenameTableRequest(
                     name="name_value",
                     new_name="new_name_value",
                 )
 
                 # Make the request
                 response = await client.rename_table(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.biglake_v1.types.RenameTableRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_biglake_v1.types.RenameTableRequest, dict]]):
                 The request object. Request message for the RenameTable
                 method in MetastoreService
             name (:class:`str`):
                 Required. The table's ``name`` field is used to identify
                 the table to rename. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}/tables/{table_id}
 
@@ -1642,15 +1642,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1.types.Table:
+            google.cloud.bigquery_biglake_v1.types.Table:
                 Represents a table.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name, new_name])
         if request is not None and has_flattened_params:
@@ -1709,33 +1709,33 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1
+            from google.cloud import bigquery_biglake_v1
 
             async def sample_get_table():
                 # Create a client
-                client = biglake_v1.MetastoreServiceAsyncClient()
+                client = bigquery_biglake_v1.MetastoreServiceAsyncClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1.GetTableRequest(
+                request = bigquery_biglake_v1.GetTableRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 response = await client.get_table(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.biglake_v1.types.GetTableRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_biglake_v1.types.GetTableRequest, dict]]):
                 The request object. Request message for the GetTable
                 method.
             name (:class:`str`):
                 Required. The name of the table to retrieve. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}/tables/{table_id}
 
                 This corresponds to the ``name`` field
@@ -1744,15 +1744,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1.types.Table:
+            google.cloud.bigquery_biglake_v1.types.Table:
                 Represents a table.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
@@ -1809,34 +1809,34 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1
+            from google.cloud import bigquery_biglake_v1
 
             async def sample_list_tables():
                 # Create a client
-                client = biglake_v1.MetastoreServiceAsyncClient()
+                client = bigquery_biglake_v1.MetastoreServiceAsyncClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1.ListTablesRequest(
+                request = bigquery_biglake_v1.ListTablesRequest(
                     parent="parent_value",
                 )
 
                 # Make the request
                 page_result = client.list_tables(request=request)
 
                 # Handle the response
                 async for response in page_result:
                     print(response)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.biglake_v1.types.ListTablesRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_biglake_v1.types.ListTablesRequest, dict]]):
                 The request object. Request message for the ListTables
                 method.
             parent (:class:`str`):
                 Required. The parent, which owns this collection of
                 tables. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}
 
@@ -1846,15 +1846,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1.services.metastore_service.pagers.ListTablesAsyncPager:
+            google.cloud.bigquery_biglake_v1.services.metastore_service.pagers.ListTablesAsyncPager:
                 Response message for the ListTables
                 method.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
```

### Comparing `google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/services/metastore_service/client.py` & `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/services/metastore_service/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,26 +35,26 @@
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.exceptions import MutualTLSChannelError  # type: ignore
 from google.auth.transport import mtls  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 
-from google.cloud.bigquery.biglake_v1 import gapic_version as package_version
+from google.cloud.bigquery_biglake_v1 import gapic_version as package_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.protobuf import field_mask_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 
-from google.cloud.bigquery.biglake_v1.services.metastore_service import pagers
-from google.cloud.bigquery.biglake_v1.types import metastore
+from google.cloud.bigquery_biglake_v1.services.metastore_service import pagers
+from google.cloud.bigquery_biglake_v1.types import metastore
 
 from .transports.base import DEFAULT_CLIENT_INFO, MetastoreServiceTransport
 from .transports.grpc import MetastoreServiceGrpcTransport
 from .transports.grpc_asyncio import MetastoreServiceGrpcAsyncIOTransport
 from .transports.rest import MetastoreServiceRestTransport
 
 
@@ -525,45 +525,45 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1
+            from google.cloud import bigquery_biglake_v1
 
             def sample_create_catalog():
                 # Create a client
-                client = biglake_v1.MetastoreServiceClient()
+                client = bigquery_biglake_v1.MetastoreServiceClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1.CreateCatalogRequest(
+                request = bigquery_biglake_v1.CreateCatalogRequest(
                     parent="parent_value",
                     catalog_id="catalog_id_value",
                 )
 
                 # Make the request
                 response = client.create_catalog(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.bigquery.biglake_v1.types.CreateCatalogRequest, dict]):
+            request (Union[google.cloud.bigquery_biglake_v1.types.CreateCatalogRequest, dict]):
                 The request object. Request message for the CreateCatalog
                 method.
             parent (str):
                 Required. The parent resource where this catalog will be
                 created. Format:
                 projects/{project_id_or_number}/locations/{location_id}
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            catalog (google.cloud.bigquery.biglake_v1.types.Catalog):
+            catalog (google.cloud.bigquery_biglake_v1.types.Catalog):
                 Required. The catalog to create. The ``name`` field does
                 not need to be provided.
 
                 This corresponds to the ``catalog`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             catalog_id (str):
@@ -578,15 +578,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1.types.Catalog:
+            google.cloud.bigquery_biglake_v1.types.Catalog:
                 Catalog is the container of
                 databases.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
@@ -650,33 +650,33 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1
+            from google.cloud import bigquery_biglake_v1
 
             def sample_delete_catalog():
                 # Create a client
-                client = biglake_v1.MetastoreServiceClient()
+                client = bigquery_biglake_v1.MetastoreServiceClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1.DeleteCatalogRequest(
+                request = bigquery_biglake_v1.DeleteCatalogRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 response = client.delete_catalog(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.bigquery.biglake_v1.types.DeleteCatalogRequest, dict]):
+            request (Union[google.cloud.bigquery_biglake_v1.types.DeleteCatalogRequest, dict]):
                 The request object. Request message for the DeleteCatalog
                 method.
             name (str):
                 Required. The name of the catalog to delete. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}
 
                 This corresponds to the ``name`` field
@@ -685,15 +685,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1.types.Catalog:
+            google.cloud.bigquery_biglake_v1.types.Catalog:
                 Catalog is the container of
                 databases.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
@@ -752,33 +752,33 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1
+            from google.cloud import bigquery_biglake_v1
 
             def sample_get_catalog():
                 # Create a client
-                client = biglake_v1.MetastoreServiceClient()
+                client = bigquery_biglake_v1.MetastoreServiceClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1.GetCatalogRequest(
+                request = bigquery_biglake_v1.GetCatalogRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 response = client.get_catalog(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.bigquery.biglake_v1.types.GetCatalogRequest, dict]):
+            request (Union[google.cloud.bigquery_biglake_v1.types.GetCatalogRequest, dict]):
                 The request object. Request message for the GetCatalog
                 method.
             name (str):
                 Required. The name of the catalog to retrieve. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}
 
                 This corresponds to the ``name`` field
@@ -787,15 +787,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1.types.Catalog:
+            google.cloud.bigquery_biglake_v1.types.Catalog:
                 Catalog is the container of
                 databases.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
@@ -854,34 +854,34 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1
+            from google.cloud import bigquery_biglake_v1
 
             def sample_list_catalogs():
                 # Create a client
-                client = biglake_v1.MetastoreServiceClient()
+                client = bigquery_biglake_v1.MetastoreServiceClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1.ListCatalogsRequest(
+                request = bigquery_biglake_v1.ListCatalogsRequest(
                     parent="parent_value",
                 )
 
                 # Make the request
                 page_result = client.list_catalogs(request=request)
 
                 # Handle the response
                 for response in page_result:
                     print(response)
 
         Args:
-            request (Union[google.cloud.bigquery.biglake_v1.types.ListCatalogsRequest, dict]):
+            request (Union[google.cloud.bigquery_biglake_v1.types.ListCatalogsRequest, dict]):
                 The request object. Request message for the ListCatalogs
                 method.
             parent (str):
                 Required. The parent, which owns this collection of
                 catalogs. Format:
                 projects/{project_id_or_number}/locations/{location_id}
 
@@ -891,15 +891,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1.services.metastore_service.pagers.ListCatalogsPager:
+            google.cloud.bigquery_biglake_v1.services.metastore_service.pagers.ListCatalogsPager:
                 Response message for the ListCatalogs
                 method.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
@@ -972,45 +972,45 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1
+            from google.cloud import bigquery_biglake_v1
 
             def sample_create_database():
                 # Create a client
-                client = biglake_v1.MetastoreServiceClient()
+                client = bigquery_biglake_v1.MetastoreServiceClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1.CreateDatabaseRequest(
+                request = bigquery_biglake_v1.CreateDatabaseRequest(
                     parent="parent_value",
                     database_id="database_id_value",
                 )
 
                 # Make the request
                 response = client.create_database(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.bigquery.biglake_v1.types.CreateDatabaseRequest, dict]):
+            request (Union[google.cloud.bigquery_biglake_v1.types.CreateDatabaseRequest, dict]):
                 The request object. Request message for the
                 CreateDatabase method.
             parent (str):
                 Required. The parent resource where this database will
                 be created. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            database (google.cloud.bigquery.biglake_v1.types.Database):
+            database (google.cloud.bigquery_biglake_v1.types.Database):
                 Required. The database to create. The ``name`` field
                 does not need to be provided.
 
                 This corresponds to the ``database`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             database_id (str):
@@ -1025,15 +1025,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1.types.Database:
+            google.cloud.bigquery_biglake_v1.types.Database:
                 Database is the container of tables.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, database, database_id])
         if request is not None and has_flattened_params:
@@ -1095,33 +1095,33 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1
+            from google.cloud import bigquery_biglake_v1
 
             def sample_delete_database():
                 # Create a client
-                client = biglake_v1.MetastoreServiceClient()
+                client = bigquery_biglake_v1.MetastoreServiceClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1.DeleteDatabaseRequest(
+                request = bigquery_biglake_v1.DeleteDatabaseRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 response = client.delete_database(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.bigquery.biglake_v1.types.DeleteDatabaseRequest, dict]):
+            request (Union[google.cloud.bigquery_biglake_v1.types.DeleteDatabaseRequest, dict]):
                 The request object. Request message for the
                 DeleteDatabase method.
             name (str):
                 Required. The name of the database to delete. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}
 
                 This corresponds to the ``name`` field
@@ -1130,15 +1130,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1.types.Database:
+            google.cloud.bigquery_biglake_v1.types.Database:
                 Database is the container of tables.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
@@ -1197,35 +1197,35 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1
+            from google.cloud import bigquery_biglake_v1
 
             def sample_update_database():
                 # Create a client
-                client = biglake_v1.MetastoreServiceClient()
+                client = bigquery_biglake_v1.MetastoreServiceClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1.UpdateDatabaseRequest(
+                request = bigquery_biglake_v1.UpdateDatabaseRequest(
                 )
 
                 # Make the request
                 response = client.update_database(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.bigquery.biglake_v1.types.UpdateDatabaseRequest, dict]):
+            request (Union[google.cloud.bigquery_biglake_v1.types.UpdateDatabaseRequest, dict]):
                 The request object. Request message for the
                 UpdateDatabase method.
-            database (google.cloud.bigquery.biglake_v1.types.Database):
+            database (google.cloud.bigquery_biglake_v1.types.Database):
                 Required. The database to update.
 
                 The database's ``name`` field is used to identify the
                 database to update. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}
 
                 This corresponds to the ``database`` field
@@ -1245,15 +1245,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1.types.Database:
+            google.cloud.bigquery_biglake_v1.types.Database:
                 Database is the container of tables.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([database, update_mask])
         if request is not None and has_flattened_params:
@@ -1314,33 +1314,33 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1
+            from google.cloud import bigquery_biglake_v1
 
             def sample_get_database():
                 # Create a client
-                client = biglake_v1.MetastoreServiceClient()
+                client = bigquery_biglake_v1.MetastoreServiceClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1.GetDatabaseRequest(
+                request = bigquery_biglake_v1.GetDatabaseRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 response = client.get_database(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.bigquery.biglake_v1.types.GetDatabaseRequest, dict]):
+            request (Union[google.cloud.bigquery_biglake_v1.types.GetDatabaseRequest, dict]):
                 The request object. Request message for the GetDatabase
                 method.
             name (str):
                 Required. The name of the database to retrieve. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}
 
                 This corresponds to the ``name`` field
@@ -1349,15 +1349,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1.types.Database:
+            google.cloud.bigquery_biglake_v1.types.Database:
                 Database is the container of tables.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
@@ -1414,34 +1414,34 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1
+            from google.cloud import bigquery_biglake_v1
 
             def sample_list_databases():
                 # Create a client
-                client = biglake_v1.MetastoreServiceClient()
+                client = bigquery_biglake_v1.MetastoreServiceClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1.ListDatabasesRequest(
+                request = bigquery_biglake_v1.ListDatabasesRequest(
                     parent="parent_value",
                 )
 
                 # Make the request
                 page_result = client.list_databases(request=request)
 
                 # Handle the response
                 for response in page_result:
                     print(response)
 
         Args:
-            request (Union[google.cloud.bigquery.biglake_v1.types.ListDatabasesRequest, dict]):
+            request (Union[google.cloud.bigquery_biglake_v1.types.ListDatabasesRequest, dict]):
                 The request object. Request message for the ListDatabases
                 method.
             parent (str):
                 Required. The parent, which owns this collection of
                 databases. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}
 
@@ -1451,15 +1451,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1.services.metastore_service.pagers.ListDatabasesPager:
+            google.cloud.bigquery_biglake_v1.services.metastore_service.pagers.ListDatabasesPager:
                 Response message for the
                 ListDatabases method.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
@@ -1532,45 +1532,45 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1
+            from google.cloud import bigquery_biglake_v1
 
             def sample_create_table():
                 # Create a client
-                client = biglake_v1.MetastoreServiceClient()
+                client = bigquery_biglake_v1.MetastoreServiceClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1.CreateTableRequest(
+                request = bigquery_biglake_v1.CreateTableRequest(
                     parent="parent_value",
                     table_id="table_id_value",
                 )
 
                 # Make the request
                 response = client.create_table(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.bigquery.biglake_v1.types.CreateTableRequest, dict]):
+            request (Union[google.cloud.bigquery_biglake_v1.types.CreateTableRequest, dict]):
                 The request object. Request message for the CreateTable
                 method.
             parent (str):
                 Required. The parent resource where this table will be
                 created. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            table (google.cloud.bigquery.biglake_v1.types.Table):
+            table (google.cloud.bigquery_biglake_v1.types.Table):
                 Required. The table to create. The ``name`` field does
                 not need to be provided for the table creation.
 
                 This corresponds to the ``table`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             table_id (str):
@@ -1584,15 +1584,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1.types.Table:
+            google.cloud.bigquery_biglake_v1.types.Table:
                 Represents a table.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, table, table_id])
         if request is not None and has_flattened_params:
@@ -1653,33 +1653,33 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1
+            from google.cloud import bigquery_biglake_v1
 
             def sample_delete_table():
                 # Create a client
-                client = biglake_v1.MetastoreServiceClient()
+                client = bigquery_biglake_v1.MetastoreServiceClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1.DeleteTableRequest(
+                request = bigquery_biglake_v1.DeleteTableRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 response = client.delete_table(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.bigquery.biglake_v1.types.DeleteTableRequest, dict]):
+            request (Union[google.cloud.bigquery_biglake_v1.types.DeleteTableRequest, dict]):
                 The request object. Request message for the DeleteTable
                 method.
             name (str):
                 Required. The name of the table to delete. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}/tables/{table_id}
 
                 This corresponds to the ``name`` field
@@ -1688,15 +1688,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1.types.Table:
+            google.cloud.bigquery_biglake_v1.types.Table:
                 Represents a table.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
@@ -1754,35 +1754,35 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1
+            from google.cloud import bigquery_biglake_v1
 
             def sample_update_table():
                 # Create a client
-                client = biglake_v1.MetastoreServiceClient()
+                client = bigquery_biglake_v1.MetastoreServiceClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1.UpdateTableRequest(
+                request = bigquery_biglake_v1.UpdateTableRequest(
                 )
 
                 # Make the request
                 response = client.update_table(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.bigquery.biglake_v1.types.UpdateTableRequest, dict]):
+            request (Union[google.cloud.bigquery_biglake_v1.types.UpdateTableRequest, dict]):
                 The request object. Request message for the UpdateTable
                 method.
-            table (google.cloud.bigquery.biglake_v1.types.Table):
+            table (google.cloud.bigquery_biglake_v1.types.Table):
                 Required. The table to update.
 
                 The table's ``name`` field is used to identify the table
                 to update. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}/tables/{table_id}
 
                 This corresponds to the ``table`` field
@@ -1802,15 +1802,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1.types.Table:
+            google.cloud.bigquery_biglake_v1.types.Table:
                 Represents a table.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([table, update_mask])
         if request is not None and has_flattened_params:
@@ -1872,34 +1872,34 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1
+            from google.cloud import bigquery_biglake_v1
 
             def sample_rename_table():
                 # Create a client
-                client = biglake_v1.MetastoreServiceClient()
+                client = bigquery_biglake_v1.MetastoreServiceClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1.RenameTableRequest(
+                request = bigquery_biglake_v1.RenameTableRequest(
                     name="name_value",
                     new_name="new_name_value",
                 )
 
                 # Make the request
                 response = client.rename_table(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.bigquery.biglake_v1.types.RenameTableRequest, dict]):
+            request (Union[google.cloud.bigquery_biglake_v1.types.RenameTableRequest, dict]):
                 The request object. Request message for the RenameTable
                 method in MetastoreService
             name (str):
                 Required. The table's ``name`` field is used to identify
                 the table to rename. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}/tables/{table_id}
 
@@ -1917,15 +1917,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1.types.Table:
+            google.cloud.bigquery_biglake_v1.types.Table:
                 Represents a table.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name, new_name])
         if request is not None and has_flattened_params:
@@ -1984,33 +1984,33 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1
+            from google.cloud import bigquery_biglake_v1
 
             def sample_get_table():
                 # Create a client
-                client = biglake_v1.MetastoreServiceClient()
+                client = bigquery_biglake_v1.MetastoreServiceClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1.GetTableRequest(
+                request = bigquery_biglake_v1.GetTableRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 response = client.get_table(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.bigquery.biglake_v1.types.GetTableRequest, dict]):
+            request (Union[google.cloud.bigquery_biglake_v1.types.GetTableRequest, dict]):
                 The request object. Request message for the GetTable
                 method.
             name (str):
                 Required. The name of the table to retrieve. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}/tables/{table_id}
 
                 This corresponds to the ``name`` field
@@ -2019,15 +2019,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1.types.Table:
+            google.cloud.bigquery_biglake_v1.types.Table:
                 Represents a table.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
@@ -2084,34 +2084,34 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1
+            from google.cloud import bigquery_biglake_v1
 
             def sample_list_tables():
                 # Create a client
-                client = biglake_v1.MetastoreServiceClient()
+                client = bigquery_biglake_v1.MetastoreServiceClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1.ListTablesRequest(
+                request = bigquery_biglake_v1.ListTablesRequest(
                     parent="parent_value",
                 )
 
                 # Make the request
                 page_result = client.list_tables(request=request)
 
                 # Handle the response
                 for response in page_result:
                     print(response)
 
         Args:
-            request (Union[google.cloud.bigquery.biglake_v1.types.ListTablesRequest, dict]):
+            request (Union[google.cloud.bigquery_biglake_v1.types.ListTablesRequest, dict]):
                 The request object. Request message for the ListTables
                 method.
             parent (str):
                 Required. The parent, which owns this collection of
                 tables. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}
 
@@ -2121,15 +2121,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1.services.metastore_service.pagers.ListTablesPager:
+            google.cloud.bigquery_biglake_v1.services.metastore_service.pagers.ListTablesPager:
                 Response message for the ListTables
                 method.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
```

### Comparing `google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/services/metastore_service/pagers.py` & `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/services/metastore_service/pagers.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,31 +20,31 @@
     Callable,
     Iterator,
     Optional,
     Sequence,
     Tuple,
 )
 
-from google.cloud.bigquery.biglake_v1.types import metastore
+from google.cloud.bigquery_biglake_v1.types import metastore
 
 
 class ListCatalogsPager:
     """A pager for iterating through ``list_catalogs`` requests.
 
     This class thinly wraps an initial
-    :class:`google.cloud.bigquery.biglake_v1.types.ListCatalogsResponse` object, and
+    :class:`google.cloud.bigquery_biglake_v1.types.ListCatalogsResponse` object, and
     provides an ``__iter__`` method to iterate through its
     ``catalogs`` field.
 
     If there are more pages, the ``__iter__`` method will make additional
     ``ListCatalogs`` requests and continue to iterate
     through the ``catalogs`` field on the
     corresponding responses.
 
-    All the usual :class:`google.cloud.bigquery.biglake_v1.types.ListCatalogsResponse`
+    All the usual :class:`google.cloud.bigquery_biglake_v1.types.ListCatalogsResponse`
     attributes are available on the pager. If multiple requests are made, only
     the most recent response is retained, and thus used for attribute lookup.
     """
 
     def __init__(
         self,
         method: Callable[..., metastore.ListCatalogsResponse],
@@ -54,17 +54,17 @@
         metadata: Sequence[Tuple[str, str]] = ()
     ):
         """Instantiate the pager.
 
         Args:
             method (Callable): The method that was originally called, and
                 which instantiated this pager.
-            request (google.cloud.bigquery.biglake_v1.types.ListCatalogsRequest):
+            request (google.cloud.bigquery_biglake_v1.types.ListCatalogsRequest):
                 The initial request object.
-            response (google.cloud.bigquery.biglake_v1.types.ListCatalogsResponse):
+            response (google.cloud.bigquery_biglake_v1.types.ListCatalogsResponse):
                 The initial response object.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         self._method = method
         self._request = metastore.ListCatalogsRequest(request)
         self._response = response
@@ -89,24 +89,24 @@
         return "{0}<{1!r}>".format(self.__class__.__name__, self._response)
 
 
 class ListCatalogsAsyncPager:
     """A pager for iterating through ``list_catalogs`` requests.
 
     This class thinly wraps an initial
-    :class:`google.cloud.bigquery.biglake_v1.types.ListCatalogsResponse` object, and
+    :class:`google.cloud.bigquery_biglake_v1.types.ListCatalogsResponse` object, and
     provides an ``__aiter__`` method to iterate through its
     ``catalogs`` field.
 
     If there are more pages, the ``__aiter__`` method will make additional
     ``ListCatalogs`` requests and continue to iterate
     through the ``catalogs`` field on the
     corresponding responses.
 
-    All the usual :class:`google.cloud.bigquery.biglake_v1.types.ListCatalogsResponse`
+    All the usual :class:`google.cloud.bigquery_biglake_v1.types.ListCatalogsResponse`
     attributes are available on the pager. If multiple requests are made, only
     the most recent response is retained, and thus used for attribute lookup.
     """
 
     def __init__(
         self,
         method: Callable[..., Awaitable[metastore.ListCatalogsResponse]],
@@ -116,17 +116,17 @@
         metadata: Sequence[Tuple[str, str]] = ()
     ):
         """Instantiates the pager.
 
         Args:
             method (Callable): The method that was originally called, and
                 which instantiated this pager.
-            request (google.cloud.bigquery.biglake_v1.types.ListCatalogsRequest):
+            request (google.cloud.bigquery_biglake_v1.types.ListCatalogsRequest):
                 The initial request object.
-            response (google.cloud.bigquery.biglake_v1.types.ListCatalogsResponse):
+            response (google.cloud.bigquery_biglake_v1.types.ListCatalogsResponse):
                 The initial response object.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         self._method = method
         self._request = metastore.ListCatalogsRequest(request)
         self._response = response
@@ -155,24 +155,24 @@
         return "{0}<{1!r}>".format(self.__class__.__name__, self._response)
 
 
 class ListDatabasesPager:
     """A pager for iterating through ``list_databases`` requests.
 
     This class thinly wraps an initial
-    :class:`google.cloud.bigquery.biglake_v1.types.ListDatabasesResponse` object, and
+    :class:`google.cloud.bigquery_biglake_v1.types.ListDatabasesResponse` object, and
     provides an ``__iter__`` method to iterate through its
     ``databases`` field.
 
     If there are more pages, the ``__iter__`` method will make additional
     ``ListDatabases`` requests and continue to iterate
     through the ``databases`` field on the
     corresponding responses.
 
-    All the usual :class:`google.cloud.bigquery.biglake_v1.types.ListDatabasesResponse`
+    All the usual :class:`google.cloud.bigquery_biglake_v1.types.ListDatabasesResponse`
     attributes are available on the pager. If multiple requests are made, only
     the most recent response is retained, and thus used for attribute lookup.
     """
 
     def __init__(
         self,
         method: Callable[..., metastore.ListDatabasesResponse],
@@ -182,17 +182,17 @@
         metadata: Sequence[Tuple[str, str]] = ()
     ):
         """Instantiate the pager.
 
         Args:
             method (Callable): The method that was originally called, and
                 which instantiated this pager.
-            request (google.cloud.bigquery.biglake_v1.types.ListDatabasesRequest):
+            request (google.cloud.bigquery_biglake_v1.types.ListDatabasesRequest):
                 The initial request object.
-            response (google.cloud.bigquery.biglake_v1.types.ListDatabasesResponse):
+            response (google.cloud.bigquery_biglake_v1.types.ListDatabasesResponse):
                 The initial response object.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         self._method = method
         self._request = metastore.ListDatabasesRequest(request)
         self._response = response
@@ -217,24 +217,24 @@
         return "{0}<{1!r}>".format(self.__class__.__name__, self._response)
 
 
 class ListDatabasesAsyncPager:
     """A pager for iterating through ``list_databases`` requests.
 
     This class thinly wraps an initial
-    :class:`google.cloud.bigquery.biglake_v1.types.ListDatabasesResponse` object, and
+    :class:`google.cloud.bigquery_biglake_v1.types.ListDatabasesResponse` object, and
     provides an ``__aiter__`` method to iterate through its
     ``databases`` field.
 
     If there are more pages, the ``__aiter__`` method will make additional
     ``ListDatabases`` requests and continue to iterate
     through the ``databases`` field on the
     corresponding responses.
 
-    All the usual :class:`google.cloud.bigquery.biglake_v1.types.ListDatabasesResponse`
+    All the usual :class:`google.cloud.bigquery_biglake_v1.types.ListDatabasesResponse`
     attributes are available on the pager. If multiple requests are made, only
     the most recent response is retained, and thus used for attribute lookup.
     """
 
     def __init__(
         self,
         method: Callable[..., Awaitable[metastore.ListDatabasesResponse]],
@@ -244,17 +244,17 @@
         metadata: Sequence[Tuple[str, str]] = ()
     ):
         """Instantiates the pager.
 
         Args:
             method (Callable): The method that was originally called, and
                 which instantiated this pager.
-            request (google.cloud.bigquery.biglake_v1.types.ListDatabasesRequest):
+            request (google.cloud.bigquery_biglake_v1.types.ListDatabasesRequest):
                 The initial request object.
-            response (google.cloud.bigquery.biglake_v1.types.ListDatabasesResponse):
+            response (google.cloud.bigquery_biglake_v1.types.ListDatabasesResponse):
                 The initial response object.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         self._method = method
         self._request = metastore.ListDatabasesRequest(request)
         self._response = response
@@ -283,24 +283,24 @@
         return "{0}<{1!r}>".format(self.__class__.__name__, self._response)
 
 
 class ListTablesPager:
     """A pager for iterating through ``list_tables`` requests.
 
     This class thinly wraps an initial
-    :class:`google.cloud.bigquery.biglake_v1.types.ListTablesResponse` object, and
+    :class:`google.cloud.bigquery_biglake_v1.types.ListTablesResponse` object, and
     provides an ``__iter__`` method to iterate through its
     ``tables`` field.
 
     If there are more pages, the ``__iter__`` method will make additional
     ``ListTables`` requests and continue to iterate
     through the ``tables`` field on the
     corresponding responses.
 
-    All the usual :class:`google.cloud.bigquery.biglake_v1.types.ListTablesResponse`
+    All the usual :class:`google.cloud.bigquery_biglake_v1.types.ListTablesResponse`
     attributes are available on the pager. If multiple requests are made, only
     the most recent response is retained, and thus used for attribute lookup.
     """
 
     def __init__(
         self,
         method: Callable[..., metastore.ListTablesResponse],
@@ -310,17 +310,17 @@
         metadata: Sequence[Tuple[str, str]] = ()
     ):
         """Instantiate the pager.
 
         Args:
             method (Callable): The method that was originally called, and
                 which instantiated this pager.
-            request (google.cloud.bigquery.biglake_v1.types.ListTablesRequest):
+            request (google.cloud.bigquery_biglake_v1.types.ListTablesRequest):
                 The initial request object.
-            response (google.cloud.bigquery.biglake_v1.types.ListTablesResponse):
+            response (google.cloud.bigquery_biglake_v1.types.ListTablesResponse):
                 The initial response object.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         self._method = method
         self._request = metastore.ListTablesRequest(request)
         self._response = response
@@ -345,24 +345,24 @@
         return "{0}<{1!r}>".format(self.__class__.__name__, self._response)
 
 
 class ListTablesAsyncPager:
     """A pager for iterating through ``list_tables`` requests.
 
     This class thinly wraps an initial
-    :class:`google.cloud.bigquery.biglake_v1.types.ListTablesResponse` object, and
+    :class:`google.cloud.bigquery_biglake_v1.types.ListTablesResponse` object, and
     provides an ``__aiter__`` method to iterate through its
     ``tables`` field.
 
     If there are more pages, the ``__aiter__`` method will make additional
     ``ListTables`` requests and continue to iterate
     through the ``tables`` field on the
     corresponding responses.
 
-    All the usual :class:`google.cloud.bigquery.biglake_v1.types.ListTablesResponse`
+    All the usual :class:`google.cloud.bigquery_biglake_v1.types.ListTablesResponse`
     attributes are available on the pager. If multiple requests are made, only
     the most recent response is retained, and thus used for attribute lookup.
     """
 
     def __init__(
         self,
         method: Callable[..., Awaitable[metastore.ListTablesResponse]],
@@ -372,17 +372,17 @@
         metadata: Sequence[Tuple[str, str]] = ()
     ):
         """Instantiates the pager.
 
         Args:
             method (Callable): The method that was originally called, and
                 which instantiated this pager.
-            request (google.cloud.bigquery.biglake_v1.types.ListTablesRequest):
+            request (google.cloud.bigquery_biglake_v1.types.ListTablesRequest):
                 The initial request object.
-            response (google.cloud.bigquery.biglake_v1.types.ListTablesResponse):
+            response (google.cloud.bigquery_biglake_v1.types.ListTablesResponse):
                 The initial response object.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         self._method = method
         self._request = metastore.ListTablesRequest(request)
         self._response = response
```

### Comparing `google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/services/metastore_service/transports/__init__.py` & `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/services/metastore_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/services/metastore_service/transports/base.py` & `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/services/metastore_service/transports/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 
-from google.cloud.bigquery.biglake_v1 import gapic_version as package_version
-from google.cloud.bigquery.biglake_v1.types import metastore
+from google.cloud.bigquery_biglake_v1 import gapic_version as package_version
+from google.cloud.bigquery_biglake_v1.types import metastore
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
     gapic_version=package_version.__version__
 )
 
 
 class MetastoreServiceTransport(abc.ABC):
```

### Comparing `google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/services/metastore_service/transports/grpc.py` & `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/services/metastore_service/transports/grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 from google.api_core import gapic_v1, grpc_helpers
 import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 import grpc  # type: ignore
 
-from google.cloud.bigquery.biglake_v1.types import metastore
+from google.cloud.bigquery_biglake_v1.types import metastore
 
 from .base import DEFAULT_CLIENT_INFO, MetastoreServiceTransport
 
 
 class MetastoreServiceGrpcTransport(MetastoreServiceTransport):
     """gRPC backend transport for MetastoreService.
```

### Comparing `google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/services/metastore_service/transports/grpc_asyncio.py` & `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/services/metastore_service/transports/grpc_asyncio.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 from google.api_core import gapic_v1, grpc_helpers_async
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 import grpc  # type: ignore
 from grpc.experimental import aio  # type: ignore
 
-from google.cloud.bigquery.biglake_v1.types import metastore
+from google.cloud.bigquery_biglake_v1.types import metastore
 
 from .base import DEFAULT_CLIENT_INFO, MetastoreServiceTransport
 from .grpc import MetastoreServiceGrpcTransport
 
 
 class MetastoreServiceGrpcAsyncIOTransport(MetastoreServiceTransport):
     """gRPC AsyncIO backend transport for MetastoreService.
```

### Comparing `google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/services/metastore_service/transports/rest.py` & `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/services/metastore_service/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 
-from google.cloud.bigquery.biglake_v1.types import metastore
+from google.cloud.bigquery_biglake_v1.types import metastore
 
 from .base import DEFAULT_CLIENT_INFO as BASE_DEFAULT_CLIENT_INFO
 from .base import MetastoreServiceTransport
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
     gapic_version=BASE_DEFAULT_CLIENT_INFO.gapic_version,
     grpc_version=None,
```

### Comparing `google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/types/__init__.py` & `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/types/metastore.py` & `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1/types/metastore.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,15 +121,15 @@
 
 class Database(proto.Message):
     r"""Database is the container of tables.
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
     Attributes:
-        hive_options (google.cloud.bigquery.biglake_v1.types.HiveDatabaseOptions):
+        hive_options (google.cloud.bigquery_biglake_v1.types.HiveDatabaseOptions):
             Options of a Hive database.
 
             This field is a member of `oneof`_ ``options``.
         name (str):
             Output only. The resource name. Format:
             projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}
         create_time (google.protobuf.timestamp_pb2.Timestamp):
@@ -142,15 +142,15 @@
             Output only. The deletion time of the
             database. Only set after the database is
             deleted.
         expire_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. The time when this database is
             considered expired. Only set after the database
             is deleted.
-        type_ (google.cloud.bigquery.biglake_v1.types.Database.Type):
+        type_ (google.cloud.bigquery_biglake_v1.types.Database.Type):
             The database type.
     """
 
     class Type(proto.Enum):
         r"""The database type.
 
         Values:
@@ -202,15 +202,15 @@
 
 class Table(proto.Message):
     r"""Represents a table.
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
     Attributes:
-        hive_options (google.cloud.bigquery.biglake_v1.types.HiveTableOptions):
+        hive_options (google.cloud.bigquery_biglake_v1.types.HiveTableOptions):
             Options of a Hive table.
 
             This field is a member of `oneof`_ ``options``.
         name (str):
             Output only. The resource name. Format:
             projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}/tables/{table_id}
         create_time (google.protobuf.timestamp_pb2.Timestamp):
@@ -221,15 +221,15 @@
         delete_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. The deletion time of the table.
             Only set after the table is deleted.
         expire_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. The time when this table is
             considered expired. Only set after the table is
             deleted.
-        type_ (google.cloud.bigquery.biglake_v1.types.Table.Type):
+        type_ (google.cloud.bigquery_biglake_v1.types.Table.Type):
             The table type.
         etag (str):
             The checksum of a table object computed by
             the server based on the value of other fields.
             It may be sent on update requests to ensure the
             client has an up-to-date value before
             proceeding. It is only checked for update table
@@ -294,15 +294,15 @@
     r"""Request message for the CreateCatalog method.
 
     Attributes:
         parent (str):
             Required. The parent resource where this catalog will be
             created. Format:
             projects/{project_id_or_number}/locations/{location_id}
-        catalog (google.cloud.bigquery.biglake_v1.types.Catalog):
+        catalog (google.cloud.bigquery_biglake_v1.types.Catalog):
             Required. The catalog to create. The ``name`` field does not
             need to be provided.
         catalog_id (str):
             Required. The ID to use for the catalog,
             which will become the final component of the
             catalog's resource name.
     """
@@ -389,15 +389,15 @@
     )
 
 
 class ListCatalogsResponse(proto.Message):
     r"""Response message for the ListCatalogs method.
 
     Attributes:
-        catalogs (MutableSequence[google.cloud.bigquery.biglake_v1.types.Catalog]):
+        catalogs (MutableSequence[google.cloud.bigquery_biglake_v1.types.Catalog]):
             The catalogs from the specified project.
         next_page_token (str):
             A token, which can be sent as ``page_token`` to retrieve the
             next page. If this field is omitted, there are no subsequent
             pages.
     """
 
@@ -420,15 +420,15 @@
     r"""Request message for the CreateDatabase method.
 
     Attributes:
         parent (str):
             Required. The parent resource where this database will be
             created. Format:
             projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}
-        database (google.cloud.bigquery.biglake_v1.types.Database):
+        database (google.cloud.bigquery_biglake_v1.types.Database):
             Required. The database to create. The ``name`` field does
             not need to be provided.
         database_id (str):
             Required. The ID to use for the database,
             which will become the final component of the
             database's resource name.
     """
@@ -463,15 +463,15 @@
     )
 
 
 class UpdateDatabaseRequest(proto.Message):
     r"""Request message for the UpdateDatabase method.
 
     Attributes:
-        database (google.cloud.bigquery.biglake_v1.types.Database):
+        database (google.cloud.bigquery_biglake_v1.types.Database):
             Required. The database to update.
 
             The database's ``name`` field is used to identify the
             database to update. Format:
             projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}
         update_mask (google.protobuf.field_mask_pb2.FieldMask):
             The list of fields to update.
@@ -546,15 +546,15 @@
     )
 
 
 class ListDatabasesResponse(proto.Message):
     r"""Response message for the ListDatabases method.
 
     Attributes:
-        databases (MutableSequence[google.cloud.bigquery.biglake_v1.types.Database]):
+        databases (MutableSequence[google.cloud.bigquery_biglake_v1.types.Database]):
             The databases from the specified catalog.
         next_page_token (str):
             A token, which can be sent as ``page_token`` to retrieve the
             next page. If this field is omitted, there are no subsequent
             pages.
     """
 
@@ -577,15 +577,15 @@
     r"""Request message for the CreateTable method.
 
     Attributes:
         parent (str):
             Required. The parent resource where this table will be
             created. Format:
             projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}
-        table (google.cloud.bigquery.biglake_v1.types.Table):
+        table (google.cloud.bigquery_biglake_v1.types.Table):
             Required. The table to create. The ``name`` field does not
             need to be provided for the table creation.
         table_id (str):
             Required. The ID to use for the table, which
             will become the final component of the table's
             resource name.
     """
@@ -620,15 +620,15 @@
     )
 
 
 class UpdateTableRequest(proto.Message):
     r"""Request message for the UpdateTable method.
 
     Attributes:
-        table (google.cloud.bigquery.biglake_v1.types.Table):
+        table (google.cloud.bigquery_biglake_v1.types.Table):
             Required. The table to update.
 
             The table's ``name`` field is used to identify the table to
             update. Format:
             projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}/tables/{table_id}
         update_mask (google.protobuf.field_mask_pb2.FieldMask):
             The list of fields to update.
@@ -708,15 +708,15 @@
         page_token (str):
             A page token, received from a previous ``ListTables`` call.
             Provide this to retrieve the subsequent page.
 
             When paginating, all other parameters provided to
             ``ListTables`` must match the call that provided the page
             token.
-        view (google.cloud.bigquery.biglake_v1.types.TableView):
+        view (google.cloud.bigquery_biglake_v1.types.TableView):
             The view for the returned tables.
     """
 
     parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
@@ -735,15 +735,15 @@
     )
 
 
 class ListTablesResponse(proto.Message):
     r"""Response message for the ListTables method.
 
     Attributes:
-        tables (MutableSequence[google.cloud.bigquery.biglake_v1.types.Table]):
+        tables (MutableSequence[google.cloud.bigquery_biglake_v1.types.Table]):
             The tables from the specified database.
         next_page_token (str):
             A token, which can be sent as ``page_token`` to retrieve the
             next page. If this field is omitted, there are no subsequent
             pages.
     """
 
@@ -789,15 +789,15 @@
     r"""Options of a Hive table.
 
     Attributes:
         parameters (MutableMapping[str, str]):
             Stores user supplied Hive table parameters.
         table_type (str):
             Hive table type. For example, MANAGED_TABLE, EXTERNAL_TABLE.
-        storage_descriptor (google.cloud.bigquery.biglake_v1.types.HiveTableOptions.StorageDescriptor):
+        storage_descriptor (google.cloud.bigquery_biglake_v1.types.HiveTableOptions.StorageDescriptor):
             Stores physical storage information of the
             data.
     """
 
     class SerDeInfo(proto.Message):
         r"""Serializer and deserializer information.
 
@@ -821,15 +821,15 @@
                 is stored, starting with "gs://".
             input_format (str):
                 The fully qualified Java class name of the
                 input format.
             output_format (str):
                 The fully qualified Java class name of the
                 output format.
-            serde_info (google.cloud.bigquery.biglake_v1.types.HiveTableOptions.SerDeInfo):
+            serde_info (google.cloud.bigquery_biglake_v1.types.HiveTableOptions.SerDeInfo):
                 Serializer and deserializer information.
         """
 
         location_uri: str = proto.Field(
             proto.STRING,
             number=1,
         )
```

### Comparing `google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/__init__.py` & `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from google.cloud.bigquery.biglake_v1alpha1 import gapic_version as package_version
+from google.cloud.bigquery_biglake_v1alpha1 import gapic_version as package_version
 
 __version__ = package_version.__version__
 
 
 from .services.metastore_service import (
     MetastoreServiceAsyncClient,
     MetastoreServiceClient,
```

### Comparing `google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/gapic_metadata.json` & `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/gapic_metadata.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'libraryPackage'": "'google.cloud.bigquery_biglake_v1alpha1'"}*

```diff
@@ -1,11 +1,11 @@
 {
     "comment": "This file maps proto services/RPCs to the corresponding library clients/methods",
     "language": "python",
-    "libraryPackage": "google.cloud.bigquery.biglake_v1alpha1",
+    "libraryPackage": "google.cloud.bigquery_biglake_v1alpha1",
     "protoPackage": "google.cloud.bigquery.biglake.v1alpha1",
     "schema": "1.0",
     "services": {
         "MetastoreService": {
             "clients": {
                 "grpc": {
                     "libraryClient": "MetastoreServiceClient",
```

### Comparing `google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/gapic_version.py` & `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/gapic_version.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-
-__version__ = "0.3.0"  # {x-release-please-version}
+__version__ = "0.4.0"  # {x-release-please-version}
```

### Comparing `google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/services/__init__.py` & `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/__init__.py` & `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/async_client.py` & `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/async_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,26 +31,26 @@
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.api_core.client_options import ClientOptions
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 
-from google.cloud.bigquery.biglake_v1alpha1 import gapic_version as package_version
+from google.cloud.bigquery_biglake_v1alpha1 import gapic_version as package_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.protobuf import field_mask_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 
-from google.cloud.bigquery.biglake_v1alpha1.services.metastore_service import pagers
-from google.cloud.bigquery.biglake_v1alpha1.types import metastore
+from google.cloud.bigquery_biglake_v1alpha1.services.metastore_service import pagers
+from google.cloud.bigquery_biglake_v1alpha1.types import metastore
 
 from .client import MetastoreServiceClient
 from .transports.base import DEFAULT_CLIENT_INFO, MetastoreServiceTransport
 from .transports.grpc_asyncio import MetastoreServiceGrpcAsyncIOTransport
 
 
 class MetastoreServiceAsyncClient:
@@ -252,45 +252,45 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1alpha1
+            from google.cloud import bigquery_biglake_v1alpha1
 
             async def sample_create_catalog():
                 # Create a client
-                client = biglake_v1alpha1.MetastoreServiceAsyncClient()
+                client = bigquery_biglake_v1alpha1.MetastoreServiceAsyncClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1alpha1.CreateCatalogRequest(
+                request = bigquery_biglake_v1alpha1.CreateCatalogRequest(
                     parent="parent_value",
                     catalog_id="catalog_id_value",
                 )
 
                 # Make the request
                 response = await client.create_catalog(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.biglake_v1alpha1.types.CreateCatalogRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_biglake_v1alpha1.types.CreateCatalogRequest, dict]]):
                 The request object. Request message for the CreateCatalog
                 method.
             parent (:class:`str`):
                 Required. The parent resource where this catalog will be
                 created. Format:
                 projects/{project_id_or_number}/locations/{location_id}
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            catalog (:class:`google.cloud.bigquery.biglake_v1alpha1.types.Catalog`):
+            catalog (:class:`google.cloud.bigquery_biglake_v1alpha1.types.Catalog`):
                 Required. The catalog to create. The ``name`` field does
                 not need to be provided.
 
                 This corresponds to the ``catalog`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             catalog_id (:class:`str`):
@@ -305,15 +305,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1alpha1.types.Catalog:
+            google.cloud.bigquery_biglake_v1alpha1.types.Catalog:
                 Catalog is the container of
                 databases.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
@@ -377,33 +377,33 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1alpha1
+            from google.cloud import bigquery_biglake_v1alpha1
 
             async def sample_delete_catalog():
                 # Create a client
-                client = biglake_v1alpha1.MetastoreServiceAsyncClient()
+                client = bigquery_biglake_v1alpha1.MetastoreServiceAsyncClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1alpha1.DeleteCatalogRequest(
+                request = bigquery_biglake_v1alpha1.DeleteCatalogRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 response = await client.delete_catalog(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.biglake_v1alpha1.types.DeleteCatalogRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_biglake_v1alpha1.types.DeleteCatalogRequest, dict]]):
                 The request object. Request message for the DeleteCatalog
                 method.
             name (:class:`str`):
                 Required. The name of the catalog to delete. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}
 
                 This corresponds to the ``name`` field
@@ -412,15 +412,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1alpha1.types.Catalog:
+            google.cloud.bigquery_biglake_v1alpha1.types.Catalog:
                 Catalog is the container of
                 databases.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
@@ -479,33 +479,33 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1alpha1
+            from google.cloud import bigquery_biglake_v1alpha1
 
             async def sample_get_catalog():
                 # Create a client
-                client = biglake_v1alpha1.MetastoreServiceAsyncClient()
+                client = bigquery_biglake_v1alpha1.MetastoreServiceAsyncClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1alpha1.GetCatalogRequest(
+                request = bigquery_biglake_v1alpha1.GetCatalogRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 response = await client.get_catalog(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.biglake_v1alpha1.types.GetCatalogRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_biglake_v1alpha1.types.GetCatalogRequest, dict]]):
                 The request object. Request message for the GetCatalog
                 method.
             name (:class:`str`):
                 Required. The name of the catalog to retrieve. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}
 
                 This corresponds to the ``name`` field
@@ -514,15 +514,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1alpha1.types.Catalog:
+            google.cloud.bigquery_biglake_v1alpha1.types.Catalog:
                 Catalog is the container of
                 databases.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
@@ -581,34 +581,34 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1alpha1
+            from google.cloud import bigquery_biglake_v1alpha1
 
             async def sample_list_catalogs():
                 # Create a client
-                client = biglake_v1alpha1.MetastoreServiceAsyncClient()
+                client = bigquery_biglake_v1alpha1.MetastoreServiceAsyncClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1alpha1.ListCatalogsRequest(
+                request = bigquery_biglake_v1alpha1.ListCatalogsRequest(
                     parent="parent_value",
                 )
 
                 # Make the request
                 page_result = client.list_catalogs(request=request)
 
                 # Handle the response
                 async for response in page_result:
                     print(response)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.biglake_v1alpha1.types.ListCatalogsRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_biglake_v1alpha1.types.ListCatalogsRequest, dict]]):
                 The request object. Request message for the ListCatalogs
                 method.
             parent (:class:`str`):
                 Required. The parent, which owns this collection of
                 catalogs. Format:
                 projects/{project_id_or_number}/locations/{location_id}
 
@@ -618,15 +618,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1alpha1.services.metastore_service.pagers.ListCatalogsAsyncPager:
+            google.cloud.bigquery_biglake_v1alpha1.services.metastore_service.pagers.ListCatalogsAsyncPager:
                 Response message for the ListCatalogs
                 method.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
@@ -699,45 +699,45 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1alpha1
+            from google.cloud import bigquery_biglake_v1alpha1
 
             async def sample_create_database():
                 # Create a client
-                client = biglake_v1alpha1.MetastoreServiceAsyncClient()
+                client = bigquery_biglake_v1alpha1.MetastoreServiceAsyncClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1alpha1.CreateDatabaseRequest(
+                request = bigquery_biglake_v1alpha1.CreateDatabaseRequest(
                     parent="parent_value",
                     database_id="database_id_value",
                 )
 
                 # Make the request
                 response = await client.create_database(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.biglake_v1alpha1.types.CreateDatabaseRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_biglake_v1alpha1.types.CreateDatabaseRequest, dict]]):
                 The request object. Request message for the
                 CreateDatabase method.
             parent (:class:`str`):
                 Required. The parent resource where this database will
                 be created. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            database (:class:`google.cloud.bigquery.biglake_v1alpha1.types.Database`):
+            database (:class:`google.cloud.bigquery_biglake_v1alpha1.types.Database`):
                 Required. The database to create. The ``name`` field
                 does not need to be provided.
 
                 This corresponds to the ``database`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             database_id (:class:`str`):
@@ -752,15 +752,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1alpha1.types.Database:
+            google.cloud.bigquery_biglake_v1alpha1.types.Database:
                 Database is the container of tables.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, database, database_id])
         if request is not None and has_flattened_params:
@@ -822,33 +822,33 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1alpha1
+            from google.cloud import bigquery_biglake_v1alpha1
 
             async def sample_delete_database():
                 # Create a client
-                client = biglake_v1alpha1.MetastoreServiceAsyncClient()
+                client = bigquery_biglake_v1alpha1.MetastoreServiceAsyncClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1alpha1.DeleteDatabaseRequest(
+                request = bigquery_biglake_v1alpha1.DeleteDatabaseRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 response = await client.delete_database(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.biglake_v1alpha1.types.DeleteDatabaseRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_biglake_v1alpha1.types.DeleteDatabaseRequest, dict]]):
                 The request object. Request message for the
                 DeleteDatabase method.
             name (:class:`str`):
                 Required. The name of the database to delete. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}
 
                 This corresponds to the ``name`` field
@@ -857,15 +857,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1alpha1.types.Database:
+            google.cloud.bigquery_biglake_v1alpha1.types.Database:
                 Database is the container of tables.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
@@ -924,35 +924,35 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1alpha1
+            from google.cloud import bigquery_biglake_v1alpha1
 
             async def sample_update_database():
                 # Create a client
-                client = biglake_v1alpha1.MetastoreServiceAsyncClient()
+                client = bigquery_biglake_v1alpha1.MetastoreServiceAsyncClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1alpha1.UpdateDatabaseRequest(
+                request = bigquery_biglake_v1alpha1.UpdateDatabaseRequest(
                 )
 
                 # Make the request
                 response = await client.update_database(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.biglake_v1alpha1.types.UpdateDatabaseRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_biglake_v1alpha1.types.UpdateDatabaseRequest, dict]]):
                 The request object. Request message for the
                 UpdateDatabase method.
-            database (:class:`google.cloud.bigquery.biglake_v1alpha1.types.Database`):
+            database (:class:`google.cloud.bigquery_biglake_v1alpha1.types.Database`):
                 Required. The database to update.
 
                 The database's ``name`` field is used to identify the
                 database to update. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}
 
                 This corresponds to the ``database`` field
@@ -972,15 +972,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1alpha1.types.Database:
+            google.cloud.bigquery_biglake_v1alpha1.types.Database:
                 Database is the container of tables.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([database, update_mask])
         if request is not None and has_flattened_params:
@@ -1041,33 +1041,33 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1alpha1
+            from google.cloud import bigquery_biglake_v1alpha1
 
             async def sample_get_database():
                 # Create a client
-                client = biglake_v1alpha1.MetastoreServiceAsyncClient()
+                client = bigquery_biglake_v1alpha1.MetastoreServiceAsyncClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1alpha1.GetDatabaseRequest(
+                request = bigquery_biglake_v1alpha1.GetDatabaseRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 response = await client.get_database(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.biglake_v1alpha1.types.GetDatabaseRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_biglake_v1alpha1.types.GetDatabaseRequest, dict]]):
                 The request object. Request message for the GetDatabase
                 method.
             name (:class:`str`):
                 Required. The name of the database to retrieve. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}
 
                 This corresponds to the ``name`` field
@@ -1076,15 +1076,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1alpha1.types.Database:
+            google.cloud.bigquery_biglake_v1alpha1.types.Database:
                 Database is the container of tables.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
@@ -1141,34 +1141,34 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1alpha1
+            from google.cloud import bigquery_biglake_v1alpha1
 
             async def sample_list_databases():
                 # Create a client
-                client = biglake_v1alpha1.MetastoreServiceAsyncClient()
+                client = bigquery_biglake_v1alpha1.MetastoreServiceAsyncClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1alpha1.ListDatabasesRequest(
+                request = bigquery_biglake_v1alpha1.ListDatabasesRequest(
                     parent="parent_value",
                 )
 
                 # Make the request
                 page_result = client.list_databases(request=request)
 
                 # Handle the response
                 async for response in page_result:
                     print(response)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.biglake_v1alpha1.types.ListDatabasesRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_biglake_v1alpha1.types.ListDatabasesRequest, dict]]):
                 The request object. Request message for the ListDatabases
                 method.
             parent (:class:`str`):
                 Required. The parent, which owns this collection of
                 databases. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}
 
@@ -1178,15 +1178,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1alpha1.services.metastore_service.pagers.ListDatabasesAsyncPager:
+            google.cloud.bigquery_biglake_v1alpha1.services.metastore_service.pagers.ListDatabasesAsyncPager:
                 Response message for the
                 ListDatabases method.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
@@ -1259,45 +1259,45 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1alpha1
+            from google.cloud import bigquery_biglake_v1alpha1
 
             async def sample_create_table():
                 # Create a client
-                client = biglake_v1alpha1.MetastoreServiceAsyncClient()
+                client = bigquery_biglake_v1alpha1.MetastoreServiceAsyncClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1alpha1.CreateTableRequest(
+                request = bigquery_biglake_v1alpha1.CreateTableRequest(
                     parent="parent_value",
                     table_id="table_id_value",
                 )
 
                 # Make the request
                 response = await client.create_table(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.biglake_v1alpha1.types.CreateTableRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_biglake_v1alpha1.types.CreateTableRequest, dict]]):
                 The request object. Request message for the CreateTable
                 method.
             parent (:class:`str`):
                 Required. The parent resource where this table will be
                 created. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            table (:class:`google.cloud.bigquery.biglake_v1alpha1.types.Table`):
+            table (:class:`google.cloud.bigquery_biglake_v1alpha1.types.Table`):
                 Required. The table to create. The ``name`` field does
                 not need to be provided for the table creation.
 
                 This corresponds to the ``table`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             table_id (:class:`str`):
@@ -1311,15 +1311,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1alpha1.types.Table:
+            google.cloud.bigquery_biglake_v1alpha1.types.Table:
                 Represents a table.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, table, table_id])
         if request is not None and has_flattened_params:
@@ -1380,33 +1380,33 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1alpha1
+            from google.cloud import bigquery_biglake_v1alpha1
 
             async def sample_delete_table():
                 # Create a client
-                client = biglake_v1alpha1.MetastoreServiceAsyncClient()
+                client = bigquery_biglake_v1alpha1.MetastoreServiceAsyncClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1alpha1.DeleteTableRequest(
+                request = bigquery_biglake_v1alpha1.DeleteTableRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 response = await client.delete_table(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.biglake_v1alpha1.types.DeleteTableRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_biglake_v1alpha1.types.DeleteTableRequest, dict]]):
                 The request object. Request message for the DeleteTable
                 method.
             name (:class:`str`):
                 Required. The name of the table to delete. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}/tables/{table_id}
 
                 This corresponds to the ``name`` field
@@ -1415,15 +1415,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1alpha1.types.Table:
+            google.cloud.bigquery_biglake_v1alpha1.types.Table:
                 Represents a table.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
@@ -1481,35 +1481,35 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1alpha1
+            from google.cloud import bigquery_biglake_v1alpha1
 
             async def sample_update_table():
                 # Create a client
-                client = biglake_v1alpha1.MetastoreServiceAsyncClient()
+                client = bigquery_biglake_v1alpha1.MetastoreServiceAsyncClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1alpha1.UpdateTableRequest(
+                request = bigquery_biglake_v1alpha1.UpdateTableRequest(
                 )
 
                 # Make the request
                 response = await client.update_table(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.biglake_v1alpha1.types.UpdateTableRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_biglake_v1alpha1.types.UpdateTableRequest, dict]]):
                 The request object. Request message for the UpdateTable
                 method.
-            table (:class:`google.cloud.bigquery.biglake_v1alpha1.types.Table`):
+            table (:class:`google.cloud.bigquery_biglake_v1alpha1.types.Table`):
                 Required. The table to update.
 
                 The table's ``name`` field is used to identify the table
                 to update. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}/tables/{table_id}
 
                 This corresponds to the ``table`` field
@@ -1529,15 +1529,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1alpha1.types.Table:
+            google.cloud.bigquery_biglake_v1alpha1.types.Table:
                 Represents a table.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([table, update_mask])
         if request is not None and has_flattened_params:
@@ -1599,34 +1599,34 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1alpha1
+            from google.cloud import bigquery_biglake_v1alpha1
 
             async def sample_rename_table():
                 # Create a client
-                client = biglake_v1alpha1.MetastoreServiceAsyncClient()
+                client = bigquery_biglake_v1alpha1.MetastoreServiceAsyncClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1alpha1.RenameTableRequest(
+                request = bigquery_biglake_v1alpha1.RenameTableRequest(
                     name="name_value",
                     new_name="new_name_value",
                 )
 
                 # Make the request
                 response = await client.rename_table(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.biglake_v1alpha1.types.RenameTableRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_biglake_v1alpha1.types.RenameTableRequest, dict]]):
                 The request object. Request message for the RenameTable
                 method in MetastoreService
             name (:class:`str`):
                 Required. The table's ``name`` field is used to identify
                 the table to rename. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}/tables/{table_id}
 
@@ -1644,15 +1644,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1alpha1.types.Table:
+            google.cloud.bigquery_biglake_v1alpha1.types.Table:
                 Represents a table.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name, new_name])
         if request is not None and has_flattened_params:
@@ -1711,33 +1711,33 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1alpha1
+            from google.cloud import bigquery_biglake_v1alpha1
 
             async def sample_get_table():
                 # Create a client
-                client = biglake_v1alpha1.MetastoreServiceAsyncClient()
+                client = bigquery_biglake_v1alpha1.MetastoreServiceAsyncClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1alpha1.GetTableRequest(
+                request = bigquery_biglake_v1alpha1.GetTableRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 response = await client.get_table(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.biglake_v1alpha1.types.GetTableRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_biglake_v1alpha1.types.GetTableRequest, dict]]):
                 The request object. Request message for the GetTable
                 method.
             name (:class:`str`):
                 Required. The name of the table to retrieve. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}/tables/{table_id}
 
                 This corresponds to the ``name`` field
@@ -1746,15 +1746,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1alpha1.types.Table:
+            google.cloud.bigquery_biglake_v1alpha1.types.Table:
                 Represents a table.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
@@ -1811,34 +1811,34 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1alpha1
+            from google.cloud import bigquery_biglake_v1alpha1
 
             async def sample_list_tables():
                 # Create a client
-                client = biglake_v1alpha1.MetastoreServiceAsyncClient()
+                client = bigquery_biglake_v1alpha1.MetastoreServiceAsyncClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1alpha1.ListTablesRequest(
+                request = bigquery_biglake_v1alpha1.ListTablesRequest(
                     parent="parent_value",
                 )
 
                 # Make the request
                 page_result = client.list_tables(request=request)
 
                 # Handle the response
                 async for response in page_result:
                     print(response)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.biglake_v1alpha1.types.ListTablesRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_biglake_v1alpha1.types.ListTablesRequest, dict]]):
                 The request object. Request message for the ListTables
                 method.
             parent (:class:`str`):
                 Required. The parent, which owns this collection of
                 tables. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}
 
@@ -1848,15 +1848,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1alpha1.services.metastore_service.pagers.ListTablesAsyncPager:
+            google.cloud.bigquery_biglake_v1alpha1.services.metastore_service.pagers.ListTablesAsyncPager:
                 Response message for the ListTables
                 method.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
@@ -1928,62 +1928,62 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1alpha1
+            from google.cloud import bigquery_biglake_v1alpha1
 
             async def sample_create_lock():
                 # Create a client
-                client = biglake_v1alpha1.MetastoreServiceAsyncClient()
+                client = bigquery_biglake_v1alpha1.MetastoreServiceAsyncClient()
 
                 # Initialize request argument(s)
-                lock = biglake_v1alpha1.Lock()
+                lock = bigquery_biglake_v1alpha1.Lock()
                 lock.table_id = "table_id_value"
 
-                request = biglake_v1alpha1.CreateLockRequest(
+                request = bigquery_biglake_v1alpha1.CreateLockRequest(
                     parent="parent_value",
                     lock=lock,
                 )
 
                 # Make the request
                 response = await client.create_lock(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.biglake_v1alpha1.types.CreateLockRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_biglake_v1alpha1.types.CreateLockRequest, dict]]):
                 The request object. Request message for the CreateLock
                 method.
             parent (:class:`str`):
                 Required. The parent resource where this lock will be
                 created. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            lock (:class:`google.cloud.bigquery.biglake_v1alpha1.types.Lock`):
+            lock (:class:`google.cloud.bigquery_biglake_v1alpha1.types.Lock`):
                 Required. The lock to create. The ``name`` field does
                 not need to be provided for the lock creation.
 
                 This corresponds to the ``lock`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1alpha1.types.Lock:
+            google.cloud.bigquery_biglake_v1alpha1.types.Lock:
                 Represents a lock.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, lock])
         if request is not None and has_flattened_params:
@@ -2042,30 +2042,30 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1alpha1
+            from google.cloud import bigquery_biglake_v1alpha1
 
             async def sample_delete_lock():
                 # Create a client
-                client = biglake_v1alpha1.MetastoreServiceAsyncClient()
+                client = bigquery_biglake_v1alpha1.MetastoreServiceAsyncClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1alpha1.DeleteLockRequest(
+                request = bigquery_biglake_v1alpha1.DeleteLockRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 await client.delete_lock(request=request)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.biglake_v1alpha1.types.DeleteLockRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_biglake_v1alpha1.types.DeleteLockRequest, dict]]):
                 The request object. Request message for the DeleteLock
                 method.
             name (:class:`str`):
                 Required. The name of the lock to delete. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}/locks/{lock_id}
 
                 This corresponds to the ``name`` field
@@ -2132,33 +2132,33 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1alpha1
+            from google.cloud import bigquery_biglake_v1alpha1
 
             async def sample_check_lock():
                 # Create a client
-                client = biglake_v1alpha1.MetastoreServiceAsyncClient()
+                client = bigquery_biglake_v1alpha1.MetastoreServiceAsyncClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1alpha1.CheckLockRequest(
+                request = bigquery_biglake_v1alpha1.CheckLockRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 response = await client.check_lock(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.biglake_v1alpha1.types.CheckLockRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_biglake_v1alpha1.types.CheckLockRequest, dict]]):
                 The request object. Request message for the CheckLock
                 method.
             name (:class:`str`):
                 Required. The name of the lock to check. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}/locks/{lock_id}
 
                 This corresponds to the ``name`` field
@@ -2167,15 +2167,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1alpha1.types.Lock:
+            google.cloud.bigquery_biglake_v1alpha1.types.Lock:
                 Represents a lock.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
@@ -2232,34 +2232,34 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1alpha1
+            from google.cloud import bigquery_biglake_v1alpha1
 
             async def sample_list_locks():
                 # Create a client
-                client = biglake_v1alpha1.MetastoreServiceAsyncClient()
+                client = bigquery_biglake_v1alpha1.MetastoreServiceAsyncClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1alpha1.ListLocksRequest(
+                request = bigquery_biglake_v1alpha1.ListLocksRequest(
                     parent="parent_value",
                 )
 
                 # Make the request
                 page_result = client.list_locks(request=request)
 
                 # Handle the response
                 async for response in page_result:
                     print(response)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.biglake_v1alpha1.types.ListLocksRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_biglake_v1alpha1.types.ListLocksRequest, dict]]):
                 The request object. Request message for the ListLocks
                 method.
             parent (:class:`str`):
                 Required. The parent, which owns this collection of
                 locks. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}
 
@@ -2269,15 +2269,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1alpha1.services.metastore_service.pagers.ListLocksAsyncPager:
+            google.cloud.bigquery_biglake_v1alpha1.services.metastore_service.pagers.ListLocksAsyncPager:
                 Response message for the ListLocks
                 method.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
```

### Comparing `google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/client.py` & `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,26 +35,26 @@
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.exceptions import MutualTLSChannelError  # type: ignore
 from google.auth.transport import mtls  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 
-from google.cloud.bigquery.biglake_v1alpha1 import gapic_version as package_version
+from google.cloud.bigquery_biglake_v1alpha1 import gapic_version as package_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.protobuf import field_mask_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 
-from google.cloud.bigquery.biglake_v1alpha1.services.metastore_service import pagers
-from google.cloud.bigquery.biglake_v1alpha1.types import metastore
+from google.cloud.bigquery_biglake_v1alpha1.services.metastore_service import pagers
+from google.cloud.bigquery_biglake_v1alpha1.types import metastore
 
 from .transports.base import DEFAULT_CLIENT_INFO, MetastoreServiceTransport
 from .transports.grpc import MetastoreServiceGrpcTransport
 from .transports.grpc_asyncio import MetastoreServiceGrpcAsyncIOTransport
 from .transports.rest import MetastoreServiceRestTransport
 
 
@@ -551,45 +551,45 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1alpha1
+            from google.cloud import bigquery_biglake_v1alpha1
 
             def sample_create_catalog():
                 # Create a client
-                client = biglake_v1alpha1.MetastoreServiceClient()
+                client = bigquery_biglake_v1alpha1.MetastoreServiceClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1alpha1.CreateCatalogRequest(
+                request = bigquery_biglake_v1alpha1.CreateCatalogRequest(
                     parent="parent_value",
                     catalog_id="catalog_id_value",
                 )
 
                 # Make the request
                 response = client.create_catalog(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.bigquery.biglake_v1alpha1.types.CreateCatalogRequest, dict]):
+            request (Union[google.cloud.bigquery_biglake_v1alpha1.types.CreateCatalogRequest, dict]):
                 The request object. Request message for the CreateCatalog
                 method.
             parent (str):
                 Required. The parent resource where this catalog will be
                 created. Format:
                 projects/{project_id_or_number}/locations/{location_id}
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            catalog (google.cloud.bigquery.biglake_v1alpha1.types.Catalog):
+            catalog (google.cloud.bigquery_biglake_v1alpha1.types.Catalog):
                 Required. The catalog to create. The ``name`` field does
                 not need to be provided.
 
                 This corresponds to the ``catalog`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             catalog_id (str):
@@ -604,15 +604,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1alpha1.types.Catalog:
+            google.cloud.bigquery_biglake_v1alpha1.types.Catalog:
                 Catalog is the container of
                 databases.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
@@ -676,33 +676,33 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1alpha1
+            from google.cloud import bigquery_biglake_v1alpha1
 
             def sample_delete_catalog():
                 # Create a client
-                client = biglake_v1alpha1.MetastoreServiceClient()
+                client = bigquery_biglake_v1alpha1.MetastoreServiceClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1alpha1.DeleteCatalogRequest(
+                request = bigquery_biglake_v1alpha1.DeleteCatalogRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 response = client.delete_catalog(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.bigquery.biglake_v1alpha1.types.DeleteCatalogRequest, dict]):
+            request (Union[google.cloud.bigquery_biglake_v1alpha1.types.DeleteCatalogRequest, dict]):
                 The request object. Request message for the DeleteCatalog
                 method.
             name (str):
                 Required. The name of the catalog to delete. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}
 
                 This corresponds to the ``name`` field
@@ -711,15 +711,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1alpha1.types.Catalog:
+            google.cloud.bigquery_biglake_v1alpha1.types.Catalog:
                 Catalog is the container of
                 databases.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
@@ -778,33 +778,33 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1alpha1
+            from google.cloud import bigquery_biglake_v1alpha1
 
             def sample_get_catalog():
                 # Create a client
-                client = biglake_v1alpha1.MetastoreServiceClient()
+                client = bigquery_biglake_v1alpha1.MetastoreServiceClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1alpha1.GetCatalogRequest(
+                request = bigquery_biglake_v1alpha1.GetCatalogRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 response = client.get_catalog(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.bigquery.biglake_v1alpha1.types.GetCatalogRequest, dict]):
+            request (Union[google.cloud.bigquery_biglake_v1alpha1.types.GetCatalogRequest, dict]):
                 The request object. Request message for the GetCatalog
                 method.
             name (str):
                 Required. The name of the catalog to retrieve. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}
 
                 This corresponds to the ``name`` field
@@ -813,15 +813,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1alpha1.types.Catalog:
+            google.cloud.bigquery_biglake_v1alpha1.types.Catalog:
                 Catalog is the container of
                 databases.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
@@ -880,34 +880,34 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1alpha1
+            from google.cloud import bigquery_biglake_v1alpha1
 
             def sample_list_catalogs():
                 # Create a client
-                client = biglake_v1alpha1.MetastoreServiceClient()
+                client = bigquery_biglake_v1alpha1.MetastoreServiceClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1alpha1.ListCatalogsRequest(
+                request = bigquery_biglake_v1alpha1.ListCatalogsRequest(
                     parent="parent_value",
                 )
 
                 # Make the request
                 page_result = client.list_catalogs(request=request)
 
                 # Handle the response
                 for response in page_result:
                     print(response)
 
         Args:
-            request (Union[google.cloud.bigquery.biglake_v1alpha1.types.ListCatalogsRequest, dict]):
+            request (Union[google.cloud.bigquery_biglake_v1alpha1.types.ListCatalogsRequest, dict]):
                 The request object. Request message for the ListCatalogs
                 method.
             parent (str):
                 Required. The parent, which owns this collection of
                 catalogs. Format:
                 projects/{project_id_or_number}/locations/{location_id}
 
@@ -917,15 +917,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1alpha1.services.metastore_service.pagers.ListCatalogsPager:
+            google.cloud.bigquery_biglake_v1alpha1.services.metastore_service.pagers.ListCatalogsPager:
                 Response message for the ListCatalogs
                 method.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
@@ -998,45 +998,45 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1alpha1
+            from google.cloud import bigquery_biglake_v1alpha1
 
             def sample_create_database():
                 # Create a client
-                client = biglake_v1alpha1.MetastoreServiceClient()
+                client = bigquery_biglake_v1alpha1.MetastoreServiceClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1alpha1.CreateDatabaseRequest(
+                request = bigquery_biglake_v1alpha1.CreateDatabaseRequest(
                     parent="parent_value",
                     database_id="database_id_value",
                 )
 
                 # Make the request
                 response = client.create_database(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.bigquery.biglake_v1alpha1.types.CreateDatabaseRequest, dict]):
+            request (Union[google.cloud.bigquery_biglake_v1alpha1.types.CreateDatabaseRequest, dict]):
                 The request object. Request message for the
                 CreateDatabase method.
             parent (str):
                 Required. The parent resource where this database will
                 be created. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            database (google.cloud.bigquery.biglake_v1alpha1.types.Database):
+            database (google.cloud.bigquery_biglake_v1alpha1.types.Database):
                 Required. The database to create. The ``name`` field
                 does not need to be provided.
 
                 This corresponds to the ``database`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             database_id (str):
@@ -1051,15 +1051,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1alpha1.types.Database:
+            google.cloud.bigquery_biglake_v1alpha1.types.Database:
                 Database is the container of tables.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, database, database_id])
         if request is not None and has_flattened_params:
@@ -1121,33 +1121,33 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1alpha1
+            from google.cloud import bigquery_biglake_v1alpha1
 
             def sample_delete_database():
                 # Create a client
-                client = biglake_v1alpha1.MetastoreServiceClient()
+                client = bigquery_biglake_v1alpha1.MetastoreServiceClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1alpha1.DeleteDatabaseRequest(
+                request = bigquery_biglake_v1alpha1.DeleteDatabaseRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 response = client.delete_database(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.bigquery.biglake_v1alpha1.types.DeleteDatabaseRequest, dict]):
+            request (Union[google.cloud.bigquery_biglake_v1alpha1.types.DeleteDatabaseRequest, dict]):
                 The request object. Request message for the
                 DeleteDatabase method.
             name (str):
                 Required. The name of the database to delete. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}
 
                 This corresponds to the ``name`` field
@@ -1156,15 +1156,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1alpha1.types.Database:
+            google.cloud.bigquery_biglake_v1alpha1.types.Database:
                 Database is the container of tables.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
@@ -1223,35 +1223,35 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1alpha1
+            from google.cloud import bigquery_biglake_v1alpha1
 
             def sample_update_database():
                 # Create a client
-                client = biglake_v1alpha1.MetastoreServiceClient()
+                client = bigquery_biglake_v1alpha1.MetastoreServiceClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1alpha1.UpdateDatabaseRequest(
+                request = bigquery_biglake_v1alpha1.UpdateDatabaseRequest(
                 )
 
                 # Make the request
                 response = client.update_database(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.bigquery.biglake_v1alpha1.types.UpdateDatabaseRequest, dict]):
+            request (Union[google.cloud.bigquery_biglake_v1alpha1.types.UpdateDatabaseRequest, dict]):
                 The request object. Request message for the
                 UpdateDatabase method.
-            database (google.cloud.bigquery.biglake_v1alpha1.types.Database):
+            database (google.cloud.bigquery_biglake_v1alpha1.types.Database):
                 Required. The database to update.
 
                 The database's ``name`` field is used to identify the
                 database to update. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}
 
                 This corresponds to the ``database`` field
@@ -1271,15 +1271,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1alpha1.types.Database:
+            google.cloud.bigquery_biglake_v1alpha1.types.Database:
                 Database is the container of tables.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([database, update_mask])
         if request is not None and has_flattened_params:
@@ -1340,33 +1340,33 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1alpha1
+            from google.cloud import bigquery_biglake_v1alpha1
 
             def sample_get_database():
                 # Create a client
-                client = biglake_v1alpha1.MetastoreServiceClient()
+                client = bigquery_biglake_v1alpha1.MetastoreServiceClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1alpha1.GetDatabaseRequest(
+                request = bigquery_biglake_v1alpha1.GetDatabaseRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 response = client.get_database(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.bigquery.biglake_v1alpha1.types.GetDatabaseRequest, dict]):
+            request (Union[google.cloud.bigquery_biglake_v1alpha1.types.GetDatabaseRequest, dict]):
                 The request object. Request message for the GetDatabase
                 method.
             name (str):
                 Required. The name of the database to retrieve. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}
 
                 This corresponds to the ``name`` field
@@ -1375,15 +1375,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1alpha1.types.Database:
+            google.cloud.bigquery_biglake_v1alpha1.types.Database:
                 Database is the container of tables.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
@@ -1440,34 +1440,34 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1alpha1
+            from google.cloud import bigquery_biglake_v1alpha1
 
             def sample_list_databases():
                 # Create a client
-                client = biglake_v1alpha1.MetastoreServiceClient()
+                client = bigquery_biglake_v1alpha1.MetastoreServiceClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1alpha1.ListDatabasesRequest(
+                request = bigquery_biglake_v1alpha1.ListDatabasesRequest(
                     parent="parent_value",
                 )
 
                 # Make the request
                 page_result = client.list_databases(request=request)
 
                 # Handle the response
                 for response in page_result:
                     print(response)
 
         Args:
-            request (Union[google.cloud.bigquery.biglake_v1alpha1.types.ListDatabasesRequest, dict]):
+            request (Union[google.cloud.bigquery_biglake_v1alpha1.types.ListDatabasesRequest, dict]):
                 The request object. Request message for the ListDatabases
                 method.
             parent (str):
                 Required. The parent, which owns this collection of
                 databases. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}
 
@@ -1477,15 +1477,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1alpha1.services.metastore_service.pagers.ListDatabasesPager:
+            google.cloud.bigquery_biglake_v1alpha1.services.metastore_service.pagers.ListDatabasesPager:
                 Response message for the
                 ListDatabases method.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
@@ -1558,45 +1558,45 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1alpha1
+            from google.cloud import bigquery_biglake_v1alpha1
 
             def sample_create_table():
                 # Create a client
-                client = biglake_v1alpha1.MetastoreServiceClient()
+                client = bigquery_biglake_v1alpha1.MetastoreServiceClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1alpha1.CreateTableRequest(
+                request = bigquery_biglake_v1alpha1.CreateTableRequest(
                     parent="parent_value",
                     table_id="table_id_value",
                 )
 
                 # Make the request
                 response = client.create_table(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.bigquery.biglake_v1alpha1.types.CreateTableRequest, dict]):
+            request (Union[google.cloud.bigquery_biglake_v1alpha1.types.CreateTableRequest, dict]):
                 The request object. Request message for the CreateTable
                 method.
             parent (str):
                 Required. The parent resource where this table will be
                 created. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            table (google.cloud.bigquery.biglake_v1alpha1.types.Table):
+            table (google.cloud.bigquery_biglake_v1alpha1.types.Table):
                 Required. The table to create. The ``name`` field does
                 not need to be provided for the table creation.
 
                 This corresponds to the ``table`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             table_id (str):
@@ -1610,15 +1610,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1alpha1.types.Table:
+            google.cloud.bigquery_biglake_v1alpha1.types.Table:
                 Represents a table.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, table, table_id])
         if request is not None and has_flattened_params:
@@ -1679,33 +1679,33 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1alpha1
+            from google.cloud import bigquery_biglake_v1alpha1
 
             def sample_delete_table():
                 # Create a client
-                client = biglake_v1alpha1.MetastoreServiceClient()
+                client = bigquery_biglake_v1alpha1.MetastoreServiceClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1alpha1.DeleteTableRequest(
+                request = bigquery_biglake_v1alpha1.DeleteTableRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 response = client.delete_table(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.bigquery.biglake_v1alpha1.types.DeleteTableRequest, dict]):
+            request (Union[google.cloud.bigquery_biglake_v1alpha1.types.DeleteTableRequest, dict]):
                 The request object. Request message for the DeleteTable
                 method.
             name (str):
                 Required. The name of the table to delete. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}/tables/{table_id}
 
                 This corresponds to the ``name`` field
@@ -1714,15 +1714,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1alpha1.types.Table:
+            google.cloud.bigquery_biglake_v1alpha1.types.Table:
                 Represents a table.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
@@ -1780,35 +1780,35 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1alpha1
+            from google.cloud import bigquery_biglake_v1alpha1
 
             def sample_update_table():
                 # Create a client
-                client = biglake_v1alpha1.MetastoreServiceClient()
+                client = bigquery_biglake_v1alpha1.MetastoreServiceClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1alpha1.UpdateTableRequest(
+                request = bigquery_biglake_v1alpha1.UpdateTableRequest(
                 )
 
                 # Make the request
                 response = client.update_table(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.bigquery.biglake_v1alpha1.types.UpdateTableRequest, dict]):
+            request (Union[google.cloud.bigquery_biglake_v1alpha1.types.UpdateTableRequest, dict]):
                 The request object. Request message for the UpdateTable
                 method.
-            table (google.cloud.bigquery.biglake_v1alpha1.types.Table):
+            table (google.cloud.bigquery_biglake_v1alpha1.types.Table):
                 Required. The table to update.
 
                 The table's ``name`` field is used to identify the table
                 to update. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}/tables/{table_id}
 
                 This corresponds to the ``table`` field
@@ -1828,15 +1828,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1alpha1.types.Table:
+            google.cloud.bigquery_biglake_v1alpha1.types.Table:
                 Represents a table.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([table, update_mask])
         if request is not None and has_flattened_params:
@@ -1898,34 +1898,34 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1alpha1
+            from google.cloud import bigquery_biglake_v1alpha1
 
             def sample_rename_table():
                 # Create a client
-                client = biglake_v1alpha1.MetastoreServiceClient()
+                client = bigquery_biglake_v1alpha1.MetastoreServiceClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1alpha1.RenameTableRequest(
+                request = bigquery_biglake_v1alpha1.RenameTableRequest(
                     name="name_value",
                     new_name="new_name_value",
                 )
 
                 # Make the request
                 response = client.rename_table(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.bigquery.biglake_v1alpha1.types.RenameTableRequest, dict]):
+            request (Union[google.cloud.bigquery_biglake_v1alpha1.types.RenameTableRequest, dict]):
                 The request object. Request message for the RenameTable
                 method in MetastoreService
             name (str):
                 Required. The table's ``name`` field is used to identify
                 the table to rename. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}/tables/{table_id}
 
@@ -1943,15 +1943,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1alpha1.types.Table:
+            google.cloud.bigquery_biglake_v1alpha1.types.Table:
                 Represents a table.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name, new_name])
         if request is not None and has_flattened_params:
@@ -2010,33 +2010,33 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1alpha1
+            from google.cloud import bigquery_biglake_v1alpha1
 
             def sample_get_table():
                 # Create a client
-                client = biglake_v1alpha1.MetastoreServiceClient()
+                client = bigquery_biglake_v1alpha1.MetastoreServiceClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1alpha1.GetTableRequest(
+                request = bigquery_biglake_v1alpha1.GetTableRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 response = client.get_table(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.bigquery.biglake_v1alpha1.types.GetTableRequest, dict]):
+            request (Union[google.cloud.bigquery_biglake_v1alpha1.types.GetTableRequest, dict]):
                 The request object. Request message for the GetTable
                 method.
             name (str):
                 Required. The name of the table to retrieve. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}/tables/{table_id}
 
                 This corresponds to the ``name`` field
@@ -2045,15 +2045,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1alpha1.types.Table:
+            google.cloud.bigquery_biglake_v1alpha1.types.Table:
                 Represents a table.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
@@ -2110,34 +2110,34 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1alpha1
+            from google.cloud import bigquery_biglake_v1alpha1
 
             def sample_list_tables():
                 # Create a client
-                client = biglake_v1alpha1.MetastoreServiceClient()
+                client = bigquery_biglake_v1alpha1.MetastoreServiceClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1alpha1.ListTablesRequest(
+                request = bigquery_biglake_v1alpha1.ListTablesRequest(
                     parent="parent_value",
                 )
 
                 # Make the request
                 page_result = client.list_tables(request=request)
 
                 # Handle the response
                 for response in page_result:
                     print(response)
 
         Args:
-            request (Union[google.cloud.bigquery.biglake_v1alpha1.types.ListTablesRequest, dict]):
+            request (Union[google.cloud.bigquery_biglake_v1alpha1.types.ListTablesRequest, dict]):
                 The request object. Request message for the ListTables
                 method.
             parent (str):
                 Required. The parent, which owns this collection of
                 tables. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}
 
@@ -2147,15 +2147,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1alpha1.services.metastore_service.pagers.ListTablesPager:
+            google.cloud.bigquery_biglake_v1alpha1.services.metastore_service.pagers.ListTablesPager:
                 Response message for the ListTables
                 method.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
@@ -2227,62 +2227,62 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1alpha1
+            from google.cloud import bigquery_biglake_v1alpha1
 
             def sample_create_lock():
                 # Create a client
-                client = biglake_v1alpha1.MetastoreServiceClient()
+                client = bigquery_biglake_v1alpha1.MetastoreServiceClient()
 
                 # Initialize request argument(s)
-                lock = biglake_v1alpha1.Lock()
+                lock = bigquery_biglake_v1alpha1.Lock()
                 lock.table_id = "table_id_value"
 
-                request = biglake_v1alpha1.CreateLockRequest(
+                request = bigquery_biglake_v1alpha1.CreateLockRequest(
                     parent="parent_value",
                     lock=lock,
                 )
 
                 # Make the request
                 response = client.create_lock(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.bigquery.biglake_v1alpha1.types.CreateLockRequest, dict]):
+            request (Union[google.cloud.bigquery_biglake_v1alpha1.types.CreateLockRequest, dict]):
                 The request object. Request message for the CreateLock
                 method.
             parent (str):
                 Required. The parent resource where this lock will be
                 created. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            lock (google.cloud.bigquery.biglake_v1alpha1.types.Lock):
+            lock (google.cloud.bigquery_biglake_v1alpha1.types.Lock):
                 Required. The lock to create. The ``name`` field does
                 not need to be provided for the lock creation.
 
                 This corresponds to the ``lock`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1alpha1.types.Lock:
+            google.cloud.bigquery_biglake_v1alpha1.types.Lock:
                 Represents a lock.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, lock])
         if request is not None and has_flattened_params:
@@ -2341,30 +2341,30 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1alpha1
+            from google.cloud import bigquery_biglake_v1alpha1
 
             def sample_delete_lock():
                 # Create a client
-                client = biglake_v1alpha1.MetastoreServiceClient()
+                client = bigquery_biglake_v1alpha1.MetastoreServiceClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1alpha1.DeleteLockRequest(
+                request = bigquery_biglake_v1alpha1.DeleteLockRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 client.delete_lock(request=request)
 
         Args:
-            request (Union[google.cloud.bigquery.biglake_v1alpha1.types.DeleteLockRequest, dict]):
+            request (Union[google.cloud.bigquery_biglake_v1alpha1.types.DeleteLockRequest, dict]):
                 The request object. Request message for the DeleteLock
                 method.
             name (str):
                 Required. The name of the lock to delete. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}/locks/{lock_id}
 
                 This corresponds to the ``name`` field
@@ -2431,33 +2431,33 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1alpha1
+            from google.cloud import bigquery_biglake_v1alpha1
 
             def sample_check_lock():
                 # Create a client
-                client = biglake_v1alpha1.MetastoreServiceClient()
+                client = bigquery_biglake_v1alpha1.MetastoreServiceClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1alpha1.CheckLockRequest(
+                request = bigquery_biglake_v1alpha1.CheckLockRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 response = client.check_lock(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.bigquery.biglake_v1alpha1.types.CheckLockRequest, dict]):
+            request (Union[google.cloud.bigquery_biglake_v1alpha1.types.CheckLockRequest, dict]):
                 The request object. Request message for the CheckLock
                 method.
             name (str):
                 Required. The name of the lock to check. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}/locks/{lock_id}
 
                 This corresponds to the ``name`` field
@@ -2466,15 +2466,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1alpha1.types.Lock:
+            google.cloud.bigquery_biglake_v1alpha1.types.Lock:
                 Represents a lock.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
@@ -2531,34 +2531,34 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import biglake_v1alpha1
+            from google.cloud import bigquery_biglake_v1alpha1
 
             def sample_list_locks():
                 # Create a client
-                client = biglake_v1alpha1.MetastoreServiceClient()
+                client = bigquery_biglake_v1alpha1.MetastoreServiceClient()
 
                 # Initialize request argument(s)
-                request = biglake_v1alpha1.ListLocksRequest(
+                request = bigquery_biglake_v1alpha1.ListLocksRequest(
                     parent="parent_value",
                 )
 
                 # Make the request
                 page_result = client.list_locks(request=request)
 
                 # Handle the response
                 for response in page_result:
                     print(response)
 
         Args:
-            request (Union[google.cloud.bigquery.biglake_v1alpha1.types.ListLocksRequest, dict]):
+            request (Union[google.cloud.bigquery_biglake_v1alpha1.types.ListLocksRequest, dict]):
                 The request object. Request message for the ListLocks
                 method.
             parent (str):
                 Required. The parent, which owns this collection of
                 locks. Format:
                 projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}
 
@@ -2568,15 +2568,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.biglake_v1alpha1.services.metastore_service.pagers.ListLocksPager:
+            google.cloud.bigquery_biglake_v1alpha1.services.metastore_service.pagers.ListLocksPager:
                 Response message for the ListLocks
                 method.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
```

### Comparing `google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/pagers.py` & `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/pagers.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,31 +20,31 @@
     Callable,
     Iterator,
     Optional,
     Sequence,
     Tuple,
 )
 
-from google.cloud.bigquery.biglake_v1alpha1.types import metastore
+from google.cloud.bigquery_biglake_v1alpha1.types import metastore
 
 
 class ListCatalogsPager:
     """A pager for iterating through ``list_catalogs`` requests.
 
     This class thinly wraps an initial
-    :class:`google.cloud.bigquery.biglake_v1alpha1.types.ListCatalogsResponse` object, and
+    :class:`google.cloud.bigquery_biglake_v1alpha1.types.ListCatalogsResponse` object, and
     provides an ``__iter__`` method to iterate through its
     ``catalogs`` field.
 
     If there are more pages, the ``__iter__`` method will make additional
     ``ListCatalogs`` requests and continue to iterate
     through the ``catalogs`` field on the
     corresponding responses.
 
-    All the usual :class:`google.cloud.bigquery.biglake_v1alpha1.types.ListCatalogsResponse`
+    All the usual :class:`google.cloud.bigquery_biglake_v1alpha1.types.ListCatalogsResponse`
     attributes are available on the pager. If multiple requests are made, only
     the most recent response is retained, and thus used for attribute lookup.
     """
 
     def __init__(
         self,
         method: Callable[..., metastore.ListCatalogsResponse],
@@ -54,17 +54,17 @@
         metadata: Sequence[Tuple[str, str]] = ()
     ):
         """Instantiate the pager.
 
         Args:
             method (Callable): The method that was originally called, and
                 which instantiated this pager.
-            request (google.cloud.bigquery.biglake_v1alpha1.types.ListCatalogsRequest):
+            request (google.cloud.bigquery_biglake_v1alpha1.types.ListCatalogsRequest):
                 The initial request object.
-            response (google.cloud.bigquery.biglake_v1alpha1.types.ListCatalogsResponse):
+            response (google.cloud.bigquery_biglake_v1alpha1.types.ListCatalogsResponse):
                 The initial response object.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         self._method = method
         self._request = metastore.ListCatalogsRequest(request)
         self._response = response
@@ -89,24 +89,24 @@
         return "{0}<{1!r}>".format(self.__class__.__name__, self._response)
 
 
 class ListCatalogsAsyncPager:
     """A pager for iterating through ``list_catalogs`` requests.
 
     This class thinly wraps an initial
-    :class:`google.cloud.bigquery.biglake_v1alpha1.types.ListCatalogsResponse` object, and
+    :class:`google.cloud.bigquery_biglake_v1alpha1.types.ListCatalogsResponse` object, and
     provides an ``__aiter__`` method to iterate through its
     ``catalogs`` field.
 
     If there are more pages, the ``__aiter__`` method will make additional
     ``ListCatalogs`` requests and continue to iterate
     through the ``catalogs`` field on the
     corresponding responses.
 
-    All the usual :class:`google.cloud.bigquery.biglake_v1alpha1.types.ListCatalogsResponse`
+    All the usual :class:`google.cloud.bigquery_biglake_v1alpha1.types.ListCatalogsResponse`
     attributes are available on the pager. If multiple requests are made, only
     the most recent response is retained, and thus used for attribute lookup.
     """
 
     def __init__(
         self,
         method: Callable[..., Awaitable[metastore.ListCatalogsResponse]],
@@ -116,17 +116,17 @@
         metadata: Sequence[Tuple[str, str]] = ()
     ):
         """Instantiates the pager.
 
         Args:
             method (Callable): The method that was originally called, and
                 which instantiated this pager.
-            request (google.cloud.bigquery.biglake_v1alpha1.types.ListCatalogsRequest):
+            request (google.cloud.bigquery_biglake_v1alpha1.types.ListCatalogsRequest):
                 The initial request object.
-            response (google.cloud.bigquery.biglake_v1alpha1.types.ListCatalogsResponse):
+            response (google.cloud.bigquery_biglake_v1alpha1.types.ListCatalogsResponse):
                 The initial response object.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         self._method = method
         self._request = metastore.ListCatalogsRequest(request)
         self._response = response
@@ -155,24 +155,24 @@
         return "{0}<{1!r}>".format(self.__class__.__name__, self._response)
 
 
 class ListDatabasesPager:
     """A pager for iterating through ``list_databases`` requests.
 
     This class thinly wraps an initial
-    :class:`google.cloud.bigquery.biglake_v1alpha1.types.ListDatabasesResponse` object, and
+    :class:`google.cloud.bigquery_biglake_v1alpha1.types.ListDatabasesResponse` object, and
     provides an ``__iter__`` method to iterate through its
     ``databases`` field.
 
     If there are more pages, the ``__iter__`` method will make additional
     ``ListDatabases`` requests and continue to iterate
     through the ``databases`` field on the
     corresponding responses.
 
-    All the usual :class:`google.cloud.bigquery.biglake_v1alpha1.types.ListDatabasesResponse`
+    All the usual :class:`google.cloud.bigquery_biglake_v1alpha1.types.ListDatabasesResponse`
     attributes are available on the pager. If multiple requests are made, only
     the most recent response is retained, and thus used for attribute lookup.
     """
 
     def __init__(
         self,
         method: Callable[..., metastore.ListDatabasesResponse],
@@ -182,17 +182,17 @@
         metadata: Sequence[Tuple[str, str]] = ()
     ):
         """Instantiate the pager.
 
         Args:
             method (Callable): The method that was originally called, and
                 which instantiated this pager.
-            request (google.cloud.bigquery.biglake_v1alpha1.types.ListDatabasesRequest):
+            request (google.cloud.bigquery_biglake_v1alpha1.types.ListDatabasesRequest):
                 The initial request object.
-            response (google.cloud.bigquery.biglake_v1alpha1.types.ListDatabasesResponse):
+            response (google.cloud.bigquery_biglake_v1alpha1.types.ListDatabasesResponse):
                 The initial response object.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         self._method = method
         self._request = metastore.ListDatabasesRequest(request)
         self._response = response
@@ -217,24 +217,24 @@
         return "{0}<{1!r}>".format(self.__class__.__name__, self._response)
 
 
 class ListDatabasesAsyncPager:
     """A pager for iterating through ``list_databases`` requests.
 
     This class thinly wraps an initial
-    :class:`google.cloud.bigquery.biglake_v1alpha1.types.ListDatabasesResponse` object, and
+    :class:`google.cloud.bigquery_biglake_v1alpha1.types.ListDatabasesResponse` object, and
     provides an ``__aiter__`` method to iterate through its
     ``databases`` field.
 
     If there are more pages, the ``__aiter__`` method will make additional
     ``ListDatabases`` requests and continue to iterate
     through the ``databases`` field on the
     corresponding responses.
 
-    All the usual :class:`google.cloud.bigquery.biglake_v1alpha1.types.ListDatabasesResponse`
+    All the usual :class:`google.cloud.bigquery_biglake_v1alpha1.types.ListDatabasesResponse`
     attributes are available on the pager. If multiple requests are made, only
     the most recent response is retained, and thus used for attribute lookup.
     """
 
     def __init__(
         self,
         method: Callable[..., Awaitable[metastore.ListDatabasesResponse]],
@@ -244,17 +244,17 @@
         metadata: Sequence[Tuple[str, str]] = ()
     ):
         """Instantiates the pager.
 
         Args:
             method (Callable): The method that was originally called, and
                 which instantiated this pager.
-            request (google.cloud.bigquery.biglake_v1alpha1.types.ListDatabasesRequest):
+            request (google.cloud.bigquery_biglake_v1alpha1.types.ListDatabasesRequest):
                 The initial request object.
-            response (google.cloud.bigquery.biglake_v1alpha1.types.ListDatabasesResponse):
+            response (google.cloud.bigquery_biglake_v1alpha1.types.ListDatabasesResponse):
                 The initial response object.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         self._method = method
         self._request = metastore.ListDatabasesRequest(request)
         self._response = response
@@ -283,24 +283,24 @@
         return "{0}<{1!r}>".format(self.__class__.__name__, self._response)
 
 
 class ListTablesPager:
     """A pager for iterating through ``list_tables`` requests.
 
     This class thinly wraps an initial
-    :class:`google.cloud.bigquery.biglake_v1alpha1.types.ListTablesResponse` object, and
+    :class:`google.cloud.bigquery_biglake_v1alpha1.types.ListTablesResponse` object, and
     provides an ``__iter__`` method to iterate through its
     ``tables`` field.
 
     If there are more pages, the ``__iter__`` method will make additional
     ``ListTables`` requests and continue to iterate
     through the ``tables`` field on the
     corresponding responses.
 
-    All the usual :class:`google.cloud.bigquery.biglake_v1alpha1.types.ListTablesResponse`
+    All the usual :class:`google.cloud.bigquery_biglake_v1alpha1.types.ListTablesResponse`
     attributes are available on the pager. If multiple requests are made, only
     the most recent response is retained, and thus used for attribute lookup.
     """
 
     def __init__(
         self,
         method: Callable[..., metastore.ListTablesResponse],
@@ -310,17 +310,17 @@
         metadata: Sequence[Tuple[str, str]] = ()
     ):
         """Instantiate the pager.
 
         Args:
             method (Callable): The method that was originally called, and
                 which instantiated this pager.
-            request (google.cloud.bigquery.biglake_v1alpha1.types.ListTablesRequest):
+            request (google.cloud.bigquery_biglake_v1alpha1.types.ListTablesRequest):
                 The initial request object.
-            response (google.cloud.bigquery.biglake_v1alpha1.types.ListTablesResponse):
+            response (google.cloud.bigquery_biglake_v1alpha1.types.ListTablesResponse):
                 The initial response object.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         self._method = method
         self._request = metastore.ListTablesRequest(request)
         self._response = response
@@ -345,24 +345,24 @@
         return "{0}<{1!r}>".format(self.__class__.__name__, self._response)
 
 
 class ListTablesAsyncPager:
     """A pager for iterating through ``list_tables`` requests.
 
     This class thinly wraps an initial
-    :class:`google.cloud.bigquery.biglake_v1alpha1.types.ListTablesResponse` object, and
+    :class:`google.cloud.bigquery_biglake_v1alpha1.types.ListTablesResponse` object, and
     provides an ``__aiter__`` method to iterate through its
     ``tables`` field.
 
     If there are more pages, the ``__aiter__`` method will make additional
     ``ListTables`` requests and continue to iterate
     through the ``tables`` field on the
     corresponding responses.
 
-    All the usual :class:`google.cloud.bigquery.biglake_v1alpha1.types.ListTablesResponse`
+    All the usual :class:`google.cloud.bigquery_biglake_v1alpha1.types.ListTablesResponse`
     attributes are available on the pager. If multiple requests are made, only
     the most recent response is retained, and thus used for attribute lookup.
     """
 
     def __init__(
         self,
         method: Callable[..., Awaitable[metastore.ListTablesResponse]],
@@ -372,17 +372,17 @@
         metadata: Sequence[Tuple[str, str]] = ()
     ):
         """Instantiates the pager.
 
         Args:
             method (Callable): The method that was originally called, and
                 which instantiated this pager.
-            request (google.cloud.bigquery.biglake_v1alpha1.types.ListTablesRequest):
+            request (google.cloud.bigquery_biglake_v1alpha1.types.ListTablesRequest):
                 The initial request object.
-            response (google.cloud.bigquery.biglake_v1alpha1.types.ListTablesResponse):
+            response (google.cloud.bigquery_biglake_v1alpha1.types.ListTablesResponse):
                 The initial response object.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         self._method = method
         self._request = metastore.ListTablesRequest(request)
         self._response = response
@@ -411,24 +411,24 @@
         return "{0}<{1!r}>".format(self.__class__.__name__, self._response)
 
 
 class ListLocksPager:
     """A pager for iterating through ``list_locks`` requests.
 
     This class thinly wraps an initial
-    :class:`google.cloud.bigquery.biglake_v1alpha1.types.ListLocksResponse` object, and
+    :class:`google.cloud.bigquery_biglake_v1alpha1.types.ListLocksResponse` object, and
     provides an ``__iter__`` method to iterate through its
     ``locks`` field.
 
     If there are more pages, the ``__iter__`` method will make additional
     ``ListLocks`` requests and continue to iterate
     through the ``locks`` field on the
     corresponding responses.
 
-    All the usual :class:`google.cloud.bigquery.biglake_v1alpha1.types.ListLocksResponse`
+    All the usual :class:`google.cloud.bigquery_biglake_v1alpha1.types.ListLocksResponse`
     attributes are available on the pager. If multiple requests are made, only
     the most recent response is retained, and thus used for attribute lookup.
     """
 
     def __init__(
         self,
         method: Callable[..., metastore.ListLocksResponse],
@@ -438,17 +438,17 @@
         metadata: Sequence[Tuple[str, str]] = ()
     ):
         """Instantiate the pager.
 
         Args:
             method (Callable): The method that was originally called, and
                 which instantiated this pager.
-            request (google.cloud.bigquery.biglake_v1alpha1.types.ListLocksRequest):
+            request (google.cloud.bigquery_biglake_v1alpha1.types.ListLocksRequest):
                 The initial request object.
-            response (google.cloud.bigquery.biglake_v1alpha1.types.ListLocksResponse):
+            response (google.cloud.bigquery_biglake_v1alpha1.types.ListLocksResponse):
                 The initial response object.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         self._method = method
         self._request = metastore.ListLocksRequest(request)
         self._response = response
@@ -473,24 +473,24 @@
         return "{0}<{1!r}>".format(self.__class__.__name__, self._response)
 
 
 class ListLocksAsyncPager:
     """A pager for iterating through ``list_locks`` requests.
 
     This class thinly wraps an initial
-    :class:`google.cloud.bigquery.biglake_v1alpha1.types.ListLocksResponse` object, and
+    :class:`google.cloud.bigquery_biglake_v1alpha1.types.ListLocksResponse` object, and
     provides an ``__aiter__`` method to iterate through its
     ``locks`` field.
 
     If there are more pages, the ``__aiter__`` method will make additional
     ``ListLocks`` requests and continue to iterate
     through the ``locks`` field on the
     corresponding responses.
 
-    All the usual :class:`google.cloud.bigquery.biglake_v1alpha1.types.ListLocksResponse`
+    All the usual :class:`google.cloud.bigquery_biglake_v1alpha1.types.ListLocksResponse`
     attributes are available on the pager. If multiple requests are made, only
     the most recent response is retained, and thus used for attribute lookup.
     """
 
     def __init__(
         self,
         method: Callable[..., Awaitable[metastore.ListLocksResponse]],
@@ -500,17 +500,17 @@
         metadata: Sequence[Tuple[str, str]] = ()
     ):
         """Instantiates the pager.
 
         Args:
             method (Callable): The method that was originally called, and
                 which instantiated this pager.
-            request (google.cloud.bigquery.biglake_v1alpha1.types.ListLocksRequest):
+            request (google.cloud.bigquery_biglake_v1alpha1.types.ListLocksRequest):
                 The initial request object.
-            response (google.cloud.bigquery.biglake_v1alpha1.types.ListLocksResponse):
+            response (google.cloud.bigquery_biglake_v1alpha1.types.ListLocksResponse):
                 The initial response object.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         self._method = method
         self._request = metastore.ListLocksRequest(request)
         self._response = response
```

### Comparing `google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/transports/__init__.py` & `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/transports/base.py` & `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/transports/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 from google.protobuf import empty_pb2  # type: ignore
 
-from google.cloud.bigquery.biglake_v1alpha1 import gapic_version as package_version
-from google.cloud.bigquery.biglake_v1alpha1.types import metastore
+from google.cloud.bigquery_biglake_v1alpha1 import gapic_version as package_version
+from google.cloud.bigquery_biglake_v1alpha1.types import metastore
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
     gapic_version=package_version.__version__
 )
 
 
 class MetastoreServiceTransport(abc.ABC):
```

### Comparing `google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/transports/grpc.py` & `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/transports/grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from google.api_core import gapic_v1, grpc_helpers
 import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.protobuf import empty_pb2  # type: ignore
 import grpc  # type: ignore
 
-from google.cloud.bigquery.biglake_v1alpha1.types import metastore
+from google.cloud.bigquery_biglake_v1alpha1.types import metastore
 
 from .base import DEFAULT_CLIENT_INFO, MetastoreServiceTransport
 
 
 class MetastoreServiceGrpcTransport(MetastoreServiceTransport):
     """gRPC backend transport for MetastoreService.
```

### Comparing `google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/transports/grpc_asyncio.py` & `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/transports/grpc_asyncio.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from google.api_core import gapic_v1, grpc_helpers_async
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.protobuf import empty_pb2  # type: ignore
 import grpc  # type: ignore
 from grpc.experimental import aio  # type: ignore
 
-from google.cloud.bigquery.biglake_v1alpha1.types import metastore
+from google.cloud.bigquery_biglake_v1alpha1.types import metastore
 
 from .base import DEFAULT_CLIENT_INFO, MetastoreServiceTransport
 from .grpc import MetastoreServiceGrpcTransport
 
 
 class MetastoreServiceGrpcAsyncIOTransport(MetastoreServiceTransport):
     """gRPC AsyncIO backend transport for MetastoreService.
```

### Comparing `google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/transports/rest.py` & `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 
 from google.protobuf import empty_pb2  # type: ignore
 
-from google.cloud.bigquery.biglake_v1alpha1.types import metastore
+from google.cloud.bigquery_biglake_v1alpha1.types import metastore
 
 from .base import DEFAULT_CLIENT_INFO as BASE_DEFAULT_CLIENT_INFO
 from .base import MetastoreServiceTransport
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
     gapic_version=BASE_DEFAULT_CLIENT_INFO.gapic_version,
     grpc_version=None,
```

### Comparing `google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/types/__init__.py` & `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/types/metastore.py` & `google-cloud-bigquery-biglake-0.4.0/google/cloud/bigquery_biglake_v1alpha1/types/metastore.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 
 class Database(proto.Message):
     r"""Database is the container of tables.
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
     Attributes:
-        hive_options (google.cloud.bigquery.biglake_v1alpha1.types.HiveDatabaseOptions):
+        hive_options (google.cloud.bigquery_biglake_v1alpha1.types.HiveDatabaseOptions):
             Options of a Hive database.
 
             This field is a member of `oneof`_ ``options``.
         name (str):
             Output only. The resource name. Format:
             projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}
         create_time (google.protobuf.timestamp_pb2.Timestamp):
@@ -148,15 +148,15 @@
             Output only. The deletion time of the
             database. Only set after the database is
             deleted.
         expire_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. The time when this database is
             considered expired. Only set after the database
             is deleted.
-        type_ (google.cloud.bigquery.biglake_v1alpha1.types.Database.Type):
+        type_ (google.cloud.bigquery_biglake_v1alpha1.types.Database.Type):
             The database type.
     """
 
     class Type(proto.Enum):
         r"""The database type.
 
         Values:
@@ -208,15 +208,15 @@
 
 class Table(proto.Message):
     r"""Represents a table.
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
     Attributes:
-        hive_options (google.cloud.bigquery.biglake_v1alpha1.types.HiveTableOptions):
+        hive_options (google.cloud.bigquery_biglake_v1alpha1.types.HiveTableOptions):
             Options of a Hive table.
 
             This field is a member of `oneof`_ ``options``.
         name (str):
             Output only. The resource name. Format:
             projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}/tables/{table_id}
         create_time (google.protobuf.timestamp_pb2.Timestamp):
@@ -227,15 +227,15 @@
         delete_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. The deletion time of the table.
             Only set after the table is deleted.
         expire_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. The time when this table is
             considered expired. Only set after the table is
             deleted.
-        type_ (google.cloud.bigquery.biglake_v1alpha1.types.Table.Type):
+        type_ (google.cloud.bigquery_biglake_v1alpha1.types.Table.Type):
             The table type.
         etag (str):
             The checksum of a table object computed by
             the server based on the value of other fields.
             It may be sent on update requests to ensure the
             client has an up-to-date value before
             proceeding. It is only checked for update table
@@ -309,17 +309,17 @@
 
             This field is a member of `oneof`_ ``resources``.
         name (str):
             Output only. The resource name. Format:
             projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}/locks/{lock_id}
         create_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. The creation time of the lock.
-        type_ (google.cloud.bigquery.biglake_v1alpha1.types.Lock.Type):
+        type_ (google.cloud.bigquery_biglake_v1alpha1.types.Lock.Type):
             The lock type.
-        state (google.cloud.bigquery.biglake_v1alpha1.types.Lock.State):
+        state (google.cloud.bigquery_biglake_v1alpha1.types.Lock.State):
             Output only. The lock state.
     """
 
     class Type(proto.Enum):
         r"""The lock type.
 
         Values:
@@ -377,15 +377,15 @@
     r"""Request message for the CreateCatalog method.
 
     Attributes:
         parent (str):
             Required. The parent resource where this catalog will be
             created. Format:
             projects/{project_id_or_number}/locations/{location_id}
-        catalog (google.cloud.bigquery.biglake_v1alpha1.types.Catalog):
+        catalog (google.cloud.bigquery_biglake_v1alpha1.types.Catalog):
             Required. The catalog to create. The ``name`` field does not
             need to be provided.
         catalog_id (str):
             Required. The ID to use for the catalog,
             which will become the final component of the
             catalog's resource name.
     """
@@ -472,15 +472,15 @@
     )
 
 
 class ListCatalogsResponse(proto.Message):
     r"""Response message for the ListCatalogs method.
 
     Attributes:
-        catalogs (MutableSequence[google.cloud.bigquery.biglake_v1alpha1.types.Catalog]):
+        catalogs (MutableSequence[google.cloud.bigquery_biglake_v1alpha1.types.Catalog]):
             The catalogs from the specified project.
         next_page_token (str):
             A token, which can be sent as ``page_token`` to retrieve the
             next page. If this field is omitted, there are no subsequent
             pages.
     """
 
@@ -503,15 +503,15 @@
     r"""Request message for the CreateDatabase method.
 
     Attributes:
         parent (str):
             Required. The parent resource where this database will be
             created. Format:
             projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}
-        database (google.cloud.bigquery.biglake_v1alpha1.types.Database):
+        database (google.cloud.bigquery_biglake_v1alpha1.types.Database):
             Required. The database to create. The ``name`` field does
             not need to be provided.
         database_id (str):
             Required. The ID to use for the database,
             which will become the final component of the
             database's resource name.
     """
@@ -546,15 +546,15 @@
     )
 
 
 class UpdateDatabaseRequest(proto.Message):
     r"""Request message for the UpdateDatabase method.
 
     Attributes:
-        database (google.cloud.bigquery.biglake_v1alpha1.types.Database):
+        database (google.cloud.bigquery_biglake_v1alpha1.types.Database):
             Required. The database to update.
 
             The database's ``name`` field is used to identify the
             database to update. Format:
             projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}
         update_mask (google.protobuf.field_mask_pb2.FieldMask):
             The list of fields to update.
@@ -629,15 +629,15 @@
     )
 
 
 class ListDatabasesResponse(proto.Message):
     r"""Response message for the ListDatabases method.
 
     Attributes:
-        databases (MutableSequence[google.cloud.bigquery.biglake_v1alpha1.types.Database]):
+        databases (MutableSequence[google.cloud.bigquery_biglake_v1alpha1.types.Database]):
             The databases from the specified catalog.
         next_page_token (str):
             A token, which can be sent as ``page_token`` to retrieve the
             next page. If this field is omitted, there are no subsequent
             pages.
     """
 
@@ -660,15 +660,15 @@
     r"""Request message for the CreateTable method.
 
     Attributes:
         parent (str):
             Required. The parent resource where this table will be
             created. Format:
             projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}
-        table (google.cloud.bigquery.biglake_v1alpha1.types.Table):
+        table (google.cloud.bigquery_biglake_v1alpha1.types.Table):
             Required. The table to create. The ``name`` field does not
             need to be provided for the table creation.
         table_id (str):
             Required. The ID to use for the table, which
             will become the final component of the table's
             resource name.
     """
@@ -703,15 +703,15 @@
     )
 
 
 class UpdateTableRequest(proto.Message):
     r"""Request message for the UpdateTable method.
 
     Attributes:
-        table (google.cloud.bigquery.biglake_v1alpha1.types.Table):
+        table (google.cloud.bigquery_biglake_v1alpha1.types.Table):
             Required. The table to update.
 
             The table's ``name`` field is used to identify the table to
             update. Format:
             projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}/tables/{table_id}
         update_mask (google.protobuf.field_mask_pb2.FieldMask):
             The list of fields to update.
@@ -791,15 +791,15 @@
         page_token (str):
             A page token, received from a previous ``ListTables`` call.
             Provide this to retrieve the subsequent page.
 
             When paginating, all other parameters provided to
             ``ListTables`` must match the call that provided the page
             token.
-        view (google.cloud.bigquery.biglake_v1alpha1.types.TableView):
+        view (google.cloud.bigquery_biglake_v1alpha1.types.TableView):
             The view for the returned tables.
     """
 
     parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
@@ -818,15 +818,15 @@
     )
 
 
 class ListTablesResponse(proto.Message):
     r"""Response message for the ListTables method.
 
     Attributes:
-        tables (MutableSequence[google.cloud.bigquery.biglake_v1alpha1.types.Table]):
+        tables (MutableSequence[google.cloud.bigquery_biglake_v1alpha1.types.Table]):
             The tables from the specified database.
         next_page_token (str):
             A token, which can be sent as ``page_token`` to retrieve the
             next page. If this field is omitted, there are no subsequent
             pages.
     """
 
@@ -849,15 +849,15 @@
     r"""Request message for the CreateLock method.
 
     Attributes:
         parent (str):
             Required. The parent resource where this lock will be
             created. Format:
             projects/{project_id_or_number}/locations/{location_id}/catalogs/{catalog_id}/databases/{database_id}
-        lock (google.cloud.bigquery.biglake_v1alpha1.types.Lock):
+        lock (google.cloud.bigquery_biglake_v1alpha1.types.Lock):
             Required. The lock to create. The ``name`` field does not
             need to be provided for the lock creation.
     """
 
     parent: str = proto.Field(
         proto.STRING,
         number=1,
@@ -936,15 +936,15 @@
     )
 
 
 class ListLocksResponse(proto.Message):
     r"""Response message for the ListLocks method.
 
     Attributes:
-        locks (MutableSequence[google.cloud.bigquery.biglake_v1alpha1.types.Lock]):
+        locks (MutableSequence[google.cloud.bigquery_biglake_v1alpha1.types.Lock]):
             The locks from the specified database.
         next_page_token (str):
             A token, which can be sent as ``page_token`` to retrieve the
             next page. If this field is omitted, there are no subsequent
             pages.
     """
 
@@ -990,15 +990,15 @@
     r"""Options of a Hive table.
 
     Attributes:
         parameters (MutableMapping[str, str]):
             Stores user supplied Hive table parameters.
         table_type (str):
             Hive table type. For example, MANAGED_TABLE, EXTERNAL_TABLE.
-        storage_descriptor (google.cloud.bigquery.biglake_v1alpha1.types.HiveTableOptions.StorageDescriptor):
+        storage_descriptor (google.cloud.bigquery_biglake_v1alpha1.types.HiveTableOptions.StorageDescriptor):
             Stores physical storage information of the
             data.
     """
 
     class SerDeInfo(proto.Message):
         r"""Serializer and deserializer information.
 
@@ -1022,15 +1022,15 @@
                 is stored, starting with "gs://".
             input_format (str):
                 The fully qualified Java class name of the
                 input format.
             output_format (str):
                 The fully qualified Java class name of the
                 output format.
-            serde_info (google.cloud.bigquery.biglake_v1alpha1.types.HiveTableOptions.SerDeInfo):
+            serde_info (google.cloud.bigquery_biglake_v1alpha1.types.HiveTableOptions.SerDeInfo):
                 Serializer and deserializer information.
         """
 
         location_uri: str = proto.Field(
             proto.STRING,
             number=1,
         )
```

### Comparing `google-cloud-bigquery-biglake-0.3.0/google_cloud_bigquery_biglake.egg-info/PKG-INFO` & `google-cloud-bigquery-biglake-0.4.0/google_cloud_bigquery_biglake.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-bigquery-biglake
-Version: 0.3.0
+Version: 0.4.0
 Summary: Google Cloud Bigquery Biglake API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-bigquery-biglake-0.3.0/google_cloud_bigquery_biglake.egg-info/SOURCES.txt` & `google-cloud-bigquery-biglake-0.4.0/google_cloud_bigquery_biglake.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 LICENSE
 MANIFEST.in
 README.rst
 setup.py
-google/cloud/bigquery/biglake/__init__.py
-google/cloud/bigquery/biglake/gapic_version.py
-google/cloud/bigquery/biglake/py.typed
-google/cloud/bigquery/biglake_v1/__init__.py
-google/cloud/bigquery/biglake_v1/gapic_metadata.json
-google/cloud/bigquery/biglake_v1/gapic_version.py
-google/cloud/bigquery/biglake_v1/py.typed
-google/cloud/bigquery/biglake_v1/services/__init__.py
-google/cloud/bigquery/biglake_v1/services/metastore_service/__init__.py
-google/cloud/bigquery/biglake_v1/services/metastore_service/async_client.py
-google/cloud/bigquery/biglake_v1/services/metastore_service/client.py
-google/cloud/bigquery/biglake_v1/services/metastore_service/pagers.py
-google/cloud/bigquery/biglake_v1/services/metastore_service/transports/__init__.py
-google/cloud/bigquery/biglake_v1/services/metastore_service/transports/base.py
-google/cloud/bigquery/biglake_v1/services/metastore_service/transports/grpc.py
-google/cloud/bigquery/biglake_v1/services/metastore_service/transports/grpc_asyncio.py
-google/cloud/bigquery/biglake_v1/services/metastore_service/transports/rest.py
-google/cloud/bigquery/biglake_v1/types/__init__.py
-google/cloud/bigquery/biglake_v1/types/metastore.py
-google/cloud/bigquery/biglake_v1alpha1/__init__.py
-google/cloud/bigquery/biglake_v1alpha1/gapic_metadata.json
-google/cloud/bigquery/biglake_v1alpha1/gapic_version.py
-google/cloud/bigquery/biglake_v1alpha1/py.typed
-google/cloud/bigquery/biglake_v1alpha1/services/__init__.py
-google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/__init__.py
-google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/async_client.py
-google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/client.py
-google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/pagers.py
-google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/transports/__init__.py
-google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/transports/base.py
-google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/transports/grpc.py
-google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/transports/grpc_asyncio.py
-google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/transports/rest.py
-google/cloud/bigquery/biglake_v1alpha1/types/__init__.py
-google/cloud/bigquery/biglake_v1alpha1/types/metastore.py
+google/cloud/bigquery_biglake/__init__.py
+google/cloud/bigquery_biglake/gapic_version.py
+google/cloud/bigquery_biglake/py.typed
+google/cloud/bigquery_biglake_v1/__init__.py
+google/cloud/bigquery_biglake_v1/gapic_metadata.json
+google/cloud/bigquery_biglake_v1/gapic_version.py
+google/cloud/bigquery_biglake_v1/py.typed
+google/cloud/bigquery_biglake_v1/services/__init__.py
+google/cloud/bigquery_biglake_v1/services/metastore_service/__init__.py
+google/cloud/bigquery_biglake_v1/services/metastore_service/async_client.py
+google/cloud/bigquery_biglake_v1/services/metastore_service/client.py
+google/cloud/bigquery_biglake_v1/services/metastore_service/pagers.py
+google/cloud/bigquery_biglake_v1/services/metastore_service/transports/__init__.py
+google/cloud/bigquery_biglake_v1/services/metastore_service/transports/base.py
+google/cloud/bigquery_biglake_v1/services/metastore_service/transports/grpc.py
+google/cloud/bigquery_biglake_v1/services/metastore_service/transports/grpc_asyncio.py
+google/cloud/bigquery_biglake_v1/services/metastore_service/transports/rest.py
+google/cloud/bigquery_biglake_v1/types/__init__.py
+google/cloud/bigquery_biglake_v1/types/metastore.py
+google/cloud/bigquery_biglake_v1alpha1/__init__.py
+google/cloud/bigquery_biglake_v1alpha1/gapic_metadata.json
+google/cloud/bigquery_biglake_v1alpha1/gapic_version.py
+google/cloud/bigquery_biglake_v1alpha1/py.typed
+google/cloud/bigquery_biglake_v1alpha1/services/__init__.py
+google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/__init__.py
+google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/async_client.py
+google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/client.py
+google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/pagers.py
+google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/transports/__init__.py
+google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/transports/base.py
+google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/transports/grpc.py
+google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/transports/grpc_asyncio.py
+google/cloud/bigquery_biglake_v1alpha1/services/metastore_service/transports/rest.py
+google/cloud/bigquery_biglake_v1alpha1/types/__init__.py
+google/cloud/bigquery_biglake_v1alpha1/types/metastore.py
 google_cloud_bigquery_biglake.egg-info/PKG-INFO
 google_cloud_bigquery_biglake.egg-info/SOURCES.txt
 google_cloud_bigquery_biglake.egg-info/dependency_links.txt
 google_cloud_bigquery_biglake.egg-info/namespace_packages.txt
 google_cloud_bigquery_biglake.egg-info/not-zip-safe
 google_cloud_bigquery_biglake.egg-info/requires.txt
 google_cloud_bigquery_biglake.egg-info/top_level.txt
 tests/__init__.py
 tests/unit/__init__.py
 tests/unit/gapic/__init__.py
-tests/unit/gapic/biglake_v1/__init__.py
-tests/unit/gapic/biglake_v1/test_metastore_service.py
-tests/unit/gapic/biglake_v1alpha1/__init__.py
-tests/unit/gapic/biglake_v1alpha1/test_metastore_service.py
+tests/unit/gapic/bigquery_biglake_v1/__init__.py
+tests/unit/gapic/bigquery_biglake_v1/test_metastore_service.py
+tests/unit/gapic/bigquery_biglake_v1alpha1/__init__.py
+tests/unit/gapic/bigquery_biglake_v1alpha1/test_metastore_service.py
```

### Comparing `google-cloud-bigquery-biglake-0.3.0/setup.py` & `google-cloud-bigquery-biglake-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 name = "google-cloud-bigquery-biglake"
 
 
 description = "Google Cloud Bigquery Biglake API client library"
 
 version = {}
 with open(
-    os.path.join(package_root, "google/cloud/bigquery/biglake/gapic_version.py")
+    os.path.join(package_root, "google/cloud/bigquery_biglake/gapic_version.py")
 ) as fp:
     exec(fp.read(), version)
 version = version["__version__"]
 
 if version[0] == "0":
     release_status = "Development Status :: 4 - Beta"
 else:
@@ -53,15 +53,15 @@
 
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

### Comparing `google-cloud-bigquery-biglake-0.3.0/tests/__init__.py` & `google-cloud-bigquery-biglake-0.4.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.3.0/tests/unit/__init__.py` & `google-cloud-bigquery-biglake-0.4.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.3.0/tests/unit/gapic/__init__.py` & `google-cloud-bigquery-biglake-0.4.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.3.0/tests/unit/gapic/biglake_v1/__init__.py` & `google-cloud-bigquery-biglake-0.4.0/tests/unit/gapic/bigquery_biglake_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.3.0/tests/unit/gapic/biglake_v1/test_metastore_service.py` & `google-cloud-bigquery-biglake-0.4.0/tests/unit/gapic/bigquery_biglake_v1/test_metastore_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,21 +40,21 @@
 from grpc.experimental import aio
 from proto.marshal.rules import wrappers
 from proto.marshal.rules.dates import DurationRule, TimestampRule
 import pytest
 from requests import PreparedRequest, Request, Response
 from requests.sessions import Session
 
-from google.cloud.bigquery.biglake_v1.services.metastore_service import (
+from google.cloud.bigquery_biglake_v1.services.metastore_service import (
     MetastoreServiceAsyncClient,
     MetastoreServiceClient,
     pagers,
     transports,
 )
-from google.cloud.bigquery.biglake_v1.types import metastore
+from google.cloud.bigquery_biglake_v1.types import metastore
 
 
 def client_cert_source_callback():
     return b"cert bytes", b"key bytes"
 
 
 # If default endpoint is localhost, then default mtls endpoint will be the same.
@@ -644,15 +644,15 @@
             always_use_jwt_access=True,
             api_audience=None,
         )
 
 
 def test_metastore_service_client_client_options_from_dict():
     with mock.patch(
-        "google.cloud.bigquery.biglake_v1.services.metastore_service.transports.MetastoreServiceGrpcTransport.__init__"
+        "google.cloud.bigquery_biglake_v1.services.metastore_service.transports.MetastoreServiceGrpcTransport.__init__"
     ) as grpc_transport:
         grpc_transport.return_value = None
         client = MetastoreServiceClient(
             client_options={"api_endpoint": "squid.clam.whelk"}
         )
         grpc_transport.assert_called_once_with(
             credentials=None,
@@ -9678,15 +9678,15 @@
             credentials_file="credentials.json",
         )
 
 
 def test_metastore_service_base_transport():
     # Instantiate the base transport.
     with mock.patch(
-        "google.cloud.bigquery.biglake_v1.services.metastore_service.transports.MetastoreServiceTransport.__init__"
+        "google.cloud.bigquery_biglake_v1.services.metastore_service.transports.MetastoreServiceTransport.__init__"
     ) as Transport:
         Transport.return_value = None
         transport = transports.MetastoreServiceTransport(
             credentials=ga_credentials.AnonymousCredentials(),
         )
 
     # Every method on the transport should just blindly
@@ -9725,15 +9725,15 @@
 
 
 def test_metastore_service_base_transport_with_credentials_file():
     # Instantiate the base transport with a credentials file
     with mock.patch.object(
         google.auth, "load_credentials_from_file", autospec=True
     ) as load_creds, mock.patch(
-        "google.cloud.bigquery.biglake_v1.services.metastore_service.transports.MetastoreServiceTransport._prep_wrapped_messages"
+        "google.cloud.bigquery_biglake_v1.services.metastore_service.transports.MetastoreServiceTransport._prep_wrapped_messages"
     ) as Transport:
         Transport.return_value = None
         load_creds.return_value = (ga_credentials.AnonymousCredentials(), None)
         transport = transports.MetastoreServiceTransport(
             credentials_file="credentials.json",
             quota_project_id="octopus",
         )
@@ -9747,15 +9747,15 @@
             quota_project_id="octopus",
         )
 
 
 def test_metastore_service_base_transport_with_adc():
     # Test the default credentials are used if credentials and credentials_file are None.
     with mock.patch.object(google.auth, "default", autospec=True) as adc, mock.patch(
-        "google.cloud.bigquery.biglake_v1.services.metastore_service.transports.MetastoreServiceTransport._prep_wrapped_messages"
+        "google.cloud.bigquery_biglake_v1.services.metastore_service.transports.MetastoreServiceTransport._prep_wrapped_messages"
     ) as Transport:
         Transport.return_value = None
         adc.return_value = (ga_credentials.AnonymousCredentials(), None)
         transport = transports.MetastoreServiceTransport()
         adc.assert_called_once()
```

### Comparing `google-cloud-bigquery-biglake-0.3.0/tests/unit/gapic/biglake_v1alpha1/__init__.py` & `google-cloud-bigquery-biglake-0.4.0/tests/unit/gapic/bigquery_biglake_v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.3.0/tests/unit/gapic/biglake_v1alpha1/test_metastore_service.py` & `google-cloud-bigquery-biglake-0.4.0/tests/unit/gapic/bigquery_biglake_v1alpha1/test_metastore_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,21 +40,21 @@
 from grpc.experimental import aio
 from proto.marshal.rules import wrappers
 from proto.marshal.rules.dates import DurationRule, TimestampRule
 import pytest
 from requests import PreparedRequest, Request, Response
 from requests.sessions import Session
 
-from google.cloud.bigquery.biglake_v1alpha1.services.metastore_service import (
+from google.cloud.bigquery_biglake_v1alpha1.services.metastore_service import (
     MetastoreServiceAsyncClient,
     MetastoreServiceClient,
     pagers,
     transports,
 )
-from google.cloud.bigquery.biglake_v1alpha1.types import metastore
+from google.cloud.bigquery_biglake_v1alpha1.types import metastore
 
 
 def client_cert_source_callback():
     return b"cert bytes", b"key bytes"
 
 
 # If default endpoint is localhost, then default mtls endpoint will be the same.
@@ -644,15 +644,15 @@
             always_use_jwt_access=True,
             api_audience=None,
         )
 
 
 def test_metastore_service_client_client_options_from_dict():
     with mock.patch(
-        "google.cloud.bigquery.biglake_v1alpha1.services.metastore_service.transports.MetastoreServiceGrpcTransport.__init__"
+        "google.cloud.bigquery_biglake_v1alpha1.services.metastore_service.transports.MetastoreServiceGrpcTransport.__init__"
     ) as grpc_transport:
         grpc_transport.return_value = None
         client = MetastoreServiceClient(
             client_options={"api_endpoint": "squid.clam.whelk"}
         )
         grpc_transport.assert_called_once_with(
             credentials=None,
@@ -11975,15 +11975,15 @@
             credentials_file="credentials.json",
         )
 
 
 def test_metastore_service_base_transport():
     # Instantiate the base transport.
     with mock.patch(
-        "google.cloud.bigquery.biglake_v1alpha1.services.metastore_service.transports.MetastoreServiceTransport.__init__"
+        "google.cloud.bigquery_biglake_v1alpha1.services.metastore_service.transports.MetastoreServiceTransport.__init__"
     ) as Transport:
         Transport.return_value = None
         transport = transports.MetastoreServiceTransport(
             credentials=ga_credentials.AnonymousCredentials(),
         )
 
     # Every method on the transport should just blindly
@@ -12026,15 +12026,15 @@
 
 
 def test_metastore_service_base_transport_with_credentials_file():
     # Instantiate the base transport with a credentials file
     with mock.patch.object(
         google.auth, "load_credentials_from_file", autospec=True
     ) as load_creds, mock.patch(
-        "google.cloud.bigquery.biglake_v1alpha1.services.metastore_service.transports.MetastoreServiceTransport._prep_wrapped_messages"
+        "google.cloud.bigquery_biglake_v1alpha1.services.metastore_service.transports.MetastoreServiceTransport._prep_wrapped_messages"
     ) as Transport:
         Transport.return_value = None
         load_creds.return_value = (ga_credentials.AnonymousCredentials(), None)
         transport = transports.MetastoreServiceTransport(
             credentials_file="credentials.json",
             quota_project_id="octopus",
         )
@@ -12048,15 +12048,15 @@
             quota_project_id="octopus",
         )
 
 
 def test_metastore_service_base_transport_with_adc():
     # Test the default credentials are used if credentials and credentials_file are None.
     with mock.patch.object(google.auth, "default", autospec=True) as adc, mock.patch(
-        "google.cloud.bigquery.biglake_v1alpha1.services.metastore_service.transports.MetastoreServiceTransport._prep_wrapped_messages"
+        "google.cloud.bigquery_biglake_v1alpha1.services.metastore_service.transports.MetastoreServiceTransport._prep_wrapped_messages"
     ) as Transport:
         Transport.return_value = None
         adc.return_value = (ga_credentials.AnonymousCredentials(), None)
         transport = transports.MetastoreServiceTransport()
         adc.assert_called_once()
```

