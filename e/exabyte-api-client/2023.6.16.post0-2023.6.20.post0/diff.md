# Comparing `tmp/exabyte-api-client-2023.6.16.post0.tar.gz` & `tmp/exabyte-api-client-2023.6.20.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exabyte-api-client-2023.6.16.post0.tar", last modified: Fri Jun 16 01:19:32 2023, max compression
+gzip compressed data, was "exabyte-api-client-2023.6.20.post0.tar", last modified: Tue Jun 20 02:15:41 2023, max compression
```

## Comparing `exabyte-api-client-2023.6.16.post0.tar` & `exabyte-api-client-2023.6.20.post0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:19:32.410457 exabyte-api-client-2023.6.16.post0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:19:32.402457 exabyte-api-client-2023.6.16.post0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:19:32.406457 exabyte-api-client-2023.6.16.post0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-06-16 01:18:55.000000 exabyte-api-client-2023.6.16.post0/.github/workflows/cicd.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-06-16 01:18:55.000000 exabyte-api-client-2023.6.16.post0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-16 01:18:55.000000 exabyte-api-client-2023.6.16.post0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-16 01:18:55.000000 exabyte-api-client-2023.6.16.post0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-16 01:19:32.410457 exabyte-api-client-2023.6.16.post0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-16 01:18:55.000000 exabyte-api-client-2023.6.16.post0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:19:32.402457 exabyte-api-client-2023.6.16.post0/exabyte_api_client/
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-16 01:18:55.000000 exabyte-api-client-2023.6.16.post0/exabyte_api_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-16 01:19:32.000000 exabyte-api-client-2023.6.16.post0/exabyte_api_client/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:19:32.406457 exabyte-api-client-2023.6.16.post0/exabyte_api_client/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-16 01:18:55.000000 exabyte-api-client-2023.6.16.post0/exabyte_api_client/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-16 01:18:55.000000 exabyte-api-client-2023.6.16.post0/exabyte_api_client/endpoints/bank_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 01:18:55.000000 exabyte-api-client-2023.6.16.post0/exabyte_api_client/endpoints/bank_materials.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-16 01:18:55.000000 exabyte-api-client-2023.6.16.post0/exabyte_api_client/endpoints/bank_workflows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-16 01:18:55.000000 exabyte-api-client-2023.6.16.post0/exabyte_api_client/endpoints/charges.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-06-16 01:18:55.000000 exabyte-api-client-2023.6.16.post0/exabyte_api_client/endpoints/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-16 01:18:55.000000 exabyte-api-client-2023.6.16.post0/exabyte_api_client/endpoints/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-06-16 01:18:55.000000 exabyte-api-client-2023.6.16.post0/exabyte_api_client/endpoints/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-06-16 01:18:55.000000 exabyte-api-client-2023.6.16.post0/exabyte_api_client/endpoints/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-16 01:18:55.000000 exabyte-api-client-2023.6.16.post0/exabyte_api_client/endpoints/logout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-06-16 01:18:55.000000 exabyte-api-client-2023.6.16.post0/exabyte_api_client/endpoints/materials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:19:32.406457 exabyte-api-client-2023.6.16.post0/exabyte_api_client/endpoints/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 01:18:55.000000 exabyte-api-client-2023.6.16.post0/exabyte_api_client/endpoints/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-16 01:18:55.000000 exabyte-api-client-2023.6.16.post0/exabyte_api_client/endpoints/mixins/default.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-16 01:18:55.000000 exabyte-api-client-2023.6.16.post0/exabyte_api_client/endpoints/mixins/set.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-16 01:18:55.000000 exabyte-api-client-2023.6.16.post0/exabyte_api_client/endpoints/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-06-16 01:18:55.000000 exabyte-api-client-2023.6.16.post0/exabyte_api_client/endpoints/raw_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-16 01:18:55.000000 exabyte-api-client-2023.6.16.post0/exabyte_api_client/endpoints/refined_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-16 01:18:55.000000 exabyte-api-client-2023.6.16.post0/exabyte_api_client/endpoints/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:19:32.406457 exabyte-api-client-2023.6.16.post0/exabyte_api_client/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 01:18:55.000000 exabyte-api-client-2023.6.16.post0/exabyte_api_client/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-06-16 01:18:55.000000 exabyte-api-client-2023.6.16.post0/exabyte_api_client/utils/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-16 01:18:55.000000 exabyte-api-client-2023.6.16.post0/exabyte_api_client/utils/materials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:19:32.406457 exabyte-api-client-2023.6.16.post0/exabyte_api_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-16 01:19:32.000000 exabyte-api-client-2023.6.16.post0/exabyte_api_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-06-16 01:19:32.000000 exabyte-api-client-2023.6.16.post0/exabyte_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 01:19:32.000000 exabyte-api-client-2023.6.16.post0/exabyte_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-16 01:19:32.000000 exabyte-api-client-2023.6.16.post0/exabyte_api_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-16 01:19:32.000000 exabyte-api-client-2023.6.16.post0/exabyte_api_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-16 01:18:55.000000 exabyte-api-client-2023.6.16.post0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-16 01:18:55.000000 exabyte-api-client-2023.6.16.post0/requirements-dev.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1221 2023-06-16 01:18:55.000000 exabyte-api-client-2023.6.16.post0/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-16 01:19:32.410457 exabyte-api-client-2023.6.16.post0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:19:32.406457 exabyte-api-client-2023.6.16.post0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-16 01:18:55.000000 exabyte-api-client-2023.6.16.post0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:19:32.406457 exabyte-api-client-2023.6.16.post0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-16 01:18:55.000000 exabyte-api-client-2023.6.16.post0/tests/data/login.json
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-16 01:18:55.000000 exabyte-api-client-2023.6.16.post0/tests/data/logout.json
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-16 01:18:55.000000 exabyte-api-client-2023.6.16.post0/tests/data/material.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:19:32.406457 exabyte-api-client-2023.6.16.post0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-16 01:18:55.000000 exabyte-api-client-2023.6.16.post0/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-06-16 01:18:55.000000 exabyte-api-client-2023.6.16.post0/tests/integration/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-06-16 01:18:55.000000 exabyte-api-client-2023.6.16.post0/tests/integration/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-16 01:18:55.000000 exabyte-api-client-2023.6.16.post0/tests/integration/test_materials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:19:32.410457 exabyte-api-client-2023.6.16.post0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-16 01:18:55.000000 exabyte-api-client-2023.6.16.post0/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-16 01:18:55.000000 exabyte-api-client-2023.6.16.post0/tests/unit/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-16 01:18:55.000000 exabyte-api-client-2023.6.16.post0/tests/unit/test_bank_materials.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-16 01:18:55.000000 exabyte-api-client-2023.6.16.post0/tests/unit/test_bank_workflows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-16 01:18:55.000000 exabyte-api-client-2023.6.16.post0/tests/unit/test_httpBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-16 01:18:55.000000 exabyte-api-client-2023.6.16.post0/tests/unit/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-16 01:18:55.000000 exabyte-api-client-2023.6.16.post0/tests/unit/test_login.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-16 01:18:55.000000 exabyte-api-client-2023.6.16.post0/tests/unit/test_logout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-16 01:18:55.000000 exabyte-api-client-2023.6.16.post0/tests/unit/test_materials.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-16 01:18:55.000000 exabyte-api-client-2023.6.16.post0/tests/unit/test_refined_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-16 01:18:55.000000 exabyte-api-client-2023.6.16.post0/tests/unit/test_workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:15:41.380164 exabyte-api-client-2023.6.20.post0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:15:41.376165 exabyte-api-client-2023.6.20.post0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:15:41.380164 exabyte-api-client-2023.6.20.post0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-06-20 02:15:02.000000 exabyte-api-client-2023.6.20.post0/.github/workflows/cicd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-06-20 02:15:02.000000 exabyte-api-client-2023.6.20.post0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-20 02:15:02.000000 exabyte-api-client-2023.6.20.post0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-20 02:15:02.000000 exabyte-api-client-2023.6.20.post0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-20 02:15:41.380164 exabyte-api-client-2023.6.20.post0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-20 02:15:02.000000 exabyte-api-client-2023.6.20.post0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:15:41.376165 exabyte-api-client-2023.6.20.post0/exabyte_api_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-20 02:15:02.000000 exabyte-api-client-2023.6.20.post0/exabyte_api_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-20 02:15:41.000000 exabyte-api-client-2023.6.20.post0/exabyte_api_client/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:15:41.380164 exabyte-api-client-2023.6.20.post0/exabyte_api_client/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-06-20 02:15:02.000000 exabyte-api-client-2023.6.20.post0/exabyte_api_client/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-20 02:15:02.000000 exabyte-api-client-2023.6.20.post0/exabyte_api_client/endpoints/bank_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-20 02:15:02.000000 exabyte-api-client-2023.6.20.post0/exabyte_api_client/endpoints/bank_materials.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-20 02:15:02.000000 exabyte-api-client-2023.6.20.post0/exabyte_api_client/endpoints/bank_workflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-20 02:15:02.000000 exabyte-api-client-2023.6.20.post0/exabyte_api_client/endpoints/charges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-06-20 02:15:02.000000 exabyte-api-client-2023.6.20.post0/exabyte_api_client/endpoints/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-20 02:15:02.000000 exabyte-api-client-2023.6.20.post0/exabyte_api_client/endpoints/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-06-20 02:15:02.000000 exabyte-api-client-2023.6.20.post0/exabyte_api_client/endpoints/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-06-20 02:15:02.000000 exabyte-api-client-2023.6.20.post0/exabyte_api_client/endpoints/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-20 02:15:02.000000 exabyte-api-client-2023.6.20.post0/exabyte_api_client/endpoints/logout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-06-20 02:15:02.000000 exabyte-api-client-2023.6.20.post0/exabyte_api_client/endpoints/materials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:15:41.380164 exabyte-api-client-2023.6.20.post0/exabyte_api_client/endpoints/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 02:15:02.000000 exabyte-api-client-2023.6.20.post0/exabyte_api_client/endpoints/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-20 02:15:02.000000 exabyte-api-client-2023.6.20.post0/exabyte_api_client/endpoints/mixins/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-20 02:15:02.000000 exabyte-api-client-2023.6.20.post0/exabyte_api_client/endpoints/mixins/set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-20 02:15:02.000000 exabyte-api-client-2023.6.20.post0/exabyte_api_client/endpoints/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-06-20 02:15:02.000000 exabyte-api-client-2023.6.20.post0/exabyte_api_client/endpoints/raw_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-20 02:15:02.000000 exabyte-api-client-2023.6.20.post0/exabyte_api_client/endpoints/refined_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-20 02:15:02.000000 exabyte-api-client-2023.6.20.post0/exabyte_api_client/endpoints/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:15:41.380164 exabyte-api-client-2023.6.20.post0/exabyte_api_client/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 02:15:02.000000 exabyte-api-client-2023.6.20.post0/exabyte_api_client/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-06-20 02:15:02.000000 exabyte-api-client-2023.6.20.post0/exabyte_api_client/utils/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-20 02:15:02.000000 exabyte-api-client-2023.6.20.post0/exabyte_api_client/utils/materials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:15:41.380164 exabyte-api-client-2023.6.20.post0/exabyte_api_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-20 02:15:41.000000 exabyte-api-client-2023.6.20.post0/exabyte_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-06-20 02:15:41.000000 exabyte-api-client-2023.6.20.post0/exabyte_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 02:15:41.000000 exabyte-api-client-2023.6.20.post0/exabyte_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-20 02:15:41.000000 exabyte-api-client-2023.6.20.post0/exabyte_api_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-20 02:15:41.000000 exabyte-api-client-2023.6.20.post0/exabyte_api_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-20 02:15:02.000000 exabyte-api-client-2023.6.20.post0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-20 02:15:02.000000 exabyte-api-client-2023.6.20.post0/requirements-dev.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1221 2023-06-20 02:15:02.000000 exabyte-api-client-2023.6.20.post0/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-20 02:15:41.384165 exabyte-api-client-2023.6.20.post0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:15:41.380164 exabyte-api-client-2023.6.20.post0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-20 02:15:02.000000 exabyte-api-client-2023.6.20.post0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:15:41.380164 exabyte-api-client-2023.6.20.post0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-20 02:15:02.000000 exabyte-api-client-2023.6.20.post0/tests/data/login.json
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-20 02:15:02.000000 exabyte-api-client-2023.6.20.post0/tests/data/logout.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-20 02:15:02.000000 exabyte-api-client-2023.6.20.post0/tests/data/material.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:15:41.380164 exabyte-api-client-2023.6.20.post0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-20 02:15:02.000000 exabyte-api-client-2023.6.20.post0/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-06-20 02:15:02.000000 exabyte-api-client-2023.6.20.post0/tests/integration/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-06-20 02:15:02.000000 exabyte-api-client-2023.6.20.post0/tests/integration/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-20 02:15:02.000000 exabyte-api-client-2023.6.20.post0/tests/integration/test_materials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:15:41.380164 exabyte-api-client-2023.6.20.post0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-20 02:15:02.000000 exabyte-api-client-2023.6.20.post0/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-20 02:15:02.000000 exabyte-api-client-2023.6.20.post0/tests/unit/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-20 02:15:02.000000 exabyte-api-client-2023.6.20.post0/tests/unit/test_bank_materials.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-20 02:15:02.000000 exabyte-api-client-2023.6.20.post0/tests/unit/test_bank_workflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-20 02:15:02.000000 exabyte-api-client-2023.6.20.post0/tests/unit/test_httpBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-20 02:15:02.000000 exabyte-api-client-2023.6.20.post0/tests/unit/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-20 02:15:02.000000 exabyte-api-client-2023.6.20.post0/tests/unit/test_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-20 02:15:02.000000 exabyte-api-client-2023.6.20.post0/tests/unit/test_logout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-20 02:15:02.000000 exabyte-api-client-2023.6.20.post0/tests/unit/test_materials.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-20 02:15:02.000000 exabyte-api-client-2023.6.20.post0/tests/unit/test_refined_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-20 02:15:02.000000 exabyte-api-client-2023.6.20.post0/tests/unit/test_workflows.py
```

### Comparing `exabyte-api-client-2023.6.16.post0/.github/workflows/cicd.yml` & `exabyte-api-client-2023.6.20.post0/.github/workflows/cicd.yml`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,38 @@
 
 concurrency:
   group: ${{ github.workflow }}-${{ github.event.pull_request.number || github.ref }}
   cancel-in-progress: true
 
 jobs:
 
+  run-linter:
+    runs-on: ubuntu-20.04
+    strategy:
+      matrix:
+        python-version: [3.8.6]
+
+    steps:
+      - name: Checkout this repository
+        uses: actions/checkout@v3
+        with:
+          lfs: true
+
+      - name: Checkout actions repository
+        uses: actions/checkout@v3
+        with:
+          repository: Exabyte-io/actions
+          token: ${{ secrets.BOT_GITHUB_TOKEN }}
+          path: actions
+
+      - name: Run ruff linter
+        uses: ./actions/py/lint
+        with:
+          python-version: ${{ matrix.python-version }}
+
   run-tests:
     runs-on: ubuntu-20.04
     strategy:
       matrix:
         python-version: [3.6, 3.7, 3.8]
 
     steps:
@@ -43,15 +67,15 @@
           TEST_PORT: 443
           TEST_ACCOUNT_ID: ${{ secrets.DEMO_ACCOUNT_ID }}
           TEST_AUTH_TOKEN: ${{ secrets.DEMO_AUTH_TOKEN }}
           TEST_SECURE: true
 
 
   publish:
-    needs: run-tests
+    needs: [run-linter, run-tests]
     runs-on: ubuntu-latest
     if: github.ref_name == 'dev'
 
     steps:
       - name: Checkout this repository
         uses: actions/checkout@v2
         with:
```

