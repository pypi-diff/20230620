# Comparing `tmp/opal-common-0.7.0.tar.gz` & `tmp/opal-common-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opal-common-0.7.0.tar", last modified: Wed May 10 19:01:52 2023, max compression
+gzip compressed data, was "opal-common-0.7.1.tar", last modified: Tue Jun 20 13:40:51 2023, max compression
```

## Comparing `opal-common-0.7.0.tar` & `opal-common-0.7.1.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.319177 opal-common-0.7.0/
--rw-r--r--   0 asafc      (501) staff       (20)     8348 2023-05-10 19:01:52.318951 opal-common-0.7.0/PKG-INFO
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.309658 opal-common-0.7.0/opal_common/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)      797 2022-10-11 10:23:16.000000 opal-common-0.7.0/opal_common/async_utils.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.311000 opal-common-0.7.0/opal_common/authentication/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/authentication/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     1477 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/authentication/authz.py
--rw-r--r--   0 asafc      (501) staff       (20)     3267 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/authentication/casting.py
--rw-r--r--   0 asafc      (501) staff       (20)     5016 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/authentication/deps.py
--rw-r--r--   0 asafc      (501) staff       (20)     4669 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/authentication/signer.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.311211 opal-common-0.7.0/opal_common/authentication/tests/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/authentication/tests/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)    17336 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/authentication/tests/jwt_signer_test.py
--rw-r--r--   0 asafc      (501) staff       (20)      958 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/authentication/types.py
--rw-r--r--   0 asafc      (501) staff       (20)     4225 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/authentication/verifier.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.311659 opal-common-0.7.0/opal_common/cli/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/cli/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     6657 2023-05-10 06:45:11.000000 opal-common-0.7.0/opal_common/cli/commands.py
--rw-r--r--   0 asafc      (501) staff       (20)      703 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/cli/docs.py
--rw-r--r--   0 asafc      (501) staff       (20)      167 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/cli/typer_app.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.312085 opal-common-0.7.0/opal_common/confi/
--rw-r--r--   0 asafc      (501) staff       (20)       21 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/confi/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     2278 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/confi/cli.py
--rw-r--r--   0 asafc      (501) staff       (20)    13780 2023-05-10 06:45:11.000000 opal-common-0.7.0/opal_common/confi/confi.py
--rw-r--r--   0 asafc      (501) staff       (20)     2719 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/confi/types.py
--rw-r--r--   0 asafc      (501) staff       (20)     6831 2023-05-10 17:44:40.000000 opal-common-0.7.0/opal_common/config.py
--rw-r--r--   0 asafc      (501) staff       (20)     1492 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/corn_utils.py
--rw-r--r--   0 asafc      (501) staff       (20)     6050 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/emport.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.312413 opal-common-0.7.0/opal_common/engine/
--rw-r--r--   0 asafc      (501) staff       (20)       90 2023-05-10 17:44:40.000000 opal-common-0.7.0/opal_common/engine/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)      576 2023-05-10 17:44:40.000000 opal-common-0.7.0/opal_common/engine/parsing.py
--rw-r--r--   0 asafc      (501) staff       (20)      593 2023-05-10 17:44:40.000000 opal-common-0.7.0/opal_common/engine/paths.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.312968 opal-common-0.7.0/opal_common/fetcher/
--rw-r--r--   0 asafc      (501) staff       (20)      143 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/fetcher/__init__.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.313480 opal-common-0.7.0/opal_common/fetcher/engine/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/fetcher/engine/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     2653 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/fetcher/engine/base_fetching_engine.py
--rw-r--r--   0 asafc      (501) staff       (20)      296 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/fetcher/engine/core_callbacks.py
--rw-r--r--   0 asafc      (501) staff       (20)     1536 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/fetcher/engine/fetch_worker.py
--rw-r--r--   0 asafc      (501) staff       (20)     8485 2023-05-10 06:45:11.000000 opal-common-0.7.0/opal_common/fetcher/engine/fetching_engine.py
--rw-r--r--   0 asafc      (501) staff       (20)     1191 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/fetcher/events.py
--rw-r--r--   0 asafc      (501) staff       (20)     2548 2023-05-10 06:45:11.000000 opal-common-0.7.0/opal_common/fetcher/fetch_provider.py
--rw-r--r--   0 asafc      (501) staff       (20)     3030 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/fetcher/fetcher_register.py
--rw-r--r--   0 asafc      (501) staff       (20)      116 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/fetcher/logger.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.313832 opal-common-0.7.0/opal_common/fetcher/providers/
--rw-r--r--   0 asafc      (501) staff       (20)       67 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/fetcher/providers/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     1710 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/fetcher/providers/fastapi_rpc_fetch_provider.py
--rw-r--r--   0 asafc      (501) staff       (20)     3525 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/fetcher/providers/http_fetch_provider.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.314236 opal-common-0.7.0/opal_common/fetcher/tests/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/fetcher/tests/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     1917 2023-05-10 06:45:11.000000 opal-common-0.7.0/opal_common/fetcher/tests/failure_handler_test.py
--rw-r--r--   0 asafc      (501) staff       (20)     4291 2023-05-10 17:44:36.000000 opal-common-0.7.0/opal_common/fetcher/tests/http_fetch_test.py
--rw-r--r--   0 asafc      (501) staff       (20)     2140 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/fetcher/tests/rpc_fetch_test.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.315286 opal-common-0.7.0/opal_common/git/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/git/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     5461 2023-02-01 11:46:28.000000 opal-common-0.7.0/opal_common/git/branch_tracker.py
--rw-r--r--   0 asafc      (501) staff       (20)    15557 2023-05-10 17:44:40.000000 opal-common-0.7.0/opal_common/git/bundle_maker.py
--rw-r--r--   0 asafc      (501) staff       (20)     1887 2023-05-10 06:45:11.000000 opal-common-0.7.0/opal_common/git/bundle_utils.py
--rw-r--r--   0 asafc      (501) staff       (20)     8684 2023-05-10 06:45:11.000000 opal-common-0.7.0/opal_common/git/commit_viewer.py
--rw-r--r--   0 asafc      (501) staff       (20)     7948 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/git/diff_viewer.py
--rw-r--r--   0 asafc      (501) staff       (20)     1580 2023-02-01 11:46:28.000000 opal-common-0.7.0/opal_common/git/env.py
--rw-r--r--   0 asafc      (501) staff       (20)      299 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/git/exceptions.py
--rw-r--r--   0 asafc      (501) staff       (20)     8535 2023-05-10 06:45:11.000000 opal-common-0.7.0/opal_common/git/repo_cloner.py
--rw-r--r--   0 asafc      (501) staff       (20)     4237 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/git/tar_file_to_local_git_extractor.py
--rw-r--r--   0 asafc      (501) staff       (20)      182 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/http.py
--rw-r--r--   0 asafc      (501) staff       (20)     1832 2023-05-10 06:45:11.000000 opal-common-0.7.0/opal_common/logger.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.315895 opal-common-0.7.0/opal_common/logging/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/logging/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)      412 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/logging/decorators.py
--rw-r--r--   0 asafc      (501) staff       (20)     1166 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/logging/filter.py
--rw-r--r--   0 asafc      (501) staff       (20)      617 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/logging/formatter.py
--rw-r--r--   0 asafc      (501) staff       (20)      700 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/logging/intercept.py
--rw-r--r--   0 asafc      (501) staff       (20)     1355 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/logging/thirdparty.py
--rw-r--r--   0 asafc      (501) staff       (20)     3520 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/middleware.py
--rw-r--r--   0 asafc      (501) staff       (20)     4067 2023-05-10 06:45:11.000000 opal-common-0.7.0/opal_common/paths.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.316740 opal-common-0.7.0/opal_common/schemas/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/schemas/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     6313 2023-05-10 06:45:11.000000 opal-common-0.7.0/opal_common/schemas/data.py
--rw-r--r--   0 asafc      (501) staff       (20)     1387 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/schemas/policy.py
--rw-r--r--   0 asafc      (501) staff       (20)     1767 2023-02-24 20:59:56.000000 opal-common-0.7.0/opal_common/schemas/policy_source.py
--rw-r--r--   0 asafc      (501) staff       (20)      508 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/schemas/scopes.py
--rw-r--r--   0 asafc      (501) staff       (20)     1573 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/schemas/security.py
--rw-r--r--   0 asafc      (501) staff       (20)     2003 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/schemas/store.py
--rw-r--r--   0 asafc      (501) staff       (20)     1438 2023-05-10 06:45:11.000000 opal-common-0.7.0/opal_common/schemas/webhook.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.317101 opal-common-0.7.0/opal_common/security/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/security/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)      799 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/security/sslcontext.py
--rw-r--r--   0 asafc      (501) staff       (20)     3294 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/security/tarsafe.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.317589 opal-common-0.7.0/opal_common/sources/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/sources/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     9414 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/sources/api_policy_source.py
--rw-r--r--   0 asafc      (501) staff       (20)     4283 2023-05-10 06:45:11.000000 opal-common-0.7.0/opal_common/sources/base_policy_source.py
--rw-r--r--   0 asafc      (501) staff       (20)     4238 2023-05-10 06:45:11.000000 opal-common-0.7.0/opal_common/sources/git_policy_source.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.317950 opal-common-0.7.0/opal_common/synchronization/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/synchronization/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     1294 2023-02-01 11:46:28.000000 opal-common-0.7.0/opal_common/synchronization/expiring_redis_lock.py
--rw-r--r--   0 asafc      (501) staff       (20)     2990 2023-05-10 06:45:11.000000 opal-common-0.7.0/opal_common/synchronization/named_lock.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.318272 opal-common-0.7.0/opal_common/tests/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/tests/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     9622 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/tests/path_utils_test.py
--rw-r--r--   0 asafc      (501) staff       (20)     1223 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/tests/url_utils_test.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.318728 opal-common-0.7.0/opal_common/topics/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/topics/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     2371 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/topics/listener.py
--rw-r--r--   0 asafc      (501) staff       (20)     6517 2023-05-10 06:45:11.000000 opal-common-0.7.0/opal_common/topics/publisher.py
--rw-r--r--   0 asafc      (501) staff       (20)     1054 2023-05-10 06:45:11.000000 opal-common-0.7.0/opal_common/topics/utils.py
--rw-r--r--   0 asafc      (501) staff       (20)      988 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/urls.py
--rw-r--r--   0 asafc      (501) staff       (20)     5917 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/utils.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.310246 opal-common-0.7.0/opal_common.egg-info/
--rw-r--r--   0 asafc      (501) staff       (20)     8348 2023-05-10 19:01:52.000000 opal-common-0.7.0/opal_common.egg-info/PKG-INFO
--rw-r--r--   0 asafc      (501) staff       (20)     3207 2023-05-10 19:01:52.000000 opal-common-0.7.0/opal_common.egg-info/SOURCES.txt
--rw-r--r--   0 asafc      (501) staff       (20)        1 2023-05-10 19:01:52.000000 opal-common-0.7.0/opal_common.egg-info/dependency_links.txt
--rw-r--r--   0 asafc      (501) staff       (20)      471 2023-05-10 19:01:52.000000 opal-common-0.7.0/opal_common.egg-info/requires.txt
--rw-r--r--   0 asafc      (501) staff       (20)       12 2023-05-10 19:01:52.000000 opal-common-0.7.0/opal_common.egg-info/top_level.txt
--rw-r--r--   0 asafc      (501) staff       (20)       38 2023-05-10 19:01:52.319215 opal-common-0.7.0/setup.cfg
--rw-r--r--   0 asafc      (501) staff       (20)     2601 2022-10-01 21:13:25.000000 opal-common-0.7.0/setup.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 13:40:51.786460 opal-common-0.7.1/
+-rw-r--r--   0 roekatz    (501) staff       (20)     8924 2023-06-20 13:40:51.785072 opal-common-0.7.1/PKG-INFO
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 13:40:51.756429 opal-common-0.7.1/opal_common/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      797 2023-05-09 07:59:18.000000 opal-common-0.7.1/opal_common/async_utils.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 13:40:51.761371 opal-common-0.7.1/opal_common/authentication/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/authentication/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1477 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/authentication/authz.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     3267 2023-05-09 07:59:18.000000 opal-common-0.7.1/opal_common/authentication/casting.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     5016 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/authentication/deps.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4669 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/authentication/signer.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 13:40:51.761822 opal-common-0.7.1/opal_common/authentication/tests/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/authentication/tests/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    17336 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/authentication/tests/jwt_signer_test.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      958 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/authentication/types.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4225 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/authentication/verifier.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 13:40:51.763223 opal-common-0.7.1/opal_common/cli/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/cli/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     6657 2023-05-29 10:10:14.000000 opal-common-0.7.1/opal_common/cli/commands.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      703 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/cli/docs.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      167 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/cli/typer_app.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 13:40:51.764860 opal-common-0.7.1/opal_common/confi/
+-rw-r--r--   0 roekatz    (501) staff       (20)       21 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/confi/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2278 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/confi/cli.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    13780 2023-05-29 10:10:14.000000 opal-common-0.7.1/opal_common/confi/confi.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2719 2023-04-18 15:25:03.000000 opal-common-0.7.1/opal_common/confi/types.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     6831 2023-05-29 10:10:14.000000 opal-common-0.7.1/opal_common/config.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1492 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/corn_utils.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     6050 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/emport.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 13:40:51.766164 opal-common-0.7.1/opal_common/engine/
+-rw-r--r--   0 roekatz    (501) staff       (20)       90 2023-05-29 10:10:14.000000 opal-common-0.7.1/opal_common/engine/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      576 2023-05-29 10:10:14.000000 opal-common-0.7.1/opal_common/engine/parsing.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      593 2023-05-29 10:10:14.000000 opal-common-0.7.1/opal_common/engine/paths.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 13:40:51.768152 opal-common-0.7.1/opal_common/fetcher/
+-rw-r--r--   0 roekatz    (501) staff       (20)      143 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/fetcher/__init__.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 13:40:51.769154 opal-common-0.7.1/opal_common/fetcher/engine/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/fetcher/engine/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2653 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/fetcher/engine/base_fetching_engine.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      296 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/fetcher/engine/core_callbacks.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1536 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/fetcher/engine/fetch_worker.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     8485 2023-05-29 10:10:14.000000 opal-common-0.7.1/opal_common/fetcher/engine/fetching_engine.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1191 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/fetcher/events.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2548 2023-05-29 10:10:14.000000 opal-common-0.7.1/opal_common/fetcher/fetch_provider.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     3030 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/fetcher/fetcher_register.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      116 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/fetcher/logger.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 13:40:51.771615 opal-common-0.7.1/opal_common/fetcher/providers/
+-rw-r--r--   0 roekatz    (501) staff       (20)       67 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/fetcher/providers/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1710 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/fetcher/providers/fastapi_rpc_fetch_provider.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     3525 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/fetcher/providers/http_fetch_provider.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 13:40:51.772430 opal-common-0.7.1/opal_common/fetcher/tests/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/fetcher/tests/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1917 2023-05-29 10:10:14.000000 opal-common-0.7.1/opal_common/fetcher/tests/failure_handler_test.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4291 2023-05-29 10:10:14.000000 opal-common-0.7.1/opal_common/fetcher/tests/http_fetch_test.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2140 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/fetcher/tests/rpc_fetch_test.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 13:40:51.775132 opal-common-0.7.1/opal_common/git/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/git/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     5461 2023-05-29 10:10:14.000000 opal-common-0.7.1/opal_common/git/branch_tracker.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    15557 2023-05-29 10:10:14.000000 opal-common-0.7.1/opal_common/git/bundle_maker.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1887 2023-05-29 10:10:14.000000 opal-common-0.7.1/opal_common/git/bundle_utils.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     8684 2023-05-29 10:10:14.000000 opal-common-0.7.1/opal_common/git/commit_viewer.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     7948 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/git/diff_viewer.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1580 2023-05-29 10:10:14.000000 opal-common-0.7.1/opal_common/git/env.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      299 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/git/exceptions.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     8535 2023-05-29 10:10:14.000000 opal-common-0.7.1/opal_common/git/repo_cloner.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4237 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/git/tar_file_to_local_git_extractor.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      182 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/http.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1832 2023-05-29 10:10:14.000000 opal-common-0.7.1/opal_common/logger.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 13:40:51.776128 opal-common-0.7.1/opal_common/logging/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/logging/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      412 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/logging/decorators.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1166 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/logging/filter.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      617 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/logging/formatter.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      700 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/logging/intercept.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1355 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/logging/thirdparty.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     3520 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/middleware.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4067 2023-05-29 10:10:14.000000 opal-common-0.7.1/opal_common/paths.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 13:40:51.777772 opal-common-0.7.1/opal_common/schemas/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/schemas/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     6313 2023-05-29 10:10:14.000000 opal-common-0.7.1/opal_common/schemas/data.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1387 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/schemas/policy.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1767 2023-05-29 10:10:14.000000 opal-common-0.7.1/opal_common/schemas/policy_source.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      508 2023-04-04 11:14:44.000000 opal-common-0.7.1/opal_common/schemas/scopes.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1573 2023-05-23 16:26:33.000000 opal-common-0.7.1/opal_common/schemas/security.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2003 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/schemas/store.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1438 2023-05-29 10:10:14.000000 opal-common-0.7.1/opal_common/schemas/webhook.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 13:40:51.780428 opal-common-0.7.1/opal_common/security/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/security/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      799 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/security/sslcontext.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     3294 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/security/tarsafe.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 13:40:51.781791 opal-common-0.7.1/opal_common/sources/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/sources/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    11067 2023-06-03 11:34:06.000000 opal-common-0.7.1/opal_common/sources/api_policy_source.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4283 2023-05-29 10:10:14.000000 opal-common-0.7.1/opal_common/sources/base_policy_source.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4238 2023-05-29 10:10:14.000000 opal-common-0.7.1/opal_common/sources/git_policy_source.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 13:40:51.782277 opal-common-0.7.1/opal_common/synchronization/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/synchronization/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1294 2023-05-29 10:10:14.000000 opal-common-0.7.1/opal_common/synchronization/expiring_redis_lock.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2990 2023-05-29 10:10:14.000000 opal-common-0.7.1/opal_common/synchronization/named_lock.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 13:40:51.782832 opal-common-0.7.1/opal_common/tests/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/tests/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     9622 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/tests/path_utils_test.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1223 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/tests/url_utils_test.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 13:40:51.784737 opal-common-0.7.1/opal_common/topics/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/topics/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2371 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/topics/listener.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     6728 2023-06-20 13:37:00.000000 opal-common-0.7.1/opal_common/topics/publisher.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1054 2023-05-29 10:10:14.000000 opal-common-0.7.1/opal_common/topics/utils.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      988 2022-12-08 13:40:17.000000 opal-common-0.7.1/opal_common/urls.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     8371 2023-06-03 11:34:06.000000 opal-common-0.7.1/opal_common/utils.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 13:40:51.758950 opal-common-0.7.1/opal_common.egg-info/
+-rw-r--r--   0 roekatz    (501) staff       (20)     8924 2023-06-20 13:40:51.000000 opal-common-0.7.1/opal_common.egg-info/PKG-INFO
+-rw-r--r--   0 roekatz    (501) staff       (20)     3207 2023-06-20 13:40:51.000000 opal-common-0.7.1/opal_common.egg-info/SOURCES.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)        1 2023-06-20 13:40:51.000000 opal-common-0.7.1/opal_common.egg-info/dependency_links.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)      471 2023-06-20 13:40:51.000000 opal-common-0.7.1/opal_common.egg-info/requires.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)       12 2023-06-20 13:40:51.000000 opal-common-0.7.1/opal_common.egg-info/top_level.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)       38 2023-06-20 13:40:51.786647 opal-common-0.7.1/setup.cfg
+-rw-r--r--   0 roekatz    (501) staff       (20)     2601 2022-12-08 13:40:17.000000 opal-common-0.7.1/setup.py
```

### Comparing `opal-common-0.7.0/PKG-INFO` & `opal-common-0.7.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opal-common
-Version: 0.7.0
+Version: 0.7.1
 Summary: OPAL is an administration layer for Open Policy Agent (OPA), detecting changes to both policy and data and pushing live updates to your agents. opal-common contains common code used by both opal-client and opal-server.
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
-Metadata-Version: 2.1 Name: opal-common Version: 0.7.0 Summary: OPAL is an
+Metadata-Version: 2.1 Name: opal-common Version: 0.7.1 Summary: OPAL is an
 administration layer for Open Policy Agent (OPA), detecting changes to both
 policy and data and pushing live updates to your agents. opal-common contains
 common code used by both opal-client and opal-server. Home-page: https://
 github.com/permitio/opal Author: Or Weis, Asaf Cohen Author-email: or@permit.io
 License: Apache 2.0 Classifier: Operating System :: OS Independent Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
