# Comparing `tmp/opal-client-0.7.1.tar.gz` & `tmp/opal-client-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opal-client-0.7.1.tar", last modified: Tue Jun 20 13:40:52 2023, max compression
+gzip compressed data, was "opal-client-0.7.2.tar", last modified: Tue Jun 20 15:19:31 2023, max compression
```

## Comparing `opal-client-0.7.1.tar` & `opal-client-0.7.2.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 13:40:52.394622 opal-client-0.7.1/
--rw-r--r--   0 roekatz    (501) staff       (20)     9040 2023-06-20 13:40:52.394277 opal-client-0.7.1/PKG-INFO
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 13:40:52.376216 opal-client-0.7.1/opal_client/
--rw-r--r--   0 roekatz    (501) staff       (20)       31 2022-12-08 13:40:17.000000 opal-client-0.7.1/opal_client/__init__.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 13:40:52.379836 opal-client-0.7.1/opal_client/callbacks/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-client-0.7.1/opal_client/callbacks/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     3034 2022-12-08 13:40:17.000000 opal-client-0.7.1/opal_client/callbacks/api.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4329 2023-04-18 15:25:03.000000 opal-client-0.7.1/opal_client/callbacks/register.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2960 2023-05-29 10:10:14.000000 opal-client-0.7.1/opal_client/callbacks/reporter.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2213 2023-05-29 10:10:14.000000 opal-client-0.7.1/opal_client/cli.py
--rw-r--r--   0 roekatz    (501) staff       (20)    20027 2023-06-03 11:34:06.000000 opal-client-0.7.1/opal_client/client.py
--rw-r--r--   0 roekatz    (501) staff       (20)    11947 2023-06-03 11:34:06.000000 opal-client-0.7.1/opal_client/config.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 13:40:52.382804 opal-client-0.7.1/opal_client/data/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-client-0.7.1/opal_client/data/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)      863 2022-12-08 13:40:17.000000 opal-client-0.7.1/opal_client/data/api.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4286 2023-05-09 07:59:18.000000 opal-client-0.7.1/opal_client/data/fetcher.py
--rw-r--r--   0 roekatz    (501) staff       (20)      842 2022-12-08 13:40:17.000000 opal-client-0.7.1/opal_client/data/rpc.py
--rw-r--r--   0 roekatz    (501) staff       (20)    20126 2023-05-29 10:10:14.000000 opal-client-0.7.1/opal_client/data/updater.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 13:40:52.384943 opal-client-0.7.1/opal_client/engine/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2023-05-29 10:10:14.000000 opal-client-0.7.1/opal_client/engine/__init__.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 13:40:52.385633 opal-client-0.7.1/opal_client/engine/healthcheck/
--rw-r--r--   0 roekatz    (501) staff       (20)     1123 2023-05-29 10:10:14.000000 opal-client-0.7.1/opal_client/engine/healthcheck/opal.rego
--rw-r--r--   0 roekatz    (501) staff       (20)     3517 2023-05-29 10:10:14.000000 opal-client-0.7.1/opal_client/engine/logger.py
--rw-r--r--   0 roekatz    (501) staff       (20)     5702 2023-05-29 10:10:14.000000 opal-client-0.7.1/opal_client/engine/options.py
--rw-r--r--   0 roekatz    (501) staff       (20)    10724 2023-05-29 10:10:14.000000 opal-client-0.7.1/opal_client/engine/runner.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2220 2022-12-08 13:40:17.000000 opal-client-0.7.1/opal_client/limiter.py
--rw-r--r--   0 roekatz    (501) staff       (20)       33 2022-12-08 13:40:17.000000 opal-client-0.7.1/opal_client/logger.py
--rw-r--r--   0 roekatz    (501) staff       (20)       96 2022-12-08 13:40:17.000000 opal-client-0.7.1/opal_client/main.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 13:40:52.387080 opal-client-0.7.1/opal_client/policy/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-client-0.7.1/opal_client/policy/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)      501 2022-12-08 13:40:17.000000 opal-client-0.7.1/opal_client/policy/api.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4968 2023-05-29 10:10:14.000000 opal-client-0.7.1/opal_client/policy/fetcher.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1797 2023-05-29 10:10:14.000000 opal-client-0.7.1/opal_client/policy/options.py
--rw-r--r--   0 roekatz    (501) staff       (20)      596 2022-12-08 13:40:17.000000 opal-client-0.7.1/opal_client/policy/topics.py
--rw-r--r--   0 roekatz    (501) staff       (20)    13450 2023-05-29 10:10:14.000000 opal-client-0.7.1/opal_client/policy/updater.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 13:40:52.390563 opal-client-0.7.1/opal_client/policy_store/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-client-0.7.1/opal_client/policy_store/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1650 2023-05-29 10:10:14.000000 opal-client-0.7.1/opal_client/policy_store/api.py
--rw-r--r--   0 roekatz    (501) staff       (20)     8442 2023-05-29 10:10:14.000000 opal-client-0.7.1/opal_client/policy_store/base_policy_store_client.py
--rw-r--r--   0 roekatz    (501) staff       (20)    12318 2023-05-29 10:10:14.000000 opal-client-0.7.1/opal_client/policy_store/cedar_client.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2352 2023-05-29 10:10:14.000000 opal-client-0.7.1/opal_client/policy_store/mock_policy_store_client.py
--rw-r--r--   0 roekatz    (501) staff       (20)    34604 2023-06-19 14:15:56.000000 opal-client-0.7.1/opal_client/policy_store/opa_client.py
--rw-r--r--   0 roekatz    (501) staff       (20)     6605 2023-06-03 11:34:06.000000 opal-client-0.7.1/opal_client/policy_store/policy_store_client_factory.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1831 2023-05-29 10:10:14.000000 opal-client-0.7.1/opal_client/policy_store/schemas.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 13:40:52.393654 opal-client-0.7.1/opal_client/tests/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-client-0.7.1/opal_client/tests/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     7279 2023-05-29 10:10:14.000000 opal-client-0.7.1/opal_client/tests/data_updater_test.py
--rw-r--r--   0 roekatz    (501) staff       (20)     3974 2023-05-29 10:10:14.000000 opal-client-0.7.1/opal_client/tests/opa_client_test.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4415 2023-05-29 10:10:14.000000 opal-client-0.7.1/opal_client/tests/server_to_client_intergation_test.py
--rw-r--r--   0 roekatz    (501) staff       (20)      322 2022-12-08 13:40:17.000000 opal-client-0.7.1/opal_client/utils.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 13:40:52.378362 opal-client-0.7.1/opal_client.egg-info/
--rw-r--r--   0 roekatz    (501) staff       (20)     9040 2023-06-20 13:40:52.000000 opal-client-0.7.1/opal_client.egg-info/PKG-INFO
--rw-r--r--   0 roekatz    (501) staff       (20)     1501 2023-06-20 13:40:52.000000 opal-client-0.7.1/opal_client.egg-info/SOURCES.txt
--rw-r--r--   0 roekatz    (501) staff       (20)        1 2023-06-20 13:40:52.000000 opal-client-0.7.1/opal_client.egg-info/dependency_links.txt
--rw-r--r--   0 roekatz    (501) staff       (20)       52 2023-06-20 13:40:52.000000 opal-client-0.7.1/opal_client.egg-info/entry_points.txt
--rw-r--r--   0 roekatz    (501) staff       (20)      436 2023-06-20 13:40:52.000000 opal-client-0.7.1/opal_client.egg-info/requires.txt
--rw-r--r--   0 roekatz    (501) staff       (20)       12 2023-06-20 13:40:52.000000 opal-client-0.7.1/opal_client.egg-info/top_level.txt
--rw-r--r--   0 roekatz    (501) staff       (20)       38 2023-06-20 13:40:52.396659 opal-client-0.7.1/setup.cfg
--rw-r--r--   0 roekatz    (501) staff       (20)     2834 2023-05-29 10:10:14.000000 opal-client-0.7.1/setup.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 15:19:31.515220 opal-client-0.7.2/
+-rw-r--r--   0 roekatz    (501) staff       (20)     9040 2023-06-20 15:19:31.515009 opal-client-0.7.2/PKG-INFO
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 15:19:31.503329 opal-client-0.7.2/opal_client/
+-rw-r--r--   0 roekatz    (501) staff       (20)       31 2022-12-08 13:40:17.000000 opal-client-0.7.2/opal_client/__init__.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 15:19:31.507553 opal-client-0.7.2/opal_client/callbacks/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-client-0.7.2/opal_client/callbacks/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     3034 2022-12-08 13:40:17.000000 opal-client-0.7.2/opal_client/callbacks/api.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4329 2023-04-18 15:25:03.000000 opal-client-0.7.2/opal_client/callbacks/register.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2960 2023-05-29 10:10:14.000000 opal-client-0.7.2/opal_client/callbacks/reporter.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2213 2023-05-29 10:10:14.000000 opal-client-0.7.2/opal_client/cli.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    20027 2023-06-03 11:34:06.000000 opal-client-0.7.2/opal_client/client.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    11947 2023-06-03 11:34:06.000000 opal-client-0.7.2/opal_client/config.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 15:19:31.508716 opal-client-0.7.2/opal_client/data/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-client-0.7.2/opal_client/data/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      863 2022-12-08 13:40:17.000000 opal-client-0.7.2/opal_client/data/api.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4286 2023-05-09 07:59:18.000000 opal-client-0.7.2/opal_client/data/fetcher.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      842 2022-12-08 13:40:17.000000 opal-client-0.7.2/opal_client/data/rpc.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    20126 2023-05-29 10:10:14.000000 opal-client-0.7.2/opal_client/data/updater.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 15:19:31.509811 opal-client-0.7.2/opal_client/engine/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2023-05-29 10:10:14.000000 opal-client-0.7.2/opal_client/engine/__init__.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 15:19:31.510037 opal-client-0.7.2/opal_client/engine/healthcheck/
+-rw-r--r--   0 roekatz    (501) staff       (20)     1123 2023-05-29 10:10:14.000000 opal-client-0.7.2/opal_client/engine/healthcheck/opal.rego
+-rw-r--r--   0 roekatz    (501) staff       (20)     3517 2023-05-29 10:10:14.000000 opal-client-0.7.2/opal_client/engine/logger.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     5702 2023-05-29 10:10:14.000000 opal-client-0.7.2/opal_client/engine/options.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    10724 2023-05-29 10:10:14.000000 opal-client-0.7.2/opal_client/engine/runner.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2220 2022-12-08 13:40:17.000000 opal-client-0.7.2/opal_client/limiter.py
+-rw-r--r--   0 roekatz    (501) staff       (20)       33 2022-12-08 13:40:17.000000 opal-client-0.7.2/opal_client/logger.py
+-rw-r--r--   0 roekatz    (501) staff       (20)       96 2022-12-08 13:40:17.000000 opal-client-0.7.2/opal_client/main.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 15:19:31.511232 opal-client-0.7.2/opal_client/policy/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-client-0.7.2/opal_client/policy/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      501 2022-12-08 13:40:17.000000 opal-client-0.7.2/opal_client/policy/api.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4968 2023-05-29 10:10:14.000000 opal-client-0.7.2/opal_client/policy/fetcher.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1797 2023-05-29 10:10:14.000000 opal-client-0.7.2/opal_client/policy/options.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      596 2022-12-08 13:40:17.000000 opal-client-0.7.2/opal_client/policy/topics.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    13450 2023-05-29 10:10:14.000000 opal-client-0.7.2/opal_client/policy/updater.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 15:19:31.513845 opal-client-0.7.2/opal_client/policy_store/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-client-0.7.2/opal_client/policy_store/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1650 2023-05-29 10:10:14.000000 opal-client-0.7.2/opal_client/policy_store/api.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     8442 2023-05-29 10:10:14.000000 opal-client-0.7.2/opal_client/policy_store/base_policy_store_client.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    12318 2023-05-29 10:10:14.000000 opal-client-0.7.2/opal_client/policy_store/cedar_client.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2352 2023-05-29 10:10:14.000000 opal-client-0.7.2/opal_client/policy_store/mock_policy_store_client.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    34604 2023-06-19 14:15:56.000000 opal-client-0.7.2/opal_client/policy_store/opa_client.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     6605 2023-06-03 11:34:06.000000 opal-client-0.7.2/opal_client/policy_store/policy_store_client_factory.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1831 2023-05-29 10:10:14.000000 opal-client-0.7.2/opal_client/policy_store/schemas.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 15:19:31.514706 opal-client-0.7.2/opal_client/tests/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-client-0.7.2/opal_client/tests/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     7279 2023-05-29 10:10:14.000000 opal-client-0.7.2/opal_client/tests/data_updater_test.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     3974 2023-05-29 10:10:14.000000 opal-client-0.7.2/opal_client/tests/opa_client_test.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4415 2023-05-29 10:10:14.000000 opal-client-0.7.2/opal_client/tests/server_to_client_intergation_test.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      322 2022-12-08 13:40:17.000000 opal-client-0.7.2/opal_client/utils.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 15:19:31.506662 opal-client-0.7.2/opal_client.egg-info/
+-rw-r--r--   0 roekatz    (501) staff       (20)     9040 2023-06-20 15:19:31.000000 opal-client-0.7.2/opal_client.egg-info/PKG-INFO
+-rw-r--r--   0 roekatz    (501) staff       (20)     1501 2023-06-20 15:19:31.000000 opal-client-0.7.2/opal_client.egg-info/SOURCES.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)        1 2023-06-20 15:19:31.000000 opal-client-0.7.2/opal_client.egg-info/dependency_links.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)       52 2023-06-20 15:19:31.000000 opal-client-0.7.2/opal_client.egg-info/entry_points.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)      436 2023-06-20 15:19:31.000000 opal-client-0.7.2/opal_client.egg-info/requires.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)       12 2023-06-20 15:19:31.000000 opal-client-0.7.2/opal_client.egg-info/top_level.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)       38 2023-06-20 15:19:31.515272 opal-client-0.7.2/setup.cfg
+-rw-r--r--   0 roekatz    (501) staff       (20)     2834 2023-05-29 10:10:14.000000 opal-client-0.7.2/setup.py
```

### Comparing `opal-client-0.7.1/PKG-INFO` & `opal-client-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opal-client
-Version: 0.7.1
+Version: 0.7.2
 Summary: OPAL is an administration layer for Open Policy Agent (OPA), detecting changes to both policy and data and pushing live updates to your agents. The opal-client is deployed alongside a policy-store (e.g: OPA), keeping it up-to-date, by connecting to an opal-server and subscribing to pub/sub updates for policy and policy data changes.
 Home-page: https://github.com/permitio/opal
 Author: Or Weis, Asaf Cohen
 Author-email: or@permit.io
 License: Apache 2.0
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: opal-client Version: 0.7.1 Summary: OPAL is an
+Metadata-Version: 2.1 Name: opal-client Version: 0.7.2 Summary: OPAL is an
 administration layer for Open Policy Agent (OPA), detecting changes to both
 policy and data and pushing live updates to your agents. The opal-client is
 deployed alongside a policy-store (e.g: OPA), keeping it up-to-date, by
 connecting to an opal-server and subscribing to pub/sub updates for policy and
 policy data changes. Home-page: https://github.com/permitio/opal Author: Or
 Weis, Asaf Cohen Author-email: or@permit.io License: Apache 2.0 Classifier:
 Operating System :: OS Independent Classifier: License :: OSI Approved ::
