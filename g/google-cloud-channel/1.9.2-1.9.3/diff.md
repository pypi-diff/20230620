# Comparing `tmp/google-cloud-channel-1.9.2.tar.gz` & `tmp/google-cloud-channel-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-channel-1.9.2.tar", last modified: Tue Oct  4 00:21:44 2022, max compression
+gzip compressed data, was "google-cloud-channel-1.9.3.tar", last modified: Mon Oct 10 16:04:35 2022, max compression
```

## Comparing `google-cloud-channel-1.9.2.tar` & `google-cloud-channel-1.9.3.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:21:44.066008 google-cloud-channel-1.9.2/
--rw-rw-r--   0 root         (0)     1003    11358 2022-10-04 00:18:21.000000 google-cloud-channel-1.9.2/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2022-10-04 00:18:21.000000 google-cloud-channel-1.9.2/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4551 2022-10-04 00:21:44.066008 google-cloud-channel-1.9.2/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3816 2022-10-04 00:18:21.000000 google-cloud-channel-1.9.2/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:21:44.058004 google-cloud-channel-1.9.2/google/
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:21:44.058004 google-cloud-channel-1.9.2/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:21:44.058004 google-cloud-channel-1.9.2/google/cloud/channel/
--rw-rw-r--   0 root         (0)     1003     7904 2022-10-04 00:18:21.000000 google-cloud-channel-1.9.2/google/cloud/channel/__init__.py
--rw-rw-r--   0 root         (0)     1003       81 2022-10-04 00:18:21.000000 google-cloud-channel-1.9.2/google/cloud/channel/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:21:44.058004 google-cloud-channel-1.9.2/google/cloud/channel_v1/
--rw-rw-r--   0 root         (0)     1003     7497 2022-10-04 00:18:21.000000 google-cloud-channel-1.9.2/google/cloud/channel_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    12994 2022-10-04 00:18:21.000000 google-cloud-channel-1.9.2/google/cloud/channel_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       81 2022-10-04 00:18:21.000000 google-cloud-channel-1.9.2/google/cloud/channel_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:21:44.058004 google-cloud-channel-1.9.2/google/cloud/channel_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-04 00:18:21.000000 google-cloud-channel-1.9.2/google/cloud/channel_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:21:44.062006 google-cloud-channel-1.9.2/google/cloud/channel_v1/services/cloud_channel_service/
--rw-rw-r--   0 root         (0)     1003      789 2022-10-04 00:18:21.000000 google-cloud-channel-1.9.2/google/cloud/channel_v1/services/cloud_channel_service/__init__.py
--rw-rw-r--   0 root         (0)     1003   234033 2022-10-04 00:18:21.000000 google-cloud-channel-1.9.2/google/cloud/channel_v1/services/cloud_channel_service/async_client.py
--rw-rw-r--   0 root         (0)     1003   253796 2022-10-04 00:18:21.000000 google-cloud-channel-1.9.2/google/cloud/channel_v1/services/cloud_channel_service/client.py
--rw-rw-r--   0 root         (0)     1003    67334 2022-10-04 00:18:21.000000 google-cloud-channel-1.9.2/google/cloud/channel_v1/services/cloud_channel_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:21:44.062006 google-cloud-channel-1.9.2/google/cloud/channel_v1/services/cloud_channel_service/transports/
--rw-rw-r--   0 root         (0)     1003     1246 2022-10-04 00:18:21.000000 google-cloud-channel-1.9.2/google/cloud/channel_v1/services/cloud_channel_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    28810 2022-10-04 00:18:21.000000 google-cloud-channel-1.9.2/google/cloud/channel_v1/services/cloud_channel_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003   111678 2022-10-04 00:18:21.000000 google-cloud-channel-1.9.2/google/cloud/channel_v1/services/cloud_channel_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003   113206 2022-10-04 00:18:21.000000 google-cloud-channel-1.9.2/google/cloud/channel_v1/services/cloud_channel_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:21:44.066008 google-cloud-channel-1.9.2/google/cloud/channel_v1/types/
--rw-rw-r--   0 root         (0)     1003     7250 2022-10-04 00:18:21.000000 google-cloud-channel-1.9.2/google/cloud/channel_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     3691 2022-10-04 00:18:21.000000 google-cloud-channel-1.9.2/google/cloud/channel_v1/types/channel_partner_links.py
--rw-rw-r--   0 root         (0)     1003     6401 2022-10-04 00:18:21.000000 google-cloud-channel-1.9.2/google/cloud/channel_v1/types/common.py
--rw-rw-r--   0 root         (0)     1003     6172 2022-10-04 00:18:21.000000 google-cloud-channel-1.9.2/google/cloud/channel_v1/types/customers.py
--rw-rw-r--   0 root         (0)     1003    12652 2022-10-04 00:18:21.000000 google-cloud-channel-1.9.2/google/cloud/channel_v1/types/entitlements.py
--rw-rw-r--   0 root         (0)     1003    14293 2022-10-04 00:18:21.000000 google-cloud-channel-1.9.2/google/cloud/channel_v1/types/offers.py
--rw-rw-r--   0 root         (0)     1003     1756 2022-10-04 00:18:21.000000 google-cloud-channel-1.9.2/google/cloud/channel_v1/types/operations.py
--rw-rw-r--   0 root         (0)     1003     3680 2022-10-04 00:18:21.000000 google-cloud-channel-1.9.2/google/cloud/channel_v1/types/products.py
--rw-rw-r--   0 root         (0)     1003     8164 2022-10-04 00:18:21.000000 google-cloud-channel-1.9.2/google/cloud/channel_v1/types/repricing.py
--rw-rw-r--   0 root         (0)     1003    78612 2022-10-04 00:18:21.000000 google-cloud-channel-1.9.2/google/cloud/channel_v1/types/service.py
--rw-rw-r--   0 root         (0)     1003     3866 2022-10-04 00:18:21.000000 google-cloud-channel-1.9.2/google/cloud/channel_v1/types/subscriber_event.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:21:44.066008 google-cloud-channel-1.9.2/google_cloud_channel.egg-info/
--rw-r--r--   0 root         (0)     1003     4551 2022-10-04 00:21:44.000000 google-cloud-channel-1.9.2/google_cloud_channel.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1815 2022-10-04 00:21:44.000000 google-cloud-channel-1.9.2/google_cloud_channel.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2022-10-04 00:21:44.000000 google-cloud-channel-1.9.2/google_cloud_channel.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2022-10-04 00:21:44.000000 google-cloud-channel-1.9.2/google_cloud_channel.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2022-10-04 00:21:44.000000 google-cloud-channel-1.9.2/google_cloud_channel.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      160 2022-10-04 00:21:44.000000 google-cloud-channel-1.9.2/google_cloud_channel.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2022-10-04 00:21:44.000000 google-cloud-channel-1.9.2/google_cloud_channel.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2022-10-04 00:21:44.066008 google-cloud-channel-1.9.2/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2164 2022-10-04 00:18:21.000000 google-cloud-channel-1.9.2/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:21:44.066008 google-cloud-channel-1.9.2/tests/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-04 00:18:21.000000 google-cloud-channel-1.9.2/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:21:44.066008 google-cloud-channel-1.9.2/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-04 00:18:21.000000 google-cloud-channel-1.9.2/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:21:44.066008 google-cloud-channel-1.9.2/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-04 00:18:21.000000 google-cloud-channel-1.9.2/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:21:44.066008 google-cloud-channel-1.9.2/tests/unit/gapic/channel_v1/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-04 00:18:21.000000 google-cloud-channel-1.9.2/tests/unit/gapic/channel_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   466590 2022-10-04 00:18:21.000000 google-cloud-channel-1.9.2/tests/unit/gapic/channel_v1/test_cloud_channel_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:04:35.789640 google-cloud-channel-1.9.3/
+-rw-rw-r--   0 root         (0)     1003    11358 2022-10-10 16:01:27.000000 google-cloud-channel-1.9.3/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2022-10-10 16:01:27.000000 google-cloud-channel-1.9.3/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4551 2022-10-10 16:04:35.789640 google-cloud-channel-1.9.3/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3816 2022-10-10 16:01:27.000000 google-cloud-channel-1.9.3/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:04:35.777640 google-cloud-channel-1.9.3/google/
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:04:35.777640 google-cloud-channel-1.9.3/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:04:35.781640 google-cloud-channel-1.9.3/google/cloud/channel/
+-rw-rw-r--   0 root         (0)     1003     7904 2022-10-10 16:01:27.000000 google-cloud-channel-1.9.3/google/cloud/channel/__init__.py
+-rw-rw-r--   0 root         (0)     1003       81 2022-10-10 16:01:27.000000 google-cloud-channel-1.9.3/google/cloud/channel/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:04:35.781640 google-cloud-channel-1.9.3/google/cloud/channel_v1/
+-rw-rw-r--   0 root         (0)     1003     7497 2022-10-10 16:01:27.000000 google-cloud-channel-1.9.3/google/cloud/channel_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12994 2022-10-10 16:01:27.000000 google-cloud-channel-1.9.3/google/cloud/channel_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003       81 2022-10-10 16:01:27.000000 google-cloud-channel-1.9.3/google/cloud/channel_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:04:35.781640 google-cloud-channel-1.9.3/google/cloud/channel_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:01:27.000000 google-cloud-channel-1.9.3/google/cloud/channel_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:04:35.781640 google-cloud-channel-1.9.3/google/cloud/channel_v1/services/cloud_channel_service/
+-rw-rw-r--   0 root         (0)     1003      789 2022-10-10 16:01:27.000000 google-cloud-channel-1.9.3/google/cloud/channel_v1/services/cloud_channel_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003   234033 2022-10-10 16:01:27.000000 google-cloud-channel-1.9.3/google/cloud/channel_v1/services/cloud_channel_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003   253796 2022-10-10 16:01:27.000000 google-cloud-channel-1.9.3/google/cloud/channel_v1/services/cloud_channel_service/client.py
+-rw-rw-r--   0 root         (0)     1003    67334 2022-10-10 16:01:27.000000 google-cloud-channel-1.9.3/google/cloud/channel_v1/services/cloud_channel_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:04:35.785640 google-cloud-channel-1.9.3/google/cloud/channel_v1/services/cloud_channel_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1246 2022-10-10 16:01:27.000000 google-cloud-channel-1.9.3/google/cloud/channel_v1/services/cloud_channel_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    28810 2022-10-10 16:01:27.000000 google-cloud-channel-1.9.3/google/cloud/channel_v1/services/cloud_channel_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003   111678 2022-10-10 16:01:27.000000 google-cloud-channel-1.9.3/google/cloud/channel_v1/services/cloud_channel_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003   113206 2022-10-10 16:01:27.000000 google-cloud-channel-1.9.3/google/cloud/channel_v1/services/cloud_channel_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:04:35.785640 google-cloud-channel-1.9.3/google/cloud/channel_v1/types/
+-rw-rw-r--   0 root         (0)     1003     7250 2022-10-10 16:01:27.000000 google-cloud-channel-1.9.3/google/cloud/channel_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3691 2022-10-10 16:01:27.000000 google-cloud-channel-1.9.3/google/cloud/channel_v1/types/channel_partner_links.py
+-rw-rw-r--   0 root         (0)     1003     6401 2022-10-10 16:01:27.000000 google-cloud-channel-1.9.3/google/cloud/channel_v1/types/common.py
+-rw-rw-r--   0 root         (0)     1003     6172 2022-10-10 16:01:27.000000 google-cloud-channel-1.9.3/google/cloud/channel_v1/types/customers.py
+-rw-rw-r--   0 root         (0)     1003    12652 2022-10-10 16:01:27.000000 google-cloud-channel-1.9.3/google/cloud/channel_v1/types/entitlements.py
+-rw-rw-r--   0 root         (0)     1003    14293 2022-10-10 16:01:27.000000 google-cloud-channel-1.9.3/google/cloud/channel_v1/types/offers.py
+-rw-rw-r--   0 root         (0)     1003     1756 2022-10-10 16:01:27.000000 google-cloud-channel-1.9.3/google/cloud/channel_v1/types/operations.py
+-rw-rw-r--   0 root         (0)     1003     3680 2022-10-10 16:01:27.000000 google-cloud-channel-1.9.3/google/cloud/channel_v1/types/products.py
+-rw-rw-r--   0 root         (0)     1003     8164 2022-10-10 16:01:27.000000 google-cloud-channel-1.9.3/google/cloud/channel_v1/types/repricing.py
+-rw-rw-r--   0 root         (0)     1003    78612 2022-10-10 16:01:27.000000 google-cloud-channel-1.9.3/google/cloud/channel_v1/types/service.py
+-rw-rw-r--   0 root         (0)     1003     3866 2022-10-10 16:01:27.000000 google-cloud-channel-1.9.3/google/cloud/channel_v1/types/subscriber_event.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:04:35.789640 google-cloud-channel-1.9.3/google_cloud_channel.egg-info/
+-rw-r--r--   0 root         (0)     1003     4551 2022-10-10 16:04:35.000000 google-cloud-channel-1.9.3/google_cloud_channel.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1815 2022-10-10 16:04:35.000000 google-cloud-channel-1.9.3/google_cloud_channel.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-10-10 16:04:35.000000 google-cloud-channel-1.9.3/google_cloud_channel.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2022-10-10 16:04:35.000000 google-cloud-channel-1.9.3/google_cloud_channel.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-10-10 16:04:35.000000 google-cloud-channel-1.9.3/google_cloud_channel.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      232 2022-10-10 16:04:35.000000 google-cloud-channel-1.9.3/google_cloud_channel.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2022-10-10 16:04:35.000000 google-cloud-channel-1.9.3/google_cloud_channel.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2022-10-10 16:04:35.789640 google-cloud-channel-1.9.3/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2233 2022-10-10 16:01:27.000000 google-cloud-channel-1.9.3/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:04:35.789640 google-cloud-channel-1.9.3/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:01:27.000000 google-cloud-channel-1.9.3/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:04:35.789640 google-cloud-channel-1.9.3/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:01:27.000000 google-cloud-channel-1.9.3/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:04:35.789640 google-cloud-channel-1.9.3/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:01:27.000000 google-cloud-channel-1.9.3/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:04:35.789640 google-cloud-channel-1.9.3/tests/unit/gapic/channel_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:01:27.000000 google-cloud-channel-1.9.3/tests/unit/gapic/channel_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   466590 2022-10-10 16:01:27.000000 google-cloud-channel-1.9.3/tests/unit/gapic/channel_v1/test_cloud_channel_service.py
```

### Comparing `google-cloud-channel-1.9.2/LICENSE` & `google-cloud-channel-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-channel-1.9.2/MANIFEST.in` & `google-cloud-channel-1.9.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-channel-1.9.2/PKG-INFO` & `google-cloud-channel-1.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-channel
-Version: 1.9.2
+Version: 1.9.3
 Home-page: https://github.com/googleapis/python-channel
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `google-cloud-channel-1.9.2/README.rst` & `google-cloud-channel-1.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-channel-1.9.2/google/cloud/channel/__init__.py` & `google-cloud-channel-1.9.3/google/cloud/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-channel-1.9.2/google/cloud/channel_v1/__init__.py` & `google-cloud-channel-1.9.3/google/cloud/channel_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-channel-1.9.2/google/cloud/channel_v1/gapic_metadata.json` & `google-cloud-channel-1.9.3/google/cloud/channel_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-channel-1.9.2/google/cloud/channel_v1/services/__init__.py` & `google-cloud-channel-1.9.3/google/cloud/channel_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-channel-1.9.2/google/cloud/channel_v1/services/cloud_channel_service/__init__.py` & `google-cloud-channel-1.9.3/google/cloud/channel_v1/services/cloud_channel_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-channel-1.9.2/google/cloud/channel_v1/services/cloud_channel_service/async_client.py` & `google-cloud-channel-1.9.3/google/cloud/channel_v1/services/cloud_channel_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-channel-1.9.2/google/cloud/channel_v1/services/cloud_channel_service/client.py` & `google-cloud-channel-1.9.3/google/cloud/channel_v1/services/cloud_channel_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-channel-1.9.2/google/cloud/channel_v1/services/cloud_channel_service/pagers.py` & `google-cloud-channel-1.9.3/google/cloud/channel_v1/services/cloud_channel_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-channel-1.9.2/google/cloud/channel_v1/services/cloud_channel_service/transports/__init__.py` & `google-cloud-channel-1.9.3/google/cloud/channel_v1/services/cloud_channel_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-channel-1.9.2/google/cloud/channel_v1/services/cloud_channel_service/transports/base.py` & `google-cloud-channel-1.9.3/google/cloud/channel_v1/services/cloud_channel_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-channel-1.9.2/google/cloud/channel_v1/services/cloud_channel_service/transports/grpc.py` & `google-cloud-channel-1.9.3/google/cloud/channel_v1/services/cloud_channel_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-channel-1.9.2/google/cloud/channel_v1/services/cloud_channel_service/transports/grpc_asyncio.py` & `google-cloud-channel-1.9.3/google/cloud/channel_v1/services/cloud_channel_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-channel-1.9.2/google/cloud/channel_v1/types/__init__.py` & `google-cloud-channel-1.9.3/google/cloud/channel_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-channel-1.9.2/google/cloud/channel_v1/types/channel_partner_links.py` & `google-cloud-channel-1.9.3/google/cloud/channel_v1/types/channel_partner_links.py`

 * *Files identical despite different names*

