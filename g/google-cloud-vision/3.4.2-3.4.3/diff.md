# Comparing `tmp/google-cloud-vision-3.4.2.tar.gz` & `tmp/google-cloud-vision-3.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-vision-3.4.2.tar", last modified: Wed May 31 20:49:38 2023, max compression
+gzip compressed data, was "google-cloud-vision-3.4.3.tar", last modified: Tue Jun 20 15:29:37 2023, max compression
```

## Comparing `google-cloud-vision-3.4.2.tar` & `google-cloud-vision-3.4.3.tar`

### file list

```diff
@@ -1,210 +1,210 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.287655 google-cloud-vision-3.4.2/
--rw-rw-r--   0 root         (0)     1003    11358 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     5881 2023-05-31 20:49:38.287655 google-cloud-vision-3.4.2/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     4968 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.243637 google-cloud-vision-3.4.2/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.247639 google-cloud-vision-3.4.2/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.251640 google-cloud-vision-3.4.2/google/cloud/vision/
--rw-rw-r--   0 root         (0)     1003    10158 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       80 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.251640 google-cloud-vision-3.4.2/google/cloud/vision_helpers/
--rw-rw-r--   0 root         (0)     1003     3638 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_helpers/__init__.py
--rw-rw-r--   0 root         (0)     1003     4181 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_helpers/decorators.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.251640 google-cloud-vision-3.4.2/google/cloud/vision_v1/
--rw-rw-r--   0 root         (0)     1003     8417 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    10150 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       80 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.251640 google-cloud-vision-3.4.2/google/cloud/vision_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.251640 google-cloud-vision-3.4.2/google/cloud/vision_v1/services/image_annotator/
--rw-rw-r--   0 root         (0)     1003      769 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/services/image_annotator/__init__.py
--rw-rw-r--   0 root         (0)     1003    30191 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/services/image_annotator/async_client.py
--rw-rw-r--   0 root         (0)     1003    39070 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/services/image_annotator/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.255642 google-cloud-vision-3.4.2/google/cloud/vision_v1/services/image_annotator/transports/
--rw-rw-r--   0 root         (0)     1003     1418 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/services/image_annotator/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9543 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/services/image_annotator/transports/base.py
--rw-rw-r--   0 root         (0)     1003    17763 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/services/image_annotator/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    18097 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/services/image_annotator/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    33053 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/services/image_annotator/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.255642 google-cloud-vision-3.4.2/google/cloud/vision_v1/services/product_search/
--rw-rw-r--   0 root         (0)     1003      765 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/services/product_search/__init__.py
--rw-rw-r--   0 root         (0)     1003   110841 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/services/product_search/async_client.py
--rw-rw-r--   0 root         (0)     1003   118546 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/services/product_search/client.py
--rw-rw-r--   0 root         (0)     1003    21786 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/services/product_search/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.255642 google-cloud-vision-3.4.2/google/cloud/vision_v1/services/product_search/transports/
--rw-rw-r--   0 root         (0)     1003     1404 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/services/product_search/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    22251 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/services/product_search/transports/base.py
--rw-rw-r--   0 root         (0)     1003    41006 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/services/product_search/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    41751 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/services/product_search/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   106831 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/services/product_search/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.259644 google-cloud-vision-3.4.2/google/cloud/vision_v1/types/
--rw-rw-r--   0 root         (0)     1003     5104 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     3163 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/types/geometry.py
--rw-rw-r--   0 root         (0)     1003    57369 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/types/image_annotator.py
--rw-rw-r--   0 root         (0)     1003     8095 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/types/product_search.py
--rw-rw-r--   0 root         (0)     1003    34296 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/types/product_search_service.py
--rw-rw-r--   0 root         (0)     1003    14108 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/types/text_annotation.py
--rw-rw-r--   0 root         (0)     1003     6798 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/types/web_detection.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.259644 google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/
--rw-rw-r--   0 root         (0)     1003     3530 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003     1073 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       80 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.259644 google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.259644 google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/services/image_annotator/
--rw-rw-r--   0 root         (0)     1003      769 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/services/image_annotator/__init__.py
--rw-rw-r--   0 root         (0)     1003    13774 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/services/image_annotator/async_client.py
--rw-rw-r--   0 root         (0)     1003    22022 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/services/image_annotator/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.259644 google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/services/image_annotator/transports/
--rw-rw-r--   0 root         (0)     1003     1418 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/services/image_annotator/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6594 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/services/image_annotator/transports/base.py
--rw-rw-r--   0 root         (0)     1003    12086 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/services/image_annotator/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    12291 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/services/image_annotator/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    12849 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/services/image_annotator/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.259644 google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/types/
--rw-rw-r--   0 root         (0)     1003     2054 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     2372 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/types/geometry.py
--rw-rw-r--   0 root         (0)     1003    36850 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/types/image_annotator.py
--rw-rw-r--   0 root         (0)     1003    13946 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/types/text_annotation.py
--rw-rw-r--   0 root         (0)     1003     6774 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/types/web_detection.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.263645 google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/
--rw-rw-r--   0 root         (0)     1003     4513 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003     1505 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       80 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.263645 google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.263645 google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/services/image_annotator/
--rw-rw-r--   0 root         (0)     1003      769 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/services/image_annotator/__init__.py
--rw-rw-r--   0 root         (0)     1003    19293 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/services/image_annotator/async_client.py
--rw-rw-r--   0 root         (0)     1003    27363 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/services/image_annotator/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.263645 google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/services/image_annotator/transports/
--rw-rw-r--   0 root         (0)     1003     1418 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/services/image_annotator/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7741 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/services/image_annotator/transports/base.py
--rw-rw-r--   0 root         (0)     1003    14438 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/services/image_annotator/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    14719 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/services/image_annotator/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    19695 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/services/image_annotator/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.263645 google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/types/
--rw-rw-r--   0 root         (0)     1003     2684 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     3184 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/types/geometry.py
--rw-rw-r--   0 root         (0)     1003    47056 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/types/image_annotator.py
--rw-rw-r--   0 root         (0)     1003    14255 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/types/text_annotation.py
--rw-rw-r--   0 root         (0)     1003     6774 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/types/web_detection.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.263645 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/
--rw-rw-r--   0 root         (0)     1003     7754 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003     8961 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       80 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.263645 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.267647 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/image_annotator/
--rw-rw-r--   0 root         (0)     1003      769 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/image_annotator/__init__.py
--rw-rw-r--   0 root         (0)     1003    19480 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/image_annotator/async_client.py
--rw-rw-r--   0 root         (0)     1003    28835 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/image_annotator/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.267647 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/image_annotator/transports/
--rw-rw-r--   0 root         (0)     1003     1418 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/image_annotator/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7602 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/image_annotator/transports/base.py
--rw-rw-r--   0 root         (0)     1003    14454 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/image_annotator/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    14735 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/image_annotator/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    19695 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/image_annotator/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.267647 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/product_search/
--rw-rw-r--   0 root         (0)     1003      765 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/product_search/__init__.py
--rw-rw-r--   0 root         (0)     1003   104793 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/product_search/async_client.py
--rw-rw-r--   0 root         (0)     1003   113091 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/product_search/client.py
--rw-rw-r--   0 root         (0)     1003    22017 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/product_search/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.267647 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/product_search/transports/
--rw-rw-r--   0 root         (0)     1003     1404 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/product_search/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    21005 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/product_search/transports/base.py
--rw-rw-r--   0 root         (0)     1003    39061 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/product_search/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    39775 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/product_search/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   100971 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/product_search/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.271648 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/types/
--rw-rw-r--   0 root         (0)     1003     4658 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     3184 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/types/geometry.py
--rw-rw-r--   0 root         (0)     1003    49756 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/types/image_annotator.py
--rw-rw-r--   0 root         (0)     1003     8172 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/types/product_search.py
--rw-rw-r--   0 root         (0)     1003    31431 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/types/product_search_service.py
--rw-rw-r--   0 root         (0)     1003    14255 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/types/text_annotation.py
--rw-rw-r--   0 root         (0)     1003     6774 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/types/web_detection.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.271648 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/
--rw-rw-r--   0 root         (0)     1003     8625 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003    10164 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       80 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.271648 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.271648 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/image_annotator/
--rw-rw-r--   0 root         (0)     1003      769 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/image_annotator/__init__.py
--rw-rw-r--   0 root         (0)     1003    29872 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/image_annotator/async_client.py
--rw-rw-r--   0 root         (0)     1003    39259 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/image_annotator/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.275650 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/image_annotator/transports/
--rw-rw-r--   0 root         (0)     1003     1418 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/image_annotator/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9001 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/image_annotator/transports/base.py
--rw-rw-r--   0 root         (0)     1003    17798 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/image_annotator/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    18132 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/image_annotator/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    30869 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/image_annotator/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.275650 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/product_search/
--rw-rw-r--   0 root         (0)     1003      765 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/product_search/__init__.py
--rw-rw-r--   0 root         (0)     1003   110849 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/product_search/async_client.py
--rw-rw-r--   0 root         (0)     1003   119297 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/product_search/client.py
--rw-rw-r--   0 root         (0)     1003    22017 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/product_search/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.275650 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/product_search/transports/
--rw-rw-r--   0 root         (0)     1003     1404 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/product_search/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    21446 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/product_search/transports/base.py
--rw-rw-r--   0 root         (0)     1003    41195 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/product_search/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    41940 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/product_search/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   106302 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/product_search/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.279651 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/types/
--rw-rw-r--   0 root         (0)     1003     5270 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     2803 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/types/face.py
--rw-rw-r--   0 root         (0)     1003     3184 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/types/geometry.py
--rw-rw-r--   0 root         (0)     1003    56382 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/types/image_annotator.py
--rw-rw-r--   0 root         (0)     1003     8172 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/types/product_search.py
--rw-rw-r--   0 root         (0)     1003    34408 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/types/product_search_service.py
--rw-rw-r--   0 root         (0)     1003    14255 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/types/text_annotation.py
--rw-rw-r--   0 root         (0)     1003     6861 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/types/web_detection.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.279651 google-cloud-vision-3.4.2/google_cloud_vision.egg-info/
--rw-r--r--   0 root         (0)     1003     5881 2023-05-31 20:49:38.000000 google-cloud-vision-3.4.2/google_cloud_vision.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     8892 2023-05-31 20:49:38.000000 google-cloud-vision-3.4.2/google_cloud_vision.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-05-31 20:49:38.000000 google-cloud-vision-3.4.2/google_cloud_vision.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-05-31 20:49:38.000000 google-cloud-vision-3.4.2/google_cloud_vision.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-05-31 20:49:38.000000 google-cloud-vision-3.4.2/google_cloud_vision.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-05-31 20:49:38.000000 google-cloud-vision-3.4.2/google_cloud_vision.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-05-31 20:49:38.000000 google-cloud-vision-3.4.2/google_cloud_vision.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-05-31 20:49:38.287655 google-cloud-vision-3.4.2/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2917 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.279651 google-cloud-vision-3.4.2/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.279651 google-cloud-vision-3.4.2/tests/data/
--rw-rw-r--   0 root         (0)     1003   283497 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/tests/data/faces.jpg
--rw-rw-r--   0 root         (0)     1003    21568 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/tests/data/logo.png
--rw-rw-r--   0 root         (0)     1003    15615 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/tests/data/pdf_test.pdf
--rw-rw-r--   0 root         (0)     1003    38159 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/tests/system.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.279651 google-cloud-vision-3.4.2/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.279651 google-cloud-vision-3.4.2/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.283653 google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   127996 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1/test_image_annotator.py
--rw-rw-r--   0 root         (0)     1003   460770 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1/test_product_search.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.283653 google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1p1beta1/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1p1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003    70208 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1p1beta1/test_image_annotator.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.283653 google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1p2beta1/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1p2beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003    90057 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1p2beta1/test_image_annotator.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.283653 google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1p3beta1/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1p3beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003    91693 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1p3beta1/test_image_annotator.py
--rw-rw-r--   0 root         (0)     1003   443181 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1p3beta1/test_product_search.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.283653 google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1p4beta1/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1p4beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003   128156 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1p4beta1/test_image_annotator.py
--rw-rw-r--   0 root         (0)     1003   461030 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1p4beta1/test_product_search.py
--rw-rw-r--   0 root         (0)     1003     4068 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/tests/unit/test_decorators.py
--rw-rw-r--   0 root         (0)     1003     5105 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/tests/unit/test_helpers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.798543 google-cloud-vision-3.4.3/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     5795 2023-06-20 15:29:37.798543 google-cloud-vision-3.4.3/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     4882 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.762554 google-cloud-vision-3.4.3/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.762554 google-cloud-vision-3.4.3/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.766553 google-cloud-vision-3.4.3/google/cloud/vision/
+-rw-rw-r--   0 root         (0)     1003    10158 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       80 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.766553 google-cloud-vision-3.4.3/google/cloud/vision_helpers/
+-rw-rw-r--   0 root         (0)     1003     3638 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_helpers/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4181 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_helpers/decorators.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.766553 google-cloud-vision-3.4.3/google/cloud/vision_v1/
+-rw-rw-r--   0 root         (0)     1003     8417 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10150 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       80 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.766553 google-cloud-vision-3.4.3/google/cloud/vision_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.766553 google-cloud-vision-3.4.3/google/cloud/vision_v1/services/image_annotator/
+-rw-rw-r--   0 root         (0)     1003      769 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/services/image_annotator/__init__.py
+-rw-rw-r--   0 root         (0)     1003    30191 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/services/image_annotator/async_client.py
+-rw-rw-r--   0 root         (0)     1003    39070 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/services/image_annotator/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.770551 google-cloud-vision-3.4.3/google/cloud/vision_v1/services/image_annotator/transports/
+-rw-rw-r--   0 root         (0)     1003     1418 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/services/image_annotator/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9543 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/services/image_annotator/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17763 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/services/image_annotator/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    18097 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/services/image_annotator/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    33053 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/services/image_annotator/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.770551 google-cloud-vision-3.4.3/google/cloud/vision_v1/services/product_search/
+-rw-rw-r--   0 root         (0)     1003      765 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/services/product_search/__init__.py
+-rw-rw-r--   0 root         (0)     1003   110841 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/services/product_search/async_client.py
+-rw-rw-r--   0 root         (0)     1003   118546 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/services/product_search/client.py
+-rw-rw-r--   0 root         (0)     1003    21786 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/services/product_search/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.770551 google-cloud-vision-3.4.3/google/cloud/vision_v1/services/product_search/transports/
+-rw-rw-r--   0 root         (0)     1003     1404 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/services/product_search/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    22251 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/services/product_search/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    41006 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/services/product_search/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    41751 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/services/product_search/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   106831 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/services/product_search/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.774550 google-cloud-vision-3.4.3/google/cloud/vision_v1/types/
+-rw-rw-r--   0 root         (0)     1003     5104 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3163 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/types/geometry.py
+-rw-rw-r--   0 root         (0)     1003    57369 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/types/image_annotator.py
+-rw-rw-r--   0 root         (0)     1003     8095 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/types/product_search.py
+-rw-rw-r--   0 root         (0)     1003    34296 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/types/product_search_service.py
+-rw-rw-r--   0 root         (0)     1003    14108 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/types/text_annotation.py
+-rw-rw-r--   0 root         (0)     1003     6798 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/types/web_detection.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.774550 google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/
+-rw-rw-r--   0 root         (0)     1003     3530 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1073 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       80 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.774550 google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.774550 google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/services/image_annotator/
+-rw-rw-r--   0 root         (0)     1003      769 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/services/image_annotator/__init__.py
+-rw-rw-r--   0 root         (0)     1003    13774 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/services/image_annotator/async_client.py
+-rw-rw-r--   0 root         (0)     1003    22022 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/services/image_annotator/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.774550 google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/services/image_annotator/transports/
+-rw-rw-r--   0 root         (0)     1003     1418 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/services/image_annotator/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6594 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/services/image_annotator/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    12086 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/services/image_annotator/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    12291 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/services/image_annotator/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    12849 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/services/image_annotator/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.774550 google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/types/
+-rw-rw-r--   0 root         (0)     1003     2054 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2372 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/types/geometry.py
+-rw-rw-r--   0 root         (0)     1003    36850 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/types/image_annotator.py
+-rw-rw-r--   0 root         (0)     1003    13946 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/types/text_annotation.py
+-rw-rw-r--   0 root         (0)     1003     6774 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/types/web_detection.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.778549 google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/
+-rw-rw-r--   0 root         (0)     1003     4513 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1505 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       80 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.778549 google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.778549 google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/services/image_annotator/
+-rw-rw-r--   0 root         (0)     1003      769 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/services/image_annotator/__init__.py
+-rw-rw-r--   0 root         (0)     1003    19293 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/services/image_annotator/async_client.py
+-rw-rw-r--   0 root         (0)     1003    27363 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/services/image_annotator/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.778549 google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/services/image_annotator/transports/
+-rw-rw-r--   0 root         (0)     1003     1418 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/services/image_annotator/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7741 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/services/image_annotator/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    14438 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/services/image_annotator/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    14719 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/services/image_annotator/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    19695 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/services/image_annotator/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.778549 google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/types/
+-rw-rw-r--   0 root         (0)     1003     2684 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3184 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/types/geometry.py
+-rw-rw-r--   0 root         (0)     1003    47056 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/types/image_annotator.py
+-rw-rw-r--   0 root         (0)     1003    14255 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/types/text_annotation.py
+-rw-rw-r--   0 root         (0)     1003     6774 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/types/web_detection.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.778549 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/
+-rw-rw-r--   0 root         (0)     1003     7754 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8961 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       80 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.778549 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.782548 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/image_annotator/
+-rw-rw-r--   0 root         (0)     1003      769 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/image_annotator/__init__.py
+-rw-rw-r--   0 root         (0)     1003    19480 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/image_annotator/async_client.py
+-rw-rw-r--   0 root         (0)     1003    28835 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/image_annotator/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.782548 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/image_annotator/transports/
+-rw-rw-r--   0 root         (0)     1003     1418 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/image_annotator/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7602 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/image_annotator/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    14454 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/image_annotator/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    14735 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/image_annotator/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    19695 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/image_annotator/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.782548 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/product_search/
+-rw-rw-r--   0 root         (0)     1003      765 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/product_search/__init__.py
+-rw-rw-r--   0 root         (0)     1003   104793 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/product_search/async_client.py
+-rw-rw-r--   0 root         (0)     1003   113091 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/product_search/client.py
+-rw-rw-r--   0 root         (0)     1003    22017 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/product_search/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.782548 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/product_search/transports/
+-rw-rw-r--   0 root         (0)     1003     1404 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/product_search/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    21005 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/product_search/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    39061 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/product_search/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    39775 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/product_search/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   100971 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/product_search/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.786547 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/types/
+-rw-rw-r--   0 root         (0)     1003     4658 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3184 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/types/geometry.py
+-rw-rw-r--   0 root         (0)     1003    49756 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/types/image_annotator.py
+-rw-rw-r--   0 root         (0)     1003     8172 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/types/product_search.py
+-rw-rw-r--   0 root         (0)     1003    31431 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/types/product_search_service.py
+-rw-rw-r--   0 root         (0)     1003    14255 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/types/text_annotation.py
+-rw-rw-r--   0 root         (0)     1003     6774 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/types/web_detection.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.786547 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/
+-rw-rw-r--   0 root         (0)     1003     8625 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10164 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       80 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.786547 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.786547 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/image_annotator/
+-rw-rw-r--   0 root         (0)     1003      769 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/image_annotator/__init__.py
+-rw-rw-r--   0 root         (0)     1003    29872 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/image_annotator/async_client.py
+-rw-rw-r--   0 root         (0)     1003    39259 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/image_annotator/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.786547 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/image_annotator/transports/
+-rw-rw-r--   0 root         (0)     1003     1418 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/image_annotator/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9001 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/image_annotator/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17798 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/image_annotator/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    18132 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/image_annotator/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    30869 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/image_annotator/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.790545 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/product_search/
+-rw-rw-r--   0 root         (0)     1003      765 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/product_search/__init__.py
+-rw-rw-r--   0 root         (0)     1003   110849 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/product_search/async_client.py
+-rw-rw-r--   0 root         (0)     1003   119297 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/product_search/client.py
+-rw-rw-r--   0 root         (0)     1003    22017 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/product_search/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.790545 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/product_search/transports/
+-rw-rw-r--   0 root         (0)     1003     1404 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/product_search/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    21446 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/product_search/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    41195 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/product_search/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    41940 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/product_search/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   106302 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/product_search/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.790545 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/types/
+-rw-rw-r--   0 root         (0)     1003     5270 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2803 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/types/face.py
+-rw-rw-r--   0 root         (0)     1003     3184 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/types/geometry.py
+-rw-rw-r--   0 root         (0)     1003    56382 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/types/image_annotator.py
+-rw-rw-r--   0 root         (0)     1003     8172 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/types/product_search.py
+-rw-rw-r--   0 root         (0)     1003    34408 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/types/product_search_service.py
+-rw-rw-r--   0 root         (0)     1003    14255 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/types/text_annotation.py
+-rw-rw-r--   0 root         (0)     1003     6861 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/types/web_detection.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.794544 google-cloud-vision-3.4.3/google_cloud_vision.egg-info/
+-rw-r--r--   0 root         (0)     1003     5795 2023-06-20 15:29:37.000000 google-cloud-vision-3.4.3/google_cloud_vision.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     8892 2023-06-20 15:29:37.000000 google-cloud-vision-3.4.3/google_cloud_vision.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-06-20 15:29:37.000000 google-cloud-vision-3.4.3/google_cloud_vision.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-06-20 15:29:37.000000 google-cloud-vision-3.4.3/google_cloud_vision.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-06-20 15:29:37.000000 google-cloud-vision-3.4.3/google_cloud_vision.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-06-20 15:29:37.000000 google-cloud-vision-3.4.3/google_cloud_vision.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-06-20 15:29:37.000000 google-cloud-vision-3.4.3/google_cloud_vision.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-06-20 15:29:37.802542 google-cloud-vision-3.4.3/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2917 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.794544 google-cloud-vision-3.4.3/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.794544 google-cloud-vision-3.4.3/tests/data/
+-rw-rw-r--   0 root         (0)     1003   283497 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/tests/data/faces.jpg
+-rw-rw-r--   0 root         (0)     1003    21568 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/tests/data/logo.png
+-rw-rw-r--   0 root         (0)     1003    15615 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/tests/data/pdf_test.pdf
+-rw-rw-r--   0 root         (0)     1003    38159 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/tests/system.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.794544 google-cloud-vision-3.4.3/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.794544 google-cloud-vision-3.4.3/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.794544 google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   127996 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1/test_image_annotator.py
+-rw-rw-r--   0 root         (0)     1003   460770 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1/test_product_search.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.798543 google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1p1beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1p1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    70208 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1p1beta1/test_image_annotator.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.798543 google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1p2beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1p2beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    90057 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1p2beta1/test_image_annotator.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.798543 google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1p3beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1p3beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    91693 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1p3beta1/test_image_annotator.py
+-rw-rw-r--   0 root         (0)     1003   443181 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1p3beta1/test_product_search.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.798543 google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1p4beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1p4beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   128156 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1p4beta1/test_image_annotator.py
+-rw-rw-r--   0 root         (0)     1003   461030 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1p4beta1/test_product_search.py
+-rw-rw-r--   0 root         (0)     1003     4068 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/tests/unit/test_decorators.py
+-rw-rw-r--   0 root         (0)     1003     5105 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/tests/unit/test_helpers.py
```

### Comparing `google-cloud-vision-3.4.2/LICENSE` & `google-cloud-vision-3.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/MANIFEST.in` & `google-cloud-vision-3.4.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/PKG-INFO` & `google-cloud-vision-3.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-vision
-Version: 3.4.2
+Version: 3.4.3
 Summary: Google Cloud Vision API client library
 Home-page: https://github.com/googleapis/python-vision
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
@@ -91,15 +91,15 @@
 ^^^^^^^^^^^^^^^^^^^^^^^^^^
 Python == 2.7.
 
 The last version of this library compatible with Python 2.7 is google-cloud-vision==1.0.0.
 
 RaspberryPi ARM devices 
 ^^^^^^^^^^^^^^^^^^^^^^^