### Comparing `exabyte-api-client-2023.6.16.post0/.gitignore` & `exabyte-api-client-2023.6.20.post0/.gitignore`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2023.6.16.post0/LICENSE.md` & `exabyte-api-client-2023.6.20.post0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2023.6.16.post0/PKG-INFO` & `exabyte-api-client-2023.6.20.post0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exabyte-api-client
-Version: 2023.6.16.post0
+Version: 2023.6.20.post0
 Summary: Exabyte Python Client for RESTful API
 Home-page: https://github.com/Exabyte-io/api-client
 Author: Exabyte Inc.
 Author-email: info@mat3ra.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `exabyte-api-client-2023.6.16.post0/README.md` & `exabyte-api-client-2023.6.20.post0/README.md`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2023.6.16.post0/exabyte_api_client/__init__.py` & `exabyte-api-client-2023.6.20.post0/exabyte_api_client/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# ruff: noqa: F401
 try:
     from ._version import version as __version__
 except ModuleNotFoundError:
     __version__ = None
 
 from exabyte_api_client.endpoints.bank_materials import BankMaterialEndpoints
 from exabyte_api_client.endpoints.bank_workflows import BankWorkflowEndpoints
```

### Comparing `exabyte-api-client-2023.6.16.post0/exabyte_api_client/endpoints/__init__.py` & `exabyte-api-client-2023.6.20.post0/exabyte_api_client/endpoints/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import json
+import json  # noqa: F401
 
 from ..utils.http import Connection
 
 
 class BaseEndpoint(object):
     """
     Base class for Exabyte RESTful API endpoints.
@@ -13,15 +13,15 @@
         version (str): Exabyte API version. Defaults to 2018-10-1.
         secure (bool): whether to use secure http protocol (https vs http). Defaults to True.
 
     Attributes:
         conn (httplib.ExabyteConnection): ExabyteConnection instance.
     """
 
