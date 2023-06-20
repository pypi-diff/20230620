# Comparing `tmp/google-cloud-bigquery-analyticshub-0.3.2.tar.gz` & `tmp/google-cloud-bigquery-analyticshub-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-bigquery-analyticshub-0.3.2.tar", last modified: Mon Mar 27 15:54:52 2023, max compression
+gzip compressed data, was "google-cloud-bigquery-analyticshub-0.4.0.tar", last modified: Tue Jun 20 13:26:56 2023, max compression
```

## Comparing `google-cloud-bigquery-analyticshub-0.3.2.tar` & `google-cloud-bigquery-analyticshub-0.4.0.tar`

### file list

```diff
@@ -1,51 +1,50 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:54:52.691237 google-cloud-bigquery-analyticshub-0.3.2/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 15:52:01.000000 google-cloud-bigquery-analyticshub-0.3.2/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 15:52:01.000000 google-cloud-bigquery-analyticshub-0.3.2/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4978 2023-03-27 15:54:52.691237 google-cloud-bigquery-analyticshub-0.3.2/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     4033 2023-03-27 15:52:01.000000 google-cloud-bigquery-analyticshub-0.3.2/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:54:52.683236 google-cloud-bigquery-analyticshub-0.3.2/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:54:52.683236 google-cloud-bigquery-analyticshub-0.3.2/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:54:52.683236 google-cloud-bigquery-analyticshub-0.3.2/google/cloud/bigquery/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:54:52.683236 google-cloud-bigquery-analyticshub-0.3.2/google/cloud/bigquery/analyticshub/
--rw-rw-r--   0 root         (0)     1003     2347 2023-03-27 15:52:01.000000 google-cloud-bigquery-analyticshub-0.3.2/google/cloud/bigquery/analyticshub/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:52:01.000000 google-cloud-bigquery-analyticshub-0.3.2/google/cloud/bigquery/analyticshub/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       95 2023-03-27 15:52:01.000000 google-cloud-bigquery-analyticshub-0.3.2/google/cloud/bigquery/analyticshub/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:54:52.683236 google-cloud-bigquery-analyticshub-0.3.2/google/cloud/bigquery/analyticshub_v1/
--rw-rw-r--   0 root         (0)     1003     2171 2023-03-27 15:52:01.000000 google-cloud-bigquery-analyticshub-0.3.2/google/cloud/bigquery/analyticshub_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     4388 2023-03-27 15:52:01.000000 google-cloud-bigquery-analyticshub-0.3.2/google/cloud/bigquery/analyticshub_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:52:01.000000 google-cloud-bigquery-analyticshub-0.3.2/google/cloud/bigquery/analyticshub_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       95 2023-03-27 15:52:01.000000 google-cloud-bigquery-analyticshub-0.3.2/google/cloud/bigquery/analyticshub_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:54:52.683236 google-cloud-bigquery-analyticshub-0.3.2/google/cloud/bigquery/analyticshub_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:52:01.000000 google-cloud-bigquery-analyticshub-0.3.2/google/cloud/bigquery/analyticshub_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:54:52.687236 google-cloud-bigquery-analyticshub-0.3.2/google/cloud/bigquery/analyticshub_v1/services/analytics_hub_service/
--rw-rw-r--   0 root         (0)     1003      789 2023-03-27 15:52:01.000000 google-cloud-bigquery-analyticshub-0.3.2/google/cloud/bigquery/analyticshub_v1/services/analytics_hub_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    81268 2023-03-27 15:52:01.000000 google-cloud-bigquery-analyticshub-0.3.2/google/cloud/bigquery/analyticshub_v1/services/analytics_hub_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    93123 2023-03-27 15:52:01.000000 google-cloud-bigquery-analyticshub-0.3.2/google/cloud/bigquery/analyticshub_v1/services/analytics_hub_service/client.py
--rw-rw-r--   0 root         (0)     1003    16387 2023-03-27 15:52:01.000000 google-cloud-bigquery-analyticshub-0.3.2/google/cloud/bigquery/analyticshub_v1/services/analytics_hub_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:54:52.687236 google-cloud-bigquery-analyticshub-0.3.2/google/cloud/bigquery/analyticshub_v1/services/analytics_hub_service/transports/
--rw-rw-r--   0 root         (0)     1003     1246 2023-03-27 15:52:01.000000 google-cloud-bigquery-analyticshub-0.3.2/google/cloud/bigquery/analyticshub_v1/services/analytics_hub_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    12705 2023-03-27 15:52:01.000000 google-cloud-bigquery-analyticshub-0.3.2/google/cloud/bigquery/analyticshub_v1/services/analytics_hub_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    28714 2023-03-27 15:52:01.000000 google-cloud-bigquery-analyticshub-0.3.2/google/cloud/bigquery/analyticshub_v1/services/analytics_hub_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    29292 2023-03-27 15:52:01.000000 google-cloud-bigquery-analyticshub-0.3.2/google/cloud/bigquery/analyticshub_v1/services/analytics_hub_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:54:52.687236 google-cloud-bigquery-analyticshub-0.3.2/google/cloud/bigquery/analyticshub_v1/types/
--rw-rw-r--   0 root         (0)     1003     1851 2023-03-27 15:52:01.000000 google-cloud-bigquery-analyticshub-0.3.2/google/cloud/bigquery/analyticshub_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    26368 2023-03-27 15:52:01.000000 google-cloud-bigquery-analyticshub-0.3.2/google/cloud/bigquery/analyticshub_v1/types/analyticshub.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:54:52.687236 google-cloud-bigquery-analyticshub-0.3.2/google_cloud_bigquery_analyticshub.egg-info/
--rw-r--r--   0 root         (0)     1003     4978 2023-03-27 15:54:52.000000 google-cloud-bigquery-analyticshub-0.3.2/google_cloud_bigquery_analyticshub.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1856 2023-03-27 15:54:52.000000 google-cloud-bigquery-analyticshub-0.3.2/google_cloud_bigquery_analyticshub.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 15:54:52.000000 google-cloud-bigquery-analyticshub-0.3.2/google_cloud_bigquery_analyticshub.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       42 2023-03-27 15:54:52.000000 google-cloud-bigquery-analyticshub-0.3.2/google_cloud_bigquery_analyticshub.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 15:54:52.000000 google-cloud-bigquery-analyticshub-0.3.2/google_cloud_bigquery_analyticshub.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-03-27 15:54:52.000000 google-cloud-bigquery-analyticshub-0.3.2/google_cloud_bigquery_analyticshub.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 15:54:52.000000 google-cloud-bigquery-analyticshub-0.3.2/google_cloud_bigquery_analyticshub.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 15:54:52.691237 google-cloud-bigquery-analyticshub-0.3.2/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3055 2023-03-27 15:52:01.000000 google-cloud-bigquery-analyticshub-0.3.2/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:54:52.687236 google-cloud-bigquery-analyticshub-0.3.2/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:52:01.000000 google-cloud-bigquery-analyticshub-0.3.2/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:54:52.687236 google-cloud-bigquery-analyticshub-0.3.2/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:52:01.000000 google-cloud-bigquery-analyticshub-0.3.2/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:54:52.691237 google-cloud-bigquery-analyticshub-0.3.2/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:52:01.000000 google-cloud-bigquery-analyticshub-0.3.2/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:54:52.691237 google-cloud-bigquery-analyticshub-0.3.2/tests/unit/gapic/analyticshub_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:52:01.000000 google-cloud-bigquery-analyticshub-0.3.2/tests/unit/gapic/analyticshub_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   206173 2023-03-27 15:52:01.000000 google-cloud-bigquery-analyticshub-0.3.2/tests/unit/gapic/analyticshub_v1/test_analytics_hub_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:26:56.120734 google-cloud-bigquery-analyticshub-0.4.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-06-20 13:23:47.000000 google-cloud-bigquery-analyticshub-0.4.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-06-20 13:23:47.000000 google-cloud-bigquery-analyticshub-0.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4933 2023-06-20 13:26:56.120734 google-cloud-bigquery-analyticshub-0.4.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3997 2023-06-20 13:23:47.000000 google-cloud-bigquery-analyticshub-0.4.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:26:56.108733 google-cloud-bigquery-analyticshub-0.4.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:26:56.112733 google-cloud-bigquery-analyticshub-0.4.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:26:56.112733 google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub/
+-rw-rw-r--   0 root         (0)     1003     2347 2023-06-20 13:23:47.000000 google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-20 13:23:47.000000 google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       95 2023-06-20 13:23:47.000000 google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:26:56.112733 google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/
+-rw-rw-r--   0 root         (0)     1003     2171 2023-06-20 13:23:47.000000 google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4388 2023-06-20 13:23:47.000000 google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-20 13:23:47.000000 google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       95 2023-06-20 13:23:47.000000 google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:26:56.112733 google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-20 13:23:47.000000 google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:26:56.116734 google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/
+-rw-rw-r--   0 root         (0)     1003      789 2023-06-20 13:23:47.000000 google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    81556 2023-06-20 13:23:47.000000 google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    93411 2023-06-20 13:23:47.000000 google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/client.py
+-rw-rw-r--   0 root         (0)     1003    16387 2023-06-20 13:23:47.000000 google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:26:56.116734 google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1246 2023-06-20 13:23:47.000000 google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12705 2023-06-20 13:23:47.000000 google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    28714 2023-06-20 13:23:47.000000 google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    29292 2023-06-20 13:23:47.000000 google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:26:56.116734 google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1851 2023-06-20 13:23:47.000000 google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    26368 2023-06-20 13:23:47.000000 google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/types/analyticshub.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:26:56.116734 google-cloud-bigquery-analyticshub-0.4.0/google_cloud_bigquery_analyticshub.egg-info/
+-rw-r--r--   0 root         (0)     1003     4933 2023-06-20 13:26:56.000000 google-cloud-bigquery-analyticshub-0.4.0/google_cloud_bigquery_analyticshub.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1874 2023-06-20 13:26:56.000000 google-cloud-bigquery-analyticshub-0.4.0/google_cloud_bigquery_analyticshub.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-06-20 13:26:56.000000 google-cloud-bigquery-analyticshub-0.4.0/google_cloud_bigquery_analyticshub.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-06-20 13:26:56.000000 google-cloud-bigquery-analyticshub-0.4.0/google_cloud_bigquery_analyticshub.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-06-20 13:26:56.000000 google-cloud-bigquery-analyticshub-0.4.0/google_cloud_bigquery_analyticshub.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-06-20 13:26:56.000000 google-cloud-bigquery-analyticshub-0.4.0/google_cloud_bigquery_analyticshub.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-06-20 13:26:56.000000 google-cloud-bigquery-analyticshub-0.4.0/google_cloud_bigquery_analyticshub.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-06-20 13:26:56.120734 google-cloud-bigquery-analyticshub-0.4.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3021 2023-06-20 13:23:47.000000 google-cloud-bigquery-analyticshub-0.4.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:26:56.116734 google-cloud-bigquery-analyticshub-0.4.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-20 13:23:47.000000 google-cloud-bigquery-analyticshub-0.4.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:26:56.116734 google-cloud-bigquery-analyticshub-0.4.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-20 13:23:47.000000 google-cloud-bigquery-analyticshub-0.4.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:26:56.116734 google-cloud-bigquery-analyticshub-0.4.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-20 13:23:47.000000 google-cloud-bigquery-analyticshub-0.4.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:26:56.120734 google-cloud-bigquery-analyticshub-0.4.0/tests/unit/gapic/bigquery_analyticshub_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-20 13:23:47.000000 google-cloud-bigquery-analyticshub-0.4.0/tests/unit/gapic/bigquery_analyticshub_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   206173 2023-06-20 13:23:47.000000 google-cloud-bigquery-analyticshub-0.4.0/tests/unit/gapic/bigquery_analyticshub_v1/test_analytics_hub_service.py
```

### Comparing `google-cloud-bigquery-analyticshub-0.3.2/LICENSE` & `google-cloud-bigquery-analyticshub-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-analyticshub-0.3.2/MANIFEST.in` & `google-cloud-bigquery-analyticshub-0.4.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-analyticshub-0.3.2/PKG-INFO` & `google-cloud-bigquery-analyticshub-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-bigquery-analyticshub
-Version: 0.3.2
+Version: 0.4.0
 Summary: Google Cloud Bigquery Analyticshub API client library
