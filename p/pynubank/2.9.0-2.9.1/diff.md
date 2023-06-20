# Comparing `tmp/pynubank-2.9.0.tar.gz` & `tmp/pynubank-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pynubank-2.9.0.tar", last modified: Wed Dec 16 03:00:19 2020, max compression
+gzip compressed data, was "dist/pynubank-2.9.1.tar", last modified: Thu Dec 31 02:23:13 2020, max compression
```

## Comparing `pynubank-2.9.0.tar` & `pynubank-2.9.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-16 03:00:19.164068 pynubank-2.9.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5449 2020-12-16 03:00:19.164068 pynubank-2.9.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     4086 2020-12-16 02:59:50.000000 pynubank-2.9.0/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-16 03:00:19.156064 pynubank-2.9.0/pynubank/
--rw-rw-r--   0 travis    (2000) travis    (2000)      126 2020-12-16 02:59:50.000000 pynubank-2.9.0/pynubank/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1645 2020-12-16 02:59:50.000000 pynubank-2.9.0/pynubank/cli.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      571 2020-12-16 02:59:50.000000 pynubank-2.9.0/pynubank/exception.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7033 2020-12-16 02:59:50.000000 pynubank-2.9.0/pynubank/nubank.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-16 03:00:19.160066 pynubank-2.9.0/pynubank/queries/
--rw-rw-r--   0 travis    (2000) travis    (2000)      133 2020-12-16 02:59:50.000000 pynubank-2.9.0/pynubank/queries/account_balance.gql
--rw-rw-r--   0 travis    (2000) travis    (2000)     1124 2020-12-16 02:59:50.000000 pynubank-2.9.0/pynubank/queries/account_feed.gql
--rw-rw-r--   0 travis    (2000) travis    (2000)      154 2020-12-16 02:59:50.000000 pynubank-2.9.0/pynubank/queries/account_id.gql
--rw-rw-r--   0 travis    (2000) travis    (2000)      390 2020-12-16 02:59:50.000000 pynubank-2.9.0/pynubank/queries/account_investments.gql
--rw-rw-r--   0 travis    (2000) travis    (2000)      218 2020-12-16 02:59:50.000000 pynubank-2.9.0/pynubank/queries/create_boleto.gql
--rw-rw-r--   0 travis    (2000) travis    (2000)      210 2020-12-16 02:59:50.000000 pynubank-2.9.0/pynubank/queries/create_money_request.gql
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2020-12-16 02:59:50.000000 pynubank-2.9.0/pynubank/queries/create_pix_money_request.gql
--rw-rw-r--   0 travis    (2000) travis    (2000)      270 2020-12-16 02:59:50.000000 pynubank-2.9.0/pynubank/queries/get_pix_keys.gql
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-16 03:00:19.160066 pynubank-2.9.0/pynubank/utils/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-16 02:59:50.000000 pynubank-2.9.0/pynubank/utils/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3089 2020-12-16 02:59:50.000000 pynubank-2.9.0/pynubank/utils/certificate_generator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1062 2020-12-16 02:59:50.000000 pynubank-2.9.0/pynubank/utils/discovery.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      494 2020-12-16 02:59:50.000000 pynubank-2.9.0/pynubank/utils/graphql.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1213 2020-12-16 02:59:50.000000 pynubank-2.9.0/pynubank/utils/http.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3969 2020-12-16 02:59:50.000000 pynubank-2.9.0/pynubank/utils/mock_http.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-16 03:00:19.164068 pynubank-2.9.0/pynubank/utils/mocked_responses/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-16 02:59:50.000000 pynubank-2.9.0/pynubank/utils/mocked_responses/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      151 2020-12-16 02:59:50.000000 pynubank-2.9.0/pynubank/utils/mocked_responses/account_balance.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1900 2020-12-16 02:59:50.000000 pynubank-2.9.0/pynubank/utils/mocked_responses/account_feed.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1547 2020-12-16 02:59:50.000000 pynubank-2.9.0/pynubank/utils/mocked_responses/account_investments.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     2345 2020-12-16 02:59:50.000000 pynubank-2.9.0/pynubank/utils/mocked_responses/bills.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     3691 2020-12-16 02:59:50.000000 pynubank-2.9.0/pynubank/utils/mocked_responses/bills_summary.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      333 2020-12-16 02:59:50.000000 pynubank-2.9.0/pynubank/utils/mocked_responses/boleto_create.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     7082 2020-12-16 02:59:50.000000 pynubank-2.9.0/pynubank/utils/mocked_responses/customer.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1286 2020-12-16 02:59:50.000000 pynubank-2.9.0/pynubank/utils/mocked_responses/discovery_api.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     2929 2020-12-16 02:59:50.000000 pynubank-2.9.0/pynubank/utils/mocked_responses/discovery_app.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1607 2020-12-16 02:59:50.000000 pynubank-2.9.0/pynubank/utils/mocked_responses/discovery_login.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1515 2020-12-16 02:59:50.000000 pynubank-2.9.0/pynubank/utils/mocked_responses/discovery_login_alternative.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      187 2020-12-16 02:59:50.000000 pynubank-2.9.0/pynubank/utils/mocked_responses/money.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1099 2020-12-16 02:59:50.000000 pynubank-2.9.0/pynubank/utils/mocked_responses/pix_keys.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      441 2020-12-16 02:59:50.000000 pynubank-2.9.0/pynubank/utils/mocked_responses/pix_money_request.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      877 2020-12-16 02:59:50.000000 pynubank-2.9.0/pynubank/utils/mocked_responses/proxy_events.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-16 03:00:19.156064 pynubank-2.9.0/pynubank.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5449 2020-12-16 03:00:19.000000 pynubank-2.9.0/pynubank.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1866 2020-12-16 03:00:19.000000 pynubank-2.9.0/pynubank.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-12-16 03:00:19.000000 pynubank-2.9.0/pynubank.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       48 2020-12-16 03:00:19.000000 pynubank-2.9.0/pynubank.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       51 2020-12-16 03:00:19.000000 pynubank-2.9.0/pynubank.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       15 2020-12-16 03:00:19.000000 pynubank-2.9.0/pynubank.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       93 2020-12-16 03:00:19.168070 pynubank-2.9.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1029 2020-12-16 02:59:50.000000 pynubank-2.9.0/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-16 03:00:19.164068 pynubank-2.9.0/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-16 02:59:50.000000 pynubank-2.9.0/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       43 2020-12-16 02:59:50.000000 pynubank-2.9.0/tests/conftest.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-16 03:00:19.164068 pynubank-2.9.0/tests/fixtures/
--rw-rw-r--   0 travis    (2000) travis    (2000)       84 2020-12-16 02:59:50.000000 pynubank-2.9.0/tests/fixtures/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      269 2020-12-16 02:59:50.000000 pynubank-2.9.0/tests/fixtures/gen_certificate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      260 2020-12-16 02:59:50.000000 pynubank-2.9.0/tests/fixtures/proxy.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3619 2020-12-16 02:59:50.000000 pynubank-2.9.0/tests/test_certificate_generator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1788 2020-12-16 02:59:50.000000 pynubank-2.9.0/tests/test_cli.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1036 2020-12-16 02:59:50.000000 pynubank-2.9.0/tests/test_discovery.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3128 2020-12-16 02:59:50.000000 pynubank-2.9.0/tests/test_http_client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1486 2020-12-16 02:59:50.000000 pynubank-2.9.0/tests/test_mock_http_client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16582 2020-12-16 02:59:50.000000 pynubank-2.9.0/tests/test_nubank_client.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-31 02:23:13.204898 pynubank-2.9.1/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5449 2020-12-31 02:23:13.204898 pynubank-2.9.1/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4086 2020-12-31 02:22:46.000000 pynubank-2.9.1/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-31 02:23:13.196898 pynubank-2.9.1/pynubank/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      126 2020-12-31 02:22:46.000000 pynubank-2.9.1/pynubank/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1645 2020-12-31 02:22:46.000000 pynubank-2.9.1/pynubank/cli.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      571 2020-12-31 02:22:46.000000 pynubank-2.9.1/pynubank/exception.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7058 2020-12-31 02:22:46.000000 pynubank-2.9.1/pynubank/nubank.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-31 02:23:13.196898 pynubank-2.9.1/pynubank/queries/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      133 2020-12-31 02:22:46.000000 pynubank-2.9.1/pynubank/queries/account_balance.gql
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1124 2020-12-31 02:22:46.000000 pynubank-2.9.1/pynubank/queries/account_feed.gql
+-rw-rw-r--   0 travis    (2000) travis    (2000)      154 2020-12-31 02:22:46.000000 pynubank-2.9.1/pynubank/queries/account_id.gql
+-rw-rw-r--   0 travis    (2000) travis    (2000)      390 2020-12-31 02:22:46.000000 pynubank-2.9.1/pynubank/queries/account_investments.gql
+-rw-rw-r--   0 travis    (2000) travis    (2000)      218 2020-12-31 02:22:46.000000 pynubank-2.9.1/pynubank/queries/create_boleto.gql
+-rw-rw-r--   0 travis    (2000) travis    (2000)      210 2020-12-31 02:22:46.000000 pynubank-2.9.1/pynubank/queries/create_money_request.gql
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2020-12-31 02:22:46.000000 pynubank-2.9.1/pynubank/queries/create_pix_money_request.gql
+-rw-rw-r--   0 travis    (2000) travis    (2000)      270 2020-12-31 02:22:46.000000 pynubank-2.9.1/pynubank/queries/get_pix_keys.gql
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-31 02:23:13.200898 pynubank-2.9.1/pynubank/utils/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-31 02:22:46.000000 pynubank-2.9.1/pynubank/utils/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3089 2020-12-31 02:22:46.000000 pynubank-2.9.1/pynubank/utils/certificate_generator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1062 2020-12-31 02:22:46.000000 pynubank-2.9.1/pynubank/utils/discovery.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      494 2020-12-31 02:22:46.000000 pynubank-2.9.1/pynubank/utils/graphql.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1213 2020-12-31 02:22:46.000000 pynubank-2.9.1/pynubank/utils/http.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3969 2020-12-31 02:22:46.000000 pynubank-2.9.1/pynubank/utils/mock_http.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-31 02:23:13.200898 pynubank-2.9.1/pynubank/utils/mocked_responses/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-31 02:22:46.000000 pynubank-2.9.1/pynubank/utils/mocked_responses/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      151 2020-12-31 02:22:46.000000 pynubank-2.9.1/pynubank/utils/mocked_responses/account_balance.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1900 2020-12-31 02:22:46.000000 pynubank-2.9.1/pynubank/utils/mocked_responses/account_feed.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1547 2020-12-31 02:22:46.000000 pynubank-2.9.1/pynubank/utils/mocked_responses/account_investments.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2345 2020-12-31 02:22:46.000000 pynubank-2.9.1/pynubank/utils/mocked_responses/bills.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3691 2020-12-31 02:22:46.000000 pynubank-2.9.1/pynubank/utils/mocked_responses/bills_summary.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      333 2020-12-31 02:22:46.000000 pynubank-2.9.1/pynubank/utils/mocked_responses/boleto_create.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7082 2020-12-31 02:22:46.000000 pynubank-2.9.1/pynubank/utils/mocked_responses/customer.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1286 2020-12-31 02:22:46.000000 pynubank-2.9.1/pynubank/utils/mocked_responses/discovery_api.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2929 2020-12-31 02:22:46.000000 pynubank-2.9.1/pynubank/utils/mocked_responses/discovery_app.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1607 2020-12-31 02:22:46.000000 pynubank-2.9.1/pynubank/utils/mocked_responses/discovery_login.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1515 2020-12-31 02:22:46.000000 pynubank-2.9.1/pynubank/utils/mocked_responses/discovery_login_alternative.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      187 2020-12-31 02:22:46.000000 pynubank-2.9.1/pynubank/utils/mocked_responses/money.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1099 2020-12-31 02:22:46.000000 pynubank-2.9.1/pynubank/utils/mocked_responses/pix_keys.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      441 2020-12-31 02:22:46.000000 pynubank-2.9.1/pynubank/utils/mocked_responses/pix_money_request.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      877 2020-12-31 02:22:46.000000 pynubank-2.9.1/pynubank/utils/mocked_responses/proxy_events.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-31 02:23:13.196898 pynubank-2.9.1/pynubank.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5449 2020-12-31 02:23:13.000000 pynubank-2.9.1/pynubank.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1866 2020-12-31 02:23:13.000000 pynubank-2.9.1/pynubank.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-12-31 02:23:13.000000 pynubank-2.9.1/pynubank.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       48 2020-12-31 02:23:13.000000 pynubank-2.9.1/pynubank.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       51 2020-12-31 02:23:13.000000 pynubank-2.9.1/pynubank.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       15 2020-12-31 02:23:13.000000 pynubank-2.9.1/pynubank.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       93 2020-12-31 02:23:13.204898 pynubank-2.9.1/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1029 2020-12-31 02:22:46.000000 pynubank-2.9.1/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-31 02:23:13.200898 pynubank-2.9.1/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-31 02:22:46.000000 pynubank-2.9.1/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       43 2020-12-31 02:22:46.000000 pynubank-2.9.1/tests/conftest.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-31 02:23:13.204898 pynubank-2.9.1/tests/fixtures/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       84 2020-12-31 02:22:46.000000 pynubank-2.9.1/tests/fixtures/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      269 2020-12-31 02:22:46.000000 pynubank-2.9.1/tests/fixtures/gen_certificate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      260 2020-12-31 02:22:46.000000 pynubank-2.9.1/tests/fixtures/proxy.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3619 2020-12-31 02:22:46.000000 pynubank-2.9.1/tests/test_certificate_generator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1788 2020-12-31 02:22:46.000000 pynubank-2.9.1/tests/test_cli.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1036 2020-12-31 02:22:46.000000 pynubank-2.9.1/tests/test_discovery.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3128 2020-12-31 02:22:46.000000 pynubank-2.9.1/tests/test_http_client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1486 2020-12-31 02:22:46.000000 pynubank-2.9.1/tests/test_mock_http_client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16582 2020-12-31 02:22:46.000000 pynubank-2.9.1/tests/test_nubank_client.py
```

### Comparing `pynubank-2.9.0/PKG-INFO` & `pynubank-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynubank
-Version: 2.9.0
+Version: 2.9.1
 Summary: UNKNOWN
 Home-page: https://github.com/andreroggeri/pynubank
 Author: André Roggeri Campos
 Author-email: a.roggeri.c@gmail.com
 License: MIT
 Description: # pynubank
         ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pynubank)
