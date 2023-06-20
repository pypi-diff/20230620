# Comparing `tmp/google-cloud-discoveryengine-0.8.1.tar.gz` & `tmp/google-cloud-discoveryengine-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-discoveryengine-0.8.1.tar", last modified: Wed Jun  7 15:37:20 2023, max compression
+gzip compressed data, was "google-cloud-discoveryengine-0.9.0.tar", last modified: Tue Jun 20 13:27:20 2023, max compression
```

## Comparing `google-cloud-discoveryengine-0.8.1.tar` & `google-cloud-discoveryengine-0.9.0.tar`

### file list

```diff
@@ -1,199 +1,199 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.706534 google-cloud-discoveryengine-0.8.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4587 2023-06-07 15:37:20.706534 google-cloud-discoveryengine-0.8.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3663 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.670532 google-cloud-discoveryengine-0.8.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.674532 google-cloud-discoveryengine-0.8.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.674532 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine/
--rw-rw-r--   0 root         (0)     1003     5697 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.678532 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/
--rw-rw-r--   0 root         (0)     1003     4020 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     8490 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.678532 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.678532 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/completion_service/
--rw-rw-r--   0 root         (0)     1003      781 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/completion_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    17074 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/completion_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    26167 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/completion_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.678532 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/completion_service/transports/
--rw-rw-r--   0 root         (0)     1003     1442 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/completion_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6703 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/completion_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13608 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/completion_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13816 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/completion_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    23102 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/completion_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.678532 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/document_service/
--rw-rw-r--   0 root         (0)     1003      773 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/document_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    47501 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/document_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    58096 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/document_service/client.py
--rw-rw-r--   0 root         (0)     1003     5885 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/document_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.682533 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/document_service/transports/
--rw-rw-r--   0 root         (0)     1003     1414 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/document_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    10026 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/document_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    22476 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/document_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    22924 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/document_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    60840 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/document_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.682533 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/schema_service/
--rw-rw-r--   0 root         (0)     1003      765 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/schema_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    38042 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/schema_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    48349 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/schema_service/client.py
--rw-rw-r--   0 root         (0)     1003     5793 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/schema_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.682533 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/schema_service/transports/
--rw-rw-r--   0 root         (0)     1003     1386 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/schema_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8545 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/schema_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    18663 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/schema_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    19066 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/schema_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    49720 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/schema_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.682533 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/search_service/
--rw-rw-r--   0 root         (0)     1003      765 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/search_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    17593 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/search_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    28224 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/search_service/client.py
--rw-rw-r--   0 root         (0)     1003     5721 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/search_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.682533 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/search_service/transports/
--rw-rw-r--   0 root         (0)     1003     1386 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/search_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6595 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/search_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13393 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/search_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13611 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/search_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    22989 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/search_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.686533 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/user_event_service/
--rw-rw-r--   0 root         (0)     1003      777 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/user_event_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    27405 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/user_event_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    37270 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/user_event_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.686533 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/user_event_service/transports/
--rw-rw-r--   0 root         (0)     1003     1428 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/user_event_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8157 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/user_event_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    17214 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/user_event_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    17552 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/user_event_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    41428 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/user_event_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.686533 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/types/
--rw-rw-r--   0 root         (0)     1003     3050 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     3977 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/types/common.py
--rw-rw-r--   0 root         (0)     1003     4614 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/types/completion_service.py
--rw-rw-r--   0 root         (0)     1003     6357 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/types/document.py
--rw-rw-r--   0 root         (0)     1003     9309 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/types/document_service.py
--rw-rw-r--   0 root         (0)     1003    21849 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/types/import_config.py
--rw-rw-r--   0 root         (0)     1003     4073 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/types/purge_config.py
--rw-rw-r--   0 root         (0)     1003     2392 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/types/schema.py
--rw-rw-r--   0 root         (0)     1003     8915 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/types/schema_service.py
--rw-rw-r--   0 root         (0)     1003    16487 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/types/search_service.py
--rw-rw-r--   0 root         (0)     1003    27255 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/types/user_event.py
--rw-rw-r--   0 root         (0)     1003     3424 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/types/user_event_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.690533 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/
--rw-rw-r--   0 root         (0)     1003     4372 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/__init__.py
--rw-rw-r--   0 root         (0)     1003     9266 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.690533 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.690533 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/completion_service/
--rw-rw-r--   0 root         (0)     1003      781 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/completion_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    17110 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/completion_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    26203 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/completion_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.690533 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/completion_service/transports/
--rw-rw-r--   0 root         (0)     1003     1442 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/completion_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6711 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/completion_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13616 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/completion_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13824 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/completion_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    22926 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/completion_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.690533 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/document_service/
--rw-rw-r--   0 root         (0)     1003      773 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/document_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    47829 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/document_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    58424 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/document_service/client.py
--rw-rw-r--   0 root         (0)     1003     5921 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/document_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.690533 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/document_service/transports/
--rw-rw-r--   0 root         (0)     1003     1414 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/document_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    10042 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/document_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    22600 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/document_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    23048 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/document_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    60520 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/document_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.694534 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/
--rw-rw-r--   0 root         (0)     1003      797 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    17422 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    27322 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.694534 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/
--rw-rw-r--   0 root         (0)     1003     1519 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6712 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13617 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13829 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    23083 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.694534 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/schema_service/
--rw-rw-r--   0 root         (0)     1003      765 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/schema_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    38222 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/schema_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    48529 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/schema_service/client.py
--rw-rw-r--   0 root         (0)     1003     5829 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/schema_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.694534 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/schema_service/transports/
--rw-rw-r--   0 root         (0)     1003     1386 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/schema_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8553 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/schema_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    18711 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/schema_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    19114 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/schema_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    49372 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/schema_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.698534 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/search_service/
--rw-rw-r--   0 root         (0)     1003      765 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/search_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    17633 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/search_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    28264 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/search_service/client.py
--rw-rw-r--   0 root         (0)     1003     5757 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/search_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.698534 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/search_service/transports/
--rw-rw-r--   0 root         (0)     1003     1386 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/search_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6603 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/search_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13401 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/search_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13619 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/search_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    22813 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/search_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.698534 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/user_event_service/
--rw-rw-r--   0 root         (0)     1003      777 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/user_event_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    27473 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/user_event_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    37338 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/user_event_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.698534 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/
--rw-rw-r--   0 root         (0)     1003     1428 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8165 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    17230 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    17568 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    41036 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.702534 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/types/
--rw-rw-r--   0 root         (0)     1003     3197 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     5368 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/types/common.py
--rw-rw-r--   0 root         (0)     1003     4646 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/types/completion_service.py
--rw-rw-r--   0 root         (0)     1003     6373 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/types/document.py
--rw-rw-r--   0 root         (0)     1003     9481 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/types/document_service.py
--rw-rw-r--   0 root         (0)     1003    22061 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/types/import_config.py
--rw-rw-r--   0 root         (0)     1003     4085 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/types/purge_config.py
--rw-rw-r--   0 root         (0)     1003    10788 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/types/recommendation_service.py
--rw-rw-r--   0 root         (0)     1003     2396 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/types/schema.py
--rw-rw-r--   0 root         (0)     1003     9031 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/types/schema_service.py
--rw-rw-r--   0 root         (0)     1003    37375 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/types/search_service.py
--rw-rw-r--   0 root         (0)     1003    27718 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/types/user_event.py
--rw-rw-r--   0 root         (0)     1003     3436 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/types/user_event_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.702534 google-cloud-discoveryengine-0.8.1/google_cloud_discoveryengine.egg-info/
--rw-r--r--   0 root         (0)     1003     4587 2023-06-07 15:37:20.000000 google-cloud-discoveryengine-0.8.1/google_cloud_discoveryengine.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003    10665 2023-06-07 15:37:20.000000 google-cloud-discoveryengine-0.8.1/google_cloud_discoveryengine.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-06-07 15:37:20.000000 google-cloud-discoveryengine-0.8.1/google_cloud_discoveryengine.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-06-07 15:37:20.000000 google-cloud-discoveryengine-0.8.1/google_cloud_discoveryengine.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-06-07 15:37:20.000000 google-cloud-discoveryengine-0.8.1/google_cloud_discoveryengine.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-06-07 15:37:20.000000 google-cloud-discoveryengine-0.8.1/google_cloud_discoveryengine.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-06-07 15:37:20.000000 google-cloud-discoveryengine-0.8.1/google_cloud_discoveryengine.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2023-06-07 15:37:20.706534 google-cloud-discoveryengine-0.8.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2956 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.702534 google-cloud-discoveryengine-0.8.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.702534 google-cloud-discoveryengine-0.8.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.702534 google-cloud-discoveryengine-0.8.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.706534 google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    83160 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1/test_completion_service.py
--rw-rw-r--   0 root         (0)     1003   201237 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1/test_document_service.py
--rw-rw-r--   0 root         (0)     1003   168146 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1/test_schema_service.py
--rw-rw-r--   0 root         (0)     1003    93087 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1/test_search_service.py
--rw-rw-r--   0 root         (0)     1003   119289 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1/test_user_event_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.706534 google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1beta/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1beta/__init__.py
--rw-rw-r--   0 root         (0)     1003    83584 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1beta/test_completion_service.py
--rw-rw-r--   0 root         (0)     1003   201685 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1beta/test_document_service.py
--rw-rw-r--   0 root         (0)     1003    86195 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1beta/test_recommendation_service.py
--rw-rw-r--   0 root         (0)     1003   168594 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1beta/test_schema_service.py
--rw-rw-r--   0 root         (0)     1003    93887 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1beta/test_search_service.py
--rw-rw-r--   0 root         (0)     1003   119713 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1beta/test_user_event_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.875496 google-cloud-discoveryengine-0.9.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4587 2023-06-20 13:27:20.875496 google-cloud-discoveryengine-0.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3663 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.835491 google-cloud-discoveryengine-0.9.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.839492 google-cloud-discoveryengine-0.9.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.843492 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine/
+-rw-rw-r--   0 root         (0)     1003     5697 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.843492 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/
+-rw-rw-r--   0 root         (0)     1003     4020 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8490 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.843492 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.843492 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/completion_service/
+-rw-rw-r--   0 root         (0)     1003      781 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/completion_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    17074 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/completion_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    26167 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/completion_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.843492 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/completion_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1442 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/completion_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6703 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/completion_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13608 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/completion_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13816 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/completion_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    23102 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/completion_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.843492 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/document_service/
+-rw-rw-r--   0 root         (0)     1003      773 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/document_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    47501 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/document_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    58096 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/document_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5885 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/document_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.847493 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/document_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1414 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/document_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10026 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/document_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    22476 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/document_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    22924 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/document_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    60840 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/document_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.847493 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/schema_service/
+-rw-rw-r--   0 root         (0)     1003      765 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/schema_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    38042 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/schema_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    48349 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/schema_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5793 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/schema_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.847493 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/schema_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1386 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/schema_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8545 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/schema_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    18663 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/schema_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    19066 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/schema_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    49720 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/schema_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.847493 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/search_service/
+-rw-rw-r--   0 root         (0)     1003      765 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/search_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    17593 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/search_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    28224 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/search_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5721 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/search_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.851493 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/search_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1386 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/search_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6595 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/search_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13393 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/search_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13611 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/search_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    22989 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/search_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.851493 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/user_event_service/
+-rw-rw-r--   0 root         (0)     1003      777 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/user_event_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    27405 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/user_event_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    37270 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/user_event_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.851493 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/user_event_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1428 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/user_event_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8157 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/user_event_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17214 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/user_event_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    17552 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/user_event_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    41428 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/user_event_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.855494 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/types/
+-rw-rw-r--   0 root         (0)     1003     3050 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3977 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/types/common.py
+-rw-rw-r--   0 root         (0)     1003     4614 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/types/completion_service.py
+-rw-rw-r--   0 root         (0)     1003     6357 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/types/document.py
+-rw-rw-r--   0 root         (0)     1003     9309 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/types/document_service.py
+-rw-rw-r--   0 root         (0)     1003    21849 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/types/import_config.py
+-rw-rw-r--   0 root         (0)     1003     4073 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/types/purge_config.py
+-rw-rw-r--   0 root         (0)     1003     2392 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/types/schema.py
+-rw-rw-r--   0 root         (0)     1003     8915 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/types/schema_service.py
+-rw-rw-r--   0 root         (0)     1003    16487 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/types/search_service.py
+-rw-rw-r--   0 root         (0)     1003    27255 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/types/user_event.py
+-rw-rw-r--   0 root         (0)     1003     3424 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/types/user_event_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.855494 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/
+-rw-rw-r--   0 root         (0)     1003     4372 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9266 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.855494 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.855494 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/completion_service/
+-rw-rw-r--   0 root         (0)     1003      781 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/completion_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    17110 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/completion_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    26203 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/completion_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.855494 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1442 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6711 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13616 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13824 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    22926 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.855494 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/document_service/
+-rw-rw-r--   0 root         (0)     1003      773 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/document_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    47829 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/document_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    58424 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/document_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5921 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/document_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.859494 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1414 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10042 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    22600 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    23048 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    60520 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.859494 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/
+-rw-rw-r--   0 root         (0)     1003      797 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    17422 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    27322 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.859494 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1519 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6712 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13617 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13829 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    23083 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.859494 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/schema_service/
+-rw-rw-r--   0 root         (0)     1003      765 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/schema_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    38222 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/schema_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    48529 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/schema_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5829 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/schema_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.863494 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1386 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8553 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    18711 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    19114 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    49372 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.863494 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/search_service/
+-rw-rw-r--   0 root         (0)     1003      765 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/search_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    17633 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/search_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    28264 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/search_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5757 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/search_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.863494 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1386 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6603 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13401 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13619 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    22813 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.863494 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/user_event_service/
+-rw-rw-r--   0 root         (0)     1003      777 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/user_event_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    27473 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/user_event_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    37338 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/user_event_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.867495 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1428 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8165 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17230 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    17568 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    41036 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.867495 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/types/
+-rw-rw-r--   0 root         (0)     1003     3197 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     5368 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/types/common.py
+-rw-rw-r--   0 root         (0)     1003     4809 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/types/completion_service.py
+-rw-rw-r--   0 root         (0)     1003     6716 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/types/document.py
+-rw-rw-r--   0 root         (0)     1003     9481 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/types/document_service.py
+-rw-rw-r--   0 root         (0)     1003    22350 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/types/import_config.py
+-rw-rw-r--   0 root         (0)     1003     4085 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/types/purge_config.py
+-rw-rw-r--   0 root         (0)     1003    10788 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/types/recommendation_service.py
+-rw-rw-r--   0 root         (0)     1003     2396 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/types/schema.py
+-rw-rw-r--   0 root         (0)     1003     9031 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/types/schema_service.py
+-rw-rw-r--   0 root         (0)     1003    40476 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/types/search_service.py
+-rw-rw-r--   0 root         (0)     1003    27718 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/types/user_event.py
+-rw-rw-r--   0 root         (0)     1003     3436 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/types/user_event_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.871495 google-cloud-discoveryengine-0.9.0/google_cloud_discoveryengine.egg-info/
+-rw-r--r--   0 root         (0)     1003     4587 2023-06-20 13:27:20.000000 google-cloud-discoveryengine-0.9.0/google_cloud_discoveryengine.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003    10665 2023-06-20 13:27:20.000000 google-cloud-discoveryengine-0.9.0/google_cloud_discoveryengine.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-06-20 13:27:20.000000 google-cloud-discoveryengine-0.9.0/google_cloud_discoveryengine.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-06-20 13:27:20.000000 google-cloud-discoveryengine-0.9.0/google_cloud_discoveryengine.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-06-20 13:27:20.000000 google-cloud-discoveryengine-0.9.0/google_cloud_discoveryengine.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-06-20 13:27:20.000000 google-cloud-discoveryengine-0.9.0/google_cloud_discoveryengine.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-06-20 13:27:20.000000 google-cloud-discoveryengine-0.9.0/google_cloud_discoveryengine.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2023-06-20 13:27:20.875496 google-cloud-discoveryengine-0.9.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2956 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.871495 google-cloud-discoveryengine-0.9.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.871495 google-cloud-discoveryengine-0.9.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.871495 google-cloud-discoveryengine-0.9.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.871495 google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    83160 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1/test_completion_service.py
+-rw-rw-r--   0 root         (0)     1003   201237 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1/test_document_service.py
+-rw-rw-r--   0 root         (0)     1003   168146 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1/test_schema_service.py
+-rw-rw-r--   0 root         (0)     1003    93087 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1/test_search_service.py
+-rw-rw-r--   0 root         (0)     1003   119289 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1/test_user_event_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.875496 google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1beta/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003    83584 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1beta/test_completion_service.py
+-rw-rw-r--   0 root         (0)     1003   201685 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1beta/test_document_service.py
+-rw-rw-r--   0 root         (0)     1003    86195 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1beta/test_recommendation_service.py
+-rw-rw-r--   0 root         (0)     1003   168594 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1beta/test_schema_service.py
+-rw-rw-r--   0 root         (0)     1003    94203 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1beta/test_search_service.py
+-rw-rw-r--   0 root         (0)     1003   119544 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1beta/test_user_event_service.py
```

### Comparing `google-cloud-discoveryengine-0.8.1/LICENSE` & `google-cloud-discoveryengine-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/MANIFEST.in` & `google-cloud-discoveryengine-0.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/PKG-INFO` & `google-cloud-discoveryengine-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-discoveryengine
-Version: 0.8.1
+Version: 0.9.0
 Summary: Google Cloud Discoveryengine API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-discoveryengine-0.8.1/README.rst` & `google-cloud-discoveryengine-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine/__init__.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine/gapic_version.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine/gapic_version.py`

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
-__version__ = "0.8.1"  # {x-release-please-version}
+__version__ = "0.9.0"  # {x-release-please-version}
```

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/__init__.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/gapic_metadata.json` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/gapic_version.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/gapic_version.py`

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
-__version__ = "0.8.1"  # {x-release-please-version}
+__version__ = "0.9.0"  # {x-release-please-version}
```

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/__init__.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/completion_service/__init__.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/completion_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/completion_service/async_client.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/completion_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/completion_service/client.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/completion_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/completion_service/transports/__init__.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/completion_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/completion_service/transports/base.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/completion_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/completion_service/transports/grpc.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/completion_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/completion_service/transports/grpc_asyncio.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/completion_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/completion_service/transports/rest.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/completion_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/document_service/__init__.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/document_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/document_service/async_client.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/document_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/document_service/client.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/document_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/document_service/pagers.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/document_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/document_service/transports/__init__.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/document_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/document_service/transports/base.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/document_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/document_service/transports/grpc.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/document_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/document_service/transports/grpc_asyncio.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/document_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/document_service/transports/rest.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/document_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/schema_service/__init__.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/schema_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/schema_service/async_client.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/schema_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/schema_service/client.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/schema_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/schema_service/pagers.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/schema_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/schema_service/transports/__init__.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/schema_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/schema_service/transports/base.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/schema_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/schema_service/transports/grpc.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/schema_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/schema_service/transports/grpc_asyncio.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/schema_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/schema_service/transports/rest.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/schema_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/search_service/__init__.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/search_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/search_service/async_client.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/search_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/search_service/client.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/search_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/search_service/pagers.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/search_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/search_service/transports/__init__.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/search_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/search_service/transports/base.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/search_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/search_service/transports/grpc.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/search_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/search_service/transports/grpc_asyncio.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/search_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/search_service/transports/rest.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/search_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/user_event_service/__init__.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/user_event_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/user_event_service/async_client.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/user_event_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/user_event_service/client.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/user_event_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/user_event_service/transports/__init__.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/user_event_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/user_event_service/transports/base.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/user_event_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/user_event_service/transports/grpc.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/user_event_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/user_event_service/transports/grpc_asyncio.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/user_event_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/user_event_service/transports/rest.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/user_event_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/types/__init__.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/types/common.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/types/common.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/types/completion_service.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/types/completion_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/types/document.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/types/document.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/types/document_service.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/types/document_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/types/import_config.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/types/import_config.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/types/purge_config.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/types/purge_config.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/types/schema.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/types/schema.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/types/schema_service.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/types/schema_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/types/search_service.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/types/search_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/types/user_event.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/types/user_event.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/types/user_event_service.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/types/user_event_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/__init__.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/gapic_metadata.json` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/gapic_version.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/gapic_version.py`

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
-__version__ = "0.8.1"  # {x-release-please-version}
+__version__ = "0.9.0"  # {x-release-please-version}
```

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/__init__.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/completion_service/__init__.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/completion_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/completion_service/async_client.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/completion_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/completion_service/client.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/completion_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/completion_service/transports/__init__.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/completion_service/transports/base.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/completion_service/transports/grpc.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/completion_service/transports/grpc_asyncio.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/completion_service/transports/rest.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/document_service/__init__.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/document_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/document_service/async_client.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/document_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/document_service/client.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/document_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/document_service/pagers.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/document_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/document_service/transports/__init__.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/document_service/transports/base.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/document_service/transports/grpc.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/document_service/transports/grpc_asyncio.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/document_service/transports/rest.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/__init__.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/async_client.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/client.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/__init__.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/base.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/grpc.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/grpc_asyncio.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/rest.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/schema_service/__init__.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/schema_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/schema_service/async_client.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/schema_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/schema_service/client.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/schema_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/schema_service/pagers.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/schema_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/schema_service/transports/__init__.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/schema_service/transports/base.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/schema_service/transports/grpc.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/schema_service/transports/grpc_asyncio.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/schema_service/transports/rest.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/search_service/__init__.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/search_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/search_service/async_client.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/search_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/search_service/client.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/search_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/search_service/pagers.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/search_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/search_service/transports/__init__.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/search_service/transports/base.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/search_service/transports/grpc.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/search_service/transports/grpc_asyncio.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/search_service/transports/rest.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/user_event_service/__init__.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/user_event_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/user_event_service/async_client.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/user_event_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/user_event_service/client.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/user_event_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/__init__.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/base.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/grpc.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/grpc_asyncio.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/rest.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/types/__init__.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/types/common.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/types/common.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/types/completion_service.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/types/completion_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,17 @@
             -  ``search-history`` - Using suggestions generated from the
                past history of
                [SearchService.Search][google.cloud.discoveryengine.v1beta.SearchService.Search]
                API calls. Do not use it when there is no traffic for
                Search API.
             -  ``user-event`` - Using suggestions generated from
                user-imported search events.
