# Comparing `tmp/mindflow-0.5.0.tar.gz` & `tmp/mindflow-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mindflow-0.5.0.tar", last modified: Tue Jun 20 21:45:57 2023, max compression
+gzip compressed data, was "mindflow-0.5.1.tar", last modified: Tue Jun 20 21:55:15 2023, max compression
```

## Comparing `mindflow-0.5.0.tar` & `mindflow-0.5.1.tar`

### file list

```diff
@@ -1,108 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:57.624683 mindflow-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-20 21:45:45.000000 mindflow-0.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-20 21:45:45.000000 mindflow-0.5.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 21:45:45.000000 mindflow-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-20 21:45:45.000000 mindflow-0.5.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-06-20 21:45:57.624683 mindflow-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9080 2023-06-20 21:45:45.000000 mindflow-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-20 21:45:45.000000 mindflow-0.5.0/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:57.604683 mindflow-0.5.0/mindflow/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:57.608683 mindflow-0.5.0/mindflow/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/cli/cli_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:57.612683 mindflow-0.5.0/mindflow/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/cli/commands/chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/cli/commands/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/cli/commands/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/cli/commands/gen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:57.612683 mindflow-0.5.0/mindflow/cli/commands/git/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/cli/commands/git/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/cli/commands/git/add.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/cli/commands/git/commit.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/cli/commands/git/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/cli/commands/git/mr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/cli/commands/git/pr.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/cli/commands/git/push.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/cli/commands/index.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/cli/commands/inspect.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/cli/commands/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/cli/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:57.616683 mindflow-0.5.0/mindflow/core/
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/command_parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:57.616683 mindflow-0.5.0/mindflow/core/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/commands/chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/commands/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/commands/gen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:57.620683 mindflow-0.5.0/mindflow/core/commands/git/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/commands/git/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/commands/git/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/commands/git/commit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/commands/git/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/commands/git/mr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/commands/git/pr.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/commands/git/push.py
--rw-r--r--   0 runner    (1001) docker     (123)    11835 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/commands/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/commands/inspect.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/commands/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/commands/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/execute.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:57.620683 mindflow-0.5.0/mindflow/core/file_processing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/file_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/file_processing/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/file_processing/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/prompt_builders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:57.620683 mindflow-0.5.0/mindflow/core/resolving/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/resolving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/resolving/resolve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:57.620683 mindflow-0.5.0/mindflow/core/resolving/resolvers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/resolving/resolvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/resolving/resolvers/document_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/resolving/resolvers/file_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:57.620683 mindflow-0.5.0/mindflow/core/text_processing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/text_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/text_processing/utf8.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/text_processing/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/token_counting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:57.620683 mindflow-0.5.0/mindflow/core/types/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/types/conversation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:57.624683 mindflow-0.5.0/mindflow/core/types/definitions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/types/definitions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/types/definitions/conversation.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/types/definitions/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/types/definitions/mind_flow_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    14100 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/types/definitions/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/types/definitions/model_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/types/definitions/object.py
--rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/types/definitions/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/types/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/types/mindflow_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/types/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/types/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:57.624683 mindflow-0.5.0/mindflow/core/types/store_traits/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/types/store_traits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/types/store_traits/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/types/store_traits/pinecone.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/types/store_traits/static.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:57.624683 mindflow-0.5.0/mindflow/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/unit_tests/dummy_diff.txt
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/unit_tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    12249 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/unit_tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:57.608683 mindflow-0.5.0/mindflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-06-20 21:45:57.000000 mindflow-0.5.0/mindflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-06-20 21:45:57.000000 mindflow-0.5.0/mindflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 21:45:57.000000 mindflow-0.5.0/mindflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-20 21:45:57.000000 mindflow-0.5.0/mindflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-20 21:45:57.000000 mindflow-0.5.0/mindflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 21:45:57.000000 mindflow-0.5.0/mindflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-20 21:45:45.000000 mindflow-0.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 21:45:57.624683 mindflow-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-20 21:45:45.000000 mindflow-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:15.304136 mindflow-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-20 21:55:02.000000 mindflow-0.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-20 21:55:02.000000 mindflow-0.5.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 21:55:02.000000 mindflow-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-20 21:55:02.000000 mindflow-0.5.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-06-20 21:55:15.304136 mindflow-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9080 2023-06-20 21:55:02.000000 mindflow-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-20 21:55:02.000000 mindflow-0.5.1/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:15.296136 mindflow-0.5.1/mindflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:15.296136 mindflow-0.5.1/mindflow/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/cli/cli_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:15.296136 mindflow-0.5.1/mindflow/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/cli/commands/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/cli/commands/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/cli/commands/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/cli/commands/gen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:15.296136 mindflow-0.5.1/mindflow/cli/commands/git/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/cli/commands/git/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/cli/commands/git/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/cli/commands/git/commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/cli/commands/git/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/cli/commands/git/mr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/cli/commands/git/pr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/cli/commands/git/push.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/cli/commands/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/cli/commands/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/cli/commands/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/cli/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:15.300136 mindflow-0.5.1/mindflow/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/command_parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:15.300136 mindflow-0.5.1/mindflow/core/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/commands/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/commands/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/commands/gen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:15.300136 mindflow-0.5.1/mindflow/core/commands/git/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/commands/git/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/commands/git/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/commands/git/commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/commands/git/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/commands/git/mr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/commands/git/pr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/commands/git/push.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11833 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/commands/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/commands/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/commands/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/commands/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/execute.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:15.300136 mindflow-0.5.1/mindflow/core/file_processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/file_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/file_processing/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/file_processing/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/prompt_builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:15.300136 mindflow-0.5.1/mindflow/core/resolving/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/resolving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/resolving/resolve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:15.300136 mindflow-0.5.1/mindflow/core/resolving/resolvers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/resolving/resolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/resolving/resolvers/document_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/resolving/resolvers/file_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:15.300136 mindflow-0.5.1/mindflow/core/text_processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/text_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/text_processing/utf8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/text_processing/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/token_counting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:15.304136 mindflow-0.5.1/mindflow/core/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/types/conversation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:15.304136 mindflow-0.5.1/mindflow/core/types/definitions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/types/definitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/types/definitions/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/types/definitions/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/types/definitions/mind_flow_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14100 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/types/definitions/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/types/definitions/model_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/types/definitions/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/types/definitions/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/types/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/types/mindflow_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/types/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/types/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:15.304136 mindflow-0.5.1/mindflow/core/types/store_traits/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/types/store_traits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/types/store_traits/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/types/store_traits/pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/types/store_traits/static.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:15.304136 mindflow-0.5.1/mindflow/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/unit_tests/dummy_diff.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/unit_tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12249 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/unit_tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:15.296136 mindflow-0.5.1/mindflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-06-20 21:55:15.000000 mindflow-0.5.1/mindflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-06-20 21:55:15.000000 mindflow-0.5.1/mindflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 21:55:15.000000 mindflow-0.5.1/mindflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-20 21:55:15.000000 mindflow-0.5.1/mindflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-20 21:55:15.000000 mindflow-0.5.1/mindflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 21:55:15.000000 mindflow-0.5.1/mindflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-20 21:55:02.000000 mindflow-0.5.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 21:55:15.304136 mindflow-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-20 21:55:02.000000 mindflow-0.5.1/setup.py
```

### Comparing `mindflow-0.5.0/.gitignore` & `mindflow-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.0/Makefile` & `mindflow-0.5.1/Makefile`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.0/PKG-INFO` & `mindflow-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindflow
-Version: 0.5.0
+Version: 0.5.1
 Summary: AI-powered search engine for your code!
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # :brain: mindflow :ocean:
 The [ChatGPT](https://openai.com/blog/chatgpt)-powered swiss army knife for the modern developer! We provide an AI-powered CLI git wrapper, boilerplate code generator, code search engine, a conversation history manager, and much more!
```