### Comparing `google-cloud-channel-1.9.2/google/cloud/channel_v1/types/common.py` & `google-cloud-channel-1.9.3/google/cloud/channel_v1/types/common.py`

 * *Files identical despite different names*

### Comparing `google-cloud-channel-1.9.2/google/cloud/channel_v1/types/customers.py` & `google-cloud-channel-1.9.3/google/cloud/channel_v1/types/customers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-channel-1.9.2/google/cloud/channel_v1/types/entitlements.py` & `google-cloud-channel-1.9.3/google/cloud/channel_v1/types/entitlements.py`

 * *Files identical despite different names*

### Comparing `google-cloud-channel-1.9.2/google/cloud/channel_v1/types/offers.py` & `google-cloud-channel-1.9.3/google/cloud/channel_v1/types/offers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-channel-1.9.2/google/cloud/channel_v1/types/operations.py` & `google-cloud-channel-1.9.3/google/cloud/channel_v1/types/operations.py`

 * *Files identical despite different names*

### Comparing `google-cloud-channel-1.9.2/google/cloud/channel_v1/types/products.py` & `google-cloud-channel-1.9.3/google/cloud/channel_v1/types/products.py`

 * *Files identical despite different names*

### Comparing `google-cloud-channel-1.9.2/google/cloud/channel_v1/types/repricing.py` & `google-cloud-channel-1.9.3/google/cloud/channel_v1/types/repricing.py`

 * *Files identical despite different names*