@@ -12,43 +12,47 @@
 WWW/HTTP :: WSGI Requires-Python: >=3.7 Description-Content-Type: text/markdown
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
@@ -80,8 +84,9 @@
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

### Comparing `opal-common-0.7.0/opal_common/async_utils.py` & `opal-common-0.7.1/opal_common/async_utils.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/authentication/authz.py` & `opal-common-0.7.1/opal_common/authentication/authz.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/authentication/casting.py` & `opal-common-0.7.1/opal_common/authentication/casting.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/authentication/deps.py` & `opal-common-0.7.1/opal_common/authentication/deps.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/authentication/signer.py` & `opal-common-0.7.1/opal_common/authentication/signer.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/authentication/tests/jwt_signer_test.py` & `opal-common-0.7.1/opal_common/authentication/tests/jwt_signer_test.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/authentication/types.py` & `opal-common-0.7.1/opal_common/authentication/types.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/authentication/verifier.py` & `opal-common-0.7.1/opal_common/authentication/verifier.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/cli/commands.py` & `opal-common-0.7.1/opal_common/cli/commands.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/cli/docs.py` & `opal-common-0.7.1/opal_common/cli/docs.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/confi/cli.py` & `opal-common-0.7.1/opal_common/confi/cli.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/confi/confi.py` & `opal-common-0.7.1/opal_common/confi/confi.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/confi/types.py` & `opal-common-0.7.1/opal_common/confi/types.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/config.py` & `opal-common-0.7.1/opal_common/config.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/corn_utils.py` & `opal-common-0.7.1/opal_common/corn_utils.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/emport.py` & `opal-common-0.7.1/opal_common/emport.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/engine/parsing.py` & `opal-common-0.7.1/opal_common/engine/parsing.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/engine/paths.py` & `opal-common-0.7.1/opal_common/engine/paths.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/fetcher/engine/base_fetching_engine.py` & `opal-common-0.7.1/opal_common/fetcher/engine/base_fetching_engine.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/fetcher/engine/fetch_worker.py` & `opal-common-0.7.1/opal_common/fetcher/engine/fetch_worker.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/fetcher/engine/fetching_engine.py` & `opal-common-0.7.1/opal_common/fetcher/engine/fetching_engine.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/fetcher/events.py` & `opal-common-0.7.1/opal_common/fetcher/events.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/fetcher/fetch_provider.py` & `opal-common-0.7.1/opal_common/fetcher/fetch_provider.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/fetcher/fetcher_register.py` & `opal-common-0.7.1/opal_common/fetcher/fetcher_register.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/fetcher/providers/fastapi_rpc_fetch_provider.py` & `opal-common-0.7.1/opal_common/fetcher/providers/fastapi_rpc_fetch_provider.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/fetcher/providers/http_fetch_provider.py` & `opal-common-0.7.1/opal_common/fetcher/providers/http_fetch_provider.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/fetcher/tests/failure_handler_test.py` & `opal-common-0.7.1/opal_common/fetcher/tests/failure_handler_test.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/fetcher/tests/http_fetch_test.py` & `opal-common-0.7.1/opal_common/fetcher/tests/http_fetch_test.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/fetcher/tests/rpc_fetch_test.py` & `opal-common-0.7.1/opal_common/fetcher/tests/rpc_fetch_test.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/git/branch_tracker.py` & `opal-common-0.7.1/opal_common/git/branch_tracker.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/git/bundle_maker.py` & `opal-common-0.7.1/opal_common/git/bundle_maker.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/git/bundle_utils.py` & `opal-common-0.7.1/opal_common/git/bundle_utils.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/git/commit_viewer.py` & `opal-common-0.7.1/opal_common/git/commit_viewer.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/git/diff_viewer.py` & `opal-common-0.7.1/opal_common/git/diff_viewer.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/git/env.py` & `opal-common-0.7.1/opal_common/git/env.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/git/repo_cloner.py` & `opal-common-0.7.1/opal_common/git/repo_cloner.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/git/tar_file_to_local_git_extractor.py` & `opal-common-0.7.1/opal_common/git/tar_file_to_local_git_extractor.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/logger.py` & `opal-common-0.7.1/opal_common/logger.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/logging/filter.py` & `opal-common-0.7.1/opal_common/logging/filter.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/logging/formatter.py` & `opal-common-0.7.1/opal_common/logging/formatter.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/logging/intercept.py` & `opal-common-0.7.1/opal_common/logging/intercept.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/logging/thirdparty.py` & `opal-common-0.7.1/opal_common/logging/thirdparty.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/middleware.py` & `opal-common-0.7.1/opal_common/middleware.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/paths.py` & `opal-common-0.7.1/opal_common/paths.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/schemas/data.py` & `opal-common-0.7.1/opal_common/schemas/data.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/schemas/policy.py` & `opal-common-0.7.1/opal_common/schemas/policy.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/schemas/policy_source.py` & `opal-common-0.7.1/opal_common/schemas/policy_source.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/schemas/security.py` & `opal-common-0.7.1/opal_common/schemas/security.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/schemas/store.py` & `opal-common-0.7.1/opal_common/schemas/store.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/schemas/webhook.py` & `opal-common-0.7.1/opal_common/schemas/webhook.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/security/sslcontext.py` & `opal-common-0.7.1/opal_common/security/sslcontext.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/security/tarsafe.py` & `opal-common-0.7.1/opal_common/security/tarsafe.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/sources/api_policy_source.py` & `opal-common-0.7.1/opal_common/sources/api_policy_source.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from datetime import datetime
 from pathlib import Path
 from typing import Optional, Tuple
