# Comparing `tmp/kiara_plugin.core_types-0.4.8.tar.gz` & `tmp/kiara_plugin.core_types-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiara_plugin.core_types-0.4.8.tar", last modified: Sun Jul 10 20:57:30 2022, max compression
+gzip compressed data, was "kiara_plugin.core_types-0.4.9.tar", last modified: Mon Jul 11 13:54:26 2022, max compression
```

## Comparing `kiara_plugin.core_types-0.4.8.tar` & `kiara_plugin.core_types-0.4.9.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 20:57:30.848661 kiara_plugin.core_types-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (121)      669 2022-07-10 20:56:41.000000 kiara_plugin.core_types-0.4.8/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (121)      139 2022-07-10 20:56:41.000000 kiara_plugin.core_types-0.4.8/.envrc.disabled
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-07-10 20:56:41.000000 kiara_plugin.core_types-0.4.8/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-07-10 20:56:41.000000 kiara_plugin.core_types-0.4.8/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 20:57:30.840661 kiara_plugin.core_types-0.4.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 20:57:30.840661 kiara_plugin.core_types-0.4.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      834 2022-07-10 20:56:41.000000 kiara_plugin.core_types-0.4.8/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (121)      900 2022-07-10 20:56:41.000000 kiara_plugin.core_types-0.4.8/.github/ISSUE_TEMPLATE/suggest-a-module.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 20:57:30.840661 kiara_plugin.core_types-0.4.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      887 2022-07-10 20:56:41.000000 kiara_plugin.core_types-0.4.8/.github/workflows/build-darwin.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     8179 2022-07-10 20:56:41.000000 kiara_plugin.core_types-0.4.8/.github/workflows/build-linux.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      688 2022-07-10 20:56:41.000000 kiara_plugin.core_types-0.4.8/.github/workflows/build-windows.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      806 2022-07-10 20:56:41.000000 kiara_plugin.core_types-0.4.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1834 2022-07-10 20:56:41.000000 kiara_plugin.core_types-0.4.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-07-10 20:56:41.000000 kiara_plugin.core_types-0.4.8/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-07-10 20:56:41.000000 kiara_plugin.core_types-0.4.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)    16725 2022-07-10 20:56:41.000000 kiara_plugin.core_types-0.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      396 2022-07-10 20:56:41.000000 kiara_plugin.core_types-0.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2242 2022-07-10 20:56:41.000000 kiara_plugin.core_types-0.4.8/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     5473 2022-07-10 20:57:30.848661 kiara_plugin.core_types-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4587 2022-07-10 20:56:41.000000 kiara_plugin.core_types-0.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 20:57:30.840661 kiara_plugin.core_types-0.4.8/ci/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 20:57:30.844661 kiara_plugin.core_types-0.4.8/ci/conda/
--rwxr-xr-x   0 runner    (1001) docker     (121)     7458 2022-07-10 20:56:41.000000 kiara_plugin.core_types-0.4.8/ci/conda/build-conda-packages.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 20:57:30.844661 kiara_plugin.core_types-0.4.8/ci/conda/kiara_plugin.core_types/
--rw-r--r--   0 runner    (1001) docker     (121)      863 2022-07-10 20:56:41.000000 kiara_plugin.core_types-0.4.8/ci/conda/kiara_plugin.core_types/meta.yaml.template
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-07-10 20:56:41.000000 kiara_plugin.core_types-0.4.8/commitlint.config.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 20:57:30.844661 kiara_plugin.core_types-0.4.8/docs/
--rw-r--r--   0 runner    (1001) docker     (121)       97 2022-07-10 20:56:41.000000 kiara_plugin.core_types-0.4.8/docs/SUMMARY.md
--rw-r--r--   0 runner    (1001) docker     (121)      242 2022-07-10 20:56:41.000000 kiara_plugin.core_types-0.4.8/docs/SUMMARY.md.rej
--rw-r--r--   0 runner    (1001) docker     (121)      835 2022-07-10 20:56:41.000000 kiara_plugin.core_types-0.4.8/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 20:57:30.844661 kiara_plugin.core_types-0.4.8/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (121)      144 2022-07-10 20:56:41.000000 kiara_plugin.core_types-0.4.8/docs/stylesheets/extra.css
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-07-10 20:56:41.000000 kiara_plugin.core_types-0.4.8/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 20:57:30.840661 kiara_plugin.core_types-0.4.8/examples/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 20:57:30.844661 kiara_plugin.core_types-0.4.8/examples/data/
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-07-10 20:56:41.000000 kiara_plugin.core_types-0.4.8/examples/data/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 20:57:30.844661 kiara_plugin.core_types-0.4.8/examples/data/journals/
--rw-r--r--   0 runner    (1001) docker     (121)     2667 2022-07-10 20:56:41.000000 kiara_plugin.core_types-0.4.8/examples/data/journals/JournalEdges1902.csv
--rw-r--r--   0 runner    (1001) docker     (121)    33121 2022-07-10 20:56:41.000000 kiara_plugin.core_types-0.4.8/examples/data/journals/JournalNodes1902.csv
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-07-10 20:56:41.000000 kiara_plugin.core_types-0.4.8/examples/data/journals/Readme.md
--rw-r--r--   0 runner    (1001) docker     (121)     1418 2022-07-10 20:56:41.000000 kiara_plugin.core_types-0.4.8/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)      362 2022-07-10 20:56:41.000000 kiara_plugin.core_types-0.4.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 20:57:30.840661 kiara_plugin.core_types-0.4.8/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 20:57:30.844661 kiara_plugin.core_types-0.4.8/scripts/documentation/
--rw-r--r--   0 runner    (1001) docker     (121)      865 2022-07-10 20:56:41.000000 kiara_plugin.core_types-0.4.8/scripts/documentation/gen_api_doc_pages.py
--rw-r--r--   0 runner    (1001) docker     (121)      571 2022-07-10 20:56:41.000000 kiara_plugin.core_types-0.4.8/scripts/documentation/gen_info_pages.py
--rw-r--r--   0 runner    (1001) docker     (121)     1855 2022-07-10 20:56:41.000000 kiara_plugin.core_types-0.4.8/scripts/documentation/gen_module_doc.py
--rw-r--r--   0 runner    (1001) docker     (121)     3712 2022-07-10 20:57:30.848661 kiara_plugin.core_types-0.4.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     1396 2022-07-10 20:56:41.000000 kiara_plugin.core_types-0.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 20:57:30.840661 kiara_plugin.core_types-0.4.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 20:57:30.840661 kiara_plugin.core_types-0.4.8/src/kiara_plugin/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 20:57:30.844661 kiara_plugin.core_types-0.4.8/src/kiara_plugin/core_types/
--rw-r--r--   0 runner    (1001) docker     (121)     2195 2022-07-10 20:56:41.000000 kiara_plugin.core_types-0.4.8/src/kiara_plugin/core_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10237 2022-07-10 20:56:41.000000 kiara_plugin.core_types-0.4.8/src/kiara_plugin/core_types/data_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     4345 2022-07-10 20:56:41.000000 kiara_plugin.core_types-0.4.8/src/kiara_plugin/core_types/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 20:57:30.844661 kiara_plugin.core_types-0.4.8/src/kiara_plugin/core_types/modules/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-10 20:56:41.000000 kiara_plugin.core_types-0.4.8/src/kiara_plugin/core_types/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3348 2022-07-10 20:56:41.000000 kiara_plugin.core_types-0.4.8/src/kiara_plugin/core_types/modules/boolean.py
--rw-r--r--   0 runner    (1001) docker     (121)     3107 2022-07-10 20:56:41.000000 kiara_plugin.core_types-0.4.8/src/kiara_plugin/core_types/modules/date.py
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-07-10 20:56:41.000000 kiara_plugin.core_types-0.4.8/src/kiara_plugin/core_types/modules/list.py
--rw-r--r--   0 runner    (1001) docker     (121)     3041 2022-07-10 20:56:41.000000 kiara_plugin.core_types-0.4.8/src/kiara_plugin/core_types/modules/string.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 20:57:30.844661 kiara_plugin.core_types-0.4.8/src/kiara_plugin/core_types/pipelines/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-10 20:56:41.000000 kiara_plugin.core_types-0.4.8/src/kiara_plugin/core_types/pipelines/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-07-10 20:56:41.000000 kiara_plugin.core_types-0.4.8/src/kiara_plugin/core_types/pipelines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 20:57:30.844661 kiara_plugin.core_types-0.4.8/src/kiara_plugin/core_types/pipelines/logic/
--rw-r--r--   0 runner    (1001) docker     (121)      406 2022-07-10 20:56:41.000000 kiara_plugin.core_types-0.4.8/src/kiara_plugin/core_types/pipelines/logic/nand.json
--rw-r--r--   0 runner    (1001) docker     (121)      400 2022-07-10 20:56:41.000000 kiara_plugin.core_types-0.4.8/src/kiara_plugin/core_types/pipelines/logic/nor.json
--rw-r--r--   0 runner    (1001) docker     (121)      550 2022-07-10 20:56:41.000000 kiara_plugin.core_types-0.4.8/src/kiara_plugin/core_types/pipelines/logic/xor.json
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-10 20:56:41.000000 kiara_plugin.core_types-0.4.8/src/kiara_plugin/core_types/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 20:57:30.844661 kiara_plugin.core_types-0.4.8/src/kiara_plugin/core_types/resources/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-10 20:56:41.000000 kiara_plugin.core_types-0.4.8/src/kiara_plugin/core_types/resources/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 20:57:30.844661 kiara_plugin.core_types-0.4.8/src/kiara_plugin.core_types.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5473 2022-07-10 20:57:30.000000 kiara_plugin.core_types-0.4.8/src/kiara_plugin.core_types.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1958 2022-07-10 20:57:30.000000 kiara_plugin.core_types-0.4.8/src/kiara_plugin.core_types.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-10 20:57:30.000000 kiara_plugin.core_types-0.4.8/src/kiara_plugin.core_types.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      290 2022-07-10 20:57:30.000000 kiara_plugin.core_types-0.4.8/src/kiara_plugin.core_types.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-10 20:57:26.000000 kiara_plugin.core_types-0.4.8/src/kiara_plugin.core_types.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)     1706 2022-07-10 20:57:30.000000 kiara_plugin.core_types-0.4.8/src/kiara_plugin.core_types.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-07-10 20:57:30.000000 kiara_plugin.core_types-0.4.8/src/kiara_plugin.core_types.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 20:57:30.848661 kiara_plugin.core_types-0.4.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      274 2022-07-10 20:56:41.000000 kiara_plugin.core_types-0.4.8/tests/conftest.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      236 2022-07-10 20:56:41.000000 kiara_plugin.core_types-0.4.8/tests/test_kiara_modules_default.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 13:54:26.726060 kiara_plugin.core_types-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      669 2022-07-11 13:53:42.000000 kiara_plugin.core_types-0.4.9/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (121)      139 2022-07-11 13:53:42.000000 kiara_plugin.core_types-0.4.9/.envrc.disabled
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-07-11 13:53:42.000000 kiara_plugin.core_types-0.4.9/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-07-11 13:53:42.000000 kiara_plugin.core_types-0.4.9/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 13:54:26.718061 kiara_plugin.core_types-0.4.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 13:54:26.722061 kiara_plugin.core_types-0.4.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      834 2022-07-11 13:53:42.000000 kiara_plugin.core_types-0.4.9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (121)      900 2022-07-11 13:53:42.000000 kiara_plugin.core_types-0.4.9/.github/ISSUE_TEMPLATE/suggest-a-module.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 13:54:26.722061 kiara_plugin.core_types-0.4.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)      887 2022-07-11 13:53:42.000000 kiara_plugin.core_types-0.4.9/.github/workflows/build-darwin.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     8179 2022-07-11 13:53:42.000000 kiara_plugin.core_types-0.4.9/.github/workflows/build-linux.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      688 2022-07-11 13:53:42.000000 kiara_plugin.core_types-0.4.9/.github/workflows/build-windows.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      806 2022-07-11 13:53:42.000000 kiara_plugin.core_types-0.4.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1834 2022-07-11 13:53:42.000000 kiara_plugin.core_types-0.4.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)       53 2022-07-11 13:53:42.000000 kiara_plugin.core_types-0.4.9/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-07-11 13:53:42.000000 kiara_plugin.core_types-0.4.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)    16725 2022-07-11 13:53:42.000000 kiara_plugin.core_types-0.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      396 2022-07-11 13:53:42.000000 kiara_plugin.core_types-0.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     2242 2022-07-11 13:53:42.000000 kiara_plugin.core_types-0.4.9/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)     5473 2022-07-11 13:54:26.726060 kiara_plugin.core_types-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4587 2022-07-11 13:53:42.000000 kiara_plugin.core_types-0.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 13:54:26.718061 kiara_plugin.core_types-0.4.9/ci/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 13:54:26.722061 kiara_plugin.core_types-0.4.9/ci/conda/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     7458 2022-07-11 13:53:42.000000 kiara_plugin.core_types-0.4.9/ci/conda/build-conda-packages.sh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 13:54:26.722061 kiara_plugin.core_types-0.4.9/ci/conda/kiara_plugin.core_types/
+-rw-r--r--   0 runner    (1001) docker     (121)      863 2022-07-11 13:53:42.000000 kiara_plugin.core_types-0.4.9/ci/conda/kiara_plugin.core_types/meta.yaml.template
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-07-11 13:53:42.000000 kiara_plugin.core_types-0.4.9/commitlint.config.js
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 13:54:26.722061 kiara_plugin.core_types-0.4.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)       97 2022-07-11 13:53:42.000000 kiara_plugin.core_types-0.4.9/docs/SUMMARY.md
+-rw-r--r--   0 runner    (1001) docker     (121)      242 2022-07-11 13:53:42.000000 kiara_plugin.core_types-0.4.9/docs/SUMMARY.md.rej
+-rw-r--r--   0 runner    (1001) docker     (121)      835 2022-07-11 13:53:42.000000 kiara_plugin.core_types-0.4.9/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 13:54:26.722061 kiara_plugin.core_types-0.4.9/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (121)      144 2022-07-11 13:53:42.000000 kiara_plugin.core_types-0.4.9/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-07-11 13:53:42.000000 kiara_plugin.core_types-0.4.9/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 13:54:26.718061 kiara_plugin.core_types-0.4.9/examples/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 13:54:26.722061 kiara_plugin.core_types-0.4.9/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (121)      142 2022-07-11 13:53:42.000000 kiara_plugin.core_types-0.4.9/examples/data/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 13:54:26.722061 kiara_plugin.core_types-0.4.9/examples/data/journals/
+-rw-r--r--   0 runner    (1001) docker     (121)     2667 2022-07-11 13:53:42.000000 kiara_plugin.core_types-0.4.9/examples/data/journals/JournalEdges1902.csv
+-rw-r--r--   0 runner    (1001) docker     (121)    33121 2022-07-11 13:53:42.000000 kiara_plugin.core_types-0.4.9/examples/data/journals/JournalNodes1902.csv
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2022-07-11 13:53:42.000000 kiara_plugin.core_types-0.4.9/examples/data/journals/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1418 2022-07-11 13:53:42.000000 kiara_plugin.core_types-0.4.9/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      362 2022-07-11 13:53:42.000000 kiara_plugin.core_types-0.4.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 13:54:26.718061 kiara_plugin.core_types-0.4.9/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 13:54:26.722061 kiara_plugin.core_types-0.4.9/scripts/documentation/
+-rw-r--r--   0 runner    (1001) docker     (121)      865 2022-07-11 13:53:42.000000 kiara_plugin.core_types-0.4.9/scripts/documentation/gen_api_doc_pages.py
+-rw-r--r--   0 runner    (1001) docker     (121)      571 2022-07-11 13:53:42.000000 kiara_plugin.core_types-0.4.9/scripts/documentation/gen_info_pages.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1855 2022-07-11 13:53:42.000000 kiara_plugin.core_types-0.4.9/scripts/documentation/gen_module_doc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3712 2022-07-11 13:54:26.726060 kiara_plugin.core_types-0.4.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1396 2022-07-11 13:53:42.000000 kiara_plugin.core_types-0.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 13:54:26.718061 kiara_plugin.core_types-0.4.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 13:54:26.718061 kiara_plugin.core_types-0.4.9/src/kiara_plugin/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 13:54:26.722061 kiara_plugin.core_types-0.4.9/src/kiara_plugin/core_types/
+-rw-r--r--   0 runner    (1001) docker     (121)     2195 2022-07-11 13:53:42.000000 kiara_plugin.core_types-0.4.9/src/kiara_plugin/core_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10237 2022-07-11 13:53:42.000000 kiara_plugin.core_types-0.4.9/src/kiara_plugin/core_types/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4411 2022-07-11 13:53:42.000000 kiara_plugin.core_types-0.4.9/src/kiara_plugin/core_types/models.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 13:54:26.722061 kiara_plugin.core_types-0.4.9/src/kiara_plugin/core_types/modules/
+-rw-r--r--   0 runner    (1001) docker     (121)     5839 2022-07-11 13:53:42.000000 kiara_plugin.core_types-0.4.9/src/kiara_plugin/core_types/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3348 2022-07-11 13:53:42.000000 kiara_plugin.core_types-0.4.9/src/kiara_plugin/core_types/modules/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3107 2022-07-11 13:53:42.000000 kiara_plugin.core_types-0.4.9/src/kiara_plugin/core_types/modules/date.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-07-11 13:53:42.000000 kiara_plugin.core_types-0.4.9/src/kiara_plugin/core_types/modules/list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3041 2022-07-11 13:53:42.000000 kiara_plugin.core_types-0.4.9/src/kiara_plugin/core_types/modules/string.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 13:54:26.722061 kiara_plugin.core_types-0.4.9/src/kiara_plugin/core_types/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-11 13:53:42.000000 kiara_plugin.core_types-0.4.9/src/kiara_plugin/core_types/pipelines/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (121)      124 2022-07-11 13:53:42.000000 kiara_plugin.core_types-0.4.9/src/kiara_plugin/core_types/pipelines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 13:54:26.722061 kiara_plugin.core_types-0.4.9/src/kiara_plugin/core_types/pipelines/logic/
+-rw-r--r--   0 runner    (1001) docker     (121)      406 2022-07-11 13:53:42.000000 kiara_plugin.core_types-0.4.9/src/kiara_plugin/core_types/pipelines/logic/nand.json
+-rw-r--r--   0 runner    (1001) docker     (121)      400 2022-07-11 13:53:42.000000 kiara_plugin.core_types-0.4.9/src/kiara_plugin/core_types/pipelines/logic/nor.json
+-rw-r--r--   0 runner    (1001) docker     (121)      550 2022-07-11 13:53:42.000000 kiara_plugin.core_types-0.4.9/src/kiara_plugin/core_types/pipelines/logic/xor.json
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-11 13:53:42.000000 kiara_plugin.core_types-0.4.9/src/kiara_plugin/core_types/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 13:54:26.722061 kiara_plugin.core_types-0.4.9/src/kiara_plugin/core_types/resources/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-11 13:53:42.000000 kiara_plugin.core_types-0.4.9/src/kiara_plugin/core_types/resources/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 13:54:26.722061 kiara_plugin.core_types-0.4.9/src/kiara_plugin.core_types.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5473 2022-07-11 13:54:26.000000 kiara_plugin.core_types-0.4.9/src/kiara_plugin.core_types.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1958 2022-07-11 13:54:26.000000 kiara_plugin.core_types-0.4.9/src/kiara_plugin.core_types.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-11 13:54:26.000000 kiara_plugin.core_types-0.4.9/src/kiara_plugin.core_types.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      290 2022-07-11 13:54:26.000000 kiara_plugin.core_types-0.4.9/src/kiara_plugin.core_types.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-11 13:54:22.000000 kiara_plugin.core_types-0.4.9/src/kiara_plugin.core_types.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)     1706 2022-07-11 13:54:26.000000 kiara_plugin.core_types-0.4.9/src/kiara_plugin.core_types.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2022-07-11 13:54:26.000000 kiara_plugin.core_types-0.4.9/src/kiara_plugin.core_types.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 13:54:26.726060 kiara_plugin.core_types-0.4.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      274 2022-07-11 13:53:42.000000 kiara_plugin.core_types-0.4.9/tests/conftest.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      236 2022-07-11 13:53:42.000000 kiara_plugin.core_types-0.4.9/tests/test_kiara_modules_default.py
```

### Comparing `kiara_plugin.core_types-0.4.8/.cruft.json` & `kiara_plugin.core_types-0.4.9/.cruft.json`

 * *Files identical despite different names*

### Comparing `kiara_plugin.core_types-0.4.8/.github/ISSUE_TEMPLATE/bug_report.md` & `kiara_plugin.core_types-0.4.9/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.core_types-0.4.8/.github/ISSUE_TEMPLATE/suggest-a-module.md` & `kiara_plugin.core_types-0.4.9/.github/ISSUE_TEMPLATE/suggest-a-module.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.core_types-0.4.8/.github/workflows/build-darwin.yaml` & `kiara_plugin.core_types-0.4.9/.github/workflows/build-darwin.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.core_types-0.4.8/.github/workflows/build-linux.yaml` & `kiara_plugin.core_types-0.4.9/.github/workflows/build-linux.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.core_types-0.4.8/.github/workflows/build-windows.yaml` & `kiara_plugin.core_types-0.4.9/.github/workflows/build-windows.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.core_types-0.4.8/.gitignore` & `kiara_plugin.core_types-0.4.9/.gitignore`

 * *Files identical despite different names*

### Comparing `kiara_plugin.core_types-0.4.8/.pre-commit-config.yaml` & `kiara_plugin.core_types-0.4.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.core_types-0.4.8/LICENSE` & `kiara_plugin.core_types-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kiara_plugin.core_types-0.4.8/Makefile` & `kiara_plugin.core_types-0.4.9/Makefile`

 * *Files identical despite different names*

### Comparing `kiara_plugin.core_types-0.4.8/PKG-INFO` & `kiara_plugin.core_types-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiara_plugin.core_types
-Version: 0.4.8
+Version: 0.4.9
 Summary: A set of modules (and pipelines) for Kiara.
 Home-page: https://github.com/DHARPA-Project/kiara_plugin.core_types
 Author: Markus Binsteiner
 Author-email: markus@frkl.io
 License: MPL-2.0
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `kiara_plugin.core_types-0.4.8/README.md` & `kiara_plugin.core_types-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.core_types-0.4.8/ci/conda/build-conda-packages.sh` & `kiara_plugin.core_types-0.4.9/ci/conda/build-conda-packages.sh`

 * *Files identical despite different names*

