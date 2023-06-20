# Comparing `tmp/kuflow_rest-0.6.1.tar.gz` & `tmp/kuflow_rest-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuflow_rest-0.6.1.tar", max compression
+gzip compressed data, was "kuflow_rest-0.7.0.tar", max compression
```

## Comparing `kuflow_rest-0.6.1.tar` & `kuflow_rest-0.7.0.tar`

### file list

```diff
@@ -1,72 +1,86 @@
--rw-r--r--   0        0        0      875 2023-06-16 09:00:12.903233 kuflow_rest-0.6.1/README.md
--rw-r--r--   0        0        0        6 2023-06-16 09:00:12.903233 kuflow_rest-0.6.1/VERSION
--rw-r--r--   0        0        0     1335 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/__init__.py
--rw-r--r--   0        0        0     1907 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/__init__.py
--rw-r--r--   0        0        0      599 2023-06-16 09:01:21.056971 kuflow_rest-0.6.1/kuflow_rest/_generated/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     6018 2023-06-16 09:01:21.056971 kuflow_rest-0.6.1/kuflow_rest/_generated/__pycache__/_client.cpython-38.pyc
--rw-r--r--   0        0        0     2365 2023-06-16 09:01:21.084973 kuflow_rest-0.6.1/kuflow_rest/_generated/__pycache__/_configuration.cpython-38.pyc
--rw-r--r--   0        0        0      732 2023-06-16 09:01:21.096974 kuflow_rest-0.6.1/kuflow_rest/_generated/__pycache__/_patch.cpython-38.pyc
--rw-r--r--   0        0        0    57905 2023-06-16 09:01:21.076973 kuflow_rest-0.6.1/kuflow_rest/_generated/__pycache__/_serialization.cpython-38.pyc
--rw-r--r--   0        0        0      731 2023-06-16 09:01:21.084973 kuflow_rest-0.6.1/kuflow_rest/_generated/__pycache__/_vendor.cpython-38.pyc
--rw-r--r--   0        0        0      178 2023-06-16 09:01:21.084973 kuflow_rest-0.6.1/kuflow_rest/_generated/__pycache__/_version.cpython-38.pyc
--rw-r--r--   0        0        0     7108 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/_client.py
--rw-r--r--   0        0        0     3983 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/_configuration.py
--rw-r--r--   0        0        0      674 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/_patch.py
--rw-r--r--   0        0        0    78834 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/_serialization.py
--rw-r--r--   0        0        0     2007 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/_vendor.py
--rw-r--r--   0        0        0     1517 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/_version.py
--rw-r--r--   0        0        0     1854 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/aio/__init__.py
--rw-r--r--   0        0        0     7256 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/aio/_client.py
--rw-r--r--   0        0        0     4026 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/aio/_configuration.py
--rw-r--r--   0        0        0      674 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/aio/_patch.py
--rw-r--r--   0        0        0     2060 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/aio/operations/__init__.py
--rw-r--r--   0        0        0     7284 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/aio/operations/_authentication_operations.py
--rw-r--r--   0        0        0      674 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/aio/operations/_patch.py
--rw-r--r--   0        0        0     7894 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/aio/operations/_principal_operations.py
--rw-r--r--   0        0        0    35197 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/aio/operations/_process_operations.py
--rw-r--r--   0        0        0    62010 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/aio/operations/_task_operations.py
--rw-r--r--   0        0        0     5465 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/models/__init__.py
--rw-r--r--   0        0        0     3261 2023-06-16 09:01:21.060972 kuflow_rest-0.6.1/kuflow_rest/_generated/models/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2558 2023-06-16 09:01:21.080973 kuflow_rest-0.6.1/kuflow_rest/_generated/models/__pycache__/_enums.cpython-38.pyc
--rw-r--r--   0        0        0    65326 2023-06-16 09:01:21.064972 kuflow_rest-0.6.1/kuflow_rest/_generated/models/__pycache__/_models.cpython-38.pyc
--rw-r--r--   0        0        0      739 2023-06-16 09:01:21.080973 kuflow_rest-0.6.1/kuflow_rest/_generated/models/__pycache__/_patch.cpython-38.pyc
--rw-r--r--   0        0        0     3294 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/models/_enums.py
--rw-r--r--   0        0        0    75667 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/models/_models.py
--rw-r--r--   0        0        0      674 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/models/_patch.py
--rw-r--r--   0        0        0     2060 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/operations/__init__.py
--rw-r--r--   0        0        0      737 2023-06-16 09:01:21.084973 kuflow_rest-0.6.1/kuflow_rest/_generated/operations/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     5603 2023-06-16 09:01:21.084973 kuflow_rest-0.6.1/kuflow_rest/_generated/operations/__pycache__/_authentication_operations.cpython-38.pyc
--rw-r--r--   0        0        0      743 2023-06-16 09:01:21.096974 kuflow_rest-0.6.1/kuflow_rest/_generated/operations/__pycache__/_patch.cpython-38.pyc
--rw-r--r--   0        0        0     6811 2023-06-16 09:01:21.084973 kuflow_rest-0.6.1/kuflow_rest/_generated/operations/__pycache__/_principal_operations.cpython-38.pyc
--rw-r--r--   0        0        0    28491 2023-06-16 09:01:21.088974 kuflow_rest-0.6.1/kuflow_rest/_generated/operations/__pycache__/_process_operations.cpython-38.pyc
--rw-r--r--   0        0        0    51369 2023-06-16 09:01:21.096974 kuflow_rest-0.6.1/kuflow_rest/_generated/operations/__pycache__/_task_operations.cpython-38.pyc
--rw-r--r--   0        0        0     7884 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/operations/_authentication_operations.py
--rw-r--r--   0        0        0      674 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/operations/_patch.py
--rw-r--r--   0        0        0     9804 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/operations/_principal_operations.py
--rw-r--r--   0        0        0    41967 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/operations/_process_operations.py
--rw-r--r--   0        0        0    76156 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/operations/_task_operations.py
--rw-r--r--   0        0        0       26 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/py.typed
--rw-r--r--   0        0        0     7722 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_kuflow_rest_client.py
--rw-r--r--   0        0        0     4771 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/models/__init__.py
--rw-r--r--   0        0        0     2858 2023-06-16 09:01:21.100975 kuflow_rest-0.6.1/kuflow_rest/models/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     4588 2023-06-16 09:01:21.100975 kuflow_rest-0.6.1/kuflow_rest/models/__pycache__/_models.cpython-38.pyc
--rw-r--r--   0        0        0     4581 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/models/_models.py
--rw-r--r--   0        0        0     1440 2023-06-16 09:00:12.911234 kuflow_rest-0.6.1/kuflow_rest/operations/__init__.py
--rw-r--r--   0        0        0      460 2023-06-16 09:01:21.096974 kuflow_rest-0.6.1/kuflow_rest/operations/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1665 2023-06-16 09:01:21.100975 kuflow_rest-0.6.1/kuflow_rest/operations/__pycache__/_authentication_operations.cpython-38.pyc
--rw-r--r--   0        0        0     3408 2023-06-16 09:01:21.100975 kuflow_rest-0.6.1/kuflow_rest/operations/__pycache__/_principal_operations.cpython-38.pyc
--rw-r--r--   0        0        0     9051 2023-06-16 09:01:21.100975 kuflow_rest-0.6.1/kuflow_rest/operations/__pycache__/_process_operations.cpython-38.pyc
--rw-r--r--   0        0        0    16300 2023-06-16 09:01:21.100975 kuflow_rest-0.6.1/kuflow_rest/operations/__pycache__/_task_operations.cpython-38.pyc
--rw-r--r--   0        0        0     2322 2023-06-16 09:00:12.911234 kuflow_rest-0.6.1/kuflow_rest/operations/_authentication_operations.py
--rw-r--r--   0        0        0     4113 2023-06-16 09:00:12.911234 kuflow_rest-0.6.1/kuflow_rest/operations/_principal_operations.py
--rw-r--r--   0        0        0     9530 2023-06-16 09:00:12.911234 kuflow_rest-0.6.1/kuflow_rest/operations/_process_operations.py
--rw-r--r--   0        0        0    17424 2023-06-16 09:00:12.911234 kuflow_rest-0.6.1/kuflow_rest/operations/_task_operations.py
--rw-r--r--   0        0        0     6837 2023-06-16 09:00:12.911234 kuflow_rest-0.6.1/kuflow_rest/utils/__init__.py
--rw-r--r--   0        0        0     3980 2023-06-16 09:01:21.104975 kuflow_rest-0.6.1/kuflow_rest/utils/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0    31360 2023-06-16 09:01:21.108976 kuflow_rest-0.6.1/kuflow_rest/utils/__pycache__/_element_values.cpython-38.pyc
--rw-r--r--   0        0        0    17040 2023-06-16 09:01:21.104975 kuflow_rest-0.6.1/kuflow_rest/utils/__pycache__/_json_forms.cpython-38.pyc
--rw-r--r--   0        0        0    41580 2023-06-16 09:00:12.911234 kuflow_rest-0.6.1/kuflow_rest/utils/_element_values.py
--rw-r--r--   0        0        0    23171 2023-06-16 09:00:12.911234 kuflow_rest-0.6.1/kuflow_rest/utils/_json_forms.py
--rw-r--r--   0        0        0      977 2023-06-16 09:01:38.346427 kuflow_rest-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     1801 1970-01-01 00:00:00.000000 kuflow_rest-0.6.1/setup.py
--rw-r--r--   0        0        0     1639 1970-01-01 00:00:00.000000 kuflow_rest-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0      875 2023-06-20 06:25:31.586347 kuflow_rest-0.7.0/README.md
+-rw-r--r--   0        0        0        6 2023-06-20 06:25:31.586347 kuflow_rest-0.7.0/VERSION
+-rw-r--r--   0        0        0     1335 2023-06-20 06:25:31.586347 kuflow_rest-0.7.0/kuflow_rest/__init__.py
+-rw-r--r--   0        0        0     1907 2023-06-20 06:25:31.586347 kuflow_rest-0.7.0/kuflow_rest/_generated/__init__.py
+-rw-r--r--   0        0        0      599 2023-06-20 06:26:39.291781 kuflow_rest-0.7.0/kuflow_rest/_generated/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     6018 2023-06-20 06:26:39.291781 kuflow_rest-0.7.0/kuflow_rest/_generated/__pycache__/_client.cpython-38.pyc
+-rw-r--r--   0        0        0     2365 2023-06-20 06:26:39.319784 kuflow_rest-0.7.0/kuflow_rest/_generated/__pycache__/_configuration.cpython-38.pyc
+-rw-r--r--   0        0        0      732 2023-06-20 06:26:39.335785 kuflow_rest-0.7.0/kuflow_rest/_generated/__pycache__/_patch.cpython-38.pyc
+-rw-r--r--   0        0        0    57905 2023-06-20 06:26:39.311783 kuflow_rest-0.7.0/kuflow_rest/_generated/__pycache__/_serialization.cpython-38.pyc
+-rw-r--r--   0        0        0      731 2023-06-20 06:26:39.323784 kuflow_rest-0.7.0/kuflow_rest/_generated/__pycache__/_vendor.cpython-38.pyc
+-rw-r--r--   0        0        0      178 2023-06-20 06:26:39.319784 kuflow_rest-0.7.0/kuflow_rest/_generated/__pycache__/_version.cpython-38.pyc
+-rw-r--r--   0        0        0     7108 2023-06-20 06:25:31.586347 kuflow_rest-0.7.0/kuflow_rest/_generated/_client.py
+-rw-r--r--   0        0        0     3983 2023-06-20 06:25:31.586347 kuflow_rest-0.7.0/kuflow_rest/_generated/_configuration.py
+-rw-r--r--   0        0        0      674 2023-06-20 06:25:31.586347 kuflow_rest-0.7.0/kuflow_rest/_generated/_patch.py
+-rw-r--r--   0        0        0    78834 2023-06-20 06:25:31.586347 kuflow_rest-0.7.0/kuflow_rest/_generated/_serialization.py
+-rw-r--r--   0        0        0     2007 2023-06-20 06:25:31.586347 kuflow_rest-0.7.0/kuflow_rest/_generated/_vendor.py
+-rw-r--r--   0        0        0     1517 2023-06-20 06:25:31.586347 kuflow_rest-0.7.0/kuflow_rest/_generated/_version.py
+-rw-r--r--   0        0        0     1854 2023-06-20 06:25:31.586347 kuflow_rest-0.7.0/kuflow_rest/_generated/aio/__init__.py
+-rw-r--r--   0        0        0     7256 2023-06-20 06:25:31.586347 kuflow_rest-0.7.0/kuflow_rest/_generated/aio/_client.py
+-rw-r--r--   0        0        0     4026 2023-06-20 06:25:31.586347 kuflow_rest-0.7.0/kuflow_rest/_generated/aio/_configuration.py
+-rw-r--r--   0        0        0      674 2023-06-20 06:25:31.586347 kuflow_rest-0.7.0/kuflow_rest/_generated/aio/_patch.py
+-rw-r--r--   0        0        0     2060 2023-06-20 06:25:31.586347 kuflow_rest-0.7.0/kuflow_rest/_generated/aio/operations/__init__.py
+-rw-r--r--   0        0        0     7284 2023-06-20 06:25:31.586347 kuflow_rest-0.7.0/kuflow_rest/_generated/aio/operations/_authentication_operations.py
+-rw-r--r--   0        0        0      674 2023-06-20 06:25:31.586347 kuflow_rest-0.7.0/kuflow_rest/_generated/aio/operations/_patch.py
+-rw-r--r--   0        0        0     7894 2023-06-20 06:25:31.586347 kuflow_rest-0.7.0/kuflow_rest/_generated/aio/operations/_principal_operations.py
+-rw-r--r--   0        0        0    35197 2023-06-20 06:25:31.586347 kuflow_rest-0.7.0/kuflow_rest/_generated/aio/operations/_process_operations.py
+-rw-r--r--   0        0        0    62010 2023-06-20 06:25:31.586347 kuflow_rest-0.7.0/kuflow_rest/_generated/aio/operations/_task_operations.py
+-rw-r--r--   0        0        0     5465 2023-06-20 06:25:31.586347 kuflow_rest-0.7.0/kuflow_rest/_generated/models/__init__.py
+-rw-r--r--   0        0        0     3261 2023-06-20 06:26:39.295781 kuflow_rest-0.7.0/kuflow_rest/_generated/models/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2558 2023-06-20 06:26:39.315783 kuflow_rest-0.7.0/kuflow_rest/_generated/models/__pycache__/_enums.cpython-38.pyc
+-rw-r--r--   0        0        0    65326 2023-06-20 06:26:39.299782 kuflow_rest-0.7.0/kuflow_rest/_generated/models/__pycache__/_models.cpython-38.pyc
+-rw-r--r--   0        0        0      739 2023-06-20 06:26:39.319784 kuflow_rest-0.7.0/kuflow_rest/_generated/models/__pycache__/_patch.cpython-38.pyc
+-rw-r--r--   0        0        0     3294 2023-06-20 06:25:31.586347 kuflow_rest-0.7.0/kuflow_rest/_generated/models/_enums.py
+-rw-r--r--   0        0        0    75667 2023-06-20 06:25:31.586347 kuflow_rest-0.7.0/kuflow_rest/_generated/models/_models.py
+-rw-r--r--   0        0        0      674 2023-06-20 06:25:31.590348 kuflow_rest-0.7.0/kuflow_rest/_generated/models/_patch.py
+-rw-r--r--   0        0        0     2060 2023-06-20 06:25:31.590348 kuflow_rest-0.7.0/kuflow_rest/_generated/operations/__init__.py
+-rw-r--r--   0        0        0      737 2023-06-20 06:26:39.319784 kuflow_rest-0.7.0/kuflow_rest/_generated/operations/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     5603 2023-06-20 06:26:39.319784 kuflow_rest-0.7.0/kuflow_rest/_generated/operations/__pycache__/_authentication_operations.cpython-38.pyc
+-rw-r--r--   0        0        0      743 2023-06-20 06:26:39.335785 kuflow_rest-0.7.0/kuflow_rest/_generated/operations/__pycache__/_patch.cpython-38.pyc
+-rw-r--r--   0        0        0     6811 2023-06-20 06:26:39.323784 kuflow_rest-0.7.0/kuflow_rest/_generated/operations/__pycache__/_principal_operations.cpython-38.pyc
+-rw-r--r--   0        0        0    28491 2023-06-20 06:26:39.327784 kuflow_rest-0.7.0/kuflow_rest/_generated/operations/__pycache__/_process_operations.cpython-38.pyc
+-rw-r--r--   0        0        0    51369 2023-06-20 06:26:39.335785 kuflow_rest-0.7.0/kuflow_rest/_generated/operations/__pycache__/_task_operations.cpython-38.pyc
+-rw-r--r--   0        0        0     7884 2023-06-20 06:25:31.590348 kuflow_rest-0.7.0/kuflow_rest/_generated/operations/_authentication_operations.py
+-rw-r--r--   0        0        0      674 2023-06-20 06:25:31.590348 kuflow_rest-0.7.0/kuflow_rest/_generated/operations/_patch.py
+-rw-r--r--   0        0        0     9804 2023-06-20 06:25:31.590348 kuflow_rest-0.7.0/kuflow_rest/_generated/operations/_principal_operations.py
+-rw-r--r--   0        0        0    41967 2023-06-20 06:25:31.590348 kuflow_rest-0.7.0/kuflow_rest/_generated/operations/_process_operations.py
+-rw-r--r--   0        0        0    76156 2023-06-20 06:25:31.590348 kuflow_rest-0.7.0/kuflow_rest/_generated/operations/_task_operations.py
+-rw-r--r--   0        0        0       26 2023-06-20 06:25:31.590348 kuflow_rest-0.7.0/kuflow_rest/_generated/py.typed
+-rw-r--r--   0        0        0     7722 2023-06-20 06:25:31.590348 kuflow_rest-0.7.0/kuflow_rest/_kuflow_rest_client.py
+-rw-r--r--   0        0        0     4771 2023-06-20 06:25:31.590348 kuflow_rest-0.7.0/kuflow_rest/models/__init__.py
+-rw-r--r--   0        0        0     2858 2023-06-20 06:26:39.339785 kuflow_rest-0.7.0/kuflow_rest/models/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     4588 2023-06-20 06:26:39.339785 kuflow_rest-0.7.0/kuflow_rest/models/__pycache__/_models.cpython-38.pyc
+-rw-r--r--   0        0        0     4581 2023-06-20 06:25:31.590348 kuflow_rest-0.7.0/kuflow_rest/models/_models.py
+-rw-r--r--   0        0        0     1440 2023-06-20 06:25:31.590348 kuflow_rest-0.7.0/kuflow_rest/operations/__init__.py
+-rw-r--r--   0        0        0      460 2023-06-20 06:26:39.335785 kuflow_rest-0.7.0/kuflow_rest/operations/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1665 2023-06-20 06:26:39.335785 kuflow_rest-0.7.0/kuflow_rest/operations/__pycache__/_authentication_operations.cpython-38.pyc
+-rw-r--r--   0        0        0     3408 2023-06-20 06:26:39.339785 kuflow_rest-0.7.0/kuflow_rest/operations/__pycache__/_principal_operations.cpython-38.pyc
+-rw-r--r--   0        0        0     9051 2023-06-20 06:26:39.339785 kuflow_rest-0.7.0/kuflow_rest/operations/__pycache__/_process_operations.cpython-38.pyc
+-rw-r--r--   0        0        0    16300 2023-06-20 06:26:39.339785 kuflow_rest-0.7.0/kuflow_rest/operations/__pycache__/_task_operations.cpython-38.pyc
+-rw-r--r--   0        0        0     2322 2023-06-20 06:25:31.590348 kuflow_rest-0.7.0/kuflow_rest/operations/_authentication_operations.py
+-rw-r--r--   0        0        0     4113 2023-06-20 06:25:31.590348 kuflow_rest-0.7.0/kuflow_rest/operations/_principal_operations.py
+-rw-r--r--   0        0        0     9530 2023-06-20 06:25:31.590348 kuflow_rest-0.7.0/kuflow_rest/operations/_process_operations.py
+-rw-r--r--   0        0        0    17424 2023-06-20 06:25:31.590348 kuflow_rest-0.7.0/kuflow_rest/operations/_task_operations.py
+-rw-r--r--   0        0        0     2046 2023-06-20 06:25:31.590348 kuflow_rest-0.7.0/kuflow_rest/utils/__init__.py
+-rw-r--r--   0        0        0      935 2023-06-20 06:26:39.339785 kuflow_rest-0.7.0/kuflow_rest/utils/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    10617 2023-06-20 06:26:39.343785 kuflow_rest-0.7.0/kuflow_rest/utils/__pycache__/_process_page_item_utils.cpython-38.pyc
+-rw-r--r--   0        0        0     9710 2023-06-20 06:26:39.343785 kuflow_rest-0.7.0/kuflow_rest/utils/__pycache__/_process_save_element_command_utils.cpython-38.pyc
+-rw-r--r--   0        0        0    10024 2023-06-20 06:26:39.347786 kuflow_rest-0.7.0/kuflow_rest/utils/__pycache__/_process_utils.cpython-38.pyc
+-rw-r--r--   0        0        0    14985 2023-06-20 06:26:39.347786 kuflow_rest-0.7.0/kuflow_rest/utils/__pycache__/_task_page_item_utils.cpython-38.pyc
+-rw-r--r--   0        0        0    13767 2023-06-20 06:26:39.347786 kuflow_rest-0.7.0/kuflow_rest/utils/__pycache__/_task_save_element_command_utils.cpython-38.pyc
+-rw-r--r--   0        0        0    14250 2023-06-20 06:26:39.351786 kuflow_rest-0.7.0/kuflow_rest/utils/__pycache__/_task_save_json_forms_value_data_utils.cpython-38.pyc
+-rw-r--r--   0        0        0    26608 2023-06-20 06:26:39.355786 kuflow_rest-0.7.0/kuflow_rest/utils/__pycache__/_task_utils.cpython-38.pyc
+-rw-r--r--   0        0        0    15400 2023-06-20 06:26:39.343785 kuflow_rest-0.7.0/kuflow_rest/utils/__pycache__/element_values.cpython-38.pyc
+-rw-r--r--   0        0        0    17854 2023-06-20 06:26:39.351786 kuflow_rest-0.7.0/kuflow_rest/utils/__pycache__/json_forms.cpython-38.pyc
+-rw-r--r--   0        0        0    13065 2023-06-20 06:25:31.590348 kuflow_rest-0.7.0/kuflow_rest/utils/_process_page_item_utils.py
+-rw-r--r--   0        0        0    11649 2023-06-20 06:25:31.590348 kuflow_rest-0.7.0/kuflow_rest/utils/_process_save_element_command_utils.py
+-rw-r--r--   0        0        0    11857 2023-06-20 06:25:31.590348 kuflow_rest-0.7.0/kuflow_rest/utils/_process_utils.py
+-rw-r--r--   0        0        0    18132 2023-06-20 06:25:31.590348 kuflow_rest-0.7.0/kuflow_rest/utils/_task_page_item_utils.py
+-rw-r--r--   0        0        0    16181 2023-06-20 06:25:31.590348 kuflow_rest-0.7.0/kuflow_rest/utils/_task_save_element_command_utils.py
+-rw-r--r--   0        0        0    15393 2023-06-20 06:25:31.590348 kuflow_rest-0.7.0/kuflow_rest/utils/_task_save_json_forms_value_data_utils.py
+-rw-r--r--   0        0        0    29269 2023-06-20 06:25:31.590348 kuflow_rest-0.7.0/kuflow_rest/utils/_task_utils.py
+-rw-r--r--   0        0        0    18805 2023-06-20 06:25:31.590348 kuflow_rest-0.7.0/kuflow_rest/utils/element_values.py
+-rw-r--r--   0        0        0    23991 2023-06-20 06:25:31.590348 kuflow_rest-0.7.0/kuflow_rest/utils/json_forms.py
+-rw-r--r--   0        0        0      977 2023-06-20 06:26:56.169144 kuflow_rest-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1801 1970-01-01 00:00:00.000000 kuflow_rest-0.7.0/setup.py
+-rw-r--r--   0        0        0     1639 1970-01-01 00:00:00.000000 kuflow_rest-0.7.0/PKG-INFO
```

### Comparing `kuflow_rest-0.6.1/README.md` & `kuflow_rest-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.1/kuflow_rest/__init__.py` & `kuflow_rest-0.7.0/kuflow_rest/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 # SOFTWARE.
 #
 
 from ._kuflow_rest_client import KuFlowRestClient
 from ._generated._serialization import Deserializer, Serializer, Model
 
 __all__ = ["Deserializer", "KuFlowRestClient", "Model", "Serializer"]