+            -  ``document-completable`` - Using suggestions taken
+               directly from user-imported document fields marked as
+               completable.
 
             Default values:
 
             -  ``document`` is the default model for regular dataStores.
             -  ``search-history`` is the default model for
                [IndustryVertical.SITE_SEARCH][google.cloud.discoveryengine.v1beta.IndustryVertical.SITE_SEARCH]
                dataStores.
```

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/types/document.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/types/document.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,16 +113,22 @@
                 ``gs://bucket-name/path/to/file``) are supported. The
                 maximum file size is 100 MB.
 
                 This field is a member of `oneof`_ ``content``.
             mime_type (str):
                 The MIME type of the content. Supported types:
 
-                -  ``application/pdf`` (PDF)
+                -  ``application/pdf`` (PDF, only native PDFs are supported
+                   for now)
                 -  ``text/html`` (HTML)
+                -  ``application/vnd.openxmlformats-officedocument.wordprocessingml.document``
+                   (DOCX)
+                -  ``application/vnd.openxmlformats-officedocument.presentationml.presentation``
+                   (PPTX)
+                -  ``text/plain`` (TXT)
 
                 See
                 https://www.iana.org/assignments/media-types/media-types.xhtml.
         """
 
         raw_bytes: bytes = proto.Field(
             proto.BYTES,
```

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/types/document_service.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/types/document_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/types/import_config.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/types/import_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,19 @@
                with the ID set to the first 128 bits of SHA256(URI)
                encoded as a hex string.
             -  ``custom``: One custom data JSON per row in arbitrary
                format that conforms the defined
                [Schema][google.cloud.discoveryengine.v1beta.Schema] of
                the data store. This can only be used by the GENERIC Data
                Store vertical.