### Comparing `mindflow-0.5.0/README.md` & `mindflow-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.0/mindflow/cli/cli_main.py` & `mindflow-0.5.1/mindflow/cli/cli_main.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.0/mindflow/cli/commands/chat.py` & `mindflow-0.5.1/mindflow/cli/commands/chat.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.0/mindflow/cli/commands/config.py` & `mindflow-0.5.1/mindflow/cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.0/mindflow/cli/commands/git/commit.py` & `mindflow-0.5.1/mindflow/cli/commands/git/commit.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.0/mindflow/cli/commands/git/diff.py` & `mindflow-0.5.1/mindflow/cli/commands/git/diff.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.0/mindflow/cli/commands/git/mr.py` & `mindflow-0.5.1/mindflow/cli/commands/git/mr.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.0/mindflow/cli/commands/git/pr.py` & `mindflow-0.5.1/mindflow/cli/commands/git/pr.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.0/mindflow/cli/util.py` & `mindflow-0.5.1/mindflow/cli/util.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.0/mindflow/core/commands/chat.py` & `mindflow-0.5.1/mindflow/core/commands/chat.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.0/mindflow/core/commands/delete.py` & `mindflow-0.5.1/mindflow/core/commands/delete.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,17 +8,26 @@
     get_document_id,
 )
 from mindflow.core.resolving.resolve import resolve_paths_to_document_references
 
 
 def run_delete(document_paths: List[str]) -> str:
     """Delete documents from MindFlow index."""
