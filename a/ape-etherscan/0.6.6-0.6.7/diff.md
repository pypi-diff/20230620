# Comparing `tmp/ape-etherscan-0.6.6.tar.gz` & `tmp/ape-etherscan-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-etherscan-0.6.6.tar", last modified: Thu Jun  8 14:11:21 2023, max compression
+gzip compressed data, was "ape-etherscan-0.6.7.tar", last modified: Tue Jun 20 00:43:37 2023, max compression
```

## Comparing `ape-etherscan-0.6.6.tar` & `ape-etherscan-0.6.7.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:11:21.869400 ape-etherscan-0.6.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:11:21.861400 ape-etherscan-0.6.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:11:21.861400 ape-etherscan-0.6.6/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:11:21.865400 ape-etherscan-0.6.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/.github/workflows/commit.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/.github/workflows/stale-prs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-06-08 14:11:21.869400 ape-etherscan-0.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:11:21.865400 ape-etherscan-0.6.6/ape_etherscan/
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/ape_etherscan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13354 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/ape_etherscan/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/ape_etherscan/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/ape_etherscan/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/ape_etherscan/explorer.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/ape_etherscan/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/ape_etherscan/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/ape_etherscan/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/ape_etherscan/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12407 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/ape_etherscan/verify.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-08 14:11:21.000000 ape-etherscan-0.6.6/ape_etherscan/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:11:21.865400 ape-etherscan-0.6.6/ape_etherscan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-06-08 14:11:21.000000 ape-etherscan-0.6.6/ape_etherscan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-08 14:11:21.000000 ape-etherscan-0.6.6/ape_etherscan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 14:11:21.000000 ape-etherscan-0.6.6/ape_etherscan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 14:11:21.000000 ape-etherscan-0.6.6/ape_etherscan.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-08 14:11:21.000000 ape-etherscan-0.6.6/ape_etherscan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-08 14:11:21.000000 ape-etherscan-0.6.6/ape_etherscan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-08 14:11:21.869400 ape-etherscan-0.6.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:11:21.865400 ape-etherscan-0.6.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15347 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:11:21.869400 ape-etherscan-0.6.6/tests/mock_responses/
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/tests/mock_responses/get_account_transactions.json
--rw-r--r--   0 runner    (1001) docker     (123)    85181 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/tests/mock_responses/get_contract_response.json
--rw-r--r--   0 runner    (1001) docker     (123)    93453 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/tests/mock_responses/get_proxy_contract_response.json
--rw-r--r--   0 runner    (1001) docker     (123)    93483 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/tests/mock_responses/get_vyper_contract_response.json
--rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/tests/test_etherscan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:43:37.871966 ape-etherscan-0.6.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:43:37.867966 ape-etherscan-0.6.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:43:37.867966 ape-etherscan-0.6.7/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:43:37.867966 ape-etherscan-0.6.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/.github/workflows/commit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/.github/workflows/stale-prs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-06-20 00:43:37.871966 ape-etherscan-0.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:43:37.867966 ape-etherscan-0.6.7/ape_etherscan/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/ape_etherscan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13354 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/ape_etherscan/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/ape_etherscan/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/ape_etherscan/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/ape_etherscan/explorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/ape_etherscan/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/ape_etherscan/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/ape_etherscan/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/ape_etherscan/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12584 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/ape_etherscan/verify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-20 00:43:37.000000 ape-etherscan-0.6.7/ape_etherscan/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:43:37.867966 ape-etherscan-0.6.7/ape_etherscan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-06-20 00:43:37.000000 ape-etherscan-0.6.7/ape_etherscan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-20 00:43:37.000000 ape-etherscan-0.6.7/ape_etherscan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 00:43:37.000000 ape-etherscan-0.6.7/ape_etherscan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 00:43:37.000000 ape-etherscan-0.6.7/ape_etherscan.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-20 00:43:37.000000 ape-etherscan-0.6.7/ape_etherscan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-20 00:43:37.000000 ape-etherscan-0.6.7/ape_etherscan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-20 00:43:37.871966 ape-etherscan-0.6.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:43:37.867966 ape-etherscan-0.6.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15418 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:43:37.871966 ape-etherscan-0.6.7/tests/mock_responses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/tests/mock_responses/get_account_transactions.json
+-rw-r--r--   0 runner    (1001) docker     (123)    85181 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/tests/mock_responses/get_contract_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)    93453 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/tests/mock_responses/get_proxy_contract_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)    93483 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/tests/mock_responses/get_vyper_contract_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/tests/test_etherscan.py
```

### Comparing `ape-etherscan-0.6.6/.github/ISSUE_TEMPLATE/bug.md` & `ape-etherscan-0.6.7/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.6/.github/ISSUE_TEMPLATE/feature.md` & `ape-etherscan-0.6.7/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.6/.github/ISSUE_TEMPLATE/work-item.md` & `ape-etherscan-0.6.7/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.6/.github/release-drafter.yml` & `ape-etherscan-0.6.7/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.6/.github/workflows/codeql.yml` & `ape-etherscan-0.6.7/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.6/.github/workflows/commit.yaml` & `ape-etherscan-0.6.7/.github/workflows/commit.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,14 @@
         - uses: actions/checkout@v3
           with:
               fetch-depth: 0
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
-              python-version: 3.8
+              python-version: "3.10"
 
         - name: Install Dependencies
           run: pip install commitizen
 
         - name: Check commit history
           run: cz check --rev-range $(git rev-list --all --reverse | head -1)..HEAD
