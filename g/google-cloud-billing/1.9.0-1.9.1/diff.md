# Comparing `tmp/google-cloud-billing-1.9.0.tar.gz` & `tmp/google-cloud-billing-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-billing-1.9.0.tar", last modified: Wed Jan 11 15:55:39 2023, max compression
+gzip compressed data, was "google-cloud-billing-1.9.1.tar", last modified: Mon Jan 23 16:17:07 2023, max compression
```

## Comparing `google-cloud-billing-1.9.0.tar` & `google-cloud-billing-1.9.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:55:39.220684 google-cloud-billing-1.9.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-01-11 15:52:01.000000 google-cloud-billing-1.9.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-01-11 15:52:01.000000 google-cloud-billing-1.9.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4549 2023-01-11 15:55:39.220684 google-cloud-billing-1.9.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3633 2023-01-11 15:52:01.000000 google-cloud-billing-1.9.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:55:39.208683 google-cloud-billing-1.9.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:55:39.208683 google-cloud-billing-1.9.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:55:39.212683 google-cloud-billing-1.9.0/google/cloud/billing/
--rw-rw-r--   0 root         (0)     1003     2494 2023-01-11 15:52:01.000000 google-cloud-billing-1.9.0/google/cloud/billing/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-01-11 15:52:01.000000 google-cloud-billing-1.9.0/google/cloud/billing/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       81 2023-01-11 15:52:01.000000 google-cloud-billing-1.9.0/google/cloud/billing/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:55:39.212683 google-cloud-billing-1.9.0/google/cloud/billing_v1/
--rw-rw-r--   0 root         (0)     1003     2228 2023-01-11 15:52:01.000000 google-cloud-billing-1.9.0/google/cloud/billing_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     3973 2023-01-11 15:52:01.000000 google-cloud-billing-1.9.0/google/cloud/billing_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-01-11 15:52:01.000000 google-cloud-billing-1.9.0/google/cloud/billing_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       81 2023-01-11 15:52:01.000000 google-cloud-billing-1.9.0/google/cloud/billing_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:55:39.212683 google-cloud-billing-1.9.0/google/cloud/billing_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-11 15:52:01.000000 google-cloud-billing-1.9.0/google/cloud/billing_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:55:39.216683 google-cloud-billing-1.9.0/google/cloud/billing_v1/services/cloud_billing/
--rw-rw-r--   0 root         (0)     1003      761 2023-01-11 15:52:01.000000 google-cloud-billing-1.9.0/google/cloud/billing_v1/services/cloud_billing/__init__.py
--rw-rw-r--   0 root         (0)     1003    67354 2023-01-11 15:52:01.000000 google-cloud-billing-1.9.0/google/cloud/billing_v1/services/cloud_billing/async_client.py
--rw-rw-r--   0 root         (0)     1003    73536 2023-01-11 15:52:01.000000 google-cloud-billing-1.9.0/google/cloud/billing_v1/services/cloud_billing/client.py
--rw-rw-r--   0 root         (0)     1003    11291 2023-01-11 15:52:01.000000 google-cloud-billing-1.9.0/google/cloud/billing_v1/services/cloud_billing/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:55:39.216683 google-cloud-billing-1.9.0/google/cloud/billing_v1/services/cloud_billing/transports/
--rw-rw-r--   0 root         (0)     1003     1175 2023-01-11 15:52:01.000000 google-cloud-billing-1.9.0/google/cloud/billing_v1/services/cloud_billing/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    14313 2023-01-11 15:52:01.000000 google-cloud-billing-1.9.0/google/cloud/billing_v1/services/cloud_billing/transports/base.py
--rw-rw-r--   0 root         (0)     1003    27382 2023-01-11 15:52:01.000000 google-cloud-billing-1.9.0/google/cloud/billing_v1/services/cloud_billing/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    27819 2023-01-11 15:52:01.000000 google-cloud-billing-1.9.0/google/cloud/billing_v1/services/cloud_billing/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:55:39.216683 google-cloud-billing-1.9.0/google/cloud/billing_v1/services/cloud_catalog/
--rw-rw-r--   0 root         (0)     1003      761 2023-01-11 15:52:01.000000 google-cloud-billing-1.9.0/google/cloud/billing_v1/services/cloud_catalog/__init__.py
--rw-rw-r--   0 root         (0)     1003    17110 2023-01-11 15:52:01.000000 google-cloud-billing-1.9.0/google/cloud/billing_v1/services/cloud_catalog/async_client.py
--rw-rw-r--   0 root         (0)     1003    26415 2023-01-11 15:52:01.000000 google-cloud-billing-1.9.0/google/cloud/billing_v1/services/cloud_catalog/client.py
--rw-rw-r--   0 root         (0)     1003    10578 2023-01-11 15:52:01.000000 google-cloud-billing-1.9.0/google/cloud/billing_v1/services/cloud_catalog/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:55:39.216683 google-cloud-billing-1.9.0/google/cloud/billing_v1/services/cloud_catalog/transports/
--rw-rw-r--   0 root         (0)     1003     1175 2023-01-11 15:52:01.000000 google-cloud-billing-1.9.0/google/cloud/billing_v1/services/cloud_catalog/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6639 2023-01-11 15:52:01.000000 google-cloud-billing-1.9.0/google/cloud/billing_v1/services/cloud_catalog/transports/base.py
--rw-rw-r--   0 root         (0)     1003    12934 2023-01-11 15:52:01.000000 google-cloud-billing-1.9.0/google/cloud/billing_v1/services/cloud_catalog/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13182 2023-01-11 15:52:01.000000 google-cloud-billing-1.9.0/google/cloud/billing_v1/services/cloud_catalog/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:55:39.216683 google-cloud-billing-1.9.0/google/cloud/billing_v1/types/
--rw-rw-r--   0 root         (0)     1003     1831 2023-01-11 15:52:01.000000 google-cloud-billing-1.9.0/google/cloud/billing_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    12080 2023-01-11 15:52:01.000000 google-cloud-billing-1.9.0/google/cloud/billing_v1/types/cloud_billing.py
--rw-rw-r--   0 root         (0)     1003    18550 2023-01-11 15:52:01.000000 google-cloud-billing-1.9.0/google/cloud/billing_v1/types/cloud_catalog.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:55:39.220684 google-cloud-billing-1.9.0/google_cloud_billing.egg-info/
--rw-r--r--   0 root         (0)     1003     4549 2023-01-11 15:55:39.000000 google-cloud-billing-1.9.0/google_cloud_billing.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2034 2023-01-11 15:55:39.000000 google-cloud-billing-1.9.0/google_cloud_billing.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-01-11 15:55:39.000000 google-cloud-billing-1.9.0/google_cloud_billing.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-01-11 15:55:39.000000 google-cloud-billing-1.9.0/google_cloud_billing.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-01-11 15:55:39.000000 google-cloud-billing-1.9.0/google_cloud_billing.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-01-11 15:55:39.000000 google-cloud-billing-1.9.0/google_cloud_billing.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-01-11 15:55:39.000000 google-cloud-billing-1.9.0/google_cloud_billing.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-01-11 15:55:39.220684 google-cloud-billing-1.9.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3022 2023-01-11 15:52:01.000000 google-cloud-billing-1.9.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:55:39.220684 google-cloud-billing-1.9.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-11 15:52:01.000000 google-cloud-billing-1.9.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:55:39.220684 google-cloud-billing-1.9.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-11 15:52:01.000000 google-cloud-billing-1.9.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:55:39.220684 google-cloud-billing-1.9.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-11 15:52:01.000000 google-cloud-billing-1.9.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:55:39.220684 google-cloud-billing-1.9.0/tests/unit/gapic/billing_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-11 15:52:01.000000 google-cloud-billing-1.9.0/tests/unit/gapic/billing_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   149893 2023-01-11 15:52:01.000000 google-cloud-billing-1.9.0/tests/unit/gapic/billing_v1/test_cloud_billing.py
--rw-rw-r--   0 root         (0)     1003    75095 2023-01-11 15:52:01.000000 google-cloud-billing-1.9.0/tests/unit/gapic/billing_v1/test_cloud_catalog.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:17:07.842662 google-cloud-billing-1.9.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-01-23 16:13:17.000000 google-cloud-billing-1.9.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-01-23 16:13:17.000000 google-cloud-billing-1.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4549 2023-01-23 16:17:07.842662 google-cloud-billing-1.9.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3633 2023-01-23 16:13:17.000000 google-cloud-billing-1.9.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:17:07.830660 google-cloud-billing-1.9.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:17:07.830660 google-cloud-billing-1.9.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:17:07.834661 google-cloud-billing-1.9.1/google/cloud/billing/
+-rw-rw-r--   0 root         (0)     1003     2494 2023-01-23 16:13:17.000000 google-cloud-billing-1.9.1/google/cloud/billing/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-01-23 16:13:17.000000 google-cloud-billing-1.9.1/google/cloud/billing/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       81 2023-01-23 16:13:17.000000 google-cloud-billing-1.9.1/google/cloud/billing/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:17:07.834661 google-cloud-billing-1.9.1/google/cloud/billing_v1/
+-rw-rw-r--   0 root         (0)     1003     2228 2023-01-23 16:13:17.000000 google-cloud-billing-1.9.1/google/cloud/billing_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3973 2023-01-23 16:13:17.000000 google-cloud-billing-1.9.1/google/cloud/billing_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-01-23 16:13:17.000000 google-cloud-billing-1.9.1/google/cloud/billing_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       81 2023-01-23 16:13:17.000000 google-cloud-billing-1.9.1/google/cloud/billing_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:17:07.834661 google-cloud-billing-1.9.1/google/cloud/billing_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:13:17.000000 google-cloud-billing-1.9.1/google/cloud/billing_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:17:07.838661 google-cloud-billing-1.9.1/google/cloud/billing_v1/services/cloud_billing/
+-rw-rw-r--   0 root         (0)     1003      761 2023-01-23 16:13:17.000000 google-cloud-billing-1.9.1/google/cloud/billing_v1/services/cloud_billing/__init__.py
+-rw-rw-r--   0 root         (0)     1003    67354 2023-01-23 16:13:17.000000 google-cloud-billing-1.9.1/google/cloud/billing_v1/services/cloud_billing/async_client.py
+-rw-rw-r--   0 root         (0)     1003    73560 2023-01-23 16:13:17.000000 google-cloud-billing-1.9.1/google/cloud/billing_v1/services/cloud_billing/client.py
+-rw-rw-r--   0 root         (0)     1003    11291 2023-01-23 16:13:17.000000 google-cloud-billing-1.9.1/google/cloud/billing_v1/services/cloud_billing/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:17:07.838661 google-cloud-billing-1.9.1/google/cloud/billing_v1/services/cloud_billing/transports/
+-rw-rw-r--   0 root         (0)     1003     1175 2023-01-23 16:13:17.000000 google-cloud-billing-1.9.1/google/cloud/billing_v1/services/cloud_billing/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    14313 2023-01-23 16:13:17.000000 google-cloud-billing-1.9.1/google/cloud/billing_v1/services/cloud_billing/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    27382 2023-01-23 16:13:17.000000 google-cloud-billing-1.9.1/google/cloud/billing_v1/services/cloud_billing/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    27819 2023-01-23 16:13:17.000000 google-cloud-billing-1.9.1/google/cloud/billing_v1/services/cloud_billing/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:17:07.838661 google-cloud-billing-1.9.1/google/cloud/billing_v1/services/cloud_catalog/
+-rw-rw-r--   0 root         (0)     1003      761 2023-01-23 16:13:17.000000 google-cloud-billing-1.9.1/google/cloud/billing_v1/services/cloud_catalog/__init__.py
+-rw-rw-r--   0 root         (0)     1003    17110 2023-01-23 16:13:17.000000 google-cloud-billing-1.9.1/google/cloud/billing_v1/services/cloud_catalog/async_client.py
+-rw-rw-r--   0 root         (0)     1003    26439 2023-01-23 16:13:17.000000 google-cloud-billing-1.9.1/google/cloud/billing_v1/services/cloud_catalog/client.py
+-rw-rw-r--   0 root         (0)     1003    10578 2023-01-23 16:13:17.000000 google-cloud-billing-1.9.1/google/cloud/billing_v1/services/cloud_catalog/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:17:07.838661 google-cloud-billing-1.9.1/google/cloud/billing_v1/services/cloud_catalog/transports/
+-rw-rw-r--   0 root         (0)     1003     1175 2023-01-23 16:13:17.000000 google-cloud-billing-1.9.1/google/cloud/billing_v1/services/cloud_catalog/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6639 2023-01-23 16:13:17.000000 google-cloud-billing-1.9.1/google/cloud/billing_v1/services/cloud_catalog/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    12934 2023-01-23 16:13:17.000000 google-cloud-billing-1.9.1/google/cloud/billing_v1/services/cloud_catalog/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13182 2023-01-23 16:13:17.000000 google-cloud-billing-1.9.1/google/cloud/billing_v1/services/cloud_catalog/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:17:07.842662 google-cloud-billing-1.9.1/google/cloud/billing_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1831 2023-01-23 16:13:17.000000 google-cloud-billing-1.9.1/google/cloud/billing_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12080 2023-01-23 16:13:17.000000 google-cloud-billing-1.9.1/google/cloud/billing_v1/types/cloud_billing.py
+-rw-rw-r--   0 root         (0)     1003    19344 2023-01-23 16:13:17.000000 google-cloud-billing-1.9.1/google/cloud/billing_v1/types/cloud_catalog.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:17:07.842662 google-cloud-billing-1.9.1/google_cloud_billing.egg-info/
+-rw-r--r--   0 root         (0)     1003     4549 2023-01-23 16:17:07.000000 google-cloud-billing-1.9.1/google_cloud_billing.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2034 2023-01-23 16:17:07.000000 google-cloud-billing-1.9.1/google_cloud_billing.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-01-23 16:17:07.000000 google-cloud-billing-1.9.1/google_cloud_billing.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-01-23 16:17:07.000000 google-cloud-billing-1.9.1/google_cloud_billing.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-01-23 16:17:07.000000 google-cloud-billing-1.9.1/google_cloud_billing.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-01-23 16:17:07.000000 google-cloud-billing-1.9.1/google_cloud_billing.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-01-23 16:17:07.000000 google-cloud-billing-1.9.1/google_cloud_billing.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-01-23 16:17:07.846662 google-cloud-billing-1.9.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3022 2023-01-23 16:13:17.000000 google-cloud-billing-1.9.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:17:07.842662 google-cloud-billing-1.9.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:13:17.000000 google-cloud-billing-1.9.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:17:07.842662 google-cloud-billing-1.9.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:13:17.000000 google-cloud-billing-1.9.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:17:07.842662 google-cloud-billing-1.9.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:13:17.000000 google-cloud-billing-1.9.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:17:07.842662 google-cloud-billing-1.9.1/tests/unit/gapic/billing_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:13:17.000000 google-cloud-billing-1.9.1/tests/unit/gapic/billing_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   149893 2023-01-23 16:13:17.000000 google-cloud-billing-1.9.1/tests/unit/gapic/billing_v1/test_cloud_billing.py
+-rw-rw-r--   0 root         (0)     1003    75095 2023-01-23 16:13:17.000000 google-cloud-billing-1.9.1/tests/unit/gapic/billing_v1/test_cloud_catalog.py
```

### Comparing `google-cloud-billing-1.9.0/LICENSE` & `google-cloud-billing-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-1.9.0/MANIFEST.in` & `google-cloud-billing-1.9.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-1.9.0/PKG-INFO` & `google-cloud-billing-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-billing
-Version: 1.9.0
+Version: 1.9.1
 Summary: Google Cloud Billing API client library
 Home-page: https://github.com/googleapis/python-billing
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-billing-1.9.0/README.rst` & `google-cloud-billing-1.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-1.9.0/google/cloud/billing/__init__.py` & `google-cloud-billing-1.9.1/google/cloud/billing/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-1.9.0/google/cloud/billing/gapic_version.py` & `google-cloud-billing-1.9.1/google/cloud/billing/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.9.0"  # {x-release-please-version}
+__version__ = "1.9.1"  # {x-release-please-version}
```

### Comparing `google-cloud-billing-1.9.0/google/cloud/billing_v1/__init__.py` & `google-cloud-billing-1.9.1/google/cloud/billing_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-1.9.0/google/cloud/billing_v1/gapic_metadata.json` & `google-cloud-billing-1.9.1/google/cloud/billing_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-1.9.0/google/cloud/billing_v1/gapic_version.py` & `google-cloud-billing-1.9.1/google/cloud/billing_v1/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.9.0"  # {x-release-please-version}
+__version__ = "1.9.1"  # {x-release-please-version}
```

### Comparing `google-cloud-billing-1.9.0/google/cloud/billing_v1/services/__init__.py` & `google-cloud-billing-1.9.1/google/cloud/billing_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-1.9.0/google/cloud/billing_v1/services/cloud_billing/__init__.py` & `google-cloud-billing-1.9.1/google/cloud/billing_v1/services/cloud_billing/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-1.9.0/google/cloud/billing_v1/services/cloud_billing/async_client.py` & `google-cloud-billing-1.9.1/google/cloud/billing_v1/services/cloud_billing/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-1.9.0/google/cloud/billing_v1/services/cloud_billing/client.py` & `google-cloud-billing-1.9.1/google/cloud/billing_v1/services/cloud_billing/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1697,15 +1697,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    def __enter__(self):
+    def __enter__(self) -> "CloudBillingClient":
         return self
 
     def __exit__(self, type, value, traceback):
         """Releases underlying transport's resources.
 
         .. warning::
             ONLY use as a context manager if the transport is NOT shared
```

### Comparing `google-cloud-billing-1.9.0/google/cloud/billing_v1/services/cloud_billing/pagers.py` & `google-cloud-billing-1.9.1/google/cloud/billing_v1/services/cloud_billing/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-1.9.0/google/cloud/billing_v1/services/cloud_billing/transports/__init__.py` & `google-cloud-billing-1.9.1/google/cloud/billing_v1/services/cloud_billing/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-1.9.0/google/cloud/billing_v1/services/cloud_billing/transports/base.py` & `google-cloud-billing-1.9.1/google/cloud/billing_v1/services/cloud_billing/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-1.9.0/google/cloud/billing_v1/services/cloud_billing/transports/grpc.py` & `google-cloud-billing-1.9.1/google/cloud/billing_v1/services/cloud_billing/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-1.9.0/google/cloud/billing_v1/services/cloud_billing/transports/grpc_asyncio.py` & `google-cloud-billing-1.9.1/google/cloud/billing_v1/services/cloud_billing/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-1.9.0/google/cloud/billing_v1/services/cloud_catalog/__init__.py` & `google-cloud-billing-1.9.1/google/cloud/billing_v1/services/cloud_catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-1.9.0/google/cloud/billing_v1/services/cloud_catalog/async_client.py` & `google-cloud-billing-1.9.1/google/cloud/billing_v1/services/cloud_catalog/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-1.9.0/google/cloud/billing_v1/services/cloud_catalog/client.py` & `google-cloud-billing-1.9.1/google/cloud/billing_v1/services/cloud_catalog/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -647,15 +647,15 @@
             response=response,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    def __enter__(self):
+    def __enter__(self) -> "CloudCatalogClient":
         return self
 
     def __exit__(self, type, value, traceback):
         """Releases underlying transport's resources.
 
         .. warning::
             ONLY use as a context manager if the transport is NOT shared
