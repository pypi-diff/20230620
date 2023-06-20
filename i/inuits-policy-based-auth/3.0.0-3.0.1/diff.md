# Comparing `tmp/inuits_policy_based_auth-3.0.0.tar.gz` & `tmp/inuits_policy_based_auth-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inuits_policy_based_auth-3.0.0.tar", last modified: Mon Apr 17 16:25:32 2023, max compression
+gzip compressed data, was "inuits_policy_based_auth-3.0.1.tar", last modified: Tue Jun 20 08:25:32 2023, max compression
```

## Comparing `inuits_policy_based_auth-3.0.0.tar` & `inuits_policy_based_auth-3.0.1.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-04-17 16:25:32.516754 inuits_policy_based_auth-3.0.0/
--rw-r--r--   0 eray      (1000) eray      (1000)    18092 2023-01-11 09:40:36.000000 inuits_policy_based_auth-3.0.0/LICENSE
--rw-r--r--   0 eray      (1000) eray      (1000)     7595 2023-04-17 16:25:32.516754 inuits_policy_based_auth-3.0.0/PKG-INFO
--rw-r--r--   0 eray      (1000) eray      (1000)     7133 2023-04-17 16:22:33.000000 inuits_policy_based_auth-3.0.0/README.md
-drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-04-17 16:25:32.509754 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/
--rw-r--r--   0 eray      (1000) eray      (1000)     1100 2023-03-17 17:05:37.000000 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/__init__.py
-drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-04-17 16:25:32.510754 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/authentication/
--rw-r--r--   0 eray      (1000) eray      (1000)        0 2023-03-17 15:56:53.000000 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/authentication/__init__.py
--rw-r--r--   0 eray      (1000) eray      (1000)     1881 2023-04-14 18:07:37.000000 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/authentication/base_authentication_policy.py
-drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-04-17 16:25:32.510754 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/authentication/policies/
--rw-r--r--   0 eray      (1000) eray      (1000)        0 2023-03-17 15:56:58.000000 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/authentication/policies/__init__.py
-drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-04-17 16:25:32.511754 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/authentication/policies/token_based_policies/
--rw-r--r--   0 eray      (1000) eray      (1000)        0 2023-03-17 17:27:12.000000 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/authentication/policies/token_based_policies/__init__.py
--rw-r--r--   0 eray      (1000) eray      (1000)    10967 2023-04-17 15:55:20.000000 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/authentication/policies/token_based_policies/authlib_flask_oauth2_policy.py
-drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-04-17 16:25:32.511754 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/authorization/
--rw-r--r--   0 eray      (1000) eray      (1000)        0 2023-03-17 15:57:41.000000 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/authorization/__init__.py
--rw-r--r--   0 eray      (1000) eray      (1000)     2744 2023-04-14 18:06:21.000000 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/authorization/base_authorization_policy.py
-drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-04-17 16:25:32.511754 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/authorization/policies/
--rw-r--r--   0 eray      (1000) eray      (1000)        0 2023-03-17 17:27:18.000000 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/authorization/policies/__init__.py
--rw-r--r--   0 eray      (1000) eray      (1000)      470 2023-01-11 11:28:59.000000 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/authorization/policies/open_data_policy.py
--rw-r--r--   0 eray      (1000) eray      (1000)      530 2023-03-20 10:09:51.000000 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/authorization/policies/scope_based_policy.py
--rw-r--r--   0 eray      (1000) eray      (1000)      571 2023-04-14 18:06:49.000000 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/authorization/policies/super_admin_policy.py
-drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-04-17 16:25:32.512754 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/contexts/
--rw-r--r--   0 eray      (1000) eray      (1000)      223 2023-01-10 14:21:54.000000 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/contexts/__init__.py
--rw-r--r--   0 eray      (1000) eray      (1000)      851 2023-04-14 18:01:31.000000 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/contexts/policy_context.py
--rw-r--r--   0 eray      (1000) eray      (1000)     1435 2023-04-14 18:12:49.000000 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/contexts/request_context.py
--rw-r--r--   0 eray      (1000) eray      (1000)     2942 2023-04-14 18:18:05.000000 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/contexts/user_context.py
--rw-r--r--   0 eray      (1000) eray      (1000)     1591 2023-04-17 09:09:37.000000 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/exceptions.py
-drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-04-17 16:25:32.512754 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/helpers/
--rw-r--r--   0 eray      (1000) eray      (1000)        0 2023-03-21 08:11:53.000000 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/helpers/__init__.py
--rw-r--r--   0 eray      (1000) eray      (1000)     4768 2023-03-22 15:11:22.000000 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/helpers/immutable_dict.py
--rw-r--r--   0 eray      (1000) eray      (1000)    10620 2023-04-17 15:12:55.000000 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/policy_factory.py
-drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-04-17 16:25:32.510754 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth.egg-info/
--rw-r--r--   0 eray      (1000) eray      (1000)     7595 2023-04-17 16:25:32.000000 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth.egg-info/PKG-INFO
--rw-r--r--   0 eray      (1000) eray      (1000)     2621 2023-04-17 16:25:32.000000 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth.egg-info/SOURCES.txt
--rw-r--r--   0 eray      (1000) eray      (1000)        1 2023-04-17 16:25:32.000000 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth.egg-info/dependency_links.txt
--rw-r--r--   0 eray      (1000) eray      (1000)      129 2023-04-17 16:25:32.000000 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth.egg-info/requires.txt
--rw-r--r--   0 eray      (1000) eray      (1000)       31 2023-04-17 16:25:32.000000 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth.egg-info/top_level.txt
--rw-r--r--   0 eray      (1000) eray      (1000)       38 2023-04-17 16:25:32.516754 inuits_policy_based_auth-3.0.0/setup.cfg
--rw-r--r--   0 eray      (1000) eray      (1000)      959 2023-04-17 16:24:22.000000 inuits_policy_based_auth-3.0.0/setup.py
-drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-04-17 16:25:32.508754 inuits_policy_based_auth-3.0.0/tests/
-drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-04-17 16:25:32.513754 inuits_policy_based_auth-3.0.0/tests/integration/
--rw-r--r--   0 eray      (1000) eray      (1000)        0 2023-01-13 15:47:05.000000 inuits_policy_based_auth-3.0.0/tests/integration/__init__.py
-drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-04-17 16:25:32.513754 inuits_policy_based_auth-3.0.0/tests/integration/authentication/
--rw-r--r--   0 eray      (1000) eray      (1000)        0 2023-01-19 13:52:33.000000 inuits_policy_based_auth-3.0.0/tests/integration/authentication/__init__.py
--rw-r--r--   0 eray      (1000) eray      (1000)     1201 2023-04-14 14:07:40.000000 inuits_policy_based_auth-3.0.0/tests/integration/authentication/test_authlib_flask_oauth2_policy.py
-drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-04-17 16:25:32.513754 inuits_policy_based_auth-3.0.0/tests/integration/authorization/
--rw-r--r--   0 eray      (1000) eray      (1000)        0 2023-01-20 08:59:06.000000 inuits_policy_based_auth-3.0.0/tests/integration/authorization/__init__.py
--rw-r--r--   0 eray      (1000) eray      (1000)     1093 2023-03-20 10:42:01.000000 inuits_policy_based_auth-3.0.0/tests/integration/authorization/test_open_data_policy.py
--rw-r--r--   0 eray      (1000) eray      (1000)     1317 2023-03-21 17:11:07.000000 inuits_policy_based_auth-3.0.0/tests/integration/authorization/test_scope_based_policy.py
--rw-r--r--   0 eray      (1000) eray      (1000)     1947 2023-04-17 14:18:39.000000 inuits_policy_based_auth-3.0.0/tests/integration/authorization/test_super_admin_policy.py
--rw-r--r--   0 eray      (1000) eray      (1000)      656 2023-01-19 15:19:28.000000 inuits_policy_based_auth-3.0.0/tests/integration/custom_token.py
--rw-r--r--   0 eray      (1000) eray      (1000)     1508 2023-04-17 14:44:09.000000 inuits_policy_based_auth-3.0.0/tests/integration/flask_process.py
-drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-04-17 16:25:32.514754 inuits_policy_based_auth-3.0.0/tests/integration/test_api/
--rw-r--r--   0 eray      (1000) eray      (1000)        0 2023-01-13 15:47:05.000000 inuits_policy_based_auth-3.0.0/tests/integration/test_api/__init__.py
--rw-r--r--   0 eray      (1000) eray      (1000)     1793 2023-04-17 15:15:06.000000 inuits_policy_based_auth-3.0.0/tests/integration/test_api/app.py
--rw-r--r--   0 eray      (1000) eray      (1000)     2593 2023-04-17 15:56:03.000000 inuits_policy_based_auth-3.0.0/tests/integration/test_api/policy_loader.py
--rw-r--r--   0 eray      (1000) eray      (1000)     3480 2023-04-17 14:31:12.000000 inuits_policy_based_auth-3.0.0/tests/integration/test_policy_factory.py
-drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-04-17 16:25:32.514754 inuits_policy_based_auth-3.0.0/tests/unit/
--rw-r--r--   0 eray      (1000) eray      (1000)        0 2023-01-13 14:32:25.000000 inuits_policy_based_auth-3.0.0/tests/unit/__init__.py
-drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-04-17 16:25:32.514754 inuits_policy_based_auth-3.0.0/tests/unit/authentication/
--rw-r--r--   0 eray      (1000) eray      (1000)        0 2023-01-13 14:32:11.000000 inuits_policy_based_auth-3.0.0/tests/unit/authentication/__init__.py
--rw-r--r--   0 eray      (1000) eray      (1000)     1345 2023-01-11 15:24:33.000000 inuits_policy_based_auth-3.0.0/tests/unit/authentication/test_base_authentication_policy.py
-drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-04-17 16:25:32.515754 inuits_policy_based_auth-3.0.0/tests/unit/authorization/
--rw-r--r--   0 eray      (1000) eray      (1000)        0 2023-01-11 10:19:57.000000 inuits_policy_based_auth-3.0.0/tests/unit/authorization/__init__.py
-drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-04-17 16:25:32.515754 inuits_policy_based_auth-3.0.0/tests/unit/authorization/policies/
--rw-r--r--   0 eray      (1000) eray      (1000)        0 2023-01-11 11:40:35.000000 inuits_policy_based_auth-3.0.0/tests/unit/authorization/policies/__init__.py
--rw-r--r--   0 eray      (1000) eray      (1000)      150 2023-01-11 11:37:14.000000 inuits_policy_based_auth-3.0.0/tests/unit/authorization/policies/dummies.py
--rw-r--r--   0 eray      (1000) eray      (1000)     1138 2023-01-11 14:27:27.000000 inuits_policy_based_auth-3.0.0/tests/unit/authorization/policies/test_open_data_policy.py
--rw-r--r--   0 eray      (1000) eray      (1000)     1105 2023-03-20 10:20:57.000000 inuits_policy_based_auth-3.0.0/tests/unit/authorization/policies/test_scope_based_policy.py
--rw-r--r--   0 eray      (1000) eray      (1000)     1040 2023-04-14 08:37:28.000000 inuits_policy_based_auth-3.0.0/tests/unit/authorization/policies/test_super_admin_policy.py
--rw-r--r--   0 eray      (1000) eray      (1000)     2024 2023-01-11 15:24:03.000000 inuits_policy_based_auth-3.0.0/tests/unit/authorization/test_base_authorization_policy.py
-drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-04-17 16:25:32.516754 inuits_policy_based_auth-3.0.0/tests/unit/helpers/
--rw-r--r--   0 eray      (1000) eray      (1000)        0 2023-03-21 13:26:01.000000 inuits_policy_based_auth-3.0.0/tests/unit/helpers/__init__.py
--rw-r--r--   0 eray      (1000) eray      (1000)     3524 2023-03-21 18:25:06.000000 inuits_policy_based_auth-3.0.0/tests/unit/helpers/test_immutable_dict.py
--rw-r--r--   0 eray      (1000) eray      (1000)    11998 2023-04-17 15:27:47.000000 inuits_policy_based_auth-3.0.0/tests/unit/test_policy_factory.py
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:25:32.956616 inuits_policy_based_auth-3.0.1/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)    18092 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/LICENSE
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     7595 2023-06-20 08:25:32.956616 inuits_policy_based_auth-3.0.1/PKG-INFO
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     7133 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/README.md
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:25:32.953282 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     1100 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/__init__.py
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:25:32.953282 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/authentication/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/authentication/__init__.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     1881 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/authentication/base_authentication_policy.py
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:25:32.953282 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/authentication/policies/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/authentication/policies/__init__.py
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:25:32.953282 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/authentication/policies/token_based_policies/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/authentication/policies/token_based_policies/__init__.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)    11621 2023-06-20 08:23:35.000000 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/authentication/policies/token_based_policies/authlib_flask_oauth2_policy.py
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:25:32.953282 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/authorization/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/authorization/__init__.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     2744 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/authorization/base_authorization_policy.py
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:25:32.956616 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/authorization/policies/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/authorization/policies/__init__.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)      470 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/authorization/policies/open_data_policy.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)      530 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/authorization/policies/scope_based_policy.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)      571 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/authorization/policies/super_admin_policy.py
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:25:32.956616 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/contexts/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)      223 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/contexts/__init__.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)      851 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/contexts/policy_context.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     1435 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/contexts/request_context.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     2942 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/contexts/user_context.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     1591 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/exceptions.py
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:25:32.956616 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/helpers/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/helpers/__init__.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     4768 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/helpers/immutable_dict.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)    10620 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/policy_factory.py
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:25:32.953282 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth.egg-info/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     7595 2023-06-20 08:25:32.000000 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth.egg-info/PKG-INFO
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     2621 2023-06-20 08:25:32.000000 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 gverm     (1000) gverm     (1001)        1 2023-06-20 08:25:32.000000 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 gverm     (1000) gverm     (1001)      129 2023-06-20 08:25:32.000000 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth.egg-info/requires.txt
+-rw-r--r--   0 gverm     (1000) gverm     (1001)       31 2023-06-20 08:25:32.000000 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth.egg-info/top_level.txt
+-rw-r--r--   0 gverm     (1000) gverm     (1001)       38 2023-06-20 08:25:32.956616 inuits_policy_based_auth-3.0.1/setup.cfg
+-rw-r--r--   0 gverm     (1000) gverm     (1001)      959 2023-06-20 08:23:35.000000 inuits_policy_based_auth-3.0.1/setup.py
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:25:32.953282 inuits_policy_based_auth-3.0.1/tests/
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:25:32.956616 inuits_policy_based_auth-3.0.1/tests/integration/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/tests/integration/__init__.py
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:25:32.956616 inuits_policy_based_auth-3.0.1/tests/integration/authentication/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/tests/integration/authentication/__init__.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     1201 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/tests/integration/authentication/test_authlib_flask_oauth2_policy.py
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:25:32.956616 inuits_policy_based_auth-3.0.1/tests/integration/authorization/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/tests/integration/authorization/__init__.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     1093 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/tests/integration/authorization/test_open_data_policy.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     1317 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/tests/integration/authorization/test_scope_based_policy.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     1947 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/tests/integration/authorization/test_super_admin_policy.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)      656 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/tests/integration/custom_token.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     1508 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/tests/integration/flask_process.py
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:25:32.956616 inuits_policy_based_auth-3.0.1/tests/integration/test_api/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/tests/integration/test_api/__init__.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     1793 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/tests/integration/test_api/app.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     2593 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/tests/integration/test_api/policy_loader.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     3480 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/tests/integration/test_policy_factory.py
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:25:32.956616 inuits_policy_based_auth-3.0.1/tests/unit/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/tests/unit/__init__.py
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:25:32.956616 inuits_policy_based_auth-3.0.1/tests/unit/authentication/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/tests/unit/authentication/__init__.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     1345 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/tests/unit/authentication/test_base_authentication_policy.py
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:25:32.956616 inuits_policy_based_auth-3.0.1/tests/unit/authorization/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/tests/unit/authorization/__init__.py
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:25:32.956616 inuits_policy_based_auth-3.0.1/tests/unit/authorization/policies/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/tests/unit/authorization/policies/__init__.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)      150 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/tests/unit/authorization/policies/dummies.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     1138 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/tests/unit/authorization/policies/test_open_data_policy.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     1105 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/tests/unit/authorization/policies/test_scope_based_policy.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     1040 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/tests/unit/authorization/policies/test_super_admin_policy.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     2024 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/tests/unit/authorization/test_base_authorization_policy.py
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:25:32.956616 inuits_policy_based_auth-3.0.1/tests/unit/helpers/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/tests/unit/helpers/__init__.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     3524 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/tests/unit/helpers/test_immutable_dict.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)    11998 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/tests/unit/test_policy_factory.py
```

### Comparing `inuits_policy_based_auth-3.0.0/LICENSE` & `inuits_policy_based_auth-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.0/PKG-INFO` & `inuits_policy_based_auth-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inuits_policy_based_auth
-Version: 3.0.0
+Version: 3.0.1
 Summary: Module for securing API endpoints based on policies.
 Author: Inuits
 Author-email: developers@inuits.eu
 License: GPLv2
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `inuits_policy_based_auth-3.0.0/README.md` & `inuits_policy_based_auth-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/__init__.py` & `inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/__init__.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/authentication/base_authentication_policy.py` & `inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/authentication/base_authentication_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/authentication/policies/token_based_policies/authlib_flask_oauth2_policy.py` & `inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/authentication/policies/token_based_policies/authlib_flask_oauth2_policy.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,38 +38,43 @@
     remote_token_validation : bool, optional
         A flag indicating whether token validation should be done remotely.
     remote_public_key : str, optional
         A string representing the public key of the authorization server used for
         remote token validation.
     realm_cache_sync_time : int, optional
         The number of seconds after which the realm cache should be refreshed.
+    remote_public_key : List[dict], optional
+        A JWKS used by the remote OpenID Connect provider to verify the JWT signature. If
+        provided, it will be used instead of the public key or JWKS provided by the issuer.
     **kwargs : dict
         Any additional keyword arguments to be passed to the JWTValidator constructor.
     """
 
     def __init__(
         self,
         logger: Logger,
         static_issuer=None,
         static_public_key=None,
         realms=None,
         role_scope_mapping_filepath=None,
         remote_token_validation=False,
         remote_public_key=None,
         realm_cache_sync_time=1800,
+        remote_jwks=None,
         **kwargs,
     ):
         validator = JWTValidator(
             logger,
             static_issuer,
             static_public_key,
             realms,
             remote_token_validation,
             remote_public_key,
             realm_cache_sync_time,
+            remote_jwks,
             **kwargs,
         )
         resource_protector = ResourceProtector()
         resource_protector.register_token_validator(validator)
         self._resource_protector = resource_protector
 
         self._logger = logger
@@ -154,14 +159,17 @@
     remote_public_key : str, optional
         A string representing the public key used by the remote OpenID Connect provider to
         verify the JWT signature. If provided, it will be used instead of the public key
         provided by the issuer.
     realm_cache_sync_time : int, optional
         An integer representing the number of seconds to cache realm configuration data
         before syncing with the issuer.
+    remote_public_key : List[dict], optional
+        A JWKS used by the remote OpenID Connect provider to verify the JWT signature. If
+        provided, it will be used instead of the public key or JWKS provided by the issuer.
     **kwargs : dict
         Additional keyword arguments to be passed to the parent class.
 
     Attributes:
     -----------
     TOKEN_TYPE : str
         A string representing the token type that this validator is responsible for.
@@ -196,24 +204,26 @@
         logger,
         static_issuer=None,
         static_public_key=None,
         realms=None,
         remote_token_validation=False,
         remote_public_key=None,
         realm_cache_sync_time=1800,
+        remote_jwks=None,
         **kwargs,
     ):
         super().__init__(**kwargs)
         self.logger = logger
         self.static_issuer = static_issuer
         self.static_public_key = static_public_key
         self.realms = realms if realms else []
         self.remote_token_validation = remote_token_validation
         self.remote_public_key = remote_public_key
         self.realm_cache_sync_time = realm_cache_sync_time
+        self.remote_jwks = remote_jwks
         self.realm_config_cache = {}
         self.claims_options = {
             "exp": {"essential": True},
             "azp": {"essential": True},
             "sub": {"essential": True},
         }
 
@@ -234,22 +244,23 @@
         """
 
         issuer = self.__get_unverified_issuer(token_string)
         if not issuer:
             return None
 
         realm_config = self.__get_realm_config_by_issuer(issuer)
-        public_key = ""
+        decode_key = ""
         if "public_key" in realm_config:
-            public_key = f'-----BEGIN PUBLIC KEY-----\n{realm_config["public_key"]}\n-----END PUBLIC KEY-----'
-
+            decode_key = f'-----BEGIN PUBLIC KEY-----\n{realm_config["public_key"]}\n-----END PUBLIC KEY-----'
+        elif self.remote_jwks is not None:
+            decode_key = self.remote_jwks
         try:
             claims = jwt.decode(
                 token_string,
-                public_key,
+                decode_key,
                 claims_options=self.claims_options,
                 claims_cls=self.token_cls,
             )
             claims.validate()
 
             if self.remote_token_validation:
                 result = requests.get(
```