```

### Comparing `pynubank-2.9.0/README.md` & `pynubank-2.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pynubank-2.9.0/pynubank/cli.py` & `pynubank-2.9.1/pynubank/cli.py`

 * *Files identical despite different names*

### Comparing `pynubank-2.9.0/pynubank/exception.py` & `pynubank-2.9.1/pynubank/exception.py`

 * *Files identical despite different names*

### Comparing `pynubank-2.9.0/pynubank/nubank.py` & `pynubank-2.9.1/pynubank/nubank.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,29 +41,28 @@
             "login": cpf,
             "password": password,
             "client_id": "other.conta",
             "client_secret": "yQPeLzoHuJzlMMSAjC-LgNUJdUecx8XO"
         }
         return self.client.post(self.discovery.get_url('login'), json=payload)
 
-    def _find_url(self, known_keys: set, links: dict) -> str:
-        intersection = known_keys.intersection(links)
-        iterator = iter(intersection)
-        key = next(iterator, None)
+    def _find_url(self, known_keys: list, links: dict) -> str:
+        links_keys = links.keys()
+        common_keys = [item for item in links_keys if item in known_keys]
+        key = next(iter(common_keys), None)
         return links.get(key, {}).get('href', None)
 
     def _save_auth_data(self, auth_data: dict) -> None:
         self.client.set_header('Authorization', f'Bearer {auth_data["access_token"]}')
 
         links = auth_data['_links']
         self.query_url = links['ghostflame']['href']