-Note: Raspberry Pi ARMv6 is not supported because there is an internal binary google that does not comply with armv6 processors.
+Note: Raspberry Pi ARMv6 is not supported.
 
 Mac/Linux
 ^^^^^^^^^
 
 .. code-block:: console
 
     pip install virtualenv
```

### Comparing `google-cloud-vision-3.4.2/README.rst` & `google-cloud-vision-3.4.3/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 ^^^^^^^^^^^^^^^^^^^^^^^^^^
 Python == 2.7.
 
 The last version of this library compatible with Python 2.7 is google-cloud-vision==1.0.0.
 
 RaspberryPi ARM devices 
 ^^^^^^^^^^^^^^^^^^^^^^^
-Note: Raspberry Pi ARMv6 is not supported because there is an internal binary google that does not comply with armv6 processors.
+Note: Raspberry Pi ARMv6 is not supported.
 
 Mac/Linux
 ^^^^^^^^^
 
 .. code-block:: console
 
     pip install virtualenv
```

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision/__init__.py` & `google-cloud-vision-3.4.3/google/cloud/vision/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision/gapic_version.py` & `google-cloud-vision-3.4.3/google/cloud/vision/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "3.4.2"  # {x-release-please-version}
+__version__ = "3.4.3"  # {x-release-please-version}
```

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_helpers/__init__.py` & `google-cloud-vision-3.4.3/google/cloud/vision_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_helpers/decorators.py` & `google-cloud-vision-3.4.3/google/cloud/vision_helpers/decorators.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1/__init__.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1/gapic_metadata.json` & `google-cloud-vision-3.4.3/google/cloud/vision_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1/gapic_version.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "3.4.2"  # {x-release-please-version}
+__version__ = "3.4.3"  # {x-release-please-version}
```

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1/services/__init__.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1/services/image_annotator/__init__.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1/services/image_annotator/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1/services/image_annotator/async_client.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1/services/image_annotator/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1/services/image_annotator/client.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1/services/image_annotator/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1/services/image_annotator/transports/__init__.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1/services/image_annotator/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1/services/image_annotator/transports/base.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1/services/image_annotator/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1/services/image_annotator/transports/grpc.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1/services/image_annotator/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1/services/image_annotator/transports/grpc_asyncio.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1/services/image_annotator/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1/services/image_annotator/transports/rest.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1/services/image_annotator/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1/services/product_search/__init__.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1/services/product_search/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1/services/product_search/async_client.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1/services/product_search/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1/services/product_search/client.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1/services/product_search/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1/services/product_search/pagers.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1/services/product_search/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1/services/product_search/transports/__init__.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1/services/product_search/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1/services/product_search/transports/base.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1/services/product_search/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1/services/product_search/transports/grpc.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1/services/product_search/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1/services/product_search/transports/grpc_asyncio.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1/services/product_search/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1/services/product_search/transports/rest.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1/services/product_search/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1/types/__init__.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1/types/geometry.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1/types/geometry.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1/types/image_annotator.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1/types/image_annotator.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1/types/product_search.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1/types/product_search.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1/types/product_search_service.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1/types/product_search_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1/types/text_annotation.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1/types/text_annotation.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1/types/web_detection.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1/types/web_detection.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/__init__.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/gapic_metadata.json` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/gapic_version.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "3.4.2"  # {x-release-please-version}
+__version__ = "3.4.3"  # {x-release-please-version}
```

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/services/__init__.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/services/image_annotator/__init__.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/services/image_annotator/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/services/image_annotator/async_client.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/services/image_annotator/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/services/image_annotator/client.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/services/image_annotator/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/services/image_annotator/transports/__init__.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/services/image_annotator/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/services/image_annotator/transports/base.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/services/image_annotator/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/services/image_annotator/transports/grpc.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/services/image_annotator/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/services/image_annotator/transports/grpc_asyncio.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/services/image_annotator/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/services/image_annotator/transports/rest.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/services/image_annotator/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/types/__init__.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/types/geometry.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/types/geometry.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/types/image_annotator.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/types/image_annotator.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/types/text_annotation.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/types/text_annotation.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/types/web_detection.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/types/web_detection.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/__init__.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/gapic_metadata.json` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/gapic_version.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "3.4.2"  # {x-release-please-version}
+__version__ = "3.4.3"  # {x-release-please-version}
```

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/services/__init__.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/services/image_annotator/__init__.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/services/image_annotator/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/services/image_annotator/async_client.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/services/image_annotator/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/services/image_annotator/client.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/services/image_annotator/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/services/image_annotator/transports/__init__.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/services/image_annotator/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/services/image_annotator/transports/base.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/services/image_annotator/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/services/image_annotator/transports/grpc.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/services/image_annotator/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/services/image_annotator/transports/grpc_asyncio.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/services/image_annotator/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/services/image_annotator/transports/rest.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/services/image_annotator/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/types/__init__.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/types/geometry.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/types/geometry.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/types/image_annotator.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/types/image_annotator.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/types/text_annotation.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/types/text_annotation.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/types/web_detection.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/types/web_detection.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/__init__.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/gapic_metadata.json` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/gapic_version.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "3.4.2"  # {x-release-please-version}
+__version__ = "3.4.3"  # {x-release-please-version}
```

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/__init__.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/image_annotator/__init__.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/image_annotator/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/image_annotator/async_client.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/image_annotator/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/image_annotator/client.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/image_annotator/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/image_annotator/transports/__init__.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/image_annotator/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/image_annotator/transports/base.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/image_annotator/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/image_annotator/transports/grpc.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/image_annotator/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/image_annotator/transports/grpc_asyncio.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/image_annotator/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/image_annotator/transports/rest.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/image_annotator/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/product_search/__init__.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/product_search/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/product_search/async_client.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/product_search/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/product_search/client.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/product_search/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/product_search/pagers.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/product_search/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/product_search/transports/__init__.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/product_search/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/product_search/transports/base.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/product_search/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/product_search/transports/grpc.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/product_search/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/product_search/transports/grpc_asyncio.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/product_search/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/product_search/transports/rest.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/product_search/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/types/__init__.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/types/geometry.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/types/geometry.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/types/image_annotator.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/types/image_annotator.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/types/product_search.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/types/product_search.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/types/product_search_service.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/types/product_search_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/types/text_annotation.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/types/text_annotation.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/types/web_detection.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/types/web_detection.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/__init__.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/gapic_metadata.json` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/gapic_version.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "3.4.2"  # {x-release-please-version}
+__version__ = "3.4.3"  # {x-release-please-version}
```

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/__init__.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/image_annotator/__init__.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/image_annotator/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/image_annotator/async_client.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/image_annotator/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/image_annotator/client.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/image_annotator/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/image_annotator/transports/__init__.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/image_annotator/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/image_annotator/transports/base.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/image_annotator/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/image_annotator/transports/grpc.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/image_annotator/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/image_annotator/transports/grpc_asyncio.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/image_annotator/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/image_annotator/transports/rest.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/image_annotator/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/product_search/__init__.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/product_search/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/product_search/async_client.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/product_search/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/product_search/client.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/product_search/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/product_search/pagers.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/product_search/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/product_search/transports/__init__.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/product_search/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/product_search/transports/base.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/product_search/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/product_search/transports/grpc.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/product_search/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/product_search/transports/grpc_asyncio.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/product_search/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/product_search/transports/rest.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/product_search/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/types/__init__.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/types/face.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/types/face.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/types/geometry.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/types/geometry.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/types/image_annotator.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/types/image_annotator.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/types/product_search.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/types/product_search.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/types/product_search_service.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/types/product_search_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/types/text_annotation.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/types/text_annotation.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/types/web_detection.py` & `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/types/web_detection.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/google_cloud_vision.egg-info/PKG-INFO` & `google-cloud-vision-3.4.3/google_cloud_vision.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-vision
-Version: 3.4.2
+Version: 3.4.3
 Summary: Google Cloud Vision API client library
 Home-page: https://github.com/googleapis/python-vision
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
@@ -91,15 +91,15 @@
 ^^^^^^^^^^^^^^^^^^^^^^^^^^
 Python == 2.7.
 
 The last version of this library compatible with Python 2.7 is google-cloud-vision==1.0.0.
 
 RaspberryPi ARM devices 
 ^^^^^^^^^^^^^^^^^^^^^^^
-Note: Raspberry Pi ARMv6 is not supported because there is an internal binary google that does not comply with armv6 processors.
+Note: Raspberry Pi ARMv6 is not supported.
 
 Mac/Linux
 ^^^^^^^^^
 
 .. code-block:: console
 
     pip install virtualenv
```

