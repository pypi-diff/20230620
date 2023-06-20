# Comparing `tmp/dls-bxflow-epsic-1.1.3.tar.gz` & `tmp/dls-bxflow-epsic-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dls-bxflow-epsic-1.1.3.tar", last modified: Tue May 30 04:46:05 2023, max compression
+gzip compressed data, was "dls-bxflow-epsic-1.2.0.tar", last modified: Tue Jun 20 11:14:40 2023, max compression
```

## Comparing `dls-bxflow-epsic-1.1.3.tar` & `dls-bxflow-epsic-1.2.0.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:46:05.810609 dls-bxflow-epsic-1.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:46:05.802609 dls-bxflow-epsic-1.1.3/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:46:05.802609 dls-bxflow-epsic-1.1.3/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.dae-devops/docs/documenting.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:46:05.802609 dls-bxflow-epsic-1.1.3/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:46:05.802609 dls-bxflow-epsic-1.1.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:46:05.798609 dls-bxflow-epsic-1.1.3/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:46:05.802609 dls-bxflow-epsic-1.1.3/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:46:05.802609 dls-bxflow-epsic-1.1.3/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:46:05.802609 dls-bxflow-epsic-1.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6925 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:46:05.802609 dls-bxflow-epsic-1.1.3/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7323 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/Makefile-conda
--rw-r--r--   0 runner    (1001) docker     (123)    13883 2023-05-30 04:46:05.806609 dls-bxflow-epsic-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:46:05.802609 dls-bxflow-epsic-1.1.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:46:05.798609 dls-bxflow-epsic-1.1.3/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:46:05.802609 dls-bxflow-epsic-1.1.3/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:46:05.802609 dls-bxflow-epsic-1.1.3/docs/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/docs/explanations/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/docs/explanations/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/docs/explanations/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/docs/explanations/todo.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:46:05.806609 dls-bxflow-epsic-1.1.3/docs/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/docs/how-to/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/docs/how-to/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/docs/how-to/documenting.rst
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/docs/how-to/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/docs/how-to/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/docs/how-to/testing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:46:05.806609 dls-bxflow-epsic-1.1.3/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:46:05.806609 dls-bxflow-epsic-1.1.3/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/docs/reference/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/docs/reference/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/docs/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/docs/reference/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:46:05.806609 dls-bxflow-epsic-1.1.3/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/docs/tutorials/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/docs/tutorials/tbd.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 04:46:05.810609 dls-bxflow-epsic-1.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:46:05.798609 dls-bxflow-epsic-1.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:46:05.806609 dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-30 04:46:05.000000 dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:46:05.806609 dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic/algorithms/mib_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:46:05.806609 dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic/collectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic/collectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic/collectors/mib_scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic/epsic_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic/epsic_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     9647 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:46:05.806609 dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13883 2023-05-30 04:46:05.000000 dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-30 04:46:05.000000 dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 04:46:05.000000 dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-30 04:46:05.000000 dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-30 04:46:05.000000 dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-30 04:46:05.000000 dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:46:05.806609 dls-bxflow-epsic-1.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/tests/base_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/tests/test_stub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:14:40.375035 dls-bxflow-epsic-1.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:14:40.367035 dls-bxflow-epsic-1.2.0/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:14:40.367035 dls-bxflow-epsic-1.2.0/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/.dae-devops/docs/documenting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:14:40.367035 dls-bxflow-epsic-1.2.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:14:40.367035 dls-bxflow-epsic-1.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:14:40.363035 dls-bxflow-epsic-1.2.0/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:14:40.367035 dls-bxflow-epsic-1.2.0/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:14:40.367035 dls-bxflow-epsic-1.2.0/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:14:40.367035 dls-bxflow-epsic-1.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6925 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:14:40.367035 dls-bxflow-epsic-1.2.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7323 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/Makefile-conda
+-rw-r--r--   0 runner    (1001) docker     (123)    13883 2023-06-20 11:14:40.375035 dls-bxflow-epsic-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:14:40.367035 dls-bxflow-epsic-1.2.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:14:40.363035 dls-bxflow-epsic-1.2.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:14:40.371035 dls-bxflow-epsic-1.2.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:14:40.371035 dls-bxflow-epsic-1.2.0/docs/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/docs/explanations/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/docs/explanations/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/docs/explanations/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/docs/explanations/todo.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:14:40.371035 dls-bxflow-epsic-1.2.0/docs/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/docs/how-to/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/docs/how-to/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/docs/how-to/documenting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/docs/how-to/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/docs/how-to/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/docs/how-to/testing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:14:40.371035 dls-bxflow-epsic-1.2.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:14:40.371035 dls-bxflow-epsic-1.2.0/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/docs/reference/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/docs/reference/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/docs/reference/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:14:40.371035 dls-bxflow-epsic-1.2.0/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/docs/tutorials/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/docs/tutorials/tbd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 11:14:40.375035 dls-bxflow-epsic-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:14:40.367035 dls-bxflow-epsic-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:14:40.371035 dls-bxflow-epsic-1.2.0/src/dls_bxflow_epsic/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/src/dls_bxflow_epsic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/src/dls_bxflow_epsic/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-20 11:14:40.000000 dls-bxflow-epsic-1.2.0/src/dls_bxflow_epsic/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:14:40.371035 dls-bxflow-epsic-1.2.0/src/dls_bxflow_epsic/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/src/dls_bxflow_epsic/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/src/dls_bxflow_epsic/algorithms/mib_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:14:40.371035 dls-bxflow-epsic-1.2.0/src/dls_bxflow_epsic/collectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/src/dls_bxflow_epsic/collectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/src/dls_bxflow_epsic/collectors/mib_scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/src/dls_bxflow_epsic/epsic_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/src/dls_bxflow_epsic/epsic_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9647 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/src/dls_bxflow_epsic/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/src/dls_bxflow_epsic/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:14:40.371035 dls-bxflow-epsic-1.2.0/src/dls_bxflow_epsic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13883 2023-06-20 11:14:40.000000 dls-bxflow-epsic-1.2.0/src/dls_bxflow_epsic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-20 11:14:40.000000 dls-bxflow-epsic-1.2.0/src/dls_bxflow_epsic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 11:14:40.000000 dls-bxflow-epsic-1.2.0/src/dls_bxflow_epsic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-20 11:14:40.000000 dls-bxflow-epsic-1.2.0/src/dls_bxflow_epsic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-20 11:14:40.000000 dls-bxflow-epsic-1.2.0/src/dls_bxflow_epsic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-20 11:14:40.000000 dls-bxflow-epsic-1.2.0/src/dls_bxflow_epsic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:14:40.375035 dls-bxflow-epsic-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/tests/base_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-20 11:14:32.000000 dls-bxflow-epsic-1.2.0/tests/test_stub.py
```

### Comparing `dls-bxflow-epsic-1.1.3/.dae-devops/Makefile` & `dls-bxflow-epsic-1.2.0/.dae-devops/Makefile`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.3/.dae-devops/docs/conventions.rst` & `dls-bxflow-epsic-1.2.0/.dae-devops/docs/conventions.rst`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.3/.dae-devops/docs/developing.rst` & `dls-bxflow-epsic-1.2.0/.dae-devops/docs/developing.rst`

 * *Files 12% similar despite different names*

```diff
@@ -10,22 +10,22 @@
 Clone the repository::
 
     $ cd <your development area>
     $ git clone https://github.com/DiamondLightSource/dls-bxflow-epsic.git
 
 It is recommended that you install into a virtual environment so this
 installation will not interfere with any existing Python software.