-
-        feed_url_keys = {'events', 'magnitude'}
-        bills_url_keys = {'bills_summary'}
-        customer_url_keys = {'customer'}
+        feed_url_keys = ['events', 'magnitude']
+        bills_url_keys = ['bills_summary']
+        customer_url_keys = ['customer']
 
         self.feed_url = self._find_url(feed_url_keys, links)
         self.bills_url = self._find_url(bills_url_keys, links)
         self.customer_url = self._find_url(customer_url_keys, links)
 
     def get_qr_code(self) -> Tuple[str, QRCode]:
         content = str(uuid.uuid4())
```

### Comparing `pynubank-2.9.0/pynubank/queries/account_feed.gql` & `pynubank-2.9.1/pynubank/queries/account_feed.gql`

 * *Files identical despite different names*

### Comparing `pynubank-2.9.0/pynubank/utils/certificate_generator.py` & `pynubank-2.9.1/pynubank/utils/certificate_generator.py`

 * *Files identical despite different names*

### Comparing `pynubank-2.9.0/pynubank/utils/discovery.py` & `pynubank-2.9.1/pynubank/utils/discovery.py`

 * *Files identical despite different names*

### Comparing `pynubank-2.9.0/pynubank/utils/http.py` & `pynubank-2.9.1/pynubank/utils/http.py`

 * *Files identical despite different names*

### Comparing `pynubank-2.9.0/pynubank/utils/mock_http.py` & `pynubank-2.9.1/pynubank/utils/mock_http.py`

 * *Files identical despite different names*

### Comparing `pynubank-2.9.0/pynubank/utils/mocked_responses/account_feed.json` & `pynubank-2.9.1/pynubank/utils/mocked_responses/account_feed.json`

 * *Files identical despite different names*

### Comparing `pynubank-2.9.0/pynubank/utils/mocked_responses/account_investments.json` & `pynubank-2.9.1/pynubank/utils/mocked_responses/account_investments.json`

 * *Files identical despite different names*

### Comparing `pynubank-2.9.0/pynubank/utils/mocked_responses/bills.json` & `pynubank-2.9.1/pynubank/utils/mocked_responses/bills.json`

 * *Files identical despite different names*

### Comparing `pynubank-2.9.0/pynubank/utils/mocked_responses/bills_summary.json` & `pynubank-2.9.1/pynubank/utils/mocked_responses/bills_summary.json`

 * *Files identical despite different names*

### Comparing `pynubank-2.9.0/pynubank/utils/mocked_responses/customer.json` & `pynubank-2.9.1/pynubank/utils/mocked_responses/customer.json`

 * *Files identical despite different names*

### Comparing `pynubank-2.9.0/pynubank/utils/mocked_responses/discovery_api.json` & `pynubank-2.9.1/pynubank/utils/mocked_responses/discovery_api.json`

 * *Files identical despite different names*

### Comparing `pynubank-2.9.0/pynubank/utils/mocked_responses/discovery_app.json` & `pynubank-2.9.1/pynubank/utils/mocked_responses/discovery_app.json`

 * *Files identical despite different names*

### Comparing `pynubank-2.9.0/pynubank/utils/mocked_responses/discovery_login.json` & `pynubank-2.9.1/pynubank/utils/mocked_responses/discovery_login.json`

 * *Files identical despite different names*

### Comparing `pynubank-2.9.0/pynubank/utils/mocked_responses/discovery_login_alternative.json` & `pynubank-2.9.1/pynubank/utils/mocked_responses/discovery_login_alternative.json`

 * *Files identical despite different names*

### Comparing `pynubank-2.9.0/pynubank/utils/mocked_responses/pix_keys.json` & `pynubank-2.9.1/pynubank/utils/mocked_responses/pix_keys.json`

 * *Files identical despite different names*

### Comparing `pynubank-2.9.0/pynubank/utils/mocked_responses/proxy_events.json` & `pynubank-2.9.1/pynubank/utils/mocked_responses/proxy_events.json`

 * *Files identical despite different names*

### Comparing `pynubank-2.9.0/pynubank.egg-info/PKG-INFO` & `pynubank-2.9.1/pynubank.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynubank
-Version: 2.9.0
+Version: 2.9.1
 Summary: UNKNOWN
 Home-page: https://github.com/andreroggeri/pynubank
 Author: André Roggeri Campos
 Author-email: a.roggeri.c@gmail.com
 License: MIT
 Description: # pynubank
         ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pynubank)