+from urllib.parse import urlparse
 
 import aiohttp
 from fastapi import status
 from fastapi.exceptions import HTTPException
 from opal_common.git.tar_file_to_local_git_extractor import TarFileToLocalGitExtractor
 from opal_common.logger import logger
 from opal_common.sources.base_policy_source import BasePolicySource
 from opal_common.utils import (
+    build_aws_rest_auth_headers,
     get_authorization_header,
     hash_file,
     throw_if_bad_status_code,
     tuple_to_dict,
 )
+from opal_server.config import PolicyBundleServerType
 from tenacity import AsyncRetrying
 from tenacity.wait import wait_fixed
 
 BundleHash = str
 
 
 class ApiPolicySource(BasePolicySource):
@@ -31,32 +34,38 @@
     You can read more on OPA bundles here:
     https://www.openpolicyagent.org/docs/latest/management-bundles/
 
     Args:
         remote_source_url(str): the base address to request the policy from
         local_clone_path(str):  path for the local git to manage policies
         polling_interval(int):  how many seconds need to wait between polling
-        token (str, optional):  auth token to include in connections to OPAL server. Defaults to POLICY_BUNDLE_SERVER_TOKEN.
+        token (str, optional):  auth token to include in connections to bundle server. Defaults to POLICY_BUNDLE_SERVER_TOKEN.
+        token_id (str, optional):  auth token ID to include in connections to bundle server. Defaults to POLICY_BUNDLE_SERVER_TOKEN_ID.
+        bundle_server_type (PolicyBundleServerType, optional):  the type of bundle server
     """
 
     def __init__(
         self,
         remote_source_url: str,
         local_clone_path: str,
         polling_interval: int = 0,
         token: Optional[str] = None,
+        token_id: Optional[str] = None,
+        bundle_server_type: Optional[PolicyBundleServerType] = None,
         policy_bundle_path=".",
         policy_bundle_git_add_pattern="*",
     ):
         super().__init__(
             remote_source_url=remote_source_url,
             local_clone_path=local_clone_path,
             polling_interval=polling_interval,
         )
         self.token = token
+        self.token_id = token_id
+        self.server_type = bundle_server_type
         self.bundle_hash = None
         self.etag = None
         self.tmp_bundle_path = Path(policy_bundle_path)
         self.policy_bundle_git_add_pattern = policy_bundle_git_add_pattern
         self.tar_to_git = TarFileToLocalGitExtractor(
             self.local_clone_path,
             self.tmp_bundle_path,
@@ -87,18 +96,42 @@
                     (
                         self.local_git,
                         prev_commit,
                         new_commit,
                     ) = self.tar_to_git.extract_bundle_to_local_git(
                         commit_msg=commit_msg
                     )
-                    return True, prev_version, current_hash, prev_commit, new_commit
+                    return (
+                        True,
+                        prev_version,
+                        current_hash,
+                        prev_commit,
+                        new_commit,
+                    )
                 else:
                     return False, None, current_hash, None, None
 
+    def build_auth_headers(self, token=None, path=None):
+        # if it's a simple HTTP server with a bearer token
+        if self.server_type == PolicyBundleServerType.HTTP and token is not None:
+            return tuple_to_dict(get_authorization_header(token))
+        # if it's an AWS s3 server and we have the token and it's id -
+        elif (
+            self.server_type == PolicyBundleServerType.AWS_S3
+            and token is not None
+            and self.token_id is not None
+        ):
+            split_url = urlparse(self.remote_source_url)
+            host = split_url.netloc
+            path = split_url.path + "/" + path
+
+            return build_aws_rest_auth_headers(self.token_id, token, host, path)
+        else:
+            return {}
+
     async def fetch_policy_bundle_from_api_source(
         self, url: str, token: Optional[str]
     ) -> Tuple[Path, BundleHash, BundleHash]:
         """Fetches the bundle. May throw, in which case we retry again. Checks
         that the bundle file isn't the same with Etag, if server doesn't have
         Etag it checks it with hash on the bundle file.
 
