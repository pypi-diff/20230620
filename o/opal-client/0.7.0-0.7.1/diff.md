# Comparing `tmp/opal-client-0.7.0.tar.gz` & `tmp/opal-client-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opal-client-0.7.0.tar", last modified: Wed May 10 19:01:52 2023, max compression
+gzip compressed data, was "opal-client-0.7.1.tar", last modified: Tue Jun 20 13:40:52 2023, max compression
```

## Comparing `opal-client-0.7.0.tar` & `opal-client-0.7.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.622918 opal-client-0.7.0/
--rw-r--r--   0 asafc      (501) staff       (20)     8464 2023-05-10 19:01:52.622656 opal-client-0.7.0/PKG-INFO
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.617684 opal-client-0.7.0/opal_client/
--rw-r--r--   0 asafc      (501) staff       (20)       31 2022-10-01 21:13:25.000000 opal-client-0.7.0/opal_client/__init__.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.618972 opal-client-0.7.0/opal_client/callbacks/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-client-0.7.0/opal_client/callbacks/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     3034 2022-10-01 21:13:25.000000 opal-client-0.7.0/opal_client/callbacks/api.py
--rw-r--r--   0 asafc      (501) staff       (20)     4329 2022-12-02 16:23:06.000000 opal-client-0.7.0/opal_client/callbacks/register.py
--rw-r--r--   0 asafc      (501) staff       (20)     2960 2023-05-10 06:45:11.000000 opal-client-0.7.0/opal_client/callbacks/reporter.py
--rw-r--r--   0 asafc      (501) staff       (20)     2213 2023-05-10 17:44:36.000000 opal-client-0.7.0/opal_client/cli.py
--rw-r--r--   0 asafc      (501) staff       (20)    19776 2023-05-10 17:44:40.000000 opal-client-0.7.0/opal_client/client.py
--rw-r--r--   0 asafc      (501) staff       (20)    10945 2023-05-10 17:44:40.000000 opal-client-0.7.0/opal_client/config.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.619510 opal-client-0.7.0/opal_client/data/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-client-0.7.0/opal_client/data/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)      863 2022-10-01 21:13:25.000000 opal-client-0.7.0/opal_client/data/api.py
--rw-r--r--   0 asafc      (501) staff       (20)     4286 2022-10-12 14:50:19.000000 opal-client-0.7.0/opal_client/data/fetcher.py
--rw-r--r--   0 asafc      (501) staff       (20)      842 2022-10-01 21:13:25.000000 opal-client-0.7.0/opal_client/data/rpc.py
--rw-r--r--   0 asafc      (501) staff       (20)    19105 2023-05-10 06:45:11.000000 opal-client-0.7.0/opal_client/data/updater.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.620090 opal-client-0.7.0/opal_client/engine/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2023-05-10 17:44:40.000000 opal-client-0.7.0/opal_client/engine/__init__.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.620200 opal-client-0.7.0/opal_client/engine/healthcheck/
--rw-r--r--   0 asafc      (501) staff       (20)     1123 2023-05-10 17:44:40.000000 opal-client-0.7.0/opal_client/engine/healthcheck/opal.rego
--rw-r--r--   0 asafc      (501) staff       (20)     3517 2023-05-10 17:44:40.000000 opal-client-0.7.0/opal_client/engine/logger.py
--rw-r--r--   0 asafc      (501) staff       (20)     5702 2023-05-10 17:44:40.000000 opal-client-0.7.0/opal_client/engine/options.py
--rw-r--r--   0 asafc      (501) staff       (20)    10724 2023-05-10 17:44:40.000000 opal-client-0.7.0/opal_client/engine/runner.py
--rw-r--r--   0 asafc      (501) staff       (20)     2220 2022-10-01 21:13:25.000000 opal-client-0.7.0/opal_client/limiter.py
--rw-r--r--   0 asafc      (501) staff       (20)       33 2022-10-01 21:13:25.000000 opal-client-0.7.0/opal_client/logger.py
--rw-r--r--   0 asafc      (501) staff       (20)       96 2022-10-01 21:13:25.000000 opal-client-0.7.0/opal_client/main.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.621151 opal-client-0.7.0/opal_client/policy/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-client-0.7.0/opal_client/policy/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)      501 2022-10-01 21:13:25.000000 opal-client-0.7.0/opal_client/policy/api.py
--rw-r--r--   0 asafc      (501) staff       (20)     4968 2023-02-01 11:46:28.000000 opal-client-0.7.0/opal_client/policy/fetcher.py
--rw-r--r--   0 asafc      (501) staff       (20)     1797 2023-02-01 11:46:28.000000 opal-client-0.7.0/opal_client/policy/options.py
--rw-r--r--   0 asafc      (501) staff       (20)      596 2022-10-01 21:13:25.000000 opal-client-0.7.0/opal_client/policy/topics.py
--rw-r--r--   0 asafc      (501) staff       (20)    13450 2023-05-10 17:44:36.000000 opal-client-0.7.0/opal_client/policy/updater.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.622068 opal-client-0.7.0/opal_client/policy_store/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-client-0.7.0/opal_client/policy_store/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     1650 2023-05-10 06:45:11.000000 opal-client-0.7.0/opal_client/policy_store/api.py
--rw-r--r--   0 asafc      (501) staff       (20)     8442 2023-05-10 17:44:40.000000 opal-client-0.7.0/opal_client/policy_store/base_policy_store_client.py
--rw-r--r--   0 asafc      (501) staff       (20)    12318 2023-05-10 17:44:40.000000 opal-client-0.7.0/opal_client/policy_store/cedar_client.py
--rw-r--r--   0 asafc      (501) staff       (20)     2352 2023-05-10 06:45:11.000000 opal-client-0.7.0/opal_client/policy_store/mock_policy_store_client.py
--rw-r--r--   0 asafc      (501) staff       (20)    32177 2023-05-10 17:44:40.000000 opal-client-0.7.0/opal_client/policy_store/opa_client.py
--rw-r--r--   0 asafc      (501) staff       (20)     5741 2023-05-10 17:44:40.000000 opal-client-0.7.0/opal_client/policy_store/policy_store_client_factory.py
--rw-r--r--   0 asafc      (501) staff       (20)     1815 2023-05-10 17:44:40.000000 opal-client-0.7.0/opal_client/policy_store/schemas.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.622485 opal-client-0.7.0/opal_client/tests/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-client-0.7.0/opal_client/tests/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     7279 2023-05-10 06:45:11.000000 opal-client-0.7.0/opal_client/tests/data_updater_test.py
--rw-r--r--   0 asafc      (501) staff       (20)     1960 2023-05-10 06:45:11.000000 opal-client-0.7.0/opal_client/tests/opa_client_test.py
--rw-r--r--   0 asafc      (501) staff       (20)     4415 2023-05-10 06:45:11.000000 opal-client-0.7.0/opal_client/tests/server_to_client_intergation_test.py
--rw-r--r--   0 asafc      (501) staff       (20)      322 2022-10-01 21:13:25.000000 opal-client-0.7.0/opal_client/utils.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.618529 opal-client-0.7.0/opal_client.egg-info/
--rw-r--r--   0 asafc      (501) staff       (20)     8464 2023-05-10 19:01:52.000000 opal-client-0.7.0/opal_client.egg-info/PKG-INFO
--rw-r--r--   0 asafc      (501) staff       (20)     1501 2023-05-10 19:01:52.000000 opal-client-0.7.0/opal_client.egg-info/SOURCES.txt
--rw-r--r--   0 asafc      (501) staff       (20)        1 2023-05-10 19:01:52.000000 opal-client-0.7.0/opal_client.egg-info/dependency_links.txt
--rw-r--r--   0 asafc      (501) staff       (20)       52 2023-05-10 19:01:52.000000 opal-client-0.7.0/opal_client.egg-info/entry_points.txt
--rw-r--r--   0 asafc      (501) staff       (20)      436 2023-05-10 19:01:52.000000 opal-client-0.7.0/opal_client.egg-info/requires.txt
--rw-r--r--   0 asafc      (501) staff       (20)       12 2023-05-10 19:01:52.000000 opal-client-0.7.0/opal_client.egg-info/top_level.txt
--rw-r--r--   0 asafc      (501) staff       (20)       38 2023-05-10 19:01:52.622958 opal-client-0.7.0/setup.cfg
--rw-r--r--   0 asafc      (501) staff       (20)     2834 2023-05-10 17:44:40.000000 opal-client-0.7.0/setup.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 13:40:52.394622 opal-client-0.7.1/
+-rw-r--r--   0 roekatz    (501) staff       (20)     9040 2023-06-20 13:40:52.394277 opal-client-0.7.1/PKG-INFO
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 13:40:52.376216 opal-client-0.7.1/opal_client/
+-rw-r--r--   0 roekatz    (501) staff       (20)       31 2022-12-08 13:40:17.000000 opal-client-0.7.1/opal_client/__init__.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 13:40:52.379836 opal-client-0.7.1/opal_client/callbacks/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-client-0.7.1/opal_client/callbacks/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     3034 2022-12-08 13:40:17.000000 opal-client-0.7.1/opal_client/callbacks/api.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4329 2023-04-18 15:25:03.000000 opal-client-0.7.1/opal_client/callbacks/register.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2960 2023-05-29 10:10:14.000000 opal-client-0.7.1/opal_client/callbacks/reporter.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2213 2023-05-29 10:10:14.000000 opal-client-0.7.1/opal_client/cli.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    20027 2023-06-03 11:34:06.000000 opal-client-0.7.1/opal_client/client.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    11947 2023-06-03 11:34:06.000000 opal-client-0.7.1/opal_client/config.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 13:40:52.382804 opal-client-0.7.1/opal_client/data/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-client-0.7.1/opal_client/data/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      863 2022-12-08 13:40:17.000000 opal-client-0.7.1/opal_client/data/api.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4286 2023-05-09 07:59:18.000000 opal-client-0.7.1/opal_client/data/fetcher.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      842 2022-12-08 13:40:17.000000 opal-client-0.7.1/opal_client/data/rpc.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    20126 2023-05-29 10:10:14.000000 opal-client-0.7.1/opal_client/data/updater.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 13:40:52.384943 opal-client-0.7.1/opal_client/engine/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2023-05-29 10:10:14.000000 opal-client-0.7.1/opal_client/engine/__init__.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 13:40:52.385633 opal-client-0.7.1/opal_client/engine/healthcheck/
+-rw-r--r--   0 roekatz    (501) staff       (20)     1123 2023-05-29 10:10:14.000000 opal-client-0.7.1/opal_client/engine/healthcheck/opal.rego
+-rw-r--r--   0 roekatz    (501) staff       (20)     3517 2023-05-29 10:10:14.000000 opal-client-0.7.1/opal_client/engine/logger.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     5702 2023-05-29 10:10:14.000000 opal-client-0.7.1/opal_client/engine/options.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    10724 2023-05-29 10:10:14.000000 opal-client-0.7.1/opal_client/engine/runner.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2220 2022-12-08 13:40:17.000000 opal-client-0.7.1/opal_client/limiter.py
+-rw-r--r--   0 roekatz    (501) staff       (20)       33 2022-12-08 13:40:17.000000 opal-client-0.7.1/opal_client/logger.py
+-rw-r--r--   0 roekatz    (501) staff       (20)       96 2022-12-08 13:40:17.000000 opal-client-0.7.1/opal_client/main.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 13:40:52.387080 opal-client-0.7.1/opal_client/policy/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-client-0.7.1/opal_client/policy/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      501 2022-12-08 13:40:17.000000 opal-client-0.7.1/opal_client/policy/api.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4968 2023-05-29 10:10:14.000000 opal-client-0.7.1/opal_client/policy/fetcher.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1797 2023-05-29 10:10:14.000000 opal-client-0.7.1/opal_client/policy/options.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      596 2022-12-08 13:40:17.000000 opal-client-0.7.1/opal_client/policy/topics.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    13450 2023-05-29 10:10:14.000000 opal-client-0.7.1/opal_client/policy/updater.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 13:40:52.390563 opal-client-0.7.1/opal_client/policy_store/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-client-0.7.1/opal_client/policy_store/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1650 2023-05-29 10:10:14.000000 opal-client-0.7.1/opal_client/policy_store/api.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     8442 2023-05-29 10:10:14.000000 opal-client-0.7.1/opal_client/policy_store/base_policy_store_client.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    12318 2023-05-29 10:10:14.000000 opal-client-0.7.1/opal_client/policy_store/cedar_client.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2352 2023-05-29 10:10:14.000000 opal-client-0.7.1/opal_client/policy_store/mock_policy_store_client.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    34604 2023-06-19 14:15:56.000000 opal-client-0.7.1/opal_client/policy_store/opa_client.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     6605 2023-06-03 11:34:06.000000 opal-client-0.7.1/opal_client/policy_store/policy_store_client_factory.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1831 2023-05-29 10:10:14.000000 opal-client-0.7.1/opal_client/policy_store/schemas.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 13:40:52.393654 opal-client-0.7.1/opal_client/tests/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-client-0.7.1/opal_client/tests/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     7279 2023-05-29 10:10:14.000000 opal-client-0.7.1/opal_client/tests/data_updater_test.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     3974 2023-05-29 10:10:14.000000 opal-client-0.7.1/opal_client/tests/opa_client_test.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4415 2023-05-29 10:10:14.000000 opal-client-0.7.1/opal_client/tests/server_to_client_intergation_test.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      322 2022-12-08 13:40:17.000000 opal-client-0.7.1/opal_client/utils.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 13:40:52.378362 opal-client-0.7.1/opal_client.egg-info/
+-rw-r--r--   0 roekatz    (501) staff       (20)     9040 2023-06-20 13:40:52.000000 opal-client-0.7.1/opal_client.egg-info/PKG-INFO
+-rw-r--r--   0 roekatz    (501) staff       (20)     1501 2023-06-20 13:40:52.000000 opal-client-0.7.1/opal_client.egg-info/SOURCES.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)        1 2023-06-20 13:40:52.000000 opal-client-0.7.1/opal_client.egg-info/dependency_links.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)       52 2023-06-20 13:40:52.000000 opal-client-0.7.1/opal_client.egg-info/entry_points.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)      436 2023-06-20 13:40:52.000000 opal-client-0.7.1/opal_client.egg-info/requires.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)       12 2023-06-20 13:40:52.000000 opal-client-0.7.1/opal_client.egg-info/top_level.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)       38 2023-06-20 13:40:52.396659 opal-client-0.7.1/setup.cfg
+-rw-r--r--   0 roekatz    (501) staff       (20)     2834 2023-05-29 10:10:14.000000 opal-client-0.7.1/setup.py
```

### Comparing `opal-client-0.7.0/PKG-INFO` & `opal-client-0.7.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opal-client
-Version: 0.7.0
+Version: 0.7.1
 Summary: OPAL is an administration layer for Open Policy Agent (OPA), detecting changes to both policy and data and pushing live updates to your agents. The opal-client is deployed alongside a policy-store (e.g: OPA), keeping it up-to-date, by connecting to an opal-server and subscribing to pub/sub updates for policy and policy data changes.
 Home-page: https://github.com/permitio/opal
 Author: Or Weis, Asaf Cohen
 Author-email: or@permit.io
 License: Apache 2.0
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
@@ -48,34 +48,37 @@
 
 <a href="https://bit.ly/permit-slack" target="_blank">
     <img src="https://img.shields.io/badge/Slack%20Community-4A154B?logo=slack&logoColor=white" alt="Join our Slack!">
 </a>
 <a href="https://twitter.com/intent/follow?original_referer=https%3A%2F%2Fpublish.twitter.com%2F%3FbuttonType%3DFollowButton%26query%3Dhttps%253A%252F%252Ftwitter.com%252Fpermit_io%26widget%3DButton&ref_src=twsrc%5Etfw&region=follow_link&screen_name=permit_io&tw_p=followbutton"><img src="https://img.shields.io/twitter/follow/permit_io?label=Follow%20%40permit_io&style=social">
 </a>
 