```

### Comparing `ape-etherscan-0.6.6/.github/workflows/prtitle.yaml` & `ape-etherscan-0.6.7/.github/workflows/prtitle.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
         steps:
         - uses: actions/checkout@v3
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
-              python-version: 3.8
+              python-version: "3.10"
 
         - name: Install Dependencies
           run: pip install commitizen
 
         - name: Check PR Title
           env:
               TITLE: ${{ github.event.pull_request.title }}
```

### Comparing `ape-etherscan-0.6.6/.github/workflows/publish.yaml` & `ape-etherscan-0.6.7/.github/workflows/publish.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     steps:
     - uses: actions/checkout@v3
 
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
-        python-version: 3.8
+        python-version: "3.10"
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install -e .[release]
         
     - name: Build
```

### Comparing `ape-etherscan-0.6.6/.github/workflows/stale-prs.yml` & `ape-etherscan-0.6.7/.github/workflows/stale-prs.yml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.6/.github/workflows/test.yaml` & `ape-etherscan-0.6.7/.github/workflows/test.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
         steps:
         - uses: actions/checkout@v3
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
-              python-version: 3.8
+              python-version: "3.10"
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install .[lint]
 
         - name: Run Black
@@ -43,15 +43,15 @@
 
         steps:
         - uses: actions/checkout@v3
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
-              python-version: 3.8
+              python-version: "3.10"
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install .[lint,test]
 
         - name: Run MyPy
@@ -59,15 +59,15 @@
 
     functional:
         runs-on: ${{ matrix.os }}
 
         strategy:
             matrix:
                 os: [ubuntu-latest, macos-latest]   # eventually add `windows-latest`
-                python-version: [3.8, 3.9, "3.10"]
+                python-version: [3.8, 3.9, "3.10", "3.11"]
 
         steps:
         - uses: actions/checkout@v3
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
@@ -92,14 +92,14 @@
 #
 #        steps:
 #        - uses: actions/checkout@v2
 #
 #        - name: Setup Python
 #          uses: actions/setup-python@v2
 #          with:
-#              python-version: 3.8
+#              python-version: "3.10"
 #
 #        - name: Install Dependencies
 #          run: pip install .[test]
 #
 #        - name: Run Tests
 #          run: pytest -m "fuzzing" --no-cov -s
```

### Comparing `ape-etherscan-0.6.6/.gitignore` & `ape-etherscan-0.6.7/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.6/.pre-commit-config.yaml` & `ape-etherscan-0.6.7/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 -   repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
         name: black
 
 -   repo: https://github.com/pycqa/flake8
-    rev: 5.0.4
+    rev: 6.0.0
     hooks:
     -   id: flake8
 
 -   repo: https://github.com/pre-commit/mirrors-mypy
     rev: v0.991
     hooks:
     -   id: mypy
```

### Comparing `ape-etherscan-0.6.6/CONTRIBUTING.md` & `ape-etherscan-0.6.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.6/LICENSE` & `ape-etherscan-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.6/PKG-INFO` & `ape-etherscan-0.6.7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,131 +1,16 @@
 Metadata-Version: 2.1
 Name: ape-etherscan