-    def __init__(self, host, port, version='2018-10-1', secure=True, **kwargs):
+    def __init__(self, host, port, version="2018-10-1", secure=True, **kwargs):
         self.conn = Connection(host, port, version=version, secure=secure, **kwargs)
 
     def request(self, method, endpoint_path, params=None, data=None, headers=None):
         """
         Sends an HTTP request with given params, headers and data to the given endpoint.
 
         Args:
@@ -33,13 +33,13 @@
 
         Returns:
             json: response
         """
         with self.conn:
             self.conn.request(method, endpoint_path, params, data, headers)
             response = self.conn.json()
-            if response['status'] != 'success':
-                raise BaseException(response['data']['message'])
-            return response['data']
+            if response["status"] != "success":
+                raise BaseException(response["data"]["message"])
+            return response["data"]
 
     def get_headers(self, account_id, auth_token, content_type="application/json"):
-        return {'X-Account-Id': account_id, 'X-Auth-Token': auth_token, 'Content-Type': content_type}
+        return {"X-Account-Id": account_id, "X-Auth-Token": auth_token, "Content-Type": content_type}
```

### Comparing `exabyte-api-client-2023.6.16.post0/exabyte_api_client/endpoints/bank_entity.py` & `exabyte-api-client-2023.6.20.post0/exabyte_api_client/endpoints/bank_entity.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,8 +40,8 @@
             id_ (str): bank entity ID.
             account_id (str): ID of account to copy the bank entity into.
 
         Returns:
              dict: new entity.
         """
         params = {"accountId": account_id}
-        return self.request('POST', '/'.join((self.name, id_, "copy")), params=params, headers=self.headers)
+        return self.request("POST", "/".join((self.name, id_, "copy")), params=params, headers=self.headers)
```

### Comparing `exabyte-api-client-2023.6.16.post0/exabyte_api_client/endpoints/bank_materials.py` & `exabyte-api-client-2023.6.20.post0/exabyte_api_client/endpoints/bank_materials.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,8 +18,8 @@
 
     Attributes:
         name (str): endpoint name.
     """
 
     def __init__(self, host, port, account_id, auth_token, version=DEFAULT_API_VERSION, secure=SECURE, **kwargs):
         super(BankMaterialEndpoints, self).__init__(host, port, account_id, auth_token, version, secure, **kwargs)
-        self.name = 'bank-materials'
+        self.name = "bank-materials"
```

### Comparing `exabyte-api-client-2023.6.16.post0/exabyte_api_client/endpoints/bank_workflows.py` & `exabyte-api-client-2023.6.20.post0/exabyte_api_client/endpoints/bank_workflows.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,8 +18,8 @@
 
     Attributes:
         name (str): endpoint name.
     """
 
     def __init__(self, host, port, account_id, auth_token, version=DEFAULT_API_VERSION, secure=SECURE, **kwargs):
         super(BankWorkflowEndpoints, self).__init__(host, port, account_id, auth_token, version, secure, **kwargs)
-        self.name = 'bank-workflows'
+        self.name = "bank-workflows"
```

### Comparing `exabyte-api-client-2023.6.16.post0/exabyte_api_client/endpoints/charges.py` & `exabyte-api-client-2023.6.20.post0/exabyte_api_client/endpoints/charges.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         user_id (str): user ID.
         auth_token (str): authentication token.
         headers (dict): default HTTP headers.
     """
 
     def __init__(self, host, port, account_id, auth_token, version=DEFAULT_API_VERSION, secure=SECURE, **kwargs):
         super(ChargeEndpoints, self).__init__(host, port, account_id, auth_token, version, secure, **kwargs)
-        self.name = 'charges'
+        self.name = "charges"
 
     def delete(self, id_):
         raise NotImplementedError
 
     def update(self, id_, modifier):
         raise NotImplementedError
```

### Comparing `exabyte-api-client-2023.6.16.post0/exabyte_api_client/endpoints/entity.py` & `exabyte-api-client-2023.6.20.post0/exabyte_api_client/endpoints/entity.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,66 +36,66 @@
             query (dict): Mongo query. Defaults to {}.
             projection (dict): Mongo projection. Defaults to {}.
 
         Returns:
             list[dict]
         """
         params = {"query": json.dumps(query or {}), "projection": json.dumps(projection or {})}
-        return self.request('GET', self.name, params=params, headers=self.headers)
+        return self.request("GET", self.name, params=params, headers=self.headers)
 
     def get(self, id_):
         """
         Returns a entity with given ID.
 
         Args:
             id_ (str): entity ID.
 
         Returns:
              dict: entity.
         """
-        return self.request('GET', '/'.join((self.name, id_)), headers=self.headers)
+        return self.request("GET", "/".join((self.name, id_)), headers=self.headers)
 
     def delete(self, id_):
         """
         Deletes a given entity.
 
         Args:
             id_ (str): entity ID.
         """
-        return self.request('DELETE', '/'.join((self.name, id_)), headers=self.headers)
+        return self.request("DELETE", "/".join((self.name, id_)), headers=self.headers)
 
     def update(self, id_, modifier):
         """
         Updates a entity with given ID.
 
         Args:
             id_ (str): entity ID.
             modifier (dict): a dictionary of key-values to update entity with.
 
         Returns:
              dict: updated entity.
         """
-        return self.request('PATCH', '/'.join((self.name, id_)), data=json.dumps(modifier), headers=self.headers)
+        return self.request("PATCH", "/".join((self.name, id_)), data=json.dumps(modifier), headers=self.headers)
 
     def create(self, config):
         """
         Creates a new entity.
 
         Args:
             config (dict): entity config.
 
         Returns:
              dict: new entity.
         """
-        return self.request('PUT', '/'.join((self.name, "create")), data=json.dumps(config), headers=self.headers)
+        return self.request("PUT", "/".join((self.name, "create")), data=json.dumps(config), headers=self.headers)
 
     def copy(self, id_):
         """
         Copies a entity with given ID.
 
         Args:
             id_ (str): entity ID.
 
         Returns:
              dict: new entity.
         """
-        return self.request('POST', '/'.join((self.name, id_, "copy")), headers=self.headers)
+        return self.request("POST", "/".join((self.name, id_, "copy")), headers=self.headers)
```

### Comparing `exabyte-api-client-2023.6.16.post0/exabyte_api_client/endpoints/jobs.py` & `exabyte-api-client-2023.6.20.post0/exabyte_api_client/endpoints/jobs.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,42 +21,42 @@
 
     Attributes:
         name (str): endpoint name.
     """
 
     def __init__(self, host, port, account_id, auth_token, version=DEFAULT_API_VERSION, secure=SECURE, **kwargs):
         super(JobEndpoints, self).__init__(host, port, account_id, auth_token, version, secure, **kwargs)
