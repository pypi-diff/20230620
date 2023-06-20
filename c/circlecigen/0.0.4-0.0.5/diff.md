# Comparing `tmp/circlecigen-0.0.4.tar.gz` & `tmp/circlecigen-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circlecigen-0.0.4.tar", last modified: Mon Jun 19 15:35:52 2023, max compression
+gzip compressed data, was "circlecigen-0.0.5.tar", last modified: Tue Jun 20 04:07:01 2023, max compression
```

## Comparing `circlecigen-0.0.4.tar` & `circlecigen-0.0.5.tar`

### file list

```diff
@@ -1,55 +1,57 @@
-drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-19 15:35:52.652210 circlecigen-0.0.4/
-drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-19 15:35:52.648210 circlecigen-0.0.4/.circleci/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4013 2023-06-19 15:35:47.000000 circlecigen-0.0.4/.circleci/config.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      350 2023-06-19 15:35:47.000000 circlecigen-0.0.4/.codeclimate.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2023-06-19 15:35:47.000000 circlecigen-0.0.4/.gitignore
--rw-r--r--   0 circleci  (3434) circleci  (3434)      866 2023-06-19 15:35:47.000000 circlecigen-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)    18369 2023-06-19 15:35:47.000000 circlecigen-0.0.4/.pylintrc
--rw-r--r--   0 circleci  (3434) circleci  (3434)        7 2023-06-19 15:35:47.000000 circlecigen-0.0.4/.python-version
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1075 2023-06-19 15:35:47.000000 circlecigen-0.0.4/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)    22062 2023-06-19 15:35:52.652210 circlecigen-0.0.4/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      432 2023-06-19 15:35:47.000000 circlecigen-0.0.4/Pipfile
--rw-r--r--   0 circleci  (3434) circleci  (3434)    21426 2023-06-19 15:35:47.000000 circlecigen-0.0.4/README.md
-drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-19 15:35:52.648210 circlecigen-0.0.4/env_test/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3037 2023-06-19 15:35:47.000000 circlecigen-0.0.4/env_test/config.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)       82 2023-06-19 15:35:47.000000 circlecigen-0.0.4/env_test/default.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)       39 2023-06-19 15:35:47.000000 circlecigen-0.0.4/env_test/dev.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5415 2023-06-19 15:35:47.000000 circlecigen-0.0.4/env_test/generated_config.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      782 2023-06-19 15:35:47.000000 circlecigen-0.0.4/env_test/multi.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      146 2023-06-19 15:35:47.000000 circlecigen-0.0.4/env_test/nonprod-us-east-2.tfvars.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      146 2023-06-19 15:35:47.000000 circlecigen-0.0.4/env_test/nonprod-us-west-2.tfvars.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)       43 2023-06-19 15:35:47.000000 circlecigen-0.0.4/env_test/nonprod.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      556 2023-06-19 15:35:47.000000 circlecigen-0.0.4/env_test/post-approve.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      312 2023-06-19 15:35:47.000000 circlecigen-0.0.4/env_test/pre-approve.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      140 2023-06-19 15:35:47.000000 circlecigen-0.0.4/env_test/prod-us-east-2.tfvars.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      140 2023-06-19 15:35:47.000000 circlecigen-0.0.4/env_test/prod-us-west-2.tfvars.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)       40 2023-06-19 15:35:47.000000 circlecigen-0.0.4/env_test/prod.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      313 2023-06-19 15:35:47.000000 circlecigen-0.0.4/notes.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      246 2023-06-19 15:35:47.000000 circlecigen-0.0.4/op.env
--rw-r--r--   0 circleci  (3434) circleci  (3434)      711 2023-06-19 15:35:47.000000 circlecigen-0.0.4/pyproject.toml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      365 2023-06-19 15:35:47.000000 circlecigen-0.0.4/requirements.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-06-19 15:35:52.652210 circlecigen-0.0.4/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      791 2023-06-19 15:35:47.000000 circlecigen-0.0.4/setup.py
-drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-19 15:35:52.652210 circlecigen-0.0.4/src/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-19 15:35:47.000000 circlecigen-0.0.4/src/__init__.py
-drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-19 15:35:52.652210 circlecigen-0.0.4/src/circlecigen.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    22062 2023-06-19 15:35:52.000000 circlecigen-0.0.4/src/circlecigen.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1088 2023-06-19 15:35:52.000000 circlecigen-0.0.4/src/circlecigen.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-06-19 15:35:52.000000 circlecigen-0.0.4/src/circlecigen.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       48 2023-06-19 15:35:52.000000 circlecigen-0.0.4/src/circlecigen.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-06-19 15:35:52.000000 circlecigen-0.0.4/src/circlecigen.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2573 2023-06-19 15:35:47.000000 circlecigen-0.0.4/src/circlecigen.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5572 2023-06-19 15:35:47.000000 circlecigen-0.0.4/src/template.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2091 2023-06-19 15:35:47.000000 circlecigen-0.0.4/src/tfvars.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      808 2023-06-19 15:35:47.000000 circlecigen-0.0.4/src/utils.py
-drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-19 15:35:52.652210 circlecigen-0.0.4/test/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5415 2023-06-19 15:35:47.000000 circlecigen-0.0.4/test/generated_config.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1592 2023-06-19 15:35:47.000000 circlecigen-0.0.4/test/generated_config_setup.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      146 2023-06-19 15:35:47.000000 circlecigen-0.0.4/test/nonprod-us-east-2.tfvars.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      146 2023-06-19 15:35:47.000000 circlecigen-0.0.4/test/nonprod-us-west-2.tfvars.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      140 2023-06-19 15:35:47.000000 circlecigen-0.0.4/test/prod-us-east-2.tfvars.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      140 2023-06-19 15:35:47.000000 circlecigen-0.0.4/test/prod-us-west-2.tfvars.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2262 2023-06-19 15:35:47.000000 circlecigen-0.0.4/test/test_circlecigen.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2334 2023-06-19 15:35:47.000000 circlecigen-0.0.4/test/test_template.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2336 2023-06-19 15:35:47.000000 circlecigen-0.0.4/test/test_tfvars.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1486 2023-06-19 15:35:47.000000 circlecigen-0.0.4/test/test_utils.py
+drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-20 04:07:01.712526 circlecigen-0.0.5/
+drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-20 04:07:01.708527 circlecigen-0.0.5/.circleci/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3975 2023-06-20 04:06:42.000000 circlecigen-0.0.5/.circleci/config.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      350 2023-06-20 04:06:42.000000 circlecigen-0.0.5/.codeclimate.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2023-06-20 04:06:42.000000 circlecigen-0.0.5/.gitignore
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      866 2023-06-20 04:06:42.000000 circlecigen-0.0.5/.pre-commit-config.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    18369 2023-06-20 04:06:42.000000 circlecigen-0.0.5/.pylintrc
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        7 2023-06-20 04:06:42.000000 circlecigen-0.0.5/.python-version
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1075 2023-06-20 04:06:42.000000 circlecigen-0.0.5/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    22357 2023-06-20 04:07:01.712526 circlecigen-0.0.5/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      432 2023-06-20 04:06:42.000000 circlecigen-0.0.5/Pipfile
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    21721 2023-06-20 04:06:42.000000 circlecigen-0.0.5/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-20 04:06:42.000000 circlecigen-0.0.5/__init__.py
+drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-20 04:07:01.708527 circlecigen-0.0.5/circlecigen.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    22357 2023-06-20 04:07:01.000000 circlecigen-0.0.5/circlecigen.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1096 2023-06-20 04:07:01.000000 circlecigen-0.0.5/circlecigen.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-06-20 04:07:01.000000 circlecigen-0.0.5/circlecigen.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       52 2023-06-20 04:07:01.000000 circlecigen-0.0.5/circlecigen.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        4 2023-06-20 04:07:01.000000 circlecigen-0.0.5/circlecigen.egg-info/top_level.txt
+drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-20 04:07:01.708527 circlecigen-0.0.5/env_test/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3037 2023-06-20 04:06:42.000000 circlecigen-0.0.5/env_test/config.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       82 2023-06-20 04:06:42.000000 circlecigen-0.0.5/env_test/default.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       39 2023-06-20 04:06:42.000000 circlecigen-0.0.5/env_test/dev.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5543 2023-06-20 04:06:42.000000 circlecigen-0.0.5/env_test/generated_config.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      782 2023-06-20 04:06:42.000000 circlecigen-0.0.5/env_test/multi.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      146 2023-06-20 04:06:42.000000 circlecigen-0.0.5/env_test/nonprod-us-east-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      146 2023-06-20 04:06:42.000000 circlecigen-0.0.5/env_test/nonprod-us-west-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       43 2023-06-20 04:06:42.000000 circlecigen-0.0.5/env_test/nonprod.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      587 2023-06-20 04:06:42.000000 circlecigen-0.0.5/env_test/post-approve.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      312 2023-06-20 04:06:42.000000 circlecigen-0.0.5/env_test/pre-approve.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      140 2023-06-20 04:06:42.000000 circlecigen-0.0.5/env_test/prod-us-east-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      140 2023-06-20 04:06:42.000000 circlecigen-0.0.5/env_test/prod-us-west-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       40 2023-06-20 04:06:42.000000 circlecigen-0.0.5/env_test/prod.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      313 2023-06-20 04:06:42.000000 circlecigen-0.0.5/notes.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      246 2023-06-20 04:06:42.000000 circlecigen-0.0.5/op.env
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      711 2023-06-20 04:06:42.000000 circlecigen-0.0.5/pyproject.toml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      365 2023-06-20 04:06:42.000000 circlecigen-0.0.5/requirements.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-06-20 04:07:01.712526 circlecigen-0.0.5/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      760 2023-06-20 04:06:42.000000 circlecigen-0.0.5/setup.py
+drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-20 04:07:01.708527 circlecigen-0.0.5/src/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-20 04:06:42.000000 circlecigen-0.0.5/src/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      160 2023-06-20 04:07:01.000000 circlecigen-0.0.5/src/_version.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2585 2023-06-20 04:06:42.000000 circlecigen-0.0.5/src/circlecigen.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5805 2023-06-20 04:06:42.000000 circlecigen-0.0.5/src/template.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2428 2023-06-20 04:06:42.000000 circlecigen-0.0.5/src/tfvars.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      808 2023-06-20 04:06:42.000000 circlecigen-0.0.5/src/utils.py
+drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-20 04:07:01.712526 circlecigen-0.0.5/test/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5543 2023-06-20 04:06:42.000000 circlecigen-0.0.5/test/generated_config.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1592 2023-06-20 04:06:42.000000 circlecigen-0.0.5/test/generated_config_setup.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      146 2023-06-20 04:06:42.000000 circlecigen-0.0.5/test/nonprod-us-east-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      146 2023-06-20 04:06:42.000000 circlecigen-0.0.5/test/nonprod-us-west-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      140 2023-06-20 04:06:42.000000 circlecigen-0.0.5/test/prod-us-east-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      140 2023-06-20 04:06:42.000000 circlecigen-0.0.5/test/prod-us-west-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2266 2023-06-20 04:06:42.000000 circlecigen-0.0.5/test/test_circlecigen.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2338 2023-06-20 04:06:42.000000 circlecigen-0.0.5/test/test_template.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2340 2023-06-20 04:06:42.000000 circlecigen-0.0.5/test/test_tfvars.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1490 2023-06-20 04:06:42.000000 circlecigen-0.0.5/test/test_utils.py
```

### Comparing `circlecigen-0.0.4/.circleci/config.yml` & `circlecigen-0.0.5/.circleci/config.yml`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
       - run:
           name: lint
           command: pylint src
       - run:
           name: unit test
           command: |
             sudo pip install -r requirements.txt
-            PYTHONPATH=.:./src coverage run -m pytest -vv -l
+            coverage run -m pytest -vv -l
             coverage xml --omit='src/test*'
             coverage report
       - run:
           name: report test coverage
           command: |
             cc-test-reporter format-coverage -t coverage.py
             cc-test-reporter upload-coverage
@@ -109,15 +109,15 @@
           env-file: op.env
       - set-credentials:
           environment: test
       - run:
           name: Build
           command: |
             sudo pip install -r requirements.txt
-            PYTHONPATH=.:./src python -m build
+            python -m build
       - run:
           name: upload to test.pypi
           command: python -m twine upload --repository testpypi dist/*
       - persist_to_workspace:
           root: .
           paths:
             - dist/
```