-Make sure to have at least python version >=3.10 then::
+Make sure to have at least python version 3.10 then::
 
     $ python3 -m venv /scratch/$USER/myvenv
     $ source /scratch/$USER/myvenv/bin/activate
     $ pip install --upgrade pip
 
 Install the package in edit mode which will also install all its dependencies::
 
     $ cd dls-bxflow-epsic
     $ pip install -e .[dev,docs]
 
 Now you may begin modifying the code.
 
 
-.. # dae_devops_fingerprint 541a732e9b67fb4322c7d4286330894f
+.. # dae_devops_fingerprint 29833ac3c02790256dee4294547276fc
```

### Comparing `dls-bxflow-epsic-1.1.3/.dae-devops/docs/devops.rst` & `dls-bxflow-epsic-1.2.0/.dae-devops/docs/devops.rst`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.3/.dae-devops/docs/docs_structure.rst` & `dls-bxflow-epsic-1.2.0/.dae-devops/docs/docs_structure.rst`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.3/.dae-devops/docs/documenting.rst` & `dls-bxflow-epsic-1.2.0/.dae-devops/docs/documenting.rst`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.3/.dae-devops/docs/installing.rst` & `dls-bxflow-epsic-1.2.0/.dae-devops/docs/installing.rst`

 * *Files 7% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 .. # ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 .. # ********** For repository_name dls-bxflow-epsic
 
 Installing
 =======================================================================
 
 
-You will need python >=3.10 or later. 
+You will need python 3.10 or later. 
 
-On a Diamond Light Source internal computer, you can achieve Python >=3.10 by::
+On a Diamond Light Source internal computer, you can achieve Python 3.10 by::
 
-    $ module load python/>=3.10
+    $ module load python/3.10
 
 You can check your version of python by typing into a terminal::
 
     $ python3 --version
 
 It is recommended that you install into a virtual environment so this
 installation will not interfere with any existing Python software::
@@ -35,8 +35,8 @@
 
 The package should now be installed and the command line should be available.
 You can check the version that has been installed by typing::
 
     $ dls-bxflow-epsic --version
     $ dls-bxflow-epsic --version-json
 