-        self.name = 'jobs'
+        self.name = "jobs"
 
     def submit(self, id_):
         """
         Submits a given job.
 
         Args:
             id_ (str): job ID.
         """
-        self.request('POST', '/'.join((self.name, id_, "submit")), headers=self.headers)
+        self.request("POST", "/".join((self.name, id_, "submit")), headers=self.headers)
 
     def purge(self, id_):
         """
         Purges a given job.
 
         Args:
             id_ (str): job ID.
         """
-        self.request('POST', '/'.join((self.name, id_, "submit")), headers=self.headers)
+        self.request("POST", "/".join((self.name, id_, "submit")), headers=self.headers)
 
     def terminate(self, id_):
         """
         Terminates a given job.
 
         Args:
             id_ (str): job ID.
         """
-        self.request('POST', '/'.join((self.name, id_, "submit")), headers=self.headers)
+        self.request("POST", "/".join((self.name, id_, "submit")), headers=self.headers)
 
     def get_config(self, material_ids, workflow_id, project_id, owner_id, name, compute=None, is_multi_material=False):
         """
         Returns a job config based on the given parameters.
 
         Args:
             material_ids (list): list of material IDs.
@@ -67,24 +67,18 @@
             compute (dict): job compute configuration. Default config is used if not passed.
             is_multi_material (bool): whether the job is multi-material. Defaults to False.
 
         Returns:
             dict
         """
         config = {
-            "_project": {
-                "_id": project_id
-            },
-            "workflow": {
-                "_id": workflow_id
-            },
-            "owner": {
-                "_id": owner_id
-            },
-            "name": name
+            "_project": {"_id": project_id},
+            "workflow": {"_id": workflow_id},
+            "owner": {"_id": owner_id},
+            "name": name,
         }
 
         if compute:
             config.update({"compute": compute})
         if is_multi_material:
             config.update({"_materials": [{"_id": id} for id in material_ids]})
         else:
@@ -108,18 +102,16 @@
         """
         return {
             "ppn": ppn,
             "nodes": nodes,
             "queue": queue,
             "timeLimit": time_limit,
             "notify": notify,
-            "cluster": {
-                "fqdn": cluster
-            },
-            "arguments": {}
+            "cluster": {"fqdn": cluster},
+            "arguments": {},
         }
 
     def create_by_ids(self, materials, workflow_id, project_id, owner_id, prefix, compute=None):
         """
         Creates jobs from the given materials
 
         Args:
@@ -148,29 +140,29 @@
             id_ (str): job ID.
             files (list): list of paths relative to the job working directory.
 
         Returns:
             list: [{"file": "", "URL": ""}]
         """
         data = json.dumps({"files": files})
-        response = self.request('POST', '/'.join((self.name, id_, "presigned-urls")), data=data, headers=self.headers)
+        response = self.request("POST", "/".join((self.name, id_, "presigned-urls")), data=data, headers=self.headers)
         return response["presignedURLs"]
 
     def list_files(self, id_):
         """
         Returns a list of job files.
 
         Args:
             id_ (str): job ID.
 
         Returns:
             list: [{ "key" : str, "size" : int, "bucket" : str, "region" : str,
                      "provider" : str, "lastModified" : int, "name" : str, "signedURL" : str }]
         """
-        response = self.request('GET', '/'.join(('jobs', id_, 'files')), headers=self.headers)
+        response = self.request("GET", "/".join(("jobs", id_, "files")), headers=self.headers)
         return response
 
     def insert_output_files(self, id_, data):
         """
         Inserts job output files.
         Implements https://docs.mat3ra.com/api/#!/Job/post_jobs_id_output_files
```

### Comparing `exabyte-api-client-2023.6.16.post0/exabyte_api_client/endpoints/login.py` & `exabyte-api-client-2023.6.20.post0/exabyte_api_client/endpoints/login.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,27 +20,27 @@
         name (str): endpoint name.
         username (str): username.
         password (str): password.
     """
 
     def __init__(self, host, port, username, password, version=DEFAULT_API_VERSION, secure=SECURE, **kwargs):
         super(LoginEndpoint, self).__init__(host, port, version, secure, **kwargs)
-        self.name = 'login'
+        self.name = "login"
         self.username = username
         self.password = password
 
     def login(self):
         """
         Logs in as a given user and generates an API token.
 
         Returns:
              dict
         """
-        data = {'username': self.username, 'password': self.password}
-        return self.request('POST', self.name, data=data)
+        data = {"username": self.username, "password": self.password}
+        return self.request("POST", self.name, data=data)
 
     @staticmethod
     def get_endpoint_options(host, port, username, password, version=DEFAULT_API_VERSION, secure=SECURE):
         """
         Logs in with given parameters and returns options to use for further calls to the RESTful API.
 
         Args:
```

### Comparing `exabyte-api-client-2023.6.16.post0/exabyte_api_client/endpoints/logout.py` & `exabyte-api-client-2023.6.20.post0/exabyte_api_client/endpoints/logout.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     Attributes:
         name (str): endpoint name.
         headers (dict): default HTTP headers.
     """
 
     def __init__(self, host, port, account_id, auth_token, version=DEFAULT_API_VERSION, secure=SECURE, **kwargs):
         super(LogoutEndpoint, self).__init__(host, port, version, secure, **kwargs)
-        self.name = 'logout'
+        self.name = "logout"
         self.headers = self.get_headers(account_id, auth_token)
 
     def logout(self):
         """
         Deletes current API token.
         """
-        return self.request('POST', self.name, headers=self.headers)
+        return self.request("POST", self.name, headers=self.headers)
```

### Comparing `exabyte-api-client-2023.6.16.post0/exabyte_api_client/endpoints/materials.py` & `exabyte-api-client-2023.6.20.post0/exabyte_api_client/endpoints/materials.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
     Attributes:
         name (str): endpoint name.
     """
 
     def __init__(self, host, port, account_id, auth_token, version=DEFAULT_API_VERSION, secure=SECURE, **kwargs):
         super(MaterialEndpoints, self).__init__(host, port, account_id, auth_token, version, secure, **kwargs)
-        self.name = 'materials'
+        self.name = "materials"
 
     def import_from_file(self, name, content, owner_id=None, format="poscar", tags=()):
         """
         Imports a material from the given file.
 
         Args:
             name (str): material name.
@@ -40,15 +40,15 @@
             owner_id (str): owner ID. Material is created under user's default account by default.
             tags (tuple[str]) a list of tags that should be assigned to the material.
 
         Returns:
             dict
         """
         data = {"name": name, "content": content, "format": format, "ownerId": owner_id, "tags": tags}
-        return self.request('POST', "/".join((self.name, "import")), headers=self.headers, data=json.dumps(data))
+        return self.request("POST", "/".join((self.name, "import")), headers=self.headers, data=json.dumps(data))
 
     def import_from_materialsproject(self, api_key, material_ids, owner_id=None, tags=[]):
         """
         Imports a given material from materialsproject
 
         Args:
             api_key (str): materialsproject API key.
```

### Comparing `exabyte-api-client-2023.6.16.post0/exabyte_api_client/endpoints/mixins/set.py` & `exabyte-api-client-2023.6.20.post0/exabyte_api_client/endpoints/mixins/set.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 
         Args:
             config (dict): entity set config.
 
         Returns:
              dict: new entity set.
         """