-Home-page: https://github.com/googleapis/python-bigquery-analyticshub
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
 
-Python Client for BigQuery Analytics Hub API
-============================================
+Python Client for BigQuery Analytics Hub
+========================================
 
 |preview| |pypi| |versions|
 
-`BigQuery Analytics Hub API`_: Analytics Hub is a data exchange that allows you to efficiently and securely exchange data assets across organizations to address challenges of data reliability and cost. Curate a library of internal and external assets, including unique datasets like Google Trends, backed by the power of BigQuery.
+`BigQuery Analytics Hub`_: Analytics Hub is a data exchange that allows you to efficiently and securely exchange data assets across organizations to address challenges of data reliability and cost. Curate a library of internal and external assets, including unique datasets like Google Trends, backed by the power of BigQuery.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-bigquery-analyticshub.svg
    :target: https://pypi.org/project/google-cloud-bigquery-analyticshub/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-bigquery-analyticshub.svg
    :target: https://pypi.org/project/google-cloud-bigquery-analyticshub/
-.. _BigQuery Analytics Hub API: https://cloud.google.com/analytics-hub
+.. _BigQuery Analytics Hub: https://cloud.google.com/analytics-hub
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/analyticshub/latest
 .. _Product Documentation:  https://cloud.google.com/analytics-hub
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the BigQuery Analytics Hub API.`_
+3. `Enable the BigQuery Analytics Hub.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the BigQuery Analytics Hub API.:  https://cloud.google.com/analytics-hub
+.. _Enable the BigQuery Analytics Hub.:  https://cloud.google.com/analytics-hub
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-bigquery-analyticshub
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for BigQuery Analytics Hub API
+-  Read the `Client Library Documentation`_ for BigQuery Analytics Hub
    to see other available methods on the client.
--  Read the `BigQuery Analytics Hub API Product documentation`_ to learn
+-  Read the `BigQuery Analytics Hub Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _BigQuery Analytics Hub API Product documentation:  https://cloud.google.com/analytics-hub
+.. _BigQuery Analytics Hub Product documentation:  https://cloud.google.com/analytics-hub
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-bigquery-analyticshub-0.3.2/README.rst` & `google-cloud-bigquery-analyticshub-0.4.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Python Client for BigQuery Analytics Hub API
-============================================
+Python Client for BigQuery Analytics Hub
+========================================
 
 |preview| |pypi| |versions|
 
-`BigQuery Analytics Hub API`_: Analytics Hub is a data exchange that allows you to efficiently and securely exchange data assets across organizations to address challenges of data reliability and cost. Curate a library of internal and external assets, including unique datasets like Google Trends, backed by the power of BigQuery.
+`BigQuery Analytics Hub`_: Analytics Hub is a data exchange that allows you to efficiently and securely exchange data assets across organizations to address challenges of data reliability and cost. Curate a library of internal and external assets, including unique datasets like Google Trends, backed by the power of BigQuery.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-bigquery-analyticshub.svg
    :target: https://pypi.org/project/google-cloud-bigquery-analyticshub/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-bigquery-analyticshub.svg
    :target: https://pypi.org/project/google-cloud-bigquery-analyticshub/
-.. _BigQuery Analytics Hub API: https://cloud.google.com/analytics-hub
+.. _BigQuery Analytics Hub: https://cloud.google.com/analytics-hub
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/analyticshub/latest
 .. _Product Documentation:  https://cloud.google.com/analytics-hub
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the BigQuery Analytics Hub API.`_
+3. `Enable the BigQuery Analytics Hub.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the BigQuery Analytics Hub API.:  https://cloud.google.com/analytics-hub
+.. _Enable the BigQuery Analytics Hub.:  https://cloud.google.com/analytics-hub
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -92,16 +92,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-bigquery-analyticshub
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for BigQuery Analytics Hub API
+-  Read the `Client Library Documentation`_ for BigQuery Analytics Hub
    to see other available methods on the client.
--  Read the `BigQuery Analytics Hub API Product documentation`_ to learn
+-  Read the `BigQuery Analytics Hub Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _BigQuery Analytics Hub API Product documentation:  https://cloud.google.com/analytics-hub
+.. _BigQuery Analytics Hub Product documentation:  https://cloud.google.com/analytics-hub
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-bigquery-analyticshub-0.3.2/google/cloud/bigquery/analyticshub/__init__.py` & `google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,26 +9,24 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from google.cloud.bigquery.analyticshub import gapic_version as package_version
+from google.cloud.bigquery_analyticshub_v1 import gapic_version as package_version
 
 __version__ = package_version.__version__
 
 
-from google.cloud.bigquery.analyticshub_v1.services.analytics_hub_service.async_client import (
+from .services.analytics_hub_service import (
     AnalyticsHubServiceAsyncClient,
-)
-from google.cloud.bigquery.analyticshub_v1.services.analytics_hub_service.client import (
     AnalyticsHubServiceClient,
 )
-from google.cloud.bigquery.analyticshub_v1.types.analyticshub import (
+from .types.analyticshub import (
     CreateDataExchangeRequest,
     CreateListingRequest,
     DataExchange,
     DataProvider,
     DeleteDataExchangeRequest,
     DeleteListingRequest,
     DestinationDataset,
@@ -46,32 +44,32 @@
     SubscribeListingRequest,
     SubscribeListingResponse,
     UpdateDataExchangeRequest,
     UpdateListingRequest,
 )
 
 __all__ = (
-    "AnalyticsHubServiceClient",
     "AnalyticsHubServiceAsyncClient",
+    "AnalyticsHubServiceClient",
     "CreateDataExchangeRequest",
     "CreateListingRequest",
     "DataExchange",
     "DataProvider",
     "DeleteDataExchangeRequest",
     "DeleteListingRequest",
     "DestinationDataset",
     "DestinationDatasetReference",
     "GetDataExchangeRequest",
     "GetListingRequest",
     "ListDataExchangesRequest",
     "ListDataExchangesResponse",
-    "Listing",
     "ListListingsRequest",
     "ListListingsResponse",
     "ListOrgDataExchangesRequest",
     "ListOrgDataExchangesResponse",
+    "Listing",
     "Publisher",
     "SubscribeListingRequest",
     "SubscribeListingResponse",
     "UpdateDataExchangeRequest",
     "UpdateListingRequest",
 )
```

### Comparing `google-cloud-bigquery-analyticshub-0.3.2/google/cloud/bigquery/analyticshub/gapic_version.py` & `google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub/gapic_version.py`

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
-__version__ = "0.3.2"  # {x-release-please-version}
+__version__ = "0.4.0"  # {x-release-please-version}
```

### Comparing `google-cloud-bigquery-analyticshub-0.3.2/google/cloud/bigquery/analyticshub_v1/__init__.py` & `google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,24 +9,26 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from google.cloud.bigquery.analyticshub_v1 import gapic_version as package_version
+from google.cloud.bigquery_analyticshub import gapic_version as package_version
 
 __version__ = package_version.__version__
 
 
-from .services.analytics_hub_service import (
+from google.cloud.bigquery_analyticshub_v1.services.analytics_hub_service.async_client import (
     AnalyticsHubServiceAsyncClient,
+)
+from google.cloud.bigquery_analyticshub_v1.services.analytics_hub_service.client import (
     AnalyticsHubServiceClient,
 )
-from .types.analyticshub import (
+from google.cloud.bigquery_analyticshub_v1.types.analyticshub import (
     CreateDataExchangeRequest,
     CreateListingRequest,
     DataExchange,
     DataProvider,
     DeleteDataExchangeRequest,
     DeleteListingRequest,
     DestinationDataset,
@@ -44,32 +46,32 @@
     SubscribeListingRequest,
     SubscribeListingResponse,
     UpdateDataExchangeRequest,
     UpdateListingRequest,
 )
 
 __all__ = (
-    "AnalyticsHubServiceAsyncClient",
     "AnalyticsHubServiceClient",
+    "AnalyticsHubServiceAsyncClient",
     "CreateDataExchangeRequest",
     "CreateListingRequest",
     "DataExchange",
     "DataProvider",
     "DeleteDataExchangeRequest",
     "DeleteListingRequest",
     "DestinationDataset",
     "DestinationDatasetReference",
     "GetDataExchangeRequest",
     "GetListingRequest",
     "ListDataExchangesRequest",
     "ListDataExchangesResponse",
+    "Listing",
     "ListListingsRequest",
     "ListListingsResponse",
     "ListOrgDataExchangesRequest",
     "ListOrgDataExchangesResponse",
-    "Listing",
     "Publisher",
     "SubscribeListingRequest",
     "SubscribeListingResponse",
     "UpdateDataExchangeRequest",
     "UpdateListingRequest",
 )
```

### Comparing `google-cloud-bigquery-analyticshub-0.3.2/google/cloud/bigquery/analyticshub_v1/gapic_metadata.json` & `google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/gapic_metadata.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'libraryPackage'": "'google.cloud.bigquery_analyticshub_v1'"}*

```diff
@@ -1,11 +1,11 @@
 {
     "comment": "This file maps proto services/RPCs to the corresponding library clients/methods",
     "language": "python",
-    "libraryPackage": "google.cloud.bigquery.analyticshub_v1",
+    "libraryPackage": "google.cloud.bigquery_analyticshub_v1",
     "protoPackage": "google.cloud.bigquery.analyticshub.v1",
     "schema": "1.0",
     "services": {
         "AnalyticsHubService": {
             "clients": {
                 "grpc": {
                     "libraryClient": "AnalyticsHubServiceClient",
```

### Comparing `google-cloud-bigquery-analyticshub-0.3.2/google/cloud/bigquery/analyticshub_v1/gapic_version.py` & `google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/gapic_version.py`

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
-__version__ = "0.3.2"  # {x-release-please-version}
+__version__ = "0.4.0"  # {x-release-please-version}
```

### Comparing `google-cloud-bigquery-analyticshub-0.3.2/google/cloud/bigquery/analyticshub_v1/services/__init__.py` & `google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-analyticshub-0.3.2/google/cloud/bigquery/analyticshub_v1/services/analytics_hub_service/__init__.py` & `google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-analyticshub-0.3.2/google/cloud/bigquery/analyticshub_v1/services/analytics_hub_service/async_client.py` & `google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/async_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,27 +31,27 @@
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.api_core.client_options import ClientOptions
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 
-from google.cloud.bigquery.analyticshub_v1 import gapic_version as package_version
+from google.cloud.bigquery_analyticshub_v1 import gapic_version as package_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.iam.v1 import iam_policy_pb2  # type: ignore
 from google.iam.v1 import policy_pb2  # type: ignore
 from google.protobuf import field_mask_pb2  # type: ignore
 
-from google.cloud.bigquery.analyticshub_v1.services.analytics_hub_service import pagers
-from google.cloud.bigquery.analyticshub_v1.types import analyticshub
+from google.cloud.bigquery_analyticshub_v1.services.analytics_hub_service import pagers
+from google.cloud.bigquery_analyticshub_v1.types import analyticshub
 
 from .client import AnalyticsHubServiceClient
 from .transports.base import DEFAULT_CLIENT_INFO, AnalyticsHubServiceTransport
 from .transports.grpc_asyncio import AnalyticsHubServiceGrpcAsyncIOTransport
 
 
 class AnalyticsHubServiceAsyncClient:
@@ -249,34 +249,34 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import analyticshub_v1
+            from google.cloud import bigquery_analyticshub_v1
 
             async def sample_list_data_exchanges():
                 # Create a client
-                client = analyticshub_v1.AnalyticsHubServiceAsyncClient()
+                client = bigquery_analyticshub_v1.AnalyticsHubServiceAsyncClient()
 
                 # Initialize request argument(s)
-                request = analyticshub_v1.ListDataExchangesRequest(
+                request = bigquery_analyticshub_v1.ListDataExchangesRequest(
                     parent="parent_value",
                 )
 
                 # Make the request
                 page_result = client.list_data_exchanges(request=request)
 
                 # Handle the response
                 async for response in page_result:
                     print(response)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.analyticshub_v1.types.ListDataExchangesRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_analyticshub_v1.types.ListDataExchangesRequest, dict]]):
                 The request object. Message for requesting the list of
                 data exchanges.
             parent (:class:`str`):
                 Required. The parent resource path of the data
                 exchanges. e.g. ``projects/myproject/locations/US``.
 
                 This corresponds to the ``parent`` field
@@ -285,15 +285,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.analyticshub_v1.services.analytics_hub_service.pagers.ListDataExchangesAsyncPager:
+            google.cloud.bigquery_analyticshub_v1.services.analytics_hub_service.pagers.ListDataExchangesAsyncPager:
                 Message for response to the list of
                 data exchanges.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
@@ -365,34 +365,34 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import analyticshub_v1
+            from google.cloud import bigquery_analyticshub_v1
 
             async def sample_list_org_data_exchanges():
                 # Create a client
-                client = analyticshub_v1.AnalyticsHubServiceAsyncClient()
+                client = bigquery_analyticshub_v1.AnalyticsHubServiceAsyncClient()
 
                 # Initialize request argument(s)
-                request = analyticshub_v1.ListOrgDataExchangesRequest(
+                request = bigquery_analyticshub_v1.ListOrgDataExchangesRequest(
                     organization="organization_value",
                 )
 
                 # Make the request
                 page_result = client.list_org_data_exchanges(request=request)
 
                 # Handle the response
                 async for response in page_result:
                     print(response)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.analyticshub_v1.types.ListOrgDataExchangesRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_analyticshub_v1.types.ListOrgDataExchangesRequest, dict]]):
                 The request object. Message for requesting the list of
                 data exchanges from projects in an
                 organization and location.
             organization (:class:`str`):
                 Required. The organization resource path of the projects
                 containing DataExchanges. e.g.
                 ``organizations/myorg/locations/US``.