-.. # dae_devops_fingerprint 2536adcdc877e553821264097f0af330
+.. # dae_devops_fingerprint 8a36471be569817b021d617c3891644b
```

### Comparing `dls-bxflow-epsic-1.1.3/.dae-devops/docs/testing.rst` & `dls-bxflow-epsic-1.2.0/.dae-devops/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.3/.devcontainer/Dockerfile` & `dls-bxflow-epsic-1.2.0/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.3/.devcontainer/devcontainer.json` & `dls-bxflow-epsic-1.2.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.3/.github/CONTRIBUTING.rst` & `dls-bxflow-epsic-1.2.0/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.3/.github/actions/install_requirements/action.yml` & `dls-bxflow-epsic-1.2.0/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.3/.github/dependabot.yml` & `dls-bxflow-epsic-1.2.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.3/.github/pages/index.html` & `dls-bxflow-epsic-1.2.0/.github/pages/index.html`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.3/.github/pages/make_switcher.py` & `dls-bxflow-epsic-1.2.0/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.3/.github/workflows/code.yml` & `dls-bxflow-epsic-1.2.0/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.3/.github/workflows/docs.yml` & `dls-bxflow-epsic-1.2.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.3/.github/workflows/docs_clean.yml` & `dls-bxflow-epsic-1.2.0/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.3/.github/workflows/linkcheck.yml` & `dls-bxflow-epsic-1.2.0/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.3/.gitignore` & `dls-bxflow-epsic-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.3/.gitlab-ci.yml` & `dls-bxflow-epsic-1.2.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.3/.vscode/launch.json` & `dls-bxflow-epsic-1.2.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.3/LICENSE` & `dls-bxflow-epsic-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.3/Makefile` & `dls-bxflow-epsic-1.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.3/Makefile-conda` & `dls-bxflow-epsic-1.2.0/Makefile-conda`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.3/PKG-INFO` & `dls-bxflow-epsic-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dls-bxflow-epsic
-Version: 1.1.3
+Version: 1.2.0
 Summary: Bxflow beamline code for ePSIC.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `dls-bxflow-epsic-1.1.3/docs/conf.py` & `dls-bxflow-epsic-1.2.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,17 +184,17 @@
 
 # I got this from https://github.com/sphinx-doc/sphinx/issues/4054.
 # It will allow the ${token} replacement in the rst documents.
 ultimate_replacements = {
     "$" + "{repository_name}": "dls-bxflow-epsic",
     "$" + "{package_name}": "dls_bxflow_epsic",
     "$" + "{git_url}": "https://github.com/DiamondLightSource",
-    "$" + "{python_version_at_least}": ">=3.10",
+    "$" + "{python_version_at_least}": "3.10",
 }
 
 
 def setup(app):
     app.add_config_value("ultimate_replacements", {}, True)
     app.connect("source-read", ultimateReplace)
 
 
-# dae_devops_fingerprint 3f4594f6f175a8e6f58718c177489f82
+# dae_devops_fingerprint 8e603e29e8b9baa409c57595a0c5e916
```

### Comparing `dls-bxflow-epsic-1.1.3/docs/images/dls-favicon.ico` & `dls-bxflow-epsic-1.2.0/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.3/docs/images/dls-logo.svg` & `dls-bxflow-epsic-1.2.0/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.3/docs/reference/classes.rst` & `dls-bxflow-epsic-1.2.0/docs/reference/classes.rst`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.3/pyproject.toml` & `dls-bxflow-epsic-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic/__main__.py` & `dls-bxflow-epsic-1.2.0/src/dls_bxflow_epsic/__main__.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic/algorithms/mib_converter.py` & `dls-bxflow-epsic-1.2.0/src/dls_bxflow_epsic/algorithms/mib_converter.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic/collectors/mib_scraper.py` & `dls-bxflow-epsic-1.2.0/src/dls_bxflow_epsic/collectors/mib_scraper.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic/epsic_main.py` & `dls-bxflow-epsic-1.2.0/src/dls_bxflow_epsic/epsic_main.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic/epsic_workflow.py` & `dls-bxflow-epsic-1.2.0/src/dls_bxflow_epsic/epsic_workflow.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic/utilities.py` & `dls-bxflow-epsic-1.2.0/src/dls_bxflow_epsic/utilities.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic/version.py` & `dls-bxflow-epsic-1.2.0/src/dls_bxflow_epsic/version.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic.egg-info/PKG-INFO` & `dls-bxflow-epsic-1.2.0/src/dls_bxflow_epsic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dls-bxflow-epsic
-Version: 1.1.3
+Version: 1.2.0
 Summary: Bxflow beamline code for ePSIC.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic.egg-info/SOURCES.txt` & `dls-bxflow-epsic-1.2.0/src/dls_bxflow_epsic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.3/tests/base_tester.py` & `dls-bxflow-epsic-1.2.0/tests/base_tester.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.3/tests/conftest.py` & `dls-bxflow-epsic-1.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.3/tests/test_stub.py` & `dls-bxflow-epsic-1.2.0/tests/test_stub.py`

 * *Files identical despite different names*