### Comparing `google-cloud-vision-3.4.2/google_cloud_vision.egg-info/SOURCES.txt` & `google-cloud-vision-3.4.3/google_cloud_vision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/setup.py` & `google-cloud-vision-3.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/tests/__init__.py` & `google-cloud-vision-3.4.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/tests/data/faces.jpg` & `google-cloud-vision-3.4.3/tests/data/faces.jpg`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/tests/data/logo.png` & `google-cloud-vision-3.4.3/tests/data/logo.png`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/tests/data/pdf_test.pdf` & `google-cloud-vision-3.4.3/tests/data/pdf_test.pdf`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/tests/system.py` & `google-cloud-vision-3.4.3/tests/system.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/tests/unit/__init__.py` & `google-cloud-vision-3.4.3/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/tests/unit/gapic/__init__.py` & `google-cloud-vision-3.4.3/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1/__init__.py` & `google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1/test_image_annotator.py` & `google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1/test_image_annotator.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1/test_product_search.py` & `google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1/test_product_search.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1p1beta1/__init__.py` & `google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1p1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1p1beta1/test_image_annotator.py` & `google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1p1beta1/test_image_annotator.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1p2beta1/__init__.py` & `google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1p2beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1p2beta1/test_image_annotator.py` & `google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1p2beta1/test_image_annotator.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1p3beta1/__init__.py` & `google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1p3beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1p3beta1/test_image_annotator.py` & `google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1p3beta1/test_image_annotator.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1p3beta1/test_product_search.py` & `google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1p3beta1/test_product_search.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1p4beta1/__init__.py` & `google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1p4beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1p4beta1/test_image_annotator.py` & `google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1p4beta1/test_image_annotator.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1p4beta1/test_product_search.py` & `google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1p4beta1/test_product_search.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/tests/unit/test_decorators.py` & `google-cloud-vision-3.4.3/tests/unit/test_decorators.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.2/tests/unit/test_helpers.py` & `google-cloud-vision-3.4.3/tests/unit/test_helpers.py`

 * *Files identical despite different names*