### Comparing `circlecigen-0.0.4/.pre-commit-config.yaml` & `circlecigen-0.0.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.4/.pylintrc` & `circlecigen-0.0.5/.pylintrc`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.4/LICENSE` & `circlecigen-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.4/PKG-INFO` & `circlecigen-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: circlecigen
-Version: 0.0.4
-Summary: Opinionated generation of continuation pipelines
-Home-page: https://github.com/ThoughtWorks-DPS/circlecigen
-Author: Nic Cheneweth
-Author-email: Nic Cheneweth <nchenewe@thoughtworks.com>
-Project-URL: Homepage, https://github.com/ThoughtWorks-DPS/circlecigen
-Project-URL: Bug Tracker, https://github.com/ThoughtWorks-DPS/circlecigen/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <div align="center">
 	<p>
 		<img alt="Thoughtworks Logo" src="https://raw.githubusercontent.com/ThoughtWorks-DPS/static/master/thoughtworks_flamingo_wave.png?sanitize=true" width=200 />
     <br />
 		<img alt="DPS Title" src="https://raw.githubusercontent.com/ThoughtWorks-DPS/static/master/EMPCPlatformStarterKitsImage.png?sanitize=true" width=350/>
 	</p>
   <br />
@@ -271,15 +255,15 @@
 Next, the pipeline files.  
 
 **.circleci/config.yml**  
 Of course you must have the regular circleci pipeline file that responds to triggers and actually forms the basis of the generated pipeline. Everything in this file up through the Jobs: or workflow: directive (whichever comes first) forms the starting point for the generated pipeline.  
 
 **.circleci/pre-approve.yml**  
 