@@ -403,15 +403,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.analyticshub_v1.services.analytics_hub_service.pagers.ListOrgDataExchangesAsyncPager:
+            google.cloud.bigquery_analyticshub_v1.services.analytics_hub_service.pagers.ListOrgDataExchangesAsyncPager:
                 Message for response to listing data
                 exchanges in an organization and
                 location.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
@@ -485,33 +485,33 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import analyticshub_v1
+            from google.cloud import bigquery_analyticshub_v1
 
             async def sample_get_data_exchange():
                 # Create a client
-                client = analyticshub_v1.AnalyticsHubServiceAsyncClient()
+                client = bigquery_analyticshub_v1.AnalyticsHubServiceAsyncClient()
 
                 # Initialize request argument(s)
-                request = analyticshub_v1.GetDataExchangeRequest(
+                request = bigquery_analyticshub_v1.GetDataExchangeRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 response = await client.get_data_exchange(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.analyticshub_v1.types.GetDataExchangeRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_analyticshub_v1.types.GetDataExchangeRequest, dict]]):
                 The request object. Message for getting a data exchange.
             name (:class:`str`):
                 Required. The resource name of the data exchange. e.g.
                 ``projects/myproject/locations/US/dataExchanges/123``.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
@@ -519,15 +519,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.analyticshub_v1.types.DataExchange:
+            google.cloud.bigquery_analyticshub_v1.types.DataExchange:
                 A data exchange is a container that
                 lets you share data. Along with the
                 descriptive information about the data
                 exchange, it contains listings that
                 reference shared datasets.
 
         """
@@ -590,61 +590,61 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import analyticshub_v1
+            from google.cloud import bigquery_analyticshub_v1
 
             async def sample_create_data_exchange():
                 # Create a client
-                client = analyticshub_v1.AnalyticsHubServiceAsyncClient()
+                client = bigquery_analyticshub_v1.AnalyticsHubServiceAsyncClient()
 
                 # Initialize request argument(s)
-                data_exchange = analyticshub_v1.DataExchange()
+                data_exchange = bigquery_analyticshub_v1.DataExchange()
                 data_exchange.display_name = "display_name_value"
 
-                request = analyticshub_v1.CreateDataExchangeRequest(
+                request = bigquery_analyticshub_v1.CreateDataExchangeRequest(
                     parent="parent_value",
                     data_exchange_id="data_exchange_id_value",
                     data_exchange=data_exchange,
                 )
 
                 # Make the request
                 response = await client.create_data_exchange(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.analyticshub_v1.types.CreateDataExchangeRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_analyticshub_v1.types.CreateDataExchangeRequest, dict]]):
                 The request object. Message for creating a data exchange.
             parent (:class:`str`):
                 Required. The parent resource path of the data exchange.
                 e.g. ``projects/myproject/locations/US``.
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            data_exchange (:class:`google.cloud.bigquery.analyticshub_v1.types.DataExchange`):
+            data_exchange (:class:`google.cloud.bigquery_analyticshub_v1.types.DataExchange`):
                 Required. The data exchange to
                 create.
 
                 This corresponds to the ``data_exchange`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.analyticshub_v1.types.DataExchange:
+            google.cloud.bigquery_analyticshub_v1.types.DataExchange:
                 A data exchange is a container that
                 lets you share data. Along with the
                 descriptive information about the data
                 exchange, it contains listings that
                 reference shared datasets.
 
         """
@@ -709,38 +709,38 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import analyticshub_v1
+            from google.cloud import bigquery_analyticshub_v1
 
             async def sample_update_data_exchange():
                 # Create a client
-                client = analyticshub_v1.AnalyticsHubServiceAsyncClient()
+                client = bigquery_analyticshub_v1.AnalyticsHubServiceAsyncClient()
 
                 # Initialize request argument(s)
-                data_exchange = analyticshub_v1.DataExchange()
+                data_exchange = bigquery_analyticshub_v1.DataExchange()
                 data_exchange.display_name = "display_name_value"
 
-                request = analyticshub_v1.UpdateDataExchangeRequest(
+                request = bigquery_analyticshub_v1.UpdateDataExchangeRequest(
                     data_exchange=data_exchange,
                 )
 
                 # Make the request
                 response = await client.update_data_exchange(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.analyticshub_v1.types.UpdateDataExchangeRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_analyticshub_v1.types.UpdateDataExchangeRequest, dict]]):
                 The request object. Message for updating a data exchange.
-            data_exchange (:class:`google.cloud.bigquery.analyticshub_v1.types.DataExchange`):
+            data_exchange (:class:`google.cloud.bigquery_analyticshub_v1.types.DataExchange`):
                 Required. The data exchange to
                 update.
 
                 This corresponds to the ``data_exchange`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             update_mask (:class:`google.protobuf.field_mask_pb2.FieldMask`):
@@ -755,15 +755,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.analyticshub_v1.types.DataExchange:
+            google.cloud.bigquery_analyticshub_v1.types.DataExchange:
                 A data exchange is a container that
                 lets you share data. Along with the
                 descriptive information about the data
                 exchange, it contains listings that
                 reference shared datasets.
 
         """
@@ -829,30 +829,30 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import analyticshub_v1
+            from google.cloud import bigquery_analyticshub_v1
 
             async def sample_delete_data_exchange():
                 # Create a client
-                client = analyticshub_v1.AnalyticsHubServiceAsyncClient()
+                client = bigquery_analyticshub_v1.AnalyticsHubServiceAsyncClient()
 
                 # Initialize request argument(s)
-                request = analyticshub_v1.DeleteDataExchangeRequest(
+                request = bigquery_analyticshub_v1.DeleteDataExchangeRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 await client.delete_data_exchange(request=request)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.analyticshub_v1.types.DeleteDataExchangeRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_analyticshub_v1.types.DeleteDataExchangeRequest, dict]]):
                 The request object. Message for deleting a data exchange.
             name (:class:`str`):
                 Required. The full name of the data exchange resource
                 that you want to delete. For example,
                 ``projects/myproject/locations/US/dataExchanges/123``.
 
                 This corresponds to the ``name`` field
@@ -919,34 +919,34 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import analyticshub_v1
+            from google.cloud import bigquery_analyticshub_v1
 
             async def sample_list_listings():
                 # Create a client
-                client = analyticshub_v1.AnalyticsHubServiceAsyncClient()
+                client = bigquery_analyticshub_v1.AnalyticsHubServiceAsyncClient()
 
                 # Initialize request argument(s)
-                request = analyticshub_v1.ListListingsRequest(
+                request = bigquery_analyticshub_v1.ListListingsRequest(
                     parent="parent_value",
                 )
 
                 # Make the request
                 page_result = client.list_listings(request=request)
 
                 # Handle the response
                 async for response in page_result:
                     print(response)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.analyticshub_v1.types.ListListingsRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_analyticshub_v1.types.ListListingsRequest, dict]]):
                 The request object. Message for requesting the list of
                 listings.
             parent (:class:`str`):
                 Required. The parent resource path of the listing. e.g.
                 ``projects/myproject/locations/US/dataExchanges/123``.
 
                 This corresponds to the ``parent`` field
@@ -955,15 +955,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.analyticshub_v1.services.analytics_hub_service.pagers.ListListingsAsyncPager:
+            google.cloud.bigquery_analyticshub_v1.services.analytics_hub_service.pagers.ListListingsAsyncPager:
                 Message for response to the list of
                 Listings.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
@@ -1034,33 +1034,33 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import analyticshub_v1
+            from google.cloud import bigquery_analyticshub_v1
 
             async def sample_get_listing():
                 # Create a client
-                client = analyticshub_v1.AnalyticsHubServiceAsyncClient()
+                client = bigquery_analyticshub_v1.AnalyticsHubServiceAsyncClient()
 
                 # Initialize request argument(s)
-                request = analyticshub_v1.GetListingRequest(
+                request = bigquery_analyticshub_v1.GetListingRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 response = await client.get_listing(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.analyticshub_v1.types.GetListingRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_analyticshub_v1.types.GetListingRequest, dict]]):
                 The request object. Message for getting a listing.
             name (:class:`str`):
                 Required. The resource name of the listing. e.g.
                 ``projects/myproject/locations/US/dataExchanges/123/listings/456``.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
@@ -1068,15 +1068,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.analyticshub_v1.types.Listing:
+            google.cloud.bigquery_analyticshub_v1.types.Listing:
                 A listing is what gets published into
                 a data exchange that a subscriber can
                 subscribe to. It contains a reference to
                 the data source along with descriptive
                 information that will help subscribers
                 find and subscribe the data.
 
@@ -1140,59 +1140,59 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import analyticshub_v1
+            from google.cloud import bigquery_analyticshub_v1
 
             async def sample_create_listing():
                 # Create a client
-                client = analyticshub_v1.AnalyticsHubServiceAsyncClient()
+                client = bigquery_analyticshub_v1.AnalyticsHubServiceAsyncClient()
 
                 # Initialize request argument(s)
-                listing = analyticshub_v1.Listing()
+                listing = bigquery_analyticshub_v1.Listing()
                 listing.display_name = "display_name_value"
 
-                request = analyticshub_v1.CreateListingRequest(
+                request = bigquery_analyticshub_v1.CreateListingRequest(
                     parent="parent_value",
                     listing_id="listing_id_value",
                     listing=listing,
                 )
 
                 # Make the request
                 response = await client.create_listing(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.analyticshub_v1.types.CreateListingRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_analyticshub_v1.types.CreateListingRequest, dict]]):
                 The request object. Message for creating a listing.
             parent (:class:`str`):
                 Required. The parent resource path of the listing. e.g.
                 ``projects/myproject/locations/US/dataExchanges/123``.
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            listing (:class:`google.cloud.bigquery.analyticshub_v1.types.Listing`):
+            listing (:class:`google.cloud.bigquery_analyticshub_v1.types.Listing`):
                 Required. The listing to create.
                 This corresponds to the ``listing`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.analyticshub_v1.types.Listing:
+            google.cloud.bigquery_analyticshub_v1.types.Listing:
                 A listing is what gets published into
                 a data exchange that a subscriber can
                 subscribe to. It contains a reference to
                 the data source along with descriptive
                 information that will help subscribers
                 find and subscribe the data.
 