-    document_references: List[DocumentReference] = resolve_paths_to_document_references(document_paths)
-
-    document_ids = [document_id for document_id in [get_document_id(document_reference.path, document_reference.document_type) for document_reference in document_references] if document_id is not None]
+    document_references: List[DocumentReference] = resolve_paths_to_document_references(
+        document_paths
+    )
+
+    document_ids = [
+        document_id
+        for document_id in [
+            get_document_id(document_reference.path, document_reference.document_type)
+            for document_reference in document_references
+        ]
+        if document_id is not None
+    ]
 
     if not document_ids:
         return "No document IDs resolved. Nothing to delete."
 
     documents = Document.load_bulk_ignore_missing(document_ids)
     if not documents:
         return "No documents found to delete."
@@ -26,8 +35,8 @@
     document_chunk_ids = get_document_chunk_ids(documents)
     if not DocumentChunk.load_bulk_ignore_missing(document_chunk_ids):
         return "No document chunks found to delete."
 
     Document.delete_bulk(document_ids)
     DocumentChunk.delete_bulk(document_chunk_ids)
 
-    return True, "Documents and associated chunks deleted successfully."
+    return "Documents and associated chunks deleted successfully."
```

### Comparing `mindflow-0.5.0/mindflow/core/commands/gen.py` & `mindflow-0.5.1/mindflow/core/commands/gen.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.0/mindflow/core/commands/git/commit.py` & `mindflow-0.5.1/mindflow/core/commands/git/commit.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.0/mindflow/core/commands/git/diff.py` & `mindflow-0.5.1/mindflow/core/commands/git/diff.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.0/mindflow/core/commands/git/mr.py` & `mindflow-0.5.1/mindflow/core/commands/git/mr.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.0/mindflow/core/commands/git/pr.py` & `mindflow-0.5.1/mindflow/core/commands/git/pr.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.0/mindflow/core/commands/index.py` & `mindflow-0.5.1/mindflow/core/commands/index.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         document_paths
     )
 
     if not (
         indexable_documents := get_indexable_documents(
             document_references, completion_model
         )
-    ):  
+    ):
         return "No documents to index"
 
     print_total_size_of_documents(indexable_documents)
     print_total_tokens_and_ask_to_continue(indexable_documents, completion_model)
 
     index_documents(indexable_documents, completion_model, embedding_model)
```

### Comparing `mindflow-0.5.0/mindflow/core/commands/inspect.py` & `mindflow-0.5.1/mindflow/core/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.0/mindflow/core/commands/login.py` & `mindflow-0.5.1/mindflow/core/commands/login.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.0/mindflow/core/commands/query.py` & `mindflow-0.5.1/mindflow/core/commands/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,17 @@
     if not (
         top_document_chunks := DocumentChunk.query(
             vector=np.array(embedding_model(query)).reshape(1, -1),
             ids=document_chunk_ids,
             top_k=100,
         )
     ):
-        return "No index for requested hashes. Please generate index for passed content."
+        return (
+            "No index for requested hashes. Please generate index for passed content."
+        )
 
     document_selection_batch: List[Tuple[str, DocumentChunk]] = [
         (document_hash_to_path[document_chunk.id.split("_")[0]], document_chunk)
         for document_chunk in top_document_chunks
     ]
 
     trimmed_content: str = select_and_trim_text_to_fit_context_window(
```

### Comparing `mindflow-0.5.0/mindflow/core/errors.py` & `mindflow-0.5.1/mindflow/core/errors.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.0/mindflow/core/file_processing/extract.py` & `mindflow-0.5.1/mindflow/core/file_processing/extract.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.0/mindflow/core/file_processing/git.py` & `mindflow-0.5.1/mindflow/core/file_processing/git.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,10 +25,10 @@
             ["git", "-C", os.fspath(path), "ls-files"],
             capture_output=True,
             timeout=10,
             check=True,
         )
         git_files = output.stdout.decode().strip().split("\n")
         return [os.path.abspath(os.path.join(os.fspath(path), f)) for f in git_files]