+            -  ``csv``: A CSV file with header conforming the defined
+               [Schema][google.cloud.discoveryengine.v1beta.Schema] of
+               the data store. Each entry after the header will be
+               imported as a Document. This can only be used by the
+               GENERIC Data Store vertical.
 
             Supported values for user even imports:
 
             -  ``user_event`` (default): One JSON
                [UserEvent][google.cloud.discoveryengine.v1beta.UserEvent]
                per line.
     """
@@ -203,25 +208,24 @@
     Setting any member of the oneof automatically clears all other
     members.
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
     Attributes:
         inline_source (google.cloud.discoveryengine_v1beta.types.ImportUserEventsRequest.InlineSource):
-            Required. The Inline source for the input
-            content for UserEvents.
+            The Inline source for the input content for
+            UserEvents.
 
             This field is a member of `oneof`_ ``source``.
         gcs_source (google.cloud.discoveryengine_v1beta.types.GcsSource):
-            Required. Cloud Storage location for the
-            input content.
+            Cloud Storage location for the input content.
 
             This field is a member of `oneof`_ ``source``.
         bigquery_source (google.cloud.discoveryengine_v1beta.types.BigQuerySource):
-            Required. BigQuery input source.
+            BigQuery input source.
 
             This field is a member of `oneof`_ ``source``.
         parent (str):
             Required. Parent DataStore resource name, of the form
             ``projects/{project}/locations/{location}/collections/{collection}/dataStores/{data_store}``
         error_config (google.cloud.discoveryengine_v1beta.types.ImportErrorConfig):
             The desired location of errors incurred
@@ -450,16 +454,16 @@
             [GcsSource][google.cloud.discoveryengine.v1beta.GcsSource]
             or
             [BigQuerySource][google.cloud.discoveryengine.v1beta.BigQuerySource],
             and when
             [GcsSource.data_schema][google.cloud.discoveryengine.v1beta.GcsSource.data_schema]
             or
             [BigQuerySource.data_schema][google.cloud.discoveryengine.v1beta.BigQuerySource.data_schema]
-            is ``custom``. Otherwise, an INVALID_ARGUMENT error is
-            thrown.
+            is ``custom`` or ``csv``. Otherwise, an INVALID_ARGUMENT
+            error is thrown.
         id_field (str):
             The field in the Cloud Storage and BigQuery sources that
             indicates the unique IDs of the documents.
 
             For
             [GcsSource][google.cloud.discoveryengine.v1beta.GcsSource]
             it is the key of the JSON field. For instance, ``my_id`` for
```

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/types/purge_config.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/types/purge_config.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/types/recommendation_service.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/types/recommendation_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/types/schema.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/types/schema.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/types/schema_service.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/types/schema_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/types/search_service.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/types/search_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -522,24 +522,31 @@
         Attributes:
             snippet_spec (google.cloud.discoveryengine_v1beta.types.SearchRequest.ContentSearchSpec.SnippetSpec):
                 If there is no snippet spec provided, there
                 will be no snippet in the search result.
             summary_spec (google.cloud.discoveryengine_v1beta.types.SearchRequest.ContentSearchSpec.SummarySpec):
                 If there is no summary spec provided, there
                 will be no summary in the search response.
+            extractive_content_spec (google.cloud.discoveryengine_v1beta.types.SearchRequest.ContentSearchSpec.ExtractiveContentSpec):
+                If there is no extractive_content_spec provided, there will
+                be no extractive answer in the search response.
         """
 
         class SnippetSpec(proto.Message):
             r"""The specification that configs the snippet in the search
             results.
 
             Attributes:
                 max_snippet_count (int):
-                    Max number of snippets returned in each search result. If
-                    the matching snippets is less than the max_snippet_count,
+                    Max number of snippets returned in each search result.
+
+                    A snippet is an infomartive summary of a content with
+                    highlighting for UI rendering.
+
+                    If the matching snippets is less than the max_snippet_count,
                     return all of the snippets; otherwise, return the
                     max_snippet_count.
 
                     At most 5 snippets will be returned for each SearchResult.
                 reference_only (bool):
                     if true, only snippet reference is returned.
             """