-        path_ = '/'.join((self.name, "create-set"))
-        return self.request('PUT', path_, data=json.dumps(config), headers=self.headers)
+        path_ = "/".join((self.name, "create-set"))
+        return self.request("PUT", path_, data=json.dumps(config), headers=self.headers)
 
     def move_to_set(self, _id, old_set_id, new_set_id):
         """
         Moves a entity with given ID to a new set.
 
         Args:
             _id (str): entity ID.
             old_set_id (str): old entity set ID.
             new_set_id (str): new entity set ID.
         """
         params = {"oldSetId": old_set_id, "newSetId": new_set_id}
-        self.request('POST', '/'.join((self.name, _id, "move-to-set")), params=params, headers=self.headers)
+        self.request("POST", "/".join((self.name, _id, "move-to-set")), params=params, headers=self.headers)
```

### Comparing `exabyte-api-client-2023.6.16.post0/exabyte_api_client/endpoints/projects.py` & `exabyte-api-client-2023.6.20.post0/exabyte_api_client/endpoints/projects.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         user_id (str): user ID.
         auth_token (str): authentication token.
         headers (dict): default HTTP headers.
     """
 
     def __init__(self, host, port, account_id, auth_token, version=DEFAULT_API_VERSION, secure=SECURE, **kwargs):
         super(ProjectEndpoints, self).__init__(host, port, account_id, auth_token, version, secure, **kwargs)
-        self.name = 'projects'
+        self.name = "projects"
 
     def delete(self, id_):
         raise NotImplementedError
 
     def update(self, id_, modifier):
         raise NotImplementedError
```

### Comparing `exabyte-api-client-2023.6.16.post0/exabyte_api_client/endpoints/raw_properties.py` & `exabyte-api-client-2023.6.20.post0/exabyte_api_client/endpoints/raw_properties.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,14 @@
         user_id (str): user ID.
         auth_token (str): authentication token.
         headers (dict): default HTTP headers.
     """
 
     def __init__(self, host, port, account_id, auth_token, version=DEFAULT_API_VERSION, secure=SECURE, **kwargs):
         super(RawPropertiesEndpoints, self).__init__(host, port, account_id, auth_token, version, secure, **kwargs)
-        self.name = 'raw-properties'
+        self.name = "raw-properties"
 
     def delete(self, id_):
         raise NotImplementedError
 
     def update(self, id_, modifier):
         raise NotImplementedError
```

### Comparing `exabyte-api-client-2023.6.16.post0/exabyte_api_client/endpoints/refined_properties.py` & `exabyte-api-client-2023.6.20.post0/exabyte_api_client/endpoints/refined_properties.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         user_id (str): user ID.
         auth_token (str): authentication token.
         headers (dict): default HTTP headers.
     """
 
     def __init__(self, host, port, account_id, auth_token, version=DEFAULT_API_VERSION, secure=SECURE, **kwargs):
         super(RefinedPropertiesEndpoints, self).__init__(host, port, account_id, auth_token, version, secure, **kwargs)
-        self.name = 'refined-properties'
+        self.name = "refined-properties"
 
     def delete(self, id_):
         raise NotImplementedError
 
     def update(self, id_, modifier):
         raise NotImplementedError
```

### Comparing `exabyte-api-client-2023.6.16.post0/exabyte_api_client/endpoints/workflows.py` & `exabyte-api-client-2023.6.20.post0/exabyte_api_client/endpoints/workflows.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,8 +22,8 @@
         user_id (str): user ID.
         auth_token (str): authentication token.
         headers (dict): default HTTP headers.
     """
 
     def __init__(self, host, port, account_id, auth_token, version=DEFAULT_API_VERSION, secure=SECURE, **kwargs):
         super(WorkflowEndpoints, self).__init__(host, port, account_id, auth_token, version, secure, **kwargs)
-        self.name = 'workflows'
+        self.name = "workflows"
```

### Comparing `exabyte-api-client-2023.6.16.post0/exabyte_api_client/utils/http.py` & `exabyte-api-client-2023.6.20.post0/exabyte_api_client/utils/http.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         session (requests.sessions.Session): session instance.
         response (requests.models.Response): response instance.
     """
 
     def __init__(self, **kwargs):
         self.response = None
         self.session = requests.Session()
-        self.session.timeout = kwargs.get('timeout', 60)
+        self.session.timeout = kwargs.get("timeout", 60)
 
     def request(self, method, url, params=None, data=None, headers=None):
         """
         Sends an HTTP request with given params, headers and data to the given url.
 
         Args:
             method (str): HTTP method to use.
@@ -125,15 +125,15 @@
             timeout (int): session timeout in seconds.
 
     Attributes:
         preamble (str): common part of URL endpoints, e.g. https://platform.mat3ra.com:4000/api/v1/.
     """
 
     def __init__(self, host, port, version, secure, **kwargs):
-        self.preamble = '{}://{}:{}/api/{}/'.format('https' if secure else 'http', host, port, version)
+        self.preamble = "{}://{}:{}/api/{}/".format("https" if secure else "http", host, port, version)
         super(Connection, self).__init__(**kwargs)
 
     def request(self, method, endpoint_path, params=None, data=None, headers=None):
         """
         Sends an HTTP request with given params, headers and data to the given endpoint.
 
         Args:
```

### Comparing `exabyte-api-client-2023.6.16.post0/exabyte_api_client/utils/materials.py` & `exabyte-api-client-2023.6.20.post0/exabyte_api_client/utils/materials.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,9 +34,9 @@
         ", ".join(material["tags"]),
         len(material["basis"]["coordinates"]),
         lattice["a"],
         lattice["b"],
         lattice["c"],
         lattice["alpha"],
         lattice["beta"],
-        lattice["gamma"]
+        lattice["gamma"],
     ]
```

### Comparing `exabyte-api-client-2023.6.16.post0/exabyte_api_client.egg-info/PKG-INFO` & `exabyte-api-client-2023.6.20.post0/exabyte_api_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exabyte-api-client
-Version: 2023.6.16.post0
+Version: 2023.6.20.post0
 Summary: Exabyte Python Client for RESTful API
 Home-page: https://github.com/Exabyte-io/api-client
 Author: Exabyte Inc.
 Author-email: info@mat3ra.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `exabyte-api-client-2023.6.16.post0/exabyte_api_client.egg-info/SOURCES.txt` & `exabyte-api-client-2023.6.20.post0/exabyte_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2023.6.16.post0/run-tests.sh` & `exabyte-api-client-2023.6.20.post0/run-tests.sh`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2023.6.16.post0/setup.cfg` & `exabyte-api-client-2023.6.20.post0/setup.cfg`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2023.6.16.post0/tests/__init__.py` & `exabyte-api-client-2023.6.20.post0/tests/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Base class for testing endpoints.
     """
 
     def __init__(self, *args, **kwargs):
         super(EndpointBaseTest, self).__init__(*args, **kwargs)
 
     def get_file_path(self, filename):
-        return os.path.join(os.path.dirname(__file__), 'data', filename)
+        return os.path.join(os.path.dirname(__file__), "data", filename)
 
     def get_content(self, filename):
         with open(self.get_file_path(filename)) as f:
             return f.read()
 
     def get_content_in_json(self, filename):
         with open(self.get_file_path(filename)) as f:
```