-Version: 0.6.6
+Version: 0.6.7
 Summary: ape-etherscan: Etherscan Explorer Plugin for Ethereum-based networks
 Home-page: https://github.com/ApeWorX/ape-etherscan
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
-Description: # Quick Start
-        
-        The following blockchain explorers are supported in this plugin:
-        
-        - [Etherscan](https://etherscan.io/) for Ethereum networks.
-        - [Ftmscan](https://ftmscan.com) for Fantom networks.
-        - [Arbiscan](https://arbiscan.io) for Arbitrum networks.
-        - [Optimistic Etherscan](https://optimistic.etherscan.io) for Optimism networks.
-        - [Polygonscan](https://polygonscan.com) for Polygon networks.
-        - [Polygonscan ZkEVM](https://zkevm.polygonscan.com) for Polygon ZkEVM networks.
-        - [Snowtrace](https://snowtrace.io) for Avalanche networks.
-        - [Basescan](https://basescan.org) for Base networks.
-        - [Bscscan](https://bscscan.com) for Binance-Smart-Chain networks.
-        
-        ## Dependencies
-        
-        - [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
-        
-        ## Installation
-        
-        ### via `pip`
-        
-        You can install the latest release via [`pip`](https://pypi.org/project/pip/):
-        
-        ```bash
-        pip install ape-etherscan
-        ```
-        
-        ### via `setuptools`
-        
-        You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
-        
-        ```bash
-        git clone https://github.com/ApeWorX/ape-etherscan.git
-        cd ape-etherscan
-        python3 setup.py install
-        ```
-        
-        ## Quick Usage
-        
-        ## Set up the environment
-        
-        Specify API keys as environment variables. You could put them in your shell's config like `~/.profile`
-        or use a tool like [direnv](https://direnv.net/) and store them locally in `.envrc`.
-        
-        You can also specify multiple comma-separated keys, a random key will be chosen for each request.
-        This could be useful if you hit API rate limits.
-        
-        You can obtain an API key by registering with Etherscan and visiting [this page](https://etherscan.io/myapikey).
-        
-        ```bash
-        export ETHERSCAN_API_KEY=SAMPLE_KEY
-        export FTMSCAN_API_KEY=SAMPLE_KEY
-        export ARBISCAN_API_KEY=SAMPLE_KEY
-        export POLYGON_ZKEVM_ETHERSCAN_API_KEY=SAMPLE_KEY
-        export BASESCAN_API_KEY=SAMPLE_KEY
-        ```
-        
-        ## Transaction URLs
-        
-        When you have this plugin installed, Etherscan explorer URLs appear in CLI output.
-        
-        ```bash
-        INFO: Submitted 0x123321123321123321123321123aaaadaaaee4b2aaa07901b80716cc357a9646
-        etherscan URL: https://rinkeby.etherscan.io/tx/0x123321123321123321123321123aaaadaaaee4b2aaa07901b80716cc357a9646
-        ```
-        
-        ## Contract Types
-        
-        The `ape-etherscan` plugin also assists in fetching `contract_types`.
-        Use the `Contract` top-level construct to create contract instances.
-        When the explorer plugin locates a contract type for a given address, the `Contract` return-value uses that contract type.
-        
-        ```python
-        from ape import accounts, Contract
-        
-        contract = Contract("0x55a8a39bc9694714e2874c1ce77aa1e599461e18")
-        receipt = contract.call_mutable_method("arg0", sender=accounts.load("acct"))
-        ```
-        
-        The first line `contract = Contract("0x55a8a39bc9694714e2874c1ce77aa1e599461e18")` checks if ape has a cached contract-type for the address `0x55a8a39bc9694714e2874c1ce77aa1e599461e18`.
-        If it does not find a cached contract type, it uses an explorer plugin to attempt to find one.
-        If found, the contract type is then cached to disk and in memory for the active session so that subsequent invocations don't require HTTP calls.
-        The return value from `Contract` is a `ContractInstance`, so it is connected to your active provider and ready for transactions.
-        
-        **NOTE**: Vyper contracts from Etherscan always return the name `Vyper_contract`.
-        However, if the plugin detects that the contract type has a method named `symbol`, it will use the return value from that call instead.
-        
-        ## Contract Verification
-        
-        Use the `ape-etherscan` plugin to publish and verify your contracts.
-        Contract verification associates a contract type from Ape with an Ethereum address on Etherscan.
-        Learn more about Etherscan verification [here](https://info.etherscan.com/types-of-contract-verification/).
-        
-        To verify contract in Ape, you can set the `publish` key to `True` when deploying:
-        
-        ```python
-        from ape import accounts, project
-        
-        account = accounts.load("testnetacct")
-        account.deploy(project.MyContract, publish=True)
-        ```
-        
-        You can also use the explorer class directly to publish at a later time:
-        
-        ```python
-        from ape import networks
-        
-        etherscan = networks.provider.network.explorer
-        etherscan.publish_contract("0x55a8a39bc9694714e2874c1ce77aa1e599461e18")
-        ```
-        
-        **NOTE**: You must set an Etherscan API key environment variable to use the publishing feature.
-        
 Keywords: ethereum
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
@@ -136,7 +21,122 @@
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: doc
 Provides-Extra: release
 Provides-Extra: dev
+License-File: LICENSE
+
+# Quick Start
+
+The following blockchain explorers are supported in this plugin:
+
+- [Etherscan](https://etherscan.io/) for Ethereum networks.
+- [Ftmscan](https://ftmscan.com) for Fantom networks.
+- [Arbiscan](https://arbiscan.io) for Arbitrum networks.
+- [Optimistic Etherscan](https://optimistic.etherscan.io) for Optimism networks.
+- [Polygonscan](https://polygonscan.com) for Polygon networks.
+- [Polygonscan ZkEVM](https://zkevm.polygonscan.com) for Polygon ZkEVM networks.
+- [Snowtrace](https://snowtrace.io) for Avalanche networks.
+- [Basescan](https://basescan.org) for Base networks.
+- [Bscscan](https://bscscan.com) for Binance-Smart-Chain networks.
+
+## Dependencies
+
+- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+
+## Installation
+
+### via `pip`
+
+You can install the latest release via [`pip`](https://pypi.org/project/pip/):
+
+```bash
+pip install ape-etherscan
+```
+
+### via `setuptools`
+
+You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
+
+```bash
+git clone https://github.com/ApeWorX/ape-etherscan.git
+cd ape-etherscan
+python3 setup.py install
+```
+
+## Quick Usage
+
+## Set up the environment
+
+Specify API keys as environment variables. You could put them in your shell's config like `~/.profile`
+or use a tool like [direnv](https://direnv.net/) and store them locally in `.envrc`.
+
+You can also specify multiple comma-separated keys, a random key will be chosen for each request.
+This could be useful if you hit API rate limits.
+
+You can obtain an API key by registering with Etherscan and visiting [this page](https://etherscan.io/myapikey).
+
+```bash
+export ETHERSCAN_API_KEY=SAMPLE_KEY
+export FTMSCAN_API_KEY=SAMPLE_KEY
+export ARBISCAN_API_KEY=SAMPLE_KEY
+export POLYGON_ZKEVM_ETHERSCAN_API_KEY=SAMPLE_KEY
+export BASESCAN_API_KEY=SAMPLE_KEY
+```
+
+## Transaction URLs
+
+When you have this plugin installed, Etherscan explorer URLs appear in CLI output.
+
+```bash
+INFO: Submitted 0x123321123321123321123321123aaaadaaaee4b2aaa07901b80716cc357a9646
+etherscan URL: https://rinkeby.etherscan.io/tx/0x123321123321123321123321123aaaadaaaee4b2aaa07901b80716cc357a9646
+```
+
+## Contract Types
+
+The `ape-etherscan` plugin also assists in fetching `contract_types`.
+Use the `Contract` top-level construct to create contract instances.
+When the explorer plugin locates a contract type for a given address, the `Contract` return-value uses that contract type.
+
+```python
+from ape import accounts, Contract
+
+contract = Contract("0x55a8a39bc9694714e2874c1ce77aa1e599461e18")
+receipt = contract.call_mutable_method("arg0", sender=accounts.load("acct"))
+```
+
+The first line `contract = Contract("0x55a8a39bc9694714e2874c1ce77aa1e599461e18")` checks if ape has a cached contract-type for the address `0x55a8a39bc9694714e2874c1ce77aa1e599461e18`.
+If it does not find a cached contract type, it uses an explorer plugin to attempt to find one.
+If found, the contract type is then cached to disk and in memory for the active session so that subsequent invocations don't require HTTP calls.
+The return value from `Contract` is a `ContractInstance`, so it is connected to your active provider and ready for transactions.
+
+**NOTE**: Vyper contracts from Etherscan always return the name `Vyper_contract`.
+However, if the plugin detects that the contract type has a method named `symbol`, it will use the return value from that call instead.
+
+## Contract Verification
+
+Use the `ape-etherscan` plugin to publish and verify your contracts.
+Contract verification associates a contract type from Ape with an Ethereum address on Etherscan.
+Learn more about Etherscan verification [here](https://info.etherscan.com/types-of-contract-verification/).
+
+To verify contract in Ape, you can set the `publish` key to `True` when deploying:
+
+```python
+from ape import accounts, project
+
+account = accounts.load("testnetacct")
+account.deploy(project.MyContract, publish=True)
+```
+
+You can also use the explorer class directly to publish at a later time:
+
+```python
+from ape import networks
+
+etherscan = networks.provider.network.explorer
+etherscan.publish_contract("0x55a8a39bc9694714e2874c1ce77aa1e599461e18")
+```
+
+**NOTE**: You must set an Etherscan API key environment variable to use the publishing feature.
```

### Comparing `ape-etherscan-0.6.6/README.md` & `ape-etherscan-0.6.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 - [Polygonscan ZkEVM](https://zkevm.polygonscan.com) for Polygon ZkEVM networks.
 - [Snowtrace](https://snowtrace.io) for Avalanche networks.
 - [Basescan](https://basescan.org) for Base networks.
 - [Bscscan](https://bscscan.com) for Binance-Smart-Chain networks.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
+- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ape-etherscan-0.6.6/ape_etherscan/__init__.py` & `ape-etherscan-0.6.7/ape_etherscan/__init__.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.6/ape_etherscan/client.py` & `ape-etherscan-0.6.7/ape_etherscan/client.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.6/ape_etherscan/config.py` & `ape-etherscan-0.6.7/ape_etherscan/config.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.6/ape_etherscan/exceptions.py` & `ape-etherscan-0.6.7/ape_etherscan/exceptions.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.6/ape_etherscan/explorer.py` & `ape-etherscan-0.6.7/ape_etherscan/explorer.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.6/ape_etherscan/query.py` & `ape-etherscan-0.6.7/ape_etherscan/query.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.6/ape_etherscan/types.py` & `ape-etherscan-0.6.7/ape_etherscan/types.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.6/ape_etherscan/utils.py` & `ape-etherscan-0.6.7/ape_etherscan/utils.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.6/ape_etherscan/verify.py` & `ape-etherscan-0.6.7/ape_etherscan/verify.py`

 * *Files 2% similar despite different names*

```diff
@@ -304,14 +304,19 @@
                 sources[imported_source_id] = {
                     "content": (base_dir / imported_source_id).read_text()
                 }
                 build_map(imported_source_id)
 
         build_map(source_id)
 
+        # "libraries" field not allows in `settings` dict.
+        if "libraries" in settings:
+            # libraries are handled below.
+            settings.pop("libraries")
+
         data = {
             "language": compiler.name.capitalize(),
             "sources": sources,
             "settings": settings,
         }
         if hasattr(compiler, "libraries") and compiler.libraries:
             libraries = compiler.libraries
```

### Comparing `ape-etherscan-0.6.6/ape_etherscan.egg-info/PKG-INFO` & `ape-etherscan-0.6.7/ape_etherscan.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,131 +1,16 @@
 Metadata-Version: 2.1
 Name: ape-etherscan
-Version: 0.6.6
+Version: 0.6.7
 Summary: ape-etherscan: Etherscan Explorer Plugin for Ethereum-based networks
 Home-page: https://github.com/ApeWorX/ape-etherscan
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
-Description: # Quick Start
-        
-        The following blockchain explorers are supported in this plugin:
-        
-        - [Etherscan](https://etherscan.io/) for Ethereum networks.
-        - [Ftmscan](https://ftmscan.com) for Fantom networks.
-        - [Arbiscan](https://arbiscan.io) for Arbitrum networks.
-        - [Optimistic Etherscan](https://optimistic.etherscan.io) for Optimism networks.
-        - [Polygonscan](https://polygonscan.com) for Polygon networks.
-        - [Polygonscan ZkEVM](https://zkevm.polygonscan.com) for Polygon ZkEVM networks.
-        - [Snowtrace](https://snowtrace.io) for Avalanche networks.
-        - [Basescan](https://basescan.org) for Base networks.
-        - [Bscscan](https://bscscan.com) for Binance-Smart-Chain networks.
-        
-        ## Dependencies
-        
-        - [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
-        
-        ## Installation
-        
-        ### via `pip`
-        
-        You can install the latest release via [`pip`](https://pypi.org/project/pip/):
-        
-        ```bash
-        pip install ape-etherscan
-        ```
-        
-        ### via `setuptools`
-        
-        You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
-        
-        ```bash
-        git clone https://github.com/ApeWorX/ape-etherscan.git
-        cd ape-etherscan
-        python3 setup.py install
-        ```
-        
-        ## Quick Usage
-        
-        ## Set up the environment
-        
-        Specify API keys as environment variables. You could put them in your shell's config like `~/.profile`
-        or use a tool like [direnv](https://direnv.net/) and store them locally in `.envrc`.
-        
-        You can also specify multiple comma-separated keys, a random key will be chosen for each request.
-        This could be useful if you hit API rate limits.
-        
-        You can obtain an API key by registering with Etherscan and visiting [this page](https://etherscan.io/myapikey).
-        
-        ```bash
-        export ETHERSCAN_API_KEY=SAMPLE_KEY
-        export FTMSCAN_API_KEY=SAMPLE_KEY
-        export ARBISCAN_API_KEY=SAMPLE_KEY
-        export POLYGON_ZKEVM_ETHERSCAN_API_KEY=SAMPLE_KEY
-        export BASESCAN_API_KEY=SAMPLE_KEY
-        ```
-        
-        ## Transaction URLs
-        
-        When you have this plugin installed, Etherscan explorer URLs appear in CLI output.
-        
-        ```bash
-        INFO: Submitted 0x123321123321123321123321123aaaadaaaee4b2aaa07901b80716cc357a9646
-        etherscan URL: https://rinkeby.etherscan.io/tx/0x123321123321123321123321123aaaadaaaee4b2aaa07901b80716cc357a9646
-        ```
-        
-        ## Contract Types
-        
-        The `ape-etherscan` plugin also assists in fetching `contract_types`.
-        Use the `Contract` top-level construct to create contract instances.
-        When the explorer plugin locates a contract type for a given address, the `Contract` return-value uses that contract type.
-        
-        ```python
-        from ape import accounts, Contract
-        
-        contract = Contract("0x55a8a39bc9694714e2874c1ce77aa1e599461e18")
-        receipt = contract.call_mutable_method("arg0", sender=accounts.load("acct"))
-        ```
-        
-        The first line `contract = Contract("0x55a8a39bc9694714e2874c1ce77aa1e599461e18")` checks if ape has a cached contract-type for the address `0x55a8a39bc9694714e2874c1ce77aa1e599461e18`.
-        If it does not find a cached contract type, it uses an explorer plugin to attempt to find one.
-        If found, the contract type is then cached to disk and in memory for the active session so that subsequent invocations don't require HTTP calls.
-        The return value from `Contract` is a `ContractInstance`, so it is connected to your active provider and ready for transactions.
-        
-        **NOTE**: Vyper contracts from Etherscan always return the name `Vyper_contract`.
-        However, if the plugin detects that the contract type has a method named `symbol`, it will use the return value from that call instead.
-        
-        ## Contract Verification
-        
-        Use the `ape-etherscan` plugin to publish and verify your contracts.
-        Contract verification associates a contract type from Ape with an Ethereum address on Etherscan.
-        Learn more about Etherscan verification [here](https://info.etherscan.com/types-of-contract-verification/).
-        
-        To verify contract in Ape, you can set the `publish` key to `True` when deploying:
-        
-        ```python
-        from ape import accounts, project
-        
-        account = accounts.load("testnetacct")
-        account.deploy(project.MyContract, publish=True)
-        ```
-        
-        You can also use the explorer class directly to publish at a later time:
-        
-        ```python
-        from ape import networks
-        
-        etherscan = networks.provider.network.explorer
-        etherscan.publish_contract("0x55a8a39bc9694714e2874c1ce77aa1e599461e18")
-        ```
-        
-        **NOTE**: You must set an Etherscan API key environment variable to use the publishing feature.
-        
 Keywords: ethereum
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
@@ -136,7 +21,122 @@
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: doc
 Provides-Extra: release
 Provides-Extra: dev
+License-File: LICENSE
+
+# Quick Start
+
+The following blockchain explorers are supported in this plugin:
+
+- [Etherscan](https://etherscan.io/) for Ethereum networks.
+- [Ftmscan](https://ftmscan.com) for Fantom networks.
+- [Arbiscan](https://arbiscan.io) for Arbitrum networks.
+- [Optimistic Etherscan](https://optimistic.etherscan.io) for Optimism networks.
+- [Polygonscan](https://polygonscan.com) for Polygon networks.
+- [Polygonscan ZkEVM](https://zkevm.polygonscan.com) for Polygon ZkEVM networks.
+- [Snowtrace](https://snowtrace.io) for Avalanche networks.
+- [Basescan](https://basescan.org) for Base networks.
+- [Bscscan](https://bscscan.com) for Binance-Smart-Chain networks.
+
+## Dependencies
+
+- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+
+## Installation
+
+### via `pip`
+
+You can install the latest release via [`pip`](https://pypi.org/project/pip/):
+
+```bash
+pip install ape-etherscan
+```
+
+### via `setuptools`
+
+You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
+
+```bash
+git clone https://github.com/ApeWorX/ape-etherscan.git
+cd ape-etherscan
+python3 setup.py install
+```
+
+## Quick Usage
+
+## Set up the environment
+
+Specify API keys as environment variables. You could put them in your shell's config like `~/.profile`
+or use a tool like [direnv](https://direnv.net/) and store them locally in `.envrc`.
+
+You can also specify multiple comma-separated keys, a random key will be chosen for each request.
+This could be useful if you hit API rate limits.
+
+You can obtain an API key by registering with Etherscan and visiting [this page](https://etherscan.io/myapikey).
+
+```bash
+export ETHERSCAN_API_KEY=SAMPLE_KEY
+export FTMSCAN_API_KEY=SAMPLE_KEY
+export ARBISCAN_API_KEY=SAMPLE_KEY
+export POLYGON_ZKEVM_ETHERSCAN_API_KEY=SAMPLE_KEY
+export BASESCAN_API_KEY=SAMPLE_KEY
+```
+
+## Transaction URLs
+
+When you have this plugin installed, Etherscan explorer URLs appear in CLI output.
+
+```bash
+INFO: Submitted 0x123321123321123321123321123aaaadaaaee4b2aaa07901b80716cc357a9646
+etherscan URL: https://rinkeby.etherscan.io/tx/0x123321123321123321123321123aaaadaaaee4b2aaa07901b80716cc357a9646
+```
+
+## Contract Types
+
+The `ape-etherscan` plugin also assists in fetching `contract_types`.
+Use the `Contract` top-level construct to create contract instances.
+When the explorer plugin locates a contract type for a given address, the `Contract` return-value uses that contract type.
+
+```python
+from ape import accounts, Contract
+
+contract = Contract("0x55a8a39bc9694714e2874c1ce77aa1e599461e18")
+receipt = contract.call_mutable_method("arg0", sender=accounts.load("acct"))
+```
+
+The first line `contract = Contract("0x55a8a39bc9694714e2874c1ce77aa1e599461e18")` checks if ape has a cached contract-type for the address `0x55a8a39bc9694714e2874c1ce77aa1e599461e18`.
+If it does not find a cached contract type, it uses an explorer plugin to attempt to find one.
+If found, the contract type is then cached to disk and in memory for the active session so that subsequent invocations don't require HTTP calls.
+The return value from `Contract` is a `ContractInstance`, so it is connected to your active provider and ready for transactions.
+
+**NOTE**: Vyper contracts from Etherscan always return the name `Vyper_contract`.
+However, if the plugin detects that the contract type has a method named `symbol`, it will use the return value from that call instead.
+
+## Contract Verification
+
+Use the `ape-etherscan` plugin to publish and verify your contracts.
+Contract verification associates a contract type from Ape with an Ethereum address on Etherscan.
+Learn more about Etherscan verification [here](https://info.etherscan.com/types-of-contract-verification/).
+
+To verify contract in Ape, you can set the `publish` key to `True` when deploying:
+
+```python
+from ape import accounts, project
+
+account = accounts.load("testnetacct")
+account.deploy(project.MyContract, publish=True)
+```
+
+You can also use the explorer class directly to publish at a later time:
+
+```python
+from ape import networks
+
+etherscan = networks.provider.network.explorer
+etherscan.publish_contract("0x55a8a39bc9694714e2874c1ce77aa1e599461e18")
+```
+
+**NOTE**: You must set an Etherscan API key environment variable to use the publishing feature.
```

### Comparing `ape-etherscan-0.6.6/ape_etherscan.egg-info/SOURCES.txt` & `ape-etherscan-0.6.7/ape_etherscan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.6/ape_etherscan.egg-info/requires.txt` & `ape-etherscan-0.6.7/ape_etherscan.egg-info/requires.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-eth-ape<0.7,>=0.6.7
+eth-ape<0.7,>=0.6.11
 requests
 
 [dev]
 ape-arbitrum
 ape-base
 ape-bsc
 ape-fantom
 ape-optimism
 ape-polygon
-ape-polygon
+ape-polygon-zkevm
 ape-infura
 ape-solidity
 pytest>=6.0
 pytest-xdist
 pytest-cov
 hypothesis<7,>=6.2.0
 pytest-mock
-black>=23.3.0
+black<24,>=23.3.0
 mypy<1,>=0.991
 types-requests>=2.28.7
 types-setuptools
-flake8>=5.0.4
-isort>=5.10.1
+flake8<7,>=6.0.0
+isort<6,>=5.10.1
 mdformat>=0.7.16
 mdformat-gfm>=0.3.5
 mdformat-frontmatter>=0.4.1
 Sphinx<4,>=3.4.3
 sphinx_rtd_theme<1,>=0.1.9
 towncrier<20,>=19.2.0
 setuptools
@@ -40,20 +40,20 @@
 
 [doc]
 Sphinx<4,>=3.4.3
 sphinx_rtd_theme<1,>=0.1.9
 towncrier<20,>=19.2.0
 
 [lint]
-black>=23.3.0
+black<24,>=23.3.0
 mypy<1,>=0.991
 types-requests>=2.28.7
 types-setuptools
-flake8>=5.0.4
-isort>=5.10.1
+flake8<7,>=6.0.0
+isort<6,>=5.10.1
 mdformat>=0.7.16
 mdformat-gfm>=0.3.5
 mdformat-frontmatter>=0.4.1
 
 [release]
 setuptools
 setuptools-scm
@@ -63,15 +63,15 @@
 [test]
 ape-arbitrum
 ape-base
 ape-bsc
 ape-fantom
 ape-optimism
 ape-polygon
-ape-polygon
+ape-polygon-zkevm
 ape-infura
 ape-solidity
 pytest>=6.0
 pytest-xdist
 pytest-cov
 hypothesis<7,>=6.2.0
 pytest-mock
```

### Comparing `ape-etherscan-0.6.6/pyproject.toml` & `ape-etherscan-0.6.7/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # NOTE: you have to use single-quoted strings in TOML for regular expressions.
 # It's the equivalent of r-strings in Python.  Multiline strings are treated as
 # verbose regular expressions by Black.  Use [ ] to denote a significant space
 # character.
 
 [tool.black]
 line-length = 100
-target-version = ['py38', 'py39', 'py310']
+target-version = ['py38', 'py39', 'py310', 'py311']
 include = '\.pyi?$'
 
 [tool.pytest.ini_options]
 addopts = """
     -p no:ape_test
     --cov-branch
     --cov-report term
```

### Comparing `ape-etherscan-0.6.6/setup.py` & `ape-etherscan-0.6.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,30 +6,30 @@
     "test": [  # `test` GitHub Action jobs uses this
         "ape-arbitrum",  # Needed for Arbitrum integration
         "ape-base",  # Needed for Base networks integration
         "ape-bsc",  # For testing BSC integration
         "ape-fantom",  # For testing Fantom integration
         "ape-optimism",  # Needed for Optimism integration
         "ape-polygon",  # Needed for Polygon integration
-        "ape-polygon",  # Needed for Polygon ZkEVM integration
+        "ape-polygon-zkevm",  # Needed for Polygon ZkEVM integration
         "ape-infura",  # Needed for live network tests
         "ape-solidity",  # Needed for contract verification tests
         "pytest>=6.0",  # Core testing package
         "pytest-xdist",  # multi-process runner
         "pytest-cov",  # Coverage analyzer plugin
         "hypothesis>=6.2.0,<7",  # Strategy-based fuzzer
         "pytest-mock",  # Test mocker
     ],
     "lint": [
-        "black>=23.3.0",  # auto-formatter and linter
+        "black>=23.3.0,<24",  # auto-formatter and linter
         "mypy>=0.991,<1",  # Static type analyzer
         "types-requests>=2.28.7",  # Needed due to mypy typeshed
         "types-setuptools",  # Needed due to mypy typeshed
-        "flake8>=5.0.4",  # Style linter
-        "isort>=5.10.1",  # Import sorting linter
+        "flake8>=6.0.0,<7",  # Style linter
+        "isort>=5.10.1,<6",  # Import sorting linter
         "mdformat>=0.7.16",  # Auto-formatter for markdown
         "mdformat-gfm>=0.3.5",  # Needed for formatting GitHub-flavored markdown
         "mdformat-frontmatter>=0.4.1",  # Needed for frontmatters-style headers in issue templates
     ],
     "doc": [
         "Sphinx>=3.4.3,<4",  # Documentation generator
         "sphinx_rtd_theme>=0.1.9,<1",  # Readthedocs.org theme
@@ -71,15 +71,15 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/ape-etherscan",
     include_package_data=True,
     install_requires=[
-        "eth-ape>=0.6.7,<0.7",
+        "eth-ape>=0.6.11,<0.7",
         "requests",  # Use same version as eth-ape
     ],
     python_requires=">=3.8,<4",
     extras_require=extras_require,
     py_modules=["ape_etherscan"],
     license="Apache-2.0",
     zip_safe=False,
```

### Comparing `ape-etherscan-0.6.6/tests/conftest.py` & `ape-etherscan-0.6.7/tests/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import ape
 import pytest
 from ape.api import ExplorerAPI
 from ape.exceptions import NetworkError
 from ape.logging import logger
 from ape.types import AddressType
 from ape.utils import cached_property
+from ape_solidity._utils import OUTPUT_SELECTION
 from requests import Response
 
 from ape_etherscan import Etherscan
 from ape_etherscan.client import _APIClient
 from ape_etherscan.types import EtherscanResponse
 
 ape.config.DATA_FOLDER = Path(mkdtemp()).resolve()
@@ -80,16 +81,16 @@
     "sources": {
         "foo.sol": {"content": FOO_SOURCE_CODE},
         ".cache/bar/local/bar.sol": {"content": BAR_SOURCE_CODE},
     },
     "settings": {
         "optimizer": {"enabled": True, "runs": 200},
         "outputSelection": {
-            "foo.sol": {"foo": ["abi", "bin", "bin-runtime", "devdoc", "userdoc", "srcmap"]},
-            "bar.sol": {"bar": ["abi", "bin", "bin-runtime", "devdoc", "userdoc", "srcmap"]},
+            "subcontracts/foo.sol": {"*": OUTPUT_SELECTION, "": ["ast"]},
+            ".cache/bar/local/bar.sol": {"*": OUTPUT_SELECTION, "": ["ast"]},
         },
         "remappings": ["@bar=.cache/bar/local"],
     },
     "libraryname1": "MyLib",
     "libraryaddress1": "0x274b028b03A250cA03644E6c578D81f019eE1323",
 }
 
@@ -416,15 +417,15 @@
             setattr(response, key, val)
 
         return response
 
 
 @pytest.fixture
 def verification_params(address_to_verify):
-    ctor_args = "00002833623465633162323163303133643932303665363338366532313839353566356166306565336362000000000000000000000000000000000000000000000000"  # noqa: E501
+    ctor_args = "000000000000000000000000000000000000000000000000000000000000002833623465633162323163303133643932303665363338366532313839353566356166306565336362000000000000000000000000000000000000000000000000"  # noqa: E501
 
     return {
         "action": "verifysourcecode",
         "codeformat": "solidity-standard-json-input",
         "constructorArguements": ctor_args,
         "contractaddress": address_to_verify,
         "contractname": "foo.sol:foo",
```

### Comparing `ape-etherscan-0.6.6/tests/mock_responses/get_account_transactions.json` & `ape-etherscan-0.6.7/tests/mock_responses/get_account_transactions.json`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.6/tests/mock_responses/get_contract_response.json` & `ape-etherscan-0.6.7/tests/mock_responses/get_contract_response.json`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.6/tests/mock_responses/get_proxy_contract_response.json` & `ape-etherscan-0.6.7/tests/mock_responses/get_proxy_contract_response.json`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.6/tests/mock_responses/get_vyper_contract_response.json` & `ape-etherscan-0.6.7/tests/mock_responses/get_vyper_contract_response.json`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.6/tests/test_etherscan.py` & `ape-etherscan-0.6.7/tests/test_etherscan.py`

 * *Files identical despite different names*