@@ -1258,38 +1258,38 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import analyticshub_v1
+            from google.cloud import bigquery_analyticshub_v1
 
             async def sample_update_listing():
                 # Create a client
-                client = analyticshub_v1.AnalyticsHubServiceAsyncClient()
+                client = bigquery_analyticshub_v1.AnalyticsHubServiceAsyncClient()
 
                 # Initialize request argument(s)
-                listing = analyticshub_v1.Listing()
+                listing = bigquery_analyticshub_v1.Listing()
                 listing.display_name = "display_name_value"
 
-                request = analyticshub_v1.UpdateListingRequest(
+                request = bigquery_analyticshub_v1.UpdateListingRequest(
                     listing=listing,
                 )
 
                 # Make the request
                 response = await client.update_listing(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.analyticshub_v1.types.UpdateListingRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_analyticshub_v1.types.UpdateListingRequest, dict]]):
                 The request object. Message for updating a Listing.
-            listing (:class:`google.cloud.bigquery.analyticshub_v1.types.Listing`):
+            listing (:class:`google.cloud.bigquery_analyticshub_v1.types.Listing`):
                 Required. The listing to update.
                 This corresponds to the ``listing`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             update_mask (:class:`google.protobuf.field_mask_pb2.FieldMask`):
                 Required. Field mask specifies the fields to update in
                 the listing resource. The fields specified in the
@@ -1302,15 +1302,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.analyticshub_v1.types.Listing:
+            google.cloud.bigquery_analyticshub_v1.types.Listing:
                 A listing is what gets published into
                 a data exchange that a subscriber can
                 subscribe to. It contains a reference to
                 the data source along with descriptive
                 information that will help subscribers
                 find and subscribe the data.
 
@@ -1377,30 +1377,30 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import analyticshub_v1
+            from google.cloud import bigquery_analyticshub_v1
 
             async def sample_delete_listing():
                 # Create a client
-                client = analyticshub_v1.AnalyticsHubServiceAsyncClient()
+                client = bigquery_analyticshub_v1.AnalyticsHubServiceAsyncClient()
 
                 # Initialize request argument(s)
-                request = analyticshub_v1.DeleteListingRequest(
+                request = bigquery_analyticshub_v1.DeleteListingRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 await client.delete_listing(request=request)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.analyticshub_v1.types.DeleteListingRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_analyticshub_v1.types.DeleteListingRequest, dict]]):
                 The request object. Message for deleting a listing.
             name (:class:`str`):
                 Required. Resource name of the listing to delete. e.g.
                 ``projects/myproject/locations/US/dataExchanges/123/listings/456``.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
@@ -1471,39 +1471,39 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import analyticshub_v1
+            from google.cloud import bigquery_analyticshub_v1
 
             async def sample_subscribe_listing():
                 # Create a client
-                client = analyticshub_v1.AnalyticsHubServiceAsyncClient()
+                client = bigquery_analyticshub_v1.AnalyticsHubServiceAsyncClient()
 
                 # Initialize request argument(s)
-                destination_dataset = analyticshub_v1.DestinationDataset()
+                destination_dataset = bigquery_analyticshub_v1.DestinationDataset()
                 destination_dataset.dataset_reference.dataset_id = "dataset_id_value"
                 destination_dataset.dataset_reference.project_id = "project_id_value"
                 destination_dataset.location = "location_value"
 
-                request = analyticshub_v1.SubscribeListingRequest(
+                request = bigquery_analyticshub_v1.SubscribeListingRequest(
                     destination_dataset=destination_dataset,
                     name="name_value",
                 )
 
                 # Make the request
                 response = await client.subscribe_listing(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.bigquery.analyticshub_v1.types.SubscribeListingRequest, dict]]):
+            request (Optional[Union[google.cloud.bigquery_analyticshub_v1.types.SubscribeListingRequest, dict]]):
                 The request object. Message for subscribing to a listing.
             name (:class:`str`):
                 Required. Resource name of the listing that you want to
                 subscribe to. e.g.
                 ``projects/myproject/locations/US/dataExchanges/123/listings/456``.
 
                 This corresponds to the ``name`` field
@@ -1512,15 +1512,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.analyticshub_v1.types.SubscribeListingResponse:
+            google.cloud.bigquery_analyticshub_v1.types.SubscribeListingResponse:
                 Message for response when you
                 subscribe to a listing.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
@@ -1578,20 +1578,20 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import analyticshub_v1
+            from google.cloud import bigquery_analyticshub_v1
             from google.iam.v1 import iam_policy_pb2  # type: ignore
 
             async def sample_get_iam_policy():
                 # Create a client
-                client = analyticshub_v1.AnalyticsHubServiceAsyncClient()
+                client = bigquery_analyticshub_v1.AnalyticsHubServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = iam_policy_pb2.GetIamPolicyRequest(
                     resource="resource_value",
                 )
 
                 # Make the request
@@ -1720,20 +1720,20 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import analyticshub_v1
+            from google.cloud import bigquery_analyticshub_v1
             from google.iam.v1 import iam_policy_pb2  # type: ignore
 
             async def sample_set_iam_policy():
                 # Create a client
-                client = analyticshub_v1.AnalyticsHubServiceAsyncClient()
+                client = bigquery_analyticshub_v1.AnalyticsHubServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = iam_policy_pb2.SetIamPolicyRequest(
                     resource="resource_value",
                 )
 
                 # Make the request
@@ -1862,20 +1862,20 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import analyticshub_v1
+            from google.cloud import bigquery_analyticshub_v1
             from google.iam.v1 import iam_policy_pb2  # type: ignore
 
             async def sample_test_iam_permissions():
                 # Create a client
-                client = analyticshub_v1.AnalyticsHubServiceAsyncClient()
+                client = bigquery_analyticshub_v1.AnalyticsHubServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = iam_policy_pb2.TestIamPermissionsRequest(
                     resource="resource_value",
                     permissions=['permissions_value1', 'permissions_value2'],
                 )
```

### Comparing `google-cloud-bigquery-analyticshub-0.3.2/google/cloud/bigquery/analyticshub_v1/services/analytics_hub_service/client.py` & `google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,27 +35,27 @@
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.exceptions import MutualTLSChannelError  # type: ignore
 from google.auth.transport import mtls  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 
-from google.cloud.bigquery.analyticshub_v1 import gapic_version as package_version
+from google.cloud.bigquery_analyticshub_v1 import gapic_version as package_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.iam.v1 import iam_policy_pb2  # type: ignore
 from google.iam.v1 import policy_pb2  # type: ignore
 from google.protobuf import field_mask_pb2  # type: ignore
 
-from google.cloud.bigquery.analyticshub_v1.services.analytics_hub_service import pagers
-from google.cloud.bigquery.analyticshub_v1.types import analyticshub
+from google.cloud.bigquery_analyticshub_v1.services.analytics_hub_service import pagers
+from google.cloud.bigquery_analyticshub_v1.types import analyticshub
 
 from .transports.base import DEFAULT_CLIENT_INFO, AnalyticsHubServiceTransport
 from .transports.grpc import AnalyticsHubServiceGrpcTransport
 from .transports.grpc_asyncio import AnalyticsHubServiceGrpcAsyncIOTransport
 
 
 class AnalyticsHubServiceClientMeta(type):
@@ -510,34 +510,34 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import analyticshub_v1
+            from google.cloud import bigquery_analyticshub_v1
 
             def sample_list_data_exchanges():
                 # Create a client
-                client = analyticshub_v1.AnalyticsHubServiceClient()
+                client = bigquery_analyticshub_v1.AnalyticsHubServiceClient()
 
                 # Initialize request argument(s)