### Comparing `exabyte-api-client-2023.6.16.post0/tests/data/material.json` & `exabyte-api-client-2023.6.20.post0/tests/data/material.json`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2023.6.16.post0/tests/integration/__init__.py` & `exabyte-api-client-2023.6.20.post0/tests/integration/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,14 +7,14 @@
     """
     Base class for endpoints integration tests.
     """
 
     def __init__(self, *args, **kwargs):
         super(BaseIntegrationTest, self).__init__(*args, **kwargs)
         self.endpoint_kwargs = {
-            'host': os.environ['TEST_HOST'],
-            'port': os.environ['TEST_PORT'],
-            'account_id': os.environ['TEST_ACCOUNT_ID'],
-            'auth_token': os.environ['TEST_AUTH_TOKEN'],
-            'secure': os.environ.get('TEST_SECURE', 'False').lower() == 'true',
-            'version': os.environ.get('TEST_VERSION', '2018-10-01')
+            "host": os.environ["TEST_HOST"],
+            "port": os.environ["TEST_PORT"],
+            "account_id": os.environ["TEST_ACCOUNT_ID"],
+            "auth_token": os.environ["TEST_AUTH_TOKEN"],
+            "secure": os.environ.get("TEST_SECURE", "False").lower() == "true",
+            "version": os.environ.get("TEST_VERSION", "2018-10-01"),
         }
```

### Comparing `exabyte-api-client-2023.6.16.post0/tests/integration/entity.py` & `exabyte-api-client-2023.6.20.post0/tests/integration/entity.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         Returns a selector to access entities created in tests.
         Override upon inheritance as necessary.
         """
         return {"tags": "INTEGRATION-TEST"}
 
     def tearDown(self):
         for entity in [e for e in self.endpoints.list(query=self.entities_selector())]:
-            self.endpoints.delete(entity['_id'])
+            self.endpoints.delete(entity["_id"])
 
     def get_default_config(self):
         """
         Returns the default entity config.
         Override upon inheritance.
         """
         raise NotImplementedError
@@ -35,28 +35,28 @@
         entity.update(kwargs or {})
         entity["tags"] = entity.get("tags", [])
         entity["tags"].append("INTEGRATION-TEST")
         return self.endpoints.create(entity)
 
     def list_entities_test(self):
         entity = self.create_entity()
-        self.assertIn(entity['_id'], [e['_id'] for e in self.endpoints.list(query=self.entities_selector())])
+        self.assertIn(entity["_id"], [e["_id"] for e in self.endpoints.list(query=self.entities_selector())])
 
     def get_entity_by_id_test(self):
         entity = self.create_entity()
-        self.assertEqual(self.endpoints.get(entity['_id'])['_id'], entity['_id'])
+        self.assertEqual(self.endpoints.get(entity["_id"])["_id"], entity["_id"])
 
     def create_entity_test(self):
         name = "test-{}".format(time.time())
         job = self.create_entity({"name": name})
-        self.assertEqual(job['name'], name)
-        self.assertIsNotNone(job['_id'])
+        self.assertEqual(job["name"], name)
+        self.assertIsNotNone(job["_id"])
 
     def delete_entity_test(self):
         entity = self.create_entity()
-        self.endpoints.delete(entity['_id'])
-        self.assertNotIn(entity['_id'], [e['_id'] for e in self.endpoints.list(query=self.entities_selector())])
+        self.endpoints.delete(entity["_id"])
+        self.assertNotIn(entity["_id"], [e["_id"] for e in self.endpoints.list(query=self.entities_selector())])
 
     def update_entity_test(self):
         entity = self.create_entity()
-        updated_entity = self.endpoints.update(entity['_id'], {'name': 'UPDATED'})
-        self.assertEqual(updated_entity['name'], 'UPDATED')
+        updated_entity = self.endpoints.update(entity["_id"], {"name": "UPDATED"})
+        self.assertEqual(updated_entity["name"], "UPDATED")
```

### Comparing `exabyte-api-client-2023.6.16.post0/tests/integration/test_jobs.py` & `exabyte-api-client-2023.6.20.post0/tests/integration/test_jobs.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,36 +5,31 @@
 from tests.integration.entity import EntityIntegrationTest
 
 
 class JobEndpointsIntegrationTest(EntityIntegrationTest):
     """
     Job endpoints integration tests.
     """
+
     KNOWN_COMPLETED_JOB_ID = "9gyhfncWDhnSyzALv"
 
     def __init__(self, *args, **kwargs):
         super(JobEndpointsIntegrationTest, self).__init__(*args, **kwargs)
         self.endpoints = JobEndpoints(**self.endpoint_kwargs)
 
     def get_default_config(self):
         """
         Returns the default entity config.
         Override upon inheritance.
         """
-        now_time = datetime.datetime.today().strftime('%Y-%m-%d %H:%M:%S')
+        now_time = datetime.datetime.today().strftime("%Y-%m-%d %H:%M:%S")
         return {"name": "API-CLIENT TEST JOB {}".format(now_time)}
 
-    def get_compute_params(self, nodes=1, notify='n', ppn=1, queue='D', time_limit='00:05:00'):
-        return {
-            "nodes": nodes,
-            "notify": notify,
-            "ppn": ppn,
-            "queue": queue,
-            "timeLimit": time_limit
-        }
+    def get_compute_params(self, nodes=1, notify="n", ppn=1, queue="D", time_limit="00:05:00"):
+        return {"nodes": nodes, "notify": notify, "ppn": ppn, "queue": queue, "timeLimit": time_limit}
 
     def test_list_jobs(self):
         self.list_entities_test()
 
     def test_get_job_by_id(self):
         self.get_entity_by_id_test()
 
@@ -54,29 +49,27 @@
             if job["status"] == "finished":
                 return
             time.sleep(5)
         raise BaseException("job with ID {} did not finish within {} seconds".format(id_, timeout))
 
     def test_submit_job_and_wait_to_finish(self):
         job = self.create_entity()
-        self.endpoints.submit(job['_id'])
-        self.assertEqual('submitted', self.endpoints.get(job['_id'])['status'])
+        self.endpoints.submit(job["_id"])
+        self.assertEqual("submitted", self.endpoints.get(job["_id"])["status"])
         self._wait_for_job_to_finish(job["_id"])
 
     def test_create_job_timeLimit(self):
         time_limit = "00:10:00"
         job = self.create_entity({"compute": self.get_compute_params(time_limit=time_limit)})
-        self.assertEqual(self.endpoints.get(job['_id'])['_id'], job['_id'])
-        self.assertEqual(self.endpoints.get(job['_id'])['compute']['timeLimit'], time_limit)
+        self.assertEqual(self.endpoints.get(job["_id"])["_id"], job["_id"])
+        self.assertEqual(self.endpoints.get(job["_id"])["compute"]["timeLimit"], time_limit)
 
     def test_create_job_notify(self):
-        job = self.create_entity({"compute": self.get_compute_params(notify='abe')})
-        self.assertEqual(self.endpoints.get(job['_id'])['_id'], job['_id'])
-        self.assertEqual(self.endpoints.get(job['_id'])['compute']['notify'], 'abe')
+        job = self.create_entity({"compute": self.get_compute_params(notify="abe")})
+        self.assertEqual(self.endpoints.get(job["_id"])["_id"], job["_id"])
+        self.assertEqual(self.endpoints.get(job["_id"])["compute"]["notify"], "abe")
 
     def test_list_files(self):
-        http_response_data = self.endpoints.list_files(
-            self.KNOWN_COMPLETED_JOB_ID
-        )
+        http_response_data = self.endpoints.list_files(self.KNOWN_COMPLETED_JOB_ID)
         self.assertIsInstance(http_response_data, list)
         self.assertGreater(len(http_response_data), 0)
         self.assertIsInstance(http_response_data[0], dict)
```

### Comparing `exabyte-api-client-2023.6.16.post0/tests/integration/test_materials.py` & `exabyte-api-client-2023.6.20.post0/tests/integration/test_materials.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     """
 
     def __init__(self, *args, **kwargs):
         super(MaterialEndpointsIntegrationTest, self).__init__(*args, **kwargs)
         self.endpoints = MaterialEndpoints(**self.endpoint_kwargs)
 
     def get_default_config(self):
-        return self.get_content_in_json('material.json')
+        return self.get_content_in_json("material.json")
 
     def test_list_materials(self):
         self.list_entities_test()
 
     def test_get_material_by_id(self):
         self.get_entity_by_id_test()
 