### Comparing `google-cloud-channel-1.9.2/google/cloud/channel_v1/types/service.py` & `google-cloud-channel-1.9.3/google/cloud/channel_v1/types/service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-channel-1.9.2/google/cloud/channel_v1/types/subscriber_event.py` & `google-cloud-channel-1.9.3/google/cloud/channel_v1/types/subscriber_event.py`

 * *Files identical despite different names*

### Comparing `google-cloud-channel-1.9.2/google_cloud_channel.egg-info/PKG-INFO` & `google-cloud-channel-1.9.3/google_cloud_channel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-channel
-Version: 1.9.2
+Version: 1.9.3
 Home-page: https://github.com/googleapis/python-channel
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `google-cloud-channel-1.9.2/google_cloud_channel.egg-info/SOURCES.txt` & `google-cloud-channel-1.9.3/google_cloud_channel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-channel-1.9.2/setup.py` & `google-cloud-channel-1.9.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #
 
 import io
 import os
 
 import setuptools  # type: ignore
 
-version = "1.9.2"
+version = "1.9.3"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
 
@@ -44,15 +44,15 @@
     ],
     namespace_packages=("google", "google.cloud"),
     platforms="Posix; MacOS X; Windows",
     include_package_data=True,
     install_requires=(
         "google-api-core[grpc] >= 1.32.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*",
         "proto-plus >= 1.22.0, <2.0.0dev",
-        "protobuf >= 3.20.2, <5.0.0dev",
+        "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
     ),
     python_requires=">=3.7",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3.7",
```

### Comparing `google-cloud-channel-1.9.2/tests/__init__.py` & `google-cloud-channel-1.9.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-channel-1.9.2/tests/unit/__init__.py` & `google-cloud-channel-1.9.3/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-channel-1.9.2/tests/unit/gapic/__init__.py` & `google-cloud-channel-1.9.3/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-channel-1.9.2/tests/unit/gapic/channel_v1/__init__.py` & `google-cloud-channel-1.9.3/tests/unit/gapic/channel_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-channel-1.9.2/tests/unit/gapic/channel_v1/test_cloud_channel_service.py` & `google-cloud-channel-1.9.3/tests/unit/gapic/channel_v1/test_cloud_channel_service.py`

 * *Files identical despite different names*