-                request = analyticshub_v1.ListDataExchangesRequest(
+                request = bigquery_analyticshub_v1.ListDataExchangesRequest(
                     parent="parent_value",
                 )
 
                 # Make the request
                 page_result = client.list_data_exchanges(request=request)
 
                 # Handle the response
                 for response in page_result:
                     print(response)
 
         Args:
-            request (Union[google.cloud.bigquery.analyticshub_v1.types.ListDataExchangesRequest, dict]):
+            request (Union[google.cloud.bigquery_analyticshub_v1.types.ListDataExchangesRequest, dict]):
                 The request object. Message for requesting the list of
                 data exchanges.
             parent (str):
                 Required. The parent resource path of the data
                 exchanges. e.g. ``projects/myproject/locations/US``.
 
                 This corresponds to the ``parent`` field
@@ -546,15 +546,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.analyticshub_v1.services.analytics_hub_service.pagers.ListDataExchangesPager:
+            google.cloud.bigquery_analyticshub_v1.services.analytics_hub_service.pagers.ListDataExchangesPager:
                 Message for response to the list of
                 data exchanges.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
@@ -626,34 +626,34 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import analyticshub_v1
+            from google.cloud import bigquery_analyticshub_v1
 
             def sample_list_org_data_exchanges():
                 # Create a client
-                client = analyticshub_v1.AnalyticsHubServiceClient()
+                client = bigquery_analyticshub_v1.AnalyticsHubServiceClient()
 
                 # Initialize request argument(s)
-                request = analyticshub_v1.ListOrgDataExchangesRequest(
+                request = bigquery_analyticshub_v1.ListOrgDataExchangesRequest(
                     organization="organization_value",
                 )
 
                 # Make the request
                 page_result = client.list_org_data_exchanges(request=request)
 
                 # Handle the response
                 for response in page_result:
                     print(response)
 
         Args:
-            request (Union[google.cloud.bigquery.analyticshub_v1.types.ListOrgDataExchangesRequest, dict]):
+            request (Union[google.cloud.bigquery_analyticshub_v1.types.ListOrgDataExchangesRequest, dict]):
                 The request object. Message for requesting the list of
                 data exchanges from projects in an
                 organization and location.
             organization (str):
                 Required. The organization resource path of the projects
                 containing DataExchanges. e.g.
                 ``organizations/myorg/locations/US``.
@@ -664,15 +664,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.analyticshub_v1.services.analytics_hub_service.pagers.ListOrgDataExchangesPager:
+            google.cloud.bigquery_analyticshub_v1.services.analytics_hub_service.pagers.ListOrgDataExchangesPager:
                 Message for response to listing data
                 exchanges in an organization and
                 location.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
@@ -746,33 +746,33 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import analyticshub_v1
+            from google.cloud import bigquery_analyticshub_v1
 
             def sample_get_data_exchange():
                 # Create a client
-                client = analyticshub_v1.AnalyticsHubServiceClient()
+                client = bigquery_analyticshub_v1.AnalyticsHubServiceClient()
 
                 # Initialize request argument(s)
-                request = analyticshub_v1.GetDataExchangeRequest(
+                request = bigquery_analyticshub_v1.GetDataExchangeRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 response = client.get_data_exchange(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.bigquery.analyticshub_v1.types.GetDataExchangeRequest, dict]):
+            request (Union[google.cloud.bigquery_analyticshub_v1.types.GetDataExchangeRequest, dict]):
                 The request object. Message for getting a data exchange.
             name (str):
                 Required. The resource name of the data exchange. e.g.
                 ``projects/myproject/locations/US/dataExchanges/123``.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
@@ -780,15 +780,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.analyticshub_v1.types.DataExchange:
+            google.cloud.bigquery_analyticshub_v1.types.DataExchange:
                 A data exchange is a container that
                 lets you share data. Along with the
                 descriptive information about the data
                 exchange, it contains listings that
                 reference shared datasets.
 
         """
@@ -851,61 +851,61 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import analyticshub_v1
+            from google.cloud import bigquery_analyticshub_v1
 
             def sample_create_data_exchange():
                 # Create a client
-                client = analyticshub_v1.AnalyticsHubServiceClient()
+                client = bigquery_analyticshub_v1.AnalyticsHubServiceClient()
 
                 # Initialize request argument(s)
-                data_exchange = analyticshub_v1.DataExchange()
+                data_exchange = bigquery_analyticshub_v1.DataExchange()
                 data_exchange.display_name = "display_name_value"
 
-                request = analyticshub_v1.CreateDataExchangeRequest(
+                request = bigquery_analyticshub_v1.CreateDataExchangeRequest(
                     parent="parent_value",
                     data_exchange_id="data_exchange_id_value",
                     data_exchange=data_exchange,
                 )
 
                 # Make the request
                 response = client.create_data_exchange(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.bigquery.analyticshub_v1.types.CreateDataExchangeRequest, dict]):
+            request (Union[google.cloud.bigquery_analyticshub_v1.types.CreateDataExchangeRequest, dict]):
                 The request object. Message for creating a data exchange.
             parent (str):
                 Required. The parent resource path of the data exchange.
                 e.g. ``projects/myproject/locations/US``.
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            data_exchange (google.cloud.bigquery.analyticshub_v1.types.DataExchange):
+            data_exchange (google.cloud.bigquery_analyticshub_v1.types.DataExchange):
                 Required. The data exchange to
                 create.
 
                 This corresponds to the ``data_exchange`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.analyticshub_v1.types.DataExchange:
+            google.cloud.bigquery_analyticshub_v1.types.DataExchange:
                 A data exchange is a container that
                 lets you share data. Along with the
                 descriptive information about the data
                 exchange, it contains listings that
                 reference shared datasets.
 
         """
@@ -970,38 +970,38 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import analyticshub_v1
+            from google.cloud import bigquery_analyticshub_v1
 
             def sample_update_data_exchange():
                 # Create a client
-                client = analyticshub_v1.AnalyticsHubServiceClient()
+                client = bigquery_analyticshub_v1.AnalyticsHubServiceClient()
 
                 # Initialize request argument(s)
-                data_exchange = analyticshub_v1.DataExchange()
+                data_exchange = bigquery_analyticshub_v1.DataExchange()
                 data_exchange.display_name = "display_name_value"
 
-                request = analyticshub_v1.UpdateDataExchangeRequest(
+                request = bigquery_analyticshub_v1.UpdateDataExchangeRequest(
                     data_exchange=data_exchange,
                 )
 
                 # Make the request
                 response = client.update_data_exchange(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.bigquery.analyticshub_v1.types.UpdateDataExchangeRequest, dict]):
+            request (Union[google.cloud.bigquery_analyticshub_v1.types.UpdateDataExchangeRequest, dict]):
                 The request object. Message for updating a data exchange.
-            data_exchange (google.cloud.bigquery.analyticshub_v1.types.DataExchange):
+            data_exchange (google.cloud.bigquery_analyticshub_v1.types.DataExchange):
                 Required. The data exchange to
                 update.
 
                 This corresponds to the ``data_exchange`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             update_mask (google.protobuf.field_mask_pb2.FieldMask):
@@ -1016,15 +1016,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.analyticshub_v1.types.DataExchange:
+            google.cloud.bigquery_analyticshub_v1.types.DataExchange:
                 A data exchange is a container that
                 lets you share data. Along with the
                 descriptive information about the data
                 exchange, it contains listings that
                 reference shared datasets.
 
         """
@@ -1090,30 +1090,30 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import analyticshub_v1
+            from google.cloud import bigquery_analyticshub_v1
 
             def sample_delete_data_exchange():
                 # Create a client
-                client = analyticshub_v1.AnalyticsHubServiceClient()
+                client = bigquery_analyticshub_v1.AnalyticsHubServiceClient()
 
                 # Initialize request argument(s)
-                request = analyticshub_v1.DeleteDataExchangeRequest(
+                request = bigquery_analyticshub_v1.DeleteDataExchangeRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 client.delete_data_exchange(request=request)
 
         Args:
-            request (Union[google.cloud.bigquery.analyticshub_v1.types.DeleteDataExchangeRequest, dict]):
+            request (Union[google.cloud.bigquery_analyticshub_v1.types.DeleteDataExchangeRequest, dict]):
                 The request object. Message for deleting a data exchange.
             name (str):
                 Required. The full name of the data exchange resource
                 that you want to delete. For example,
                 ``projects/myproject/locations/US/dataExchanges/123``.
 
                 This corresponds to the ``name`` field
@@ -1180,34 +1180,34 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import analyticshub_v1
+            from google.cloud import bigquery_analyticshub_v1
 
             def sample_list_listings():
                 # Create a client
-                client = analyticshub_v1.AnalyticsHubServiceClient()
+                client = bigquery_analyticshub_v1.AnalyticsHubServiceClient()
 
                 # Initialize request argument(s)
-                request = analyticshub_v1.ListListingsRequest(
+                request = bigquery_analyticshub_v1.ListListingsRequest(
                     parent="parent_value",
                 )
 
                 # Make the request
                 page_result = client.list_listings(request=request)
 
                 # Handle the response
                 for response in page_result:
                     print(response)
 
         Args:
-            request (Union[google.cloud.bigquery.analyticshub_v1.types.ListListingsRequest, dict]):
+            request (Union[google.cloud.bigquery_analyticshub_v1.types.ListListingsRequest, dict]):
                 The request object. Message for requesting the list of
                 listings.
             parent (str):
                 Required. The parent resource path of the listing. e.g.
                 ``projects/myproject/locations/US/dataExchanges/123``.
 
                 This corresponds to the ``parent`` field
@@ -1216,15 +1216,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.analyticshub_v1.services.analytics_hub_service.pagers.ListListingsPager:
+            google.cloud.bigquery_analyticshub_v1.services.analytics_hub_service.pagers.ListListingsPager:
                 Message for response to the list of
                 Listings.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
@@ -1295,33 +1295,33 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import analyticshub_v1
+            from google.cloud import bigquery_analyticshub_v1
 
             def sample_get_listing():
                 # Create a client
-                client = analyticshub_v1.AnalyticsHubServiceClient()
+                client = bigquery_analyticshub_v1.AnalyticsHubServiceClient()
 
                 # Initialize request argument(s)
-                request = analyticshub_v1.GetListingRequest(
+                request = bigquery_analyticshub_v1.GetListingRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 response = client.get_listing(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.bigquery.analyticshub_v1.types.GetListingRequest, dict]):
+            request (Union[google.cloud.bigquery_analyticshub_v1.types.GetListingRequest, dict]):
                 The request object. Message for getting a listing.
             name (str):
                 Required. The resource name of the listing. e.g.
                 ``projects/myproject/locations/US/dataExchanges/123/listings/456``.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
@@ -1329,15 +1329,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.analyticshub_v1.types.Listing:
+            google.cloud.bigquery_analyticshub_v1.types.Listing:
                 A listing is what gets published into
                 a data exchange that a subscriber can
                 subscribe to. It contains a reference to
                 the data source along with descriptive
                 information that will help subscribers
                 find and subscribe the data.
 
@@ -1401,59 +1401,59 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import analyticshub_v1
+            from google.cloud import bigquery_analyticshub_v1
 
             def sample_create_listing():
                 # Create a client
-                client = analyticshub_v1.AnalyticsHubServiceClient()
+                client = bigquery_analyticshub_v1.AnalyticsHubServiceClient()
 
                 # Initialize request argument(s)
-                listing = analyticshub_v1.Listing()
+                listing = bigquery_analyticshub_v1.Listing()
                 listing.display_name = "display_name_value"
 
-                request = analyticshub_v1.CreateListingRequest(
+                request = bigquery_analyticshub_v1.CreateListingRequest(
                     parent="parent_value",
                     listing_id="listing_id_value",
                     listing=listing,
                 )
 
                 # Make the request
                 response = client.create_listing(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.bigquery.analyticshub_v1.types.CreateListingRequest, dict]):
+            request (Union[google.cloud.bigquery_analyticshub_v1.types.CreateListingRequest, dict]):
                 The request object. Message for creating a listing.
             parent (str):
                 Required. The parent resource path of the listing. e.g.
                 ``projects/myproject/locations/US/dataExchanges/123``.
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            listing (google.cloud.bigquery.analyticshub_v1.types.Listing):
+            listing (google.cloud.bigquery_analyticshub_v1.types.Listing):
                 Required. The listing to create.
                 This corresponds to the ``listing`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.analyticshub_v1.types.Listing:
+            google.cloud.bigquery_analyticshub_v1.types.Listing:
                 A listing is what gets published into
                 a data exchange that a subscriber can
                 subscribe to. It contains a reference to
                 the data source along with descriptive
                 information that will help subscribers
                 find and subscribe the data.
 
@@ -1519,38 +1519,38 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import analyticshub_v1
+            from google.cloud import bigquery_analyticshub_v1
 
             def sample_update_listing():
                 # Create a client
-                client = analyticshub_v1.AnalyticsHubServiceClient()
+                client = bigquery_analyticshub_v1.AnalyticsHubServiceClient()
 
                 # Initialize request argument(s)
-                listing = analyticshub_v1.Listing()
+                listing = bigquery_analyticshub_v1.Listing()
                 listing.display_name = "display_name_value"
 
-                request = analyticshub_v1.UpdateListingRequest(
+                request = bigquery_analyticshub_v1.UpdateListingRequest(
                     listing=listing,
                 )
 
                 # Make the request
                 response = client.update_listing(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.bigquery.analyticshub_v1.types.UpdateListingRequest, dict]):
+            request (Union[google.cloud.bigquery_analyticshub_v1.types.UpdateListingRequest, dict]):
                 The request object. Message for updating a Listing.
-            listing (google.cloud.bigquery.analyticshub_v1.types.Listing):
+            listing (google.cloud.bigquery_analyticshub_v1.types.Listing):
                 Required. The listing to update.
                 This corresponds to the ``listing`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             update_mask (google.protobuf.field_mask_pb2.FieldMask):
                 Required. Field mask specifies the fields to update in
                 the listing resource. The fields specified in the
@@ -1563,15 +1563,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.analyticshub_v1.types.Listing:
+            google.cloud.bigquery_analyticshub_v1.types.Listing:
                 A listing is what gets published into
                 a data exchange that a subscriber can
                 subscribe to. It contains a reference to
                 the data source along with descriptive
                 information that will help subscribers
                 find and subscribe the data.
 
@@ -1638,30 +1638,30 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import analyticshub_v1
+            from google.cloud import bigquery_analyticshub_v1
 
             def sample_delete_listing():
                 # Create a client
-                client = analyticshub_v1.AnalyticsHubServiceClient()
+                client = bigquery_analyticshub_v1.AnalyticsHubServiceClient()
 
                 # Initialize request argument(s)
-                request = analyticshub_v1.DeleteListingRequest(
+                request = bigquery_analyticshub_v1.DeleteListingRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 client.delete_listing(request=request)
 
         Args:
-            request (Union[google.cloud.bigquery.analyticshub_v1.types.DeleteListingRequest, dict]):
+            request (Union[google.cloud.bigquery_analyticshub_v1.types.DeleteListingRequest, dict]):
                 The request object. Message for deleting a listing.
             name (str):
                 Required. Resource name of the listing to delete. e.g.
                 ``projects/myproject/locations/US/dataExchanges/123/listings/456``.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
@@ -1732,39 +1732,39 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import analyticshub_v1
+            from google.cloud import bigquery_analyticshub_v1
 
             def sample_subscribe_listing():
                 # Create a client
-                client = analyticshub_v1.AnalyticsHubServiceClient()
+                client = bigquery_analyticshub_v1.AnalyticsHubServiceClient()
 
                 # Initialize request argument(s)
-                destination_dataset = analyticshub_v1.DestinationDataset()
+                destination_dataset = bigquery_analyticshub_v1.DestinationDataset()
                 destination_dataset.dataset_reference.dataset_id = "dataset_id_value"
                 destination_dataset.dataset_reference.project_id = "project_id_value"
                 destination_dataset.location = "location_value"
 
-                request = analyticshub_v1.SubscribeListingRequest(
+                request = bigquery_analyticshub_v1.SubscribeListingRequest(
                     destination_dataset=destination_dataset,
                     name="name_value",
                 )
 
                 # Make the request
                 response = client.subscribe_listing(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.bigquery.analyticshub_v1.types.SubscribeListingRequest, dict]):
+            request (Union[google.cloud.bigquery_analyticshub_v1.types.SubscribeListingRequest, dict]):
                 The request object. Message for subscribing to a listing.
             name (str):
                 Required. Resource name of the listing that you want to
                 subscribe to. e.g.
                 ``projects/myproject/locations/US/dataExchanges/123/listings/456``.
 
                 This corresponds to the ``name`` field
@@ -1773,15 +1773,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.bigquery.analyticshub_v1.types.SubscribeListingResponse:
+            google.cloud.bigquery_analyticshub_v1.types.SubscribeListingResponse:
                 Message for response when you
                 subscribe to a listing.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
@@ -1839,20 +1839,20 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import analyticshub_v1
+            from google.cloud import bigquery_analyticshub_v1
             from google.iam.v1 import iam_policy_pb2  # type: ignore
 
             def sample_get_iam_policy():
                 # Create a client
-                client = analyticshub_v1.AnalyticsHubServiceClient()
+                client = bigquery_analyticshub_v1.AnalyticsHubServiceClient()
 
                 # Initialize request argument(s)
                 request = iam_policy_pb2.GetIamPolicyRequest(
                     resource="resource_value",
                 )
 
                 # Make the request
@@ -1980,20 +1980,20 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import analyticshub_v1
+            from google.cloud import bigquery_analyticshub_v1
             from google.iam.v1 import iam_policy_pb2  # type: ignore
 
             def sample_set_iam_policy():
                 # Create a client
-                client = analyticshub_v1.AnalyticsHubServiceClient()
+                client = bigquery_analyticshub_v1.AnalyticsHubServiceClient()
 
                 # Initialize request argument(s)
                 request = iam_policy_pb2.SetIamPolicyRequest(
                     resource="resource_value",
                 )
 
                 # Make the request
@@ -2121,20 +2121,20 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud.bigquery import analyticshub_v1
+            from google.cloud import bigquery_analyticshub_v1
             from google.iam.v1 import iam_policy_pb2  # type: ignore
 
             def sample_test_iam_permissions():
                 # Create a client
-                client = analyticshub_v1.AnalyticsHubServiceClient()
+                client = bigquery_analyticshub_v1.AnalyticsHubServiceClient()
 
                 # Initialize request argument(s)
                 request = iam_policy_pb2.TestIamPermissionsRequest(
                     resource="resource_value",
                     permissions=['permissions_value1', 'permissions_value2'],
                 )
```

### Comparing `google-cloud-bigquery-analyticshub-0.3.2/google/cloud/bigquery/analyticshub_v1/services/analytics_hub_service/pagers.py` & `google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/pagers.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,31 +20,31 @@
     Callable,
     Iterator,
     Optional,
     Sequence,
     Tuple,
 )
 
-from google.cloud.bigquery.analyticshub_v1.types import analyticshub
+from google.cloud.bigquery_analyticshub_v1.types import analyticshub
 
 
 class ListDataExchangesPager:
     """A pager for iterating through ``list_data_exchanges`` requests.
 
     This class thinly wraps an initial
-    :class:`google.cloud.bigquery.analyticshub_v1.types.ListDataExchangesResponse` object, and
+    :class:`google.cloud.bigquery_analyticshub_v1.types.ListDataExchangesResponse` object, and
     provides an ``__iter__`` method to iterate through its
     ``data_exchanges`` field.
 
     If there are more pages, the ``__iter__`` method will make additional
     ``ListDataExchanges`` requests and continue to iterate
     through the ``data_exchanges`` field on the
     corresponding responses.
 
-    All the usual :class:`google.cloud.bigquery.analyticshub_v1.types.ListDataExchangesResponse`
+    All the usual :class:`google.cloud.bigquery_analyticshub_v1.types.ListDataExchangesResponse`
     attributes are available on the pager. If multiple requests are made, only
     the most recent response is retained, and thus used for attribute lookup.
     """
 
     def __init__(
         self,
         method: Callable[..., analyticshub.ListDataExchangesResponse],
@@ -54,17 +54,17 @@
         metadata: Sequence[Tuple[str, str]] = ()
     ):
         """Instantiate the pager.
 
         Args:
             method (Callable): The method that was originally called, and
                 which instantiated this pager.
-            request (google.cloud.bigquery.analyticshub_v1.types.ListDataExchangesRequest):
+            request (google.cloud.bigquery_analyticshub_v1.types.ListDataExchangesRequest):
                 The initial request object.
-            response (google.cloud.bigquery.analyticshub_v1.types.ListDataExchangesResponse):
+            response (google.cloud.bigquery_analyticshub_v1.types.ListDataExchangesResponse):
                 The initial response object.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         self._method = method
         self._request = analyticshub.ListDataExchangesRequest(request)
         self._response = response
@@ -89,24 +89,24 @@
         return "{0}<{1!r}>".format(self.__class__.__name__, self._response)
 
 
 class ListDataExchangesAsyncPager:
     """A pager for iterating through ``list_data_exchanges`` requests.
 
     This class thinly wraps an initial
-    :class:`google.cloud.bigquery.analyticshub_v1.types.ListDataExchangesResponse` object, and
+    :class:`google.cloud.bigquery_analyticshub_v1.types.ListDataExchangesResponse` object, and
     provides an ``__aiter__`` method to iterate through its
     ``data_exchanges`` field.
 
     If there are more pages, the ``__aiter__`` method will make additional
     ``ListDataExchanges`` requests and continue to iterate
     through the ``data_exchanges`` field on the
     corresponding responses.
 
-    All the usual :class:`google.cloud.bigquery.analyticshub_v1.types.ListDataExchangesResponse`
+    All the usual :class:`google.cloud.bigquery_analyticshub_v1.types.ListDataExchangesResponse`
     attributes are available on the pager. If multiple requests are made, only
     the most recent response is retained, and thus used for attribute lookup.
     """
 
     def __init__(
         self,
         method: Callable[..., Awaitable[analyticshub.ListDataExchangesResponse]],
@@ -116,17 +116,17 @@
         metadata: Sequence[Tuple[str, str]] = ()
     ):
         """Instantiates the pager.
 
         Args:
             method (Callable): The method that was originally called, and
                 which instantiated this pager.
-            request (google.cloud.bigquery.analyticshub_v1.types.ListDataExchangesRequest):
+            request (google.cloud.bigquery_analyticshub_v1.types.ListDataExchangesRequest):
                 The initial request object.
-            response (google.cloud.bigquery.analyticshub_v1.types.ListDataExchangesResponse):
+            response (google.cloud.bigquery_analyticshub_v1.types.ListDataExchangesResponse):
                 The initial response object.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         self._method = method
         self._request = analyticshub.ListDataExchangesRequest(request)
         self._response = response
@@ -155,24 +155,24 @@
         return "{0}<{1!r}>".format(self.__class__.__name__, self._response)
 
 
 class ListOrgDataExchangesPager:
     """A pager for iterating through ``list_org_data_exchanges`` requests.
 
     This class thinly wraps an initial
-    :class:`google.cloud.bigquery.analyticshub_v1.types.ListOrgDataExchangesResponse` object, and
+    :class:`google.cloud.bigquery_analyticshub_v1.types.ListOrgDataExchangesResponse` object, and
     provides an ``__iter__`` method to iterate through its
     ``data_exchanges`` field.
 
     If there are more pages, the ``__iter__`` method will make additional
     ``ListOrgDataExchanges`` requests and continue to iterate
     through the ``data_exchanges`` field on the
     corresponding responses.
 
-    All the usual :class:`google.cloud.bigquery.analyticshub_v1.types.ListOrgDataExchangesResponse`
+    All the usual :class:`google.cloud.bigquery_analyticshub_v1.types.ListOrgDataExchangesResponse`
     attributes are available on the pager. If multiple requests are made, only
     the most recent response is retained, and thus used for attribute lookup.
     """
 
     def __init__(
         self,
         method: Callable[..., analyticshub.ListOrgDataExchangesResponse],
@@ -182,17 +182,17 @@
         metadata: Sequence[Tuple[str, str]] = ()
     ):
         """Instantiate the pager.
 
         Args:
             method (Callable): The method that was originally called, and
                 which instantiated this pager.
-            request (google.cloud.bigquery.analyticshub_v1.types.ListOrgDataExchangesRequest):
+            request (google.cloud.bigquery_analyticshub_v1.types.ListOrgDataExchangesRequest):
                 The initial request object.
-            response (google.cloud.bigquery.analyticshub_v1.types.ListOrgDataExchangesResponse):
+            response (google.cloud.bigquery_analyticshub_v1.types.ListOrgDataExchangesResponse):
                 The initial response object.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         self._method = method
         self._request = analyticshub.ListOrgDataExchangesRequest(request)
         self._response = response
@@ -217,24 +217,24 @@
         return "{0}<{1!r}>".format(self.__class__.__name__, self._response)
 
 
 class ListOrgDataExchangesAsyncPager:
     """A pager for iterating through ``list_org_data_exchanges`` requests.
 
     This class thinly wraps an initial
-    :class:`google.cloud.bigquery.analyticshub_v1.types.ListOrgDataExchangesResponse` object, and
+    :class:`google.cloud.bigquery_analyticshub_v1.types.ListOrgDataExchangesResponse` object, and
     provides an ``__aiter__`` method to iterate through its
     ``data_exchanges`` field.
 
     If there are more pages, the ``__aiter__`` method will make additional
     ``ListOrgDataExchanges`` requests and continue to iterate
     through the ``data_exchanges`` field on the
     corresponding responses.
 
-    All the usual :class:`google.cloud.bigquery.analyticshub_v1.types.ListOrgDataExchangesResponse`
+    All the usual :class:`google.cloud.bigquery_analyticshub_v1.types.ListOrgDataExchangesResponse`
     attributes are available on the pager. If multiple requests are made, only
     the most recent response is retained, and thus used for attribute lookup.
     """
 
     def __init__(
         self,
         method: Callable[..., Awaitable[analyticshub.ListOrgDataExchangesResponse]],
@@ -244,17 +244,17 @@
         metadata: Sequence[Tuple[str, str]] = ()
     ):
         """Instantiates the pager.
 
         Args:
             method (Callable): The method that was originally called, and
                 which instantiated this pager.
-            request (google.cloud.bigquery.analyticshub_v1.types.ListOrgDataExchangesRequest):
+            request (google.cloud.bigquery_analyticshub_v1.types.ListOrgDataExchangesRequest):
                 The initial request object.
-            response (google.cloud.bigquery.analyticshub_v1.types.ListOrgDataExchangesResponse):
+            response (google.cloud.bigquery_analyticshub_v1.types.ListOrgDataExchangesResponse):
                 The initial response object.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         self._method = method
         self._request = analyticshub.ListOrgDataExchangesRequest(request)
         self._response = response
@@ -283,24 +283,24 @@
         return "{0}<{1!r}>".format(self.__class__.__name__, self._response)
 
 
 class ListListingsPager:
     """A pager for iterating through ``list_listings`` requests.
 
     This class thinly wraps an initial
-    :class:`google.cloud.bigquery.analyticshub_v1.types.ListListingsResponse` object, and
+    :class:`google.cloud.bigquery_analyticshub_v1.types.ListListingsResponse` object, and
     provides an ``__iter__`` method to iterate through its
     ``listings`` field.
 
     If there are more pages, the ``__iter__`` method will make additional
     ``ListListings`` requests and continue to iterate
     through the ``listings`` field on the
     corresponding responses.
 
-    All the usual :class:`google.cloud.bigquery.analyticshub_v1.types.ListListingsResponse`
+    All the usual :class:`google.cloud.bigquery_analyticshub_v1.types.ListListingsResponse`
     attributes are available on the pager. If multiple requests are made, only
     the most recent response is retained, and thus used for attribute lookup.
     """
 
     def __init__(
         self,
         method: Callable[..., analyticshub.ListListingsResponse],
@@ -310,17 +310,17 @@
         metadata: Sequence[Tuple[str, str]] = ()
     ):
         """Instantiate the pager.
 
         Args:
             method (Callable): The method that was originally called, and
                 which instantiated this pager.
-            request (google.cloud.bigquery.analyticshub_v1.types.ListListingsRequest):
+            request (google.cloud.bigquery_analyticshub_v1.types.ListListingsRequest):
                 The initial request object.
-            response (google.cloud.bigquery.analyticshub_v1.types.ListListingsResponse):
+            response (google.cloud.bigquery_analyticshub_v1.types.ListListingsResponse):
                 The initial response object.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         self._method = method
         self._request = analyticshub.ListListingsRequest(request)
         self._response = response
@@ -345,24 +345,24 @@
         return "{0}<{1!r}>".format(self.__class__.__name__, self._response)
 
 
 class ListListingsAsyncPager:
     """A pager for iterating through ``list_listings`` requests.
 
     This class thinly wraps an initial
-    :class:`google.cloud.bigquery.analyticshub_v1.types.ListListingsResponse` object, and
+    :class:`google.cloud.bigquery_analyticshub_v1.types.ListListingsResponse` object, and
     provides an ``__aiter__`` method to iterate through its
     ``listings`` field.
 
     If there are more pages, the ``__aiter__`` method will make additional
     ``ListListings`` requests and continue to iterate
     through the ``listings`` field on the
     corresponding responses.
 
-    All the usual :class:`google.cloud.bigquery.analyticshub_v1.types.ListListingsResponse`
+    All the usual :class:`google.cloud.bigquery_analyticshub_v1.types.ListListingsResponse`
     attributes are available on the pager. If multiple requests are made, only
     the most recent response is retained, and thus used for attribute lookup.
     """
 
     def __init__(
         self,
         method: Callable[..., Awaitable[analyticshub.ListListingsResponse]],
@@ -372,17 +372,17 @@
         metadata: Sequence[Tuple[str, str]] = ()
     ):
         """Instantiates the pager.
 
         Args:
             method (Callable): The method that was originally called, and
                 which instantiated this pager.
-            request (google.cloud.bigquery.analyticshub_v1.types.ListListingsRequest):
+            request (google.cloud.bigquery_analyticshub_v1.types.ListListingsRequest):
                 The initial request object.
-            response (google.cloud.bigquery.analyticshub_v1.types.ListListingsResponse):
+            response (google.cloud.bigquery_analyticshub_v1.types.ListListingsResponse):
                 The initial response object.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         self._method = method
         self._request = analyticshub.ListListingsRequest(request)
         self._response = response
```

### Comparing `google-cloud-bigquery-analyticshub-0.3.2/google/cloud/bigquery/analyticshub_v1/services/analytics_hub_service/transports/__init__.py` & `google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-analyticshub-0.3.2/google/cloud/bigquery/analyticshub_v1/services/analytics_hub_service/transports/base.py` & `google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/transports/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.iam.v1 import iam_policy_pb2  # type: ignore
 from google.iam.v1 import policy_pb2  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 from google.protobuf import empty_pb2  # type: ignore
 
-from google.cloud.bigquery.analyticshub_v1 import gapic_version as package_version
-from google.cloud.bigquery.analyticshub_v1.types import analyticshub
+from google.cloud.bigquery_analyticshub_v1 import gapic_version as package_version
+from google.cloud.bigquery_analyticshub_v1.types import analyticshub
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
     gapic_version=package_version.__version__
 )
 
 
 class AnalyticsHubServiceTransport(abc.ABC):