-__version__ = "0.6.1"
+__version__ = "0.7.0"
```

### Comparing `kuflow_rest-0.6.1/kuflow_rest/_generated/__init__.py` & `kuflow_rest-0.7.0/kuflow_rest/_generated/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.1/kuflow_rest/_generated/__pycache__/__init__.cpython-38.pyc` & `kuflow_rest-0.7.0/kuflow_rest/_generated/__pycache__/__init__.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Jun 16 09:00:12 2023 UTC, .py size: 1907 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 9c24 8c64 7307 0000  U........$.ds...
+00000000: 550d 0d0a 0000 0000 5b46 9164 7307 0000  U.......[F.ds...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 7e00 0000 6400  .....@...s~...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6503 5a04 7a18 6400 6403  m.Z...e.Z.z.d.d.
 00000050: 6c05 6d06 5a07 0100 6400 6404 6c05 5400  l.m.Z...d.d.l.T.
 00000060: 5700 6e18 0400 6508 6b0a 724c 0100 0100  W.n...e.k.rL....
 00000070: 0100 6700 5a07 5900 6e02 5800 6400 6405  ..g.Z.Y.n.X.d.d.
```

### Comparing `kuflow_rest-0.6.1/kuflow_rest/_generated/__pycache__/_client.cpython-38.pyc` & `kuflow_rest-0.7.0/kuflow_rest/_generated/__pycache__/_client.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Jun 16 09:00:12 2023 UTC, .py size: 7108 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 9c24 8c64 c41b 0000  U........$.d....
+00000000: 550d 0d0a 0000 0000 5b46 9164 c41b 0000  U.......[F.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 9a00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 6d09 5a09 0100 6405 6406 6c0a 6d0b 5a0c  m.Z...d.d.l.m.Z.
 00000070: 0100 6405 6407 6c0d 6d0e 5a0e 0100 6405  ..d.d.l.m.Z...d.
```

### Comparing `kuflow_rest-0.6.1/kuflow_rest/_generated/__pycache__/_configuration.cpython-38.pyc` & `kuflow_rest-0.7.0/kuflow_rest/_generated/__pycache__/_configuration.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Jun 16 09:00:12 2023 UTC, .py size: 3983 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 9c24 8c64 8f0f 0000  U........$.d....
+00000000: 550d 0d0a 0000 0000 5b46 9164 8f0f 0000  U.......[F.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5800 0000 6400  .....@...sX...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6404 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6502 7244 6400 6406 6c09 6d0a 5a0a  ..e.rDd.d.l.m.Z.
 00000070: 0100 4700 6407 6408 8400 6408 6504 8303  ..G.d.d...d.e...
```

### Comparing `kuflow_rest-0.6.1/kuflow_rest/_generated/__pycache__/_patch.cpython-38.pyc` & `kuflow_rest-0.7.0/kuflow_rest/_generated/__pycache__/_patch.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Jun 16 09:00:12 2023 UTC, .py size: 674 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 9c24 8c64 a202 0000  U........$.d....
+00000000: 550d 0d0a 0000 0000 5b46 9164 a202 0000  U.......[F.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2e00 0000 5500  .....@...s....U.
 00000030: 6400 5a00 6401 6402 6c01 6d02 5a02 0100  d.Z.d.d.l.m.Z...
 00000040: 6700 5a03 6502 6504 1900 6505 6403 3c00  g.Z.e.e...e.d.<.
 00000050: 6404 6405 8400 5a06 6406 5300 2907 7a7b  d.d...Z.d.S.).z{
 00000060: 4375 7374 6f6d 697a 6520 6765 6e65 7261  Customize genera
 00000070: 7465 6420 636f 6465 2068 6572 652e 0a0a  ted code here...
```

### Comparing `kuflow_rest-0.6.1/kuflow_rest/_generated/__pycache__/_serialization.cpython-38.pyc` & `kuflow_rest-0.7.0/kuflow_rest/_generated/__pycache__/_serialization.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Jun 16 09:00:12 2023 UTC, .py size: 78834 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 9c24 8c64 f233 0100  U........$.d.3..
+00000000: 550d 0d0a 0000 0000 5b46 9164 f233 0100  U.......[F.d.3..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 c602 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a03 6400 6402 6c04 5a04 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6402 6c05 5a05 6400 6402 6c06 5a06 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6403 6c07 6d08 5a08 0100 6400 6402 6c09  d.l.m.Z...d.d.l.
 00000070: 5a09 6400 6402 6c0a 5a0a 6400 6402 6c0b  Z.d.d.l.Z.d.d.l.
```

### Comparing `kuflow_rest-0.6.1/kuflow_rest/_generated/__pycache__/_vendor.cpython-38.pyc` & `kuflow_rest-0.7.0/kuflow_rest/_generated/__pycache__/_vendor.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Jun 16 09:00:12 2023 UTC, .py size: 2007 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 9c24 8c64 d707 0000  U........$.d....
+00000000: 550d 0d0a 0000 0000 5b46 9164 d707 0000  U.......[F.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 1c00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6402  d.l.m.Z.m.Z...d.
 00000040: 6403 8400 5a03 6404 5300 2905 e900 0000  d...Z.d.S.).....
 00000050: 0029 02da 044c 6973 74da 0463 6173 7463  .)...List..castc
 00000060: 0100 0000 0000 0000 0000 0000 0400 0000  ................
 00000070: 0a00 0000 0b00 0000 7376 0000 007c 00a0  ........sv...|..
```

### Comparing `kuflow_rest-0.6.1/kuflow_rest/_generated/_client.py` & `kuflow_rest-0.7.0/kuflow_rest/_generated/_client.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.1/kuflow_rest/_generated/_configuration.py` & `kuflow_rest-0.7.0/kuflow_rest/_generated/_configuration.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.1/kuflow_rest/_generated/_patch.py` & `kuflow_rest-0.7.0/kuflow_rest/_generated/_patch.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.1/kuflow_rest/_generated/_serialization.py` & `kuflow_rest-0.7.0/kuflow_rest/_generated/_serialization.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.1/kuflow_rest/_generated/_vendor.py` & `kuflow_rest-0.7.0/kuflow_rest/_generated/_vendor.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.1/kuflow_rest/_generated/_version.py` & `kuflow_rest-0.7.0/kuflow_rest/_generated/_version.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,8 +26,8 @@
 # --------------------------------------------------------------------------
 #
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 #
 # --------------------------------------------------------------------------
 
-VERSION = "0.6.1"
+VERSION = "0.7.0"
```

### Comparing `kuflow_rest-0.6.1/kuflow_rest/_generated/aio/__init__.py` & `kuflow_rest-0.7.0/kuflow_rest/_generated/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.1/kuflow_rest/_generated/aio/_client.py` & `kuflow_rest-0.7.0/kuflow_rest/_generated/aio/_client.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.1/kuflow_rest/_generated/aio/_configuration.py` & `kuflow_rest-0.7.0/kuflow_rest/_generated/aio/_configuration.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.1/kuflow_rest/_generated/aio/_patch.py` & `kuflow_rest-0.7.0/kuflow_rest/_generated/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.1/kuflow_rest/_generated/aio/operations/__init__.py` & `kuflow_rest-0.7.0/kuflow_rest/_generated/aio/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.1/kuflow_rest/_generated/aio/operations/_authentication_operations.py` & `kuflow_rest-0.7.0/kuflow_rest/_generated/aio/operations/_authentication_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.1/kuflow_rest/_generated/aio/operations/_patch.py` & `kuflow_rest-0.7.0/kuflow_rest/_generated/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.1/kuflow_rest/_generated/aio/operations/_principal_operations.py` & `kuflow_rest-0.7.0/kuflow_rest/_generated/aio/operations/_principal_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.1/kuflow_rest/_generated/aio/operations/_process_operations.py` & `kuflow_rest-0.7.0/kuflow_rest/_generated/aio/operations/_process_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.1/kuflow_rest/_generated/aio/operations/_task_operations.py` & `kuflow_rest-0.7.0/kuflow_rest/_generated/aio/operations/_task_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.1/kuflow_rest/_generated/models/__init__.py` & `kuflow_rest-0.7.0/kuflow_rest/_generated/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.1/kuflow_rest/_generated/models/__pycache__/__init__.cpython-38.pyc` & `kuflow_rest-0.7.0/kuflow_rest/_generated/models/__pycache__/__init__.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Jun 16 09:00:12 2023 UTC, .py size: 5465 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 9c24 8c64 5915 0000  U........$.dY...
+00000000: 550d 0d0a 0000 0000 5b46 9164 5915 0000  U.......[F.dY...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0037 0000 0040 0000 0073 4403 0000 6400  .7...@...sD...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c00  d.l.m.Z...d.d.l.
 00000040: 6d02 5a02 0100 6400 6403 6c00 6d03 5a03  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c00 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c00 6d05 5a05 0100 6400 6406 6c00  d.l.m.Z...d.d.l.
 00000070: 6d06 5a06 0100 6400 6407 6c00 6d07 5a07  m.Z...d.d.l.m.Z.
```

### Comparing `kuflow_rest-0.6.1/kuflow_rest/_generated/models/__pycache__/_enums.cpython-38.pyc` & `kuflow_rest-0.7.0/kuflow_rest/_generated/models/__pycache__/_enums.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Jun 16 09:00:12 2023 UTC, .py size: 3294 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 9c24 8c64 de0c 0000  U........$.d....
+00000000: 550d 0d0a 0000 0000 5b46 9164 de0c 0000  U.......[F.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 e200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 4700 6403 6404 8400 6404  m.Z...G.d.d...d.
 00000050: 6504 6501 6503 6405 8d05 5a05 4700 6406  e.e.e.d...Z.G.d.
 00000060: 6407 8400 6407 6504 6501 6503 6405 8d05  d...d.e.e.e.d...
 00000070: 5a06 4700 6408 6409 8400 6409 6504 6501  Z.G.d.d...d.e.e.
```

### Comparing `kuflow_rest-0.6.1/kuflow_rest/_generated/models/__pycache__/_models.cpython-38.pyc` & `kuflow_rest-0.7.0/kuflow_rest/_generated/models/__pycache__/_models.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Jun 16 09:00:12 2023 UTC, .py size: 75667 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 9c24 8c64 9327 0100  U........$.d.'..
+00000000: 550d 0d0a 0000 0000 5b46 9164 9327 0100  U.......[F.d.'..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8e03 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 6d04 5a04 6d05 5a05  d.l.m.Z.m.Z.m.Z.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 0100 6403  m.Z.m.Z.m.Z...d.
 00000060: 6404 6c09 6d0a 5a0a 0100 6501 6a0b 6405  d.l.m.Z...e.j.d.
 00000070: 6b05 7254 6400 6406 6c02 6d0c 5a0c 0100  k.rTd.d.l.m.Z...
```

### Comparing `kuflow_rest-0.6.1/kuflow_rest/_generated/models/__pycache__/_patch.cpython-38.pyc` & `kuflow_rest-0.7.0/kuflow_rest/_generated/models/__pycache__/_patch.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Jun 16 09:00:12 2023 UTC, .py size: 674 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 9c24 8c64 a202 0000  U........$.d....
+00000000: 550d 0d0a 0000 0000 5b46 9164 a202 0000  U.......[F.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2e00 0000 5500  .....@...s....U.
 00000030: 6400 5a00 6401 6402 6c01 6d02 5a02 0100  d.Z.d.d.l.m.Z...
 00000040: 6700 5a03 6502 6504 1900 6505 6403 3c00  g.Z.e.e...e.d.<.
 00000050: 6404 6405 8400 5a06 6406 5300 2907 7a7b  d.d...Z.d.S.).z{
 00000060: 4375 7374 6f6d 697a 6520 6765 6e65 7261  Customize genera
 00000070: 7465 6420 636f 6465 2068 6572 652e 0a0a  ted code here...
```

### Comparing `kuflow_rest-0.6.1/kuflow_rest/_generated/models/_enums.py` & `kuflow_rest-0.7.0/kuflow_rest/_generated/models/_enums.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.1/kuflow_rest/_generated/models/_models.py` & `kuflow_rest-0.7.0/kuflow_rest/_generated/models/_models.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.1/kuflow_rest/_generated/models/_patch.py` & `kuflow_rest-0.7.0/kuflow_rest/_generated/models/_patch.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.1/kuflow_rest/_generated/operations/__init__.py` & `kuflow_rest-0.7.0/kuflow_rest/_generated/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.1/kuflow_rest/_generated/operations/__pycache__/__init__.cpython-38.pyc` & `kuflow_rest-0.7.0/kuflow_rest/_generated/operations/__pycache__/__init__.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Jun 16 09:00:12 2023 UTC, .py size: 2060 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 9c24 8c64 0c08 0000  U........$.d....
+00000000: 550d 0d0a 0000 0000 5b46 9164 0c08 0000  U.......[F.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7a00 0000 6400  .....@...sz...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c08 6d09 5a0a 0100 6400 6406 6c08  d.l.m.Z...d.d.l.
 00000070: 5400 6400 6407 6c08 6d0b 5a0c 0100 6408  T.d.d.l.m.Z...d.
```

### Comparing `kuflow_rest-0.6.1/kuflow_rest/_generated/operations/__pycache__/_authentication_operations.cpython-38.pyc` & `kuflow_rest-0.7.0/kuflow_rest/_generated/operations/__pycache__/_authentication_operations.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Jun 16 09:00:12 2023 UTC, .py size: 7884 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 9c24 8c64 cc1e 0000  U........$.d....
+00000000: 550d 0d0a 0000 0000 5b46 9164 cc1e 0000  U.......[F.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 0401 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 6d09 5a09 6d0a 5a0a  m.Z.m.Z.m.Z.m.Z.
 00000060: 0100 6400 6403 6c0b 6d0c 5a0c 6d0d 5a0d  ..d.d.l.m.Z.m.Z.
 00000070: 6d0e 5a0e 6d0f 5a0f 6d10 5a10 6d11 5a11  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `kuflow_rest-0.6.1/kuflow_rest/_generated/operations/__pycache__/_patch.cpython-38.pyc` & `kuflow_rest-0.7.0/kuflow_rest/_generated/operations/__pycache__/_patch.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Jun 16 09:00:12 2023 UTC, .py size: 674 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 9c24 8c64 a202 0000  U........$.d....
+00000000: 550d 0d0a 0000 0000 5b46 9164 a202 0000  U.......[F.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2e00 0000 5500  .....@...s....U.
 00000030: 6400 5a00 6401 6402 6c01 6d02 5a02 0100  d.Z.d.d.l.m.Z...
 00000040: 6700 5a03 6502 6504 1900 6505 6403 3c00  g.Z.e.e...e.d.<.
 00000050: 6404 6405 8400 5a06 6406 5300 2907 7a7b  d.d...Z.d.S.).z{
 00000060: 4375 7374 6f6d 697a 6520 6765 6e65 7261  Customize genera
 00000070: 7465 6420 636f 6465 2068 6572 652e 0a0a  ted code here...
```

### Comparing `kuflow_rest-0.6.1/kuflow_rest/_generated/operations/__pycache__/_principal_operations.cpython-38.pyc` & `kuflow_rest-0.7.0/kuflow_rest/_generated/operations/__pycache__/_principal_operations.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Jun 16 09:00:12 2023 UTC, .py size: 9804 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 9c24 8c64 4c26 0000  U........$.dL&..
+00000000: 550d 0d0a 0000 0000 5b46 9164 4c26 0000  U.......[F.dL&..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 4801 0000 6400  .....@...sH...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 6d07 5a07  m.Z.m.Z.m.Z.m.Z.
 00000050: 0100 6400 6402 6c08 6d09 5a09 6d0a 5a0a  ..d.d.l.m.Z.m.Z.
 00000060: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  m.Z.m.Z.m.Z.m.Z.
 00000070: 0100 6400 6403 6c0f 6d10 5a10 0100 6400  ..d.d.l.m.Z...d.
```

### Comparing `kuflow_rest-0.6.1/kuflow_rest/_generated/operations/__pycache__/_process_operations.cpython-38.pyc` & `kuflow_rest-0.7.0/kuflow_rest/_generated/operations/__pycache__/_process_operations.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Jun 16 09:00:12 2023 UTC, .py size: 41967 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 9c24 8c64 efa3 0000  U........$.d....
+00000000: 550d 0d0a 0000 0000 5b46 9164 efa3 0000  U.......[F.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 c201 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 6d09 5a09 6d0a 5a0a  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d0b 5a0b 0100 6400 6403 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
 00000070: 6d0e 5a0e 6d0f 5a0f 6d10 5a10 6d11 5a11  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `kuflow_rest-0.6.1/kuflow_rest/_generated/operations/__pycache__/_task_operations.cpython-38.pyc` & `kuflow_rest-0.7.0/kuflow_rest/_generated/operations/__pycache__/_task_operations.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Jun 16 09:00:12 2023 UTC, .py size: 76156 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 9c24 8c64 7c29 0100  U........$.d|)..
+00000000: 550d 0d0a 0000 0000 5b46 9164 7c29 0100  U.......[F.d|)..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000b 0000 0040 0000 0073 9c02 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 6d09 5a09 6d0a 5a0a  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d0b 5a0b 6d0c 5a0c 0100 6400 6403 6c0d  m.Z.m.Z...d.d.l.
 00000070: 6d0e 5a0e 6d0f 5a0f 6d10 5a10 6d11 5a11  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `kuflow_rest-0.6.1/kuflow_rest/_generated/operations/_authentication_operations.py` & `kuflow_rest-0.7.0/kuflow_rest/_generated/operations/_authentication_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.1/kuflow_rest/_generated/operations/_patch.py` & `kuflow_rest-0.7.0/kuflow_rest/_generated/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.1/kuflow_rest/_generated/operations/_principal_operations.py` & `kuflow_rest-0.7.0/kuflow_rest/_generated/operations/_principal_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.1/kuflow_rest/_generated/operations/_process_operations.py` & `kuflow_rest-0.7.0/kuflow_rest/_generated/operations/_process_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.1/kuflow_rest/_generated/operations/_task_operations.py` & `kuflow_rest-0.7.0/kuflow_rest/_generated/operations/_task_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.1/kuflow_rest/_kuflow_rest_client.py` & `kuflow_rest-0.7.0/kuflow_rest/_kuflow_rest_client.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.1/kuflow_rest/models/__init__.py` & `kuflow_rest-0.7.0/kuflow_rest/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.1/kuflow_rest/models/__pycache__/__init__.cpython-38.pyc` & `kuflow_rest-0.7.0/kuflow_rest/models/__pycache__/__init__.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Jun 16 09:00:12 2023 UTC, .py size: 4771 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 9c24 8c64 a312 0000  U........$.d....
+00000000: 550d 0d0a 0000 0000 5b46 9164 a312 0000  U.......[F.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 003d 0000 0040 0000 0073 aa01 0000 6400  .=...@...s....d.
 00000030: 6401 6c00 6d01 5a02 0100 6400 6402 6c00  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 6d09 5a09 6d0a 5a0a  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0f 5a0f 6d10 5a10 6d11 5a11 6d12 5a12  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `kuflow_rest-0.6.1/kuflow_rest/models/__pycache__/_models.cpython-38.pyc` & `kuflow_rest-0.7.0/kuflow_rest/models/__pycache__/_models.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Jun 16 09:00:12 2023 UTC, .py size: 4581 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 9c24 8c64 e511 0000  U........$.d....
+00000000: 550d 0d0a 0000 0000 5b46 9164 e511 0000  U.......[F.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 7400 0000 6400  .....@...st...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6402  d.l.m.Z.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 4700 6404 6405  d.l.m.Z...G.d.d.
 00000050: 8400 6405 8302 5a05 4700 6406 6407 8400  ..d...Z.G.d.d...
 00000060: 6407 8302 5a06 4700 6408 6409 8400 6409  d...Z.G.d.d...d.
 00000070: 8302 5a07 4700 640a 640b 8400 640b 8302  ..Z.G.d.d...d...
```

### Comparing `kuflow_rest-0.6.1/kuflow_rest/models/_models.py` & `kuflow_rest-0.7.0/kuflow_rest/models/_models.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.1/kuflow_rest/operations/__init__.py` & `kuflow_rest-0.7.0/kuflow_rest/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.1/kuflow_rest/operations/__pycache__/_authentication_operations.cpython-38.pyc` & `kuflow_rest-0.7.0/kuflow_rest/operations/__pycache__/_authentication_operations.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Jun 16 09:00:12 2023 UTC, .py size: 2322 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 9c24 8c64 1209 0000  U........$.d....
+00000000: 550d 0d0a 0000 0000 5b46 9164 1209 0000  U.......[F.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6402 6403 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a04 6d05 5a06 0100 4700 6404 6405  m.Z.m.Z...G.d.d.
 00000050: 8400 6405 8302 5a07 6406 5300 2907 e900  ..d...Z.d.S.)...
 00000060: 0000 0029 01da 0341 6e79 e902 0000 0029  ...)...Any.....)
 00000070: 02da 066d 6f64 656c 73da 104b 7546 6c6f  ...models..KuFlo
```

### Comparing `kuflow_rest-0.6.1/kuflow_rest/operations/__pycache__/_principal_operations.cpython-38.pyc` & `kuflow_rest-0.7.0/kuflow_rest/operations/__pycache__/_principal_operations.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Jun 16 09:00:12 2023 UTC, .py size: 4113 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 9c24 8c64 1110 0000  U........$.d....
+00000000: 550d 0d0a 0000 0000 5b46 9164 1110 0000  U.......[F.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3a00 0000 6400  .....@...s:...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 0100 6402 6403 6c05 6d06 5a07  m.Z...d.d.l.m.Z.
 00000050: 6d08 5a09 0100 4700 6404 6405 8400 6405  m.Z...G.d.d...d.
 00000060: 8302 5a0a 6406 5300 2907 e900 0000 0029  ..Z.d.S.)......)
 00000070: 04da 0341 6e79 da04 4c69 7374 da08 4f70  ...Any..List..Op
```

### Comparing `kuflow_rest-0.6.1/kuflow_rest/operations/__pycache__/_process_operations.cpython-38.pyc` & `kuflow_rest-0.7.0/kuflow_rest/operations/__pycache__/_process_operations.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Jun 16 09:00:12 2023 UTC, .py size: 9530 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 9c24 8c64 3a25 0000  U........$.d:%..
+00000000: 550d 0d0a 0000 0000 5b46 9164 3a25 0000  U.......[F.d:%..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4200 0000 6400  .....@...sB...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 0100 6402 6403 6c05 6d06 5a07  m.Z...d.d.l.m.Z.
 00000050: 0100 6402 6404 6c08 6d09 5a0a 0100 4700  ..d.d.l.m.Z...G.
 00000060: 6405 6406 8400 6406 8302 5a0b 6407 5300  d.d...d...Z.d.S.
 00000070: 2908 e900 0000 0029 04da 0341 6e79 da04  )......)...Any..
```

### Comparing `kuflow_rest-0.6.1/kuflow_rest/operations/__pycache__/_task_operations.cpython-38.pyc` & `kuflow_rest-0.7.0/kuflow_rest/operations/__pycache__/_task_operations.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Jun 16 09:00:12 2023 UTC, .py size: 17424 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 9c24 8c64 1044 0000  U........$.d.D..
+00000000: 550d 0d0a 0000 0000 5b46 9164 1044 0000  U.......[F.d.D..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 0100 6402 6403 6c06  m.Z.m.Z...d.d.l.
 00000050: 6d07 5a08 0100 6402 6404 6c09 6d0a 5a0b  m.Z...d.d.l.m.Z.
 00000060: 0100 4700 6405 6406 8400 6406 8302 5a0c  ..G.d.d...d...Z.
 00000070: 6407 5300 2908 e900 0000 0029 05da 0341  d.S.)......)...A
```

### Comparing `kuflow_rest-0.6.1/kuflow_rest/operations/_authentication_operations.py` & `kuflow_rest-0.7.0/kuflow_rest/operations/_authentication_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.1/kuflow_rest/operations/_principal_operations.py` & `kuflow_rest-0.7.0/kuflow_rest/operations/_principal_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.1/kuflow_rest/operations/_process_operations.py` & `kuflow_rest-0.7.0/kuflow_rest/operations/_process_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.1/kuflow_rest/operations/_task_operations.py` & `kuflow_rest-0.7.0/kuflow_rest/operations/_task_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.1/kuflow_rest/utils/_json_forms.py` & `kuflow_rest-0.7.0/kuflow_rest/utils/json_forms.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,128 +19,138 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 
-from typing import Union, List, Dict, Optional
+from typing import Any, Union, List, Dict, Optional
 from datetime import date, datetime
 import math
 import re
+from abc import ABC, abstractmethod
 
 from ..models import (
-    PrincipalType,
     JsonFormsFile,
     JsonFormsPrincipal,
-    JsonFormsValue,
+    PrincipalType,
     Task,
     TaskPageItem,
     TaskSaveJsonFormsValueDataCommand,
 )
 
-SimpleType = Union[str, int, float, bool, date, JsonFormsPrincipal, JsonFormsFile]
+JsonFormsSimpleType = Union[str, int, float, bool, date, JsonFormsPrincipal, JsonFormsFile]
 
 ContainerArrayType = List["ComplexType"]
 
 ContainerRecordType = Dict[str, "ComplexType"]
 
 ContainerType = Union[ContainerArrayType, ContainerRecordType]
 
-ComplexType = Union[SimpleType, ContainerType]
+ComplexType = Union[JsonFormsSimpleType, ContainerType]
 
 JsonFormsModels = Union[Task, TaskPageItem, TaskSaveJsonFormsValueDataCommand]
 
 
+class JsonFormDataAccessor(ABC):
+    @abstractmethod
+    def get_data(self) -> Optional[Dict[str, Any]]:
+        raise NotImplementedError
+
+    @abstractmethod
+    def set_data(self, data: Optional[Dict[str, Any]]):
+        raise NotImplementedError
+
+
 class JsonFormsProperty:
     container: ContainerType
     path: str
     value: ComplexType
 
     def __init__(self, container: ContainerType, path: str, value: ComplexType):
         self.container = container
         self.path = path
         self.value = value
 
 
-def get_json_forms_property_as_str(model: JsonFormsModels, property_path: str) -> str:
+def get_json_forms_property_as_str(accessor: JsonFormDataAccessor, property_path: str) -> str:
     """
     Get a json property as "str" following the "propertyPath" passed.
 
     Arguments:
-        model: Related model
+        accessor: Json form data accessor.
         property_path: Property path to find. ie: "user.name" or "users.0.name"
 
     Return:
         the property value if exists.
 
     Raises:
         ValueError: If property value doesn't exist or has incorrect format
     """
-    value = find_json_forms_property_as_str(model, property_path)
+    value = find_json_forms_property_as_str(accessor, property_path)
     if value is None:
         raise ValueError("Property value doesn't exist")
     return value
 
 
-def find_json_forms_property_as_str(model: JsonFormsModels, property_path: str) -> Optional[str]:
+def find_json_forms_property_as_str(accessor: JsonFormDataAccessor, property_path: str) -> Optional[str]:
     """
     Try to find a json property as "str" following the "propertyPath" passed.
 
     Arguments:
-        model: Related model
+        accessor: Json form data accessor.
         property_path: Property path to find. ie: "user.name" or "users.0.name"
 
     Return:
         The property value if exists.
 
     Raises:
         ValueError: If property value has incorrect format
     """
-    value = find_json_forms_property_value(model, property_path)
+    value = find_json_forms_property_value(accessor, property_path)
     if value is not None:
         return str(value)
     return None
 
 
-def get_json_forms_property_as_int(model, property_path) -> int:
+def get_json_forms_property_as_int(accessor: JsonFormDataAccessor, property_path: str) -> int:
     """
     Get a json property as "int" following the "propertyPath" passed.
 
     Arguments:
-        model: Related model
+        accessor: Json form data accessor.
         property_path: Property path to find. ie: "user.name" or "users.0.name"
 
     Return:
         the property value if exists.
 
     Raises:
         ValueError: If property value doesn't exist or has incorrect format
     """
-    value = find_json_forms_property_as_int(model, property_path)
+    value = find_json_forms_property_as_int(accessor, property_path)
     if value is None:
         raise ValueError("Property value doesn't exist")
     return value
 
 
-def find_json_forms_property_as_int(model, property_path) -> Optional[int]:
+def find_json_forms_property_as_int(accessor: JsonFormDataAccessor, property_path: str) -> Optional[int]:
     """
     Try to find a json property as "int" following the "propertyPath" passed.
 
     Arguments:
-        model: Related model
+        accessor: Json form data accessor.
         property_path: Property path to find. ie: "user.name" or "users.0.name"
 
     Return:
         The property value if exists.
 
     Raises:
         ValueError: If property value has incorrect format
     """
-    value = find_json_forms_property_value(model, property_path)
+    value = find_json_forms_property_value(accessor, property_path)
     if value is None:
         return None
 
     if isinstance(value, int):
         if not math.isnan(value):
             return value
 
@@ -149,49 +159,49 @@
             return int(value)
         except ValueError:
             pass
 
     raise ValueError(f"Property {property_path} is not a int")
 
 
-def get_json_forms_property_as_float(model, property_path) -> float:
+def get_json_forms_property_as_float(accessor: JsonFormDataAccessor, property_path: str) -> float:
     """
     Get a json property as "float" following the "propertyPath" passed.
 
     Arguments:
-        model: Related model
+        accessor: Json form data accessor.
         property_path: Property path to find. ie: "user.name" or "users.0.name"
 
     Return:
         the property value if exists.
 
     Raises:
         ValueError: If property value doesn't exist or has incorrect format
     """
-    value = find_json_forms_property_as_float(model, property_path)
+    value = find_json_forms_property_as_float(accessor, property_path)
     if value is None:
         raise ValueError("Property value doesn't exist")
     return value
 
 
-def find_json_forms_property_as_float(model, property_path) -> Optional[float]:
+def find_json_forms_property_as_float(accessor: JsonFormDataAccessor, property_path: str) -> Optional[float]:
     """
     Try to find a json property as "float" following the "propertyPath" passed.
 
     Arguments:
-        model: Related model
+        accessor: Json form data accessor.
         property_path: Property path to find. ie: "user.name" or "users.0.name"
 
     Return:
         The property value if exists.
 
     Raises:
         ValueError: If property value has incorrect format
     """
-    value = find_json_forms_property_value(model, property_path)
+    value = find_json_forms_property_value(accessor, property_path)
     if value is None:
         return None
 
     if isinstance(value, int):
         if not math.isnan(value):
             return float(value)
 
@@ -204,49 +214,49 @@
             return float(value)
         except ValueError:
             pass
 
     raise ValueError(f"Property {property_path} is not a float")
 
 
-def get_json_forms_property_as_date(model, property_path) -> date:
+def get_json_forms_property_as_date(accessor: JsonFormDataAccessor, property_path: str) -> date:
     """
     Get a json property as "date" following the "propertyPath" passed.
 
     Arguments:
-        model: Related model
+        accessor: Json form data accessor.
         property_path: Property path to find. ie: "user.name" or "users.0.name"
 
     Return:
         the property value if exists.
 
     Raises:
         ValueError: If property value doesn't exist or has incorrect format
     """
-    value = find_json_forms_property_as_date(model, property_path)
+    value = find_json_forms_property_as_date(accessor, property_path)
     if value is None:
         raise ValueError("Property value doesn't exist")
     return value
 
 
-def find_json_forms_property_as_date(model, property_path) -> Optional[date]:
+def find_json_forms_property_as_date(accessor: JsonFormDataAccessor, property_path: str) -> Optional[date]:
     """
     Try to find a json property as "date" following the "propertyPath" passed.
 
     Arguments:
-        model: Related model
+        accessor: Json form data accessor.
         property_path: Property path to find. ie: "user.name" or "users.0.name"
 
     Return:
         The property value if exists.
 
     Raises:
         ValueError: If property value has incorrect format
     """
-    value = find_json_forms_property_value(model, property_path)
+    value = find_json_forms_property_value(accessor, property_path)
     if value is None:
         return None
 
     if isinstance(value, date):
         return value
 
     if isinstance(value, str):
@@ -254,49 +264,49 @@
             return date.fromisoformat(value)
         except ValueError:
             pass
 
     raise ValueError(f"Property {property_path} is not a date following ISO 8601 format")
 
 
-def get_json_forms_property_as_datetime(model, property_path) -> datetime:
+def get_json_forms_property_as_datetime(accessor: JsonFormDataAccessor, property_path: str) -> datetime:
     """
     Get a json property as "datetime" following the "propertyPath" passed.
 
     Arguments:
-        model: Related model
+        accessor: Json form data accessor.
         property_path: Property path to find. ie: "user.name" or "users.0.name"
 
     Return:
         the property value if exists.
 
     Raises:
         ValueError: If property value doesn't exist or has incorrect format
     """
-    value = find_json_forms_property_as_datetime(model, property_path)
+    value = find_json_forms_property_as_datetime(accessor, property_path)
     if value is None:
         raise ValueError("Property value doesn't exist")
     return value
 
 
-def find_json_forms_property_as_datetime(model, property_path) -> Optional[datetime]:
+def find_json_forms_property_as_datetime(accessor: JsonFormDataAccessor, property_path: str) -> Optional[datetime]:
     """
     Try to find a json property as "datetime" following the "propertyPath" passed.
 
     Arguments:
-        model: Related model
+        accessor: Json form data accessor.
         property_path: Property path to find. ie: "user.name" or "users.0.name"
 
     Return:
         The property value if exists.
 
     Raises:
         ValueError: If property value has incorrect format
     """
-    value = find_json_forms_property_value(model, property_path)
+    value = find_json_forms_property_value(accessor, property_path)
     if value is None:
         return None
 
     if isinstance(value, datetime):
         return value
 
     if isinstance(value, str):
@@ -304,218 +314,222 @@
             return datetime.fromisoformat(value)
         except ValueError:
             pass
 
     raise ValueError(f"Property {property_path} is not a date-time following ISO 8601 format")
 
 
-def get_json_forms_property_as_json_forms_file(model, property_path) -> JsonFormsFile:
+def get_json_forms_property_as_json_forms_file(accessor: JsonFormDataAccessor, property_path: str) -> JsonFormsFile:
     """
     Get a json property as "JsonFormsFile" following the "propertyPath" passed.
 
     Arguments:
-        model: Related model
+        accessor: Json form data accessor.
         property_path: Property path to find. ie: "user.name" or "users.0.name"
 
     Return:
         the property value if exists.
 
     Raises:
         ValueError: If property value doesn't exist or has incorrect format
     """
-    value = find_json_forms_property_as_json_forms_file(model, property_path)
+    value = find_json_forms_property_as_json_forms_file(accessor, property_path)
     if value is None:
         raise ValueError("Property value doesn't exist")
     return value
 
 
-def find_json_forms_property_as_json_forms_file(model, property_path) -> Optional[JsonFormsFile]:
+def find_json_forms_property_as_json_forms_file(
+    accessor: JsonFormDataAccessor, property_path: str
+) -> Optional[JsonFormsFile]:
     """
     Try to find a json property as "JsonFormsFile" following the "propertyPath" passed.
 
     Arguments:
-        model: Related model
+        accessor: Json form data accessor.
         property_path: Property path to find. ie: "user.name" or "users.0.name"
 
     Return:
         The property value if exists.
 
     Raises:
         ValueError: If property value has incorrect format
     """
-    value = find_json_forms_property_value(model, property_path)
+    value = find_json_forms_property_value(accessor, property_path)
     if value is None:
         return None
 
     json_forms_file = try_parse_json_forms_file(value)
     if json_forms_file is None:
         raise ValueError(f"Property {property_path} is not a file")
 
     return json_forms_file
 
 
-def get_json_forms_property_as_json_forms_principal(model, property_path) -> JsonFormsPrincipal:
+def get_json_forms_property_as_json_forms_principal(
+    accessor: JsonFormDataAccessor, property_path: str
+) -> JsonFormsPrincipal:
     """
     Get a json property as "JsonFormsPrincipal" following the "propertyPath" passed.
 
     Arguments:
-        model: Related model
+        accessor: Json form data accessor.
         property_path: Property path to find. ie: "user.name" or "users.0.name"
 
     Return:
         the property value if exists.
 
     Raises:
         ValueError: If property value doesn't exist or has incorrect format
     """
-    value = find_json_forms_property_as_json_forms_principal(model, property_path)
+    value = find_json_forms_property_as_json_forms_principal(accessor, property_path)
     if value is None:
         raise ValueError("Property value doesn't exist")
     return value
 
 
-def find_json_forms_property_as_json_forms_principal(model, property_path) -> Optional[JsonFormsPrincipal]:
+def find_json_forms_property_as_json_forms_principal(
+    accessor: JsonFormDataAccessor, property_path: str
+) -> Optional[JsonFormsPrincipal]:
     """
     Try to find a json property as "JsonFormsPrincipal" following the "propertyPath" passed.
 
     Arguments:
-        model: Related model
+        accessor: Json form data accessor.
         property_path: Property path to find. ie: "user.name" or "users.0.name"
 
     Return:
         The property value if exists.
 
     Raises:
         ValueError: If property value has incorrect format
     """
-    value = find_json_forms_property_value(model, property_path)
+    value = find_json_forms_property_value(accessor, property_path)
     if value is None:
         return None
 
     json_forms_file = try_parse_json_forms_principal(value)
     if json_forms_file is None:
         raise ValueError(f"Property {property_path} is not a principal")
 
     return json_forms_file
 
 
-def get_json_forms_property_as_list(model, property_path) -> list:
+def get_json_forms_property_as_list(accessor: JsonFormDataAccessor, property_path: str) -> list:
     """
     Get a json property as "list" following the "propertyPath" passed.
 
     Arguments:
-        model: Related model
+        accessor: Json form data accessor.
         property_path: Property path to find. ie: "user.name" or "users.0.name"
 
     Return:
         the property value if exists.
 
     Raises:
         ValueError: If property value doesn't exist or has incorrect format
     """
-    value = find_json_forms_property_as_list(model, property_path)
+    value = find_json_forms_property_as_list(accessor, property_path)
     if value is None:
         raise ValueError("Property value doesn't exist")
     return value
 
 
-def find_json_forms_property_as_list(model, property_path) -> Optional[list]:
+def find_json_forms_property_as_list(accessor: JsonFormDataAccessor, property_path: str) -> Optional[list]:
     """
     Try to find a json property as "list" following the "propertyPath" passed.
 
     Arguments:
-        model: Related model
+        accessor: Json form data accessor.
         property_path: Property path to find. ie: "user.name" or "users.0.name"
 
     Return:
         The property value if exists.
 
     Raises:
         ValueError: If property value has incorrect format
     """
-    value = find_json_forms_property_value(model, property_path)
+    value = find_json_forms_property_value(accessor, property_path)
     if value is None:
         return None
 
     if isinstance(value, list):
         return value
 
     raise ValueError(f"Property {property_path} is not a list")
 
 
-def get_json_forms_property_as_dict(model, property_path) -> dict:
+def get_json_forms_property_as_dict(accessor: JsonFormDataAccessor, property_path: str) -> dict:
     """
     Get a json property as "dict" following the "propertyPath" passed.
 
     Arguments:
-        model: Related model
+        accessor: Json form data accessor.
         property_path: Property path to find. ie: "user.name" or "users.0.name"
 
     Return:
         the property value if exists.
 
     Raises:
         ValueError: If property value doesn't exist or has incorrect format
     """
-    value = find_json_forms_property_as_dict(model, property_path)
+    value = find_json_forms_property_as_dict(accessor, property_path)
     if value is None:
         raise ValueError("Property value doesn't exist")
     return value
 
 
-def find_json_forms_property_as_dict(model, property_path) -> Optional[dict]:
+def find_json_forms_property_as_dict(accessor: JsonFormDataAccessor, property_path: str) -> Optional[dict]:
     """
     Try to find a json property as "dict" following the "propertyPath" passed.
 
     Arguments:
-        model: Related model
+        accessor: Json form data accessor.
         property_path: Property path to find. ie: "user.name" or "users.0.name"
 
     Return:
         The property value if exists.
 
     Raises:
         ValueError: If property value has incorrect format
     """
-    value = find_json_forms_property_value(model, property_path)
+    value = find_json_forms_property_value(accessor, property_path)
     if value is None:
         return None
 
     if isinstance(value, dict):
         return value
 
     raise ValueError(f"Property {property_path} is not a dict")
 
 
 def find_json_forms_property_value(
-    model: JsonFormsModels, property_path: str, create_missing_parents: bool = True
+    accessor: JsonFormDataAccessor, property_path: str, create_missing_parents: bool = True
 ) -> Optional[ComplexType]:
-    property = find_json_forms_property(model, property_path, create_missing_parents)
+    property = find_json_forms_property(accessor, property_path, create_missing_parents)
     if property is not None:
         return property.value
     return None
 
 
 def update_json_forms_property(
-    model: JsonFormsModels,
-    property_path: str,
-    value: Optional[SimpleType],
+    accessor: JsonFormDataAccessor, property_path: str, value: Optional[JsonFormsSimpleType]
 ) -> None:
     """
     Update a json forms data property in the task passed following the "property_path".
 
     Arguments:
-        model: Related model
+        accessor: Json form data accessor.
         property_path: Property path to find. ie: "user.name" or "users.0.name"
         value: Value to update
 
     Raises:
         ValueError: If property value has incorrect format
     """
-    property = find_json_forms_property(model, property_path, True)
+    property = find_json_forms_property(accessor, property_path, True)
 
     value = transform_json_forms_property_value(value)
 
     if property is None:
         raise ValueError(f"Property {property_path} doesn't exist")
 
     json_forms_property_container = property.container
@@ -536,31 +550,31 @@
             del json_forms_property_container[json_forms_property_path]
     else:
         raise ValueError(f"Incorrect property path {json_forms_property_path}")
 
 
 # flake8: noqa: C901
 def find_json_forms_property(
-    model: JsonFormsModels, property_path: str, create_missing_parents: bool = False
+    accessor: JsonFormDataAccessor, property_path: str, create_missing_parents: bool = False
 ) -> Optional[JsonFormsProperty]:
     """
     Try to find a json property following the "property_path" passed.
 
     Arguments:
-        model: Related model
+        accessor: Json form data accessor.
         property_path: Property path to find. ie: "user.name" or "users.0.name"
         create_missing_parents: Create parent paths if are missing
 
     Return:
         The property value if exists.
 
     Raises:
         ValueError: If property value has incorrect format or a wrong path
     """
-    property_data = get_json_forms_value_data(model, create_missing_parents)
+    property_data = get_json_forms_value_data(accessor, create_missing_parents)
     if property_data is None:
         return None
 
     property_container: ContainerType = property_data
     property_value_path = ""
     property_value: Optional[ComplexType] = None
 
@@ -617,15 +631,15 @@
         if property_value is not None and is_json_forms_type_container(property_value) and idx + 1 < len(paths):
             property_container = property_value
             property_value = None
 
     return JsonFormsProperty(container=property_container, path=property_value_path, value=property_value)
 
 
-def transform_json_forms_property_value(value: Optional[SimpleType]) -> Optional[SimpleType]:
+def transform_json_forms_property_value(value: Optional[JsonFormsSimpleType]) -> Optional[JsonFormsSimpleType]:
     if value is None:
         return None
     elif isinstance(value, JsonFormsPrincipal):
         return generate_value_for_json_forms_principal(value)
     elif isinstance(value, JsonFormsFile):
         return generate_value_for_json_forms_file(value)
     elif isinstance(value, date):
@@ -732,24 +746,15 @@
     return isinstance(value, dict)
 
 
 def is_json_forms_type_container_array(value: Optional[ComplexType]) -> bool:
     return isinstance(value, list)
 
 
-def get_json_forms_value_data(model: JsonFormsModels, create_missing_parents: bool) -> Optional[ContainerType]:
-    data: Optional[ContainerType] = None
-
-    if isinstance(model, Task) or isinstance(model, TaskPageItem):
-        data = model.json_forms_value.data if model.json_forms_value else None
-    else:
-        data = model.data
+def get_json_forms_value_data(accessor: JsonFormDataAccessor, create_missing_parents: bool) -> Optional[ContainerType]:
+    data: Optional[ContainerType] = accessor.get_data()
 
     if data is None and create_missing_parents:
         data = {}
-        if isinstance(model, Task) or isinstance(model, TaskPageItem):
-            model.json_forms_value = model.json_forms_value or JsonFormsValue()
-            model.json_forms_value.data = data
-        else:
-            model.data = data
+        accessor.set_data(data)
 
     return data
```

### Comparing `kuflow_rest-0.6.1/pyproject.toml` & `kuflow_rest-0.7.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kuflow-rest"
-version = "0.6.1"
+version = "0.7.0"
 description = "Client for KuFlow Rest Api"
 license = "MIT"
 authors = ["KuFlow S.L. <kuflow@kuflow.com>"]
 homepage = "https://kuflow.com/"
 documentation = "https://docs.kuflow.com/"
 repository = "https://github.com/kuflow/kuflow-sdk-python"
 readme = "README.md"
```

### Comparing `kuflow_rest-0.6.1/setup.py` & `kuflow_rest-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 {'': ['*']}
 
 install_requires = \
 ['azure-core>=1.26.4,<2.0.0', 'isodate>=0.6.1,<0.7.0']
 
 setup_kwargs = {
     'name': 'kuflow-rest',
-    'version': '0.6.1',
+    'version': '0.7.0',
     'description': 'Client for KuFlow Rest Api',
     'long_description': '[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)\n[![Python](https://img.shields.io/pypi/pyversions/kuflow-rest.svg)](https://pypi.org/project/kuflow-rest)\n[![PyPI](https://img.shields.io/pypi/v/kuflow-rest.svg)](https://pypi.org/project/kuflow-rest)\n\n# KuFlow Rest\n\nThis is a client for the KuFlow API Rest that allows you to interact with our API in a comfortable way in the creation of your workers and tools.\n\n## Documentation\n\nMore detailed docs are available in the [documentation pages](https://docs.kuflow.com/developers/).\n\n## Contributing\n\nWe are happy to receive your help and comments, together we will dance a wonderful KuFlow. Please review our [contribution guide](CONTRIBUTING.md).\n\n## License\n\n[MIT License](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)\n',
     'author': 'KuFlow S.L.',
     'author_email': 'kuflow@kuflow.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://kuflow.com/',
```

### Comparing `kuflow_rest-0.6.1/PKG-INFO` & `kuflow_rest-0.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kuflow-rest
-Version: 0.6.1
+Version: 0.7.0
 Summary: Client for KuFlow Rest Api
 Home-page: https://kuflow.com/
 License: MIT
 Author: KuFlow S.L.
 Author-email: kuflow@kuflow.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