### Comparing `kiara_plugin.core_types-0.4.8/ci/conda/kiara_plugin.core_types/meta.yaml.template` & `kiara_plugin.core_types-0.4.9/ci/conda/kiara_plugin.core_types/meta.yaml.template`

 * *Files identical despite different names*

### Comparing `kiara_plugin.core_types-0.4.8/docs/index.md` & `kiara_plugin.core_types-0.4.9/docs/index.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.core_types-0.4.8/examples/data/journals/JournalEdges1902.csv` & `kiara_plugin.core_types-0.4.9/examples/data/journals/JournalEdges1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin.core_types-0.4.8/examples/data/journals/JournalNodes1902.csv` & `kiara_plugin.core_types-0.4.9/examples/data/journals/JournalNodes1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin.core_types-0.4.8/mkdocs.yml` & `kiara_plugin.core_types-0.4.9/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.core_types-0.4.8/scripts/documentation/gen_api_doc_pages.py` & `kiara_plugin.core_types-0.4.9/scripts/documentation/gen_api_doc_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.core_types-0.4.8/scripts/documentation/gen_info_pages.py` & `kiara_plugin.core_types-0.4.9/scripts/documentation/gen_info_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.core_types-0.4.8/scripts/documentation/gen_module_doc.py` & `kiara_plugin.core_types-0.4.9/scripts/documentation/gen_module_doc.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.core_types-0.4.8/setup.cfg` & `kiara_plugin.core_types-0.4.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `kiara_plugin.core_types-0.4.8/setup.py` & `kiara_plugin.core_types-0.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.core_types-0.4.8/src/kiara_plugin/core_types/__init__.py` & `kiara_plugin.core_types-0.4.9/src/kiara_plugin/core_types/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.core_types-0.4.8/src/kiara_plugin/core_types/data_types.py` & `kiara_plugin.core_types-0.4.9/src/kiara_plugin/core_types/data_types.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.core_types-0.4.8/src/kiara_plugin/core_types/models.py` & `kiara_plugin.core_types-0.4.9/src/kiara_plugin/core_types/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,14 +68,17 @@
         self._value_hash = compute_cid(obj)
         return self._value_hash
 
     def __getitem__(self, item):
 
         return self.list_data.__getitem__(item)
 