```

### Comparing `pynubank-2.9.0/pynubank.egg-info/SOURCES.txt` & `pynubank-2.9.1/pynubank.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynubank-2.9.0/setup.py` & `pynubank-2.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 def read(fname):
     with open(os.path.join(os.path.dirname(__file__), fname)) as f:
         return f.read()
 
 setup(
     name='pynubank',
-    version='2.9.0',
+    version='2.9.1',
     url='https://github.com/andreroggeri/pynubank',
     author='André Roggeri Campos',
     author_email='a.roggeri.c@gmail.com',
     license='MIT',
     packages=find_packages(),
     package_data={'pynubank': ['queries/*.gql', 'utils/mocked_responses/*.json']},
     install_requires=['requests', 'qrcode', 'pyOpenSSL', 'colorama', 'requests-pkcs12'],
```

### Comparing `pynubank-2.9.0/tests/test_certificate_generator.py` & `pynubank-2.9.1/tests/test_certificate_generator.py`

 * *Files identical despite different names*

### Comparing `pynubank-2.9.0/tests/test_cli.py` & `pynubank-2.9.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pynubank-2.9.0/tests/test_discovery.py` & `pynubank-2.9.1/tests/test_discovery.py`

 * *Files identical despite different names*

### Comparing `pynubank-2.9.0/tests/test_http_client.py` & `pynubank-2.9.1/tests/test_http_client.py`

 * *Files identical despite different names*

### Comparing `pynubank-2.9.0/tests/test_mock_http_client.py` & `pynubank-2.9.1/tests/test_mock_http_client.py`

 * *Files identical despite different names*

### Comparing `pynubank-2.9.0/tests/test_nubank_client.py` & `pynubank-2.9.1/tests/test_nubank_client.py`

 * *Files identical despite different names*