@@ -109,33 +142,37 @@
             url(str): the base address to request the bundle.tar.gz file from
             token (str, optional): Auth token to include in connections to OPAL server. Defaults to POLICY_BUNDLE_SERVER_TOKEN.
         Returns:
             Path: path to the bundle file that we just downloaded from the remote API source
             BundleHash: previous bundle hash on None if this is the initial bundle file
             BundleHash: current bundle hash
         """
-        auth_headers = tuple_to_dict(get_authorization_header(token)) if token else {}
+        path = "bundle.tar.gz"
+
+        auth_headers = self.build_auth_headers(token=token, path=path)
         etag_headers = (
             {"ETag": self.etag, "If-None-Match": self.etag} if self.etag else {}
         )
-        full_url = f"{url}/bundle.tar.gz"
+
+        full_url = f"{url}/{path}"
 
         async with aiohttp.ClientSession() as session:
             try:
                 async with session.get(
                     f"{full_url}",
                     headers={
                         "content-type": "application/gzip",
                         **auth_headers,
                         **etag_headers,
                     },
                 ) as response:
                     if response.status == status.HTTP_404_NOT_FOUND:
                         logger.warning(
-                            "requested url not found: {full_url}", full_url=full_url
+                            "requested url not found: {full_url}",
+                            full_url=full_url,
                         )
                         raise HTTPException(
                             status_code=status.HTTP_404_NOT_FOUND,
                             detail=f"requested url not found: {full_url}",
                         )
                     if response.status == status.HTTP_304_NOT_MODIFIED:
                         logger.info(
@@ -152,15 +189,15 @@
                     response_bytes = await response.read()
                     tmp_file_path = self.tmp_bundle_path
                     with open(tmp_file_path, "wb") as file:
                         file.write(response_bytes)
 
                     if not current_etag:
                         logger.info(
-                            "Etag is turnned off, you may want to turn it on at your bundle server"
+                            "Etag is turned off, you may want to turn it on at your bundle server"
                         )
                         current_bundle_hash = hash_file(tmp_file_path)
                         logger.info("Bundle hash is {hash}", hash=current_bundle_hash)
                         if self.bundle_hash == current_bundle_hash:
                             logger.info(
                                 "No new bundle, hash is: {hash}",
                                 hash=current_bundle_hash,
@@ -169,21 +206,26 @@
                         else:
                             logger.info(
                                 "New bundle found, hash is: {hash}",
                                 hash=current_bundle_hash,
                             )
                             prev_bundle_hash = self.bundle_hash
                             self.bundle_hash = current_bundle_hash
-                            return tmp_file_path, prev_bundle_hash, current_bundle_hash
+                            return (
+                                tmp_file_path,
+                                prev_bundle_hash,
+                                current_bundle_hash,
+                            )
                     else:
                         if (
                             self.etag == current_etag
                         ):  # validate against bad etag implementation
                             logger.info(
-                                "No new bundle, hash is: {hash}", hash=current_etag
+                                "No new bundle, hash is: {hash}",
+                                hash=current_etag,
                             )
                             return False, None, current_etag
                         prev_etag = self.etag
                         self.etag = current_etag
                         return tmp_file_path, prev_etag, current_etag
 
             except (aiohttp.ClientError, HTTPException) as e:
@@ -196,15 +238,16 @@
     async def check_for_changes(self):
         """Calling this method will trigger an api check to the remote.
 
         If after the request the watcher detects new bundle, it will
         call the callbacks registered with _on_new_policy().
         """
         logger.info(
-            "Fetching changes from remote: '{remote}'", remote=self.remote_source_url
+            "Fetching changes from remote: '{remote}'",
+            remote=self.remote_source_url,
         )
         (
             has_changes,
             prev,
             latest,
             prev_commit,
             new_commit,
```

### Comparing `opal-common-0.7.0/opal_common/sources/base_policy_source.py` & `opal-common-0.7.1/opal_common/sources/base_policy_source.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/sources/git_policy_source.py` & `opal-common-0.7.1/opal_common/sources/git_policy_source.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/synchronization/expiring_redis_lock.py` & `opal-common-0.7.1/opal_common/synchronization/expiring_redis_lock.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/synchronization/named_lock.py` & `opal-common-0.7.1/opal_common/synchronization/named_lock.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/tests/path_utils_test.py` & `opal-common-0.7.1/opal_common/tests/path_utils_test.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/tests/url_utils_test.py` & `opal-common-0.7.1/opal_common/tests/url_utils_test.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/topics/listener.py` & `opal-common-0.7.1/opal_common/topics/listener.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/topics/publisher.py` & `opal-common-0.7.1/opal_common/topics/publisher.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,39 +8,43 @@
 class TopicPublisher:
     """abstract publisher, base class for client side and server side
     publisher."""
 
     def __init__(self):
         """inits the publisher's asyncio tasks list."""
         self._tasks: List[asyncio.Task] = []