-    except GitError as error:
+    except subprocess.CalledProcessError as error:
         logging.debug("Failed extract git files with 'git ls-files': %s", error)
         return []
```

### Comparing `mindflow-0.5.0/mindflow/core/prompt_builders.py` & `mindflow-0.5.1/mindflow/core/prompt_builders.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.0/mindflow/core/prompts.py` & `mindflow-0.5.1/mindflow/core/prompts.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.0/mindflow/core/resolving/resolve.py` & `mindflow-0.5.1/mindflow/core/resolving/resolve.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.0/mindflow/core/resolving/resolvers/file_resolver.py` & `mindflow-0.5.1/mindflow/core/resolving/resolvers/file_resolver.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.0/mindflow/core/token_counting.py` & `mindflow-0.5.1/mindflow/core/token_counting.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.0/mindflow/core/types/definitions/mind_flow_model.py` & `mindflow-0.5.1/mindflow/core/types/definitions/mind_flow_model.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.0/mindflow/core/types/definitions/model.py` & `mindflow-0.5.1/mindflow/core/types/definitions/model.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.0/mindflow/core/types/definitions/object.py` & `mindflow-0.5.1/mindflow/core/types/definitions/object.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.0/mindflow/core/types/definitions/service.py` & `mindflow-0.5.1/mindflow/core/types/definitions/service.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.0/mindflow/core/types/document.py` & `mindflow-0.5.1/mindflow/core/types/document.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.0/mindflow/core/types/mindflow_model.py` & `mindflow-0.5.1/mindflow/core/types/mindflow_model.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.0/mindflow/core/types/model.py` & `mindflow-0.5.1/mindflow/core/types/model.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.0/mindflow/core/types/service.py` & `mindflow-0.5.1/mindflow/core/types/service.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.0/mindflow/core/types/store_traits/json.py` & `mindflow-0.5.1/mindflow/core/types/store_traits/json.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.0/mindflow/core/types/store_traits/pinecone.py` & `mindflow-0.5.1/mindflow/core/types/store_traits/pinecone.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.0/mindflow/core/types/store_traits/static.py` & `mindflow-0.5.1/mindflow/core/types/store_traits/static.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.0/mindflow/unit_tests/dummy_diff.txt` & `mindflow-0.5.1/mindflow/unit_tests/dummy_diff.txt`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.0/mindflow/unit_tests/test_utils.py` & `mindflow-0.5.1/mindflow/unit_tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.0/mindflow.egg-info/PKG-INFO` & `mindflow-0.5.1/mindflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindflow
-Version: 0.5.0
+Version: 0.5.1
 Summary: AI-powered search engine for your code!
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # :brain: mindflow :ocean:
 The [ChatGPT](https://openai.com/blog/chatgpt)-powered swiss army knife for the modern developer! We provide an AI-powered CLI git wrapper, boilerplate code generator, code search engine, a conversation history manager, and much more!
```

### Comparing `mindflow-0.5.0/mindflow.egg-info/SOURCES.txt` & `mindflow-0.5.1/mindflow.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 mindflow/cli/commands/git/__init__.py
 mindflow/cli/commands/git/add.py
 mindflow/cli/commands/git/commit.py
 mindflow/cli/commands/git/diff.py
 mindflow/cli/commands/git/mr.py
 mindflow/cli/commands/git/pr.py
 mindflow/cli/commands/git/push.py
+mindflow/core/__init__.py
 mindflow/core/command_parse.py
 mindflow/core/constants.py
 mindflow/core/errors.py
 mindflow/core/execute.py
 mindflow/core/prompt_builders.py
 mindflow/core/prompts.py
 mindflow/core/settings.py
```

### Comparing `mindflow-0.5.0/setup.py` & `mindflow-0.5.1/setup.py`

 * *Files identical despite different names*