@@ -569,24 +576,74 @@
             """
 
             summary_result_count: int = proto.Field(
                 proto.INT32,
                 number=1,
             )
 
+        class ExtractiveContentSpec(proto.Message):
+            r"""The specification that configs the extractive content in
+            search results.
+
+            Attributes:
+                max_extractive_answer_count (int):
+                    The max number of extractive answers returned in each search
+                    result.
+
+                    An extractive answer is a verbatim answer extracted from the
+                    original document, which provides precise and contextually
+                    relevant answer to the search query.
+
+                    If the number of matching answers is less than the
+                    extractive_answer_count, return all of the answers;
+                    otherwise, return the extractive_answer_count.
+
+                    At most 5 answers will be returned for each SearchResult.
+                max_extractive_segment_count (int):
+                    The max number of extractive segments returned in each
+                    search result.
+
+                    An extractive segment is a text segment extracted from the
+                    original document which is relevant to the search query and
+                    in general more verbose than an extrative answer. The
+                    segment could then be used as input for LLMs to generate
+                    summaries and answers.
+
+                    If the number of matching segments is less than the
+                    max_extractive_segment_count, return all of the segments;
+                    otherwise, return the max_extractive_segment_count.
+
+                    Currently one segment will be returned for each
+                    SearchResult.
+            """
+
+            max_extractive_answer_count: int = proto.Field(
+                proto.INT32,
+                number=1,
+            )
+            max_extractive_segment_count: int = proto.Field(
+                proto.INT32,
+                number=2,
+            )
+
         snippet_spec: "SearchRequest.ContentSearchSpec.SnippetSpec" = proto.Field(
             proto.MESSAGE,
             number=1,
             message="SearchRequest.ContentSearchSpec.SnippetSpec",
         )
         summary_spec: "SearchRequest.ContentSearchSpec.SummarySpec" = proto.Field(
             proto.MESSAGE,
             number=2,
             message="SearchRequest.ContentSearchSpec.SummarySpec",
         )
+        extractive_content_spec: "SearchRequest.ContentSearchSpec.ExtractiveContentSpec" = proto.Field(
+            proto.MESSAGE,
+            number=3,
+            message="SearchRequest.ContentSearchSpec.ExtractiveContentSpec",
+        )
 
     serving_config: str = proto.Field(
         proto.STRING,
         number=1,
     )
     branch: str = proto.Field(
         proto.STRING,
@@ -688,14 +745,21 @@
             [total_size][google.cloud.discoveryengine.v1beta.SearchResponse.total_size]
             that matches.
         attribution_token (str):
             A unique search token. This should be included in the
             [UserEvent][google.cloud.discoveryengine.v1beta.UserEvent]
             logs resulting from this search, which enables accurate
             attribution of search model performance.
+        redirect_uri (str):
+            The URI of a customer-defined redirect page. If redirect
+            action is triggered, no search is performed, and only
+            [redirect_uri][google.cloud.discoveryengine.v1beta.SearchResponse.redirect_uri]
+            and
+            [attribution_token][google.cloud.discoveryengine.v1beta.SearchResponse.attribution_token]
+            are set in the response.
         next_page_token (str):
             A token that can be sent as
             [SearchRequest.page_token][google.cloud.discoveryengine.v1beta.SearchRequest.page_token]
             to retrieve the next page. If this field is omitted, there
             are no subsequent pages.
         corrected_query (str):
             Contains the spell corrected query, if found. If the spell
@@ -883,14 +947,18 @@
         proto.INT32,
         number=3,
     )
     attribution_token: str = proto.Field(
         proto.STRING,
         number=4,
     )
+    redirect_uri: str = proto.Field(
+        proto.STRING,
+        number=12,
+    )
     next_page_token: str = proto.Field(
         proto.STRING,
         number=5,
     )
     corrected_query: str = proto.Field(
         proto.STRING,
         number=7,
```

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/types/user_event.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/types/user_event.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/types/user_event_service.py` & `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/types/user_event_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/google_cloud_discoveryengine.egg-info/PKG-INFO` & `google-cloud-discoveryengine-0.9.0/google_cloud_discoveryengine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-discoveryengine
-Version: 0.8.1
+Version: 0.9.0
 Summary: Google Cloud Discoveryengine API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-discoveryengine-0.8.1/google_cloud_discoveryengine.egg-info/SOURCES.txt` & `google-cloud-discoveryengine-0.9.0/google_cloud_discoveryengine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/setup.py` & `google-cloud-discoveryengine-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/tests/__init__.py` & `google-cloud-discoveryengine-0.9.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/tests/unit/__init__.py` & `google-cloud-discoveryengine-0.9.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/tests/unit/gapic/__init__.py` & `google-cloud-discoveryengine-0.9.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1/__init__.py` & `google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1/test_completion_service.py` & `google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1/test_completion_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1/test_document_service.py` & `google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1/test_document_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1/test_schema_service.py` & `google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1/test_schema_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1/test_search_service.py` & `google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1/test_search_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1/test_user_event_service.py` & `google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1/test_user_event_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1beta/__init__.py` & `google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1beta/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1beta/test_completion_service.py` & `google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1beta/test_completion_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1beta/test_document_service.py` & `google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1beta/test_document_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1beta/test_recommendation_service.py` & `google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1beta/test_recommendation_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1beta/test_schema_service.py` & `google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1beta/test_schema_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1beta/test_search_service.py` & `google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1beta/test_search_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -723,14 +723,15 @@
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.search), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = search_service.SearchResponse(
             total_size=1086,
             attribution_token="attribution_token_value",
+            redirect_uri="redirect_uri_value",
             next_page_token="next_page_token_value",
             corrected_query="corrected_query_value",
             applied_controls=["applied_controls_value"],
         )
         response = client.search(request)
 
         # Establish that the underlying gRPC stub method was called.
@@ -738,14 +739,15 @@
         _, args, _ = call.mock_calls[0]
         assert args[0] == search_service.SearchRequest()
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.SearchPager)
     assert response.total_size == 1086
     assert response.attribution_token == "attribution_token_value"
+    assert response.redirect_uri == "redirect_uri_value"
     assert response.next_page_token == "next_page_token_value"
     assert response.corrected_query == "corrected_query_value"
     assert response.applied_controls == ["applied_controls_value"]
 
 
 def test_search_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
@@ -779,14 +781,15 @@
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.search), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             search_service.SearchResponse(
                 total_size=1086,
                 attribution_token="attribution_token_value",
+                redirect_uri="redirect_uri_value",
                 next_page_token="next_page_token_value",
                 corrected_query="corrected_query_value",
                 applied_controls=["applied_controls_value"],
             )
         )
         response = await client.search(request)
 
@@ -795,14 +798,15 @@
         _, args, _ = call.mock_calls[0]
         assert args[0] == search_service.SearchRequest()
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.SearchAsyncPager)
     assert response.total_size == 1086
     assert response.attribution_token == "attribution_token_value"
+    assert response.redirect_uri == "redirect_uri_value"
     assert response.next_page_token == "next_page_token_value"
     assert response.corrected_query == "corrected_query_value"
     assert response.applied_controls == ["applied_controls_value"]
 
 
 @pytest.mark.asyncio
 async def test_search_async_from_dict():
@@ -1081,14 +1085,15 @@
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = search_service.SearchResponse(
             total_size=1086,
             attribution_token="attribution_token_value",
+            redirect_uri="redirect_uri_value",
             next_page_token="next_page_token_value",
             corrected_query="corrected_query_value",
             applied_controls=["applied_controls_value"],
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
@@ -1100,14 +1105,15 @@
         req.return_value = response_value
         response = client.search(request)
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.SearchPager)
     assert response.total_size == 1086
     assert response.attribution_token == "attribution_token_value"
+    assert response.redirect_uri == "redirect_uri_value"
     assert response.next_page_token == "next_page_token_value"
     assert response.corrected_query == "corrected_query_value"
     assert response.applied_controls == ["applied_controls_value"]
 
 
 def test_search_rest_required_fields(request_type=search_service.SearchRequest):
     transport_class = transports.SearchServiceRestTransport
```

### Comparing `google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1beta/test_user_event_service.py` & `google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1beta/test_user_event_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1950,25 +1950,15 @@
 
 def test_import_user_events_rest_unset_required_fields():
     transport = transports.UserEventServiceRestTransport(
         credentials=ga_credentials.AnonymousCredentials
     )
 
     unset_fields = transport.import_user_events._get_unset_required_fields({})
-    assert set(unset_fields) == (
-        set(())
-        & set(
-            (
-                "inlineSource",
-                "gcsSource",
-                "bigquerySource",
-                "parent",
-            )
-        )
-    )
+    assert set(unset_fields) == (set(()) & set(("parent",)))
 
 
 @pytest.mark.parametrize("null_interceptor", [True, False])
 def test_import_user_events_rest_interceptors(null_interceptor):
     transport = transports.UserEventServiceRestTransport(
         credentials=ga_credentials.AnonymousCredentials(),
         interceptor=None
```