### Comparing `inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/authorization/base_authorization_policy.py` & `inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/authorization/base_authorization_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/authorization/policies/scope_based_policy.py` & `inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/authorization/policies/scope_based_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/authorization/policies/super_admin_policy.py` & `inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/authorization/policies/super_admin_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/contexts/policy_context.py` & `inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/contexts/policy_context.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/contexts/request_context.py` & `inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/contexts/request_context.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/contexts/user_context.py` & `inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/contexts/user_context.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/exceptions.py` & `inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/exceptions.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/helpers/immutable_dict.py` & `inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/helpers/immutable_dict.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/policy_factory.py` & `inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/policy_factory.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.0/inuits_policy_based_auth.egg-info/PKG-INFO` & `inuits_policy_based_auth-3.0.1/inuits_policy_based_auth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inuits-policy-based-auth
-Version: 3.0.0
+Version: 3.0.1
 Summary: Module for securing API endpoints based on policies.
 Author: Inuits
 Author-email: developers@inuits.eu
 License: GPLv2
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `inuits_policy_based_auth-3.0.0/inuits_policy_based_auth.egg-info/SOURCES.txt` & `inuits_policy_based_auth-3.0.1/inuits_policy_based_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.0/setup.py` & `inuits_policy_based_auth-3.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,9 +25,9 @@
     ],
     license="GPLv2",
     long_description=long_desc,
     long_description_content_type="text/markdown",
     name="inuits_policy_based_auth",
     packages=find_packages(exclude=["tests"]),
     provides=["inuits_policy_based_auth"],
-    version="3.0.0",
+    version="3.0.1",
 )
```