```

### Comparing `google-cloud-bigquery-analyticshub-0.3.2/google/cloud/bigquery/analyticshub_v1/services/analytics_hub_service/transports/grpc.py` & `google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/transports/grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.iam.v1 import iam_policy_pb2  # type: ignore
 from google.iam.v1 import policy_pb2  # type: ignore
 from google.protobuf import empty_pb2  # type: ignore
 import grpc  # type: ignore
 
-from google.cloud.bigquery.analyticshub_v1.types import analyticshub
+from google.cloud.bigquery_analyticshub_v1.types import analyticshub
 
 from .base import DEFAULT_CLIENT_INFO, AnalyticsHubServiceTransport
 
 
 class AnalyticsHubServiceGrpcTransport(AnalyticsHubServiceTransport):
     """gRPC backend transport for AnalyticsHubService.
```

### Comparing `google-cloud-bigquery-analyticshub-0.3.2/google/cloud/bigquery/analyticshub_v1/services/analytics_hub_service/transports/grpc_asyncio.py` & `google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/transports/grpc_asyncio.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.iam.v1 import iam_policy_pb2  # type: ignore
 from google.iam.v1 import policy_pb2  # type: ignore
 from google.protobuf import empty_pb2  # type: ignore
 import grpc  # type: ignore
 from grpc.experimental import aio  # type: ignore
 
-from google.cloud.bigquery.analyticshub_v1.types import analyticshub
+from google.cloud.bigquery_analyticshub_v1.types import analyticshub
 
 from .base import DEFAULT_CLIENT_INFO, AnalyticsHubServiceTransport
 from .grpc import AnalyticsHubServiceGrpcTransport
 
 
 class AnalyticsHubServiceGrpcAsyncIOTransport(AnalyticsHubServiceTransport):
     """gRPC AsyncIO backend transport for AnalyticsHubService.
