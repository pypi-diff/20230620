# Comparing `tmp/soda-core-dremio-3.0.40.tar.gz` & `tmp/soda-core-dremio-3.0.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda-core-dremio-3.0.40.tar", last modified: Fri Jun 16 08:29:19 2023, max compression
+gzip compressed data, was "soda-core-dremio-3.0.41.tar", last modified: Tue Jun 20 12:55:22 2023, max compression
```

## Comparing `soda-core-dremio-3.0.40.tar` & `soda-core-dremio-3.0.41.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 08:29:19.454727 soda-core-dremio-3.0.40/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-06-16 08:29:19.454727 soda-core-dremio-3.0.40/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-16 08:29:19.454727 soda-core-dremio-3.0.40/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      585 2023-06-16 08:28:48.000000 soda-core-dremio-3.0.40/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 08:29:19.450727 soda-core-dremio-3.0.40/soda/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 08:29:19.450727 soda-core-dremio-3.0.40/soda/data_sources/
--rw-r--r--   0 runner    (1001) docker     (122)     5458 2023-06-16 08:28:48.000000 soda-core-dremio-3.0.40/soda/data_sources/dremio_data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 08:29:19.454727 soda-core-dremio-3.0.40/soda_core_dremio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-06-16 08:29:19.000000 soda-core-dremio-3.0.40/soda_core_dremio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      268 2023-06-16 08:29:19.000000 soda-core-dremio-3.0.40/soda_core_dremio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-16 08:29:19.000000 soda-core-dremio-3.0.40/soda_core_dremio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-06-16 08:29:19.000000 soda-core-dremio-3.0.40/soda_core_dremio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-16 08:29:19.000000 soda-core-dremio-3.0.40/soda_core_dremio.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 08:29:19.454727 soda-core-dremio-3.0.40/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      141 2023-06-16 08:28:48.000000 soda-core-dremio-3.0.40/tests/test_dremio.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 12:55:22.858844 soda-core-dremio-3.0.41/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-06-20 12:55:22.858844 soda-core-dremio-3.0.41/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-20 12:55:22.858844 soda-core-dremio-3.0.41/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      585 2023-06-20 12:54:46.000000 soda-core-dremio-3.0.41/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 12:55:22.858844 soda-core-dremio-3.0.41/soda/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 12:55:22.858844 soda-core-dremio-3.0.41/soda/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (122)     5458 2023-06-20 12:54:46.000000 soda-core-dremio-3.0.41/soda/data_sources/dremio_data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 12:55:22.858844 soda-core-dremio-3.0.41/soda_core_dremio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-06-20 12:55:22.000000 soda-core-dremio-3.0.41/soda_core_dremio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      268 2023-06-20 12:55:22.000000 soda-core-dremio-3.0.41/soda_core_dremio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-20 12:55:22.000000 soda-core-dremio-3.0.41/soda_core_dremio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-06-20 12:55:22.000000 soda-core-dremio-3.0.41/soda_core_dremio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-20 12:55:22.000000 soda-core-dremio-3.0.41/soda_core_dremio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 12:55:22.858844 soda-core-dremio-3.0.41/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      141 2023-06-20 12:54:46.000000 soda-core-dremio-3.0.41/tests/test_dremio.py
```

### Comparing `soda-core-dremio-3.0.40/soda/data_sources/dremio_data_source.py` & `soda-core-dremio-3.0.41/soda/data_sources/dremio_data_source.py`

 * *Files identical despite different names*