### Comparing `inuits_policy_based_auth-3.0.0/tests/integration/authentication/test_authlib_flask_oauth2_policy.py` & `inuits_policy_based_auth-3.0.1/tests/integration/authentication/test_authlib_flask_oauth2_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.0/tests/integration/authorization/test_open_data_policy.py` & `inuits_policy_based_auth-3.0.1/tests/integration/authorization/test_open_data_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.0/tests/integration/authorization/test_scope_based_policy.py` & `inuits_policy_based_auth-3.0.1/tests/integration/authorization/test_scope_based_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.0/tests/integration/authorization/test_super_admin_policy.py` & `inuits_policy_based_auth-3.0.1/tests/integration/authorization/test_super_admin_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.0/tests/integration/custom_token.py` & `inuits_policy_based_auth-3.0.1/tests/integration/custom_token.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.0/tests/integration/flask_process.py` & `inuits_policy_based_auth-3.0.1/tests/integration/flask_process.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.0/tests/integration/test_api/app.py` & `inuits_policy_based_auth-3.0.1/tests/integration/test_api/app.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.0/tests/integration/test_api/policy_loader.py` & `inuits_policy_based_auth-3.0.1/tests/integration/test_api/policy_loader.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.0/tests/integration/test_policy_factory.py` & `inuits_policy_based_auth-3.0.1/tests/integration/test_policy_factory.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.0/tests/unit/authentication/test_base_authentication_policy.py` & `inuits_policy_based_auth-3.0.1/tests/unit/authentication/test_base_authentication_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.0/tests/unit/authorization/policies/test_open_data_policy.py` & `inuits_policy_based_auth-3.0.1/tests/unit/authorization/policies/test_open_data_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.0/tests/unit/authorization/policies/test_scope_based_policy.py` & `inuits_policy_based_auth-3.0.1/tests/unit/authorization/policies/test_scope_based_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.0/tests/unit/authorization/policies/test_super_admin_policy.py` & `inuits_policy_based_auth-3.0.1/tests/unit/authorization/policies/test_super_admin_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.0/tests/unit/authorization/test_base_authorization_policy.py` & `inuits_policy_based_auth-3.0.1/tests/unit/authorization/test_base_authorization_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.0/tests/unit/helpers/test_immutable_dict.py` & `inuits_policy_based_auth-3.0.1/tests/unit/helpers/test_immutable_dict.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.0/tests/unit/test_policy_factory.py` & `inuits_policy_based_auth-3.0.1/tests/unit/test_policy_factory.py`

 * *Files identical despite different names*