+    def __iter__(self):
+        return self.list_data.__iter__()
+
     def __len__(self):
         return self.list_data.__len__()
 
 
 class DictModel(BaseModel, Mapping):
     class Config:
         json_loads = orjson.loads
```

### Comparing `kiara_plugin.core_types-0.4.8/src/kiara_plugin/core_types/modules/boolean.py` & `kiara_plugin.core_types-0.4.9/src/kiara_plugin/core_types/modules/boolean.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.core_types-0.4.8/src/kiara_plugin/core_types/modules/date.py` & `kiara_plugin.core_types-0.4.9/src/kiara_plugin/core_types/modules/date.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.core_types-0.4.8/src/kiara_plugin/core_types/modules/list.py` & `kiara_plugin.core_types-0.4.9/src/kiara_plugin/core_types/modules/list.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.core_types-0.4.8/src/kiara_plugin/core_types/modules/string.py` & `kiara_plugin.core_types-0.4.9/src/kiara_plugin/core_types/modules/string.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.core_types-0.4.8/src/kiara_plugin/core_types/pipelines/logic/xor.json` & `kiara_plugin.core_types-0.4.9/src/kiara_plugin/core_types/pipelines/logic/xor.json`

 * *Files identical despite different names*

### Comparing `kiara_plugin.core_types-0.4.8/src/kiara_plugin.core_types.egg-info/PKG-INFO` & `kiara_plugin.core_types-0.4.9/src/kiara_plugin.core_types.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiara-plugin.core-types
-Version: 0.4.8
+Version: 0.4.9
 Summary: A set of modules (and pipelines) for Kiara.
 Home-page: https://github.com/DHARPA-Project/kiara_plugin.core_types
 Author: Markus Binsteiner
 Author-email: markus@frkl.io
 License: MPL-2.0
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `kiara_plugin.core_types-0.4.8/src/kiara_plugin.core_types.egg-info/SOURCES.txt` & `kiara_plugin.core_types-0.4.9/src/kiara_plugin.core_types.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin.core_types-0.4.8/src/kiara_plugin.core_types.egg-info/requires.txt` & `kiara_plugin.core_types-0.4.9/src/kiara_plugin.core_types.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,69 +1,69 @@
 kiara>=0.4.14
 
 [all]
 
 [all_dev]
-mknotebooks>=0.7.0
-pp-ez>=0.2.0
 pip-licenses>=3.3.0
-mkdocstrings-python-legacy
-types-pkg-resources
-types-python-dateutil
+setup-cfg-fmt>=1.16.0
+flake8>=3.8.4
+mike>=1.0.1
+mkdocs-literate-nav>=0.4.0
+pytest-cov>=2.11.1
 watchgod>=0.6
-ipython
-mypy>=0.800
 mkdocs-macros-plugin<0.6.0,>=0.5.0
-mkdocs-section-index>0.3.0
+pp-ez>=0.2.0
+mknotebooks>=0.7.0
+mkdocs-material>=8.0.0
+mkdocstrings-python-legacy
 mkdocs-awesome-pages-plugin>=2.5.0
-tox>=3.21.2
-mkdocs-literate-nav>=0.4.0
-coveralls>=3.2.0
-mike>=1.0.1
-pre-commit>=2.9.3
+wheel
 cruft>=2.6.0
 icecream>=2.1.0
-pytest-cov>=2.11.1
+ipython
+coveralls>=3.2.0
+mkdocs-section-index>0.3.0
+types-python-dateutil
+mypy>=0.800
+tox>=3.21.2
 black
+pre-commit>=2.9.3
 pytest>=6.2.2
-wheel
-setup-cfg-fmt>=1.16.0
-mkdocs-material>=8.0.0
-flake8>=3.8.4
+types-pkg-resources
 
 [all_dev:python_version >= "3.7"]
 mkdocs-gen-files>=0.3.1
 
 [dev_all]
-mknotebooks>=0.7.0
-pp-ez>=0.2.0
 pip-licenses>=3.3.0
-mkdocstrings-python-legacy
-types-pkg-resources
-types-python-dateutil
+setup-cfg-fmt>=1.16.0
+flake8>=3.8.4
+mike>=1.0.1
+mkdocs-literate-nav>=0.4.0
+pytest-cov>=2.11.1
 watchgod>=0.6
-ipython
-mypy>=0.800
 mkdocs-macros-plugin<0.6.0,>=0.5.0
-mkdocs-section-index>0.3.0
+pp-ez>=0.2.0
+mknotebooks>=0.7.0
+mkdocs-material>=8.0.0
+mkdocstrings-python-legacy
 mkdocs-awesome-pages-plugin>=2.5.0
-tox>=3.21.2
-mkdocs-literate-nav>=0.4.0
-coveralls>=3.2.0
-mike>=1.0.1
-pre-commit>=2.9.3
+wheel
 cruft>=2.6.0
 icecream>=2.1.0
-pytest-cov>=2.11.1
+ipython
+coveralls>=3.2.0
+mkdocs-section-index>0.3.0
+types-python-dateutil
+mypy>=0.800
+tox>=3.21.2
 black
+pre-commit>=2.9.3
 pytest>=6.2.2
-wheel
-setup-cfg-fmt>=1.16.0
-mkdocs-material>=8.0.0
-flake8>=3.8.4
+types-pkg-resources
 
 [dev_all:python_version >= "3.7"]
 mkdocs-gen-files>=0.3.1
 
 [dev_documentation]
 icecream>=2.1.0
 mike>=1.0.1
```

