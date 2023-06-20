# Comparing `tmp/mindflow-0.4.0.tar.gz` & `tmp/mindflow-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mindflow-0.4.0.tar", last modified: Mon Apr 24 20:38:26 2023, max compression
+gzip compressed data, was "mindflow-0.5.0.tar", last modified: Tue Jun 20 21:45:57 2023, max compression
```

## Comparing `mindflow-0.4.0.tar` & `mindflow-0.5.0.tar`

### file list

```diff
@@ -1,119 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:26.774243 mindflow-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-24 20:38:15.000000 mindflow-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-24 20:38:15.000000 mindflow-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-24 20:38:15.000000 mindflow-0.4.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-24 20:38:15.000000 mindflow-0.4.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 20:38:15.000000 mindflow-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-04-24 20:38:15.000000 mindflow-0.4.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-04-24 20:38:26.774243 mindflow-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9080 2023-04-24 20:38:15.000000 mindflow-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-24 20:38:15.000000 mindflow-0.4.0/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:26.754243 mindflow-0.4.0/mindflow/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:26.758243 mindflow-0.4.0/mindflow/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/cli/cli_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:26.758243 mindflow-0.4.0/mindflow/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/cli/commands/chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/cli/commands/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/cli/commands/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/cli/commands/gen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:26.758243 mindflow-0.4.0/mindflow/cli/commands/git/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/cli/commands/git/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/cli/commands/git/add.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/cli/commands/git/commit.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/cli/commands/git/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/cli/commands/git/mr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/cli/commands/git/pr.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/cli/commands/git/push.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/cli/commands/index.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/cli/commands/inspect.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/cli/commands/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/cli/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:26.762243 mindflow-0.4.0/mindflow/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/core/chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/core/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/core/gen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:26.762243 mindflow-0.4.0/mindflow/core/git/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/core/git/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/core/git/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/core/git/commit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/core/git/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/core/git/mr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/core/git/pr.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/core/git/push.py
--rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/core/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/core/inspect.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/core/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/core/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:26.762243 mindflow-0.4.0/mindflow/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/db/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:26.766243 mindflow-0.4.0/mindflow/db/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/db/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/db/db/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/db/db/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/db/db/pinecone.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/db/db/static.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:26.766243 mindflow-0.4.0/mindflow/db/objects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/db/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/db/objects/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/db/objects/conversation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/db/objects/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/db/objects/mindflow_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/db/objects/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/db/objects/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:26.766243 mindflow-0.4.0/mindflow/db/objects/static_definition/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/db/objects/static_definition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/db/objects/static_definition/conversation.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/db/objects/static_definition/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/db/objects/static_definition/mind_flow_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    14264 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/db/objects/static_definition/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/db/objects/static_definition/model_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/db/objects/static_definition/object.py
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/db/objects/static_definition/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/db/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:26.770243 mindflow-0.4.0/mindflow/resolving/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/resolving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/resolving/resolve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:26.770243 mindflow-0.4.0/mindflow/resolving/resolvers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/resolving/resolvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/resolving/resolvers/base_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/resolving/resolvers/file_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:26.770243 mindflow-0.4.0/mindflow/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/unit_tests/dummy_diff.txt
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/unit_tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    12244 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/unit_tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:26.770243 mindflow-0.4.0/mindflow/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/utils/command_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/utils/diff_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/utils/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/utils/execute.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:26.774243 mindflow-0.4.0/mindflow/utils/files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/utils/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/utils/files/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/utils/files/git.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/utils/files/utf8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/utils/prompt_builders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/utils/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/utils/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/utils/token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:26.754243 mindflow-0.4.0/mindflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-04-24 20:38:26.000000 mindflow-0.4.0/mindflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-04-24 20:38:26.000000 mindflow-0.4.0/mindflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 20:38:26.000000 mindflow-0.4.0/mindflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-24 20:38:26.000000 mindflow-0.4.0/mindflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-24 20:38:26.000000 mindflow-0.4.0/mindflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-24 20:38:26.000000 mindflow-0.4.0/mindflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-24 20:38:15.000000 mindflow-0.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 20:38:26.774243 mindflow-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-24 20:38:15.000000 mindflow-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:57.624683 mindflow-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-20 21:45:45.000000 mindflow-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-20 21:45:45.000000 mindflow-0.5.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 21:45:45.000000 mindflow-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-20 21:45:45.000000 mindflow-0.5.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-06-20 21:45:57.624683 mindflow-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9080 2023-06-20 21:45:45.000000 mindflow-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-20 21:45:45.000000 mindflow-0.5.0/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:57.604683 mindflow-0.5.0/mindflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:57.608683 mindflow-0.5.0/mindflow/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/cli/cli_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:57.612683 mindflow-0.5.0/mindflow/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/cli/commands/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/cli/commands/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/cli/commands/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/cli/commands/gen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:57.612683 mindflow-0.5.0/mindflow/cli/commands/git/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/cli/commands/git/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/cli/commands/git/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/cli/commands/git/commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/cli/commands/git/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/cli/commands/git/mr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/cli/commands/git/pr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/cli/commands/git/push.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/cli/commands/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/cli/commands/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/cli/commands/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/cli/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:57.616683 mindflow-0.5.0/mindflow/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/command_parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:57.616683 mindflow-0.5.0/mindflow/core/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/commands/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/commands/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/commands/gen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:57.620683 mindflow-0.5.0/mindflow/core/commands/git/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/commands/git/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/commands/git/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/commands/git/commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/commands/git/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/commands/git/mr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/commands/git/pr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/commands/git/push.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11835 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/commands/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/commands/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/commands/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/commands/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/execute.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:57.620683 mindflow-0.5.0/mindflow/core/file_processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/file_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/file_processing/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/file_processing/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/prompt_builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:57.620683 mindflow-0.5.0/mindflow/core/resolving/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/resolving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/resolving/resolve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:57.620683 mindflow-0.5.0/mindflow/core/resolving/resolvers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/resolving/resolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/resolving/resolvers/document_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/resolving/resolvers/file_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:57.620683 mindflow-0.5.0/mindflow/core/text_processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/text_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/text_processing/utf8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/text_processing/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/token_counting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:57.620683 mindflow-0.5.0/mindflow/core/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/types/conversation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:57.624683 mindflow-0.5.0/mindflow/core/types/definitions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/types/definitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/types/definitions/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/types/definitions/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/types/definitions/mind_flow_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14100 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/types/definitions/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/types/definitions/model_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/types/definitions/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/types/definitions/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/types/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/types/mindflow_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/types/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/types/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:57.624683 mindflow-0.5.0/mindflow/core/types/store_traits/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/types/store_traits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/types/store_traits/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/types/store_traits/pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/core/types/store_traits/static.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:57.624683 mindflow-0.5.0/mindflow/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/unit_tests/dummy_diff.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/unit_tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12249 2023-06-20 21:45:45.000000 mindflow-0.5.0/mindflow/unit_tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:45:57.608683 mindflow-0.5.0/mindflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-06-20 21:45:57.000000 mindflow-0.5.0/mindflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-06-20 21:45:57.000000 mindflow-0.5.0/mindflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 21:45:57.000000 mindflow-0.5.0/mindflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-20 21:45:57.000000 mindflow-0.5.0/mindflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-20 21:45:57.000000 mindflow-0.5.0/mindflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 21:45:57.000000 mindflow-0.5.0/mindflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-20 21:45:45.000000 mindflow-0.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 21:45:57.624683 mindflow-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-20 21:45:45.000000 mindflow-0.5.0/setup.py
```

### Comparing `mindflow-0.4.0/.gitignore` & `mindflow-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mindflow-0.4.0/Makefile` & `mindflow-0.5.0/Makefile`

 * *Files identical despite different names*

### Comparing `mindflow-0.4.0/PKG-INFO` & `mindflow-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindflow
-Version: 0.4.0
+Version: 0.5.0
 Summary: AI-powered search engine for your code!
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # :brain: mindflow :ocean:
 The [ChatGPT](https://openai.com/blog/chatgpt)-powered swiss army knife for the modern developer! We provide an AI-powered CLI git wrapper, boilerplate code generator, code search engine, a conversation history manager, and much more!
```

### Comparing `mindflow-0.4.0/README.md` & `mindflow-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `mindflow-0.4.0/mindflow/cli/cli_main.py` & `mindflow-0.5.0/mindflow/cli/cli_main.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.4.0/mindflow/cli/commands/chat.py` & `mindflow-0.5.0/mindflow/cli/commands/chat.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,89 +1,74 @@
-"""
-`ask` command
-"""
 import click
 from typing import Tuple
 import os
 
-from mindflow.core.chat import run_chat
-from mindflow.core.index import run_index
-from mindflow.core.query import run_query
-from mindflow.db.db.json import JSON_DATABASE
-from mindflow.db.objects.conversation import Conversation
-from mindflow.db.objects.static_definition.conversation import ConversationID
+from mindflow.core.commands.chat import run_chat
+from mindflow.core.commands.index import run_index
+from mindflow.core.commands.query import run_query
+from mindflow.core.types.store_traits.json import save_json_store
+from mindflow.core.types.conversation import Conversation
+from mindflow.core.types.definitions.conversation import ConversationID
 
 
-def _parse_chat_prompt_args(prompt_args: Tuple[str]):
-    # takes a list of strings and returns a string along with any filenames/directories that were passed.
-    # note: if the user passes a string that contains a bunch of text, with a filename/directory in the middle,
-    # those filenames/directories will be ignored and treated as plain text.
-
+def parse_chat_prompt_and_paths_from_args(prompt_args: Tuple[str]):
     prompt = " ".join(prompt_args)  # include files/directories in prompt
     paths = []
 
     for arg in prompt_args:
-        # check if valid path string
         if os.path.exists(arg):
             paths.append(arg)
 
     return prompt, paths
 
 
 @click.command(
     help='Interact with ChatGPT, you can reference files and directories by passing them as arguments. Example: `mf chat "Please summarize this file" path/to/file.txt`'
 )
 @click.option("-s", "--skip-index", type=bool, default=False, is_flag=True)
 @click.argument("prompt_args", nargs=-1, type=str, required=True)
 def chat(prompt_args: Tuple[str], skip_index: bool):
-    prompt, paths = _parse_chat_prompt_args(prompt_args)
-
-    # if paths:
-    has_dirs = False
-    for path in paths:
-        if os.path.isdir(path):
-            has_dirs = True
-            break
+    prompt, paths = parse_chat_prompt_and_paths_from_args(prompt_args)
 
-    if has_dirs:
+    if any(os.path.isdir(path) for path in paths):
         if skip_index:
             click.echo(
                 "Skipping indexing step, only using the current index for context. You can run `mf index` to pre-index specific paths."
             )
         else:
             click.echo(
                 "Indexing paths... Note: this may take a while, if you want to skip this step, use the `--skip-index` flag. If you do so, you can pre-select specific paths to index with `mf index`.\n"
             )
 
-            run_index(paths, refresh=False, verbose=False)
+            run_index(paths)
             click.echo("")
         print(run_query(paths, prompt))
-    else:
-        print(run_chat(paths, prompt))
-        JSON_DATABASE.save_file()
+        save_json_store()
+        return
+
+    print(run_chat(paths, prompt))
+    save_json_store()
 
 
 @click.group(help="Manage conversation histories.")
 def history():
     pass
 
 
 @history.command(help="View chat history stats.")
 def stats():
-    conversation = Conversation.load(ConversationID.CHAT_0.value)
-    if conversation is None:
+    if (conversation := Conversation.load(ConversationID.CHAT_0.value)) is None:
         print("No conversation history found.")
         return
 
     print("Num messages:", len(conversation.messages))
     print("Total tokens:", conversation.total_tokens)
 
 
 @history.command(help="Clear the chat history.")
 def clear():
-    conversation = Conversation.load(ConversationID.CHAT_0.value)
-    if conversation is None:
+    if (conversation := Conversation.load(ConversationID.CHAT_0.value)) is None:
         print("No conversation history found.")
         return
 
     conversation.messages = []
     conversation.save()
```

### Comparing `mindflow-0.4.0/mindflow/cli/commands/config.py` & `mindflow-0.5.0/mindflow/cli/commands/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 import sys
 from typing import List
 import click
-from mindflow.db.db.json import JSON_DATABASE
-from mindflow.db.objects.mindflow_model import (
+from mindflow.core.types.store_traits.json import save_json_store
+from mindflow.core.types.mindflow_model import (
     MindFlowModel,
     MindFlowModelConfig,
     MindFlowModelID,
 )
 
-from mindflow.db.objects.static_definition.model import (
+from mindflow.core.types.definitions.model import (
     ModelID,
 )
-from mindflow.db.objects.model import Model
-from mindflow.db.utils import getOrCreateObject
+from mindflow.core.types.model import Model
 
 
 @click.command(
     help="Configure MindFlow. For example, you can configure the model to use."
 )
 def config():
     config_options = ["model"]
     selected_config = select_option(
         "What do you want to configure? Enter #", config_options, config_options
     )
     if selected_config == "model":
-        model_selection()
+        configure_model()
 
-    JSON_DATABASE.save_file()
+    save_json_store()
 
 
-def model_selection():
+def configure_model():
     mindflow_model_ids = [
         MindFlowModelID.QUERY.value,
         MindFlowModelID.INDEX.value,
         MindFlowModelID.EMBEDDING.value,
     ]
     mindflow_model_options: List[MindFlowModel] = [
         MindFlowModel.load(mindflow_model_id)
@@ -45,22 +44,22 @@
 
     selected_mindflow_model: MindFlowModel = select_option(
         "Select MindFlow model. Enter #",
         mindflow_model_options,
         mindflow_model_descriptions,
     )
     if selected_mindflow_model.id == MindFlowModelID.QUERY.value:
-        query_model_selection()
+        configure_query_model()
     elif selected_mindflow_model.id == MindFlowModelID.INDEX.value:
-        index_model_selection()
+        configure_index_model()
     elif selected_mindflow_model.id == MindFlowModelID.EMBEDDING.value:
-        embedding_model_selection()
+        configure_embedding_model()
 
 
-def query_model_selection():
+def configure_query_model():
     model_ids = [
         ModelID.GPT_3_5_TURBO.value,
         ModelID.GPT_4.value,
         ModelID.CLAUDE_INSTANT_V1.value,
         ModelID.CLAUDE_V1.value,
     ]
     model_options: List[Model] = [Model.load(model_id) for model_id in model_ids]
@@ -69,25 +68,24 @@
     ]
 
     selected_model: Model = select_option(
         "Select chat model. Recommended GPT-4/Claude V1. Enter #",
         model_options,
         model_descriptions,
     )
-
-    mindflow_model_config: MindFlowModelConfig = getOrCreateObject(
-        MindFlowModelConfig, f"{MindFlowModelID.QUERY.value}_config"
-    )
+    mindflow_model_config: MindFlowModelConfig = MindFlowModelConfig.load(
+        f"{MindFlowModelID.QUERY.value}_config"
+    ) or MindFlowModelConfig(f"{MindFlowModelID.QUERY.value}_config")
     mindflow_model_config.model = selected_model.id
     mindflow_model_config.save()
 
     print(f"Query Model: {selected_model.id} saved!")
 
 
-def index_model_selection():
+def configure_index_model():
     model_ids = [
         ModelID.GPT_3_5_TURBO.value,
         ModelID.GPT_4.value,
         ModelID.CLAUDE_INSTANT_V1.value,
         ModelID.CLAUDE_V1.value,
     ]
     model_options: List[Model] = [Model.load(model_id) for model_id in model_ids]
@@ -96,62 +94,61 @@
     ]
 
     selected_model: Model = select_option(
         "Select chat model. Recommended GPT-3.5 Turbo/Claude Instant V1. Enter #",
         model_options,
         model_descriptions,
     )
-    mindflow_model_config: MindFlowModelConfig = getOrCreateObject(
-        MindFlowModelConfig, f"{MindFlowModelID.INDEX.value}_config"
-    )
+    mindflow_model_config: MindFlowModelConfig = MindFlowModelConfig.load(
+        f"{MindFlowModelID.INDEX.value}_config"
+    ) or MindFlowModelConfig(f"{MindFlowModelID.INDEX.value}_config")
     mindflow_model_config.model = selected_model.id
     mindflow_model_config.save()
 
     print(f"Index Model: {selected_model.id} saved!")
 
 
-def embedding_model_selection():
+def configure_embedding_model():
     model_ids = [ModelID.TEXT_EMBEDDING_ADA_002.value]
     model_options: List[Model] = [Model.load(model_id) for model_id in model_ids]
     model_descriptions: List[str] = [
         model.config_description for model in model_options
     ]
 
     selected_model: Model = select_option(
         "Select chat model. Only one option... for now :) Enter #",
         model_options,
         model_descriptions,
     )
-
-    mindflow_model_config: MindFlowModelConfig = getOrCreateObject(
-        MindFlowModelConfig, f"{MindFlowModelID.EMBEDDING.value}_config"
-    )
+    mindflow_model_config: MindFlowModelConfig = MindFlowModelConfig.load(
+        f"{MindFlowModelID.EMBEDDING.value}_config"
+    ) or MindFlowModelConfig(f"{MindFlowModelID.EMBEDDING.value}_config")
     mindflow_model_config.model = selected_model.id
     mindflow_model_config.save()
 
     print(f"Embedding Model: {selected_model.id} saved!")
 
 
 def clear_console(lines: int):
     for _ in range(lines):
         sys.stdout.write("\033[F")  # Move cursor up one line
         sys.stdout.write("\033[K")  # Clear the line
 
 
-# Takes a prompt and a list of descriptions and returns the index of the selected description
 def select_option(prompt: str, options: List, descriptions: List[str]) -> int:
-    # Print options with numbers
     for i, description in enumerate(descriptions, 1):
         click.echo(f"{i}: {description}")
 
-    # Validate input and adjust index for 0-based list
     lines_to_clear = len(descriptions)
     while True:
-        selected_option_index = click.prompt(prompt, type=int)
         lines_to_clear += 1
-        if 1 <= selected_option_index <= len(descriptions):
+        if (
+            1
+            <= (selected_option_index := click.prompt(prompt, type=int))
+            <= len(descriptions)
+        ):
             break
         click.echo("Invalid selection. Please try again.")
         lines_to_clear += 1
 
     clear_console(lines_to_clear)
     return options[selected_option_index - 1]
```

### Comparing `mindflow-0.4.0/mindflow/cli/commands/git/commit.py` & `mindflow-0.5.0/mindflow/cli/commands/git/commit.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Tuple, Optional
 
 import click
 
 from mindflow.cli.util import passthrough_command
-from mindflow.core.git.commit import run_commit
+from mindflow.core.commands.git.commit import run_commit
 
 
 @passthrough_command(help="Generate a git commit response by feeding git diff to gpt")
 # @overloaded_option(
 #     "-m",
 #     "--message",
 #     help="Don't use mindflow to generate a commit message, use this one instead.",
@@ -16,17 +16,14 @@
 @click.option(
     "-m",
     "--message",
     help="Don't use mindflow to generate a commit message, use this one instead.",
     default=None,
 )
 def commit(args: Tuple[str], message: Optional[str] = None):
-    """
-    Commit command.
-    """
     if message is not None:
         click.echo(
             f"Warning: Using message '{message}' instead of mindflow generated message."
         )
         click.echo("It's recommended that you don't use the -m/--message flag.")
 
     print(run_commit(args, message_overwrite=message))
```

### Comparing `mindflow-0.4.0/mindflow/cli/commands/git/diff.py` & `mindflow-0.5.0/mindflow/cli/commands/git/diff.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 """
 `diff` command
 """
 from typing import Tuple
 import click
 
 from mindflow.cli.util import passthrough_command
-from mindflow.core.git.diff import run_diff
+from mindflow.core.commands.git.diff import run_diff
 
 
 @passthrough_command(
     help="Wrapper around git diff that summarizes the output. Treat this command exactly like git diff, it supports all arguments that git diff provides."
 )
 @click.option("--detailed", type=bool, default=False, is_flag=True)
 def diff(args: Tuple[str], detailed: bool):
     if not detailed:
         click.echo(
             "Working on a summary of the diff, use the `--detailed` flag to show a much more thorough breakdown of the diff...\n"
         )
-    diff_output = run_diff(args, detailed=detailed)
-    if diff_output is not None:
+    if (diff_output := run_diff(args, detailed=detailed)) is not None:
         click.echo(diff_output)
-    else:
-        pass
```

### Comparing `mindflow-0.4.0/mindflow/cli/commands/git/mr.py` & `mindflow-0.5.0/mindflow/cli/commands/git/mr.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional, Tuple
 
 import click
 from mindflow.cli.util import passthrough_command
-from mindflow.core.git.mr import run_mr
+from mindflow.core.commands.git.mr import run_mr
 
 
 @click.group()
 def mr():
     """
     MR command.
     """
@@ -25,17 +25,14 @@
     "--description",
     help="Don't use mindflow to generate a pr body, use this one instead.",
     default=None,
 )
 def create(
     args: Tuple[str], title: Optional[str] = None, description: Optional[str] = None
 ):
-    """
-    PR command.
-    """
     if title is not None:
         click.echo(
             f"Warning: Using message '{title}' instead of mindflow generated message."
         )
         click.echo("It's recommended that you don't use the -t/--title flag.")
 
     if description is not None:
```

### Comparing `mindflow-0.4.0/mindflow/cli/commands/git/pr.py` & `mindflow-0.5.0/mindflow/cli/commands/git/pr.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional, Tuple
 
 import click
 from mindflow.cli.util import passthrough_command
-from mindflow.core.git.pr import run_pr
+from mindflow.core.commands.git.pr import run_pr
 
 
 @click.group()
 def pr():
     """
     PR command.
     """
@@ -23,17 +23,14 @@
 @click.option(
     "-b",
     "--body",
     help="Don't use mindflow to generate a pr body, use this one instead.",
     default=None,
 )
 def create(args: Tuple[str], title: Optional[str] = None, body: Optional[str] = None):
-    """
-    PR command.
-    """
     if title is not None:
         click.echo(
             f"Warning: Using message '{title}' instead of mindflow generated message."
         )
         click.echo("It's recommended that you don't use the -t/--title flag.")
 
     if body is not None:
```

### Comparing `mindflow-0.4.0/mindflow/cli/util.py` & `mindflow-0.5.0/mindflow/cli/util.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.4.0/mindflow/core/gen.py` & `mindflow-0.5.0/mindflow/core/commands/gen.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,72 +1,63 @@
 import os
 from typing import Union
 import click
-from mindflow.db.objects.conversation import Conversation
-from mindflow.db.objects.static_definition.conversation import ConversationID
-from mindflow.settings import Settings
-from mindflow.utils.errors import ModelError
-from mindflow.utils.helpers import get_text_within_xml
+from mindflow.core.types.conversation import Conversation
+from mindflow.core.types.definitions.conversation import ConversationID
+from mindflow.core.settings import Settings
+from mindflow.core.errors import ModelError
+from mindflow.core.text_processing.xml import get_text_within_xml
 
-from mindflow.utils.prompt_builders import (
+from mindflow.core.prompt_builders import (
     Role,
-    build_prompt,
-    create_message,
-    prune_messages,
+    build_prompt_from_conversation_messages,
+    create_conversation_message,
+    prune_messages_to_fit_context_window,
 )
-from mindflow.utils.token import estimate_tokens_from_messages
+from mindflow.core.token_counting import get_token_count_of_messages_for_model
 
 
-CODE_GEN_SYSTEM_PROMPT = "All responses must be valid code for the specified language. Do not use any special characters or symbols, any additional information must be put in comments."
-
-
-def run_code_generation(output_path: str, prompt: str):
+def run_code_generation(output_path: str, prompt: str) -> str:
     settings = Settings()
     completion_model = settings.mindflow_models.query.model
 
     if os.path.exists(output_path):
         click.confirm(
             f"The output path '{output_path}' already exists. Do you want to overwrite it?",
             abort=True,
         )
         os.remove(output_path)
 
-    output_path_dir = os.path.dirname(output_path)
-    if len(output_path_dir) > 0:
+    if len((output_path_dir := os.path.dirname(output_path))) > 0:
         os.makedirs(output_path_dir, exist_ok=True)
 
-    conversation = Conversation.load(ConversationID.CODE_GEN_0.value)
-    if conversation is None:
+    if (conversation := Conversation.load(ConversationID.CODE_GEN_0.value)) is None:
         conversation = Conversation(
             {"id": ConversationID.CODE_GEN_0.value, "messages": [], "total_tokens": 0}
         )
 
     conversation.messages.append(
-        create_message(
+        create_conversation_message(
             Role.USER.value,
             f"Generate code for '{output_path}' with the following prompt: '{prompt}'. Do NOT use any special characters or symbols, any additional information must be put in comments. Please put the code within XML tags like <GEN></GEN>.",
         )
     )
-    conversation.messages = prune_messages(conversation.messages, completion_model)
+    conversation.messages = prune_messages_to_fit_context_window(
+        conversation.messages, completion_model
+    )
 
     response: Union[ModelError, str] = completion_model(
-        build_prompt(conversation.messages, completion_model)
+        build_prompt_from_conversation_messages(conversation.messages, completion_model)
     )
     if isinstance(response, ModelError):
         return response.message
 
-    response = get_text_within_xml(response, "GEN")
+    with open(output_path, "w") as f:
+        f.write(get_text_within_xml(response, "GEN"))
 
-    parse_and_write_file(response, output_path)
-    conversation.total_tokens = estimate_tokens_from_messages(
+    conversation.total_tokens = get_token_count_of_messages_for_model(
         conversation.messages, completion_model
     )
 
     conversation.save()
 
     return f"Code generation complete. Your code is ready to go at {output_path}!"
-
-
-def parse_and_write_file(response: str, output_path: str):
-    # take the response and parse it into a valid file.
-    with open(output_path, "w") as f:
-        f.write(response)
```

### Comparing `mindflow-0.4.0/mindflow/core/git/diff.py` & `mindflow-0.5.0/mindflow/core/commands/git/diff.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-"""
-`diff` command
-"""
 import concurrent.futures
+import os
 
 from typing import Dict, Optional, Union
 from typing import List
 from typing import Tuple
 
-from mindflow.db.objects.model import ConfiguredModel
-from mindflow.settings import Settings
-from mindflow.utils.constants import MinimumReservedLength
-from mindflow.utils.errors import ModelError
-from mindflow.utils.execute import execute_no_trace
-from mindflow.utils.prompt_builders import Role, build_prompt, create_message
-from mindflow.utils.prompts import GIT_DIFF_PROMPT_PREFIX
+from mindflow.core.types.model import ConfiguredModel
+from mindflow.core.settings import Settings
+from mindflow.core.constants import MinimumReservedLength
+from mindflow.core.errors import ModelError
+from mindflow.core.execute import execute_command_and_print_without_trace
+from mindflow.core.prompt_builders import (
+    Role,
+    build_prompt_from_conversation_messages,
+    create_conversation_message,
+)
+from mindflow.core.prompts import GIT_DIFF_PROMPT_PREFIX, GIT_DIFF_SUMMARIZE_PROMPT
 
-from mindflow.utils.diff_parser import parse_git_diff
-from mindflow.utils.token import get_token_count
+from mindflow.core.token_counting import get_token_count_of_text_for_model
 from tqdm import tqdm
 
 
 def run_diff(args: Tuple[str], detailed: bool = True) -> Optional[str]:
-    """
-    This function is used to generate a git diff response by feeding git diff to gpt.
-    """
-    command = ["git", "diff"] + list(args)
-
+    """Execute git diff and summarize with GPT."""
     settings = Settings()
     completion_model: ConfiguredModel = settings.mindflow_models.query.model
 
-    # Execute the git diff command and retrieve the output as a string
-    diff_result = execute_no_trace(command)
-    if diff_result.strip() == "":
+    diff_result = execute_command_and_print_without_trace(
+        ["git", "diff"] + list(args)
+    ).strip()
+    if not diff_result:
         return None
 
     diff_dict, excluded_filenames = parse_git_diff(diff_result)
-    if len(diff_dict) <= 0:
+    if not diff_dict:
         return None
 
     batched_parsed_diff_result = batch_git_diffs(diff_dict, completion_model)
 
     diff_summary: str = ""
     if len(batched_parsed_diff_result) == 1:
         content = ""
         for file_name, diff_content in batched_parsed_diff_result[0]:
             content += f"*{file_name}*\n DIFF CONTENT: {diff_content}\n\n"
         diff_response: Union[ModelError, str] = completion_model(
-            build_prompt(
+            build_prompt_from_conversation_messages(
                 [
-                    create_message(Role.SYSTEM.value, GIT_DIFF_PROMPT_PREFIX),
-                    create_message(Role.USER.value, content),
+                    create_conversation_message(
+                        Role.SYSTEM.value, GIT_DIFF_PROMPT_PREFIX
+                    ),
+                    create_conversation_message(Role.USER.value, content),
                 ],
                 completion_model,
             )
         )
         if isinstance(diff_response, ModelError):
             return diff_response.diff_message
         diff_summary += diff_response
@@ -62,18 +62,20 @@
             futures = []
             for batch in batched_parsed_diff_result:
                 content = ""
                 for file_name, diff_content in batch:
                     content += f"*{file_name}*\n DIFF CONTENT: {diff_content}\n\n"
                 future: concurrent.futures.Future = executor.submit(
                     completion_model,
-                    build_prompt(
+                    build_prompt_from_conversation_messages(
                         [
-                            create_message(Role.SYSTEM.value, GIT_DIFF_PROMPT_PREFIX),
-                            create_message(Role.USER.value, content),
+                            create_conversation_message(
+                                Role.SYSTEM.value, GIT_DIFF_PROMPT_PREFIX
+                            ),
+                            create_conversation_message(Role.USER.value, content),
                         ],
                         completion_model,
                     ),
                 )
                 futures.append(future)
 
             # Process the results as they become available
@@ -86,74 +88,137 @@
 
     if len(excluded_filenames) > 0:
         diff_summary += f"\n\nNOTE: The following files were excluded from the diff: {', '.join(excluded_filenames)}"
 
     if detailed:
         return diff_summary
 
-    GIT_DIFF_SUMMARIZE_PROMPT = 'What is the higher level purpose of these changes? Keep it short and sweet, don\'t provide any useless or redundant information like "made changes to the code". Do NOT speak in generalities, be specific.'
     summarized = completion_model(
-        build_prompt(
+        build_prompt_from_conversation_messages(
             [
-                create_message(Role.SYSTEM.value, GIT_DIFF_SUMMARIZE_PROMPT),
-                create_message(Role.USER.value, content),
+                create_conversation_message(
+                    Role.SYSTEM.value, GIT_DIFF_SUMMARIZE_PROMPT
+                ),
+                create_conversation_message(Role.USER.value, content),
             ],
             completion_model,
         )
     )
     return summarized
 
 
-import re
+# NOTE: make sure to have a the "." in the file extension (if applicable)
+# NOTE: these are things that WON'T already be git ignored.
+IGNORE_FILE_EXTENSIONS = [
+    ".pyc",
+    ".ipynb",
+    ".ipynb_checkpoints",
+    ".png",
+    ".jpg",
+    ".jpeg",
+    ".svg",
+    ".gif",
+    ".mp4",
+    ".mp3",
+    ".mov",
+    ".wav",
+    ".avi",
+    ".zip",
+    ".tar",
+    ".gzip",
+    ".pth",
+    ".pt",
+    ".exe",
+    ".jar",
+    ".csv",  # maybe not?
+    ".bmp",
+    ".emg",
+]
+
+
+def parse_git_diff(diff_str: str):
+    diffs = {}
+    current_file = None
+    current_diff = []  # type: ignore
+
+    excluded_files = []
+
+    for line in diff_str.splitlines(keepends=True):
+        if line.startswith("diff --git"):
+            # Starting a new file
+            if current_file:
+                # Add the previous diff to the dictionary
+                diffs[current_file] = "".join(current_diff)
+
+            current_file = line.split()[-1]
+            current_ext = os.path.splitext(current_file)[1]
+
+            if current_ext in IGNORE_FILE_EXTENSIONS:
+                excluded_files.append(current_file)
+
+                # Ignore this file
+                current_file = None
+                current_diff = []
+                continue
+
+            current_diff = [line]
+        else:
+            # skip lines if we are ignoring this file (TODO - this is a bit hacky)
+            if current_file:
+                current_diff.append(line)
+
+    # Add the last diff to the dictionary
+    if current_file:
+        diffs[current_file] = "".join(current_diff)
+
+    return diffs, excluded_files
 
 
 def batch_git_diffs(
     file_diffs: Dict[str, str], model: ConfiguredModel
 ) -> List[List[Tuple[str, str]]]:
     batches = []
     current_batch: List = []
     current_batch_text = ""
     for file_name, diff_content in file_diffs.items():
         if (
-            get_token_count(model, diff_content)
+            get_token_count_of_text_for_model(model, diff_content)
             > model.hard_token_limit - MinimumReservedLength.DIFF.value
         ):
-            ## Split the diff into chunks that are less than the token limit
             chunks = [diff_content]
             while True:
                 new_chunks = []
                 for chunk in chunks:
                     if (
-                        get_token_count(model, chunk)
+                        get_token_count_of_text_for_model(model, chunk)
                         > model.hard_token_limit - MinimumReservedLength.DIFF.value
                     ):
                         half_len = len(chunk) // 2
                         left_half = chunk[:half_len]
                         right_half = chunk[half_len:]
                         new_chunks.extend([left_half, right_half])
                     else:
                         new_chunks.append(chunk)
                 if new_chunks == chunks:
                     break
                 chunks = new_chunks
 
-            ## Add the chunks to the batch or multiple batches
             for chunk in chunks:
                 if (
-                    get_token_count(model, current_batch_text + chunk)
+                    get_token_count_of_text_for_model(model, current_batch_text + chunk)
                     > model.hard_token_limit - MinimumReservedLength.DIFF.value
                 ):
                     batches.append(current_batch)
                     current_batch = []
                     current_batch_text = ""
                 current_batch.append((file_name, chunk))
                 current_batch_text += chunk
 
         elif (
-            get_token_count(model, current_batch_text + diff_content)
+            get_token_count_of_text_for_model(model, current_batch_text + diff_content)
             > model.hard_token_limit - MinimumReservedLength.DIFF.value
         ):
             batches.append(current_batch)
             current_batch = [(file_name, diff_content)]
             current_batch_text = diff_content
         else:
             current_batch.append((file_name, diff_content))
```

### Comparing `mindflow-0.4.0/mindflow/core/git/pr.py` & `mindflow-0.5.0/mindflow/core/commands/git/pr.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,48 @@
 import concurrent.futures
 import subprocess
-from typing import List, Optional, Tuple, Union
+from typing import Optional, Tuple, Union
 
-from mindflow.core.git.diff import run_diff
-from mindflow.settings import Settings
-from mindflow.utils.command_parse import get_flag_value
-from mindflow.utils.errors import ModelError
-from mindflow.utils.execute import execute_no_trace
-from mindflow.utils.prompt_builders import Role, build_prompt, create_message
-from mindflow.utils.prompts import PR_BODY_PREFIX
-from mindflow.utils.prompts import PR_TITLE_PREFIX
+from mindflow.core.commands.git.diff import run_diff
+from mindflow.core.settings import Settings
+from mindflow.core.command_parse import get_flag_values_from_args
+from mindflow.core.errors import ModelError
+from mindflow.core.execute import execute_command_and_print_without_trace
+from mindflow.core.prompt_builders import (
+    Role,
+    build_prompt_from_conversation_messages,
+    create_conversation_message,
+)
+from mindflow.core.prompts import PR_BODY_PREFIX
+from mindflow.core.prompts import PR_TITLE_PREFIX
 
 
 def run_pr(args: Tuple[str], title: Optional[str] = None, body: Optional[str] = None):
-    base_branch = get_flag_value(args, ["--base", "-B"])
-
-    if base_branch is None:
-        # Determine the name of the default branch
-        base_branch = (
+    if (base_branch_name := get_flag_values_from_args(args, ["--base", "-B"])) is None:
+        base_branch_name = (
             subprocess.check_output(["git", "symbolic-ref", "refs/remotes/origin/HEAD"])
             .decode()
             .strip()
             .split("/")[-1]
         )
 
     if not title or not body:
-        title_body_tuple = create_title_and_body(base_branch, title, body)
+        title, body = create_title_and_body(base_branch_name, title, body) or (
+            None,
+            None,
+        )
 
-    if not title_body_tuple:
+    if not title or not body:
         return
 
-    title, body = title_body_tuple
-
-    command: List[str] = ["gh", "pr", "create"] + list(args) + ["--title", title, "--body", body]  # type: ignore
-    print(execute_no_trace(command))
+    print(
+        execute_command_and_print_without_trace(
+            ["gh", "pr", "create"] + list(args) + ["--title", title, "--body", body]
+        )
+    )
 
 
 def create_title_and_body(
     base_branch, title: Optional[str], body: Optional[str]
 ) -> Optional[Tuple[str, str]]:
     settings = Settings()
     completion_model = settings.mindflow_models.query.model
@@ -45,25 +50,25 @@
     diff_output = run_diff((base_branch,))
     if not diff_output:
         diff_output = ""
 
     title_response: Union[ModelError, str]
     body_response: Union[ModelError, str]
     if title is None and body is None:
-        pr_title_prompt = build_prompt(
+        pr_title_prompt = build_prompt_from_conversation_messages(
             [
-                create_message(Role.SYSTEM.value, PR_TITLE_PREFIX),
-                create_message(Role.USER.value, diff_output),
+                create_conversation_message(Role.SYSTEM.value, PR_TITLE_PREFIX),
+                create_conversation_message(Role.USER.value, diff_output),
             ],
             completion_model,
         )
-        pr_body_prompt = build_prompt(
+        pr_body_prompt = build_prompt_from_conversation_messages(
             [
-                create_message(Role.SYSTEM.value, PR_BODY_PREFIX),
-                create_message(Role.USER.value, diff_output),
+                create_conversation_message(Role.SYSTEM.value, PR_BODY_PREFIX),
+                create_conversation_message(Role.USER.value, diff_output),
             ],
             completion_model,
         )
 
         with concurrent.futures.ThreadPoolExecutor() as executor:
             future_title = executor.submit(
                 settings.mindflow_models.query.model, pr_title_prompt
@@ -72,35 +77,36 @@
                 settings.mindflow_models.query.model, pr_body_prompt
             )
 
         title_response = future_title.result()
         body_response = future_body.result()
     else:
         if title is None:
-            pr_title_prompt = build_prompt(
+            pr_title_prompt = build_prompt_from_conversation_messages(
                 [
-                    create_message(Role.SYSTEM.value, PR_TITLE_PREFIX),
-                    create_message(Role.USER.value, diff_output),
+                    create_conversation_message(Role.SYSTEM.value, PR_TITLE_PREFIX),
+                    create_conversation_message(Role.USER.value, diff_output),
                 ],
                 completion_model,
             )
             title_response = completion_model(pr_title_prompt)
         if body is None:
-            pr_body_prompt = build_prompt(
+            pr_body_prompt = build_prompt_from_conversation_messages(
                 [
-                    create_message(Role.SYSTEM.value, PR_BODY_PREFIX),
-                    create_message(Role.USER.value, diff_output),
+                    create_conversation_message(Role.SYSTEM.value, PR_BODY_PREFIX),
+                    create_conversation_message(Role.USER.value, diff_output),
                 ],
                 completion_model,
             )
             body_response = completion_model(pr_body_prompt)
 
     if isinstance(title_response, ModelError):
         print(title_response.pr_message)
         return None
     if isinstance(body_response, ModelError):
         print(body_response.pr_message)
         return None
 
-    title = title if title is not None else title_response
-    body = body if body is not None else body_response
-    return title, body
+    return (
+        title if title is not None else title_response,
+        body if body is not None else body_response,
+    )
```

### Comparing `mindflow-0.4.0/mindflow/core/inspect.py` & `mindflow-0.5.0/mindflow/core/commands/delete.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,57 +1,33 @@
-"""
-`inspect` command
-"""
-import json
-from typing import List, Optional, Tuple
+from typing import List
 
-from mindflow.db.objects.document import (
+from mindflow.core.types.document import (
     Document,
     DocumentChunk,
+    DocumentReference,
     get_document_chunk_ids,
     get_document_id,
 )
-from mindflow.resolving.resolve import resolve_all
+from mindflow.core.resolving.resolve import resolve_paths_to_document_references
 
 
-def run_inspect(document_paths: List[str]) -> str:
-    """
-    This function is used to inspect your MindFlow index.
-    """
-    resolved: List[Tuple[str, str]] = resolve_all(document_paths)
-
-    document_ids = [
-        document_id
-        for document_id in [
-            get_document_id(doc_path, doc_type) for doc_path, doc_type in resolved
-        ]
-        if document_id is not None
-    ]
-    document_chunk_ids = get_document_chunk_ids(
-        Document.load_bulk(document_ids, return_none=False)
-    )
-
-    if len(document_chunk_ids) == 0:
-        return "No documents to inspect"
-
-    document_chunks: List[Optional[DocumentChunk]] = DocumentChunk.load_bulk(
-        document_chunk_ids, return_none=False
-    )
-
-    # Dump the document chunks to JSON without the embedding
-    inspect_output = json.dumps(
-        {
-            document_chunk.id: {
-                k: v
-                for k, v in document_chunk.todict(document_chunk).items()
-                if k != "embedding"
-            }
-            for document_chunk in document_chunks
-            if document_chunk is not None
-        },
-        indent=4,
-    )
-
-    if inspect_output != "null":
-        return inspect_output
-    else:
-        return "No documents to inspect"
+def run_delete(document_paths: List[str]) -> str:
+    """Delete documents from MindFlow index."""
+    document_references: List[DocumentReference] = resolve_paths_to_document_references(document_paths)
+
+    document_ids = [document_id for document_id in [get_document_id(document_reference.path, document_reference.document_type) for document_reference in document_references] if document_id is not None]
+
+    if not document_ids:
+        return "No document IDs resolved. Nothing to delete."
+
+    documents = Document.load_bulk_ignore_missing(document_ids)
+    if not documents:
+        return "No documents found to delete."
+
+    document_chunk_ids = get_document_chunk_ids(documents)
+    if not DocumentChunk.load_bulk_ignore_missing(document_chunk_ids):
+        return "No document chunks found to delete."
+
+    Document.delete_bulk(document_ids)
+    DocumentChunk.delete_bulk(document_chunk_ids)
+
+    return True, "Documents and associated chunks deleted successfully."
```

### Comparing `mindflow-0.4.0/mindflow/core/login.py` & `mindflow-0.5.0/mindflow/core/commands/login.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from mindflow.cli.commands.config import select_option
-from mindflow.db.db.json import JSON_DATABASE
-from mindflow.db.objects.service import ServiceConfig
-from mindflow.db.objects.static_definition.service import ServiceConfigID
+from mindflow.core.types.store_traits.json import save_json_store
+from mindflow.core.types.service import ServiceConfig
+from mindflow.core.types.definitions.service import ServiceConfigID
 
 
 def run_login():
     service_ids = [
         ServiceConfigID.OPENAI.value,
         ServiceConfigID.ANTHROPIC.value,
         ServiceConfigID.PINECONE.value,
@@ -22,8 +22,8 @@
 
     service_config.api_key = input("Enter API key: ")
     if service_config.id == ServiceConfigID.PINECONE.value:
         service_config.environment = input("Enter environment: ")
 
     service_config.save()
 
-    JSON_DATABASE.save_file()
+    save_json_store()
```

### Comparing `mindflow-0.4.0/mindflow/core/query.py` & `mindflow-0.5.0/mindflow/core/commands/query.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,128 +1,124 @@
-"""
-`query` command
-"""
 import sys
 
 from typing import Dict, List, Union, Tuple
 
 import numpy as np
 
-from mindflow.db.objects.document import (
+from mindflow.core.types.document import (
     Document,
     DocumentChunk,
     get_document_chunk_ids,
     get_document_id,
 )
-from mindflow.db.objects.model import ConfiguredModel
-from mindflow.resolving.resolve import resolve_all
-from mindflow.settings import Settings
-from mindflow.utils.constants import MinimumReservedLength
-from mindflow.utils.errors import ModelError
-from mindflow.utils.prompt_builders import Role, build_prompt, create_message
-from mindflow.utils.prompts import QUERY_PROMPT_PREFIX
-from mindflow.utils.token import get_token_count
+from mindflow.core.types.model import ConfiguredModel
+from mindflow.core.resolving.resolve import resolve_paths_to_document_references
+from mindflow.core.settings import Settings
+from mindflow.core.constants import MinimumReservedLength
+from mindflow.core.errors import ModelError
+from mindflow.core.prompt_builders import (
+    Role,
+    build_prompt_from_conversation_messages,
+    create_conversation_message,
+)
+from mindflow.core.prompts import QUERY_PROMPT_PREFIX
+from mindflow.core.token_counting import get_token_count_of_text_for_model
 
 
-def run_query(document_paths: List[str], query: str):
-    """
-    This function is used to ask a custom question about files, folders, and websites.
-    """
+def run_query(document_paths: List[str], query: str) -> str:
+    """Query files, folders, and websites."""
     settings = Settings()
     completion_model = settings.mindflow_models.query.model
     embedding_model = settings.mindflow_models.embedding.model
 
-    # Resolve all paths and get a mapping to their local paths
-    resolved: List[Tuple[str, str]] = resolve_all(document_paths)
-    document_hash_to_path: Dict[str, str] = {}
-    for document_path, document_type in resolved:
-        document_id = get_document_id(document_path, document_type)
-        if document_id is not None:
-            document_hash_to_path[document_id] = document_path
-
-    # Query vector DB for the top 100 document chunks
-    document_chunk_ids = get_document_chunk_ids(
-        Document.load_bulk(list(document_hash_to_path.keys()), return_none=False)
-    )
-    top_document_chunks: List[DocumentChunk] = DocumentChunk.query(
-        vector=np.array(embedding_model(query)).reshape(1, -1), ids=document_chunk_ids
+    document_hash_to_path: Dict[str, str] = {
+        document_id: doc_reference.path
+        for doc_reference in resolve_paths_to_document_references(document_paths)
+        if (
+            document_id := get_document_id(
+                doc_reference.path, doc_reference.document_type
+            )
+        )
+        is not None
+    }
+
+    document_chunk_ids: List[str] = get_document_chunk_ids(
+        Document.load_bulk_ignore_missing(list(document_hash_to_path.keys()))
     )
 
-    # Create a list of tuples of the form (path, DocumentChunk) to be used in select_content
+    if not (
+        top_document_chunks := DocumentChunk.query(
+            vector=np.array(embedding_model(query)).reshape(1, -1),
+            ids=document_chunk_ids,
+            top_k=100,
+        )
+    ):
+        return "No index for requested hashes. Please generate index for passed content."
+
     document_selection_batch: List[Tuple[str, DocumentChunk]] = [
         (document_hash_to_path[document_chunk.id.split("_")[0]], document_chunk)
         for document_chunk in top_document_chunks
     ]
 
-    if len(top_document_chunks) == 0:
-        print(
-            "No index for requested hashes. Please generate index for passed content."
-        )
-        sys.exit(1)
-
-    # Select the top content that can fit in the prompt
-    selected_content: str = select_content(
+    trimmed_content: str = select_and_trim_text_to_fit_context_window(
         query, document_selection_batch, completion_model
     )
     response: Union[ModelError, str] = completion_model(
-        build_prompt(
+        build_prompt_from_conversation_messages(
             [
-                create_message(Role.SYSTEM.value, QUERY_PROMPT_PREFIX),
-                create_message(Role.USER.value, f"{query}\n\n{selected_content}"),
+                create_conversation_message(Role.SYSTEM.value, QUERY_PROMPT_PREFIX),
+                create_conversation_message(
+                    Role.USER.value, f"{query}\n\n{trimmed_content}"
+                ),
             ],
             completion_model,
         )
     )
     if isinstance(response, ModelError):
         return response.query_message
 
     return response
 
 
-def select_content(
+def select_and_trim_text_to_fit_context_window(
     query: str,
     top_document_chunks: List[Tuple[str, DocumentChunk]],
     completion_model: ConfiguredModel,
 ) -> str:
-    """
-    This function is used to generate a prompt based on a question or summarization task
-    """
-
     selected_content: str = ""
     for path, document_chunk in top_document_chunks:
         with open(path, "r", encoding="utf-8") as file:
             file.seek(document_chunk.start_pos)
-            text = file.read(
-                int(document_chunk.end_pos) - int(document_chunk.start_pos)
+            selected_content += formatted_chunk(
+                path,
+                document_chunk,
+                file.read(int(document_chunk.end_pos) - int(document_chunk.start_pos)),
             )
-
-            selected_content += formatted_chunk(path, document_chunk, text)
-
             if (
-                get_token_count(completion_model, query + selected_content)
+                get_token_count_of_text_for_model(
+                    completion_model, query + selected_content
+                )
                 > completion_model.hard_token_limit
             ):
                 break
 
-    # Perform a binary search to trim the selected content to fit within the token limit
     left, right = 0, len(selected_content)
     while left <= right:
         mid = (left + right) // 2
         if (
-            get_token_count(completion_model, query + selected_content[:mid])
+            get_token_count_of_text_for_model(
+                completion_model, query + selected_content[:mid]
+            )
             <= completion_model.hard_token_limit - MinimumReservedLength.QUERY.value
         ):
             left = mid + 1
-        else:
-            right = mid - 1
-
-    # Trim the selected content to the new bounds
-    selected_content = selected_content[:right]
+            continue
+        right = mid - 1
 
-    return selected_content
+    return selected_content[:right]
 
 
 def formatted_chunk(path: str, document_chunk: DocumentChunk, text: str) -> str:
     return (
         "Path: "
         + path
         + " Start: "
```

### Comparing `mindflow-0.4.0/mindflow/db/objects/mindflow_model.py` & `mindflow-0.5.0/mindflow/core/types/mindflow_model.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,101 +1,80 @@
 import sys
 from typing import Dict
-from typing import Optional
-from mindflow.db.db.json import JSON_DATABASE
-from mindflow.db.db.static import STATIC_DATABASE
-
-from mindflow.db.db.database import Collection
-from mindflow.db.objects.base import BaseObject
-from mindflow.db.objects.model import ConfiguredModel
-from mindflow.db.objects.service import ConfiguredServices
-from mindflow.db.objects.static_definition.mind_flow_model import MindFlowModelID
-from mindflow.db.objects.static_definition.service import (
+from mindflow.core.types.store_traits.static import StaticStore
+from mindflow.core.types.store_traits.json import JsonStore
+
+from mindflow.core.types.model import ConfiguredModel
+from mindflow.core.types.service import ConfiguredServices
+from mindflow.core.types.definitions.mind_flow_model import MindFlowModelID
+from mindflow.core.types.definitions.service import (
     ServiceConfigParameterKey,
     ServiceID,
 )
 
 
-class MindFlowModel(BaseObject):
-    """MindFlow model object."""
-
+class MindFlowModel(StaticStore):
     id: str  # index, query, embedding
     name: str
     defaults: Dict[str, str]
     model: str
 
-    _collection: Collection = Collection.MIND_FLOW_MODEL
-    _database = STATIC_DATABASE
-
-
-class MindFlowModelConfig(BaseObject):
-    """MindFlow model config object."""
 
+class MindFlowModelConfig(JsonStore):
     id: str
     model: str
 
-    _collection: Collection = Collection.CONFIGURATIONS
-    _database = JSON_DATABASE
-
 
 class ConfiguredMindFlowModel:
-    """MindFlow model object."""
-
     id: str  # index, query, embedding
     name: str
     defaults: Dict[str, str]
     model: ConfiguredModel
 
     def __init__(self, mindflow_model_id: str, configured_services: ConfiguredServices):
         self.id = mindflow_model_id
 
-        mind_flow_model = MindFlowModel.load(mindflow_model_id)
-        mind_flow_model_config = MindFlowModelConfig.load(f"{mindflow_model_id}_config")
-
-        if mind_flow_model:
+        if mind_flow_model := MindFlowModel.load(mindflow_model_id):
             for key, value in mind_flow_model.__dict__.items():
                 setattr(self, key, value)
 
-        model_id: Optional[str] = None
-        if mind_flow_model_config:
-            if hasattr(mind_flow_model_config, "model"):
-                model_id = mind_flow_model_config.model
-
-        if model_id is None:
+        if (
+            model_id := getattr(
+                MindFlowModelConfig.load(f"{mindflow_model_id}_config"), "model", None
+            )
+        ) is None:
             model_id = self.get_default_model_id(mindflow_model_id, configured_services)
 
         self.model = ConfiguredModel(model_id)
 
     def get_default_model_id(
         self, mindflow_model_id: str, configured_services: ConfiguredServices
     ) -> str:
-        model_id: Optional[str] = None
-        if hasattr(configured_services.openai, ServiceConfigParameterKey.API_KEY.value):
-            service = configured_services.openai
-            model_id = self.defaults.get(ServiceID.OPENAI.value, None)
-        elif hasattr(
-            configured_services.anthropic, ServiceConfigParameterKey.API_KEY.value
-        ):
-            service = configured_services.anthropic
-            model_id = self.defaults.get(ServiceID.ANTHROPIC.value, None)
-        else:
-            print(
-                "No service API key configured. Please configure an API key for at least one service."
-            )
-            sys.exit(1)
-
-        if model_id is None:
-            raise Exception(
-                "No default model configured for mindflow model: "
-                + mindflow_model_id
-                + " and service: "
-                + service.id
-            )
-
-        return model_id
+        services = {
+            ServiceID.OPENAI.value: configured_services.openai,
+            ServiceID.ANTHROPIC.value: configured_services.anthropic,
+        }
+
+        for service_id, service in services.items():
+            if hasattr(service, ServiceConfigParameterKey.API_KEY.value):
+                model_id = self.defaults.get(service_id)
+                if model_id is not None:
+                    return model_id
+                else:
+                    raise Exception(
+                        "No default model configured for mindflow model: "
+                        + mindflow_model_id
+                        + " and service: "
+                        + service.id
+                    )
+
+        print(
+            "No service API key configured. Please configure an API key for at least one service."
+        )
+        sys.exit(1)
 
 
 class ConfiguredMindFlowModels:
     def __init__(self, configured_services: ConfiguredServices):
         self._configured_services = configured_services
         self._mind_flow_models: Dict[str, ConfiguredMindFlowModel] = {}
```

### Comparing `mindflow-0.4.0/mindflow/db/objects/service.py` & `mindflow-0.5.0/mindflow/core/types/service.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,42 @@
-from mindflow.db.db.json import JSON_DATABASE
-from mindflow.db.db.static import STATIC_DATABASE
-from mindflow.db.db.database import Collection
-from mindflow.db.objects.base import BaseObject
-from mindflow.db.objects.static_definition.service import ServiceID
+from mindflow.core.types.store_traits.json import JsonStore
+from mindflow.core.types.store_traits.static import StaticStore
+from mindflow.core.types.definitions.service import ServiceID
 
 
-class Service(BaseObject):
+class Service(StaticStore):
     id: str
     name: str
     url: str
     api_url: str
 
-    _collection: Collection = Collection.SERVICE
-    _database = STATIC_DATABASE
-
-
-class ServiceConfig(BaseObject):
-    """Service config object."""
 
+class ServiceConfig(JsonStore):
     id: str
     api_key: str
     api_secret: str
     environment: str
 
-    _collection: Collection = Collection.CONFIGURATIONS
-    _database = JSON_DATABASE
-
 
 class ConfiguredService:
     id: str
     name: str
     url: str
     api_url: str
 
     api_key: str
     api_secret: str
     environment: str
 
     def __init__(self, service_id: str):
-        service = Service.load(service_id)
-        service_config = ServiceConfig.load(f"{service_id}_config")
-
-        if service:
+        if service := Service.load(service_id):
             for key, value in service.__dict__.items():
                 setattr(self, key, value)
 
-        if service_config:
+        if service_config := ServiceConfig.load(f"{service_id}_config"):
             for key, value in service_config.__dict__.items():
                 if value not in [None, ""]:
                     setattr(self, key, value)
 
 
 class ConfiguredServices:
     def __init__(self):
```

### Comparing `mindflow-0.4.0/mindflow/db/objects/static_definition/mind_flow_model.py` & `mindflow-0.5.0/mindflow/core/types/definitions/mind_flow_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,51 @@
-from mindflow.db.objects.static_definition.model import ModelID
-from mindflow.db.objects.static_definition.model_type import ModelType
-from mindflow.utils.enum import ExtendedEnum
+from enum import Enum
 
+from mindflow.core.types.definitions.model import ModelID
+from mindflow.core.types.definitions.model_type import ModelType
 
-class MindFlowModelParameterKey(ExtendedEnum):
+
+class MindFlowModelParameterKey(Enum):
     ID = "id"
     NAME = "name"
     DEFAULTS = "defaults"
     DESCRIPTION = "description"
 
 
-class MindFlowModelID(ExtendedEnum):
+class MindFlowModelID(Enum):
     QUERY = "query"
     INDEX = "index"
     EMBEDDING = "embedding"
 
 
-class MindFlowModelDefaults(ExtendedEnum):
+class MindFlowModelDefaults(Enum):
     QUERY: dict = {
         "openai": ModelID.GPT_3_5_TURBO.value,
     }
     INDEX: dict = {
         "openai": ModelID.GPT_3_5_TURBO.value,
     }
     EMBEDDING: dict = {
         "openai": ModelID.TEXT_EMBEDDING_ADA_002.value,
     }
 
 
-class MindFlowModelName(ExtendedEnum):
+class MindFlowModelName(Enum):
     QUERY = "Query"
     INDEX = "Index"
     EMBEDDING = "Embedding"
 
 
-class MindFlowModelType(ExtendedEnum):
+class MindFlowModelType(Enum):
     QUERY = ModelType.TEXT_COMPLETION.value
     INDEX = ModelType.TEXT_COMPLETION.value
     EMBEDDING = ModelType.TEXT_EMBEDDING.value
 
 
-class MindFlowModelDescription(ExtendedEnum):
+class MindFlowModelDescription(Enum):
     QUERY = f"{MindFlowModelName.QUERY}:    Used to respond to chat, queries, and git functionality."
     INDEX = f"{MindFlowModelName.INDEX}:    Used to generate index summaries used for search."
     EMBEDDING = f"{MindFlowModelName.EMBEDDING}:    Used to generate embeddings for text used in search."
 
 
 MINDFLOW_MODEL_STATIC = {
     MindFlowModelID.QUERY.value: {
```

### Comparing `mindflow-0.4.0/mindflow/db/objects/static_definition/model.py` & `mindflow-0.5.0/mindflow/core/types/definitions/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-from mindflow.db.objects.static_definition.model_type import ModelType
-from mindflow.utils.enum import ExtendedEnum
+from enum import Enum
 
+from mindflow.core.types.definitions.model_type import ModelType
 
-class ModelID(ExtendedEnum):
+
+class ModelID(Enum):
     GPT_3_5_TURBO = "gpt-3.5-turbo"
     GPT_3_5_TURBO_0301 = "gpt-3.5-turbo-0301"
 
     GPT_4 = "gpt-4"
     GPT_4_0314 = "gpt-4-0314"
     GPT_4_32K = "gpt-4-32k"
     GPT_4_32K_0314 = "gpt-4-32k-0314"
@@ -14,28 +15,28 @@
     CLAUDE_V1 = "claude-v1"
     CLAUDE_V1_2 = "claude-v1.2"
     CLAUDE_INSTANT_V1 = "claude-instant-v1"
 
     TEXT_EMBEDDING_ADA_002 = "text-embedding-ada-002"
 
 
-class ModelParameterKey(ExtendedEnum):
+class ModelParameterKey(Enum):
     ID = "id"
     NAME = "name"
     SERVICE = "service"
     MODEL_TYPE = "model_type"
     SOFT_TOKEN_LIMIT = "soft_token_limit"
     HARD_TOKEN_LIMIT = "hard_token_limit"
     TOKEN_COST = "token_cost"
     TOKEN_COST_UNIT = "token_cost_unit"
     DESCRIPTION = "description"
     CONFIG_DESCRIPTION = "config_description"
 
 
-class ModelService(ExtendedEnum):
+class ModelService(Enum):
     GPT_3_5_TURBO = "openai"
     GPT_3_5_TURBO_0301 = "openai"
 
     GPT_4 = "openai"
     GPT_4_0314 = "openai"
     GPT_4_32K = "openai"
     GPT_4_32K_0314 = "openai"
@@ -43,23 +44,23 @@
     TEXT_EMBEDDING_ADA_002 = "openai"
 
     CLAUDE_V1 = "anthropic"
     CLAUDE_V1_2 = "anthropic"
     CLAUDE_INSTANT_V1 = "anthropic"
 
 
-class ModelConfigParameterKey(ExtendedEnum):
+class ModelConfigParameterKey(Enum):
     SOFT_TOKEN_LIMIT = "soft_token_limit"
 
 
-class ModelConfigParameterName(ExtendedEnum):
+class ModelConfigParameterName(Enum):
     SOFT_TOKEN_LIMIT = "Soft Token Limit"
 
 
-class ModelName(ExtendedEnum):
+class ModelName(Enum):
     GPT_3_5_TURBO = "GPT 3.5 Turbo"
     GPT_3_5_TURBO_0301 = "GPT 3.5 Turbo March 1st"
 
     GPT_4 = "GPT 4"
     GPT_4_0314 = "GPT 4 March 14th"
     GPT_4_32K = "GPT 4 32K"
     GPT_4_32K_0314 = "GPT 4 32K March 14th"
@@ -67,15 +68,15 @@
     TEXT_EMBEDDING_ADA_002 = "Text Embedding Ada 002"
 
     CLAUDE_V1 = "Claude V1"
     CLAUDE_V1_2 = "Claude V1.2"
     CLAUDE_INSTANT_V1 = "Claude Instant V1"
 
 
-class ModelSoftTokenLimit(ExtendedEnum):
+class ModelSoftTokenLimit(Enum):
     GPT_3_5_TURBO = 500
     GPT_3_5_TURBO_0301 = 500
 
     GPT_4 = 500
     GPT_4_0314 = 500
     GPT_4_32K = 500
     GPT_4_32K_0314 = 500
@@ -83,107 +84,107 @@
     TEXT_EMBEDDING_ADA_002 = 8191
 
     CLAUDE_V1 = 500
     CLAUDE_V1_2 = 500
     CLAUDE_INSTANT_V1 = 500
 
 
-class ModelHardTokenLimit(ExtendedEnum):
+class ModelHardTokenLimit(Enum):
     GPT_3_5_TURBO = 4000
     GPT_3_5_TURBO_0301 = 4000
 
     GPT_4 = 8192
     GPT_4_0314 = 8192
     GPT_4_32K = 32_768
     GPT_4_32K_0314 = 32_768
 
     TEXT_EMBEDDING_ADA_002 = 8191
 
     CLAUDE_V1 = 9000
     CLAUDE_INSTANT_V1 = 9000
 
 
-class ModelTokenCost(ExtendedEnum):
+class ModelTokenCost(Enum):
     GPT_3_5_TURBO = 0.002
     GPT_3_5_TURBO_0301 = 0.002
 
     GPT_4 = 0.002
     GPT_4_0314 = 0.002
     GPT_4_32K = 0.002
     GPT_4_32K_0314 = 0.002
 
     CLAUDE_V1 = 2.90
     CLAUDE_INSTANT_V1 = 0.43
 
     TEXT_EMBEDDING_ADA_002 = 0.0004
 
 
-class ModelTokenCostUnit(ExtendedEnum):
+class ModelTokenCostUnit(Enum):
     THOUSAND = 1000
     MILLION = 1_000_000
 
 
-class ModelDescription(ExtendedEnum):
+class ModelDescription(Enum):
     GPT_3_5_TURBO = f"GPT 3.5 Turbo: {str(ModelHardTokenLimit.GPT_3_5_TURBO.value)} token Limit. ${str(ModelTokenCost.GPT_3_5_TURBO.value)} per {str(ModelTokenCostUnit.THOUSAND.value)} tokens.     OpenAI's most powerful model. Longer outputs, more coherent, and more creative."
     GPT_3_5_TURBO_0301 = f"GPT 3.5 Turbo March 1st: {str(ModelHardTokenLimit.GPT_3_5_TURBO_0301.value)} token Limit. ${str(ModelTokenCost.GPT_3_5_TURBO_0301.value)} per {str(ModelTokenCostUnit.THOUSAND.value)} tokens.     OpenAI's most powerful model. Longer outputs, more coherent, and more creative."
 
     GPT_4 = f"GPT 4: {str(ModelHardTokenLimit.GPT_4.value)} token Limit. ${str(ModelTokenCost.GPT_4.value)} per {str(ModelTokenCostUnit.THOUSAND.value)} tokens.     OpenAI's most powerful model. Longer outputs, more coherent, and more creative."
     GPT_4_0314 = f"GPT 4 March 14th: {str(ModelHardTokenLimit.GPT_4_0314.value)} token Limit. ${str(ModelTokenCost.GPT_4_0314.value)} per {str(ModelTokenCostUnit.THOUSAND.value)} tokens.     OpenAI's most powerful model. Longer outputs, more coherent, and more creative."
     GPT_4_32K = f"GPT 4 32K: {str(ModelHardTokenLimit.GPT_4_32K.value)} token Limit. ${str(ModelTokenCost.GPT_4_32K.value)} per {str(ModelTokenCostUnit.THOUSAND.value)} tokens.     OpenAI's most powerful model. Longer outputs, more coherent, and more creative."
     GPT_4_32K_0314 = f"GPT 4 32K March 14th: {str(ModelHardTokenLimit.GPT_4_32K_0314.value)} token Limit. ${str(ModelTokenCost.GPT_4_32K_0314.value)} per {str(ModelTokenCostUnit.THOUSAND.value)} tokens.     OpenAI's most powerful model. Longer outputs, more coherent, and more creative."
 
     CLAUDE_V1 = f"Claude V1: {str(ModelHardTokenLimit.CLAUDE_V1.value)} token Limit. ${str(ModelTokenCost.CLAUDE_V1.value)} per {str(ModelTokenCostUnit.MILLION.value)} tokens. Anthropic's largest and most powerful model"
     CLAUDE_INSTANT_V1 = f"Claude Instant V1: {str(ModelHardTokenLimit.CLAUDE_INSTANT_V1.value)} token Limit. ${str(ModelTokenCost.CLAUDE_INSTANT_V1.value)} per {str(ModelTokenCostUnit.MILLION.value)} tokens. Anthropic's smaller, faster, and cheaper model."
 
     TEXT_EMBEDDING_ADA_002 = f"Text Embedding Ada 002: {str(ModelHardTokenLimit.TEXT_EMBEDDING_ADA_002)} token Limit. ${str(ModelTokenCost.TEXT_EMBEDDING_ADA_002)} per {str(ModelTokenCostUnit.THOUSAND)} tokens.   OpenAI's best advertised embedding model. Fast and cheap! Recommended for generating deep and shallow indexes"
 
 
-class ModelConfigDescription(ExtendedEnum):
+class ModelConfigDescription(Enum):
     GPT_3_5_TURBO = f"{ModelName.GPT_3_5_TURBO.value}:       OpenAI's Fast, cheap, and still powerful model.       Token Limit: {str(ModelHardTokenLimit.GPT_3_5_TURBO.value)}."
     GPT_4 = f"{ModelName.GPT_4.value}:               OpenAI's most powerful model (slower + expensive).    Token Limit: {str(ModelHardTokenLimit.GPT_4.value)}. Get access -> https://openai.com/waitlist/gpt-4-api."
     TEXT_EMBEDDING_ADA_002 = f"{ModelName.TEXT_EMBEDDING_ADA_002.value}:   OpenAI's best and cheapest embedding model.    Token Limit: {str(ModelHardTokenLimit.TEXT_EMBEDDING_ADA_002.value)}"
 
     CLAUDE_INSTANT_V1 = f"{ModelName.CLAUDE_INSTANT_V1.value}:   Anthropic's Fast, cheap, and still powerful model.    Token Limit: {str(ModelHardTokenLimit.CLAUDE_INSTANT_V1.value)}. Get access -> https://www.anthropic.com/earlyaccess"
     CLAUDE_V1 = f"{ModelName.CLAUDE_V1.value}:           Anthropic's most powerful model (slower + expensive). Token Limit: {str(ModelHardTokenLimit.CLAUDE_V1.value)}. Get access -> https://www.anthropic.com/earlyaccess"
 
 
 ## Service Models (By Type)
-class ModelTextCompletionOpenAI(ExtendedEnum):
+class ModelTextCompletionOpenAI(Enum):
     GPT_3_5_TURBO = ModelID.GPT_3_5_TURBO.value
     GPT_3_5_TURBO_0301 = ModelID.GPT_3_5_TURBO_0301.value
 
     GPT_4 = ModelID.GPT_4.value
     GPT_4_0314 = ModelID.GPT_4_0314.value
     GPT_4_32K = ModelID.GPT_4_32K.value
     GPT_4_32K_0314 = ModelID.GPT_4_32K_0314.value
 
 
-class ModelTextCompletionAnthropic(ExtendedEnum):
+class ModelTextCompletionAnthropic(Enum):
     CLAUDE_V1 = ModelID.CLAUDE_V1.value
     CLAUDE_INSTANT_V1 = ModelID.CLAUDE_INSTANT_V1.value
 
 
-class ModelTextEmbeddingOpenAI(ExtendedEnum):
+class ModelTextEmbeddingOpenAI(Enum):
     TEXT_EMBEDDING_ADA_002 = ModelID.TEXT_EMBEDDING_ADA_002.value
 
 
 ## Service Models (ALL)
-class ModelOpenAI(ExtendedEnum):
+class ModelOpenAI(Enum):
     GPT_3_5_TURBO = ModelID.GPT_3_5_TURBO.value
     GPT_3_5_TURBO_0301 = ModelID.GPT_3_5_TURBO_0301.value
 
     GPT_4 = ModelID.GPT_4.value
     GPT_4_0314 = ModelID.GPT_4_0314.value
     GPT_4_32K = ModelID.GPT_4_32K.value
     GPT_4_32K_0314 = ModelID.GPT_4_32K_0314.value
 
     TEXT_EMBEDDING_ADA_002 = ModelID.TEXT_EMBEDDING_ADA_002.value
 
 
-class ModelAnthropic(ExtendedEnum):
+class ModelAnthropic(Enum):
     CLAUDE_V1 = ModelID.CLAUDE_V1.value
     CLAUDE_INSTANT_V1 = ModelID.CLAUDE_INSTANT_V1.value
 
 
 MODEL_STATIC: dict = {
     ModelID.GPT_3_5_TURBO.value: {
         ModelParameterKey.ID.value: ModelID.GPT_3_5_TURBO.value,
```

### Comparing `mindflow-0.4.0/mindflow/db/objects/static_definition/object.py` & `mindflow-0.5.0/mindflow/core/types/definitions/object.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,34 @@
-from mindflow.db.objects.document import Document
-from mindflow.db.objects.mindflow_model import MindFlowModel
-from mindflow.db.objects.mindflow_model import MindFlowModelConfig
-from mindflow.db.objects.model import Model
-from mindflow.db.objects.model import ModelConfig
-from mindflow.db.objects.service import Service
-from mindflow.db.objects.service import ServiceConfig
-from mindflow.utils.enum import ExtendedEnum
+from enum import Enum
 
+from mindflow.core.types.document import Document
+from mindflow.core.types.mindflow_model import MindFlowModel, MindFlowModelConfig
+from mindflow.core.types.model import Model, ModelConfig
+from mindflow.core.types.service import Service, ServiceConfig
 
-class ObjectID(ExtendedEnum):
+
+class ObjectID(Enum):
     SERVICE = "service"
     SERVICE_CONFIG = "service_config"
     MODEL = "model"
     MODEL_CONFIG = "model_config"
     MINDFLOW_MODEL_CONFIG = "mindflow_model_config"
     DOCUMENT = "document"
 
 
-class ObjectName(ExtendedEnum):
+class ObjectName(Enum):
     SERVICE = "Service"
     SERVICE_CONFIG = "Service Configurations"
     MODEL = "Model"
     MODEL_CONFIG = "Model Configurations"
     MINDFLOW_MODEL_CONFIG = "Mindflow Model Configurations"
     DOCUMENT = "Document"
 
 
-class ObjectType(ExtendedEnum):
+class ObjectType(Enum):
     SERVICE = Service
     SERVICE_CONFIG = ServiceConfig
     MODEL = Model
     MODEL_CONFIG = ModelConfig
     MINDFLOW_MODEL = MindFlowModel
     MINDFLOW_MODEL_CONFIG = MindFlowModelConfig
     DOCUMENT = Document
```

### Comparing `mindflow-0.4.0/mindflow/db/objects/static_definition/service.py` & `mindflow-0.5.0/mindflow/core/types/definitions/service.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,93 +1,98 @@
-from mindflow.db.objects.static_definition.model import ModelID
-from mindflow.db.objects.static_definition.model import ModelOpenAI, ModelAnthropic
-from mindflow.db.objects.static_definition.model import ModelTextCompletionOpenAI
-from mindflow.db.objects.static_definition.model import ModelTextEmbeddingOpenAI
-from mindflow.utils.enum import ExtendedEnum
+from enum import Enum
 
+from mindflow.core.types.definitions.model import ModelID
+from mindflow.core.types.definitions.model import (
+    ModelOpenAI,
+    ModelAnthropic,
+    ModelTextCompletionOpenAI,
+    ModelTextEmbeddingOpenAI,
+    ModelTextCompletionAnthropic,
+)
 
-class ServiceID(ExtendedEnum):
+
+class ServiceID(Enum):
     OPENAI = "openai"
     ANTHROPIC = "anthropic"
     PINECONE = "pinecone"
 
 
-class ServiceConfigID(ExtendedEnum):
+class ServiceConfigID(Enum):
     OPENAI = "openai_config"
     ANTHROPIC = "anthropic_config"
     PINECONE = "pinecone_config"
 
 
-class ServiceParameterKey(ExtendedEnum):
+class ServiceParameterKey(Enum):
     ID = "id"
     NAME = "name"
     URL = "url"
     API_URL = "api_url"
     DEFAULT_INDEX_MODEL = "default_index_model"
     DEFAULT_QUERY_MODEL = "default_query_model"
     DEFAULT_EMBEDDING_MODEL = "default_embedding_model"
 
 
-class ServiceConfigParameterKey(ExtendedEnum):
+class ServiceConfigParameterKey(Enum):
     API_KEY = "api_key"
     API_SECRET = "api_secret"
 
     MODELS = "models"
 
 
-class ServiceConfigParameterName(ExtendedEnum):
+class ServiceConfigParameterName(Enum):
     API_KEY = "API Key"
     API_SECRET = "API Secret"
 
     MODELS = "Models"
 
 
-class ServiceName(ExtendedEnum):
+class ServiceName(Enum):
     OPENAI = "OpenAI"
     ANTHROPIC = "Anthropic"
     PINECONE = "Pinecone"
 
 
-class ServiceURL(ExtendedEnum):
+class ServiceURL(Enum):
     OPENAI = ""
     ANTHROPIC = ""
     PINECONE = ""
 
 
-class ServiceAPIURL(ExtendedEnum):
+class ServiceAPIURL(Enum):
     OPENAI = ""
     ANTHROPIC = ""
     PINECONE = ""
 
 
-class ServiceDefaultIndexModel(ExtendedEnum):
+class ServiceDefaultIndexModel(Enum):
     OPENAI = ModelID.GPT_3_5_TURBO.value
     ANTHROPIC = ModelID.CLAUDE_INSTANT_V1.value
 
 
-class ServiceDefaultQueryModel(ExtendedEnum):
+class ServiceDefaultQueryModel(Enum):
     OPENAI = ModelID.GPT_3_5_TURBO.value
     ANTHROPIC = ModelID.CLAUDE_V1.value
 
 
-class ServiceDefaultEmbeddingModel(ExtendedEnum):
+class ServiceDefaultEmbeddingModel(Enum):
     OPENAI = ModelID.TEXT_EMBEDDING_ADA_002.value
 
 
 ## Service Model Types
-class ServiceModelTypeTextEmbedding(ExtendedEnum):
+class ServiceModelTypeTextEmbedding(Enum):
     OPENAI = ModelTextEmbeddingOpenAI
 
 
-class ServiceModelTypeTextCompletion(ExtendedEnum):
+class ServiceModelTypeTextCompletion(Enum):
     OPENAI = ModelTextCompletionOpenAI
-    ANTHROPIC = ModelTextCompletionOpenAI
+    ANTHROPIC = ModelTextCompletionAnthropic
 
 
-class ServiceModel(ExtendedEnum):
+class ServiceModel(Enum):
     OPENAI = ModelOpenAI
     ANTHROPIC = ModelAnthropic
 
 
 SERVICE_STATIC = {
     ServiceID.OPENAI.value: {
         ServiceParameterKey.ID.value: ServiceID.OPENAI.value,
```

### Comparing `mindflow-0.4.0/mindflow/unit_tests/dummy_diff.txt` & `mindflow-0.5.0/mindflow/unit_tests/dummy_diff.txt`

 * *Files identical despite different names*

### Comparing `mindflow-0.4.0/mindflow/unit_tests/test_utils.py` & `mindflow-0.5.0/mindflow/unit_tests/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from mindflow.utils.diff_parser import parse_git_diff
+from mindflow.core.commands.git.diff import parse_git_diff
 
 
 def test_diff_parser():
     diff = open("mindflow/unit_tests/dummy_diff.txt", "r").read()
     diffs, excluded_files = parse_git_diff(diff)
 
     assert excluded_files == ["b/mindflow/test.ipynb"]
```

### Comparing `mindflow-0.4.0/mindflow/utils/errors.py` & `mindflow-0.5.0/mindflow/core/errors.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 GITHUB_ISSUE_MESSAGE = "If the problem persists, please raise an issue at: https://github.com/nollied/mindflow-cli/issues"
 CONNECTION_MESSAGE = "Please check your internet connection and try again."
 
 
 class ModelError(Exception):
-    """Base class for all exceptions raised by this module."""
-
     def __init__(self, message):
         self.message = message
         super().__init__(self.message)
 
     @property
     def base_message(self):
         return f"Model API failed to return response for chat/query. {CONNECTION_MESSAGE}. {GITHUB_ISSUE_MESSAGE}."
@@ -39,12 +37,10 @@
 
     @property
     def embedding_message(self):
         return f"Warning: Model API failed to return response for embedding. {CONNECTION_MESSAGE}. {GITHUB_ISSUE_MESSAGE}"
 
 
 class EmbeddingModelError(Exception):
-    """Base class for all exceptions raised by this module."""
-
     def __init__(self, message):
         self.message = message
         super().__init__(self.message)
```

### Comparing `mindflow-0.4.0/mindflow/utils/files/extract.py` & `mindflow-0.5.0/mindflow/core/file_processing/extract.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,28 @@
-"""
-Module for recursively extracting all files from a file path.
-"""
 import logging
 import os
 from typing import List
-from typing import Union
 
-from mindflow.utils.files.git import get_git_files
-from mindflow.utils.files.git import is_within_git_repo
+from mindflow.core.file_processing.git import (
+    is_path_within_git_repo,
+    get_all_unignored_git_files_from_path,
+)
 
 
-def extract_files(path) -> List[str]:
-    """
-    Extract all files from a directory.
-    """
+def extract_files_from_directory(path) -> List[str]:
     file_paths = []
     if os.path.isfile(path):
         return [os.fspath(path)]
-    if is_within_git_repo(path):
-        return get_git_files(path)
+    if is_path_within_git_repo(path):
+        return get_all_unignored_git_files_from_path(path)
     try:
         with os.scandir(path) as paths:
             for scanned_path in paths:
                 if scanned_path.is_file():
                     file_paths.append(os.path.abspath(scanned_path.path))
                 elif os.path.isdir(path):
-                    file_paths.extend(extract_files(scanned_path.path))
+                    file_paths.extend(extract_files_from_directory(scanned_path.path))
         return file_paths
     except IsADirectoryError as error:
         logging.debug("Could not read directory/file: %s", path)
         logging.debug(error)
         return file_paths
```

### Comparing `mindflow-0.4.0/mindflow/utils/files/git.py` & `mindflow-0.5.0/mindflow/core/file_processing/git.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,49 +1,29 @@
-"""
-Handles git related operations.
-"""
+"""Handles git related operations."""
 import logging
 import os
 import subprocess
 from typing import List
 from typing import Union
 
 
-class NotInGit(BaseException):
-    """
-    Raised when the given path is not within a git repository.
-    """
-
-
-class GitError(BaseException):
-    """
-    Raised when a git command fails.
-    """
-
-
-def is_within_git_repo(path: Union[str, os.PathLike]) -> bool:
-    """
-    Checks if the given path is within a git repository.
-    """
+def is_path_within_git_repo(path: Union[str, os.PathLike]) -> bool:
     try:
         output = subprocess.run(
-            ["git", "-C", path, "rev-parse", "--git-dir"],
+            ["git", "-C", str(path), "rev-parse", "--git-dir"],
             capture_output=True,
             timeout=10,
             check=True,
         )
         return output.returncode == 0
-    except NotInGit:
+    except subprocess.CalledProcessError:
         return False
 
 
-def get_git_files(path: Union[str, os.PathLike]) -> List[str]:
-    """
-    Extract all files from a git repository that are not gitignored.
-    """
+def get_all_unignored_git_files_from_path(path: Union[str, os.PathLike]) -> List[str]:
     try:
         output = subprocess.run(
             ["git", "-C", os.fspath(path), "ls-files"],
             capture_output=True,
             timeout=10,
             check=True,
         )
```

### Comparing `mindflow-0.4.0/mindflow/utils/prompt_builders.py` & `mindflow-0.5.0/mindflow/core/prompt_builders.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,74 +1,65 @@
 from enum import Enum
 from typing import Dict, Union
 from typing import List
-from mindflow.db.objects.model import ConfiguredModel
+from mindflow.core.types.model import ConfiguredModel
 
-from mindflow.db.objects.static_definition.service import ServiceID
 import anthropic
-from mindflow.utils.constants import MinimumReservedLength
 
-from mindflow.utils.token import get_token_count
+from mindflow.core.types.definitions.service import ServiceID
+from mindflow.core.constants import MinimumReservedLength
+from mindflow.core.token_counting import get_token_count_of_text_for_model
 
 
 class Role(Enum):
     SYSTEM = "system"
     USER = "user"
     ASSISTANT = "assistant"
 
 
-def create_message(role: str, prompt: str) -> Dict[str, str]:
+def create_conversation_message(role: str, prompt: str) -> Dict[str, str]:
     return {"role": role, "content": prompt}
 
 
-# messages = [
-#     {
-#         "role": "*role*",
-#         "content": "*content*",
-#     }
-# ]
-def build_prompt(
+def build_prompt_from_conversation_messages(
     messages: List[Dict[str, str]], model: ConfiguredModel
 ) -> Union[List[Dict], str]:
     if model.service == ServiceID.OPENAI.value:
         return messages
-    else:
-        full_prompt: str = ""
-        for message in messages:
-            role = message["role"]
-            prompt = message["content"]
-
-            if role == Role.SYSTEM.value:
-                full_prompt += anthropic.HUMAN_PROMPT
-                full_prompt += prompt
-                full_prompt += (
-                    anthropic.AI_PROMPT
-                    + " Sure! I will respond to all following messages with a response like you have just outlined for me."
-                )
-            elif role == Role.USER.value:
-                full_prompt += anthropic.HUMAN_PROMPT
-                full_prompt += prompt
-            elif role == Role.ASSISTANT.value:
-                full_prompt += anthropic.AI_PROMPT
-                full_prompt += prompt
 
-        full_prompt += anthropic.AI_PROMPT
+    prompt_parts = []
+    for message in messages:
+        role = message["role"]
+        prompt = message["content"]
+
+        if role == Role.SYSTEM.value:
+            prompt_parts.append(anthropic.HUMAN_PROMPT + prompt)
+            prompt_parts.append(
+                anthropic.AI_PROMPT
+                + " Sure! I will respond to all following messages with a response like you have just outlined for me."
+            )
+        elif role in [Role.USER.value, Role.ASSISTANT.value]:
+            prompt_parts.append(
+                (
+                    anthropic.HUMAN_PROMPT
+                    if role == Role.USER.value
+                    else anthropic.AI_PROMPT
+                )
+                + prompt
+            )
 
-        return full_prompt
+    return "".join(prompt_parts) + anthropic.AI_PROMPT
 
 
-def prune_messages(
+def prune_messages_to_fit_context_window(
     messages: List[Dict[str, str]], model: ConfiguredModel
 ) -> List[Dict[str, str]]:
-    """
-    Prunes the messages to a maximum length.
-    """
     # Improvement can be made on the estimation here for Anthropic system messages
     content = ""
     for i in range(0, len(messages)):
         content += f"{messages[i]['role']}\n\n {messages[i]['content']}"
         if (
-            get_token_count(model, content)
+            get_token_count_of_text_for_model(model, content)
             > model.hard_token_limit - MinimumReservedLength.CHAT.value
         ):
             return messages[:i]
     return messages
```

### Comparing `mindflow-0.4.0/mindflow/utils/prompts.py` & `mindflow-0.5.0/mindflow/core/prompts.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-This file contains the prompts that are used in the CLI.
-"""
+"""This file contains the prompts that are used in the CLI."""
 
 GIT_DIFF_PROMPT_PREFIX = "The following is a git diff from my code repository. \
     Please thoroughly explain to me in bullet points the changes for each file. \
         In your response back to me, only provide the file name with its bulleted summary indented once and nothing else in the format:\n \
             \
             - *file_name*:\n \
                 - change1\n \
@@ -19,7 +17,8 @@
 CHAT_PROMPT_PREFIX = "You are a helpful virtual assistant responding to a users query using your general knowledge and the text provided below."
 COMMIT_PROMPT_PREFIX = "Please provide a commit message for the following changes. Only respond with a single commit message and nothing else. Put the response within XML tage like <COMMIT></COMMIT>."
 PR_TITLE_PREFIX = "Please provide a title for the following pull request using this git diff summary. Only respond with the title and nothing else."
 PR_BODY_PREFIX = "Please provide a body for the following pull request using this git diff summary. I want you to keep it high level, and give core \
       themes and reasons for changes. Try to include some titles and bullet points. Only respond with the body and nothing else."
 QUERY_PROMPT_PREFIX = "You are a helpful virtual assistant responding to a users query using your general knowledge and the text provided below."
 DEFAULT_CONVERSATION_SYSTEM_PROMPT = "You are a senior software engineer responding to another software engineer's chat messages regarding your codebase, make sure to be polite and helpful, and provide thorough answers with example code when necessary."
+GIT_DIFF_SUMMARIZE_PROMPT = 'What is the higher level purpose of these changes? Keep it short and sweet, don\'t provide any useless or redundant information like "made changes to the code". Do NOT speak in generalities, be specific.'
```

### Comparing `mindflow-0.4.0/mindflow/utils/token.py` & `mindflow-0.5.0/mindflow/core/token_counting.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,59 +1,54 @@
 import os
 from typing import Dict, List
-from mindflow.db.objects.model import ConfiguredModel
+from mindflow.core.types.model import ConfiguredModel
 
 
-def get_token_count(model: ConfiguredModel, text: str) -> int:
-    """
-    This function is used to get the token count of a string.
-    """
+def get_token_count_of_text_for_model(model: ConfiguredModel, text: str) -> int:
     try:
         return len(model.tokenizer.encode(text))
     except Exception:
         return len(text) // 3
 
 
-def get_batch_token_count(model: ConfiguredModel, texts: List[str]) -> int:
-    """
-    This function is used to get the token count of a list of strings.
-    """
+def get_batch_token_count_of_text_for_model(
+    model: ConfiguredModel, texts: List[str]
+) -> int:
     try:
-        return sum([len(encoding) for encoding in model.tokenizer.encode_batch(texts)])
+        return sum(len(encoding) for encoding in model.tokenizer.encode_batch(texts))
     except Exception:
-        return sum([len(text) // 3 for text in texts])
+        return sum(len(text) // 3 for text in texts)
 
 
-def estimate_tokens_from_messages(
+def get_token_count_of_messages_for_model(
     messages: List[Dict[str, str]],
     model: ConfiguredModel,
 ):
-    content = ""
-    for i in range(len(messages)):
-        content += f"{messages[i]['role']}\n\n {messages[i]['content']}"
+    return get_token_count_of_text_for_model(
+        model,
+        "\n\n".join(
+            [f"{message['role']}\n\n{message['content']}" for message in messages]
+        ),
+    )
 
-    return get_token_count(model, content)
 
-
-def estimate_tokens_from_paths(
+def get_token_count_from_document_query_for_model(
     document_paths: List[str],
     query: str,
     model: ConfiguredModel,
     return_texts: bool = False,
 ):
     texts = [query]
     for document_path in document_paths:
-        # check if directory
         if os.path.isdir(document_path):
             raise NotImplementedError("Directory support not yet implemented.")
 
         if not os.path.exists(document_path):
             raise FileNotFoundError(f"Could not find file at {document_path}")
 
         file_text = {open(document_path, "r").read()}
-        text = f"```{file_text}```"
-        texts.append(text)
+        texts.append(f"```{file_text}```")
 
-    tokens = get_batch_token_count(model, texts)
+    tokens = get_batch_token_count_of_text_for_model(model, texts)
     if return_texts:
         return tokens, texts
     return tokens
```

### Comparing `mindflow-0.4.0/mindflow.egg-info/PKG-INFO` & `mindflow-0.5.0/mindflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindflow
-Version: 0.4.0
+Version: 0.5.0
 Summary: AI-powered search engine for your code!
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # :brain: mindflow :ocean:
 The [ChatGPT](https://openai.com/blog/chatgpt)-powered swiss army knife for the modern developer! We provide an AI-powered CLI git wrapper, boilerplate code generator, code search engine, a conversation history manager, and much more!
```

### Comparing `mindflow-0.4.0/setup.py` & `mindflow-0.5.0/setup.py`

 * *Files identical despite different names*