@@ -27,9 +27,9 @@
         self.delete_entity_test()
 
     def test_update_material(self):
         self.update_entity_test()
 
     def test_get_material_by_formula(self):
         material = self.create_entity()
-        materials = self.endpoints.list(query={"_id": material["_id"], "formula": 'Si'})
-        self.assertIn(material['_id'], [m['_id'] for m in materials])
+        materials = self.endpoints.list(query={"_id": material["_id"], "formula": "Si"})
+        self.assertIn(material["_id"], [m["_id"] for m in materials])
```

### Comparing `exabyte-api-client-2023.6.16.post0/tests/unit/__init__.py` & `exabyte-api-client-2023.6.20.post0/tests/unit/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,17 +8,17 @@
     Base class for endpoints unit tests.
     """
 
     def __init__(self, *args, **kwargs):
         super(EndpointBaseUnitTest, self).__init__(*args, **kwargs)
         self.port = 4000
         self.version = "2018-10-01"
-        self.host = 'platform.mat3ra.com'
-        self.account_id = 'ubxMkAyx37Rjn8qK9'
-        self.auth_token = 'XihOnUA8EqytSui1icz6fYhsJ2tUsJGGTlV03upYPSF'
+        self.host = "platform.mat3ra.com"
+        self.account_id = "ubxMkAyx37Rjn8qK9"
+        self.auth_token = "XihOnUA8EqytSui1icz6fYhsJ2tUsJGGTlV03upYPSF"
 
-    def mock_response(self, content, status_code=200, reason='OK'):
+    def mock_response(self, content, status_code=200, reason="OK"):
         response = Response()
         response._content = content.encode()
         response.status_code = status_code
         response.reason = reason
         return response
```

### Comparing `exabyte-api-client-2023.6.16.post0/tests/unit/entity.py` & `exabyte-api-client-2023.6.20.post0/tests/unit/entity.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,29 +9,29 @@
     def __init__(self, *args, **kwargs):
         super(EntityEndpointsUnitTest, self).__init__(*args, **kwargs)
         self.endpoints = None
         self.endpoint_name = None
 
     @property
     def base_url(self):
-        return 'https://{}:{}/api/{}/{}'.format(self.host, self.port, self.version, self.endpoint_name)
+        return "https://{}:{}/api/{}/{}".format(self.host, self.port, self.version, self.endpoint_name)
 
     def list(self, mock_request):
         mock_request.return_value = self.mock_response('{"status": "success", "data": []}')
         self.assertEqual(self.endpoints.list(), [])
-        self.assertEqual(mock_request.call_args[1]['method'], 'get')
+        self.assertEqual(mock_request.call_args[1]["method"], "get")
 
     def get(self, mock_request):
         mock_request.return_value = self.mock_response('{"status": "success", "data": {}}')
-        self.assertEqual(self.endpoints.get('28FMvD5knJZZx452H'), {})
-        expected_url = '{}/28FMvD5knJZZx452H'.format(self.base_url, self.port)
-        self.assertEqual(mock_request.call_args[1]['url'], expected_url)
+        self.assertEqual(self.endpoints.get("28FMvD5knJZZx452H"), {})
+        expected_url = "{}/28FMvD5knJZZx452H".format(self.base_url)
+        self.assertEqual(mock_request.call_args[1]["url"], expected_url)
 
     def create(self, mock_request):
         mock_request.return_value = self.mock_response('{"status": "success", "data": {}}')
         self.endpoints.create({})
-        self.assertEqual(mock_request.call_args[1]['headers']['Content-Type'], 'application/json')
+        self.assertEqual(mock_request.call_args[1]["headers"]["Content-Type"], "application/json")
 
     def delete(self, mock_request):
         mock_request.return_value = self.mock_response('{"status": "success", "data": {}}')
-        self.assertEqual(self.endpoints.delete('28FMvD5knJZZx452H'), {})
-        self.assertEqual(mock_request.call_args[1]['method'], 'delete')
+        self.assertEqual(self.endpoints.delete("28FMvD5knJZZx452H"), {})
+        self.assertEqual(mock_request.call_args[1]["method"], "delete")
```

### Comparing `exabyte-api-client-2023.6.16.post0/tests/unit/test_bank_materials.py` & `exabyte-api-client-2023.6.20.post0/tests/unit/test_bank_materials.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,14 @@
     """
 
     def __init__(self, *args, **kwargs):
         super(EndpointMaterialsBankUnitTest, self).__init__(*args, **kwargs)
         self.endpoint_name = "bank-materials"
         self.endpoints = BankMaterialEndpoints(self.host, self.port, self.account_id, self.auth_token)
 
-    @mock.patch('requests.sessions.Session.request')
+    @mock.patch("requests.sessions.Session.request")
     def test_list(self, mock_request):
         self.list(mock_request)
 
-    @mock.patch('requests.sessions.Session.request')
+    @mock.patch("requests.sessions.Session.request")
     def test_get(self, mock_request):
         self.get(mock_request)
```

### Comparing `exabyte-api-client-2023.6.16.post0/tests/unit/test_bank_workflows.py` & `exabyte-api-client-2023.6.20.post0/tests/unit/test_bank_workflows.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,14 @@
     """
 
     def __init__(self, *args, **kwargs):
         super(EndpointWorkflowsBankUnitTest, self).__init__(*args, **kwargs)
         self.endpoint_name = "bank-workflows"
         self.endpoints = BankWorkflowEndpoints(self.host, self.port, self.account_id, self.auth_token)
 
-    @mock.patch('requests.sessions.Session.request')
+    @mock.patch("requests.sessions.Session.request")
     def test_list(self, mock_request):
         self.list(mock_request)
 
-    @mock.patch('requests.sessions.Session.request')
+    @mock.patch("requests.sessions.Session.request")
     def test_get(self, mock_request):
         self.get(mock_request)
```

### Comparing `exabyte-api-client-2023.6.16.post0/tests/unit/test_httpBase.py` & `exabyte-api-client-2023.6.20.post0/tests/unit/test_httpBase.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,24 +9,24 @@
     Class for testing functionality implemented inside HTTPBase module.
     """
 
     def __init__(self, *args, **kwargs):
         super(HTTPBaseUnitTest, self).__init__(*args, **kwargs)
 
     def test_preamble_secure(self):
-        conn = Connection(self.host, self.port, version='2018-10-1', secure=True)
-        self.assertEqual(conn.preamble, 'https://{}:{}/api/2018-10-1/'.format(self.host, self.port))
+        conn = Connection(self.host, self.port, version="2018-10-1", secure=True)
+        self.assertEqual(conn.preamble, "https://{}:{}/api/2018-10-1/".format(self.host, self.port))
 
     def test_preamble_unsecure(self):
-        conn = Connection(self.host, self.port, version='2018-10-1', secure=False)
-        self.assertEqual(conn.preamble, 'http://{}:{}/api/2018-10-1/'.format(self.host, self.port))
+        conn = Connection(self.host, self.port, version="2018-10-1", secure=False)
+        self.assertEqual(conn.preamble, "http://{}:{}/api/2018-10-1/".format(self.host, self.port))
 
     def test_preamble_version(self):
-        conn = Connection(self.host, self.port, version='2018-10-2', secure=True)
-        self.assertEqual(conn.preamble, 'https://{}:{}/api/2018-10-2/'.format(self.host, self.port))
+        conn = Connection(self.host, self.port, version="2018-10-2", secure=True)
+        self.assertEqual(conn.preamble, "https://{}:{}/api/2018-10-2/".format(self.host, self.port))
 
-    @mock.patch('requests.sessions.Session.request')
+    @mock.patch("requests.sessions.Session.request")
     def test_raise_http_error(self, mock_request):
-        mock_request.return_value = self.mock_response('', 401, reason='Unauthorized')
+        mock_request.return_value = self.mock_response("", 401, reason="Unauthorized")
         with self.assertRaises(HTTPError):