-
-
 ## What is OPAL?
 
-OPAL is an administration layer for <a href="https://www.openpolicyagent.org/">Open Policy Agent (OPA)</a>, detecting changes to both policy and policy data in realtime and pushing live updates to your agents. OPAL brings open-policy up to the speed needed by live applications.
+OPAL is an administration layer for Policy Engines such as <a target="_blank" href="https://www.openpolicyagent.org/">Open Policy Agent (OPA)</a>, and <a target="_blank" href="https://github.com/permitio/cedar-agent">AWS' Cedar Agent</a> detecting changes to both policy and policy data in realtime and pushing live updates to your agents. OPAL brings open-policy up to the speed needed by live applications.
 
 As your application state changes (whether it's via your APIs, DBs, git, S3 or 3rd-party SaaS services), OPAL will make sure your services are always in sync with the authorization data and policy they need (and only those they need).
 
-Check out our main site at <a href="https://opal.ac">OPAL.ac</a>, <a href="https://youtu.be/tG8jrdcc7Zo">this video</a> briefly explaining OPAL and how it works with OPA, and a deeper dive into it at [this OWASP DevSlop talk](https://www.youtube.com/watch?v=1_Iz0tRQCH4).
+Check out our main site at <a target="_blank" href="https://opal.ac">OPAL.ac</a>, <a target="_blank" href="https://youtu.be/tG8jrdcc7Zo">this video</a> briefly explaining OPAL and how it works with OPA, and a deeper dive into it at [this OWASP DevSlop talk](https://www.youtube.com/watch?v=1_Iz0tRQCH4).
 
 ## Why use OPAL?
 
 OPAL is the easiest way to keep your solution's authorization layer up-to-date in realtime. It aggregates policy and data from across the field and integrates them seamlessly into the authorization layer, and is microservices and cloud-native.
 
-## OPA + OPAL = 💜
+## OPA + OPAL == 💜
 
 While OPA (Open Policy Agent) decouples policy from code in a highly-performant and elegant way, the challenge of keeping policy agents up-to-date remains.
 This is especially true in applications, where each user interaction or API call may affect access-control decisions.
 OPAL runs in the background, supercharging policy-agents, keeping them in sync with events in realtime.
 
+## AWS Cedar + OPAL == 💪
+
+Cedar is a very powerful policy language, which powers AWS' AVP (Amazon Verified Permissions) - but what if you want to enjoy the power of Cedar on another cloud, locally, or on premise?
+This is where [Cedar-Agent](https://github.com/permitio/cedar-agent) and OPAL come in.
+
 ## Documentation
 
 - 📃 &nbsp; [Full documentation is available here](https://docs.opal.ac)
 - 💡 &nbsp; [Intro to OPAL](https://docs.opal.ac/getting-started/intro)
 - 🚀 &nbsp; Getting Started:
 
   OPAL is available both as **python packages** with a built-in CLI as well as pre-built **docker images** ready-to-go.
@@ -152,7 +155,8 @@
 [badge-slack-link]: https://io.permit.io/join_community
 [follow-twitter-link]: https://i.ibb.co/k4x55Lr/Group-750.png
 [badge-twitter-link]: https://twitter.com/opal_ac
 
 ## There's more!
 
 - Check out [OPToggles](https://github.com/permitio/OPToggles), which enables you to create user targeted feature flags/toggles based on Open Policy managed authorization rules!
+- Check out [Cedar-Agent](https://github.com/permitio/cedar-agent), the easiest way to deploy & run AWS Cedar.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: opal-client Version: 0.7.0 Summary: OPAL is an
+Metadata-Version: 2.1 Name: opal-client Version: 0.7.1 Summary: OPAL is an
 administration layer for Open Policy Agent (OPA), detecting changes to both
 policy and data and pushing live updates to your agents. The opal-client is
 deployed alongside a policy-store (e.g: OPA), keeping it up-to-date, by
 connecting to an opal-server and subscribing to pub/sub updates for policy and
 policy data changes. Home-page: https://github.com/permitio/opal Author: Or
 Weis, Asaf Cohen Author-email: or@permit.io License: Apache 2.0 Classifier:
 Operating System :: OS Independent Classifier: License :: OSI Approved ::
@@ -14,43 +14,47 @@
 Python: >=3.7 Description-Content-Type: text/markdown
                                     [opal]
                            ****** â¡OPALâ¡ ******
                  ***** Open Policy Administration Layer *****
 [Tests] [Package] [Package] [Downloads] [Docker_pulls] [Join_our_Slack!]
 [https://img.shields.io/twitter/follow/
 permit_io?label=Follow%20%40permit_io&style=social] ## What is OPAL? OPAL is an
-administration layer for Open_Policy_Agent_(OPA), detecting changes to both
-policy and policy data in realtime and pushing live updates to your agents.
-OPAL brings open-policy up to the speed needed by live applications. As your
-application state changes (whether it's via your APIs, DBs, git, S3 or 3rd-
-party SaaS services), OPAL will make sure your services are always in sync with
-the authorization data and policy they need (and only those they need). Check
-out our main site at OPAL.ac, this_video briefly explaining OPAL and how it
-works with OPA, and a deeper dive into it at [this OWASP DevSlop talk](https://
-www.youtube.com/watch?v=1_Iz0tRQCH4). ## Why use OPAL? OPAL is the easiest way
-to keep your solution's authorization layer up-to-date in realtime. It
-aggregates policy and data from across the field and integrates them seamlessly
-into the authorization layer, and is microservices and cloud-native. ## OPA +
-OPAL = ð While OPA (Open Policy Agent) decouples policy from code in a
-highly-performant and elegant way, the challenge of keeping policy agents up-
-to-date remains. This is especially true in applications, where each user
-interaction or API call may affect access-control decisions. OPAL runs in the
-background, supercharging policy-agents, keeping them in sync with events in
-realtime. ## Documentation - ð   [Full documentation is available here]
-(https://docs.opal.ac) - ð¡   [Intro to OPAL](https://docs.opal.ac/getting-
-started/intro) - ð   Getting Started: OPAL is available both as **python
-packages** with a built-in CLI as well as pre-built **docker images** ready-to-
-go. - [Play with a live playground environment in docker-compose](https://
-docs.opal.ac/getting-started/quickstart/opal-playground/overview)  - [Try the
-getting started guide for containers](https://docs.opal.ac/getting-started/
-running-opal/overview)  - [Check out the Helm Chart for Kubernetes](https://
-github.com/permitio/opal-helm-chart) - A video demo of OPAL is available [here]
-(https://www.youtube.com/watch?v=IkR6EGY3QfM) - You can also check out this
-webinar and Q&A about OPAL [on our YouTube channel](https://www.youtube.com/
-watch?v=A5adHlkmdC0&t=1s)
+administration layer for Policy Engines such as Open_Policy_Agent_(OPA), and
+AWS'_Cedar_Agent detecting changes to both policy and policy data in realtime
+and pushing live updates to your agents. OPAL brings open-policy up to the
+speed needed by live applications. As your application state changes (whether
+it's via your APIs, DBs, git, S3 or 3rd-party SaaS services), OPAL will make
+sure your services are always in sync with the authorization data and policy
+they need (and only those they need). Check out our main site at OPAL.ac, this
+video briefly explaining OPAL and how it works with OPA, and a deeper dive into
+it at [this OWASP DevSlop talk](https://www.youtube.com/watch?v=1_Iz0tRQCH4).
+## Why use OPAL? OPAL is the easiest way to keep your solution's authorization
+layer up-to-date in realtime. It aggregates policy and data from across the
+field and integrates them seamlessly into the authorization layer, and is
+microservices and cloud-native. ## OPA + OPAL == ð While OPA (Open Policy
+Agent) decouples policy from code in a highly-performant and elegant way, the
+challenge of keeping policy agents up-to-date remains. This is especially true
+in applications, where each user interaction or API call may affect access-
+control decisions. OPAL runs in the background, supercharging policy-agents,
+keeping them in sync with events in realtime. ## AWS Cedar + OPAL == ðª Cedar
+is a very powerful policy language, which powers AWS' AVP (Amazon Verified
+Permissions) - but what if you want to enjoy the power of Cedar on another
+cloud, locally, or on premise? This is where [Cedar-Agent](https://github.com/
+permitio/cedar-agent) and OPAL come in. ## Documentation - ð   [Full
+documentation is available here](https://docs.opal.ac) - ð¡   [Intro to OPAL]
+(https://docs.opal.ac/getting-started/intro) - ð   Getting Started: OPAL is
+available both as **python packages** with a built-in CLI as well as pre-built
+**docker images** ready-to-go. - [Play with a live playground environment in
+docker-compose](https://docs.opal.ac/getting-started/quickstart/opal-
+playground/overview)  - [Try the getting started guide for containers](https://
+docs.opal.ac/getting-started/running-opal/overview)  - [Check out the Helm
+Chart for Kubernetes](https://github.com/permitio/opal-helm-chart) - A video
+demo of OPAL is available [here](https://www.youtube.com/watch?v=IkR6EGY3QfM) -
+You can also check out this webinar and Q&A about OPAL [on our YouTube channel]
+(https://www.youtube.com/watch?v=A5adHlkmdC0&t=1s)
 - ðª   TL;DR - This one command will download and run a working configuration
 of OPAL server and OPAL client on your machine: ``` curl -L https://
 raw.githubusercontent.com/permitio/opal/master/docker/docker-compose-
 example.yml \ > docker-compose.yml && docker-compose up ```
 [https://asciinema.org/a/409288.svg]
 - ð§    "How-To"s - [How to get started with OPAL (Packages and CLI)](https://
 docs.opal.ac/getting-started/running-opal/as-python-package/overview) - [How to
@@ -82,8 +86,9 @@
 and docs) - Prior to submitting a PR - open an issue on GitHub, or make sure
 your PR addresses an existing issue well. [join-slack-link]: https://i.ibb.co/
 wzrGHQL/Group-749.png [badge-slack-link]: https://io.permit.io/join_community
 [follow-twitter-link]: https://i.ibb.co/k4x55Lr/Group-750.png [badge-twitter-
 link]: https://twitter.com/opal_ac ## There's more! - Check out [OPToggles]
 (https://github.com/permitio/OPToggles), which enables you to create user
 targeted feature flags/toggles based on Open Policy managed authorization
-rules!
+rules! - Check out [Cedar-Agent](https://github.com/permitio/cedar-agent), the
+easiest way to deploy & run AWS Cedar.
```

### Comparing `opal-client-0.7.0/opal_client/callbacks/api.py` & `opal-client-0.7.1/opal_client/callbacks/api.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.0/opal_client/callbacks/register.py` & `opal-client-0.7.1/opal_client/callbacks/register.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.0/opal_client/callbacks/reporter.py` & `opal-client-0.7.1/opal_client/callbacks/reporter.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.0/opal_client/cli.py` & `opal-client-0.7.1/opal_client/cli.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.0/opal_client/client.py` & `opal-client-0.7.1/opal_client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,24 +105,28 @@
 
         self._callbacks_register = CallbacksRegister(default_callbacks)
 
         self._startup_wait = None
         if opal_client_config.WAIT_ON_SERVER_LOAD:
             self._startup_wait = StartupLoadLimiter()
 
-        # Init policy updater
-        if policy_updater is not None:
-            self.policy_updater = policy_updater
+        if opal_client_config.POLICY_UPDATER_ENABLED:
+            # Init policy updater
+            if policy_updater is not None:
+                self.policy_updater = policy_updater
+            else:
+                self.policy_updater = PolicyUpdater(
+                    policy_store=self.policy_store,
+                    data_fetcher=self.data_fetcher,
+                    callbacks_register=self._callbacks_register,
+                    opal_client_id=opal_client_identifier,
+                )
         else:
-            self.policy_updater = PolicyUpdater(
-                policy_store=self.policy_store,
-                data_fetcher=self.data_fetcher,
-                callbacks_register=self._callbacks_register,
-                opal_client_id=opal_client_identifier,
-            )
+            self.policy_updater = None
+
         # Data updating service
         if opal_client_config.DATA_UPDATER_ENABLED:
             if data_updater is not None:
                 self.data_updater = data_updater
             else:
                 data_topics = (
                     data_topics
@@ -189,20 +193,22 @@
         inline_opa_options: Optional[OpaServerOptions] = None,
         inline_cedar_options: Optional[CedarServerOptions] = None,
     ) -> Union[OpaRunner, CedarRunner, Literal[False]]:
         if inline_opa_enabled and self.policy_store_type == PolicyStoreTypes.OPA:
             inline_opa_options = (
                 inline_opa_options or opal_client_config.INLINE_OPA_CONFIG
             )
-            rehydration_callbacks = [
-                # refetches policy code (e.g: rego) and static data from server
-                functools.partial(
-                    self.policy_updater.update_policy, force_full_update=True
-                ),
-            ]
+            rehydration_callbacks = []
+            if self.policy_updater:
+                rehydration_callbacks.append(
+                    # refetches policy code (e.g: rego) and static data from server
+                    functools.partial(
+                        self.policy_updater.update_policy, force_full_update=True
+                    ),
+                )
 
             if self.data_updater:
                 rehydration_callbacks.append(
                     functools.partial(
                         self.data_updater.get_base_policy_data,
                         data_fetch_reason="policy store rehydration",
                     )
```

### Comparing `opal-client-0.7.0/opal_client/config.py` & `opal-client-0.7.1/opal_client/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,14 +70,36 @@
 
     POLICY_STORE_POLICY_PATHS_TO_IGNORE = confi.list(
         "POLICY_STORE_POLICY_PATHS_TO_IGNORE",
         [],
         description="When loading policies manually or otherwise externally into the policy store, use this list of glob patterns to have OPAL ignore and not delete or override them, end paths (without any wildcards in the middle) with '\**' to indicate you want all nested under the path to be ignored",
     )
 
+    POLICY_UPDATER_ENABLED = confi.bool(
+        "POLICY_UPDATER_ENABLED",
+        True,
+        description="If set to False, opal client will not listen to dynamic policy updates."
+        "Policy update fetching will be completely disabled.",
+    )
+    POLICY_STORE_TLS_CLIENT_CERT = confi.str(
+        "POLICY_STORE_TLS_CLIENT_CERT",
+        None,
+        description="path to the client certificate used for tls authentication with the policy store",
+    )
+    POLICY_STORE_TLS_CLIENT_KEY = confi.str(
+        "POLICY_STORE_TLS_CLIENT_KEY",
+        None,
+        description="path to the client key used for tls authentication with the policy store",
+    )
+    POLICY_STORE_TLS_CA = confi.str(
+        "POLICY_STORE_TLS_CA",
+        None,
+        description="path to the file containing the ca certificate(s) used for tls authentication with the policy store",
+    )
+
     # create an instance of a policy store upon load
     def load_policy_store():
         from opal_client.policy_store.policy_store_client_factory import (
             PolicyStoreClientFactory,
         )
 
         return PolicyStoreClientFactory.create()
@@ -271,14 +293,17 @@
         description="Interval in seconds to backup policy store's data",
     )
     OFFLINE_MODE_ENABLED = confi.bool(
         "OFFLINE_MODE_ENABLED",
         False,
         description="If set, opal client will try to load policy store from backup file and operate even if server is unreachable. Ignored if INLINE_OPA_ENABLED=False",
     )
+    SPLIT_ROOT_DATA = confi.bool(
+        "SPLIT_ROOT_DATA", False, description="Split writing data updates to root path"
+    )
 
     def on_load(self):
         # LOGGER
         if self.INLINE_OPA_LOG_FORMAT == EngineLogFormat.NONE:
             opal_common_config.LOG_MODULE_EXCLUDE_LIST.append("opal_client.opa.logger")
             # re-assign to apply to internal confi-entries as well
             opal_common_config.LOG_MODULE_EXCLUDE_LIST = (
```

### Comparing `opal-client-0.7.0/opal_client/data/api.py` & `opal-client-0.7.1/opal_client/data/api.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.0/opal_client/data/fetcher.py` & `opal-client-0.7.1/opal_client/data/fetcher.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.0/opal_client/data/rpc.py` & `opal-client-0.7.1/opal_client/data/rpc.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.0/opal_client/data/updater.py` & `opal-client-0.7.1/opal_client/data/updater.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import asyncio
 import hashlib
 import itertools
 import json
 import uuid
-from typing import List, Optional, Tuple
+from typing import Any, Dict, List, Optional, Tuple
 
 import aiohttp
 from aiohttp.client import ClientError, ClientSession
 from fastapi_websocket_pubsub import PubSubClient
 from fastapi_websocket_rpc.rpc_channel import RpcChannel
 from opal_client.callbacks.register import CallbacksRegister
 from opal_client.callbacks.reporter import CallbacksReporter
@@ -397,23 +397,31 @@
                     ):
                         policy_store_path = f"/{policy_store_path}"
                     policy_data = result
                     # Create a report on the data-fetching
                     report = DataEntryReport(
                         entry=entry, hash=self.calc_hash(policy_data), fetched=True
                     )
-                    logger.info(
-                        "Saving fetched data to policy-store: source url='{url}', destination path='{path}'",
-                        url=url,
-                        path=policy_store_path or "/",
-                    )
+
                     try:
-                        await store_transaction.set_policy_data(
-                            policy_data, path=policy_store_path
-                        )
+                        if (
+                            opal_client_config.SPLIT_ROOT_DATA
+                            and policy_store_path in ("/", "")
+                            and isinstance(policy_data, dict)
+                        ):
+                            await self._set_split_policy_data(
+                                store_transaction, url=url, data=policy_data
+                            )
+                        else:
+                            await self._set_policy_data(
+                                store_transaction,
+                                url=url,
+                                path=policy_store_path,
+                                data=policy_data,
+                            )
                         # No exception we we're able to save to the policy-store
                         report.saved = True
                         # save the report for the entry
                         reports.append(report)
                     except Exception:
                         logger.exception("Failed to save data update to policy-store")
                         # we failed to save to policy-store
@@ -434,7 +442,24 @@
                 update.callback.callbacks
             )
             asyncio.create_task(
                 self._callbacks_reporter.report_update_results(
                     whole_report, extra_callbacks
                 )
             )
+
+    async def _set_split_policy_data(self, tx, url: str, data: Dict[str, Any]):
+        """Split data writes to root ("/") path, so they won't overwrite other
+        sources."""
+        logger.info("Splitting root data to {n} keys", n=len(data))
+
+        for prefix, obj in data.items():
+            await self._set_policy_data(tx, url=url, path=f"/{prefix}", data=obj)
+
+    async def _set_policy_data(self, tx, url: str, path: str, data: JsonableValue):
+        logger.info(
+            "Saving fetched data to policy-store: source url='{url}', destination path='{path}'",
+            url=url,
+            path=path or "/",
+        )
+
+        await tx.set_policy_data(data, path=path)
```

### Comparing `opal-client-0.7.0/opal_client/engine/healthcheck/opal.rego` & `opal-client-0.7.1/opal_client/engine/healthcheck/opal.rego`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.0/opal_client/engine/logger.py` & `opal-client-0.7.1/opal_client/engine/logger.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.0/opal_client/engine/options.py` & `opal-client-0.7.1/opal_client/engine/options.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.0/opal_client/engine/runner.py` & `opal-client-0.7.1/opal_client/engine/runner.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.0/opal_client/limiter.py` & `opal-client-0.7.1/opal_client/limiter.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.0/opal_client/policy/fetcher.py` & `opal-client-0.7.1/opal_client/policy/fetcher.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.0/opal_client/policy/options.py` & `opal-client-0.7.1/opal_client/policy/options.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.0/opal_client/policy/topics.py` & `opal-client-0.7.1/opal_client/policy/topics.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.0/opal_client/policy/updater.py` & `opal-client-0.7.1/opal_client/policy/updater.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.0/opal_client/policy_store/api.py` & `opal-client-0.7.1/opal_client/policy_store/api.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.0/opal_client/policy_store/base_policy_store_client.py` & `opal-client-0.7.1/opal_client/policy_store/base_policy_store_client.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.0/opal_client/policy_store/cedar_client.py` & `opal-client-0.7.1/opal_client/policy_store/cedar_client.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.0/opal_client/policy_store/mock_policy_store_client.py` & `opal-client-0.7.1/opal_client/policy_store/mock_policy_store_client.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.0/opal_client/policy_store/opa_client.py` & `opal-client-0.7.1/opal_client/policy_store/opa_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import asyncio
 import functools
 import json
+import ssl
 import time
 from typing import Any, Awaitable, Callable, Dict, List, Optional, Set
 from urllib.parse import urlencode
 
 import aiohttp
 import dpath
 from aiofiles.threadpool.text import AsyncTextIOWrapper
@@ -85,16 +86,18 @@
 
     POLICY_ACTIONS = ["set_policies", "set_policy", "delete_policy"]
     DATA_ACTIONS = ["set_policy_data", "delete_policy_data"]
 
     def __init__(
         self,
         data_updater_enabled: bool = True,
+        policy_updater_enabled: bool = True,
     ):
         self._data_updater_disabled = not data_updater_enabled
+        self._policy_updater_disabled = not policy_updater_enabled
         self._num_successful_policy_transactions = 0
         self._num_failed_policy_transactions = 0
         self._num_successful_data_transactions = 0
         self._num_failed_data_transactions = 0
         self._last_policy_transaction: Optional[StoreTransaction] = None
         self._last_failed_policy_transaction: Optional[StoreTransaction] = None
         self._last_data_transaction: Optional[StoreTransaction] = None
@@ -113,17 +116,17 @@
             self._last_policy_transaction is not None
             and self._last_policy_transaction.success
         )
         data_updater_is_healthy: bool = (
             self._last_data_transaction is not None
             and self._last_data_transaction.success
         )
-        is_healthy: bool = policy_updater_is_healthy and (
-            self._data_updater_disabled or data_updater_is_healthy
-        )
+        is_healthy: bool = (
+            self._policy_updater_disabled or policy_updater_is_healthy
+        ) and (self._data_updater_disabled or data_updater_is_healthy)
         logger.info(
             f"OPA client health: {is_healthy} (policy: {policy_updater_is_healthy}, data: {data_updater_is_healthy})"
         )
         return is_healthy
 
     @property
     def last_policy_transaction(self):
@@ -279,26 +282,33 @@
         opa_server_url=None,
         opa_auth_token: Optional[str] = None,
         auth_type: PolicyStoreAuth = PolicyStoreAuth.NONE,
         oauth_client_id: Optional[str] = None,
         oauth_client_secret: Optional[str] = None,
         oauth_server: Optional[str] = None,
         data_updater_enabled: bool = True,
+        policy_updater_enabled: bool = True,
         cache_policy_data: bool = False,
+        tls_client_cert: Optional[str] = None,
+        tls_client_key: Optional[str] = None,
+        tls_ca: Optional[str] = None,
     ):
         base_url = opa_server_url or opal_client_config.POLICY_STORE_URL
         self._opa_url = f"{base_url}/v1"
         self._policy_version: Optional[str] = None
         self._lock = asyncio.Lock()
         self._token = opa_auth_token
         self._auth_type: PolicyStoreAuth = auth_type
         self._oauth_client_id = oauth_client_id
         self._oauth_client_secret = oauth_client_secret
         self._oauth_server = oauth_server
         self._oauth_token_cache = {"token": None, "expires": 0}
+        self._tls_client_cert = tls_client_cert
+        self._tls_client_key = tls_client_key
+        self._tls_ca = tls_ca
 
         if auth_type == PolicyStoreAuth.TOKEN:
             if self._token is None:
                 logger.error("POLICY_STORE_AUTH_TOKEN can not be empty")
                 raise Exception("required variables for token auth are not set")
 
         if auth_type == PolicyStoreAuth.OAUTH:
@@ -314,24 +324,68 @@
             if self._oauth_server is None:
                 isError = True
                 logger.error("POLICY_STORE_AUTH_OAUTH_SERVER can not be empty")
 
             if isError:
                 raise Exception("required variables for oauth are not set")
 
+        if auth_type == PolicyStoreAuth.TLS:
+            isError = False
+            if self._tls_client_cert is None:
+                isError = True
+                logger.error("POLICY_STORE_TLS_CLIENT_CERT can not be empty")
+
+            if self._tls_client_key is None:
+                isError = True
+                logger.error("POLICY_STORE_TLS_CLIENT_KEY can not be empty")
+
+            if self._tls_ca is None:
+                isError = True
+                logger.error("POLICY_STORE_TLS_CA can not be empty")
+
+            if isError:
+                raise Exception("required variables for tls are not set")
+
         logger.info(f"Authentication mode for policy store: {auth_type}")
 
-        self._transaction_state = OpaTransactionLogState(data_updater_enabled)
+        # custom SSL context
+        self._custom_ssl_context = self._get_custom_ssl_context()
+        self._ssl_context_kwargs = (
+            {"ssl": self._custom_ssl_context}
+            if self._custom_ssl_context is not None
+            else {}
+        )
+
+        self._transaction_state = OpaTransactionLogState(
+            data_updater_enabled=data_updater_enabled,
+            policy_updater_enabled=policy_updater_enabled,
+        )
         # as long as this is null, persisting transaction log to OPA is disabled
         self._transaction_state_writer: Optional[OpaTransactionLogState] = None
 
         self._policy_data_cache: Optional[OpaStaticDataCache] = None
         if cache_policy_data:
             self._policy_data_cache = OpaStaticDataCache()
 
+    def _get_custom_ssl_context(self) -> Optional[ssl.SSLContext]:
+
+        if not self._tls_ca:
+            return None
+
+        ssl_context = ssl.create_default_context(
+            purpose=ssl.Purpose.SERVER_AUTH, cafile=self._tls_ca
+        )
+
+        if self._tls_client_key and self._tls_client_cert:
+            ssl_context.load_cert_chain(
+                certfile=self._tls_client_cert, keyfile=self._tls_client_key
+            )
+
+        return ssl_context
+
     async def get_policy_version(self) -> Optional[str]:
         return self._policy_version
 
     @retry(**RETRY_CONFIG)
     async def _get_oauth_token(self):
         logger.info("Retrieving a new OAuth access_token.")
 
@@ -403,35 +457,39 @@
             try:
                 headers = await self._get_auth_headers()
 
                 async with session.put(
                     f"{self._opa_url}/policies/{policy_id}",
                     data=policy_code,
                     headers={"content-type": "text/plain", **headers},
+                    **self._ssl_context_kwargs,
                 ) as opa_response:
                     return await proxy_response_unless_invalid(
                         opa_response,
                         accepted_status_codes=[
                             status.HTTP_200_OK,
-                            status.HTTP_400_BAD_REQUEST,  # No point in immediate retry, this means erroneous rego (bad syntax, duplicated definition, etc)
+                            # No point in immediate retry, this means erroneous rego (bad syntax, duplicated definition, etc)
+                            status.HTTP_400_BAD_REQUEST,
                         ],
                     )
             except aiohttp.ClientError as e:
                 logger.warning("Opa connection error: {err}", err=repr(e))
                 raise
 
     @fail_silently()
     @retry(**RETRY_CONFIG)
     async def get_policy(self, policy_id: str) -> Optional[str]:
         async with aiohttp.ClientSession() as session:
             try:
                 headers = await self._get_auth_headers()
 
                 async with session.get(
-                    f"{self._opa_url}/policies/{policy_id}", headers=headers
+                    f"{self._opa_url}/policies/{policy_id}",
+                    headers=headers,
+                    **self._ssl_context_kwargs,
                 ) as opa_response:
                     result = await opa_response.json()
                     return result.get("result", {}).get("raw", None)
             except aiohttp.ClientError as e:
                 logger.warning("Opa connection error: {err}", err=repr(e))
                 raise
 
@@ -439,15 +497,17 @@
     @retry(**RETRY_CONFIG)
     async def get_policies(self) -> Optional[Dict[str, str]]:
         async with aiohttp.ClientSession() as session:
             try:
                 headers = await self._get_auth_headers()
 
                 async with session.get(
-                    f"{self._opa_url}/policies", headers=headers
+                    f"{self._opa_url}/policies",
+                    headers=headers,
+                    **self._ssl_context_kwargs,
                 ) as opa_response:
                     result = await opa_response.json()
                     return OpaClient._extract_modules_from_policies_json(result)
             except aiohttp.ClientError as e:
                 logger.warning("Opa connection error: {err}", err=repr(e))
                 raise
 
@@ -464,15 +524,17 @@
             return
 
         async with aiohttp.ClientSession() as session:
             try:
                 headers = await self._get_auth_headers()
 
                 async with session.delete(
-                    f"{self._opa_url}/policies/{policy_id}", headers=headers
+                    f"{self._opa_url}/policies/{policy_id}",
+                    headers=headers,
+                    **self._ssl_context_kwargs,
                 ) as opa_response:
                     return await proxy_response_unless_invalid(
                         opa_response,
                         accepted_status_codes=[
                             status.HTTP_200_OK,
                             status.HTTP_404_NOT_FOUND,
                         ],
@@ -548,14 +610,15 @@
                     failed_ops.append(op)
 
             if len(failed_ops) == 0:
                 # all ops succeeded
                 return
 
             if len(failed_ops) == len(ops):
+
                 # all ops failed on this iteration, no point at retrying
                 for failure_msg in failure_msgs:
                     logger.error(failure_msg)
 
                 raise RuntimeError("Giving up setting / deleting failed modules to OPA")
 
             ops = failed_ops  # retry failed ops
@@ -679,14 +742,15 @@
             try:
                 headers = await self._get_auth_headers()
 
                 async with session.put(
                     f"{self._opa_url}/data{path}",
                     data=json.dumps(policy_data, default=str),
                     headers=headers,
+                    **self._ssl_context_kwargs,
                 ) as opa_response:
                     response = await proxy_response_unless_invalid(
                         opa_response,
                         accepted_status_codes=[
                             status.HTTP_204_NO_CONTENT,
                             status.HTTP_304_NOT_MODIFIED,
                         ],
@@ -708,15 +772,17 @@
             return await self.set_policy_data({})
 
         async with aiohttp.ClientSession() as session:
             try:
                 headers = await self._get_auth_headers()
 
                 async with session.delete(
-                    f"{self._opa_url}/data{path}", headers=headers
+                    f"{self._opa_url}/data{path}",
+                    headers=headers,
+                    **self._ssl_context_kwargs,
                 ) as opa_response:
                     response = await proxy_response_unless_invalid(
                         opa_response,
                         accepted_status_codes=[
                             status.HTTP_204_NO_CONTENT,
                             status.HTTP_404_NOT_FOUND,
                         ],
@@ -741,15 +807,17 @@
         if path != "" and not path.startswith("/"):
             path = "/" + path
         try:
             headers = await self._get_auth_headers()
 
             async with aiohttp.ClientSession() as session:
                 async with session.get(
-                    f"{self._opa_url}/data{path}", headers=headers
+                    f"{self._opa_url}/data{path}",
+                    headers=headers,
+                    **self._ssl_context_kwargs,
                 ) as opa_response:
                     json_response = await opa_response.json()
                     return json_response.get("result", {})
         except aiohttp.ClientError as e:
             logger.warning("Opa connection error: {err}", err=repr(e))
             raise
 
@@ -772,14 +840,15 @@
             headers = await self._get_auth_headers()
 
             async with aiohttp.ClientSession() as session:
                 async with session.post(
                     f"{self._opa_url}/data/{path}",
                     data=json.dumps(opa_input),
                     headers=headers,
+                    **self._ssl_context_kwargs,
                 ) as opa_response:
                     return await proxy_response(opa_response)
         except aiohttp.ClientError as e:
             logger.warning("Opa connection error: {err}", err=repr(e))
             raise
 
     @retry(**RETRY_CONFIG)
```

### Comparing `opal-client-0.7.0/opal_client/policy_store/policy_store_client_factory.py` & `opal-client-0.7.1/opal_client/policy_store/policy_store_client_factory.py`

 * *Files 12% similar despite different names*

```diff
@@ -66,15 +66,19 @@
         save_to_cache=True,
         token: Optional[str] = None,
         auth_type: PolicyStoreAuth = None,
         oauth_client_id: Optional[str] = None,
         oauth_client_secret: Optional[str] = None,
         oauth_server: Optional[str] = None,
         data_updater_enabled: Optional[bool] = None,
+        policy_updater_enabled: Optional[bool] = None,
         offline_mode_enabled: bool = False,
+        tls_client_cert: Optional[str] = None,
+        tls_client_key: Optional[str] = None,
+        tls_ca: Optional[str] = None,
     ) -> BasePolicyStoreClient:
         """
         Factory method - create a new policy store by type.
 
         Args:
             store_type (PolicyStoreTypes, optional): The type of policy-store to use. Defaults to opal_client_config.POLICY_STORE_TYPE.
             url (str, optional): the URL of the policy store. Defaults to opal_client_config.POLICY_STORE_URL.
@@ -101,30 +105,48 @@
         )
         oauth_server = oauth_server or opal_client_config.POLICY_STORE_AUTH_OAUTH_SERVER
         data_updater_enabled = (
             data_updater_enabled
             if data_updater_enabled is not None
             else opal_client_config.DATA_UPDATER_ENABLED
         )
+        policy_updater_enabled = (
+            policy_updater_enabled
+            if policy_updater_enabled is not None
+            else opal_client_config.POLICY_UPDATER_ENABLED
+        )
 
         res: Optional[BasePolicyStoreClient] = None
+        tls_client_cert = (
+            tls_client_cert or opal_client_config.POLICY_STORE_TLS_CLIENT_CERT
+        )
+
+        tls_client_key = (
+            tls_client_key or opal_client_config.POLICY_STORE_TLS_CLIENT_KEY
+        )
+
+        tls_ca = tls_ca or opal_client_config.POLICY_STORE_TLS_CA
 
         # OPA
         if PolicyStoreTypes.OPA == store_type:
             from opal_client.policy_store.opa_client import OpaClient
 
             res = OpaClient(
                 url,
                 opa_auth_token=store_token,
                 auth_type=auth_type,
                 oauth_client_id=oauth_client_id,
                 oauth_client_secret=oauth_client_secret,
                 oauth_server=oauth_server,
                 data_updater_enabled=data_updater_enabled,
+                policy_updater_enabled=policy_updater_enabled,
                 cache_policy_data=offline_mode_enabled,
+                tls_client_cert=tls_client_cert,
+                tls_client_key=tls_client_key,
+                tls_ca=tls_ca,
             )
         elif PolicyStoreTypes.CEDAR == store_type:
             from opal_client.policy_store.cedar_client import CedarClient
 
             res = CedarClient(
                 url,
                 cedar_auth_token=store_token,
```

### Comparing `opal-client-0.7.0/opal_client/policy_store/schemas.py` & `opal-client-0.7.1/opal_client/policy_store/schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     MOCK = "MOCK"
 
 
 class PolicyStoreAuth(Enum):
     NONE = "none"
     TOKEN = "token"
     OAUTH = "oauth"
+    TLS = "tls"
 
 
 class PolicyStoreDetails(BaseModel):
     """
     represents a policy store endpoint - contains the policy store's:
     - location (url)
     - type
```

### Comparing `opal-client-0.7.0/opal_client/tests/data_updater_test.py` & `opal-client-0.7.1/opal_client/tests/data_updater_test.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.0/opal_client/tests/server_to_client_intergation_test.py` & `opal-client-0.7.1/opal_client/tests/server_to_client_intergation_test.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.0/opal_client.egg-info/PKG-INFO` & `opal-client-0.7.1/opal_client.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opal-client
-Version: 0.7.0
+Version: 0.7.1
 Summary: OPAL is an administration layer for Open Policy Agent (OPA), detecting changes to both policy and data and pushing live updates to your agents. The opal-client is deployed alongside a policy-store (e.g: OPA), keeping it up-to-date, by connecting to an opal-server and subscribing to pub/sub updates for policy and policy data changes.
 Home-page: https://github.com/permitio/opal
 Author: Or Weis, Asaf Cohen
 Author-email: or@permit.io
 License: Apache 2.0
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
@@ -48,34 +48,37 @@
 
 <a href="https://bit.ly/permit-slack" target="_blank">
     <img src="https://img.shields.io/badge/Slack%20Community-4A154B?logo=slack&logoColor=white" alt="Join our Slack!">
 </a>
 <a href="https://twitter.com/intent/follow?original_referer=https%3A%2F%2Fpublish.twitter.com%2F%3FbuttonType%3DFollowButton%26query%3Dhttps%253A%252F%252Ftwitter.com%252Fpermit_io%26widget%3DButton&ref_src=twsrc%5Etfw&region=follow_link&screen_name=permit_io&tw_p=followbutton"><img src="https://img.shields.io/twitter/follow/permit_io?label=Follow%20%40permit_io&style=social">
 </a>
 
-
-
 ## What is OPAL?
 
-OPAL is an administration layer for <a href="https://www.openpolicyagent.org/">Open Policy Agent (OPA)</a>, detecting changes to both policy and policy data in realtime and pushing live updates to your agents. OPAL brings open-policy up to the speed needed by live applications.
+OPAL is an administration layer for Policy Engines such as <a target="_blank" href="https://www.openpolicyagent.org/">Open Policy Agent (OPA)</a>, and <a target="_blank" href="https://github.com/permitio/cedar-agent">AWS' Cedar Agent</a> detecting changes to both policy and policy data in realtime and pushing live updates to your agents. OPAL brings open-policy up to the speed needed by live applications.
 
 As your application state changes (whether it's via your APIs, DBs, git, S3 or 3rd-party SaaS services), OPAL will make sure your services are always in sync with the authorization data and policy they need (and only those they need).
 
-Check out our main site at <a href="https://opal.ac">OPAL.ac</a>, <a href="https://youtu.be/tG8jrdcc7Zo">this video</a> briefly explaining OPAL and how it works with OPA, and a deeper dive into it at [this OWASP DevSlop talk](https://www.youtube.com/watch?v=1_Iz0tRQCH4).
+Check out our main site at <a target="_blank" href="https://opal.ac">OPAL.ac</a>, <a target="_blank" href="https://youtu.be/tG8jrdcc7Zo">this video</a> briefly explaining OPAL and how it works with OPA, and a deeper dive into it at [this OWASP DevSlop talk](https://www.youtube.com/watch?v=1_Iz0tRQCH4).
 
 ## Why use OPAL?
 
 OPAL is the easiest way to keep your solution's authorization layer up-to-date in realtime. It aggregates policy and data from across the field and integrates them seamlessly into the authorization layer, and is microservices and cloud-native.
 
-## OPA + OPAL = 💜
+## OPA + OPAL == 💜
 
 While OPA (Open Policy Agent) decouples policy from code in a highly-performant and elegant way, the challenge of keeping policy agents up-to-date remains.
 This is especially true in applications, where each user interaction or API call may affect access-control decisions.
 OPAL runs in the background, supercharging policy-agents, keeping them in sync with events in realtime.
 
+## AWS Cedar + OPAL == 💪
+
+Cedar is a very powerful policy language, which powers AWS' AVP (Amazon Verified Permissions) - but what if you want to enjoy the power of Cedar on another cloud, locally, or on premise?
+This is where [Cedar-Agent](https://github.com/permitio/cedar-agent) and OPAL come in.
+
 ## Documentation
 
 - 📃 &nbsp; [Full documentation is available here](https://docs.opal.ac)
 - 💡 &nbsp; [Intro to OPAL](https://docs.opal.ac/getting-started/intro)
 - 🚀 &nbsp; Getting Started:
 
   OPAL is available both as **python packages** with a built-in CLI as well as pre-built **docker images** ready-to-go.
@@ -152,7 +155,8 @@
 [badge-slack-link]: https://io.permit.io/join_community
 [follow-twitter-link]: https://i.ibb.co/k4x55Lr/Group-750.png
 [badge-twitter-link]: https://twitter.com/opal_ac
 
 ## There's more!
 
 - Check out [OPToggles](https://github.com/permitio/OPToggles), which enables you to create user targeted feature flags/toggles based on Open Policy managed authorization rules!
+- Check out [Cedar-Agent](https://github.com/permitio/cedar-agent), the easiest way to deploy & run AWS Cedar.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: opal-client Version: 0.7.0 Summary: OPAL is an
+Metadata-Version: 2.1 Name: opal-client Version: 0.7.1 Summary: OPAL is an
 administration layer for Open Policy Agent (OPA), detecting changes to both
 policy and data and pushing live updates to your agents. The opal-client is
 deployed alongside a policy-store (e.g: OPA), keeping it up-to-date, by
 connecting to an opal-server and subscribing to pub/sub updates for policy and
 policy data changes. Home-page: https://github.com/permitio/opal Author: Or
 Weis, Asaf Cohen Author-email: or@permit.io License: Apache 2.0 Classifier:
 Operating System :: OS Independent Classifier: License :: OSI Approved ::
@@ -14,43 +14,47 @@
 Python: >=3.7 Description-Content-Type: text/markdown
                                     [opal]
                            ****** â¡OPALâ¡ ******
                  ***** Open Policy Administration Layer *****
 [Tests] [Package] [Package] [Downloads] [Docker_pulls] [Join_our_Slack!]
 [https://img.shields.io/twitter/follow/
 permit_io?label=Follow%20%40permit_io&style=social] ## What is OPAL? OPAL is an
-administration layer for Open_Policy_Agent_(OPA), detecting changes to both
-policy and policy data in realtime and pushing live updates to your agents.
-OPAL brings open-policy up to the speed needed by live applications. As your
-application state changes (whether it's via your APIs, DBs, git, S3 or 3rd-
-party SaaS services), OPAL will make sure your services are always in sync with
-the authorization data and policy they need (and only those they need). Check
-out our main site at OPAL.ac, this_video briefly explaining OPAL and how it
-works with OPA, and a deeper dive into it at [this OWASP DevSlop talk](https://
-www.youtube.com/watch?v=1_Iz0tRQCH4). ## Why use OPAL? OPAL is the easiest way
-to keep your solution's authorization layer up-to-date in realtime. It
-aggregates policy and data from across the field and integrates them seamlessly
-into the authorization layer, and is microservices and cloud-native. ## OPA +
-OPAL = ð While OPA (Open Policy Agent) decouples policy from code in a
-highly-performant and elegant way, the challenge of keeping policy agents up-
-to-date remains. This is especially true in applications, where each user
-interaction or API call may affect access-control decisions. OPAL runs in the
-background, supercharging policy-agents, keeping them in sync with events in
-realtime. ## Documentation - ð   [Full documentation is available here]
-(https://docs.opal.ac) - ð¡   [Intro to OPAL](https://docs.opal.ac/getting-
-started/intro) - ð   Getting Started: OPAL is available both as **python
-packages** with a built-in CLI as well as pre-built **docker images** ready-to-
-go. - [Play with a live playground environment in docker-compose](https://
-docs.opal.ac/getting-started/quickstart/opal-playground/overview)  - [Try the
-getting started guide for containers](https://docs.opal.ac/getting-started/
-running-opal/overview)  - [Check out the Helm Chart for Kubernetes](https://
-github.com/permitio/opal-helm-chart) - A video demo of OPAL is available [here]
-(https://www.youtube.com/watch?v=IkR6EGY3QfM) - You can also check out this
-webinar and Q&A about OPAL [on our YouTube channel](https://www.youtube.com/
-watch?v=A5adHlkmdC0&t=1s)
+administration layer for Policy Engines such as Open_Policy_Agent_(OPA), and
+AWS'_Cedar_Agent detecting changes to both policy and policy data in realtime
+and pushing live updates to your agents. OPAL brings open-policy up to the
+speed needed by live applications. As your application state changes (whether
+it's via your APIs, DBs, git, S3 or 3rd-party SaaS services), OPAL will make
+sure your services are always in sync with the authorization data and policy
+they need (and only those they need). Check out our main site at OPAL.ac, this
+video briefly explaining OPAL and how it works with OPA, and a deeper dive into
+it at [this OWASP DevSlop talk](https://www.youtube.com/watch?v=1_Iz0tRQCH4).
+## Why use OPAL? OPAL is the easiest way to keep your solution's authorization
+layer up-to-date in realtime. It aggregates policy and data from across the
+field and integrates them seamlessly into the authorization layer, and is
+microservices and cloud-native. ## OPA + OPAL == ð While OPA (Open Policy
+Agent) decouples policy from code in a highly-performant and elegant way, the
+challenge of keeping policy agents up-to-date remains. This is especially true
+in applications, where each user interaction or API call may affect access-
+control decisions. OPAL runs in the background, supercharging policy-agents,
+keeping them in sync with events in realtime. ## AWS Cedar + OPAL == ðª Cedar
+is a very powerful policy language, which powers AWS' AVP (Amazon Verified
+Permissions) - but what if you want to enjoy the power of Cedar on another
+cloud, locally, or on premise? This is where [Cedar-Agent](https://github.com/
+permitio/cedar-agent) and OPAL come in. ## Documentation - ð   [Full
+documentation is available here](https://docs.opal.ac) - ð¡   [Intro to OPAL]
+(https://docs.opal.ac/getting-started/intro) - ð   Getting Started: OPAL is
+available both as **python packages** with a built-in CLI as well as pre-built
+**docker images** ready-to-go. - [Play with a live playground environment in
+docker-compose](https://docs.opal.ac/getting-started/quickstart/opal-
+playground/overview)  - [Try the getting started guide for containers](https://
+docs.opal.ac/getting-started/running-opal/overview)  - [Check out the Helm
+Chart for Kubernetes](https://github.com/permitio/opal-helm-chart) - A video
+demo of OPAL is available [here](https://www.youtube.com/watch?v=IkR6EGY3QfM) -
+You can also check out this webinar and Q&A about OPAL [on our YouTube channel]
+(https://www.youtube.com/watch?v=A5adHlkmdC0&t=1s)
 - ðª   TL;DR - This one command will download and run a working configuration
 of OPAL server and OPAL client on your machine: ``` curl -L https://
 raw.githubusercontent.com/permitio/opal/master/docker/docker-compose-
 example.yml \ > docker-compose.yml && docker-compose up ```
 [https://asciinema.org/a/409288.svg]
 - ð§    "How-To"s - [How to get started with OPAL (Packages and CLI)](https://
 docs.opal.ac/getting-started/running-opal/as-python-package/overview) - [How to
@@ -82,8 +86,9 @@
 and docs) - Prior to submitting a PR - open an issue on GitHub, or make sure
 your PR addresses an existing issue well. [join-slack-link]: https://i.ibb.co/
 wzrGHQL/Group-749.png [badge-slack-link]: https://io.permit.io/join_community
 [follow-twitter-link]: https://i.ibb.co/k4x55Lr/Group-750.png [badge-twitter-
 link]: https://twitter.com/opal_ac ## There's more! - Check out [OPToggles]
 (https://github.com/permitio/OPToggles), which enables you to create user
 targeted feature flags/toggles based on Open Policy managed authorization
-rules!
+rules! - Check out [Cedar-Agent](https://github.com/permitio/cedar-agent), the
+easiest way to deploy & run AWS Cedar.
```

### Comparing `opal-client-0.7.0/opal_client.egg-info/SOURCES.txt` & `opal-client-0.7.1/opal_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.0/setup.py` & `opal-client-0.7.1/setup.py`

 * *Files identical despite different names*