```

### Comparing `google-cloud-billing-1.9.0/google/cloud/billing_v1/services/cloud_catalog/pagers.py` & `google-cloud-billing-1.9.1/google/cloud/billing_v1/services/cloud_catalog/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-1.9.0/google/cloud/billing_v1/services/cloud_catalog/transports/__init__.py` & `google-cloud-billing-1.9.1/google/cloud/billing_v1/services/cloud_catalog/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-1.9.0/google/cloud/billing_v1/services/cloud_catalog/transports/base.py` & `google-cloud-billing-1.9.1/google/cloud/billing_v1/services/cloud_catalog/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-1.9.0/google/cloud/billing_v1/services/cloud_catalog/transports/grpc.py` & `google-cloud-billing-1.9.1/google/cloud/billing_v1/services/cloud_catalog/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-1.9.0/google/cloud/billing_v1/services/cloud_catalog/transports/grpc_asyncio.py` & `google-cloud-billing-1.9.1/google/cloud/billing_v1/services/cloud_catalog/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-1.9.0/google/cloud/billing_v1/types/__init__.py` & `google-cloud-billing-1.9.1/google/cloud/billing_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-1.9.0/google/cloud/billing_v1/types/cloud_billing.py` & `google-cloud-billing-1.9.1/google/cloud/billing_v1/types/cloud_billing.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-1.9.0/google/cloud/billing_v1/types/cloud_catalog.py` & `google-cloud-billing-1.9.1/google/cloud/billing_v1/types/cloud_catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -360,23 +360,39 @@
     """
 
     class AggregationLevel(proto.Enum):
         r"""The level at which usage is aggregated to compute cost.
         Example: "ACCOUNT" aggregation level indicates that usage for
         tiered pricing is aggregated across all projects in a single
         account.