-            conn = Connection(self.host, self.port, version='2018-10-1', secure=True)
-            conn.request('POST', 'login', data={'username': '', 'password': ''})
+            conn = Connection(self.host, self.port, version="2018-10-1", secure=True)
+            conn.request("POST", "login", data={"username": "", "password": ""})
```

### Comparing `exabyte-api-client-2023.6.16.post0/tests/unit/test_jobs.py` & `exabyte-api-client-2023.6.20.post0/tests/unit/test_jobs.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,22 +10,22 @@
     """
 
     def __init__(self, *args, **kwargs):
         super(EndpointJobsUnitTest, self).__init__(*args, **kwargs)
         self.endpoint_name = "jobs"
         self.endpoints = JobEndpoints(self.host, self.port, self.account_id, self.auth_token)
 
-    @mock.patch('requests.sessions.Session.request')
+    @mock.patch("requests.sessions.Session.request")
     def test_list(self, mock_request):
         self.list(mock_request)
 
-    @mock.patch('requests.sessions.Session.request')
+    @mock.patch("requests.sessions.Session.request")
     def test_get(self, mock_request):
         self.get(mock_request)
 
-    @mock.patch('requests.sessions.Session.request')
+    @mock.patch("requests.sessions.Session.request")
     def test_create(self, mock_request):
         self.create(mock_request)
 
-    @mock.patch('requests.sessions.Session.request')
+    @mock.patch("requests.sessions.Session.request")
     def test_delete(self, mock_request):
         self.create(mock_request)
```

### Comparing `exabyte-api-client-2023.6.16.post0/tests/unit/test_login.py` & `exabyte-api-client-2023.6.20.post0/tests/unit/test_login.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 class EndpointLoginUnitTest(EndpointBaseUnitTest):
     """
     Class for testing login endpoint.
     """
 
     def __init__(self, *args, **kwargs):
         super(EndpointLoginUnitTest, self).__init__(*args, **kwargs)
-        self.username = 'test'
-        self.password = 'test'
+        self.username = "test"
+        self.password = "test"
         self.login_endpoint = LoginEndpoint(self.host, self.port, self.username, self.password)
 
-    @mock.patch('requests.sessions.Session.request')
+    @mock.patch("requests.sessions.Session.request")
     def test_login(self, mock_request):
-        mock_request.return_value = self.mock_response(self.get_content('login.json'))
+        mock_request.return_value = self.mock_response(self.get_content("login.json"))
         expected_result = {
-            'X-Account-Id': 'ubxMkAyx37Rjn8qK9',
-            'X-Auth-Token': 'XihOnUA8EqytSui1icz6fYhsJ2tUsJGGTlV03upYPSF'
+            "X-Account-Id": "ubxMkAyx37Rjn8qK9",
+            "X-Auth-Token": "XihOnUA8EqytSui1icz6fYhsJ2tUsJGGTlV03upYPSF",
         }
         self.assertEqual(self.login_endpoint.login(), expected_result)
-        self.assertEqual(mock_request.call_args[1]['data']['username'], self.username)
-        self.assertEqual(mock_request.call_args[1]['data']['password'], self.password)
+        self.assertEqual(mock_request.call_args[1]["data"]["username"], self.username)
+        self.assertEqual(mock_request.call_args[1]["data"]["password"], self.password)
```

### Comparing `exabyte-api-client-2023.6.16.post0/tests/unit/test_logout.py` & `exabyte-api-client-2023.6.20.post0/tests/unit/test_logout.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,13 +9,13 @@
     Class for testing logout endpoint.
     """
 
     def __init__(self, *args, **kwargs):
         super(EndpointLogoutUnitTest, self).__init__(*args, **kwargs)
         self.logout_endpoint = LogoutEndpoint(self.host, self.port, self.account_id, self.auth_token)
 
-    @mock.patch('requests.sessions.Session.request')
+    @mock.patch("requests.sessions.Session.request")
     def test_logout(self, mock_request):
-        mock_request.return_value = self.mock_response(self.get_content('logout.json'))
+        mock_request.return_value = self.mock_response(self.get_content("logout.json"))
         self.assertEqual(self.logout_endpoint.logout(), {"message": "You are successfully logged out"})
-        self.assertEqual(mock_request.call_args[1]['headers']['X-Account-Id'], self.account_id)
-        self.assertEqual(mock_request.call_args[1]['headers']['X-Auth-Token'], self.auth_token)
+        self.assertEqual(mock_request.call_args[1]["headers"]["X-Account-Id"], self.account_id)
+        self.assertEqual(mock_request.call_args[1]["headers"]["X-Auth-Token"], self.auth_token)
```

### Comparing `exabyte-api-client-2023.6.16.post0/tests/unit/test_materials.py` & `exabyte-api-client-2023.6.20.post0/tests/unit/test_materials.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,22 +10,22 @@
     """
 
     def __init__(self, *args, **kwargs):
         super(EndpointMaterialsUnitTest, self).__init__(*args, **kwargs)
         self.endpoint_name = "materials"
         self.endpoints = MaterialEndpoints(self.host, self.port, self.account_id, self.auth_token)
 
-    @mock.patch('requests.sessions.Session.request')
+    @mock.patch("requests.sessions.Session.request")
     def test_list(self, mock_request):
         self.list(mock_request)
 
-    @mock.patch('requests.sessions.Session.request')
+    @mock.patch("requests.sessions.Session.request")
     def test_get(self, mock_request):
         self.get(mock_request)
 
-    @mock.patch('requests.sessions.Session.request')
+    @mock.patch("requests.sessions.Session.request")
     def test_create(self, mock_request):
         self.create(mock_request)
 
-    @mock.patch('requests.sessions.Session.request')
+    @mock.patch("requests.sessions.Session.request")
     def test_delete(self, mock_request):
         self.create(mock_request)
```

### Comparing `exabyte-api-client-2023.6.16.post0/tests/unit/test_refined_properties.py` & `exabyte-api-client-2023.6.20.post0/tests/unit/test_refined_properties.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,14 @@
     """
 
     def __init__(self, *args, **kwargs):
         super(EndpointCharacteristicUnitTest, self).__init__(*args, **kwargs)
         self.endpoint_name = "refined-properties"
         self.endpoints = RefinedPropertiesEndpoints(self.host, self.port, self.account_id, self.auth_token)
 
-    @mock.patch('requests.sessions.Session.request')
+    @mock.patch("requests.sessions.Session.request")
     def test_list(self, mock_request):
         self.list(mock_request)
 
-    @mock.patch('requests.sessions.Session.request')
+    @mock.patch("requests.sessions.Session.request")
     def test_get(self, mock_request):
         self.get(mock_request)
```

### Comparing `exabyte-api-client-2023.6.16.post0/tests/unit/test_workflows.py` & `exabyte-api-client-2023.6.20.post0/tests/unit/test_workflows.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,22 +10,22 @@
     """
 
     def __init__(self, *args, **kwargs):
         super(EndpointWorkflowsUnitTest, self).__init__(*args, **kwargs)
         self.endpoint_name = "workflows"
         self.endpoints = WorkflowEndpoints(self.host, self.port, self.account_id, self.auth_token)
 
-    @mock.patch('requests.sessions.Session.request')
+    @mock.patch("requests.sessions.Session.request")
     def test_list(self, mock_request):
         self.list(mock_request)
 
-    @mock.patch('requests.sessions.Session.request')
+    @mock.patch("requests.sessions.Session.request")
     def test_get(self, mock_request):
         self.get(mock_request)
 
-    @mock.patch('requests.sessions.Session.request')
+    @mock.patch("requests.sessions.Session.request")
     def test_create(self, mock_request):
         self.create(mock_request)
 
-    @mock.patch('requests.sessions.Session.request')
+    @mock.patch("requests.sessions.Session.request")
     def test_delete(self, mock_request):
         self.delete(mock_request)
```