```

### Comparing `opal-client-0.7.1/opal_client/callbacks/api.py` & `opal-client-0.7.2/opal_client/callbacks/api.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.1/opal_client/callbacks/register.py` & `opal-client-0.7.2/opal_client/callbacks/register.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.1/opal_client/callbacks/reporter.py` & `opal-client-0.7.2/opal_client/callbacks/reporter.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.1/opal_client/cli.py` & `opal-client-0.7.2/opal_client/cli.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.1/opal_client/client.py` & `opal-client-0.7.2/opal_client/client.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.1/opal_client/config.py` & `opal-client-0.7.2/opal_client/config.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.1/opal_client/data/api.py` & `opal-client-0.7.2/opal_client/data/api.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.1/opal_client/data/fetcher.py` & `opal-client-0.7.2/opal_client/data/fetcher.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.1/opal_client/data/rpc.py` & `opal-client-0.7.2/opal_client/data/rpc.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.1/opal_client/data/updater.py` & `opal-client-0.7.2/opal_client/data/updater.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.1/opal_client/engine/healthcheck/opal.rego` & `opal-client-0.7.2/opal_client/engine/healthcheck/opal.rego`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.1/opal_client/engine/logger.py` & `opal-client-0.7.2/opal_client/engine/logger.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.1/opal_client/engine/options.py` & `opal-client-0.7.2/opal_client/engine/options.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.1/opal_client/engine/runner.py` & `opal-client-0.7.2/opal_client/engine/runner.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.1/opal_client/limiter.py` & `opal-client-0.7.2/opal_client/limiter.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.1/opal_client/policy/fetcher.py` & `opal-client-0.7.2/opal_client/policy/fetcher.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.1/opal_client/policy/options.py` & `opal-client-0.7.2/opal_client/policy/options.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.1/opal_client/policy/topics.py` & `opal-client-0.7.2/opal_client/policy/topics.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.1/opal_client/policy/updater.py` & `opal-client-0.7.2/opal_client/policy/updater.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.1/opal_client/policy_store/api.py` & `opal-client-0.7.2/opal_client/policy_store/api.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.1/opal_client/policy_store/base_policy_store_client.py` & `opal-client-0.7.2/opal_client/policy_store/base_policy_store_client.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.1/opal_client/policy_store/cedar_client.py` & `opal-client-0.7.2/opal_client/policy_store/cedar_client.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.1/opal_client/policy_store/mock_policy_store_client.py` & `opal-client-0.7.2/opal_client/policy_store/mock_policy_store_client.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.1/opal_client/policy_store/opa_client.py` & `opal-client-0.7.2/opal_client/policy_store/opa_client.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.1/opal_client/policy_store/policy_store_client_factory.py` & `opal-client-0.7.2/opal_client/policy_store/policy_store_client_factory.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.1/opal_client/policy_store/schemas.py` & `opal-client-0.7.2/opal_client/policy_store/schemas.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.1/opal_client/tests/data_updater_test.py` & `opal-client-0.7.2/opal_client/tests/data_updater_test.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.1/opal_client/tests/opa_client_test.py` & `opal-client-0.7.2/opal_client/tests/opa_client_test.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.1/opal_client/tests/server_to_client_intergation_test.py` & `opal-client-0.7.2/opal_client/tests/server_to_client_intergation_test.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.1/opal_client.egg-info/PKG-INFO` & `opal-client-0.7.2/opal_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opal-client
-Version: 0.7.1
+Version: 0.7.2
 Summary: OPAL is an administration layer for Open Policy Agent (OPA), detecting changes to both policy and data and pushing live updates to your agents. The opal-client is deployed alongside a policy-store (e.g: OPA), keeping it up-to-date, by connecting to an opal-server and subscribing to pub/sub updates for policy and policy data changes.
 Home-page: https://github.com/permitio/opal
 Author: Or Weis, Asaf Cohen
 Author-email: or@permit.io
 License: Apache 2.0
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: opal-client Version: 0.7.1 Summary: OPAL is an
+Metadata-Version: 2.1 Name: opal-client Version: 0.7.2 Summary: OPAL is an
 administration layer for Open Policy Agent (OPA), detecting changes to both
 policy and data and pushing live updates to your agents. The opal-client is
 deployed alongside a policy-store (e.g: OPA), keeping it up-to-date, by
 connecting to an opal-server and subscribing to pub/sub updates for policy and
 policy data changes. Home-page: https://github.com/permitio/opal Author: Or
 Weis, Asaf Cohen Author-email: or@permit.io License: Apache 2.0 Classifier:
 Operating System :: OS Independent Classifier: License :: OSI Approved ::
```

### Comparing `opal-client-0.7.1/opal_client.egg-info/SOURCES.txt` & `opal-client-0.7.2/opal_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opal-client-0.7.1/setup.py` & `opal-client-0.7.2/setup.py`

 * *Files identical despite different names*