```

### Comparing `google-cloud-bigquery-analyticshub-0.3.2/google/cloud/bigquery/analyticshub_v1/types/__init__.py` & `google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-analyticshub-0.3.2/google/cloud/bigquery/analyticshub_v1/types/analyticshub.py` & `google-cloud-bigquery-analyticshub-0.4.0/google/cloud/bigquery_analyticshub_v1/types/analyticshub.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,15 +191,15 @@
     )
 
 
 class DestinationDataset(proto.Message):
     r"""Defines the destination bigquery dataset.
 
     Attributes:
-        dataset_reference (google.cloud.bigquery.analyticshub_v1.types.DestinationDatasetReference):
+        dataset_reference (google.cloud.bigquery_analyticshub_v1.types.DestinationDatasetReference):
             Required. A reference that identifies the
             destination dataset.
         friendly_name (google.protobuf.wrappers_pb2.StringValue):
             Optional. A descriptive name for the dataset.
         description (google.protobuf.wrappers_pb2.StringValue):
             Optional. A user-friendly description of the
             dataset.
@@ -249,15 +249,15 @@
     source along with descriptive information that will help
     subscribers find and subscribe the data.
 
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
     Attributes:
-        bigquery_dataset (google.cloud.bigquery.analyticshub_v1.types.Listing.BigQueryDatasetSource):
+        bigquery_dataset (google.cloud.bigquery_analyticshub_v1.types.Listing.BigQueryDatasetSource):
             Required. Shared dataset i.e. BigQuery
             dataset source.
 
             This field is a member of `oneof`_ ``source``.
         name (str):
             Output only. The resource name of the listing. e.g.
             ``projects/myproject/locations/US/dataExchanges/123/listings/456``
@@ -278,32 +278,32 @@
         primary_contact (str):
             Optional. Email or URL of the primary point
             of contact of the listing. Max Length: 1000
             bytes.
         documentation (str):
             Optional. Documentation describing the
             listing.
-        state (google.cloud.bigquery.analyticshub_v1.types.Listing.State):
+        state (google.cloud.bigquery_analyticshub_v1.types.Listing.State):
             Output only. Current state of the listing.
         icon (bytes):
             Optional. Base64 encoded image representing
             the listing. Max Size: 3.0MiB Expected image
             dimensions are 512x512 pixels, however the API
             only performs validation on size of the encoded
             data. Note: For byte fields, the contents of the
             field are base64-encoded (which increases the
             size of the data by 33-36%) when using JSON on
             the wire.
-        data_provider (google.cloud.bigquery.analyticshub_v1.types.DataProvider):
+        data_provider (google.cloud.bigquery_analyticshub_v1.types.DataProvider):
             Optional. Details of the data provider who
             owns the source data.
-        categories (MutableSequence[google.cloud.bigquery.analyticshub_v1.types.Listing.Category]):
+        categories (MutableSequence[google.cloud.bigquery_analyticshub_v1.types.Listing.Category]):
             Optional. Categories of the listing. Up to
             two categories are allowed.
-        publisher (google.cloud.bigquery.analyticshub_v1.types.Publisher):
+        publisher (google.cloud.bigquery_analyticshub_v1.types.Publisher):
             Optional. Details of the publisher who owns
             the listing and who can share the source data.
         request_access (str):
             Optional. Email or URL of the request access
             of the listing. Subscribers can use this
             reference to request access. Max Length: 1000
             bytes.
@@ -494,15 +494,15 @@
     )
 
 
 class ListDataExchangesResponse(proto.Message):
     r"""Message for response to the list of data exchanges.
 
     Attributes:
-        data_exchanges (MutableSequence[google.cloud.bigquery.analyticshub_v1.types.DataExchange]):
+        data_exchanges (MutableSequence[google.cloud.bigquery_analyticshub_v1.types.DataExchange]):
             The list of data exchanges.
         next_page_token (str):
             A token to request the next page of results.
     """
 
     @property
     def raw_page(self):
@@ -552,15 +552,15 @@
 
 
 class ListOrgDataExchangesResponse(proto.Message):
     r"""Message for response to listing data exchanges in an
     organization and location.
 
     Attributes:
-        data_exchanges (MutableSequence[google.cloud.bigquery.analyticshub_v1.types.DataExchange]):
+        data_exchanges (MutableSequence[google.cloud.bigquery_analyticshub_v1.types.DataExchange]):
             The list of data exchanges.
         next_page_token (str):
             A token to request the next page of results.
     """
 
     @property
     def raw_page(self):
@@ -600,15 +600,15 @@
             Required. The parent resource path of the data exchange.
             e.g. ``projects/myproject/locations/US``.
         data_exchange_id (str):
             Required. The ID of the data exchange. Must contain only
             Unicode letters, numbers (0-9), underscores (_). Should not
             use characters that require URL-escaping, or characters
             outside of ASCII, spaces. Max length: 100 bytes.
-        data_exchange (google.cloud.bigquery.analyticshub_v1.types.DataExchange):
+        data_exchange (google.cloud.bigquery_analyticshub_v1.types.DataExchange):
             Required. The data exchange to create.
     """
 
     parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
@@ -628,15 +628,15 @@
 
     Attributes:
         update_mask (google.protobuf.field_mask_pb2.FieldMask):
             Required. Field mask specifies the fields to update in the
             data exchange resource. The fields specified in the
             ``updateMask`` are relative to the resource and are not a
             full request.
-        data_exchange (google.cloud.bigquery.analyticshub_v1.types.DataExchange):
+        data_exchange (google.cloud.bigquery_analyticshub_v1.types.DataExchange):
             Required. The data exchange to update.
     """
 
     update_mask: field_mask_pb2.FieldMask = proto.Field(
         proto.MESSAGE,
         number=1,
         message=field_mask_pb2.FieldMask,
@@ -694,15 +694,15 @@
     )
 
 
 class ListListingsResponse(proto.Message):
     r"""Message for response to the list of Listings.
 
     Attributes:
-        listings (MutableSequence[google.cloud.bigquery.analyticshub_v1.types.Listing]):
+        listings (MutableSequence[google.cloud.bigquery_analyticshub_v1.types.Listing]):
             The list of Listing.
         next_page_token (str):
             A token to request the next page of results.
     """
 
     @property
     def raw_page(self):
@@ -742,15 +742,15 @@
             Required. The parent resource path of the listing. e.g.
             ``projects/myproject/locations/US/dataExchanges/123``.
         listing_id (str):
             Required. The ID of the listing to create. Must contain only
             Unicode letters, numbers (0-9), underscores (_). Should not
             use characters that require URL-escaping, or characters
             outside of ASCII, spaces. Max length: 100 bytes.
-        listing (google.cloud.bigquery.analyticshub_v1.types.Listing):
+        listing (google.cloud.bigquery_analyticshub_v1.types.Listing):
             Required. The listing to create.
     """
 
     parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