-This file is a template that will be populate with instance specific info when the pipeline is generated from within the config.yml pipeline.  
+This file is a template that will be populate with instance specific info when the pipeline is generated from within the config.yml pipeline. All values in the env_instance.tfvars.json configuration are avaliable to be used in the jinja template. Keep in mind that the same yaml template is used for each role so it will not work to have a value that ONLY exists in a single instance or role if the value appears in the yaml template.    
 
 ```yaml
       - terraform/plan:
           name: {{env_instance}} change plan
           context: << pipeline.parameters.context >>
           workspace: {{env_instance}}
           var-file: {{envpath}}/{{env_instance}}.tfvars.json
@@ -653,8 +637,8 @@
           ...
           filters: *on-tag-main
 
       - terraform/apply:
           name: apply nonprod-ap-southwest-1 change plan
           ...
           filters: *on-tag-main
-```
+```
```

#### html2text {}

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1 Name: circlecigen Version: 0.0.4 Summary: Opinionated
-generation of continuation pipelines Home-page: https://github.com/
-ThoughtWorks-DPS/circlecigen Author: Nic Cheneweth Author-email: Nic Cheneweth
-thoughtworks.com> Project-URL: Homepage, https://github.com/ThoughtWorks-DPS/
-circlecigen Project-URL: Bug Tracker, https://github.com/ThoughtWorks-DPS/
-circlecigen/issues Classifier: Programming Language :: Python :: 3 Classifier:
-License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Requires-Python: >=3.10 Description-Content-Type: text/markdown
-License-File: LICENSE
                              [Thoughtworks Logo]
                                   [DPS Title]
 
                              **** circlecigen ****
 [https://dl.circleci.com/status-badge/img/gh/ThoughtWorks-DPS/circlecigen/tree/
   main.svg?style=shield] [https://img.shields.io/badge/license-MIT-blue.svg]
 
@@ -131,33 +122,37 @@
 generate each specific _instance_.tfvars.json file for use as a -var-file by
 terraform. Next, the pipeline files. **.circleci/config.yml** Of course you
 must have the regular circleci pipeline file that responds to triggers and
 actually forms the basis of the generated pipeline. Everything in this file up
 through the Jobs: or workflow: directive (whichever comes first) forms the
 starting point for the generated pipeline. **.circleci/pre-approve.yml** This
 file is a template that will be populate with instance specific info when the
-pipeline is generated from within the config.yml pipeline. ```yaml - terraform/
-plan: name: {{env_instance}} change plan context: <<
-pipeline.parameters.context >> workspace: {{env_instance}} var-file: {
-{envpath}}/{{env_instance}}.tfvars.json before-terraform: - set-environment
-filters: {{filters}}{{priorapprovalrequired}} ``` The indenting is important.
-This example is using the [twdps/terraform orb](https://circleci.com/developer/
-orbs/orb/twdps/terraform). Note that in the before-terraform parameter you can
-pass any pipeline command found in any orb you have included, but more
-importantly from the config.yaml itself. So, for the infra-dev role,
-circlecigen will create a workflow that runs a terraform plan job using the
-specific, associated _instance_.tfvar.json var-file. Each such instance runs in
-parallel. **.circleci/post-approve.yml** Then specify the job to be run if the
-above plans are approved. ```yaml - terraform/apply: name: apply {
+pipeline is generated from within the config.yml pipeline. All values in the
+env_instance.tfvars.json configuration are avaliable to be used in the jinja
+template. Keep in mind that the same yaml template is used for each role so it
+will not work to have a value that ONLY exists in a single instance or role if
+the value appears in the yaml template. ```yaml - terraform/plan: name: {
 {env_instance}} change plan context: << pipeline.parameters.context >>
 workspace: {{env_instance}} var-file: {{envpath}}/{{env_instance}}.tfvars.json
-before-terraform: - set-environment after-terraform: - after-deployment-
-commands requires: - approve {{role}} changes filters: {{filters}} ``` As you
-can see, this template will run terraform apply, and in addition to running the
-set-environment command before the terraaform plan, it will also run an after-
+before-terraform: - set-environment filters: {{filters}}{
+{priorapprovalrequired}} ``` The indenting is important. This example is using
+the [twdps/terraform orb](https://circleci.com/developer/orbs/orb/twdps/
+terraform). Note that in the before-terraform parameter you can pass any
+pipeline command found in any orb you have included, but more importantly from
+the config.yaml itself. So, for the infra-dev role, circlecigen will create a
+workflow that runs a terraform plan job using the specific, associated
+_instance_.tfvar.json var-file. Each such instance runs in parallel.
+**.circleci/post-approve.yml** Then specify the job to be run if the above
+plans are approved. ```yaml - terraform/apply: name: apply {{env_instance}}
+change plan context: << pipeline.parameters.context >> workspace: {
+{env_instance}} var-file: {{envpath}}/{{env_instance}}.tfvars.json before-
+terraform: - set-environment after-terraform: - after-deployment-commands
+requires: - approve {{role}} changes filters: {{filters}} ``` As you can see,
+this template will run terraform apply, and in addition to running the set-
+environment command before the terraaform plan, it will also run an after-
 deployment-commands after a successful apply. In a real use-case, the after-
 terraform commands are typical integration and functional tests. #### The
 primary config.yml pipeline Below is the basic layout of config.yml where the
 circlecigen package is used to create deployment pipelines used by the
 continuation orb. In this case, as is common in trunk-based development, git-
 push results in deployment to an initial development environment, whereas
 tagging the repository expected to launch a full release pipeline that will
```

### Comparing `circlecigen-0.0.4/README.md` & `circlecigen-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: circlecigen
+Version: 0.0.5
+Summary: Opinionated generation of continuation pipelines
+Home-page: https://github.com/ThoughtWorks-DPS/circlecigen
+Author: Nic Cheneweth
+Author-email: Nic Cheneweth <nchenewe@thoughtworks.com>
+Project-URL: Homepage, https://github.com/ThoughtWorks-DPS/circlecigen
+Project-URL: Bug Tracker, https://github.com/ThoughtWorks-DPS/circlecigen/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <div align="center">
 	<p>
 		<img alt="Thoughtworks Logo" src="https://raw.githubusercontent.com/ThoughtWorks-DPS/static/master/thoughtworks_flamingo_wave.png?sanitize=true" width=200 />
     <br />
 		<img alt="DPS Title" src="https://raw.githubusercontent.com/ThoughtWorks-DPS/static/master/EMPCPlatformStarterKitsImage.png?sanitize=true" width=350/>
 	</p>
   <br />
@@ -255,15 +271,15 @@
 Next, the pipeline files.  
 
 **.circleci/config.yml**  
 Of course you must have the regular circleci pipeline file that responds to triggers and actually forms the basis of the generated pipeline. Everything in this file up through the Jobs: or workflow: directive (whichever comes first) forms the starting point for the generated pipeline.  
 
 **.circleci/pre-approve.yml**  
 
-This file is a template that will be populate with instance specific info when the pipeline is generated from within the config.yml pipeline.  
+This file is a template that will be populate with instance specific info when the pipeline is generated from within the config.yml pipeline. All values in the env_instance.tfvars.json configuration are avaliable to be used in the jinja template. Keep in mind that the same yaml template is used for each role so it will not work to have a value that ONLY exists in a single instance or role if the value appears in the yaml template.    
 
 ```yaml
       - terraform/plan:
           name: {{env_instance}} change plan
           context: << pipeline.parameters.context >>
           workspace: {{env_instance}}
           var-file: {{envpath}}/{{env_instance}}.tfvars.json
@@ -637,8 +653,8 @@
           ...
           filters: *on-tag-main
 
       - terraform/apply:
           name: apply nonprod-ap-southwest-1 change plan
           ...
           filters: *on-tag-main
-```
+```
```

#### html2text {}

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1 Name: circlecigen Version: 0.0.5 Summary: Opinionated
+generation of continuation pipelines Home-page: https://github.com/
+ThoughtWorks-DPS/circlecigen Author: Nic Cheneweth Author-email: Nic Cheneweth
+thoughtworks.com> Project-URL: Homepage, https://github.com/ThoughtWorks-DPS/
+circlecigen Project-URL: Bug Tracker, https://github.com/ThoughtWorks-DPS/
+circlecigen/issues Classifier: Programming Language :: Python :: 3 Classifier:
+License :: OSI Approved :: MIT License Classifier: Operating System :: OS
+Independent Requires-Python: >=3.10 Description-Content-Type: text/markdown
+License-File: LICENSE
                              [Thoughtworks Logo]
                                   [DPS Title]
 
                              **** circlecigen ****
 [https://dl.circleci.com/status-badge/img/gh/ThoughtWorks-DPS/circlecigen/tree/
   main.svg?style=shield] [https://img.shields.io/badge/license-MIT-blue.svg]
 
@@ -122,33 +131,37 @@
 generate each specific _instance_.tfvars.json file for use as a -var-file by
 terraform. Next, the pipeline files. **.circleci/config.yml** Of course you
 must have the regular circleci pipeline file that responds to triggers and
 actually forms the basis of the generated pipeline. Everything in this file up
 through the Jobs: or workflow: directive (whichever comes first) forms the
 starting point for the generated pipeline. **.circleci/pre-approve.yml** This
 file is a template that will be populate with instance specific info when the
-pipeline is generated from within the config.yml pipeline. ```yaml - terraform/
-plan: name: {{env_instance}} change plan context: <<
-pipeline.parameters.context >> workspace: {{env_instance}} var-file: {
-{envpath}}/{{env_instance}}.tfvars.json before-terraform: - set-environment
-filters: {{filters}}{{priorapprovalrequired}} ``` The indenting is important.
-This example is using the [twdps/terraform orb](https://circleci.com/developer/
-orbs/orb/twdps/terraform). Note that in the before-terraform parameter you can
-pass any pipeline command found in any orb you have included, but more
-importantly from the config.yaml itself. So, for the infra-dev role,
-circlecigen will create a workflow that runs a terraform plan job using the
-specific, associated _instance_.tfvar.json var-file. Each such instance runs in
-parallel. **.circleci/post-approve.yml** Then specify the job to be run if the
-above plans are approved. ```yaml - terraform/apply: name: apply {
+pipeline is generated from within the config.yml pipeline. All values in the
+env_instance.tfvars.json configuration are avaliable to be used in the jinja
+template. Keep in mind that the same yaml template is used for each role so it
+will not work to have a value that ONLY exists in a single instance or role if
+the value appears in the yaml template. ```yaml - terraform/plan: name: {
 {env_instance}} change plan context: << pipeline.parameters.context >>
 workspace: {{env_instance}} var-file: {{envpath}}/{{env_instance}}.tfvars.json
-before-terraform: - set-environment after-terraform: - after-deployment-
-commands requires: - approve {{role}} changes filters: {{filters}} ``` As you
-can see, this template will run terraform apply, and in addition to running the
-set-environment command before the terraaform plan, it will also run an after-
+before-terraform: - set-environment filters: {{filters}}{
+{priorapprovalrequired}} ``` The indenting is important. This example is using
+the [twdps/terraform orb](https://circleci.com/developer/orbs/orb/twdps/
+terraform). Note that in the before-terraform parameter you can pass any
+pipeline command found in any orb you have included, but more importantly from
+the config.yaml itself. So, for the infra-dev role, circlecigen will create a
+workflow that runs a terraform plan job using the specific, associated
+_instance_.tfvar.json var-file. Each such instance runs in parallel.
+**.circleci/post-approve.yml** Then specify the job to be run if the above
+plans are approved. ```yaml - terraform/apply: name: apply {{env_instance}}
+change plan context: << pipeline.parameters.context >> workspace: {
+{env_instance}} var-file: {{envpath}}/{{env_instance}}.tfvars.json before-
+terraform: - set-environment after-terraform: - after-deployment-commands
+requires: - approve {{role}} changes filters: {{filters}} ``` As you can see,
+this template will run terraform apply, and in addition to running the set-
+environment command before the terraaform plan, it will also run an after-
 deployment-commands after a successful apply. In a real use-case, the after-
 terraform commands are typical integration and functional tests. #### The
 primary config.yml pipeline Below is the basic layout of config.yml where the
 circlecigen package is used to create deployment pipelines used by the
 continuation orb. In this case, as is common in trunk-based development, git-
 push results in deployment to an initial development environment, whereas
 tagging the repository expected to launch a full release pipeline that will
```

### Comparing `circlecigen-0.0.4/env_test/config.yml` & `circlecigen-0.0.5/env_test/config.yml`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.4/env_test/generated_config.yml` & `circlecigen-0.0.5/env_test/generated_config.yml`

 * *Files 8% similar despite different names*

```diff
@@ -79,16 +79,16 @@
           before-terraform:
             - set-environment
           filters: *on-tag-main
 
       - approve nonprod changes:
           type: approval
           requires:
-            - nonprod-us-west-2 change plan
-            - nonprod-us-east-2 change plan
+            - plan nonprod-us-west-2 change
+            - plan nonprod-us-east-2 change
           filters: *on-tag-main
 
       - terraform/apply:
           name: apply nonprod-us-west-2 change plan
           context: *context
           workspace: nonprod-us-west-2
           var-file: env_test/nonprod-us-west-2.tfvars.json
@@ -98,14 +98,15 @@
             - store-system-credentials:
                 region: nonprod-us-west-2
             - create-storage-class:
                 region-file: nonprod-us-west-2
                 workspace: nonprod-us-west-2
           requires:
             - approve nonprod changes
+          filters: *on-tag-main
 
       - terraform/apply:
           name: apply nonprod-us-east-2 change plan
           context: *context
           workspace: nonprod-us-east-2
           var-file: env_test/nonprod-us-east-2.tfvars.json
           before-terraform:
@@ -114,14 +115,15 @@
             - store-system-credentials:
                 region: nonprod-us-east-2
             - create-storage-class:
                 region-file: nonprod-us-east-2
                 workspace: nonprod-us-east-2
           requires:
             - approve nonprod changes
+          filters: *on-tag-main
 
       - terraform/plan:
           name: prod-us-west-2 change plan
           context: *context
           workspace: prod-us-west-2
           var-file: env_test/prod-us-west-2.tfvars.json
           before-terraform:
@@ -142,16 +144,16 @@
           requires:
             - approve nonprod changes
 
 
       - approve prod changes:
           type: approval
           requires:
-            - prod-us-west-2 change plan
-            - prod-us-east-2 change plan
+            - plan prod-us-west-2 change
+            - plan prod-us-east-2 change
           filters: *on-tag-main
 
       - terraform/apply:
           name: apply prod-us-west-2 change plan
           context: *context
           workspace: prod-us-west-2
           var-file: env_test/prod-us-west-2.tfvars.json
@@ -161,14 +163,15 @@
             - store-system-credentials:
                 region: prod-us-west-2
             - create-storage-class:
                 region-file: prod-us-west-2
                 workspace: prod-us-west-2
           requires:
             - approve prod changes
+          filters: *on-tag-main
 
       - terraform/apply:
           name: apply prod-us-east-2 change plan
           context: *context
           workspace: prod-us-east-2
           var-file: env_test/prod-us-east-2.tfvars.json
           before-terraform:
@@ -177,8 +180,9 @@
             - store-system-credentials:
                 region: prod-us-east-2
             - create-storage-class:
                 region-file: prod-us-east-2
                 workspace: prod-us-east-2
           requires:
             - approve prod changes
+          filters: *on-tag-main
```

### Comparing `circlecigen-0.0.4/env_test/multi.json` & `circlecigen-0.0.5/env_test/multi.json`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.4/env_test/post-approve.yml` & `circlecigen-0.0.5/env_test/post-approve.yml`

 * *Files 16% similar despite different names*

```diff
@@ -9,9 +9,10 @@
             - store-system-credentials:
                 region: {{env_instance}}
             - create-storage-class:
                 region-file: {{env_instance}}
                 workspace: {{env_instance}}
           requires:
             - approve {{role}} changes
+          filters: {{filters}}
```

### Comparing `circlecigen-0.0.4/pyproject.toml` & `circlecigen-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.4/setup.py` & `circlecigen-0.0.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import setuptools
 
-with open("README.md", "r", encoding = "utf-8") as fh:
+with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
-    name = "circlecigen",
-    author = "Nic Cheneweth",
-    author_email = "nchenewe@thoughtworks.com",
-    description = "Opinionated generation of continuation pipelines",
-    long_description = long_description,
-    long_description_content_type = "text/markdown",
-    url = "https://github.com/ThoughtWorks-DPS/circlecigen",
-    classifiers = [
+    name="circlecigen",
+    author="Nic Cheneweth",
+    author_email="nchenewe@thoughtworks.com",
+    description="Opinionated generation of continuation pipelines",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/ThoughtWorks-DPS/circlecigen",
+    classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
     ],
-    package_dir = {"": "src"},
-    packages = setuptools.find_packages(where="src"),
-    python_requires = ">=3.10",
-    entry_points = '''
+    packages=setuptools.find_packages(),
+    include_package_data=True,
+    python_requires=">=3.10",
+    entry_points='''
         [console_scripts]
-        circlecigen=circlecigen:cli
+        circlecigen=src.circlecigen:cli
     '''
 )
```

### Comparing `circlecigen-0.0.4/src/circlecigen.egg-info/PKG-INFO` & `circlecigen-0.0.5/circlecigen.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circlecigen
-Version: 0.0.4
+Version: 0.0.5
 Summary: Opinionated generation of continuation pipelines
 Home-page: https://github.com/ThoughtWorks-DPS/circlecigen
 Author: Nic Cheneweth
 Author-email: Nic Cheneweth <nchenewe@thoughtworks.com>
 Project-URL: Homepage, https://github.com/ThoughtWorks-DPS/circlecigen
 Project-URL: Bug Tracker, https://github.com/ThoughtWorks-DPS/circlecigen/issues
 Classifier: Programming Language :: Python :: 3
@@ -271,15 +271,15 @@
 Next, the pipeline files.  
 
 **.circleci/config.yml**  
 Of course you must have the regular circleci pipeline file that responds to triggers and actually forms the basis of the generated pipeline. Everything in this file up through the Jobs: or workflow: directive (whichever comes first) forms the starting point for the generated pipeline.  
 
 **.circleci/pre-approve.yml**  
 
-This file is a template that will be populate with instance specific info when the pipeline is generated from within the config.yml pipeline.  
+This file is a template that will be populate with instance specific info when the pipeline is generated from within the config.yml pipeline. All values in the env_instance.tfvars.json configuration are avaliable to be used in the jinja template. Keep in mind that the same yaml template is used for each role so it will not work to have a value that ONLY exists in a single instance or role if the value appears in the yaml template.    
 
 ```yaml
       - terraform/plan:
           name: {{env_instance}} change plan
           context: << pipeline.parameters.context >>
           workspace: {{env_instance}}
           var-file: {{envpath}}/{{env_instance}}.tfvars.json
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: circlecigen Version: 0.0.4 Summary: Opinionated
+Metadata-Version: 2.1 Name: circlecigen Version: 0.0.5 Summary: Opinionated
 generation of continuation pipelines Home-page: https://github.com/
 ThoughtWorks-DPS/circlecigen Author: Nic Cheneweth Author-email: Nic Cheneweth
 thoughtworks.com> Project-URL: Homepage, https://github.com/ThoughtWorks-DPS/
 circlecigen Project-URL: Bug Tracker, https://github.com/ThoughtWorks-DPS/
 circlecigen/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.10 Description-Content-Type: text/markdown
@@ -131,33 +131,37 @@
 generate each specific _instance_.tfvars.json file for use as a -var-file by
 terraform. Next, the pipeline files. **.circleci/config.yml** Of course you
 must have the regular circleci pipeline file that responds to triggers and
 actually forms the basis of the generated pipeline. Everything in this file up
 through the Jobs: or workflow: directive (whichever comes first) forms the
 starting point for the generated pipeline. **.circleci/pre-approve.yml** This
 file is a template that will be populate with instance specific info when the
-pipeline is generated from within the config.yml pipeline. ```yaml - terraform/
-plan: name: {{env_instance}} change plan context: <<
-pipeline.parameters.context >> workspace: {{env_instance}} var-file: {
-{envpath}}/{{env_instance}}.tfvars.json before-terraform: - set-environment
-filters: {{filters}}{{priorapprovalrequired}} ``` The indenting is important.
-This example is using the [twdps/terraform orb](https://circleci.com/developer/
-orbs/orb/twdps/terraform). Note that in the before-terraform parameter you can
-pass any pipeline command found in any orb you have included, but more
-importantly from the config.yaml itself. So, for the infra-dev role,
-circlecigen will create a workflow that runs a terraform plan job using the
-specific, associated _instance_.tfvar.json var-file. Each such instance runs in
-parallel. **.circleci/post-approve.yml** Then specify the job to be run if the
-above plans are approved. ```yaml - terraform/apply: name: apply {
+pipeline is generated from within the config.yml pipeline. All values in the
+env_instance.tfvars.json configuration are avaliable to be used in the jinja
+template. Keep in mind that the same yaml template is used for each role so it
+will not work to have a value that ONLY exists in a single instance or role if
+the value appears in the yaml template. ```yaml - terraform/plan: name: {
 {env_instance}} change plan context: << pipeline.parameters.context >>
 workspace: {{env_instance}} var-file: {{envpath}}/{{env_instance}}.tfvars.json
-before-terraform: - set-environment after-terraform: - after-deployment-
-commands requires: - approve {{role}} changes filters: {{filters}} ``` As you
-can see, this template will run terraform apply, and in addition to running the
-set-environment command before the terraaform plan, it will also run an after-
+before-terraform: - set-environment filters: {{filters}}{
+{priorapprovalrequired}} ``` The indenting is important. This example is using
+the [twdps/terraform orb](https://circleci.com/developer/orbs/orb/twdps/
+terraform). Note that in the before-terraform parameter you can pass any
+pipeline command found in any orb you have included, but more importantly from
+the config.yaml itself. So, for the infra-dev role, circlecigen will create a
+workflow that runs a terraform plan job using the specific, associated
+_instance_.tfvar.json var-file. Each such instance runs in parallel.
+**.circleci/post-approve.yml** Then specify the job to be run if the above
+plans are approved. ```yaml - terraform/apply: name: apply {{env_instance}}
+change plan context: << pipeline.parameters.context >> workspace: {
+{env_instance}} var-file: {{envpath}}/{{env_instance}}.tfvars.json before-
+terraform: - set-environment after-terraform: - after-deployment-commands
+requires: - approve {{role}} changes filters: {{filters}} ``` As you can see,
+this template will run terraform apply, and in addition to running the set-
+environment command before the terraaform plan, it will also run an after-
 deployment-commands after a successful apply. In a real use-case, the after-
 terraform commands are typical integration and functional tests. #### The
 primary config.yml pipeline Below is the basic layout of config.yml where the
 circlecigen package is used to create deployment pipelines used by the
 continuation orb. In this case, as is common in trunk-based development, git-
 push results in deployment to an initial development environment, whereas
 tagging the repository expected to launch a full release pipeline that will
```

### Comparing `circlecigen-0.0.4/src/circlecigen.egg-info/SOURCES.txt` & `circlecigen-0.0.5/circlecigen.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -2,43 +2,45 @@
 .gitignore
 .pre-commit-config.yaml
 .pylintrc
 .python-version
 LICENSE
 Pipfile
 README.md
+__init__.py
 notes.txt
 op.env
 pyproject.toml
 requirements.txt
 setup.py
 .circleci/config.yml
+circlecigen.egg-info/PKG-INFO
+circlecigen.egg-info/SOURCES.txt
+circlecigen.egg-info/dependency_links.txt
+circlecigen.egg-info/entry_points.txt
+circlecigen.egg-info/top_level.txt
 env_test/config.yml
 env_test/default.json
 env_test/dev.json
 env_test/generated_config.yml
 env_test/multi.json
 env_test/nonprod-us-east-2.tfvars.json
 env_test/nonprod-us-west-2.tfvars.json
 env_test/nonprod.json
 env_test/post-approve.yml
 env_test/pre-approve.yml
 env_test/prod-us-east-2.tfvars.json
 env_test/prod-us-west-2.tfvars.json
 env_test/prod.json
 src/__init__.py
+src/_version.py
 src/circlecigen.py
 src/template.py
 src/tfvars.py
 src/utils.py
-src/circlecigen.egg-info/PKG-INFO
-src/circlecigen.egg-info/SOURCES.txt
-src/circlecigen.egg-info/dependency_links.txt
-src/circlecigen.egg-info/entry_points.txt
-src/circlecigen.egg-info/top_level.txt
 test/generated_config.yml
 test/generated_config_setup.yml
 test/nonprod-us-east-2.tfvars.json
 test/nonprod-us-west-2.tfvars.json
 test/prod-us-east-2.tfvars.json
 test/prod-us-west-2.tfvars.json
 test/test_circlecigen.py
```

### Comparing `circlecigen-0.0.4/src/circlecigen.py` & `circlecigen-0.0.5/src/circlecigen.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import click
 from pathvalidate.click import validate_filename_arg, validate_filepath_arg
-from tfvars import generate_environment_tfvar_files
-from utils import read_json_file, validate_filepath
-from template import generate_config
+from src.tfvars import generate_environment_tfvar_files
+from src.utils import read_json_file, validate_filepath
+from src.template import generate_config
 
 @click.version_option()
 @click.command()
 @click.option("--outfile",
     default="generated_config.yml",
     help="Generated file. Default is generated_config.yml",
     callback=validate_filename_arg)
```

### Comparing `circlecigen-0.0.4/src/template.py` & `circlecigen-0.0.5/src/template.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from os.path import isfile
 from jinja2 import Environment, FileSystemLoader
-from utils import read_json_file
+from src.utils import read_json_file
 
 APPROVE_TEMPLATE="""      - approve {{role}} changes:
           type: approval
           {{approvalrequiredjobs}}
           filters: {{filter}}
 
 
@@ -26,14 +26,17 @@
 def generate_config(use_pipeline, pipepath, outfile, envpath, environs, workflow):
     """create generated_config.yaml for continuation orb"""
 
     # use the specified filter to generate a pipeline only for the desired trigger
     pipeline = environs[use_pipeline]
 
     # copy everything but the jobs and workflows from config.yml into generated_config.yml
+    # pipepath = where to find config.yml, default .circleci
+    # outfile  = where to write generated_config.yml, default .circleci
+    # workflow = what to name the generated workflow, default continuation-generated-workflow
     setup_generated_config_outfile(pipepath, outfile, workflow)
 
     # setup the jinja templates
     je = Environment(loader=FileSystemLoader(f"{pipepath}/"), autoescape=True)
     pre, approve, post = get_templates(je, pipepath)
 
     # setup Dict for the approval job template 
@@ -48,21 +51,24 @@
 
     # open the outfile for appeand and start processing roles/instances
     with open(f"{pipepath}/{outfile}", 'a', encoding="utf-8") as f:
         for role in pipeline:
             # skip the filter definition
             if role == "filter":
                 continue
+
             # when the approval template is generate, it must be populated with
             # a list of all instances for which a pre-approval template is
             # generated. That is returned by this job.
-            approvalrequiredjobs =  generate_pre_approval_jobs(f, envpath, pre, pipeline, role, priorapprovalrequired)
+            approvalrequiredjobs = generate_pre_approval_jobs(f, envpath, pre, pipeline, role, priorapprovalrequired)
+
             # generate approval job for the current role, a human will trigger the post- phase
             generate_approval_jobs(f, approve, approve_vars, approvalrequiredjobs, role)
             generate_post_approval_jobs(f, envpath, post, pipeline, role)
+
             # record the current role, to provide 'requires:' list in any subsequent pre- jobs
             priorapprovalrequired = role
 
 def generate_pre_approval_jobs(f, envpath, pre, pipeline, role, priorapprovalrequired):
     # generate a pre-approval job for each instance in the role,
     # if a pre-approval.yml file exists
     if pre:
@@ -74,15 +80,15 @@
                 "role": role,
                 "envpath": envpath
             })
             if priorapprovalrequired:
                 instance_vars.update({
                     "priorapprovalrequired": PRIOR_APPROVAL.format(priorapprovalrequired)
                 })
-            approvalrequiredjobs += f"\n            - {instance} change plan"
+            approvalrequiredjobs += f"\n            - plan {instance} change"
             f.write(pre.render(instance_vars))
         return approvalrequiredjobs
     return None
 
 def generate_approval_jobs(f, approve, approve_vars, approvalrequiredjobs, role):
     approve_vars.update ({
         "role": role,
```

### Comparing `circlecigen-0.0.4/src/tfvars.py` & `circlecigen-0.0.5/src/tfvars.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from os.path import isfile
-from utils import read_json_file, merge, write_json_file
+from src.utils import read_json_file, merge, write_json_file
 
 def generate_environment_tfvar_files(use_pipeline, envpath, environs, defaultparams):
     """create and write instance.tfvars.json files for each multi-env instance"""
 
     # use the specified filter to generate a pipeline only for the desired trigger
     pipeline = environs[use_pipeline]
 
@@ -11,14 +11,19 @@
          # skip the filter key, this is used to specify the trigger for a generated pipeline
         if role == "filter":
             continue
 
         # start with an instance.tfvars.json dict made from the default environment parameters
         role_vars = defaultparams
 
+        # if there is a matching use_pipeline.json file for values are unique to this pipeline 
+        # yet universal to all roles (contrast with default which apply also to all pipelines)
+        if isfile(f"{envpath}/{use_pipeline}.json"):
+           role_vars = merge(role_vars,read_json_file(envpath, f"{use_pipeline}.json"))
+
         # if there is a matching role.json file, get the values to merge in the next step
         if isfile(f"{envpath}/{role}.json"):
            role_vars = merge(role_vars,read_json_file(envpath, f"{role}.json"))
 
         for instance in pipeline[role]:
             instance_vars = role_vars
```

### Comparing `circlecigen-0.0.4/src/utils.py` & `circlecigen-0.0.5/src/utils.py`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.4/test/generated_config.yml` & `circlecigen-0.0.5/test/generated_config.yml`

 * *Files 8% similar despite different names*

```diff
@@ -79,16 +79,16 @@
           before-terraform:
             - set-environment
           filters: *on-tag-main
 
       - approve nonprod changes:
           type: approval
           requires:
-            - nonprod-us-west-2 change plan
-            - nonprod-us-east-2 change plan
+            - plan nonprod-us-west-2 change
+            - plan nonprod-us-east-2 change
           filters: *on-tag-main
 
       - terraform/apply:
           name: apply nonprod-us-west-2 change plan
           context: *context
           workspace: nonprod-us-west-2
           var-file: env_test/nonprod-us-west-2.tfvars.json
@@ -98,14 +98,15 @@
             - store-system-credentials:
                 region: nonprod-us-west-2
             - create-storage-class:
                 region-file: nonprod-us-west-2
                 workspace: nonprod-us-west-2
           requires:
             - approve nonprod changes
+          filters: *on-tag-main
 
       - terraform/apply:
           name: apply nonprod-us-east-2 change plan
           context: *context
           workspace: nonprod-us-east-2
           var-file: env_test/nonprod-us-east-2.tfvars.json
           before-terraform:
@@ -114,14 +115,15 @@
             - store-system-credentials:
                 region: nonprod-us-east-2
             - create-storage-class:
                 region-file: nonprod-us-east-2
                 workspace: nonprod-us-east-2
           requires:
             - approve nonprod changes
+          filters: *on-tag-main
 
       - terraform/plan:
           name: prod-us-west-2 change plan
           context: *context
           workspace: prod-us-west-2
           var-file: env_test/prod-us-west-2.tfvars.json
           before-terraform:
@@ -142,16 +144,16 @@
           requires:
             - approve nonprod changes
 
 
       - approve prod changes:
           type: approval
           requires:
-            - prod-us-west-2 change plan
-            - prod-us-east-2 change plan
+            - plan prod-us-west-2 change
+            - plan prod-us-east-2 change
           filters: *on-tag-main
 
       - terraform/apply:
           name: apply prod-us-west-2 change plan
           context: *context
           workspace: prod-us-west-2
           var-file: env_test/prod-us-west-2.tfvars.json
@@ -161,14 +163,15 @@
             - store-system-credentials:
                 region: prod-us-west-2
             - create-storage-class:
                 region-file: prod-us-west-2
                 workspace: prod-us-west-2
           requires:
             - approve prod changes
+          filters: *on-tag-main
 
       - terraform/apply:
           name: apply prod-us-east-2 change plan
           context: *context
           workspace: prod-us-east-2
           var-file: env_test/prod-us-east-2.tfvars.json
           before-terraform:
@@ -177,8 +180,9 @@
             - store-system-credentials:
                 region: prod-us-east-2
             - create-storage-class:
                 region-file: prod-us-east-2
                 workspace: prod-us-east-2
           requires:
             - approve prod changes
+          filters: *on-tag-main
```

### Comparing `circlecigen-0.0.4/test/generated_config_setup.yml` & `circlecigen-0.0.5/test/generated_config_setup.yml`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.4/test/test_circlecigen.py` & `circlecigen-0.0.5/test/test_circlecigen.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from click.testing import CliRunner
-from circlecigen import cli
+from src.circlecigen import cli
 
 def test_circlecigen_with_invalid_outfile_name():
   runner = CliRunner()
   result = runner.invoke(cli, ['sandbox', '--outfile', 'invalid:filename'])
   assert result.exit_code == 2
   assert "Invalid value for '--outfile'" in result.output
```

### Comparing `circlecigen-0.0.4/test/test_template.py` & `circlecigen-0.0.5/test/test_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import filecmp
 from jinja2 import Environment, FileSystemLoader, Template
-from template import setup_generated_config_outfile, get_templates, generate_config
+from src.template import setup_generated_config_outfile, get_templates, generate_config
 
 mock_multi = {
   "sandbox": {
     "filter": "*on-push-main",
     "dev": {
       "dev-us-east-2": {
         "aws_region": "us-east-2",
```

### Comparing `circlecigen-0.0.4/test/test_tfvars.py` & `circlecigen-0.0.5/test/test_tfvars.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import filecmp
-from tfvars import nummber_of_files_to_generate, generate_environment_tfvar_files
+from src.tfvars import nummber_of_files_to_generate, generate_environment_tfvar_files
 
 mock_envpath = "env_test"
 
 mock_multi = {
   "sandbox": {
     "filter": "*on-push-main",
     "dev": {
```

### Comparing `circlecigen-0.0.4/test/test_utils.py` & `circlecigen-0.0.5/test/test_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 from unittest.mock import patch, mock_open
 import pytest
 import click
-from utils import merge, read_json_file, write_json_file, validate_filepath
+from src.utils import merge, read_json_file, write_json_file, validate_filepath
 
 def test_merge_non_overlapping_dict():
     dict1 = {"a": 1, "b": 2}
     dict2 = {"c": 3, "d": 4}
     assert merge(dict1, dict2) == {"a": 1, "b": 2, "c": 3, "d": 4}
 
 def test_merge_overlapping_dict():
```