+        self._tasks_lock = asyncio.Lock()
 
-    def publish(self, topics: TopicList, data: Any = None):
+    async def publish(self, topics: TopicList, data: Any = None):
         raise NotImplementedError()
 
     async def __aenter__(self):
         self.start()
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.stop()
 
     def start(self):
         """starts the publisher."""
         logger.debug("started topic publisher")
 
+    async def _add_task(self, task: asyncio.Task):
+        async with self._tasks_lock:
+            self._tasks.append(task)
+
     async def wait(self):
-        await asyncio.gather(*self._tasks, return_exceptions=True)
+        async with self._tasks_lock:
+            await asyncio.gather(*self._tasks, return_exceptions=True)
+            self._tasks.clear()
 
     async def stop(self):
         """stops the publisher (cancels any running publishing tasks)"""
         logger.debug("stopping topic publisher")
-        for task in self._tasks:
-            if not task.done():
-                task.cancel()
-        await asyncio.gather(*self._tasks, return_exceptions=True)
+        await self.wait()
 
 
 class PeriodicPublisher:
     """Wrapper for a task that publishes to topic on fixed interval
     periodically."""
 
     def __init__(
@@ -100,31 +104,32 @@
 
     async def _publish_task(self):
         while True:
             await asyncio.sleep(self._interval)
             logger.info(
                 f"{self._task_name}: publishing message on topic '{self._topic}', next publish is scheduled in {self._interval} seconds"
             )
-            self._publisher.publish(topics=[self._topic], data=self._message)
+            async with self._publisher:
+                await self._publisher.publish(topics=[self._topic], data=self._message)
 
 
 class ServerSideTopicPublisher(TopicPublisher):
     """A simple wrapper around a PubSubEndpoint that exposes publish()."""
 
     def __init__(self, endpoint: PubSubEndpoint):
         """inits the publisher.
 
         Args:
             endpoint (PubSubEndpoint): a pub/sub endpoint
         """
         self._endpoint = endpoint
         super().__init__()
 
-    def publish(self, topics: TopicList, data: Any = None):
-        self._tasks.append(
+    async def publish(self, topics: TopicList, data: Any = None):
+        await self._add_task(
             asyncio.create_task(self._endpoint.publish(topics=topics, data=data))
         )
 
 
 class ClientSideTopicPublisher(TopicPublisher):
     """A simple wrapper around a PubSubClient that exposes publish().
 
@@ -159,33 +164,35 @@
 
     async def wait_until_done(self):
         """When the publisher is a used as a context manager, this method waits
         until the client is done (i.e: terminated) to prevent exiting the
         context."""
         return await self._client.wait_until_done()
 
-    def publish(self, topics: TopicList, data: Any = None):
+    async def publish(self, topics: TopicList, data: Any = None):
         """publish a message by launching a background task on the event loop.
 
         Args:
             topics (TopicList): a list of topics to publish the message to
             data (Any): optional data to publish as part of the message
         """
-        self._tasks.append(asyncio.create_task(self._publish(topics=topics, data=data)))
+        await self._add_task(
+            asyncio.create_task(self._publish(topics=topics, data=data))
+        )
 
     async def _publish(self, topics: TopicList, data: Any = None) -> bool:
         """Do not trigger directly, must be triggered via publish() in order to
         run as a monitored background asyncio task."""
         await self._client.wait_until_ready()
         logger.info("Publishing to topics: {topics}", topics=topics)
         return await self._client.publish(topics, data)
 
 
 class ScopedServerSideTopicPublisher(ServerSideTopicPublisher):
     def __init__(self, endpoint: PubSubEndpoint, scope_id: str):
         super().__init__(endpoint)
         self._scope_id = scope_id
 
-    def publish(self, topics: TopicList, data: Any = None):
+    async def publish(self, topics: TopicList, data: Any = None):
         scoped_topics = [f"{self._scope_id}:{topic}" for topic in topics]
         logger.info("Publishing to topics: {topics}", topics=scoped_topics)
-        super().publish(scoped_topics, data)
+        await super().publish(scoped_topics, data)
```

### Comparing `opal-common-0.7.0/opal_common/topics/utils.py` & `opal-common-0.7.1/opal_common/topics/utils.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common/urls.py` & `opal-common-0.7.1/opal_common/urls.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/opal_common.egg-info/PKG-INFO` & `opal-common-0.7.1/opal_common.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opal-common
-Version: 0.7.0
+Version: 0.7.1
 Summary: OPAL is an administration layer for Open Policy Agent (OPA), detecting changes to both policy and data and pushing live updates to your agents. opal-common contains common code used by both opal-client and opal-server.
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
-Metadata-Version: 2.1 Name: opal-common Version: 0.7.0 Summary: OPAL is an
+Metadata-Version: 2.1 Name: opal-common Version: 0.7.1 Summary: OPAL is an
 administration layer for Open Policy Agent (OPA), detecting changes to both
 policy and data and pushing live updates to your agents. opal-common contains
 common code used by both opal-client and opal-server. Home-page: https://
 github.com/permitio/opal Author: Or Weis, Asaf Cohen Author-email: or@permit.io
 License: Apache 2.0 Classifier: Operating System :: OS Independent Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
@@ -12,43 +12,47 @@
 WWW/HTTP :: WSGI Requires-Python: >=3.7 Description-Content-Type: text/markdown
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
@@ -80,8 +84,9 @@
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

### Comparing `opal-common-0.7.0/opal_common.egg-info/SOURCES.txt` & `opal-common-0.7.1/opal_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.0/setup.py` & `opal-common-0.7.1/setup.py`

 * *Files identical despite different names*