+
+        Values:
+            AGGREGATION_LEVEL_UNSPECIFIED (0):
+
+            ACCOUNT (1):
+
+            PROJECT (2):
+
         """
         AGGREGATION_LEVEL_UNSPECIFIED = 0
         ACCOUNT = 1
         PROJECT = 2
 
     class AggregationInterval(proto.Enum):
         r"""The interval at which usage is aggregated to compute cost.
         Example: "MONTHLY" aggregation interval indicates that usage for
         tiered pricing is aggregated every month.
+
+        Values:
+            AGGREGATION_INTERVAL_UNSPECIFIED (0):
+
+            DAILY (1):
+
+            MONTHLY (2):
+
         """
         AGGREGATION_INTERVAL_UNSPECIFIED = 0
         DAILY = 1
         MONTHLY = 2
 
     aggregation_level: AggregationLevel = proto.Field(
         proto.ENUM,
@@ -404,15 +420,30 @@
         regions (MutableSequence[str]):
             The list of regions associated with a sku.
             Empty for Global skus, which are associated with
             all Google Cloud regions.
     """
 
     class Type(proto.Enum):
-        r"""The type of Geo Taxonomy: GLOBAL, REGIONAL, or MULTI_REGIONAL."""
+        r"""The type of Geo Taxonomy: GLOBAL, REGIONAL, or MULTI_REGIONAL.
+
+        Values:
+            TYPE_UNSPECIFIED (0):
+                The type is not specified.
+            GLOBAL (1):
+                The sku is global in nature, e.g. a license
+                sku. Global skus are available in all regions,
+                and so have an empty region list.
+            REGIONAL (2):
+                The sku is available in a specific region,
+                e.g. "us-west2".
+            MULTI_REGIONAL (3):
+                The sku is associated with multiple regions,
+                e.g. "us-west2" and "us-east1".
+        """
         TYPE_UNSPECIFIED = 0
         GLOBAL = 1
         REGIONAL = 2
         MULTI_REGIONAL = 3
 
     type_: Type = proto.Field(
         proto.ENUM,
```

### Comparing `google-cloud-billing-1.9.0/google_cloud_billing.egg-info/PKG-INFO` & `google-cloud-billing-1.9.1/google_cloud_billing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-billing
-Version: 1.9.0
+Version: 1.9.1
 Summary: Google Cloud Billing API client library
 Home-page: https://github.com/googleapis/python-billing
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-billing-1.9.0/google_cloud_billing.egg-info/SOURCES.txt` & `google-cloud-billing-1.9.1/google_cloud_billing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-1.9.0/setup.py` & `google-cloud-billing-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-1.9.0/tests/__init__.py` & `google-cloud-billing-1.9.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-1.9.0/tests/unit/__init__.py` & `google-cloud-billing-1.9.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-1.9.0/tests/unit/gapic/__init__.py` & `google-cloud-billing-1.9.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-1.9.0/tests/unit/gapic/billing_v1/__init__.py` & `google-cloud-billing-1.9.1/tests/unit/gapic/billing_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-1.9.0/tests/unit/gapic/billing_v1/test_cloud_billing.py` & `google-cloud-billing-1.9.1/tests/unit/gapic/billing_v1/test_cloud_billing.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-1.9.0/tests/unit/gapic/billing_v1/test_cloud_catalog.py` & `google-cloud-billing-1.9.1/tests/unit/gapic/billing_v1/test_cloud_catalog.py`

 * *Files identical despite different names*