@@ -769,15 +769,15 @@
     r"""Message for updating a Listing.
 
     Attributes:
         update_mask (google.protobuf.field_mask_pb2.FieldMask):
             Required. Field mask specifies the fields to update in the
             listing resource. The fields specified in the ``updateMask``
             are relative to the resource and are not a full request.
-        listing (google.cloud.bigquery.analyticshub_v1.types.Listing):
+        listing (google.cloud.bigquery_analyticshub_v1.types.Listing):
             Required. The listing to update.
     """
 
     update_mask: field_mask_pb2.FieldMask = proto.Field(
         proto.MESSAGE,
         number=1,
         message=field_mask_pb2.FieldMask,
@@ -806,15 +806,15 @@
 
 class SubscribeListingRequest(proto.Message):
     r"""Message for subscribing to a listing.
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
     Attributes:
-        destination_dataset (google.cloud.bigquery.analyticshub_v1.types.DestinationDataset):
+        destination_dataset (google.cloud.bigquery_analyticshub_v1.types.DestinationDataset):
             BigQuery destination dataset to create for
             the subscriber.
 
             This field is a member of `oneof`_ ``destination``.
         name (str):
             Required. Resource name of the listing that you want to
             subscribe to. e.g.
```

### Comparing `google-cloud-bigquery-analyticshub-0.3.2/google_cloud_bigquery_analyticshub.egg-info/PKG-INFO` & `google-cloud-bigquery-analyticshub-0.4.0/google_cloud_bigquery_analyticshub.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-bigquery-analyticshub
-Version: 0.3.2
+Version: 0.4.0
 Summary: Google Cloud Bigquery Analyticshub API client library
-Home-page: https://github.com/googleapis/python-bigquery-analyticshub
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
 
-Python Client for BigQuery Analytics Hub API
-============================================
+Python Client for BigQuery Analytics Hub
+========================================
 
 |preview| |pypi| |versions|
 
-`BigQuery Analytics Hub API`_: Analytics Hub is a data exchange that allows you to efficiently and securely exchange data assets across organizations to address challenges of data reliability and cost. Curate a library of internal and external assets, including unique datasets like Google Trends, backed by the power of BigQuery.
+`BigQuery Analytics Hub`_: Analytics Hub is a data exchange that allows you to efficiently and securely exchange data assets across organizations to address challenges of data reliability and cost. Curate a library of internal and external assets, including unique datasets like Google Trends, backed by the power of BigQuery.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-bigquery-analyticshub.svg
    :target: https://pypi.org/project/google-cloud-bigquery-analyticshub/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-bigquery-analyticshub.svg
    :target: https://pypi.org/project/google-cloud-bigquery-analyticshub/
-.. _BigQuery Analytics Hub API: https://cloud.google.com/analytics-hub
+.. _BigQuery Analytics Hub: https://cloud.google.com/analytics-hub
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/analyticshub/latest
 .. _Product Documentation:  https://cloud.google.com/analytics-hub
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the BigQuery Analytics Hub API.`_
+3. `Enable the BigQuery Analytics Hub.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the BigQuery Analytics Hub API.:  https://cloud.google.com/analytics-hub
+.. _Enable the BigQuery Analytics Hub.:  https://cloud.google.com/analytics-hub
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-bigquery-analyticshub
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for BigQuery Analytics Hub API
+-  Read the `Client Library Documentation`_ for BigQuery Analytics Hub
    to see other available methods on the client.
--  Read the `BigQuery Analytics Hub API Product documentation`_ to learn
+-  Read the `BigQuery Analytics Hub Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _BigQuery Analytics Hub API Product documentation:  https://cloud.google.com/analytics-hub
+.. _BigQuery Analytics Hub Product documentation:  https://cloud.google.com/analytics-hub
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-bigquery-analyticshub-0.3.2/google_cloud_bigquery_analyticshub.egg-info/SOURCES.txt` & `google-cloud-bigquery-analyticshub-0.4.0/google_cloud_bigquery_analyticshub.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 LICENSE
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
-google/cloud/bigquery/analyticshub/__init__.py
-google/cloud/bigquery/analyticshub/gapic_version.py
-google/cloud/bigquery/analyticshub/py.typed
-google/cloud/bigquery/analyticshub_v1/__init__.py
-google/cloud/bigquery/analyticshub_v1/gapic_metadata.json
-google/cloud/bigquery/analyticshub_v1/gapic_version.py
-google/cloud/bigquery/analyticshub_v1/py.typed
-google/cloud/bigquery/analyticshub_v1/services/__init__.py
-google/cloud/bigquery/analyticshub_v1/services/analytics_hub_service/__init__.py
-google/cloud/bigquery/analyticshub_v1/services/analytics_hub_service/async_client.py
-google/cloud/bigquery/analyticshub_v1/services/analytics_hub_service/client.py
-google/cloud/bigquery/analyticshub_v1/services/analytics_hub_service/pagers.py
-google/cloud/bigquery/analyticshub_v1/services/analytics_hub_service/transports/__init__.py
-google/cloud/bigquery/analyticshub_v1/services/analytics_hub_service/transports/base.py
-google/cloud/bigquery/analyticshub_v1/services/analytics_hub_service/transports/grpc.py
-google/cloud/bigquery/analyticshub_v1/services/analytics_hub_service/transports/grpc_asyncio.py
-google/cloud/bigquery/analyticshub_v1/types/__init__.py
-google/cloud/bigquery/analyticshub_v1/types/analyticshub.py
+google/cloud/bigquery_analyticshub/__init__.py
+google/cloud/bigquery_analyticshub/gapic_version.py
+google/cloud/bigquery_analyticshub/py.typed
+google/cloud/bigquery_analyticshub_v1/__init__.py
+google/cloud/bigquery_analyticshub_v1/gapic_metadata.json
+google/cloud/bigquery_analyticshub_v1/gapic_version.py
+google/cloud/bigquery_analyticshub_v1/py.typed
+google/cloud/bigquery_analyticshub_v1/services/__init__.py
+google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/__init__.py
+google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/async_client.py
+google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/client.py
+google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/pagers.py
+google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/transports/__init__.py
+google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/transports/base.py
+google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/transports/grpc.py
+google/cloud/bigquery_analyticshub_v1/services/analytics_hub_service/transports/grpc_asyncio.py
+google/cloud/bigquery_analyticshub_v1/types/__init__.py
+google/cloud/bigquery_analyticshub_v1/types/analyticshub.py
 google_cloud_bigquery_analyticshub.egg-info/PKG-INFO
 google_cloud_bigquery_analyticshub.egg-info/SOURCES.txt
 google_cloud_bigquery_analyticshub.egg-info/dependency_links.txt
 google_cloud_bigquery_analyticshub.egg-info/namespace_packages.txt
 google_cloud_bigquery_analyticshub.egg-info/not-zip-safe
 google_cloud_bigquery_analyticshub.egg-info/requires.txt
 google_cloud_bigquery_analyticshub.egg-info/top_level.txt
 tests/__init__.py
 tests/unit/__init__.py
 tests/unit/gapic/__init__.py
-tests/unit/gapic/analyticshub_v1/__init__.py
-tests/unit/gapic/analyticshub_v1/test_analytics_hub_service.py
+tests/unit/gapic/bigquery_analyticshub_v1/__init__.py
+tests/unit/gapic/bigquery_analyticshub_v1/test_analytics_hub_service.py
```

### Comparing `google-cloud-bigquery-analyticshub-0.3.2/setup.py` & `google-cloud-bigquery-analyticshub-0.4.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 name = "google-cloud-bigquery-analyticshub"
 
 
 description = "Google Cloud Bigquery Analyticshub API client library"
 
 version = {}
 with open(
-    os.path.join(package_root, "google/cloud/bigquery/analyticshub/gapic_version.py")
+    os.path.join(package_root, "google/cloud/bigquery_analyticshub/gapic_version.py")
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
-url = "https://github.com/googleapis/python-bigquery-analyticshub"
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

### Comparing `google-cloud-bigquery-analyticshub-0.3.2/tests/__init__.py` & `google-cloud-bigquery-analyticshub-0.4.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-analyticshub-0.3.2/tests/unit/__init__.py` & `google-cloud-bigquery-analyticshub-0.4.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-analyticshub-0.3.2/tests/unit/gapic/__init__.py` & `google-cloud-bigquery-analyticshub-0.4.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-analyticshub-0.3.2/tests/unit/gapic/analyticshub_v1/__init__.py` & `google-cloud-bigquery-analyticshub-0.4.0/tests/unit/gapic/bigquery_analyticshub_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-analyticshub-0.3.2/tests/unit/gapic/analyticshub_v1/test_analytics_hub_service.py` & `google-cloud-bigquery-analyticshub-0.4.0/tests/unit/gapic/bigquery_analyticshub_v1/test_analytics_hub_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,21 +39,21 @@
 from google.type import expr_pb2  # type: ignore
 import grpc
 from grpc.experimental import aio
 from proto.marshal.rules import wrappers
 from proto.marshal.rules.dates import DurationRule, TimestampRule
 import pytest
 
-from google.cloud.bigquery.analyticshub_v1.services.analytics_hub_service import (
+from google.cloud.bigquery_analyticshub_v1.services.analytics_hub_service import (
     AnalyticsHubServiceAsyncClient,
     AnalyticsHubServiceClient,
     pagers,
     transports,
 )
-from google.cloud.bigquery.analyticshub_v1.types import analyticshub
+from google.cloud.bigquery_analyticshub_v1.types import analyticshub
 
 
 def client_cert_source_callback():
     return b"cert bytes", b"key bytes"
 
 
 # If default endpoint is localhost, then default mtls endpoint will be the same.
@@ -619,15 +619,15 @@
             always_use_jwt_access=True,
             api_audience=None,
         )
 
 
 def test_analytics_hub_service_client_client_options_from_dict():
     with mock.patch(
-        "google.cloud.bigquery.analyticshub_v1.services.analytics_hub_service.transports.AnalyticsHubServiceGrpcTransport.__init__"
+        "google.cloud.bigquery_analyticshub_v1.services.analytics_hub_service.transports.AnalyticsHubServiceGrpcTransport.__init__"
     ) as grpc_transport:
         grpc_transport.return_value = None
         client = AnalyticsHubServiceClient(
             client_options={"api_endpoint": "squid.clam.whelk"}
         )
         grpc_transport.assert_called_once_with(
             credentials=None,
@@ -5052,15 +5052,15 @@
             credentials_file="credentials.json",
         )
 
 
 def test_analytics_hub_service_base_transport():
     # Instantiate the base transport.
     with mock.patch(
-        "google.cloud.bigquery.analyticshub_v1.services.analytics_hub_service.transports.AnalyticsHubServiceTransport.__init__"
+        "google.cloud.bigquery_analyticshub_v1.services.analytics_hub_service.transports.AnalyticsHubServiceTransport.__init__"
     ) as Transport:
         Transport.return_value = None
         transport = transports.AnalyticsHubServiceTransport(
             credentials=ga_credentials.AnonymousCredentials(),
         )
 
     # Every method on the transport should just blindly
@@ -5099,15 +5099,15 @@
 
 
 def test_analytics_hub_service_base_transport_with_credentials_file():
     # Instantiate the base transport with a credentials file
     with mock.patch.object(
         google.auth, "load_credentials_from_file", autospec=True
     ) as load_creds, mock.patch(
-        "google.cloud.bigquery.analyticshub_v1.services.analytics_hub_service.transports.AnalyticsHubServiceTransport._prep_wrapped_messages"
+        "google.cloud.bigquery_analyticshub_v1.services.analytics_hub_service.transports.AnalyticsHubServiceTransport._prep_wrapped_messages"
     ) as Transport:
         Transport.return_value = None
         load_creds.return_value = (ga_credentials.AnonymousCredentials(), None)
         transport = transports.AnalyticsHubServiceTransport(
             credentials_file="credentials.json",
             quota_project_id="octopus",
         )
@@ -5121,15 +5121,15 @@
             quota_project_id="octopus",
         )
 
 
 def test_analytics_hub_service_base_transport_with_adc():
     # Test the default credentials are used if credentials and credentials_file are None.
     with mock.patch.object(google.auth, "default", autospec=True) as adc, mock.patch(
-        "google.cloud.bigquery.analyticshub_v1.services.analytics_hub_service.transports.AnalyticsHubServiceTransport._prep_wrapped_messages"
+        "google.cloud.bigquery_analyticshub_v1.services.analytics_hub_service.transports.AnalyticsHubServiceTransport._prep_wrapped_messages"
     ) as Transport:
         Transport.return_value = None
         adc.return_value = (ga_credentials.AnonymousCredentials(), None)
         transport = transports.AnalyticsHubServiceTransport()
         adc.assert_called_once()
```

